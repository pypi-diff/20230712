# Comparing `tmp/bluetooth_auto_recovery-1.2.0.tar.gz` & `tmp/bluetooth_auto_recovery-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetooth_auto_recovery-1.2.0.tar", max compression
+gzip compressed data, was "bluetooth_auto_recovery-1.2.1.tar", max compression
```

## Comparing `bluetooth_auto_recovery-1.2.0.tar` & `bluetooth_auto_recovery-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-05-10 13:17:23.980197 bluetooth_auto_recovery-1.2.0/LICENSE
--rw-r--r--   0        0        0     3840 2023-05-10 13:17:23.980197 bluetooth_auto_recovery-1.2.0/README.md
--rw-r--r--   0        0        0     2490 2023-05-10 13:17:24.884225 bluetooth_auto_recovery-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       91 2023-05-10 13:17:24.840223 bluetooth_auto_recovery-1.2.0/src/bluetooth_auto_recovery/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 13:17:23.980197 bluetooth_auto_recovery-1.2.0/src/bluetooth_auto_recovery/py.typed
--rw-r--r--   0        0        0    22347 2023-05-10 13:17:23.980197 bluetooth_auto_recovery-1.2.0/src/bluetooth_auto_recovery/recover.py
--rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 bluetooth_auto_recovery-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-12 00:44:03.779008 bluetooth_auto_recovery-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3840 2023-07-12 00:44:03.779008 bluetooth_auto_recovery-1.2.1/README.md
+-rw-r--r--   0        0        0     2522 2023-07-12 00:44:04.683021 bluetooth_auto_recovery-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-07-12 00:44:04.647021 bluetooth_auto_recovery-1.2.1/src/bluetooth_auto_recovery/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 00:44:03.779008 bluetooth_auto_recovery-1.2.1/src/bluetooth_auto_recovery/py.typed
+-rw-r--r--   0        0        0    23534 2023-07-12 00:44:03.779008 bluetooth_auto_recovery-1.2.1/src/bluetooth_auto_recovery/recover.py
+-rw-r--r--   0        0        0     5411 1970-01-01 00:00:00.000000 bluetooth_auto_recovery-1.2.1/PKG-INFO
```

### Comparing `bluetooth_auto_recovery-1.2.0/LICENSE` & `bluetooth_auto_recovery-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetooth_auto_recovery-1.2.0/README.md` & `bluetooth_auto_recovery-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bluetooth_auto_recovery-1.2.0/pyproject.toml` & `bluetooth_auto_recovery-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluetooth-auto-recovery"
-version = "1.2.0"
+version = "1.2.1"
 description = "Recover bluetooth adapters that are in an stuck state"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/bluetooth-auto-recovery"
 documentation = "https://bluetooth-auto-recovery.readthedocs.io"
 classifiers = [
@@ -29,14 +29,15 @@
 Sphinx = {version = "^5.0", optional = true}
 sphinx-rtd-theme = {version = "^1.0", optional = true}
 myst-parser = {version = "^0.18", optional = true}
 PyRIC = ">=0.1.6.3"
 btsocket = ">=0.2.0"
 async-timeout = ">=4.0.1"
 usb-devices = ">=0.4.1"
+bluetooth-adapters = ">=0.16.0"
 
 [tool.poetry.extras]
 docs = [
     "myst-parser",
     "sphinx",
     "sphinx-rtd-theme",
 ]
```

### Comparing `bluetooth_auto_recovery-1.2.0/src/bluetooth_auto_recovery/recover.py` & `bluetooth_auto_recovery-1.2.1/src/bluetooth_auto_recovery/recover.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from dataclasses import dataclass
 from fcntl import ioctl
 from typing import Any, AsyncIterator, cast
 
 import async_timeout
 import pyric.net.wireless.rfkill_h as rfkh
 import pyric.utils.rfkill as rfkill
+from bluetooth_adapters import get_adapters_from_hci
 from btsocket import btmgmt_protocol, btmgmt_socket
 from btsocket.btmgmt_socket import AF_BLUETOOTH, BTPROTO_HCI
 from usb_devices import BluetoothDevice, NotAUSBDeviceError
 
 _LOGGER = logging.getLogger(__name__)
 
 POWER_OFF_TIME = 2
@@ -198,14 +199,39 @@
         assert isinstance(protocol, BluetoothMGMTProtocol)  # nosec
         self.protocol = protocol
         await self._find_controller()
 
     async def _find_controller(self) -> None:
         """Find the controller."""
         assert self.protocol is not None  # nosec
+        loop = asyncio.get_running_loop()
+        # Try to get the adapter index from the hci device first
+        # since it can see downed adapters.
+        if adapters_from_hci := await loop.run_in_executor(None, get_adapters_from_hci):
+            _LOGGER.debug("Found adapters from hci: %s", adapters_from_hci)
+            for adapter in adapters_from_hci.values():
+                if adapter["bdaddr"] == self.mac.upper():
+                    self.idx = adapter["dev_id"]
+                    _LOGGER.debug(
+                        "Found adapter %s in hci device as %s", self.mac, self.idx
+                    )
+                    return
+
+            for adapter in adapters_from_hci.values():
+                expected_hci_name = f"hci{self._expected_hci}"
+                if adapter["name"] == expected_hci_name:
+                    self.idx = adapter["dev_id"]
+                    _LOGGER.debug(
+                        "Found adapter %s as hci device %s as %s",
+                        self.mac,
+                        self._expected_hci,
+                        self.idx,
+                    )
+                    return
+
         idxdata = await self.protocol.send("ReadControllerIndexList", None)
         if idxdata.event_frame.status.value != 0x00:  # 0x00 - Success
             _LOGGER.error(
                 "Unable to get hci controllers index list! Event frame status: %s",
                 idxdata.event_frame.status,
             )
             return
```

### Comparing `bluetooth_auto_recovery-1.2.0/PKG-INFO` & `bluetooth_auto_recovery-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluetooth-auto-recovery
-Version: 1.2.0
+Version: 1.2.1
 Summary: Recover bluetooth adapters that are in an stuck state
 Home-page: https://github.com/bluetooth-devices/bluetooth-auto-recovery
 License: MIT
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Requires-Dist: PyRIC (>=0.1.6.3)
 Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs"
 Requires-Dist: async-timeout (>=4.0.1)
+Requires-Dist: bluetooth-adapters (>=0.16.0)
 Requires-Dist: btsocket (>=0.2.0)
 Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs"
 Requires-Dist: usb-devices (>=0.4.1)
 Project-URL: Bug Tracker, https://github.com/bluetooth-devices/bluetooth-auto-recovery/issues
 Project-URL: Changelog, https://github.com/bluetooth-devices/bluetooth-auto-recovery/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://bluetooth-auto-recovery.readthedocs.io
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: bluetooth-auto-recovery Version: 1.2.0 Summary:
+Metadata-Version: 2.1 Name: bluetooth-auto-recovery Version: 1.2.1 Summary:
 Recover bluetooth adapters that are in an stuck state Home-page: https://
 github.com/bluetooth-devices/bluetooth-auto-recovery License: MIT Author: J.
 Nick Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Software Development :: Libraries Provides-Extra: docs Requires-Dist: PyRIC
 (>=0.1.6.3) Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs" Requires-Dist:
-async-timeout (>=4.0.1) Requires-Dist: btsocket (>=0.2.0) Requires-Dist: myst-
-parser (>=0.18,<0.19) ; extra == "docs" Requires-Dist: sphinx-rtd-theme
-(>=1.0,<2.0) ; extra == "docs" Requires-Dist: usb-devices (>=0.4.1) Project-
-URL: Bug Tracker, https://github.com/bluetooth-devices/bluetooth-auto-recovery/
-issues Project-URL: Changelog, https://github.com/bluetooth-devices/bluetooth-
-auto-recovery/blob/main/CHANGELOG.md Project-URL: Documentation, https://
-bluetooth-auto-recovery.readthedocs.io Project-URL: Repository, https://
-github.com/bluetooth-devices/bluetooth-auto-recovery Description-Content-Type:
-text/markdown # Bluetooth Auto Recovery
+async-timeout (>=4.0.1) Requires-Dist: bluetooth-adapters (>=0.16.0) Requires-
+Dist: btsocket (>=0.2.0) Requires-Dist: myst-parser (>=0.18,<0.19) ; extra ==
+"docs" Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs" Requires-
+Dist: usb-devices (>=0.4.1) Project-URL: Bug Tracker, https://github.com/
+bluetooth-devices/bluetooth-auto-recovery/issues Project-URL: Changelog, https:
+//github.com/bluetooth-devices/bluetooth-auto-recovery/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://bluetooth-auto-recovery.readthedocs.io
+Project-URL: Repository, https://github.com/bluetooth-devices/bluetooth-auto-
+recovery Description-Content-Type: text/markdown # Bluetooth Auto Recovery
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 Recover bluetooth adapters that are in an stuck state ## Credits The code in
 this repo originates from https://github.com/custom-components/ble_monitor/
 blob/master/custom_components/ble_monitor/bt_helpers.py ## Installation Install
 this via pip (or your favourite package manager): `pip install bluetooth-auto-
```


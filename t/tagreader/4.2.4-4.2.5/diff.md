# Comparing `tmp/tagreader-4.2.4.tar.gz` & `tmp/tagreader-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagreader-4.2.4.tar", max compression
+gzip compressed data, was "tagreader-4.2.5.tar", max compression
```

## Comparing `tagreader-4.2.4.tar` & `tagreader-4.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-06-06 13:10:02.326221 tagreader-4.2.4/LICENSE
--rw-r--r--   0        0        0     2561 2023-06-15 12:41:41.851734 tagreader-4.2.4/README.md
--rw-r--r--   0        0        0     1633 2023-07-12 12:06:22.847778 tagreader-4.2.4/pyproject.toml
--rw-r--r--   0        0        0      409 2023-07-12 09:12:52.054768 tagreader-4.2.4/tagreader/__init__.py
--rw-r--r--   0        0        0      282 2023-06-09 06:24:33.101915 tagreader-4.2.4/tagreader/__version__.py
--rw-r--r--   0        0        0    11699 2023-07-12 11:59:21.151799 tagreader-4.2.4/tagreader/cache.py
--rw-r--r--   0        0        0    22878 2023-07-12 12:01:14.138324 tagreader-4.2.4/tagreader/clients.py
--rw-r--r--   0        0        0      198 2023-06-09 06:24:33.104271 tagreader-4.2.4/tagreader/logger.py
--rw-r--r--   0        0        0    24973 2023-07-07 07:04:09.640569 tagreader-4.2.4/tagreader/odbc_handlers.py
--rw-r--r--   0        0        0     8193 2023-07-07 07:04:09.641056 tagreader-4.2.4/tagreader/utils.py
--rw-r--r--   0        0        0    32781 2023-07-07 07:04:09.641475 tagreader-4.2.4/tagreader/web_handlers.py
--rw-r--r--   0        0        0     4404 1970-01-01 00:00:00.000000 tagreader-4.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-07-12 13:01:47.766928 tagreader-4.2.5/LICENSE
+-rw-r--r--   0        0        0     1684 2023-07-12 13:01:47.766928 tagreader-4.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2640 2023-07-12 13:01:47.766928 tagreader-4.2.5/README.md
+-rw-r--r--   0        0        0      415 2023-07-12 13:01:47.766928 tagreader-4.2.5/tagreader/__init__.py
+-rw-r--r--   0        0        0      289 2023-07-12 13:01:47.782552 tagreader-4.2.5/tagreader/__version__.py
+-rw-r--r--   0        0        0    12065 2023-07-12 13:01:47.782552 tagreader-4.2.5/tagreader/cache.py
+-rw-r--r--   0        0        0    23509 2023-07-12 13:01:47.782552 tagreader-4.2.5/tagreader/clients.py
+-rw-r--r--   0        0        0      208 2023-07-12 13:01:47.782552 tagreader-4.2.5/tagreader/logger.py
+-rw-r--r--   0        0        0    25633 2023-07-12 13:01:47.782552 tagreader-4.2.5/tagreader/odbc_handlers.py
+-rw-r--r--   0        0        0     8381 2023-07-12 13:01:47.782552 tagreader-4.2.5/tagreader/utils.py
+-rw-r--r--   0        0        0    33857 2023-07-12 13:01:47.782552 tagreader-4.2.5/tagreader/web_handlers.py
+-rw-r--r--   0        0        0     4202 1970-01-01 00:00:00.000000 tagreader-4.2.5/PKG-INFO
```

### Comparing `tagreader-4.2.4/README.md` & `tagreader-4.2.5/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-# tagreader-python <!-- omit in toc -->
-
-![GitHub Build Status](https://github.com/equinor/tagreader-python/workflows/Test/badge.svg)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tagreader)
-![PyPI](https://img.shields.io/pypi/v/tagreader)
-[![Downloads](https://pepy.tech/badge/tagreader)](https://pepy.tech/project/tagreader)
-
-Tagreader is a Python package for reading trend data from the OSIsoft
-PI and Aspen Infoplus.21 IMS systems. It is intended to be easy to use,
-and present as similar interfaces as possible to the backend historians.
-
-While originally developed for Windows, Tagreader can since release 3.0.0
-also be used on Linux and Windows platforms.
-
-Queries can be performed using either REST API (preferred) or ODBC queries.
-The use of ODBC queries require installation of proprietary drivers from
-AspenTech and OSIsoft that are only available for Windows.
-
-Trend data is output as Pandas Dataframes. The HDF5 file format is used
-to cache results.
-
-## Requirements
-
-Python >=3.8 with the following packages:
-
-  + pandas >= 1.0.0
-  + requests
-  + requests-kerberos
-  + certifi >= 2023.5.7
-  + diskcache
-  + pyodbc (**)
-
-**) If using ODBC connections, you must also install proprietary drivers for
-PI ODBC and/or Aspen IP.21 SQLPlus. These drivers are only available for
-Microsoft Windows. Pyodbc will therefore not be installed for non-Windows
-systems.
-
-## Installation
-
-To install and/or upgrade:
-
-```
-pip install --upgrade tagreader
-```
-
-If you wish to use ODBC connections to the IMS servers, you will also need
-to install some proprietary drivers. There is more information in the
-[manual](docs/manual.md#odbc-drivers). Please note that the web APIs should
-normally be preferred.
-
-## Usage example
-
-```
-import tagreader
-c = tagreader.IMSClient("mysource", "aspenone")
-print(c.search("tag*"))
-df = c.read_tags(["tag1", "tag2"], "18.06.2020 08:00:00", "18.06.2020 09:00:00", 60)
-```
-
-## Jupyter Notebook Quickstart
-Jupyter Notebook examples can be found in /examples. In order to run these examples, you need to install the optional
-dependencies.
-
-```bash
-pip install tagreader[notebooks]
-```
-
-
-## Documentation
-
-There is a [quickstart](examples/quickstart.ipynb) example file that should get
-you going. Also check out the [manual](docs/manual.md) for more information.
-
-## Contributing
-
-All contributions are welcome, including code, bug reports, issues, feature
-requests, and documentation. The preferred way of submitting a contribution
-is to either create an issue on GitHub or to fork the project and make a pull
-request.
+# tagreader-python <!-- omit in toc -->
+
+![GitHub Build Status](https://github.com/equinor/tagreader-python/workflows/Test/badge.svg)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tagreader)
+![PyPI](https://img.shields.io/pypi/v/tagreader)
+[![Downloads](https://pepy.tech/badge/tagreader)](https://pepy.tech/project/tagreader)
+
+Tagreader is a Python package for reading trend data from the OSIsoft
+PI and Aspen Infoplus.21 IMS systems. It is intended to be easy to use,
+and present as similar interfaces as possible to the backend historians.
+
+While originally developed for Windows, Tagreader can since release 3.0.0
+also be used on Linux and Windows platforms.
+
+Queries can be performed using either REST API (preferred) or ODBC queries.
+The use of ODBC queries require installation of proprietary drivers from
+AspenTech and OSIsoft that are only available for Windows.
+
+Trend data is output as Pandas Dataframes. The HDF5 file format is used
+to cache results.
+
+## Requirements
+
+Python >=3.8 with the following packages:
+
+  + pandas >= 1.0.0
+  + requests
+  + requests-kerberos
+  + certifi >= 2023.5.7
+  + diskcache
+  + pyodbc (**)
+
+**) If using ODBC connections, you must also install proprietary drivers for
+PI ODBC and/or Aspen IP.21 SQLPlus. These drivers are only available for
+Microsoft Windows. Pyodbc will therefore not be installed for non-Windows
+systems.
+
+## Installation
+
+To install and/or upgrade:
+
+```
+pip install --upgrade tagreader
+```
+
+If you wish to use ODBC connections to the IMS servers, you will also need
+to install some proprietary drivers. There is more information in the
+[manual](docs/manual.md#odbc-drivers). Please note that the web APIs should
+normally be preferred.
+
+## Usage example
+
+```
+import tagreader
+c = tagreader.IMSClient("mysource", "aspenone")
+print(c.search("tag*"))
+df = c.read_tags(["tag1", "tag2"], "18.06.2020 08:00:00", "18.06.2020 09:00:00", 60)
+```
+
+## Jupyter Notebook Quickstart
+Jupyter Notebook examples can be found in /examples. In order to run these examples, you need to install the optional
+dependencies.
+
+```bash
+pip install tagreader[notebooks]
+```
+
+
+## Documentation
+
+There is a [quickstart](examples/quickstart.ipynb) example file that should get
+you going. Also check out the [manual](docs/manual.md) for more information.
+
+## Contributing
+
+All contributions are welcome, including code, bug reports, issues, feature
+requests, and documentation. The preferred way of submitting a contribution
+is to either create an issue on GitHub or to fork the project and make a pull
+request.
```

### Comparing `tagreader-4.2.4/pyproject.toml` & `tagreader-4.2.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-[tool.poetry]
-name = "tagreader"
-version = "4.2.4"
-description = "Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems."
-authors = ["Einar S. Idsø <eiids@equinor.com>"]
-license = "MIT"
-readme = "README.md"
-packages = [{include = "tagreader"}]
-keywords=["Aspen InfoPlus.21", "OSIsoft PI"]
-homepage = "https://github.com/equinor/tagreader-python"
-repository = "https://github.com/equinor/tagreader-python"
-classifiers=[
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: MIT License",
-    "Natural Language :: English",
-    "Operating System :: MacOS",
-    "Operating System :: Microsoft :: Windows",
-    "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Topic :: Utilities",
-]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-pandas = ">=1"
-pyodbc = "^4"
-certifi = "^2023"
-requests = "^2"
-requests-kerberos = "^0"
-jupyter = { version = "^1", optional = true }
-matplotlib = { version = "^3", optional = true }
-diskcache = "^5.6.1"
-
-
-[tool.poetry.group.dev.dependencies]
-pre-commit = "^3"
-pytest = "^7"
-
-[tool.poetry.extras]
-notebooks = ["jupyter", "matplotlib"]
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "tagreader"
+version = "4.2.5"
+description = "Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems."
+authors = ["Einar S. Idsø <eiids@equinor.com>"]
+license = "MIT"
+readme = "README.md"
+packages = [{include = "tagreader"}]
+keywords=["Aspen InfoPlus.21", "OSIsoft PI"]
+homepage = "https://github.com/equinor/tagreader-python"
+repository = "https://github.com/equinor/tagreader-python"
+classifiers=[
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
+    "Operating System :: MacOS",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: POSIX :: Linux",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Utilities",
+]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+pandas = ">=1"
+pyodbc = "^4"
+certifi = "^2023"
+requests = "^2"
+requests-kerberos = "^0"
+jupyter = { version = "^1", optional = true }
+matplotlib = { version = "^3", optional = true }
+diskcache = "^5.6.1"
+
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^3"
+pytest = "^7"
+
+[tool.poetry.extras]
+notebooks = ["jupyter", "matplotlib"]
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `tagreader-4.2.4/tagreader/utils.py` & `tagreader-4.2.5/tagreader/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,266 +1,264 @@
-import enum
-import logging
-import platform
-import warnings
-from datetime import datetime
-from enum import Enum
-from typing import Union
-
-import pandas as pd
-import pytz
-
-
-def is_windows() -> bool:
-    return platform.system() == "Windows"
-
-
-def is_mac() -> bool:
-    return platform.system() == "Darwin"
-
-
-def is_linux() -> bool:
-    return platform.system() == "Linux"
-
-
-if is_windows():
-    import winreg
-
-
-if is_mac():
-    import socket
-    import subprocess
-
-
-def find_registry_key(base_key, search_key_name: str):
-    search_key_name = search_key_name.lower()
-    if base_key is not None:
-        num_keys, _, _ = winreg.QueryInfoKey(base_key)
-        for i in range(0, num_keys):
-            key_name = winreg.EnumKey(base_key, i)
-            if key_name.lower() == search_key_name:
-                return winreg.OpenKey(base_key, key_name)
-            else:
-                key = find_registry_key(
-                    winreg.OpenKey(base_key, key_name), search_key_name
-                )
-            if key is not None:
-                return key
-    return None
-
-
-def find_registry_key_from_name(base_key, search_key_name: str):
-    search_key_name = search_key_name.lower()
-    num_keys, _, _ = winreg.QueryInfoKey(base_key)
-    key = key_string = None
-    for i in range(0, num_keys):
-        try:
-            key_string = winreg.EnumKey(base_key, i)
-            key = winreg.OpenKey(base_key, key_string)
-            _, num_vals, _ = winreg.QueryInfoKey(key)
-            if num_vals > 0:
-                (_, key_name, _) = winreg.EnumValue(key, 0)
-                if str(key_name).lower() == search_key_name:
-                    break
-        except Exception as err:
-            logging.error("{}: {}".format(i, err))
-    return key, key_string
-
-
-def convert_to_pydatetime(date_stamp: Union[datetime, str, pd.Timestamp]) -> datetime:
-    if isinstance(date_stamp, datetime):
-        return date_stamp
-    elif isinstance(date_stamp, pd.Timestamp):
-        return date_stamp.to_pydatetime()
-    else:
-        try:
-            return pd.to_datetime(str(date_stamp), format="ISO8601").to_pydatetime()
-        except ValueError:
-            return pd.to_datetime(str(date_stamp), dayfirst=True).to_pydatetime()
-
-
-def ensure_datetime_with_tz(
-    date_stamp: Union[datetime, str, pd.Timestamp],
-    tz: pytz.timezone = pytz.timezone("Europe/Oslo"),
-) -> datetime:
-    date_stamp = convert_to_pydatetime(date_stamp)
-
-    if not date_stamp.tzinfo:
-        date_stamp = tz.localize(date_stamp)
-
-    return date_stamp
-
-
-def urljoin(*args) -> str:
-    """
-    Joins components of URL. Ensures slashes are inserted or removed where
-    needed, and does not strip trailing slash of last element.
-
-    Returns:
-        str -- Generated URL
-    """
-    trailing_slash = "/" if args[-1].endswith("/") else ""
-    return "/".join(map(lambda x: str(x).strip("/"), args)) + trailing_slash
-
-
-class ReaderType(enum.IntEnum):
-    """Enumerates available types of data to read.
-
-    For members with more than one name per value, the first member (the
-    original) needs to be untouched since it may be used as back-reference
-    (specifically for cache hierarchies).
-    """
-
-    RAW = SAMPLED = ACTUAL = enum.auto()  # Raw sampled data
-    SHAPEPRESERVING = BESTFIT = enum.auto()  # Minimum data points for preserving shape
-    INT = INTERPOLATE = INTERPOLATED = enum.auto()  # Interpolated data
-    MIN = MINIMUM = enum.auto()  # Min value
-    MAX = MAXIMUM = enum.auto()  # Max value
-    AVG = AVERAGE = AVERAGED = enum.auto()  # Averaged data
-    VAR = VARIANCE = enum.auto()  # Variance of data
-    STD = STDDEV = enum.auto()  # Standard deviation of data
-    RNG = RANGE = enum.auto()  # Range of data
-    COUNT = enum.auto()  # Number of data points
-    GOOD = enum.auto()  # Number of good data points
-    BAD = NOTGOOD = enum.auto()  # Number of not good data points
-    TOTAL = enum.auto()  # Number of total data
-    SUM = enum.auto()  # Sum of data
-    SNAPSHOT = FINAL = LAST = enum.auto()  # Last sampled value
-
-
-def add_statoil_root_certificate(noisy: bool = True) -> bool:
-    """This is a utility function for Equinor employees on Equinor managed machines.
-
-    The function searches for the Statoil Root certificate in the
-    cert store and imports it to the cacert bundle. Does nothing if not
-    running on Equinor host.
-
-    This needs to be repeated after updating the cacert module.
-
-    Returns:
-        bool: True if function completes successfully
-    """
-    import hashlib
-    import ssl
-
-    import certifi
-
-    STATOIL_ROOT_PEM_HASH = "ce7bb185ab908d2fea28c7d097841d9d5bbf2c76"
-
-    found = False
-    der = None
-
-    if is_linux():
-        return True
-    elif is_windows():
-        if noisy:
-            print("Scanning CA certs in Windows cert store", end="")
-        for cert in ssl.enum_certificates("CA"):
-            if noisy:
-                print(".", end="")
-            der = cert[0]
-            if hashlib.sha1(der).hexdigest() == STATOIL_ROOT_PEM_HASH:
-                found = True
-                if noisy:
-                    print(" found it!")
-                break
-    elif is_mac():
-        import subprocess
-
-        macos_ca_certs = subprocess.run(
-            ["security", "find-certificate", "-a", "-c", "Statoil Root CA", "-Z"],
-            stdout=subprocess.PIPE,
-        ).stdout
-
-        if STATOIL_ROOT_PEM_HASH.upper() in str(macos_ca_certs).upper():
-            c = get_macos_statoil_certificates()
-            for cert in c:
-                if hashlib.sha1(cert).hexdigest() == STATOIL_ROOT_PEM_HASH:
-                    der = cert
-                    found = True
-                    break
-
-    if found and der:
-        pem = ssl.DER_cert_to_PEM_cert(der)
-        if pem in certifi.contents():
-            if noisy:
-                print("Certificate already exists in certifi store. Nothing to do.")
-        else:
-            if noisy:
-                print("Writing certificate to certifi store.")
-            cafile = certifi.where()
-            with open(cafile, "ab") as f:
-                f.write(bytes(pem, "ascii"))
-            if noisy:
-                print("Completed")
-    else:
-        warnings.warn("Unable to locate root certificate on this host.")
-
-    return found
-
-
-def get_macos_statoil_certificates():
-    import ssl
-    import tempfile
-
-    ctx = ssl.create_default_context()
-    macos_ca_certs = subprocess.run(
-        ["security", "find-certificate", "-a", "-c", "Statoil Root CA", "-p"],
-        stdout=subprocess.PIPE,
-    ).stdout
-    with tempfile.NamedTemporaryFile("w+b") as tmp_file:
-        tmp_file.write(macos_ca_certs)
-        ctx.load_verify_locations(tmp_file.name)
-
-    return ctx.get_ca_certs(binary_form=True)
-
-
-def is_equinor() -> bool:
-    """Determines whether code is running on an Equinor host
-
-    If Windows host:
-    Finds host's domain in Windows Registry at
-    HKLM\\SYSTEM\\ControlSet001\\Services\\Tcpip\\Parameters\\Domain
-    If mac os host:
-    Finds statoil.net as AD hostname in certificates
-    If Linux host:
-    Checks whether statoil.no is search domain
-
-    Returns:
-        bool: True if Equinor
-    """
-    if is_windows():
-        with winreg.OpenKey(
-            winreg.HKEY_LOCAL_MACHINE, r"SYSTEM\ControlSet001\Services\Tcpip\Parameters"
-        ) as key:
-            domain = winreg.QueryValueEx(key, "Domain")
-        if "statoil" in domain[0]:
-            return True
-    elif is_mac():
-        s = subprocess.run(
-            ["security", "find-certificate", "-a", "-c" "client.statoil.net"],
-            stdout=subprocess.PIPE,
-        ).stdout
-
-        host = socket.gethostname()
-
-        if host + ".client.statoil.net" in str(s):
-            return True
-        elif "client.statoil.net" in host and host in str(s):
-            return True
-    elif is_linux():
-        with open("/etc/resolv.conf", "r") as f:
-            if "statoil.no" in f.read():
-                return True
-    else:
-        raise OSError(
-            f"Unsupported system: {platform.system()}. Please report this as an issue."
-        )
-    return False
-
-
-class IMSType(str, Enum):
-    PIWEBAPI = "piwebapi"
-    ASPENONE = "aspenone"
-    PI = "pi"
-    ASPEN = "aspen"
-    IP21 = "ip21"
+import enum
+import logging
+import platform
+import warnings
+from datetime import datetime
+from enum import Enum
+from typing import Union
+
+import pandas as pd
+import pytz
+
+from tagreader.logger import logger
+
+
+def is_windows() -> bool:
+    return platform.system() == "Windows"
+
+
+def is_mac() -> bool:
+    return platform.system() == "Darwin"
+
+
+def is_linux() -> bool:
+    return platform.system() == "Linux"
+
+
+if is_windows():
+    import winreg
+
+
+if is_mac():
+    import socket
+    import subprocess
+
+
+def find_registry_key(base_key, search_key_name: str):
+    search_key_name = search_key_name.lower()
+    if base_key is not None:
+        num_keys, _, _ = winreg.QueryInfoKey(base_key)
+        for i in range(0, num_keys):
+            key_name = winreg.EnumKey(base_key, i)
+            if key_name.lower() == search_key_name:
+                return winreg.OpenKey(base_key, key_name)
+            else:
+                key = find_registry_key(
+                    winreg.OpenKey(base_key, key_name), search_key_name
+                )
+            if key is not None:
+                return key
+    return None
+
+
+def find_registry_key_from_name(base_key, search_key_name: str):
+    search_key_name = search_key_name.lower()
+    num_keys, _, _ = winreg.QueryInfoKey(base_key)
+    key = key_string = None
+    for i in range(0, num_keys):
+        try:
+            key_string = winreg.EnumKey(base_key, i)
+            key = winreg.OpenKey(base_key, key_string)
+            _, num_vals, _ = winreg.QueryInfoKey(key)
+            if num_vals > 0:
+                (_, key_name, _) = winreg.EnumValue(key, 0)
+                if str(key_name).lower() == search_key_name:
+                    break
+        except Exception as err:
+            logging.error("{}: {}".format(i, err))
+    return key, key_string
+
+
+def convert_to_pydatetime(date_stamp: Union[datetime, str, pd.Timestamp]) -> datetime:
+    if isinstance(date_stamp, datetime):
+        return date_stamp
+    elif isinstance(date_stamp, pd.Timestamp):
+        return date_stamp.to_pydatetime()
+    else:
+        try:
+            return pd.to_datetime(str(date_stamp), format="ISO8601").to_pydatetime()
+        except ValueError:
+            return pd.to_datetime(str(date_stamp), dayfirst=True).to_pydatetime()
+
+
+def ensure_datetime_with_tz(
+    date_stamp: Union[datetime, str, pd.Timestamp],
+    tz: pytz.timezone = pytz.timezone("Europe/Oslo"),
+) -> datetime:
+    date_stamp = convert_to_pydatetime(date_stamp)
+
+    if not date_stamp.tzinfo:
+        date_stamp = tz.localize(date_stamp)
+
+    return date_stamp
+
+
+def urljoin(*args) -> str:
+    """
+    Joins components of URL. Ensures slashes are inserted or removed where
+    needed, and does not strip trailing slash of last element.
+
+    Returns:
+        str -- Generated URL
+    """
+    trailing_slash = "/" if args[-1].endswith("/") else ""
+    return "/".join(map(lambda x: str(x).strip("/"), args)) + trailing_slash
+
+
+class ReaderType(enum.IntEnum):
+    """Enumerates available types of data to read.
+
+    For members with more than one name per value, the first member (the
+    original) needs to be untouched since it may be used as back-reference
+    (specifically for cache hierarchies).
+    """
+
+    RAW = SAMPLED = ACTUAL = enum.auto()  # Raw sampled data
+    SHAPEPRESERVING = BESTFIT = enum.auto()  # Minimum data points for preserving shape
+    INT = INTERPOLATE = INTERPOLATED = enum.auto()  # Interpolated data
+    MIN = MINIMUM = enum.auto()  # Min value
+    MAX = MAXIMUM = enum.auto()  # Max value
+    AVG = AVERAGE = AVERAGED = enum.auto()  # Averaged data
+    VAR = VARIANCE = enum.auto()  # Variance of data
+    STD = STDDEV = enum.auto()  # Standard deviation of data
+    RNG = RANGE = enum.auto()  # Range of data
+    COUNT = enum.auto()  # Number of data points
+    GOOD = enum.auto()  # Number of good data points
+    BAD = NOTGOOD = enum.auto()  # Number of not good data points
+    TOTAL = enum.auto()  # Number of total data
+    SUM = enum.auto()  # Sum of data
+    SNAPSHOT = FINAL = LAST = enum.auto()  # Last sampled value
+
+
+def add_statoil_root_certificate() -> bool:
+    """
+    This is a utility function for Equinor employees on Equinor managed machines.
+
+    The function searches for the Equinor Root certificate in the
+    cert store and imports it to the cacert bundle. Does nothing if not
+    running on Equinor host.
+
+    This needs to be repeated after updating the cacert module.
+
+    Returns:
+        bool: True if function completes successfully
+    """
+    import hashlib
+    import ssl
+
+    import certifi
+
+    STATOIL_ROOT_PEM_HASH = "ce7bb185ab908d2fea28c7d097841d9d5bbf2c76"
+
+    found = False
+    der = None
+
+    if is_linux():
+        return True
+    elif is_windows():
+        logger.debug("Scanning CA certificate in Windows cert store", end="")
+        for cert in ssl.enum_certificates("CA"):
+            der = cert[0]
+            if hashlib.sha1(der).hexdigest() == STATOIL_ROOT_PEM_HASH:
+                found = True
+                logger.debug("CA certificate found!")
+                break
+    elif is_mac():
+        import subprocess
+
+        macos_ca_certs = subprocess.run(
+            ["security", "find-certificate", "-a", "-c", "Statoil Root CA", "-Z"],
+            stdout=subprocess.PIPE,
+        ).stdout
+
+        if STATOIL_ROOT_PEM_HASH.upper() in str(macos_ca_certs).upper():
+            c = get_macos_equinor_certificates()
+            for cert in c:
+                if hashlib.sha1(cert).hexdigest() == STATOIL_ROOT_PEM_HASH:
+                    der = cert
+                    found = True
+                    break
+
+    if found and der:
+        pem = ssl.DER_cert_to_PEM_cert(der)
+        if pem in certifi.contents():
+            logger.debug(
+                "CA Certificate already exists in certifi store. Nothing to do."
+            )
+        else:
+            logger.debug("Writing certificate to certifi store.")
+            ca_file = certifi.where()
+            with open(ca_file, "ab") as f:
+                f.write(bytes(pem, "ascii"))
+            logger.debug("Completed")
+    else:
+        warnings.warn("Unable to locate root certificate on this host.")
+
+    return found
+
+
+def get_macos_equinor_certificates():
+    import ssl
+    import tempfile
+
+    ctx = ssl.create_default_context()
+    macos_ca_certs = subprocess.run(
+        ["security", "find-certificate", "-a", "-c", "Statoil Root CA", "-p"],
+        stdout=subprocess.PIPE,
+    ).stdout
+    with tempfile.NamedTemporaryFile("w+b") as tmp_file:
+        tmp_file.write(macos_ca_certs)
+        ctx.load_verify_locations(tmp_file.name)
+
+    return ctx.get_ca_certs(binary_form=True)
+
+
+def is_equinor() -> bool:
+    """Determines whether code is running on an Equinor host
+
+    If Windows host:
+    Finds host's domain in Windows Registry at
+    HKLM\\SYSTEM\\ControlSet001\\Services\\Tcpip\\Parameters\\Domain
+    If mac os host:
+    Finds statoil.net as AD hostname in certificates
+    If Linux host:
+    Checks whether statoil.no is search domain
+
+    Returns:
+        bool: True if Equinor
+    """
+    if is_windows():
+        with winreg.OpenKey(
+            winreg.HKEY_LOCAL_MACHINE, r"SYSTEM\ControlSet001\Services\Tcpip\Parameters"
+        ) as key:
+            domain = winreg.QueryValueEx(key, "Domain")
+        if "statoil" in domain[0]:
+            return True
+    elif is_mac():
+        s = subprocess.run(
+            ["security", "find-certificate", "-a", "-c" "client.statoil.net"],
+            stdout=subprocess.PIPE,
+        ).stdout
+
+        host = socket.gethostname()
+
+        if host + ".client.statoil.net" in str(s):
+            return True
+        elif "client.statoil.net" in host and host in str(s):
+            return True
+    elif is_linux():
+        with open("/etc/resolv.conf", "r") as f:
+            if "statoil.no" in f.read():
+                return True
+    else:
+        raise OSError(
+            f"Unsupported system: {platform.system()}. Please report this as an issue."
+        )
+    return False
+
+
+class IMSType(str, Enum):
+    PIWEBAPI = "piwebapi"
+    ASPENONE = "aspenone"
+    PI = "pi"
+    ASPEN = "aspen"
+    IP21 = "ip21"
```

### Comparing `tagreader-4.2.4/PKG-INFO` & `tagreader-4.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagreader
-Version: 4.2.4
+Version: 4.2.5
 Summary: Tagreader is a Python package for reading trend data from the OSIsoft PI and Aspen Infoplus.21 IMS systems.
 Home-page: https://github.com/equinor/tagreader-python
 License: MIT
 Keywords: Aspen InfoPlus.21,OSIsoft PI
 Author: Einar S. Idsø
 Author-email: eiids@equinor.com
 Requires-Python: >=3.8,<4.0
@@ -17,18 +17,14 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Provides-Extra: notebooks
 Requires-Dist: certifi (>=2023,<2024)
 Requires-Dist: diskcache (>=5.6.1,<6.0.0)
 Requires-Dist: jupyter (>=1,<2) ; extra == "notebooks"
```


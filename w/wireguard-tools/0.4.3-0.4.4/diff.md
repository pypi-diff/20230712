# Comparing `tmp/wireguard_tools-0.4.3.tar.gz` & `tmp/wireguard_tools-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wireguard_tools-0.4.3.tar", max compression
+gzip compressed data, was "wireguard_tools-0.4.4.tar", max compression
```

## Comparing `wireguard_tools-0.4.3.tar` & `wireguard_tools-0.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1083 2022-12-13 17:55:51.419036 wireguard_tools-0.4.3/LICENSE
-drwxr-xr-x   0        0        0        0 2022-12-13 17:55:51.419036 wireguard_tools-0.4.3/LICENSES/
--rw-r--r--   0        0        0      643 2022-12-13 17:55:51.419036 wireguard_tools-0.4.3/LICENSES/0BSD.txt
--rw-r--r--   0        0        0     1593 2022-12-13 17:55:51.419036 wireguard_tools-0.4.3/LICENSES/CC-PDDC.txt
--rw-r--r--   0        0        0     1078 2022-12-13 17:55:51.419036 wireguard_tools-0.4.3/LICENSES/MIT.txt
--rw-r--r--   0        0        0     6461 2023-02-10 16:50:15.058517 wireguard_tools-0.4.3/README.md
--rw-r--r--   0        0        0     2151 2023-06-15 19:21:39.004341 wireguard_tools-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      362 2023-06-15 19:21:39.004341 wireguard_tools-0.4.3/src/wireguard_tools/__init__.py
--rw-r--r--   0        0        0      188 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/src/wireguard_tools/__main__.py
--rw-r--r--   0        0        0     7924 2022-12-16 20:19:27.612313 wireguard_tools-0.4.3/src/wireguard_tools/cli.py
--rw-r--r--   0        0        0     5689 2022-12-19 15:20:49.914859 wireguard_tools-0.4.3/src/wireguard_tools/curve25519.py
--rw-r--r--   0        0        0        0 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/src/wireguard_tools/py.typed
--rw-r--r--   0        0        0      335 2023-03-15 16:34:00.717711 wireguard_tools-0.4.3/src/wireguard_tools/tunnel.conf
--rw-r--r--   0        0        0    11336 2023-06-15 19:18:53.774947 wireguard_tools-0.4.3/src/wireguard_tools/wireguard_config.py
--rw-r--r--   0        0        0     1250 2022-12-16 19:21:20.697346 wireguard_tools-0.4.3/src/wireguard_tools/wireguard_device.py
--rw-r--r--   0        0        0     2571 2022-12-19 15:53:22.370441 wireguard_tools-0.4.3/src/wireguard_tools/wireguard_key.py
--rw-r--r--   0        0        0     4456 2023-05-24 16:10:17.684255 wireguard_tools-0.4.3/src/wireguard_tools/wireguard_netlink.py
--rw-r--r--   0        0        0     5964 2022-12-19 15:53:36.746821 wireguard_tools-0.4.3/src/wireguard_tools/wireguard_uapi.py
--rw-r--r--   0        0        0        0 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/tests/__init__.py
--rw-r--r--   0        0        0      215 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/tests/conftest.py
--rw-r--r--   0        0        0     8965 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/tests/test_curve25519.py
--rw-r--r--   0        0        0     1460 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/tests/test_wireguard_config.py
--rw-r--r--   0        0        0      661 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/tests/test_wireguard_key.py
--rw-r--r--   0        0        0     7570 1970-01-01 00:00:00.000000 wireguard_tools-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-12-14 04:23:20.284345 wireguard_tools-0.4.4/LICENSE
+drwxr-xr-x   0        0        0        0 2022-12-14 04:23:20.284345 wireguard_tools-0.4.4/LICENSES/
+-rw-r--r--   0        0        0      643 2022-12-14 04:23:20.284345 wireguard_tools-0.4.4/LICENSES/0BSD.txt
+-rw-r--r--   0        0        0     1593 2022-12-14 04:23:20.284345 wireguard_tools-0.4.4/LICENSES/CC-PDDC.txt
+-rw-r--r--   0        0        0     1078 2022-12-14 04:23:20.284345 wireguard_tools-0.4.4/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     6958 2023-07-12 15:52:59.142155 wireguard_tools-0.4.4/README.md
+-rw-r--r--   0        0        0     2184 2023-07-12 15:53:43.571076 wireguard_tools-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      362 2023-07-12 15:53:43.571076 wireguard_tools-0.4.4/src/wireguard_tools/__init__.py
+-rw-r--r--   0        0        0      188 2022-12-14 04:23:20.288346 wireguard_tools-0.4.4/src/wireguard_tools/__main__.py
+-rw-r--r--   0        0        0     7924 2022-12-21 14:10:25.624032 wireguard_tools-0.4.4/src/wireguard_tools/cli.py
+-rw-r--r--   0        0        0     5689 2022-12-21 14:10:25.624032 wireguard_tools-0.4.4/src/wireguard_tools/curve25519.py
+-rw-r--r--   0        0        0        0 2022-12-14 04:23:20.288346 wireguard_tools-0.4.4/src/wireguard_tools/py.typed
+-rw-r--r--   0        0        0    12002 2023-07-12 15:52:59.142155 wireguard_tools-0.4.4/src/wireguard_tools/wireguard_config.py
+-rw-r--r--   0        0        0     1250 2022-12-21 14:10:25.624032 wireguard_tools-0.4.4/src/wireguard_tools/wireguard_device.py
+-rw-r--r--   0        0        0     2571 2022-12-21 14:10:25.624032 wireguard_tools-0.4.4/src/wireguard_tools/wireguard_key.py
+-rw-r--r--   0        0        0     4456 2023-07-12 15:52:59.142155 wireguard_tools-0.4.4/src/wireguard_tools/wireguard_netlink.py
+-rw-r--r--   0        0        0     5964 2022-12-21 14:10:25.624032 wireguard_tools-0.4.4/src/wireguard_tools/wireguard_uapi.py
+-rw-r--r--   0        0        0        0 2022-12-14 04:23:20.288346 wireguard_tools-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0      215 2022-12-14 04:23:20.288346 wireguard_tools-0.4.4/tests/conftest.py
+-rw-r--r--   0        0        0     8965 2022-12-14 04:23:20.288346 wireguard_tools-0.4.4/tests/test_curve25519.py
+-rw-r--r--   0        0        0     3465 2023-07-12 15:52:59.142155 wireguard_tools-0.4.4/tests/test_wireguard_config.py
+-rw-r--r--   0        0        0      661 2022-12-14 04:23:20.288346 wireguard_tools-0.4.4/tests/test_wireguard_key.py
+-rw-r--r--   0        0        0     8105 1970-01-01 00:00:00.000000 wireguard_tools-0.4.4/setup.py
+-rw-r--r--   0        0        0     8067 1970-01-01 00:00:00.000000 wireguard_tools-0.4.4/PKG-INFO
```

### Comparing `wireguard_tools-0.4.3/LICENSE` & `wireguard_tools-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.3/LICENSES/0BSD.txt` & `wireguard_tools-0.4.4/LICENSES/0BSD.txt`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.3/LICENSES/CC-PDDC.txt` & `wireguard_tools-0.4.4/LICENSES/CC-PDDC.txt`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.3/LICENSES/MIT.txt` & `wireguard_tools-0.4.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.3/README.md` & `wireguard_tools-0.4.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -80,14 +80,28 @@
 ```python
 from wireguard_tools import WireguardConfig
 
 with open("wg0.conf") as fh:
     config = WireguardConfig.from_wgconfig(fh)
 ```
 
+Also supported are the "Friendly Tags" comments as introduced by
+prometheus-wireguard-exporter, where a `[Peer]` section can contain
+comments which add a user friendly description and/or additional attributes.
+
+```
+[Peer]
+# friendly_name = Peer description for end users
+# friendly_json = {"flat"="json", "dictionary"=1, "attribute"=2}
+...
+```
+
+These will show up as additional `friendly_name` and `friendly_json` attributes
+on the WireguardPeer object.
+
 We can also serialize and deserialize from a simple dict-based format which
 uses only basic JSON datatypes and, as such, can be used to convert to various
 formats (i.e. json, yaml, toml, pickle) either to disk or to pass over a
 network.
 
 ```python
 from wireguard_tools import WireguardConfig
@@ -99,14 +113,15 @@
         dict(
             public_key="...",
             preshared_key=None,
             endpoint_host="remote_host",
             endpoint_port=5120,
             persistent_keepalive=30,
             allowed_ips=["0.0.0.0/0"],
+            friendly_name="Awesome Peer",
         ),
     ],
 )
 config = WireguardConfig.from_dict(dict_config)
 
 dict_config = config.asdict()
 pprint(dict_config)
```

### Comparing `wireguard_tools-0.4.3/pyproject.toml` & `wireguard_tools-0.4.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2022-2023 Carnegie Mellon University
 # SPDX-License-Identifier: 0BSD
 
 [tool.poetry]
 name = "wireguard-tools"
-version = "0.4.3"
+version = "0.4.4"
 description = "Pure python reimplementation of wireguard-tools"
 authors = [
     "Carnegie Mellon University <satya+group@cs.cmu.edu>",
     "Jan Harkes <jaharkes@cs.cmu.edu>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -35,15 +35,15 @@
 attrs = ">=22.1.0"
 pyroute2 = "^0.7.3"
 segno = "^1.5.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 poethepoet = "^0.16.5"
-pre-commit = "^2.16.0"
+pre-commit = { version = "^2.16.0", python = "^3.8.1" }
 tbump = "^6.9.0"
 
 [tool.poetry.group.test.dependencies]
 mypy = "^0.991"
 pytest = "^6.2.5"
 pytest-mock = "^3.6.1"
```

### Comparing `wireguard_tools-0.4.3/src/wireguard_tools/cli.py` & `wireguard_tools-0.4.4/src/wireguard_tools/cli.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.3/src/wireguard_tools/curve25519.py` & `wireguard_tools-0.4.4/src/wireguard_tools/curve25519.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.3/src/wireguard_tools/wireguard_config.py` & `wireguard_tools-0.4.4/src/wireguard_tools/wireguard_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 #
 # Copyright (c) 2022-2023 Carnegie Mellon University
 # SPDX-License-Identifier: MIT
 #
 
 from __future__ import annotations
 
+import json
 import re
 from ipaddress import (
     IPv4Address,
     IPv4Interface,
     IPv6Address,
     IPv6Interface,
     ip_address,
     ip_interface,
 )
-from typing import Any, Sequence, TextIO, TypeVar
+from typing import Any, Sequence, TextIO, TypeVar, Union
 
 from attrs import asdict, define, field
 from attrs.converters import optional
 from attrs.setters import convert as setters_convert
 from segno import QRCode, make_qr
 
 from .wireguard_key import WireguardKey
 
+SimpleJsonTypes = Union[str, int, float, bool, None]
 T = TypeVar("T")
 
 
 def _ipaddress_or_host(
     host: IPv4Address | IPv6Address | str,
 ) -> IPv4Address | IPv6Address | str:
     if isinstance(host, (IPv4Address, IPv6Address)):
@@ -61,14 +63,17 @@
         converter=optional(_ipaddress_or_host), default=None
     )
     endpoint_port: int | None = field(converter=optional(int), default=None)
     persistent_keepalive: int | None = field(converter=optional(int), default=None)
     allowed_ips: list[IPv4Interface | IPv6Interface] = field(
         converter=_list_of_ipinterface, factory=list
     )
+    # comment tags that can be parsed by prometheus-wireguard-exporter
+    friendly_name: str | None = None
+    friendly_json: dict[str, SimpleJsonTypes] | None = None
 
     # peer statistics from device
     last_handshake: float | None = field(
         converter=optional(float), default=None, eq=False
     )
     rx_bytes: int | None = field(converter=optional(int), default=None, eq=False)
     tx_bytes: int | None = field(converter=optional(int), default=None, eq=False)
@@ -111,21 +116,28 @@
                 conf["endpoint_port"] = int(port)
             elif key == "persistentkeepalive":
                 conf["persistent_keepalive"] = int(value)
             elif key == "allowedips":
                 conf.setdefault("allowed_ips", []).extend(
                     ip_interface(addr) for addr in value.split(", ")
                 )
+            elif key == "# friendly_name":
+                conf["friendly_name"] = value
+            elif key == "# friendly_json":
+                conf["friendly_json"] = json.loads(value)
         return cls(**conf)
 
     def as_wgconfig_snippet(self) -> list[str]:
-        conf = [
-            "\n[Peer]",
-            f"PublicKey = {self.public_key}",
-        ]
+        conf = ["\n[Peer]"]
+        if self.friendly_name:
+            conf.append(f"# friendly_name = {self.friendly_name}")
+        if self.friendly_json is not None:
+            value = json.dumps(self.friendly_json)
+            conf.append(f"# friendly_json = {value}")
+        conf.append(f"PublicKey = {self.public_key}")
         if self.preshared_key:
             conf.append(f"PresharedKey = {self.preshared_key}")
         if self.endpoint_host:
             conf.append(f"Endpoint = {self.endpoint_host}:{self.endpoint_port}")
         if self.persistent_keepalive:
             conf.append(f"PersistentKeepalive = {self.persistent_keepalive}")
         conf.extend([f"AllowedIPs = {addr}" for addr in self.allowed_ips])
@@ -202,16 +214,16 @@
         sections = [section.lower() for section in parts[0::2]]
         if sections.count("interface") > 1:
             raise ValueError("More than one [Interface] section in config file")
 
         config = cls()
         for section, content in zip(sections, parts[1::2]):
             key_value = [
-                (match.group(1), match.group(2))
-                for match in re.finditer(r"^(\w+)\s*=\s*(.+)$", content, re.M)
+                (match.group(1), match.group(3))
+                for match in re.finditer(r"^((# )?\w+)\s*=\s*(.+)$", content, re.M)
             ]
             if section == "interface":
                 config._update_from_conf(key_value)
             else:
                 peer = WireguardPeer.from_wgconfig(key_value)
                 config.add_peer(peer)
         return config
```

### Comparing `wireguard_tools-0.4.3/src/wireguard_tools/wireguard_device.py` & `wireguard_tools-0.4.4/src/wireguard_tools/wireguard_device.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.3/src/wireguard_tools/wireguard_key.py` & `wireguard_tools-0.4.4/src/wireguard_tools/wireguard_key.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.3/src/wireguard_tools/wireguard_netlink.py` & `wireguard_tools-0.4.4/src/wireguard_tools/wireguard_netlink.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.3/src/wireguard_tools/wireguard_uapi.py` & `wireguard_tools-0.4.4/src/wireguard_tools/wireguard_uapi.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.3/tests/test_curve25519.py` & `wireguard_tools-0.4.4/tests/test_curve25519.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.3/tests/test_wireguard_key.py` & `wireguard_tools-0.4.4/tests/test_wireguard_key.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.3/PKG-INFO` & `wireguard_tools-0.4.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wireguard-tools
-Version: 0.4.3
+Version: 0.4.4
 Summary: Pure python reimplementation of wireguard-tools
 Home-page: https://github.com/cmusatyalab/wireguard-tools
 License: MIT
 Author: Carnegie Mellon University
 Author-email: satya+group@cs.cmu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -107,14 +107,28 @@
 ```python
 from wireguard_tools import WireguardConfig
 
 with open("wg0.conf") as fh:
     config = WireguardConfig.from_wgconfig(fh)
 ```
 
+Also supported are the "Friendly Tags" comments as introduced by
+prometheus-wireguard-exporter, where a `[Peer]` section can contain
+comments which add a user friendly description and/or additional attributes.
+
+```
+[Peer]
+# friendly_name = Peer description for end users
+# friendly_json = {"flat"="json", "dictionary"=1, "attribute"=2}
+...
+```
+
+These will show up as additional `friendly_name` and `friendly_json` attributes
+on the WireguardPeer object.
+
 We can also serialize and deserialize from a simple dict-based format which
 uses only basic JSON datatypes and, as such, can be used to convert to various
 formats (i.e. json, yaml, toml, pickle) either to disk or to pass over a
 network.
 
 ```python
 from wireguard_tools import WireguardConfig
@@ -126,14 +140,15 @@
         dict(
             public_key="...",
             preshared_key=None,
             endpoint_host="remote_host",
             endpoint_port=5120,
             persistent_keepalive=30,
             allowed_ips=["0.0.0.0/0"],
+            friendly_name="Awesome Peer",
         ),
     ],
 )
 config = WireguardConfig.from_dict(dict_config)
 
 dict_config = config.asdict()
 pprint(dict_config)
```


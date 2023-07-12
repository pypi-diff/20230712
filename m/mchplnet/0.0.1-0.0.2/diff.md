# Comparing `tmp/mchplnet-0.0.1.tar.gz` & `tmp/mchplnet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mchplnet-0.0.1.tar", max compression
+gzip compressed data, was "mchplnet-0.0.2.tar", max compression
```

## Comparing `mchplnet-0.0.1.tar` & `mchplnet-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1104 2023-07-07 12:17:00.822414 mchplnet-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2023-07-11 12:20:23.551491 mchplnet-0.0.1/mchplnet/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 12:17:00.838364 mchplnet-0.0.1/mchplnet/interfaces/__init__.py
--rw-r--r--   0        0        0      492 2023-07-12 09:17:46.715161 mchplnet-0.0.1/mchplnet/interfaces/abstract_interface.py
--rw-r--r--   0        0        0      345 2023-07-11 14:38:58.077887 mchplnet-0.0.1/mchplnet/interfaces/can.py
--rw-r--r--   0        0        0     2244 2023-07-12 09:26:42.494971 mchplnet-0.0.1/mchplnet/interfaces/factory.py
--rw-r--r--   0        0        0      345 2023-07-11 14:38:58.062936 mchplnet-0.0.1/mchplnet/interfaces/lin.py
--rw-r--r--   0        0        0      347 2023-07-11 14:38:58.077887 mchplnet-0.0.1/mchplnet/interfaces/tcp_ip.py
--rw-r--r--   0        0        0     3243 2023-07-12 09:44:45.714456 mchplnet-0.0.1/mchplnet/interfaces/uart.py
--rw-r--r--   0        0        0     3031 2023-07-12 09:29:15.930644 mchplnet-0.0.1/mchplnet/lnet.py
--rw-r--r--   0        0        0     8686 2023-07-12 10:11:45.484710 mchplnet-0.0.1/mchplnet/lnetframe.py
--rw-r--r--   0        0        0        0 2023-07-07 12:17:00.844341 mchplnet-0.0.1/mchplnet/services/__init__.py
--rw-r--r--   0        0        0      234 2023-07-11 14:38:58.075893 mchplnet-0.0.1/mchplnet/services/device_info.py
--rw-r--r--   0        0        0     6168 2023-07-12 10:10:46.966881 mchplnet-0.0.1/mchplnet/services/frame_device_info.py
--rw-r--r--   0        0        0     2772 2023-07-12 10:10:46.915543 mchplnet-0.0.1/mchplnet/services/frame_getram.py
--rw-r--r--   0        0        0     2485 2023-07-12 10:09:20.481403 mchplnet-0.0.1/mchplnet/services/frame_putram.py
--rw-r--r--   0        0        0      730 2023-07-12 11:34:47.247848 mchplnet-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1227 2023-07-12 08:33:10.774146 mchplnet-0.0.1/README.md
--rw-r--r--   0        0        0     2195 1970-01-01 00:00:00.000000 mchplnet-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1104 2023-07-07 12:17:00.822414 mchplnet-0.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-11 12:20:23.551491 mchplnet-0.0.2/mchplnet/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 12:17:00.838364 mchplnet-0.0.2/mchplnet/interfaces/__init__.py
+-rw-r--r--   0        0        0      492 2023-07-12 09:17:46.715161 mchplnet-0.0.2/mchplnet/interfaces/abstract_interface.py
+-rw-r--r--   0        0        0      347 2023-07-12 11:39:11.922563 mchplnet-0.0.2/mchplnet/interfaces/can.py
+-rw-r--r--   0        0        0     2254 2023-07-12 11:39:11.947475 mchplnet-0.0.2/mchplnet/interfaces/factory.py
+-rw-r--r--   0        0        0      347 2023-07-12 11:39:11.916578 mchplnet-0.0.2/mchplnet/interfaces/lin.py
+-rw-r--r--   0        0        0      349 2023-07-12 11:39:11.877712 mchplnet-0.0.2/mchplnet/interfaces/tcp_ip.py
+-rw-r--r--   0        0        0     3245 2023-07-12 11:39:11.905615 mchplnet-0.0.2/mchplnet/interfaces/uart.py
+-rw-r--r--   0        0        0     3041 2023-07-12 11:39:11.953455 mchplnet-0.0.2/mchplnet/lnet.py
+-rw-r--r--   0        0        0     8686 2023-07-12 10:11:45.484710 mchplnet-0.0.2/mchplnet/lnetframe.py
+-rw-r--r--   0        0        0        0 2023-07-07 12:17:00.844341 mchplnet-0.0.2/mchplnet/services/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-11 14:38:58.075893 mchplnet-0.0.2/mchplnet/services/device_info.py
+-rw-r--r--   0        0        0     6172 2023-07-12 11:39:11.966411 mchplnet-0.0.2/mchplnet/services/frame_device_info.py
+-rw-r--r--   0        0        0     2774 2023-07-12 11:39:11.942492 mchplnet-0.0.2/mchplnet/services/frame_getram.py
+-rw-r--r--   0        0        0     2487 2023-07-12 11:39:11.936511 mchplnet-0.0.2/mchplnet/services/frame_putram.py
+-rw-r--r--   0        0        0      730 2023-07-12 11:46:47.066905 mchplnet-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1236 2023-07-12 11:39:49.127559 mchplnet-0.0.2/README.md
+-rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 mchplnet-0.0.2/PKG-INFO
```

### Comparing `mchplnet-0.0.1/LICENSE` & `mchplnet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mchplnet-0.0.1/mchplnet/interfaces/factory.py` & `mchplnet-0.0.2/mchplnet/interfaces/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 
-from pylnet.interfaces.abstract_interface import InterfaceABC
-from pylnet.interfaces.can import LNetCan
-from pylnet.interfaces.lin import LNetLin
-from pylnet.interfaces.tcp_ip import LNetTcpIp
-from pylnet.interfaces.uart import LNetSerial
+from mchplnet.interfaces.abstract_interface import InterfaceABC
+from mchplnet.interfaces.can import LNetCan
+from mchplnet.interfaces.lin import LNetLin
+from mchplnet.interfaces.tcp_ip import LNetTcpIp
+from mchplnet.interfaces.uart import LNetSerial
 
 
 class InterfaceType(Enum):
     SERIAL = 1
     CAN = 2
     LIN = 3
     TCP_IP = 4
```

### Comparing `mchplnet-0.0.1/mchplnet/interfaces/uart.py` & `mchplnet-0.0.2/mchplnet/interfaces/uart.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import serial
 
-from pylnet.interfaces.abstract_interface import InterfaceABC
+from mchplnet.interfaces.abstract_interface import InterfaceABC
 
 
 class LNetSerial(InterfaceABC):
     def __init__(self, *args, **kwargs):
         self.com_port = kwargs["port"] if "port" in kwargs else "COM11"
         self.baud_rate = kwargs["baud_rate"] if "baud_rate" in kwargs else 115200
         self.parity = kwargs["parity"] if "parity" in kwargs else 0
```

### Comparing `mchplnet-0.0.1/mchplnet/lnet.py` & `mchplnet-0.0.2/mchplnet/lnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from pylnet.interfaces.abstract_interface import InterfaceABC
-from pylnet.services.device_info import DeviceInfo
-from pylnet.services.frame_device_info import FrameDeviceInfo
-from pylnet.services.frame_getram import FrameGetRam
-from pylnet.services.frame_putram import FramePutRam
+from mchplnet.interfaces.abstract_interface import InterfaceABC
+from mchplnet.services.device_info import DeviceInfo
+from mchplnet.services.frame_device_info import FrameDeviceInfo
+from mchplnet.services.frame_getram import FrameGetRam
+from mchplnet.services.frame_putram import FramePutRam
 
 
 class LNet(object):
     """Handle the LNet logic and services"""
 
     def __init__(self, interface: InterfaceABC, handshake: bool = True):
         self.interface = interface
```

### Comparing `mchplnet-0.0.1/mchplnet/lnetframe.py` & `mchplnet-0.0.2/mchplnet/lnetframe.py`

 * *Files identical despite different names*

### Comparing `mchplnet-0.0.1/mchplnet/services/frame_device_info.py` & `mchplnet-0.0.2/mchplnet/services/frame_device_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from pylnet.lnetframe import LNetFrame
-from pylnet.services.device_info import DeviceInfo
+from mchplnet.lnetframe import LNetFrame
+from mchplnet.services.device_info import DeviceInfo
 
 
 class FrameDeviceInfo(LNetFrame):
     def __init__(self):
         """
         This frame is responsible for Hand-Shake, Monitor-Version, Identifying processor Type, Application Version.
         """
```

### Comparing `mchplnet-0.0.1/mchplnet/services/frame_getram.py` & `mchplnet-0.0.2/mchplnet/services/frame_getram.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pylnet.lnetframe import LNetFrame
+from mchplnet.lnetframe import LNetFrame
 
 
 class FrameGetRam(LNetFrame):
     def __init__(self, address: int, size: int, width: int):
         """
         Responsible for setting up the request frame for MCU to 'Get' the variable value.
         @param address: Address of the variable
```

### Comparing `mchplnet-0.0.1/mchplnet/services/frame_putram.py` & `mchplnet-0.0.2/mchplnet/services/frame_putram.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from pylnet.lnetframe import LNetFrame
+from mchplnet.lnetframe import LNetFrame
 
 
 class FramePutRam(LNetFrame):
     def __init__(self, address: int, size: int, width: int, value: bytearray = []):
         """
         responsible for setting up the request frame for MCU to 'Set' the variable value.
```

### Comparing `mchplnet-0.0.1/pyproject.toml` & `mchplnet-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 
 [tool.poetry]
 
 name = "mchplnet"
 
-version = "0.0.1"
+version = "0.0.2"
 
 description = "python implementation of X2Cscope"
 
 authors = ["Yash Agarwal <yash.agarwal@microchip.com>",
 
   "Edras Pacola",
```

### Comparing `mchplnet-0.0.1/README.md` & `mchplnet-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 <p align="center">
   <img src="pyx2cscope/docs/img/microchip-technology-logo.png" alt="PyX2CScope Logo" width="250">
 </p>
 
-# pylnet
-- pylnet is the Python implementation of the LNet protocol.
-- It implements multiple LNet services to commincate to embedded systems/microcontrollers.
+# mchplnet
+- mchplnet is the Python implementation of the LNet protocol.
+- It implements multiple LNet services to communicate to embedded systems/microcontrollers.
 - Currently only pyserial interface is supported 
-- Recommended to use pyx2cscope package instead of this low level implementation
+- Recommended to use pyx2cscope package instead of this low-level implementation
 
 ## Getting Started
 
 ```
-import pylnet
+import mchplnet
 import serial
-l_net = pylnet.LNet(serial.Serial('COM8', 115200))
+l_net = mchplnet.LNet(serial.Serial('COM8', 115200))
 var_address = 0x00000000
 var_size = 4 
 var_value = l_net.get_ram(var_address, var_size) 
 print(var_value)
 var_newValue = 500
 l_net.put_ram(var_address, var_size, var_newValue)
 ```
```

### Comparing `mchplnet-0.0.1/PKG-INFO` & `mchplnet-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mchplnet
-Version: 0.0.1
+Version: 0.0.2
 Summary: python implementation of X2Cscope
 Home-page: https://x2cscope.github.io/
 License: Proprietary
 Author: Yash Agarwal
 Author-email: yash.agarwal@microchip.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 2
@@ -23,26 +23,26 @@
 Project-URL: Repository, https://github.com/X2Cscope/pylnet
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="pyx2cscope/docs/img/microchip-technology-logo.png" alt="PyX2CScope Logo" width="250">
 </p>
 
-# pylnet
-- pylnet is the Python implementation of the LNet protocol.
-- It implements multiple LNet services to commincate to embedded systems/microcontrollers.
+# mchplnet
+- mchplnet is the Python implementation of the LNet protocol.
+- It implements multiple LNet services to communicate to embedded systems/microcontrollers.
 - Currently only pyserial interface is supported 
-- Recommended to use pyx2cscope package instead of this low level implementation
+- Recommended to use pyx2cscope package instead of this low-level implementation
 
 ## Getting Started
 
 ```
-import pylnet
+import mchplnet
 import serial
-l_net = pylnet.LNet(serial.Serial('COM8', 115200))
+l_net = mchplnet.LNet(serial.Serial('COM8', 115200))
 var_address = 0x00000000
 var_size = 4 
 var_value = l_net.get_ram(var_address, var_size) 
 print(var_value)
 var_newValue = 500
 l_net.put_ram(var_address, var_size, var_newValue)
 ```
```


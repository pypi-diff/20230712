# Comparing `tmp/aioping-0.3.1.tar.gz` & `tmp/aioping-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aioping-0.3.1.tar", last modified: Sun Jul  5 23:33:02 2020, max compression
+gzip compressed data, was "aioping-0.4.0.tar", last modified: Tue Jul 11 23:59:33 2023, max compression
```

## Comparing `aioping-0.3.1.tar` & `aioping-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2020-07-05 23:33:02.000000 aioping-0.3.1/
--rw-r--r--   0 anton      (501) staff       (20)      790 2020-07-05 23:33:02.000000 aioping-0.3.1/PKG-INFO
--rw-r--r--   0 anton      (501) staff       (20)     2825 2020-07-05 23:28:54.000000 aioping-0.3.1/README.rst
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2020-07-05 23:33:02.000000 aioping-0.3.1/aioping/
--rw-r--r--   0 anton      (501) staff       (20)     9204 2020-07-05 23:16:13.000000 aioping-0.3.1/aioping/__init__.py
-drwxr-xr-x   0 anton      (501) staff       (20)        0 2020-07-05 23:33:02.000000 aioping-0.3.1/aioping.egg-info/
--rw-r--r--   0 anton      (501) staff       (20)      790 2020-07-05 23:33:01.000000 aioping-0.3.1/aioping.egg-info/PKG-INFO
--rw-r--r--   0 anton      (501) staff       (20)      203 2020-07-05 23:33:01.000000 aioping-0.3.1/aioping.egg-info/SOURCES.txt
--rw-r--r--   0 anton      (501) staff       (20)        1 2020-07-05 23:33:01.000000 aioping-0.3.1/aioping.egg-info/dependency_links.txt
--rw-r--r--   0 anton      (501) staff       (20)       21 2020-07-05 23:33:01.000000 aioping-0.3.1/aioping.egg-info/requires.txt
--rw-r--r--   0 anton      (501) staff       (20)        8 2020-07-05 23:33:01.000000 aioping-0.3.1/aioping.egg-info/top_level.txt
--rw-r--r--   0 anton      (501) staff       (20)       80 2020-07-05 23:33:02.000000 aioping-0.3.1/setup.cfg
--rw-r--r--   0 anton      (501) staff       (20)      915 2020-07-05 23:16:13.000000 aioping-0.3.1/setup.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-07-11 23:59:33.833438 aioping-0.4.0/
+-rw-r--r--   0 anton      (501) staff       (20)    18092 2020-08-20 13:04:52.000000 aioping-0.4.0/LICENSE.txt
+-rw-r--r--   0 anton      (501) staff       (20)      871 2023-07-11 23:59:33.833547 aioping-0.4.0/PKG-INFO
+-rw-r--r--   0 anton      (501) staff       (20)     2758 2023-07-11 23:55:00.000000 aioping-0.4.0/README.rst
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-07-11 23:59:33.831340 aioping-0.4.0/aioping/
+-rw-r--r--   0 anton      (501) staff       (20)     9834 2023-07-11 23:40:34.000000 aioping-0.4.0/aioping/__init__.py
+drwxr-xr-x   0 anton      (501) staff       (20)        0 2023-07-11 23:59:33.833211 aioping-0.4.0/aioping.egg-info/
+-rw-r--r--   0 anton      (501) staff       (20)      871 2023-07-11 23:59:33.000000 aioping-0.4.0/aioping.egg-info/PKG-INFO
+-rw-r--r--   0 anton      (501) staff       (20)      215 2023-07-11 23:59:33.000000 aioping-0.4.0/aioping.egg-info/SOURCES.txt
+-rw-r--r--   0 anton      (501) staff       (20)        1 2023-07-11 23:59:33.000000 aioping-0.4.0/aioping.egg-info/dependency_links.txt
+-rw-r--r--   0 anton      (501) staff       (20)       21 2023-07-11 23:59:33.000000 aioping-0.4.0/aioping.egg-info/requires.txt
+-rw-r--r--   0 anton      (501) staff       (20)        8 2023-07-11 23:59:33.000000 aioping-0.4.0/aioping.egg-info/top_level.txt
+-rw-r--r--   0 anton      (501) staff       (20)       80 2023-07-11 23:59:33.833967 aioping-0.4.0/setup.cfg
+-rw-rw-r--   0 anton      (501) staff       (20)     1024 2023-07-11 23:43:03.000000 aioping-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aioping-0.3.1/PKG-INFO` & `aioping-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: aioping
-Version: 0.3.1
+Version: 0.4.0
 Summary: Asyncio ping implementation
 Home-page: https://github.com/stellarbit/aioping
+Download-URL: https://github.com/stellarbit/aioping/tarball/0.4.0
 Author: Anton Belousov
-Author-email: anton@stellarbit.com
-License: UNKNOWN
-Download-URL: https://github.com/stellarbit/aioping/tarball/0.3.1
-Description: UNKNOWN
+Author-email: anton@belousov.co
 Keywords: network,icmp,ping,asyncio
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE.txt
```

### Comparing `aioping-0.3.1/README.rst` & `aioping-0.4.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -15,27 +15,24 @@
     $ pip install git+https://github.com/stellarbit/aioping
 
 Using aioping
 -------------
 
 There are 2 ways to use the library.
 
-First one is interactive, which sends results to standard Python logger.
-Please make sure you are running this code under root, as only
-root is allowed to send ICMP packets:
+First one is interactive, which sends results to standard Python logger:
 
 .. code:: python
 
     import asyncio
     import aioping
     import logging
 
     logging.basicConfig(level=logging.INFO)     # or logging.DEBUG
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(aioping.verbose_ping("google.com"))
+    asyncio.run(aioping.verbose_ping("google.com"))
 
 Alternatively, you can call a ping function, which returns a
 ping delay in milliseconds or throws an exception in case of
 error:
 
 .. code:: python
 
@@ -46,16 +43,15 @@
         try:
             delay = await aioping.ping(host) * 1000
             print("Ping response in %s ms" % delay)
 
         except TimeoutError:
             print("Timed out")
 
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(do_ping("google.com"))
+    asyncio.run(do_ping("google.com"))
 
 Methods
 -------
 
 ``ping(dest_addr, timeout=10, family=None)``
 
 - ``dest_addr`` - destination address, IPv4, IPv6 or hostname
@@ -93,13 +89,17 @@
   - https://github.com/asantoni
   - https://github.com/eddebc
   - https://github.com/wise0wl
   - https://github.com/nARN
   - https://github.com/hergla
   - https://github.com/hanieljgoertz
   - https://github.com/Crypto-Spartan
+  - https://github.com/liordot
+  - https://github.com/dkaplan1
+  - https://github.com/haron
+  - https://github.com/matteomartelli
 
 
 License
 -------
 
 aioping is licensed under GPLv2.
```

### Comparing `aioping-0.3.1/aioping/__init__.py` & `aioping-0.4.0/aioping/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 import sys
 import socket
 import struct
 import time
 import functools
 import uuid
 import random
+import platform
+import os
 
 logger = logging.getLogger("aioping")
 default_timer = time.perf_counter
 
 if sys.platform.startswith("win"):
     if sys.version_info[0] > 3 or (sys.version_info[0] == 3 and sys.version_info[1] >= 8):
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
@@ -143,33 +145,46 @@
     :param id_:
     :param timeout:
     :return:
     """
     loop = asyncio.get_event_loop()
 
     try:
-        with async_timeout.timeout(timeout):
+        async with async_timeout.timeout(timeout):
             while True:
                 rec_packet = await loop.sock_recv(my_socket, 1024)
+
+                # No IP Header when unpriviledged on Linux
+                has_ip_header = (
+                    (os.name != "posix")
+                    or (platform.system() == "Darwin")
+                    or (my_socket.type == socket.SOCK_RAW)
+                )
+
                 time_received = default_timer()
 
-                if my_socket.family == socket.AddressFamily.AF_INET:
+                if my_socket.family == socket.AddressFamily.AF_INET and has_ip_header:
                     offset = 20
                 else:
                     offset = 0
 
                 icmp_header = rec_packet[offset:offset + 8]
 
                 type, code, checksum, packet_id, sequence = struct.unpack(
-                    "bbHHh", icmp_header
+                    "BBHHH", icmp_header
                 )
 
                 if type != ICMP_ECHO_REPLY and type != ICMP6_ECHO_REPLY:
                     continue
 
+                if not has_ip_header:  
+                    # When unprivileged on Linux, ICMP ID is rewrited by kernel
+                    # According to https://stackoverflow.com/a/14023878/4528364
+                    id_ = int.from_bytes(my_socket.getsockname()[1].to_bytes(2, "big"), "little")
+
                 if packet_id == id_:
                     data = rec_packet[offset + 8:offset + 8 + struct.calcsize("d")]
                     time_sent = struct.unpack("d", data)[0]
 
                     return time_received - time_sent
 
     except asyncio.TimeoutError:
@@ -205,26 +220,26 @@
     icmp_type = ICMP_ECHO_REQUEST if family == socket.AddressFamily.AF_INET\
         else ICMP6_ECHO_REQUEST
 
     # Header is type (8), code (8), checksum (16), id (16), sequence (16)
     my_checksum = 0
 
     # Make a dummy header with a 0 checksum.
-    header = struct.pack("BbHHh", icmp_type, 0, my_checksum, id_, 1)
+    header = struct.pack("BBHHH", icmp_type, 0, my_checksum, id_, 1)
     bytes_in_double = struct.calcsize("d")
     data = (192 - bytes_in_double) * "Q"
     data = struct.pack("d", default_timer()) + data.encode("ascii")
 
     # Calculate the checksum on the data and the dummy header.
     my_checksum = checksum(header + data)
 
     # Now that we have the right checksum, we put that in. It's just easier
     # to make up a new header than to stuff it into the dummy.
     header = struct.pack(
-        "BbHHh", icmp_type, 0, socket.htons(my_checksum), id_, 1
+        "BBHHH", icmp_type, 0, socket.htons(my_checksum), id_, 1
     )
     packet = header + data
 
     future = asyncio.get_event_loop().create_future()
     callback = functools.partial(sendto_ready, packet=packet, socket=my_socket, dest=dest_addr, future=future)
     asyncio.get_event_loop().add_writer(my_socket, callback)
 
@@ -260,29 +275,24 @@
     if family == socket.AddressFamily.AF_INET:
         icmp = proto_icmp
     else:
         icmp = proto_icmp6
 
     try:
         my_socket = socket.socket(family, socket.SOCK_RAW, icmp)
-        my_socket.setblocking(False)
 
     except OSError as e:
-        msg = e.strerror
-
         if e.errno == 1:
-            # Operation not permitted
-            msg += (
-                " - Note that ICMP messages can only be sent from processes"
-                " running as root."
-            )
-
-            raise OSError(msg)
+            # Operation not permitted, using SOCK_DGRAM instead:
+            my_socket = socket.socket(family, socket.SOCK_DGRAM, icmp)
+            logger.debug("Error using socket.SOCK_RAW: '%s'. Using socket.SOCK_DGRAM instead", e.strerror)
+        else:
+            raise
 
-        raise
+    my_socket.setblocking(False)
 
     my_id = uuid.uuid4().int & 0xFFFF
 
     await send_one_ping(my_socket, addr, my_id, timeout, family)
     delay = await receive_one_ping(my_socket, my_id, timeout)
     my_socket.close()
```

### Comparing `aioping-0.3.1/aioping.egg-info/PKG-INFO` & `aioping-0.4.0/aioping.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: aioping
-Version: 0.3.1
+Version: 0.4.0
 Summary: Asyncio ping implementation
 Home-page: https://github.com/stellarbit/aioping
+Download-URL: https://github.com/stellarbit/aioping/tarball/0.4.0
 Author: Anton Belousov
-Author-email: anton@stellarbit.com
-License: UNKNOWN
-Download-URL: https://github.com/stellarbit/aioping/tarball/0.3.1
-Description: UNKNOWN
+Author-email: anton@belousov.co
 Keywords: network,icmp,ping,asyncio
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE.txt
```


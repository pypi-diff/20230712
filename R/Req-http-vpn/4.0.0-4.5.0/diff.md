# Comparing `tmp/Req_http_vpn-4.0.0.tar.gz` & `tmp/Req_http_vpn-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Req_http_vpn-4.0.0.tar", last modified: Tue Jul 11 12:37:25 2023, max compression
+gzip compressed data, was "Req_http_vpn-4.5.0.tar", last modified: Wed Jul 12 16:29:02 2023, max compression
```

## Comparing `Req_http_vpn-4.0.0.tar` & `Req_http_vpn-4.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 12:37:25.853776 Req_http_vpn-4.0.0/
--rw-rw-rw-   0        0        0     1120 2023-07-10 19:36:20.000000 Req_http_vpn-4.0.0/LICENSE
--rw-rw-rw-   0        0        0     2129 2023-07-11 12:37:25.864777 Req_http_vpn-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2023-07-11 12:36:10.000000 Req_http_vpn-4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 12:37:25.719744 Req_http_vpn-4.0.0/Req_http_vpn.egg-info/
--rw-rw-rw-   0        0        0     2129 2023-07-11 12:37:25.000000 Req_http_vpn-4.0.0/Req_http_vpn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-07-11 12:37:25.000000 Req_http_vpn-4.0.0/Req_http_vpn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 12:37:25.000000 Req_http_vpn-4.0.0/Req_http_vpn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-11 12:37:25.000000 Req_http_vpn-4.0.0/Req_http_vpn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-11 12:37:25.000000 Req_http_vpn-4.0.0/Req_http_vpn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-11 12:37:25.847776 Req_http_vpn-4.0.0/Req_http_vpng/
--rw-rw-rw-   0        0        0     6418 2023-07-11 12:35:12.000000 Req_http_vpn-4.0.0/Req_http_vpng/Req_class.py
--rw-rw-rw-   0        0        0     1093 2023-07-11 12:34:38.000000 Req_http_vpn-4.0.0/Req_http_vpng/__init__.py
--rw-rw-rw-   0        0        0       81 2023-07-11 12:37:25.954808 Req_http_vpn-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0      969 2023-07-11 12:35:34.000000 Req_http_vpn-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:29:02.545611 Req_http_vpn-4.5.0/
+-rw-rw-rw-   0        0        0     1119 2023-07-12 16:27:50.000000 Req_http_vpn-4.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2122 2023-07-12 16:29:02.546612 Req_http_vpn-4.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1761 2023-07-12 16:24:56.000000 Req_http_vpn-4.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 16:29:02.400571 Req_http_vpn-4.5.0/Req_http_vpn/
+-rw-rw-rw-   0        0        0     8782 2023-07-12 16:21:00.000000 Req_http_vpn-4.5.0/Req_http_vpn/Req_class.py
+-rw-rw-rw-   0        0        0     1093 2023-07-11 12:34:38.000000 Req_http_vpn-4.5.0/Req_http_vpn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:29:02.541609 Req_http_vpn-4.5.0/Req_http_vpn.egg-info/
+-rw-rw-rw-   0        0        0     2122 2023-07-12 16:29:02.000000 Req_http_vpn-4.5.0/Req_http_vpn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-12 16:29:02.000000 Req_http_vpn-4.5.0/Req_http_vpn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:29:02.000000 Req_http_vpn-4.5.0/Req_http_vpn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-12 16:29:02.000000 Req_http_vpn-4.5.0/Req_http_vpn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 16:29:02.000000 Req_http_vpn-4.5.0/Req_http_vpn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       81 2023-07-12 16:29:02.554610 Req_http_vpn-4.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      967 2023-07-12 16:28:02.000000 Req_http_vpn-4.5.0/setup.py
```

### Comparing `Req_http_vpn-4.0.0/LICENSE` & `Req_http_vpn-4.5.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-MIT License
+IT License
 
 Copyright (c) 2023 Amin Rngbr
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `Req_http_vpn-4.0.0/PKG-INFO` & `Req_http_vpn-4.5.0/Req_http_vpn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Req_http_vpn
-Version: 4.0.0
+Name: Req-http-vpn
+Version: 4.5.0
 Summary: A simple and optimized library for sending HTTP requests to closed or filtered sites (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 License: LICENSE
 Keywords: http
 Description-Content-Type: text/markdown
@@ -24,15 +24,15 @@
 Basic GET usage:
 
 >>>   from Req_http_vpn import *
 >>>   from os import environ
 >>>   environ['print_access_request_library_Req_http_vpn'] = '0'
 >>>   this = Requests_filter('https://instagram.com')
 >>>   this = this.filter_req_GET()
->>>   print(this.get('status_code'))
+>>>   print(this.status_code)
    
 :Library used in the code: Requests
 :Copyright: (c) 2023 Amin Rngbr.
 :license: MIT
 
     ## Requests_filter Class
     The Req_http_vpn library is a simple library for sending **http** requests to websites that are **filtered and blocked** by governments.
```

### Comparing `Req_http_vpn-4.0.0/README.md` & `Req_http_vpn-4.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Basic GET usage:
 
 >>>   from Req_http_vpn import *
 >>>   from os import environ
 >>>   environ['print_access_request_library_Req_http_vpn'] = '0'
 >>>   this = Requests_filter('https://instagram.com')
 >>>   this = this.filter_req_GET()
->>>   print(this.get('status_code'))
+>>>   print(this.status_code)
    
 :Library used in the code: Requests
 :Copyright: (c) 2023 Amin Rngbr.
 :license: MIT
 
     ## Requests_filter Class
     The Req_http_vpn library is a simple library for sending **http** requests to websites that are **filtered and blocked** by governments.
```

### Comparing `Req_http_vpn-4.0.0/Req_http_vpn.egg-info/PKG-INFO` & `Req_http_vpn-4.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Req-http-vpn
-Version: 4.0.0
+Name: Req_http_vpn
+Version: 4.5.0
 Summary: A simple and optimized library for sending HTTP requests to closed or filtered sites (:
 Home-page: https://github.com/aminrngbr1122
 Author: Amin Rngbr
 Author-email: rngbramin@gmail.com
 License: LICENSE
 Keywords: http
 Description-Content-Type: text/markdown
@@ -24,15 +24,15 @@
 Basic GET usage:
 
 >>>   from Req_http_vpn import *
 >>>   from os import environ
 >>>   environ['print_access_request_library_Req_http_vpn'] = '0'
 >>>   this = Requests_filter('https://instagram.com')
 >>>   this = this.filter_req_GET()
->>>   print(this.get('status_code'))
+>>>   print(this.status_code)
    
 :Library used in the code: Requests
 :Copyright: (c) 2023 Amin Rngbr.
 :license: MIT
 
     ## Requests_filter Class
     The Req_http_vpn library is a simple library for sending **http** requests to websites that are **filtered and blocked** by governments.
```

### Comparing `Req_http_vpn-4.0.0/Req_http_vpng/__init__.py` & `Req_http_vpn-4.5.0/Req_http_vpn/__init__.py`

 * *Files identical despite different names*

### Comparing `Req_http_vpn-4.0.0/setup.py` & `Req_http_vpn-4.5.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import setuptools, os
 
 with open('README.md', "r") as f:
     long_description = f.read()
     
 print('Thank you for installing version 3 of this library ❤')
     
@@ -12,15 +11,15 @@
         if '__init__.py' in files:
             package_name = root.replace('/', '.').lstrip('.\\')
             ret.append(package_name)
     return ret
 
 setuptools.setup(
     name=f"Req_http_vpn",
-    version=f"4.0.0",
+    version=f"4.5.0",
     author=f"Amin Rngbr",
     author_email=f"rngbramin@gmail.com",
     description=f"A simple and optimized library for sending HTTP requests to closed or filtered sites (:",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='LICENSE',
     url=f"https://github.com/aminrngbr1122",
```


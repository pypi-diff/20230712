# Comparing `tmp/uddr_client-0.2.4.tar.gz` & `tmp/uddr_client-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uddr_client-0.2.4.tar", last modified: Wed Jun 28 20:59:38 2023, max compression
+gzip compressed data, was "uddr_client-0.2.5.tar", last modified: Wed Jul 12 18:11:09 2023, max compression
```

## Comparing `uddr_client-0.2.4.tar` & `uddr_client-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-28 20:59:38.929132 uddr_client-0.2.4/
--rw-r--r--   0 shane     (1000) shane     (1000)     1071 2023-06-14 04:19:49.000000 uddr_client-0.2.4/LICENSE.md
--rw-r--r--   0 shane     (1000) shane     (1000)     4191 2023-06-28 20:59:38.929132 uddr_client-0.2.4/PKG-INFO
--rw-r--r--   0 shane     (1000) shane     (1000)     3576 2023-06-22 21:56:00.000000 uddr_client-0.2.4/README.md
--rw-r--r--   0 shane     (1000) shane     (1000)       38 2023-06-28 20:59:38.929132 uddr_client-0.2.4/setup.cfg
--rw-r--r--   0 shane     (1000) shane     (1000)      952 2023-06-28 20:59:09.000000 uddr_client-0.2.4/setup.py
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-28 20:59:38.929132 uddr_client-0.2.4/src/
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-28 20:59:38.929132 uddr_client-0.2.4/src/uddr_client/
--rw-r--r--   0 shane     (1000) shane     (1000)       37 2023-06-09 19:52:19.000000 uddr_client-0.2.4/src/uddr_client/__init__.py
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-28 20:59:38.929132 uddr_client-0.2.4/src/uddr_client/api/
--rw-r--r--   0 shane     (1000) shane     (1000)       33 2023-06-22 21:56:00.000000 uddr_client-0.2.4/src/uddr_client/api/__init__.py
--rw-r--r--   0 shane     (1000) shane     (1000)    18903 2023-06-22 21:56:00.000000 uddr_client-0.2.4/src/uddr_client/api/api_client.py
--rw-r--r--   0 shane     (1000) shane     (1000)     2593 2023-06-22 21:56:00.000000 uddr_client-0.2.4/src/uddr_client/client.py
--rw-r--r--   0 shane     (1000) shane     (1000)     3065 2023-06-22 21:56:00.000000 uddr_client-0.2.4/src/uddr_client/connection.py
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-28 20:59:38.929132 uddr_client-0.2.4/src/uddr_client/doh/
--rw-r--r--   0 shane     (1000) shane     (1000)       33 2023-06-22 21:56:00.000000 uddr_client-0.2.4/src/uddr_client/doh/__init__.py
--rw-r--r--   0 shane     (1000) shane     (1000)     4755 2023-06-28 20:38:50.000000 uddr_client-0.2.4/src/uddr_client/doh/doh_client.py
--rw-r--r--   0 shane     (1000) shane     (1000)     1916 2023-06-28 20:57:11.000000 uddr_client-0.2.4/src/uddr_client/doh/ioc_parser.py
--rw-r--r--   0 shane     (1000) shane     (1000)     1481 2023-06-22 21:56:00.000000 uddr_client-0.2.4/src/uddr_client/response.py
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-28 20:59:38.929132 uddr_client-0.2.4/src/uddr_client.egg-info/
--rw-r--r--   0 shane     (1000) shane     (1000)     4191 2023-06-28 20:59:38.000000 uddr_client-0.2.4/src/uddr_client.egg-info/PKG-INFO
--rw-r--r--   0 shane     (1000) shane     (1000)      501 2023-06-28 20:59:38.000000 uddr_client-0.2.4/src/uddr_client.egg-info/SOURCES.txt
--rw-r--r--   0 shane     (1000) shane     (1000)        1 2023-06-28 20:59:38.000000 uddr_client-0.2.4/src/uddr_client.egg-info/dependency_links.txt
--rw-r--r--   0 shane     (1000) shane     (1000)       53 2023-06-28 20:59:38.000000 uddr_client-0.2.4/src/uddr_client.egg-info/requires.txt
--rw-r--r--   0 shane     (1000) shane     (1000)       12 2023-06-28 20:59:38.000000 uddr_client-0.2.4/src/uddr_client.egg-info/top_level.txt
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-07-12 18:11:09.443650 uddr_client-0.2.5/
+-rw-r--r--   0 shane     (1000) shane     (1000)     1071 2023-06-14 04:19:49.000000 uddr_client-0.2.5/LICENSE.md
+-rw-r--r--   0 shane     (1000) shane     (1000)     4152 2023-07-12 18:11:09.443650 uddr_client-0.2.5/PKG-INFO
+-rw-r--r--   0 shane     (1000) shane     (1000)     3537 2023-07-12 18:07:41.000000 uddr_client-0.2.5/README.md
+-rw-r--r--   0 shane     (1000) shane     (1000)       38 2023-07-12 18:11:09.443650 uddr_client-0.2.5/setup.cfg
+-rw-r--r--   0 shane     (1000) shane     (1000)      970 2023-07-12 18:08:05.000000 uddr_client-0.2.5/setup.py
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-07-12 18:11:09.433650 uddr_client-0.2.5/src/
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-07-12 18:11:09.433650 uddr_client-0.2.5/src/uddr_client/
+-rw-r--r--   0 shane     (1000) shane     (1000)       37 2023-06-09 19:52:19.000000 uddr_client-0.2.5/src/uddr_client/__init__.py
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-07-12 18:11:09.433650 uddr_client-0.2.5/src/uddr_client/api/
+-rw-r--r--   0 shane     (1000) shane     (1000)       33 2023-06-22 21:56:00.000000 uddr_client-0.2.5/src/uddr_client/api/__init__.py
+-rw-r--r--   0 shane     (1000) shane     (1000)    18903 2023-06-22 21:56:00.000000 uddr_client-0.2.5/src/uddr_client/api/api_client.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     2593 2023-06-22 21:56:00.000000 uddr_client-0.2.5/src/uddr_client/client.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     3065 2023-06-22 21:56:00.000000 uddr_client-0.2.5/src/uddr_client/connection.py
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-07-12 18:11:09.433650 uddr_client-0.2.5/src/uddr_client/doh/
+-rw-r--r--   0 shane     (1000) shane     (1000)       33 2023-06-22 21:56:00.000000 uddr_client-0.2.5/src/uddr_client/doh/__init__.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     4755 2023-06-28 20:38:50.000000 uddr_client-0.2.5/src/uddr_client/doh/doh_client.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     1916 2023-06-28 20:57:11.000000 uddr_client-0.2.5/src/uddr_client/doh/ioc_parser.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     1481 2023-06-22 21:56:00.000000 uddr_client-0.2.5/src/uddr_client/response.py
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-07-12 18:11:09.433650 uddr_client-0.2.5/src/uddr_client.egg-info/
+-rw-r--r--   0 shane     (1000) shane     (1000)     4152 2023-07-12 18:11:09.000000 uddr_client-0.2.5/src/uddr_client.egg-info/PKG-INFO
+-rw-r--r--   0 shane     (1000) shane     (1000)      501 2023-07-12 18:11:09.000000 uddr_client-0.2.5/src/uddr_client.egg-info/SOURCES.txt
+-rw-r--r--   0 shane     (1000) shane     (1000)        1 2023-07-12 18:11:09.000000 uddr_client-0.2.5/src/uddr_client.egg-info/dependency_links.txt
+-rw-r--r--   0 shane     (1000) shane     (1000)       70 2023-07-12 18:11:09.000000 uddr_client-0.2.5/src/uddr_client.egg-info/requires.txt
+-rw-r--r--   0 shane     (1000) shane     (1000)       12 2023-07-12 18:11:09.000000 uddr_client-0.2.5/src/uddr_client.egg-info/top_level.txt
```

### Comparing `uddr_client-0.2.4/LICENSE.md` & `uddr_client-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.4/PKG-INFO` & `uddr_client-0.2.5/src/uddr_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: uddr_client
-Version: 0.2.4
+Name: uddr-client
+Version: 0.2.5
 Summary: A Python client for the UDDR API.
 Home-page: https://github.com/sbarbett/uddr_client
 Author: Shane Barbetta
 Author-email: shane@barbetta.me
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -113,27 +113,27 @@
 doh.CAA    # For CAA records
 doh.DS     # For DS records
 doh.DNSKEY # For DNSKEY records
 ```
 
 ### Reverse Lookups
 
-If you pass an IP to the client, it will automatically perform a reverse lookup (PTR). IPv6 support hasn't been added yet.
+If you pass an IP to the client, it will automatically perform a reverse lookup (PTR).
 
 ### IoC Parsing
 
 This concept is borrowed from Michael Smith's [DDR-IOC-Checker](https://github.com/rybolov/DDR-IOC-Checker).
 
 Indicators of compromise passed to the DOHClient as a positional argument will be run through a parser. The parser accepts the following:
 
 1. Domain names
 2. URLs by means of stripping the protocol and path
 3. "Defanged" URLs which are intentionally obfuscated for security reasons
 4. Emails - the parser will remove the prefix and @
-5. IP addresses (not IPv6 yet)
+5. IP addresses
 
 ### Additional Methods
 
 The following methods return information about the DoH query or specific parts of the response.
 
 * `status()` - Returns an object with information about the status of the response. DoH provides a numerical code, this expands with a message and description.
 * `block_info()` - Returns a string stating whether the domain is blocked (by checking if the A record resolves to the UDDR block page).
@@ -141,12 +141,14 @@
 * `authority()` - Returns the authority section of the response, if one exists.
 
 ## Dependencies
 
 * pandas
 * xmltodict
 * python-decouple
+* requests
 
 ## License
 
 This project is licensed under the terms of the MIT license. See LICENSE.md for more details.
 
+
```

### Comparing `uddr_client-0.2.4/README.md` & `uddr_client-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,27 +94,27 @@
 doh.CAA    # For CAA records
 doh.DS     # For DS records
 doh.DNSKEY # For DNSKEY records
 ```
 
 ### Reverse Lookups
 
-If you pass an IP to the client, it will automatically perform a reverse lookup (PTR). IPv6 support hasn't been added yet.
+If you pass an IP to the client, it will automatically perform a reverse lookup (PTR).
 
 ### IoC Parsing
 
 This concept is borrowed from Michael Smith's [DDR-IOC-Checker](https://github.com/rybolov/DDR-IOC-Checker).
 
 Indicators of compromise passed to the DOHClient as a positional argument will be run through a parser. The parser accepts the following:
 
 1. Domain names
 2. URLs by means of stripping the protocol and path
 3. "Defanged" URLs which are intentionally obfuscated for security reasons
 4. Emails - the parser will remove the prefix and @
-5. IP addresses (not IPv6 yet)
+5. IP addresses
 
 ### Additional Methods
 
 The following methods return information about the DoH query or specific parts of the response.
 
 * `status()` - Returns an object with information about the status of the response. DoH provides a numerical code, this expands with a message and description.
 * `block_info()` - Returns a string stating whether the domain is blocked (by checking if the A record resolves to the UDDR block page).
@@ -122,11 +122,12 @@
 * `authority()` - Returns the authority section of the response, if one exists.
 
 ## Dependencies
 
 * pandas
 * xmltodict
 * python-decouple
+* requests
 
 ## License
 
-This project is licensed under the terms of the MIT license. See LICENSE.md for more details.
+This project is licensed under the terms of the MIT license. See LICENSE.md for more details.
```

### Comparing `uddr_client-0.2.4/setup.py` & `uddr_client-0.2.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="uddr_client", 
-    version="0.2.4",  
+    version="0.2.5",  
     description="A Python client for the UDDR API.", 
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown', 
     author="Shane Barbetta", 
     author_email="shane@barbetta.me",  
     url="https://github.com/sbarbett/uddr_client", 
     license="MIT", 
@@ -20,10 +20,11 @@
     ],
     package_dir={"": "src"},  
     packages=find_packages(where="src"),  
     python_requires=">=3.7", 
     install_requires=[
         "pandas>=2.0.2",
         "xmltodict>=0.13.0",
-	    "python-decouple>=3.8",
+	"python-decouple>=3.8",
+	"requests>=2.25.1",
     ],
 )
```

### Comparing `uddr_client-0.2.4/src/uddr_client/api/api_client.py` & `uddr_client-0.2.5/src/uddr_client/api/api_client.py`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.4/src/uddr_client/client.py` & `uddr_client-0.2.5/src/uddr_client/client.py`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.4/src/uddr_client/connection.py` & `uddr_client-0.2.5/src/uddr_client/connection.py`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.4/src/uddr_client/doh/doh_client.py` & `uddr_client-0.2.5/src/uddr_client/doh/doh_client.py`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.4/src/uddr_client/doh/ioc_parser.py` & `uddr_client-0.2.5/src/uddr_client/doh/ioc_parser.py`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.4/src/uddr_client/response.py` & `uddr_client-0.2.5/src/uddr_client/response.py`

 * *Files identical despite different names*

### Comparing `uddr_client-0.2.4/src/uddr_client.egg-info/PKG-INFO` & `uddr_client-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: uddr-client
-Version: 0.2.4
+Name: uddr_client
+Version: 0.2.5
 Summary: A Python client for the UDDR API.
 Home-page: https://github.com/sbarbett/uddr_client
 Author: Shane Barbetta
 Author-email: shane@barbetta.me
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -113,27 +113,27 @@
 doh.CAA    # For CAA records
 doh.DS     # For DS records
 doh.DNSKEY # For DNSKEY records
 ```
 
 ### Reverse Lookups
 
-If you pass an IP to the client, it will automatically perform a reverse lookup (PTR). IPv6 support hasn't been added yet.
+If you pass an IP to the client, it will automatically perform a reverse lookup (PTR).
 
 ### IoC Parsing
 
 This concept is borrowed from Michael Smith's [DDR-IOC-Checker](https://github.com/rybolov/DDR-IOC-Checker).
 
 Indicators of compromise passed to the DOHClient as a positional argument will be run through a parser. The parser accepts the following:
 
 1. Domain names
 2. URLs by means of stripping the protocol and path
 3. "Defanged" URLs which are intentionally obfuscated for security reasons
 4. Emails - the parser will remove the prefix and @
-5. IP addresses (not IPv6 yet)
+5. IP addresses
 
 ### Additional Methods
 
 The following methods return information about the DoH query or specific parts of the response.
 
 * `status()` - Returns an object with information about the status of the response. DoH provides a numerical code, this expands with a message and description.
 * `block_info()` - Returns a string stating whether the domain is blocked (by checking if the A record resolves to the UDDR block page).
@@ -141,12 +141,14 @@
 * `authority()` - Returns the authority section of the response, if one exists.
 
 ## Dependencies
 
 * pandas
 * xmltodict
 * python-decouple
+* requests
 
 ## License
 
 This project is licensed under the terms of the MIT license. See LICENSE.md for more details.
 
+
```


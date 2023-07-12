# Comparing `tmp/maci-0.3.1.tar.gz` & `tmp/maci-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maci-0.3.1.tar", last modified: Tue Jun 27 01:38:29 2023, max compression
+gzip compressed data, was "maci-0.4.0.tar", last modified: Wed Jul 12 05:42:09 2023, max compression
```

## Comparing `maci-0.3.1.tar` & `maci-0.4.0.tar`

### file list

```diff
@@ -1,60 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.544375 maci-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-27 01:38:17.000000 maci-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-27 01:38:29.544375 maci-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-06-27 01:38:29.000000 maci-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.532374 maci-0.3.1/maci/
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-27 01:38:29.000000 maci-0.3.1/maci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.536374 maci-0.3.1/maci/_hash/
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_hash/comparefilehash.py
--rw-r--r--   0 runner    (1001) docker     (122)     3736 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_hash/createfilehash.py
--rw-r--r--   0 runner    (1001) docker     (122)     3336 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_hash/createhash.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.536374 maci-0.3.1/maci/_ini/
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_ini/inibuildauto.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_ini/inibuildmanual.py
--rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_ini/inidump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_ini/iniload.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.536374 maci-0.3.1/maci/_json/
--rw-r--r--   0 runner    (1001) docker     (122)     2531 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_json/jsondump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_json/jsondumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1670 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_json/jsonload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_json/jsonloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.540374 maci-0.3.1/maci/_native/
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     2316 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/cleanformat.py
--rw-r--r--   0 runner    (1001) docker     (122)     7191 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/dump.py
--rw-r--r--   0 runner    (1001) docker     (122)     4417 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/dumpraw.py
--rw-r--r--   0 runner    (1001) docker     (122)     6484 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/dumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3633 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/load.py
--rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/loadattrs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4175 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/loaddict.py
--rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/loadraw.py
--rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/loadstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_native/loadstrdict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.540374 maci-0.3.1/maci/_toml/
--rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_toml/tomldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_toml/tomldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_toml/tomlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_toml/tomlloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.540374 maci-0.3.1/maci/_xml/
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_xml/xmlbuildmanual.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_xml/xmldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_xml/xmldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1720 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_xml/xmlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_xml/xmlloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.544375 maci-0.3.1/maci/_yaml/
--rw-r--r--   0 runner    (1001) docker     (122)     2062 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_yaml/yamldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_yaml/yamldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_yaml/yamlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-06-27 01:38:29.000000 maci-0.3.1/maci/_yaml/yamlloadstr.py
--rw-r--r--   0 runner    (1001) docker     (122)    71589 2023-06-27 01:38:29.000000 maci-0.3.1/maci/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2981 2023-06-27 01:38:29.000000 maci-0.3.1/maci/error.py
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-06-27 01:38:29.000000 maci-0.3.1/maci/hint.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.000000 maci-0.3.1/maci/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 01:38:29.536374 maci-0.3.1/maci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-06-27 01:38:29.000000 maci-0.3.1/maci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1121 2023-06-27 01:38:29.000000 maci-0.3.1/maci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 01:38:29.000000 maci-0.3.1/maci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-06-27 01:38:29.000000 maci-0.3.1/maci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-27 01:38:29.000000 maci-0.3.1/maci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1384 2023-06-27 01:38:29.544375 maci-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-06-27 01:38:17.000000 maci-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-12 05:41:56.000000 maci-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-12 05:42:09.724157 maci-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-07-12 05:42:09.000000 maci-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.720157 maci-0.4.0/maci/
+-rw-r--r--   0 runner    (1001) docker     (122)     3371 2023-07-12 05:42:09.000000 maci-0.4.0/maci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22827 2023-07-12 05:42:09.000000 maci-0.4.0/maci/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.720157 maci-0.4.0/maci/_hash/
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_hash/comparefilehash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3868 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_hash/createfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_hash/createhash.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.720157 maci-0.4.0/maci/_ini/
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_ini/inibuildauto.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_ini/inibuildmanual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_ini/inidump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_ini/iniload.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/maci/_json/
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_json/jsondump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_json/jsondumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_json/jsonload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_json/jsonloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/maci/_native/
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/cleanformat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6838 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/dump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4376 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/dumpraw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6134 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/dumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/loadattrs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/loaddict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/loadraw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2591 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/loadstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_native/loadstrdict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/maci/_toml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_toml/tomldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_toml/tomldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_toml/tomlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_toml/tomlloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/maci/_xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_xml/xmlbuildmanual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_xml/xmldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_xml/xmldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_xml/xmlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_xml/xmlloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/maci/_yaml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_yaml/yamldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_yaml/yamldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_yaml/yamlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-07-12 05:42:09.000000 maci-0.4.0/maci/_yaml/yamlloadstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    73096 2023-07-12 05:42:09.000000 maci-0.4.0/maci/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7311 2023-07-12 05:42:09.000000 maci-0.4.0/maci/data.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-12 05:42:09.000000 maci-0.4.0/maci/error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.720157 maci-0.4.0/maci/ext/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.724157 maci-0.4.0/maci/ext/defusedxml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-07-12 05:42:09.000000 maci-0.4.0/maci/ext/defusedxml/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-12 05:42:09.000000 maci-0.4.0/maci/hint.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.000000 maci-0.4.0/maci/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 05:42:09.720157 maci-0.4.0/maci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-12 05:42:09.000000 maci-0.4.0/maci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1185 2023-07-12 05:42:09.000000 maci-0.4.0/maci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 05:42:09.000000 maci-0.4.0/maci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-12 05:42:09.000000 maci-0.4.0/maci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-12 05:42:09.000000 maci-0.4.0/maci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-07-12 05:42:09.728157 maci-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-12 05:41:56.000000 maci-0.4.0/setup.py
```

### Comparing `maci-0.3.1/PKG-INFO` & `maci-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maci
-Version: 0.3.1
+Version: 0.4.0
 Summary: The easy to use library for your data, configuration, and save files
 Author: aaronater10
 Author-email: dev_admin@dunnts.com
 License: MIT
 Project-URL: Docs, https://docs.macilib.org
 Project-URL: Code, https://github.com/aaronater10/maci
 Project-URL: Bugs, https://github.com/aaronater10/maci/issues
@@ -23,15 +23,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.3.1
+##### Latest Version: 0.4.0
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.3.1/README.md` & `maci-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.3.1
+##### Latest Version: 0.4.0
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.3.1/maci/__init__.py` & `maci-0.4.0/maci/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 """
 maci - by aaronater10
 
-Version 0.3.1
+A Pythonic Configuration Language & Thin Wrapper Library
 
-The easy to use library for your data, configuration, and save files.
+Version 0.4.0
 
-Import or Export custom, or industry-common, data, config, and save files easily for
-your python program or script!
+Tutorials and docs: https://docs.macilib.org
 
-See tutorials and docs here for more info: https://docs.macilib.org
-
-Source Code: https://github.com/aaronater10/maci
+Source: https://github.com/aaronater10/maci
 """
-__version__ = '0.3.1'
+__version__ = '0.4.0'
 
 #########################################################################################################
 # Imports
 
-# Base Exceptions
+# Exceptions
 from . import error
 
 # Hints
 from . import hint
 
 # Native Lib
 from ._native.load import load
@@ -62,14 +59,15 @@
 # INI Lib
 from ._ini.iniload import iniload
 from ._ini.inidump import inidump
 from ._ini.inibuildauto import inibuildauto
 from ._ini.inibuildmanual import inibuildmanual
 
 # XML Lib
+from defusedxml import defuse_stdlib as _defuse_xml_stdlib
 from ._xml.xmlload import xmlload
 from ._xml.xmlloadstr import xmlloadstr
 from ._xml.xmldump import xmldump
 from ._xml.xmldumpstr import xmldumpstr
 from ._xml.xmlbuildmanual import xmlbuildmanual
```

### Comparing `maci-0.3.1/maci/_hash/comparefilehash.py` & `maci-0.4.0/maci/_hash/comparefilehash.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,24 +27,24 @@
 
     This is using the hashlib library shipped with the python standard library. For more
     information on hashlib, visit: https://docs.python.org/3/library/hashlib.html
     """
     ALGO_OPTIONS = ('sha256', 'sha512', 'sha384', 'sha1', 'md5')
 
     # Error checks
-    _err_msg_str_file_src = f"Only str is allowed for file_to_hash"
-    _err_msg_hash_file = f"Only str is allowed for stored_hash_file"
-    _err_msg_str_hash = f"Only str is allowed for hash_algorithm"
-    _err_msg_hash = f"Invalid or no hash option chosen for hash_algorithm"
+    err_msg_str_file_src = f"Only str is allowed for 'file_to_hash'"
+    err_msg_hash_file = f"Only str is allowed for 'stored_hash_file'"
+    err_msg_str_hash = f"Only str is allowed for 'hash_algorithm'"
+    err_msg_hash = f"Invalid or no hash option chosen for 'hash_algorithm'"
     err_msg_str_encoding = f"Only str|None or valid option is allowed for 'encoding'"
 
-    if not isinstance(file_to_hash, str): raise CompareFileHash(_err_msg_str_file_src, f'"{file_to_hash}"')
-    if not isinstance(stored_hash_file, str): raise CompareFileHash(_err_msg_hash_file, f'"{stored_hash_file}"')
-    if not isinstance(hash_algorithm, str): raise CompareFileHash(_err_msg_str_hash, f'"{hash_algorithm}"')
-    if not hash_algorithm in ALGO_OPTIONS: raise CompareFileHash(_err_msg_hash, f'"{hash_algorithm}"')
+    if not isinstance(file_to_hash, str): raise CompareFileHash(err_msg_str_file_src, f'"{file_to_hash}"')
+    if not isinstance(stored_hash_file, str): raise CompareFileHash(err_msg_hash_file, f'"{stored_hash_file}"')
+    if not isinstance(hash_algorithm, str): raise CompareFileHash(err_msg_str_hash, f'"{hash_algorithm}"')
+    if not hash_algorithm in ALGO_OPTIONS: raise CompareFileHash(err_msg_hash, f'"{hash_algorithm}"')
     if not isinstance(encoding, (str, type(None))): raise CompareFileHash(err_msg_str_encoding, f'\nGot: {repr(encoding)}')
 
     # Collect hash data, then return result
     try: _hash_data = _createfilehash(file_to_hash, None, hash_algorithm, encoding=encoding)
     except CreateFileHash as err_msg: raise CompareFileHash(err_msg)
 
     try:
```

### Comparing `maci-0.3.1/maci/_hash/createfilehash.py` & `maci-0.4.0/maci/_hash/createfilehash.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,33 +30,33 @@
 
     This is using the hashlib library shipped with the python standard library. For more
     information on hashlib, visit: https://docs.python.org/3/library/hashlib.html
     """
     ALGO_OPTIONS = ('sha256', 'sha512', 'sha384', 'sha1', 'md5')
 
     # Error checks
-    _err_msg_str_file_src = f"Only str is allowed for file_to_hash"
-    _err_msg_file_dst = f"Only str|None is allowed for file_to_store_hash"
-    _err_msg_str_hash = f"Only str is allowed for hash_algorithm"
-    _err_msg_hash = f"Invalid or no hash option chosen for hash_algorithm"
+    err_msg_str_file_src = f"Only str is allowed for 'file_to_hash'"
+    err_msg_file_dst = f"Only str|None is allowed for 'file_to_store_hash'"
+    err_msg_str_hash = f"Only str is allowed for 'hash_algorithm'"
+    err_msg_hash = f"Invalid or no hash option chosen for 'hash_algorithm'"
     err_msg_str_encoding = f"Only str|None or valid option is allowed for 'encoding'"
 
-    if not isinstance(file_to_hash, str): raise CreateFileHash(_err_msg_str_file_src, f'"{file_to_hash}"')
-    if not isinstance(file_to_store_hash, (str, type(None))): raise CreateFileHash(_err_msg_file_dst, f'"{file_to_store_hash}"')
-    if not isinstance(hash_algorithm, str): raise CreateFileHash(_err_msg_str_hash, f'"{hash_algorithm}"')
-    if not hash_algorithm in ALGO_OPTIONS: raise CreateFileHash(_err_msg_hash, f'"{hash_algorithm}"')
+    if not isinstance(file_to_hash, str): raise CreateFileHash(err_msg_str_file_src, f'"{file_to_hash}"')
+    if not isinstance(file_to_store_hash, (str, type(None))): raise CreateFileHash(err_msg_file_dst, f'"{file_to_store_hash}"')
+    if not isinstance(hash_algorithm, str): raise CreateFileHash(err_msg_str_hash, f'"{hash_algorithm}"')
+    if not hash_algorithm in ALGO_OPTIONS: raise CreateFileHash(err_msg_hash, f'"{hash_algorithm}"')
     if not isinstance(encoding, (str, type(None))): raise CreateFileHash(err_msg_str_encoding, f'\nGot: {repr(encoding)}')
 
     # Generate Hash Type
     _hash_type: _Any  # ignore type checker
     if hash_algorithm == ALGO_OPTIONS[0]: _hash_type = _hashlib.sha256() # sha256
     if hash_algorithm == ALGO_OPTIONS[1]: _hash_type = _hashlib.sha512() # sha512
     if hash_algorithm == ALGO_OPTIONS[2]: _hash_type = _hashlib.sha384() # sha384
-    if hash_algorithm == ALGO_OPTIONS[3]: _hash_type = _hashlib.sha1() # sha1
-    if hash_algorithm == ALGO_OPTIONS[4]: _hash_type = _hashlib.md5() # md5
+    if hash_algorithm == ALGO_OPTIONS[3]: _hash_type = _hashlib.sha1() # sha1  # nosec: B303, B324  # ignore sec checker - up to dev discretion
+    if hash_algorithm == ALGO_OPTIONS[4]: _hash_type = _hashlib.md5() # md5  # nosec: B303, B324  # ignore sec checker - up to dev discretion
 
     # Read source file data and update hash
     _readbytes: _Any  # ignore type checker
     try: _readbytes = _loadraw(file_to_hash)
     except LoadRaw as err_msg: raise CreateFileHash(err_msg)
 
     try: _readbytes = _readbytes.encode() if encoding is None else _readbytes.encode(encoding=encoding)
```

### Comparing `maci-0.3.1/maci/_hash/createhash.py` & `maci-0.4.0/maci/_hash/createhash.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     This is using the hashlib library shipped with the python standard library. For more
     information on hashlib, visit: https://docs.python.org/3/library/hashlib.html
     """
     ALGO_OPTIONS = ('sha256', 'sha512', 'sha384', 'sha1', 'md5')
 
     # Error checks
-    err_msg_data = f"Only str | bytes | int | List[int] | Tuple[int] | Set[int] | range | bool is allowed for 'data_to_hash'"
+    err_msg_data = f"Only str|bytes|int|List[int]|Tuple[int]|Set[int]|range|bool is allowed for 'data_to_hash'"
     err_msg_str_hash = f"Only str is allowed for 'hash_algorithm'"
     err_msg_hash = f"Invalid hash option chosen for 'hash_algorithm'. Valid options: 'sha256', 'sha512', 'sha384', 'sha1', 'md5'"
     err_msg_str_encoding = f"Only str or valid option is allowed for 'encoding'"
 
     # Check Types
     valid_types_to_hash = (str, bytes, int, list, tuple, set, range, bool)
     valid_seq_of_int_types = (list, tuple, set, range)
@@ -49,16 +49,16 @@
     if not isinstance(hash_algorithm, str): raise CreateHash(err_msg_str_hash, f'\nGot: {repr(hash_algorithm)}')
     if not hash_algorithm in ALGO_OPTIONS: raise CreateHash(err_msg_hash, f'\nGot: {repr(hash_algorithm)}')
 
     # Generate Hash Type
     if hash_algorithm == ALGO_OPTIONS[0]: hash_type = _hashlib.sha256() # sha256
     if hash_algorithm == ALGO_OPTIONS[1]: hash_type = _hashlib.sha512() # sha512
     if hash_algorithm == ALGO_OPTIONS[2]: hash_type = _hashlib.sha384() # sha384
-    if hash_algorithm == ALGO_OPTIONS[3]: hash_type = _hashlib.sha1() # sha1
-    if hash_algorithm == ALGO_OPTIONS[4]: hash_type = _hashlib.md5() # md5
+    if hash_algorithm == ALGO_OPTIONS[3]: hash_type = _hashlib.sha1() # sha1  # nosec: B303, B324  # ignore sec checker - up to dev discretion
+    if hash_algorithm == ALGO_OPTIONS[4]: hash_type = _hashlib.md5() # md5  # nosec: B303, B324  # ignore sec checker - up to dev discretion
 
     # Check and Convert data to bytes and update hash
     try: 
         if isinstance(data_to_hash, str): byte_data = data_to_hash.encode(encoding=encoding)
     except LookupError: raise CreateHash(err_msg_str_encoding, f'\nGot: {repr(encoding)}')
 
     if isinstance(data_to_hash, bytes): byte_data = data_to_hash
```

### Comparing `maci-0.3.1/maci/_ini/inibuildauto.py` & `maci-0.4.0/maci/_ini/inibuildauto.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,24 +30,24 @@
 
     This is using the native configparser library shipped with the python standard library. Using ConfigParser method
     with ExtendedInterpolation enabled by default. For more information on the configparser library, 
     visit: https://docs.python.org/3/library/configparser.html
     """
     # Error Checks
     err_msg_dict_type = f"Only dict is allowed for 'data'"
-    err_msg_dict_struct = "Please send correct dict structure"
+    err_msg_dict_struct = r"Please use correct dict structure: {'k':{'k':v}} "
 
-    if not isinstance(data, dict): raise IniBuildAuto(err_msg_dict_type, f'\nGOT: {repr(data)}')
+    if not isinstance(data, dict): raise IniBuildAuto(err_msg_dict_type, f'\nGot: {repr(data)}')
 
 
     # Auto Build INI data structure
     __ini_data = _ConfigParser(interpolation=_ExtendedInterpolation())
 
     try:
         for section,dict_value in data.items():
             if None in dict_value.values():
                 for sub_key,sub_value in dict_value.items():
                     if sub_value is None: # pragma: no branch
                         dict_value[sub_key] = 'None'
             __ini_data[section] = dict_value
         return __ini_data
-    except AttributeError as __err_msg: raise IniBuildAuto(f'{__err_msg} - {err_msg_dict_struct}', f'\nGOT: {repr(data)}')
+    except AttributeError as __err_msg: raise IniBuildAuto(f'{__err_msg} - {err_msg_dict_struct}', f'\nGot: {repr(data)}')
```

### Comparing `maci-0.3.1/maci/_ini/inibuildmanual.py` & `maci-0.4.0/maci/_ini/inibuildmanual.py`

 * *Files identical despite different names*

### Comparing `maci-0.3.1/maci/_ini/inidump.py` & `maci-0.4.0/maci/_ini/inidump.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 # Imports
 from configparser import ConfigParser as _ConfigParser
 from typing import Union as _Union
 from ..error import IniDump
 
 #########################################################################################################
 # Export ini file
-def inidump(filename: str, ini_data: _ConfigParser, *, append: bool=False, encoding: _Union[str, None]=None) -> None:
+def inidump(filename: str, data: _ConfigParser, *, append: bool=False, encoding: _Union[str, None]=None) -> None:
     """
     Exports a new file from a ini data (ConfigParser) obj
 
     Enter new filename as str. Pass ini data for output to file
     
     [Example Use]
 
-    inidump('path/to/filename.ini', ini_data)
+    inidump('path/to/filename.ini', data)
 
     This is using the native configparser library shipped with the python standard library. Using ConfigParser method.
     For more information on the configparser library, visit: https://docs.python.org/3/library/configparser.html
     """
     # Error Checks
     err_msg_file_type = "Only str is allowed for 'filename'"
-    err_msg_parser = "Only ConfigParser is allowed for 'ini_data'"
+    err_msg_parser = "Only ConfigParser is allowed for 'data'"
     err_msg_type_append = "Only bool is allowed for 'append'"
     err_msg_type_encoding = "Only str|None or valid option is allowed for 'encoding'"
 
     if not isinstance(filename, str): raise IniDump(err_msg_file_type, f'\nGot: {repr(filename)}')
-    if not isinstance(ini_data, _ConfigParser): raise IniDump(err_msg_parser, f'\nGot: {repr(ini_data)}')
+    if not isinstance(data, _ConfigParser): raise IniDump(err_msg_parser, f'\nGot: {repr(data)}')
     if not isinstance(append, bool): raise IniDump(err_msg_type_append, f'\nGot: {repr(append)}')
     if not isinstance(encoding, (str, type(None))): raise IniDump(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
 
     # Set Write Mode: 'a' = append, 'w' = write
     write_mode = 'a' if append else 'w'
 
     # Write Ini Data
     try:
         with open(filename, write_mode, encoding=encoding) as f:
-            ini_data.write(f)
-    except (FileNotFoundError, OSError) as _err_msg: raise IniDump(_err_msg, f'\nFILE: "{filename}"')
+            data.write(f)
+    except (FileNotFoundError, OSError) as _err_msg: raise IniDump(_err_msg, f'\nGot: {repr(filename)}')
     except LookupError: raise IniDump(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
```

### Comparing `maci-0.3.1/maci/_ini/iniload.py` & `maci-0.4.0/maci/_ini/iniload.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,13 +30,13 @@
 
     if not isinstance(filename, str): raise IniLoad(err_msg_file_type, f'\nGot: {repr(filename)}')
     if not isinstance(encoding, (str, type(None))): raise IniLoad(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
 
     # Load file data
     try:
         with open(filename, 'r', encoding=encoding): pass
-    except (FileNotFoundError, OSError) as _err_msg: raise IniLoad(_err_msg, f'\nFILE: "{filename}"')
+    except (FileNotFoundError, OSError) as _err_msg: raise IniLoad(_err_msg, f'\nGot: {repr(filename)}')
     except LookupError: raise IniLoad(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
 
     _parser = _ConfigParser(interpolation=_ExtendedInterpolation())
     _parser.read(filename, encoding=encoding)
     return _parser
```

### Comparing `maci-0.3.1/maci/_json/jsondump.py` & `maci-0.4.0/maci/_json/jsondump.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # jsondump
 #########################################################################################################
 # Imports
-import json as __json
-from ..error import JsonDump
+import json as _json
 from .._native.dumpraw import dumpraw as _dumpraw
-from typing import Union
+from typing import Union as _Union
+from ..error import JsonDump
 
 #########################################################################################################
 # Export json file
 def jsondump(
     filename: str,
-    data: Union[dict, list, tuple, str, int, float, bool, None],
+    data: _Union[dict, list, tuple, str, int, float, bool, None],
     *,
     append: bool=False,
     indent_level: int=4,
-    encoding: Union[str, None]=None
+    encoding: _Union[str, None]=None
 ) -> None:
     """
     Exports a new file from python data type to json data.
     
     Enter new filename as str. Pass data for output to file
     
     [Example Use]
@@ -44,12 +44,12 @@
 
     # Set Write Mode: 'a' = append, 'w' = write
     write_mode = 'a' if append else 'w'
 
     try:
         # Export data to json file
         with open(filename, write_mode, encoding=encoding) as f:
-            __json.dump(data, f, indent=indent_level)
+            _json.dump(data, f, indent=indent_level)
             if write_mode == 'a': _dumpraw(filename, '', append=True)
-    except TypeError as __err_msg: raise JsonDump(__err_msg, f'\nDATA: {repr(data)}')
-    except (FileNotFoundError, OSError) as __err_msg: raise JsonDump(__err_msg, f'\nGOT: "{filename}"')
+    except TypeError as __err_msg: raise JsonDump(__err_msg, f'\nGot: {repr(data)}')
+    except (FileNotFoundError, OSError) as __err_msg: raise JsonDump(__err_msg, f'\nGot: {repr(filename)}')
     except LookupError: raise JsonDump(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
```

### Comparing `maci-0.3.1/maci/_json/jsondumpstr.py` & `maci-0.4.0/maci/_json/jsondumpstr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # jsondumpstr
 #########################################################################################################
 # Imports
-import json as __json
+import json as _json
+from typing import Union as _Union
 from ..error import JsonDumpStr
-from typing import Union
 
 #########################################################################################################
 # Export json str
-def jsondumpstr(data: Union[dict, list, tuple, str, int, float, bool, None], *, indent_level: int=4) -> str:
+def jsondumpstr(data: _Union[dict, list, tuple, str, int, float, bool, None], *, indent_level: int=4) -> str:
     """
     Exports python data type to json string
 
     Returns a json formatted str. Assign the output to var
 
     [Example Use]
 
@@ -26,9 +26,9 @@
     err_msg_type_indent = "Only int is allowed for 'indent_level'"
 
     if not isinstance(data, (list, dict, tuple, str, int, float, bool, type(None))): raise JsonDumpStr(err_msg_type_data, f'\nGot: {repr(data)}')
     if not isinstance(indent_level, int): raise JsonDumpStr(err_msg_type_indent, f'\nGot: {repr(indent_level)}')
 
     try:
         # Export dict data to json string
-        return __json.dumps(data, indent=indent_level)
+        return _json.dumps(data, indent=indent_level)
     except TypeError as __err_msg: raise JsonDumpStr(__err_msg, f'\nGot: {data} \nINDENT_LEVEL: {indent_level}')
```

### Comparing `maci-0.3.1/maci/_json/jsonload.py` & `maci-0.4.0/maci/_json/jsonload.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # jsonload
 #########################################################################################################
 # Imports
-import json as __json
+import json as _json
+from typing import Union as _Union
 from ..error import JsonLoad
-from typing import Union
 
 #########################################################################################################
 # Import json file
-def jsonload(filename: str, *, encoding: Union[str, None]=None) -> Union[list, dict, str, int, float, bool, None]:
+def jsonload(filename: str, *, encoding: _Union[str, None]=None) -> _Union[list, dict, str, int, float, bool, None]:
     """
     Imports json data from a file
 
     Returns data with matching python data type. Assign the output to var
 
     Enter json file location as str to import.
 
@@ -29,11 +29,11 @@
     if not isinstance(filename, str): raise JsonLoad(err_msg_file_type, f'\nGot: {repr(filename)}')
     if not isinstance(encoding, (str, type(None))): raise JsonLoad(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
 
 
     # Import json file
     try:
         with open(filename, 'r', encoding=encoding) as f:
-            return __json.load(f)
-    except (FileNotFoundError, OSError) as __err_msg: raise JsonLoad(__err_msg, f'\nFILE: "{filename}"')
-    except __json.decoder.JSONDecodeError as __err_msg: raise JsonLoad(__err_msg, f'\nFILE: "{filename}"')
+            return _json.load(f)
+    except (FileNotFoundError, OSError) as __err_msg: raise JsonLoad(__err_msg, f'\nGot: {repr(filename)}')
+    except _json.decoder.JSONDecodeError as __err_msg: raise JsonLoad(__err_msg, f'\nGot: {repr(filename)}')
     except LookupError: raise JsonLoad(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
```

### Comparing `maci-0.3.1/maci/_json/jsonloadstr.py` & `maci-0.4.0/maci/_json/jsonloadstr.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # jsonloadstr
 #########################################################################################################
 # Imports
-import json as __json
+import json as _json
+from typing import Union as _Union
 from ..error import JsonLoadStr
-from typing import Union
 
 #########################################################################################################
 # Import json string
-def jsonloadstr(json_str_data: str) -> Union[list, dict, str, int, float, bool, None]:
+def jsonloadstr(json_str_data: str) -> _Union[list, dict, str, int, float, bool, None]:
     """
     Imports json data from a string
 
     Returns data with matching python data type. Assign the output to var
 
     Enter json string as str to import.
 
@@ -19,15 +19,15 @@
 
     jsonloadstr('string with json data')
 
     This is using the native json library shipped with the python standard library. For more
     information on the json library, visit: https://docs.python.org/3/library/json.html
     """
     # Error Checks
-    err_msg_data_type = "Only str is allowed for 'data'"
+    err_msg_data_type = "Only str is allowed for 'json_str_data'"
 
     if not isinstance(json_str_data, str): raise JsonLoadStr(err_msg_data_type, f'\nGot: {repr(json_str_data)}')
 
     # Import json string    
     try:
-        return __json.loads(json_str_data)
-    except __json.decoder.JSONDecodeError as __err_msg: raise JsonLoadStr(__err_msg, f'\nGot: {json_str_data}')
+        return _json.loads(json_str_data)
+    except _json.decoder.JSONDecodeError as __err_msg: raise JsonLoadStr(__err_msg, f'\nGot: {json_str_data}')
```

### Comparing `maci-0.3.1/maci/_native/build.py` & `maci-0.4.0/maci/_native/build.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # build
 #########################################################################################################
 # Imports
 from typing import Any as _Any
-from ..data import MaciDataObj
+from ..data import MaciDataObj as _MaciDataObj
 
 #########################################################################################################
 # Build manual MaciDataObj (python data)
-def build() -> 'MaciDataObj':
+def build() -> '_MaciDataObj':
     """
     Returns an empty MaciDataObj obj to manually build pythonic data with maci features
     
     Assign the output to var
 
     Literally, just use attribute assignment as you normally would
 
@@ -20,20 +20,20 @@
 
     object.attribute2 = 'string data'
 
     More information on object features: https://docs.macilib.org/docs/tools/build-data/python-data-build
     """
     # Syntax/Usage Error Messages
     err_messages: _Any = {  # ignore type checker
-        '_py_syntax_err_msg': "Must have valid Python data types to import, or syntax is not formatted correctly",
+        '_py_syntax_err_msg': "Must have valid Python data types to import, or maci syntax is incorrect",
         '_name_preexists_err_msg': "Name already preexists. Must give unique attribute names",
-        '_name_reference_does_not_exist_msg': "Name reference does not exist! Must reference attribute names that have been defined",
+        '_name_reference_does_not_exist_msg': "Map name does not exist! Must map attribute names that have been defined",
         '_assignment_locked_atrribs_err_msg': "Attribute Name Locked! Cannot be reassigned",
         '_assignment_hard_locked_atrribs_err_msg': "Attribute Name Hard Locked! Cannot be reassigned, deleted, or unlocked"
     }
-    return MaciDataObj(
+    return _MaciDataObj(
                 '',
                 attr_name_dedup=True,
                 _is_build_request=True,
                 encoding=None,
                 **err_messages,
             )
```

### Comparing `maci-0.3.1/maci/_native/cleanformat.py` & `maci-0.4.0/maci/_native/cleanformat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # cleanformat
 #########################################################################################################
 # Imports
-from typing import Union as __Union
+from typing import Union as _Union
 from ..error import CleanFormat
 
 #########################################################################################################
 # Format/Prep Dictionary, List, Tuple, or Set Data for Export
-def cleanformat(data: __Union[dict,list,tuple,set], indent_level: int=1) -> str:
+def cleanformat(data: _Union[dict,list,tuple,set], indent_level: int=1) -> str:
     """
     Formats a (single) dictionary, list, tuple, or set, to have a clean multiline output for exporting to a file.
 
     Returned output will be a str
 
     Note: Higher indent levels will decrease performance. Indentation is applied to the main data set only.
 
@@ -18,49 +18,49 @@
 
     Accepted data types: dict, list, tuple, set 
 
     [Example Use]
     
     var = cleanformat(data)
     """
-    __err_type = "Only dict|list|tuple|set is allowed for 'data'"
-    __err_indent = "Only int is allowed for 'indent_level'"
+    err_type = "Only dict|list|tuple|set is allowed for 'data'"
+    err_indent = "Only int is allowed for 'indent_level'"
 
     # Error Checks, Set indent level
     if not isinstance(indent_level, int):
-        raise CleanFormat(__err_indent, f'\nGot: {repr(indent_level)}')
+        raise CleanFormat(err_indent, f'\nGot: {repr(indent_level)}')
     indent_level = '    '*indent_level
 
     if not isinstance(data, (dict,list,tuple,set)):
-        raise CleanFormat(__err_type, f'\nGot: {repr(data)}')
+        raise CleanFormat(err_type, f'\nGot: {repr(data)}')
 
 
     # Format Data Type and Return as str
-    __build_data = ""
+    build_data = ""
 
     # Dict
     if isinstance(data, dict):
         for key,value in data.items():
-            __build_data += f"\n{indent_level}{repr(key)}: {repr(value)},"
-        __build_data = f"{{{__build_data}\n}}"
-        return __build_data
+            build_data += f"\n{indent_level}{repr(key)}: {repr(value)},"
+        build_data = f"{{{build_data}\n}}"
+        return build_data
 
     # List
     if isinstance(data, list):
         for value in data:
-            __build_data += f"\n{indent_level}{repr(value)},"
-        __build_data = f"[{__build_data}\n]"
-        return __build_data
+            build_data += f"\n{indent_level}{repr(value)},"
+        build_data = f"[{build_data}\n]"
+        return build_data
 
     # Tuple
     if isinstance(data, tuple):
         for value in data:
-            __build_data += f"\n{indent_level}{repr(value)},"
-        __build_data = f"({__build_data}\n)"
-        return __build_data
+            build_data += f"\n{indent_level}{repr(value)},"
+        build_data = f"({build_data}\n)"
+        return build_data
 
     # Set
     if isinstance(data, set): # pragma: no branch
         for value in data:
-            __build_data += f"\n{indent_level}{repr(value)},"
-        __build_data = f"{{{__build_data}\n}}"
-        return __build_data
+            build_data += f"\n{indent_level}{repr(value)},"
+        build_data = f"{{{build_data}\n}}"
+        return build_data
```

### Comparing `maci-0.3.1/maci/_native/dump.py` & `maci-0.4.0/maci/_native/dump.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # dump
 #########################################################################################################
 # Imports
-from typing import Union as __Union
-from typing import NewType as __NewType
+from typing import Union as _Union
+from typing import NewType as _NewType
 from typing import Any as _Any
 from ..error import Dump
 from ..data import __dump_data
-from ..data import MaciDataObj as __MaciDataObj
+from ..data import MaciDataObj as _MaciDataObj
+from ..hint import __ClassObject
 
 #########################################################################################################
 # Dump Data to File
-
-# Hinting reference name for "CustomClass" to denote a CustomClass can be used to dump data
-CustomClass = __NewType('CustomClass', object)
-
 def dump(
     filename: str, 
-    data: __Union['__MaciDataObj', dict, CustomClass], 
+    data: _Union['_MaciDataObj', dict, __ClassObject], 
     *,
     append: bool=False,
     indent_level: int=1,
     indentation_on: bool=True,
     multi_line_str: bool=False,
-    encoding: __Union[str, None]=None,
+    encoding: _Union[str, None]=None,
     private_attrs: bool=False,
     private_under_attrs: bool=False,
     private_dunder_attrs: bool=False,
     class_attrs: bool=False,
     private_init_attrs: bool=False,
     private_init_under_attrs: bool=False,
     private_init_dunder_attrs: bool=False,
@@ -58,57 +55,54 @@
     Normal: dump('path/of/filename', 'data')
 
     Append to File: dump('path/of/filename', 'data', append=True)
 
     Indent OFF: dump('path/of/filename', 'data', indentation_on=False)
     """
     # Error Checks & Messages
-    _err_messages: _Any = {  # ignore type checker
-        '__err_msg_no_attrs_found': "Cannot save file. No attributes found in the object passed",
-    }
-    __err_msg_type_filename = "Only str is allowed for 'filename'"
-    __err_msg_type_data = "Only MaciDataObj|dict|CustomClass is allowed for 'data'"
-    __err_msg_type_append = "Only bool is allowed for 'append'"
-    __err_msg_type_indent_level = "Only int is allowed for 'indent_level'"
-    __err_msg_type_indentation_on = "Only bool is allowed for 'indentation_on'"
-    __err_msg_type_multi_line_str = "Only bool is allowed for 'multi_line_str'"
-    __err_msg_type_encoding = "Only str|None or valid option is allowed for 'encoding'"
-    __err_msg_type_private_attrs = "Only bool is allowed for 'private_attrs'"
-    __err_msg_type_private_under_attrs = "Only bool is allowed for 'private_under_attrs'"
-    __err_msg_type_private_dunder_attrs = "Only bool is allowed for 'private_dunder_attrs'"
-    __err_msg_type_class_attrs = "Only bool is allowed for 'class_attrs'"
-    __err_msg_type_private_init_attrs = "Only bool is allowed for 'private_init_attrs'"
-    __err_msg_type_private_init_under_attrs = "Only bool is allowed for 'private_init_under_attrs'"
-    __err_msg_type_private_init_dunder_attrs = "Only bool is allowed for 'private_init_dunder_attrs'"
-    __err_msg_type_private_class_attrs = "Only bool is allowed for 'private_class_attrs'"
-    __err_msg_type_private_class_under_attrs = "Only bool is allowed for 'private_class_under_attrs'"
-    __err_msg_type_private_class_dunder_attrs = "Only bool is allowed for 'private_class_dunder_attrs'"
-    __err_msg_type_use_symbol_glyphs = "Only bool is allowed for 'use_symbol_glyphs'"
+    err_msg_type_filename = "Only str is allowed for 'filename'"
+    err_msg_type_data = "Only MaciDataObj|dict|custom ClassObject is allowed for 'data'"
+    err_msg_type_append = "Only bool is allowed for 'append'"
+    err_msg_type_indent_level = "Only int is allowed for 'indent_level'"
+    err_msg_type_indentation_on = "Only bool is allowed for 'indentation_on'"
+    err_msg_type_multi_line_str = "Only bool is allowed for 'multi_line_str'"
+    err_msg_type_encoding = "Only str|None or valid option is allowed for 'encoding'"
+    err_msg_type_private_attrs = "Only bool is allowed for 'private_attrs'"
+    err_msg_type_private_under_attrs = "Only bool is allowed for 'private_under_attrs'"
+    err_msg_type_private_dunder_attrs = "Only bool is allowed for 'private_dunder_attrs'"
+    err_msg_type_class_attrs = "Only bool is allowed for 'class_attrs'"
+    err_msg_type_private_init_attrs = "Only bool is allowed for 'private_init_attrs'"
+    err_msg_type_private_init_under_attrs = "Only bool is allowed for 'private_init_under_attrs'"
+    err_msg_type_private_init_dunder_attrs = "Only bool is allowed for 'private_init_dunder_attrs'"
+    err_msg_type_private_class_attrs = "Only bool is allowed for 'private_class_attrs'"
+    err_msg_type_private_class_under_attrs = "Only bool is allowed for 'private_class_under_attrs'"
+    err_msg_type_private_class_dunder_attrs = "Only bool is allowed for 'private_class_dunder_attrs'"
+    err_msg_type_use_symbol_glyphs = "Only bool is allowed for 'use_symbol_glyphs'"
 
 
     filter_data_object_types = (str, int, float, bool, list, tuple, set, type(None), bytes, complex, range, frozenset, bytearray, memoryview)
 
-    if not isinstance(filename, str): raise Dump(__err_msg_type_filename, f'\nGot: "{filename}"')
-    if isinstance(data, filter_data_object_types): raise Dump(__err_msg_type_data, f'\nGot: {repr(data)}')
-    if not isinstance(append, bool): raise Dump(__err_msg_type_append, f'\nGot: {repr(append)}')
-    if not isinstance(indent_level, int): raise Dump(__err_msg_type_indent_level, f'\nGot: {repr(indent_level)}')
-    if not isinstance(indentation_on, bool): raise Dump(__err_msg_type_indentation_on, f'\nGot: {repr(indentation_on)}')
-    if not isinstance(multi_line_str, bool): raise Dump(__err_msg_type_multi_line_str, f'\nGot: {repr(multi_line_str)}')
-    if not isinstance(encoding, (str, type(None))): raise Dump(__err_msg_type_encoding, f'\nGot: {repr(encoding)}')
-    if not isinstance(private_attrs, bool): raise Dump(__err_msg_type_private_attrs, f'\nGot: {repr(private_attrs)}')
-    if not isinstance(private_under_attrs, bool): raise Dump(__err_msg_type_private_under_attrs, f'\nGot: {repr(private_under_attrs)}')
-    if not isinstance(private_dunder_attrs, bool): raise Dump(__err_msg_type_private_dunder_attrs, f'\nGot: {repr(private_dunder_attrs)}')
-    if not isinstance(class_attrs, bool): raise Dump(__err_msg_type_class_attrs, f'\nGot: {repr(class_attrs)}')
-    if not isinstance(private_init_attrs, bool): raise Dump(__err_msg_type_private_init_attrs, f'\nGot: {repr(private_init_attrs)}')
-    if not isinstance(private_init_under_attrs, bool): raise Dump(__err_msg_type_private_init_under_attrs, f'\nGot: {repr(private_init_under_attrs)}')
-    if not isinstance(private_init_dunder_attrs, bool): raise Dump(__err_msg_type_private_init_dunder_attrs, f'\nGot: {repr(private_init_dunder_attrs)}')
-    if not isinstance(private_class_attrs, bool): raise Dump(__err_msg_type_private_class_attrs, f'\nGot: {repr(private_class_attrs)}')
-    if not isinstance(private_class_under_attrs, bool): raise Dump(__err_msg_type_private_class_under_attrs, f'\nGot: {repr(private_class_under_attrs)}')
-    if not isinstance(private_class_dunder_attrs, bool): raise Dump(__err_msg_type_private_class_dunder_attrs, f'\nGot: {repr(private_class_dunder_attrs)}')
-    if not isinstance(use_symbol_glyphs, bool): raise Dump(__err_msg_type_use_symbol_glyphs, f'\nGot: {repr(use_symbol_glyphs)}')
+    if not isinstance(filename, str): raise Dump(err_msg_type_filename, f'\nGot: {repr(filename)}')
+    if isinstance(data, filter_data_object_types): raise Dump(err_msg_type_data, f'\nGot: {repr(data)}')
+    if not isinstance(append, bool): raise Dump(err_msg_type_append, f'\nGot: {repr(append)}')
+    if not isinstance(indent_level, int): raise Dump(err_msg_type_indent_level, f'\nGot: {repr(indent_level)}')
+    if not isinstance(indentation_on, bool): raise Dump(err_msg_type_indentation_on, f'\nGot: {repr(indentation_on)}')
+    if not isinstance(multi_line_str, bool): raise Dump(err_msg_type_multi_line_str, f'\nGot: {repr(multi_line_str)}')
+    if not isinstance(encoding, (str, type(None))): raise Dump(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
+    if not isinstance(private_attrs, bool): raise Dump(err_msg_type_private_attrs, f'\nGot: {repr(private_attrs)}')
+    if not isinstance(private_under_attrs, bool): raise Dump(err_msg_type_private_under_attrs, f'\nGot: {repr(private_under_attrs)}')
+    if not isinstance(private_dunder_attrs, bool): raise Dump(err_msg_type_private_dunder_attrs, f'\nGot: {repr(private_dunder_attrs)}')
+    if not isinstance(class_attrs, bool): raise Dump(err_msg_type_class_attrs, f'\nGot: {repr(class_attrs)}')
+    if not isinstance(private_init_attrs, bool): raise Dump(err_msg_type_private_init_attrs, f'\nGot: {repr(private_init_attrs)}')
+    if not isinstance(private_init_under_attrs, bool): raise Dump(err_msg_type_private_init_under_attrs, f'\nGot: {repr(private_init_under_attrs)}')
+    if not isinstance(private_init_dunder_attrs, bool): raise Dump(err_msg_type_private_init_dunder_attrs, f'\nGot: {repr(private_init_dunder_attrs)}')
+    if not isinstance(private_class_attrs, bool): raise Dump(err_msg_type_private_class_attrs, f'\nGot: {repr(private_class_attrs)}')
+    if not isinstance(private_class_under_attrs, bool): raise Dump(err_msg_type_private_class_under_attrs, f'\nGot: {repr(private_class_under_attrs)}')
+    if not isinstance(private_class_dunder_attrs, bool): raise Dump(err_msg_type_private_class_dunder_attrs, f'\nGot: {repr(private_class_dunder_attrs)}')
+    if not isinstance(use_symbol_glyphs, bool): raise Dump(err_msg_type_use_symbol_glyphs, f'\nGot: {repr(use_symbol_glyphs)}')
 
     # Write built data to file, return None
     __dump_data(
         filename=filename,
         data=data,
         append=append,
         indent_level=indent_level,
@@ -121,12 +115,11 @@
         private_dunder_attrs=private_dunder_attrs,
         private_init_attrs=private_init_attrs,
         private_init_under_attrs=private_init_under_attrs,
         private_init_dunder_attrs=private_init_dunder_attrs,
         private_class_attrs=private_class_attrs,
         private_class_under_attrs=private_class_under_attrs,
         private_class_dunder_attrs=private_class_dunder_attrs,
-        use_symbol_glyphs=use_symbol_glyphs,
-        **_err_messages
+        use_symbol_glyphs=use_symbol_glyphs
     )
 
     return None
```

### Comparing `maci-0.3.1/maci/_native/dumpraw.py` & `maci-0.4.0/maci/_native/dumpraw.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # dumpraw
 #########################################################################################################
 # Imports
-from typing import Any as __Any
-from typing import Union as __Union
-from os import path as __path
+from typing import Any as _Any
+from typing import Union as _Union
+from os import path as _path
 from ..error import DumpRaw
 
 #########################################################################################################
 # Export Data to File
-def dumpraw(filename: str, *data: __Any, append: bool=False, byte_data: bool=False, newline_sep: bool=True, encoding: __Union[str, None]=None) -> None:
+def dumpraw(filename: str, *data: _Any, append: bool=False, byte_data: bool=False, newline_sep: bool=True, encoding: _Union[str, None]=None) -> None:
     """
     Exports a new file with the new data.
     
     Enter new filename as str, Pass any data type for output to file.
 
     [Options]
     append: set to True to append data to a file (Default=False, which writes a new file each time)
@@ -21,23 +21,23 @@
 
     [Example Use]
     Normal: dump('path/of/filename', 'data')
 
     Byte Data: dump('path/of/filename', b'data', byte_data=True)
     """
     # Error Checks
-    __err_msg_bytes = "Only bytes is allowed if using 'byte_data' option"
-    __err_msg_type_bytes = "Only bool is allowed for 'byte_data'"
-    __err_msg_type_str = "Only str is allowed for 'filename'"
-    __err_msg_append = "Only bool is allowed for 'append'"
+    err_msg_bytes = "Only bytes is allowed if using 'byte_data' option"
+    err_msg_type_bytes = "Only bool is allowed for 'byte_data'"
+    err_msg_type_str = "Only str is allowed for 'filename'"
+    err_msg_append = "Only bool is allowed for 'append'"
     err_msg_type_encoding = "Only str|None or valid option is allowed for 'encoding'"
 
-    if not isinstance(byte_data, bool): raise DumpRaw(__err_msg_type_bytes, f'\nGot: {repr(byte_data)}')
-    if not isinstance(filename, str): raise DumpRaw(__err_msg_type_str, f'\nGot: {repr(filename)}')
-    if (not isinstance(append, bool)): raise DumpRaw(__err_msg_append, f'\nGot: {repr(append)}')
+    if not isinstance(byte_data, bool): raise DumpRaw(err_msg_type_bytes, f'\nGot: {repr(byte_data)}')
+    if not isinstance(filename, str): raise DumpRaw(err_msg_type_str, f'\nGot: {repr(filename)}')
+    if (not isinstance(append, bool)): raise DumpRaw(err_msg_append, f'\nGot: {repr(append)}')
     if (not isinstance(encoding, (str, type(None)))): raise DumpRaw(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
 
     # Set Write Mode: 'a' = append, 'w' = write
     mode = 'a' if append else 'w'
 
     # Set Newline Separator
     set_newline_sep = ''
@@ -48,52 +48,52 @@
     # Raw Data to File
     if (mode == 'w') and (not byte_data):
         try:
             with open(filename, 'w', encoding=encoding) as f:
                 for data_to_write in data:
                     f.writelines(f"{set_newline_sep}{data_to_write}")
                     set_newline_sep = '\n' if newline_sep else ''
-        except (FileNotFoundError, OSError) as __err_msg: raise DumpRaw(__err_msg, f'\nGot: {repr(filename)}')
+        except (FileNotFoundError, OSError) as err_msg: raise DumpRaw(err_msg, f'\nGot: {repr(filename)}')
         except LookupError: raise DumpRaw(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
 
     # Byte Data Converted to File
     if (mode == 'w') and (byte_data):
         for data_to_write in data:
-            if not isinstance(data_to_write, bytes): raise DumpRaw(__err_msg_bytes, f'\nGot: {repr(data_to_write)}')
+            if not isinstance(data_to_write, bytes): raise DumpRaw(err_msg_bytes, f'\nGot: {repr(data_to_write)}')
         try:
             with open(filename, 'wb') as f:
                 for data_to_write in data:
                     f.write(data_to_write)
-        except (FileNotFoundError, OSError) as __err_msg: raise DumpRaw(__err_msg, f'\nGot: {repr(filename)}')
+        except (FileNotFoundError, OSError) as err_msg: raise DumpRaw(err_msg, f'\nGot: {repr(filename)}')
 
     
     ### Append File ###
     _new_line = '\n'
     _new_line_bytes = b'\n'
 
     # Raw Data to File
     if (mode == 'a') and (not byte_data):
         # Check if file empty. Throws error if file not found
         try:
-            if __path.getsize(filename) == 0:
+            if _path.getsize(filename) == 0:
                 set_newline_sep = ''
                 _new_line = ''
             with open(filename, 'a', encoding=encoding) as f:
                 for data_to_write in data:
                     f.writelines(f"{_new_line}{set_newline_sep}{data_to_write}")
                     set_newline_sep = '\n' if newline_sep else ''
                     _new_line = ''
-        except (FileNotFoundError, OSError) as __err_msg: raise DumpRaw(__err_msg, f'\nGot: {repr(filename)}')
+        except (FileNotFoundError, OSError) as err_msg: raise DumpRaw(err_msg, f'\nGot: {repr(filename)}')
         except LookupError: raise DumpRaw(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
 
     # Byte Data to File
     if (mode == 'a') and (byte_data):
         for data_to_write in data:
-            if not isinstance(data_to_write, bytes): raise DumpRaw(__err_msg_bytes, f'\nGot: {repr(data_to_write)}')
+            if not isinstance(data_to_write, bytes): raise DumpRaw(err_msg_bytes, f'\nGot: {repr(data_to_write)}')
         # Check if file empty. Throws error if file not found
         try: 
-            if __path.getsize(filename) == 0: _new_line_bytes = b''
+            if _path.getsize(filename) == 0: _new_line_bytes = b''
             with open(filename, 'ab') as f:
                 for data_to_write in data:
                     f.write(_new_line_bytes)
                     f.write(data_to_write)
-        except (FileNotFoundError, OSError) as __err_msg: raise DumpRaw(__err_msg, f'\nGot: {repr(filename)}')
+        except (FileNotFoundError, OSError) as err_msg: raise DumpRaw(err_msg, f'\nGot: {repr(filename)}')
```

### Comparing `maci-0.3.1/maci/_native/dumpstr.py` & `maci-0.4.0/maci/_native/dumpstr.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # dumpstr
 #########################################################################################################
 # Imports
-from typing import Union as __Union
+from typing import Union as _Union
 from typing import Any as _Any
-from typing import NewType as __NewType
+from typing import NewType as _NewType
 from typing import Optional as _Optional
 from ..error import DumpStr
 from ..data import __dump_data
-from ..data import MaciDataObj as __MaciDataObj
+from ..data import MaciDataObj as _MaciDataObj
+from ..hint import __ClassObject
 
 #########################################################################################################
 # Dump Data to String
-
-# Hinting reference name for "CustomClass" to denote a CustomClass can be used to dump data
-CustomClass = __NewType('CustomClass', object)
-
 def dumpstr(
-    data: __Union['__MaciDataObj', dict, CustomClass], 
+    data: _Union['_MaciDataObj', dict, __ClassObject], 
     *,
     indent_level: int=1,
     indentation_on: bool=True,
     multi_line_str: bool=False,
     private_attrs: bool=False,
     private_under_attrs: bool=False,
     private_dunder_attrs: bool=False,
@@ -50,53 +47,50 @@
 
     [Example Use]
     Normal: dumpstr(data)
 
     Indent OFF: dumpstr(data, indentation_on=False)
     """
     # Error Checks
-    _err_messages: _Any = {  # ignore type checker
-        '__err_msg_no_attrs_found': "Cannot dump string. No attributes found in the object passed",
-    }
-    __err_msg_type_indent_level = "Only int is allowed for 'indent_level'"
-    __err_msg_type_indentation_on = "Only bool is allowed for 'indentation_on'"
-    __err_msg_type_data = "Only MaciDataObj|dict|CustomClass is allowed for 'data'"
-    __err_msg_type_indent_level = "Only int is allowed for 'indent_level'"
-    __err_msg_type_indentation_on = "Only bool is allowed for 'indentation_on'"
-    __err_msg_type_multi_line_str = "Only bool is allowed for 'multi_line_str'"
-    __err_msg_type_private_attrs = "Only bool is allowed for 'private_attrs'"
-    __err_msg_type_private_under_attrs = "Only bool is allowed for 'private_under_attrs'"
-    __err_msg_type_private_dunder_attrs = "Only bool is allowed for 'private_dunder_attrs'"
-    __err_msg_type_class_attrs = "Only bool is allowed for 'class_attrs'"
-    __err_msg_type_private_init_attrs = "Only bool is allowed for 'private_init_attrs'"
-    __err_msg_type_private_init_under_attrs = "Only bool is allowed for 'private_init_under_attrs'"
-    __err_msg_type_private_init_dunder_attrs = "Only bool is allowed for 'private_init_dunder_attrs'"
-    __err_msg_type_private_class_attrs = "Only bool is allowed for 'private_class_attrs'"
-    __err_msg_type_private_class_under_attrs = "Only bool is allowed for 'private_class_under_attrs'"
-    __err_msg_type_private_class_dunder_attrs = "Only bool is allowed for 'private_class_dunder_attrs'"
-    __err_msg_type_use_symbol_glyphs = "Only bool is allowed for 'use_symbol_glyphs'"
+    err_msg_type_indent_level = "Only int is allowed for 'indent_level'"
+    err_msg_type_indentation_on = "Only bool is allowed for 'indentation_on'"
+    err_msg_type_data = "Only MaciDataObj|dict|custom ClassObject is allowed for 'data'"
+    err_msg_type_indent_level = "Only int is allowed for 'indent_level'"
+    err_msg_type_indentation_on = "Only bool is allowed for 'indentation_on'"
+    err_msg_type_multi_line_str = "Only bool is allowed for 'multi_line_str'"
+    err_msg_type_private_attrs = "Only bool is allowed for 'private_attrs'"
+    err_msg_type_private_under_attrs = "Only bool is allowed for 'private_under_attrs'"
+    err_msg_type_private_dunder_attrs = "Only bool is allowed for 'private_dunder_attrs'"
+    err_msg_type_class_attrs = "Only bool is allowed for 'class_attrs'"
+    err_msg_type_private_init_attrs = "Only bool is allowed for 'private_init_attrs'"
+    err_msg_type_private_init_under_attrs = "Only bool is allowed for 'private_init_under_attrs'"
+    err_msg_type_private_init_dunder_attrs = "Only bool is allowed for 'private_init_dunder_attrs'"
+    err_msg_type_private_class_attrs = "Only bool is allowed for 'private_class_attrs'"
+    err_msg_type_private_class_under_attrs = "Only bool is allowed for 'private_class_under_attrs'"
+    err_msg_type_private_class_dunder_attrs = "Only bool is allowed for 'private_class_dunder_attrs'"
+    err_msg_type_use_symbol_glyphs = "Only bool is allowed for 'use_symbol_glyphs'"
 
 
     filter_data_object_types = (str, int, float, bool, list, tuple, set, type(None), bytes, complex, range, frozenset, bytearray, memoryview)
 
-    if isinstance(data, filter_data_object_types): raise DumpStr(__err_msg_type_data, f'\nGot: {repr(data)}')
-    if not isinstance(indent_level, int): raise DumpStr(__err_msg_type_indent_level, f'\nGot: {repr(indent_level)}')
-    if not isinstance(indentation_on, bool): raise DumpStr(__err_msg_type_indentation_on, f'\nGot: {repr(indentation_on)}')
-    if not isinstance(multi_line_str, bool): raise DumpStr(__err_msg_type_multi_line_str, f'\nGot: {repr(multi_line_str)}')
-    if not isinstance(private_attrs, bool): raise DumpStr(__err_msg_type_private_attrs, f'\nGot: {repr(private_attrs)}')
-    if not isinstance(private_under_attrs, bool): raise DumpStr(__err_msg_type_private_under_attrs, f'\nGot: {repr(private_under_attrs)}')
-    if not isinstance(private_dunder_attrs, bool): raise DumpStr(__err_msg_type_private_dunder_attrs, f'\nGot: {repr(private_dunder_attrs)}')
-    if not isinstance(class_attrs, bool): raise DumpStr(__err_msg_type_class_attrs, f'\nGot: {repr(class_attrs)}')
-    if not isinstance(private_init_attrs, bool): raise DumpStr(__err_msg_type_private_init_attrs, f'\nGot: {repr(private_init_attrs)}')
-    if not isinstance(private_init_under_attrs, bool): raise DumpStr(__err_msg_type_private_init_under_attrs, f'\nGot: {repr(private_init_under_attrs)}')
-    if not isinstance(private_init_dunder_attrs, bool): raise DumpStr(__err_msg_type_private_init_dunder_attrs, f'\nGot: {repr(private_init_dunder_attrs)}')
-    if not isinstance(private_class_attrs, bool): raise DumpStr(__err_msg_type_private_class_attrs, f'\nGot: {repr(private_class_attrs)}')
-    if not isinstance(private_class_under_attrs, bool): raise DumpStr(__err_msg_type_private_class_under_attrs, f'\nGot: {repr(private_class_under_attrs)}')
-    if not isinstance(private_class_dunder_attrs, bool): raise DumpStr(__err_msg_type_private_class_dunder_attrs, f'\nGot: {repr(private_class_dunder_attrs)}')
-    if not isinstance(use_symbol_glyphs, bool): raise DumpStr(__err_msg_type_use_symbol_glyphs, f'\nGot: {repr(use_symbol_glyphs)}')
+    if isinstance(data, filter_data_object_types): raise DumpStr(err_msg_type_data, f'\nGot: {repr(data)}')
+    if not isinstance(indent_level, int): raise DumpStr(err_msg_type_indent_level, f'\nGot: {repr(indent_level)}')
+    if not isinstance(indentation_on, bool): raise DumpStr(err_msg_type_indentation_on, f'\nGot: {repr(indentation_on)}')
+    if not isinstance(multi_line_str, bool): raise DumpStr(err_msg_type_multi_line_str, f'\nGot: {repr(multi_line_str)}')
+    if not isinstance(private_attrs, bool): raise DumpStr(err_msg_type_private_attrs, f'\nGot: {repr(private_attrs)}')
+    if not isinstance(private_under_attrs, bool): raise DumpStr(err_msg_type_private_under_attrs, f'\nGot: {repr(private_under_attrs)}')
+    if not isinstance(private_dunder_attrs, bool): raise DumpStr(err_msg_type_private_dunder_attrs, f'\nGot: {repr(private_dunder_attrs)}')
+    if not isinstance(class_attrs, bool): raise DumpStr(err_msg_type_class_attrs, f'\nGot: {repr(class_attrs)}')
+    if not isinstance(private_init_attrs, bool): raise DumpStr(err_msg_type_private_init_attrs, f'\nGot: {repr(private_init_attrs)}')
+    if not isinstance(private_init_under_attrs, bool): raise DumpStr(err_msg_type_private_init_under_attrs, f'\nGot: {repr(private_init_under_attrs)}')
+    if not isinstance(private_init_dunder_attrs, bool): raise DumpStr(err_msg_type_private_init_dunder_attrs, f'\nGot: {repr(private_init_dunder_attrs)}')
+    if not isinstance(private_class_attrs, bool): raise DumpStr(err_msg_type_private_class_attrs, f'\nGot: {repr(private_class_attrs)}')
+    if not isinstance(private_class_under_attrs, bool): raise DumpStr(err_msg_type_private_class_under_attrs, f'\nGot: {repr(private_class_under_attrs)}')
+    if not isinstance(private_class_dunder_attrs, bool): raise DumpStr(err_msg_type_private_class_dunder_attrs, f'\nGot: {repr(private_class_dunder_attrs)}')
+    if not isinstance(use_symbol_glyphs, bool): raise DumpStr(err_msg_type_use_symbol_glyphs, f'\nGot: {repr(use_symbol_glyphs)}')
 
     # Return built/dumped string
     return __dump_data(
         _is_string_request=True,
         data=data,
         filename='',
         indent_level=indent_level,
@@ -108,10 +102,9 @@
         private_dunder_attrs=private_dunder_attrs,
         private_init_attrs=private_init_attrs,
         private_init_under_attrs=private_init_under_attrs,
         private_init_dunder_attrs=private_init_dunder_attrs,
         private_class_attrs=private_class_attrs,
         private_class_under_attrs=private_class_under_attrs,
         private_class_dunder_attrs=private_class_dunder_attrs,
-        use_symbol_glyphs=use_symbol_glyphs,
-        **_err_messages
+        use_symbol_glyphs=use_symbol_glyphs
     )
```

### Comparing `maci-0.3.1/maci/_native/load.py` & `maci-0.4.0/maci/_native/load.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # load
 #########################################################################################################
 # Imports
-from ast import literal_eval as __literal_eval__
-from os import path as __path
+from os import path as _path
 from typing import Any as _Any
 from typing import Optional as _Optional
-from ..data import MaciDataObj
 from ..error import Load, GeneralError
+from ..data import MaciDataObj as _MaciDataObj
+from .build import build as _build
 
 #########################################################################################################
 # Import py Data from File
-def load(filename: str, *, attr_name_dedup: bool=True, encoding: _Optional[str]=None, _ignore_maci_attr_check: bool=False) -> _Optional[MaciDataObj]:
+def load(filename: str, *, attr_name_dedup: bool=True, encoding: _Optional[str]=None, _ignore_maci_attr_check: bool=False) -> _MaciDataObj:
     """
     Imports saved python data from any text file.
 
     Returns a class of attributes. Assign the output to var
 
     Enter file location as str to import.
 
     Accepted data types: str, int, float, bool, list, dict, tuple, set, nonetype, bytes, datetime
 
-    Returns None if file empty
+    Returns empty object if file empty
 
     [Example Use]
     load('filename.data' or 'path/to/filename.data')
 
     [Warning]
     Turning OFF 'attr_name_dedup' is not recommended as you gain the ability to overwrite
     your attribute names that already preexist. This also may affect MaciDataObj behavior
@@ -40,30 +40,30 @@
     if not isinstance(filename, str): raise Load(err_msg_type_filename, f'\nGot: {repr(filename)}')
     if not isinstance(attr_name_dedup, bool): raise Load(err_msg_type_attr_name_dedup, f'\nGot: {repr(attr_name_dedup)}')
     if not isinstance(encoding, (str, type(None))): raise Load(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
     if not isinstance(_ignore_maci_attr_check, bool): raise Load(err_msg_type__ignore_maci_attr_check, f'\nGot: {repr(_ignore_maci_attr_check)}')
 
     # Check if file empty. Returns None if empty
     try:
-        if __path.getsize(filename) == 0:
-            return None
+        if _path.getsize(filename) == 0:
+            return _build()
     except (FileNotFoundError, OSError) as __err_msg: raise Load(__err_msg, f'\nGot: {repr(filename)}')
 
     # Syntax/Usage Error Messages
     __err_messages: _Any = {  # ignore type checker
-        '_py_syntax_err_msg': "Must have valid Python data types to import, or file's syntax is not formatted correctly",
+        '_py_syntax_err_msg': "Must have valid Python data types to import, or file's maci syntax is incorrect",
         '_name_preexists_err_msg': "Name already preexists. Must give unique attribute names in file",
-        '_name_reference_does_not_exist_msg': "Name reference does not exist! Must reference attribute names in file that have been defined",
+        '_name_reference_does_not_exist_msg': "Map name does not exist! Must map attribute names in file that have been defined",
         '_assignment_locked_atrribs_err_msg': "Attribute Name Locked! Cannot be reassigned",
         '_assignment_hard_locked_atrribs_err_msg': "Attribute Name Hard Locked! Cannot be reassigned, deleted, or unlocked"
     }
 
     # Return Final Import
     try:
-        return MaciDataObj(
+        return _MaciDataObj(
                     filename,
                     _is_load_request=True,
                     _ignore_internal_maci_attr_check=_ignore_maci_attr_check,
                     attr_name_dedup=attr_name_dedup,
                     encoding=encoding,
                     **__err_messages
                 )
```

### Comparing `maci-0.3.1/maci/_native/loadattrs.py` & `maci-0.4.0/maci/_native/loadattrs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # loadattrs
 #########################################################################################################
 # Imports
-from typing import NewType as __NewType
-from typing import Union as __Union
+from typing import NewType as _NewType
+from typing import Union as _Union
 from ..error import LoadAttrs, Load
-from .load import load as __load
-from ..data import MaciDataObj as __MaciDataObj
+from .load import load as _load
+from ..data import MaciDataObj as _MaciDataObj
+from ..hint import __ClassObject
 
 #########################################################################################################
 # Import Attributes from File
-
-# Hinting reference name for "CustomClass" to denote a CustomClass can be used to dump data
-CustomClass = __NewType('CustomClass', object)
-
-def loadattrs(filename: str, class_object: CustomClass, *, encoding: __Union[str, None]=None, attr_name_dedup: bool=False, _ignore_maci_attr_check: bool=True) -> None:
+def loadattrs(filename: str, class_object: __ClassObject, *, encoding: _Union[str, None]=None, attr_name_dedup: bool=False, _ignore_maci_attr_check: bool=True) -> None:
     """
     Import saved attributes from file back into a custom class. This is done in-place
 
     Enter filename as str, Pass custom class object.
 
     [Example Use]
 
@@ -27,38 +24,38 @@
     Turning OFF 'attr_name_dedup' is not recommended as you gain the ability to overwrite
     your attribute names that already preexist. This also may affect MaciDataObj behavior
     including the ability to overwrite internal dunder names. This feature is meant to protect you from accidentally
     duplicating an attribute name in a file that has already been created.
     """
     # Error Checks
     err_msg_type_filename = "Only str is allowed for 'filename'"
-    __err_msg_type_class_obj = "Only a custom class object is allowed for 'class_object'"
-    __err_msg_type_maci_obj = "Please use 'load' function to properly import a 'MaciDataObj' object"
+    err_msg_type_class_obj = "Only a custom ClassObject is allowed for 'class_object'"
+    err_msg_type_maci_obj = "Please use 'load' function to properly import a 'MaciDataObj' object"
 
     if not isinstance(filename, str): raise LoadAttrs(err_msg_type_filename, f'\nGot: {repr(filename)}')
 
     # Verify if Custom Class Obj
     _filter_objects = (str, int, float, bool, list, dict, tuple, set, type(None), bytes, complex, range, frozenset, bytearray, memoryview)
     if isinstance(class_object, _filter_objects):
-        raise LoadAttrs(__err_msg_type_class_obj, f'\nGot: {repr(class_object)}')
+        raise LoadAttrs(err_msg_type_class_obj, f'\nGot: {repr(class_object)}')
 
-    if isinstance(class_object, __MaciDataObj):
-        raise LoadAttrs(__err_msg_type_maci_obj, f'\nGot: {repr(class_object)}')
+    if isinstance(class_object, _MaciDataObj):
+        raise LoadAttrs(err_msg_type_maci_obj, f'\nGot: {repr(class_object)}')
 
-    if isinstance(class_object, type(__MaciDataObj)):
-        raise LoadAttrs(__err_msg_type_maci_obj, f'\nGot: {repr(class_object)}')
+    if isinstance(class_object, type(_MaciDataObj)):
+        raise LoadAttrs(err_msg_type_maci_obj, f'\nGot: {repr(class_object)}')
 
     # Import Attrs from File and Inject into Given Class Object
 
     # Skip Key
-    __skip_object_key = ('_MaciDataObjConstructor', '__maci_obj_format_id')
+    skip_object_key = ('_MaciDataObjConstructor', '__maci_obj_format_id')
 
     # Import Attrs
     try:
-        __imported_data = __load(filename, attr_name_dedup=attr_name_dedup, encoding=encoding, _ignore_maci_attr_check=_ignore_maci_attr_check)
-        for key,value in __imported_data.__dict__.items():
-            if key.startswith(__skip_object_key): continue
+        imported_data = _load(filename, attr_name_dedup=attr_name_dedup, encoding=encoding, _ignore_maci_attr_check=_ignore_maci_attr_check)
+        for key,value in imported_data.__dict__.items():
+            if key.startswith(skip_object_key): continue
             setattr(class_object, key, value)
-    except Load as __err_msg:
-        raise LoadAttrs(__err_msg, '')
+    except Load as err_msg:
+        raise LoadAttrs(err_msg, '')
 
     return None
```

### Comparing `maci-0.3.1/maci/_native/loaddict.py` & `maci-0.4.0/maci/_native/loaddict.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # loaddict
 #########################################################################################################
 # Imports
-from ast import literal_eval as __literal_eval__
-from os import path as __path
+from os import path as _path
 from copy import deepcopy as _deepcopy
 from typing import Any as _Any
 from typing import Optional as _Optional
-from ..data import MaciDataObj
 from ..error import LoadDict, Load
+from ..data import MaciDataObj as _MaciDataObj
 
 #########################################################################################################
 # Import py Data from File
 def loaddict(filename: str, *, attr_name_dedup: bool=True, encoding: _Optional[str]=None) -> _Optional[dict]:
     """
     Imports pythonic data from any text file
 
@@ -39,23 +38,23 @@
 
     if not isinstance(filename, str): raise LoadDict(err_msg_type_filename, f'\nGot: {repr(filename)}')
     if not isinstance(attr_name_dedup, bool): raise LoadDict(err_msg_type_attr_name_dedup, f'\nGot: {repr(attr_name_dedup)}')
     if not isinstance(encoding, (str, type(None))): raise LoadDict(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
 
     # Check if file empty. Returns None if empty
     try:
-        if __path.getsize(filename) == 0:
-            return None
-    except (FileNotFoundError, OSError) as __err_msg: raise LoadDict(__err_msg, f'\nGot: "{filename}"')
+        if _path.getsize(filename) == 0:
+            return dict()
+    except (FileNotFoundError, OSError) as __err_msg: raise LoadDict(__err_msg, f'\nGot: {repr(filename)}')
 
     # Syntax/Usage Error Messages
     err_messages: _Any = {  # ignore type checker
-        '_py_syntax_err_msg': "Must have valid Python data types to import, or file's syntax is not formatted correctly",
+        '_py_syntax_err_msg': "Must have valid Python data types to import, or file's maci syntax is incorrect",
         '_name_preexists_err_msg': "Name already preexists. Must give unique attribute names in file",
-        '_name_reference_does_not_exist_msg': "Name reference does not exist! Must reference attribute names in file that have been defined",
+        '_name_reference_does_not_exist_msg': "Map name does not exist! Must map attribute names in file that have been defined",
         '_assignment_locked_atrribs_err_msg': "Attribute Name Locked! Cannot be reassigned",
         '_assignment_hard_locked_atrribs_err_msg': "Attribute Name Hard Locked! Cannot be reassigned, deleted, or unlocked"
     }
 
     # Internal Key List to Remove from Dict
     internal_remove_key_list = {
         '_MaciDataObjConstructor__assignment_locked_attribs',
@@ -67,15 +66,15 @@
         '_MaciDataObjConstructor__assignment_locked_atrribs_err_msg',
         '_MaciDataObjConstructor__assignment_hard_locked_atrribs_err_msg',
         '_MaciDataObjConstructor__ignore_internal_maci_attr_check',
     }
 
     # Generate Dict as a Fresh Copy
     try: 
-        dict_data = _deepcopy(vars(MaciDataObj(
+        dict_data = _deepcopy(vars(_MaciDataObj(
                 filename,
                 _is_load_request=True,
                 attr_name_dedup=attr_name_dedup,
                 encoding=encoding,
                 **err_messages
             )))
     except Load as __err_msg: raise LoadDict(__err_msg) from None
```

### Comparing `maci-0.3.1/maci/_native/loadraw.py` & `maci-0.4.0/maci/_native/loadraw.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # loadraw
 #########################################################################################################
 # Imports
 from typing import Union as _Union
-from os import path as __path
+from os import path as _path
 from ..error import LoadRaw
 
 #########################################################################################################
 # Import raw data from file
 def loadraw(filename: str, *, byte_data: bool=False, encoding: _Union[str, None]=None) -> _Union[str, bytes]:
     """
     Imports any raw data from a file.
@@ -29,20 +29,20 @@
     if not isinstance(byte_data, bool): raise LoadRaw(err_msg_type_byte_data, f'\nGot: {repr(byte_data)}')
     if not isinstance(encoding, (str, type(None))): raise LoadRaw(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
 
     # Validate file exists. Import File then return the raw data
     if not byte_data:
         try:
             with open(filename, 'r', encoding=encoding) as f:
-                if __path.getsize(filename) == 0:
+                if _path.getsize(filename) == 0:
                     return ''
                 return f.read()
-        except (FileNotFoundError, OSError) as __err_msg: raise LoadRaw(__err_msg, f'\nGot: "{filename}"')
+        except (FileNotFoundError, OSError) as __err_msg: raise LoadRaw(__err_msg, f'\nGot: {repr(filename)}')
         except LookupError: raise LoadRaw(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
     
     if byte_data: # pragma: no branch
         try:
             with open(filename, 'rb') as f:
-                if __path.getsize(filename) == 0:
+                if _path.getsize(filename) == 0:
                     return b''
                 return f.read()
-        except (FileNotFoundError, OSError) as __err_msg: raise LoadRaw(__err_msg, f'\nGot: "{filename}"')
+        except (FileNotFoundError, OSError) as __err_msg: raise LoadRaw(__err_msg, f'\nGot: {repr(filename)}')
```

### Comparing `maci-0.3.1/maci/_native/loadstr.py` & `maci-0.4.0/maci/_native/loadstr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 # loadstr
 #########################################################################################################
 # Imports
 from typing import Any as _Any
 from typing import Optional as _Optional
-from ..data import MaciDataObj
 from ..error import LoadStr, Load
+from ..data import MaciDataObj as _MaciDataObj
+from .build import build as _build
 
 #########################################################################################################
 # Import py Data from String
-def loadstr(py_str_data: str, *, attr_name_dedup: bool=True) -> _Optional[MaciDataObj]:
+def loadstr(maci_str_data: str, *, attr_name_dedup: bool=True) -> _Optional[_MaciDataObj]:
     """
     Imports python data from a string.
 
     Returns a class of attributes. Assign the output to var
 
     Enter python data string as str to import.
 
     Accepted data types: str, int, float, bool, list, dict, tuple, set, nonetype, bytes, datetime
 
-    Returns None if empty
+    Returns empty object if string empty
 
     [Example Use]
 
     loadstr("data1 = 'value1'\\ndata2 = "value2")
     """
     # Error Checks
-    err_msg_type_py_str_data = "Only str is allowed for 'py_str_data'"
+    err_msg_type_maci_str_data = "Only str is allowed for 'maci_str_data'"
     err_msg_type_attr_name_dedup = "Only bool is allowed for 'attr_name_dedup'"
 
-    if not isinstance(py_str_data, str): raise LoadStr(err_msg_type_py_str_data, f'\nGot: {repr(py_str_data)}')
+    if not isinstance(maci_str_data, str): raise LoadStr(err_msg_type_maci_str_data, f'\nGot: {repr(maci_str_data)}')
     if not isinstance(attr_name_dedup, bool): raise LoadStr(err_msg_type_attr_name_dedup, f'\nGot: {repr(attr_name_dedup)}')
 
     # Check if string empty. Returns None if empty
-    if py_str_data == '': return None
+    if maci_str_data.strip() == '': return _build()
 
     # Syntax/Usage Error Messages
     __err_messages: _Any = {  # ignore type checker
-        '_py_syntax_err_msg': "Must have valid Python data types to import, or string's syntax is not formatted correctly",
+        '_py_syntax_err_msg': "Must have valid Python data types to import, or string's maci syntax is incorrect",
         '_name_preexists_err_msg': "Name already preexists. Must give unique attribute names in string",
-        '_name_reference_does_not_exist_msg': "Name reference does not exist! Must reference attribute names in string that have been defined",
-        '_assignment_locked_atrribs_err_msg': "Attribute Name Locked! Cannot be reassigned"
+        '_name_reference_does_not_exist_msg': "Map name does not exist! Must map attribute names in string that have been defined",
+        '_assignment_locked_atrribs_err_msg': "Attribute Name Locked! Cannot be reassigned",
+        '_assignment_hard_locked_atrribs_err_msg': "Attribute Name Hard Locked! Cannot be reassigned, deleted, or unlocked"
     }
 
     # Return final import
     try:
-        return MaciDataObj(
+        return _MaciDataObj(
                 '',
                 _is_load_request=True,
-                _str_data=py_str_data,
+                _str_data=maci_str_data,
                 _is_str_parse_request=True,
                 attr_name_dedup=attr_name_dedup,
                 encoding=None,
                 **__err_messages,
             )
     except Load as __err_msg:
-        __err_msg.item = __err_msg.item.replace('\nFILE: ""', "")
+        __err_msg.item = __err_msg.item.replace("\nFile: ''", "")
         raise LoadStr(__err_msg.msg, f'{__err_msg.item}')
```

### Comparing `maci-0.3.1/maci/_native/loadstrdict.py` & `maci-0.4.0/maci/_native/loadstrdict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # loadstrdict
 #########################################################################################################
 # Imports
 from copy import deepcopy as _deepcopy
 from typing import Any as _Any
-from ..data import MaciDataObj
+from typing import Optional as _Optional
 from ..error import LoadStrDict, Load
+from ..data import MaciDataObj as _MaciDataObj
 
 #########################################################################################################
 # Import py Data from String
-def loadstrdict(py_str_data: str, *, attr_name_dedup: bool=True) -> dict:
+def loadstrdict(maci_str_data: str, *, attr_name_dedup: bool=True) -> _Optional[dict]:
     """
     Imports pythonic data from a string.
 
     Returns a dict. Assign the output to var
 
     Enter pythonic data string as str to import.
 
@@ -21,26 +22,30 @@
     Returns None if empty
 
     [Example Use]
 
     loadstrdict("data1 = 'value1'\\ndata2 = "value2")
     """
     # Error Checks
-    err_msg_type_py_str_data = "Only str is allowed for 'py_str_data'"
+    err_msg_type_maci_str_data = "Only str is allowed for 'maci_str_data'"
     err_msg_type_attr_name_dedup = "Only bool is allowed for 'attr_name_dedup'"
 
-    if not isinstance(py_str_data, str): raise LoadStrDict(err_msg_type_py_str_data, f'\nGot: {repr(py_str_data)}')
+    if not isinstance(maci_str_data, str): raise LoadStrDict(err_msg_type_maci_str_data, f'\nGot: {repr(maci_str_data)}')
     if not isinstance(attr_name_dedup, bool): raise LoadStrDict(err_msg_type_attr_name_dedup, f'\nGot: {repr(attr_name_dedup)}')
 
+    # Check if string empty. Returns None if empty
+    if maci_str_data.strip() == '': return dict()
+
     # Syntax/Usage Error Messages
     __err_messages: _Any = {  # ignore type checker
-        '_py_syntax_err_msg': "Must have valid Python data types to import, or string's syntax is not formatted correctly",
+        '_py_syntax_err_msg': "Must have valid Python data types to import, or string's maci syntax is incorrect",
         '_name_preexists_err_msg': "Name already preexists. Must give unique attribute names in string",
-        '_name_reference_does_not_exist_msg': "Name reference does not exist! Must reference attribute names in string that have been defined",
-        '_assignment_locked_atrribs_err_msg': "Attribute Name Locked! Cannot be reassigned"
+        '_name_reference_does_not_exist_msg': "Map name does not exist! Must map attribute names in string that have been defined",
+        '_assignment_locked_atrribs_err_msg': "Attribute Name Locked! Cannot be reassigned",
+        '_assignment_hard_locked_atrribs_err_msg': "Attribute Name Hard Locked! Cannot be reassigned, deleted, or unlocked"
     }
 
     # Internal Key List to Remove from Dict
     internal_remove_key_list = {
         '_MaciDataObjConstructor__assignment_locked_attribs',
         '_MaciDataObjConstructor__assignment_hard_locked_attribs' ,
         '_MaciDataObjConstructor__assigned_src_reference_attr_map',
@@ -50,25 +55,25 @@
         '_MaciDataObjConstructor__assignment_locked_atrribs_err_msg',
         '_MaciDataObjConstructor__assignment_hard_locked_atrribs_err_msg',
         '_MaciDataObjConstructor__ignore_internal_maci_attr_check',
     }
 
     # Generate Dict as a Fresh Copy
     try:
-        dict_data = _deepcopy(vars(MaciDataObj(
+        dict_data = _deepcopy(vars(_MaciDataObj(
                 '',
                 _is_load_request=True,
-                _str_data=py_str_data,
+                _str_data=maci_str_data,
                 _is_str_parse_request=True,
                 attr_name_dedup=attr_name_dedup,
                 encoding=None,
                 **__err_messages,
             )))
     except Load as __err_msg:
-        __err_msg.item = __err_msg.item.replace('\nFILE: ""', "")
+        __err_msg.item = __err_msg.item.replace("\nFile: ''", "")
         raise LoadStrDict(__err_msg.msg, f'{__err_msg.item}') from None
 
     # Remove any Internal Keys
     for remove_key in internal_remove_key_list:
         if remove_key in dict_data: # pragma: no branch
             del dict_data[remove_key]
```

### Comparing `maci-0.3.1/maci/_toml/tomldump.py` & `maci-0.4.0/maci/_toml/tomldump.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # tomldump
 #########################################################################################################
 # Imports
 import tomli_w as _tomli_w
-from ..error import TomlDump
-from .._native.dumpraw import dumpraw as _dumpraw
 from typing import Dict as _Dict
 from typing import Any as _Any
+from .._native.dumpraw import dumpraw as _dumpraw
+from ..error import TomlDump
 
 #########################################################################################################
 # Dump toml file
 def tomldump(
     filename: str,
     data: _Dict[str, _Any],
     *,
@@ -44,9 +44,9 @@
 
     try:
         # Dump data to toml file
         file_data: _Any  # ignore type checker
         with open(filename, write_mode) as file_data:
             _tomli_w.dump(data, file_data, multiline_strings=multi_line_str)
             if write_mode == 'ab': _dumpraw(filename, '', append=True)
-    except TypeError as __err_msg: raise TomlDump(__err_msg, f'\nFILE: "{filename}" \nGot: {repr(data)}')
-    except (FileNotFoundError, OSError) as __err_msg: raise TomlDump(__err_msg, f'\nFILE: "{filename}"')
+    except TypeError as err_msg: raise TomlDump(err_msg, f'\nGot: {repr(filename)} \nGot: {repr(data)}')
+    except (FileNotFoundError, OSError) as err_msg: raise TomlDump(err_msg, f'\nGot: {repr(filename)}')
```

### Comparing `maci-0.3.1/maci/_toml/tomldumpstr.py` & `maci-0.4.0/maci/_toml/tomldumpstr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tomldumpstr
 #########################################################################################################
 # Imports
 import tomli_w as _tomli_w
-from ..error import TomlDumpStr
 from typing import Dict as _Dict
 from typing import Any as _Any
+from ..error import TomlDumpStr
 
 #########################################################################################################
 # Dump toml file
 def tomldumpstr(
     data: _Dict[str, _Any],
     *,
     multi_line_str: bool=False
@@ -21,17 +21,17 @@
     [Example Use]
 
     tomldumpstr(data)
 
     This is using the tomli-w library installed as a dependency from pypi.
     For more information on tomli-w, visit: https://pypi.org/project/tomli-w/
     """
-    __err_msg_type_str_data = "Only dict is allowed for 'data'"
-    __err_msg_type_str_mls = "Only bool is allowed for 'multi_line_str'"
+    err_msg_type_str_data = "Only dict is allowed for 'data'"
+    err_msg_type_str_mls = "Only bool is allowed for 'multi_line_str'"
 
-    if not isinstance(data, dict): raise TomlDumpStr(__err_msg_type_str_data, f'\nGot: {repr(data)}')
-    if not isinstance(multi_line_str, bool): raise TomlDumpStr(__err_msg_type_str_mls, f'\nGot: {repr(multi_line_str)}')
+    if not isinstance(data, dict): raise TomlDumpStr(err_msg_type_str_data, f'\nGot: {repr(data)}')
+    if not isinstance(multi_line_str, bool): raise TomlDumpStr(err_msg_type_str_mls, f'\nGot: {repr(multi_line_str)}')
 
     try:
         # Dump data to toml str
         return _tomli_w.dumps(data, multiline_strings=multi_line_str)
-    except TypeError as __err_msg: raise TomlDumpStr(__err_msg, f'\nGot: {repr(data)}')
+    except TypeError as err_msg: raise TomlDumpStr(err_msg, f'\nGot: {repr(data)}')
```

### Comparing `maci-0.3.1/maci/_toml/tomlload.py` & `maci-0.4.0/maci/_toml/tomlload.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tomlload
 #########################################################################################################
 # Imports
 import tomli as _tomli
-from ..error import TomlLoad
 from typing import Dict as _Dict
 from typing import Any as _Any
+from ..error import TomlLoad
 
 #########################################################################################################
 # Load toml file
 def tomlload(filename: str) -> _Dict[str, _Any]:
     """
     Loads toml data from a file
 
@@ -28,9 +28,9 @@
 
     if not isinstance(filename, str): raise TomlLoad(err_msg_type_file, f'\nGot: {repr(filename)}')
 
     # Load toml file
     try:
         with open(filename, 'rb') as f:
             return _tomli.load(f)
-    except (FileNotFoundError, OSError) as _err_msg: raise TomlLoad(_err_msg, f'\nFILE: "{filename}"')
-    except _tomli.TOMLDecodeError as _err_msg: raise TomlLoad(_err_msg, f'\nFILE: "{filename}"')
+    except (FileNotFoundError, OSError) as err_msg: raise TomlLoad(err_msg, f'\nGot: {repr(filename)}')
+    except _tomli.TOMLDecodeError as err_msg: raise TomlLoad(err_msg, f'\nGot: {repr(filename)}')
```

### Comparing `maci-0.3.1/maci/_toml/tomlloadstr.py` & `maci-0.4.0/maci/_toml/tomlloadstr.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tomlloadstr
 #########################################################################################################
 # Imports
 import tomli as _tomli
-from ..error import TomlLoadStr
 from typing import Dict as _Dict
 from typing import Any as _Any
+from ..error import TomlLoadStr
 
 #########################################################################################################
 # Load toml file
 def tomlloadstr(toml_str_data: str) -> _Dict[str, _Any]:
     """
     Load toml data from a string
 
@@ -18,15 +18,15 @@
 
     tomlloadstr('string with toml data')
 
     This is using the tomli library installed as a dependency from pypi.
     For more information on tomli, visit: https://pypi.org/project/tomli/
     """
     # Error Checks
-    __err_msg_type_str = "Only str is allowed for 'toml_str_data'"
+    err_msg_type_str = "Only str is allowed for 'toml_str_data'"
 
-    if not isinstance(toml_str_data, str): raise TomlLoadStr(__err_msg_type_str, f'\nGot: {repr(toml_str_data)}')
+    if not isinstance(toml_str_data, str): raise TomlLoadStr(err_msg_type_str, f'\nGot: {repr(toml_str_data)}')
 
     # Load toml data from str
     try:
         return _tomli.loads(toml_str_data)
-    except _tomli.TOMLDecodeError as _err_msg: raise TomlLoadStr(_err_msg, f'\nGot: {repr(toml_str_data)}')
+    except _tomli.TOMLDecodeError as err_msg: raise TomlLoadStr(err_msg, f'\nGot: {repr(toml_str_data)}')
```

### Comparing `maci-0.3.1/maci/_xml/xmldump.py` & `maci-0.4.0/maci/_xml/xmldump.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # xmldump
 #########################################################################################################
 # Imports
 from typing import Union as _Union
-from .._native.dumpraw import dumpraw
-from .xmldumpstr import xmldumpstr
-from xml.etree.ElementTree import ElementTree as _ElementTree
-from xml.etree.ElementTree import Element as _Element
+from .._native.dumpraw import dumpraw as _dumpraw
+from .xmldumpstr import xmldumpstr as _xmldumpstr
+from xml.etree.ElementTree import ElementTree as _ElementTree  # nosec: B405  # ignore sec checker - upto dev discretion to run provided maci._defuse_xml_stdlib()
+from xml.etree.ElementTree import Element as _Element  # nosec: B405  # ignore sec checker - upto dev discretion to run provided maci._defuse_xml_stdlib()
 from ..error import XmlDump, DumpRaw
 
 #########################################################################################################
 # Export xml file
 def xmldump(filename: str, data: _Union[_ElementTree, _Element], *, append: bool=False, encoding: _Union[str, None]=None) -> None:
     """
     Exports a new file from xml ElementTree or Element object as xml data
@@ -36,10 +36,10 @@
 
     # Export Data
     try:
         # If ElementTree, convert to Element by getting root
         if isinstance(data, _ElementTree):
             data = data.getroot()
 
-        data_str = xmldumpstr(data)
-        dumpraw(filename, data_str, encoding=encoding, append=append)
-    except DumpRaw as _err_msg: raise XmlDump(_err_msg) from None
+        data_str = _xmldumpstr(data)
+        _dumpraw(filename, data_str, encoding=encoding, append=append)
+    except DumpRaw as err_msg: raise XmlDump(err_msg) from None
```

### Comparing `maci-0.3.1/maci/_xml/xmldumpstr.py` & `maci-0.4.0/maci/_xml/xmldumpstr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # xmldumpstr
 #########################################################################################################
 # Imports
-import xml.etree.ElementTree as _xml_etree
+import xml.etree.ElementTree as _xml_etree  # nosec: B405  # ignore sec checker - upto dev discretion to run provided maci._defuse_xml_stdlib()
 from ..error import XmlDumpStr
 
 #########################################################################################################
 # Export xml str
 def xmldumpstr(data: _xml_etree.Element, *, encoding: str='utf-8') -> str:
     """
     Exports xml Element object to a string
```

### Comparing `maci-0.3.1/maci/_xml/xmlload.py` & `maci-0.4.0/maci/_yaml/yamlload.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-# xmlload
+# yamlload
 #########################################################################################################
 # Imports
+from typing import Any as _Any
 from typing import Union as _Union
-import xml.etree.ElementTree as _xml_etree
-from ..error import XmlLoad
+import yaml as _yaml  # type: ignore  # ignoring type checker for ext lib
+from ..error import YamlLoad
 
 #########################################################################################################
-# Import xml file
-def xmlload(filename: str, *, auto_get_root: bool=True) -> _Union[_xml_etree.Element, _xml_etree.ElementTree]:
+# Import yaml file
+def yamlload(filename: str, *, encoding: _Union[str, None]=None) -> _Any:
     """
-    Imports xml data from a file.
+    Imports yaml data from a file.
 
-    Returns the root Element object of the ElementTree parsed from a xml file by default. Assign the output to var
+    Returns data with matching python data type. Assign the output to var
 
-    Enter xml file location as str to import.
+    Enter yaml file location as str to import.
 
     [Example Use]
 
-    xmlload('path/to/filename.xml')
+    yamlload('path/to/filename.yml')
 
-    This is using the native xml library via etree shipped with the python standard library.
-    For more information on the xml.etree api, visit: https://docs.python.org/3/library/xml.etree.elementtree.html#module-xml.etree.ElementTree
+    This is using the PyYAML framework installed as a dependency from pypi. It is only using the
+    "safe_load" method to protect from untrusted input.
+    For more information on PyYAML, visit: https://pypi.org/project/PyYAML/
     """
     # Error Checks
-    err_msg_type_filename = "Only str is allowed for 'filename'"
-    err_msg_type_auto_get_root = "Only bool is allowed for 'auto_get_root'"
+    err_msg_type_file = "Only str is allowed for 'filename'"
+    err_msg_type_encoding = "Only str|None or valid option is allowed for 'encoding'"
 
-    if not isinstance(filename, str): raise XmlLoad(err_msg_type_filename, f'\nGot: {repr(filename)}')
-    if not isinstance(auto_get_root, bool): raise XmlLoad(err_msg_type_auto_get_root, f'\nGot: {repr(auto_get_root)}')
+    if not isinstance(filename, str): raise YamlLoad(err_msg_type_file, f'\nGot: {repr(filename)}')
+    if not isinstance(encoding, (str, type(None))): raise YamlLoad(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
 
-    # Load File Data
+
+    # Import yaml file
     try:
-        if auto_get_root:
-            return _xml_etree.parse(filename).getroot()
-        return _xml_etree.parse(filename)
-    except (FileNotFoundError, OSError) as __err_msg: raise XmlLoad(__err_msg, f'\nGot: {repr(filename)}')
-    except _xml_etree.ParseError as __err_msg: raise XmlLoad(__err_msg, f'\nGot: {repr(filename)}')
+        with open(filename, 'r', encoding=encoding) as f:
+            return _yaml.safe_load(f)
+    except (FileNotFoundError, OSError) as err_msg: raise YamlLoad(err_msg, f'\nGot: {repr(filename)}')
+    except _yaml.error.YAMLError as err_msg: raise YamlLoad(err_msg, f'\nGot: {repr(filename)}')
+    except LookupError: raise YamlLoad(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
```

### Comparing `maci-0.3.1/maci/_xml/xmlloadstr.py` & `maci-0.4.0/maci/_xml/xmlloadstr.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # xmlloadstr
 #########################################################################################################
 # Imports
-import xml.etree.ElementTree as _xml_etree
+import xml.etree.ElementTree as _xml_etree  # nosec: B405  # ignore sec checker - upto dev discretion to run provided maci._defuse_xml_stdlib()
 from ..error import XmlLoadStr
 
 #########################################################################################################
 # Import xml str
 def xmlloadstr(xml_str_data: str) -> _xml_etree.Element:
     """
     Imports xml data from a string
@@ -21,9 +21,9 @@
     """
     # Error Checks
     err_msg_str = f"Only str is allowed for 'xml_str_data'"
 
     if not isinstance(xml_str_data, str): raise XmlLoadStr(err_msg_str, f'\nGot: {repr(xml_str_data)}')
 
     # Load Str Data
-    try: return _xml_etree.fromstring(str(xml_str_data))
-    except _xml_etree.ParseError as __err_msg: raise XmlLoadStr(__err_msg, f'\nGot: {repr(xml_str_data)}')
+    try: return _xml_etree.fromstring(str(xml_str_data))  # nosec: B314  # ignore sec checker - upto dev discretion to run provided maci._defuse_xml_stdlib()
+    except _xml_etree.ParseError as err_msg: raise XmlLoadStr(err_msg, f'\nGot: {repr(xml_str_data)}')
```

### Comparing `maci-0.3.1/maci/_yaml/yamldump.py` & `maci-0.4.0/maci/_yaml/yamldump.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # yamldump
 #########################################################################################################
 # Imports
 from typing import Any as _Any
 from typing import Union as _Union
-import yaml as _yaml
+import yaml as _yaml  # type: ignore  # ignoring type checker for ext lib
 from ..error import YamlDump
 
 #########################################################################################################
 # Export yaml file
 def yamldump(filename: str, data: _Any, *, append: bool=False, encoding: _Union[str, None]=None) -> None:
     """
     Exports a new file from python data type to yaml data.
@@ -35,10 +35,10 @@
     # Set Write Mode: 'a' = append, 'w' = write
     write_mode = 'a' if append else 'w'
 
     # Export data to yaml file
     try:
         with open(filename, write_mode, encoding=encoding) as f:
             _yaml.safe_dump(data, f)
-    except _yaml.error.YAMLError as __err_msg: raise YamlDump(__err_msg, f'\nGot: {repr(data)}')
-    except (FileNotFoundError, OSError) as __err_msg: raise YamlDump(__err_msg, f'\nGot: {repr(filename)}')
+    except _yaml.error.YAMLError as err_msg: raise YamlDump(err_msg, f'\nGot: {repr(data)}')
+    except (FileNotFoundError, OSError) as err_msg: raise YamlDump(err_msg, f'\nGot: {repr(filename)}')
     except LookupError: raise YamlDump(err_msg_type_encoding, f'\nGot: {repr(encoding)}')
```

### Comparing `maci-0.3.1/maci/_yaml/yamldumpstr.py` & `maci-0.4.0/maci/_yaml/yamldumpstr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # yamldumpstr
 #########################################################################################################
 # Imports
-from typing import Any as __Any
-import yaml as __yaml
+from typing import Any as _Any
+import yaml as _yaml  # type: ignore  # ignoring type checker for ext lib
 from ..error import YamlDumpStr
 
 #########################################################################################################
 # Export yaml str
-def yamldumpstr(data: __Any) -> str:
+def yamldumpstr(data: _Any) -> str:
     """
     Exports python data type to yaml string
 
     Returns a yaml formatted str. Assign the output to var
 
     [Example Use]
 
@@ -19,9 +19,9 @@
 
     This is using the PyYAML framework installed as a dependency from pypi. It is only using the
     "safe_dump" method, which only supports standard YAML tags and cannot represent an arbitrary Python object.
     For more information on PyYAML, visit: https://pypi.org/project/PyYAML/
     
     """
     # Export data to yaml str
-    try: return __yaml.safe_dump(data, stream=None).rstrip() # Strip trailing \n, yaml parser adds this automatically
-    except __yaml.error.YAMLError as __err_msg: raise YamlDumpStr(__err_msg, f'\nGot: {repr(data)}')
+    try: return _yaml.safe_dump(data, stream=None).rstrip() # Strip trailing \n, yaml parser adds this automatically
+    except _yaml.error.YAMLError as err_msg: raise YamlDumpStr(err_msg, f'\nGot: {repr(data)}')
```

### Comparing `maci-0.3.1/maci/_yaml/yamlloadstr.py` & `maci-0.4.0/maci/_yaml/yamlloadstr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # yamlloadstr
 #########################################################################################################
 # Imports
-from typing import Any as __Any
-import yaml as __yaml
+from typing import Any as _Any
+import yaml as _yaml  # type: ignore  # ignoring type checker for ext lib
 from ..error import YamlLoadStr
 
 #########################################################################################################
 # Import yaml str
-def yamlloadstr(yaml_str_data: str) -> __Any:
+def yamlloadstr(yaml_str_data: str) -> _Any:
     """
     Imports yaml data from a string
 
     Returns data with matching python data type. Assign the output to var
 
     Enter yaml string as str to import.
 
@@ -20,15 +20,15 @@
     yamlloadstr('string with yaml data')
 
     This is using the PyYAML framework installed as a dependency from pypi. It is only using the
     "safe_load" method to protect from untrusted input.
     For more information on PyYAML, visit: https://pypi.org/project/PyYAML/
     """
     # Error Checks
-    __err_msg_type_str = "Only str is allowed for 'yaml_str_data'"
+    err_msg_type_str = "Only str is allowed for 'yaml_str_data'"
 
-    if not isinstance(yaml_str_data, str): raise YamlLoadStr(__err_msg_type_str, f'\nGot: {repr(yaml_str_data)}')
+    if not isinstance(yaml_str_data, str): raise YamlLoadStr(err_msg_type_str, f'\nGot: {repr(yaml_str_data)}')
 
     # Import yaml str
     try:       
-        return __yaml.safe_load(yaml_str_data)
-    except __yaml.error.YAMLError as __err_msg: raise YamlLoadStr(__err_msg, f'\nGot: {yaml_str_data}')
+        return _yaml.safe_load(yaml_str_data)
+    except _yaml.error.YAMLError as err_msg: raise YamlLoadStr(err_msg, f'\nGot: {yaml_str_data}')
```

### Comparing `maci-0.3.1/maci/data.py` & `maci-0.4.0/maci/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 # Imports
 
 # MaciDataObj
 from ast import literal_eval as _literal_eval
 from datetime import datetime as _datetime
 from datetime import date as _datetime_date
 from datetime import time as _datetime_time
-from copy import deepcopy
+from copy import deepcopy as _deepcopy
 from typing import Any as _Any
 from typing import Dict as _Dict
 from typing import List as _List
 from typing import Union as _Union
 from typing import Optional as _Optional
 from typing import NamedTuple as _NamedTuple
 from typing import Set as _Set
 from typing import Callable as _Callable
 from .error import Load, GeneralError, Hint
 # Dump Function
 from io import StringIO as _StringIO
-from typing import NewType as _NewType
+from typing import TypeVar as _TypeVar
 from ._native.dumpraw import dumpraw as _dumpraw
 from ._native.cleanformat import cleanformat as _cleanformat
 from .error import Dump, DumpRaw, DumpStr
 
 #########################################################################################################
 # Assignment Glyphs
 class _Glyphs(_NamedTuple):
@@ -257,21 +257,29 @@
         _assignment_glyphs_for_ref_hard_lock_checks = {__assignment_glyphs.ref_hard_lock, __assignment_glyphs.mh, __assignment_glyphs.hm}
         _assignment_glyphs_for_lock_checks = {__assignment_glyphs.lock, __assignment_glyphs.l}
         _assignment_glyphs_for_hard_lock_checks = {__assignment_glyphs.hard_lock, __assignment_glyphs.h}
         _assignment_glyphs_for_mixed_cases = __assignment_glyphs.get_mixed_case_set()
 
 
         # Main File/Str Loop
-        # To display correct line number, ensure to add +1 when ready to raise. Keeping
-        # constant +1 track will add latency to loop, so only provide as needed
-        for line_num,__file_data_line in enumerate(file_data):
+        # To display correct line number start=1
+        for line_num,__file_data_line in enumerate(file_data, start=1):
 
             # Set Skip Marker
-            try: __skip_marker = __file_data_line[0]
+            try:
+                __skip_marker = __file_data_line[0]
+                potential_name_char = __file_data_line.lstrip()[0]
             except IndexError: __skip_marker = ''
+            else:
+                # Check if there is a leading blank with data on same line
+                if (__skip_marker in __skip_markers) and (potential_name_char not in __skip_markers) and (__is_building_data_sw == False):
+                    raise Load(
+                            py_syntax_err_msg,
+                            f'\nFile: {repr(filename)} \nLine: {line_num} \nGot: {repr(__file_data_line)}'
+                        )
 
             # Skip Any Comments, Blanks, and New Lines. Do not skip during a muli-line build
             if (__is_building_data_sw == False) and (__skip_marker in __skip_markers): continue
 
             # Set Assignment Glyph: Checks valid syntax, and checks if glyph is uppercase
             if (__is_building_data_sw == False):
                 for _glyph in __assignment_glyphs:
@@ -305,59 +313,65 @@
 
                 if not __is_building_data_sw:
 
                     # Check if Value Empty
                     if __file_data_line.partition(__assignment_glyph)[2].strip() == '':
                         raise Load(
                             py_syntax_err_msg,
-                            f'\nFILE: "{filename}" \nLINE: {line_num+1} \nATTR_NAME: {__file_data_line.partition(__assignment_glyph)[0].strip()} \nGOT: {__file_data_line}'
+                            f'\nFile: {repr(filename)} \nLine: {line_num} \nAttr: {__file_data_line.partition(__assignment_glyph)[0].strip()} \nGot: {repr(__file_data_line)}'
                         )
                     
                     __current_assignment_glyph = __assignment_glyph.lower()
                     __var_token = __file_data_line.partition(__assignment_glyph)[0].strip()
                     __value_token = __file_data_line.partition(__assignment_glyph)[2].strip()
                     __value_token_multi = __file_data_line.partition(__assignment_glyph)[2].split()[0].strip()
 
                     # Set Last Token with Accommodation to Multi-Line String
                     if __file_data_line.partition(__assignment_glyph)[2].strip()[-3:] in __start_markers:
                         __last_token = __file_data_line.partition(__assignment_glyph)[2].strip()[-3:]
                     else:
                         __last_token = __file_data_line.partition(__assignment_glyph)[2].strip()[-1]
                     
                     try: __start_skip_token = __file_data_line.split(__assignment_glyph)[1].split()[1][0].strip()
-                    except IndexError: __start_skip_token = ''
+                    except IndexError: __start_skip_token = ''  # nosec: B105  # not password
                 
                 # Collect End Token if in Build
                 if __is_building_data_sw:
                     try:
                         if __file_data_line[0] in __end_markers:
                             __end_token = __file_data_line[0]
                         elif __file_data_line[0:3] in __end_markers:
                             __end_token = __file_data_line[0:3]
-                        else: __end_token = ''
-                    except IndexError: __end_token = ''
+                        else: __end_token = ''  # nosec: B105  # not password
+                    except IndexError: __end_token = ''  # nosec: B105  # not password
                 
                 # Verify Assignment Glyph is Not Attr Reference for Multiline Build Check
                 is_attr_reference_glyph = False
                 if __current_assignment_glyph in _assignment_glyphs_for_all_ref_checks:
                     is_attr_reference_glyph = True
 
-                # START BUILD: Check if value in file line is only Start Marker. Check if Multiline or Single Line
+                
+                ### START BUILD: Check if value in file line is only Start Marker. Check if Multiline or Single Line
                 if (__value_token_multi in __start_markers) \
                 and ((__last_token in __start_markers) or (__start_skip_token[0] in __skip_markers)) \
                 and (__is_building_data_sw == False) \
                 and not (is_attr_reference_glyph):
                     
                     # Check if Attr Dedup
                     if (self.__attrib_name_dedup) and (hasattr(self, __var_token)):
-                            raise Load(name_preexists_err_msg, f'\nFILE: "{filename}" \nATTR_NAME: {__var_token}')
+                            raise Load(name_preexists_err_msg, f'\nFile: {repr(filename)} \nLine: {line_num} \nAttr: {__var_token}')
 
                     # Check for Comment
                     if __skip_markers[2] in __value_token:
                         __value_token = __value_token.partition(__skip_markers[2])[0].strip()
+                    
+                    # Check if starting a build with no remaining lines to read
+                    if (len(file_data) == line_num):
+                        raise Load(py_syntax_err_msg, f'\nFile: {repr(filename)} \nLine: {line_num} \nAttr: {__var_token}')
+                    
                     # Set First Value
                     __build_data = __value_token
 
                     # Swap ignore type if multi-str. If triple-singles, then ignore triple-doubles and vice-versa
                     if __ignore_multistr_markers[0] == __value_token: __ignore_multistr_marker = __ignore_multistr_markers[1]
                     if __ignore_multistr_markers[1] == __value_token: __ignore_multistr_marker = __ignore_multistr_markers[0]
 
@@ -365,15 +379,15 @@
                     __is_building_data_sw = True
                     __body_build_data_sw = True
                     __end_data_build_sw = True
                     if __value_token in __end_multistr_markers: # pragma: no branch
                         __end_markers_build = __end_multistr_markers
                     continue
 
-                # END BUILD: Check if line of file is an End Data Build Marker. Import Built Data Type if Valid. Check if EOF in case File Missing End Marker.
+                ### END BUILD: Check if line of file is an End Data Build Marker. Import Built Data Type if Valid. Check if EOF in case File Missing End Marker.
                 elif (__end_data_build_sw) and (((__end_token in __end_markers_build) and (not __end_token == __ignore_multistr_marker)) or (f"{__eof_marker}" == f"{__file_data_line}")):
                     __build_data += f"\n{__file_data_line}"
 
                     try:
                         # Assign Attr
                         setattr(self, __var_token, _literal_eval(__build_data))
 
@@ -381,34 +395,35 @@
                         if __current_assignment_glyph in _assignment_glyphs_for_lock_checks:
                             self.__assignment_locked_attribs.add(__var_token)
 
                         # Check if Attr is Hard Locked from Re-Assignment
                         if __current_assignment_glyph in _assignment_glyphs_for_hard_lock_checks:
                             self.__assignment_hard_locked_attribs.add(__var_token)
 
-                    except SyntaxError: raise Load(py_syntax_err_msg, f'\nFILE: "{filename}" \nATTR_NAME: {__var_token}')
+                    except SyntaxError: raise Load(py_syntax_err_msg, f'\nFile: {repr(filename)} \nLine: {line_num} \nAttr: {__var_token}')
 
                     # Turn OFF/UPDATE Data Build Switches
                     __is_building_data_sw = False
                     __body_build_data_sw = False
                     __end_data_build_sw = False
                     __build_data = ''
                     __end_markers_build = __end_markers
                     continue
 
-                # CONT BUILD: Continue to Build Data
+                ### CONT BUILD: Continue to Build Data
                 elif __body_build_data_sw:
                     __build_data += f"\n{__file_data_line}"
                     
-                # IMPORT SINGLE LINE VALUES: If not multiline, assume single
+                
+                ### IMPORT SINGLE LINE VALUES: If not multiline, assume single
                 else:
                     try:
                         # Check if Attr Dedup
                         if (self.__attrib_name_dedup) and (hasattr(self, __var_token)):
-                            raise Load(name_preexists_err_msg, f'\nFILE: "{filename}" \nATTR_NAME: {__var_token}')
+                            raise Load(name_preexists_err_msg, f'\nFile: {repr(filename)} \nLine: {line_num} \nAttr: {__var_token}')
                         
                         # Check if Attr is a Reference to Another Attr's Value for Assignment. Ignore Comments
                         if __current_assignment_glyph in _assignment_glyphs_for_ref_checks:
                             __value_token = f"{__value_token} "[:__value_token.find(__skip_markers[2])].rstrip()
                             setattr(self, __var_token, getattr(self, __value_token))
                             self.__assigned_src_reference_attr_map[__var_token] = __value_token
                             self.__assigned_dst_reference_attr_map.setdefault(__value_token, {}).setdefault(__var_token, __value_token)
@@ -440,47 +455,47 @@
                             self.__assignment_locked_attribs.add(__var_token)
 
                         # Check if Attr is Hard Locked from Re-Assignment
                         if __current_assignment_glyph in _assignment_glyphs_for_hard_lock_checks:
                             self.__assignment_hard_locked_attribs.add(__var_token)
                         
                     except AttributeError:
-                        # REF_NAME: Ignores Comments to Display Attr Reference Name
+                        # Reference Name: Ignores Comments to Display Attr Reference Name
                         raise Load(
                             name_reference_does_not_exist,
-                            f'\nFILE: "{filename}" \nATTR_NAME: {__var_token} \nREF_NAME: {f"{__value_token} "[:__value_token.find(__skip_markers[2])].rstrip()}'
+                            f'\nFile: {repr(filename)} \nLine: {line_num} \nAttr: {__var_token} \nMap_Name: {f"{__value_token} "[:__value_token.find(__skip_markers[2])].rstrip()}'
                         )
                     except (ValueError, SyntaxError):
                         # Check if datetime format and set attr, else raise exception
                         datetime_format =_date_time_parse_check(__value_token)
                         if datetime_format is not None:
                             # Assign Attr to datetime object
                             setattr(self, __var_token, datetime_format)
                         else:
-                            raise Load(py_syntax_err_msg, f'\nFILE: "{filename}" \nATTR_NAME: {__var_token}')
+                            raise Load(py_syntax_err_msg, f'\nFile: {repr(filename)} \nLine: {line_num} \nAttr: {__var_token}')
 
-            else: raise Load(py_syntax_err_msg, f'\nFILE: "{filename}" \nLINE: {line_num+1}')
+            else: raise Load(py_syntax_err_msg, f'\nFile: {repr(filename)} \nLine: {line_num}')
     
 
     def __setattr__(self, _name: str, _new_value: _Any) -> None:
         # Check if Attr Already Exists, if so, Collect Original Value
         if hasattr(self, _name):
             _orig_value = self.__dict__.get(_name)
             
         # Release Attribute Reference if Name is Re-Assigned
         if hasattr(self, _name):
             self.__reference_deletion_check(_name, _src_ref_list=True)
 
         # Protect Internal List/Reference Attrs and Methods from Re-Assignment
         if hasattr(self, _name) and (_name in _MaciDataObjConstructor.__internal_check_lists_setattr_maci_names):
-            raise GeneralError('Cannot re-assign internal MaciDataObj attribute name!', f'\nATTR_NAME: "{_name}"')
+            raise GeneralError('Cannot re-assign internal MaciDataObj attribute name!', f'\nAttr: {repr(_name)}')
         
         # Protect Internal Method Names from Re-Assignment. Can be switched OFF by User
         if hasattr(self, _name) and (_name in _MaciDataObjConstructor.__internal_check_lists_setattr_maci_methods) and (not self.__ignore_internal_maci_attr_check):
-            raise GeneralError('Cannot re-assign internal MaciDataObj method name!', f'\nMETHOD_NAME: "{_name}"')
+            raise GeneralError('Cannot re-assign internal MaciDataObj method name!', f'\nMethod_Name: {repr(_name)}')
 
 
         # Always Assign Value 
         self.__dict__[_name] = _new_value
 
 
         # If attr was added to lock/hard_lock list after first assignment, assign orig value back, and raise exception
@@ -488,23 +503,23 @@
 
         # General Lock Protection
         if hasattr(self, '_MaciDataObjConstructor__assignment_locked_attribs'): # pragma: no branch
             if _name in self.__assignment_locked_attribs:
                 # PROTECT ORIGINAL VALUE
                 self.__dict__[_name] = _orig_value
                 # RAISE EXCEPTION
-                raise GeneralError(self.__assignment_locked_atrribs_err_msg, f'\nATTR_NAME: "{_name}"')
+                raise GeneralError(self.__assignment_locked_atrribs_err_msg, f'\nAttr: {repr(_name)}')
 
         # Hard Lock Protection
         if hasattr(self, '_MaciDataObjConstructor__assignment_hard_locked_attribs'):
             if _name in self.__assignment_hard_locked_attribs:
                 # PROTECT ORIGINAL VALUE
                 self.__dict__[_name] = _orig_value
                 # RAISE EXCEPTION
-                raise GeneralError(self.__assignment_hard_locked_atrribs_err_msg, f'\nATTR_NAME: "{_name}"')
+                raise GeneralError(self.__assignment_hard_locked_atrribs_err_msg, f'\nAttr: {repr(_name)}')
         
         # Always Re-Reference Attr New Value if Source not Locked
         if hasattr(self, '_MaciDataObjConstructor__assigned_dst_reference_attr_map'):
             if _name in self.__assigned_dst_reference_attr_map:
                 for key in self.__assigned_dst_reference_attr_map[_name]:
                     collected_references = []
                     collected_references.append(key)
@@ -521,30 +536,30 @@
 
 
                     # Assign New Value to All Child or Chained References and Verify None are Locked
                     for ref_name in collected_references:
                         # If Source is Locked, Block Update
                         _is_locked = ref_name in self.__assignment_locked_attribs
                         _is_hard_locked = ref_name in self.__assignment_hard_locked_attribs
-                        if _is_locked: raise GeneralError(self.__assignment_locked_atrribs_err_msg, f'\nATTR_NAME: "{ref_name}"')
-                        if _is_hard_locked: raise GeneralError(self.__assignment_hard_locked_atrribs_err_msg, f'\nATTR_NAME: "{ref_name}"')
+                        if _is_locked: raise GeneralError(self.__assignment_locked_atrribs_err_msg, f'\nAttr: {repr(ref_name)}')
+                        if _is_hard_locked: raise GeneralError(self.__assignment_hard_locked_atrribs_err_msg, f'\nAttr: {repr(ref_name)}')
 
                         # Update Reference(s) to New Value
                         self.__dict__[ref_name] = _new_value
     
     
     def __delattr__(self, _name: str) -> None:
         # Protect Internal List/Reference Attrs from Deletion
         if _name in _MaciDataObjConstructor.__internal_check_lists_delattr:
-            raise GeneralError('Cannot delete internal MaciDataObj attribute name!', f'\nATTR_NAME: "{_name}"')
+            raise GeneralError('Cannot delete internal MaciDataObj attribute name!', f'\nAttr: {repr(_name)}')
 
         # Protect Hard Locked Attr from Deletion
         if _name in self.__assignment_hard_locked_attribs:
             # RAISE EXCEPTION
-            raise GeneralError(self.__assignment_hard_locked_atrribs_err_msg, f'\nATTR_NAME: "{_name}"')
+            raise GeneralError(self.__assignment_hard_locked_atrribs_err_msg, f'\nAttr: {repr(_name)}')
 
         # Release Attribute from Lock & Reference List if Name is Deleted
         if hasattr(self, _name): # pragma: no branch
             self.__reference_deletion_check(_name, _src_ref_list=True, _dst_ref_list=True, _lock_list=True)
 
         # Allow Normal Deletion
         super().__delattr__(_name)
@@ -557,22 +572,22 @@
         """
         # Error Checks
         __err_msg_attr_name_str = "Only str is allowed for attr_name"
         __err_msg_attr_name_exist = "Hard locked attribute name does not exist! Must be created first to lock"
         __err_msg_attr_name_locked = "Attribute name already hard locked! Cannot be re-locked once locked"
         __err_msg_attr_name_other_lock = "Attribute name exists with other lock (lock_attr) already! Cannot be locked with multiple locks"
 
-        if not isinstance(attr_name, str): raise GeneralError(__err_msg_attr_name_str, f'\nATTR_NAME: "{attr_name}"')
-        if not attr_name in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nATTR_NAME: "{attr_name}"')
+        if not isinstance(attr_name, str): raise GeneralError(__err_msg_attr_name_str, f'\nAttr: {repr(attr_name)}')
+        if not attr_name in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nAttr: {repr(attr_name)}')
 
         # Assign Attr to Locked Tuple if Does Not Preexist
         if attr_name in self.__assignment_hard_locked_attribs:
-            raise GeneralError(__err_msg_attr_name_locked, f'\nATTR_NAME: "{attr_name}"')
+            raise GeneralError(__err_msg_attr_name_locked, f'\nAttr: {repr(attr_name)}')
         if attr_name in self.__assignment_locked_attribs:
-            raise GeneralError(__err_msg_attr_name_other_lock, f'\nATTR_NAME: "{attr_name}"')
+            raise GeneralError(__err_msg_attr_name_other_lock, f'\nAttr: {repr(attr_name)}')
 
         self.__assignment_hard_locked_attribs.add(attr_name)
 
 
     @_rename_exc_name_to_user_object_name
     def lock_attr(self, attr_name: str) -> None:
         """
@@ -580,42 +595,42 @@
         """
         # Error Checks
         __err_msg_attr_name_str = "Only str is allowed for attr_name"
         __err_msg_attr_name_exist = "Locked attribute name does not exist! Must be created first to lock"
         __err_msg_attr_name_locked = "Attribute name already locked! Cannot be re-locked once locked"
         __err_msg_attr_name_other_lock = "Attribute name exists with other lock (hard_lock_attr) already! Cannot be locked with multiple locks"
 
-        if not isinstance(attr_name, str): raise GeneralError(__err_msg_attr_name_str, f'\nATTR_NAME: "{attr_name}"')
-        if not attr_name in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nATTR_NAME: "{attr_name}"')
+        if not isinstance(attr_name, str): raise GeneralError(__err_msg_attr_name_str, f'\nAttr: {repr(attr_name)}')
+        if not attr_name in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nAttr: {repr(attr_name)}')
 
         # Assign Attr to Locked List if Does Not Preexist
         if attr_name in self.__assignment_locked_attribs:
-            raise GeneralError(__err_msg_attr_name_locked, f'\nATTR_NAME: "{attr_name}"')
+            raise GeneralError(__err_msg_attr_name_locked, f'\nAttr: {repr(attr_name)}')
         if attr_name in self.__assignment_hard_locked_attribs:
-            raise GeneralError(__err_msg_attr_name_other_lock, f'\nATTR_NAME: "{attr_name}"')
+            raise GeneralError(__err_msg_attr_name_other_lock, f'\nAttr: {repr(attr_name)}')
 
         self.__assignment_locked_attribs.add(attr_name)
 
 
     @_rename_exc_name_to_user_object_name
     def unlock_attr(self, attr_name: str) -> None:
         """
         Unlocks a attribute name from locked re-assignment
         """
         # Error Checks
         __err_msg_attr_name_str = "Only str is allowed for attr_name"
         __err_msg_attr_name_exist = "Unlock attribute name does not exist"
         __err_msg_attr_name_exist_unlock = "Unlock attribute name does not exist in lock! Could not find name to unlock"
 
-        if not isinstance(attr_name, str): raise GeneralError(__err_msg_attr_name_str, f'\nATTR_NAME: "{attr_name}"')
-        if not attr_name in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nATTR_NAME: "{attr_name}"')
+        if not isinstance(attr_name, str): raise GeneralError(__err_msg_attr_name_str, f'\nAttr: {repr(attr_name)}')
+        if not attr_name in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nAttr: {repr(attr_name)}')
 
         # Remove Attr from Locked List
         try: self.__assignment_locked_attribs.remove(attr_name)
-        except KeyError: raise GeneralError(__err_msg_attr_name_exist_unlock, f'\nATTR_NAME: "{attr_name}"')
+        except KeyError: raise GeneralError(__err_msg_attr_name_exist_unlock, f'\nAttr: {repr(attr_name)}')
 
 
     @_rename_exc_name_to_user_object_name
     def map_attr(self, child_attr: str, parent_attr: str) -> None:
         """
         Create a link of an attribute name to another attribute name
 
@@ -626,20 +641,20 @@
         """
         # Error Checks
         __err_msg_attr_name_str = "Only str is allowed for 'child_attr'"
         __err_msg_reference_name_str = "Only str is allowed for 'parent_attr'"
         __err_msg_attr_name_exist = f"Attribute name '{child_attr}' does not exist! Must be created first to assign to parent attribute"
         __err_msg_reference_name_exist = f"Attribute name '{parent_attr}' does not exist! Cannot assign value to child attribute"
 
-        if not isinstance(child_attr, str): raise GeneralError(__err_msg_attr_name_str, f'\nATTR_NAME: "{child_attr}"')
-        if not isinstance(parent_attr, str): raise GeneralError(__err_msg_reference_name_str, f'\nATTR_NAME: "{parent_attr}"')
+        if not isinstance(child_attr, str): raise GeneralError(__err_msg_attr_name_str, f'\nAttr: {repr(child_attr)}')
+        if not isinstance(parent_attr, str): raise GeneralError(__err_msg_reference_name_str, f'\nAttr: {repr(parent_attr)}')
 
         # Look up if Attr or Reference Name Exists
-        if not child_attr in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nATTR_NAME: "{child_attr}"')
-        if not parent_attr in self.__dict__: raise GeneralError(__err_msg_reference_name_exist, f'\nATTR_NAME: "{parent_attr}"')
+        if not child_attr in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nAttr: {repr(child_attr)}')
+        if not parent_attr in self.__dict__: raise GeneralError(__err_msg_reference_name_exist, f'\nAttr: {repr(parent_attr)}')
 
         # Set Value to Reference Value
         setattr(self, child_attr, getattr(self, parent_attr))
     
         # Assign Attr Name to Reference Name in Reference Maps
         self.__assigned_src_reference_attr_map[child_attr] = parent_attr
         self.__assigned_dst_reference_attr_map.setdefault(parent_attr, {}).setdefault(child_attr, parent_attr)
@@ -655,22 +670,22 @@
         If it is a parent attr, all child links will be detached from that parent
         """
         # Error Checks
         __err_msg_attr_name_str = "Only str is allowed for 'attr_name'"
         __err_msg_attr_name_exist = f"Attribute name does not exist! Must be created first and linked to an attribute to unlink"
         __err_msg_reference_name_exist = f"Attribute name is not mapped to anything! Cannot unmap attribute"
 
-        if not isinstance(attr_name, str): raise GeneralError(__err_msg_attr_name_str, f'\nGOT: {repr(attr_name)}')
+        if not isinstance(attr_name, str): raise GeneralError(__err_msg_attr_name_str, f'\nGot: {repr(attr_name)}')
 
         # Look up if Attr or Reference Name Exists at all or in Reference Maps
-        if not attr_name in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nGOT: {repr(attr_name)}')
+        if not attr_name in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nGot: {repr(attr_name)}')
 
         if (attr_name not in self.__assigned_src_reference_attr_map) \
         and (attr_name not in self.__assigned_dst_reference_attr_map):
-            raise GeneralError(__err_msg_reference_name_exist, f'\nATTR_NAME: {attr_name}')
+            raise GeneralError(__err_msg_reference_name_exist, f'\nAttr: {attr_name}')
         
         self.__reference_deletion_check(attr_name, _src_ref_list=True, _dst_ref_list=True, _ref_removal_request=True)
 
 
     @_rename_exc_name_to_user_object_name
     def is_parent_map(self, attr_name: str) -> bool:
         """
@@ -678,16 +693,16 @@
 
         Returns: True if Parent, and False if not
         """
         # Error Checks
         __err_msg_attr_name_str = "Only str is allowed for 'attr_name'"
         __err_msg_attr_name_exist = f"Attribute name does not exist! Must be created first to check link type"
 
-        if not isinstance(attr_name, str): raise GeneralError(__err_msg_attr_name_str, f'\nGOT: {repr(attr_name)}')
-        if not attr_name in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nGOT: {repr(attr_name)}')
+        if not isinstance(attr_name, str): raise GeneralError(__err_msg_attr_name_str, f'\nGot: {repr(attr_name)}')
+        if not attr_name in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nGot: {repr(attr_name)}')
 
         # Check Link Type
         return (attr_name in self.__assigned_dst_reference_attr_map)
     
 
     @_rename_exc_name_to_user_object_name
     def is_child_map(self, attr_name: str) -> bool:
@@ -696,16 +711,16 @@
 
         Returns: True if Child, and False if not
         """
         # Error Checks
         __err_msg_attr_name_str = "Only str is allowed for 'attr_name'"
         __err_msg_attr_name_exist = f"Attribute name does not exist! Must be created first to check link type"
 
-        if not isinstance(attr_name, str): raise GeneralError(__err_msg_attr_name_str, f'\nGOT: {repr(attr_name)}')
-        if not attr_name in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nGOT: {repr(attr_name)}')
+        if not isinstance(attr_name, str): raise GeneralError(__err_msg_attr_name_str, f'\nGot: {repr(attr_name)}')
+        if not attr_name in self.__dict__: raise GeneralError(__err_msg_attr_name_exist, f'\nGot: {repr(attr_name)}')
 
         # Check Link Type
         return (attr_name in self.__assigned_src_reference_attr_map)
 
 
     def __reference_deletion_check(
         self,
@@ -789,15 +804,15 @@
 
         attr_child == attr_parent
 
         Parent map will be -> 'parent_map': {'attr_parent': {'attr_child': 'attr_parent'}}
 
         Child map will be -> 'child_map': {'attr_child': 'attr_parent'}
         """
-        return {'parent_maps': deepcopy(self.__assigned_dst_reference_attr_map), 'child_maps': deepcopy(self.__assigned_src_reference_attr_map)}
+        return {'parent_maps': _deepcopy(self.__assigned_dst_reference_attr_map), 'child_maps': _deepcopy(self.__assigned_src_reference_attr_map)}
 
 
     @_rename_exc_name_to_user_object_name
     def get_parent_maps(self) -> _Dict[str, _Dict[str, str]]:
         """
         Get all Parent Links
 
@@ -807,15 +822,15 @@
 
         attr_parent = 'some value'
 
         attr_child == attr_parent
 
         Parent map will be -> {'attr_parent': {'attr_child': 'attr_parent'}}
         """
-        return deepcopy(self.__assigned_dst_reference_attr_map)
+        return _deepcopy(self.__assigned_dst_reference_attr_map)
 
 
     @_rename_exc_name_to_user_object_name
     def get_parent_map_chains(self, parent_attr: _Optional[str]=None, *, dup_link_check: bool=True) -> _Union[_Dict[str, _List[str]], _List[str]]:
         """
         Get Parent Map Chains
 
@@ -850,16 +865,16 @@
         """
         # Error Checks
         err_msg_parent_name_type = "Only str|None is allowed for 'parent_attr'"
         err_msg_dup_link_chk_type = "Only bool is allowed for 'dup_link_check'"
         err_msg_chain_conflict = f"Cannot build chain due to duplicate child name(s) already linked to parent! Disable this check with 'dup_link_check'"
         err_msg_parent_not_found = f"Name '{parent_attr}' does not have a chain that exists!"
 
-        if not isinstance(parent_attr, (str, type(None))): raise GeneralError(err_msg_parent_name_type, f'\nGOT: {parent_attr}')
-        if not isinstance(dup_link_check, bool): raise GeneralError(err_msg_dup_link_chk_type, f'\nGOT: {dup_link_check}')
+        if not isinstance(parent_attr, (str, type(None))): raise GeneralError(err_msg_parent_name_type, f'\nGot: {parent_attr}')
+        if not isinstance(dup_link_check, bool): raise GeneralError(err_msg_dup_link_chk_type, f'\nGot: {dup_link_check}')
 
         # Always use new objects
         all_parent_chains = {}
         chain_link_tracker = []
 
         # Seek and Build the chains that exist
         for child in self.__assigned_src_reference_attr_map:
@@ -907,15 +922,15 @@
                         all_parent_chains[parent_check] = chain_link_build
                         break
 
         # Check if parent_name was specified but not found
         if (parent_attr is not None) and (parent_attr not in all_parent_chains):
             raise GeneralError(
                 err_msg_parent_not_found,
-                f"\nGOT: {parent_attr}"
+                f"\nGot: {parent_attr}"
             )
 
         # Return single parent chain if specified, otherwise continue build
         if parent_attr in all_parent_chains:
             return all_parent_chains[parent_attr]
 
         # Return all chains if no parent specified
@@ -933,15 +948,15 @@
 
         attr_parent = 'some value'
 
         attr_child == attr_parent
 
         Child map will be -> {'attr_child': 'attr_parent'}
         """
-        return deepcopy(self.__assigned_src_reference_attr_map)
+        return _deepcopy(self.__assigned_src_reference_attr_map)
 
 
 #########################################################################################################
 # Main MaciDataObj Reference
 
 # Meta for structure references
 class __MaciDataObj(type):
@@ -994,32 +1009,45 @@
                 _assignment_locked_atrribs_err_msg=_assignment_locked_atrribs_err_msg,
                 _assignment_hard_locked_atrribs_err_msg=_assignment_hard_locked_atrribs_err_msg,
                 _is_str_parse_request=_is_str_parse_request,
                 _str_data=_str_data,
                 _is_build_request=_is_build_request,
                 _ignore_internal_maci_attr_check=_ignore_internal_maci_attr_check,
             )
+    
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, MaciDataObj):
+            return NotImplemented
+        else:
+            # Compare str repr of maci objects, which contain actual attrs & values in strings
+            return str(self) == str(other)
+
+    def __bool__(self) -> bool:
+        skip_name_keys = ('_MaciDataObjConstructor', '__maci_obj_format_id')
+        if [attr for attr in vars(self) if not attr.startswith(skip_name_keys)]:
+            return True
+        return False
 
     def __repr__(self) -> str:
         skip_name_keys = ('_MaciDataObjConstructor', '__maci_obj_format_id')
-        build_repr = ', '.join([f"{name}={value!r}" for name,value in vars(self).items() if not name.startswith(skip_name_keys)])
+        build_repr = ', '.join(f"{name}={value!r}" for name,value in vars(self).items() if not name.startswith(skip_name_keys))
         return f"{type(self).__name__}({build_repr})"
 
 
 #########################################################################################################
 # Main Dump Function
 
-# Hinting reference name for "CustomClass" to denote a CustomClass can be used to dump data
-CustomClass = _NewType('CustomClass', object)
+# Hinting reference name for "ClassObject" to denote a ClassObject can be used to dump data
+ClassObject = _TypeVar('ClassObject')
 
 def __dump_data(
     *,
     _is_string_request: bool=False,
     filename: str,
-    data: _Any, # MaciDataObj, dict, CustomClass
+    data: _Any, # objects allowed: MaciDataObj, dict, ClassObject - ignoring type checker
     append: bool=False,
     indent_level: int=1,
     indentation_on: bool=True,
     multi_line_str: bool=False,
     encoding: _Union[str, None]=None,
     class_attrs: bool=False,
     private_attrs: bool=False,
@@ -1046,18 +1074,18 @@
     __err_msg_no_attrs_found = __err_msg_no_attrs_found
 
     if _is_string_request:
         # Set Error Type
         DumpStrError = DumpStr
         # Set Values
         filename = ''
-        __err_msg_invalid_maciobj_item = f'\nDATA: {data}'
+        __err_msg_invalid_maciobj_item = f'\nGot: {repr(data)}'
     else:
         DumpError = Dump
-        __err_msg_invalid_maciobj_item = f'\nFILE: "{filename}" \nDATA: {data}'
+        __err_msg_invalid_maciobj_item = f'\nFile: {repr(filename)} \nGot: {repr(data)}'
 
     if isinstance(data, type(MaciDataObj)):
         if _is_string_request: raise DumpStrError(__err_msg_invalid_maciobj, __err_msg_invalid_maciobj_item)
         raise DumpError(__err_msg_invalid_maciobj, __err_msg_invalid_maciobj_item)
 
 
     # Setup
@@ -1079,15 +1107,15 @@
             h=__assignment_glyphs.hard_lock,
             l=__assignment_glyphs.lock,
             mh=__assignment_glyphs.ref_hard_lock,
             ml=__assignment_glyphs.ref_lock,
         )
 
     
-    ### MACI DATA: Check if MaciDataObj ###
+    ### MACI Got: Check if MaciDataObj ###
 
     # Build Out Data
     if (isinstance(data, MaciDataObj)) and (data.__maci_obj_format_id__ == __maci_obj_format_id_match):
         for key,value in data.__dict__.items():
             # If Match Prefixes, Skip
             if not key.startswith(__skip_object_key):
                 # Check Glyph Type and Build Accordingly
@@ -1420,18 +1448,18 @@
     __write_mode_allowed_list = ['w', 'a']
     try:
         # Write New File Mode
         if write_mode == 'w':
             _dumpraw(filename, data, encoding=encoding)
         # Append Append File Mode
         if write_mode == 'a':
-            _dumpraw(filename, data, append=True, encoding=encoding)        
+            _dumpraw(filename, data, append=True, encoding=encoding)
         # Raise Exception if No Match - Dev Check
         if not write_mode in __write_mode_allowed_list: # pragma: no cover
-            raise Dump(__err_msg_write_mode, f'\nGot: {write_mode}')
+            raise Dump(__err_msg_write_mode, f'\nGot: {repr(write_mode)}')
     except DumpRaw as __err_msg: raise Dump(__err_msg, '')
 
 
 # Setup Multi-String
 def __setup_multi_string(key: str, assignment_glyph: str, value: str,) -> str:
     is_set_start_new_line = '' if value.startswith('\n') else '\n'
     is_set_end_new_line = '' if value.endswith('\n') else '\n'
```

### Comparing `maci-0.3.1/maci/error.py` & `maci-0.4.0/maci/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# error - Contains exception names and handling
+# error - Contains maci and other exception names for handling
 """
-Contains exception names for handling
+Contains maci and other exception names for handling
 """
 from typing import Any as _Any
 
 # Base Exception
 class MaciError(Exception):
     """
     maci base exception
```

### Comparing `maci-0.3.1/maci.egg-info/PKG-INFO` & `maci-0.4.0/maci.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maci
-Version: 0.3.1
+Version: 0.4.0
 Summary: The easy to use library for your data, configuration, and save files
 Author: aaronater10
 Author-email: dev_admin@dunnts.com
 License: MIT
 Project-URL: Docs, https://docs.macilib.org
 Project-URL: Code, https://github.com/aaronater10/maci
 Project-URL: Bugs, https://github.com/aaronater10/maci/issues
@@ -23,15 +23,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.3.1
+##### Latest Version: 0.4.0
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.3.1/maci.egg-info/SOURCES.txt` & `maci-0.4.0/maci.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 ./README.md
 maci/__init__.py
+maci/__init__.pyi
 maci/data.py
+maci/data.pyi
 maci/error.py
 maci/hint.py
 maci/py.typed
 maci.egg-info/PKG-INFO
 maci.egg-info/SOURCES.txt
 maci.egg-info/dependency_links.txt
 maci.egg-info/requires.txt
@@ -43,8 +45,9 @@
 maci/_xml/xmldump.py
 maci/_xml/xmldumpstr.py
 maci/_xml/xmlload.py
 maci/_xml/xmlloadstr.py
 maci/_yaml/yamldump.py
 maci/_yaml/yamldumpstr.py
 maci/_yaml/yamlload.py
-maci/_yaml/yamlloadstr.py
+maci/_yaml/yamlloadstr.py
+maci/ext/defusedxml/LICENSE.txt
```

### Comparing `maci-0.3.1/setup.cfg` & `maci-0.4.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -53,19 +53,16 @@
 [options]
 py_modules = maci
 packages = maci
 package_dir = maci=maci
 include_package_data = True
 install_requires = 
 	pyyaml >= 5.4
-	types-pyyaml >= 5.4
 	tomli >= 2.0.1
 	tomli-w >= 1.0.0
+	defusedxml >= 0.7.1
 python_requires = >= 3.7
 
-[options.package_data]
-maci = py.typed
-
 [egg_info]
 tag_build = 
 tag_date = 0
```


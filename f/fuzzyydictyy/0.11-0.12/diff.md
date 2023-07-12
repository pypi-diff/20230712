# Comparing `tmp/fuzzyydictyy-0.11.tar.gz` & `tmp/fuzzyydictyy-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzyydictyy-0.11.tar", last modified: Wed Jul  5 01:51:39 2023, max compression
+gzip compressed data, was "fuzzyydictyy-0.12.tar", last modified: Wed Jul 12 13:52:54 2023, max compression
```

## Comparing `fuzzyydictyy-0.11.tar` & `fuzzyydictyy-0.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 01:51:39.237390 fuzzyydictyy-0.11/
--rw-rw-rw-   0        0        0     1148 2023-07-05 01:51:27.000000 fuzzyydictyy-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      107 2023-07-05 01:51:24.000000 fuzzyydictyy-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     2618 2023-07-05 01:51:39.237390 fuzzyydictyy-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     2016 2023-07-05 01:50:38.000000 fuzzyydictyy-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 01:51:39.233399 fuzzyydictyy-0.11/fuzzyydictyy/
--rw-rw-rw-   0        0        0     2016 2023-07-05 01:50:38.000000 fuzzyydictyy-0.11/fuzzyydictyy/README.MD
--rw-rw-rw-   0        0        0     2864 2023-07-05 01:47:37.000000 fuzzyydictyy-0.11/fuzzyydictyy/__init__.py
--rw-rw-rw-   0        0        0        9 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/fuzzyydictyy/requirements.txt
--rw-rw-rw-   0        0        0     1207 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/fuzzyydictyy/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-05 01:51:39.237390 fuzzyydictyy-0.11/fuzzyydictyy.egg-info/
--rw-rw-rw-   0        0        0     2618 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/fuzzyydictyy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-07-05 01:51:39.000000 fuzzyydictyy-0.11/fuzzyydictyy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/fuzzyydictyy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/fuzzyydictyy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/fuzzyydictyy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-05 01:51:39.238387 fuzzyydictyy-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-07-05 01:51:38.000000 fuzzyydictyy-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:52:54.825444 fuzzyydictyy-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-07-12 13:52:47.000000 fuzzyydictyy-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      107 2023-07-12 13:52:45.000000 fuzzyydictyy-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     2618 2023-07-12 13:52:54.825444 fuzzyydictyy-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     2016 2023-07-05 14:20:18.000000 fuzzyydictyy-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 13:52:54.821455 fuzzyydictyy-0.12/fuzzyydictyy/
+-rw-rw-rw-   0        0        0     2016 2023-07-05 14:20:18.000000 fuzzyydictyy-0.12/fuzzyydictyy/README.MD
+-rw-rw-rw-   0        0        0      661 2023-07-12 13:51:06.000000 fuzzyydictyy-0.12/fuzzyydictyy/__init__.py
+-rw-rw-rw-   0        0        0        9 2023-07-12 13:52:53.000000 fuzzyydictyy-0.12/fuzzyydictyy/requirements.txt
+-rw-rw-rw-   0        0        0     1207 2023-07-12 13:52:53.000000 fuzzyydictyy-0.12/fuzzyydictyy/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-12 13:52:54.825444 fuzzyydictyy-0.12/fuzzyydictyy.egg-info/
+-rw-rw-rw-   0        0        0     2618 2023-07-12 13:52:54.000000 fuzzyydictyy-0.12/fuzzyydictyy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-07-12 13:52:54.000000 fuzzyydictyy-0.12/fuzzyydictyy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 13:52:54.000000 fuzzyydictyy-0.12/fuzzyydictyy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 13:52:54.000000 fuzzyydictyy-0.12/fuzzyydictyy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 13:52:54.000000 fuzzyydictyy-0.12/fuzzyydictyy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-12 13:52:54.827439 fuzzyydictyy-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1260 2023-07-12 13:52:53.000000 fuzzyydictyy-0.12/setup.py
```

### Comparing `fuzzyydictyy-0.11/LICENSE.rst` & `fuzzyydictyy-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `fuzzyydictyy-0.11/PKG-INFO` & `fuzzyydictyy-0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzyydictyy
-Version: 0.11
+Version: 0.12
 Summary: Dict with fuzzy key matching 
 Home-page: https://github.com/hansalemaos/fuzzyydictyy
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: fuzzy,dict
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fuzzyydictyy-0.11/README.md` & `fuzzyydictyy-0.12/README.md`

 * *Files identical despite different names*

### Comparing `fuzzyydictyy-0.11/fuzzyydictyy/README.MD` & `fuzzyydictyy-0.12/fuzzyydictyy/README.MD`

 * *Files identical despite different names*

### Comparing `fuzzyydictyy-0.11/fuzzyydictyy/thirdparty.json` & `fuzzyydictyy-0.12/fuzzyydictyy/thirdparty.json`

 * *Files identical despite different names*

### Comparing `fuzzyydictyy-0.11/fuzzyydictyy.egg-info/PKG-INFO` & `fuzzyydictyy-0.12/fuzzyydictyy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzyydictyy
-Version: 0.11
+Version: 0.12
 Summary: Dict with fuzzy key matching 
 Home-page: https://github.com/hansalemaos/fuzzyydictyy
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: fuzzy,dict
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fuzzyydictyy-0.11/setup.py` & `fuzzyydictyy-0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''Dict with fuzzy key matching '''
 
 # Setting up
 setup(
     name="fuzzyydictyy",
     version=VERSION,
     license='MIT',
```


# Comparing `tmp/torscrape-0.1.1.tar.gz` & `tmp/torscrape-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torscrape-0.1.1.tar", last modified: Tue Jul 11 20:48:37 2023, max compression
+gzip compressed data, was "torscrape-0.1.13.tar", last modified: Wed Jul 12 01:02:05 2023, max compression
```

## Comparing `torscrape-0.1.1.tar` & `torscrape-0.1.13.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 20:48:37.957571 torscrape-0.1.1/
--rw-rw-rw-   0        0        0     1064 2023-07-10 18:53:46.000000 torscrape-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1930 2023-07-11 20:48:37.957061 torscrape-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1418 2023-07-10 22:51:58.000000 torscrape-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 20:48:37.950426 torscrape-0.1.1/TorScrape/
--rw-rw-rw-   0        0        0      287 2023-07-11 20:47:51.000000 torscrape-0.1.1/TorScrape/__init__.py
--rw-rw-rw-   0        0        0     2439 2023-07-11 18:06:04.000000 torscrape-0.1.1/TorScrape/instaData.py
--rw-rw-rw-   0        0        0     1241 2023-07-10 21:33:32.000000 torscrape-0.1.1/TorScrape/tiktokData.py
--rw-rw-rw-   0        0        0      108 2023-07-10 19:44:00.000000 torscrape-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 20:48:37.957571 torscrape-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1052 2023-07-11 20:48:08.000000 torscrape-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 20:48:37.956040 torscrape-0.1.1/torscrape.egg-info/
--rw-rw-rw-   0        0        0     1930 2023-07-11 20:48:37.000000 torscrape-0.1.1/torscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-07-11 20:48:37.000000 torscrape-0.1.1/torscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 20:48:37.000000 torscrape-0.1.1/torscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-11 20:48:37.000000 torscrape-0.1.1/torscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-11 20:48:37.000000 torscrape-0.1.1/torscrape.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 01:02:05.699185 torscrape-0.1.13/
+-rw-rw-rw-   0        0        0     1064 2023-07-10 18:53:46.000000 torscrape-0.1.13/LICENSE
+-rw-rw-rw-   0        0        0     1931 2023-07-12 01:02:05.699185 torscrape-0.1.13/PKG-INFO
+-rw-rw-rw-   0        0        0     1418 2023-07-10 22:51:58.000000 torscrape-0.1.13/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 01:02:05.693184 torscrape-0.1.13/TorScrape/
+-rw-rw-rw-   0        0        0      121 2023-07-11 20:57:31.000000 torscrape-0.1.13/TorScrape/__init__.py
+-rw-rw-rw-   0        0        0     2439 2023-07-11 18:06:04.000000 torscrape-0.1.13/TorScrape/instaData.py
+-rw-rw-rw-   0        0        0     1241 2023-07-10 21:33:32.000000 torscrape-0.1.13/TorScrape/tiktokData.py
+-rw-rw-rw-   0        0        0      108 2023-07-10 19:44:00.000000 torscrape-0.1.13/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 01:02:05.699185 torscrape-0.1.13/setup.cfg
+-rw-rw-rw-   0        0        0     1014 2023-07-12 00:59:01.000000 torscrape-0.1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 01:02:05.698185 torscrape-0.1.13/torscrape.egg-info/
+-rw-rw-rw-   0        0        0     1931 2023-07-12 01:02:05.000000 torscrape-0.1.13/torscrape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-07-12 01:02:05.000000 torscrape-0.1.13/torscrape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 01:02:05.000000 torscrape-0.1.13/torscrape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-12 01:02:05.000000 torscrape-0.1.13/torscrape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 01:02:05.000000 torscrape-0.1.13/torscrape.egg-info/top_level.txt
```

### Comparing `torscrape-0.1.1/LICENSE` & `torscrape-0.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `torscrape-0.1.1/PKG-INFO` & `torscrape-0.1.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torscrape
-Version: 0.1.1
+Version: 0.1.13
 Summary: A webscrape package
 Home-page: https://github.com/toreofc/TorScrape/
 Author: Tore.ofc, rxality
 Author-email: tore.ofc.99@gmail.com
 Project-URL: Bug Tracker, https://github.com/toreofc/TorScrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torscrape-0.1.1/README.md` & `torscrape-0.1.13/README.md`

 * *Files identical despite different names*

### Comparing `torscrape-0.1.1/TorScrape/instaData.py` & `torscrape-0.1.13/TorScrape/instaData.py`

 * *Files identical despite different names*

### Comparing `torscrape-0.1.1/TorScrape/tiktokData.py` & `torscrape-0.1.13/TorScrape/tiktokData.py`

 * *Files identical despite different names*

### Comparing `torscrape-0.1.1/setup.py` & `torscrape-0.1.13/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from setuptools import setup, find_packages
 
 # Get the absolute path to the requirements.txt file
 requirements_path = r"C:\Users\Tobias\Desktop\Webscrape Course\requirements.txt"
 with open(requirements_path) as f:
     requirements = f.read().splitlines()
 
-VERSION = '0.1.1'  # Update this with the actual version
+version = '0.1.13'
 
 setup(
     name='torscrape',
-    version=VERSION,
+    version=version,
     author='Tore.ofc, rxality',
     author_email='tore.ofc.99@gmail.com',
     description='A webscrape package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/toreofc/TorScrape/',
     project_urls={
```

### Comparing `torscrape-0.1.1/torscrape.egg-info/PKG-INFO` & `torscrape-0.1.13/torscrape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torscrape
-Version: 0.1.1
+Version: 0.1.13
 Summary: A webscrape package
 Home-page: https://github.com/toreofc/TorScrape/
 Author: Tore.ofc, rxality
 Author-email: tore.ofc.99@gmail.com
 Project-URL: Bug Tracker, https://github.com/toreofc/TorScrape/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


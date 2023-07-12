# Comparing `tmp/nordvpn-tray-1.0.0.tar.gz` & `tmp/nordvpn-tray-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nordvpn-tray-1.0.0.tar", last modified: Wed Jul 12 16:52:34 2023, max compression
+gzip compressed data, was "nordvpn-tray-1.0.1.tar", last modified: Wed Jul 12 17:22:05 2023, max compression
```

## Comparing `nordvpn-tray-1.0.0.tar` & `nordvpn-tray-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 16:52:34.641569 nordvpn-tray-1.0.0/
--rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 nordvpn-tray-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4804 2023-07-12 16:52:34.635698 nordvpn-tray-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3748 2023-07-11 22:24:38.000000 nordvpn-tray-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-12 16:52:34.641569 nordvpn-tray-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2630 2023-07-12 16:11:19.000000 nordvpn-tray-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:52:34.592622 nordvpn-tray-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 16:52:34.607783 nordvpn-tray-1.0.0/src/nordvpn_tray/
--rw-rw-rw-   0        0        0        0 2023-05-01 10:01:09.000000 nordvpn-tray-1.0.0/src/nordvpn_tray/__init__.py
--rw-rw-rw-   0        0        0     4899 2023-07-12 16:47:56.000000 nordvpn-tray-1.0.0/src/nordvpn_tray/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:52:34.631570 nordvpn-tray-1.0.0/src/nordvpn_tray/resources/
--rw-rw-rw-   0        0        0   119440 2023-05-01 20:17:36.000000 nordvpn-tray-1.0.0/src/nordvpn_tray/resources/nvt.ico
-drwxrwxrwx   0        0        0        0 2023-07-12 16:52:34.629183 nordvpn-tray-1.0.0/src/nordvpn_tray.egg-info/
--rw-rw-rw-   0        0        0     4804 2023-07-12 16:52:34.000000 nordvpn-tray-1.0.0/src/nordvpn_tray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-07-12 16:52:34.000000 nordvpn-tray-1.0.0/src/nordvpn_tray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 16:52:34.000000 nordvpn-tray-1.0.0/src/nordvpn_tray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-12 16:52:34.000000 nordvpn-tray-1.0.0/src/nordvpn_tray.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       67 2023-07-12 16:52:34.000000 nordvpn-tray-1.0.0/src/nordvpn_tray.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 16:52:34.000000 nordvpn-tray-1.0.0/src/nordvpn_tray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 17:22:05.989536 nordvpn-tray-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 nordvpn-tray-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4804 2023-07-12 17:22:05.983535 nordvpn-tray-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3748 2023-07-11 22:24:38.000000 nordvpn-tray-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 17:22:05.989536 nordvpn-tray-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2630 2023-07-12 17:20:27.000000 nordvpn-tray-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 17:22:05.939518 nordvpn-tray-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 17:22:05.954514 nordvpn-tray-1.0.1/src/nordvpn_tray/
+-rw-rw-rw-   0        0        0        0 2023-05-01 10:01:09.000000 nordvpn-tray-1.0.1/src/nordvpn_tray/__init__.py
+-rw-rw-rw-   0        0        0     4899 2023-07-12 16:47:56.000000 nordvpn-tray-1.0.1/src/nordvpn_tray/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 17:22:05.979536 nordvpn-tray-1.0.1/src/nordvpn_tray/resources/
+-rw-rw-rw-   0        0        0   119440 2023-05-01 20:17:36.000000 nordvpn-tray-1.0.1/src/nordvpn_tray/resources/nvt.ico
+drwxrwxrwx   0        0        0        0 2023-07-12 17:22:05.977536 nordvpn-tray-1.0.1/src/nordvpn_tray.egg-info/
+-rw-rw-rw-   0        0        0     4804 2023-07-12 17:22:05.000000 nordvpn-tray-1.0.1/src/nordvpn_tray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-07-12 17:22:05.000000 nordvpn-tray-1.0.1/src/nordvpn_tray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 17:22:05.000000 nordvpn-tray-1.0.1/src/nordvpn_tray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-12 17:22:05.000000 nordvpn-tray-1.0.1/src/nordvpn_tray.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-07-12 17:22:05.000000 nordvpn-tray-1.0.1/src/nordvpn_tray.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 17:22:05.000000 nordvpn-tray-1.0.1/src/nordvpn_tray.egg-info/top_level.txt
```

### Comparing `nordvpn-tray-1.0.0/LICENSE` & `nordvpn-tray-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.0/PKG-INFO` & `nordvpn-tray-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nordvpn-tray
-Version: 1.0.0
+Version: 1.0.1
 Summary: A cross-platform system tray application for interacting with NordVPN.
 Home-page: https://github.com/aviolaris/nordvpn-tray
 Author: Andreas Violaris
 Keywords: nord,nordvpn,nordvpn-tray,nordvpn_tray,vpn,vpn-client,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `nordvpn-tray-1.0.0/README.md` & `nordvpn-tray-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.0/setup.py` & `nordvpn-tray-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     long_description = f.read()
 
 with open('requirements.txt', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='nordvpn-tray',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     package_data={
         "nordvpn_tray": ["*.py"],
         "nordvpn_tray.resources": ["*.ico"],
     },
     description='A cross-platform system tray application for interacting with NordVPN.',
```

### Comparing `nordvpn-tray-1.0.0/src/nordvpn_tray/__main__.py` & `nordvpn-tray-1.0.1/src/nordvpn_tray/__main__.py`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.0/src/nordvpn_tray/resources/nvt.ico` & `nordvpn-tray-1.0.1/src/nordvpn_tray/resources/nvt.ico`

 * *Files identical despite different names*

### Comparing `nordvpn-tray-1.0.0/src/nordvpn_tray.egg-info/PKG-INFO` & `nordvpn-tray-1.0.1/src/nordvpn_tray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nordvpn-tray
-Version: 1.0.0
+Version: 1.0.1
 Summary: A cross-platform system tray application for interacting with NordVPN.
 Home-page: https://github.com/aviolaris/nordvpn-tray
 Author: Andreas Violaris
 Keywords: nord,nordvpn,nordvpn-tray,nordvpn_tray,vpn,vpn-client,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
```


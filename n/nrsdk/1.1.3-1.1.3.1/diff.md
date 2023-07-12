# Comparing `tmp/nrsdk-1.1.3.tar.gz` & `tmp/nrsdk-1.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrsdk-1.1.3.tar", last modified: Wed Jul 12 03:31:48 2023, max compression
+gzip compressed data, was "nrsdk-1.1.3.1.tar", last modified: Wed Jul 12 05:05:25 2023, max compression
```

## Comparing `nrsdk-1.1.3.tar` & `nrsdk-1.1.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 03:31:48.344489 nrsdk-1.1.3/
--rw-rw-rw-   0        0        0      195 2023-07-12 03:31:48.343491 nrsdk-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      881 2023-07-12 01:24:24.000000 nrsdk-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 03:31:48.329953 nrsdk-1.1.3/nrsdk/
--rw-rw-rw-   0        0        0      119 2023-07-12 01:24:24.000000 nrsdk-1.1.3/nrsdk/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-07-12 01:24:24.000000 nrsdk-1.1.3/nrsdk/base.py
-drwxrwxrwx   0        0        0        0 2023-07-12 03:31:48.340498 nrsdk-1.1.3/nrsdk/lib/
--rw-rw-rw-   0        0        0  1854976 2023-07-12 01:18:21.000000 nrsdk-1.1.3/nrsdk/lib/QLNRSdk.dll
--rw-rw-rw-   0        0        0     1975 2023-07-12 01:24:24.000000 nrsdk-1.1.3/nrsdk/mcf_reader.py
-drwxrwxrwx   0        0        0        0 2023-07-12 03:31:48.342493 nrsdk-1.1.3/nrsdk/neuro_recorder/
--rw-rw-rw-   0        0        0     4362 2023-07-12 02:11:52.000000 nrsdk-1.1.3/nrsdk/neuro_recorder/__init__.py
--rw-rw-rw-   0        0        0     8827 2023-07-12 03:07:47.000000 nrsdk-1.1.3/nrsdk/nrsdk.py
--rw-rw-rw-   0        0        0     1995 2023-07-12 01:24:24.000000 nrsdk-1.1.3/nrsdk/paradigm.py
--rw-rw-rw-   0        0        0      136 2023-07-12 01:24:24.000000 nrsdk-1.1.3/nrsdk/rsa.py
-drwxrwxrwx   0        0        0        0 2023-07-12 03:31:48.339502 nrsdk-1.1.3/nrsdk.egg-info/
--rw-rw-rw-   0        0        0      195 2023-07-12 03:31:47.000000 nrsdk-1.1.3/nrsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-07-12 03:31:47.000000 nrsdk-1.1.3/nrsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 03:31:47.000000 nrsdk-1.1.3/nrsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-07 06:05:49.000000 nrsdk-1.1.3/nrsdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-07-12 03:31:47.000000 nrsdk-1.1.3/nrsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 03:31:48.344568 nrsdk-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      569 2023-07-12 03:29:47.000000 nrsdk-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:05:25.518291 nrsdk-1.1.3.1/
+-rw-rw-rw-   0        0        0      199 2023-07-12 05:05:25.518291 nrsdk-1.1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2023-07-12 01:24:24.000000 nrsdk-1.1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 05:05:25.506236 nrsdk-1.1.3.1/nrsdk/
+-rw-rw-rw-   0        0        0      119 2023-07-12 01:24:24.000000 nrsdk-1.1.3.1/nrsdk/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-07-12 01:24:24.000000 nrsdk-1.1.3.1/nrsdk/base.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:05:25.515298 nrsdk-1.1.3.1/nrsdk/lib/
+-rw-rw-rw-   0        0        0  1854976 2023-07-12 01:18:21.000000 nrsdk-1.1.3.1/nrsdk/lib/QLNRSdk.dll
+-rw-rw-rw-   0        0        0     1975 2023-07-12 01:24:24.000000 nrsdk-1.1.3.1/nrsdk/mcf_reader.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:05:25.517292 nrsdk-1.1.3.1/nrsdk/neuro_recorder/
+-rw-rw-rw-   0        0        0     4734 2023-07-12 03:57:49.000000 nrsdk-1.1.3.1/nrsdk/neuro_recorder/__init__.py
+-rw-rw-rw-   0        0        0     8827 2023-07-12 03:07:47.000000 nrsdk-1.1.3.1/nrsdk/nrsdk.py
+-rw-rw-rw-   0        0        0     1995 2023-07-12 01:24:24.000000 nrsdk-1.1.3.1/nrsdk/paradigm.py
+-rw-rw-rw-   0        0        0      136 2023-07-12 01:24:24.000000 nrsdk-1.1.3.1/nrsdk/rsa.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:05:25.514300 nrsdk-1.1.3.1/nrsdk.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-07-12 05:05:25.000000 nrsdk-1.1.3.1/nrsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-12 05:05:25.000000 nrsdk-1.1.3.1/nrsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 05:05:25.000000 nrsdk-1.1.3.1/nrsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-07 06:05:49.000000 nrsdk-1.1.3.1/nrsdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-07-12 05:05:25.000000 nrsdk-1.1.3.1/nrsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 05:05:25.518291 nrsdk-1.1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      573 2023-07-12 05:05:16.000000 nrsdk-1.1.3.1/setup.py
```

### Comparing `nrsdk-1.1.3/README.md` & `nrsdk-1.1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.3/nrsdk/base.py` & `nrsdk-1.1.3.1/nrsdk/base.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.3/nrsdk/lib/QLNRSdk.dll` & `nrsdk-1.1.3.1/nrsdk/lib/QLNRSdk.dll`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.3/nrsdk/mcf_reader.py` & `nrsdk-1.1.3.1/nrsdk/mcf_reader.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.3/nrsdk/neuro_recorder/__init__.py` & `nrsdk-1.1.3.1/nrsdk/neuro_recorder/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,24 @@
         return self._trigger(event_id, device)
 
     # 重启设备
     def restart(self, device=None):
         return self._restart_device(device)
 
     # 开启信号采集（记录）
-    def start_collection(self, param=None, path=None, file_type=None, device=None):
+    def start_collection(self, channels=None, path=None, file_type=None, device=None):
+        if channels is None or len(channels) == 0:
+            return self._start_collection(path=path, file_type=file_type, device=device)
+
+        param = {}
+        param["channels"] =  [{}] * len(channels)
+        for i, ch in enumerate(channels):            
+            param["channels"][i] = {}
+            param["channels"][i]["channel_id"] = int(ch)
+
         return self._start_collection(param, path, file_type, device)
 
     # 停止信号采集（记录）
     def stop_collection(self, device=None):
         return self._stop_collection(device)
 
     # 刺激
```

### Comparing `nrsdk-1.1.3/nrsdk/nrsdk.py` & `nrsdk-1.1.3.1/nrsdk/nrsdk.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.3/nrsdk/paradigm.py` & `nrsdk-1.1.3.1/nrsdk/paradigm.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.3/setup.py` & `nrsdk-1.1.3.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 from setuptools import find_packages
 
-VERSION = '1.1.3'
+VERSION = '1.1.3.1'
 AUTHOR='eegion'
 EMAIL='hehuajun@eegion.com'
 REQUIRED = [
     'beautifulsoup',
     "lxml"
 ]
 
 setup(
     name='nrsdk',  # package name
     version=VERSION,  # package version
     author=AUTHOR,
     author_email=EMAIL,
     requires=REQUIRED,
-    description='Api for use quanlan device, since v1.1.3',  # package description
+    description='Api for use quanlan device, since v1.1.3.1',  # package description
     packages=find_packages(),
     package_data={
         "nrsdk": ["lib/*.dll"],
         "":["*.txt", "*.md"]
     },
     zip_safe=False,
 )
```


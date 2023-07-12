# Comparing `tmp/cbcmgr-1.4.0.tar.gz` & `tmp/cbcmgr-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.4.0.tar", last modified: Wed Jul 12 01:30:29 2023, max compression
+gzip compressed data, was "cbcmgr-1.4.1.tar", last modified: Wed Jul 12 14:07:12 2023, max compression
```

## Comparing `cbcmgr-1.4.0.tar` & `cbcmgr-1.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-12 01:30:29.498381 cbcmgr-1.4.0/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.4.0/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-12 01:30:29.498184 cbcmgr-1.4.0/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.4.0/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-12 01:30:29.468236 cbcmgr-1.4.0/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.4.0/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    10719 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    11149 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/cb_connect_lite.py
--rw-r--r--   0 michael    (501) staff       (20)    27544 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)     7249 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/cb_operation_s.py
--rw-r--r--   0 michael    (501) staff       (20)     3719 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/cb_pathmap.py
--rw-r--r--   0 michael    (501) staff       (20)    13289 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.4.0/cbcmgr/config.py
--rw-r--r--   0 michael    (501) staff       (20)     4334 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.4.0/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)      938 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/id_format.py
--rw-r--r--   0 michael    (501) staff       (20)     2373 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/mt_pool.py
--rw-r--r--   0 michael    (501) staff       (20)     2825 2023-07-07 21:38:37.000000 cbcmgr-1.4.0/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.4.0/cbcmgr/schema.py
--rw-r--r--   0 michael    (501) staff       (20)     1446 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-12 01:30:29.497832 cbcmgr-1.4.0/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-12 01:30:29.000000 cbcmgr-1.4.0/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      485 2023-07-12 01:30:29.000000 cbcmgr-1.4.0/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-12 01:30:29.000000 cbcmgr-1.4.0/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-12 01:30:29.000000 cbcmgr-1.4.0/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-12 01:30:29.000000 cbcmgr-1.4.0/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-12 01:30:29.498463 cbcmgr-1.4.0/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-12 14:07:12.307904 cbcmgr-1.4.1/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.4.1/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-12 14:07:12.307629 cbcmgr-1.4.1/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.4.1/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-12 14:07:12.139554 cbcmgr-1.4.1/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.4.1/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    10719 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    11149 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/cb_connect_lite.py
+-rw-r--r--   0 michael    (501) staff       (20)    27544 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)     7249 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/cb_operation_s.py
+-rw-r--r--   0 michael    (501) staff       (20)     3881 2023-07-12 13:52:42.000000 cbcmgr-1.4.1/cbcmgr/cb_pathmap.py
+-rw-r--r--   0 michael    (501) staff       (20)    13289 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.4.1/cbcmgr/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4334 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.4.1/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)      938 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/id_format.py
+-rw-r--r--   0 michael    (501) staff       (20)     2373 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/mt_pool.py
+-rw-r--r--   0 michael    (501) staff       (20)     2825 2023-07-07 21:38:37.000000 cbcmgr-1.4.1/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.4.1/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)     1446 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-12 14:07:12.307063 cbcmgr-1.4.1/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-12 14:07:12.000000 cbcmgr-1.4.1/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      485 2023-07-12 14:07:12.000000 cbcmgr-1.4.1/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-12 14:07:12.000000 cbcmgr-1.4.1/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-12 14:07:12.000000 cbcmgr-1.4.1/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-12 14:07:12.000000 cbcmgr-1.4.1/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-12 14:07:12.307976 cbcmgr-1.4.1/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-12 13:52:42.000000 cbcmgr-1.4.1/setup.py
```

### Comparing `cbcmgr-1.4.0/LICENSE.txt` & `cbcmgr-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/PKG-INFO` & `cbcmgr-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.4.0
+Version: 1.4.1
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.4.0/README.md` & `cbcmgr-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr/cb_connect.py` & `cbcmgr-1.4.1/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr/cb_connect_lite.py` & `cbcmgr-1.4.1/cbcmgr/cb_connect_lite.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr/cb_management.py` & `cbcmgr-1.4.1/cbcmgr/cb_management.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr/cb_operation_s.py` & `cbcmgr-1.4.1/cbcmgr/cb_operation_s.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr/cb_pathmap.py` & `cbcmgr-1.4.1/cbcmgr/cb_pathmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,19 @@
                            self.password,
                            ssl=self.ssl,
                            quota=self.quota,
                            replicas=self.replicas,
                            mode=self.mode,
                            create=True)
 
+    def connect(self):
+        for c in self.config.paths:
+            keyspace = f"{self.bucket}.{self.scope}.{c.name}"
+            self.pool.connect(keyspace)
+
     def load_data(self,
                   prefix: str,
                   json_file: str = None,
                   xml_file: str = None,
                   json_data: str = None,
                   xml_data: str = None):
```

### Comparing `cbcmgr-1.4.0/cbcmgr/cb_session.py` & `cbcmgr-1.4.1/cbcmgr/cb_session.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr/config.py` & `cbcmgr-1.4.1/cbcmgr/config.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr/exceptions.py` & `cbcmgr-1.4.1/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.4.1/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr/id_format.py` & `cbcmgr-1.4.1/cbcmgr/id_format.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr/mt_pool.py` & `cbcmgr-1.4.1/cbcmgr/mt_pool.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr/retry.py` & `cbcmgr-1.4.1/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr/schema.py` & `cbcmgr-1.4.1/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr/util.py` & `cbcmgr-1.4.1/cbcmgr/util.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.0/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.4.1/cbcmgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.4.0
+Version: 1.4.1
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.4.0/setup.py` & `cbcmgr-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.4.0',
+    version='1.4.1',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```


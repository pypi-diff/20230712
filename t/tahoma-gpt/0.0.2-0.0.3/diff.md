# Comparing `tmp/tahoma_gpt-0.0.2.tar.gz` & `tmp/tahoma_gpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoma_gpt-0.0.2.tar", last modified: Wed Jul 12 01:46:17 2023, max compression
+gzip compressed data, was "tahoma_gpt-0.0.3.tar", last modified: Wed Jul 12 01:53:52 2023, max compression
```

## Comparing `tahoma_gpt-0.0.2.tar` & `tahoma_gpt-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:46:17.941811 tahoma_gpt-0.0.2/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma_gpt-0.0.2/LICENSE
--rwxrwx---   0 neptune   (1000) neptune   (1000)      148 2023-07-12 01:27:33.000000 tahoma_gpt-0.0.2/MANIFEST.in
--rwxrwx---   0 neptune   (1000) neptune   (1000)     3207 2023-07-12 01:46:17.941921 tahoma_gpt-0.0.2/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)     2529 2023-07-12 01:28:59.000000 tahoma_gpt-0.0.2/PYPI_README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     2529 2023-07-12 01:28:25.000000 tahoma_gpt-0.0.2/README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1212 2023-07-12 01:24:52.000000 tahoma_gpt-0.0.2/pyproject.toml
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1057 2023-07-12 01:43:53.000000 tahoma_gpt-0.0.2/requirements.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-07-12 01:46:17.942274 tahoma_gpt-0.0.2/setup.cfg
--rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma_gpt-0.0.2/setup.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:46:17.938135 tahoma_gpt-0.0.2/tahoma_gpt/
--rwxrwx---   0 neptune   (1000) neptune   (1000)      138 2023-07-12 01:21:46.000000 tahoma_gpt-0.0.2/tahoma_gpt/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-07-12 01:45:52.000000 tahoma_gpt-0.0.2/tahoma_gpt/__version__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-07-11 23:44:19.000000 tahoma_gpt-0.0.2/tahoma_gpt/__version__.py~
--rwxrwx---   0 neptune   (1000) neptune   (1000)    37481 2023-07-12 01:25:54.000000 tahoma_gpt-0.0.2/tahoma_gpt/tahoma_gpt.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:46:17.941487 tahoma_gpt-0.0.2/tahoma_gpt/test/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma_gpt-0.0.2/tahoma_gpt/test/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma_gpt-0.0.2/tahoma_gpt/test/test.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:46:17.940637 tahoma_gpt-0.0.2/tahoma_gpt.egg-info/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     3207 2023-07-12 01:46:17.000000 tahoma_gpt-0.0.2/tahoma_gpt.egg-info/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)      454 2023-07-12 01:46:17.000000 tahoma_gpt-0.0.2/tahoma_gpt.egg-info/SOURCES.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-07-12 01:46:17.000000 tahoma_gpt-0.0.2/tahoma_gpt.egg-info/dependency_links.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       58 2023-07-12 01:46:17.000000 tahoma_gpt-0.0.2/tahoma_gpt.egg-info/entry_points.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1057 2023-07-12 01:46:17.000000 tahoma_gpt-0.0.2/tahoma_gpt.egg-info/requires.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       11 2023-07-12 01:46:17.000000 tahoma_gpt-0.0.2/tahoma_gpt.egg-info/top_level.txt
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:53:52.979690 tahoma_gpt-0.0.3/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma_gpt-0.0.3/LICENSE
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      148 2023-07-12 01:27:33.000000 tahoma_gpt-0.0.3/MANIFEST.in
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     3207 2023-07-12 01:53:52.979789 tahoma_gpt-0.0.3/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     2529 2023-07-12 01:28:59.000000 tahoma_gpt-0.0.3/PYPI_README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     2529 2023-07-12 01:28:25.000000 tahoma_gpt-0.0.3/README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1212 2023-07-12 01:24:52.000000 tahoma_gpt-0.0.3/pyproject.toml
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       34 2023-07-12 01:52:47.000000 tahoma_gpt-0.0.3/requirements.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-07-12 01:53:52.980116 tahoma_gpt-0.0.3/setup.cfg
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma_gpt-0.0.3/setup.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:53:52.976291 tahoma_gpt-0.0.3/tahoma_gpt/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      138 2023-07-12 01:21:46.000000 tahoma_gpt-0.0.3/tahoma_gpt/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-07-12 01:53:38.000000 tahoma_gpt-0.0.3/tahoma_gpt/__version__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-07-12 01:45:52.000000 tahoma_gpt-0.0.3/tahoma_gpt/__version__.py~
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    37481 2023-07-12 01:25:54.000000 tahoma_gpt-0.0.3/tahoma_gpt/tahoma_gpt.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:53:52.979385 tahoma_gpt-0.0.3/tahoma_gpt/test/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma_gpt-0.0.3/tahoma_gpt/test/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma_gpt-0.0.3/tahoma_gpt/test/test.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-07-12 01:53:52.978598 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     3207 2023-07-12 01:53:52.000000 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      454 2023-07-12 01:53:52.000000 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/SOURCES.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-07-12 01:53:52.000000 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/dependency_links.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       58 2023-07-12 01:53:52.000000 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/entry_points.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       34 2023-07-12 01:53:52.000000 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/requires.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       11 2023-07-12 01:53:52.000000 tahoma_gpt-0.0.3/tahoma_gpt.egg-info/top_level.txt
```

### Comparing `tahoma_gpt-0.0.2/LICENSE` & `tahoma_gpt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoma_gpt-0.0.2/PKG-INFO` & `tahoma_gpt-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma_gpt
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma-gpt
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma-gpt/issues
 Keywords: tahoma_gpt,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tahoma_gpt-0.0.2/PYPI_README.md` & `tahoma_gpt-0.0.3/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `tahoma_gpt-0.0.2/README.md` & `tahoma_gpt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tahoma_gpt-0.0.2/pyproject.toml` & `tahoma_gpt-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tahoma_gpt-0.0.2/tahoma_gpt/tahoma_gpt.py` & `tahoma_gpt-0.0.3/tahoma_gpt/tahoma_gpt.py`

 * *Files identical despite different names*

### Comparing `tahoma_gpt-0.0.2/tahoma_gpt.egg-info/PKG-INFO` & `tahoma_gpt-0.0.3/tahoma_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma-gpt
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma-gpt
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma-gpt/issues
 Keywords: tahoma_gpt,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


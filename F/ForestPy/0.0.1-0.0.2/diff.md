# Comparing `tmp/ForestPy-0.0.1.tar.gz` & `tmp/ForestPy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ForestPy-0.0.1.tar", last modified: Wed Jul 12 21:33:17 2023, max compression
+gzip compressed data, was "ForestPy-0.0.2.tar", last modified: Wed Jul 12 21:52:57 2023, max compression
```

## Comparing `ForestPy-0.0.1.tar` & `ForestPy-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 21:33:17.484104 ForestPy-0.0.1/
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 21:33:17.329103 ForestPy-0.0.1/ForestPy/
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       22 2023-07-12 21:31:42.000000 ForestPy-0.0.1/ForestPy/__init__.py
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1903 2023-07-12 21:32:00.000000 ForestPy-0.0.1/ForestPy/_modidx.py
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)    14960 2023-07-12 21:31:42.000000 ForestPy-0.0.1/ForestPy/core.py
-drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 21:33:17.460103 ForestPy-0.0.1/ForestPy.egg-info/
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1420 2023-07-12 21:33:17.000000 ForestPy-0.0.1/ForestPy.egg-info/PKG-INFO
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      334 2023-07-12 21:33:17.000000 ForestPy-0.0.1/ForestPy.egg-info/SOURCES.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-12 21:33:17.000000 ForestPy-0.0.1/ForestPy.egg-info/dependency_links.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       59 2023-07-12 21:33:17.000000 ForestPy-0.0.1/ForestPy.egg-info/entry_points.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-12 21:32:00.000000 ForestPy-0.0.1/ForestPy.egg-info/not-zip-safe
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       37 2023-07-12 21:33:17.000000 ForestPy-0.0.1/ForestPy.egg-info/requires.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)        9 2023-07-12 21:33:17.000000 ForestPy-0.0.1/ForestPy.egg-info/top_level.txt
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)    11558 2023-07-09 02:16:06.000000 ForestPy-0.0.1/LICENSE
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      111 2023-04-27 10:12:58.000000 ForestPy-0.0.1/MANIFEST.in
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1420 2023-07-12 21:33:17.481104 ForestPy-0.0.1/PKG-INFO
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)      643 2023-07-11 23:40:52.000000 ForestPy-0.0.1/README.md
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1015 2023-07-11 23:58:33.000000 ForestPy-0.0.1/settings.ini
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-12 21:33:17.485102 ForestPy-0.0.1/setup.cfg
--rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2596 2023-04-27 10:12:58.000000 ForestPy-0.0.1/setup.py
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 21:52:57.306477 ForestPy-0.0.2/
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 21:52:57.152475 ForestPy-0.0.2/ForestPy/
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       22 2023-07-12 21:51:22.000000 ForestPy-0.0.2/ForestPy/__init__.py
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1903 2023-07-12 21:51:22.000000 ForestPy-0.0.2/ForestPy/_modidx.py
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)    14960 2023-07-12 21:51:22.000000 ForestPy-0.0.2/ForestPy/core.py
+drwxrwxrwx   0 bueno     (1000) bueno     (1000)        0 2023-07-12 21:52:57.282477 ForestPy-0.0.2/ForestPy.egg-info/
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1420 2023-07-12 21:52:56.000000 ForestPy-0.0.2/ForestPy.egg-info/PKG-INFO
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      334 2023-07-12 21:52:57.000000 ForestPy-0.0.2/ForestPy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-12 21:52:56.000000 ForestPy-0.0.2/ForestPy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       59 2023-07-12 21:52:56.000000 ForestPy-0.0.2/ForestPy.egg-info/entry_points.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        1 2023-07-12 21:32:00.000000 ForestPy-0.0.2/ForestPy.egg-info/not-zip-safe
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       37 2023-07-12 21:52:56.000000 ForestPy-0.0.2/ForestPy.egg-info/requires.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)        9 2023-07-12 21:52:56.000000 ForestPy-0.0.2/ForestPy.egg-info/top_level.txt
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)    11558 2023-07-09 02:16:06.000000 ForestPy-0.0.2/LICENSE
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      111 2023-04-27 10:12:58.000000 ForestPy-0.0.2/MANIFEST.in
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     1420 2023-07-12 21:52:57.303476 ForestPy-0.0.2/PKG-INFO
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      643 2023-07-11 23:40:52.000000 ForestPy-0.0.2/README.md
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)      853 2023-07-12 21:51:22.000000 ForestPy-0.0.2/settings.ini
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)       38 2023-07-12 21:52:57.307475 ForestPy-0.0.2/setup.cfg
+-rwxrwxrwx   0 bueno     (1000) bueno     (1000)     2596 2023-04-27 10:12:58.000000 ForestPy-0.0.2/setup.py
```

### Comparing `ForestPy-0.0.1/ForestPy/_modidx.py` & `ForestPy-0.0.2/ForestPy/_modidx.py`

 * *Files identical despite different names*

### Comparing `ForestPy-0.0.1/ForestPy/core.py` & `ForestPy-0.0.2/ForestPy/core.py`

 * *Files identical despite different names*

### Comparing `ForestPy-0.0.1/ForestPy.egg-info/PKG-INFO` & `ForestPy-0.0.2/ForestPy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ForestPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A biblioteca Florestal
 Home-page: https://github.com/gabrielfbueno/ForestPy
 Author: gabrielfbueno
 Author-email: gabrielfbueno@outlook.com
 License: Apache Software License 2.0
 Keywords: nbdev python florestal inventario
 Platform: UNKNOWN
```

### Comparing `ForestPy-0.0.1/LICENSE` & `ForestPy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ForestPy-0.0.1/PKG-INFO` & `ForestPy-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ForestPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A biblioteca Florestal
 Home-page: https://github.com/gabrielfbueno/ForestPy
 Author: gabrielfbueno
 Author-email: gabrielfbueno@outlook.com
 License: Apache Software License 2.0
 Keywords: nbdev python florestal inventario
 Platform: UNKNOWN
```

### Comparing `ForestPy-0.0.1/README.md` & `ForestPy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ForestPy-0.0.1/setup.py` & `ForestPy-0.0.2/setup.py`

 * *Files identical despite different names*


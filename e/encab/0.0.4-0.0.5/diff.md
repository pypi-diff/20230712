# Comparing `tmp/encab-0.0.4.tar.gz` & `tmp/encab-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encab-0.0.4.tar", last modified: Tue Jul 11 15:05:38 2023, max compression
+gzip compressed data, was "encab-0.0.5.tar", last modified: Wed Jul 12 07:36:57 2023, max compression
```

## Comparing `encab-0.0.4.tar` & `encab-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 15:05:38.523630 encab-0.0.4/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-04-18 07:01:45.000000 encab-0.0.4/LICENSE
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4865 2023-07-11 15:05:38.523630 encab-0.0.4/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4299 2023-07-11 14:32:39.000000 encab-0.0.4/README.md
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      968 2023-07-11 14:42:58.000000 encab-0.0.4/pyproject.toml
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-07-11 15:05:38.523630 encab-0.0.4/setup.cfg
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 15:05:38.515629 encab-0.0.4/src/
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 15:05:38.519629 encab-0.0.4/src/encab/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2022-11-29 14:01:58.000000 encab-0.0.4/src/encab/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2022-12-05 16:39:25.000000 encab-0.0.4/src/encab/__main__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11043 2023-03-12 15:50:33.000000 encab-0.0.4/src/encab/config.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8042 2023-07-11 14:44:10.000000 encab-0.0.4/src/encab/encab.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 15:05:38.523630 encab-0.0.4/src/encab/ext/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-01-18 08:48:31.000000 encab-0.0.4/src/encab/ext/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6020 2023-07-11 09:18:42.000000 encab-0.0.4/src/encab/ext/log_sanitizer.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12061 2023-07-11 09:18:42.000000 encab-0.0.4/src/encab/ext/startup_script.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-07-11 09:18:42.000000 encab-0.0.4/src/encab/ext/validation.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5348 2023-03-02 07:56:10.000000 encab-0.0.4/src/encab/extensions.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7603 2023-07-11 13:57:15.000000 encab-0.0.4/src/encab/program.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10017 2023-03-02 07:37:32.000000 encab-0.0.4/src/encab/program_state.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3160 2023-01-25 12:22:05.000000 encab-0.0.4/src/encab/programs.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 15:05:38.523630 encab-0.0.4/src/encab.egg-info/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4865 2023-07-11 15:05:38.000000 encab-0.0.4/src/encab.egg-info/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      526 2023-07-11 15:05:38.000000 encab-0.0.4/src/encab.egg-info/SOURCES.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-11 15:05:38.000000 encab-0.0.4/src/encab.egg-info/dependency_links.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-07-11 15:05:38.000000 encab-0.0.4/src/encab.egg-info/entry_points.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2023-07-11 15:05:38.000000 encab-0.0.4/src/encab.egg-info/requires.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2023-07-11 15:05:38.000000 encab-0.0.4/src/encab.egg-info/top_level.txt
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-12 07:36:57.913200 encab-0.0.5/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-04-18 07:01:45.000000 encab-0.0.5/LICENSE
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4865 2023-07-12 07:36:57.913200 encab-0.0.5/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4299 2023-07-11 14:32:39.000000 encab-0.0.5/README.md
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      968 2023-07-12 07:32:46.000000 encab-0.0.5/pyproject.toml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-07-12 07:36:57.913200 encab-0.0.5/setup.cfg
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-12 07:36:57.905199 encab-0.0.5/src/
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-12 07:36:57.909199 encab-0.0.5/src/encab/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2022-11-29 14:01:58.000000 encab-0.0.5/src/encab/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2022-12-05 16:39:25.000000 encab-0.0.5/src/encab/__main__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11029 2023-07-12 07:11:39.000000 encab-0.0.5/src/encab/config.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8042 2023-07-12 07:29:23.000000 encab-0.0.5/src/encab/encab.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-12 07:36:57.913200 encab-0.0.5/src/encab/ext/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-01-18 08:48:31.000000 encab-0.0.5/src/encab/ext/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6020 2023-07-11 09:18:42.000000 encab-0.0.5/src/encab/ext/log_sanitizer.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12061 2023-07-11 09:18:42.000000 encab-0.0.5/src/encab/ext/startup_script.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-07-11 09:18:42.000000 encab-0.0.5/src/encab/ext/validation.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5348 2023-03-02 07:56:10.000000 encab-0.0.5/src/encab/extensions.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7603 2023-07-11 13:57:15.000000 encab-0.0.5/src/encab/program.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10017 2023-03-02 07:37:32.000000 encab-0.0.5/src/encab/program_state.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3160 2023-01-25 12:22:05.000000 encab-0.0.5/src/encab/programs.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-12 07:36:57.913200 encab-0.0.5/src/encab.egg-info/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4865 2023-07-12 07:36:57.000000 encab-0.0.5/src/encab.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      526 2023-07-12 07:36:57.000000 encab-0.0.5/src/encab.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-12 07:36:57.000000 encab-0.0.5/src/encab.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-07-12 07:36:57.000000 encab-0.0.5/src/encab.egg-info/entry_points.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2023-07-12 07:36:57.000000 encab-0.0.5/src/encab.egg-info/requires.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2023-07-12 07:36:57.000000 encab-0.0.5/src/encab.egg-info/top_level.txt
```

### Comparing `encab-0.0.4/LICENSE` & `encab-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `encab-0.0.4/PKG-INFO` & `encab-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: encab
-Version: 0.0.4
+Version: 0.0.5
 Summary: Docker entrypoint tool
 Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
 Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
 Project-URL: Documentation, https://encab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Encab: A Docker Entrypoint Tool
 
 **Encab** is essentially a replacement for complex, hand-written Docker Container Entrypoint scripts,
 especially when dockerizing complex legacy applications.
```

### Comparing `encab-0.0.4/README.md` & `encab-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `encab-0.0.4/pyproject.toml` & `encab-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=63.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "encab"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Sebastian Kuebeck", email="sebastian.kuebeck@encab.io" },
 ]
 description = "Docker entrypoint tool"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "PyYAML >= 6.0, < 7",
```

### Comparing `encab-0.0.4/src/encab/config.py` & `encab-0.0.5/src/encab/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def create(cls, **args):
         """
         creates an instance and sets all missing optional fields to None
 
         :return: the data class
         :rtype: same as cls
         """
-        config_class = dataclass(cls, kw_only=True)  # type: ignore
+        config_class = dataclass(cls)  # type: ignore
         config_fields = fields(config_class)
         all_args = dict(args)
         for field in config_fields:
             name = field.name
             if name not in args:
                 all_args[name] = None
```

### Comparing `encab-0.0.4/src/encab/encab.py` & `encab-0.0.5/src/encab/encab.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     try:
         config, location = load_config(encab_stream)
 
         logger = set_up_logger(config)
 
         extra = {"program": ENCAB}
 
-        logger.info("encab 0.0.4", extra=extra)
+        logger.info("encab 0.0.5", extra=extra)
         logger.info("Using configuration %s", location, extra=extra)
 
         logger.debug(
             "Encab config: %s",
             shorten(str(config), width=127, placeholder="..."),
             extra=extra,
         )
```

### Comparing `encab-0.0.4/src/encab/ext/log_sanitizer.py` & `encab-0.0.5/src/encab/ext/log_sanitizer.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.4/src/encab/ext/startup_script.py` & `encab-0.0.5/src/encab/ext/startup_script.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.4/src/encab/ext/validation.py` & `encab-0.0.5/src/encab/ext/validation.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.4/src/encab/extensions.py` & `encab-0.0.5/src/encab/extensions.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.4/src/encab/program.py` & `encab-0.0.5/src/encab/program.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.4/src/encab/program_state.py` & `encab-0.0.5/src/encab/program_state.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.4/src/encab/programs.py` & `encab-0.0.5/src/encab/programs.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.4/src/encab.egg-info/PKG-INFO` & `encab-0.0.5/src/encab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: encab
-Version: 0.0.4
+Version: 0.0.5
 Summary: Docker entrypoint tool
 Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
 Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
 Project-URL: Documentation, https://encab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Encab: A Docker Entrypoint Tool
 
 **Encab** is essentially a replacement for complex, hand-written Docker Container Entrypoint scripts,
 especially when dockerizing complex legacy applications.
```

### Comparing `encab-0.0.4/src/encab.egg-info/SOURCES.txt` & `encab-0.0.5/src/encab.egg-info/SOURCES.txt`

 * *Files identical despite different names*


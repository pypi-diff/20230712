# Comparing `tmp/pydantic-loggings-0.23.0.tar.gz` & `tmp/pydantic-loggings-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-loggings-0.23.0.tar", last modified: Tue Jul 11 17:53:31 2023, max compression
+gzip compressed data, was "pydantic-loggings-1.0.0.tar", last modified: Wed Jul 12 19:33:17 2023, max compression
```

## Comparing `pydantic-loggings-0.23.0.tar` & `pydantic-loggings-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:53:31.500630 pydantic-loggings-0.23.0/
--rw-r--r--   0 root         (0) root         (0)     3205 2023-07-11 17:53:31.500630 pydantic-loggings-0.23.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2441 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/README.md
--rw-r--r--   0 root         (0) root         (0)     2419 2023-07-11 17:53:22.000000 pydantic-loggings-0.23.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 17:53:31.500630 pydantic-loggings-0.23.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:53:31.496630 pydantic-loggings-0.23.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:53:31.500630 pydantic-loggings-0.23.0/src/pydantic_loggings/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:53:31.500630 pydantic-loggings-0.23.0/src/pydantic_loggings/base/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/base/filters.py
--rw-r--r--   0 root         (0) root         (0)      404 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/base/formatters.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/base/handlers.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/base/loggers.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/base/loggings.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:53:31.500630 pydantic-loggings-0.23.0/src/pydantic_loggings/not_set/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/not_set/__init__.py
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/not_set/filters.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/not_set/formatters.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/not_set/handlers.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/not_set/loggers.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/not_set/loggings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:53:31.500630 pydantic-loggings-0.23.0/src/pydantic_loggings/rich/
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/rich/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/rich/handlers.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/rich/loggers.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/rich/loggings.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/types_.py
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-11 17:53:21.000000 pydantic-loggings-0.23.0/src/pydantic_loggings/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:53:31.500630 pydantic-loggings-0.23.0/src/pydantic_loggings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3205 2023-07-11 17:53:31.000000 pydantic-loggings-0.23.0/src/pydantic_loggings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-11 17:53:31.000000 pydantic-loggings-0.23.0/src/pydantic_loggings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 17:53:31.000000 pydantic-loggings-0.23.0/src/pydantic_loggings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-11 17:53:31.000000 pydantic-loggings-0.23.0/src/pydantic_loggings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-11 17:53:31.000000 pydantic-loggings-0.23.0/src/pydantic_loggings.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.822171 pydantic-loggings-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)     3162 2023-07-12 19:33:17.822171 pydantic-loggings-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-07-12 19:33:06.000000 pydantic-loggings-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 19:33:17.822171 pydantic-loggings-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.818171 pydantic-loggings-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.818171 pydantic-loggings-1.0.0/src/pydantic_loggings/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.818171 pydantic-loggings-1.0.0/src/pydantic_loggings/base/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/base/filters.py
+-rw-r--r--   0 root         (0) root         (0)      404 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/base/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/base/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/base/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/base/loggings.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.822171 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      894 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/loggers.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/loggings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.822171 pydantic-loggings-1.0.0/src/pydantic_loggings/rich/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/rich/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/rich/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/rich/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/rich/loggings.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/types_.py
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-12 19:33:05.000000 pydantic-loggings-1.0.0/src/pydantic_loggings/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:33:17.818171 pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3162 2023-07-12 19:33:17.000000 pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-12 19:33:17.000000 pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:33:17.000000 pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-12 19:33:17.000000 pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-12 19:33:17.000000 pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/top_level.txt
```

### Comparing `pydantic-loggings-0.23.0/PKG-INFO` & `pydantic-loggings-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 0.23.0
+Version: 1.0.0
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
 Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
@@ -29,15 +29,15 @@
 
 ### out of the box
 
 ```py
 from pydantic_loggings.base import Logging # base Logging
 
 
-logger = Logging().configure_and_get_logger()
+logger = Logging().get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG   debug
 # 01-01 00:00:00 INFO    info
@@ -46,15 +46,15 @@
 
 ### default logging
 
 ```py
 from pydantic_loggings.not_set import Logging
 
 
-logger = Logging().configure_and_get_logger()
+logger = Logging().get_logger()
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # warning
 ```
 
@@ -65,15 +65,15 @@
 
 from pydantic_loggings.not_set import Logging
 
 
 env_file = Path(__file__).parent / '.env'
 logger = Logging(
     _env_file=env_file  # pyright: ignore [reportGeneralTypeIssues]
-).configure_and_get_logger()
+).get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 [root]   DEBUG (main.py:11) debug
 # 01-01 00:00:00 [root]    INFO (main.py:12) info
```

### Comparing `pydantic-loggings-0.23.0/README.md` & `pydantic-loggings-1.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ### out of the box
 
 ```py
 from pydantic_loggings.base import Logging # base Logging
 
 
-logger = Logging().configure_and_get_logger()
+logger = Logging().get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG   debug
 # 01-01 00:00:00 INFO    info
@@ -27,15 +27,15 @@
 
 ### default logging
 
 ```py
 from pydantic_loggings.not_set import Logging
 
 
-logger = Logging().configure_and_get_logger()
+logger = Logging().get_logger()
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # warning
 ```
 
@@ -46,15 +46,15 @@
 
 from pydantic_loggings.not_set import Logging
 
 
 env_file = Path(__file__).parent / '.env'
 logger = Logging(
     _env_file=env_file  # pyright: ignore [reportGeneralTypeIssues]
-).configure_and_get_logger()
+).get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 [root]   DEBUG (main.py:11) debug
 # 01-01 00:00:00 [root]    INFO (main.py:12) info
```

### Comparing `pydantic-loggings-0.23.0/pyproject.toml` & `pydantic-loggings-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 authors = [
   { name = "m9810223", email = "m9810223@gmail.com" },
 ]
 name = "pydantic-loggings"
 readme = "README.md"
 requires-python = ">=3.9"
-version = "0.23.0"
+version = "1.0.0"
 
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3",
```

### Comparing `pydantic-loggings-0.23.0/src/pydantic_loggings/base/loggings.py` & `pydantic-loggings-1.0.0/src/pydantic_loggings/base/loggings.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.23.0/src/pydantic_loggings/mixins.py` & `pydantic-loggings-1.0.0/src/pydantic_loggings/mixins.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.23.0/src/pydantic_loggings/not_set/formatters.py` & `pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/formatters.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.23.0/src/pydantic_loggings/not_set/handlers.py` & `pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.23.0/src/pydantic_loggings/not_set/loggers.py` & `pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/loggers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.23.0/src/pydantic_loggings/not_set/loggings.py` & `pydantic-loggings-1.0.0/src/pydantic_loggings/not_set/loggings.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,22 +66,27 @@
 
     def configure(self):
         self.configurator(self.configuration).configure()
 
     def is_valid_logger_name(self, logger_name: str, /):
         return logger_name in ['', 'root', *(self.loggers or {}).keys()]
 
-    def get_logger(self, logger_name: str = '', /):
-        return logging.getLogger(name=logger_name)
-
-    def configure_and_get_logger(
+    def get_logger(
         self,
         logger_name: str = '',
         /,
         *,
         level: t.Optional[t.Union[int, str]] = None,
+        force_level: bool = False,
+        configure: bool = True,
     ):
-        self.configure()
-        logger = self.get_logger(logger_name)
+        if configure:
+            self.configure()
+        logger = logging.getLogger(name=logger_name)
         if level is not None:
-            logger.setLevel(level=level)
+            if force_level is True:
+                logger.setLevel(level=level)
+            elif logging.NOTSET == logger.level:
+                logger.setLevel(level=level)
+            elif logging.NOTSET == logger.getEffectiveLevel():
+                logger.setLevel(level=level)
         return logger
```

### Comparing `pydantic-loggings-0.23.0/src/pydantic_loggings/rich/handlers.py` & `pydantic-loggings-1.0.0/src/pydantic_loggings/rich/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-0.23.0/src/pydantic_loggings.egg-info/PKG-INFO` & `pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 0.23.0
+Version: 1.0.0
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-logging-settings
 Project-URL: Source, https://github.com/m9810223/pydantic-logging-settings
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
@@ -29,15 +29,15 @@
 
 ### out of the box
 
 ```py
 from pydantic_loggings.base import Logging # base Logging
 
 
-logger = Logging().configure_and_get_logger()
+logger = Logging().get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 DEBUG   debug
 # 01-01 00:00:00 INFO    info
@@ -46,15 +46,15 @@
 
 ### default logging
 
 ```py
 from pydantic_loggings.not_set import Logging
 
 
-logger = Logging().configure_and_get_logger()
+logger = Logging().get_logger()
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # warning
 ```
 
@@ -65,15 +65,15 @@
 
 from pydantic_loggings.not_set import Logging
 
 
 env_file = Path(__file__).parent / '.env'
 logger = Logging(
     _env_file=env_file  # pyright: ignore [reportGeneralTypeIssues]
-).configure_and_get_logger()
+).get_logger()
 
 logger.debug('debug')
 logger.info('info')
 logger.warning('warning')
 
 # 01-01 00:00:00 [root]   DEBUG (main.py:11) debug
 # 01-01 00:00:00 [root]    INFO (main.py:12) info
```

### Comparing `pydantic-loggings-0.23.0/src/pydantic_loggings.egg-info/SOURCES.txt` & `pydantic-loggings-1.0.0/src/pydantic_loggings.egg-info/SOURCES.txt`

 * *Files identical despite different names*


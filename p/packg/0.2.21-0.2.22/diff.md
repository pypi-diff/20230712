# Comparing `tmp/packg-0.2.21.tar.gz` & `tmp/packg-0.2.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packg-0.2.21.tar", last modified: Sat Jul  8 13:02:24 2023, max compression
+gzip compressed data, was "packg-0.2.22.tar", last modified: Tue Jul 11 22:54:19 2023, max compression
```

## Comparing `packg-0.2.21.tar` & `packg-0.2.22.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-08 13:02:24.741776 packg-0.2.21/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.21/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-08 13:02:24.741776 packg-0.2.21/PKG-INFO
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-07-07 09:15:31.000000 packg-0.2.21/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2337 2023-07-06 08:44:58.000000 packg-0.2.21/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-07 09:15:31.000000 packg-0.2.21/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-07-08 13:02:24.745776 packg-0.2.21/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-08 13:02:24.557773 packg-0.2.21/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-08 13:02:24.641774 packg-0.2.21/src/packg/
--rw-------   0 gings    (14999) lmb-mit   (1061)      129 2023-07-08 13:01:40.000000 packg-0.2.21/src/packg/__init__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/caching.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5770 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/constclass.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      530 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/debugging.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/dtime.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     8349 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/import_from_source.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-08 13:02:24.729776 packg-0.2.21/src/packg/iotools/
--rw-------   0 gings    (14999) lmb-mit   (1061)      707 2023-07-08 13:01:40.000000 packg-0.2.21/src/packg/iotools/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/iotools/compressed.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      457 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/iotools/gitmatcher.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     6028 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/iotools/jsonext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    10555 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/iotools/jsonext_encoder.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4014 2023-07-08 13:01:40.000000 packg-0.2.21/src/packg/iotools/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4840 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/iotools/yamlext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5493 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/log.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/misc.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2698 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/paths.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-08 13:02:24.733776 packg-0.2.21/src/packg/run/
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3522 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/run/syncjupytext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5464 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/strings.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/system.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1328 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/tensors.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-07-07 09:15:31.000000 packg-0.2.21/src/packg/typext.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-08 13:02:24.685775 packg-0.2.21/src/packg.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-08 13:02:24.000000 packg-0.2.21/src/packg.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      763 2023-07-08 13:02:24.000000 packg-0.2.21/src/packg.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-07-08 13:02:24.000000 packg-0.2.21/src/packg.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-08 13:02:24.000000 packg-0.2.21/src/packg.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-07-08 13:02:24.000000 packg-0.2.21/src/packg.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.21/src/packg.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-11 22:54:19.812716 packg-0.2.22/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 packg-0.2.22/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-11 22:54:19.808715 packg-0.2.22/PKG-INFO
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1295 2023-07-07 09:15:31.000000 packg-0.2.22/README.md
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2337 2023-07-06 08:44:58.000000 packg-0.2.22/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-07 09:15:31.000000 packg-0.2.22/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-07-11 22:54:19.812716 packg-0.2.22/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-11 22:54:19.704713 packg-0.2.22/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-11 22:54:19.764715 packg-0.2.22/src/packg/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      129 2023-07-11 22:54:00.000000 packg-0.2.22/src/packg/__init__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3107 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/caching.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5770 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/constclass.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      530 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/debugging.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/dtime.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     8349 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/import_from_source.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-11 22:54:19.804715 packg-0.2.22/src/packg/iotools/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      707 2023-07-08 13:01:40.000000 packg-0.2.22/src/packg/iotools/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      420 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/iotools/compressed.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      457 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/iotools/gitmatcher.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     6028 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/iotools/jsonext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    10555 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/iotools/jsonext_encoder.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4014 2023-07-08 13:01:40.000000 packg-0.2.22/src/packg/iotools/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4840 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/iotools/yamlext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5915 2023-07-11 22:54:00.000000 packg-0.2.22/src/packg/log.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/misc.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2698 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/paths.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-11 22:54:19.808715 packg-0.2.22/src/packg/run/
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3522 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/run/syncjupytext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5464 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/strings.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/system.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1328 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/tensors.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      527 2023-07-07 09:15:31.000000 packg-0.2.22/src/packg/typext.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-07-11 22:54:19.784715 packg-0.2.22/src/packg.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2091 2023-07-11 22:54:19.000000 packg-0.2.22/src/packg.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      763 2023-07-11 22:54:19.000000 packg-0.2.22/src/packg.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-07-11 22:54:19.000000 packg-0.2.22/src/packg.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       96 2023-07-11 22:54:19.000000 packg-0.2.22/src/packg.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        6 2023-07-11 22:54:19.000000 packg-0.2.22/src/packg.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-28 06:28:28.000000 packg-0.2.22/src/packg.egg-info/zip-safe
```

### Comparing `packg-0.2.21/LICENSE` & `packg-0.2.22/LICENSE`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/PKG-INFO` & `packg-0.2.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.21
+Version: 0.2.22
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.21 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.22 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.21/README.md` & `packg-0.2.22/README.md`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/pyproject.toml` & `packg-0.2.22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/caching.py` & `packg-0.2.22/src/packg/caching.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/constclass.py` & `packg-0.2.22/src/packg/constclass.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/debugging.py` & `packg-0.2.22/src/packg/debugging.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/import_from_source.py` & `packg-0.2.22/src/packg/import_from_source.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/iotools/__init__.py` & `packg-0.2.22/src/packg/iotools/__init__.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/iotools/jsonext.py` & `packg-0.2.22/src/packg/iotools/jsonext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/iotools/jsonext_encoder.py` & `packg-0.2.22/src/packg/iotools/jsonext_encoder.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/iotools/misc.py` & `packg-0.2.22/src/packg/iotools/misc.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/iotools/yamlext.py` & `packg-0.2.22/src/packg/iotools/yamlext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/log.py` & `packg-0.2.22/src/packg/log.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     "<blue>{name}</blue>:<blue>{function}</blue>:<blue>{line}</blue> "
     "<level>{message}</level>")
 TIMELESS_FORMAT = (
     "<level>{level: <4.4}</level> "
     "<level>{message}</level>")
 
 
+global_logger_config = None
+
+
 def configure_logger(
         level: LevelType = "DEBUG",
         sink=sys.stderr,
         format=SHORTEST_FORMAT,  # noqa # pylint: disable=redefined-builtin
         colorize=True,
         add_sinks: Optional[List[Any]] = None,
         kwargs_handler: Optional[Dict[str, Any]] = None,
@@ -86,52 +89,65 @@
     # fix bug when combining colorama and loguru in conemu console on windows
     if (colorize and os.name == "nt" and os.environ.get("CONEMUANSI") == "ON"
             and sink in (sys.stderr, sys.stdout)):
         print("\r", end="")  # the invisible print here magically fixes the color
 
     logger_config = {"handlers": handlers, **kwargs}
     logger.configure(**logger_config)
+    global global_logger_config
+    global_logger_config = logger_config
     return logger_config
 
 
-def reroute_logger(logger_config, new_sink, handler_num: int = 0) -> None:
+def reroute_logger(new_sink, logger_config=None,  handler_num: int = 0) -> None:
     """
     Reroute a sink from one target to another. Useful for proper logging inside
     a tqdm progressbar without having to recreate the entire logger.
 
     Args:
-        logger_config: config created by configure_logger() function above.
         new_sink: new target
+        logger_config: config created by configure_logger() function above.
+            If None, use the global config.
         handler_num: index of the handler of which to change the sink
 
     Usage:
         logger_config = configure_logger(...)
         pbar = tqdm(...)
         reroute_logger(logger_config, lambda msg: pbar.write(msg, end=""))
         # use tqdm progressbar and logger together here
         pbar.close()
         reroute_logger(logger_config, sys.stderr)
 
     Notes:
         The config is modified inplace so does not need to be returned here.
         It cannot be deepcopy-ed here because sink is not pickle-able.
     """
+    if logger_config is None:
+        global global_logger_config
+        logger_config = global_logger_config
     logger_config["handlers"][handler_num]["sink"] = new_sink
     logger.configure(**logger_config)
     return logger_config
 
 
 def get_level_as_str(level: LevelType):
     if isinstance(level, str):
         return level.upper()
     if isinstance(level, int):
         return getLevelName(level).upper()
     raise TypeError(f"Level must be str or int, not {type(level)}")
 
 
+def get_level_as_int(level: str):
+    if isinstance(level, int):
+        return level
+    level_int = int(getLevelName(level.upper()))
+    return level_int
+
+
 def get_logger_level_from_args(args) -> str:
     if args.verbose:
         return "DEBUG"
     if args.quiet:
         return "WARNING"
     return "INFO"
```

### Comparing `packg-0.2.21/src/packg/paths.py` & `packg-0.2.22/src/packg/paths.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/run/syncjupytext.py` & `packg-0.2.22/src/packg/run/syncjupytext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/strings.py` & `packg-0.2.22/src/packg/strings.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/system.py` & `packg-0.2.22/src/packg/system.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/tensors.py` & `packg-0.2.22/src/packg/tensors.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg/typext.py` & `packg-0.2.22/src/packg/typext.py`

 * *Files identical despite different names*

### Comparing `packg-0.2.21/src/packg.egg-info/PKG-INFO` & `packg-0.2.22/src/packg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packg
-Version: 0.2.21
+Version: 0.2.22
 Summary: Collection of utilities used in other python projects.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: packg Version: 0.2.21 Summary: Collection of
+Metadata-Version: 2.1 Name: packg Version: 0.2.22 Summary: Collection of
 utilities used in other python projects. Author: gingsi License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/packg Keywords:
 attrs,typing,dict,attr Platform: any Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `packg-0.2.21/src/packg.egg-info/SOURCES.txt` & `packg-0.2.22/src/packg.egg-info/SOURCES.txt`

 * *Files identical despite different names*


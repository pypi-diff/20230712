# Comparing `tmp/pypomes_logging-0.1.3.tar.gz` & `tmp/pypomes_logging-0.1.5.tar.gz`

## Comparing `pypomes_logging-0.1.3.tar` & `pypomes_logging-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/src/pypomes_logging/__init__.py
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/src/pypomes_logging/logging_pomes.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/README.md
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pypomes_logging-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 pypomes_logging-0.1.5/src/pypomes_logging/__init__.py
+-rw-r--r--   0        0        0     6486 2020-02-02 00:00:00.000000 pypomes_logging-0.1.5/src/pypomes_logging/logging_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes_logging-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.1.5/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 pypomes_logging-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pypomes_logging-0.1.5/PKG-INFO
```

### Comparing `pypomes_logging-0.1.3/src/pypomes_logging/logging_pomes.py` & `pypomes_logging-0.1.5/src/pypomes_logging/logging_pomes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,92 @@
 import logging
 import os
 import tempfile
 from datetime import datetime
 from dateutil import parser
 from io import BytesIO
-from typing import Final, TextIO
+from typing import Final, Literal, TextIO
 from pypomes_core import APP_PREFIX, DATETIME_FORMAT_INV, env_get_str
 
+
+def __get_logging_level(level: Literal["debug", "info", "warning", "error", "critical"]) -> int:
+    """
+    Translate the log severity string *level* into the *logging*'s internal logging severity value.
+
+    :param level: the string log severity
+    :return: the internal logging severity value
+    """
+    result: int | None
+    match level:
+        case "debug":
+            result = logging.DEBUG          # 10
+        case "info":
+            result = logging.INFO           # 20
+        case "warning":
+            result = logging.WARN           # 30
+        case "error":
+            result = logging.ERROR          # 40
+        case "critical":
+            result = logging.CRITICAL       # 50
+        case _:
+            result = logging.NOTSET         # 0
+
+    return result
+
+
 LOGGING_ID: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_ID", f"{APP_PREFIX}")
-LOGGING_FORMAT: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_ID",
+LOGGING_FORMAT: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FORMAT",
                                          "{asctime} {levelname:1.1} {thread:5d} "
                                          "{module:20.20} {funcName:20.20} {lineno:3d} {message}")
 LOGGING_STYLE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_STYLE", "{")
 
 LOGGING_FILE_PATH: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE_PATH",
                                             os.path.join(tempfile.gettempdir(), f"{APP_PREFIX}.log"))
 LOGGING_FILE_MODE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE_MODE", "a")
 
 # define and configure the logger
 PYPOMES_LOGGER: Final[logging.Logger] = logging.getLogger(LOGGING_ID)
 
-match env_get_str(f"{APP_PREFIX}_LOGGING_LEVEL"):
-    case "d" | "debug":
-        LOGGING_LEVEL: Final[int] = logging.DEBUG
-    case "i" | "info":
-        LOGGING_LEVEL: Final[int] = logging.INFO
-    case "w" | "warning":
-        LOGGING_LEVEL: Final[int] = logging.WARN
-    case "e" | "error":
-        LOGGING_LEVEL: Final[int] = logging.ERROR
-    case "c" | "critical":
-        LOGGING_LEVEL: Final[int] = logging.CRITICAL
-    case _:
-        LOGGING_LEVEL: Final[int] = logging.NOTSET
-
-logging.basicConfig(level=LOGGING_LEVEL,
-                    filename=LOGGING_FILE_PATH,
+# define the logging severity level
+# noinspection PyTypeChecker
+LOGGING_LEVEL: Final[int] = __get_logging_level(env_get_str(f"{APP_PREFIX}_LOGGING_LEVEL"))
+
+# configure the logger
+# noinspection PyTypeChecker
+logging.basicConfig(filename=LOGGING_FILE_PATH,
                     filemode=LOGGING_FILE_MODE,
+                    format=LOGGING_FORMAT,
                     datefmt=DATETIME_FORMAT_INV,
-                    style="{",
-                    format="{asctime} {levelname:1.1} {thread:5d} "
-                           "{module:20.20} {funcName:20.20} {lineno:3d} {message}")
+                    style=LOGGING_STYLE,
+                    level=LOGGING_LEVEL)
 for _handler in logging.root.handlers:
     _handler.addFilter(logging.Filter(LOGGING_ID))
 
 
-def logging_get_entries(errors: list[str], log_level: str, log_from: str, log_to: str) -> BytesIO:
-
-    def get_level(level: str) -> int:
-
-        result: int | None
-        match level:
-            case "d" | "debug":
-                result = logging.DEBUG          # 10
-            case "i" | "info":
-                result = logging.INFO           # 20
-            case "w" | "warning":
-                result = logging.WARN           # 30
-            case "e" | "error":
-                result = logging.ERROR          # 40
-            case "c" | "critical":
-                result = logging.CRITICAL       # 50
-            case _:
-                result = logging.NOTSET         # 0
-
-        return result
+def logging_get_entries(errors: list[str],
+                        log_level:  Literal["debug", "info", "warning", "error", "critical"] = None,
+                        log_from: str = None, log_to: str = None) -> BytesIO:
+    """
+    Extract and return all entries in *PYPOMES_LOGGER*'s logging file,
+    meeting the criteria specified by *log_level* and by the inclusive interval *[log_from, log_to]*.
 
+    :param errors: errors eventually generated during execution
+    :param log_level: the logging level (defaults to all levels)
+    :param log_from: the initial timestamp (defaults to unspecified)
+    :param log_to: the finaL timestamp (defaults to unspecified)
+    :return: the logging entries meeting the specified criteria
+    """
     # inicializa variável de retorno
     result: BytesIO | None = None
 
     # obtain the logging level
-    logging_level: int = get_level(log_level)
+    # noinspection PyTypeChecker
+    logging_level: int = __get_logging_level(log_level)
 
-    # obtain the initial timestap
+    # obtain the initial timestamp
     from_stamp: datetime | None = None
     if log_from is not None:
         from_stamp = parser.parse(log_from)
         if from_stamp is None:
             errors.append(f"Value '{from_stamp}' of 'from' attribute invalid")
 
     # obtaind the final timestamp
@@ -96,51 +106,59 @@
     if len(errors) == 0:
         # no, proceed
         result = BytesIO()
         with open(LOGGING_FILE_PATH, "r") as f:
             line: str = f.readline()
             while line:
                 items: list[str] = line.split(maxsplit=3)
-                level: int = get_level(items[2])
-                if level >= logging_level:
+                # noinspection PyTypeChecker
+                msg_level: int = __get_logging_level(items[2])
+                if msg_level >= logging_level:
                     timestamp: datetime = parser.parse(f"{items[0]} {items[1]}")
                     if (from_stamp is None or timestamp >= from_stamp) and \
                        (to_stamp is None or timestamp <= to_stamp):
                         result.write(line.encode())
                 line = f.readline()
 
     return result
 
 
-def logging_log_msgs(msgs: list[str], log_level: str = None, output_dev: TextIO = None):
+def logging_log_msgs(msgs: list[str], output_dev: TextIO = None,
+                     log_level: Literal["debug", "info", "warning", "error", "critical"] = "error"):
     """
-    Write messages in *msgs* to *PYPOMES_LOGGER*, and to *output_dev*
+    Write all messages in *msgs* to *PYPOMES_LOGGER*'s logging file, and to *output_dev*
     (tipically, *sys.stdout* ou *sys.stderr*).
 
     :param msgs: the messages list
-    :param log_level: the logging level (None for no log printing)
+    :param log_level: the logging level, defaults to 'error' (None for no logging)
     :param output_dev: output device where the message is to be printed (None for no device printing)
     """
+    # define the log writer
+    log_writer: callable = None
+    match log_level:
+        case "debug":
+            log_writer = PYPOMES_LOGGER.debug
+        case "info":
+            log_writer = PYPOMES_LOGGER.info
+        case "warning":
+            log_writer = PYPOMES_LOGGER.warning
+        case "error":
+            log_writer = PYPOMES_LOGGER.error
+        case "critical":
+            log_writer = PYPOMES_LOGGER.critical
+
     # traverse the messages list
     for msg in msgs:
-        # write the message
-        match log_level:
-            case "c" | "critical":
-                PYPOMES_LOGGER.critical(msg)
-            case "d" | "debug":
-                PYPOMES_LOGGER.debug(msg)
-            case "i" | "info":
-                PYPOMES_LOGGER.info(msg)
-            case "w" | "warning":
-                PYPOMES_LOGGER.warning(msg)
-            case "e" | "error":
-                PYPOMES_LOGGER.error(msg)
+        # has the log writer been defined ?
+        if log_writer is not None:
+            # yes, log the message
+            log_writer(msg)
 
-        # o dispositivo de saída foi definido ?
+        # the output device has been defined ?
         if output_dev is not None:
-            # sim, escreva o erro nesse dispositivo
+            # yes, write the message to it
             output_dev.write(msg)
 
-            # o dispositivo de saída é 'stderr' ou 'stdout' ?
+            # the output device is 'stderr' ou 'stdout' ?
             if output_dev.name.startswith("<std"):
-                # sim, mude de linha
+                # yes, skip to the next line
                 output_dev.write("\n")
```

### Comparing `pypomes_logging-0.1.3/LICENSE` & `pypomes_logging-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_logging-0.1.3/pyproject.toml` & `pypomes_logging-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_logging"
-version = "0.1.3"
+version = "0.1.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (logging module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_logging-0.1.3/PKG-INFO` & `pypomes_logging-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_logging
-Version: 0.1.3
+Version: 0.1.5
 Summary: A collection of Python pomes, pennyeach (logging module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Logging
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Logging/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


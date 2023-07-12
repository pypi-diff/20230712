# Comparing `tmp/code_exec-0.0.1.tar.gz` & `tmp/code_exec-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_exec-0.0.1.tar", last modified: Wed Jul 12 14:04:17 2023, max compression
+gzip compressed data, was "code_exec-0.0.2.tar", last modified: Wed Jul 12 16:33:20 2023, max compression
```

## Comparing `code_exec-0.0.1.tar` & `code_exec-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 14:04:17.237573 code_exec-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-12 13:09:33.000000 code_exec-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      630 2023-07-12 14:04:17.237573 code_exec-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       89 2023-07-12 12:53:31.000000 code_exec-0.0.1/README.md
--rw-rw-rw-   0        0        0      617 2023-07-12 14:02:29.000000 code_exec-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 14:04:17.238574 code_exec-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-12 14:04:17.225584 code_exec-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 14:04:17.231572 code_exec-0.0.1/src/code_exec/
--rw-rw-rw-   0        0        0     1073 2023-07-12 13:31:09.000000 code_exec-0.0.1/src/code_exec/__init__.py
--rw-rw-rw-   0        0        0     2700 2023-07-12 13:22:11.000000 code_exec-0.0.1/src/code_exec/checker.py
--rw-rw-rw-   0        0        0     2731 2023-07-12 13:23:08.000000 code_exec-0.0.1/src/code_exec/executor.py
-drwxrwxrwx   0        0        0        0 2023-07-12 14:04:17.236575 code_exec-0.0.1/src/code_exec.egg-info/
--rw-rw-rw-   0        0        0      630 2023-07-12 14:04:17.000000 code_exec-0.0.1/src/code_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-07-12 14:04:17.000000 code_exec-0.0.1/src/code_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 14:04:17.000000 code_exec-0.0.1/src/code_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 14:04:17.000000 code_exec-0.0.1/src/code_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 16:33:20.352795 code_exec-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-12 13:09:33.000000 code_exec-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      630 2023-07-12 16:33:20.352795 code_exec-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       89 2023-07-12 12:53:31.000000 code_exec-0.0.2/README.md
+-rw-rw-rw-   0        0        0      617 2023-07-12 16:30:51.000000 code_exec-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 16:33:20.352795 code_exec-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 16:33:20.336781 code_exec-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 16:33:20.344796 code_exec-0.0.2/src/code_exec/
+-rw-rw-rw-   0        0        0     1047 2023-07-12 16:32:14.000000 code_exec-0.0.2/src/code_exec/__init__.py
+-rw-rw-rw-   0        0        0     2700 2023-07-12 13:22:11.000000 code_exec-0.0.2/src/code_exec/checker.py
+-rw-rw-rw-   0        0        0     2718 2023-07-12 16:32:25.000000 code_exec-0.0.2/src/code_exec/executor.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:33:20.352795 code_exec-0.0.2/src/code_exec.egg-info/
+-rw-rw-rw-   0        0        0      630 2023-07-12 16:33:20.000000 code_exec-0.0.2/src/code_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-07-12 16:33:20.000000 code_exec-0.0.2/src/code_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:33:20.000000 code_exec-0.0.2/src/code_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 16:33:20.000000 code_exec-0.0.2/src/code_exec.egg-info/top_level.txt
```

### Comparing `code_exec-0.0.1/LICENSE` & `code_exec-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `code_exec-0.0.1/PKG-INFO` & `code_exec-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code_exec
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small tool to execute python code more safely
 Author-email: zimolab1995 <zimolab@aliyun.com>
 Project-URL: Homepage, https://gitee.com/zimolab1995/code_exec
 Project-URL: Bug Tracker, https://gitee.com/zimolab1995/code_exec/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `code_exec-0.0.1/pyproject.toml` & `code_exec-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "code_exec"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="zimolab1995", email="zimolab@aliyun.com" },
 ]
 description = "A small tool to execute python code more safely"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `code_exec-0.0.1/src/code_exec/__init__.py` & `code_exec-0.0.2/src/code_exec/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from src.code_exec.checker import StaticCodeChecker
-from src.code_exec.executor import CodeExecutor
+from .checker import StaticCodeChecker
+from .executor import CodeExecutor
 
 DEFAULT_UNSAFE_BUILTINS = [
     "__import__",
     "exec",
     "eval",
     "quit",
     "exit",
```

### Comparing `code_exec-0.0.1/src/code_exec/checker.py` & `code_exec-0.0.2/src/code_exec/checker.py`

 * *Files identical despite different names*

### Comparing `code_exec-0.0.1/src/code_exec/executor.py` & `code_exec-0.0.2/src/code_exec/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import builtins
 import inspect
 from copy import copy
 
-from src.code_exec.checker import StaticCodeChecker
+from .checker import StaticCodeChecker
 
 
 class CodeExecutor(object):
     MODE_EXEC = "exec"
     MODE_EVAL = "eval"
 
     FILENAME_STRING = "<string>"
```

### Comparing `code_exec-0.0.1/src/code_exec.egg-info/PKG-INFO` & `code_exec-0.0.2/src/code_exec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-exec
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small tool to execute python code more safely
 Author-email: zimolab1995 <zimolab@aliyun.com>
 Project-URL: Homepage, https://gitee.com/zimolab1995/code_exec
 Project-URL: Bug Tracker, https://gitee.com/zimolab1995/code_exec/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


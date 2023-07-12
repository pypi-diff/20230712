# Comparing `tmp/log21-2.5.3.tar.gz` & `tmp/log21-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log21-2.5.3.tar", last modified: Tue Jun 27 11:02:07 2023, max compression
+gzip compressed data, was "log21-2.5.4.tar", last modified: Wed Jul 12 15:56:22 2023, max compression
```

## Comparing `log21-2.5.3.tar` & `log21-2.5.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:02:07.733104 log21-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-27 11:01:57.000000 log21-2.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-06-27 11:02:07.733104 log21-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-06-27 11:01:57.000000 log21-2.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:02:07.733104 log21-2.5.3/log21/
--rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-06-27 11:01:57.000000 log21-2.5.3/log21/Argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-06-27 11:01:57.000000 log21-2.5.3/log21/Colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:02:07.733104 log21-2.5.3/log21/CrashReporter/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-27 11:01:57.000000 log21-2.5.3/log21/CrashReporter/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-06-27 11:01:57.000000 log21-2.5.3/log21/CrashReporter/Reporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-27 11:01:57.000000 log21-2.5.3/log21/CrashReporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-27 11:01:57.000000 log21-2.5.3/log21/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-06-27 11:01:57.000000 log21-2.5.3/log21/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-27 11:01:57.000000 log21-2.5.3/log21/Levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-27 11:01:57.000000 log21-2.5.3/log21/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-06-27 11:01:57.000000 log21-2.5.3/log21/LoggingWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-27 11:01:57.000000 log21-2.5.3/log21/Manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    25520 2023-06-27 11:01:57.000000 log21-2.5.3/log21/PPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-06-27 11:01:57.000000 log21-2.5.3/log21/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-27 11:01:57.000000 log21-2.5.3/log21/StreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-06-27 11:01:57.000000 log21-2.5.3/log21/TreePrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-06-27 11:01:57.000000 log21-2.5.3/log21/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 11:02:07.733104 log21-2.5.3/log21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-06-27 11:02:07.000000 log21-2.5.3/log21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 11:02:07.000000 log21-2.5.3/log21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 11:02:07.000000 log21-2.5.3/log21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-27 11:02:07.000000 log21-2.5.3/log21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 11:02:07.000000 log21-2.5.3/log21.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-27 11:01:57.000000 log21-2.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 11:02:07.733104 log21-2.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:56:22.150226 log21-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-12 15:56:05.000000 log21-2.5.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-07-12 15:56:22.150226 log21-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-12 15:56:05.000000 log21-2.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:56:22.150226 log21-2.5.4/log21/
+-rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:56:22.150226 log21-2.5.4/log21/CrashReporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-12 15:56:05.000000 log21-2.5.4/log21/CrashReporter/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-07-12 15:56:05.000000 log21-2.5.4/log21/CrashReporter/Reporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-12 15:56:05.000000 log21-2.5.4/log21/CrashReporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-12 15:56:05.000000 log21-2.5.4/log21/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-07-12 15:56:05.000000 log21-2.5.4/log21/LoggingWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25520 2023-07-12 15:56:05.000000 log21-2.5.4/log21/PPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-07-12 15:56:05.000000 log21-2.5.4/log21/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-12 15:56:05.000000 log21-2.5.4/log21/StreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-07-12 15:56:05.000000 log21-2.5.4/log21/TreePrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-12 15:56:05.000000 log21-2.5.4/log21/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:56:22.150226 log21-2.5.4/log21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-12 15:56:05.000000 log21-2.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:56:22.150226 log21-2.5.4/setup.cfg
```

### Comparing `log21-2.5.3/LICENSE.txt` & `log21-2.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/PKG-INFO` & `log21-2.5.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.5.3
+Version: 2.5.4
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
 Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
 Project-URL: Source, https://github.com/MPCodeWriter21/log21
 Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
@@ -71,21 +71,23 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.5.3
+### 2.5.4
 
-Moved some dictionaries to `__init__` methods.
-`colors` in `Argparse.ColorizingHelpFormatter` class.
-`_level_name` in `Formatters._Formatter` class and `level_colors` in `Formatters.ColorizingFormatter` class.
-`sign_colors` in `PPrint.PrettyPrinter` class.
-`colors` in `TreePrint.TreePrint.Node` class.
+Added constant colors directly to the Colors module. Now you can do this:
+```python
+from log21 import print
+from log21.colors import GREEN, WHITE, RED
+
+print(GREEN + 'This' + WHITE + ' is' + RED + ' Red')
+```
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.5.3/README.md` & `log21-2.5.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -49,21 +49,23 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.5.3
+### 2.5.4
 
-Moved some dictionaries to `__init__` methods.
-`colors` in `Argparse.ColorizingHelpFormatter` class.
-`_level_name` in `Formatters._Formatter` class and `level_colors` in `Formatters.ColorizingFormatter` class.
-`sign_colors` in `PPrint.PrettyPrinter` class.
-`colors` in `TreePrint.TreePrint.Node` class.
+Added constant colors directly to the Colors module. Now you can do this:
+```python
+from log21 import print
+from log21.colors import GREEN, WHITE, RED
+
+print(GREEN + 'This' + WHITE + ' is' + RED + ' Red')
+```
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.5.3/log21/Argparse.py` & `log21-2.5.4/log21/Argparse.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/log21/CrashReporter/Formatters.py` & `log21-2.5.4/log21/CrashReporter/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/log21/CrashReporter/Reporters.py` & `log21-2.5.4/log21/CrashReporter/Reporters.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/log21/FileHandler.py` & `log21-2.5.4/log21/FileHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/log21/Formatters.py` & `log21-2.5.4/log21/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/log21/Logger.py` & `log21-2.5.4/log21/Logger.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/log21/LoggingWindow.py` & `log21-2.5.4/log21/LoggingWindow.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/log21/Manager.py` & `log21-2.5.4/log21/Manager.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/log21/PPrint.py` & `log21-2.5.4/log21/PPrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/log21/ProgressBar.py` & `log21-2.5.4/log21/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/log21/StreamHandler.py` & `log21-2.5.4/log21/StreamHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/log21/TreePrint.py` & `log21-2.5.4/log21/TreePrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/log21/__init__.py` & `log21-2.5.4/log21/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from log21.Argparse import ColorizingArgumentParser
 from log21.FileHandler import DecolorizingFileHandler
 from log21.LoggingWindow import LoggingWindow, LoggingWindowHandler
 from log21.StreamHandler import ColorizingStreamHandler, StreamHandler
 from log21.Formatters import ColorizingFormatter, DecolorizingFormatter
 from log21.Colors import Colors, get_color, get_colors, ansi_escape, get_color_name, closest_color
 
-__version__ = "2.5.3"
+__version__ = "2.5.4"
 __author__ = "CodeWriter21 (Mehrad Pooryoussof)"
 __github__ = "Https://GitHub.com/MPCodeWriter21/log21"
 __all__ = ['ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter', 'DecolorizingFormatter',
            'get_logger', 'Logger', 'Colors', 'get_color', 'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN',
            'INFO', 'DEBUG', 'NOTSET', 'INPUT', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter', 'pformat',
            'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager', 'get_color_name', 'closest_color',
            'ansi_escape', '__version__', '__author__', '__github__', 'debug', 'info', 'warning', 'warn', 'error',
```

### Comparing `log21-2.5.3/log21.egg-info/PKG-INFO` & `log21-2.5.4/log21.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.5.3
+Version: 2.5.4
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
 Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
 Project-URL: Source, https://github.com/MPCodeWriter21/log21
 Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
@@ -71,21 +71,23 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.5.3
+### 2.5.4
 
-Moved some dictionaries to `__init__` methods.
-`colors` in `Argparse.ColorizingHelpFormatter` class.
-`_level_name` in `Formatters._Formatter` class and `level_colors` in `Formatters.ColorizingFormatter` class.
-`sign_colors` in `PPrint.PrettyPrinter` class.
-`colors` in `TreePrint.TreePrint.Node` class.
+Added constant colors directly to the Colors module. Now you can do this:
+```python
+from log21 import print
+from log21.colors import GREEN, WHITE, RED
+
+print(GREEN + 'This' + WHITE + ' is' + RED + ' Red')
+```
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.5.3/log21.egg-info/SOURCES.txt` & `log21-2.5.4/log21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `log21-2.5.3/pyproject.toml` & `log21-2.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,13 +21,13 @@
   "Operating System :: Unix",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS :: MacOS X"
 ]
 dependencies = [
   "webcolors"
 ]
-version = "2.5.3"
+version = "2.5.4"
 
 [project.urls]
 Homepage = "https://github.com/MPCodeWriter21/log21"
 Donations = "https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md"
 Source = "https://github.com/MPCodeWriter21/log21"
```


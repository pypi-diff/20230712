# Comparing `tmp/selenium_remote-0.1.2.tar.gz` & `tmp/selenium_remote-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_remote-0.1.2.tar", max compression
+gzip compressed data, was "selenium_remote-0.1.3.tar", max compression
```

## Comparing `selenium_remote-0.1.2.tar` & `selenium_remote-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-07-11 13:29:28.122937 selenium_remote-0.1.2/LICENSE
--rw-r--r--   0        0        0       91 2023-07-11 13:29:28.122937 selenium_remote-0.1.2/README.md
--rw-r--r--   0        0        0      748 2023-07-11 14:12:34.320502 selenium_remote-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 13:36:32.954532 selenium_remote-0.1.2/selenium_remote/__init__.py
--rw-r--r--   0        0        0      139 2023-07-11 13:54:12.017532 selenium_remote-0.1.2/selenium_remote/main.py
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 selenium_remote-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-11 13:29:28.000000 selenium_remote-0.1.3/LICENSE
+-rw-r--r--   0        0        0       91 2023-07-11 13:29:28.000000 selenium_remote-0.1.3/README.md
+-rw-r--r--   0        0        0      624 2023-07-12 11:47:00.879255 selenium_remote-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 13:36:32.000000 selenium_remote-0.1.3/selenium_remote/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-12 11:46:42.715270 selenium_remote-0.1.3/selenium_remote/main.py
+-rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 selenium_remote-0.1.3/PKG-INFO
```

### Comparing `selenium_remote-0.1.2/LICENSE` & `selenium_remote-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_remote-0.1.2/PKG-INFO` & `selenium_remote-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-remote
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for haldling and using a selenium grid server.
 Author: George Pamfilis
 Author-email: gpamfilis@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


# Comparing `tmp/selenium_remote-0.1.3.tar.gz` & `tmp/selenium_remote-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium_remote-0.1.3.tar", max compression
+gzip compressed data, was "selenium_remote-0.1.4.tar", max compression
```

## Comparing `selenium_remote-0.1.3.tar` & `selenium_remote-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2023-07-11 13:29:28.000000 selenium_remote-0.1.3/LICENSE
--rw-r--r--   0        0        0       91 2023-07-11 13:29:28.000000 selenium_remote-0.1.3/README.md
--rw-r--r--   0        0        0      624 2023-07-12 11:47:00.879255 selenium_remote-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 13:36:32.000000 selenium_remote-0.1.3/selenium_remote/__init__.py
--rw-r--r--   0        0        0     1709 2023-07-12 11:46:42.715270 selenium_remote-0.1.3/selenium_remote/main.py
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 selenium_remote-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-11 13:29:28.000000 selenium_remote-0.1.4/LICENSE
+-rw-r--r--   0        0        0       91 2023-07-11 13:29:28.000000 selenium_remote-0.1.4/README.md
+-rw-r--r--   0        0        0      735 2023-07-12 11:53:11.546946 selenium_remote-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 13:36:32.000000 selenium_remote-0.1.4/selenium_remote/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-12 11:46:42.715270 selenium_remote-0.1.4/selenium_remote/main.py
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 selenium_remote-0.1.4/PKG-INFO
```

### Comparing `selenium_remote-0.1.3/LICENSE` & `selenium_remote-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_remote-0.1.3/pyproject.toml` & `selenium_remote-0.1.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "selenium-remote"
-version = "0.1.3"
-description = "A package for haldling and using a selenium grid server."
+version = "0.1.4"
+description = "A package for handling and using a selenium grid server."
 authors = ["George Pamfilis <gpamfilis@gmail.com>"]
 readme = "README.md"
 packages = [{include = "selenium_remote"}]
+repository = "https://github.com/gpamfilis/selenium-remote"
+keywords = ["selenium", "scraping", "webscraping"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fake-useragent = "^1.1.3"
 selenium = "^4.10.0"
 webdriver-manager = "^3.8.6"
```

### Comparing `selenium_remote-0.1.3/selenium_remote/main.py` & `selenium_remote-0.1.4/selenium_remote/main.py`

 * *Files identical despite different names*

### Comparing `selenium_remote-0.1.3/PKG-INFO` & `selenium_remote-0.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: selenium-remote
-Version: 0.1.3
-Summary: A package for haldling and using a selenium grid server.
+Version: 0.1.4
+Summary: A package for handling and using a selenium grid server.
+Home-page: https://github.com/gpamfilis/selenium-remote
+Keywords: selenium,scraping,webscraping
 Author: George Pamfilis
 Author-email: gpamfilis@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fake-useragent (>=1.1.3,<2.0.0)
 Requires-Dist: selenium (>=4.10.0,<5.0.0)
 Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0)
+Project-URL: Repository, https://github.com/gpamfilis/selenium-remote
 Description-Content-Type: text/markdown
 
 # selenium-remote
 This package contains utils for remote connections to a selenium server.
```


# Comparing `tmp/pytest_textual_snapshot-0.1.0.tar.gz` & `tmp/pytest_textual_snapshot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_textual_snapshot-0.1.0.tar", max compression
+gzip compressed data, was "pytest_textual_snapshot-0.2.0.tar", max compression
```

## Comparing `pytest_textual_snapshot-0.1.0.tar` & `pytest_textual_snapshot-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1078 2023-06-27 13:20:54.234165 pytest_textual_snapshot-0.1.0/LICENSE
--rw-r--r--   0        0        0     1562 2023-06-27 13:20:54.234390 pytest_textual_snapshot-0.1.0/README.md
--rw-r--r--   0        0        0     1474 2023-06-27 13:20:54.234499 pytest_textual_snapshot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7553 2023-06-27 13:20:54.234651 pytest_textual_snapshot-0.1.0/pytest_textual_snapshot.py
--rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 pytest_textual_snapshot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-27 13:20:54.234165 pytest_textual_snapshot-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1562 2023-06-27 13:20:54.234390 pytest_textual_snapshot-0.2.0/README.md
+-rw-r--r--   0        0        0     1503 2023-07-12 14:34:46.975557 pytest_textual_snapshot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7553 2023-06-27 13:20:54.234651 pytest_textual_snapshot-0.2.0/pytest_textual_snapshot.py
+-rw-r--r--   0        0        0    11112 2023-06-27 13:20:54.234850 pytest_textual_snapshot-0.2.0/resources/snapshot_report_template.jinja2
+-rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 pytest_textual_snapshot-0.2.0/PKG-INFO
```

### Comparing `pytest_textual_snapshot-0.1.0/LICENSE` & `pytest_textual_snapshot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_textual_snapshot-0.1.0/README.md` & `pytest_textual_snapshot-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_textual_snapshot-0.1.0/pyproject.toml` & `pytest_textual_snapshot-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-textual-snapshot"
-version = "0.1.0"
+version = "0.2.0"
 description = "Snapshot testing for Textual apps"
 authors = ["Darren Burns <darren@textualize.io>"]
 maintainers = ["Darren Burns <darren@textualize.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/darrenburns/pytest-textual-snapshot"
 classifiers = [
@@ -23,14 +23,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License"
 ]
+include = ["resources/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 pytest = ">=7.0.0"
 rich = ">=12.0.0"
 textual = ">=0.28.0"
 syrupy = ">=3.0.0"
```

### Comparing `pytest_textual_snapshot-0.1.0/pytest_textual_snapshot.py` & `pytest_textual_snapshot-0.2.0/pytest_textual_snapshot.py`

 * *Files identical despite different names*

### Comparing `pytest_textual_snapshot-0.1.0/PKG-INFO` & `pytest_textual_snapshot-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-textual-snapshot
-Version: 0.1.0
+Version: 0.2.0
 Summary: Snapshot testing for Textual apps
 Home-page: https://github.com/darrenburns/pytest-textual-snapshot
 License: MIT
 Author: Darren Burns
 Author-email: darren@textualize.io
 Maintainer: Darren Burns
 Maintainer-email: darren@textualize.io
```


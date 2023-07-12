# Comparing `tmp/appins-0.2.9.tar.gz` & `tmp/appins-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appins-0.2.9.tar", last modified: Sun Feb 26 21:43:41 2023, max compression
+gzip compressed data, was "appins-0.3.1.tar", last modified: Wed Jul 12 08:51:55 2023, max compression
```

## Comparing `appins-0.2.9.tar` & `appins-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1342 2023-02-18 13:26:33.609851 appins-0.2.9/.gitignore
--rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 appins-0.2.9/LICENSE
--rw-r--r--   0        0        0      343 2023-02-18 14:52:19.365671 appins-0.2.9/Makefile
--rw-r--r--   0        0        0      370 2023-02-18 20:34:14.382069 appins-0.2.9/README.md
--rw-r--r--   0        0        0       22 2023-02-26 21:43:03.147163 appins-0.2.9/appins/__init__.py
--rw-r--r--   0        0        0       29 2023-02-18 20:04:53.442182 appins-0.2.9/appins/__main__.py
--rw-r--r--   0        0        0     5215 2023-02-26 21:23:01.918727 appins-0.2.9/appins/main.py
--rw-r--r--   0        0        0     2088 2023-02-25 05:36:41.437414 appins-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      106 2023-02-26 19:09:44.102582 appins-0.2.9/requirements.txt
--rw-r--r--   0        0        0      272 2023-02-18 14:47:26.295062 appins-0.2.9/setup.cfg
--rw-r--r--   0        0        0      106 2023-02-18 19:50:11.030745 appins-0.2.9/test_build.py
--rw-r--r--   0        0        0     1755 1970-01-01 00:00:00.000000 appins-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1342 2023-02-18 13:26:33.609851 appins-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 appins-0.3.1/LICENSE
+-rw-r--r--   0        0        0      343 2023-02-18 14:52:19.365671 appins-0.3.1/Makefile
+-rw-r--r--   0        0        0      370 2023-02-18 20:34:14.382069 appins-0.3.1/README.md
+-rw-r--r--   0        0        0       22 2023-07-12 08:50:21.966094 appins-0.3.1/appins/__init__.py
+-rw-r--r--   0        0        0       29 2023-02-18 20:04:53.442182 appins-0.3.1/appins/__main__.py
+-rw-r--r--   0        0        0     8763 2023-07-05 20:08:43.691377 appins-0.3.1/appins/main.py
+-rw-r--r--   0        0        0     4759 2023-07-12 08:49:03.528997 appins-0.3.1/appins/prompt_template.txt
+-rw-r--r--   0        0        0     2193 2023-07-12 08:50:05.145867 appins-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      198 2023-07-12 08:49:09.393082 appins-0.3.1/requirements.txt
+-rw-r--r--   0        0        0      272 2023-02-18 14:47:26.295062 appins-0.3.1/setup.cfg
+-rw-r--r--   0        0        0      106 2023-02-18 19:50:11.030745 appins-0.3.1/test_build.py
+-rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 appins-0.3.1/PKG-INFO
```

### Comparing `appins-0.2.9/.gitignore` & `appins-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `appins-0.2.9/LICENSE` & `appins-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `appins-0.2.9/pyproject.toml` & `appins-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,18 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Internet :: WWW/HTTP :: Session",
 ]
 requires-python = ">=3.7"
 dependencies = [
     "typer >= 0.7.0",
     "cookiecutter >= 2.1.1",
+    "torch >= 2.0.0",
+    "transformers >= 4.30.0",
+    "accelerate >= 0.20.0",
+    "colorama >= 0.4.6",
 ]
 
 [project.scripts]
 appins = "appins.main:app"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `appins-0.2.9/PKG-INFO` & `appins-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appins
-Version: 0.2.9
+Version: 0.3.1
 Summary: appins - cli tool for enabledu ecosystem
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Requires-Dist: typer >= 0.7.0
 Requires-Dist: cookiecutter >= 2.1.1
+Requires-Dist: torch >= 2.0.0
+Requires-Dist: transformers >= 4.30.0
+Requires-Dist: accelerate >= 0.20.0
+Requires-Dist: colorama >= 0.4.6
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: requests ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pytest-asyncio ; extra == "dev"
 Requires-Dist: flake8-docstrings ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
```


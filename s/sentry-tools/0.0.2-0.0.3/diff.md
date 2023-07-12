# Comparing `tmp/sentry-tools-0.0.2.tar.gz` & `tmp/sentry-tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-tools-0.0.2.tar", last modified: Sun Mar  5 16:08:12 2023, max compression
+gzip compressed data, was "sentry-tools-0.0.3.tar", last modified: Wed Jul 12 17:35:12 2023, max compression
```

## Comparing `sentry-tools-0.0.2.tar` & `sentry-tools-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:08:12.861420 sentry-tools-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    26022 2023-03-05 16:08:08.000000 sentry-tools-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-05 16:08:08.000000 sentry-tools-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-05 16:08:12.861420 sentry-tools-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-05 16:08:08.000000 sentry-tools-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:08:12.861420 sentry-tools-0.0.2/sentry_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-05 16:08:08.000000 sentry-tools-0.0.2/sentry_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-05 16:08:08.000000 sentry-tools-0.0.2/sentry_tools/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-05 16:08:08.000000 sentry-tools-0.0.2/sentry_tools/span.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 16:08:12.861420 sentry-tools-0.0.2/sentry_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-05 16:08:12.000000 sentry-tools-0.0.2/sentry_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-05 16:08:12.000000 sentry-tools-0.0.2/sentry_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 16:08:12.000000 sentry-tools-0.0.2/sentry_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 16:08:12.000000 sentry-tools-0.0.2/sentry_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-05 16:08:12.000000 sentry-tools-0.0.2/sentry_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-05 16:08:12.865419 sentry-tools-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 16:08:08.000000 sentry-tools-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:12.567066 sentry-tools-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    26022 2023-07-12 17:35:01.000000 sentry-tools-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-12 17:35:01.000000 sentry-tools-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-12 17:35:12.567066 sentry-tools-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-12 17:35:01.000000 sentry-tools-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:12.567066 sentry-tools-0.0.3/sentry_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-12 17:35:01.000000 sentry-tools-0.0.3/sentry_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-12 17:35:01.000000 sentry-tools-0.0.3/sentry_tools/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-12 17:35:01.000000 sentry-tools-0.0.3/sentry_tools/span.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:35:12.567066 sentry-tools-0.0.3/sentry_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-12 17:35:12.000000 sentry-tools-0.0.3/sentry_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-12 17:35:12.000000 sentry-tools-0.0.3/sentry_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:35:12.000000 sentry-tools-0.0.3/sentry_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:35:12.000000 sentry-tools-0.0.3/sentry_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-12 17:35:12.000000 sentry-tools-0.0.3/sentry_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-12 17:35:12.567066 sentry-tools-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:35:01.000000 sentry-tools-0.0.3/setup.py
```

### Comparing `sentry-tools-0.0.2/LICENSE` & `sentry-tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-tools-0.0.2/PKG-INFO` & `sentry-tools-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for sentry
 Home-page: https://github.com/Voltane-EU/sentry-tools
 Author: Manuel Stingl
 Author-email: opensource@voltane.eu
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `sentry-tools-0.0.2/sentry_tools.egg-info/PKG-INFO` & `sentry-tools-0.0.3/sentry_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for sentry
 Home-page: https://github.com/Voltane-EU/sentry-tools
 Author: Manuel Stingl
 Author-email: opensource@voltane.eu
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `sentry-tools-0.0.2/setup.cfg` & `sentry-tools-0.0.3/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sentry-tools
-version = 0.0.2
+version = 0.0.3
 author = Manuel Stingl
 author_email = opensource@voltane.eu
 description = Tools for sentry
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU LGPLv2.1
 classifiers =
```


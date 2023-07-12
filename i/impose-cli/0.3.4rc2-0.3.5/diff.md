# Comparing `tmp/impose-cli-0.3.4rc2.tar.gz` & `tmp/impose-cli-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.3.4rc2.tar", last modified: Wed Jul 12 07:54:17 2023, max compression
+gzip compressed data, was "impose-cli-0.3.5.tar", last modified: Wed Jul 12 07:55:50 2023, max compression
```

## Comparing `impose-cli-0.3.4rc2.tar` & `impose-cli-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:54:17.677715 impose-cli-0.3.4rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-12 07:53:58.000000 impose-cli-0.3.4rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-12 07:54:17.677715 impose-cli-0.3.4rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-12 07:53:58.000000 impose-cli-0.3.4rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:54:17.677715 impose-cli-0.3.4rc2/impose_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:53:58.000000 impose-cli-0.3.4rc2/impose_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-07-12 07:53:58.000000 impose-cli-0.3.4rc2/impose_cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-12 07:53:58.000000 impose-cli-0.3.4rc2/impose_cli/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-12 07:53:58.000000 impose-cli-0.3.4rc2/impose_cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-12 07:53:58.000000 impose-cli-0.3.4rc2/impose_cli/impose_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:54:17.677715 impose-cli-0.3.4rc2/impose_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-12 07:54:17.000000 impose-cli-0.3.4rc2/impose_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-12 07:54:17.000000 impose-cli-0.3.4rc2/impose_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 07:54:17.000000 impose-cli-0.3.4rc2/impose_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-12 07:54:17.000000 impose-cli-0.3.4rc2/impose_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 07:54:17.000000 impose-cli-0.3.4rc2/impose_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 07:54:17.677715 impose-cli-0.3.4rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-12 07:53:58.000000 impose-cli-0.3.4rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:54:17.677715 impose-cli-0.3.4rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:53:58.000000 impose-cli-0.3.4rc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-12 07:53:58.000000 impose-cli-0.3.4rc2/tests/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:55:50.342055 impose-cli-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-12 07:55:29.000000 impose-cli-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-12 07:55:50.342055 impose-cli-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-12 07:55:29.000000 impose-cli-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:55:50.342055 impose-cli-0.3.5/impose_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:55:29.000000 impose-cli-0.3.5/impose_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11388 2023-07-12 07:55:29.000000 impose-cli-0.3.5/impose_cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-12 07:55:29.000000 impose-cli-0.3.5/impose_cli/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-12 07:55:29.000000 impose-cli-0.3.5/impose_cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-12 07:55:29.000000 impose-cli-0.3.5/impose_cli/impose_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:55:50.342055 impose-cli-0.3.5/impose_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-12 07:55:50.000000 impose-cli-0.3.5/impose_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-12 07:55:50.000000 impose-cli-0.3.5/impose_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 07:55:50.000000 impose-cli-0.3.5/impose_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-12 07:55:50.000000 impose-cli-0.3.5/impose_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 07:55:50.000000 impose-cli-0.3.5/impose_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 07:55:50.342055 impose-cli-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-12 07:55:29.000000 impose-cli-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:55:50.342055 impose-cli-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:55:29.000000 impose-cli-0.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-12 07:55:29.000000 impose-cli-0.3.5/tests/simple.py
```

### Comparing `impose-cli-0.3.4rc2/LICENSE` & `impose-cli-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.4rc2/README.md` & `impose-cli-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.4rc2/impose_cli/_utils.py` & `impose-cli-0.3.5/impose_cli/_utils.py`

 * *Files identical despite different names*

### Comparing `impose-cli-0.3.4rc2/impose_cli/impose_cli.py` & `impose-cli-0.3.5/impose_cli/impose_cli.py`

 * *Files identical despite different names*


# Comparing `tmp/ttb-0.0.tar.gz` & `tmp/ttb-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttb-0.0.tar", last modified: Wed Jul 12 10:58:46 2023, max compression
+gzip compressed data, was "ttb-0.1.tar", last modified: Wed Jul 12 11:38:43 2023, max compression
```

## Comparing `ttb-0.0.tar` & `ttb-0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 10:58:46.335877 ttb-0.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-12 10:58:03.000000 ttb-0.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2023-07-12 10:58:03.000000 ttb-0.0/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)      466 2023-07-12 10:58:46.335877 ttb-0.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      131 2023-07-12 10:58:03.000000 ttb-0.0/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-12 10:58:46.335877 ttb-0.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      467 2023-07-12 10:58:34.000000 ttb-0.0/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 10:58:46.335877 ttb-0.0/ttb/
--rw-r--r--   0 runner    (1000) runner    (1000)      511 2023-07-12 10:58:03.000000 ttb-0.0/ttb/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 10:58:46.335877 ttb-0.0/ttb.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      466 2023-07-12 10:58:46.000000 ttb-0.0/ttb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      198 2023-07-12 10:58:46.000000 ttb-0.0/ttb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-12 10:58:46.000000 ttb-0.0/ttb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-12 10:58:46.000000 ttb-0.0/ttb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1000) runner    (1000)        4 2023-07-12 10:58:46.000000 ttb-0.0/ttb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 11:38:43.977411 ttb-0.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1073 2023-07-12 10:58:03.000000 ttb-0.1/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2023-07-12 10:58:03.000000 ttb-0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)      734 2023-07-12 11:38:43.977411 ttb-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      379 2023-07-12 11:38:12.000000 ttb-0.1/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-12 11:38:43.989411 ttb-0.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      487 2023-07-12 11:35:20.000000 ttb-0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 11:38:43.977411 ttb-0.1/ttb/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1040 2023-07-12 11:32:59.000000 ttb-0.1/ttb/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 11:38:43.977411 ttb-0.1/ttb.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      734 2023-07-12 11:38:43.000000 ttb-0.1/ttb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      198 2023-07-12 11:38:43.000000 ttb-0.1/ttb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-12 11:38:43.000000 ttb-0.1/ttb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-12 11:38:43.000000 ttb-0.1/ttb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)        4 2023-07-12 11:38:43.000000 ttb-0.1/ttb.egg-info/top_level.txt
```

### Comparing `ttb-0.0/LICENSE` & `ttb-0.1/LICENSE`

 * *Files identical despite different names*


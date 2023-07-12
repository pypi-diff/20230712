# Comparing `tmp/barlidb-0.1.5.tar.gz` & `tmp/barlidb-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barlidb-0.1.5.tar", last modified: Wed Jul 12 10:49:18 2023, max compression
+gzip compressed data, was "barlidb-0.1.6.tar", last modified: Wed Jul 12 11:00:58 2023, max compression
```

## Comparing `barlidb-0.1.5.tar` & `barlidb-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 10:49:18.840472 barlidb-0.1.5/
--rw-rw-rw-   0        0        0      133 2023-07-12 10:49:18.840472 barlidb-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      998 2023-07-12 10:39:05.000000 barlidb-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 10:49:18.835430 barlidb-0.1.5/barlidb/
--rw-rw-rw-   0        0        0        0 2023-07-12 10:29:47.000000 barlidb-0.1.5/barlidb/__init__.py
--rw-rw-rw-   0        0        0       13 2023-07-12 07:44:26.000000 barlidb-0.1.5/barlidb/config.py
--rw-rw-rw-   0        0        0     1353 2023-07-12 10:43:46.000000 barlidb-0.1.5/barlidb/db.py
--rw-rw-rw-   0        0        0      314 2023-07-12 07:39:51.000000 barlidb-0.1.5/barlidb/functions.py
--rw-rw-rw-   0        0        0      632 2023-07-12 09:49:44.000000 barlidb-0.1.5/barlidb/test.py
-drwxrwxrwx   0        0        0        0 2023-07-12 10:49:18.839466 barlidb-0.1.5/barlidb.egg-info/
--rw-rw-rw-   0        0        0      133 2023-07-12 10:49:18.000000 barlidb-0.1.5/barlidb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-07-12 10:49:18.000000 barlidb-0.1.5/barlidb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 10:49:18.000000 barlidb-0.1.5/barlidb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-12 10:49:18.000000 barlidb-0.1.5/barlidb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-07-12 10:49:18.000000 barlidb-0.1.5/barlidb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 10:49:18.841549 barlidb-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      228 2023-07-12 10:48:29.000000 barlidb-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:00:58.247406 barlidb-0.1.6/
+-rw-rw-rw-   0        0        0     1174 2023-07-12 11:00:58.248607 barlidb-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      998 2023-07-12 10:39:05.000000 barlidb-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 11:00:58.243141 barlidb-0.1.6/barlidb/
+-rw-rw-rw-   0        0        0        0 2023-07-12 10:29:47.000000 barlidb-0.1.6/barlidb/__init__.py
+-rw-rw-rw-   0        0        0       13 2023-07-12 07:44:26.000000 barlidb-0.1.6/barlidb/config.py
+-rw-rw-rw-   0        0        0     1522 2023-07-12 10:58:38.000000 barlidb-0.1.6/barlidb/db.py
+-rw-rw-rw-   0        0        0      314 2023-07-12 07:39:51.000000 barlidb-0.1.6/barlidb/functions.py
+-rw-rw-rw-   0        0        0      632 2023-07-12 09:49:44.000000 barlidb-0.1.6/barlidb/test.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:00:58.247406 barlidb-0.1.6/barlidb.egg-info/
+-rw-rw-rw-   0        0        0     1174 2023-07-12 11:00:58.000000 barlidb-0.1.6/barlidb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-07-12 11:00:58.000000 barlidb-0.1.6/barlidb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:00:58.000000 barlidb-0.1.6/barlidb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-12 10:49:18.000000 barlidb-0.1.6/barlidb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-07-12 11:00:58.000000 barlidb-0.1.6/barlidb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 11:00:58.248607 barlidb-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      332 2023-07-12 10:59:01.000000 barlidb-0.1.6/setup.py
```

### Comparing `barlidb-0.1.5/README.md` & `barlidb-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `barlidb-0.1.5/barlidb/test.py` & `barlidb-0.1.6/barlidb/test.py`

 * *Files identical despite different names*


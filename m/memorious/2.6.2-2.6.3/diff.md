# Comparing `tmp/memorious-2.6.2.tar.gz` & `tmp/memorious-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memorious-2.6.2.tar", last modified: Thu May  4 11:54:31 2023, max compression
+gzip compressed data, was "memorious-2.6.3.tar", last modified: Wed Jul 12 10:28:24 2023, max compression
```

## Comparing `memorious-2.6.2.tar` & `memorious-2.6.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.941674 memorious-2.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 11:52:27.000000 memorious-2.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-04 11:54:31.941674 memorious-2.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-04 11:52:27.000000 memorious-2.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.933674 memorious-2.6.2/memorious/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.937674 memorious-2.6.2/memorious/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/asp.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    29876 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/helpers/ua.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.937674 memorious-2.6.2/memorious/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/logic/stage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.937674 memorious-2.6.2/memorious/model/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/model/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/model/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.937674 memorious-2.6.2/memorious/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/documentcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/ftm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/operations/webdav.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.941674 memorious-2.6.2/memorious/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_documentcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/tests/test_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-04 11:52:27.000000 memorious-2.6.2/memorious/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:54:31.933674 memorious-2.6.2/memorious.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:54:02.000000 memorious-2.6.2/memorious.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 11:54:31.000000 memorious-2.6.2/memorious.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 11:54:31.941674 memorious-2.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-04 11:52:27.000000 memorious-2.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:28:24.978335 memorious-2.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-12 10:26:17.000000 memorious-2.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-12 10:28:24.978335 memorious-2.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-12 10:26:17.000000 memorious-2.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:28:24.974335 memorious-2.6.3/memorious/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:28:24.974335 memorious-2.6.3/memorious/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/helpers/asp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/helpers/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/helpers/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/helpers/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/helpers/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29876 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/helpers/ua.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:28:24.974335 memorious-2.6.3/memorious/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/logic/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/logic/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/logic/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/logic/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/logic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/logic/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/logic/stage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:28:24.974335 memorious-2.6.3/memorious/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/model/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/model/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:28:24.978335 memorious-2.6.3/memorious/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/documentcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/ftm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/operations/webdav.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:28:24.978335 memorious-2.6.3/memorious/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/tests/test_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/tests/test_documentcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/tests/test_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/tests/test_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-12 10:26:17.000000 memorious-2.6.3/memorious/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:28:24.974335 memorious-2.6.3/memorious.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-12 10:28:24.000000 memorious-2.6.3/memorious.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-12 10:28:24.000000 memorious-2.6.3/memorious.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:28:24.000000 memorious-2.6.3/memorious.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-12 10:28:24.000000 memorious-2.6.3/memorious.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:28:24.000000 memorious-2.6.3/memorious.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:27:52.000000 memorious-2.6.3/memorious.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-12 10:28:24.000000 memorious-2.6.3/memorious.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 10:28:24.000000 memorious-2.6.3/memorious.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-12 10:28:24.978335 memorious-2.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-07-12 10:26:17.000000 memorious-2.6.3/setup.py
```

### Comparing `memorious-2.6.2/LICENSE` & `memorious-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/PKG-INFO` & `memorious-2.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memorious
-Version: 2.6.2
+Version: 2.6.3
 Summary: A minimalistic, recursive web crawling library for Python.
 Home-page: http://github.com/alephdata/memorious
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `memorious-2.6.2/README.rst` & `memorious-2.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/__init__.py` & `memorious-2.6.3/memorious/__init__.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/cli.py` & `memorious-2.6.3/memorious/cli.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/core.py` & `memorious-2.6.3/memorious/core.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/exc.py` & `memorious-2.6.3/memorious/exc.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/helpers/__init__.py` & `memorious-2.6.3/memorious/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/helpers/asp.py` & `memorious-2.6.3/memorious/helpers/asp.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/helpers/dates.py` & `memorious-2.6.3/memorious/helpers/dates.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/helpers/ocr.py` & `memorious-2.6.3/memorious/helpers/ocr.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/helpers/rule.py` & `memorious-2.6.3/memorious/helpers/rule.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/helpers/ua.py` & `memorious-2.6.3/memorious/helpers/ua.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/logic/check.py` & `memorious-2.6.3/memorious/logic/check.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/logic/context.py` & `memorious-2.6.3/memorious/logic/context.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/logic/crawler.py` & `memorious-2.6.3/memorious/logic/crawler.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/logic/http.py` & `memorious-2.6.3/memorious/logic/http.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/logic/manager.py` & `memorious-2.6.3/memorious/logic/manager.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/logic/mime.py` & `memorious-2.6.3/memorious/logic/mime.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/logic/stage.py` & `memorious-2.6.3/memorious/logic/stage.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/model/crawl.py` & `memorious-2.6.3/memorious/model/crawl.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/model/queue.py` & `memorious-2.6.3/memorious/model/queue.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/operations/aleph.py` & `memorious-2.6.3/memorious/operations/aleph.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/operations/clean.py` & `memorious-2.6.3/memorious/operations/clean.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/operations/db.py` & `memorious-2.6.3/memorious/operations/db.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/operations/documentcloud.py` & `memorious-2.6.3/memorious/operations/documentcloud.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/operations/extract.py` & `memorious-2.6.3/memorious/operations/extract.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/operations/fetch.py` & `memorious-2.6.3/memorious/operations/fetch.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/operations/ftm.py` & `memorious-2.6.3/memorious/operations/ftm.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/operations/ftp.py` & `memorious-2.6.3/memorious/operations/ftp.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/operations/initializers.py` & `memorious-2.6.3/memorious/operations/initializers.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/operations/parse.py` & `memorious-2.6.3/memorious/operations/parse.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/operations/store.py` & `memorious-2.6.3/memorious/operations/store.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/operations/webdav.py` & `memorious-2.6.3/memorious/operations/webdav.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/settings.py` & `memorious-2.6.3/memorious/settings.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/tests/conftest.py` & `memorious-2.6.3/memorious/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/tests/test_context.py` & `memorious-2.6.3/memorious/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/tests/test_crawler.py` & `memorious-2.6.3/memorious/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/tests/test_documentcloud.py` & `memorious-2.6.3/memorious/tests/test_documentcloud.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/tests/test_extract.py` & `memorious-2.6.3/memorious/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/tests/test_http.py` & `memorious-2.6.3/memorious/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/tests/test_manager.py` & `memorious-2.6.3/memorious/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/tests/test_operations.py` & `memorious-2.6.3/memorious/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/tests/test_reporting.py` & `memorious-2.6.3/memorious/tests/test_reporting.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/tests/test_rule.py` & `memorious-2.6.3/memorious/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious/worker.py` & `memorious-2.6.3/memorious/worker.py`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious.egg-info/PKG-INFO` & `memorious-2.6.3/memorious.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memorious
-Version: 2.6.2
+Version: 2.6.3
 Summary: A minimalistic, recursive web crawling library for Python.
 Home-page: http://github.com/alephdata/memorious
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `memorious-2.6.2/memorious.egg-info/SOURCES.txt` & `memorious-2.6.3/memorious.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/memorious.egg-info/entry_points.txt` & `memorious-2.6.3/memorious.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `memorious-2.6.2/setup.py` & `memorious-2.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="memorious",
-    version="2.6.2",
+    version="2.6.3",
     description="A minimalistic, recursive web crawling library for Python.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     classifiers=[
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```


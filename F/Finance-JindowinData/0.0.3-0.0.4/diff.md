# Comparing `tmp/Finance-JindowinData-0.0.3.tar.gz` & `tmp/Finance-JindowinData-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-JindowinData-0.0.3.tar", last modified: Tue Jul 11 12:24:09 2023, max compression
+gzip compressed data, was "dist/Finance-JindowinData-0.0.4.tar", last modified: Wed Jul 12 13:13:16 2023, max compression
```

## Comparing `Finance-JindowinData-0.0.3.tar` & `Finance-JindowinData-0.0.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/Finance_JindowinData.egg-info/
--rw-r--r--   0 root         (0) root         (0)      174 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/Finance_JindowinData.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2082 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/Finance_JindowinData.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/Finance_JindowinData.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/Finance_JindowinData.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/Finance_JindowinData.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-29 08:26:08.000000 Finance-JindowinData-0.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      174 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-29 08:15:36.000000 Finance-JindowinData-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-29 07:55:41.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/db/
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-29 07:06:10.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70281 2023-06-29 06:30:53.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/db/db_factory.py
--rw-r--r--   0 root         (0) root         (0)     7325 2023-06-29 06:30:58.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/db/fetch_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/db/kd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 06:23:48.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/db/kd/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71640 2023-06-29 06:25:49.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/db/kd/kd_engine.py
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-29 06:23:14.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/db/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/ddb/
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-29 07:24:56.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/ddb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/ddb/ch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 06:41:28.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/ddb/ch/__init__.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-29 06:43:31.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/ddb/ch/ch_engine.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-07-11 06:57:12.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/ddb/ddb_factory.py
--rw-r--r--   0 root         (0) root         (0)     8873 2023-07-11 08:47:52.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/ddb/fetch_engine.py
--rw-r--r--   0 root         (0) root         (0)      969 2023-07-11 06:57:12.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/ddb/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/file/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-11 06:57:12.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/file/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7178 2023-07-11 08:47:34.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/file/fetch_engine.py
--rw-r--r--   0 root         (0) root         (0)     3596 2023-07-11 07:23:21.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/file/file_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/file/fl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 06:57:12.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/file/fl/__init__.py
--rw-r--r--   0 root         (0) root         (0)      406 2023-07-11 06:57:12.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/file/fl/fl_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/mg/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-29 06:48:50.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/mg/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1253 2023-06-29 06:59:21.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/mg/fetch_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/mg/kn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 06:53:04.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/mg/kn/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10556 2023-06-29 07:16:40.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/mg/kn/kn_engine.py
--rw-r--r--   0 root         (0) root         (0)     6160 2023-06-29 06:52:37.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/mg/mg_factory.py
--rw-r--r--   0 root         (0) root         (0)     2403 2023-06-29 06:57:08.000000 Finance-JindowinData-0.0.3/jdwdata/DataAPI/mg/mongodb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/RetrievalAPI/
--rw-r--r--   0 root         (0) root         (0)      136 2023-07-11 08:38:16.000000 Finance-JindowinData-0.0.3/jdwdata/RetrievalAPI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2240 2023-07-11 08:17:39.000000 Finance-JindowinData-0.0.3/jdwdata/RetrievalAPI/customized.py
--rw-r--r--   0 root         (0) root         (0)     5456 2023-07-11 08:06:36.000000 Finance-JindowinData-0.0.3/jdwdata/RetrievalAPI/ddb_customized.py
--rw-r--r--   0 root         (0) root         (0)     3637 2023-07-11 08:06:45.000000 Finance-JindowinData-0.0.3/jdwdata/RetrievalAPI/file_customized.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/
--rw-r--r--   0 root         (0) root         (0)      911 2023-07-11 07:00:46.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/dummy.py
--rw-r--r--   0 root         (0) root         (0)      444 2023-06-29 07:16:42.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/futures/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:03:02.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/futures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/futures/basic.py
--rw-r--r--   0 root         (0) root         (0)     3430 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/futures/classify.py
--rw-r--r--   0 root         (0) root         (0)     1774 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/futures/index_market.py
--rw-r--r--   0 root         (0) root         (0)     1089 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/futures/yields.py
--rw-r--r--   0 root         (0) root         (0)      732 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/index_component.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/index_market.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/stock/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:03:02.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/stock/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6638 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/stock/industry.py
--rw-r--r--   0 root         (0) root         (0)     2013 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/stock/market_stock.py
--rw-r--r--   0 root         (0) root         (0)    14721 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/stock/risk_model.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/stock/yields.py
--rw-r--r--   0 root         (0) root         (0)     2764 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/universe.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-06-29 07:03:02.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/utilities.py
--rw-r--r--   0 root         (0) root         (0)     4885 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/yields.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-11 12:23:52.000000 Finance-JindowinData-0.0.3/jdwdata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 08:41:12.000000 Finance-JindowinData-0.0.3/jdwdata/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8102 2023-07-11 08:47:55.000000 Finance-JindowinData-0.0.3/jdwdata/config/export_cfg.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-07-11 08:47:19.000000 Finance-JindowinData-0.0.3/jdwdata/config/mapping_cfg.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-07-11 10:28:38.000000 Finance-JindowinData-0.0.3/jdwdata/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/jdwdata/kdutils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 06:25:24.000000 Finance-JindowinData-0.0.3/jdwdata/kdutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5188 2023-06-29 06:28:29.000000 Finance-JindowinData-0.0.3/jdwdata/kdutils/logger.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-29 06:25:19.000000 Finance-JindowinData-0.0.3/jdwdata/kdutils/singleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/requirements/
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-11 12:22:53.000000 Finance-JindowinData-0.0.3/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 12:24:09.000000 Finance-JindowinData-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2141 2023-07-11 07:00:46.000000 Finance-JindowinData-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/Finance_JindowinData.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      174 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/Finance_JindowinData.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/Finance_JindowinData.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/Finance_JindowinData.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/Finance_JindowinData.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/Finance_JindowinData.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-29 08:26:08.000000 Finance-JindowinData-0.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      174 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-29 08:15:36.000000 Finance-JindowinData-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-29 07:55:41.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/db/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-29 07:06:10.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70281 2023-06-29 06:30:53.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/db/db_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7325 2023-06-29 06:30:58.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/db/fetch_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/db/kd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 06:23:48.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/db/kd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71640 2023-06-29 06:25:49.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/db/kd/kd_engine.py
+-rw-r--r--   0 root         (0) root         (0)      583 2023-06-29 06:23:14.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/db/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/ddb/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-29 07:24:56.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/ddb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/ddb/ch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 06:41:28.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/ddb/ch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-29 06:43:31.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/ddb/ch/ch_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2023-07-12 13:08:52.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/ddb/ddb_factory.py
+-rw-r--r--   0 root         (0) root         (0)     8895 2023-07-12 13:08:52.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/ddb/fetch_engine.py
+-rw-r--r--   0 root         (0) root         (0)      969 2023-07-12 06:15:15.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/ddb/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/file/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-12 06:15:15.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/file/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7401 2023-07-12 13:08:52.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/file/fetch_engine.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-07-12 06:15:15.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/file/file_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/file/fl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 06:15:15.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/file/fl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      406 2023-07-12 06:15:15.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/file/fl/fl_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/mg/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-29 06:48:50.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/mg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-06-29 06:59:21.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/mg/fetch_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/mg/kn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 06:53:04.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/mg/kn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10556 2023-06-29 07:16:40.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/mg/kn/kn_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6160 2023-06-29 06:52:37.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/mg/mg_factory.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-06-29 06:57:08.000000 Finance-JindowinData-0.0.4/jdwdata/DataAPI/mg/mongodb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/RetrievalAPI/
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-12 06:15:15.000000 Finance-JindowinData-0.0.4/jdwdata/RetrievalAPI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-07-12 06:15:15.000000 Finance-JindowinData-0.0.4/jdwdata/RetrievalAPI/customized.py
+-rw-r--r--   0 root         (0) root         (0)     5556 2023-07-12 13:08:52.000000 Finance-JindowinData-0.0.4/jdwdata/RetrievalAPI/ddb_customized.py
+-rw-r--r--   0 root         (0) root         (0)     3637 2023-07-12 06:15:15.000000 Finance-JindowinData-0.0.4/jdwdata/RetrievalAPI/file_customized.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/
+-rw-r--r--   0 root         (0) root         (0)      911 2023-07-12 06:15:15.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/dummy.py
+-rw-r--r--   0 root         (0) root         (0)      444 2023-06-29 07:16:42.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/futures/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:03:02.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/futures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/futures/basic.py
+-rw-r--r--   0 root         (0) root         (0)     3430 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/futures/classify.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/futures/index_market.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/futures/yields.py
+-rw-r--r--   0 root         (0) root         (0)      732 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/index_component.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/index_market.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/stock/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 07:03:02.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/stock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6638 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/stock/industry.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/stock/market_stock.py
+-rw-r--r--   0 root         (0) root         (0)    14721 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/stock/risk_model.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/stock/yields.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/universe.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-29 07:03:02.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     4885 2023-06-29 07:04:08.000000 Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/yields.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-12 13:12:38.000000 Finance-JindowinData-0.0.4/jdwdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 06:15:15.000000 Finance-JindowinData-0.0.4/jdwdata/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8059 2023-07-12 13:08:52.000000 Finance-JindowinData-0.0.4/jdwdata/config/export_cfg.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-07-12 06:15:15.000000 Finance-JindowinData-0.0.4/jdwdata/config/mapping_cfg.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-07-12 06:15:15.000000 Finance-JindowinData-0.0.4/jdwdata/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/jdwdata/kdutils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 06:25:24.000000 Finance-JindowinData-0.0.4/jdwdata/kdutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5188 2023-06-29 06:28:29.000000 Finance-JindowinData-0.0.4/jdwdata/kdutils/logger.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-29 06:25:19.000000 Finance-JindowinData-0.0.4/jdwdata/kdutils/singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/requirements/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-12 06:15:15.000000 Finance-JindowinData-0.0.4/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 13:13:16.000000 Finance-JindowinData-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-07-11 07:00:46.000000 Finance-JindowinData-0.0.4/setup.py
```

### Comparing `Finance-JindowinData-0.0.3/Finance_JindowinData.egg-info/SOURCES.txt` & `Finance-JindowinData-0.0.4/Finance_JindowinData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/DataAPI/db/db_factory.py` & `Finance-JindowinData-0.0.4/jdwdata/DataAPI/db/db_factory.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/DataAPI/db/fetch_engine.py` & `Finance-JindowinData-0.0.4/jdwdata/DataAPI/db/fetch_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/DataAPI/db/kd/kd_engine.py` & `Finance-JindowinData-0.0.4/jdwdata/DataAPI/db/kd/kd_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/DataAPI/db/utilities.py` & `Finance-JindowinData-0.0.4/jdwdata/DataAPI/db/utilities.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/DataAPI/ddb/ddb_factory.py` & `Finance-JindowinData-0.0.4/jdwdata/DataAPI/ddb/ddb_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def __init__(self, engine_class, url=None):
         self._fetch_engine = self.create_engine(engine_class, url=url)
 
 
 class CustomizeFactory(EngineFactory):
     def allign_data(self, data, table_name, begin_date=None, end_date=None, codes=None):
-        return self._fetch_engine.exportCfg.handle_allignment(table_name, begin_date, end_date, codes, data)
+        return self._fetch_engine.exportCfg.handle_allignment(table_name, begin_date, end_date, codes, data, self._fetch_engine.get_all_codes())
 
     def del_flag(self, data):
         if data is not None and 'flag' in data.columns:
             del data['flag']
         return data
 
     def custom(self, clause_list, table, columns=None, format_data=0):
```

### Comparing `Finance-JindowinData-0.0.3/jdwdata/DataAPI/ddb/fetch_engine.py` & `Finance-JindowinData-0.0.4/jdwdata/DataAPI/ddb/fetch_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,12 +209,12 @@
 
                 data = self._engine.ddb_engine().run(sql)
                 if len(data) > 0:
                     if column != '':
                         data = self.exportCfg.handle_transpose(
                             data, column, table_name)
                         data = self.exportCfg.handle_allignment(
-                            table_name, start_date, end_date, codes, data)
+                            table_name, start_date, end_date, codes, data, self.get_all_codes())
                         data = self.exportCfg.handle_map_cond(
                             data, table_name, params.get('cond', None))
                     return data
         return None
```

### Comparing `Finance-JindowinData-0.0.3/jdwdata/DataAPI/ddb/utilities.py` & `Finance-JindowinData-0.0.4/jdwdata/DataAPI/ddb/utilities.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/DataAPI/file/fetch_engine.py` & `Finance-JindowinData-0.0.4/jdwdata/DataAPI/file/fetch_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,20 @@
             return sub_folder_name
         return subfolder
 
     def get_template(self):
         df = pd.read_feather(os.path.join(self.base_dir, 'template.fea'))
         return df
 
+    def get_all_codes(self):
+        df = pd.read_feather(os.path.join(self.base_dir, 'template.fea'))
+        all_codes = list(df.columns)
+        all_codes.remove('index')
+        return all_codes
+
     def get_clause_date(self, caluse, symbol, trans_indexs):
         if symbol in caluse:
             tmpstrs = caluse.split(symbol)
             col = tmpstrs[0].replace(' ', '')
             if (isinstance(trans_indexs, list)
                     and col in trans_indexs) or (isinstance(trans_indexs, str)
                                                  and col == trans_indexs):
@@ -108,15 +114,15 @@
                 self.extract_subfolder_cond(cond, table_cfg['SubFolder']))
         else:
             file = self.exportCfg.make_filename(self.base_dir, table_name, col)
         df = pd.read_feather(file)
         df = self.exportCfg.handle_date_filter(df, end_date, start_date,
                                                table_cfg)
         df = self.exportCfg.handle_allignment(table_name, start_date, end_date,
-                                              codes, df, self.get_template())
+                                              codes, df, self.get_all_codes())
         df = self.exportCfg.handle_map_cond(df, table_name, cond)
         df = self.exportCfg.handle_codes(df, table_name, codes)
         if 'flag' in df.columns:
             del df['flag']
         return df
 
     def custom(self, table, clause_list, columns):
@@ -175,11 +181,11 @@
                                                 sub_folder)
         else:
             file = self.exportCfg.make_filename(self.base_dir, table_name, col)
         df = pd.read_feather(file)
         df = self.exportCfg.handle_date_filter(df, end_date, start_date,
                                                table_cfg)
         df = self.exportCfg.handle_allignment(table_name, start_date, end_date,
-                                              None, df)
+                                              None, df, self.get_all_codes())
         if 'flag' in df.columns:
             del df['flag']
         return df
```

### Comparing `Finance-JindowinData-0.0.3/jdwdata/DataAPI/file/file_factory.py` & `Finance-JindowinData-0.0.4/jdwdata/DataAPI/file/file_factory.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/DataAPI/mg/fetch_engine.py` & `Finance-JindowinData-0.0.4/jdwdata/DataAPI/mg/fetch_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/DataAPI/mg/kn/kn_engine.py` & `Finance-JindowinData-0.0.4/jdwdata/DataAPI/mg/kn/kn_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/DataAPI/mg/mg_factory.py` & `Finance-JindowinData-0.0.4/jdwdata/DataAPI/mg/mg_factory.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/DataAPI/mg/mongodb.py` & `Finance-JindowinData-0.0.4/jdwdata/DataAPI/mg/mongodb.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/RetrievalAPI/customized.py` & `Finance-JindowinData-0.0.4/jdwdata/RetrievalAPI/customized.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/RetrievalAPI/ddb_customized.py` & `Finance-JindowinData-0.0.4/jdwdata/RetrievalAPI/ddb_customized.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,27 +16,31 @@
 
     def allign_data(self,
                     data,
                     table_name,
                     begin_date=None,
                     end_date=None,
                     codes=None):
-        data = self._engine.allign_data(data=data,
+        if codes is None:
+            data = self._engine.allign_data(data=data,
                                         table_name=table_name,
                                         begin_date=begin_date,
                                         end_date=end_date,
-                                        codes=codes)
+                                        codes=None)
         return data
 
     def add_def_cols(self, columns, table_name):
         transepose_indexs, transepose_cols = self._export_cfg.get_transpose_conf(
             table_name)
-        columns = columns + transepose_indexs + transepose_cols
-        columns = list(set(columns))
-        return columns
+        columns = transepose_indexs + transepose_cols + columns
+        cols = []
+        for col in columns:
+            if col not in cols:
+                cols.append(col)
+        return cols
 
     def sequence(self,
                  table_name,
                  columns,
                  begin_date,
                  end_date,
                  format_data=0,
```

### Comparing `Finance-JindowinData-0.0.3/jdwdata/RetrievalAPI/file_customized.py` & `Finance-JindowinData-0.0.4/jdwdata/RetrievalAPI/file_customized.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/__init__.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/dummy.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/dummy.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/futures/basic.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/futures/basic.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/futures/classify.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/futures/classify.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/futures/index_market.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/futures/index_market.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/futures/yields.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/futures/yields.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/index_component.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/index_component.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/index_market.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/index_market.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/stock/industry.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/stock/industry.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/stock/market_stock.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/stock/market_stock.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/stock/risk_model.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/stock/risk_model.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/stock/yields.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/stock/yields.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/universe.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/universe.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/utilities.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/utilities.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/SurfaceAPI/yields.py` & `Finance-JindowinData-0.0.4/jdwdata/SurfaceAPI/yields.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/__init__.py` & `Finance-JindowinData-0.0.4/jdwdata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 import warnings
 from .env import checkout_config
 
 try:
     import jdwdata.DataAPI.mg as MGAPI
 except ImportError:
```

### Comparing `Finance-JindowinData-0.0.3/jdwdata/config/export_cfg.py` & `Finance-JindowinData-0.0.4/jdwdata/config/export_cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
     def handle_allignment(self,
                           table,
                           start_date,
                           end_date,
                           codes,
                           data,
-                          template_df=None):
+                          all_codes=None):
         tranpose_index, trans_cols = self.get_transpose_conf(table)
         if tranpose_index is not None and len(tranpose_index) > 0 and len(
                 data) > 0:
             if tranpose_index[0] in data.columns:
                 data.set_index(tranpose_index, inplace=True)
             if len(tranpose_index) == 1 and (
                     'date' in tranpose_index[0].lower()
@@ -146,22 +146,20 @@
                     data = data.reindex(index=trade_dates,
                                         columns=data.columns)
                 elif start_date is not None:
                     trade_dates = bizDatesList(
                         'china.sse', start_date,
                         dt.datetime.now().strftime('%Y-%m-%d'))
                     data = data.reindex(index=trade_dates, columns=codes)
-            if len(trans_cols) == 1 and trans_cols[0] == 'code':
-                if codes is None and template_df is not None:
-                    all_codes = list(template_df.columns)
-                    all_codes.remove('index')
+            if len(trans_cols) == 1 and trans_cols[0] == 'code' and 'code' not in data.columns:
+                if codes is None and all_codes is not None:
                     data = data.reindex(index=data.index, columns=all_codes)
                 else:
                     data = data.reindex(index=data.index, columns=codes)
-            elif len(trans_cols) == 1 and trans_cols[0] == 'indexCode':
+            elif len(trans_cols) == 1 and trans_cols[0] == 'indexCode' and 'indexCode' not in data.columns:
                 if codes is None:
                     data = data.reindex(index=data.index,
                                         columns=self.index_codes)
                 else:
                     data = data.reindex(index=data.index, columns=codes)
         return data
```

### Comparing `Finance-JindowinData-0.0.3/jdwdata/config/mapping_cfg.py` & `Finance-JindowinData-0.0.4/jdwdata/config/mapping_cfg.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/env.py` & `Finance-JindowinData-0.0.4/jdwdata/env.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/jdwdata/kdutils/logger.py` & `Finance-JindowinData-0.0.4/jdwdata/kdutils/logger.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinData-0.0.3/setup.py` & `Finance-JindowinData-0.0.4/setup.py`

 * *Files identical despite different names*


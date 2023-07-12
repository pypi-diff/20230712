# Comparing `tmp/singlestoredb-0.7.1.tar.gz` & `tmp/singlestoredb-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singlestoredb-0.7.1.tar", last modified: Thu Jun 15 18:35:43 2023, max compression
+gzip compressed data, was "singlestoredb-0.8.0.tar", last modified: Wed Jul 12 15:59:59 2023, max compression
```

## Comparing `singlestoredb-0.7.1.tar` & `singlestoredb-0.8.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.492792 singlestoredb-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11341 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-06-15 18:35:43.492792 singlestoredb-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-06-15 18:35:43.492792 singlestoredb-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.484792 singlestoredb-0.7.1/singlestoredb/
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7599 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     6314 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    43470 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)    12515 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.484792 singlestoredb-0.7.1/singlestoredb/http/
--rw-r--r--   0 runner    (1001) docker     (122)      912 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29448 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/http/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.484792 singlestoredb-0.7.1/singlestoredb/management/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14097 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/management/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     6501 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/management/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/management/region.py
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/management/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    18491 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/management/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.484792 singlestoredb-0.7.1/singlestoredb/mysql/
--rw-r--r--   0 runner    (1001) docker     (122)     4363 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)    57359 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/accel.c
--rw-r--r--   0 runner    (1001) docker     (122)    10324 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/charset.py
--rw-r--r--   0 runner    (1001) docker     (122)    58930 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.488792 singlestoredb-0.7.1/singlestoredb/mysql/constants/
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/CLIENT.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/COMMAND.py
--rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/CR.py
--rw-r--r--   0 runner    (1001) docker     (122)    12311 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/ER.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/FIELD_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/FLAG.py
--rw-r--r--   0 runner    (1001) docker     (122)      348 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/SERVER_STATUS.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)    21092 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/cursors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/err.py
--rw-r--r--   0 runner    (1001) docker     (122)      589 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/optionfile.py
--rw-r--r--   0 runner    (1001) docker     (122)    12081 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.488792 singlestoredb-0.7.1/singlestoredb/mysql/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_DictCursor.py
--rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_SSCursor.py
--rw-r--r--   0 runner    (1001) docker     (122)    15465 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (122)    32297 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_err.py
--rw-r--r--   0 runner    (1001) docker     (122)    18965 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (122)     2502 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_load_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_nextset.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/test_optionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.488792 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.488792 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (122)    31414 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     8022 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2819 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
--rw-r--r--   0 runner    (1001) docker     (122)      435 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/mysql/times.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.492792 singlestoredb-0.7.1/singlestoredb/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/empty.sql
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/local_infile.csv
--rw-r--r--   0 runner    (1001) docker     (122)     8968 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test.sql
--rwxr-xr-x   0 runner    (1001) docker     (122)    40220 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_basics.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11184 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    50732 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_dbapi.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1131 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     8580 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_http.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     9721 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_management.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6582 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_results.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4500 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_types.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10408 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/test_xdict.py
--rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9969 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.492792 singlestoredb-0.7.1/singlestoredb/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24503 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/utils/convert_rows.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/utils/results.py
--rw-r--r--   0 runner    (1001) docker     (122)    12896 2023-06-15 18:35:18.000000 singlestoredb-0.7.1/singlestoredb/utils/xdict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 18:35:43.484792 singlestoredb-0.7.1/singlestoredb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7340 2023-06-15 18:35:43.000000 singlestoredb-0.7.1/singlestoredb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-06-15 18:35:43.000000 singlestoredb-0.7.1/singlestoredb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 18:35:43.000000 singlestoredb-0.7.1/singlestoredb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-15 18:35:43.000000 singlestoredb-0.7.1/singlestoredb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-15 18:35:43.000000 singlestoredb-0.7.1/singlestoredb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:59.957802 singlestoredb-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11341 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-07-12 15:59:59.957802 singlestoredb-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6299 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-07-12 15:59:59.957802 singlestoredb-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:59.937801 singlestoredb-0.8.0/singlestoredb/
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7599 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6314 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43473 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12515 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:59.937801 singlestoredb-0.8.0/singlestoredb/http/
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31143 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/http/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:59.941801 singlestoredb-0.8.0/singlestoredb/management/
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14097 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/management/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6501 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/management/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/management/region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/management/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18491 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/management/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:59.945801 singlestoredb-0.8.0/singlestoredb/mysql/
+-rw-r--r--   0 runner    (1001) docker     (122)     4363 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57359 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/accel.c
+-rw-r--r--   0 runner    (1001) docker     (122)    10324 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/charset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58930 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:59.945801 singlestoredb-0.8.0/singlestoredb/mysql/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/constants/CLIENT.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/constants/COMMAND.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/constants/CR.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12311 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/constants/ER.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/constants/FIELD_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/constants/FLAG.py
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/constants/SERVER_STATUS.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5630 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21092 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/err.py
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/optionfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12081 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:59.949801 singlestoredb-0.8.0/singlestoredb/mysql/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/test_DictCursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/test_SSCursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15465 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32297 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2002 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/test_err.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18965 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2502 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/test_load_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2725 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/test_nextset.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/test_optionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:59.949801 singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:59.949801 singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10171 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31414 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8022 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2819 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/mysql/times.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:59.953801 singlestoredb-0.8.0/singlestoredb/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/empty.sql
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/local_infile.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     9030 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/test.sql
+-rwxr-xr-x   0 runner    (1001) docker     (122)    42272 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/test_basics.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11184 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    50732 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/test_dbapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1131 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8580 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/test_http.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     9721 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/test_management.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6582 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/test_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4500 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/test_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10408 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/test_xdict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4673 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9969 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:59.957802 singlestoredb-0.8.0/singlestoredb/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24503 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/utils/convert_rows.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/utils/results.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12896 2023-07-12 15:59:19.000000 singlestoredb-0.8.0/singlestoredb/utils/xdict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:59:59.937801 singlestoredb-0.8.0/singlestoredb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-07-12 15:59:59.000000 singlestoredb-0.8.0/singlestoredb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3095 2023-07-12 15:59:59.000000 singlestoredb-0.8.0/singlestoredb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 15:59:59.000000 singlestoredb-0.8.0/singlestoredb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-12 15:59:59.000000 singlestoredb-0.8.0/singlestoredb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-07-12 15:59:59.000000 singlestoredb-0.8.0/singlestoredb.egg-info/top_level.txt
```

### Comparing `singlestoredb-0.7.1/LICENSE` & `singlestoredb-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/PKG-INFO` & `singlestoredb-0.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 0.7.1
+Version: 0.8.0
 Summary: Interface to the SingleStore database and cluster management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Database
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dataframe
 Provides-Extra: dbt
 Provides-Extra: ed22519
 Provides-Extra: gssapi
 Provides-Extra: ibis
 Provides-Extra: kerberos
```

### Comparing `singlestoredb-0.7.1/README.md` & `singlestoredb-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/setup.cfg` & `singlestoredb-0.8.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 [metadata]
 name = singlestoredb
-version = 0.7.1
+version = 0.8.0
 description = Interface to the SingleStore database and cluster management APIs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/singlestore-labs/singlestoredb-python
 author = SingleStore
 author_email = support@singlestore.com
 license = Apache-2.0
-license_file = LICENSE
 license_files = LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
 	Topic :: Database
 
 [options]
 packages = find:
 install_requires = 
 	PyJWT
 	build
 	requests
 	sqlparams
 	wheel
-python_requires = >=3.6
+python_requires = >=3.8
 tests_require = 
 	coverage
 	pytest
 	pandas
 
 [options.packages.find]
 exclude =
```

### Comparing `singlestoredb-0.7.1/setup.py` & `singlestoredb-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/__init__.py` & `singlestoredb-0.8.0/singlestoredb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 >>> cur = conn.cursor()
 >>> cur.execute('select * from customers')
 >>> for row in cur:
 ...     print(row)
 
 """
 
-__version__ = '0.7.1'
+__version__ = '0.8.0'
 
 from .config import options, get_option, set_option, describe_option
 from .connection import connect, apilevel, threadsafety, paramstyle
 from .exceptions import (
     Warning, Error, InterfaceError, DatabaseError, OperationalError,
     IntegrityError, InternalError, ProgrammingError, NotSupportedError,
     DataError, ManagementError,
```

### Comparing `singlestoredb-0.7.1/singlestoredb/auth.py` & `singlestoredb-0.8.0/singlestoredb/auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/config.py` & `singlestoredb-0.8.0/singlestoredb/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/connection.py` & `singlestoredb-0.8.0/singlestoredb/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1024,15 +1024,15 @@
     OperationalError = exceptions.OperationalError
     IntegrityError = exceptions.IntegrityError
     InternalError = exceptions.InternalError
     ProgrammingError = exceptions.ProgrammingError
     NotSupportedError = exceptions.NotSupportedError
 
     #: Read-only DB-API parameter style
-    paramstyle = 'named'
+    paramstyle = 'pyformat'
 
     # Must be set by subclass
     driver = ''
 
     # Populated when first needed
     _map_param_converter: Optional[sqlparams.SQLParams] = None
     _positional_param_converter: Optional[sqlparams.SQLParams] = None
```

### Comparing `singlestoredb-0.7.1/singlestoredb/converters.py` & `singlestoredb-0.8.0/singlestoredb/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/exceptions.py` & `singlestoredb-0.8.0/singlestoredb/exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/http/__init__.py` & `singlestoredb-0.8.0/singlestoredb/http/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/http/connection.py` & `singlestoredb-0.8.0/singlestoredb/http/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 #!/usr/bin/env python
 """SingleStoreDB HTTP API interface."""
+import datetime
+import decimal
 import functools
 import json
 import re
+import time
 from base64 import b64decode
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
@@ -159,46 +162,96 @@
     if x is None:
         return None
     if converter is None:
         return b64decode(x)
     return converter(b64decode(x))
 
 
-shapely_Point = None
-shapely_Polygon = None
-shapely_LineString = None
-np_ndarray = None
-pygeos_Geometry = None
+def encode_timedelta(obj: datetime.timedelta) -> str:
+    """Encode timedelta as str."""
+    seconds = int(obj.seconds) % 60
+    minutes = int(obj.seconds // 60) % 60
+    hours = int(obj.seconds // 3600) % 24 + int(obj.days) * 24
+    if obj.microseconds:
+        fmt = '{0:02d}:{1:02d}:{2:02d}.{3:06d}'
+    else:
+        fmt = '{0:02d}:{1:02d}:{2:02d}'
+    return fmt.format(hours, minutes, seconds, obj.microseconds)
+
+
+def encode_time(obj: datetime.time) -> str:
+    """Encode time as str."""
+    if obj.microsecond:
+        fmt = '{0.hour:02}:{0.minute:02}:{0.second:02}.{0.microsecond:06}'
+    else:
+        fmt = '{0.hour:02}:{0.minute:02}:{0.second:02}'
+    return fmt.format(obj)
+
+
+def encode_datetime(obj: datetime.datetime) -> str:
+    """Encode datetime as str."""
+    if obj.microsecond:
+        fmt = '{0.year:04}-{0.month:02}-{0.day:02} ' \
+              '{0.hour:02}:{0.minute:02}:{0.second:02}.{0.microsecond:06}'
+    else:
+        fmt = '{0.year:04}-{0.month:02}-{0.day:02} ' \
+              '{0.hour:02}:{0.minute:02}:{0.second:02}'
+    return fmt.format(obj)
+
+
+def encode_date(obj: datetime.date) -> str:
+    """Encode date as str."""
+    fmt = '{0.year:04}-{0.month:02}-{0.day:02}'
+    return fmt.format(obj)
+
+
+def encode_struct_time(obj: time.struct_time) -> str:
+    """Encode time struct to str."""
+    return encode_datetime(datetime.datetime(*obj[:6]))
+
+
+def encode_decimal(o: decimal.Decimal) -> str:
+    """Encode decimal to str."""
+    return format(o, 'f')
+
+
+# Most argument encoding is done by the JSON encoder, but these
+# are exceptions to the rule.
+encoders = {
+    datetime.datetime: encode_datetime,
+    datetime.date: encode_date,
+    datetime.time: encode_time,
+    datetime.timedelta: encode_timedelta,
+    time.struct_time: encode_struct_time,
+    decimal.Decimal: encode_decimal,
+}
 
 
 if has_shapely:
-    shapely_Point = shapely.geometry.Point
-    shapely_Polygon = shapely.geometry.Polygon
-    shapely_LineString = shapely.geometry.LineString
+    encoders[shapely.geometry.Point] = shapely.wkt.dumps
+    encoders[shapely.geometry.Polygon] = shapely.wkt.dumps
+    encoders[shapely.geometry.LineString] = shapely.wkt.dumps
 
 if has_numpy:
-    np_ndarray = np.ndarray
+
+    def encode_ndarray(obj: np.ndarray) -> bytes:  # type: ignore
+        """Encode an ndarray as bytes."""
+        return obj.tobytes()
+
+    encoders[np.ndarray] = encode_ndarray
 
 if has_pygeos:
-    pygeos_Geometry = pygeos.Geometry
+    encoders[pygeos.Geometry] = pygeos.io.to_wkt
 
 
 def convert_special_type(arg: Any) -> Any:
     """Convert special data type objects."""
-    dtype = type(arg)
-    if dtype is np_ndarray:
-        return arg.tobytes()
-    if dtype is shapely_Point:
-        return shapely.wkt.dumps(arg)
-    if dtype is shapely_Polygon:
-        return shapely.wkt.dumps(arg)
-    if dtype is shapely_LineString:
-        return shapely.wkt.dumps(arg)
-    if dtype is pygeos_Geometry:
-        return pygeos.io.to_wkt(arg)
+    func = encoders.get(type(arg), None)
+    if func is not None:
+        return func(arg)  # type: ignore
     return arg
 
 
 def convert_special_params(
     params: Optional[Union[Sequence[Any], Dict[str, Any]]] = None,
 ) -> Optional[Union[Sequence[Any], Dict[str, Any]]]:
     """Convert parameters of special data types."""
```

### Comparing `singlestoredb-0.7.1/singlestoredb/management/cluster.py` & `singlestoredb-0.8.0/singlestoredb/management/cluster.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/management/manager.py` & `singlestoredb-0.8.0/singlestoredb/management/manager.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/management/region.py` & `singlestoredb-0.8.0/singlestoredb/management/region.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/management/utils.py` & `singlestoredb-0.8.0/singlestoredb/management/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/management/workspace.py` & `singlestoredb-0.8.0/singlestoredb/management/workspace.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/__init__.py` & `singlestoredb-0.8.0/singlestoredb/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/_auth.py` & `singlestoredb-0.8.0/singlestoredb/mysql/_auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/accel.c` & `singlestoredb-0.8.0/singlestoredb/mysql/accel.c`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/charset.py` & `singlestoredb-0.8.0/singlestoredb/mysql/charset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/connection.py` & `singlestoredb-0.8.0/singlestoredb/mysql/connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/constants/CLIENT.py` & `singlestoredb-0.8.0/singlestoredb/mysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/constants/COMMAND.py` & `singlestoredb-0.8.0/singlestoredb/mysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/constants/CR.py` & `singlestoredb-0.8.0/singlestoredb/mysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/constants/ER.py` & `singlestoredb-0.8.0/singlestoredb/mysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/converters.py` & `singlestoredb-0.8.0/singlestoredb/mysql/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/cursors.py` & `singlestoredb-0.8.0/singlestoredb/mysql/cursors.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/err.py` & `singlestoredb-0.8.0/singlestoredb/mysql/err.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/optionfile.py` & `singlestoredb-0.8.0/singlestoredb/mysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/protocol.py` & `singlestoredb-0.8.0/singlestoredb/mysql/protocol.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/__init__.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/base.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/base.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/conftest.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_DictCursor.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/test_DictCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_SSCursor.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/test_SSCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_basic.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_connection.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_converters.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_cursor.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_issues.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_load_local.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/test_load_local.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_nextset.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/test_nextset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/test_optionfile.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/test_optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py` & `singlestoredb-0.8.0/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/tests/test.sql` & `singlestoredb-0.8.0/singlestoredb/tests/test.sql`

 * *Files 1% similar despite different names*

```diff
@@ -352,13 +352,17 @@
 -- Table of extended data types
 --
 CREATE ROWSTORE TABLE IF NOT EXISTS `extended_types` (
     `id` INT(11),
     `geography` GEOGRAPHY,
     `geographypoint` GEOGRAPHYPOINT,
     `vectors` BLOB,
+    `dt` DATETIME,
+    `d` DATE,
+    `t` TIME,
+    `td` TIME,
     `testkey` LONGTEXT
 )
 COLLATE='utf8_unicode_ci';
 
 
 COMMIT;
```

### Comparing `singlestoredb-0.7.1/singlestoredb/tests/test_basics.py` & `singlestoredb-0.8.0/singlestoredb/tests/test_basics.py`

 * *Files 7% similar despite different names*

```diff
@@ -505,22 +505,44 @@
 
         import uuid
 
         key = str(uuid.uuid4())
 
         # shapely data
         data = [
-            (1, 'POLYGON((1 1, 2 1, 2 2, 1 2, 1 1))', 'POINT(1.5 1.5)', [0.5, 0.6], key),
-            (2, 'POLYGON((5 1, 6 1, 6 2, 5 2, 5 1))', 'POINT(5.5 1.5)', [1.3, 2.5], key),
             (
-                3, 'POLYGON((5 5, 6 5, 6 6, 5 6, 5 5))',
-                'POINT(5.5 5.5)', [10.3, 11.1], key,
+                1, 'POLYGON((1 1, 2 1, 2 2, 1 2, 1 1))', 'POINT(1.5 1.5)',
+                [0.5, 0.6], datetime.datetime(1950, 1, 2, 12, 13, 14),
+                datetime.date(1950, 1, 2), datetime.time(12, 13, 14),
+                datetime.timedelta(seconds=123456), key,
+            ),
+            (
+                2, 'POLYGON((5 1, 6 1, 6 2, 5 2, 5 1))', 'POINT(5.5 1.5)',
+                [1.3, 2.5], datetime.datetime(1960, 3, 4, 15, 16, 17),
+                datetime.date(1960, 3, 4), datetime.time(15, 16, 17),
+                datetime.timedelta(seconds=2), key,
+            ),
+            (
+                3, 'POLYGON((5 5, 6 5, 6 6, 5 6, 5 5))', 'POINT(5.5 5.5)',
+                [10.3, 11.1], datetime.datetime(1970, 6, 7, 18, 19, 20),
+                datetime.date(1970, 5, 6), datetime.time(18, 19, 20),
+                datetime.timedelta(seconds=-2), key,
+            ),
+            (
+                4, 'POLYGON((1 5, 2 5, 2 6, 1 6, 1 5))', 'POINT(1.5 5.5)',
+                [3.3, 3.4], datetime.datetime(1980, 8, 9, 21, 22, 23),
+                datetime.date(1980, 7, 8), datetime.time(21, 22, 23),
+                datetime.timedelta(seconds=-123456), key,
+            ),
+            (
+                5, 'POLYGON((3 3, 4 3, 4 4, 3 4, 3 3))', 'POINT(3.5 3.5)',
+                [2.9, 9.5], datetime.datetime(2010, 10, 11, 1, 2, 3),
+                datetime.date(2010, 8, 9), datetime.time(1, 2, 3),
+                datetime.timedelta(seconds=0), key,
             ),
-            (4, 'POLYGON((1 5, 2 5, 2 6, 1 6, 1 5))', 'POINT(1.5 5.5)', [3.3, 3.4], key),
-            (5, 'POLYGON((3 3, 4 3, 4 4, 3 4, 3 3))', 'POINT(3.5 3.5)', [2.9, 9.5], key),
         ]
 
         new_data = []
         for i, row in enumerate(data):
             row = list(row)
             row[1] = shapely.wkt.loads(row[1])
             row[2] = shapely.wkt.loads(row[2])
@@ -528,16 +550,16 @@
                 row[3] = ''
             else:
                 row[3] = np.array(row[3], dtype='<f4')
             new_data.append(row)
 
         self.cur.executemany(
             'INSERT INTO extended_types '
-            '(id, geography, geographypoint, vectors, testkey) '
-            'VALUES (%s, %s, %s, %s, %s)', new_data,
+            '(id, geography, geographypoint, vectors, dt, d, t, td, testkey) '
+            'VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s)', new_data,
         )
 
         self.cur.execute(
             'SELECT * FROM extended_types WHERE testkey = %s ORDER BY id', [key],
         )
 
         for data_row, row in zip(new_data, self.cur):
@@ -547,22 +569,44 @@
             if 'http' in self.conn.driver:
                 assert row[3] == b''
             else:
                 assert (data_row[3] == np.frombuffer(row[3], dtype='<f4')).all()
 
         # pygeos data
         data = [
-            (6, 'POLYGON((1 1, 2 1, 2 2, 1 2, 1 1))', 'POINT(1.5 1.5)', [0.5, 0.6], key),
-            (7, 'POLYGON((5 1, 6 1, 6 2, 5 2, 5 1))', 'POINT(5.5 1.5)', [1.3, 2.5], key),
             (
-                8, 'POLYGON((5 5, 6 5, 6 6, 5 6, 5 5))',
-                'POINT(5.5 5.5)', [10.3, 11.1], key,
+                6, 'POLYGON((1 1, 2 1, 2 2, 1 2, 1 1))', 'POINT(1.5 1.5)',
+                [0.5, 0.6], datetime.datetime(1950, 1, 2, 12, 13, 14),
+                datetime.date(1950, 1, 2), datetime.time(12, 13, 14),
+                datetime.timedelta(seconds=123456), key,
+            ),
+            (
+                7, 'POLYGON((5 1, 6 1, 6 2, 5 2, 5 1))', 'POINT(5.5 1.5)',
+                [1.3, 2.5], datetime.datetime(1960, 3, 4, 15, 16, 17),
+                datetime.date(1960, 3, 4), datetime.time(15, 16, 17),
+                datetime.timedelta(seconds=2), key,
+            ),
+            (
+                8, 'POLYGON((5 5, 6 5, 6 6, 5 6, 5 5))', 'POINT(5.5 5.5)',
+                [10.3, 11.1], datetime.datetime(1970, 6, 7, 18, 19, 20),
+                datetime.date(1970, 5, 6), datetime.time(18, 19, 20),
+                datetime.timedelta(seconds=-2), key,
+            ),
+            (
+                9, 'POLYGON((1 5, 2 5, 2 6, 1 6, 1 5))', 'POINT(1.5 5.5)',
+                [3.3, 3.4], datetime.datetime(1980, 8, 9, 21, 22, 23),
+                datetime.date(1980, 7, 8), datetime.time(21, 22, 23),
+                datetime.timedelta(seconds=-123456), key,
+            ),
+            (
+                10, 'POLYGON((3 3, 4 3, 4 4, 3 4, 3 3))', 'POINT(3.5 3.5)',
+                [2.9, 9.5], datetime.datetime(2010, 10, 11, 1, 2, 3),
+                datetime.date(2010, 8, 9), datetime.time(1, 2, 3),
+                datetime.timedelta(seconds=0), key,
             ),
-            (9, 'POLYGON((1 5, 2 5, 2 6, 1 6, 1 5))', 'POINT(1.5 5.5)', [3.3, 3.4], key),
-            (10, 'POLYGON((3 3, 4 3, 4 4, 3 4, 3 3))', 'POINT(3.5 3.5)', [2.9, 9.5], key),
         ]
 
         new_data = []
         for i, row in enumerate(data):
             row = list(row)
             row[1] = pygeos.io.from_wkt(row[1])
             row[2] = pygeos.io.from_wkt(row[2])
@@ -570,16 +614,16 @@
                 row[3] = ''
             else:
                 row[3] = np.array(row[3], dtype='<f4')
             new_data.append(row)
 
         self.cur.executemany(
             'INSERT INTO extended_types '
-            '(id, geography, geographypoint, vectors, testkey) '
-            'VALUES (%s, %s, %s, %s, %s)', new_data,
+            '(id, geography, geographypoint, vectors, dt, d, t, td, testkey) '
+            'VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s)', new_data,
         )
 
         self.cur.execute(
             'SELECT * FROM extended_types WHERE id >= 6 and testkey = %s ORDER BY id', [
                 key,
             ],
         )
```

### Comparing `singlestoredb-0.7.1/singlestoredb/tests/test_config.py` & `singlestoredb-0.8.0/singlestoredb/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/tests/test_connection.py` & `singlestoredb-0.8.0/singlestoredb/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/tests/test_dbapi.py` & `singlestoredb-0.8.0/singlestoredb/tests/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/tests/test_exceptions.py` & `singlestoredb-0.8.0/singlestoredb/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/tests/test_http.py` & `singlestoredb-0.8.0/singlestoredb/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/tests/test_management.py` & `singlestoredb-0.8.0/singlestoredb/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/tests/test_results.py` & `singlestoredb-0.8.0/singlestoredb/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/tests/test_types.py` & `singlestoredb-0.8.0/singlestoredb/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/tests/test_xdict.py` & `singlestoredb-0.8.0/singlestoredb/tests/test_xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/tests/utils.py` & `singlestoredb-0.8.0/singlestoredb/tests/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/types.py` & `singlestoredb-0.8.0/singlestoredb/types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/utils/config.py` & `singlestoredb-0.8.0/singlestoredb/utils/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/utils/convert_rows.py` & `singlestoredb-0.8.0/singlestoredb/utils/convert_rows.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/utils/results.py` & `singlestoredb-0.8.0/singlestoredb/utils/results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb/utils/xdict.py` & `singlestoredb-0.8.0/singlestoredb/utils/xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-0.7.1/singlestoredb.egg-info/PKG-INFO` & `singlestoredb-0.8.0/singlestoredb.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 0.7.1
+Version: 0.8.0
 Summary: Interface to the SingleStore database and cluster management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Database
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dataframe
 Provides-Extra: dbt
 Provides-Extra: ed22519
 Provides-Extra: gssapi
 Provides-Extra: ibis
 Provides-Extra: kerberos
```

### Comparing `singlestoredb-0.7.1/singlestoredb.egg-info/SOURCES.txt` & `singlestoredb-0.8.0/singlestoredb.egg-info/SOURCES.txt`

 * *Files identical despite different names*


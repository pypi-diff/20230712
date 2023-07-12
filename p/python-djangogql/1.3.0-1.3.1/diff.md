# Comparing `tmp/python-djangogql-1.3.0.tar.gz` & `tmp/python-djangogql-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-djangogql-1.3.0.tar", last modified: Tue Jul 11 18:09:52 2023, max compression
+gzip compressed data, was "python-djangogql-1.3.1.tar", last modified: Wed Jul 12 00:05:09 2023, max compression
```

## Comparing `python-djangogql-1.3.0.tar` & `python-djangogql-1.3.1.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.037632 python-djangogql-1.3.0/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1086 2023-07-09 22:53:34.000000 python-djangogql-1.3.0/LICENSE
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       74 2023-07-08 20:27:42.000000 python-djangogql-1.3.0/MANIFEST.in
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-11 18:09:52.037632 python-djangogql-1.3.0/PKG-INFO
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      319 2023-07-09 21:56:06.000000 python-djangogql-1.3.0/README.md
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.029632 python-djangogql-1.3.0/djangogql/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 01:33:53.000000 python-djangogql-1.3.0/djangogql/__init__.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.029632 python-djangogql-1.3.0/djangogql/account/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 21:39:57.000000 python-djangogql-1.3.0/djangogql/account/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1740 2023-07-09 21:42:29.000000 python-djangogql-1.3.0/djangogql/account/mixins.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1833 2023-07-09 15:12:17.000000 python-djangogql-1.3.0/djangogql/auth_backend.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1435 2023-07-10 00:14:32.000000 python-djangogql-1.3.0/djangogql/context.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.033632 python-djangogql-1.3.0/djangogql/core/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      162 2023-07-10 00:14:38.000000 python-djangogql-1.3.0/djangogql/core/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    15901 2023-07-10 00:13:32.000000 python-djangogql-1.3.0/djangogql/core/connection.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      511 2023-07-10 00:14:08.000000 python-djangogql-1.3.0/djangogql/core/context.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1467 2023-07-08 20:10:57.000000 python-djangogql-1.3.0/djangogql/core/dataloaders.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1062 2023-07-10 17:27:11.000000 python-djangogql-1.3.0/djangogql/core/enums.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3642 2023-07-10 17:27:09.000000 python-djangogql-1.3.0/djangogql/core/fields.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5010 2023-07-10 17:27:06.000000 python-djangogql-1.3.0/djangogql/core/filters.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    17475 2023-07-10 17:26:55.000000 python-djangogql-1.3.0/djangogql/core/mutations.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.033632 python-djangogql-1.3.0/djangogql/core/types/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      119 2023-07-07 20:06:42.000000 python-djangogql-1.3.0/djangogql/core/types/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      864 2023-04-29 23:33:17.000000 python-djangogql-1.3.0/djangogql/core/types/base.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2384 2023-07-07 20:06:42.000000 python-djangogql-1.3.0/djangogql/core/types/common.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1801 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/djangogql/core/types/filter_converter.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3663 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/djangogql/core/types/filter_input.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3857 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/djangogql/core/types/model.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7466 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/djangogql/core/types/model_converter.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1193 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/djangogql/core/types/registry.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      970 2023-05-04 18:55:33.000000 python-djangogql-1.3.0/djangogql/core/types/sort_input.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      587 2023-07-07 20:06:42.000000 python-djangogql-1.3.0/djangogql/core/types/upload.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      826 2023-03-05 02:44:45.000000 python-djangogql-1.3.0/djangogql/core/validators.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.033632 python-djangogql-1.3.0/djangogql/db/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 18:13:19.000000 python-djangogql-1.3.0/djangogql/db/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      377 2023-07-08 18:13:32.000000 python-djangogql-1.3.0/djangogql/db/utils.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1746 2023-07-08 20:10:02.000000 python-djangogql-1.3.0/djangogql/decorators.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      424 2023-07-08 15:32:48.000000 python-djangogql-1.3.0/djangogql/exceptions.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5320 2023-07-09 15:01:48.000000 python-djangogql-1.3.0/djangogql/jwt.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1943 2023-07-09 15:25:27.000000 python-djangogql-1.3.0/djangogql/middleware.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3630 2023-07-09 18:06:00.000000 python-djangogql-1.3.0/djangogql/permissions.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3010 2023-07-09 18:05:20.000000 python-djangogql-1.3.0/djangogql/settings.py
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.029632 python-djangogql-1.3.0/djangogql/templates/
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.033632 python-djangogql-1.3.0/djangogql/templates/graphql/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2012 2023-07-08 20:26:43.000000 python-djangogql-1.3.0/djangogql/templates/graphql/playground.html
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.033632 python-djangogql-1.3.0/djangogql/utils/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7716 2023-07-10 17:27:24.000000 python-djangogql-1.3.0/djangogql/utils/__init__.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1227 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/djangogql/utils/fields.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2140 2023-07-07 20:06:42.000000 python-djangogql-1.3.0/djangogql/utils/files.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      978 2023-03-17 18:04:54.000000 python-djangogql-1.3.0/djangogql/utils/filters.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3632 2023-07-11 00:24:22.000000 python-djangogql-1.3.0/djangogql/utils/sorting.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    10231 2023-07-09 15:40:58.000000 python-djangogql-1.3.0/djangogql/views.py
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       88 2023-07-09 16:38:33.000000 python-djangogql-1.3.0/pyproject.toml
-drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-11 18:09:52.037632 python-djangogql-1.3.0/python_djangogql.egg-info/
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-11 18:09:52.000000 python-djangogql-1.3.0/python_djangogql.egg-info/PKG-INFO
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1381 2023-07-11 18:09:52.000000 python-djangogql-1.3.0/python_djangogql.egg-info/SOURCES.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-11 18:09:52.000000 python-djangogql-1.3.0/python_djangogql.egg-info/dependency_links.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-09 23:00:28.000000 python-djangogql-1.3.0/python_djangogql.egg-info/not-zip-safe
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      164 2023-07-11 18:09:52.000000 python-djangogql-1.3.0/python_djangogql.egg-info/requires.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       10 2023-07-11 18:09:52.000000 python-djangogql-1.3.0/python_djangogql.egg-info/top_level.txt
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       38 2023-07-11 18:09:52.037632 python-djangogql-1.3.0/setup.cfg
--rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1573 2023-07-11 18:09:37.000000 python-djangogql-1.3.0/setup.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.468482 python-djangogql-1.3.1/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1086 2023-07-09 22:53:34.000000 python-djangogql-1.3.1/LICENSE
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       74 2023-07-08 20:27:42.000000 python-djangogql-1.3.1/MANIFEST.in
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-12 00:05:09.468482 python-djangogql-1.3.1/PKG-INFO
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      319 2023-07-09 21:56:06.000000 python-djangogql-1.3.1/README.md
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.460482 python-djangogql-1.3.1/djangogql/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 01:33:53.000000 python-djangogql-1.3.1/djangogql/__init__.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.460482 python-djangogql-1.3.1/djangogql/account/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-09 21:39:57.000000 python-djangogql-1.3.1/djangogql/account/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1740 2023-07-09 21:42:29.000000 python-djangogql-1.3.1/djangogql/account/mixins.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1833 2023-07-09 15:12:17.000000 python-djangogql-1.3.1/djangogql/auth_backend.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1435 2023-07-10 00:14:32.000000 python-djangogql-1.3.1/djangogql/context.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.464482 python-djangogql-1.3.1/djangogql/core/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      162 2023-07-10 00:14:38.000000 python-djangogql-1.3.1/djangogql/core/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    15901 2023-07-10 00:13:32.000000 python-djangogql-1.3.1/djangogql/core/connection.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      511 2023-07-10 00:14:08.000000 python-djangogql-1.3.1/djangogql/core/context.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1467 2023-07-08 20:10:57.000000 python-djangogql-1.3.1/djangogql/core/dataloaders.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1062 2023-07-10 17:27:11.000000 python-djangogql-1.3.1/djangogql/core/enums.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3642 2023-07-10 17:27:09.000000 python-djangogql-1.3.1/djangogql/core/fields.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5010 2023-07-10 17:27:06.000000 python-djangogql-1.3.1/djangogql/core/filters.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    17475 2023-07-10 17:26:55.000000 python-djangogql-1.3.1/djangogql/core/mutations.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.464482 python-djangogql-1.3.1/djangogql/core/types/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      119 2023-07-07 20:06:42.000000 python-djangogql-1.3.1/djangogql/core/types/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      864 2023-04-29 23:33:17.000000 python-djangogql-1.3.1/djangogql/core/types/base.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2384 2023-07-07 20:06:42.000000 python-djangogql-1.3.1/djangogql/core/types/common.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7851 2023-07-12 00:03:45.000000 python-djangogql-1.3.1/djangogql/core/types/converter.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3641 2023-07-12 00:03:59.000000 python-djangogql-1.3.1/djangogql/core/types/filter_input.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3837 2023-07-12 00:04:17.000000 python-djangogql-1.3.1/djangogql/core/types/model.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1193 2023-07-11 18:09:37.000000 python-djangogql-1.3.1/djangogql/core/types/registry.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      970 2023-05-04 18:55:33.000000 python-djangogql-1.3.1/djangogql/core/types/sort_input.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      587 2023-07-07 20:06:42.000000 python-djangogql-1.3.1/djangogql/core/types/upload.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      826 2023-03-05 02:44:45.000000 python-djangogql-1.3.1/djangogql/core/validators.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.464482 python-djangogql-1.3.1/djangogql/db/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-08 18:13:19.000000 python-djangogql-1.3.1/djangogql/db/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      377 2023-07-08 18:13:32.000000 python-djangogql-1.3.1/djangogql/db/utils.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1746 2023-07-08 20:10:02.000000 python-djangogql-1.3.1/djangogql/decorators.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      424 2023-07-08 15:32:48.000000 python-djangogql-1.3.1/djangogql/exceptions.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     5320 2023-07-09 15:01:48.000000 python-djangogql-1.3.1/djangogql/jwt.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1943 2023-07-09 15:25:27.000000 python-djangogql-1.3.1/djangogql/middleware.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3630 2023-07-09 18:06:00.000000 python-djangogql-1.3.1/djangogql/permissions.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3010 2023-07-09 18:05:20.000000 python-djangogql-1.3.1/djangogql/settings.py
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.460482 python-djangogql-1.3.1/djangogql/templates/
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.464482 python-djangogql-1.3.1/djangogql/templates/graphql/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2012 2023-07-08 20:26:43.000000 python-djangogql-1.3.1/djangogql/templates/graphql/playground.html
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.464482 python-djangogql-1.3.1/djangogql/utils/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     7716 2023-07-10 17:27:24.000000 python-djangogql-1.3.1/djangogql/utils/__init__.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1227 2023-07-11 18:09:37.000000 python-djangogql-1.3.1/djangogql/utils/fields.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     2140 2023-07-07 20:06:42.000000 python-djangogql-1.3.1/djangogql/utils/files.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      978 2023-03-17 18:04:54.000000 python-djangogql-1.3.1/djangogql/utils/filters.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     3632 2023-07-11 00:24:22.000000 python-djangogql-1.3.1/djangogql/utils/sorting.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)    10231 2023-07-09 15:40:58.000000 python-djangogql-1.3.1/djangogql/views.py
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       88 2023-07-09 16:38:33.000000 python-djangogql-1.3.1/pyproject.toml
+drwxrwxr-x   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        0 2023-07-12 00:05:09.468482 python-djangogql-1.3.1/python_djangogql.egg-info/
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1353 2023-07-12 00:05:09.000000 python-djangogql-1.3.1/python_djangogql.egg-info/PKG-INFO
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1334 2023-07-12 00:05:09.000000 python-djangogql-1.3.1/python_djangogql.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-12 00:05:09.000000 python-djangogql-1.3.1/python_djangogql.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)        1 2023-07-09 23:00:28.000000 python-djangogql-1.3.1/python_djangogql.egg-info/not-zip-safe
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)      164 2023-07-12 00:05:09.000000 python-djangogql-1.3.1/python_djangogql.egg-info/requires.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       10 2023-07-12 00:05:09.000000 python-djangogql-1.3.1/python_djangogql.egg-info/top_level.txt
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)       38 2023-07-12 00:05:09.468482 python-djangogql-1.3.1/setup.cfg
+-rw-rw-r--   0 felipefariapessoal  (1001) felipefariapessoal  (1001)     1573 2023-07-12 00:04:34.000000 python-djangogql-1.3.1/setup.py
```

### Comparing `python-djangogql-1.3.0/LICENSE` & `python-djangogql-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/PKG-INFO` & `python-djangogql-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-djangogql
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Django app to build graphql APIs
 Home-page: https://github.com/felipevisu/djangogql
 Author: Felipe Faria
 Author-email: felipevisu@gmail.com
 License: MIT
 Keywords: api graphql graphene django
 Platform: any
```

### Comparing `python-djangogql-1.3.0/djangogql/account/mixins.py` & `python-djangogql-1.3.1/djangogql/account/mixins.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/auth_backend.py` & `python-djangogql-1.3.1/djangogql/auth_backend.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/context.py` & `python-djangogql-1.3.1/djangogql/context.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/core/connection.py` & `python-djangogql-1.3.1/djangogql/core/connection.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/core/dataloaders.py` & `python-djangogql-1.3.1/djangogql/core/dataloaders.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/core/enums.py` & `python-djangogql-1.3.1/djangogql/core/enums.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/core/fields.py` & `python-djangogql-1.3.1/djangogql/core/fields.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/core/filters.py` & `python-djangogql-1.3.1/djangogql/core/filters.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/core/mutations.py` & `python-djangogql-1.3.1/djangogql/core/mutations.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/core/types/base.py` & `python-djangogql-1.3.1/djangogql/core/types/base.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/core/types/common.py` & `python-djangogql-1.3.1/djangogql/core/types/common.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/core/types/filter_input.py` & `python-djangogql-1.3.1/djangogql/core/types/filter_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django_filters.filterset import FILTER_FOR_DBFIELD_DEFAULTS, BaseFilterSet
 from graphene import Argument, InputField, InputObjectType, String
 from graphene.types.inputobjecttype import InputObjectTypeOptions
 from graphene.types.utils import yank_fields_from_attrs
 
 from ..filters import GlobalIDFilter, GlobalIDMultipleChoiceFilter
 from .common import NonNullList
-from .filter_converter import convert_form_field
+from .converter import convert_field
 
 GLOBAL_ID_FILTERS = {
     models.AutoField: {"filter_class": GlobalIDFilter},
     models.OneToOneField: {"filter_class": GlobalIDFilter},
     models.ForeignKey: {"filter_class": GlobalIDFilter},
     models.ManyToManyField: {"filter_class": GlobalIDMultipleChoiceFilter},
     models.ManyToOneRel: {"filter_class": GlobalIDMultipleChoiceFilter},
@@ -64,17 +64,17 @@
 
         cls.filterset_class = get_filterset_class(cls.custom_filterset_class)
 
         args = {}
         for name, filter_field in cls.filterset_class.base_filters.items():
             input_class = getattr(filter_field, "input_class", None)
             if input_class:
-                field_type = convert_form_field(filter_field)
+                field_type = convert_field(filter_field)
             else:
-                field_type = convert_form_field(filter_field.field)
+                field_type = convert_field(filter_field.field)
                 field_type.description = getattr(filter_field, "help_text", "")
             kwargs = getattr(field_type, "kwargs", {})
             field_type.kwargs = kwargs
             args[name] = field_type
         return args
```

### Comparing `python-djangogql-1.3.0/djangogql/core/types/model.py` & `python-djangogql-1.3.1/djangogql/core/types/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import graphene
 from django.db.models import Model, Q
 from graphene.types.objecttype import ObjectType, ObjectTypeOptions
 from graphene.types.utils import yank_fields_from_attrs
 
 from ...utils.fields import get_model_fields
-from .model_converter import convert_django_field_with_choices
+from .converter import convert_field_with_choices
 from .registry import get_global_registry
 
 ALL_FIELDS = "__all__"
 
 
 def construct_fields(
     model, registry, only_fields, exclude_fields, convert_choices_to_enum
@@ -40,15 +40,15 @@
         if not isinstance(_convert_choices_to_enum, bool):
             # then `convert_choices_to_enum` is a list of field names to convert
             if name in _convert_choices_to_enum:
                 _convert_choices_to_enum = True
             else:
                 _convert_choices_to_enum = False
 
-        converted = convert_django_field_with_choices(
+        converted = convert_field_with_choices(
             field, registry, convert_choices_to_enum=_convert_choices_to_enum
         )
         fields[name] = converted
 
     return fields
```

### Comparing `python-djangogql-1.3.0/djangogql/core/types/model_converter.py` & `python-djangogql-1.3.1/djangogql/core/types/converter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 import re
 from collections import OrderedDict
 from functools import singledispatch, wraps
 
 import graphene
+from django import forms
+from django.core.exceptions import ImproperlyConfigured
 from django.db import models
 from django.utils.encoding import force_str
 from graphene.utils.str_converters import to_camel_case
 from graphql import GraphQLError
 from text_unidecode import unidecode
 
+from ..filters import (
+    EnumFilter,
+    GlobalIDFormField,
+    GlobalIDMultipleChoiceField,
+    ListObjectTypeFilter,
+    ObjectTypeFilter,
+)
+from .common import NonNullList
+
 
 def to_const(string):
     return re.sub(r"[\W|^]+", "_", unidecode(string)).upper()
 
 
 try:
     from graphql import assert_name
@@ -97,138 +108,147 @@
 def convert_choice_field_to_enum(field, name=None):
     if name is None:
         name = generate_enum_name(field.model._meta, field)
     choices = field.choices
     return convert_choices_to_named_enum_with_descriptions(name, choices)
 
 
-def convert_django_field_with_choices(
-    field, registry=None, convert_choices_to_enum=True
-):
+def convert_field_with_choices(field, registry=None, convert_choices_to_enum=True):
     if registry is not None:
         converted = registry.get_converted_field(field)
         if converted:
             return converted
     choices = getattr(field, "choices", None)
     if choices and convert_choices_to_enum:
         EnumCls = convert_choice_field_to_enum(field)
         required = not (field.blank or field.null)
 
         converted = EnumCls(
-            description=get_django_field_description(field), required=required
+            description=get_field_description(field), required=required
         ).mount_as(BlankValueField)
     else:
-        converted = convert_django_field(field, registry)
+        converted = convert_field(field, registry)
     if registry is not None:
         registry.register_converted_field(field, converted)
     return converted
 
 
-def get_django_field_description(field):
+def get_field_description(field):
     return str(field.help_text) if field.help_text else None
 
 
+def get_field_required(field):
+    if hasattr(field, "required"):
+        return field.required
+    if hasattr(field, "null"):
+        return not field.null
+    return False
+
+
 @singledispatch
-def convert_django_field(field, registry=None):
-    raise Exception(
-        "Don't know how to convert the Django field {} ({})".format(
-            field, field.__class__
-        )
+def convert_field(field):
+    raise ImproperlyConfigured(
+        "Don't know how to convert the Django form field %s (%s) "
+        "to Graphene type" % (field, field.__class__)
     )
 
 
-@convert_django_field.register(models.CharField)
-@convert_django_field.register(models.TextField)
-@convert_django_field.register(models.EmailField)
-@convert_django_field.register(models.SlugField)
-@convert_django_field.register(models.URLField)
-@convert_django_field.register(models.GenericIPAddressField)
-@convert_django_field.register(models.FileField)
-@convert_django_field.register(models.FilePathField)
+@convert_field.register(models.CharField)
+@convert_field.register(models.TextField)
+@convert_field.register(models.EmailField)
+@convert_field.register(models.SlugField)
+@convert_field.register(models.URLField)
+@convert_field.register(models.GenericIPAddressField)
+@convert_field.register(models.FileField)
+@convert_field.register(models.FilePathField)
+@convert_field.register(forms.CharField)
 def convert_field_to_string(field, registry=None):
     return graphene.String(
-        description=get_django_field_description(field), required=not field.null
+        description=get_field_description(field), required=get_field_required(field)
     )
 
 
-@convert_django_field.register(models.BigAutoField)
-@convert_django_field.register(models.AutoField)
-def convert_field_to_id(field, registry=None):
-    return graphene.ID(
-        description=get_django_field_description(field), required=not field.null
+@convert_field.register(models.BooleanField)
+@convert_field.register(forms.BooleanField)
+@convert_field.register(forms.NullBooleanField)
+def convert_field_to_nullboolean(field, registry=None):
+    return graphene.Boolean(description=get_field_description(field))
+
+
+@convert_field.register(models.FloatField)
+@convert_field.register(models.DurationField)
+@convert_field.register(forms.DecimalField)
+@convert_field.register(forms.FloatField)
+def convert_field_to_float(field, registry=None):
+    return graphene.Float(
+        description=field.help_text, required=get_field_required(field)
     )
 
 
-if hasattr(models, "SmallAutoField"):
+@convert_field.register(ObjectTypeFilter)
+@convert_field.register(EnumFilter)
+def convert_convert_enum(field, registry=None):
+    return field.input_class()
 
-    @convert_django_field.register(models.SmallAutoField)
-    def convert_field_small_to_id(field, registry=None):
-        return convert_field_to_id(field, registry)
 
+@convert_field.register(models.BigAutoField)
+@convert_field.register(models.AutoField)
+@convert_field.register(GlobalIDFormField)
+def convert_field_to_id(field, registry=None):
+    return graphene.ID(required=get_field_required(field))
 
-@convert_django_field.register(models.UUIDField)
-def convert_field_to_uuid(field, registry=None):
-    return graphene.UUID(
-        description=get_django_field_description(field), required=not field.null
-    )
 
+@convert_field.register(ListObjectTypeFilter)
+def convert_list_object_type(field, registry=None):
+    return NonNullList(field.input_class)
 
-@convert_django_field.register(models.PositiveIntegerField)
-@convert_django_field.register(models.PositiveSmallIntegerField)
-@convert_django_field.register(models.SmallIntegerField)
-@convert_django_field.register(models.IntegerField)
-def convert_field_to_int(field, registry=None):
-    return graphene.Int(
-        description=get_django_field_description(field), required=not field.null
-    )
+
+@convert_field.register(GlobalIDMultipleChoiceField)
+def convert_field_to_list(field):
+    return NonNullList(graphene.ID, required=get_field_required(field))
 
 
-@convert_django_field.register(models.BooleanField)
-def convert_field_to_boolean(field, registry=None):
-    return graphene.Boolean(
-        description=get_django_field_description(field), required=not field.null
+@convert_field.register(models.PositiveIntegerField)
+@convert_field.register(models.PositiveSmallIntegerField)
+@convert_field.register(models.SmallIntegerField)
+@convert_field.register(models.IntegerField)
+def convert_field_to_int(field, registry=None):
+    return graphene.Int(
+        description=get_field_description(field), required=not field.null
     )
 
 
-@convert_django_field.register(models.DecimalField)
+@convert_field.register(models.DecimalField)
 def convert_field_to_decimal(field, registry=None):
     return graphene.Decimal(
-        description=get_django_field_description(field), required=not field.null
-    )
-
-
-@convert_django_field.register(models.FloatField)
-@convert_django_field.register(models.DurationField)
-def convert_field_to_float(field, registry=None):
-    return graphene.Float(
-        description=get_django_field_description(field), required=not field.null
+        description=get_field_description(field), required=not field.null
     )
 
 
-@convert_django_field.register(models.DateTimeField)
+@convert_field.register(models.DateTimeField)
 def convert_datetime_to_string(field, registry=None):
     return graphene.DateTime(
-        description=get_django_field_description(field), required=not field.null
+        description=get_field_description(field), required=not field.null
     )
 
 
-@convert_django_field.register(models.DateField)
+@convert_field.register(models.DateField)
 def convert_date_to_string(field, registry=None):
     return graphene.Date(
-        description=get_django_field_description(field), required=not field.null
+        description=get_field_description(field), required=not field.null
     )
 
 
-@convert_django_field.register(models.TimeField)
+@convert_field.register(models.TimeField)
 def convert_time_to_string(field, registry=None):
     return graphene.Time(
-        description=get_django_field_description(field), required=not field.null
+        description=get_field_description(field), required=not field.null
     )
 
 
-@convert_django_field.register(models.ManyToManyField)
-@convert_django_field.register(models.ManyToManyRel)
-@convert_django_field.register(models.ManyToOneRel)
-@convert_django_field.register(models.ForeignKey)
-@convert_django_field.register(models.JSONField)
+@convert_field.register(models.ManyToManyField)
+@convert_field.register(models.ManyToManyRel)
+@convert_field.register(models.ManyToOneRel)
+@convert_field.register(models.ForeignKey)
+@convert_field.register(models.JSONField)
 def convert_field_to_list_or_connection(field, registry=None):
     return None
```

### Comparing `python-djangogql-1.3.0/djangogql/core/types/registry.py` & `python-djangogql-1.3.1/djangogql/core/types/registry.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/core/types/sort_input.py` & `python-djangogql-1.3.1/djangogql/core/types/sort_input.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/core/types/upload.py` & `python-djangogql-1.3.1/djangogql/core/types/upload.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/core/validators.py` & `python-djangogql-1.3.1/djangogql/core/validators.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/decorators.py` & `python-djangogql-1.3.1/djangogql/decorators.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/jwt.py` & `python-djangogql-1.3.1/djangogql/jwt.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/middleware.py` & `python-djangogql-1.3.1/djangogql/middleware.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/permissions.py` & `python-djangogql-1.3.1/djangogql/permissions.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/settings.py` & `python-djangogql-1.3.1/djangogql/settings.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/templates/graphql/playground.html` & `python-djangogql-1.3.1/djangogql/templates/graphql/playground.html`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/utils/__init__.py` & `python-djangogql-1.3.1/djangogql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/utils/fields.py` & `python-djangogql-1.3.1/djangogql/utils/fields.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/utils/files.py` & `python-djangogql-1.3.1/djangogql/utils/files.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/utils/filters.py` & `python-djangogql-1.3.1/djangogql/utils/filters.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/utils/sorting.py` & `python-djangogql-1.3.1/djangogql/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/djangogql/views.py` & `python-djangogql-1.3.1/djangogql/views.py`

 * *Files identical despite different names*

### Comparing `python-djangogql-1.3.0/python_djangogql.egg-info/PKG-INFO` & `python-djangogql-1.3.1/python_djangogql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-djangogql
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Django app to build graphql APIs
 Home-page: https://github.com/felipevisu/djangogql
 Author: Felipe Faria
 Author-email: felipevisu@gmail.com
 License: MIT
 Keywords: api graphql graphene django
 Platform: any
```

### Comparing `python-djangogql-1.3.0/python_djangogql.egg-info/SOURCES.txt` & `python-djangogql-1.3.1/python_djangogql.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,17 @@
 djangogql/core/fields.py
 djangogql/core/filters.py
 djangogql/core/mutations.py
 djangogql/core/validators.py
 djangogql/core/types/__init__.py
 djangogql/core/types/base.py
 djangogql/core/types/common.py
-djangogql/core/types/filter_converter.py
+djangogql/core/types/converter.py
 djangogql/core/types/filter_input.py
 djangogql/core/types/model.py
-djangogql/core/types/model_converter.py
 djangogql/core/types/registry.py
 djangogql/core/types/sort_input.py
 djangogql/core/types/upload.py
 djangogql/db/__init__.py
 djangogql/db/utils.py
 djangogql/templates/graphql/playground.html
 djangogql/utils/__init__.py
```

### Comparing `python-djangogql-1.3.0/setup.py` & `python-djangogql-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="python-djangogql",
-    version="1.3.0",
+    version="1.3.1",
     description="A Django app to build graphql APIs",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/felipevisu/djangogql",
     author="Felipe Faria",
     author_email="felipevisu@gmail.com",
     license="MIT",
```


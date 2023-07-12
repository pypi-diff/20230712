# Comparing `tmp/django-file-explorer-1.6.0.tar.gz` & `tmp/django-file-explorer-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-file-explorer-1.6.0.tar", last modified: Tue Jul  4 04:55:30 2023, max compression
+gzip compressed data, was "django-file-explorer-1.6.1.tar", last modified: Wed Jul 12 06:06:13 2023, max compression
```

## Comparing `django-file-explorer-1.6.0.tar` & `django-file-explorer-1.6.1.tar`

### file list

```diff
@@ -1,76 +1,81 @@
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.191729 django-file-explorer-1.6.0/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     5710 2023-07-04 04:55:30.191729 django-file-explorer-1.6.0/PKG-INFO
--rwxrwxr-x   0 sigma     (1000) sigma     (1000)     4754 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/README.md
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.187729 django-file-explorer-1.6.0/django_file_explorer.egg-info/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     5710 2023-07-04 04:55:30.000000 django-file-explorer-1.6.0/django_file_explorer.egg-info/PKG-INFO
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1988 2023-07-04 04:55:30.000000 django-file-explorer-1.6.0/django_file_explorer.egg-info/SOURCES.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        1 2023-07-04 04:55:30.000000 django-file-explorer-1.6.0/django_file_explorer.egg-info/dependency_links.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       60 2023-07-04 04:55:30.000000 django-file-explorer-1.6.0/django_file_explorer.egg-info/requires.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       19 2023-07-04 04:55:30.000000 django-file-explorer-1.6.0/django_file_explorer.egg-info/top_level.txt
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.187729 django-file-explorer-1.6.0/explorer/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       21 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1273 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/admin.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      148 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/apps.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.187729 django-file-explorer-1.6.0/explorer/migrations/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      870 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/migrations/0001_initial.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      764 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/migrations/0002_option.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1164 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/migrations/0003_userrole.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      534 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/migrations/0004_auto_20221117_1449.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      373 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/migrations/0005_rename_opertations_userrole_actions.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      835 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/migrations/0006_auto_20230215_1122.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/migrations/__init__.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.187729 django-file-explorer-1.6.0/explorer/models/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       68 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/models/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      872 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/models/action.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1074 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/models/user_role.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      944 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/models/volume.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.183730 django-file-explorer-1.6.0/explorer/static/
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.187729 django-file-explorer-1.6.0/explorer/static/explorer/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      128 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/static/explorer/action.css
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3421 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/static/explorer/action.js
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2383 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/static/explorer/checkbox.js
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      104 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/static/explorer/common.js
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      119 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/static/explorer/icons.css
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       32 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/static/explorer/navigation.css
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1342 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/static/explorer/onload.js
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      360 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/static/explorer/summary.css
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       85 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/static/explorer/volume.css
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1663 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/static/explorer/volume.js
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.183730 django-file-explorer-1.6.0/explorer/templates/
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.187729 django-file-explorer-1.6.0/explorer/templates/explorer/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1051 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/templates/explorer/about.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2868 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/templates/explorer/base.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      374 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/templates/explorer/error.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     7985 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/templates/explorer/index.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2288 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/templates/explorer/login.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      450 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/templates/explorer/logout.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      331 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/templates/explorer/warning.html
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       60 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/tests.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      407 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/urls.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.187729 django-file-explorer-1.6.0/explorer/views/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      103 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      835 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/about.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.191729 django-file-explorer-1.6.0/explorer/views/extractor/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/extractor/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3703 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/extractor/location.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1683 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/extractor/request.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1163 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/extractor/user.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.191729 django-file-explorer-1.6.0/explorer/views/logger/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/logger/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3785 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/logger/logger.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1059 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/login.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      542 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/logout.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     5657 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/main.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.191729 django-file-explorer-1.6.0/explorer/views/operations/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/operations/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     4248 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/operations/action.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     6689 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/operations/explorer.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2717 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/operations/location.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.191729 django-file-explorer-1.6.0/explorer/views/utils/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/utils/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      605 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/utils/path.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:30.191729 django-file-explorer-1.6.0/explorer/views/validator/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/validator/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     6065 2023-07-04 04:55:26.000000 django-file-explorer-1.6.0/explorer/views/validator/request.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       38 2023-07-04 04:55:30.191729 django-file-explorer-1.6.0/setup.cfg
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1598 2023-06-16 05:35:59.000000 django-file-explorer-1.6.0/setup.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.785067 django-file-explorer-1.6.1/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     5943 2023-07-12 06:06:13.785067 django-file-explorer-1.6.1/PKG-INFO
+-rwxrwxr-x   0 sigma     (1000) sigma     (1000)     4987 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/README.md
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.781066 django-file-explorer-1.6.1/django_file_explorer.egg-info/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     5943 2023-07-12 06:06:13.000000 django-file-explorer-1.6.1/django_file_explorer.egg-info/PKG-INFO
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     2089 2023-07-12 06:06:13.000000 django-file-explorer-1.6.1/django_file_explorer.egg-info/SOURCES.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        1 2023-07-12 06:06:13.000000 django-file-explorer-1.6.1/django_file_explorer.egg-info/dependency_links.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       60 2023-07-12 06:06:13.000000 django-file-explorer-1.6.1/django_file_explorer.egg-info/requires.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       19 2023-07-12 06:06:13.000000 django-file-explorer-1.6.1/django_file_explorer.egg-info/top_level.txt
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.781066 django-file-explorer-1.6.1/explorer/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       21 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1273 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/admin.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      148 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/apps.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.781066 django-file-explorer-1.6.1/explorer/migrations/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      870 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/migrations/0001_initial.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      764 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/migrations/0002_option.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1164 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/migrations/0003_userrole.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      534 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/migrations/0004_auto_20221117_1449.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      373 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/migrations/0005_rename_opertations_userrole_actions.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      835 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/migrations/0006_auto_20230215_1122.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/migrations/__init__.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.781066 django-file-explorer-1.6.1/explorer/models/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       68 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/models/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      872 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/models/action.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1074 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/models/user_role.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      944 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/models/volume.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.777066 django-file-explorer-1.6.1/explorer/static/
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.777066 django-file-explorer-1.6.1/explorer/static/bootstrap/
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.781066 django-file-explorer-1.6.1/explorer/static/bootstrap/css/
+-rw-r--r--   0 sigma     (1000) sigma     (1000)   162264 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/static/bootstrap/css/bootstrap.min.css
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.781066 django-file-explorer-1.6.1/explorer/static/bootstrap/js/
+-rw-r--r--   0 sigma     (1000) sigma     (1000)    83376 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/static/bootstrap/js/bootstrap.bundle.min.js
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.781066 django-file-explorer-1.6.1/explorer/static/explorer/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      128 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/static/explorer/action.css
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3421 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/static/explorer/action.js
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     2383 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/static/explorer/checkbox.js
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      104 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/static/explorer/common.js
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      119 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/static/explorer/icons.css
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       32 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/static/explorer/navigation.css
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1342 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/static/explorer/onload.js
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      360 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/static/explorer/summary.css
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       85 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/static/explorer/volume.css
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1663 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/static/explorer/volume.js
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.777066 django-file-explorer-1.6.1/explorer/templates/
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.785067 django-file-explorer-1.6.1/explorer/templates/explorer/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1051 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/templates/explorer/about.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     2627 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/templates/explorer/base.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      374 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/templates/explorer/error.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     7985 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/templates/explorer/index.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     2288 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/templates/explorer/login.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      450 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/templates/explorer/logout.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      331 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/templates/explorer/warning.html
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       60 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/tests.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      407 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/urls.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.785067 django-file-explorer-1.6.1/explorer/views/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      103 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      835 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/about.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.785067 django-file-explorer-1.6.1/explorer/views/extractor/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/extractor/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3703 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/extractor/location.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1683 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/extractor/request.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1163 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/extractor/user.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.785067 django-file-explorer-1.6.1/explorer/views/logger/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/logger/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3785 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/logger/logger.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1059 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/login.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      542 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/logout.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     5657 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/main.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.785067 django-file-explorer-1.6.1/explorer/views/operations/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/operations/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     4248 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/operations/action.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     6689 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/operations/explorer.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     2717 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/operations/location.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.785067 django-file-explorer-1.6.1/explorer/views/utils/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/utils/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      605 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/utils/path.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:13.785067 django-file-explorer-1.6.1/explorer/views/validator/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        0 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/validator/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     6065 2023-07-12 06:06:09.000000 django-file-explorer-1.6.1/explorer/views/validator/request.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       38 2023-07-12 06:06:13.785067 django-file-explorer-1.6.1/setup.cfg
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1598 2023-06-16 05:35:59.000000 django-file-explorer-1.6.1/setup.py
```

### Comparing `django-file-explorer-1.6.0/PKG-INFO` & `django-file-explorer-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-file-explorer
-Version: 1.6.0
+Version: 1.6.1
 Summary: Django app to explore directory.
 Author: Tahir Rafique
 Author-email: tahirrafiqueasad@gmail.com
 License: MIT
 Keywords: explorer,file explorer,directory explorer,django explorer,location explorer
 Classifier: Framework :: Django :: 3.2
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -154,11 +154,12 @@
 
 ## Author
 
 **Tahir Rafique**
 
 ## Releases
 
-| Date      | Version | Summary                                |
-| --------- | ------- | -------------------------------------- |
-| 4-Jul-23  | v1.6.0  | Adding file unzip option.              |
-| 16-Jun-23 | v1.5.0  | Separating vscode icons from this app. |
+| Date      | Version | Summary                                                      |
+| --------- | ------- | ------------------------------------------------------------ |
+| 12-Jul-23 | v1.6.1  | Adding local bootstrap 4.6.2 files. This will correct the wrong appearance of UI when there is no Internet connection. |
+| 4-Jul-23  | v1.6.0  | Adding file unzip option.                                    |
+| 16-Jun-23 | v1.5.0  | Separating vscode icons from this app.                       |
```

### Comparing `django-file-explorer-1.6.0/README.md` & `django-file-explorer-1.6.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -131,11 +131,12 @@
 
 ## Author
 
 **Tahir Rafique**
 
 ## Releases
 
-| Date      | Version | Summary                                |
-| --------- | ------- | -------------------------------------- |
-| 4-Jul-23  | v1.6.0  | Adding file unzip option.              |
-| 16-Jun-23 | v1.5.0  | Separating vscode icons from this app. |
+| Date      | Version | Summary                                                      |
+| --------- | ------- | ------------------------------------------------------------ |
+| 12-Jul-23 | v1.6.1  | Adding local bootstrap 4.6.2 files. This will correct the wrong appearance of UI when there is no Internet connection. |
+| 4-Jul-23  | v1.6.0  | Adding file unzip option.                                    |
+| 16-Jun-23 | v1.5.0  | Separating vscode icons from this app.                       |
```

### Comparing `django-file-explorer-1.6.0/django_file_explorer.egg-info/PKG-INFO` & `django-file-explorer-1.6.1/django_file_explorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-file-explorer
-Version: 1.6.0
+Version: 1.6.1
 Summary: Django app to explore directory.
 Author: Tahir Rafique
 Author-email: tahirrafiqueasad@gmail.com
 License: MIT
 Keywords: explorer,file explorer,directory explorer,django explorer,location explorer
 Classifier: Framework :: Django :: 3.2
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -154,11 +154,12 @@
 
 ## Author
 
 **Tahir Rafique**
 
 ## Releases
 
-| Date      | Version | Summary                                |
-| --------- | ------- | -------------------------------------- |
-| 4-Jul-23  | v1.6.0  | Adding file unzip option.              |
-| 16-Jun-23 | v1.5.0  | Separating vscode icons from this app. |
+| Date      | Version | Summary                                                      |
+| --------- | ------- | ------------------------------------------------------------ |
+| 12-Jul-23 | v1.6.1  | Adding local bootstrap 4.6.2 files. This will correct the wrong appearance of UI when there is no Internet connection. |
+| 4-Jul-23  | v1.6.0  | Adding file unzip option.                                    |
+| 16-Jun-23 | v1.5.0  | Separating vscode icons from this app.                       |
```

### Comparing `django-file-explorer-1.6.0/django_file_explorer.egg-info/SOURCES.txt` & `django-file-explorer-1.6.1/django_file_explorer.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 explorer/migrations/0005_rename_opertations_userrole_actions.py
 explorer/migrations/0006_auto_20230215_1122.py
 explorer/migrations/__init__.py
 explorer/models/__init__.py
 explorer/models/action.py
 explorer/models/user_role.py
 explorer/models/volume.py
+explorer/static/bootstrap/css/bootstrap.min.css
+explorer/static/bootstrap/js/bootstrap.bundle.min.js
 explorer/static/explorer/action.css
 explorer/static/explorer/action.js
 explorer/static/explorer/checkbox.js
 explorer/static/explorer/common.js
 explorer/static/explorer/icons.css
 explorer/static/explorer/navigation.css
 explorer/static/explorer/onload.js
```

### Comparing `django-file-explorer-1.6.0/explorer/admin.py` & `django-file-explorer-1.6.1/explorer/admin.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/migrations/0001_initial.py` & `django-file-explorer-1.6.1/explorer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/migrations/0002_option.py` & `django-file-explorer-1.6.1/explorer/migrations/0002_option.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/migrations/0003_userrole.py` & `django-file-explorer-1.6.1/explorer/migrations/0003_userrole.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/migrations/0004_auto_20221117_1449.py` & `django-file-explorer-1.6.1/explorer/migrations/0004_auto_20221117_1449.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/migrations/0006_auto_20230215_1122.py` & `django-file-explorer-1.6.1/explorer/migrations/0006_auto_20230215_1122.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/models/action.py` & `django-file-explorer-1.6.1/explorer/models/action.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/models/user_role.py` & `django-file-explorer-1.6.1/explorer/models/user_role.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/models/volume.py` & `django-file-explorer-1.6.1/explorer/models/volume.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/static/explorer/action.js` & `django-file-explorer-1.6.1/explorer/static/explorer/action.js`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/static/explorer/checkbox.js` & `django-file-explorer-1.6.1/explorer/static/explorer/checkbox.js`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/static/explorer/onload.js` & `django-file-explorer-1.6.1/explorer/static/explorer/onload.js`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/static/explorer/volume.js` & `django-file-explorer-1.6.1/explorer/static/explorer/volume.js`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/templates/explorer/about.html` & `django-file-explorer-1.6.1/explorer/templates/explorer/about.html`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/templates/explorer/base.html` & `django-file-explorer-1.6.1/explorer/templates/explorer/base.html`

 * *Files 11% similar despite different names*

```diff
@@ -23,19 +23,17 @@
     <link rel="stylesheet" href="{% static 'explorer/summary.css' %}">
     <link rel="stylesheet" href="{% static 'explorer/volume.css' %}">
     <link rel="stylesheet" href="{% static 'explorer/action.css' %}">
     <link rel="stylesheet" href="{% static 'explorer/navigation.css' %}">
     <link rel="stylesheet" href="{% static 'explorer/icons.css' %}">
 
     <!-- BOOTSTRAP -->
-    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.6.1/dist/css/bootstrap.min.css">
-    <script src="https://cdn.jsdelivr.net/npm/jquery@3.6.0/dist/jquery.slim.min.js"></script>
-    <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js"></script>
-    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.1/dist/js/bootstrap.bundle.min.js"></script>
     <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
+    <link rel="stylesheet" href="{% static 'bootstrap/css/bootstrap.min.css' %}">
+    <script src="{% static 'bootstrap/js/bootstrap.bundle.min.js' %}"></script>
 
     <!-- <script>
         // GLOBAL VARIABLES
         var volume_data = JSON.parse("{{ volume_data|escapejs }}");
     </script> -->
     <!-- GLOBAL -->
     {{ volume_data|json_script:"volume_data" }}
```

### Comparing `django-file-explorer-1.6.0/explorer/templates/explorer/index.html` & `django-file-explorer-1.6.1/explorer/templates/explorer/index.html`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/templates/explorer/login.html` & `django-file-explorer-1.6.1/explorer/templates/explorer/login.html`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/views/about.py` & `django-file-explorer-1.6.1/explorer/views/about.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/views/extractor/location.py` & `django-file-explorer-1.6.1/explorer/views/extractor/location.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/views/extractor/request.py` & `django-file-explorer-1.6.1/explorer/views/extractor/request.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/views/extractor/user.py` & `django-file-explorer-1.6.1/explorer/views/extractor/user.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/views/logger/logger.py` & `django-file-explorer-1.6.1/explorer/views/logger/logger.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/views/login.py` & `django-file-explorer-1.6.1/explorer/views/login.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/views/logout.py` & `django-file-explorer-1.6.1/explorer/views/logout.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/views/main.py` & `django-file-explorer-1.6.1/explorer/views/main.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/views/operations/action.py` & `django-file-explorer-1.6.1/explorer/views/operations/action.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/views/operations/explorer.py` & `django-file-explorer-1.6.1/explorer/views/operations/explorer.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/views/operations/location.py` & `django-file-explorer-1.6.1/explorer/views/operations/location.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/views/utils/path.py` & `django-file-explorer-1.6.1/explorer/views/utils/path.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/explorer/views/validator/request.py` & `django-file-explorer-1.6.1/explorer/views/validator/request.py`

 * *Files identical despite different names*

### Comparing `django-file-explorer-1.6.0/setup.py` & `django-file-explorer-1.6.1/setup.py`

 * *Files identical despite different names*


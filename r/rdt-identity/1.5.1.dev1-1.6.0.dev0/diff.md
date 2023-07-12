# Comparing `tmp/rdt_identity-1.5.1.dev1.tar.gz` & `tmp/rdt_identity-1.6.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt_identity-1.5.1.dev1.tar", last modified: Mon Jul 10 20:51:23 2023, max compression
+gzip compressed data, was "rdt_identity-1.6.0.dev0.tar", last modified: Wed Jul 12 17:39:54 2023, max compression
```

## Comparing `rdt_identity-1.5.1.dev1.tar` & `rdt_identity-1.6.0.dev0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.896900 rdt_identity-1.5.1.dev1/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    44576 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7964 2023-07-10 20:51:23.897003 rdt_identity-1.5.1.dev1/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.884719 rdt_identity-1.5.1.dev1/rdt/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.884791 rdt_identity-1.5.1.dev1/rdt/transformers/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.884859 rdt_identity-1.5.1.dev1/rdt/transformers/addons/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.888351 rdt_identity-1.5.1.dev1/rdt/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/rdt/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/rdt/transformers/addons/identity/identity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-07-10 20:51:23.897564 rdt_identity-1.5.1.dev1/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4134 2023-07-10 19:31:05.000000 rdt_identity-1.5.1.dev1/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.888840 rdt_identity-1.5.1.dev1/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.885124 rdt_identity-1.5.1.dev1/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.889681 rdt_identity-1.5.1.dev1/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.890220 rdt_identity-1.5.1.dev1/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    45119 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.891770 rdt_identity-1.5.1.dev1/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.892133 rdt_identity-1.5.1.dev1/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-06-28 22:45:00.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5946 2023-07-05 23:04:49.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10507 2023-06-28 22:45:00.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev1/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.892671 rdt_identity-1.5.1.dev1/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev1/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.893015 rdt_identity-1.5.1.dev1/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.5.1.dev1/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.893518 rdt_identity-1.5.1.dev1/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-06-20 18:01:47.000000 rdt_identity-1.5.1.dev1/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103941 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.895367 rdt_identity-1.5.1.dev1/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.895543 rdt_identity-1.5.1.dev1/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.895888 rdt_identity-1.5.1.dev1/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:23.896723 rdt_identity-1.5.1.dev1/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18310 2023-07-05 23:04:49.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19138 2023-06-28 22:45:00.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt_identity-1.5.1.dev1/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.145932 rdt_identity-1.6.0.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    44576 2023-07-12 17:38:30.000000 rdt_identity-1.6.0.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7964 2023-07-12 17:39:54.146032 rdt_identity-1.6.0.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.133123 rdt_identity-1.6.0.dev0/rdt/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.133190 rdt_identity-1.6.0.dev0/rdt/transformers/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.133258 rdt_identity-1.6.0.dev0/rdt/transformers/addons/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.137372 rdt_identity-1.6.0.dev0/rdt/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/rdt/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/rdt/transformers/addons/identity/identity.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-07-12 17:39:54.146575 rdt_identity-1.6.0.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4134 2023-07-12 17:39:40.000000 rdt_identity-1.6.0.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.138097 rdt_identity-1.6.0.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/tests/code_style.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/contributing.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.133564 rdt_identity-1.6.0.dev0/tests/datasets/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.139350 rdt_identity-1.6.0.dev0/tests/datasets/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/datasets/tests/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/datasets/tests/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/datasets/tests/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/datasets/tests/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/datasets/tests/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.139920 rdt_identity-1.6.0.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    45119 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/integration/test_hyper_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/integration/test_transformers.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.141343 rdt_identity-1.6.0.dev0/tests/integration/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.141668 rdt_identity-1.6.0.dev0/tests/integration/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7106 2023-07-12 17:38:36.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-06-28 22:45:00.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5946 2023-07-05 23:04:49.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10507 2023-06-28 22:45:00.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.6.0.dev0/tests/integration/transformers/test_text.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.142190 rdt_identity-1.6.0.dev0/tests/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/performance/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/performance/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.6.0.dev0/tests/performance/test_performance.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.142516 rdt_identity-1.6.0.dev0/tests/performance/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/performance/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.6.0.dev0/tests/performance/tests/test_profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.142983 rdt_identity-1.6.0.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-06-20 18:01:47.000000 rdt_identity-1.6.0.dev0/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   103941 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/unit/test_hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.144869 rdt_identity-1.6.0.dev0/tests/unit/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.145022 rdt_identity-1.6.0.dev0/tests/unit/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/addons/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.145337 rdt_identity-1.6.0.dev0/tests/unit/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/addons/identity/test_identity.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:54.145795 rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    29367 2023-07-12 17:38:36.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18310 2023-07-05 23:04:49.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19138 2023-06-28 22:45:00.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt_identity-1.6.0.dev0/tests/unit/transformers/test_utils.py
```

### Comparing `rdt_identity-1.5.1.dev1/CONTRIBUTING.rst` & `rdt_identity-1.6.0.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/HISTORY.md` & `rdt_identity-1.6.0.dev0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/LICENSE` & `rdt_identity-1.6.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/PKG-INFO` & `rdt_identity-1.6.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt_identity
-Version: 1.5.1.dev1
+Version: 1.6.0.dev0
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt,rdt_identity
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rdt_identity Version: 1.5.1.dev1 Summary:
+Metadata-Version: 2.1 Name: rdt_identity Version: 1.6.0.dev0 Summary:
 Reversible Data Transforms Home-page: https://github.com/sdv-dev/RDT Author:
 DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1 Keywords:
 rdt,rdt_identity Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: Free for non-commercial
 use Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `rdt_identity-1.5.1.dev1/README.md` & `rdt_identity-1.6.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/RELEASE.md` & `rdt_identity-1.6.0.dev0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/rdt/transformers/addons/identity/identity.py` & `rdt_identity-1.6.0.dev0/rdt/transformers/addons/identity/identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/setup.cfg` & `rdt_identity-1.6.0.dev0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.5.1.dev1
+current_version = 1.6.0.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `rdt_identity-1.5.1.dev1/setup.py` & `rdt_identity-1.6.0.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,10 +135,10 @@
         exclude=['rdt.transformers.addons.*']
     ),
     python_requires='>=3.8,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/RDT',
-    version='1.5.1.dev1',
+    version='1.6.0.dev0',
     zip_safe=False,
 )
```

### Comparing `rdt_identity-1.5.1.dev1/tests/__init__.py` & `rdt_identity-1.6.0.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/code_style.py` & `rdt_identity-1.6.0.dev0/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/contributing.py` & `rdt_identity-1.6.0.dev0/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/datasets/tests/test_boolean.py` & `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/datasets/tests/test_categorical.py` & `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/datasets/tests/test_datetime.py` & `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/datasets/tests/test_numerical.py` & `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/datasets/tests/test_utils.py` & `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/integration/test_hyper_transformer.py` & `rdt_identity-1.6.0.dev0/tests/integration/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/integration/test_transformers.py` & `rdt_identity-1.6.0.dev0/tests/integration/test_transformers.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/integration/transformers/pii/test_anonymizer.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,34 @@
 
     expected_transformed = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
     })
 
     pd.testing.assert_frame_equal(transformed, expected_transformed)
     assert len(reverse_transform['username']) == 5
+    assert reverse_transform['username'].isna().sum() == 1
+
+
+def test_anonymizedfaker_with_nans_missing_value_generation_none():
+    """End to end test settings missing_value_generation=None."""
+    data = pd.DataFrame({
+        'id': [1, 2, 3, 4, 5],
+        'username': ['a', np.nan, 'c', 'd', 'e']
+    })
+
+    instance = AnonymizedFaker(missing_value_generation=None)
+    transformed = instance.fit_transform(data, 'username')
+    reverse_transform = instance.reverse_transform(transformed)
+
+    expected_transformed = pd.DataFrame({
+        'id': [1, 2, 3, 4, 5],
+    })
+
+    pd.testing.assert_frame_equal(transformed, expected_transformed)
+    assert len(reverse_transform['username']) == 5
     assert reverse_transform['username'].isna().sum() == 0
 
 
 def test_anonymizedfaker_custom_provider_with_nans():
     """End to end test with a custom provider for the ``AnonymizedFaker`` with `` nans``."""
     data = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
@@ -98,15 +118,15 @@
     expected_transformed = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
         'username': ['a', 'b', 'c', 'd', 'e'],
     })
 
     pd.testing.assert_frame_equal(transformed, expected_transformed)
     assert len(reverse_transform['cc']) == 5
-    assert reverse_transform['cc'].isna().sum() == 0
+    assert reverse_transform['cc'].isna().sum() == 1
 
 
 def test_anonymizedfaker_enforce_uniqueness():
     """Test that ``AnonymizedFaker`` works with uniqueness.
 
     Also ensure that when we call ``reset_randomization`` the generator will be able to
     create values again.
```

### Comparing `rdt_identity-1.5.1.dev1/tests/integration/transformers/test_base.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/integration/transformers/test_boolean.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/integration/transformers/test_categorical.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/integration/transformers/test_datetime.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/integration/transformers/test_numerical.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/integration/transformers/test_text.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/performance/test_performance.py` & `rdt_identity-1.6.0.dev0/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/performance/tests/test_profiling.py` & `rdt_identity-1.6.0.dev0/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/test___init__.py` & `rdt_identity-1.6.0.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/test_hyper_transformer.py` & `rdt_identity-1.6.0.dev0/tests/unit/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/transformers/addons/identity/test_identity.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/transformers/pii/test_anonymizer.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,31 @@
         mock_check_provider_function.assert_called_once_with('BaseProvider', 'lexify')
         assert instance.provider_name == 'BaseProvider'
         assert instance.function_name == 'lexify'
         assert instance.function_kwargs == {}
         assert instance.locales is None
         assert mock_faker.Faker.called_once_with(None)
         assert instance.enforce_uniqueness is False
+        assert instance.missing_value_generation == 'random'
+
+    def test___init__error_missing_value_generation(self):
+        """Test that the ``__init__`` raises an error if the missing value generation is invalid.
+
+        Test that the ``__init__`` raises an error if the missing value generation is invalid.
+
+        Side effects:
+            - ``ValueError`` is raised.
+        """
+        expected_message = (
+            "Missing value generation 'invalid' is not supported "
+            "for AnonymizedFaker. Please use either 'random' or None."
+        )
+        # Run and Assert
+        with pytest.raises(TransformerInputError, match=expected_message):
+            AnonymizedFaker(missing_value_generation='invalid')
 
     @patch('rdt.transformers.pii.anonymizer.faker')
     @patch('rdt.transformers.pii.anonymizer.AnonymizedFaker.check_provider_function')
     def test___init__custom(self, mock_check_provider_function, mock_faker):
         """Test the instantiation of the transformer with custom parameters.
 
         Test that the transformer can be instantiated with a custom provider and function, and
@@ -308,23 +325,24 @@
             - ``pd.Series`` containing 3 strings.
 
         Side Effects:
             - ``instance.data_length`` equals to the length of the input data.
         """
         # Setup
         transformer = AnonymizedFaker()
-        columns_data = pd.Series(['1', '2', '3'])
+        columns_data = pd.Series(['1', '2', '3', None, np.nan])
         transformer.columns = ['col']
 
         # Run
         transformer._fit(columns_data)
 
         # Assert
-        assert transformer.data_length == 3
+        assert transformer.data_length == 5
         assert transformer.output_properties == {None: {'next_transformer': None}}
+        assert transformer._nan_frequency == 0.4
 
     def test__transform(self):
         """Test the ``_transform`` method.
 
         Validate that the ``_transform`` method returns ``None``.
 
         Setup:
@@ -373,14 +391,34 @@
         # Run
         result = instance._reverse_transform(None)
 
         # Assert
         assert function.call_args_list == [call(), call(), call()]
         np.testing.assert_array_equal(result, np.array(['a', 'b', 'c']))
 
+    def test__reverse_transform_with_nans(self):
+        """Test that ``_reverse_transform`` generates NaNs."""
+        # Setup
+        instance = AnonymizedFaker()
+        instance.data_length = 4
+        instance._nan_frequency = 0.25
+        function = Mock()
+        function.side_effect = ['a', 'b', 'c', 'd']
+
+        instance._function = function
+
+        # Run
+        result = instance._reverse_transform(None)
+        result = pd.Series(result)
+
+        # Assert
+        assert function.call_args_list == [call(), call(), call(), call()]
+        assert instance.missing_value_generation == 'random'
+        assert result.isna().sum() == 1
+
     def test__reverse_transform_not_enough_unique_values(self):
         """Test the ``_reverse_transform`` method.
 
         Test that when calling the ``_reverse_transform`` method and the ``instance._function`` is
         not generating enough unique values raises an error.
 
         Setup:
```

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/transformers/pii/test_utils.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/transformers/test___init__.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_base.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_boolean.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_categorical.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_datetime.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_null.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_null.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_numerical.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_text.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.5.1.dev1/tests/unit/transformers/test_utils.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*


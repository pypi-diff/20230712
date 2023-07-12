# Comparing `tmp/rdt_identity-1.6.0.tar.gz` & `tmp/rdt_identity-1.6.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt_identity-1.6.0.tar", last modified: Wed Jul 12 20:34:36 2023, max compression
+gzip compressed data, was "rdt_identity-1.6.0.dev0.tar", last modified: Wed Jul 12 17:39:54 2023, max compression
```

## Comparing `rdt_identity-1.6.0.tar` & `rdt_identity-1.6.0.dev0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.182358 rdt_identity-1.6.0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt_identity-1.6.0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt_identity-1.6.0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    46119 2023-07-12 20:34:31.000000 rdt_identity-1.6.0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt_identity-1.6.0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7959 2023-07-12 20:34:36.182459 rdt_identity-1.6.0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt_identity-1.6.0/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.170201 rdt_identity-1.6.0/rdt/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.170320 rdt_identity-1.6.0/rdt/transformers/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.170413 rdt_identity-1.6.0/rdt/transformers/addons/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.173766 rdt_identity-1.6.0/rdt/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/rdt/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1170 2023-01-18 20:52:41.000000 rdt_identity-1.6.0/rdt/transformers/addons/identity/identity.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1590 2023-07-12 20:34:36.182989 rdt_identity-1.6.0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4129 2023-07-12 20:34:31.000000 rdt_identity-1.6.0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.174261 rdt_identity-1.6.0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt_identity-1.6.0/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt_identity-1.6.0/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.170717 rdt_identity-1.6.0/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.175134 rdt_identity-1.6.0/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.175782 rdt_identity-1.6.0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    45119 2023-06-01 21:46:38.000000 rdt_identity-1.6.0/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt_identity-1.6.0/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.177033 rdt_identity-1.6.0/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.177392 rdt_identity-1.6.0/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7106 2023-07-12 20:34:31.000000 rdt_identity-1.6.0/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt_identity-1.6.0/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-07-12 20:34:31.000000 rdt_identity-1.6.0/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt_identity-1.6.0/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5946 2023-07-12 20:34:31.000000 rdt_identity-1.6.0/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10507 2023-07-12 20:34:31.000000 rdt_identity-1.6.0/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt_identity-1.6.0/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.178010 rdt_identity-1.6.0/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt_identity-1.6.0/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.178325 rdt_identity-1.6.0/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt_identity-1.6.0/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.178835 rdt_identity-1.6.0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-07-12 20:34:31.000000 rdt_identity-1.6.0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103941 2023-06-01 21:46:38.000000 rdt_identity-1.6.0/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.181161 rdt_identity-1.6.0/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.181327 rdt_identity-1.6.0/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.181709 rdt_identity-1.6.0/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt_identity-1.6.0/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 20:34:36.182217 rdt_identity-1.6.0/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt_identity-1.6.0/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    29367 2023-07-12 20:34:31.000000 rdt_identity-1.6.0/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt_identity-1.6.0/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt_identity-1.6.0/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt_identity-1.6.0/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt_identity-1.6.0/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt_identity-1.6.0/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18310 2023-07-12 20:34:31.000000 rdt_identity-1.6.0/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19138 2023-07-12 20:34:31.000000 rdt_identity-1.6.0/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt_identity-1.6.0/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt_identity-1.6.0/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt_identity-1.6.0/tests/unit/transformers/test_utils.py
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

### Comparing `rdt_identity-1.6.0/CONTRIBUTING.rst` & `rdt_identity-1.6.0.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/HISTORY.md` & `rdt_identity-1.6.0.dev0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,9 @@
 # History
 
-## 1.6.0 -2023-07-12
-
-This release adds the ability to generate missing values to the `AnonymizedFaker`. Users can now provide the `missing_value_generation` parameter during initialization. They can set it to `None` to not generate any missing values, or `'random'` to generate random missing values in the same proportion as the fitted data.
-
-Additionally, this release improves the `NullTransformer` by allowing nulls to be replaced on the forward transform even if `missing_value_generation` is set to None. It also fixes a bug that was causing the `UnixTimestampEncoder` to return a different dtype than the input on `reverse_transform`. This was particularly problematic when datetime columns are represented as ints.
-
-### New Features
-
-* AnonymizedFaker should be able to model and generate missing values - Issue [#660](https://github.com/sdv-dev/RDT/issues/660) by @R-Palazzo
-
-### Bugs
-
-* The datetime transformers don't give me back the same dtype sometimes - Issue [#657](https://github.com/sdv-dev/RDT/issues/657) by @frances-h
-* RDT NullTransformer doesn't replace nulls if missing_value_generation is None - Issue [#658](https://github.com/sdv-dev/RDT/issues/658) by @amontanez24
-
-### Maintenance
-
-* Remove python 3.7 builds - Issue [#663](https://github.com/sdv-dev/RDT/issues/663) by @amontanez24
-* Drop support for Python 3.7 - Issue [#666](https://github.com/sdv-dev/RDT/issues/666) by @amontanez24
-
-### Internal
-
-* Add add-on modules to sys.modules - Issue [#653](https://github.com/sdv-dev/RDT/issues/653) by @amontanez24
-
 ## 1.5.0 - 2023-06-01
 
 This release adds a new parameter called `missing_value_generation` to the initialization of certain transformers to specify how missing values should be created. The parameter can be used in the `FloatFormatter`, `BinaryEncoder`, `UnixTimestampEncoder`, `OptimizedTimestampEncoder`, `GaussianNormalizer` and `ClusterBasedNormalizer`. Additionally, it fixes a bug that was causing every column that had nulls to generate them in the same place.
 
 ### Deprecations
 
 * The `model_missing_values` parameter is being deprecated in favor of the new `missing_value_generation` parameter.
```

### Comparing `rdt_identity-1.6.0/LICENSE` & `rdt_identity-1.6.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/PKG-INFO` & `rdt_identity-1.6.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt_identity
-Version: 1.6.0
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
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: rdt_identity Version: 1.6.0 Summary: Reversible
-Data Transforms Home-page: https://github.com/sdv-dev/RDT Author: DataCebo,
-Inc. Author-email: info@sdv.dev License: BSL-1.1 Keywords: rdt,rdt_identity
-Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
-:: Developers Classifier: License :: Free for non-commercial use Classifier:
-Natural Language :: English Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8,<3.12
-Description-Content-Type: text/markdown License-File: LICENSE License-File:
-AUTHORS.rst
+Metadata-Version: 2.1 Name: rdt_identity Version: 1.6.0.dev0 Summary:
+Reversible Data Transforms Home-page: https://github.com/sdv-dev/RDT Author:
+DataCebo, Inc. Author-email: info@sdv.dev License: BSL-1.1 Keywords:
+rdt,rdt_identity Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+Intended Audience :: Developers Classifier: License :: Free for non-commercial
+use Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
+>=3.8,<3.12 Description-Content-Type: text/markdown License-File: LICENSE
+License-File: AUTHORS.rst
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
 [![Development Status](https://img.shields.io/badge/Development%20Status-3%20--
                   %20Alpha-yellow)](https://pypi.org/search/
     ?q=&o=&c=Development+Status+%3A%3A+3+-+Alpha) [![PyPi Shield](https://
    img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT) [![Unit
```

### Comparing `rdt_identity-1.6.0/README.md` & `rdt_identity-1.6.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/RELEASE.md` & `rdt_identity-1.6.0.dev0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/rdt/transformers/addons/identity/identity.py` & `rdt_identity-1.6.0.dev0/rdt/transformers/addons/identity/identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/setup.cfg` & `rdt_identity-1.6.0.dev0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.6.0
+current_version = 1.6.0.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `rdt_identity-1.6.0/setup.py` & `rdt_identity-1.6.0.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,10 +135,10 @@
         exclude=['rdt.transformers.addons.*']
     ),
     python_requires='>=3.8,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/RDT',
-    version='1.6.0',
+    version='1.6.0.dev0',
     zip_safe=False,
 )
```

### Comparing `rdt_identity-1.6.0/tests/__init__.py` & `rdt_identity-1.6.0.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/code_style.py` & `rdt_identity-1.6.0.dev0/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/contributing.py` & `rdt_identity-1.6.0.dev0/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/datasets/tests/test_boolean.py` & `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/datasets/tests/test_categorical.py` & `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/datasets/tests/test_datetime.py` & `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/datasets/tests/test_numerical.py` & `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/datasets/tests/test_utils.py` & `rdt_identity-1.6.0.dev0/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/integration/test_hyper_transformer.py` & `rdt_identity-1.6.0.dev0/tests/integration/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/integration/test_transformers.py` & `rdt_identity-1.6.0.dev0/tests/integration/test_transformers.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/integration/transformers/pii/test_anonymizer.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/integration/transformers/test_base.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/integration/transformers/test_boolean.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/integration/transformers/test_categorical.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/integration/transformers/test_datetime.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/integration/transformers/test_numerical.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/integration/transformers/test_text.py` & `rdt_identity-1.6.0.dev0/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/performance/test_performance.py` & `rdt_identity-1.6.0.dev0/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/performance/tests/test_profiling.py` & `rdt_identity-1.6.0.dev0/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/test___init__.py` & `rdt_identity-1.6.0.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/test_hyper_transformer.py` & `rdt_identity-1.6.0.dev0/tests/unit/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/transformers/addons/identity/test_identity.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/transformers/pii/test_anonymizer.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/transformers/pii/test_utils.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/transformers/test___init__.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/transformers/test_base.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/transformers/test_boolean.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/transformers/test_categorical.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/transformers/test_datetime.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/transformers/test_null.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_null.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/transformers/test_numerical.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/transformers/test_text.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt_identity-1.6.0/tests/unit/transformers/test_utils.py` & `rdt_identity-1.6.0.dev0/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*


# Comparing `tmp/rdt-1.5.1.dev1.tar.gz` & `tmp/rdt-1.6.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt-1.5.1.dev1.tar", last modified: Mon Jul 10 20:51:21 2023, max compression
+gzip compressed data, was "rdt-1.6.0.dev0.tar", last modified: Wed Jul 12 17:39:50 2023, max compression
```

## Comparing `rdt-1.5.1.dev1.tar` & `rdt-1.6.0.dev0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.622820 rdt-1.5.1.dev1/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    44576 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    52585 2023-07-10 20:51:21.623031 rdt-1.5.1.dev1/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.603252 rdt-1.5.1.dev1/rdt/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5342 2023-06-29 00:04:59.000000 rdt-1.5.1.dev1/rdt/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      729 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/rdt/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    30929 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/rdt/hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.605381 rdt-1.5.1.dev1/rdt/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      262 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/rdt/performance/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.607368 rdt-1.5.1.dev1/rdt/performance/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      847 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/rdt/performance/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1158 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/rdt/performance/datasets/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6125 2022-08-18 00:01:17.000000 rdt-1.5.1.dev1/rdt/performance/datasets/boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11724 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/performance/datasets/categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5734 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/rdt/performance/datasets/datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8406 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/rdt/performance/datasets/numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1893 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/performance/datasets/pii.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1898 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/rdt/performance/datasets/text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      558 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/rdt/performance/datasets/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3372 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/performance/performance.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3442 2022-08-18 00:01:17.000000 rdt-1.5.1.dev1/rdt/performance/profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.609571 rdt-1.5.1.dev1/rdt/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4940 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/rdt/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.609874 rdt-1.5.1.dev1/rdt/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3345 2023-07-10 19:31:05.000000 rdt-1.5.1.dev1/rdt/transformers/addons/addons_setup.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    15934 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/transformers/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3792 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/transformers/boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21411 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/rdt/transformers/categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10281 2023-07-05 23:04:49.000000 rdt-1.5.1.dev1/rdt/transformers/datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5878 2023-06-28 22:45:00.000000 rdt-1.5.1.dev1/rdt/transformers/null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22319 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/transformers/numerical.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.610523 rdt-1.5.1.dev1/rdt/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2022-08-18 00:01:17.000000 rdt-1.5.1.dev1/rdt/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12447 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/rdt/transformers/pii/anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1052 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/rdt/transformers/pii/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4847 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/rdt/transformers/text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4576 2023-04-26 21:05:25.000000 rdt-1.5.1.dev1/rdt/transformers/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.604701 rdt-1.5.1.dev1/rdt.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    52585 2023-07-10 20:51:21.000000 rdt-1.5.1.dev1/rdt.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2835 2023-07-10 20:51:21.000000 rdt-1.5.1.dev1/rdt.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-10 20:51:21.000000 rdt-1.5.1.dev1/rdt.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-10 20:51:21.000000 rdt-1.5.1.dev1/rdt.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1448 2023-07-10 20:51:21.000000 rdt-1.5.1.dev1/rdt.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-07-10 20:51:21.000000 rdt-1.5.1.dev1/rdt.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-07-10 20:51:21.623563 rdt-1.5.1.dev1/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4134 2023-07-10 19:31:05.000000 rdt-1.5.1.dev1/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.611028 rdt-1.5.1.dev1/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.599424 rdt-1.5.1.dev1/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.612002 rdt-1.5.1.dev1/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.612600 rdt-1.5.1.dev1/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    45119 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.614165 rdt-1.5.1.dev1/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.614517 rdt-1.5.1.dev1/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6410 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-06-28 22:45:00.000000 rdt-1.5.1.dev1/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5946 2023-07-05 23:04:49.000000 rdt-1.5.1.dev1/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10507 2023-06-28 22:45:00.000000 rdt-1.5.1.dev1/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.615245 rdt-1.5.1.dev1/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.615580 rdt-1.5.1.dev1/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt-1.5.1.dev1/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.616280 rdt-1.5.1.dev1/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-06-20 18:01:47.000000 rdt-1.5.1.dev1/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   103941 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.619763 rdt-1.5.1.dev1/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.620691 rdt-1.5.1.dev1/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.621658 rdt-1.5.1.dev1/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-10 20:51:21.622565 rdt-1.5.1.dev1/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt-1.5.1.dev1/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27923 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt-1.5.1.dev1/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18310 2023-07-05 23:04:49.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19138 2023-06-28 22:45:00.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt-1.5.1.dev1/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.295483 rdt-1.6.0.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    44576 2023-07-12 17:38:30.000000 rdt-1.6.0.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    52585 2023-07-12 17:39:50.295704 rdt-1.6.0.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.276897 rdt-1.6.0.dev0/rdt/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5342 2023-07-12 17:39:40.000000 rdt-1.6.0.dev0/rdt/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      729 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/rdt/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    30929 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/rdt/hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.279098 rdt-1.6.0.dev0/rdt/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      262 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/rdt/performance/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.281041 rdt-1.6.0.dev0/rdt/performance/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      847 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/rdt/performance/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1158 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/rdt/performance/datasets/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6125 2022-08-18 00:01:17.000000 rdt-1.6.0.dev0/rdt/performance/datasets/boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11724 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/rdt/performance/datasets/categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5734 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/rdt/performance/datasets/datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8406 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/rdt/performance/datasets/numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1893 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/rdt/performance/datasets/pii.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1898 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/rdt/performance/datasets/text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      558 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/rdt/performance/datasets/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3372 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/rdt/performance/performance.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3442 2022-08-18 00:01:17.000000 rdt-1.6.0.dev0/rdt/performance/profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.283415 rdt-1.6.0.dev0/rdt/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4940 2023-04-13 17:39:49.000000 rdt-1.6.0.dev0/rdt/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.283697 rdt-1.6.0.dev0/rdt/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3345 2023-07-10 19:31:05.000000 rdt-1.6.0.dev0/rdt/transformers/addons/addons_setup.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    15934 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/rdt/transformers/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3792 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/rdt/transformers/boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21411 2023-04-13 17:39:49.000000 rdt-1.6.0.dev0/rdt/transformers/categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10281 2023-07-05 23:04:49.000000 rdt-1.6.0.dev0/rdt/transformers/datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5878 2023-06-28 22:45:00.000000 rdt-1.6.0.dev0/rdt/transformers/null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22319 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/rdt/transformers/numerical.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.284414 rdt-1.6.0.dev0/rdt/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2022-08-18 00:01:17.000000 rdt-1.6.0.dev0/rdt/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13633 2023-07-12 17:38:36.000000 rdt-1.6.0.dev0/rdt/transformers/pii/anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1052 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/rdt/transformers/pii/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4847 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/rdt/transformers/text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4576 2023-04-26 21:05:25.000000 rdt-1.6.0.dev0/rdt/transformers/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.278423 rdt-1.6.0.dev0/rdt.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    52585 2023-07-12 17:39:50.000000 rdt-1.6.0.dev0/rdt.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2835 2023-07-12 17:39:50.000000 rdt-1.6.0.dev0/rdt.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-12 17:39:50.000000 rdt-1.6.0.dev0/rdt.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-12 17:39:50.000000 rdt-1.6.0.dev0/rdt.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1448 2023-07-12 17:39:50.000000 rdt-1.6.0.dev0/rdt.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-07-12 17:39:50.000000 rdt-1.6.0.dev0/rdt.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-07-12 17:39:50.296294 rdt-1.6.0.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4134 2023-07-12 17:39:40.000000 rdt-1.6.0.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.285257 rdt-1.6.0.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/tests/code_style.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/tests/contributing.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.273264 rdt-1.6.0.dev0/tests/datasets/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.286309 rdt-1.6.0.dev0/tests/datasets/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/datasets/tests/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/datasets/tests/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/datasets/tests/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/datasets/tests/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/datasets/tests/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.287092 rdt-1.6.0.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    45119 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/tests/integration/test_hyper_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/tests/integration/test_transformers.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.288620 rdt-1.6.0.dev0/tests/integration/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/integration/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.289004 rdt-1.6.0.dev0/tests/integration/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/integration/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7106 2023-07-12 17:38:36.000000 rdt-1.6.0.dev0/tests/integration/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/tests/integration/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-06-28 22:45:00.000000 rdt-1.6.0.dev0/tests/integration/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt-1.6.0.dev0/tests/integration/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5946 2023-07-05 23:04:49.000000 rdt-1.6.0.dev0/tests/integration/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10507 2023-06-28 22:45:00.000000 rdt-1.6.0.dev0/tests/integration/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt-1.6.0.dev0/tests/integration/transformers/test_text.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.289636 rdt-1.6.0.dev0/tests/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/performance/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/performance/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt-1.6.0.dev0/tests/performance/test_performance.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.289957 rdt-1.6.0.dev0/tests/performance/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/performance/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt-1.6.0.dev0/tests/performance/tests/test_profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.290604 rdt-1.6.0.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-06-20 18:01:47.000000 rdt-1.6.0.dev0/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   103941 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/tests/unit/test_hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.293882 rdt-1.6.0.dev0/tests/unit/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/unit/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.294137 rdt-1.6.0.dev0/tests/unit/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/unit/transformers/addons/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.294665 rdt-1.6.0.dev0/tests/unit/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/unit/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/tests/unit/transformers/addons/identity/test_identity.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-12 17:39:50.295247 rdt-1.6.0.dev0/tests/unit/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt-1.6.0.dev0/tests/unit/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    29367 2023-07-12 17:38:36.000000 rdt-1.6.0.dev0/tests/unit/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/tests/unit/transformers/pii/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-01-18 20:52:41.000000 rdt-1.6.0.dev0/tests/unit/transformers/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/tests/unit/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/tests/unit/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt-1.6.0.dev0/tests/unit/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18310 2023-07-05 23:04:49.000000 rdt-1.6.0.dev0/tests/unit/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19138 2023-06-28 22:45:00.000000 rdt-1.6.0.dev0/tests/unit/transformers/test_null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt-1.6.0.dev0/tests/unit/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt-1.6.0.dev0/tests/unit/transformers/test_text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt-1.6.0.dev0/tests/unit/transformers/test_utils.py
```

### Comparing `rdt-1.5.1.dev1/CONTRIBUTING.rst` & `rdt-1.6.0.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/HISTORY.md` & `rdt-1.6.0.dev0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/LICENSE` & `rdt-1.6.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/PKG-INFO` & `rdt-1.6.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt
-Version: 1.5.1.dev1
+Version: 1.6.0.dev0
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rdt Version: 1.5.1.dev1 Summary: Reversible Data
+Metadata-Version: 2.1 Name: rdt Version: 1.6.0.dev0 Summary: Reversible Data
 Transforms Home-page: https://github.com/sdv-dev/RDT Author: DataCebo, Inc.
 Author-email: info@sdv.dev License: BSL-1.1 Keywords: rdt Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `rdt-1.5.1.dev1/README.md` & `rdt-1.6.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/RELEASE.md` & `rdt-1.6.0.dev0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/__init__.py` & `rdt-1.6.0.dev0/rdt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for RDT."""
 
 
 __author__ = 'DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
-__version__ = '1.5.1.dev1'
+__version__ = '1.6.0.dev0'
 
 
 import sys
 import warnings
 from operator import attrgetter
 from types import ModuleType
```

### Comparing `rdt-1.5.1.dev1/rdt/errors.py` & `rdt-1.6.0.dev0/rdt/errors.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/hyper_transformer.py` & `rdt-1.6.0.dev0/rdt/hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/performance/datasets/__init__.py` & `rdt-1.6.0.dev0/rdt/performance/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/performance/datasets/base.py` & `rdt-1.6.0.dev0/rdt/performance/datasets/base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/performance/datasets/boolean.py` & `rdt-1.6.0.dev0/rdt/performance/datasets/boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/performance/datasets/categorical.py` & `rdt-1.6.0.dev0/rdt/performance/datasets/categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/performance/datasets/datetime.py` & `rdt-1.6.0.dev0/rdt/performance/datasets/datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/performance/datasets/numerical.py` & `rdt-1.6.0.dev0/rdt/performance/datasets/numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/performance/datasets/pii.py` & `rdt-1.6.0.dev0/rdt/performance/datasets/pii.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/performance/datasets/text.py` & `rdt-1.6.0.dev0/rdt/performance/datasets/text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/performance/datasets/utils.py` & `rdt-1.6.0.dev0/rdt/performance/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/performance/performance.py` & `rdt-1.6.0.dev0/rdt/performance/performance.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/performance/profiling.py` & `rdt-1.6.0.dev0/rdt/performance/profiling.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/transformers/__init__.py` & `rdt-1.6.0.dev0/rdt/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/transformers/addons/addons_setup.py` & `rdt-1.6.0.dev0/rdt/transformers/addons/addons_setup.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/transformers/base.py` & `rdt-1.6.0.dev0/rdt/transformers/base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/transformers/boolean.py` & `rdt-1.6.0.dev0/rdt/transformers/boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/transformers/categorical.py` & `rdt-1.6.0.dev0/rdt/transformers/categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/transformers/datetime.py` & `rdt-1.6.0.dev0/rdt/transformers/datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/transformers/null.py` & `rdt-1.6.0.dev0/rdt/transformers/null.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/transformers/numerical.py` & `rdt-1.6.0.dev0/rdt/transformers/numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/transformers/pii/anonymizer.py` & `rdt-1.6.0.dev0/rdt/transformers/pii/anonymizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,22 @@
             Keyword args to pass into the ``function_name`` when being called.
         locales (list):
             List of localized providers to use instead of the global provider.
         enforce_uniqueness (bool):
             Whether or not to ensure that the new anonymized data is all unique. If it isn't
             possible to create the requested number of rows, then an error will be raised.
             Defaults to ``False``.
+        missing_value_generation (str or None):
+            The way missing values are being handled. There are two strategies:
+
+                * ``random``: Randomly generates missing values based on the percentage of
+                  missing values.
+                * ``None``: Don't learn anything during fit. Then during reverse transform,
+                  don't create any missing values.
+
     """
 
     IS_GENERATOR = True
     INPUT_SDTYPE = 'pii'
 
     @staticmethod
     def check_provider_function(provider_name, function_name):
@@ -81,15 +89,15 @@
                 f"Locales {missed_locales} do not support provider '{self.provider_name}' "
                 f"and function '{self.function_name}'.\nIn place of these locales, 'en_US' will "
                 'be used instead. Please refer to the localized provider docs for more '
                 'information: https://faker.readthedocs.io/en/master/locales.html'
             )
 
     def __init__(self, provider_name=None, function_name=None, function_kwargs=None,
-                 locales=None, enforce_uniqueness=False):
+                 locales=None, enforce_uniqueness=False, missing_value_generation='random'):
         super().__init__()
         self.data_length = None
         self.enforce_uniqueness = enforce_uniqueness
         self.provider_name = provider_name if provider_name else 'BaseProvider'
         if self.provider_name != 'BaseProvider' and function_name is None:
             raise TransformerInputError(
                 'Please specify the function name to use from the '
@@ -103,14 +111,23 @@
 
         self._faker_random_seed = None
         self.locales = locales
         self.faker = faker.Faker(self.locales)
         if self.locales:
             self._check_locales()
 
+        if missing_value_generation not in ['random', None]:
+            raise TransformerInputError(
+                f"Missing value generation '{missing_value_generation}' is not supported "
+                "for AnonymizedFaker. Please use either 'random' or None."
+            )
+
+        self.missing_value_generation = missing_value_generation
+        self._nan_frequency = 0.0
+
     def reset_randomization(self):
         """Create a new ``Faker`` instance."""
         super().reset_randomization()
         self.faker = faker.Faker(self.locales)
         self.faker.seed_instance(self._faker_random_seed)
 
     def _function(self):
@@ -134,14 +151,16 @@
 
         Args:
             data (pandas.Series):
                 Data to fit to.
         """
         self._set_faker_seed(data)
         self.data_length = len(data)
+        if self.missing_value_generation == 'random':
+            self._nan_frequency = data.isna().sum() / len(data)
 
     def _transform(self, _data):
         """Drop the input column by returning ``None``."""
         return None
 
     def _reverse_transform(self, data):
         """Generate new anonymized data using a ``faker.provider.function``.
@@ -166,14 +185,19 @@
         except faker.exceptions.UniquenessException as exception:
             raise TransformerProcessingError(
                 f'The Faker function you specified is not able to generate {sample_size} unique '
                 'values. Please use a different Faker function for column '
                 f"('{self.get_input_column()}')."
             ) from exception
 
+        if self.missing_value_generation == 'random':
+            num_nans = int(self._nan_frequency * sample_size)
+            nan_indices = np.random.choice(sample_size, num_nans, replace=False)
+            reverse_transformed[nan_indices] = np.nan
+
         return reverse_transformed
 
     def __repr__(self):
         """Represent initialization of transformer as text.
 
         Returns:
             str:
```

### Comparing `rdt-1.5.1.dev1/rdt/transformers/pii/utils.py` & `rdt-1.6.0.dev0/rdt/transformers/pii/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/transformers/text.py` & `rdt-1.6.0.dev0/rdt/transformers/text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt/transformers/utils.py` & `rdt-1.6.0.dev0/rdt/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt.egg-info/PKG-INFO` & `rdt-1.6.0.dev0/rdt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdt
-Version: 1.5.1.dev1
+Version: 1.6.0.dev0
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rdt Version: 1.5.1.dev1 Summary: Reversible Data
+Metadata-Version: 2.1 Name: rdt Version: 1.6.0.dev0 Summary: Reversible Data
 Transforms Home-page: https://github.com/sdv-dev/RDT Author: DataCebo, Inc.
 Author-email: info@sdv.dev License: BSL-1.1 Keywords: rdt Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `rdt-1.5.1.dev1/rdt.egg-info/SOURCES.txt` & `rdt-1.6.0.dev0/rdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/rdt.egg-info/requires.txt` & `rdt-1.6.0.dev0/rdt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/setup.cfg` & `rdt-1.6.0.dev0/setup.cfg`

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

### Comparing `rdt-1.5.1.dev1/setup.py` & `rdt-1.6.0.dev0/setup.py`

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

### Comparing `rdt-1.5.1.dev1/tests/__init__.py` & `rdt-1.6.0.dev0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/code_style.py` & `rdt-1.6.0.dev0/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/contributing.py` & `rdt-1.6.0.dev0/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/datasets/tests/test_boolean.py` & `rdt-1.6.0.dev0/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/datasets/tests/test_categorical.py` & `rdt-1.6.0.dev0/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/datasets/tests/test_datetime.py` & `rdt-1.6.0.dev0/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/datasets/tests/test_numerical.py` & `rdt-1.6.0.dev0/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/datasets/tests/test_utils.py` & `rdt-1.6.0.dev0/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/integration/test_hyper_transformer.py` & `rdt-1.6.0.dev0/tests/integration/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/integration/test_transformers.py` & `rdt-1.6.0.dev0/tests/integration/test_transformers.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/integration/transformers/pii/test_anonymizer.py` & `rdt-1.6.0.dev0/tests/integration/transformers/pii/test_anonymizer.py`

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

### Comparing `rdt-1.5.1.dev1/tests/integration/transformers/test_base.py` & `rdt-1.6.0.dev0/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/integration/transformers/test_boolean.py` & `rdt-1.6.0.dev0/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/integration/transformers/test_categorical.py` & `rdt-1.6.0.dev0/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/integration/transformers/test_datetime.py` & `rdt-1.6.0.dev0/tests/integration/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/integration/transformers/test_numerical.py` & `rdt-1.6.0.dev0/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/integration/transformers/test_text.py` & `rdt-1.6.0.dev0/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/performance/test_performance.py` & `rdt-1.6.0.dev0/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/performance/tests/test_profiling.py` & `rdt-1.6.0.dev0/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/unit/test___init__.py` & `rdt-1.6.0.dev0/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/unit/test_hyper_transformer.py` & `rdt-1.6.0.dev0/tests/unit/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/unit/transformers/addons/identity/test_identity.py` & `rdt-1.6.0.dev0/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/unit/transformers/pii/test_anonymizer.py` & `rdt-1.6.0.dev0/tests/unit/transformers/pii/test_anonymizer.py`

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

### Comparing `rdt-1.5.1.dev1/tests/unit/transformers/pii/test_utils.py` & `rdt-1.6.0.dev0/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/unit/transformers/test___init__.py` & `rdt-1.6.0.dev0/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/unit/transformers/test_base.py` & `rdt-1.6.0.dev0/tests/unit/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/unit/transformers/test_boolean.py` & `rdt-1.6.0.dev0/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/unit/transformers/test_categorical.py` & `rdt-1.6.0.dev0/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/unit/transformers/test_datetime.py` & `rdt-1.6.0.dev0/tests/unit/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/unit/transformers/test_null.py` & `rdt-1.6.0.dev0/tests/unit/transformers/test_null.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/unit/transformers/test_numerical.py` & `rdt-1.6.0.dev0/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/unit/transformers/test_text.py` & `rdt-1.6.0.dev0/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.5.1.dev1/tests/unit/transformers/test_utils.py` & `rdt-1.6.0.dev0/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*


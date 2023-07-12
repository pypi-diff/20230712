# Comparing `tmp/abqpy2017-0.0.1.tar.gz` & `tmp/abqpy2017-2017.5.4.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abqpy2017-0.0.1.tar", last modified: Wed Jul 12 04:43:07 2023, max compression
+gzip compressed data, was "abqpy2017-2017.5.4.post2.tar", last modified: Wed Jul 12 11:48:43 2023, max compression
```

## Comparing `abqpy2017-0.0.1.tar` & `abqpy2017-2017.5.4.post2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:43:07.717397 abqpy2017-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-12 04:43:07.717397 abqpy2017-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 04:42:55.000000 abqpy2017-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:43:07.717397 abqpy2017-0.0.1/abqpy2017.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-12 04:43:07.000000 abqpy2017-0.0.1/abqpy2017.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-12 04:43:07.000000 abqpy2017-0.0.1/abqpy2017.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 04:43:07.000000 abqpy2017-0.0.1/abqpy2017.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 04:43:07.000000 abqpy2017-0.0.1/abqpy2017.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 04:43:07.000000 abqpy2017-0.0.1/abqpy2017.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-12 04:42:55.000000 abqpy2017-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 04:43:07.717397 abqpy2017-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:48:43.787962 abqpy2017-2017.5.4.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-12 11:48:43.787962 abqpy2017-2017.5.4.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 11:48:29.000000 abqpy2017-2017.5.4.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 11:48:43.787962 abqpy2017-2017.5.4.post2/abqpy2017.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-12 11:48:43.000000 abqpy2017-2017.5.4.post2/abqpy2017.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-12 11:48:43.000000 abqpy2017-2017.5.4.post2/abqpy2017.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:48:43.000000 abqpy2017-2017.5.4.post2/abqpy2017.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 11:48:43.000000 abqpy2017-2017.5.4.post2/abqpy2017.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 11:48:43.000000 abqpy2017-2017.5.4.post2/abqpy2017.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-12 11:48:29.000000 abqpy2017-2017.5.4.post2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 11:48:43.787962 abqpy2017-2017.5.4.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-12 11:48:29.000000 abqpy2017-2017.5.4.post2/setup.py
```


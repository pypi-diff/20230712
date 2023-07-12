# Comparing `tmp/hmatrices-0.1.0.tar.gz` & `tmp/hmatrices-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmatrices-0.1.0.tar", max compression
+gzip compressed data, was "hmatrices-0.1.1.tar", max compression
```

## Comparing `hmatrices-0.1.0.tar` & `hmatrices-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-11 21:12:28.452092 hmatrices-0.1.0/README.md
--rw-r--r--   0        0        0      146 2023-07-11 21:25:37.772360 hmatrices-0.1.0/hmatrices/__init__.py
--rw-r--r--   0        0        0      294 2023-07-11 21:14:24.282925 hmatrices-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 hmatrices-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      397 2023-07-12 11:24:03.914458 hmatrices-0.1.1/README.md
+-rw-r--r--   0        0        0      403 2023-07-12 13:31:48.729920 hmatrices-0.1.1/hmatrices/__init__.py
+-rw-r--r--   0        0        0      294 2023-07-12 13:42:00.566896 hmatrices-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 hmatrices-0.1.1/PKG-INFO
```


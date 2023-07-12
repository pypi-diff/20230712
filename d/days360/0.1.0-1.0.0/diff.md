# Comparing `tmp/days360-0.1.0.tar.gz` & `tmp/days360-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "days360-0.1.0.tar", max compression
+gzip compressed data, was "days360-1.0.0.tar", max compression
```

## Comparing `days360-0.1.0.tar` & `days360-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      350 2023-07-12 15:56:01.310513 days360-0.1.0/README.md
--rw-r--r--   0        0        0      159 2023-07-12 15:25:38.141249 days360-0.1.0/days360/__init__.py
--rw-r--r--   0        0        0     3275 2023-07-12 15:56:06.796621 days360-0.1.0/days360/days360.py
--rw-r--r--   0        0        0      435 2023-07-12 15:56:07.853812 days360-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 days360-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-12 16:46:32.936705 days360-1.0.0/Readme.md
+-rw-r--r--   0        0        0      159 2023-07-12 15:25:38.141249 days360-1.0.0/days360/__init__.py
+-rw-r--r--   0        0        0     3275 2023-07-12 16:10:03.393954 days360-1.0.0/days360/days360.py
+-rw-r--r--   0        0        0        0 2023-07-12 16:46:31.405282 days360-1.0.0/days360/py.typed
+-rw-r--r--   0        0        0      435 2023-07-12 16:47:37.195393 days360-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 days360-1.0.0/PKG-INFO
```

### Comparing `days360-0.1.0/days360/days360.py` & `days360-1.0.0/days360/days360.py`

 * *Files identical despite different names*


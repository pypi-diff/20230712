# Comparing `tmp/upyog-0.7.3.tar.gz` & `tmp/upyog-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upyog-0.7.3.tar", last modified: Wed Jul  5 17:45:31 2023, max compression
+gzip compressed data, was "upyog-0.7.4.tar", last modified: Wed Jul 12 15:49:35 2023, max compression
```

## Comparing `upyog-0.7.3.tar` & `upyog-0.7.4.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.046680 upyog-0.7.3/
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3549 2023-07-05 17:45:00.000000 upyog-0.7.3/CHANGELOG.md
--rw-r--r--   0 rahulsomani   (501) staff       (20)      133 2022-01-27 18:07:46.000000 upyog-0.7.3/MANIFEST.in
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-07-05 17:45:31.046813 upyog-0.7.3/PKG-INFO
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)      618 2022-01-15 04:03:41.000000 upyog-0.7.3/README.md
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.036974 upyog-0.7.3/assets/
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.038521 upyog-0.7.3/assets/fonts/
--rw-rwxrwx   0 rahulsomani   (501) staff       (20)    28432 2022-01-27 13:15:35.000000 upyog-0.7.3/assets/fonts/EuroStyleNormal.ttf
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)     1399 2023-07-05 17:45:31.047271 upyog-0.7.3/setup.cfg
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)      251 2022-01-17 09:53:10.000000 upyog-0.7.3/setup.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.040025 upyog-0.7.3/upyog/
--rwxr-xr-x   0 rahulsomani   (501) staff       (20)       28 2022-10-28 02:44:32.000000 upyog-0.7.3/upyog/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      644 2023-01-24 04:50:27.000000 upyog-0.7.3/upyog/all.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.041749 upyog-0.7.3/upyog/ann/
--rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2022-01-22 05:11:22.000000 upyog-0.7.3/upyog/ann/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     4426 2022-01-22 20:02:13.000000 upyog-0.7.3/upyog/ann/annoy.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3066 2023-04-16 03:50:08.000000 upyog-0.7.3/upyog/cli.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.043133 upyog-0.7.3/upyog/image/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      141 2022-09-04 09:39:14.000000 upyog-0.7.3/upyog/image/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3340 2023-04-21 18:57:17.000000 upyog-0.7.3/upyog/image/cli.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2286 2022-09-01 09:27:43.000000 upyog-0.7.3/upyog/image/composition.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)    17235 2023-05-23 10:33:14.000000 upyog-0.7.3/upyog/image/draw.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1526 2023-04-15 11:13:07.000000 upyog-0.7.3/upyog/image/io.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1442 2023-02-28 09:04:05.000000 upyog-0.7.3/upyog/image/pil_operators.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1518 2023-05-17 11:01:32.000000 upyog-0.7.3/upyog/image/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     7939 2023-02-28 09:16:20.000000 upyog-0.7.3/upyog/image/visualiser.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1306 2023-05-17 15:42:19.000000 upyog-0.7.3/upyog/imports.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.044598 upyog-0.7.3/upyog/ml/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      211 2023-05-17 15:36:44.000000 upyog-0.7.3/upyog/ml/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2799 2023-06-21 20:09:18.000000 upyog-0.7.3/upyog/ml/coreml_utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1803 2023-05-25 07:42:54.000000 upyog-0.7.3/upyog/ml/eval_dataset.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      523 2023-05-25 07:42:28.000000 upyog-0.7.3/upyog/ml/imports.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3662 2023-05-17 16:21:13.000000 upyog-0.7.3/upyog/ml/model_utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1707 2023-05-17 11:41:09.000000 upyog-0.7.3/upyog/ml/preprocessing.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2373 2023-06-25 04:18:02.000000 upyog-0.7.3/upyog/ml/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2321 2023-06-25 04:00:34.000000 upyog-0.7.3/upyog/ml/visualise.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1198 2022-06-01 05:03:09.000000 upyog-0.7.3/upyog/nb2script.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.045358 upyog-0.7.3/upyog/os/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      137 2022-10-26 00:24:39.000000 upyog-0.7.3/upyog/os/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     6159 2023-04-16 07:09:32.000000 upyog-0.7.3/upyog/os/cli.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-08-03 15:10:12.000000 upyog-0.7.3/upyog/os/patch_pathlib.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     4424 2023-05-25 07:33:09.000000 upyog-0.7.3/upyog/os/read_files.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     3459 2023-05-17 10:58:12.000000 upyog-0.7.3/upyog/os/utils.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.046498 upyog-0.7.3/upyog/utils/
--rw-r--r--   0 rahulsomani   (501) staff       (20)      144 2023-06-21 15:08:49.000000 upyog-0.7.3/upyog/utils/__init__.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-04-05 12:59:08.000000 upyog-0.7.3/upyog/utils/boxes.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1483 2023-06-21 18:28:22.000000 upyog-0.7.3/upyog/utils/date_utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)    14495 2023-01-11 07:05:00.000000 upyog-0.7.3/upyog/utils/download.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1324 2023-01-12 17:22:00.000000 upyog-0.7.3/upyog/utils/prettify_df.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)     2636 2023-06-21 15:10:08.000000 upyog-0.7.3/upyog/utils/utils.py
--rw-r--r--   0 rahulsomani   (501) staff       (20)      556 2022-08-08 14:04:02.000000 upyog-0.7.3/upyog/utils/zip_utils.py
-drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-05 17:45:31.041447 upyog-0.7.3/upyog.egg-info/
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-07-05 17:45:30.000000 upyog-0.7.3/upyog.egg-info/PKG-INFO
--rw-r--r--   0 rahulsomani   (501) staff       (20)     1048 2023-07-05 17:45:31.000000 upyog-0.7.3/upyog.egg-info/SOURCES.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2023-07-05 17:45:30.000000 upyog-0.7.3/upyog.egg-info/dependency_links.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)      454 2023-07-05 17:45:30.000000 upyog-0.7.3/upyog.egg-info/entry_points.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2022-01-17 09:58:14.000000 upyog-0.7.3/upyog.egg-info/not-zip-safe
--rw-r--r--   0 rahulsomani   (501) staff       (20)      192 2023-07-05 17:45:30.000000 upyog-0.7.3/upyog.egg-info/requires.txt
--rw-r--r--   0 rahulsomani   (501) staff       (20)       12 2023-07-05 17:45:30.000000 upyog-0.7.3/upyog.egg-info/top_level.txt
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-12 15:49:35.333026 upyog-0.7.4/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3614 2023-07-12 15:49:24.000000 upyog-0.7.4/CHANGELOG.md
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      159 2023-07-12 15:48:21.000000 upyog-0.7.4/MANIFEST.in
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-07-12 15:49:35.333117 upyog-0.7.4/PKG-INFO
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)      618 2022-01-15 04:03:41.000000 upyog-0.7.4/README.md
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-12 15:49:35.324180 upyog-0.7.4/assets/
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-12 15:49:35.325620 upyog-0.7.4/assets/fonts/
+-rw-rwxrwx   0 rahulsomani   (501) staff       (20)    28432 2022-01-27 13:15:35.000000 upyog-0.7.4/assets/fonts/EuroStyleNormal.ttf
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)     1399 2023-07-12 15:49:35.333540 upyog-0.7.4/setup.cfg
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)      251 2022-01-17 09:53:10.000000 upyog-0.7.4/setup.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-12 15:49:35.326691 upyog-0.7.4/upyog/
+-rwxr-xr-x   0 rahulsomani   (501) staff       (20)       28 2022-10-28 02:44:32.000000 upyog-0.7.4/upyog/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      644 2023-01-24 04:50:27.000000 upyog-0.7.4/upyog/all.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-12 15:49:35.328375 upyog-0.7.4/upyog/ann/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        0 2022-01-22 05:11:22.000000 upyog-0.7.4/upyog/ann/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     4426 2022-01-22 20:02:13.000000 upyog-0.7.4/upyog/ann/annoy.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3066 2023-04-16 03:50:08.000000 upyog-0.7.4/upyog/cli.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-12 15:49:35.329860 upyog-0.7.4/upyog/image/
+-rw-rw-r--   0 rahulsomani   (501) staff       (20)   310420 2020-01-23 18:30:00.000000 upyog-0.7.4/upyog/image/_Inter-Light.ttf
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      141 2022-09-04 09:39:14.000000 upyog-0.7.4/upyog/image/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3340 2023-04-21 18:57:17.000000 upyog-0.7.4/upyog/image/cli.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2286 2022-09-01 09:27:43.000000 upyog-0.7.4/upyog/image/composition.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)    17235 2023-05-23 10:33:14.000000 upyog-0.7.4/upyog/image/draw.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1526 2023-07-06 15:00:39.000000 upyog-0.7.4/upyog/image/io.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1442 2023-02-28 09:04:05.000000 upyog-0.7.4/upyog/image/pil_operators.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1518 2023-05-17 11:01:32.000000 upyog-0.7.4/upyog/image/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     7939 2023-02-28 09:16:20.000000 upyog-0.7.4/upyog/image/visualiser.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1306 2023-05-17 15:42:19.000000 upyog-0.7.4/upyog/imports.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-12 15:49:35.331015 upyog-0.7.4/upyog/ml/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      211 2023-05-17 15:36:44.000000 upyog-0.7.4/upyog/ml/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2799 2023-06-21 20:09:18.000000 upyog-0.7.4/upyog/ml/coreml_utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1803 2023-05-25 07:42:54.000000 upyog-0.7.4/upyog/ml/eval_dataset.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      523 2023-05-25 07:42:28.000000 upyog-0.7.4/upyog/ml/imports.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3662 2023-05-17 16:21:13.000000 upyog-0.7.4/upyog/ml/model_utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1707 2023-05-17 11:41:09.000000 upyog-0.7.4/upyog/ml/preprocessing.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2373 2023-06-25 04:18:02.000000 upyog-0.7.4/upyog/ml/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2321 2023-06-25 04:00:34.000000 upyog-0.7.4/upyog/ml/visualise.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1198 2022-06-01 05:03:09.000000 upyog-0.7.4/upyog/nb2script.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-12 15:49:35.331752 upyog-0.7.4/upyog/os/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      137 2022-10-26 00:24:39.000000 upyog-0.7.4/upyog/os/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     6159 2023-04-16 07:09:32.000000 upyog-0.7.4/upyog/os/cli.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-08-03 15:10:12.000000 upyog-0.7.4/upyog/os/patch_pathlib.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     4424 2023-05-25 07:33:09.000000 upyog-0.7.4/upyog/os/read_files.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     3459 2023-05-17 10:58:12.000000 upyog-0.7.4/upyog/os/utils.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-12 15:49:35.332895 upyog-0.7.4/upyog/utils/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      144 2023-06-21 15:08:49.000000 upyog-0.7.4/upyog/utils/__init__.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      426 2022-04-05 12:59:08.000000 upyog-0.7.4/upyog/utils/boxes.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1483 2023-06-21 18:28:22.000000 upyog-0.7.4/upyog/utils/date_utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)    14495 2023-01-11 07:05:00.000000 upyog-0.7.4/upyog/utils/download.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1324 2023-01-12 17:22:00.000000 upyog-0.7.4/upyog/utils/prettify_df.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     2636 2023-06-21 15:10:08.000000 upyog-0.7.4/upyog/utils/utils.py
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      556 2022-08-08 14:04:02.000000 upyog-0.7.4/upyog/utils/zip_utils.py
+drwxr-xr-x   0 rahulsomani   (501) staff       (20)        0 2023-07-12 15:49:35.328091 upyog-0.7.4/upyog.egg-info/
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1115 2023-07-12 15:49:35.000000 upyog-0.7.4/upyog.egg-info/PKG-INFO
+-rw-r--r--   0 rahulsomani   (501) staff       (20)     1077 2023-07-12 15:49:35.000000 upyog-0.7.4/upyog.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2023-07-12 15:49:35.000000 upyog-0.7.4/upyog.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      454 2023-07-12 15:49:35.000000 upyog-0.7.4/upyog.egg-info/entry_points.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)        1 2022-01-17 09:58:14.000000 upyog-0.7.4/upyog.egg-info/not-zip-safe
+-rw-r--r--   0 rahulsomani   (501) staff       (20)      192 2023-07-12 15:49:35.000000 upyog-0.7.4/upyog.egg-info/requires.txt
+-rw-r--r--   0 rahulsomani   (501) staff       (20)       12 2023-07-12 15:49:35.000000 upyog-0.7.4/upyog.egg-info/top_level.txt
```

### Comparing `upyog-0.7.3/CHANGELOG.md` & `upyog-0.7.4/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+## 0.7.4 -- 12 Jul 2023
+* Include font distributed with package
+
 ## 0.7.3 -- 5 July 2023
 * Minor changes
 * Update dependency
 
 ## 0.7.2 -- 25 May 2023
 * Font path bugfix...
 * Port over more ML utilities to `upyog.ml`
```

### Comparing `upyog-0.7.3/PKG-INFO` & `upyog-0.7.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upyog
-Version: 0.7.3
+Version: 0.7.4
 Summary: Myriad Utilities
 Author: Rahul Somani
 Author-email: rsomani95@gmail.com
 License: MIT
 Keywords: utilities
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `upyog-0.7.3/README.md` & `upyog-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/assets/fonts/EuroStyleNormal.ttf` & `upyog-0.7.4/assets/fonts/EuroStyleNormal.ttf`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/setup.cfg` & `upyog-0.7.4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = upyog
-version = 0.7.3
+version = 0.7.4
 author = Rahul Somani
 author_email = rsomani95@gmail.com
 description = Myriad Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = utilities
 license = MIT
```

### Comparing `upyog-0.7.3/upyog/all.py` & `upyog-0.7.4/upyog/all.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/ann/annoy.py` & `upyog-0.7.4/upyog/ann/annoy.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/cli.py` & `upyog-0.7.4/upyog/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/image/cli.py` & `upyog-0.7.4/upyog/image/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/image/composition.py` & `upyog-0.7.4/upyog/image/composition.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/image/draw.py` & `upyog-0.7.4/upyog/image/draw.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/image/io.py` & `upyog-0.7.4/upyog/image/io.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/image/pil_operators.py` & `upyog-0.7.4/upyog/image/pil_operators.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/image/utils.py` & `upyog-0.7.4/upyog/image/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/image/visualiser.py` & `upyog-0.7.4/upyog/image/visualiser.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/imports.py` & `upyog-0.7.4/upyog/imports.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/ml/coreml_utils.py` & `upyog-0.7.4/upyog/ml/coreml_utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/ml/eval_dataset.py` & `upyog-0.7.4/upyog/ml/eval_dataset.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/ml/imports.py` & `upyog-0.7.4/upyog/ml/imports.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/ml/model_utils.py` & `upyog-0.7.4/upyog/ml/model_utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/ml/preprocessing.py` & `upyog-0.7.4/upyog/ml/preprocessing.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/ml/utils.py` & `upyog-0.7.4/upyog/ml/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/ml/visualise.py` & `upyog-0.7.4/upyog/ml/visualise.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/nb2script.py` & `upyog-0.7.4/upyog/nb2script.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/os/cli.py` & `upyog-0.7.4/upyog/os/cli.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/os/read_files.py` & `upyog-0.7.4/upyog/os/read_files.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/os/utils.py` & `upyog-0.7.4/upyog/os/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/utils/date_utils.py` & `upyog-0.7.4/upyog/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/utils/download.py` & `upyog-0.7.4/upyog/utils/download.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/utils/prettify_df.py` & `upyog-0.7.4/upyog/utils/prettify_df.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/utils/utils.py` & `upyog-0.7.4/upyog/utils/utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog/utils/zip_utils.py` & `upyog-0.7.4/upyog/utils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `upyog-0.7.3/upyog.egg-info/PKG-INFO` & `upyog-0.7.4/upyog.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upyog
-Version: 0.7.3
+Version: 0.7.4
 Summary: Myriad Utilities
 Author: Rahul Somani
 Author-email: rsomani95@gmail.com
 License: MIT
 Keywords: utilities
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
```

### Comparing `upyog-0.7.3/upyog.egg-info/SOURCES.txt` & `upyog-0.7.4/upyog.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 upyog.egg-info/dependency_links.txt
 upyog.egg-info/entry_points.txt
 upyog.egg-info/not-zip-safe
 upyog.egg-info/requires.txt
 upyog.egg-info/top_level.txt
 upyog/ann/__init__.py
 upyog/ann/annoy.py
+upyog/image/_Inter-Light.ttf
 upyog/image/__init__.py
 upyog/image/cli.py
 upyog/image/composition.py
 upyog/image/draw.py
 upyog/image/io.py
 upyog/image/pil_operators.py
 upyog/image/utils.py
```


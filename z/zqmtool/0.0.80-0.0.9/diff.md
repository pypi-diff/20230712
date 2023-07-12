# Comparing `tmp/zqmtool-0.0.80.tar.gz` & `tmp/zqmtool-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zqmtool-0.0.80.tar", last modified: Wed Jul 12 07:26:00 2023, max compression
+gzip compressed data, was "zqmtool-0.0.9.tar", last modified: Wed Sep  7 20:47:33 2022, max compression
```

## Comparing `zqmtool-0.0.80.tar` & `zqmtool-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,20 @@
-drwxr-xr-x   0 zouqiming   (501) staff       (20)        0 2023-07-12 07:26:00.635176 zqmtool-0.0.80/
--rw-r--r--   0 zouqiming   (501) staff       (20)     1053 2023-07-12 07:25:10.000000 zqmtool-0.0.80/LICENSE
--rw-r--r--   0 zouqiming   (501) staff       (20)      266 2023-07-12 07:26:00.635026 zqmtool-0.0.80/PKG-INFO
--rw-r--r--   0 zouqiming   (501) staff       (20)      132 2023-07-12 07:25:10.000000 zqmtool-0.0.80/README.md
--rw-r--r--   0 zouqiming   (501) staff       (20)       38 2023-07-12 07:26:00.635220 zqmtool-0.0.80/setup.cfg
--rw-r--r--   0 zouqiming   (501) staff       (20)      338 2023-07-12 07:25:35.000000 zqmtool-0.0.80/setup.py
-drwxr-xr-x   0 zouqiming   (501) staff       (20)        0 2023-07-12 07:26:00.633237 zqmtool-0.0.80/zqmtool/
--rw-r--r--   0 zouqiming   (501) staff       (20)        0 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/__init__.py
--rw-r--r--   0 zouqiming   (501) staff       (20)    10171 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/get_foreground_mask.py
-drwxr-xr-x   0 zouqiming   (501) staff       (20)        0 2023-07-12 07:26:00.634113 zqmtool-0.0.80/zqmtool/gymEnvs/
--rw-r--r--   0 zouqiming   (501) staff       (20)        0 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/gymEnvs/__init__.py
--rw-r--r--   0 zouqiming   (501) staff       (20)     9992 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/gymEnvs/maze.py
--rw-r--r--   0 zouqiming   (501) staff       (20)     8750 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/gymEnvs/mnist_maze.py
--rw-r--r--   0 zouqiming   (501) staff       (20)    12986 2023-07-08 09:20:40.000000 zqmtool-0.0.80/zqmtool/image.py
-drwxr-xr-x   0 zouqiming   (501) staff       (20)        0 2023-07-12 07:26:00.634264 zqmtool-0.0.80/zqmtool/lib/
--rw-r--r--   0 zouqiming   (501) staff       (20)        0 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/lib/__init__.py
--rw-r--r--   0 zouqiming   (501) staff       (20)    10322 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/multi_view_stereo.py
--rw-r--r--   0 zouqiming   (501) staff       (20)     5334 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/other.py
--rw-r--r--   0 zouqiming   (501) staff       (20)      207 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/point.py
-drwxr-xr-x   0 zouqiming   (501) staff       (20)        0 2023-07-12 07:26:00.634869 zqmtool-0.0.80/zqmtool/rl/
--rw-r--r--   0 zouqiming   (501) staff       (20)        0 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/rl/__init__.py
--rw-r--r--   0 zouqiming   (501) staff       (20)    14840 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/rl/collector.py
--rw-r--r--   0 zouqiming   (501) staff       (20)     8958 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/rl/offpolicy.py
--rw-r--r--   0 zouqiming   (501) staff       (20)     3091 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/rl/policy.py
--rw-r--r--   0 zouqiming   (501) staff       (20)     8727 2023-04-27 10:17:55.000000 zqmtool-0.0.80/zqmtool/rl/trajectory.py
--rw-r--r--   0 zouqiming   (501) staff       (20)    19213 2023-07-05 12:16:28.000000 zqmtool-0.0.80/zqmtool/ssl.py
-drwxr-xr-x   0 zouqiming   (501) staff       (20)        0 2023-07-12 07:26:00.633759 zqmtool-0.0.80/zqmtool.egg-info/
--rw-r--r--   0 zouqiming   (501) staff       (20)      266 2023-07-12 07:26:00.000000 zqmtool-0.0.80/zqmtool.egg-info/PKG-INFO
--rw-r--r--   0 zouqiming   (501) staff       (20)      519 2023-07-12 07:26:00.000000 zqmtool-0.0.80/zqmtool.egg-info/SOURCES.txt
--rw-r--r--   0 zouqiming   (501) staff       (20)        1 2023-07-12 07:26:00.000000 zqmtool-0.0.80/zqmtool.egg-info/dependency_links.txt
--rw-r--r--   0 zouqiming   (501) staff       (20)        8 2023-07-12 07:26:00.000000 zqmtool-0.0.80/zqmtool.egg-info/top_level.txt
+drwxr-xr-x   0 johnson    (501) staff       (20)        0 2022-09-07 20:47:33.383723 zqmtool-0.0.9/
+-rw-r--r--   0 johnson    (501) staff       (20)     1063 2022-09-07 14:20:31.000000 zqmtool-0.0.9/LICENSE
+-rw-r--r--   0 johnson    (501) staff       (20)      239 2022-09-07 20:47:33.383339 zqmtool-0.0.9/PKG-INFO
+-rw-r--r--   0 johnson    (501) staff       (20)       20 2022-09-07 14:16:12.000000 zqmtool-0.0.9/README.md
+-rw-r--r--   0 johnson    (501) staff       (20)       84 2022-09-07 14:22:19.000000 zqmtool-0.0.9/pyproject.toml
+-rw-r--r--   0 johnson    (501) staff       (20)       38 2022-09-07 20:47:33.383884 zqmtool-0.0.9/setup.cfg
+-rw-r--r--   0 johnson    (501) staff       (20)      520 2022-09-07 20:45:25.000000 zqmtool-0.0.9/setup.py
+drwxr-xr-x   0 johnson    (501) staff       (20)        0 2022-09-07 20:47:33.372904 zqmtool-0.0.9/src_armed/
+drwxr-xr-x   0 johnson    (501) staff       (20)        0 2022-09-07 20:47:33.379861 zqmtool-0.0.9/src_armed/zqmtool/
+-rw-r--r--   0 johnson    (501) staff       (20)     1170 2022-09-07 20:44:50.000000 zqmtool-0.0.9/src_armed/zqmtool/__init__.py
+-rw-r--r--   0 johnson    (501) staff       (20)     4353 2022-09-07 20:44:50.000000 zqmtool-0.0.9/src_armed/zqmtool/file.py
+-rw-r--r--   0 johnson    (501) staff       (20)     9557 2022-09-07 20:44:50.000000 zqmtool-0.0.9/src_armed/zqmtool/image.py
+-rw-r--r--   0 johnson    (501) staff       (20)     2645 2022-09-07 20:44:50.000000 zqmtool-0.0.9/src_armed/zqmtool/point.py
+drwxr-xr-x   0 johnson    (501) staff       (20)        0 2022-09-07 20:47:33.382334 zqmtool-0.0.9/src_armed/zqmtool/pytransform/
+-rw-r--r--   0 johnson    (501) staff       (20)    13587 2022-09-07 16:41:16.000000 zqmtool-0.0.9/src_armed/zqmtool/pytransform/__init__.py
+drwxr-xr-x   0 johnson    (501) staff       (20)        0 2022-09-07 20:47:33.381793 zqmtool-0.0.9/src_armed/zqmtool.egg-info/
+-rw-r--r--   0 johnson    (501) staff       (20)      239 2022-09-07 20:47:33.000000 zqmtool-0.0.9/src_armed/zqmtool.egg-info/PKG-INFO
+-rw-r--r--   0 johnson    (501) staff       (20)      357 2022-09-07 20:47:33.000000 zqmtool-0.0.9/src_armed/zqmtool.egg-info/SOURCES.txt
+-rw-r--r--   0 johnson    (501) staff       (20)        1 2022-09-07 20:47:33.000000 zqmtool-0.0.9/src_armed/zqmtool.egg-info/dependency_links.txt
+-rw-r--r--   0 johnson    (501) staff       (20)        8 2022-09-07 20:47:33.000000 zqmtool-0.0.9/src_armed/zqmtool.egg-info/top_level.txt
```

### Comparing `zqmtool-0.0.80/LICENSE` & `zqmtool-0.0.9/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,21 @@
-Copyright <2022> <ZOU QIMING>
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Copyright (c) 2022 LZC6244
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```


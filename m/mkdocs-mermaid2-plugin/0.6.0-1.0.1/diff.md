# Comparing `tmp/mkdocs-mermaid2-plugin-0.6.0.tar.gz` & `tmp/mkdocs-mermaid2-plugin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-mermaid2-plugin-0.6.0.tar", last modified: Wed Apr 20 06:45:50 2022, max compression
+gzip compressed data, was "mkdocs-mermaid2-plugin-1.0.1.tar", last modified: Wed Jul 12 11:13:43 2023, max compression
```

## Comparing `mkdocs-mermaid2-plugin-0.6.0.tar` & `mkdocs-mermaid2-plugin-1.0.1.tar`

### file list

```diff
@@ -1,48 +1,55 @@
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/.github/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/.github/workflows/
--rw-r--r--   0 laurent    (501) staff       (20)      359 2020-05-29 08:04:22.000000 mkdocs-mermaid2-plugin-0.6.0/.github/workflows/greetings.yml
--rw-r--r--   0 laurent    (501) staff       (20)     1203 2020-05-04 07:28:44.000000 mkdocs-mermaid2-plugin-0.6.0/.gitignore
--rw-r--r--   0 laurent    (501) staff       (20)     1079 2020-05-04 07:28:44.000000 mkdocs-mermaid2-plugin-0.6.0/LICENSE
--rw-r--r--   0 laurent    (501) staff       (20)       36 2020-05-04 07:28:44.000000 mkdocs-mermaid2-plugin-0.6.0/MANIFEST.in
--rw-r--r--   0 laurent    (501) staff       (20)     1052 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/PKG-INFO
--rwxr-xr-x   0 laurent    (501) staff       (20)    22723 2021-08-29 15:21:36.000000 mkdocs-mermaid2-plugin-0.6.0/README.md
--rw-r--r--   0 laurent    (501) staff       (20)    18021 2020-08-20 13:19:58.000000 mkdocs-mermaid2-plugin-0.6.0/error.png
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/mermaid2/
--rwxr-xr-x   0 laurent    (501) staff       (20)      213 2020-08-24 08:41:41.000000 mkdocs-mermaid2-plugin-0.6.0/mermaid2/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)     1735 2020-08-24 10:05:52.000000 mkdocs-mermaid2-plugin-0.6.0/mermaid2/fence.py
--rwxr-xr-x   0 laurent    (501) staff       (20)     8423 2021-08-29 15:24:53.000000 mkdocs-mermaid2-plugin-0.6.0/mermaid2/plugin.py
--rw-r--r--   0 laurent    (501) staff       (20)     3087 2020-09-06 14:18:16.000000 mkdocs-mermaid2-plugin-0.6.0/mermaid2/pyjs.py
--rw-r--r--   0 laurent    (501) staff       (20)     1049 2020-09-06 09:45:38.000000 mkdocs-mermaid2-plugin-0.6.0/mermaid2/util.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/mkdocs_mermaid2_plugin.egg-info/
--rw-r--r--   0 laurent    (501) staff       (20)     1052 2022-04-20 06:45:48.000000 mkdocs-mermaid2-plugin-0.6.0/mkdocs_mermaid2_plugin.egg-info/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)      812 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/mkdocs_mermaid2_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 laurent    (501) staff       (20)        1 2022-04-20 06:45:48.000000 mkdocs-mermaid2-plugin-0.6.0/mkdocs_mermaid2_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 laurent    (501) staff       (20)       67 2022-04-20 06:45:48.000000 mkdocs-mermaid2-plugin-0.6.0/mkdocs_mermaid2_plugin.egg-info/entry_points.txt
--rw-r--r--   0 laurent    (501) staff       (20)      122 2022-04-20 06:45:48.000000 mkdocs-mermaid2-plugin-0.6.0/mkdocs_mermaid2_plugin.egg-info/requires.txt
--rw-r--r--   0 laurent    (501) staff       (20)        9 2022-04-20 06:45:48.000000 mkdocs-mermaid2-plugin-0.6.0/mkdocs_mermaid2_plugin.egg-info/top_level.txt
--rw-r--r--   0 laurent    (501) staff       (20)       38 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/setup.cfg
--rwxr-xr-x   0 laurent    (501) staff       (20)     1778 2021-08-29 15:25:11.000000 mkdocs-mermaid2-plugin-0.6.0/setup.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/test/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/test/medium/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/test/medium/docs/
--rw-r--r--   0 laurent    (501) staff       (20)     1174 2020-09-06 14:32:59.000000 mkdocs-mermaid2-plugin-0.6.0/test/medium/docs/index.md
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/test/medium/docs/js/
--rw-r--r--   0 laurent    (501) staff       (20)      735 2020-08-20 09:48:10.000000 mkdocs-mermaid2-plugin-0.6.0/test/medium/docs/js/extra.js
--rw-r--r--   0 laurent    (501) staff       (20)      181 2020-12-16 12:46:31.000000 mkdocs-mermaid2-plugin-0.6.0/test/medium/docs/second.md
--rw-r--r--   0 laurent    (501) staff       (20)      643 2020-12-16 12:46:47.000000 mkdocs-mermaid2-plugin-0.6.0/test/medium/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/test/simple/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/test/simple/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      302 2020-08-30 15:25:03.000000 mkdocs-mermaid2-plugin-0.6.0/test/simple/docs/index.md
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/test/simple/docs/js/
--rw-r--r--   0 laurent    (501) staff       (20)      735 2020-08-20 09:48:10.000000 mkdocs-mermaid2-plugin-0.6.0/test/simple/docs/js/extra.js
--rw-r--r--   0 laurent    (501) staff       (20)      266 2020-08-30 15:18:45.000000 mkdocs-mermaid2-plugin-0.6.0/test/simple/docs/second.md
--rw-r--r--   0 laurent    (501) staff       (20)      331 2020-09-06 15:02:02.000000 mkdocs-mermaid2-plugin-0.6.0/test/simple/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/test/superfences/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/test/superfences/docs/
--rw-r--r--   0 laurent    (501) staff       (20)     1147 2020-09-06 14:41:13.000000 mkdocs-mermaid2-plugin-0.6.0/test/superfences/docs/index.md
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2022-04-20 06:45:50.000000 mkdocs-mermaid2-plugin-0.6.0/test/superfences/docs/js/
--rw-r--r--   0 laurent    (501) staff       (20)    10474 2020-09-03 17:39:38.000000 mkdocs-mermaid2-plugin-0.6.0/test/superfences/docs/js/loader.js
--rw-r--r--   0 laurent    (501) staff       (20)      423 2020-09-06 15:09:03.000000 mkdocs-mermaid2-plugin-0.6.0/test/superfences/docs/second.md
--rw-r--r--   0 laurent    (501) staff       (20)      872 2020-09-06 14:39:25.000000 mkdocs-mermaid2-plugin-0.6.0/test/superfences/mkdocs.yml
--rwxr-xr-x   0 laurent    (501) staff       (20)     1118 2021-08-29 14:44:14.000000 mkdocs-mermaid2-plugin-0.6.0/update_pypi.sh
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/.github/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/.github/workflows/
+-rw-r--r--   0 laurent    (501) staff       (20)      359 2020-05-29 08:04:22.000000 mkdocs-mermaid2-plugin-1.0.1/.github/workflows/greetings.yml
+-rw-r--r--   0 laurent    (501) staff       (20)     1203 2020-05-04 07:28:44.000000 mkdocs-mermaid2-plugin-1.0.1/.gitignore
+-rw-r--r--   0 laurent    (501) staff       (20)     1079 2020-05-04 07:28:44.000000 mkdocs-mermaid2-plugin-1.0.1/LICENSE
+-rw-r--r--   0 laurent    (501) staff       (20)       36 2020-05-04 07:28:44.000000 mkdocs-mermaid2-plugin-1.0.1/MANIFEST.in
+-rw-r--r--   0 laurent    (501) staff       (20)     1054 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/PKG-INFO
+-rwxr-xr-x   0 laurent    (501) staff       (20)    26900 2023-04-30 12:54:23.000000 mkdocs-mermaid2-plugin-1.0.1/README.md
+-rw-r--r--   0 laurent    (501) staff       (20)    18021 2020-08-20 13:19:58.000000 mkdocs-mermaid2-plugin-1.0.1/error.png
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/mermaid2/
+-rwxr-xr-x   0 laurent    (501) staff       (20)      213 2020-08-24 08:41:41.000000 mkdocs-mermaid2-plugin-1.0.1/mermaid2/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1735 2020-08-24 10:05:52.000000 mkdocs-mermaid2-plugin-1.0.1/mermaid2/fence.py
+-rwxr-xr-x   0 laurent    (501) staff       (20)    10260 2023-04-30 13:13:11.000000 mkdocs-mermaid2-plugin-1.0.1/mermaid2/plugin.py
+-rw-r--r--   0 laurent    (501) staff       (20)     3087 2020-09-06 14:18:16.000000 mkdocs-mermaid2-plugin-1.0.1/mermaid2/pyjs.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1049 2020-09-06 09:45:38.000000 mkdocs-mermaid2-plugin-1.0.1/mermaid2/util.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/
+-rw-r--r--   0 laurent    (501) staff       (20)     1054 2023-07-12 11:13:41.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)      945 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        1 2023-07-12 11:13:41.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       66 2023-07-12 11:13:41.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 laurent    (501) staff       (20)      123 2023-07-12 11:13:41.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/requires.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        9 2023-07-12 11:13:41.000000 mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/top_level.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       38 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/setup.cfg
+-rwxr-xr-x   0 laurent    (501) staff       (20)     1872 2023-07-12 11:13:09.000000 mkdocs-mermaid2-plugin-1.0.1/setup.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/test/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:42.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)     1174 2020-09-06 14:32:59.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/index.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/js/
+-rw-r--r--   0 laurent    (501) staff       (20)      735 2020-08-20 09:48:10.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/js/extra.js
+-rw-r--r--   0 laurent    (501) staff       (20)      181 2020-12-16 12:46:31.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/second.md
+-rw-r--r--   0 laurent    (501) staff       (20)      643 2020-12-16 12:46:47.000000 mkdocs-mermaid2-plugin-1.0.1/test/medium/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      512 2023-04-27 13:33:52.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/docs/index.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/docs/js/
+-rw-r--r--   0 laurent    (501) staff       (20)      735 2020-08-20 09:48:10.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/docs/js/extra.js
+-rw-r--r--   0 laurent    (501) staff       (20)      266 2020-08-30 15:18:45.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/docs/second.md
+-rw-r--r--   0 laurent    (501) staff       (20)      331 2020-09-06 15:02:02.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      302 2023-04-27 12:26:03.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/docs/index.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/docs/js/
+-rw-r--r--   0 laurent    (501) staff       (20)      735 2023-04-27 12:26:03.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/docs/js/extra.js
+-rw-r--r--   0 laurent    (501) staff       (20)      266 2023-04-27 12:26:03.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/docs/second.md
+-rw-r--r--   0 laurent    (501) staff       (20)      353 2023-04-27 12:40:01.000000 mkdocs-mermaid2-plugin-1.0.1/test/simple_pre_10/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)     1147 2020-09-06 14:41:13.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/index.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 11:13:43.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/js/
+-rw-r--r--   0 laurent    (501) staff       (20)    10474 2020-09-03 17:39:38.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/js/loader.js
+-rw-r--r--   0 laurent    (501) staff       (20)      423 2020-09-06 15:09:03.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/second.md
+-rw-r--r--   0 laurent    (501) staff       (20)      872 2020-09-06 14:39:25.000000 mkdocs-mermaid2-plugin-1.0.1/test/superfences/mkdocs.yml
+-rwxr-xr-x   0 laurent    (501) staff       (20)     1118 2021-08-29 14:44:14.000000 mkdocs-mermaid2-plugin-1.0.1/update_pypi.sh
```

### Comparing `mkdocs-mermaid2-plugin-0.6.0/.gitignore` & `mkdocs-mermaid2-plugin-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-0.6.0/LICENSE` & `mkdocs-mermaid2-plugin-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-0.6.0/PKG-INFO` & `mkdocs-mermaid2-plugin-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: mkdocs-mermaid2-plugin
-Version: 0.6.0
+Version: 1.0.1
 Summary: A MkDocs plugin for including mermaid graphs in markdown sources
 Home-page: https://github.com/fralau/mkdocs-mermaid2-plugin
 Author: pugong, Fralau
 Author-email: pugong.liu@gmail.com, fralau2035@yahoo.com
 License: MIT
 Keywords: mkdocs python markdown mermaid
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
+Provides-Extra: test
 License-File: LICENSE
 
 A mkdocs plugin that interprets mermaid graphs in the markdown file.To install, please follow instructions in the readme file.This is a fork of the Pugong Liu's excellent project, which is no longer maintained.
-
```

### Comparing `mkdocs-mermaid2-plugin-0.6.0/README.md` & `mkdocs-mermaid2-plugin-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,145 @@
 # mkdocs-mermaid2-plugin
 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-mermaid2-plugin)](https://pypi.org/project/mkdocs-mermaid2-plugin/)
+![Github](https://img.shields.io/github/v/tag/fralau/mkdocs-mermaid2-plugin?label=github%20tag)
 ![Downloads(PyPI)](https://img.shields.io/pypi/dm/mkdocs-mermaid2-plugin)
 
 
 An [MkDocs](https://www.mkdocs.org/) plugin that renders textual graph
 descriptions into [Mermaid](https://mermaid-js.github.io/mermaid) graphs
 (flow charts, sequence diagrams, pie charts, etc.).
 
 
 
-
-> This is a fork from
-> [Pugong Liu's excellent project](https://github.com/pugong/mkdocs-mermaid-plugin), 
-> which is no longer maintained. It offers expanded documentation as
-> well as new functions.
-
+> As of version 1.0.0, this plugin works with versions of the Mermaid library > 10,
+> **and** with lower versions.
 
 
 <!-- To update the toc, run the following command:
 markdown-toc -i README.md 
 -->
 
 <!-- toc -->
 
-- [mkdocs-mermaid2-plugin](#mkdocs-mermaid2-plugin)
-  - [How it works](#how-it-works)
-  - [Installation](#installation)
-    - [Automatic](#automatic)
-    - [Manual](#manual)
-  - [Configuration](#configuration)
-    - [Basic configuration](#basic-configuration)
-    - [Specifying the version of the Mermaid library](#specifying-the-version-of-the-mermaid-library)
-    - [Explicit declaration of the Mermaid library](#explicit-declaration-of-the-mermaid-library)
-  - [Usage](#usage)
-    - [General Principle](#general-principle)
-    - [How to write Mermaid diagrams](#how-to-write-mermaid-diagrams)
-    - [Adding arguments to the Mermaid engine](#adding-arguments-to-the-mermaid-engine)
-    - [Testing](#testing)
-    - [Adding a Javascript callback function](#adding-a-javascript-callback-function)
-      - [Use Case](#use-case)
-      - [Method](#method)
-  - [Tips and Tricks](#tips-and-tricks)
-    - [Setting the security level to "loose"](#setting-the-security-level-to-loose)
-    - [Formating text in diagrams](#formating-text-in-diagrams)
-    - [Adding Hyperlinks to a Diagram (versions of Mermaid javascript >~ 8.5.0)](#adding-hyperlinks-to-a-diagram-versions-of-mermaid-javascript--850)
-    - [Adding Hyperlinks to a Diagram (versions of Mermaid javascript <~ 8.5.0)](#adding-hyperlinks-to-a-diagram-versions-of-mermaid-javascript--850-1)
-    - [Auto-configure dark mode based on Host OS](#auto-configure-dark-mode-based-on-host-os)
-    - [Material Theme: Switching the Mermaid diagram on the fly between light and dark mode](#material-theme-switching-the-mermaid-diagram-on-the-fly-between-light-and-dark-mode)
-  - [Compatibility](#compatibility)
-    - [List](#list)
-    - [Using Mermaid and code highlighting at the same time](#using-mermaid-and-code-highlighting-at-the-same-time)
-      - [Usage](#usage-1)
-      - [Use of markdown extensions](#use-of-markdown-extensions)
-      - [Declaring the superfences extension](#declaring-the-superfences-extension)
-  - [Troubleshooting: the mermaid diagram is not being displayed](#troubleshooting-the-mermaid-diagram-is-not-being-displayed)
-    - [Seeing an error message at the place of the diagram?](#seeing-an-error-message-at-the-place-of-the-diagram)
-    - [The mermaid source code appears as-is (not read)?](#the-mermaid-source-code-appears-as-is-not-read)
-    - [Using another theme than material ?](#using-another-theme-than-material-)
-    - [Using superfences, but no diagram is displayed?](#using-superfences-but-no-diagram-is-displayed)
-    - [Is mkdocs' version up to date (>= 1.1) ?](#is-mkdocs-version-up-to-date--11-)
-    - [Is the javascript library properly called?](#is-the-javascript-library-properly-called)
-  - [Troubleshooting: other issues](#troubleshooting-other-issues)
-    - [Rich text diagrams, or links are not displayed properly?](#rich-text-diagrams-or-links-are-not-displayed-properly)
-    - [With pymdownx.details, diagrams in collapsed elements are not displayed?](#with-pymdownxdetails-diagrams-in-collapsed-elements-are-not-displayed)
-  - [Using the mermaid2.dumps() function](#using-the-mermaid2dumps-function)
+- [Introduction](#introduction)
+- [Installation](#installation)
+  * [Automatic](#automatic)
+  * [Manual](#manual)
+  * [Test](#test)
+- [How it works](#how-it-works)
+- [Configuration](#configuration)
+  * [Basic configuration](#basic-configuration)
+  * [Specifying the version of the Mermaid library](#specifying-the-version-of-the-mermaid-library)
+  * [Explicit declaration of the Mermaid library](#explicit-declaration-of-the-mermaid-library)
+- [Usage](#usage)
+  * [General Principle](#general-principle)
+  * [How to write Mermaid diagrams](#how-to-write-mermaid-diagrams)
+  * [Adding arguments to the Mermaid engine](#adding-arguments-to-the-mermaid-engine)
+  * [Testing](#testing)
+  * [Adding a Javascript callback function](#adding-a-javascript-callback-function)
+    + [Use Case](#use-case)
+    + [Method](#method)
+- [Tips and Tricks](#tips-and-tricks)
+  * [Setting the security level to "loose"](#setting-the-security-level-to-loose)
+  * [Formatting text in diagrams](#formatting-text-in-diagrams)
+  * [Adding Hyperlinks to a Diagram (versions of Mermaid javascript >~ 8.5.0)](#adding-hyperlinks-to-a-diagram-versions-of-mermaid-javascript--850)
+  * [Adding Hyperlinks to a Diagram (versions of Mermaid javascript <~ 8.5.0)](#adding-hyperlinks-to-a-diagram-versions-of-mermaid-javascript--850)
+  * [Auto-configure dark mode based on Host OS](#auto-configure-dark-mode-based-on-host-os)
+  * [Material Theme: Switching the Mermaid diagram on the fly between light and dark mode](#material-theme-switching-the-mermaid-diagram-on-the-fly-between-light-and-dark-mode)
+- [Compatibility](#compatibility)
+  * [List](#list)
+  * [Using Mermaid and code highlighting at the same time](#using-mermaid-and-code-highlighting-at-the-same-time)
+    + [Usage](#usage-1)
+    + [Use of markdown extensions](#use-of-markdown-extensions)
+    + [Declaring the superfences extension](#declaring-the-superfences-extension)
+- [Troubleshooting](#troubleshooting)
+  * [The mermaid diagram is not displayed (or displayed incorrectly)](#the-mermaid-diagram-is-not-displayed-or-displayed-incorrectly)
+    + [Seeing an error message at the place of the diagram?](#seeing-an-error-message-at-the-place-of-the-diagram)
+    + [The mermaid source code appears as-is (not read)?](#the-mermaid-source-code-appears-as-is-not-read)
+    + [Using another theme than material ?](#using-another-theme-than-material-)
+    + [Using superfences, but no diagram is displayed?](#using-superfences-but-no-diagram-is-displayed)
+    + [Is mkdocs' version up to date (>= 1.1) ?](#is-mkdocs-version-up-to-date--11-)
+    + [Is the javascript library properly called?](#is-the-javascript-library-properly-called)
+    + [A certain type of diagram (e.g. mindmap, etc.) is not displayed, or the syntax is incorrectly interpreted?](#a-certain-type-of-diagram-eg-mindmap-etc-is-not-displayed-or-the-syntax-is-incorrectly-interpreted)
+  * [Other issues](#other-issues)
+    + [Rich text diagrams, or links are not displayed properly?](#rich-text-diagrams-or-links-are-not-displayed-properly)
+    + [With pymdownx.details, diagrams in collapsed elements are not displayed?](#with-pymdownxdetails-diagrams-in-collapsed-elements-are-not-displayed)
+- [Using the mermaid2.dumps() function](#using-the-mermaid2dumps-function)
+- [How to contribute](#how-to-contribute)
+- [Credits](#credits)
 
 <!-- tocstop -->
 
-## How it works
+## Introduction
+
+Mermaid2 allows you to insert mermaid markup in the markdown 
+of your mkdocs pages.
+
+For example, a markdown page containing the following diagram:
+
+    ```mermaid
+    graph LR
+        hello --> world
+        world --> again
+        again --> hello
+    ```
+
+will then be displayed in the final HTML page as:
+
+```mermaid
+graph LR
+    hello --> world
+    world --> again
+    again --> hello
+```
+
+The diagram will be rendered on the fly by the web browser,
+with the use of the mermaid javascript library. 
+mkdocs-mermaid2 takes care of inserting the javascript library into
+the html page.
+
+> You can use all the diagrams types supported by the version of the Mermaid 
+> javascript library that you are using (flowchart, class, state, timeline, 
+> etc.).
+
+
+## Installation
+
+### Automatic
+
+
+```bash
+pip install mkdocs-mermaid2-plugin
+```
+
+### Manual
+Clone this repository in a local directory and install the package:
+
+```bash
+python setup.py install
+```
+
+### Test
+For running the examples the `test` directory, 
+you will also need the mkdocs-material theme. You may 
+[install it directly](https://squidfunk.github.io/mkdocs-material/getting-started/),
+or use the following command to install the whole package:
+
+```bash
+pip install mkdocs-mermaid2-plugin[test]
+```
+
 
-**If you do not wish to learn the details under the hood,
-skip to the [Installation](#installation) section**.
+## How it works
 
-Normally mkdocs inserts the Mermaid code (text) describing the diagram 
+When converting the markdown into HTML, mkdocs normally inserts the
+Mermaid code (text) describing the diagram 
 into segments `<pre><code class='mermaid>`:
 
     <pre><div class="mermaid">
     ...
     </div></pre>
 
 To make the HTML/css page more robust, the mermaid plugin converts 
@@ -88,55 +148,59 @@
     <div class="mermaid">
     ...
     </div>
 
 It also inserts a call to the 
 [javascript library](https://github.com/mermaid-js/mermaid) :
 
-    <script>
-    mermaid.initialize(...)
-    </script>
 
-To interpret that code it inserts a call to the Mermaid library:
-```javascript
-<script src="https://unpkg.com/mermaid/dist/mermaid.min.js">
+
+> **From version 1.0 of mkdocs-mermaid2:**
+
+[For versions from 10.0.0 of the Mermaid javascript library, the plugin uses the ESM format](https://github.com/mermaid-js/mermaid/releases/tag/v10.0.0), since
+it is the only one available. This requires a specific call from the HTML
+page e.g.:
+```html
+<script type="module">
+import mermaid from "https://unpkg.com/mermaid@10.0.2/dist/mermaid.esm.min.mjs"
 </script>
 ```
 
-The user's browser will then read this code and render it on the fly.
+For an earlier version of the library, the plugin uses the traditional call
+from HTML:
+```html
+<script src="https://unpkg.com/mermaid@8.8.2/dist/mermaid.min.js">
+</script>
+```
 
-> No svg/png images are harmed during the rendering of that graph.
+To start displaying of the diagrams, the plugin then automatically inserts 
+a separate call to initialize the Mermaid library:
 
+    <script>
+    mermaid.initialize()
+    </script>
 
 
-## Installation
+The user's browser will then read this code and render it on the fly.
 
-### Automatic
+> No svg/png images are produced during the rendering of that graph.
 
 
-```bash
-pip install mkdocs-mermaid2-plugin
-```
 
-### Manual
-Clone this repository in a local directory and install the package:
 
-```bash
-python setup.py install
-```
 
 ## Configuration
 
 ### Basic configuration
-To enable this plugin, you need to declare it in your config file
+To enable this plugin, you need to declare it in your [mkdocs config file](https://www.mkdocs.org/user-guide/configuration/)
 (`mkdocs.yml`).
 
 In order to work, the plugin also requires the
 [mermaid](https://www.npmjs.com/package/mermaid) javascript
-library (in the exemple below, it fetched from the last version
+library (in the example below, it fetched from the last version
 from the [unpkg](https://unpkg.com/) repository; change the version
 no as needed).
 
 ```yaml
 plugins:
     - search
     - mermaid2
@@ -154,39 +218,63 @@
 
 You may specify a different version of the Mermaid library, like so:
 
 ```yaml
 plugins:
   - search
   - mermaid2:
-      version: 8.6.4
+      version: 10.0.2
 ```
 
+The plugin will insert the correct call to the javascript library
+inside the final HTML page.
 
 
 ### Explicit declaration of the Mermaid library
-> If you use a version of the plugin >= 0.4, the basic steps are sufficient.
 
 You _may_ specify the mermaid library explicitly, as long as it is
 call mermaid (independently of extension):
 
 ```yaml
 extra_javascript:
     - https://unpkg.com/mermaid@8.7.0/dist/mermaid.min.js
 ```
 
-For the latest version:
+This will be translated in the final HTML page as:
+
+```html
+<script src="https://unpkg.com/mermaid@8.7.0/dist/mermaid.min.js">
+```
+
+> This will work **only** for versions of the Mermaid javascript 
+> library that can be called in that way, i.e. that do not use the ES Module
+> standard (ESM). [Above version 10.0.0 only ESM format libraries are
+> available](https://github.com/mermaid-js/mermaid/releases/tag/v10.0.0).
+
+
+As a workaround you could declare a local script file:
 
 ```yaml
 extra_javascript:
-    - https://unpkg.com/mermaid/dist/mermaid.min.js
+    - js/mermaidloader.js
+```
+
+Where `js` is a subdirectory of the document directory (`docs`).
+
+If you are using a local javascript file, it is up to you to write the import,
+with a version of the Mermaid library > 10 e.g.:
+
+```yaml
+import mermaid from "https://unpkg.com/mermaid@10.0.2/dist/mermaid.esm.min.mjs"
 ```
 
+No explicit call to `mermaid.initialize()` is required, since it is
+automatically inserted by the plugin.
+
 
-> **Note for plugin version < 0.4:** You **must*** include the mermaid.min.js (local or remotely) in your `mkdocs.yml`. If you want to be on the safe side, you may want to specify a version that you know is working for you, e.g. `https://unpkg.com/mermaid@8.7.0/dist/mermaid.min.js` 
 
 
 
 
 ## Usage
 
 ### General Principle
@@ -199,25 +287,23 @@
     graph TD
     A[Client] --> B[Load Balancer]
     B --> C[Server01]
     B --> D[Server02]
     ```
 
 ### How to write Mermaid diagrams
-* For instructions on how to make a diagram, see 
-  [the official website](https://mermaid-js.github.io/mermaid/#/).
-* If you are not familiar, see the [n00bs' introduction to mermaid](https://mermaid-js.github.io/mermaid/#/n00b-overview).
-* In case of doubt, you will want to test your diagrams in the
-  [Mermaid Live Editor](https://mermaid-js.github.io/mermaid-live-editor).
 
+* For instructions on how to make a diagram, see [the official website](https://mermaid.js.org).
+* If you are not familiar, see the [Mermaid Overview for Beginners](https://mermaid.js.org/community/n00b-overview.html).
+* In case of doubt, you will want to test your diagrams in the [Mermaid Live Editor](https://mermaid.live).
 
 ### Adding arguments to the Mermaid engine
 
 By default, the plugin automatically inserts 
-the a Javascript command `mermaid.initialize();`
+a Javascript command `mermaid.initialize();`
 in the HTML pages, which starts the interpretation.
 Sometimes, however, you may want to add some
 initialization commands (see [full list](https://github.com/knsv/mermaid/blob/master/docs/mermaidAPI.md#mermaidapi-configuration-defaults)).
 
 For example, you could change the theme of the diagram, 
 using 'dark' instead of the default one. 
 Simply add those arguments in the config file, e.g.
@@ -315,15 +401,15 @@
 
 ```yaml
     - mermaid2:
         arguments:
           securityLevel: 'loose'
 ```
 
-### Formating text in diagrams
+### Formatting text in diagrams
 > To enable this function, you need to [relax mermaid's security level to 'loose'](#setting-the-security-level-to-loose).
 
 You may use HTML in the diagram.
 
 > **Note:** This is guaranteed to work with Mermaid 8.6.4, but
 > does not work e.g. on 8.7.0.
 
@@ -360,15 +446,15 @@
 
 ### Adding Hyperlinks to a Diagram (versions of Mermaid javascript <~ 8.5.0)
 > To enable this function, you need to [relax mermaid's security level to 'loose'](#setting-the-security-level-to-loose).
 
 It is possible to add hyperlinks to a  diagram, e.g.:
 
 ```
-box1[An <b>important</b> <a href="http://google.com">link</a>] 
+box1[An <b>important</b> <a href="https://google.com">link</a>] 
 ```
 
 
 ### Auto-configure dark mode based on Host OS
 
 Using a combination of the unquote (`^`) functionality of this plugin and the
 [prefers-color-scheme](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-color-scheme)
@@ -423,29 +509,29 @@
       primary: black
       accent: deep orange
       toggle:
         icon: material/toggle-switch
         name: Switch to light mode
 
   # https://facelessuser.github.io/pymdown-extensions/extensions/superfences/
-  - pymdownx.superfences:
+  pymdownx.superfences:
       custom_fences:
         - name: mermaid
           class: mermaid
           format: !!python/name:mermaid2.fence_mermaid
 
-
-
-
 plugins:
   - mermaid2:
       arguments:
         # test if its __palette_1 (dark) or __palette_2 (light)
+        # for mkdocs-material >=8.0.0
         theme: |
-          ^(JSON.parse(window.localStorage.getItem('/.__palette')).index == 1) ? 'dark' : 'light'
+          ^(JSON.parse(__md_get("__palette").index == 1)) ? 'dark' : 'light'
+#       for mkdocs-material <8.0.0
+#         ^(JSON.parse(window.localStorage.getItem(__prefix('__palette'))).index == 1) ? 'dark' : 'light'
 
 extra_javascript:
     - extra/refresh_on_toggle_dark_light.js
 ```
 
 > The caret operator (`^`) means "unquote". It is used here to insert Javascript code into the initialization code of `mermaid.initialize()`.
 
@@ -471,29 +557,28 @@
   location.reload();
 });
 ```
 
 ## Compatibility
 
 ### List
-Here is a short list of comptabilities and incompatibilities for
+Here is a short list of compatibilities and incompatibilities for
 the mermaid plugin:
 
-Item | Type | Status | Note 
---|--|--|--
-**mkdocs** | theme | YES | (default) plugin version >= 0.5 | 
-**material** | theme | YES |  |
-**windmill** | theme | YES | plugin version >= 0.5 | 
-**admonition** | extension | YES | 
-**footnotes** | extension | YES | 
-**minify** | plugin | NO | Breaks the mermaid diagrams.
-**pymdownx.highlight** | extension | NO | Use [pymdownx.superfences](#declaring-the-superfences-extension)
-**pymdownx.superfences** | extension | OK | [see paragraph](#declaring-the-superfences-extension)
-**search** | plugin | OK | Do not forget to declare it in `config.yml`.
-
+| Item                     | Type      | Status | Note                                                             |
+|--------------------------|-----------|--------|------------------------------------------------------------------|
+| **mkdocs**               | theme     | YES    | (default) plugin version >= 0.5                                  | 
+| **material**             | theme     | YES    |                                                                  |
+| **windmill**             | theme     | YES    | plugin version >= 0.5                                            | 
+| **admonition**           | extension | YES    |                                                                  |
+| **footnotes**            | extension | YES    |                                                                  |
+| **minify**               | plugin    | NO     | Breaks the mermaid diagrams.                                     |
+| **pymdownx.highlight**   | extension | NO     | Use [pymdownx.superfences](#declaring-the-superfences-extension) |
+| **pymdownx.superfences** | extension | OK     | [see paragraph](#declaring-the-superfences-extension)            |
+| **search**               | plugin    | OK     | Do not forget to declare it in `config.yml`.                     |
 
 ### Using Mermaid and code highlighting at the same time
 
 #### Usage
 
 It is quite natural that we want to display **mermaid diagrams**,
 while having usual **code highlighting** (for bash, python, etc.).
@@ -542,106 +627,107 @@
 > (e.g. `<small>` must have its corresponding `</small>` tag).
 > Otherwise, the extension system will attempt to close those tags 
 > and it will break the diagram.
 
 
 
 
+## Troubleshooting
 
-
-## Troubleshooting: the mermaid diagram is not being displayed
+### The mermaid diagram is not displayed (or displayed incorrectly)
 
 > To start with, use a simple diagram that you know is syntactically correct.
 
 e.g.
 
     ```mermaid
     graph TD
     A[Client] --> B[Load Balancer]
     B --> C[Server01]
     B --> D[Server02]
     ```
 
-### Seeing an error message at the place of the diagram?
+#### Seeing an error message at the place of the diagram?
 
 In recent versions of the javascript library (> 8.6.0), a pretty
 error message is displayed in case of incorrect syntax:
 
 ![error message](error.png)
 
 > **In earlier versions, the library displays nothing, which 
 > can be confusing.**
 
 If you see the error message, it is at least an indication that 
 the mermaid javascript library was called.
 
-### The mermaid source code appears as-is (not read)?
+#### The mermaid source code appears as-is (not read)?
 In that case, the javascript library was probably not called.
 See the next questions.
 
 
-### Using another theme than material ?
+#### Using another theme than material ?
 
 If the diagram is not rendered, upgrade to plugin version >= 0.5.0
 
-### Using superfences, but no diagram is displayed?
+#### Using superfences, but no diagram is displayed?
 
 If you are using the superfences extension, but you see the source
 code, you probably forgot to declare the custom_fences. 
 Se more explanations under [Declaring the superfences extension](#declaring-the-superfences-extension)
 
-### Is mkdocs' version up to date (>= 1.1) ?
+#### Is mkdocs' version up to date (>= 1.1) ?
 
 Use `mkdocs -v`.
 
 If not, update it:
 
     pip install mkdocs --upgrade
 
 Or, if you cloned this repo:
 
     python setup.py install
 
 
-### Is the javascript library properly called?
-
-> ***Note that that this is no longer mandatory since version 0.4 of the
-> plugin.*** You may want to try to remove this call, in case there was
-> an error.
+#### Is the javascript library properly called?
 
 In order to work, the proper javascript library must called from
-the html page.
-
-The configuration file (`mkdocs.yml`) should contain the following line:
-
-    extra_javascript:
-        - https://unpkg.com/mermaid/dist/mermaid.min.js
+the html page (this is done automatically).
+If necessary check the link used in the HTML page generated, e.g.:
 
+```HTML
+<script type="module">import mermaid from "https://unpkg.com/mermaid@10.0.2/dist/mermaid.esm.min.mjs"</script>
+```
 
 Every diagram should start with a valid preamble, e.g. `graph TD`.
 
 In case of doubt, you may want to test your diagram in the
 [Mermaid Live Editor](https://mermaid-js.github.io/mermaid-live-editor).
 
 
 > Note, however, that the Mermaid Live Editor **does not
 > support loose mode** (with HTML code in the mermaid code).
 
-## Troubleshooting: other issues
+#### A certain type of diagram (e.g. mindmap, etc.) is not displayed, or the syntax is incorrectly interpreted?
 
-### Rich text diagrams, or links are not displayed properly?
+Check the version of the javascript mermaid library you are using (it's indicated
+in the error message; as a last resort, check in the html page). 
+You can [change the library version if needed](#specifying-the-version-of-the-mermaid-library).
+
+### Other issues
+
+#### Rich text diagrams, or links are not displayed properly?
 
 1. As a first step, [set the security level to 'loose'](#setting-the-security-level-to-loose).
 2. Make sure you use a compatible version of the javascript library
    (8.6.4, 8.8.0, ~~8.7.0~~). In principle, the version used
    by the plugin is compatible (see instructions to 
    [change the version](#specifying-the-version-of-the-mermaid-library)).
 
 
-### With pymdownx.details, diagrams in collapsed elements are not displayed?
+#### With pymdownx.details, diagrams in collapsed elements are not displayed?
 
 **This fix is experimental (it has been tested once and it worked).**
 
 If you declared `pymdownx.details` in `config.yml` 
 (under `markdown_extensions`), you may notice that a diagram will not
 display correctly in that case:
 
@@ -728,7 +814,29 @@
     barbaz: bazbar,
     foo: {
         bar: 2
     },
     bar: true
 }
 ```
+
+## How to contribute
+
+Contributions are welcome.
+
+Use the Issues to signal a bug or propose a feature you believe is necessary.
+
+If this is a usage question, prefer the discussions.
+
+Always open an Issue and consider the answers, before submitting a PR.
+
+## Credits
+
+mkdocs-mermaid2 is a fork from
+[Pugong Liu's excellent project](https://github.com/pugong/mkdocs-mermaid-plugin), 
+which is no longer maintained. This new plugin offers expanded documentation as
+well as new functions.
+
+It is also compatible with versions of the mermaid library > 10.0.
+
+Thanks to all the members of the community who participated to the 
+improvement of this project with ideas and PRs.
```

### Comparing `mkdocs-mermaid2-plugin-0.6.0/error.png` & `mkdocs-mermaid2-plugin-1.0.1/error.png`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-0.6.0/mermaid2/fence.py` & `mkdocs-mermaid2-plugin-1.0.1/mermaid2/fence.py`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-0.6.0/mermaid2/plugin.py` & `mkdocs-mermaid2-plugin-1.0.1/mermaid2/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 """
 Main plugin module for mermaid2
 """
 
 import os
 
+
 from mkdocs.plugins import BasePlugin
 from mkdocs.config.config_options import Type as PluginType
 from bs4 import BeautifulSoup
 
 from . import pyjs
 from .util import info, libname, url_exists
 
 
 # ------------------------
 # Constants and utilities
 # ------------------------
 # the default (recommended) mermaid lib
-MERMAID_LIB_VERSION = '8.8.0'
-MERMAID_LIB = "https://unpkg.com/mermaid@%s/dist/mermaid.min.js"
+MERMAID_LIB_VERSION = '10.0.2'
+# MERMAID_LIB = "https://unpkg.com/mermaid@%s/dist/mermaid.min.js"
+MERMAID_LIB_PRE_10 = "https://unpkg.com/mermaid@%s/dist/mermaid.min.js"
+MERMAID_LIB = "https://unpkg.com/mermaid@%s/dist/mermaid.esm.min.mjs"
+
+
+MERMAID_CODE_PRE_10 = '<script src="%s">\n'
+MERMAID_CODE = '<script type="module">import mermaid from "%s"</script>\n'
+
+
+
 # Two conditions for activating custom fences:
 SUPERFENCES_EXTENSION = 'pymdownx.superfences'
 CUSTOM_FENCE_FN = 'fence_mermaid_custom' 
 
+
+
 # ------------------------
 # Plugin
 # ------------------------
 class MarkdownMermaidPlugin(BasePlugin):
     """
     Plugin for interpreting Mermaid code
     """
@@ -48,17 +60,40 @@
         which also includes the contents of the yaml config file.
         """
         return self._full_config  
     
     @property
     def mermaid_args(self):
         """
-        The arguments for mermaid.
+        The arguments for mermaid, found in the config file.
         """
         return self._mermaid_args
+    
+    @property
+    def mermaid_version(self) -> str:
+        """
+        The version of mermaid
+        This information comes from the YAML file parameter,
+        or, if empty, from MERMAID_LIB_VERSION.
+        """
+        version = self.config['version']
+        assert version, "No correct version of mermaid is provided!"
+        return version
+    
+    @property
+    def mermaid_major_version(self) -> int:
+        """
+        Major version of mermaid (e.g. 8. 9, 10) as int
+        """
+        major = self.mermaid_version.split('.')[0]
+        try:
+            return int(major)
+        except: 
+            ValueError("Mermaid version provided has incorrect format")
+
 
     @property
     def extra_mermaid_lib(self) -> str:
         """
         Provides the mermaid library defined in mkdocs.yml (if any)
         """
         extra_javascript = self.full_config.get('extra_javascript', [])
@@ -68,24 +103,39 @@
                 return lib
         return ''
 
 
     @property
     def mermaid_lib(self) -> str:
         """
-        Provides the actual mermaid library used
+        Provides the url of mermaid library according to version
+        (distinction between version < 10 and after)
         """
         if not hasattr(self, '_mermaid_lib'):
-            mermaid_version = self.config['version']
-            lib = self.extra_mermaid_lib or MERMAID_LIB % mermaid_version 
-            if not url_exists(lib):
+            if self.mermaid_major_version < 10:
+                mermaid_lib = MERMAID_LIB_PRE_10 % self.mermaid_version
+            else:
+                # newer versions
+                mermaid_lib = MERMAID_LIB % self.mermaid_version
+            # make checks
+            if not url_exists(mermaid_lib):
                 raise FileNotFoundError("Cannot find Mermaid library: %s" %
-                                        lib)
-            self._mermaid_lib = lib
+                                        mermaid_lib)
+            self._mermaid_lib = mermaid_lib
         return self._mermaid_lib
+    
+    @property
+    def mermaid_script(self) -> str:
+        """
+        Provides the mermaid script to be inserted into the code
+        """
+        if self.mermaid_major_version < 10:
+            return MERMAID_CODE_PRE_10 % self.mermaid_lib
+        else:
+            return MERMAID_CODE % self.mermaid_lib
 
     @property
     def activate_custom_loader(self) -> bool:
         """
         Predicate: activate the custom loader for superfences?
         The rule is to activate:
             1. superfences extension is activated
@@ -131,17 +181,19 @@
         """
         The initial configuration
         store the configuration in properties
         """
         # the full config info for the plugin is there
         # we copy it into our own variable, to keep it accessible
         self._full_config = config
-        # here we use the standard self.config property:
-        # (this can get confusing...)
+        # Storing the arguments to be passed to the Javascript library;
+        # they are found under `mermaid2:arguments` in the config file:
         self._mermaid_args = self.config['arguments']
+        # Here we used the standard self.config property
+        # (this can get confusing...)
         assert isinstance(self.mermaid_args, dict)
         info("Initialization arguments:", self.mermaid_args)
         # info on the javascript library:
         if self.extra_mermaid_lib:
             info("Explicit mermaid javascript library:\n  ", 
                  self.extra_mermaid_lib)
         else:
@@ -188,24 +240,27 @@
             # Count the diagrams <div class = 'mermaid'> ... </div>
             mermaids = len(soup.select("div.mermaid"))
         # if yes, add the javascript snippets:
         if mermaids:
             info("Page '%s': found %s diagrams, adding scripts" % 
                     (page_name, mermaids))
             if not self.extra_mermaid_lib:
-                # if no extra library mentioned specify it
-                new_tag = soup.new_tag("script", src=self.mermaid_lib)
+                # if no extra library mentioned,
+                # add the <SCRIPT> tag needed for mermaid
+                info("Adding call to script for version"
+                     f"{self.mermaid_version}.")
+                new_tag = BeautifulSoup(self.mermaid_script, 'html.parser')
                 soup.body.append(new_tag)
                 # info(new_tag)
+            # insertion of the <script> tag, with the initialization arguments
+            # (self.mermaid_args), as found in the config file.
             new_tag = soup.new_tag("script")
-            # initialization command
             if self.activate_custom_loader:
                 # if the superfences extension is present, use the specific loader
                 self.mermaid_args['startOnLoad'] = False
                 js_args =  pyjs.dumps(self.mermaid_args) 
-                #new_tag.string = "window.mermaidConfig = {\n    default: %s\n}" % js_args
                 new_tag.string = "window.mermaidConfig = {default: %s}" % js_args
             else:
                 js_args =  pyjs.dumps(self.mermaid_args) 
                 new_tag.string="mermaid.initialize(%s);" % js_args
             soup.body.append(new_tag)
-        return str(soup)
+        return str(soup)
```

### Comparing `mkdocs-mermaid2-plugin-0.6.0/mermaid2/pyjs.py` & `mkdocs-mermaid2-plugin-1.0.1/mermaid2/pyjs.py`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-0.6.0/mermaid2/util.py` & `mkdocs-mermaid2-plugin-1.0.1/mermaid2/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-0.6.0/mkdocs_mermaid2_plugin.egg-info/PKG-INFO` & `mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: mkdocs-mermaid2-plugin
-Version: 0.6.0
+Version: 1.0.1
 Summary: A MkDocs plugin for including mermaid graphs in markdown sources
 Home-page: https://github.com/fralau/mkdocs-mermaid2-plugin
 Author: pugong, Fralau
 Author-email: pugong.liu@gmail.com, fralau2035@yahoo.com
 License: MIT
 Keywords: mkdocs python markdown mermaid
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
+Provides-Extra: test
 License-File: LICENSE
 
 A mkdocs plugin that interprets mermaid graphs in the markdown file.To install, please follow instructions in the readme file.This is a fork of the Pugong Liu's excellent project, which is no longer maintained.
-
```

### Comparing `mkdocs-mermaid2-plugin-0.6.0/mkdocs_mermaid2_plugin.egg-info/SOURCES.txt` & `mkdocs-mermaid2-plugin-1.0.1/mkdocs_mermaid2_plugin.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,11 +21,15 @@
 test/medium/docs/index.md
 test/medium/docs/second.md
 test/medium/docs/js/extra.js
 test/simple/mkdocs.yml
 test/simple/docs/index.md
 test/simple/docs/second.md
 test/simple/docs/js/extra.js
+test/simple_pre_10/mkdocs.yml
+test/simple_pre_10/docs/index.md
+test/simple_pre_10/docs/second.md
+test/simple_pre_10/docs/js/extra.js
 test/superfences/mkdocs.yml
 test/superfences/docs/index.md
 test/superfences/docs/second.md
 test/superfences/docs/js/loader.js
```

### Comparing `mkdocs-mermaid2-plugin-0.6.0/setup.py` & `mkdocs-mermaid2-plugin-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-import os
 from setuptools import setup, find_packages
 
 
-VERSION = '0.6.0'
+VERSION = '1.0.1'
+
+# required if you want to run tests
+# pip install 'mkdocs-mermaid2-plugin[test]'
+TEST_REQUIRE = ['mkdocs-material']
+
 
 def readme():
     """print long description"""
     with open('README.md') as f:
         return f.read()
 
+
 LONG_DESCRIPTION = (
     "A mkdocs plugin that interprets mermaid graphs in the markdown file."
     "To install, please follow instructions in the readme file."
     "This is a fork of the Pugong Liu's excellent project, "
     "which is no longer maintained."
 )
 
@@ -28,19 +33,20 @@
     license='MIT',
     python_requires='>=3.5',
     install_requires=[
         'setuptools>=18.5',
         'beautifulsoup4>=4.6.3',
         'mkdocs>=1.0.4',
         'jsbeautifier',
-        'pyyaml', # for testing
-        'mkdocs-material', # for testing
         'requests',
         'pymdown-extensions >= 8.0'
     ],
+    extras_require={
+        'test': TEST_REQUIRE,
+    },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
```

### Comparing `mkdocs-mermaid2-plugin-0.6.0/test/medium/docs/index.md` & `mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-0.6.0/test/medium/docs/js/extra.js` & `mkdocs-mermaid2-plugin-1.0.1/test/medium/docs/js/extra.js`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-0.6.0/test/medium/mkdocs.yml` & `mkdocs-mermaid2-plugin-1.0.1/test/medium/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-0.6.0/test/simple/docs/js/extra.js` & `mkdocs-mermaid2-plugin-1.0.1/test/simple/docs/js/extra.js`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-0.6.0/test/superfences/docs/index.md` & `mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-0.6.0/test/superfences/docs/js/loader.js` & `mkdocs-mermaid2-plugin-1.0.1/test/superfences/docs/js/loader.js`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-0.6.0/test/superfences/mkdocs.yml` & `mkdocs-mermaid2-plugin-1.0.1/test/superfences/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-mermaid2-plugin-0.6.0/update_pypi.sh` & `mkdocs-mermaid2-plugin-1.0.1/update_pypi.sh`

 * *Files identical despite different names*


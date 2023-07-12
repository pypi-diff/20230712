# Comparing `tmp/isic-cli-6.1.0.tar.gz` & `tmp/isic-cli-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic-cli-6.1.0.tar", last modified: Tue Jun  6 15:21:11 2023, max compression
+gzip compressed data, was "isic-cli-6.2.0.tar", last modified: Wed Jul 12 21:10:56 2023, max compression
```

## Comparing `isic-cli-6.1.0.tar` & `isic-cli-6.2.0.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.457223 isic-cli-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-06 15:20:46.000000 isic-cli-6.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-06 15:20:46.000000 isic-cli-6.1.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.449222 isic-cli-6.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.453223 isic-cli-6.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-06 15:20:46.000000 isic-cli-6.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-06 15:20:46.000000 isic-cli-6.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-06 15:20:46.000000 isic-cli-6.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 15:20:46.000000 isic-cli-6.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-06 15:21:11.457223 isic-cli-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-06 15:20:46.000000 isic-cli-6.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.453223 isic-cli-6.1.0/isic_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.457223 isic-cli-6.1.0/isic_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/accession.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.457223 isic-cli-6.1.0/isic_cli/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/io/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.457223 isic-cli-6.1.0/isic_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-06 15:20:46.000000 isic-cli-6.1.0/isic_cli/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.453223 isic-cli-6.1.0/isic_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-06 15:21:11.000000 isic-cli-6.1.0/isic_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-06 15:21:11.000000 isic-cli-6.1.0/isic_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:21:11.000000 isic-cli-6.1.0/isic_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 15:21:11.000000 isic-cli-6.1.0/isic_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-06 15:21:11.000000 isic-cli-6.1.0/isic_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 15:21:11.000000 isic-cli-6.1.0/isic_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-06 15:20:46.000000 isic-cli-6.1.0/justfile
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-06 15:20:46.000000 isic-cli-6.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 15:21:11.457223 isic-cli-6.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-06 15:20:46.000000 isic-cli-6.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:21:11.457223 isic-cli-6.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_cli_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_cli_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_cli_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_cli_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-06 15:20:46.000000 isic-cli-6.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.472213 isic-cli-6.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.468213 isic-cli-6.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.468213 isic-cli-6.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.github/workflows/release.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      415 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.github/zip_and_upload_package.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-12 21:10:32.000000 isic-cli-6.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 21:10:32.000000 isic-cli-6.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-12 21:10:56.472213 isic-cli-6.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-12 21:10:32.000000 isic-cli-6.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.468213 isic-cli-6.2.0/isic_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.472213 isic-cli-6.2.0/isic_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/accession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.472213 isic-cli-6.2.0/isic_cli/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/io/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.472213 isic-cli-6.2.0/isic_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-12 21:10:32.000000 isic-cli-6.2.0/isic_cli/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.468213 isic-cli-6.2.0/isic_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-12 21:10:56.000000 isic-cli-6.2.0/isic_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-12 21:10:56.000000 isic-cli-6.2.0/isic_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:10:56.000000 isic-cli-6.2.0/isic_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 21:10:56.000000 isic-cli-6.2.0/isic_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-12 21:10:56.000000 isic-cli-6.2.0/isic_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 21:10:56.000000 isic-cli-6.2.0/isic_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-12 21:10:32.000000 isic-cli-6.2.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-12 21:10:32.000000 isic-cli-6.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:10:56.472213 isic-cli-6.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-12 21:10:32.000000 isic-cli-6.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:10:56.472213 isic-cli-6.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_cli_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_cli_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_cli_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-12 21:10:32.000000 isic-cli-6.2.0/tox.ini
```

### Comparing `isic-cli-6.1.0/.github/workflows/ci.yml` & `isic-cli-6.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/.github/workflows/release.yml` & `isic-cli-6.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/.gitignore` & `isic-cli-6.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/LICENSE` & `isic-cli-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/PKG-INFO` & `isic-cli-6.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 6.1.0
+Version: 6.2.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
@@ -19,28 +19,27 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # isic-cli
-[![PyPI](https://img.shields.io/pypi/v/isic-cli)](https://pypi.org/project/isic-cli/)
 
 The official command line tool for interacting with the [ISIC Archive](https://isic-archive.com).
 
-## Quickstart
-
-``` sh
-pip install isic-cli  # requires python >= 3.9
-isic user login  # optional
-```
+## Installation
+- Download the [latest isic-cli release](https://github.com/ImageMarkup/isic-cli/releases/latest).
+- Extract the executable to a location where it can be invoked from the command line.
 
+If running on macOS, you may need to [add the executable to the list of trusted software](https://support.apple.com/guide/mac-help/apple-cant-check-app-for-malicious-software-mchleab3a043/mac) to launch isic-cli in the same way you would any other registered app.
 
 ## Common use cases
 
+Note: `isic` will be `isic.exe` on Windows.
+
 ### Downloading images
 
 ``` sh
 isic image download images/  # downloads the entire archive, images and metadata, to images/
 
 # optionally filter the results
 isic image download --search 'diagnosis:"basal cell carcinoma"' images/
```

### Comparing `isic-cli-6.1.0/isic_cli/cli/__init__.py` & `isic-cli-6.2.0/isic_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/isic_cli/cli/accession.py` & `isic-cli-6.2.0/isic_cli/cli/accession.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/isic_cli/cli/collection.py` & `isic-cli-6.2.0/isic_cli/cli/collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/isic_cli/cli/image.py` & `isic-cli-6.2.0/isic_cli/cli/image.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/isic_cli/cli/metadata.py` & `isic-cli-6.2.0/isic_cli/cli/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import OrderedDict, defaultdict
 import csv
+import io
 import itertools
 from pathlib import Path
 import sys
 
 import click
 from click.types import IntRange
 from humanize import intcomma
@@ -23,26 +24,25 @@
 @click.pass_obj
 def metadata(obj):
     pass
 
 
 @metadata.command(name="validate")
 @click.argument(
-    "csv_path",
-    type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True, path_type=Path),
+    "csv_file",
+    type=click.File("rb"),
 )
-def validate(csv_path: Path):
+def validate(csv_file: io.BufferedReader):
     """Validate metadata from a local csv."""
     # These imports are slow, inline them.
     import numpy as np
     import pandas as pd
 
     console = Console()
-    with open(csv_path) as csv:
-        df = pd.read_csv(csv, header=0)
+    df = pd.read_csv(csv_file, header=0)
 
     # pydantic expects None for the absence of a value, not NaN
     df = df.replace({np.nan: None})
 
     # keyed by column, message
     column_problems: dict[tuple[str, str], list[int]] = defaultdict(list)
```

### Comparing `isic-cli-6.1.0/isic_cli/cli/types.py` & `isic-cli-6.2.0/isic_cli/cli/types.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/isic_cli/cli/user.py` & `isic-cli-6.2.0/isic_cli/cli/user.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/isic_cli/cli/utils.py` & `isic-cli-6.2.0/isic_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/isic_cli/io/http.py` & `isic-cli-6.2.0/isic_cli/io/http.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/isic_cli/session.py` & `isic-cli-6.2.0/isic_cli/session.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/isic_cli/utils/version.py` & `isic-cli-6.2.0/isic_cli/utils/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,21 +62,19 @@
             return
 
         upgrade_type_available = upgrade_type(this_version, newest_version)
 
         if upgrade_type_available == "major":
             click.secho(
                 """There is a new major version of isic-cli available.
-You must upgrade before continuing.
-If you are using pip, then you can upgrade by running the following command:
+You must upgrade before continuing. See https://github.com/ImageMarkup/isic-cli for instructions.
 """,
                 fg="yellow",
                 err=True,
             )
-            click.echo(click.style("pip install --upgrade isic-cli", fg="green"), err=True)
             sys.exit(1)
         elif upgrade_type_available == "minor":
             click.secho(
                 "Psst, there's a new version of isic-cli available. Upgrade!\n",
                 fg="yellow",
                 err=True,
             )
```

### Comparing `isic-cli-6.1.0/isic_cli.egg-info/PKG-INFO` & `isic-cli-6.2.0/isic_cli.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 6.1.0
+Version: 6.2.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
@@ -19,28 +19,27 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # isic-cli
-[![PyPI](https://img.shields.io/pypi/v/isic-cli)](https://pypi.org/project/isic-cli/)
 
 The official command line tool for interacting with the [ISIC Archive](https://isic-archive.com).
 
-## Quickstart
-
-``` sh
-pip install isic-cli  # requires python >= 3.9
-isic user login  # optional
-```
+## Installation
+- Download the [latest isic-cli release](https://github.com/ImageMarkup/isic-cli/releases/latest).
+- Extract the executable to a location where it can be invoked from the command line.
 
+If running on macOS, you may need to [add the executable to the list of trusted software](https://support.apple.com/guide/mac-help/apple-cant-check-app-for-malicious-software-mchleab3a043/mac) to launch isic-cli in the same way you would any other registered app.
 
 ## Common use cases
 
+Note: `isic` will be `isic.exe` on Windows.
+
 ### Downloading images
 
 ``` sh
 isic image download images/  # downloads the entire archive, images and metadata, to images/
 
 # optionally filter the results
 isic image download --search 'diagnosis:"basal cell carcinoma"' images/
```

### Comparing `isic-cli-6.1.0/isic_cli.egg-info/SOURCES.txt` & `isic-cli-6.2.0/isic_cli.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 .gitignore
 LICENSE
 README.md
 justfile
 pyproject.toml
 setup.py
 tox.ini
+.github/zip_and_upload_package.sh
 .github/workflows/ci.yml
+.github/workflows/package.yml
 .github/workflows/release.yml
 isic_cli/__init__.py
 isic_cli/oauth.py
 isic_cli/session.py
 isic_cli.egg-info/PKG-INFO
 isic_cli.egg-info/SOURCES.txt
 isic_cli.egg-info/dependency_links.txt
 isic_cli.egg-info/entry_points.txt
 isic_cli.egg-info/requires.txt
 isic_cli.egg-info/top_level.txt
 isic_cli/cli/__init__.py
+isic_cli/cli/__main__.py
 isic_cli/cli/accession.py
 isic_cli/cli/collection.py
 isic_cli/cli/context.py
 isic_cli/cli/image.py
 isic_cli/cli/metadata.py
 isic_cli/cli/types.py
 isic_cli/cli/user.py
```

### Comparing `isic-cli-6.1.0/pyproject.toml` & `isic-cli-6.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/setup.py` & `isic-cli-6.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/tests/conftest.py` & `isic-cli-6.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/tests/test_cli_base.py` & `isic-cli-6.2.0/tests/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/tests/test_cli_collection.py` & `isic-cli-6.2.0/tests/test_cli_collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/tests/test_cli_image.py` & `isic-cli-6.2.0/tests/test_cli_image.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/tests/test_cli_metadata.py` & `isic-cli-6.2.0/tests/test_cli_metadata.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/tests/test_utils.py` & `isic-cli-6.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-6.1.0/tox.ini` & `isic-cli-6.2.0/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -23,17 +23,35 @@
     pytest-mock
 commands =
     pytest {posargs}
 
 [testenv:type]
 skipsdist = true
 skip_install = true
+deps =
+    pyright
 commands =
     pyright {posargs:.}
 
+[testenv:package]
+deps =
+    pyinstaller
+commands =
+    pyinstaller \
+        --clean \
+        --noconfirm \
+        --onefile \
+        --name isic \
+        --recursive-copy-metadata isic_cli \
+        --collect-data isic_cli \
+        --specpath {env_tmp_dir} \
+        --workpath {env_tmp_dir} \
+        --collect-all dateutil \
+        {env_site_packages_dir}/isic_cli/cli/__main__.py
+
 [testenv:format]
 skipsdist = true
 skip_install = true
 deps =
     black
     isort
 commands =
```


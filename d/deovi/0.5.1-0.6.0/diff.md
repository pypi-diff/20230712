# Comparing `tmp/deovi-0.5.1.tar.gz` & `tmp/deovi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deovi-0.5.1.tar", last modified: Tue Mar  7 02:38:49 2023, max compression
+gzip compressed data, was "deovi-0.6.0.tar", last modified: Wed Jul 12 20:41:16 2023, max compression
```

## Comparing `deovi-0.5.1.tar` & `deovi-0.6.0.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-03-07 02:38:49.712889 deovi-0.5.1/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1075 2022-09-12 23:01:15.000000 deovi-0.5.1/LICENCE.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      173 2022-09-12 23:01:15.000000 deovi-0.5.1/MANIFEST.in
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1468 2023-03-07 02:38:49.712889 deovi-0.5.1/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      689 2023-03-07 02:37:37.000000 deovi-0.5.1/README.rst
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-03-07 02:38:49.708889 deovi-0.5.1/deovi/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      686 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-03-07 02:38:49.708889 deovi-0.5.1/deovi/cli/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/cli/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1940 2023-03-07 02:37:37.000000 deovi-0.5.1/deovi/cli/collect.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1768 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/cli/entrypoint.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1117 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/cli/job.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1837 2023-03-04 01:47:57.000000 deovi-0.5.1/deovi/cli/rename.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      232 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/cli/version.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-03-07 02:38:49.708889 deovi-0.5.1/deovi/collector/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      409 2023-03-04 01:47:57.000000 deovi-0.5.1/deovi/collector/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    16743 2023-03-07 02:37:37.000000 deovi-0.5.1/deovi/collector/collect.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1150 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/exceptions.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1128 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/logger.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-03-07 02:38:49.712889 deovi-0.5.1/deovi/renamer/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/renamer/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    10871 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/renamer/jobs.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4581 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/renamer/printer.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4505 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/renamer/runner.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    11870 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/renamer/tasks.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5033 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/renamer/validators.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-03-07 02:38:49.712889 deovi-0.5.1/deovi/utils/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/utils/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2348 2023-03-07 02:37:37.000000 deovi-0.5.1/deovi/utils/checksum.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      643 2022-09-12 23:01:15.000000 deovi-0.5.1/deovi/utils/jsons.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1208 2023-03-07 02:37:37.000000 deovi-0.5.1/deovi/utils/tests.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-03-07 02:38:49.708889 deovi-0.5.1/deovi.egg-info/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1468 2023-03-07 02:38:49.000000 deovi-0.5.1/deovi.egg-info/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      725 2023-03-07 02:38:49.000000 deovi-0.5.1/deovi.egg-info/SOURCES.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-03-07 02:38:49.000000 deovi-0.5.1/deovi.egg-info/dependency_links.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       60 2023-03-07 02:38:49.000000 deovi-0.5.1/deovi.egg-info/entry_points.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      181 2023-03-07 02:38:49.000000 deovi-0.5.1/deovi.egg-info/requires.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        6 2023-03-07 02:38:49.000000 deovi-0.5.1/deovi.egg-info/top_level.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-03-04 01:42:58.000000 deovi-0.5.1/deovi.egg-info/zip-safe
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1419 2023-03-07 02:38:49.712889 deovi-0.5.1/setup.cfg
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2022-09-12 23:01:15.000000 deovi-0.5.1/setup.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1075 2022-09-12 23:01:15.000000 deovi-0.6.0/LICENCE.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      173 2022-09-12 23:01:15.000000 deovi-0.6.0/MANIFEST.in
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1784 2023-07-12 20:41:16.054276 deovi-0.6.0/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      979 2023-07-12 20:40:49.000000 deovi-0.6.0/README.rst
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/deovi/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      686 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/deovi/cli/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/cli/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1940 2023-03-07 02:37:37.000000 deovi-0.6.0/deovi/cli/collect.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1860 2023-07-12 20:40:49.000000 deovi-0.6.0/deovi/cli/entrypoint.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1117 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/cli/job.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1751 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/cli/rename.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3794 2023-07-12 20:40:49.000000 deovi-0.6.0/deovi/cli/scrap.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      232 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/cli/version.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/deovi/collector/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      463 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/collector/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    13819 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/collector/collect.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6637 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/collector/storage.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1150 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/exceptions.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1128 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/logger.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/deovi/renamer/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/renamer/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    10871 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/renamer/jobs.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4685 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/renamer/printer.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4505 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/renamer/runner.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    11870 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/renamer/tasks.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5033 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/renamer/validators.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6193 2023-07-12 20:40:49.000000 deovi-0.6.0/deovi/scrapper.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/deovi/utils/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2022-09-12 23:01:15.000000 deovi-0.6.0/deovi/utils/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4720 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/utils/checksum.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      717 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/utils/jsons.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3347 2023-05-09 00:34:27.000000 deovi-0.6.0/deovi/utils/tests.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-12 20:41:16.054276 deovi-0.6.0/deovi.egg-info/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1784 2023-07-12 20:41:16.000000 deovi-0.6.0/deovi.egg-info/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      789 2023-07-12 20:41:16.000000 deovi-0.6.0/deovi.egg-info/SOURCES.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-07-12 20:41:16.000000 deovi-0.6.0/deovi.egg-info/dependency_links.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       60 2023-07-12 20:41:16.000000 deovi-0.6.0/deovi.egg-info/entry_points.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      234 2023-07-12 20:41:16.000000 deovi-0.6.0/deovi.egg-info/requires.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        6 2023-07-12 20:41:16.000000 deovi-0.6.0/deovi.egg-info/top_level.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-03-04 01:42:58.000000 deovi-0.6.0/deovi.egg-info/zip-safe
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1482 2023-07-12 20:41:16.058276 deovi-0.6.0/setup.cfg
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2022-09-12 23:01:15.000000 deovi-0.6.0/setup.py
```

### Comparing `deovi-0.5.1/LICENCE.txt` & `deovi-0.6.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `deovi-0.5.1/PKG-INFO` & `deovi-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deovi
-Version: 0.5.1
+Version: 0.6.0
 Summary: Utility to rename files and collect their filepaths
 Home-page: https://github.com/sveetch/deovi
 Author: David Thenon
 Author-email: sveetch@gmail.com
 License: MIT
 Keywords: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,25 +12,29 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
+Provides-Extra: scrapping
 Provides-Extra: dev
 Provides-Extra: quality
 Provides-Extra: doc
 Provides-Extra: release
 License-File: LICENCE.txt
 
 .. _Python: https://www.python.org/
 .. _Click: https://click.palletsprojects.com
 .. _Python Slugify: https://github.com/un33k/python-slugify
 .. _Unidecode: https://github.com/avian2/unidecode/tree/master/unidecode
 .. _PyYAML: https://github.com/yaml/pyyaml/
+.. _deepdiff: https://github.com/seperman/deepdiff
+.. _tmdbv3api: https://github.com/AnthonyBloomer/tmdbv3api
+.. _requests: https://requests.readthedocs.io/en/latest/
 
 =====
 Deovi
 =====
 
 A set of utilities to collect and rename media files.
 
@@ -40,12 +44,18 @@
 * Read the documentation on `Read the docs <https://deovi.readthedocs.io/>`_;
 * Download its `PyPi package <https://pypi.python.org/pypi/deovi>`_;
 * Clone it on its `Github repository <https://github.com/sveetch/deovi>`_;
 
 Dependancies
 ************
 
-* `Python`_>=3.8;
-* `Click`_>=8.0;
-* `Python Slugify`_>= 5.0.0;
+* `Python`_ >=3.8;
+* `Click`_ >=8.0;
+* `Python Slugify`_ >=5.0.0;
 * `Unidecode`_;
 * `PyYAML`_;
+
+And optional dependancies when ``scrapping`` feature is enabled:
+
+* `deepdiff`_;
+* `tmdbv3api`_ ==1.7.7;
+* `requests`_;
```

### Comparing `deovi-0.5.1/deovi/__init__.py` & `deovi-0.6.0/deovi/__init__.py`

 * *Files identical despite different names*

### Comparing `deovi-0.5.1/deovi/cli/collect.py` & `deovi-0.6.0/deovi/cli/collect.py`

 * *Files identical despite different names*

### Comparing `deovi-0.5.1/deovi/cli/entrypoint.py` & `deovi-0.6.0/deovi/cli/entrypoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import click
 
 from ..logger import init_logger
 from ..cli.version import version_command
 from ..cli.rename import rename_command
 from ..cli.job import job_command
 from ..cli.collect import collect_command
+from ..cli.scrap import scrap_command
 
 
 # Help alias on "-h" argument
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
 # Default logger conf
@@ -61,7 +62,8 @@
 
 
 # Attach commands methods to the main grouper
 cli_frontend.add_command(version_command, name="version")
 cli_frontend.add_command(rename_command, name="rename")
 cli_frontend.add_command(job_command, name="job")
 cli_frontend.add_command(collect_command, name="collect")
+cli_frontend.add_command(scrap_command, name="scrap")
```

### Comparing `deovi-0.5.1/deovi/cli/job.py` & `deovi-0.6.0/deovi/cli/job.py`

 * *Files identical despite different names*

### Comparing `deovi-0.5.1/deovi/cli/rename.py` & `deovi-0.6.0/deovi/cli/rename.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,15 @@
 
     A job file is a JSON file with some parameters and tasks to define formatting. Job
     does not recursively walk on files from its basepath directory.
 
     Default behavior is to not change anything, just list task it would do and
     you need to enable commit with the '--commit' argument.
 
-    You can't mix job and init modes and so mix Job filepath and directory
-    paths.
-
-    Finally, if any job task fails all renamed file will be reversed to their
+    Finally, if any job task fails all renamed files will be reversed to their
     original filename.
     """
     logger = logging.getLogger("deovi")
 
     if not jobs:
         logger.critical("There is no job file to process.")
         raise click.Abort()
```

### Comparing `deovi-0.5.1/deovi/collector/collect.py` & `deovi-0.6.0/deovi/collector/collect.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import datetime
-import hashlib
 import json
-import shutil
-import uuid
-from pathlib import Path
 
 import yaml
 
 from ..renamer.printer import PrinterInterface
 from ..utils.jsons import ExtendedJsonEncoder
-from ..utils.checksum import directory_payload_checksum
+from ..utils.checksum import ChecksumOperator
 from ..exceptions import CollectorError
-
+from .storage import AssetStorage
 
 # Non exhaustive list of Video containers with their file extension and name
-# TODO: Should also describe some music only containers
+# NOTE: May also describe some music only containers
 MEDIAS_CONTAINERS = {
     "3gp": "3GPP",
     "asf": "Advanced Systems Format",
     "avi": "AVI",
     "flv": "Flash Video",
     "f4v": "Flash Video",
     "mov": "QuickTime",
@@ -83,17 +79,14 @@
     """
     Collect informations about media files.
 
     Attributes:
         registry (dict): The registry where is collected all informations from scanning.
         stats (dict): Global statistics for all collected directories, files and total
             size.
-        file_storage_directory (string): A directory path where to store collected
-            files. It will be filled from ``run()`` method using the dump filename as
-            its base name.
         file_storage_queue (list): A list where each item is a tuple with source and
             destination to use for copying files.
 
     Arguments:
         basepath (pathlib.Path): The base directory for all directories to scan.
             Directories does not have to start directly from the basepath but must
             start from it.
@@ -115,22 +108,22 @@
             By default this is True and so covers are managed and dumped.
     """
     def __init__(self, basepath, extensions=MEDIAS_EXTENSIONS, allow_empty_dir=False,
                  manifest=MANIFEST_FILENAME, cover_name=COVER_NAME,
                  cover_extensions=COVER_EXTENSIONS, allow_media_cover=True):
         super().__init__()
 
+        self.checksum_op = ChecksumOperator()
         self.basepath = basepath
         self.extensions = extensions
         self.allow_empty_dir = allow_empty_dir
         self.manifest_filename = manifest
         self.cover_name = cover_name
         self.cover_extensions = cover_extensions
         self.allow_media_cover = allow_media_cover
-        self.file_storage_directory = None
         self.file_storage_queue = []
 
         # Build elligible file names for cover from cover base file name and enabled
         # cover extensions
         self.cover_files = [
             self.cover_name + item
             for item in self.cover_extensions
@@ -142,15 +135,15 @@
         """
         Reset registry and global states.
 
         This is the method to use if you plan to make multiple usage of ``run`` or
         ``scan_directory`` for different basepath since registry and global states are
         cumulative.
         """
-        self.file_storage_directory = None
+        self.storage = AssetStorage(allowed_cover_filenames=self.cover_files)
         self.file_storage_queue = []
 
         self.registry = {}
         self.stats = {
             "directories": 0,
             "files": 0,
             "size": 0,
@@ -177,31 +170,48 @@
         Process field fields
 
         File field are collected as a tuple with file source path and destination path
         but only the destination path will be stored. The source path will just be
         used to copy the file source to its destination.
 
         Copying source file to destination is done through a queue to be performed
-        after the end of collection, storage and dump.
+        after the end of collection.
 
         At this stage, we don't validate if a file item exist or not, since it has
-        already by done during collection.
+        already be done during collection.
 
         Returns:
             dict: Given data possibly patched on file fields. Patch fields are
                 transformed to just keep the final file path (not the original one).
         """
         for field in fields:
             if data.get(field):
                 source, destination = data.get(field)
                 self.file_storage_queue.append((source, destination))
                 data[field] = destination
 
         return data
 
+    def store(self, data):
+        """
+        Store given directory data.
+
+        Arguments:
+            data (dict): The data payload to store. It must have at least a ``path``
+                item which will be used as the item key in the store.
+
+        Returns:
+            string: Item key name used to store the data.
+        """
+        key = str(data["path"].relative_to(self.basepath))
+
+        self.registry[key] = self._process_file_fields(["cover"], data)
+
+        return key
+
     def scan_file(self, path):
         """
         Scan a media file to get its informations.
 
         Implemention does not support file without any suffix (file extension).
 
         Arguments:
@@ -241,47 +251,14 @@
         }
 
         self.stats["files"] += 1
         self.stats["size"] += data["size"]
 
         return data
 
-    def get_directory_cover(self, path):
-        """
-        Search for a directory cover image in given path.
-
-        The filename must match an expected cover filename and must exists.
-
-        Arguments:
-            path (pathlib.Path): A Path object for the directory where to find
-                cover image file.
-
-        Returns:
-            tuple: A tuple of two items ``(source, destination)`` where source is the
-                source cover file (Path object) and destination a filename (Path object)
-                with a uuid4 instead of source file name but keeping source extension.
-        """
-        for filename in self.cover_files:
-            filepath = path / filename
-
-            if filepath.exists():
-                base_storage = (
-                    ""
-                    if not self.file_storage_directory
-                    else self.file_storage_directory
-                )
-                return (
-                    filepath.resolve(),
-                    base_storage / Path(
-                        "".join([str(uuid.uuid4()), filepath.suffix])
-                    ),
-                )
-
-        return None
-
     def get_directory_manifest(self, path):
         """
         Search for a YAML manifest to load medias informations related to
         given directory path.
 
         It should be safe to run with invalid manifests.
 
@@ -317,40 +294,18 @@
                         ", ".join(reserved),
                         str(manifest_path),
                     ))
                     manifest = {}
 
         return manifest
 
-    def store(self, data):
-        """
-        Store given directory data.
-
-        Arguments:
-            data (dict): The data payload to store. It must have at least a ``path``
-                item which will be used as the item key in the store.
-
-        Returns:
-            string: Item key name used to store the data.
-        """
-        key = str(data["path"].relative_to(self.basepath))
-
-        self.registry[key] = self._process_file_fields(["cover"], data)
-
-        return key
-
     def scan_directory(self, path, checksum=False):
         """
         Scan a directory to get its media files.
 
-        TODO: Implement directory checksum
-
-        Does not return anything, the directories informations (and possible media files
-        informations) are stored in ``Collector.registry``.
-
         Arguments:
             path (pathlib.Path): Directory to scan for informations, for direct children
                 files and to recursively search for children directories.
 
         Raises:
             CollectorError: If given path is not a directory inside
                 basepath directory.
@@ -393,101 +348,58 @@
             self.stats["size"] += data["size"]
 
             # Get possible manifest to extend data
             data.update(**self.get_directory_manifest(path))
 
             # Discover cover if any
             if self.allow_media_cover:
-                data["cover"] = self.get_directory_cover(path)
+                data["cover"] = self.storage.get_directory_cover(path)
 
             # Perform content checksum if enabled
             if checksum:
-                data["checksum"] = directory_payload_checksum(
+                # Add file checksums
+                self.checksum_op.payload_files(
                     data,
                     files_fields=["cover"],
-                    storage=self.file_storage_directory,
+                    storage=self.storage.storage_path,
+                )
+                # Then build directory info checksum
+                data["checksum"] = self.checksum_op.directory_payload(
+                    data,
+                    files_fields=["cover"],
+                    storage=self.storage.storage_path,
                 )
 
             # Store collected data
             self.store(data)
 
         return data
 
-    def get_directory_storage(self, filepath):
-        """
-        Compute storage directory name from given filename and current datetime.
-
-        Keyword Arguments:
-            filepath (pathlib.Path): A file path, commonly without any directory path,
-                if there is any directory path it is ignored, only the filename is used
-                to compute return filename.
-
-        Returns:
-            pathlib.Path: A filename composed from the filepath filename (without dirs
-            or extension) and a computed unique hash.
-        """
-        if not filepath:
-            return None
-
-        file_hash = hashlib.blake2b(
-            "{}_{}".format(
-                filepath.name,
-                datetime.datetime.now().isoformat(),
-            ).encode("utf-8"),
-            digest_size=10
-        ).hexdigest()
-
-        return filepath.parent / Path("{}_{}".format(filepath.stem, file_hash))
-
-    def store_files(self, files):
-        """
-        Store files from given list to their destination.
-
-        Arguments:
-            files (list): List of tuple ``(source, destination)`` where both items are
-                Path objects as returned from ``Collector.get_directory_cover()``.
-
-        Returns:
-            list: List of stored file in their final destination.
-        """
-        stored = []
-
-        if len(files) > 0:
-            if not self.file_storage_directory.exists():
-                self.file_storage_directory.mkdir(parents=True, exist_ok=True)
-
-            for source, destination in files:
-                if not source.exists():
-                    msg = "File to store does not exists from your filesystem: {}"
-                    self.log_warning(msg.format(source))
-
-                shutil.copy(source, destination)
-                stored.append(destination)
-
-        return stored
-
     def run(self, destination=None, checksum=False):
         """
         Recursively scan everything from basepath to produce a registry of collected
         informations.
 
         Keyword Arguments:
             destination (pathlib.Path): Destination path to write a JSON file with
-                every collected informations. Default is ``None`` so no JSON registry
+                every collected informations. Default is ``None`` so no JSON dump
                 file will be written to the filesystem.
+            checksum (boolean): Whether to enable directory checksums or not. Default
+                to False, no checksum are done.
 
         Returns:
             dict: Dictionnary of global states for collected directories and files.
         """
-        self.file_storage_directory = self.get_directory_storage(destination)
+        # Set storage basepath from destination location
+        self.storage.set_basepath(destination, checksum=checksum)
 
         self.scan_directory(self.basepath, checksum=checksum)
 
         if self.registry and destination:
             with destination.open("w") as fp:
                 json.dump(self.registry, fp, indent=4, cls=ExtendedJsonEncoder)
                 self.log_info("Registry saved to: {}".format(str(destination)))
 
             # Proceed to copy queued files into storage dir
-            self.store_files(self.file_storage_queue)
+            self.storage.store_assets(self.file_storage_queue)
 
         return self.stats
```

### Comparing `deovi-0.5.1/deovi/exceptions.py` & `deovi-0.6.0/deovi/exceptions.py`

 * *Files identical despite different names*

### Comparing `deovi-0.5.1/deovi/logger.py` & `deovi-0.6.0/deovi/logger.py`

 * *Files identical despite different names*

### Comparing `deovi-0.5.1/deovi/renamer/jobs.py` & `deovi-0.6.0/deovi/renamer/jobs.py`

 * *Files identical despite different names*

### Comparing `deovi-0.5.1/deovi/renamer/printer.py` & `deovi-0.6.0/deovi/renamer/printer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 class PrinterInterface:
     """
     Printer interface to output messages.
 
     This is a common interface for objects to use logging and optional message
     formatting.
+
+    TODO: This is common to other module, it need to be moved to utils or elsewhere
+    more "common".
     """
 
     def __init__(self, *args, **kwargs):
         self.logger = logging.getLogger("deovi")
         self.max_label = 0
 
     def set_label_length(self, tasks):
```

### Comparing `deovi-0.5.1/deovi/renamer/runner.py` & `deovi-0.6.0/deovi/renamer/runner.py`

 * *Files identical despite different names*

### Comparing `deovi-0.5.1/deovi/renamer/tasks.py` & `deovi-0.6.0/deovi/renamer/tasks.py`

 * *Files identical despite different names*

### Comparing `deovi-0.5.1/deovi/renamer/validators.py` & `deovi-0.6.0/deovi/renamer/validators.py`

 * *Files identical despite different names*

### Comparing `deovi-0.5.1/deovi/utils/jsons.py` & `deovi-0.6.0/deovi/utils/jsons.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 
 class ExtendedJsonEncoder(json.JSONEncoder):
     """
     Additional opiniated support for more basic object types.
     """
     def default(self, obj):
+        if isinstance(obj, bytes):
+            return obj.decode("utf-8")
         # Support for pathlib.Path to a string
         if isinstance(obj, Path):
             return str(obj)
         # Support for set to a list
         if isinstance(obj, set):
             return list(obj)
         if isinstance(obj, (datetime.datetime, datetime.date, datetime.time)):
```

### Comparing `deovi-0.5.1/deovi.egg-info/PKG-INFO` & `deovi-0.6.0/deovi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deovi
-Version: 0.5.1
+Version: 0.6.0
 Summary: Utility to rename files and collect their filepaths
 Home-page: https://github.com/sveetch/deovi
 Author: David Thenon
 Author-email: sveetch@gmail.com
 License: MIT
 Keywords: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,25 +12,29 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
+Provides-Extra: scrapping
 Provides-Extra: dev
 Provides-Extra: quality
 Provides-Extra: doc
 Provides-Extra: release
 License-File: LICENCE.txt
 
 .. _Python: https://www.python.org/
 .. _Click: https://click.palletsprojects.com
 .. _Python Slugify: https://github.com/un33k/python-slugify
 .. _Unidecode: https://github.com/avian2/unidecode/tree/master/unidecode
 .. _PyYAML: https://github.com/yaml/pyyaml/
+.. _deepdiff: https://github.com/seperman/deepdiff
+.. _tmdbv3api: https://github.com/AnthonyBloomer/tmdbv3api
+.. _requests: https://requests.readthedocs.io/en/latest/
 
 =====
 Deovi
 =====
 
 A set of utilities to collect and rename media files.
 
@@ -40,12 +44,18 @@
 * Read the documentation on `Read the docs <https://deovi.readthedocs.io/>`_;
 * Download its `PyPi package <https://pypi.python.org/pypi/deovi>`_;
 * Clone it on its `Github repository <https://github.com/sveetch/deovi>`_;
 
 Dependancies
 ************
 
-* `Python`_>=3.8;
-* `Click`_>=8.0;
-* `Python Slugify`_>= 5.0.0;
+* `Python`_ >=3.8;
+* `Click`_ >=8.0;
+* `Python Slugify`_ >=5.0.0;
 * `Unidecode`_;
 * `PyYAML`_;
+
+And optional dependancies when ``scrapping`` feature is enabled:
+
+* `deepdiff`_;
+* `tmdbv3api`_ ==1.7.7;
+* `requests`_;
```

### Comparing `deovi-0.5.1/deovi.egg-info/SOURCES.txt` & `deovi-0.6.0/deovi.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 deovi/__init__.py
 deovi/exceptions.py
 deovi/logger.py
+deovi/scrapper.py
 deovi.egg-info/PKG-INFO
 deovi.egg-info/SOURCES.txt
 deovi.egg-info/dependency_links.txt
 deovi.egg-info/entry_points.txt
 deovi.egg-info/requires.txt
 deovi.egg-info/top_level.txt
 deovi.egg-info/zip-safe
 deovi/cli/__init__.py
 deovi/cli/collect.py
 deovi/cli/entrypoint.py
 deovi/cli/job.py
 deovi/cli/rename.py
+deovi/cli/scrap.py
 deovi/cli/version.py
 deovi/collector/__init__.py
 deovi/collector/collect.py
+deovi/collector/storage.py
 deovi/renamer/__init__.py
 deovi/renamer/jobs.py
 deovi/renamer/printer.py
 deovi/renamer/runner.py
 deovi/renamer/tasks.py
 deovi/renamer/validators.py
 deovi/utils/__init__.py
```

### Comparing `deovi-0.5.1/setup.cfg` & `deovi-0.6.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deovi
-version = 0.5.1
+version = 0.6.0
 description = Utility to rename files and collect their filepaths
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = David Thenon
 author_email = sveetch@gmail.com
 url = https://github.com/sveetch/deovi
 license = MIT
@@ -18,23 +18,27 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 include_package_data = True
 install_requires = 
-	click>=8.0
+	click>=8.0,<9.0
 	colorama
 	colorlog
 	python-slugify[unidecode]
 	PyYAML
 packages = find:
 zip_safe = True
 
 [options.extras_require]
+scrapping = 
+	deepdiff
+	tmdbv3api==1.7.7
+	requests
 dev = 
 	pytest
 	freezegun
 quality = 
 	flake8
 	tox
 doc = 
@@ -71,18 +75,18 @@
 python_files = 
 	*.py
 testpaths = 
 	tests
 
 [tox:tox]
 minversion = 3.4.0
-envlist = py{38,39,310}
+envlist = py{38,310}
 
 [testenv]
 commands = 
-	pip install -e .[dev]
+	pip install -e .[scrapping,dev]
 	pytest -vv tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```


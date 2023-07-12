# Comparing `tmp/download_water_data-0.4.0.tar.gz` & `tmp/download_water_data-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "download_water_data-0.4.0.tar", last modified: Mon Apr 19 11:25:52 2021, max compression
+gzip compressed data, was "download_water_data-0.5.0.tar", last modified: Wed Jul 12 06:48:21 2023, max compression
```

## Comparing `download_water_data-0.4.0.tar` & `download_water_data-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2021-04-19 11:25:52.081594 download_water_data-0.4.0/
--rw-rw-rw-   0        0        0     1074 2021-04-19 10:56:02.000000 download_water_data-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     4449 2021-04-19 11:25:52.081594 download_water_data-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2953 2021-04-19 11:22:01.000000 download_water_data-0.4.0/README.rst
-drwxrwxrwx   0        0        0        0 2021-04-19 11:25:52.061648 download_water_data-0.4.0/download_water_data/
--rw-rw-rw-   0        0        0        0 2017-12-26 06:04:36.000000 download_water_data-0.4.0/download_water_data/__init__.py
--rw-rw-rw-   0        0        0     6115 2021-04-19 11:19:24.000000 download_water_data-0.4.0/download_water_data/__main__.py
-drwxrwxrwx   0        0        0        0 2021-04-19 11:25:52.080597 download_water_data-0.4.0/download_water_data.egg-info/
--rw-rw-rw-   0        0        0     4449 2021-04-19 11:25:52.000000 download_water_data-0.4.0/download_water_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2021-04-19 11:25:52.000000 download_water_data-0.4.0/download_water_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-19 11:25:52.000000 download_water_data-0.4.0/download_water_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2021-04-19 11:25:52.000000 download_water_data-0.4.0/download_water_data.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2021-04-19 11:25:52.000000 download_water_data-0.4.0/download_water_data.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-04-19 11:25:52.081594 download_water_data-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2004 2021-04-19 10:56:02.000000 download_water_data-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 06:48:21.410476 download_water_data-0.5.0/
+-rw-rw-rw-   0        0        0     1074 2023-07-12 06:29:02.000000 download_water_data-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     3798 2023-07-12 06:48:21.409475 download_water_data-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2999 2023-07-12 06:43:40.000000 download_water_data-0.5.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-12 06:48:21.396475 download_water_data-0.5.0/download_water_data/
+-rw-rw-rw-   0        0        0        0 2023-07-12 06:29:02.000000 download_water_data-0.5.0/download_water_data/__init__.py
+-rw-rw-rw-   0        0        0     6255 2023-07-12 06:44:03.000000 download_water_data-0.5.0/download_water_data/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 06:48:21.408476 download_water_data-0.5.0/download_water_data.egg-info/
+-rw-rw-rw-   0        0        0     3798 2023-07-12 06:48:21.000000 download_water_data-0.5.0/download_water_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-07-12 06:48:21.000000 download_water_data-0.5.0/download_water_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 06:48:21.000000 download_water_data-0.5.0/download_water_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-07-12 06:48:21.000000 download_water_data-0.5.0/download_water_data.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-12 06:48:21.000000 download_water_data-0.5.0/download_water_data.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 06:48:21.410476 download_water_data-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1958 2023-07-12 06:32:30.000000 download_water_data-0.5.0/setup.py
```

### Comparing `download_water_data-0.4.0/LICENSE` & `download_water_data-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `download_water_data-0.4.0/PKG-INFO` & `download_water_data-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: download_water_data
-Version: 0.4.0
+Version: 0.5.0
 Summary: Downloader for the Global Surface Water Data of the Copernicus Programme
 Home-page: https://github.com/mentaljam/download_water_data
 Author: Petr Tsymbarovich
 Author-email: petr@tsymbarovich.ru
 License: MIT
-Description: Download Water Data
-        ===================
-        
-        Downloader for the `Global Surface Water`_ data of the Copernicus Programme.
-        
-        It is based on the original downloadWaterData.py.
-        
-        .. image:: https://img.shields.io/pypi/pyversions/download_water_data.svg
-            :target: https://pypi.python.org/pypi/download-water-data
-        
-        .. image:: https://img.shields.io/pypi/v/download-water-data.svg
-            :target: https://pypi.python.org/pypi/download-water-data
-        
-        .. image:: https://img.shields.io/github/issues/mentaljam/download_water_data.svg
-            :target: https://github.com/mentaljam/download_water_data/issues
-        
-        Requirements
-        ------------
-        
-        This tool runs on Windows/Mac/Unix and requires `Python`_ version 2 or 3.
-        
-        Usage
-        -----
-        
-        **Install with** `pip`_
-        
-        - Install the tool with ``python -m pip install download_water_data``
-        - Run the tool with ``python -m download_water_data <arguments>`` or just
-          ``download_water_data <arguments>`` if the Python Scripts directory is in your system ``PATH``
-        
-        **Download without installing**
-        
-        -  Download the `latest`_ ``download_water_data.pyz`` file
-        -  Open a terminal or console
-        -  Run the tool with ``python download_water_data.pyz <arguments>``
-        
-        To **interrupt** tool execution press ``Ctrl+C``.
-        
-        Arguments
-        ---------
-        
-        Possible tool arguments and options can be listed with the ``-h`` option:
-        
-        ::
-        
-            $ download_water_data -h
-        
-            usage: download_water_data.py [-h] [-v] [-d PATH] [-a] [DS [DS ...]]
-        
-            Full Download Script for Global Surface Water Data.
-        
-            positional arguments:
-              DS                    one or more datasets names to download (occurrence,
-                                    change, seasonality, recurrence, transitions, extent),
-                                    use the "-a" option to download all the datasets
-        
-            optional arguments:
-              -h, --help            show this help message and exit
-              -v, --version         show program's version number and exit
-              -d PATH, --directory PATH
-                                    destination directory where to download the data (by
-                                    default the current working directory is used)
-              -r {1_0,1_1,1_1_2019,1_3_2020}, --revision {1_0,1_1,1_1_2019,1_3_2020}
-                                    data revision (default is 1_3_2020)
-              -a, --all             download all datasets (default is false)
-              -f, --force           rewrite existing files (default is false)
-        
-        Examples
-        --------
-        
-        To download the **occurrence** and **change** datasets run
-        
-        ``download_water_data occurrence change``
-        
-        To download all the datasets run
-        
-        ``download_water_data -a``
-        
-        To change the destination directory add the ``-d`` option
-        
-        ``download_water_data -a -d 'download/path'``
-        
-        .. _Global Surface Water: https://global-surface-water.appspot.com
-        .. _Python: https://www.python.org
-        .. _pip: https://pip.pypa.io/en/stable
-        .. _latest: https://github.com/mentaljam/download_water_data/releases/latest
-        
 Keywords: Copernicus global surface water download
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
+License-File: LICENSE
+
+Download Water Data
+===================
+
+Downloader for the `Global Surface Water`_ data of the Copernicus Programme.
+
+It is based on the original downloadWaterData.py.
+
+.. image:: https://img.shields.io/pypi/pyversions/download_water_data.svg
+    :target: https://pypi.python.org/pypi/download-water-data
+
+.. image:: https://img.shields.io/pypi/v/download-water-data.svg
+    :target: https://pypi.python.org/pypi/download-water-data
+
+.. image:: https://img.shields.io/github/issues/mentaljam/download_water_data.svg
+    :target: https://github.com/mentaljam/download_water_data/issues
+
+Requirements
+------------
+
+This tool runs on Windows/Mac/Unix and requires `Python`_ version 2 or 3.
+
+Usage
+-----
+
+**Install with** `pip`_
+
+- Install the tool with ``python -m pip install download_water_data``
+- Run the tool with ``python -m download_water_data <arguments>`` or just
+  ``download_water_data <arguments>`` if the Python Scripts directory is in your system ``PATH``
+
+**Download without installing**
+
+-  Download the `latest`_ ``download_water_data.pyz`` file
+-  Open a terminal or console
+-  Run the tool with ``python download_water_data.pyz <arguments>``
+
+To **interrupt** tool execution press ``Ctrl+C``.
+
+Arguments
+---------
+
+Possible tool arguments and options can be listed with the ``-h`` option:
+
+::
+
+    $ download_water_data -h
+
+    usage: download_water_data [-h] [-v] [-d PATH] [-r {1_0,1_1,1_1_2019,1_3_2020,1_4_2021}] [-a] [-f] [DS ...]
+
+    Full Download Script for Global Surface Water Data.
+
+    positional arguments:
+      DS                    one or more datasets names to download (occurrence,
+                            change, seasonality, recurrence, transitions, extent),
+                            use the "-a" option to download all the datasets
+
+    options:
+      -h, --help            show this help message and exit
+      -v, --version         show program's version number and exit
+      -d PATH, --directory PATH
+                            destination directory where to download the data (by
+                            default the current working directory is used)
+      -r {1_0,1_1,1_1_2019,1_3_2020,1_4_2021}, --revision {1_0,1_1,1_1_2019,1_3_2020,1_4_2021}
+                            data revision (default is 1_4_2021)
+      -a, --all             download all datasets (default is false)
+      -f, --force           rewrite existing files (default is false)
+
+Examples
+--------
+
+To download the **occurrence** and **change** datasets run
+
+``download_water_data occurrence change``
+
+To download all the datasets run
+
+``download_water_data -a``
+
+To change the destination directory add the ``-d`` option
+
+``download_water_data -a -d 'download/path'``
+
+.. _Global Surface Water: https://global-surface-water.appspot.com
+.. _Python: https://www.python.org
+.. _pip: https://pip.pypa.io/en/stable
+.. _latest: https://github.com/mentaljam/download_water_data/releases/latest
```

### Comparing `download_water_data-0.4.0/README.rst` & `download_water_data-0.5.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -41,31 +41,31 @@
 
 Possible tool arguments and options can be listed with the ``-h`` option:
 
 ::
 
     $ download_water_data -h
 
-    usage: download_water_data.py [-h] [-v] [-d PATH] [-a] [DS [DS ...]]
+    usage: download_water_data [-h] [-v] [-d PATH] [-r {1_0,1_1,1_1_2019,1_3_2020,1_4_2021}] [-a] [-f] [DS ...]
 
     Full Download Script for Global Surface Water Data.
 
     positional arguments:
       DS                    one or more datasets names to download (occurrence,
                             change, seasonality, recurrence, transitions, extent),
                             use the "-a" option to download all the datasets
 
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       -v, --version         show program's version number and exit
       -d PATH, --directory PATH
                             destination directory where to download the data (by
                             default the current working directory is used)
-      -r {1_0,1_1,1_1_2019,1_3_2020}, --revision {1_0,1_1,1_1_2019,1_3_2020}
-                            data revision (default is 1_3_2020)
+      -r {1_0,1_1,1_1_2019,1_3_2020,1_4_2021}, --revision {1_0,1_1,1_1_2019,1_3_2020,1_4_2021}
+                            data revision (default is 1_4_2021)
       -a, --all             download all datasets (default is false)
       -f, --force           rewrite existing files (default is false)
 
 Examples
 --------
 
 To download the **occurrence** and **change** datasets run
```

### Comparing `download_water_data-0.4.0/download_water_data/__main__.py` & `download_water_data-0.5.0/download_water_data/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 https://global-surface-water.appspot.com/download
 
 Based on the original downloadWaterData.py'''
 
 __author__ = 'Petr Tsymbarovich'
 __email__ = 'petr@tsymbarovich.ru'
 __license__ = 'MIT'
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 
 import sys
 import signal
 import os
 import argparse
 if sys.version_info.major == 2:
     # Python 2
@@ -20,23 +20,23 @@
     from urllib2 import HTTPError
 else:
     # Python 3
     from urllib.request import urlretrieve
     from urllib.error import HTTPError
 
 
-KNOWN_DATASETS = ['occurrence', 'change', 'seasonality', 'recurrence', 'transitions', 'extent']
-REVISIONS = ['1_0', '1_1', '1_1_2019', '1_3_2020']
+KNOWN_DATASETS = 'occurrence', 'change', 'seasonality', 'recurrence', 'transitions', 'extent'
+REVISIONS = '1_0', '1_1', '1_1_2019', '1_3_2020', '1_4_2021'
 _GLOBALS = {}
 
 
 def templates(revision):
     '''Configure URL and file templates'''
 
-    v10, v11, v11_2019, v13_2020 = REVISIONS
+    v10, v11, v11_2019, v13_2020, v14_2021 = REVISIONS
     url_tmpl  = 'http://storage.googleapis.com/global-surface-water/downloads'
     file_tmpl = '{ds}_{lon}_{lat}'
     if revision == v10:
         padding   = 15
     elif revision == v11:
         url_tmpl  += '2'
         file_tmpl += '_v' + v11
@@ -45,14 +45,18 @@
         url_tmpl  += '2019v2'
         file_tmpl += 'v' + v11_2019
         padding   = 24
     elif revision == v13_2020:
         url_tmpl  += '2020'
         file_tmpl += 'v' + v13_2020
         padding   = 24
+    elif revision == v14_2021:
+        url_tmpl  += '2021'
+        file_tmpl += 'v' + v14_2021
+        padding   = 24
     url_tmpl  += '/{ds}/{file}'
     file_tmpl += '.tif'
     return (url_tmpl, file_tmpl, padding)
 
 
 def sigint_handler(signum, frame):
     '''Handler for interruption signal (Ctrl+C).'''
```

### Comparing `download_water_data-0.4.0/download_water_data.egg-info/PKG-INFO` & `download_water_data-0.5.0/download_water_data.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: download-water-data
-Version: 0.4.0
+Version: 0.5.0
 Summary: Downloader for the Global Surface Water Data of the Copernicus Programme
 Home-page: https://github.com/mentaljam/download_water_data
 Author: Petr Tsymbarovich
 Author-email: petr@tsymbarovich.ru
 License: MIT
-Description: Download Water Data
-        ===================
-        
-        Downloader for the `Global Surface Water`_ data of the Copernicus Programme.
-        
-        It is based on the original downloadWaterData.py.
-        
-        .. image:: https://img.shields.io/pypi/pyversions/download_water_data.svg
-            :target: https://pypi.python.org/pypi/download-water-data
-        
-        .. image:: https://img.shields.io/pypi/v/download-water-data.svg
-            :target: https://pypi.python.org/pypi/download-water-data
-        
-        .. image:: https://img.shields.io/github/issues/mentaljam/download_water_data.svg
-            :target: https://github.com/mentaljam/download_water_data/issues
-        
-        Requirements
-        ------------
-        
-        This tool runs on Windows/Mac/Unix and requires `Python`_ version 2 or 3.
-        
-        Usage
-        -----
-        
-        **Install with** `pip`_
-        
-        - Install the tool with ``python -m pip install download_water_data``
-        - Run the tool with ``python -m download_water_data <arguments>`` or just
-          ``download_water_data <arguments>`` if the Python Scripts directory is in your system ``PATH``
-        
-        **Download without installing**
-        
-        -  Download the `latest`_ ``download_water_data.pyz`` file
-        -  Open a terminal or console
-        -  Run the tool with ``python download_water_data.pyz <arguments>``
-        
-        To **interrupt** tool execution press ``Ctrl+C``.
-        
-        Arguments
-        ---------
-        
-        Possible tool arguments and options can be listed with the ``-h`` option:
-        
-        ::
-        
-            $ download_water_data -h
-        
-            usage: download_water_data.py [-h] [-v] [-d PATH] [-a] [DS [DS ...]]
-        
-            Full Download Script for Global Surface Water Data.
-        
-            positional arguments:
-              DS                    one or more datasets names to download (occurrence,
-                                    change, seasonality, recurrence, transitions, extent),
-                                    use the "-a" option to download all the datasets
-        
-            optional arguments:
-              -h, --help            show this help message and exit
-              -v, --version         show program's version number and exit
-              -d PATH, --directory PATH
-                                    destination directory where to download the data (by
-                                    default the current working directory is used)
-              -r {1_0,1_1,1_1_2019,1_3_2020}, --revision {1_0,1_1,1_1_2019,1_3_2020}
-                                    data revision (default is 1_3_2020)
-              -a, --all             download all datasets (default is false)
-              -f, --force           rewrite existing files (default is false)
-        
-        Examples
-        --------
-        
-        To download the **occurrence** and **change** datasets run
-        
-        ``download_water_data occurrence change``
-        
-        To download all the datasets run
-        
-        ``download_water_data -a``
-        
-        To change the destination directory add the ``-d`` option
-        
-        ``download_water_data -a -d 'download/path'``
-        
-        .. _Global Surface Water: https://global-surface-water.appspot.com
-        .. _Python: https://www.python.org
-        .. _pip: https://pip.pypa.io/en/stable
-        .. _latest: https://github.com/mentaljam/download_water_data/releases/latest
-        
 Keywords: Copernicus global surface water download
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
+License-File: LICENSE
+
+Download Water Data
+===================
+
+Downloader for the `Global Surface Water`_ data of the Copernicus Programme.
+
+It is based on the original downloadWaterData.py.
+
+.. image:: https://img.shields.io/pypi/pyversions/download_water_data.svg
+    :target: https://pypi.python.org/pypi/download-water-data
+
+.. image:: https://img.shields.io/pypi/v/download-water-data.svg
+    :target: https://pypi.python.org/pypi/download-water-data
+
+.. image:: https://img.shields.io/github/issues/mentaljam/download_water_data.svg
+    :target: https://github.com/mentaljam/download_water_data/issues
+
+Requirements
+------------
+
+This tool runs on Windows/Mac/Unix and requires `Python`_ version 2 or 3.
+
+Usage
+-----
+
+**Install with** `pip`_
+
+- Install the tool with ``python -m pip install download_water_data``
+- Run the tool with ``python -m download_water_data <arguments>`` or just
+  ``download_water_data <arguments>`` if the Python Scripts directory is in your system ``PATH``
+
+**Download without installing**
+
+-  Download the `latest`_ ``download_water_data.pyz`` file
+-  Open a terminal or console
+-  Run the tool with ``python download_water_data.pyz <arguments>``
+
+To **interrupt** tool execution press ``Ctrl+C``.
+
+Arguments
+---------
+
+Possible tool arguments and options can be listed with the ``-h`` option:
+
+::
+
+    $ download_water_data -h
+
+    usage: download_water_data [-h] [-v] [-d PATH] [-r {1_0,1_1,1_1_2019,1_3_2020,1_4_2021}] [-a] [-f] [DS ...]
+
+    Full Download Script for Global Surface Water Data.
+
+    positional arguments:
+      DS                    one or more datasets names to download (occurrence,
+                            change, seasonality, recurrence, transitions, extent),
+                            use the "-a" option to download all the datasets
+
+    options:
+      -h, --help            show this help message and exit
+      -v, --version         show program's version number and exit
+      -d PATH, --directory PATH
+                            destination directory where to download the data (by
+                            default the current working directory is used)
+      -r {1_0,1_1,1_1_2019,1_3_2020,1_4_2021}, --revision {1_0,1_1,1_1_2019,1_3_2020,1_4_2021}
+                            data revision (default is 1_4_2021)
+      -a, --all             download all datasets (default is false)
+      -f, --force           rewrite existing files (default is false)
+
+Examples
+--------
+
+To download the **occurrence** and **change** datasets run
+
+``download_water_data occurrence change``
+
+To download all the datasets run
+
+``download_water_data -a``
+
+To change the destination directory add the ``-d`` option
+
+``download_water_data -a -d 'download/path'``
+
+.. _Global Surface Water: https://global-surface-water.appspot.com
+.. _Python: https://www.python.org
+.. _pip: https://pip.pypa.io/en/stable
+.. _latest: https://github.com/mentaljam/download_water_data/releases/latest
```

### Comparing `download_water_data-0.4.0/setup.py` & `download_water_data-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 '''Setup script for download_water_data.'''
 
 from distutils import cmd
 import zipapp
-import os.path
+from pathlib import Path
 from setuptools import setup
 from download_water_data.__main__ import __version__
 
-SRC_DIR = os.path.abspath(os.path.dirname(__file__))
+SRC_DIR = Path(__file__).parent
 
 class PyzCommand(cmd.Command):
     '''A custom command to generate download_water_data.pyz.'''
 
     description = 'generate download_water_data.pyz'
     user_options = []
 
@@ -18,29 +18,31 @@
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         '''Run command.'''
-        out_dir = os.path.join(SRC_DIR, 'dist')
-        if not os.path.isdir(out_dir):
-            os.makedirs(out_dir)
-        with open(os.path.join(SRC_DIR, 'download_water_data', '__main__.py'), 'rb') as main:
-            zipapp.create_archive(main, os.path.join(out_dir, 'download_water_data.pyz'),
-                                  interpreter='/usr/bin/env python')
+        out_dir = SRC_DIR / 'dist'
+        out_dir.mkdir(exist_ok=True)
+        with SRC_DIR.joinpath('download_water_data', '__main__.py').open('rb') as main:
+            zipapp.create_archive(
+                source=main,
+                target=out_dir / 'download_water_data.pyz',
+                interpreter='/usr/bin/env python',
+            )
 
 setup(
     cmdclass={
         'pyz': PyzCommand,
     },
     name='download_water_data',
     version=__version__,
     description='Downloader for the Global Surface Water Data of the Copernicus Programme',
-    long_description=open(os.path.join(SRC_DIR, 'README.rst'), 'r').read(),
+    long_description=SRC_DIR.joinpath('README.rst').read_text(),
     url='https://github.com/mentaljam/download_water_data',
     author='Petr Tsymbarovich',
     author_email='petr@tsymbarovich.ru',
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
```


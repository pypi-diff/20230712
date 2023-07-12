# Comparing `tmp/pyipsw-0.0.1.tar.gz` & `tmp/pyipsw-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyipsw-0.0.1.tar", last modified: Thu Jul 15 14:24:43 2021, max compression
+gzip compressed data, was "pyipsw-0.0.2.tar", last modified: Wed Jul 12 06:07:38 2023, max compression
```

## Comparing `pyipsw-0.0.1.tar` & `pyipsw-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 14:24:43.430554 pyipsw-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-07-15 14:24:32.000000 pyipsw-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5143 2021-07-15 14:24:43.430554 pyipsw-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3908 2021-07-15 14:24:32.000000 pyipsw-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 14:24:43.426554 pyipsw-0.0.1/pyipsw/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-15 14:24:32.000000 pyipsw-0.0.1/pyipsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-07-15 14:24:32.000000 pyipsw-0.0.1/pyipsw/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1971 2021-07-15 14:24:32.000000 pyipsw-0.0.1/pyipsw/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4914 2021-07-15 14:24:32.000000 pyipsw-0.0.1/pyipsw/pyipsw.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-15 14:24:43.426554 pyipsw-0.0.1/pyipsw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5143 2021-07-15 14:24:43.000000 pyipsw-0.0.1/pyipsw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-07-15 14:24:43.000000 pyipsw-0.0.1/pyipsw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-15 14:24:43.000000 pyipsw-0.0.1/pyipsw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-07-15 14:24:43.000000 pyipsw-0.0.1/pyipsw.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-07-15 14:24:43.000000 pyipsw-0.0.1/pyipsw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-07-15 14:24:43.000000 pyipsw-0.0.1/pyipsw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-07-15 14:24:32.000000 pyipsw-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-15 14:24:43.430554 pyipsw-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2021-07-15 14:24:32.000000 pyipsw-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:07:38.536712 pyipsw-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-12 06:07:20.000000 pyipsw-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-12 06:07:38.536712 pyipsw-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-12 06:07:20.000000 pyipsw-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:07:38.532712 pyipsw-0.0.2/pyipsw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 06:07:20.000000 pyipsw-0.0.2/pyipsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-12 06:07:20.000000 pyipsw-0.0.2/pyipsw/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-12 06:07:20.000000 pyipsw-0.0.2/pyipsw/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-12 06:07:20.000000 pyipsw-0.0.2/pyipsw/pyipsw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:07:38.532712 pyipsw-0.0.2/pyipsw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-12 06:07:38.000000 pyipsw-0.0.2/pyipsw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-12 06:07:38.000000 pyipsw-0.0.2/pyipsw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 06:07:38.000000 pyipsw-0.0.2/pyipsw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-12 06:07:38.000000 pyipsw-0.0.2/pyipsw.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 06:07:38.000000 pyipsw-0.0.2/pyipsw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 06:07:38.000000 pyipsw-0.0.2/pyipsw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-12 06:07:20.000000 pyipsw-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 06:07:20.000000 pyipsw-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 06:07:38.536712 pyipsw-0.0.2/setup.cfg
```

### Comparing `pyipsw-0.0.1/LICENSE` & `pyipsw-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyipsw-0.0.1/README.md` & `pyipsw-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [![Python application](https://github.com/matan1008/pyipsw/workflows/Python%20application/badge.svg)](https://github.com/matan1008/pyipsw/actions/workflows/python-app.yml "Python application action")
 [![Pypi version](https://img.shields.io/pypi/v/pyipsw.svg)](https://pypi.org/project/pyipsw/ "PyPi package")
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/matan1008/pyipsw.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/matan1008/pyipsw/context:python)
 
 - [Description](#description)
 - [Installation](#installation)
 - [Usage](#usage)
     * [CLI](#cli)
 
 # Description
@@ -12,23 +11,23 @@
 `pyipsw` is a utility created in order to access ipsw.me data easily using python / cli.
 
 # Installation
 
 Install the last released version using `pip`:
 
 ```shell
-python3 -m pip install --user -U pyipsw
+python3 -m pip install -U pyipsw
 ```
 
 Or install the latest version from sources:
 
 ```shell
 git clone git@github.com:matan1008/pyipsw.git
 cd pyipsw
-python3 -m pip install --user -U -e .
+python3 -m pip install -U -e .
 ```
 
 # Usage
 
 ## CLI
 
 In order to show data about devices, just run the devices command:
@@ -91,8 +90,8 @@
 ------------------------------------------------------------------------------------
 ```
 
 You can also download the firmwares with:
 
 ```shell
 pyipsw download-devices /tmp/firmwares -f "'iPhone10' in device and '14.4' in version"
-```
+```
```

### Comparing `pyipsw-0.0.1/pyipsw/cli.py` & `pyipsw-0.0.2/pyipsw/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
 from humanfriendly.tables import format_smart_table
 
-from pyipsw.pyipsw import get_devices, DEVICES_FIELDS, get_itunes, ITUNES_FIELDS, download_devices
+from pyipsw.pyipsw import DEVICES_FIELDS, ITUNES_FIELDS, download_devices, get_devices, get_itunes
 
 DEFAULT_DEVICES_COLUMNS = ['device', 'version', 'buildid', 'filename']
 DEFAULT_ITUNES_COLUMNS = ['os', 'version', 'releasedate', 'url']
 
 
 @click.group()
 def cli():
```

### Comparing `pyipsw-0.0.1/pyipsw/pyipsw.py` & `pyipsw-0.0.2/pyipsw/pyipsw.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from functools import lru_cache
 import hashlib
 import os
+from functools import lru_cache
 
-from tqdm import tqdm
 import requests
+from tqdm import tqdm
 
 IPSW_API_FIRMWARES_JSON = 'https://api.ipsw.me/v2.1/firmwares.json/condensed'
 DEVICES_FIELDS = ['device', 'name', 'version', 'buildid', 'url', 'uploaddate', 'size', 'signed', 'sha1sum',
                   'releasedate', 'platform', 'md5sum', 'filename', 'cpid', 'bdid', 'BoardConfig']
 ITUNES_FIELDS = ['os', 'version', 'url', 'releasedate', 'uploaddate', '64biturl']
 DOWNLOAD_CHUNK_SIZE = 8192
```


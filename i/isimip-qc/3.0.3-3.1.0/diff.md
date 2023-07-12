# Comparing `tmp/isimip-qc-3.0.3.tar.gz` & `tmp/isimip-qc-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/isimip-qc-3.0.3.tar", last modified: Fri Jun 30 12:32:15 2023, max compression
+gzip compressed data, was "isimip-qc-3.1.0.tar", last modified: Wed Jul 12 12:01:59 2023, max compression
```

## Comparing `isimip-qc-3.0.3.tar` & `isimip-qc-3.1.0.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 buechner  (2091) users      (100)        0 2023-06-30 12:32:15.000000 isimip-qc-3.0.3/
--rw-r--r--   0 buechner  (2091) users      (100)     1102 2020-08-12 10:35:03.000000 isimip-qc-3.0.3/LICENSE
--rw-r--r--   0 buechner  (2091) users      (100)    12423 2023-06-30 12:32:15.000000 isimip-qc-3.0.3/PKG-INFO
--rw-r--r--   0 buechner  (2091) users      (100)    10473 2023-05-08 13:27:31.000000 isimip-qc-3.0.3/README.md
-drwxr-xr-x   0 buechner  (2091) users      (100)        0 2023-06-30 12:32:15.000000 isimip-qc-3.0.3/isimip_qc/
--rw-r--r--   0 buechner  (2091) users      (100)       32 2023-06-30 12:30:53.000000 isimip-qc-3.0.3/isimip_qc/__init__.py
-drwxr-xr-x   0 buechner  (2091) users      (100)        0 2023-06-30 12:32:15.000000 isimip-qc-3.0.3/isimip_qc/checks/
--rw-r--r--   0 buechner  (2091) users      (100)     2367 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/checks/3d.py
--rw-r--r--   0 buechner  (2091) users      (100)      790 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/checks/__init__.py
--rw-r--r--   0 buechner  (2091) users      (100)     4121 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/checks/attributes.py
--rw-r--r--   0 buechner  (2091) users      (100)     2867 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/checks/dataset.py
--rw-r--r--   0 buechner  (2091) users      (100)     5113 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/checks/dimensions.py
-drwxr-xr-x   0 buechner  (2091) users      (100)        0 2023-06-30 12:32:15.000000 isimip-qc-3.0.3/isimip_qc/checks/variables/
--rw-r--r--   0 buechner  (2091) users      (100)        0 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/checks/variables/__init__.py
--rw-r--r--   0 buechner  (2091) users      (100)     6546 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/checks/variables/latlon.py
--rw-r--r--   0 buechner  (2091) users      (100)     6920 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/checks/variables/time.py
--rw-r--r--   0 buechner  (2091) users      (100)     4781 2023-03-16 09:37:51.000000 isimip-qc-3.0.3/isimip_qc/checks/variables/time_resolution.py
--rw-r--r--   0 buechner  (2091) users      (100)    13127 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/checks/variables/var.py
--rw-r--r--   0 buechner  (2091) users      (100)     5206 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/checks/variables/var3d.py
--rw-r--r--   0 buechner  (2091) users      (100)     1961 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/config.py
--rw-r--r--   0 buechner  (2091) users      (100)      524 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/exceptions.py
--rw-r--r--   0 buechner  (2091) users      (100)     1692 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/fixes.py
--rw-r--r--   0 buechner  (2091) users      (100)     9308 2023-06-30 12:29:27.000000 isimip-qc-3.0.3/isimip_qc/main.py
--rw-r--r--   0 buechner  (2091) users      (100)     9190 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/models.py
-drwxr-xr-x   0 buechner  (2091) users      (100)        0 2023-06-30 12:32:15.000000 isimip-qc-3.0.3/isimip_qc/utils/
--rw-r--r--   0 buechner  (2091) users      (100)        0 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/utils/__init__.py
--rw-r--r--   0 buechner  (2091) users      (100)      366 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/utils/datamodel.py
--rw-r--r--   0 buechner  (2091) users      (100)     1298 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/utils/files.py
--rw-r--r--   0 buechner  (2091) users      (100)      224 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/isimip_qc/utils/logging.py
-drwxr-xr-x   0 buechner  (2091) users      (100)        0 2023-06-30 12:32:15.000000 isimip-qc-3.0.3/isimip_qc.egg-info/
--rw-r--r--   0 buechner  (2091) users      (100)    12423 2023-06-30 12:32:14.000000 isimip-qc-3.0.3/isimip_qc.egg-info/PKG-INFO
--rw-r--r--   0 buechner  (2091) users      (100)      837 2023-06-30 12:32:15.000000 isimip-qc-3.0.3/isimip_qc.egg-info/SOURCES.txt
--rw-r--r--   0 buechner  (2091) users      (100)        1 2023-06-30 12:32:14.000000 isimip-qc-3.0.3/isimip_qc.egg-info/dependency_links.txt
--rw-r--r--   0 buechner  (2091) users      (100)       51 2023-06-30 12:32:14.000000 isimip-qc-3.0.3/isimip_qc.egg-info/entry_points.txt
--rw-r--r--   0 buechner  (2091) users      (100)       76 2023-06-30 12:32:14.000000 isimip-qc-3.0.3/isimip_qc.egg-info/requires.txt
--rw-r--r--   0 buechner  (2091) users      (100)       10 2023-06-30 12:32:14.000000 isimip-qc-3.0.3/isimip_qc.egg-info/top_level.txt
--rw-r--r--   0 buechner  (2091) users      (100)     1061 2023-06-30 12:32:15.000000 isimip-qc-3.0.3/setup.cfg
--rw-r--r--   0 buechner  (2091) users      (100)       38 2023-03-08 13:09:33.000000 isimip-qc-3.0.3/setup.py
+drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-07-12 12:01:59.605442 isimip-qc-3.1.0/
+-rw-r--r--   0 jochen    (1000) staff       (20)     1102 2021-11-24 12:01:57.000000 isimip-qc-3.1.0/LICENSE
+-rw-r--r--   0 jochen    (1000) staff       (20)    12015 2023-07-12 12:01:59.605539 isimip-qc-3.1.0/PKG-INFO
+-rw-r--r--   0 jochen    (1000) staff       (20)    11234 2023-07-12 11:48:54.000000 isimip-qc-3.1.0/README.md
+drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-07-12 12:01:59.601005 isimip-qc-3.1.0/isimip_qc/
+-rw-r--r--   0 jochen    (1000) staff       (20)       32 2023-07-12 12:00:38.000000 isimip-qc-3.1.0/isimip_qc/__init__.py
+drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-07-12 12:01:59.603064 isimip-qc-3.1.0/isimip_qc/checks/
+-rw-r--r--   0 jochen    (1000) staff       (20)     2367 2023-04-12 15:03:21.000000 isimip-qc-3.1.0/isimip_qc/checks/3d.py
+-rw-r--r--   0 jochen    (1000) staff       (20)      790 2021-11-24 12:01:57.000000 isimip-qc-3.1.0/isimip_qc/checks/__init__.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     4121 2021-11-24 12:01:57.000000 isimip-qc-3.1.0/isimip_qc/checks/attributes.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     2867 2023-04-12 16:14:13.000000 isimip-qc-3.1.0/isimip_qc/checks/dataset.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     5113 2023-02-27 16:08:55.000000 isimip-qc-3.1.0/isimip_qc/checks/dimensions.py
+-rw-r--r--   0 jochen    (1000) staff       (20)      428 2023-07-12 11:37:12.000000 isimip-qc-3.1.0/isimip_qc/checks/experiments.py
+drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-07-12 12:01:59.604441 isimip-qc-3.1.0/isimip_qc/checks/variables/
+-rw-r--r--   0 jochen    (1000) staff       (20)        0 2021-11-24 12:01:57.000000 isimip-qc-3.1.0/isimip_qc/checks/variables/__init__.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     6546 2023-02-27 16:08:55.000000 isimip-qc-3.1.0/isimip_qc/checks/variables/latlon.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     6920 2022-12-14 13:58:36.000000 isimip-qc-3.1.0/isimip_qc/checks/variables/time.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     4781 2023-04-12 15:03:21.000000 isimip-qc-3.1.0/isimip_qc/checks/variables/time_resolution.py
+-rw-r--r--   0 jochen    (1000) staff       (20)    13127 2023-02-27 16:08:55.000000 isimip-qc-3.1.0/isimip_qc/checks/variables/var.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     5206 2021-11-24 12:01:57.000000 isimip-qc-3.1.0/isimip_qc/checks/variables/var3d.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     2023 2023-07-12 11:48:54.000000 isimip-qc-3.1.0/isimip_qc/config.py
+-rw-r--r--   0 jochen    (1000) staff       (20)      524 2021-11-24 12:01:57.000000 isimip-qc-3.1.0/isimip_qc/exceptions.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     1692 2021-11-24 12:01:57.000000 isimip-qc-3.1.0/isimip_qc/fixes.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     9458 2023-07-12 11:49:04.000000 isimip-qc-3.1.0/isimip_qc/main.py
+-rw-r--r--   0 jochen    (1000) staff       (20)    10187 2023-07-12 11:48:54.000000 isimip-qc-3.1.0/isimip_qc/models.py
+drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-07-12 12:01:59.605198 isimip-qc-3.1.0/isimip_qc/utils/
+-rw-r--r--   0 jochen    (1000) staff       (20)        0 2021-11-24 12:01:57.000000 isimip-qc-3.1.0/isimip_qc/utils/__init__.py
+-rw-r--r--   0 jochen    (1000) staff       (20)      366 2023-02-27 16:08:55.000000 isimip-qc-3.1.0/isimip_qc/utils/datamodel.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     1153 2023-07-12 11:37:12.000000 isimip-qc-3.1.0/isimip_qc/utils/experiments.py
+-rw-r--r--   0 jochen    (1000) staff       (20)     1298 2023-02-27 16:08:55.000000 isimip-qc-3.1.0/isimip_qc/utils/files.py
+-rw-r--r--   0 jochen    (1000) staff       (20)      224 2022-12-14 13:58:36.000000 isimip-qc-3.1.0/isimip_qc/utils/logging.py
+drwxr-xr-x   0 jochen    (1000) staff       (20)        0 2023-07-12 12:01:59.601848 isimip-qc-3.1.0/isimip_qc.egg-info/
+-rw-r--r--   0 jochen    (1000) staff       (20)    12015 2023-07-12 12:01:59.000000 isimip-qc-3.1.0/isimip_qc.egg-info/PKG-INFO
+-rw-r--r--   0 jochen    (1000) staff       (20)      900 2023-07-12 12:01:59.000000 isimip-qc-3.1.0/isimip_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen    (1000) staff       (20)        1 2023-07-12 12:01:59.000000 isimip-qc-3.1.0/isimip_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen    (1000) staff       (20)       50 2023-07-12 12:01:59.000000 isimip-qc-3.1.0/isimip_qc.egg-info/entry_points.txt
+-rw-r--r--   0 jochen    (1000) staff       (20)       81 2023-07-12 12:01:59.000000 isimip-qc-3.1.0/isimip_qc.egg-info/requires.txt
+-rw-r--r--   0 jochen    (1000) staff       (20)       10 2023-07-12 12:01:59.000000 isimip-qc-3.1.0/isimip_qc.egg-info/top_level.txt
+-rw-r--r--   0 jochen    (1000) staff       (20)     1066 2023-07-12 12:01:59.605957 isimip-qc-3.1.0/setup.cfg
+-rw-r--r--   0 jochen    (1000) staff       (20)       38 2023-02-27 16:08:55.000000 isimip-qc-3.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `isimip-qc-3.0.3/LICENSE` & `isimip-qc-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/PKG-INFO` & `isimip-qc-3.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,165 +1,194 @@
 Metadata-Version: 2.1
 Name: isimip-qc
-Version: 3.0.3
+Version: 3.1.0
 Summary: A command line tool for the quality control of climate impact data of the ISIMIP project.
 Home-page: https://github.com/ISI-MIP/isimip-qc
 Author: Matthias Büchner, Jochen Klar
 License: MIT
-Description: ISIMIP quality control
-        ======================
-        
-        [![Python Version](https://img.shields.io/badge/python->=3.6-blue)](https://www.python.org/)
-        [![License](https://img.shields.io/badge/License-MIT-green)](https://github.com/ISI-MIP/isimip-qc/blob/master/LICENSE)
-        
-        A command line tool for the quality control of climate impact data of the ISIMIP project. It mainly covers tests of:
-        - the file name against the protocol schemas and patterns
-        - variables, dimensions and global attributes
-        - data model and types
-        - some consistency checks on the NetCDF time axis and
-        - if the data is within a valid value range (when defined in the ISIMIP protocol)
-        
-        **This is still work in progress.**
-        
-        
-        Setup
-        -----
-        
-        The application is written in Python (> 3.6) uses only dependencies, which can be installed without administrator priviledges. The installation of Python (and its developing packages), however differs from operating system to operating system. Optional Git is needed if the application is installed directly from GitHub. The installation of Python 3 and Git for different plattforms is documented [here](https://github.com/ISI-MIP/isimip-utils/blob/master/docs/prerequisites.md).
-        
-        The tool itself can be installed via pip. Usually you want to create a [virtual environment](https://docs.python.org/3/library/venv.html) first, but this is optional.
-        
-        ```bash
-        # setup venv on Linux/macOS/Windows WSL
-        python3 -m venv env
-        source env/bin/activate
-        
-        # setup venv on Windows cmd
-        python -m venv env
-        call env\Scripts\activate.bat
-        
-        # install from the Python Package Index (PyPI), recommended
-        pip install isimip-qc
-        
-        # update from PyPI
-        pip install --upgrade rdmo
-        
-        # install directly from GitHub
-        pip install git+https://github.com/ISI-MIP/isimip-qc
-        
-        # update from Github
-        pip install --upgrade git+https://github.com/ISI-MIP/isimip-qc
-        ```
-        
-        Usage
-        -----
-        
-        The tool has several options which can be inspected using the help option `-h, --help`:
-        
-        ```plain
-        usage: isimip-qc [-h] [--config-file CONFIG_FILE] [-c] [-m] [-O]
-                         [--unchecked-path UNCHECKED_PATH] [--checked-path CHECKED_PATH]
-                         [--protocol-location PROTOCOL_LOCATIONS] [--log-level LOG_LEVEL]
-                         [--log-path LOG_PATH] [--log-path-level LOG_PATH_LEVEL] [--include INCLUDE_LIST]
-                         [--exclude EXCLUDE_LIST] [-f] [-w] [-e] [-r [MINMAX]] [-nt] [--fix]
-                         [--fix-datamodel [FIX_DATAMODEL]] [--check CHECK] [--force-copy-move] [-V]
-                         schema_path
-        
-        Check ISIMIP files for matching protocol definitions
-        
-        positional arguments:
-          schema_path           ISIMIP schema_path, e.g. ISIMIP3a/OutputData/water_global
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --config-file CONFIG_FILE
-                                file path of the config file
-          -c, --copy            copy checked files to CHECKED_PATH if no warnings or errors were found
-          -m, --move            move checked files to CHECKED_PATH if no warnings or errors were found
-          -O, --overwrite       overwrite files in CHECKED_PATH if present. Default is False.
-          --unchecked-path UNCHECKED_PATH
-                                base path of the unchecked files
-          --checked-path CHECKED_PATH
-                                base path for the checked files
-          --protocol-location PROTOCOL_LOCATIONS
-                                URL or file path to the protocol when different from official repository
-          --log-level LOG_LEVEL
-                                log level (CRITICAL, ERROR, WARN, VRDETAIL, CHECKING, SUMMARY, INFO, or
-                                DEBUG) [default: CHECKING]
-          --log-path LOG_PATH   base path for the individual log files
-          --log-path-level LOG_PATH_LEVEL
-                                log level for the individual log files [default: WARN]
-          --include INCLUDE_LIST
-                                patterns of files to include. Exclude those that don't match any.
-          --exclude EXCLUDE_LIST
-                                patterns of files to exclude. Include only those that don't match any.
-          -f, --first-file      only process first file found in UNCHECKED_PATH
-          -w, --stop-on-warnings
-                                stop execution on warnings
-          -e, --stop-on-errors  stop execution on errors
-          -r [MINMAX], --minmax [MINMAX]
-                                test values for valid range (slow, argument MINMAX defaults to show the
-                                top 10 values)
-          -nt, --skip-time-span-check
-                                skip check for simulated time period
-          --fix                 try to fix warnings detected on the original files
-          --fix-datamodel [FIX_DATAMODEL]
-                                also fix warnings on data model found using NCCOPY or CDO (slow). Choose
-                                preferred tool per lower case argument.
-          --check CHECK         perform only one particular check
-          --force-copy-move     copy or move files despite errors
-          -V, --version         show program's version number and exit
-        ```
-        
-        The only mandatory argument is the `schema_path`, which specifies the pattern and schema to use. The `schema_path` consitst of the `simulation_round`, the `product`, and the `sector` seperated by slashes, e.g. `ISIMIP3a/OutputData/water_global`. If the only argument used is `schema_path`, the current user path when calling the tool should be same as the directory of the files to be checked.
-        
-        ### The options in detail
-        
-        * `--config-file`: Default values for the optional arguments are set in the code, but can also be provided via:
-            * a config file given by `--config-file`, or located at `isimip-qc.conf`, `~/.isimip-qc.conf`, or `/etc/isimip-qc.conf`. The config file needs to have a section `isimip-qc` and uses lower case variables and underscores, e.g.:
-                ```
-                [isimip-qc]
-                pattern_locations = /path/to/isimip-protocol-3/output/pattern/
-                schema_locations = path/to/isimip-protocol-3/output/schema/
-                ```
-        
-            * environment variables (in caps and with underscores, e.g. `UNCHECKED_PATH`).
-        * `-c, --copy` and `-m, --move`: Copy or move files that have successfully passed the checks to a final destination. Effective only when no warnings have been found on the file.
-        * '-O, --overwrite`: Allow overwriting of existing files in CHECKED_PATH. Default is to skip copy or move in case the target file is already present.
-        * `--unchecked-path UNCHECKED_PATH`: Any files in this folder **and** its subfolders will be included into the list of files to test.
-        * `--checked-path CHECKED_PATH`: Target folder for the `--copy` or `--move` operation. The subfolder structure below CHECKED_PATH will be created and filled according to the sub-structure found in UNCHECKED_PATH
-        * `--protocol-location PROTOCOL_LOCATIONS`: For working with local copies of the ISIMIP protocol (append `/output` to the cloned repositories folder). Omit option for using the online GitHub protocol versions for [ISIMIP2](https://github.com/ISI-MIP/isimip-protocol-2) or [ISIMIP3](https://github.com/ISI-MIP/isimip-protocol-3). An internet connection is required for reading the online protocols.
-        * `--log-level LOG_LEVEL`: Set the detail level of log output. Default is `CHECKING`. Log levels from `CRITICAL` to `VRDETAIL` will not show the file currently checked in the terminal but write all of them to the data file specific log file.<br>
-        `CRITICAL` : only very severe errors<br>
-        `ERROR`: all errors<br>
-        `WARN`: warnings and all errors<br>
-        `VRDETAIL`: same as CHECKING but with details on time and location of valid ranges violations when invoked with `--minmax` option. Very slow when violations are detected.<br>
-        `CHECKING`: includes warnings and errors<br>
-        `SUMMARY`: includes warnings, errors and the summary shown at the end<br>
-        `INFO`: includes `SUMMARY` and details for successful checks<br>
-        `DEBUG`: all the above plus details for some debugging cases.
-        * `--log-path LOG_PATH`: Also write the logs to a file where the folder structure below LOG_PATH is taken from UNCHECKED_PATH.
-        * `--log-path-level LOG_PATH_LEVEL`: The log level used for the file specific logs below `LOG_PATH`. The default is `WARN` and should suffice for most cases.
-        * `--include INCLUDE_LIST` : Provide a comma-separated list of strings to include for the checks if any of them matches the file path or name, e.g. 'daily,dis' will only check `*daily*` or `*discharge*` files while skipping others.
-        * `--exclude EXCLUDE_LIST` : Provide a comma-separated list of strings to exclude from the checks if any of them matches the file path or name, e.g. 'monthly,histsoc' will skip any `*monthly*` or `*histsoc*` files.
-        * `-f, --first-file`: Only test the first file found in UNCHECKED_PATH. Useful for revealing issues that may occur on all your files.
-        * `-w, --stop-on-warnings`: The tool will stop after the first file where WARNINGs have been identified.
-        * `-e, --stop-on-errors`: The tool will stop after the first file where ERRORs have been identified.
-        * `-r [MINMAX], --minmax [MINMAX]`: Test the data for valid ranges when defined in the protocol. Per default and when violations are detected the top 20 minimum and maximum values along with their time and geographic location will be logged as well. MINMAX is optional and defines how many values should be reported instead of 20. This test drastically slows down the run time of the tool.
-        * -nt, --skip-time-span-check: Skip checking non-dialy data for proper coverage of simulation periods.
-        * `--fix`: Activates a number of fixes for WARNINGs by taking the default values from the protocol, e.g. variable attributes and units. In additions an unique identifier (UUID), the version of this tool and the protocol version (by a git hash) are being written to the global attributes section of the NetCDF file. **Attention**: Fixes and are going to be applied on **your original files** in UNCHECKED_PATH.
-        * `--fix-datamodel [FIX_DATAMODEL]`: Fixes to the data model and compression level of the NetCDF file can't be made on-the-fly with the libraries used by the tool. We here rely on the external tools [cdo](https://code.mpimet.mpg.de/projects/cdo/) or nccopy (from the [NetCDF library](https://www.unidata.ucar.edu/software/netcdf/)) to rewrite the entire file. Default is `nccopy`. Please try to create the files with the proper data model (compressed NETCDF4_CLASSIC) in your postprocessing chain before submitting them to the data server.
-        * `--check CHECK`: Perform only one particular check. The list of CHECKs can be taken from the funtions defined in the `isimip_qc/checks/*.py` files.
-        * `--force-copy-move`: Copy or move files despite errors found during checks.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+ISIMIP quality control
+======================
+
+[![Python Version](https://img.shields.io/badge/python->=3.6-blue)](https://www.python.org/)
+[![License](https://img.shields.io/badge/License-MIT-green)](https://github.com/ISI-MIP/isimip-qc/blob/master/LICENSE)
+
+A command line tool for the quality control of climate impact data of the ISIMIP project. It mainly covers tests of:
+- the file name against the protocol schemas and patterns
+- variables, dimensions and global attributes
+- data model and types
+- some consistency checks on the NetCDF time axis and
+- if the data is within a valid value range (when defined in the ISIMIP protocol)
+
+**This is still work in progress.**
+
+
+Setup
+-----
+
+The application is written in Python (> 3.6) uses only dependencies, which can be installed without administrator priviledges. The installation of Python (and its developing packages), however differs from operating system to operating system. Optional Git is needed if the application is installed directly from GitHub. The installation of Python 3 and Git for different plattforms is documented [here](https://github.com/ISI-MIP/isimip-utils/blob/master/docs/prerequisites.md).
+
+The tool itself can be installed via pip. Usually you want to create a [virtual environment](https://docs.python.org/3/library/venv.html) first, but this is optional.
+
+```bash
+# setup venv on Linux/macOS/Windows WSL
+python3 -m venv env
+source env/bin/activate
+
+# setup venv on Windows cmd
+python -m venv env
+call env\Scripts\activate.bat
+
+# install from the Python Package Index (PyPI), recommended
+pip install isimip-qc
+
+# update from PyPI
+pip install --upgrade rdmo
+
+# install directly from GitHub
+pip install git+https://github.com/ISI-MIP/isimip-qc
+
+# update from Github
+pip install --upgrade git+https://github.com/ISI-MIP/isimip-qc
+```
+
+Usage
+-----
+
+The tool has several options which can be inspected using the help option `-h, --help`:
+
+```plain
+usage: isimip-qc [-h] [--config-file CONFIG_FILE] [-c] [-m] [-O]
+                 [--unchecked-path UNCHECKED_PATH] [--checked-path CHECKED_PATH]
+                 [--protocol-location PROTOCOL_LOCATIONS] [--log-level LOG_LEVEL]
+                 [--log-path LOG_PATH] [--log-path-level LOG_PATH_LEVEL] [--include INCLUDE_LIST]
+                 [--exclude EXCLUDE_LIST] [-f] [-w] [-e] [-r [MINMAX]] [-nt] [--fix]
+                 [--fix-datamodel [FIX_DATAMODEL]] [--check CHECK] [--force-copy-move] [-V]
+                 schema_path
+
+Check ISIMIP files for matching protocol definitions
+
+positional arguments:
+  schema_path           ISIMIP schema_path, e.g. ISIMIP3a/OutputData/water_global
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --config-file CONFIG_FILE
+                        file path of the config file
+  -c, --copy            copy checked files to CHECKED_PATH if no warnings or errors were found
+  -m, --move            move checked files to CHECKED_PATH if no warnings or errors were found
+  -O, --overwrite       overwrite files in CHECKED_PATH if present. Default is False.
+  --unchecked-path UNCHECKED_PATH
+                        base path of the unchecked files
+  --checked-path CHECKED_PATH
+                        base path for the checked files
+  --protocol-location PROTOCOL_LOCATIONS
+                        URL or file path to the protocol when different from official repository
+  --log-level LOG_LEVEL
+                        log level (CRITICAL, ERROR, WARN, VRDETAIL, CHECKING, SUMMARY, INFO, or
+                        DEBUG) [default: CHECKING]
+  --log-path LOG_PATH   base path for the individual log files
+  --log-path-level LOG_PATH_LEVEL
+                        log level for the individual log files [default: WARN]
+  --include INCLUDE_LIST
+                        patterns of files to include. Exclude those that don't match any.
+  --exclude EXCLUDE_LIST
+                        patterns of files to exclude. Include only those that don't match any.
+  -f, --first-file      only process first file found in UNCHECKED_PATH
+  -w, --stop-on-warnings
+                        stop execution on warnings
+  -e, --stop-on-errors  stop execution on errors
+  -r [MINMAX], --minmax [MINMAX]
+                        test values for valid range (slow, argument MINMAX defaults to show the
+                        top 10 values)
+  -nt, --skip-time-span-check
+                        skip check for simulated time period
+  --fix                 try to fix warnings detected on the original files
+  --fix-datamodel [FIX_DATAMODEL]
+                        also fix warnings on data model found using NCCOPY or CDO (slow). Choose
+                        preferred tool per lower case argument.
+  --check CHECK         perform only one particular check
+  --force-copy-move     copy or move files despite errors
+  -V, --version         show program's version number and exit
+```
+
+The only mandatory argument is the `schema_path`, which specifies the pattern and schema to use. The `schema_path` consitst of the `simulation_round`, the `product`, and the `sector` seperated by slashes, e.g. `ISIMIP3a/OutputData/water_global`. If the only argument used is `schema_path`, the current user path when calling the tool should be same as the directory of the files to be checked.
+
+### The options in detail
+
+* `--config-file`: Default values for the optional arguments are set in the code, but can also be provided via:
+    * a config file given by `--config-file`, or located at `isimip-qc.conf`, `~/.isimip-qc.conf`, or `/etc/isimip-qc.conf`. The config file needs to have a section `isimip-qc` and uses lower case variables and underscores, e.g.:
+        ```
+        [isimip-qc]
+        pattern_locations = /path/to/isimip-protocol-3/output/pattern/
+        schema_locations = path/to/isimip-protocol-3/output/schema/
+        ```
+
+    * environment variables (in caps and with underscores, e.g. `UNCHECKED_PATH`).
+* `-c, --copy` and `-m, --move`: Copy or move files that have successfully passed the checks to a final destination. Effective only when no warnings have been found on the file.
+* '-O, --overwrite`: Allow overwriting of existing files in CHECKED_PATH. Default is to skip copy or move in case the target file is already present.
+* `--unchecked-path UNCHECKED_PATH`: Any files in this folder **and** its subfolders will be included into the list of files to test.
+* `--checked-path CHECKED_PATH`: Target folder for the `--copy` or `--move` operation. The subfolder structure below CHECKED_PATH will be created and filled according to the sub-structure found in UNCHECKED_PATH
+* `--protocol-location PROTOCOL_LOCATIONS`: For working with local copies of the ISIMIP protocol (append `/output` to the cloned repositories folder). Omit option for using the online GitHub protocol versions for [ISIMIP2](https://github.com/ISI-MIP/isimip-protocol-2) or [ISIMIP3](https://github.com/ISI-MIP/isimip-protocol-3). An internet connection is required for reading the online protocols.
+* `--log-level LOG_LEVEL`: Set the detail level of log output. Default is `CHECKING`. Log levels from `CRITICAL` to `VRDETAIL` will not show the file currently checked in the terminal but write all of them to the data file specific log file.<br>
+`CRITICAL` : only very severe errors<br>
+`ERROR`: all errors<br>
+`WARN`: warnings and all errors<br>
+`VRDETAIL`: same as CHECKING but with details on time and location of valid ranges violations when invoked with `--minmax` option. Very slow when violations are detected.<br>
+`CHECKING`: includes warnings and errors<br>
+`SUMMARY`: includes warnings, errors and the summary shown at the end<br>
+`INFO`: includes `SUMMARY` and details for successful checks<br>
+`DEBUG`: all the above plus details for some debugging cases.
+* `--log-path LOG_PATH`: Also write the logs to a file where the folder structure below LOG_PATH is taken from UNCHECKED_PATH.
+* `--log-path-level LOG_PATH_LEVEL`: The log level used for the file specific logs below `LOG_PATH`. The default is `WARN` and should suffice for most cases.
+* `--include INCLUDE_LIST` : Provide a comma-separated list of strings to include for the checks if any of them matches the file path or name, e.g. 'daily,dis' will only check `*daily*` or `*discharge*` files while skipping others.
+* `--exclude EXCLUDE_LIST` : Provide a comma-separated list of strings to exclude from the checks if any of them matches the file path or name, e.g. 'monthly,histsoc' will skip any `*monthly*` or `*histsoc*` files.
+* `-f, --first-file`: Only test the first file found in UNCHECKED_PATH. Useful for revealing issues that may occur on all your files.
+* `-w, --stop-on-warnings`: The tool will stop after the first file where WARNINGs have been identified.
+* `-e, --stop-on-errors`: The tool will stop after the first file where ERRORs have been identified.
+* `-r [MINMAX], --minmax [MINMAX]`: Test the data for valid ranges when defined in the protocol. Per default and when violations are detected the top 20 minimum and maximum values along with their time and geographic location will be logged as well. MINMAX is optional and defines how many values should be reported instead of 20. This test drastically slows down the run time of the tool.
+* -nt, --skip-time-span-check: Skip checking non-dialy data for proper coverage of simulation periods.
+* `--fix`: Activates a number of fixes for WARNINGs by taking the default values from the protocol, e.g. variable attributes and units. In additions an unique identifier (UUID), the version of this tool and the protocol version (by a git hash) are being written to the global attributes section of the NetCDF file. **Attention**: Fixes and are going to be applied on **your original files** in UNCHECKED_PATH.
+* `--fix-datamodel [FIX_DATAMODEL]`: Fixes to the data model and compression level of the NetCDF file can't be made on-the-fly with the libraries used by the tool. We here rely on the external tools [cdo](https://code.mpimet.mpg.de/projects/cdo/) or nccopy (from the [NetCDF library](https://www.unidata.ucar.edu/software/netcdf/)) to rewrite the entire file. Default is `nccopy`. Please try to create the files with the proper data model (compressed NETCDF4_CLASSIC) in your postprocessing chain before submitting them to the data server.
+* `--check CHECK`: Perform only one particular check. The list of CHECKs can be taken from the funtions defined in the `isimip_qc/checks/*.py` files.
+* `--force-copy-move`: Copy or move files despite errors found during checks.
+
+
+Scripts/Notebooks
+-----------------
+
+The different functions of the tool can also be used in Python scripts or Jupyter Notebooks. Before any functions are called, the global settings object needs to be initialized using the `init_settings` function, e.g.:
+
+```python
+from isimip_qc.checks import checks
+from isimip_qc.main import init_settings
+from isimip_qc.models import File
+
+settings = init_settings(
+    schema_path='ISIMIP3b/OutputData/water_global',
+    config_file='~/data/isimip/isimip.conf'
+)
+
+file_path = '~/data/isimip/qc/unchecked/h08_ipsl-cm6a-lr_w5e5_ssp585_2015soc_default_dis_global_monthly_2015_2100.nc'
+
+file = File(file_path)
+file.open_log()
+file.match()
+file.open_dataset()
+
+for check in checks:
+    check(file)
+
+file.close_dataset()
+```
```

### Comparing `isimip-qc-3.0.3/README.md` & `isimip-qc-3.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -139,7 +139,36 @@
 * `-e, --stop-on-errors`: The tool will stop after the first file where ERRORs have been identified.
 * `-r [MINMAX], --minmax [MINMAX]`: Test the data for valid ranges when defined in the protocol. Per default and when violations are detected the top 20 minimum and maximum values along with their time and geographic location will be logged as well. MINMAX is optional and defines how many values should be reported instead of 20. This test drastically slows down the run time of the tool.
 * -nt, --skip-time-span-check: Skip checking non-dialy data for proper coverage of simulation periods.
 * `--fix`: Activates a number of fixes for WARNINGs by taking the default values from the protocol, e.g. variable attributes and units. In additions an unique identifier (UUID), the version of this tool and the protocol version (by a git hash) are being written to the global attributes section of the NetCDF file. **Attention**: Fixes and are going to be applied on **your original files** in UNCHECKED_PATH.
 * `--fix-datamodel [FIX_DATAMODEL]`: Fixes to the data model and compression level of the NetCDF file can't be made on-the-fly with the libraries used by the tool. We here rely on the external tools [cdo](https://code.mpimet.mpg.de/projects/cdo/) or nccopy (from the [NetCDF library](https://www.unidata.ucar.edu/software/netcdf/)) to rewrite the entire file. Default is `nccopy`. Please try to create the files with the proper data model (compressed NETCDF4_CLASSIC) in your postprocessing chain before submitting them to the data server.
 * `--check CHECK`: Perform only one particular check. The list of CHECKs can be taken from the funtions defined in the `isimip_qc/checks/*.py` files.
 * `--force-copy-move`: Copy or move files despite errors found during checks.
+
+
+Scripts/Notebooks
+-----------------
+
+The different functions of the tool can also be used in Python scripts or Jupyter Notebooks. Before any functions are called, the global settings object needs to be initialized using the `init_settings` function, e.g.:
+
+```python
+from isimip_qc.checks import checks
+from isimip_qc.main import init_settings
+from isimip_qc.models import File
+
+settings = init_settings(
+    schema_path='ISIMIP3b/OutputData/water_global',
+    config_file='~/data/isimip/isimip.conf'
+)
+
+file_path = '~/data/isimip/qc/unchecked/h08_ipsl-cm6a-lr_w5e5_ssp585_2015soc_default_dis_global_monthly_2015_2100.nc'
+
+file = File(file_path)
+file.open_log()
+file.match()
+file.open_dataset()
+
+for check in checks:
+    check(file)
+
+file.close_dataset()
+```
```

### Comparing `isimip-qc-3.0.3/isimip_qc/checks/3d.py` & `isimip-qc-3.1.0/isimip_qc/checks/3d.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/isimip_qc/checks/__init__.py` & `isimip-qc-3.1.0/isimip_qc/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/isimip_qc/checks/attributes.py` & `isimip-qc-3.1.0/isimip_qc/checks/attributes.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/isimip_qc/checks/dataset.py` & `isimip-qc-3.1.0/isimip_qc/checks/dataset.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/isimip_qc/checks/dimensions.py` & `isimip-qc-3.1.0/isimip_qc/checks/dimensions.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/isimip_qc/checks/variables/latlon.py` & `isimip-qc-3.1.0/isimip_qc/checks/variables/latlon.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/isimip_qc/checks/variables/time.py` & `isimip-qc-3.1.0/isimip_qc/checks/variables/time.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/isimip_qc/checks/variables/time_resolution.py` & `isimip-qc-3.1.0/isimip_qc/checks/variables/time_resolution.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/isimip_qc/checks/variables/var.py` & `isimip-qc-3.1.0/isimip_qc/checks/variables/var.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/isimip_qc/checks/variables/var3d.py` & `isimip-qc-3.1.0/isimip_qc/checks/variables/var3d.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/isimip_qc/config.py` & `isimip-qc-3.1.0/isimip_qc/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from pathlib import Path
 
 import colorlog
 
-from isimip_utils.config import ISIMIPSettings
+from isimip_utils.config import Settings as BaseSettings
 from isimip_utils.decorators import cached_property
 from isimip_utils.fetch import fetch_definitions, fetch_pattern, fetch_schema
 
 from datetime import datetime
 
 logger = colorlog.getLogger(__name__)
 
 
-class Settings(ISIMIPSettings):
+class Settings(BaseSettings):
 
-    def setup(self, parser):
-        super().setup(parser)
+    def setup(self, args):
+        super().setup(args)
 
         self.NOW = datetime.utcnow().strftime("%Y%m%dT%H%MZ")
 
         # set create pathes and set default values
         if self.UNCHECKED_PATH is not None:
             self.UNCHECKED_PATH = Path(self.UNCHECKED_PATH).expanduser()
         else:
             self.UNCHECKED_PATH = Path().cwd()
 
         if self.CHECKED_PATH is not None:
             self.CHECKED_PATH = Path(self.CHECKED_PATH).expanduser()
 
         self.LOG_LEVEL = self.LOG_LEVEL.upper()
+        self.LOG_PATH_LEVEL = self.LOG_PATH_LEVEL.upper()
         if self.LOG_PATH is not None:
             self.LOG_PATH = Path(self.LOG_PATH).expanduser()
 
         # setup logs
         colorlog.basicConfig(level=self.LOG_LEVEL,
                              format=' %(log_color)s%(levelname)-8s : %(message)s%(reset)s')
```

### Comparing `isimip-qc-3.0.3/isimip_qc/exceptions.py` & `isimip-qc-3.1.0/isimip_qc/exceptions.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/isimip_qc/fixes.py` & `isimip-qc-3.1.0/isimip_qc/fixes.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/isimip_qc/main.py` & `isimip-qc-3.1.0/isimip_qc/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import argparse
 from os import path
 import sys
 
-from isimip_qc import VERSION
-
 import colorlog
 
+from isimip_utils.parser import ArgumentParser
+
+from . import VERSION
 from .checks import checks
 from .config import settings
 from .exceptions import FileCritical, FileError, FileWarning
 from .models import File, Summary
 from .utils.files import walk_files
 from .utils.logging import CHECKING
 
 logger = colorlog.getLogger(__name__)
 
 
 def get_parser():
-    parser = argparse.ArgumentParser(description='Check ISIMIP files for matching protocol definitions')
+    parser = ArgumentParser(prog='isimip-qc', description='Check ISIMIP files for matching protocol definitions')
+
     # mandatory
     parser.add_argument('schema_path', help='ISIMIP schema_path, e.g. ISIMIP3a/OutputData/water_global')
+
     # optional
-    parser.add_argument('--config-file', dest='config_file',
-                        help='file path of the config file')
     parser.add_argument('-c', '--copy', dest='copy', action='store_true',
                         help='copy checked files to CHECKED_PATH if no warnings or errors were found')
     parser.add_argument('-m', '--move', dest='move', action='store_true',
                         help='move checked files to CHECKED_PATH if no warnings or errors were found')
     parser.add_argument('-O', '--overwrite', dest='overwrite', action='store_true',
                         help='overwrite files in CHECKED_PATH if present. Default is False.')
     parser.add_argument('--unchecked-path', dest='unchecked_path',
@@ -65,17 +65,26 @@
     parser.add_argument('--force-copy-move', dest='force_copy_move', action='store_true', default=False,
                         help='Copy or move files despite errors')
     parser.add_argument('-V', '--version', action='version',
                         version=VERSION)
     return parser
 
 
+def init_settings(**kwargs):
+    parser = get_parser()
+    args = parser.get_defaults()
+    args.update(kwargs)
+    settings.setup(args)
+    return settings
+
+
 def main():
     parser = get_parser()
-    settings.setup(parser)
+    args = vars(parser.parse_args())
+    settings.setup(args)
     summary = Summary()
 
     if settings.DEFINITIONS is None:
         parser.error('no definitions could be found. Check schema_path argument.')
     if settings.PATTERN is None:
         parser.error('no pattern could be found. Check schema_path argument.')
     if settings.SCHEMA is None:
@@ -182,15 +191,16 @@
                         elif settings.COPY:
                             file.copy()
                     else:
                         logger.warn('File has not been moved or copied due to warnings or erros found.')
 
                 # collect stats about the file
                 summary.update_specifiers(file.specifiers)
-                summary.update_variables(file.specifiers.get('variable'))
+                summary.update_variables(file.specifiers)
+                summary.update_experiments(file.specifiers)
 
             else:
                 file.close_dataset()
 
             # close the log for this file
             file.close_log()
         else:
```

### Comparing `isimip-qc-3.0.3/isimip_qc/models.py` & `isimip-qc-3.1.0/isimip_qc/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import logging
 import shutil
+from pathlib import Path
 from collections import Counter
 
 import colorlog
 import jsonschema
 from prettytable.colortable import PrettyTable
 
 from isimip_utils.netcdf import (get_dimensions, get_global_attributes,
                                  get_variables, open_dataset_read,
                                  open_dataset_write)
 from isimip_utils.patterns import match_file
 from isimip_utils.exceptions import DidNotMatch
 
 from .config import settings
 from .utils.datamodel import call_cdo, call_nccopy
+from .utils.experiments import get_experiment
 from .utils.files import copy_file, move_file
 from .utils.logging import SUMMARY
 
 
 class File(object):
 
     def __init__(self, file_path):
+        file_path = Path(file_path).expanduser()
         self.path = file_path.relative_to(settings.UNCHECKED_PATH)
         self.abs_path = file_path
 
         self.infos = []
         self.warnings = []
         self.errors = []
         self.criticals = []
@@ -62,30 +65,35 @@
         else:
             self.dataset = open_dataset_read(self.abs_path)
 
     def close_dataset(self):
         self.dataset.close()
 
     def debug(self, message, *args):
-        self.logger.debug(message, *args)
+        if self.logger is not None:
+            self.logger.debug(message, *args)
 
     def info(self, message, *args, fix=None):
-        self.logger.info(message, *args)
+        if self.logger is not None:
+            self.logger.info(message, *args)
         self.infos.append((message % args, fix))
 
     def warn(self, message, *args, fix=None, fix_datamodel=None):
-        self.logger.warn(message, *args)
+        if self.logger is not None:
+            self.logger.warn(message, *args)
         self.warnings.append((message % args, fix, fix_datamodel))
 
     def error(self, message, *args):
-        self.logger.error(message, *args)
+        if self.logger is not None:
+            self.logger.error(message, *args)
         self.errors.append((message % args))
 
     def critical(self, message, *args):
-        self.logger.critical(message, *args)
+        if self.logger is not None:
+            self.logger.critical(message, *args)
         self.criticals.append((message % args))
 
     def fix_infos(self):
         for info in self.infos[:]:
             message, fix = info
             if fix:
                 fix['func'](*fix['args'])
@@ -151,15 +159,15 @@
     def is_clean(self):
         return not (self.has_warnings or self.has_errors or self.has_criticals)
 
     def get_logger(self):
         # setup a log handler for the command line and one for the file
         logger_name = str(self.path)
         logger = colorlog.getLogger(logger_name)
-        logger.setLevel(settings.LOG_PATH_LEVEL)
+        logger.setLevel(settings.LOG_LEVEL)
 
         # do not propagate messages to the root logger,
         # which is configured in settings.setup()
         logger.propagate = False
 
         # add handlers
         logger.addHandler(self.get_stream_handler())
@@ -215,33 +223,40 @@
 
 
 class Summary(object):
 
     def __init__(self):
         self.specifiers = {}
         self.variables = {}
+        self.experiments = Counter()
 
     def update_specifiers(self, specifiers):
         for identifier, specifier in specifiers.items():
             if identifier not in self.specifiers:
                 self.specifiers[identifier] = Counter()
             self.specifiers[identifier][specifier] += 1
 
-    def update_variables(self, variable):
+    def update_variables(self, specifiers):
+        variable = specifiers.get('variable')
         if variable is not None:
             if variable not in self.variables:
                 definition = settings.DEFINITIONS['variable'].get(variable)
                 self.variables[variable] = {
                     'specifier': variable,
                     'sectors': definition.get('sectors'),
                     'count': 1
                 }
             else:
                 self.variables[variable]['count'] += 1
 
+    def update_experiments(self, specifiers):
+        experiment = get_experiment(specifiers)
+        if experiment is not None:
+            self.experiments[experiment] += 1
+
     def log_specifiers(self):
         table = PrettyTable()
         table.field_names = ['Identifier', 'Specifier', 'Count']
         table.align['Identifier'] = 'l'
         table.align['Specifier'] = 'l'
         table.align['Count'] = 'r'
 
@@ -262,10 +277,23 @@
 
         for specifier, variable in self.variables.items():
             table.add_row([specifier, ', '.join(variable.get('sectors')), variable.get('count')])
 
         for line in table.get_string().splitlines():
             colorlog.log(SUMMARY, line)
 
+    def log_experiments(self):
+        table = PrettyTable()
+        table.field_names = ['Experiment', 'Count']
+        table.align['Experiment'] = 'l'
+        table.align['Count'] = 'r'
+
+        for experiment, count in self.experiments.items():
+            table.add_row([experiment, count])
+
+        for line in table.get_string().splitlines():
+            colorlog.log(SUMMARY, line)
+
     def log(self):
         self.log_specifiers()
         self.log_variables()
+        self.log_experiments()
```

### Comparing `isimip-qc-3.0.3/isimip_qc/utils/files.py` & `isimip-qc-3.1.0/isimip_qc/utils/files.py`

 * *Files identical despite different names*

### Comparing `isimip-qc-3.0.3/isimip_qc.egg-info/PKG-INFO` & `isimip-qc-3.1.0/isimip_qc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,165 +1,194 @@
 Metadata-Version: 2.1
 Name: isimip-qc
-Version: 3.0.3
+Version: 3.1.0
 Summary: A command line tool for the quality control of climate impact data of the ISIMIP project.
 Home-page: https://github.com/ISI-MIP/isimip-qc
 Author: Matthias Büchner, Jochen Klar
 License: MIT
-Description: ISIMIP quality control
-        ======================
-        
-        [![Python Version](https://img.shields.io/badge/python->=3.6-blue)](https://www.python.org/)
-        [![License](https://img.shields.io/badge/License-MIT-green)](https://github.com/ISI-MIP/isimip-qc/blob/master/LICENSE)
-        
-        A command line tool for the quality control of climate impact data of the ISIMIP project. It mainly covers tests of:
-        - the file name against the protocol schemas and patterns
-        - variables, dimensions and global attributes
-        - data model and types
-        - some consistency checks on the NetCDF time axis and
-        - if the data is within a valid value range (when defined in the ISIMIP protocol)
-        
-        **This is still work in progress.**
-        
-        
-        Setup
-        -----
-        
-        The application is written in Python (> 3.6) uses only dependencies, which can be installed without administrator priviledges. The installation of Python (and its developing packages), however differs from operating system to operating system. Optional Git is needed if the application is installed directly from GitHub. The installation of Python 3 and Git for different plattforms is documented [here](https://github.com/ISI-MIP/isimip-utils/blob/master/docs/prerequisites.md).
-        
-        The tool itself can be installed via pip. Usually you want to create a [virtual environment](https://docs.python.org/3/library/venv.html) first, but this is optional.
-        
-        ```bash
-        # setup venv on Linux/macOS/Windows WSL
-        python3 -m venv env
-        source env/bin/activate
-        
-        # setup venv on Windows cmd
-        python -m venv env
-        call env\Scripts\activate.bat
-        
-        # install from the Python Package Index (PyPI), recommended
-        pip install isimip-qc
-        
-        # update from PyPI
-        pip install --upgrade rdmo
-        
-        # install directly from GitHub
-        pip install git+https://github.com/ISI-MIP/isimip-qc
-        
-        # update from Github
-        pip install --upgrade git+https://github.com/ISI-MIP/isimip-qc
-        ```
-        
-        Usage
-        -----
-        
-        The tool has several options which can be inspected using the help option `-h, --help`:
-        
-        ```plain
-        usage: isimip-qc [-h] [--config-file CONFIG_FILE] [-c] [-m] [-O]
-                         [--unchecked-path UNCHECKED_PATH] [--checked-path CHECKED_PATH]
-                         [--protocol-location PROTOCOL_LOCATIONS] [--log-level LOG_LEVEL]
-                         [--log-path LOG_PATH] [--log-path-level LOG_PATH_LEVEL] [--include INCLUDE_LIST]
-                         [--exclude EXCLUDE_LIST] [-f] [-w] [-e] [-r [MINMAX]] [-nt] [--fix]
-                         [--fix-datamodel [FIX_DATAMODEL]] [--check CHECK] [--force-copy-move] [-V]
-                         schema_path
-        
-        Check ISIMIP files for matching protocol definitions
-        
-        positional arguments:
-          schema_path           ISIMIP schema_path, e.g. ISIMIP3a/OutputData/water_global
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --config-file CONFIG_FILE
-                                file path of the config file
-          -c, --copy            copy checked files to CHECKED_PATH if no warnings or errors were found
-          -m, --move            move checked files to CHECKED_PATH if no warnings or errors were found
-          -O, --overwrite       overwrite files in CHECKED_PATH if present. Default is False.
-          --unchecked-path UNCHECKED_PATH
-                                base path of the unchecked files
-          --checked-path CHECKED_PATH
-                                base path for the checked files
-          --protocol-location PROTOCOL_LOCATIONS
-                                URL or file path to the protocol when different from official repository
-          --log-level LOG_LEVEL
-                                log level (CRITICAL, ERROR, WARN, VRDETAIL, CHECKING, SUMMARY, INFO, or
-                                DEBUG) [default: CHECKING]
-          --log-path LOG_PATH   base path for the individual log files
-          --log-path-level LOG_PATH_LEVEL
-                                log level for the individual log files [default: WARN]
-          --include INCLUDE_LIST
-                                patterns of files to include. Exclude those that don't match any.
-          --exclude EXCLUDE_LIST
-                                patterns of files to exclude. Include only those that don't match any.
-          -f, --first-file      only process first file found in UNCHECKED_PATH
-          -w, --stop-on-warnings
-                                stop execution on warnings
-          -e, --stop-on-errors  stop execution on errors
-          -r [MINMAX], --minmax [MINMAX]
-                                test values for valid range (slow, argument MINMAX defaults to show the
-                                top 10 values)
-          -nt, --skip-time-span-check
-                                skip check for simulated time period
-          --fix                 try to fix warnings detected on the original files
-          --fix-datamodel [FIX_DATAMODEL]
-                                also fix warnings on data model found using NCCOPY or CDO (slow). Choose
-                                preferred tool per lower case argument.
-          --check CHECK         perform only one particular check
-          --force-copy-move     copy or move files despite errors
-          -V, --version         show program's version number and exit
-        ```
-        
-        The only mandatory argument is the `schema_path`, which specifies the pattern and schema to use. The `schema_path` consitst of the `simulation_round`, the `product`, and the `sector` seperated by slashes, e.g. `ISIMIP3a/OutputData/water_global`. If the only argument used is `schema_path`, the current user path when calling the tool should be same as the directory of the files to be checked.
-        
-        ### The options in detail
-        
-        * `--config-file`: Default values for the optional arguments are set in the code, but can also be provided via:
-            * a config file given by `--config-file`, or located at `isimip-qc.conf`, `~/.isimip-qc.conf`, or `/etc/isimip-qc.conf`. The config file needs to have a section `isimip-qc` and uses lower case variables and underscores, e.g.:
-                ```
-                [isimip-qc]
-                pattern_locations = /path/to/isimip-protocol-3/output/pattern/
-                schema_locations = path/to/isimip-protocol-3/output/schema/
-                ```
-        
-            * environment variables (in caps and with underscores, e.g. `UNCHECKED_PATH`).
-        * `-c, --copy` and `-m, --move`: Copy or move files that have successfully passed the checks to a final destination. Effective only when no warnings have been found on the file.
-        * '-O, --overwrite`: Allow overwriting of existing files in CHECKED_PATH. Default is to skip copy or move in case the target file is already present.
-        * `--unchecked-path UNCHECKED_PATH`: Any files in this folder **and** its subfolders will be included into the list of files to test.
-        * `--checked-path CHECKED_PATH`: Target folder for the `--copy` or `--move` operation. The subfolder structure below CHECKED_PATH will be created and filled according to the sub-structure found in UNCHECKED_PATH
-        * `--protocol-location PROTOCOL_LOCATIONS`: For working with local copies of the ISIMIP protocol (append `/output` to the cloned repositories folder). Omit option for using the online GitHub protocol versions for [ISIMIP2](https://github.com/ISI-MIP/isimip-protocol-2) or [ISIMIP3](https://github.com/ISI-MIP/isimip-protocol-3). An internet connection is required for reading the online protocols.
-        * `--log-level LOG_LEVEL`: Set the detail level of log output. Default is `CHECKING`. Log levels from `CRITICAL` to `VRDETAIL` will not show the file currently checked in the terminal but write all of them to the data file specific log file.<br>
-        `CRITICAL` : only very severe errors<br>
-        `ERROR`: all errors<br>
-        `WARN`: warnings and all errors<br>
-        `VRDETAIL`: same as CHECKING but with details on time and location of valid ranges violations when invoked with `--minmax` option. Very slow when violations are detected.<br>
-        `CHECKING`: includes warnings and errors<br>
-        `SUMMARY`: includes warnings, errors and the summary shown at the end<br>
-        `INFO`: includes `SUMMARY` and details for successful checks<br>
-        `DEBUG`: all the above plus details for some debugging cases.
-        * `--log-path LOG_PATH`: Also write the logs to a file where the folder structure below LOG_PATH is taken from UNCHECKED_PATH.
-        * `--log-path-level LOG_PATH_LEVEL`: The log level used for the file specific logs below `LOG_PATH`. The default is `WARN` and should suffice for most cases.
-        * `--include INCLUDE_LIST` : Provide a comma-separated list of strings to include for the checks if any of them matches the file path or name, e.g. 'daily,dis' will only check `*daily*` or `*discharge*` files while skipping others.
-        * `--exclude EXCLUDE_LIST` : Provide a comma-separated list of strings to exclude from the checks if any of them matches the file path or name, e.g. 'monthly,histsoc' will skip any `*monthly*` or `*histsoc*` files.
-        * `-f, --first-file`: Only test the first file found in UNCHECKED_PATH. Useful for revealing issues that may occur on all your files.
-        * `-w, --stop-on-warnings`: The tool will stop after the first file where WARNINGs have been identified.
-        * `-e, --stop-on-errors`: The tool will stop after the first file where ERRORs have been identified.
-        * `-r [MINMAX], --minmax [MINMAX]`: Test the data for valid ranges when defined in the protocol. Per default and when violations are detected the top 20 minimum and maximum values along with their time and geographic location will be logged as well. MINMAX is optional and defines how many values should be reported instead of 20. This test drastically slows down the run time of the tool.
-        * -nt, --skip-time-span-check: Skip checking non-dialy data for proper coverage of simulation periods.
-        * `--fix`: Activates a number of fixes for WARNINGs by taking the default values from the protocol, e.g. variable attributes and units. In additions an unique identifier (UUID), the version of this tool and the protocol version (by a git hash) are being written to the global attributes section of the NetCDF file. **Attention**: Fixes and are going to be applied on **your original files** in UNCHECKED_PATH.
-        * `--fix-datamodel [FIX_DATAMODEL]`: Fixes to the data model and compression level of the NetCDF file can't be made on-the-fly with the libraries used by the tool. We here rely on the external tools [cdo](https://code.mpimet.mpg.de/projects/cdo/) or nccopy (from the [NetCDF library](https://www.unidata.ucar.edu/software/netcdf/)) to rewrite the entire file. Default is `nccopy`. Please try to create the files with the proper data model (compressed NETCDF4_CLASSIC) in your postprocessing chain before submitting them to the data server.
-        * `--check CHECK`: Perform only one particular check. The list of CHECKs can be taken from the funtions defined in the `isimip_qc/checks/*.py` files.
-        * `--force-copy-move`: Copy or move files despite errors found during checks.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+ISIMIP quality control
+======================
+
+[![Python Version](https://img.shields.io/badge/python->=3.6-blue)](https://www.python.org/)
+[![License](https://img.shields.io/badge/License-MIT-green)](https://github.com/ISI-MIP/isimip-qc/blob/master/LICENSE)
+
+A command line tool for the quality control of climate impact data of the ISIMIP project. It mainly covers tests of:
+- the file name against the protocol schemas and patterns
+- variables, dimensions and global attributes
+- data model and types
+- some consistency checks on the NetCDF time axis and
+- if the data is within a valid value range (when defined in the ISIMIP protocol)
+
+**This is still work in progress.**
+
+
+Setup
+-----
+
+The application is written in Python (> 3.6) uses only dependencies, which can be installed without administrator priviledges. The installation of Python (and its developing packages), however differs from operating system to operating system. Optional Git is needed if the application is installed directly from GitHub. The installation of Python 3 and Git for different plattforms is documented [here](https://github.com/ISI-MIP/isimip-utils/blob/master/docs/prerequisites.md).
+
+The tool itself can be installed via pip. Usually you want to create a [virtual environment](https://docs.python.org/3/library/venv.html) first, but this is optional.
+
+```bash
+# setup venv on Linux/macOS/Windows WSL
+python3 -m venv env
+source env/bin/activate
+
+# setup venv on Windows cmd
+python -m venv env
+call env\Scripts\activate.bat
+
+# install from the Python Package Index (PyPI), recommended
+pip install isimip-qc
+
+# update from PyPI
+pip install --upgrade rdmo
+
+# install directly from GitHub
+pip install git+https://github.com/ISI-MIP/isimip-qc
+
+# update from Github
+pip install --upgrade git+https://github.com/ISI-MIP/isimip-qc
+```
+
+Usage
+-----
+
+The tool has several options which can be inspected using the help option `-h, --help`:
+
+```plain
+usage: isimip-qc [-h] [--config-file CONFIG_FILE] [-c] [-m] [-O]
+                 [--unchecked-path UNCHECKED_PATH] [--checked-path CHECKED_PATH]
+                 [--protocol-location PROTOCOL_LOCATIONS] [--log-level LOG_LEVEL]
+                 [--log-path LOG_PATH] [--log-path-level LOG_PATH_LEVEL] [--include INCLUDE_LIST]
+                 [--exclude EXCLUDE_LIST] [-f] [-w] [-e] [-r [MINMAX]] [-nt] [--fix]
+                 [--fix-datamodel [FIX_DATAMODEL]] [--check CHECK] [--force-copy-move] [-V]
+                 schema_path
+
+Check ISIMIP files for matching protocol definitions
+
+positional arguments:
+  schema_path           ISIMIP schema_path, e.g. ISIMIP3a/OutputData/water_global
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --config-file CONFIG_FILE
+                        file path of the config file
+  -c, --copy            copy checked files to CHECKED_PATH if no warnings or errors were found
+  -m, --move            move checked files to CHECKED_PATH if no warnings or errors were found
+  -O, --overwrite       overwrite files in CHECKED_PATH if present. Default is False.
+  --unchecked-path UNCHECKED_PATH
+                        base path of the unchecked files
+  --checked-path CHECKED_PATH
+                        base path for the checked files
+  --protocol-location PROTOCOL_LOCATIONS
+                        URL or file path to the protocol when different from official repository
+  --log-level LOG_LEVEL
+                        log level (CRITICAL, ERROR, WARN, VRDETAIL, CHECKING, SUMMARY, INFO, or
+                        DEBUG) [default: CHECKING]
+  --log-path LOG_PATH   base path for the individual log files
+  --log-path-level LOG_PATH_LEVEL
+                        log level for the individual log files [default: WARN]
+  --include INCLUDE_LIST
+                        patterns of files to include. Exclude those that don't match any.
+  --exclude EXCLUDE_LIST
+                        patterns of files to exclude. Include only those that don't match any.
+  -f, --first-file      only process first file found in UNCHECKED_PATH
+  -w, --stop-on-warnings
+                        stop execution on warnings
+  -e, --stop-on-errors  stop execution on errors
+  -r [MINMAX], --minmax [MINMAX]
+                        test values for valid range (slow, argument MINMAX defaults to show the
+                        top 10 values)
+  -nt, --skip-time-span-check
+                        skip check for simulated time period
+  --fix                 try to fix warnings detected on the original files
+  --fix-datamodel [FIX_DATAMODEL]
+                        also fix warnings on data model found using NCCOPY or CDO (slow). Choose
+                        preferred tool per lower case argument.
+  --check CHECK         perform only one particular check
+  --force-copy-move     copy or move files despite errors
+  -V, --version         show program's version number and exit
+```
+
+The only mandatory argument is the `schema_path`, which specifies the pattern and schema to use. The `schema_path` consitst of the `simulation_round`, the `product`, and the `sector` seperated by slashes, e.g. `ISIMIP3a/OutputData/water_global`. If the only argument used is `schema_path`, the current user path when calling the tool should be same as the directory of the files to be checked.
+
+### The options in detail
+
+* `--config-file`: Default values for the optional arguments are set in the code, but can also be provided via:
+    * a config file given by `--config-file`, or located at `isimip-qc.conf`, `~/.isimip-qc.conf`, or `/etc/isimip-qc.conf`. The config file needs to have a section `isimip-qc` and uses lower case variables and underscores, e.g.:
+        ```
+        [isimip-qc]
+        pattern_locations = /path/to/isimip-protocol-3/output/pattern/
+        schema_locations = path/to/isimip-protocol-3/output/schema/
+        ```
+
+    * environment variables (in caps and with underscores, e.g. `UNCHECKED_PATH`).
+* `-c, --copy` and `-m, --move`: Copy or move files that have successfully passed the checks to a final destination. Effective only when no warnings have been found on the file.
+* '-O, --overwrite`: Allow overwriting of existing files in CHECKED_PATH. Default is to skip copy or move in case the target file is already present.
+* `--unchecked-path UNCHECKED_PATH`: Any files in this folder **and** its subfolders will be included into the list of files to test.
+* `--checked-path CHECKED_PATH`: Target folder for the `--copy` or `--move` operation. The subfolder structure below CHECKED_PATH will be created and filled according to the sub-structure found in UNCHECKED_PATH
+* `--protocol-location PROTOCOL_LOCATIONS`: For working with local copies of the ISIMIP protocol (append `/output` to the cloned repositories folder). Omit option for using the online GitHub protocol versions for [ISIMIP2](https://github.com/ISI-MIP/isimip-protocol-2) or [ISIMIP3](https://github.com/ISI-MIP/isimip-protocol-3). An internet connection is required for reading the online protocols.
+* `--log-level LOG_LEVEL`: Set the detail level of log output. Default is `CHECKING`. Log levels from `CRITICAL` to `VRDETAIL` will not show the file currently checked in the terminal but write all of them to the data file specific log file.<br>
+`CRITICAL` : only very severe errors<br>
+`ERROR`: all errors<br>
+`WARN`: warnings and all errors<br>
+`VRDETAIL`: same as CHECKING but with details on time and location of valid ranges violations when invoked with `--minmax` option. Very slow when violations are detected.<br>
+`CHECKING`: includes warnings and errors<br>
+`SUMMARY`: includes warnings, errors and the summary shown at the end<br>
+`INFO`: includes `SUMMARY` and details for successful checks<br>
+`DEBUG`: all the above plus details for some debugging cases.
+* `--log-path LOG_PATH`: Also write the logs to a file where the folder structure below LOG_PATH is taken from UNCHECKED_PATH.
+* `--log-path-level LOG_PATH_LEVEL`: The log level used for the file specific logs below `LOG_PATH`. The default is `WARN` and should suffice for most cases.
+* `--include INCLUDE_LIST` : Provide a comma-separated list of strings to include for the checks if any of them matches the file path or name, e.g. 'daily,dis' will only check `*daily*` or `*discharge*` files while skipping others.
+* `--exclude EXCLUDE_LIST` : Provide a comma-separated list of strings to exclude from the checks if any of them matches the file path or name, e.g. 'monthly,histsoc' will skip any `*monthly*` or `*histsoc*` files.
+* `-f, --first-file`: Only test the first file found in UNCHECKED_PATH. Useful for revealing issues that may occur on all your files.
+* `-w, --stop-on-warnings`: The tool will stop after the first file where WARNINGs have been identified.
+* `-e, --stop-on-errors`: The tool will stop after the first file where ERRORs have been identified.
+* `-r [MINMAX], --minmax [MINMAX]`: Test the data for valid ranges when defined in the protocol. Per default and when violations are detected the top 20 minimum and maximum values along with their time and geographic location will be logged as well. MINMAX is optional and defines how many values should be reported instead of 20. This test drastically slows down the run time of the tool.
+* -nt, --skip-time-span-check: Skip checking non-dialy data for proper coverage of simulation periods.
+* `--fix`: Activates a number of fixes for WARNINGs by taking the default values from the protocol, e.g. variable attributes and units. In additions an unique identifier (UUID), the version of this tool and the protocol version (by a git hash) are being written to the global attributes section of the NetCDF file. **Attention**: Fixes and are going to be applied on **your original files** in UNCHECKED_PATH.
+* `--fix-datamodel [FIX_DATAMODEL]`: Fixes to the data model and compression level of the NetCDF file can't be made on-the-fly with the libraries used by the tool. We here rely on the external tools [cdo](https://code.mpimet.mpg.de/projects/cdo/) or nccopy (from the [NetCDF library](https://www.unidata.ucar.edu/software/netcdf/)) to rewrite the entire file. Default is `nccopy`. Please try to create the files with the proper data model (compressed NETCDF4_CLASSIC) in your postprocessing chain before submitting them to the data server.
+* `--check CHECK`: Perform only one particular check. The list of CHECKs can be taken from the funtions defined in the `isimip_qc/checks/*.py` files.
+* `--force-copy-move`: Copy or move files despite errors found during checks.
+
+
+Scripts/Notebooks
+-----------------
+
+The different functions of the tool can also be used in Python scripts or Jupyter Notebooks. Before any functions are called, the global settings object needs to be initialized using the `init_settings` function, e.g.:
+
+```python
+from isimip_qc.checks import checks
+from isimip_qc.main import init_settings
+from isimip_qc.models import File
+
+settings = init_settings(
+    schema_path='ISIMIP3b/OutputData/water_global',
+    config_file='~/data/isimip/isimip.conf'
+)
+
+file_path = '~/data/isimip/qc/unchecked/h08_ipsl-cm6a-lr_w5e5_ssp585_2015soc_default_dis_global_monthly_2015_2100.nc'
+
+file = File(file_path)
+file.open_log()
+file.match()
+file.open_dataset()
+
+for check in checks:
+    check(file)
+
+file.close_dataset()
+```
```

### Comparing `isimip-qc-3.0.3/isimip_qc.egg-info/SOURCES.txt` & `isimip-qc-3.1.0/isimip_qc.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 isimip_qc.egg-info/requires.txt
 isimip_qc.egg-info/top_level.txt
 isimip_qc/checks/3d.py
 isimip_qc/checks/__init__.py
 isimip_qc/checks/attributes.py
 isimip_qc/checks/dataset.py
 isimip_qc/checks/dimensions.py
+isimip_qc/checks/experiments.py
 isimip_qc/checks/variables/__init__.py
 isimip_qc/checks/variables/latlon.py
 isimip_qc/checks/variables/time.py
 isimip_qc/checks/variables/time_resolution.py
 isimip_qc/checks/variables/var.py
 isimip_qc/checks/variables/var3d.py
 isimip_qc/utils/__init__.py
 isimip_qc/utils/datamodel.py
+isimip_qc/utils/experiments.py
 isimip_qc/utils/files.py
 isimip_qc/utils/logging.py
```

### Comparing `isimip-qc-3.0.3/setup.cfg` & `isimip-qc-3.1.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 [options]
 python_requires = >=3.6
 packages = find:
 include_package_data = true
 install_requires = 
 	colorlog
-	isimip-utils
+	isimip-utils>=1.2
 	jsonschema
 	netCDF4
 	prettytable
 	python-dotenv
 	requests
 
 [options.entry_points]
```


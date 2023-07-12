# Comparing `tmp/mighty_logger-0.9.2.tar.gz` & `tmp/mighty_logger-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mighty_logger-0.9.2.tar", last modified: Fri Jun 30 19:35:28 2023, max compression
+gzip compressed data, was "mighty_logger-0.9.3.tar", last modified: Wed Jul 12 09:58:22 2023, max compression
```

## Comparing `mighty_logger-0.9.2.tar` & `mighty_logger-0.9.3.tar`

### file list

```diff
@@ -1,40 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.903619 mighty_logger-0.9.2/
--rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.9.2/LICENSE
--rw-rw-rw-   0        0        0    10873 2023-06-30 19:35:28.904619 mighty_logger-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     9941 2023-06-30 19:23:51.000000 mighty_logger-0.9.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.723312 mighty_logger-0.9.2/mighty_logger/
--rw-rw-rw-   0        0        0      846 2023-06-30 19:00:03.000000 mighty_logger-0.9.2/mighty_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.802614 mighty_logger-0.9.2/mighty_logger/basic/
--rw-rw-rw-   0        0        0      808 2023-06-30 12:57:57.000000 mighty_logger-0.9.2/mighty_logger/basic/__init__.py
--rw-rw-rw-   0        0        0     8659 2023-06-30 18:38:56.000000 mighty_logger-0.9.2/mighty_logger/basic/basic_logger.py
--rw-rw-rw-   0        0        0     1805 2023-06-30 18:18:43.000000 mighty_logger-0.9.2/mighty_logger/basic/exceptions.py
--rw-rw-rw-   0        0        0     3379 2023-06-30 13:42:10.000000 mighty_logger-0.9.2/mighty_logger/basic/exporter.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.863621 mighty_logger-0.9.2/mighty_logger/basic/lib_types/
--rw-rw-rw-   0        0        0      961 2023-06-30 12:33:00.000000 mighty_logger-0.9.2/mighty_logger/basic/lib_types/__init__.py
--rw-rw-rw-   0        0        0     1163 2023-06-30 13:42:10.000000 mighty_logger-0.9.2/mighty_logger/basic/lib_types/animation_type.py
--rw-rw-rw-   0        0        0     2079 2023-06-30 13:42:10.000000 mighty_logger-0.9.2/mighty_logger/basic/lib_types/entry_type.py
--rw-rw-rw-   0        0        0     1415 2023-06-30 13:42:10.000000 mighty_logger-0.9.2/mighty_logger/basic/lib_types/environment_type.py
--rw-rw-rw-   0        0        0      891 2023-06-30 18:04:36.000000 mighty_logger-0.9.2/mighty_logger/basic/lib_types/sorting_key_type.py
--rw-rw-rw-   0        0        0     6706 2023-06-30 13:06:13.000000 mighty_logger-0.9.2/mighty_logger/basic/lib_types/text_buffer_type.py
--rw-rw-rw-   0        0        0     8207 2023-06-30 13:47:39.000000 mighty_logger-0.9.2/mighty_logger/basic/modifier.py
--rw-rw-rw-   0        0        0      842 2023-06-30 13:13:13.000000 mighty_logger-0.9.2/mighty_logger/basic/singleton.py
--rw-rw-rw-   0        0        0    10557 2023-06-30 13:13:13.000000 mighty_logger-0.9.2/mighty_logger/basic/text_buffer.py
--rw-rw-rw-   0        0        0    31663 2023-06-30 19:11:51.000000 mighty_logger-0.9.2/mighty_logger/mighty_logger.py
--rw-rw-rw-   0        0        0     7446 2023-06-30 19:10:22.000000 mighty_logger-0.9.2/mighty_logger/simple_logger.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.870619 mighty_logger-0.9.2/mighty_logger/src/
--rw-rw-rw-   0        0        0      928 2023-06-30 14:44:07.000000 mighty_logger-0.9.2/mighty_logger/src/__init__.py
--rw-rw-rw-   0        0        0     9983 2023-06-30 14:44:07.000000 mighty_logger-0.9.2/mighty_logger/src/animations.py
--rw-rw-rw-   0        0        0     4664 2023-06-30 14:44:07.000000 mighty_logger-0.9.2/mighty_logger/src/ansi_format.py
--rw-rw-rw-   0        0        0     9688 2023-06-30 14:46:54.000000 mighty_logger-0.9.2/mighty_logger/src/color_picker.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.875620 mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/
--rw-rw-rw-   0        0        0      865 2023-06-30 14:14:17.000000 mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/__init__.py
--rw-rw-rw-   0        0        0    47441 2023-06-30 14:22:00.000000 mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/entry_types.py
--rw-rw-rw-   0        0        0     1030 2023-06-30 14:14:17.000000 mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/environments.py
--rw-rw-rw-   0        0        0      956 2023-06-30 18:04:36.000000 mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/sorting_keys.py
-drwxrwxrwx   0        0        0        0 2023-06-30 19:35:28.756613 mighty_logger-0.9.2/mighty_logger.egg-info/
--rw-rw-rw-   0        0        0    10873 2023-06-30 19:35:28.000000 mighty_logger-0.9.2/mighty_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1140 2023-06-30 19:35:28.000000 mighty_logger-0.9.2/mighty_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 19:35:28.000000 mighty_logger-0.9.2/mighty_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-30 19:35:28.000000 mighty_logger-0.9.2/mighty_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1869 2023-06-30 19:23:51.000000 mighty_logger-0.9.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 19:35:28.905620 mighty_logger-0.9.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 09:58:22.763353 mighty_logger-0.9.3/
+-rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.9.3/LICENSE
+-rw-rw-rw-   0        0        0     9902 2023-07-12 09:58:22.764353 mighty_logger-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8973 2023-07-12 09:39:43.000000 mighty_logger-0.9.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 09:58:22.678766 mighty_logger-0.9.3/mighty_logger/
+-rw-rw-rw-   0        0        0      861 2023-07-04 16:28:33.000000 mighty_logger-0.9.3/mighty_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 09:58:22.735628 mighty_logger-0.9.3/mighty_logger/basic/
+-rw-rw-rw-   0        0        0      836 2023-07-04 16:29:00.000000 mighty_logger-0.9.3/mighty_logger/basic/__init__.py
+-rw-rw-rw-   0        0        0     7576 2023-07-04 17:04:11.000000 mighty_logger-0.9.3/mighty_logger/basic/basic_logger.py
+-rw-rw-rw-   0        0        0     1370 2023-07-02 15:20:50.000000 mighty_logger-0.9.3/mighty_logger/basic/exceptions.py
+-rw-rw-rw-   0        0        0     2607 2023-07-04 14:49:44.000000 mighty_logger-0.9.3/mighty_logger/basic/exporter.py
+drwxrwxrwx   0        0        0        0 2023-07-12 09:58:22.754351 mighty_logger-0.9.3/mighty_logger/basic/lib_types/
+-rw-rw-rw-   0        0        0      934 2023-07-02 15:05:20.000000 mighty_logger-0.9.3/mighty_logger/basic/lib_types/__init__.py
+-rw-rw-rw-   0        0        0      912 2023-07-02 15:18:08.000000 mighty_logger-0.9.3/mighty_logger/basic/lib_types/animation_type.py
+-rw-rw-rw-   0        0        0     1798 2023-07-02 15:18:23.000000 mighty_logger-0.9.3/mighty_logger/basic/lib_types/entry_type.py
+-rw-rw-rw-   0        0        0     1290 2023-07-02 15:20:29.000000 mighty_logger-0.9.3/mighty_logger/basic/lib_types/environment_type.py
+-rw-rw-rw-   0        0        0      797 2023-07-02 15:20:29.000000 mighty_logger-0.9.3/mighty_logger/basic/lib_types/sorting_key_type.py
+-rw-rw-rw-   0        0        0     2623 2023-07-04 17:40:06.000000 mighty_logger-0.9.3/mighty_logger/basic/lib_types/text_buffer_type.py
+-rw-rw-rw-   0        0        0     7018 2023-07-04 14:49:44.000000 mighty_logger-0.9.3/mighty_logger/basic/modifier.py
+-rw-rw-rw-   0        0        0      757 2023-07-02 15:22:45.000000 mighty_logger-0.9.3/mighty_logger/basic/singleton.py
+-rw-rw-rw-   0        0        0     9274 2023-07-04 16:52:30.000000 mighty_logger-0.9.3/mighty_logger/basic/text_buffer.py
+-rw-rw-rw-   0        0        0    19889 2023-07-11 17:36:31.000000 mighty_logger-0.9.3/mighty_logger/mighty_logger.py
+-rw-rw-rw-   0        0        0     5994 2023-07-09 10:51:28.000000 mighty_logger-0.9.3/mighty_logger/simple_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-12 09:58:22.762354 mighty_logger-0.9.3/mighty_logger/src/
+-rw-rw-rw-   0        0        0     1081 2023-07-04 14:45:31.000000 mighty_logger-0.9.3/mighty_logger/src/__init__.py
+-rw-rw-rw-   0        0        0     9825 2023-07-02 15:30:09.000000 mighty_logger-0.9.3/mighty_logger/src/animations.py
+-rw-rw-rw-   0        0        0     3541 2023-07-02 15:30:09.000000 mighty_logger-0.9.3/mighty_logger/src/ansi_format.py
+-rw-rw-rw-   0        0        0     6656 2023-07-02 15:30:09.000000 mighty_logger-0.9.3/mighty_logger/src/color_picker.py
+-rw-rw-rw-   0        0        0    36171 2023-07-02 15:24:11.000000 mighty_logger-0.9.3/mighty_logger/src/entry_types.py
+-rw-rw-rw-   0        0        0      968 2023-07-02 15:24:25.000000 mighty_logger-0.9.3/mighty_logger/src/environments.py
+-rw-rw-rw-   0        0        0      901 2023-07-02 15:24:25.000000 mighty_logger-0.9.3/mighty_logger/src/sorting_keys.py
+drwxrwxrwx   0        0        0        0 2023-07-12 09:58:22.689378 mighty_logger-0.9.3/mighty_logger.egg-info/
+-rw-rw-rw-   0        0        0     9902 2023-07-12 09:58:22.000000 mighty_logger-0.9.3/mighty_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1026 2023-07-12 09:58:22.000000 mighty_logger-0.9.3/mighty_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 09:58:22.000000 mighty_logger-0.9.3/mighty_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-12 09:58:22.000000 mighty_logger-0.9.3/mighty_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1823 2023-07-04 14:50:52.000000 mighty_logger-0.9.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 09:58:22.765354 mighty_logger-0.9.3/setup.cfg
```

### Comparing `mighty_logger-0.9.2/LICENSE` & `mighty_logger-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.9.2/PKG-INFO` & `mighty_logger-0.9.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mighty_logger
-Version: 0.9.2
-Summary: Powerful functional logger
+Version: 0.9.3
+Summary: Mighty functional logger
 Author-email: Kalynovsky 'Nakamura Akira' Valentin <nakama3942@gmail.com>
 License: Apache License Version 2.0
 Project-URL: Repository, https://github.com/Nakama3942/mighty_logger
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,55 +21,47 @@
 [![template](https://img.shields.io/badge/Repository-template-darkred?style=for-the-badge)](https://github.com/Nakama3942/template_rep)
 [![GitHub license](https://img.shields.io/github/license/Nakama3942/mighty_logger?color=gold&style=for-the-badge)](https://github.com/Nakama3942/mighty_logger/blob/master/LICENSE)
 [![CHANGELOG](https://img.shields.io/badge/here-CHANGELOG-yellow?style=for-the-badge)](https://github.com/Nakama3942/mighty_logger/blob/master/CHANGELOG.md)
 [![PULL_REQUEST_TEMPLATE](https://img.shields.io/badge/here-PULL_REQUEST_TEMPLATE-orange?style=for-the-badge)](https://github.com/Nakama3942/mighty_logger/blob/master/.github/PULL_REQUEST_TEMPLATE.md)
 
 ![PyPI](https://img.shields.io/pypi/v/mighty-logger?color=yellow&logo=pypi&logoColor=white&style=for-the-badge)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/Nakama3942/mighty_logger?label=latest%20release&logo=github&style=for-the-badge)
-![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Nakama3942/mighty_logger?color=orange&include_prereleases&label=latest%20pre-release&logo=github&style=for-the-badge)
 ![GitHub commits since latest release (by date including pre-releases)](https://img.shields.io/github/commits-since/Nakama3942/mighty_logger/v0.5.0?include_prereleases&style=for-the-badge)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mighty-logger?style=for-the-badge)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/mighty-logger?style=for-the-badge)
 ![PyPI - Format](https://img.shields.io/pypi/format/mighty-logger?label=PyPI%20format&style=for-the-badge)
 ![PyPI - Status](https://img.shields.io/pypi/status/mighty-logger?label=PyPI%20status&style=for-the-badge)
 
 ![GitHub last commit](https://img.shields.io/github/last-commit/Nakama3942/mighty_logger?style=for-the-badge)
 ![GitHub Release Date](https://img.shields.io/github/release-date/Nakama3942/mighty_logger?style=for-the-badge)
-![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/Nakama3942/mighty_logger?label=%28pre-%29release%20date&style=for-the-badge)
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/Nakama3942/mighty_logger?color=darkgreen&style=for-the-badge)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Nakama3942/mighty_logger?color=darkgreen&style=for-the-badge)
 ![Lines of code](https://img.shields.io/tokei/lines/github/Nakama3942/mighty_logger?style=for-the-badge)
 
 </div>
 
 # Mighty Logger
 
 ### Content
 
-- [Qt_Сolored-logger](#mighty-logger)
-  - [Content](#content)
-  - [Preamble](#preamble)
-  - [Overview](#overview)
-  - [Important releases](#important-releases)
-  - [LICENSE](#license)
-  - [Installation](#installation)
-  - [Usage](#usage)
-  - [Additional functionality](#additional-functionality)
-  - [Data](#data)
-  - [Troubleshooting](#troubleshooting)
-  - [Authors](#authors)
+- [Mighty Logger](#mighty-logger)
+	- [Content](#content)
+	- [Preamble](#preamble)
+	- [Overview](#overview)
+    - [LICENSE](#license)
+	- [Important releases](#important-releases)
+	- [Features](#features)
+	- [Installation](#installation)
+	- [Usage](#usage)
+	- [Troubleshooting](#troubleshooting)
+	- [Authors](#authors)
 
 ## Preamble
 
-<!--
-This library it was renamed to "Mighty logger" but before this library named is "Qt Colored logger". Old commits may search in this repository, but download old build may on next link: https://pypi.org/project/qt-colored-logger/ .
--->
-
 > I often came across the opinion that it is better to use not standard output to the console, but full-fledged logging... However, the standard libraries do not provide exactly what I need... Therefore, I decided to make my own library! Which will implement the functionality I need.
 
 I was inspired by the [colored-logs](https://pypi.org/project/colored-logs/) library.
 
 ---
 
 *This library has been renamed to "Mighty logger", but this library used to be called "Qt Colored logger". You can search for old commits in this repository, but you can download the old build from the [link](https://pypi.org/project/qt-colored-logger/).*
@@ -78,118 +70,125 @@
 
 ## Overview
 
 The library implements the formation of a beautifully formatted colored text, similar to a log, which has all the necessary information:
 
 - Device name and registered profile, system name, etc. (this data is displayed only once at the beginning of the logging)
 - Log entry time
-- Log entry status
+- Log entry category
 - Log entry type
 - Entry message
 
-Any information to the output can be turned off (according to the default, everything is included). It is also possible to change the output settings during the logging process. It is possible to change the colors of the foreground text and the background, icons ~~and animations~~.
+Any information to the output can be turned off (according to the default, everything is included). It is also possible to change the output settings during the logging process. It is possible to change the colors of the foreground text and the background, icons and animations.
+
+- [Content](#content)
+
+## LICENSE
+
+The full text of the license can be found at the following [link](https://github.com/Nakama3942/mighty_logger/blob/master/LICENSE).
+
+> Copyright © 2023 Kalynovsky Valentin. All rights reserved.
+>
+> Licensed under the Apache License, Version 2.0 (the "License");
+> you may not use this file except in compliance with the License.
+> You may obtain a copy of the License at
+>
+>     http://www.apache.org/licenses/LICENSE-2.0
+>
+> Unless required by applicable law or agreed to in writing, software
+> distributed under the License is distributed on an "AS IS" BASIS,
+> WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+> See the License for the specific language governing permissions and
 
 - [Content](#content)
 
 ## Important releases
 
-<details><summary>See the important releases (possible spoilers)</summary>
+<details><summary>See the important releases</summary>
 
 - [x] v0.0.1 - Alpha-release (the very first version of the simplest Logger has been published)
 - [x] v0.0.2 - Little update (added multiple entry types and colors)
 - [x] v0.0.3 - Types update (added even more multiple entry types and colors)
 - [x] v0.0.4 - Color update (added the entire X11 color table and reworked the color system)
-- [x] v0.1.0 - First official release (complete basic HTML logger)
+- [x] v0.1.0 - "First release" update (complete basic HTML logger)
 - [x] v0.2.0 - Structural update (added basic console logger with HTML base)
+- [x] v0.2.1 - Protections update (hidden part of the functionality)
 - [x] v0.3.0 - Background update (added background for log entries)
 - [x] v0.4.0 - Buffer update (added text buffer)
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
-- [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
+- [x] v0.5.1 - Hints update (added hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
-- [x] v0.6.1 - Animation update (added animations in processes)
-- [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
+- [x] v0.6.1 - Animation update (extended animations in processes)
+- [x] v0.7.0 - "Buffer improvement" update (buffer development completed)
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
 - [x] v0.8.0 - Export update (added conversion to csv)
 - [x] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [x] v0.9.1 - Documenting update (documented library)
 - [x] v0.9.2 - Feature update (made optimizations)
-- [ ] v0.9.3 - Web docs update (added generation of web docs)
+- [x] v0.9.3 - Web docs update (added generation of web docs)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
 
-## LICENSE
-
-The full text of the license can be found at the following [link](https://github.com/Nakama3942/mighty_logger/blob/master/LICENSE).
-
-> Copyright © 2023 Kalynovsky Valentin. All rights reserved.
-> 
-> Licensed under the Apache License, Version 2.0 (the "License");
-> you may not use this file except in compliance with the License.
-> You may obtain a copy of the License at
-> 
->     http://www.apache.org/licenses/LICENSE-2.0
-> 
-> Unless required by applicable law or agreed to in writing, software
-> distributed under the License is distributed on an "AS IS" BASIS,
-> WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-> See the License for the specific language governing permissions and
+## Features
 
-- [Content](#content)
+- **Support for a large number of logger entry types** (empty, entry: debug, debug_performance, performance, event, audit, metrics, user, message, info, notice, warning, error, critical, resolved, unresolved)
+- **Support for five working environments** (CONSOLE, PLAIN_CONSOLE, HTML, MARKDOWN, PLAIN)
+- **Provides publisher methods**
+- **Provides to sort the logs**
+- **Provides to search the logs**
+- **Provides to select the desired logs**
+- **Provides to export logs to csv**
+- **Implemented own Text Buffer**
+- **Provided the ability to control the Buffer**
+- **Logs can be saved and loaded**
+- **Implemented wrapper method for Python input()**
+- **You can run logging Processes**
+- **You can run logging Timers**
+- **Implemented a simplified Logger class**
+- **When creating a Logger, an entry is created about the characteristics of the system**
+- **Show time of logging for every entry log**
+- **Provided are more than 20 animations for indefinite processes and 6 for definite processes**
+- **Provided are ANSI escape code table**
+- **Provides colors in RGB, HEX, ANSI**
+- **Provided are 4 sorting options** (by time, by reverse time, by category, by type)
+- **Provided are 5 exceptions**
 
 ## Installation
 
-Despite the fact that the library was originally developed for use in PyQt, it does not require PyQt to be installed, since this framework for outputting to Text fields, which support not only Plain Text, uses HTML and this library simply simplifies the logging process, since the creation process already formatted strings is registered in this library.
-
 To install the library, enter the command:
 
 ```sh
 pip install mighty_logger
 ```
 
 ## Usage
 
-ATTENTION!!! OUTDATED MATERIAL! RELEVANCE - v0.6.1! WILL BE OVERWRITTEN IN v0.9.1!
-
 This is the simplest example of using the library:
 
 ```python
 from mighty_logger import Logger
-from mighty_logger.src import StatusMessagePatterns
 
 if __name__ == "__main__":
-	logger = Logger(program_name="Test", console_width=115)
-	logger.message(status_message=StatusMessagePatterns.custom("Hooray"), message_text="Hello world!")
+	logger = Logger()
+	logger.message("Hello world!")
+	print("\n".join(logger.might.buffer))
 ```
 
-The outputs in console will contain the following text (GitHub, PyPi and possibly some other sites do not support displaying colors in Markdown - use resources that support them, such as PyCharm):
+The outputs in console will contain the following text:
 
 <pre>
-<span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span>
-<span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry>         </span><span style='color: #da70d6;'>*2023-06-08 14:01:39.423493 </span>💬 <span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span>
+-Unknown?entry> $DESKTOP-8KG0R64:User:Windows:10.0.19045:64bit:WindowsPE:AMD64
+-?entry>          *2023-07-04 21:12:05.919593 📝 #STATUS: @MESSAGE - Hello world!
 </pre>
 
-See the APPLYING.md file for more details.
-
-- [Content](#content)
-
-## *Additional functionality*
-
-*Additional functionality is also planned. Let's keep it a secret for now. Let it be a surprise.*
-
-- [Content](#content)
-
-## Data
-
-See the DATA.md file.
-
 - [Content](#content)
 
 ## Troubleshooting
 
 All functionality of the library has been tested by me, but if you have problems using it, the code does not work, have suggestions for optimization or advice for improving the style of the code and the name - I invite you [here](https://github.com/Nakama3942/mighty_logger/blob/master/CONTRIBUTING.md) and [here](https://github.com/Nakama3942/mighty_logger/blob/master/CODE_OF_CONDUCT.md).
 
 - [Content](#content)
```

### Comparing `mighty_logger-0.9.2/mighty_logger/__init__.py` & `mighty_logger-0.9.3/mighty_logger/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
 A root package that provides access to a implementation of the powerful logger.
-
-.. versionadded:: 0.0.0
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -14,12 +12,13 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from .mighty_logger import MightyLogger
 from .simple_logger import Logger
 
 __authot__ = "Kalynovsky 'Nakamura Akira' Valentin"
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 __email__ = "nakama3942@gmail.com"
```

### Comparing `mighty_logger-0.9.2/mighty_logger/basic/__init__.py` & `mighty_logger-0.9.3/mighty_logger/basic/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
 A package with base classes intended for use within a library.
-
-.. versionadded:: 0.0.0
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -19,7 +17,8 @@
 """
 
 from .exceptions import ColorException,\
 	ReCreationException,\
 	EnvironmentException,\
 	InitException,\
 	MessageException
+from .text_buffer import BasicTextBuffer, TextBuffer
```

### Comparing `mighty_logger-0.9.2/mighty_logger/basic/basic_logger.py` & `mighty_logger-0.9.3/mighty_logger/basic/basic_logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,49 +19,32 @@
 from os import getlogin
 from datetime import datetime
 
 from mighty_logger.basic.lib_types.entry_type import EntryType
 from mighty_logger.basic.lib_types.environment_type import EnvironmentType
 from mighty_logger.basic.exceptions import MessageException
 from mighty_logger.basic.singleton import Singleton
-from mighty_logger.src.lib_types_collection.environments import LogEnvironments
+from mighty_logger.src.environments import LogEnvironments
 from mighty_logger.src.ansi_format import GetAnsiFormat
 
 class BasicLogger(Singleton):
-	"""
-	The base class of the Logger, which stores the main attributes and implements
-	the most important functionality - the formation of the Logger entry string.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	def __init__(
 		self,
 		program_name: str,
 		env: EnvironmentType
 	) -> None:
 		self._ID: int = randint(1000000, 9999999)
 		self._program_name: str = program_name
 		self._environment: EnvironmentType = env
 		self._settings: dict = {}
 
 	def _initialized_data(
 		self,
-		colors: list[str, str],
+		colors: list[str, str]
 	) -> str:
-		"""
-		A method that assemble an entry of system initialized data.
-
-		.. versionadded:: 0.0.0
-
-		:param colors: Color string list of initialized data
-		:type colors: list[str, str]
-		:return: A string with initialized data
-		:rtype: str
-		"""
 		match self._environment.environment_name:
 			case LogEnvironments.CONSOLE.environment_name:
 				return (
 					f"{colors[1]}" +
 					f"{colors[0]}-{self._program_name}?entry> " +
 					f"${platform.node()}:{getlogin()}" +
 					f":{platform.system()}" +
@@ -116,33 +99,14 @@
 		self,
 		entry_type: EntryType,
 		icon_set: int,
 		animation: str,
 		message_text: str,
 		local_settings: dict
 	) -> str:
-		"""
-		A method that assemble an entry into a string and returns it.
-
-		.. versionadded:: 0.0.0
-
-		:param entry_type: Type of entry to be generated
-		:type entry_type: EntryType
-		:param icon_set: Icon set number
-		:type icon_set: int
-		:param animation: Animation frame of entry
-		:type animation: str
-		:param message_text: Message of entry
-		:type message_text: str
-		:param local_settings: Settings for the string of the current entry
-		:type local_settings: dict
-		:return: The formed entry string
-		:rtype: str
-		:raises MessageException: Message is too short (less than 10 characters)
-		"""
 		if len(message_text) < 10:
 			raise MessageException("Message is too short (less than 10 characters)")
 
 		bold = local_settings['bold'] if 'bold' in local_settings else self._settings['global_bold_font']
 		italic = local_settings['italic'] if 'italic' in local_settings else self._settings['global_italic_font']
 		invert = local_settings['invert'] if 'invert' in local_settings else self._settings['global_invert_font']
 		background = local_settings['background'] if 'background' in local_settings else self._settings['global_background']
@@ -200,11 +164,11 @@
 					(f"</b>" if bold else "")
 				)
 			case LogEnvironments.PLAIN.environment_name:
 				return (
 					f"-?entry> {animation} " +
 					f"*{datetime.now()} " +
 					f"{entry_type.icon[icon_set]} " +
-					f"#STATUS: " if status_entry else "" +
+					f"#STATUS: " +
 					f"{entry_type.type_category}{entry_type.type_name} - " +
 					f"{message_text}"
 				)
```

### Comparing `mighty_logger-0.9.2/mighty_logger/basic/exporter.py` & `mighty_logger-0.9.3/mighty_logger/basic/exporter.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,46 +13,31 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from re import sub
 
 from mighty_logger.basic.lib_types.environment_type import EnvironmentType
-from mighty_logger.src.lib_types_collection.environments import LogEnvironments
+from mighty_logger.src.environments import LogEnvironments
 
 class Exporter:
-	"""
-	A class that implements the functionality of exporting a string
-	in the format of Logger entries to other formats.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	def __init__(
 			self,
 			entries: list[str],
 			environment: EnvironmentType
 	) -> None:
 		self.__entries: list[str] = entries
 		self.__env: EnvironmentType = environment
 		self.__csv: list[dict] = []
 
 	@property
 	def entries(self) -> list[str]:
 		return self.__entries
 
 	def export_to_csv(self) -> None:
-		"""
-		The method that implements the export of Logger entries rows to the csv table format.
-		The strings are converted into dictionaries, from which it will then be possible
-		to assemble a csv table at the time the file is saved in the new format.
-		This method does not implement saving the exported data.
-
-		.. versionadded:: 0.0.0
-		"""
 		cleared_entry = ""
 		csv_entry = {}
 
 		for entry in self.__entries[1:]:
 			match self.__env.environment_name:
 				case LogEnvironments.CONSOLE.environment_name:
 					cleared_entry = sub(r"\033\[.*?m", "", entry)
@@ -79,22 +64,14 @@
 				csv_entry["Message"] = " ".join(entry_data[6:])
 
 				self.__csv.append(csv_entry.copy())
 				csv_entry.clear()
 				continue
 
 	def save_to_csv(self, file_name: str) -> None:
-		"""
-		Implements the saving of the generated dictionary strings to the csv file of the table.
-
-		.. versionadded:: 0.0.0
-
-		:param file_name: The name of the file where you want to save the csv table
-		:type file_name: str
-		"""
 		with open(f"{file_name}.csv", "w", encoding="utf-8") as csv:
 			# Write headers (first line) to file
 			headers = self.__csv[0].keys()
 			csv.write(",".join(headers) + "\n")
 
 			# Write data to file
 			for row in self.__csv:
```

### Comparing `mighty_logger-0.9.2/mighty_logger/basic/lib_types/__init__.py` & `mighty_logger-0.9.3/mighty_logger/basic/lib_types/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
 A package that contains the data types that are used in the library.
-
-.. versionadded:: 0.0.0
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `mighty_logger-0.9.2/mighty_logger/basic/lib_types/animation_type.py` & `mighty_logger-0.9.3/mighty_logger/basic/lib_types/animation_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,35 +11,19 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 class BasicAnimationType:
-	"""
-	Basic wrapper class for animations type.
-
-	.. versionadded:: 0.0.0
-	"""
-
-	def __init__(self, animation: list):
+	def __init__(self, animation: list) -> None:
 		self.__animation: list = animation
 
 	@property
 	def animation(self) -> list:
 		return self.__animation
 
 class IndefiniteAnimationType(BasicAnimationType):
-	"""
-	Wrapper class for indefinite animations type.
-
-	.. versionadded:: 0.0.0
-	"""
 	...
 
 class DefiniteAnimationType(BasicAnimationType):
-	"""
-	Wrapper class for definite animations type.
-
-	.. versionadded:: 0.0.0
-	"""
 	...
```

### Comparing `mighty_logger-0.9.2/mighty_logger/basic/lib_types/entry_type.py` & `mighty_logger-0.9.3/mighty_logger/basic/lib_types/entry_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,38 +11,30 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 class EntryType:
-	"""
-	The data type that characterizes the entry type.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	def __init__(
 		self,
 		*,
 		type_category: str,
 		type_name: str,
 		time_color: tuple,
 		status_color: tuple,
-		status_message_color: tuple,
 		type_color: tuple,
 		message_color: tuple,
 		background_color: tuple,
 		icon: tuple
 	) -> None:
 		self.__type_category: str = type_category
 		self.__type_name: str = type_name
 		self.__time_color: tuple = time_color
 		self.__status_color: tuple = status_color
-		self.__status_message_color: tuple = status_message_color
 		self.__type_color: tuple = type_color
 		self.__message_color: tuple = message_color
 		self.__background_color: tuple = background_color
 		self.__icon: tuple = icon
 
 	@property
 	def type_category(self) -> str:
@@ -57,18 +49,14 @@
 		return self.__time_color
 
 	@property
 	def status_color(self) -> tuple:
 		return self.__status_color
 
 	@property
-	def status_message_color(self) -> tuple:
-		return self.__status_message_color
-
-	@property
 	def type_color(self) -> tuple:
 		return self.__type_color
 
 	@property
 	def message_color(self) -> tuple:
 		return self.__message_color
```

### Comparing `mighty_logger-0.9.2/mighty_logger/basic/lib_types/environment_type.py` & `mighty_logger-0.9.3/mighty_logger/basic/lib_types/environment_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,14 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 class EnvironmentType:
-	"""
-	A data type that characterizes the environments in which the Logger can operate.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	def __init__(
 		self,
 		environment_name: str,
 		environment_code: int,
 		updatable: bool,
 		weak_environment: bool
 	) -> None:
```

### Comparing `mighty_logger-0.9.2/mighty_logger/basic/lib_types/sorting_key_type.py` & `mighty_logger-0.9.3/mighty_logger/basic/lib_types/sorting_key_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,19 +11,13 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 class SortingKeyType:
-	"""
-	A data type that characterizes the sort keys for entries.
-
-	.. versionadded:: 0.0.0
-	"""
-
-	def __init__(self, sorting_key: str):
+	def __init__(self, sorting_key: str) -> None:
 		self.__sorting_key: str = sorting_key
 
 	@property
 	def sorting_key(self) -> str:
 		return self.__sorting_key
```

### Comparing `mighty_logger-0.9.2/mighty_logger/basic/singleton.py` & `mighty_logger-0.9.3/mighty_logger/basic/singleton.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,13 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 class Singleton:
-	"""
-	A class that implements the Singleton pattern.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	_instance = None
 
 	def __new__(cls, *args, **kwargs):
 		if cls._instance is None:
 			cls._instance = super().__new__(cls)
 		return cls._instance
```

### Comparing `mighty_logger-0.9.2/mighty_logger/basic/text_buffer.py` & `mighty_logger-0.9.3/mighty_logger/basic/text_buffer.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,27 +17,26 @@
 from re import sub
 from sys import stdout
 
 from mighty_logger.basic.lib_types.environment_type import EnvironmentType
 from mighty_logger.basic.lib_types.text_buffer_type import TextBufferType
 from mighty_logger.basic.exceptions import ReCreationException, EnvironmentException
 from mighty_logger.basic.singleton import Singleton
-from mighty_logger.src.lib_types_collection.environments import LogEnvironments
+from mighty_logger.src.environments import LogEnvironments
 
 class BasicTextBuffer(Singleton, TextBufferType):
-	"""
-	A class with a basic implementation of a simple Text Buffer. It is intended
-	to be used in conjunction with HTML, but this is optional.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	def __init__(self, env: EnvironmentType) -> None:
 		if not hasattr(self, "_text_buffer"):
-			super().__init__(env)
+			if env.environment_name in [
+				LogEnvironments.CONSOLE.environment_name,
+				LogEnvironments.PLAIN_CONSOLE.environment_name
+			]:
+				raise EnvironmentException("This environment is not supported")
+			else:
+				super().__init__(env)
 		else:
 			raise ReCreationException("BasicTextBuffer class object already created")
 
 	def append(self, message: str) -> None:
 		self._text_buffer.append(f"{message}")
 
 	def insert(self, number_string: int, message: str) -> None:
@@ -62,18 +61,14 @@
 		self._text_buffer.pop(number_string)
 
 	def clear(self) -> None:
 		self._text_buffer.clear()
 
 	def save(self, name_file: str, clean: bool) -> None:
 		match self._environment.environment_name:
-			case LogEnvironments.CONSOLE.environment_name:
-				raise EnvironmentException("This environment is not supported")
-			case LogEnvironments.PLAIN_CONSOLE.environment_name:
-				raise EnvironmentException("This environment is not supported")
 			case LogEnvironments.HTML.environment_name:
 				with open(f"{name_file}.html", "w", encoding="utf-8") as text_buffer_file:
 					if clean:
 						text_buffer_file.write('<pre>' + self._text_buffer[0] + '\n'.join([entry for entry in self._text_buffer[1:] if sub(r"<.*?>", "", entry).startswith("-")]) + '</body></pre>')
 					else:
 						text_buffer_file.write('<pre>' + self._text_buffer[0] + '\n'.join(self._text_buffer[1:]) + '</body></pre>')
 			case LogEnvironments.MARKDOWN.environment_name:
@@ -87,18 +82,14 @@
 					if clean:
 						text_buffer_file.write('\n'.join([entry for entry in self._text_buffer if entry.startswith("-")]))
 					else:
 						text_buffer_file.write('\n'.join(self._text_buffer))
 
 	def load(self, name_file: str) -> None:
 		match self._environment.environment_name:
-			case LogEnvironments.CONSOLE.environment_name:
-				raise EnvironmentException("This environment is not supported")
-			case LogEnvironments.PLAIN_CONSOLE.environment_name:
-				raise EnvironmentException("This environment is not supported")
 			case LogEnvironments.HTML.environment_name:
 				with open(f"{name_file}.html", "r", encoding="utf-8") as text_buffer_file:
 					self.clear()
 					self._text_buffer = text_buffer_file.read()\
 						.replace("<pre>", "")\
 						.replace("</body></pre>", "")\
 						.replace("><", ">\n<", 1)\
@@ -122,29 +113,27 @@
 	def update_console(self) -> None:
 		super().update_console()
 
 	def update_entry(self) -> None:
 		super().update_console()
 
 class TextBuffer(Singleton, TextBufferType):
-	"""
-	A class with an advanced implementation of the console Text Buffer. It is not necessary to use it
-	only in the console, but almost all methods are reimplemented for more complex algorithms, taking
-	into account the width of the console (number of characters per line) and use ANSI escape codes
-	that are only found in the console.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	def __init__(self, env: EnvironmentType, console_width: int = 60) -> None:
 		if not hasattr(self, "_text_buffer"):
-			super().__init__(env)
-			self._cursor_string: int = 0
-			self._buffer_size: int = 0
-			self.width = console_width
+			if env.environment_name in [
+				LogEnvironments.HTML.environment_name,
+				LogEnvironments.MARKDOWN.environment_name,
+				LogEnvironments.PLAIN.environment_name
+			]:
+				raise EnvironmentException("This environment is not supported")
+			else:
+				super().__init__(env)
+				self._cursor_string: int = 0
+				self._buffer_size: int = 0
+				self.width = console_width
 		else:
 			raise ReCreationException("TextBuffer class object already created")
 
 	def append(self, message: str) -> None:
 		excess_console_string = len(sub(r"\033\[.*?m", "", message)) // self.width
 		self._buffer_size += 1 + excess_console_string
 		self._text_buffer.append(f"{message}")
@@ -203,20 +192,14 @@
 						text_buffer_file.write('\n'.join(self._text_buffer))
 			case LogEnvironments.PLAIN_CONSOLE.environment_name:
 				with open(f"{name_file}.txt", "w", encoding="utf-8") as text_buffer_file:
 					if clean:
 						text_buffer_file.write('\n'.join([entry for entry in self._text_buffer if entry.startswith("-")]))
 					else:
 						text_buffer_file.write('\n'.join(self._text_buffer))
-			case LogEnvironments.HTML.environment_name:
-				raise EnvironmentException("This environment is not supported")
-			case LogEnvironments.MARKDOWN.environment_name:
-				raise EnvironmentException("This environment is not supported")
-			case LogEnvironments.PLAIN.environment_name:
-				raise EnvironmentException("This environment is not supported")
 
 	def load(self, name_file: str) -> None:
 		match self._environment.environment_name:
 			case LogEnvironments.CONSOLE.environment_name:
 				with open(f"{name_file}.contxt", "r", encoding="utf-8") as text_buffer_file:
 					self.clear()
 					data = text_buffer_file.read().split("\n")
@@ -224,20 +207,14 @@
 						self.append(entry)
 			case LogEnvironments.PLAIN_CONSOLE.environment_name:
 				with open(f"{name_file}.txt", "r", encoding="utf-8") as text_buffer_file:
 					self.clear()
 					data = text_buffer_file.read().split("\n")
 					for entry in data:
 						self.append(entry)
-			case LogEnvironments.HTML.environment_name:
-				raise EnvironmentException("This environment is not supported")
-			case LogEnvironments.MARKDOWN.environment_name:
-				raise EnvironmentException("This environment is not supported")
-			case LogEnvironments.PLAIN.environment_name:
-				raise EnvironmentException("This environment is not supported")
 
 	def input(self, input_text: str) -> str:
 		data = input(f"\r{input_text}")
 		stdout.write(f'\033[1A')
 		stdout.flush()
 		return data
```

### Comparing `mighty_logger-0.9.2/mighty_logger/simple_logger.py` & `mighty_logger-0.9.3/mighty_logger/simple_logger.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,240 +11,164 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from mighty_logger.basic.lib_types.environment_type import EnvironmentType
+from mighty_logger.basic.exceptions import ReCreationException
 from mighty_logger.basic.singleton import Singleton
-from mighty_logger.src.lib_types_collection.entry_types import LoggerEntryTypes, ServiceProcessEntryTypes
-from mighty_logger.src.lib_types_collection.environments import LogEnvironments
+from mighty_logger.src.entry_types import LoggerEntryTypes, ServiceProcessEntryTypes
+from mighty_logger.src.environments import LogEnvironments
 from mighty_logger.mighty_logger import MightyLogger
 
 class Logger(Singleton):
 	"""
 	Lightweight Logger automates work with entry types.
-
-	.. versionadded:: 0.0.0
 	"""
 
 	def __init__(
 		self,
+		*,
 		program_name: str = "Unknown",
 		log_environment: EnvironmentType = LogEnvironments.PLAIN,
 		console_width: int = 60,
 		icon_set: int = 1,
 		global_bold_font: bool = False,
 		global_italic_font: bool = False,
 		global_invert_font: bool = False,
 		global_background: bool = False
 	) -> None:
-		if MightyLogger._instance is not None:
-			self.__logger = MightyLogger._instance
-			self.notice("An existing logger was taken into use")
+
+		if not hasattr(self, "_Logger__logger"):
+			if MightyLogger._instance is not None:
+				self.__logger = MightyLogger._instance
+				self.notice("An existing logger was taken into use")
+			else:
+				self.__logger = MightyLogger(
+					program_name=program_name,
+					log_environment=log_environment,
+					console_width=console_width,
+					icon_set=icon_set,
+					global_bold_font=global_bold_font,
+					global_italic_font=global_italic_font,
+					global_invert_font=global_invert_font,
+					global_background=global_background
+				)
 		else:
-			self.__logger = MightyLogger(
-				program_name=program_name,
-				log_environment=log_environment,
-				console_width=console_width,
-				icon_set=icon_set,
-				global_bold_font=global_bold_font,
-				global_italic_font=global_italic_font,
-				global_invert_font=global_invert_font,
-				global_background=global_background
-			)
+			raise ReCreationException("Logger class object already created")
 
+	@property
 	def might(self) -> MightyLogger:
-		"""
-		Provides access to "mighty" Logger methods.
-
-		.. versionadded:: 0.0.0
-
-		:return: A "mighty" Logger
-		:rtype: MightyLogger
-		"""
 		return self.__logger
 
 	def debug(self, message_text: str) -> None:
 		"""
 		Debugging information logging:
 		Can be used to log entry any information while debugging an application.
 
-		.. versionadded:: 0.0.0
-
 		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.debug, message_text)
 
 	def debug_performance(self, message_text: str) -> None:
 		"""
 		Performance debugging information logging:
 		Can be used to log entry the execution time of operations or other
 		performance information while the application is being debugged.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.debug_performance, message_text)
 
 	def performance(self, message_text: str) -> None:
 		"""
 		Performance information logging:
 		Can be used to log entry the execution time of operations or
 		other application performance information.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.performance, message_text)
 
 	def event(self, message_text: str) -> None:
 		"""
 		Event information logging:
 		Can be used to log entry specific events in the application,
 		such as button presses or mouse cursor movements.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.event, message_text)
 
 	def audit(self, message_text: str) -> None:
 		"""
 		Audit information logging:
 		Can be used to log entry changes in the system, such as creating or
 		deleting users, as well as changes in security settings.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.audit, message_text)
 
 	def metrics(self, message_text: str) -> None:
 		"""
 		Metrics information logging:
 		Can be used to log entry metrics to track application performance and identify issues.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.metrics, message_text)
 
 	def user(self, message_text: str) -> None:
 		"""
 		User information logging:
 		Can be used to log entry custom logs to store additional information
 		that may be useful for diagnosing problems.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.user, message_text)
 
 	def message(self, message_text: str) -> None:
 		"""
 		Message information logging:
 		Can be used for the usual output of ordinary messages about the program's operation.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.message, message_text)
 
 	def info(self, message_text: str) -> None:
 		"""
 		Default information logging:
 		Can be used to log entry messages with specific content about the operation of the program.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.info, message_text)
 
 	def notice(self, message_text: str) -> None:
 		"""
 		Notice information logging:
 		Can be used to flag important events that might be missed with a normal logging level.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.notice, message_text)
 
 	def warning(self, message_text: str) -> None:
 		"""
 		Warning information logging:
 		Can be used to log entry warnings that the program may work with unpredictable results.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.warning, message_text)
 
 	def error(self, message_text: str) -> None:
 		"""
 		Error information logging:
 		Used to log entry errors and crashes in the program.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.error, message_text)
 
 	def critical(self, message_text: str) -> None:
 		"""
 		Critical error information logging:
 		Used to log entry for critical and unpredictable program failures.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(LoggerEntryTypes.critical, message_text)
 
 	def success(self, message_text: str) -> None:
 		"""
 		Success information logging:
 		Used to log entry a message about the success of the process.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(ServiceProcessEntryTypes.success, message_text)
 
 	def fail(self, message_text: str) -> None:
 		"""
 		Fail information logging:
 		Used to log entry a message about the failed execution of the process.
-
-		.. versionadded:: 0.0.0
-
-		:param message_text: Log entry message
-		:type message_text: str
 		"""
 		self.__logger.entry(ServiceProcessEntryTypes.fail, message_text)
```

### Comparing `mighty_logger-0.9.2/mighty_logger/src/__init__.py` & `mighty_logger-0.9.3/mighty_logger/src/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
 A package with the implementation of various data (ANSI, colors, etc.).
-
-.. versionadded:: 0.0.0
 \n
 Copyright © 2023 Kalynovsky Valentin. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -25,7 +23,10 @@
 	AnsiColor,\
 	Dec2Hex,\
 	Dec2Ansi,\
 	Hex2Dec,\
 	Hex2Ansi,\
 	Ansi2Dec,\
 	Ansi2Hex
+from .entry_types import LoggerEntryTypes, ProcessEntryTypes, SelectionTypes, SelectionCategories
+from .environments import LogEnvironments
+from .sorting_keys import SortingKeys
```

### Comparing `mighty_logger-0.9.2/mighty_logger/src/animations.py` & `mighty_logger-0.9.3/mighty_logger/src/animations.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,19 +16,14 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from mighty_logger.basic.lib_types.animation_type import IndefiniteAnimationType, DefiniteAnimationType
 
 class IndefiniteAnimations:
-	"""
-	The class with sets indefinite animations.
-
-	.. versionadded:: 0.0.0
-	"""
 	Dots = IndefiniteAnimationType([
 		'.       ',
 		'..      ',
 		'...     ',
 		'....    ',
 		'.....   ',
 		'......  ',
@@ -432,19 +427,14 @@
 		'........',
 		'........',
 		'........',
 		'........'
 	])
 
 class DefiniteAnimations:
-	"""
-	The class with sets definite animations.
-
-	.. versionadded:: 0.0.0
-	"""
 	Dots = DefiniteAnimationType([
 		'        ',
 		'.       ',
 		'..      ',
 		'...     ',
 		'....    ',
 		'.....   ',
```

### Comparing `mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/entry_types.py` & `mighty_logger-0.9.3/mighty_logger/src/entry_types.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,20 +14,14 @@
 limitations under the License.
 """
 
 from mighty_logger.basic.lib_types.entry_type import EntryType
 from mighty_logger.src.color_picker import AnsiColor, HexColor
 
 class ServiceLogger:
-	"""
-	Class for Logger service strings.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	initial = (
 		(
 			(AnsiColor('GOLD', "foreground"), AnsiColor('INDIGO', "foreground")),
 			("", ""),
 			(HexColor('GOLD'), HexColor('INDIGO')),
 			(HexColor('GOLD'), HexColor('INDIGO')),
 			("", "")
@@ -35,27 +29,16 @@
 			("", AnsiColor('GOLD', "background")),
 			("", ""),
 			("", HexColor('GOLD')),
 			("", HexColor('GOLD')),
 			("", "")
 		)
 	)
-	"""
-	Colors for the starting initialization string.
-	
-	.. versionadded:: 0.0.0
-	"""
 
 class LoggerEntryTypes:
-	"""
-	A class with standard entry types. Is available.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	debug = EntryType(
 		type_category="%",
 		type_name="DEBUG",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
@@ -65,21 +48,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('BURLYWOOD', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('BURLYWOOD'), HexColor('NAVY')),
 			(HexColor('BURLYWOOD'), HexColor('NAVY')),
 			("", "")
 		),
@@ -95,20 +71,14 @@
 			("", ""),
 			("", HexColor('TAN')),
 			("", HexColor('TAN')),
 			("", "")
 		),
 		icon=('🐛', '🐞', '🚧', '🔬')
 	)
-	"""
-	Debugging information logging:
-	Can be used to log entry any information while debugging an application.
-	
-	.. versionadded:: 0.0.0
-	"""
 	debug_performance = EntryType(
 		type_category="%",
 		type_name="DEBUG-PERFORMANCE",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
@@ -118,21 +88,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('NAVAJOWHITE', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('NAVAJOWHITE'), HexColor('NAVY')),
 			(HexColor('NAVAJOWHITE'), HexColor('NAVY')),
 			("", "")
 		),
@@ -148,21 +111,14 @@
 			("", ""),
 			("", HexColor('WHEAT')),
 			("", HexColor('WHEAT')),
 			("", "")
 		),
 		icon=('⏱️', '⌛️', '🔍', '📈')
 	)
-	"""
-	Performance debugging information logging:
-	Can be used to log entry the execution time of operations or other
-	performance information while the application is being debugged.
-	
-	.. versionadded:: 0.0.0
-	"""
 	performance = EntryType(
 		type_category="%",
 		type_name="PERFORMANCE",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
@@ -172,21 +128,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('BLANCHEDALMOND', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('BLANCHEDALMOND'), HexColor('NAVY')),
 			(HexColor('BLANCHEDALMOND'), HexColor('NAVY')),
 			("", "")
 		),
@@ -202,21 +151,14 @@
 			("", ""),
 			("", HexColor('BISQUE')),
 			("", HexColor('BISQUE')),
 			("", "")
 		),
 		icon=('⏱️', '🚀', '📊', '⚡️')
 	)
-	"""
-	Performance information logging:
-	Can be used to log entry the execution time of operations or
-	other application performance information.
-	
-	.. versionadded:: 0.0.0
-	"""
 	event = EntryType(
 		type_category="~",
 		type_name="EVENT",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
@@ -226,21 +168,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('GREENYELLOW', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('GREENYELLOW'), HexColor('NAVY')),
 			(HexColor('GREENYELLOW'), HexColor('NAVY')),
 			("", "")
 		),
@@ -256,21 +191,14 @@
 			("", ""),
 			("", HexColor('YELLOWGREEN')),
 			("", HexColor('YELLOWGREEN')),
 			("", "")
 		),
 		icon=('🔔', '🎉', '📣', '🚨')
 	)
-	"""
-	Event information logging:
-	Can be used to log entry specific events in the application,
-	such as button presses or mouse cursor movements.
-	
-	.. versionadded:: 0.0.0
-	"""
 	audit = EntryType(
 		type_category="~",
 		type_name="AUDIT",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
@@ -280,21 +208,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('MEDIUMSPRINGGREEN', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('MEDIUMSPRINGGREEN'), HexColor('NAVY')),
 			(HexColor('MEDIUMSPRINGGREEN'), HexColor('NAVY')),
 			("", "")
 		),
@@ -310,21 +231,14 @@
 			("", ""),
 			("", HexColor('SPRINGGREEN')),
 			("", HexColor('SPRINGGREEN')),
 			("", "")
 		),
 		icon=('🔍', '🔒', '📋', '🔐')
 	)
-	"""
-	Audit information logging:
-	Can be used to log entry changes in the system, such as creating or
-	deleting users, as well as changes in security settings.
-	
-	.. versionadded:: 0.0.0
-	"""
 	metrics = EntryType(
 		type_category="~",
 		type_name="METRICS",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
@@ -334,21 +248,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('PALEGREEN', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('PALEGREEN'), HexColor('NAVY')),
 			(HexColor('PALEGREEN'), HexColor('NAVY')),
 			("", "")
 		),
@@ -364,20 +271,14 @@
 			("", ""),
 			("", HexColor('LIGHTGREEN')),
 			("", HexColor('LIGHTGREEN')),
 			("", "")
 		),
 		icon=('📊', '📈', '📉', '📄')
 	)
-	"""
-	Metrics information logging:
-	Can be used to log entry metrics to track application performance and identify issues.
-	
-	.. versionadded:: 0.0.0
-	"""
 	user = EntryType(
 		type_category="~",
 		type_name="USER",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
@@ -387,21 +288,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('CHARTREUSE', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('CHARTREUSE'), HexColor('NAVY')),
 			(HexColor('CHARTREUSE'), HexColor('NAVY')),
 			("", "")
 		),
@@ -417,21 +311,14 @@
 			("", ""),
 			("", HexColor('LAWNGREEN')),
 			("", HexColor('LAWNGREEN')),
 			("", "")
 		),
 		icon=('👤', '👥', '🙋‍♂️', '🙋‍♀️')
 	)
-	"""
-	User information logging:
-	Can be used to log entry custom logs to store additional information
-	that may be useful for diagnosing problems.
-	
-	.. versionadded:: 0.0.0
-	"""
 	message = EntryType(
 		type_category="@",
 		type_name="MESSAGE",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
@@ -441,21 +328,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('PALETURQUOISE', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('PALETURQUOISE'), HexColor('NAVY')),
 			(HexColor('PALETURQUOISE'), HexColor('NAVY')),
 			("", "")
 		),
@@ -471,20 +351,14 @@
 			("", ""),
 			("", HexColor('POWDERBLUE')),
 			("", HexColor('POWDERBLUE')),
 			("", "")
 		),
 		icon=('💬', '📝', '🗒️', '📨')
 	)
-	"""
-	Message information logging:
-	Can be used for the usual output of ordinary messages about the program's operation.
-	
-	.. versionadded:: 0.0.0
-	"""
 	info = EntryType(
 		type_category="@",
 		type_name="INFO",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
@@ -494,21 +368,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('LIGHTSKYBLUE', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('LIGHTSKYBLUE'), HexColor('NAVY')),
 			(HexColor('LIGHTSKYBLUE'), HexColor('NAVY')),
 			("", "")
 		),
@@ -524,20 +391,14 @@
 			("", ""),
 			("", HexColor('SKYBLUE')),
 			("", HexColor('SKYBLUE')),
 			("", "")
 		),
 		icon=('ℹ️', '🔍', '📌', '🔔')
 	)
-	"""
-	Default information logging:
-	Can be used to log entry messages with specific content about the operation of the program.
-	
-	.. versionadded:: 0.0.0
-	"""
 	notice = EntryType(
 		type_category="@",
 		type_name="NOTICE",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
@@ -547,21 +408,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('LIGHTBLUE', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('LIGHTBLUE'), HexColor('NAVY')),
 			(HexColor('LIGHTBLUE'), HexColor('NAVY')),
 			("", "")
 		),
@@ -577,20 +431,14 @@
 			("", ""),
 			("", HexColor('LIGHTSTEELBLUE')),
 			("", HexColor('LIGHTSTEELBLUE')),
 			("", "")
 		),
 		icon=('📌', '📎', '🔖', '🚩')
 	)
-	"""
-	Notice information logging:
-	Can be used to flag important events that might be missed with a normal logging level.
-	
-	.. versionadded:: 0.0.0
-	"""
 	warning = EntryType(
 		type_category="!",
 		type_name="WARNING",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
@@ -600,21 +448,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('YELLOW', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('YELLOW'), HexColor('NAVY')),
 			(HexColor('YELLOW'), HexColor('NAVY')),
 			("", "")
 		),
@@ -630,20 +471,14 @@
 			("", ""),
 			("", HexColor('DARKYELLOW')),
 			("", HexColor('DARKYELLOW')),
 			("", "")
 		),
 		icon=('⚠️', '⚡️', '⛔️', '⚠️')
 	)
-	"""
-	Warning information logging:
-	Can be used to log entry warnings that the program may work with unpredictable results.
-	
-	.. versionadded:: 0.0.0
-	"""
 	error = EntryType(
 		type_category="!",
 		type_name="!ERROR",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('PLUM', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('PLUM')),
@@ -653,21 +488,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('ORANGE', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('ORANGE')),
 			(HexColor('ORANGE'), HexColor('ORANGE')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('DARKORANGE', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('DARKORANGE')),
-			(HexColor('DARKORANGE'), HexColor('DARKORANGE')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('FIREBRICK', "foreground"), AnsiColor('GAINSBORO', "foreground")),
 			("", ""),
 			(HexColor('FIREBRICK'), HexColor('GAINSBORO')),
 			(HexColor('FIREBRICK'), HexColor('GAINSBORO')),
 			("", "")
 		),
@@ -683,20 +511,14 @@
 			("", ""),
 			("", HexColor('DARKRED')),
 			("", HexColor('DARKRED')),
 			("", "")
 		),
 		icon=('❌', '🚫', '💔', '🔺')
 	)
-	"""
-	Error information logging:
-	Used to log entry errors and crashes in the program.
-	
-	.. versionadded:: 0.0.0
-	"""
 	critical = EntryType(
 		type_category="!",
 		type_name="!!@CRITICAL",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('PLUM', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('PLUM')),
@@ -706,21 +528,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('ORANGE', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('ORANGE')),
 			(HexColor('ORANGE'), HexColor('ORANGE')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('DARKORANGE', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('DARKORANGE')),
-			(HexColor('DARKORANGE'), HexColor('DARKORANGE')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('FIREBRICK', "foreground"), AnsiColor('DARKSALMON', "foreground")),
 			("", ""),
 			(HexColor('FIREBRICK'), HexColor('DARKSALMON')),
 			(HexColor('FIREBRICK'), HexColor('DARKSALMON')),
 			("", "")
 		),
@@ -736,20 +551,14 @@
 			("", ""),
 			("", HexColor('MAROON')),
 			("", HexColor('MAROON')),
 			("", "")
 		),
 		icon=('🔥', '🚨', '⛔️', '🚒')
 	)
-	"""
-	Critical error information logging:
-	Used to log entry for critical and unpredictable program failures.
-	
-	.. versionadded:: 0.0.0
-	"""
 	resolved = EntryType(
 		type_category="!",
 		type_name="RESOLVED",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('LAVENDERBLUSH', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
@@ -759,21 +568,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('CHARTREUSE', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
 			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('LAWNGREEN', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('LAWNGREEN')),
-			(HexColor('DARKORANGE'), HexColor('LAWNGREEN')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('GREEN', "foreground"), AnsiColor('PALEGREEN', "foreground")),
 			("", ""),
 			(HexColor('GREEN'), HexColor('PALEGREEN')),
 			(HexColor('GREEN'), HexColor('PALEGREEN')),
 			("", "")
 		),
@@ -789,20 +591,14 @@
 			("", ""),
 			("", HexColor('DARKGREEN')),
 			("", HexColor('DARKGREEN')),
 			("", "")
 		),
 		icon=('✅', '❗', '🟦', '🟢')
 	)
-	"""
-	Resolved information logging:
-	Used to log entry resolved solutions to problems and errors.
-	
-	.. versionadded:: 0.6.0
-	"""
 	unresolved = EntryType(
 		type_category="!",
 		type_name="UNRESOLVED",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('LAVENDERBLUSH', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
@@ -812,21 +608,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('ORANGE', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('ORANGE')),
 			(HexColor('ORANGE'), HexColor('ORANGE')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('DARKORANGE', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('DARKORANGE')),
-			(HexColor('DARKORANGE'), HexColor('DARKORANGE')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('FIREBRICK', "foreground"), AnsiColor('YELLOW', "foreground")),
 			("", ""),
 			(HexColor('FIREBRICK'), HexColor('YELLOW')),
 			(HexColor('FIREBRICK'), HexColor('YELLOW')),
 			("", "")
 		),
@@ -842,28 +631,16 @@
 			("", ""),
 			("", HexColor('DARKRED')),
 			("", HexColor('DARKRED')),
 			("", "")
 		),
 		icon=('❎', '❓', '🟥', '🔴')
 	)
-	"""
-	Unresolved information logging:
-	Used to log entry unresolved solutions to problems and errors.
-	
-	.. versionadded:: 0.6.0
-	"""
 
 class ProcessEntryTypes:
-	"""
-	Class with additional entry types when logging Processes. Is available.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	achievement = EntryType(
 		type_category="&",
 		type_name="ACHIEVEMENT",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
@@ -873,21 +650,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('YELLOW', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('YELLOW'), HexColor('NAVY')),
 			(HexColor('YELLOW'), HexColor('NAVY')),
 			("", "")
 		),
@@ -903,20 +673,14 @@
 			("", ""),
 			("", HexColor('DARKYELLOW')),
 			("", HexColor('DARKYELLOW')),
 			("", "")
 		),
 		icon=('🏆', '🏆', '🌟', '🎖️')
 	)
-	"""
-	Achievement information logging:
-	Used to log entry the achievements gained while executing a process.
-	
-	.. versionadded:: 0.0.0
-	"""
 	milestone = EntryType(
 		type_category="&",
 		type_name="MILESTONE",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('LAVENDERBLUSH', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
@@ -926,21 +690,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('CHARTREUSE', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
 			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('LAWNGREEN', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('LAWNGREEN')),
-			(HexColor('DARKORANGE'), HexColor('LAWNGREEN')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('GREEN', "foreground"), AnsiColor('PALEGREEN', "foreground")),
 			("", ""),
 			(HexColor('GREEN'), HexColor('PALEGREEN')),
 			(HexColor('GREEN'), HexColor('PALEGREEN')),
 			("", "")
 		),
@@ -956,28 +713,16 @@
 			("", ""),
 			("", HexColor('DARKGREEN')),
 			("", HexColor('DARKGREEN')),
 			("", "")
 		),
 		icon=('🔖', '🔖', '🎯', '🗺️')
 	)
-	"""
-	Milestone information logging:
-	Used to log entry the milestones gained while executing a process.
-	
-	.. versionadded:: 0.0.0
-	"""
 
 class ServiceProcessEntryTypes:
-	"""
-	A class with utility types used for Process logging. Is not available.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	initiation = EntryType(
 		type_category="&",
 		type_name="INITIATION",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('LAVENDERBLUSH', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
@@ -987,21 +732,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('CHARTREUSE', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
 			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('LAWNGREEN', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('LAWNGREEN')),
-			(HexColor('DARKORANGE'), HexColor('LAWNGREEN')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('GREEN', "foreground"), AnsiColor('PALEGREEN', "foreground")),
 			("", ""),
 			(HexColor('GREEN'), HexColor('PALEGREEN')),
 			(HexColor('GREEN'), HexColor('PALEGREEN')),
 			("", "")
 		),
@@ -1017,20 +755,14 @@
 			("", ""),
 			("", HexColor('DARKGREEN')),
 			("", HexColor('DARKGREEN')),
 			("", "")
 		),
 		icon=('🚀', '🚀', '🔥', '🔧')
 	)
-	"""
-	Initiation information logging:
-	Used to explain the running process.
-	
-	.. versionadded:: 0.0.0
-	"""
 	process = EntryType(
 		type_category="&",
 		type_name="PROGRESS",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('PURPLE', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('PURPLE')),
@@ -1040,21 +772,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('LIGHTSKYBLUE', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('LIGHTSKYBLUE'), HexColor('NAVY')),
 			(HexColor('LIGHTSKYBLUE'), HexColor('NAVY')),
 			("", "")
 		),
@@ -1070,20 +795,14 @@
 			("", ""),
 			("", HexColor('SKYBLUE')),
 			("", HexColor('SKYBLUE')),
 			("", "")
 		),
 		icon=('⏳', '🔄', '⚙️', '🕰️')
 	)
-	"""
-	Process information logging:
-	Used to refine the progress of a Process.
-	
-	.. versionadded:: 0.0.0
-	"""
 	success = EntryType(
 		type_category="&",
 		type_name="SUCCESS",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('LAVENDERBLUSH', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
@@ -1093,21 +812,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('CHARTREUSE', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
 			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('LAWNGREEN', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('LAWNGREEN')),
-			(HexColor('DARKORANGE'), HexColor('LAWNGREEN')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('GREEN', "foreground"), AnsiColor('PALEGREEN', "foreground")),
 			("", ""),
 			(HexColor('GREEN'), HexColor('PALEGREEN')),
 			(HexColor('GREEN'), HexColor('PALEGREEN')),
 			("", "")
 		),
@@ -1123,20 +835,14 @@
 			("", ""),
 			("", HexColor('DARKGREEN')),
 			("", HexColor('DARKGREEN')),
 			("", "")
 		),
 		icon=('✔️', '🎉', '👍', '✅')
 	)
-	"""
-	Success information logging:
-	Used to log entry a message about the success of the process.
-	
-	.. versionadded:: 0.0.0
-	"""
 	fail = EntryType(
 		type_category="&",
 		type_name="FAIL",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('LAVENDERBLUSH', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
@@ -1146,21 +852,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('ORANGE', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('ORANGE')),
 			(HexColor('ORANGE'), HexColor('ORANGE')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('DARKORANGE', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('DARKORANGE')),
-			(HexColor('DARKORANGE'), HexColor('DARKORANGE')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('FIREBRICK', "foreground"), AnsiColor('YELLOW', "foreground")),
 			("", ""),
 			(HexColor('FIREBRICK'), HexColor('YELLOW')),
 			(HexColor('FIREBRICK'), HexColor('YELLOW')),
 			("", "")
 		),
@@ -1176,28 +875,16 @@
 			("", ""),
 			("", HexColor('DARKRED')),
 			("", HexColor('DARKRED')),
 			("", "")
 		),
 		icon=('❌', '🚫', '👎', '❎')
 	)
-	"""
-	Fail information logging:
-	Used to log entry a message about the failed execution of the process.
-	
-	.. versionadded:: 0.0.0
-	"""
 
 class ServiceTimerEntryTypes:
-	"""
-	A class with utility types used for Timer logging. Is not available.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	start_timer = EntryType(
 		type_category="^",
 		type_name="START-TIMER",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('LAVENDERBLUSH', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('LAVENDERBLUSH')),
@@ -1207,21 +894,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('CHARTREUSE', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
 			(HexColor('ORANGE'), HexColor('CHARTREUSE')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('LAWNGREEN', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('LAWNGREEN')),
-			(HexColor('DARKORANGE'), HexColor('LAWNGREEN')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('SEAGREEN', "foreground"), AnsiColor('PALEGREEN', "foreground")),
 			("", ""),
 			(HexColor('SEAGREEN'), HexColor('PALEGREEN')),
 			(HexColor('SEAGREEN'), HexColor('PALEGREEN')),
 			("", "")
 		),
@@ -1237,20 +917,14 @@
 			("", ""),
 			("", HexColor('FORESTGREEN')),
 			("", HexColor('FORESTGREEN')),
 			("", "")
 		),
 		icon=('⏰', '🕑', '🟩', '⏳')
 	)
-	"""
-	Information logging of starting Timer:
-	Used to notify the start of the Timer.
-	
-	.. versionadded:: 0.0.0
-	"""
 	timer_mark = EntryType(
 		type_category="^",
 		type_name="TIMER-MARK",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('DARKMAGENTA', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('DARKMAGENTA')),
@@ -1260,21 +934,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('KHAKI', "foreground"), AnsiColor('SIENNA', "foreground")),
 			("", ""),
 			(HexColor('KHAKI'), HexColor('SIENNA')),
 			(HexColor('KHAKI'), HexColor('SIENNA')),
 			("", "")
 		),
@@ -1290,20 +957,14 @@
 			("", ""),
 			("", HexColor('DARKKHAKI')),
 			("", HexColor('DARKKHAKI')),
 			("", "")
 		),
 		icon=('⌚', '🕕', '🟨', '⏱️')
 	)
-	"""
-	Information logging of mark Timer:
-	Used to notify the mark of the Timer.
-	
-	.. versionadded:: 0.0.0
-	"""
 	stop_timer = EntryType(
 		type_category="^",
 		type_name="STOP-TIMER",
 		time_color=(
 			(AnsiColor('ORCHID', "foreground"), AnsiColor('PURPLE', "foreground")),
 			("", ""),
 			(HexColor('ORCHID'), HexColor('PURPLE')),
@@ -1313,21 +974,14 @@
 		status_color=(
 			(AnsiColor('ORANGE', "foreground"), AnsiColor('DARKRED', "foreground")),
 			("", ""),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			(HexColor('ORANGE'), HexColor('DARKRED')),
 			("", "")
 		),
-		status_message_color=(
-			(AnsiColor('DARKORANGE', "foreground"), AnsiColor('MAROON', "foreground")),
-			("", ""),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			(HexColor('DARKORANGE'), HexColor('MAROON')),
-			("", "")
-		),
 		type_color=(
 			(AnsiColor('LIGHTSKYBLUE', "foreground"), AnsiColor('NAVY', "foreground")),
 			("", ""),
 			(HexColor('LIGHTSKYBLUE'), HexColor('NAVY')),
 			(HexColor('LIGHTSKYBLUE'), HexColor('NAVY')),
 			("", "")
 		),
@@ -1343,360 +997,311 @@
 			("", ""),
 			("", HexColor('SKYBLUE')),
 			("", HexColor('SKYBLUE')),
 			("", "")
 		),
 		icon=('⏲️', '🕙', '🟪', '⌛')
 	)
-	"""
-	Information logging of stopping Timer:
-	Used to notify the stop of the Timer.
-	
-	.. versionadded:: 0.0.0
-	"""
 
 class SelectionTypes:
-	"""
-	A class with a list of all entry types.
-	Needed only for the select() method of the Modifier class.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	debug = EntryType(
 		type_category="",
 		type_name="DEBUG",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	debug_performance = EntryType(
 		type_category="",
 		type_name="DEBUG-PERFORMANCE",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	performance = EntryType(
 		type_category="",
 		type_name="PERFORMANCE",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	event = EntryType(
 		type_category="",
 		type_name="EVENT",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	audit = EntryType(
 		type_category="",
 		type_name="AUDIT",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	metrics = EntryType(
 		type_category="",
 		type_name="METRICS",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	user = EntryType(
 		type_category="",
 		type_name="USER",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	message = EntryType(
 		type_category="",
 		type_name="MESSAGE",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	info = EntryType(
 		type_category="",
 		type_name="INFO",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	notice = EntryType(
 		type_category="",
 		type_name="NOTICE",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	warning = EntryType(
 		type_category="",
 		type_name="WARNING",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	error = EntryType(
 		type_category="",
 		type_name="!ERROR",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	critical = EntryType(
 		type_category="",
 		type_name="!!@CRITICAL",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	resolved = EntryType(
 		type_category="",
 		type_name="RESOLVED",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	unresolved = EntryType(
 		type_category="",
 		type_name="UNRESOLVED",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	achievement = EntryType(
 		type_category="",
 		type_name="ACHIEVEMENT",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	milestone = EntryType(
 		type_category="",
 		type_name="MILESTONE",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	initiation = EntryType(
 		type_category="",
 		type_name="INITIATION",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	process = EntryType(
 		type_category="",
 		type_name="PROGRESS",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	success = EntryType(
 		type_category="",
 		type_name="SUCCESS",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	fail = EntryType(
 		type_category="",
 		type_name="FAIL",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	start_timer = EntryType(
 		type_category="",
 		type_name="START-TIMER",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	timer_mark = EntryType(
 		type_category="",
 		type_name="TIMER-MARK",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	stop_timer = EntryType(
 		type_category="",
 		type_name="STOP-TIMER",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 
 class SelectionCategories:
-	"""
-	A class with a list of all entry categories.
-	Needed only for the select() method of the Modifier class.
-
-	.. versionadded:: 0.0.0
-	"""
 	debug = EntryType(
 		type_category="%",
 		type_name="",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	event = EntryType(
 		type_category="~",
 		type_name="",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	message = EntryType(
 		type_category="@",
 		type_name="",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	error = EntryType(
 		type_category="!",
 		type_name="",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	process = EntryType(
 		type_category="&",
 		type_name="",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
 	timer = EntryType(
 		type_category="^",
 		type_name="",
 		time_color = (),
 		status_color = (),
-		status_message_color = (),
 		type_color = (),
 		message_color = (),
 		background_color = (),
 		icon = ()
 	)
```

### Comparing `mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/environments.py` & `mighty_logger-0.9.3/mighty_logger/src/environments.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,12 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from mighty_logger.basic.lib_types.environment_type import EnvironmentType
 
 class LogEnvironments:
-	"""
-	Environments of Logger.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	CONSOLE = EnvironmentType("CONSOLE", 0, True, False)
 	PLAIN_CONSOLE = EnvironmentType("PLAIN_CONSOLE", 1, True, False)
 	HTML = EnvironmentType("HTML", 2, False, True)
 	MARKDOWN = EnvironmentType("MARKDOWN", 3, False, True)
 	PLAIN = EnvironmentType("PLAIN", 4, False, False)
```

### Comparing `mighty_logger-0.9.2/mighty_logger/src/lib_types_collection/sorting_keys.py` & `mighty_logger-0.9.3/mighty_logger/src/sorting_keys.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,11 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from mighty_logger.basic.lib_types.sorting_key_type import SortingKeyType
 
 class SortingKeys:
-	"""
-	Sort keys.
-
-	.. versionadded:: 0.0.0
-	"""
-
 	SORT_ON_TIME = SortingKeyType("time")
 	SORT_ON_TIME_WITH_REVERSE = SortingKeyType("time_with_reverse")
 	SORT_ON_CATEGORY = SortingKeyType("category")
 	SORT_ON_TYPE = SortingKeyType("type")
```

### Comparing `mighty_logger-0.9.2/mighty_logger.egg-info/PKG-INFO` & `mighty_logger-0.9.3/mighty_logger.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mighty-logger
-Version: 0.9.2
-Summary: Powerful functional logger
+Version: 0.9.3
+Summary: Mighty functional logger
 Author-email: Kalynovsky 'Nakamura Akira' Valentin <nakama3942@gmail.com>
 License: Apache License Version 2.0
 Project-URL: Repository, https://github.com/Nakama3942/mighty_logger
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,55 +21,47 @@
 [![template](https://img.shields.io/badge/Repository-template-darkred?style=for-the-badge)](https://github.com/Nakama3942/template_rep)
 [![GitHub license](https://img.shields.io/github/license/Nakama3942/mighty_logger?color=gold&style=for-the-badge)](https://github.com/Nakama3942/mighty_logger/blob/master/LICENSE)
 [![CHANGELOG](https://img.shields.io/badge/here-CHANGELOG-yellow?style=for-the-badge)](https://github.com/Nakama3942/mighty_logger/blob/master/CHANGELOG.md)
 [![PULL_REQUEST_TEMPLATE](https://img.shields.io/badge/here-PULL_REQUEST_TEMPLATE-orange?style=for-the-badge)](https://github.com/Nakama3942/mighty_logger/blob/master/.github/PULL_REQUEST_TEMPLATE.md)
 
 ![PyPI](https://img.shields.io/pypi/v/mighty-logger?color=yellow&logo=pypi&logoColor=white&style=for-the-badge)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/Nakama3942/mighty_logger?label=latest%20release&logo=github&style=for-the-badge)
-![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/Nakama3942/mighty_logger?color=orange&include_prereleases&label=latest%20pre-release&logo=github&style=for-the-badge)
 ![GitHub commits since latest release (by date including pre-releases)](https://img.shields.io/github/commits-since/Nakama3942/mighty_logger/v0.5.0?include_prereleases&style=for-the-badge)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mighty-logger?style=for-the-badge)
-![PyPI - Wheel](https://img.shields.io/pypi/wheel/mighty-logger?style=for-the-badge)
 ![PyPI - Format](https://img.shields.io/pypi/format/mighty-logger?label=PyPI%20format&style=for-the-badge)
 ![PyPI - Status](https://img.shields.io/pypi/status/mighty-logger?label=PyPI%20status&style=for-the-badge)
 
 ![GitHub last commit](https://img.shields.io/github/last-commit/Nakama3942/mighty_logger?style=for-the-badge)
 ![GitHub Release Date](https://img.shields.io/github/release-date/Nakama3942/mighty_logger?style=for-the-badge)
-![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/Nakama3942/mighty_logger?label=%28pre-%29release%20date&style=for-the-badge)
 
 ![GitHub repo size](https://img.shields.io/github/repo-size/Nakama3942/mighty_logger?color=darkgreen&style=for-the-badge)
 ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/Nakama3942/mighty_logger?color=darkgreen&style=for-the-badge)
 ![Lines of code](https://img.shields.io/tokei/lines/github/Nakama3942/mighty_logger?style=for-the-badge)
 
 </div>
 
 # Mighty Logger
 
 ### Content
 
-- [Qt_Сolored-logger](#mighty-logger)
-  - [Content](#content)
-  - [Preamble](#preamble)
-  - [Overview](#overview)
-  - [Important releases](#important-releases)
-  - [LICENSE](#license)
-  - [Installation](#installation)
-  - [Usage](#usage)
-  - [Additional functionality](#additional-functionality)
-  - [Data](#data)
-  - [Troubleshooting](#troubleshooting)
-  - [Authors](#authors)
+- [Mighty Logger](#mighty-logger)
+	- [Content](#content)
+	- [Preamble](#preamble)
+	- [Overview](#overview)
+    - [LICENSE](#license)
+	- [Important releases](#important-releases)
+	- [Features](#features)
+	- [Installation](#installation)
+	- [Usage](#usage)
+	- [Troubleshooting](#troubleshooting)
+	- [Authors](#authors)
 
 ## Preamble
 
-<!--
-This library it was renamed to "Mighty logger" but before this library named is "Qt Colored logger". Old commits may search in this repository, but download old build may on next link: https://pypi.org/project/qt-colored-logger/ .
--->
-
 > I often came across the opinion that it is better to use not standard output to the console, but full-fledged logging... However, the standard libraries do not provide exactly what I need... Therefore, I decided to make my own library! Which will implement the functionality I need.
 
 I was inspired by the [colored-logs](https://pypi.org/project/colored-logs/) library.
 
 ---
 
 *This library has been renamed to "Mighty logger", but this library used to be called "Qt Colored logger". You can search for old commits in this repository, but you can download the old build from the [link](https://pypi.org/project/qt-colored-logger/).*
@@ -78,118 +70,125 @@
 
 ## Overview
 
 The library implements the formation of a beautifully formatted colored text, similar to a log, which has all the necessary information:
 
 - Device name and registered profile, system name, etc. (this data is displayed only once at the beginning of the logging)
 - Log entry time
-- Log entry status
+- Log entry category
 - Log entry type
 - Entry message
 
-Any information to the output can be turned off (according to the default, everything is included). It is also possible to change the output settings during the logging process. It is possible to change the colors of the foreground text and the background, icons ~~and animations~~.
+Any information to the output can be turned off (according to the default, everything is included). It is also possible to change the output settings during the logging process. It is possible to change the colors of the foreground text and the background, icons and animations.
+
+- [Content](#content)
+
+## LICENSE
+
+The full text of the license can be found at the following [link](https://github.com/Nakama3942/mighty_logger/blob/master/LICENSE).
+
+> Copyright © 2023 Kalynovsky Valentin. All rights reserved.
+>
+> Licensed under the Apache License, Version 2.0 (the "License");
+> you may not use this file except in compliance with the License.
+> You may obtain a copy of the License at
+>
+>     http://www.apache.org/licenses/LICENSE-2.0
+>
+> Unless required by applicable law or agreed to in writing, software
+> distributed under the License is distributed on an "AS IS" BASIS,
+> WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+> See the License for the specific language governing permissions and
 
 - [Content](#content)
 
 ## Important releases
 
-<details><summary>See the important releases (possible spoilers)</summary>
+<details><summary>See the important releases</summary>
 
 - [x] v0.0.1 - Alpha-release (the very first version of the simplest Logger has been published)
 - [x] v0.0.2 - Little update (added multiple entry types and colors)
 - [x] v0.0.3 - Types update (added even more multiple entry types and colors)
 - [x] v0.0.4 - Color update (added the entire X11 color table and reworked the color system)
-- [x] v0.1.0 - First official release (complete basic HTML logger)
+- [x] v0.1.0 - "First release" update (complete basic HTML logger)
 - [x] v0.2.0 - Structural update (added basic console logger with HTML base)
+- [x] v0.2.1 - Protections update (hidden part of the functionality)
 - [x] v0.3.0 - Background update (added background for log entries)
 - [x] v0.4.0 - Buffer update (added text buffer)
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
-- [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
+- [x] v0.5.1 - Hints update (added hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
-- [x] v0.6.1 - Animation update (added animations in processes)
-- [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
+- [x] v0.6.1 - Animation update (extended animations in processes)
+- [x] v0.7.0 - "Buffer improvement" update (buffer development completed)
 - [x] v0.7.1 - Modding update (buffer modification added - sorting, searching and selecting)
 - [x] v0.7.2 - Categories update (separated the entry category from the type)
 - [x] v0.8.0 - Export update (added conversion to csv)
 - [x] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [x] v0.9.1 - Documenting update (documented library)
 - [x] v0.9.2 - Feature update (made optimizations)
-- [ ] v0.9.3 - Web docs update (added generation of web docs)
+- [x] v0.9.3 - Web docs update (added generation of web docs)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
 
 - [Content](#content)
 
-## LICENSE
-
-The full text of the license can be found at the following [link](https://github.com/Nakama3942/mighty_logger/blob/master/LICENSE).
-
-> Copyright © 2023 Kalynovsky Valentin. All rights reserved.
-> 
-> Licensed under the Apache License, Version 2.0 (the "License");
-> you may not use this file except in compliance with the License.
-> You may obtain a copy of the License at
-> 
->     http://www.apache.org/licenses/LICENSE-2.0
-> 
-> Unless required by applicable law or agreed to in writing, software
-> distributed under the License is distributed on an "AS IS" BASIS,
-> WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-> See the License for the specific language governing permissions and
+## Features
 
-- [Content](#content)
+- **Support for a large number of logger entry types** (empty, entry: debug, debug_performance, performance, event, audit, metrics, user, message, info, notice, warning, error, critical, resolved, unresolved)
+- **Support for five working environments** (CONSOLE, PLAIN_CONSOLE, HTML, MARKDOWN, PLAIN)
+- **Provides publisher methods**
+- **Provides to sort the logs**
+- **Provides to search the logs**
+- **Provides to select the desired logs**
+- **Provides to export logs to csv**
+- **Implemented own Text Buffer**
+- **Provided the ability to control the Buffer**
+- **Logs can be saved and loaded**
+- **Implemented wrapper method for Python input()**
+- **You can run logging Processes**
+- **You can run logging Timers**
+- **Implemented a simplified Logger class**
+- **When creating a Logger, an entry is created about the characteristics of the system**
+- **Show time of logging for every entry log**
+- **Provided are more than 20 animations for indefinite processes and 6 for definite processes**
+- **Provided are ANSI escape code table**
+- **Provides colors in RGB, HEX, ANSI**
+- **Provided are 4 sorting options** (by time, by reverse time, by category, by type)
+- **Provided are 5 exceptions**
 
 ## Installation
 
-Despite the fact that the library was originally developed for use in PyQt, it does not require PyQt to be installed, since this framework for outputting to Text fields, which support not only Plain Text, uses HTML and this library simply simplifies the logging process, since the creation process already formatted strings is registered in this library.
-
 To install the library, enter the command:
 
 ```sh
 pip install mighty_logger
 ```
 
 ## Usage
 
-ATTENTION!!! OUTDATED MATERIAL! RELEVANCE - v0.6.1! WILL BE OVERWRITTEN IN v0.9.1!
-
 This is the simplest example of using the library:
 
 ```python
 from mighty_logger import Logger
-from mighty_logger.src import StatusMessagePatterns
 
 if __name__ == "__main__":
-	logger = Logger(program_name="Test", console_width=115)
-	logger.message(status_message=StatusMessagePatterns.custom("Hooray"), message_text="Hello world!")
+	logger = Logger()
+	logger.message("Hello world!")
+	print("\n".join(logger.might.buffer))
 ```
 
-The outputs in console will contain the following text (GitHub, PyPi and possibly some other sites do not support displaying colors in Markdown - use resources that support them, such as PyCharm):
+The outputs in console will contain the following text:
 
 <pre>
-<span style='background-color: #;'><span style='color: #ffd700;'>-Test?entry> $███████████████^████@███████:██████████:█████:█████████:█████</span></span>
-<span style='background-color: #;'><span style='color: #b0e0e6;'>-?entry>         </span><span style='color: #da70d6;'>*2023-06-08 14:01:39.423493 </span>💬 <span style='color: #ffa500;'>#STATUS: </span><span style='color: #ff8c00;'>Hooray </span><span style='color: #afeeee;'>@MESSAGE - </span><span style='color: #b0e0e6;'>Hello world!</span></span>
+-Unknown?entry> $DESKTOP-8KG0R64:User:Windows:10.0.19045:64bit:WindowsPE:AMD64
+-?entry>          *2023-07-04 21:12:05.919593 📝 #STATUS: @MESSAGE - Hello world!
 </pre>
 
-See the APPLYING.md file for more details.
-
-- [Content](#content)
-
-## *Additional functionality*
-
-*Additional functionality is also planned. Let's keep it a secret for now. Let it be a surprise.*
-
-- [Content](#content)
-
-## Data
-
-See the DATA.md file.
-
 - [Content](#content)
 
 ## Troubleshooting
 
 All functionality of the library has been tested by me, but if you have problems using it, the code does not work, have suggestions for optimization or advice for improving the style of the code and the name - I invite you [here](https://github.com/Nakama3942/mighty_logger/blob/master/CONTRIBUTING.md) and [here](https://github.com/Nakama3942/mighty_logger/blob/master/CODE_OF_CONDUCT.md).
 
 - [Content](#content)
```

### Comparing `mighty_logger-0.9.2/pyproject.toml` & `mighty_logger-0.9.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mighty_logger"
-version = "0.9.2"
+version = "0.9.3"
 authors = [
 	{name = "Kalynovsky 'Nakamura Akira' Valentin", email = "nakama3942@gmail.com"},
 ]
-description = "Powerful functional logger"
+description = "Mighty functional logger"
 readme = "README.md"
 license = {text = "Apache License Version 2.0"}
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
 	"License :: OSI Approved :: Apache Software License",
 	"Operating System :: OS Independent",
@@ -42,11 +42,10 @@
 Repository = "https://github.com/Nakama3942/mighty_logger"
 Releases = "https://github.com/Nakama3942/mighty_logger/releases"
 
 [tool.setuptools]
 packages = [
 	'mighty_logger',
 	'mighty_logger.src',
-	'mighty_logger.src.lib_types_collection',
 	'mighty_logger.basic',
 	'mighty_logger.basic.lib_types'
 ]
```


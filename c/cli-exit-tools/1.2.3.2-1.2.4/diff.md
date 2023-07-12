# Comparing `tmp/cli_exit_tools-1.2.3.2.tar.gz` & `tmp/cli_exit_tools-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_exit_tools-1.2.3.2.tar", last modified: Thu Jun  2 08:57:38 2022, max compression
+gzip compressed data, was "cli_exit_tools-1.2.4.tar", last modified: Wed Jul 12 14:33:52 2023, max compression
```

## Comparing `cli_exit_tools-1.2.3.2.tar` & `cli_exit_tools-1.2.4.tar`

### file list

```diff
@@ -1,23 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 08:57:38.061936 cli_exit_tools-1.2.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-06-02 08:56:38.000000 cli_exit_tools-1.2.3.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-06-02 08:56:38.000000 cli_exit_tools-1.2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-02 08:56:38.000000 cli_exit_tools-1.2.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13378 2022-06-02 08:57:38.061936 cli_exit_tools-1.2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12714 2022-06-02 08:57:35.000000 cli_exit_tools-1.2.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 08:57:38.061936 cli_exit_tools-1.2.3.2/cli_exit_tools/
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-06-02 08:56:38.000000 cli_exit_tools-1.2.3.2/cli_exit_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-06-02 08:56:38.000000 cli_exit_tools-1.2.3.2/cli_exit_tools/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6645 2022-06-02 08:56:38.000000 cli_exit_tools-1.2.3.2/cli_exit_tools/cli_exit_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-06-02 08:56:38.000000 cli_exit_tools-1.2.3.2/cli_exit_tools/cli_exit_tools_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 08:56:38.000000 cli_exit_tools-1.2.3.2/cli_exit_tools/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 08:57:38.061936 cli_exit_tools-1.2.3.2/cli_exit_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13378 2022-06-02 08:57:37.000000 cli_exit_tools-1.2.3.2/cli_exit_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-06-02 08:57:38.000000 cli_exit_tools-1.2.3.2/cli_exit_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 08:57:37.000000 cli_exit_tools-1.2.3.2/cli_exit_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-06-02 08:57:37.000000 cli_exit_tools-1.2.3.2/cli_exit_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 08:57:31.000000 cli_exit_tools-1.2.3.2/cli_exit_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-06-02 08:57:37.000000 cli_exit_tools-1.2.3.2/cli_exit_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-02 08:57:37.000000 cli_exit_tools-1.2.3.2/cli_exit_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-06-02 08:56:38.000000 cli_exit_tools-1.2.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-02 08:57:38.065936 cli_exit_tools-1.2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4167 2022-06-02 08:56:38.000000 cli_exit_tools-1.2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.381497 cli_exit_tools-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.373497 cli_exit_tools-1.2.4/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.361497 cli_exit_tools-1.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.373497 cli_exit_tools-1.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14021 2023-07-12 14:33:52.381497 cli_exit_tools-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.377498 cli_exit_tools-1.2.4/cli_exit_tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.381497 cli_exit_tools-1.2.4/cli_exit_tools/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools/cli_exit_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools/cli_exit_tools_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.377498 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14021 2023-07-12 14:33:52.000000 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-12 14:33:52.000000 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:33:52.000000 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 14:33:52.000000 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-12 14:33:52.000000 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 14:33:52.000000 cli_exit_tools-1.2.4/cli_exit_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/cli_exit_tools.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:33:52.381497 cli_exit_tools-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.381497 cli_exit_tools-1.2.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:33:52.381497 cli_exit_tools-1.2.4/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-12 14:33:04.000000 cli_exit_tools-1.2.4/tests/test_cli.py
```

### Comparing `cli_exit_tools-1.2.3.2/CHANGES.rst` & `cli_exit_tools-1.2.4/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.2.4
+---------
+2023-07-12:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+
 v1.2.3.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v1.2.3.1
 --------
 2022-06-01: update github actions test matrix
```

### Comparing `cli_exit_tools-1.2.3.2/LICENSE` & `cli_exit_tools-1.2.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 1990-2022 Robert Nowotny
+Copyright (c) 1990-2023 Robert Nowotny
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `cli_exit_tools-1.2.3.2/PKG-INFO` & `cli_exit_tools-1.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: cli_exit_tools
-Version: 1.2.3.2
+Version: 1.2.4
 Summary: functions to exit an cli application properly
-Home-page: https://github.com/bitranox/cli_exit_tools
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/cli_exit_tools
+Project-URL: Documentation, https://github.com/bitranox/cli_exit_tools/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/cli_exit_tools.git
+Project-URL: Changelog, https://github.com/bitranox/cli_exit_tools/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 cli_exit_tools
 ==============
 
 
-Version v1.2.3.2 as of 2022-06-02 see `Changelog`_
+Version v1.2.4 as of 2023-07-12 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml
 
 
@@ -41,30 +45,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/cli-exit-tools?label=PyPI%20Package
    :target: https://badge.fury.io/py/cli_exit_tools
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/cli_exit_tools
    :target: https://codecov.io/gh/bitranox/cli_exit_tools
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/cli_exit_tools?branch=master
-   :target: https://bettercodehub.com/results/bitranox/cli_exit_tools
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/cli_exit_tools?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/cli_exit_tools/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/cli_exit_tools?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/cli_exit_tools/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/cli_exit_tools?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/cli_exit_tools/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/cli_exit_tools
+.. |snyk| image:: https://snyk.io/test/github/bitranox/cli_exit_tools/badge.svg
    :target: https://snyk.io/test/github/bitranox/cli_exit_tools
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/cli-exit-tools
    :target: https://pypi.org/project/cli-exit-tools/
@@ -75,22 +76,22 @@
 - print the traceback information (can be set with commandline option)
 - get a proper exit code from the Exception
 - flush the streams, to make sure output is written in proper order
 - demo how to integrate into Your cli module (see usage)
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/cli_exit_tools>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/cli_exit_tools/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -142,15 +143,15 @@
         >>> info()
         Info for ...
 
         """
         __init__conf__.print_info()
 
 
-    @click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)
+    @click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)    # type: ignore
     @click.version_option(
         version=__init__conf__.version, prog_name=__init__conf__.shell_command, message=f"{__init__conf__.shell_command} version {__init__conf__.version}"
     )
     @click.option("--traceback/--no-traceback", is_flag=True, type=bool, default=None, help="return traceback information on cli")
     def cli_main(traceback: Optional[bool] = None) -> None:
         if traceback is not None:
             cli_exit_tools.config.traceback = traceback
@@ -161,15 +162,15 @@
         """get program informations"""
         info()
 
 
     # entry point if main
     if __name__ == "__main__":
         try:
-            cli_main()
+            cli_main()      # type: ignore
         except Exception as exc:
             cli_exit_tools.print_exception_message()
             sys.exit(cli_exit_tools.get_system_exit_code(exc))
         finally:
             cli_exit_tools.flush_streams()
 
 - get the system exit code
@@ -312,14 +313,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade cli_exit_tools
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade cli_exit_tools[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/cli_exit_tools.git
 
@@ -335,22 +343,22 @@
     # for the latest development version :
     cli_exit_tools @ git+https://github.com/bitranox/cli_exit_tools.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/cli_exit_tools.git
     $ cd cli_exit_tools
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -401,14 +409,27 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.2.4
+---------
+2023-07-12:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+
 v1.2.3.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v1.2.3.1
 --------
 2022-06-01: update github actions test matrix
```

### Comparing `cli_exit_tools-1.2.3.2/README.rst` & `cli_exit_tools-1.2.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 cli_exit_tools
 ==============
 
 
-Version v1.2.3.2 as of 2022-06-02 see `Changelog`_
+Version v1.2.4 as of 2023-07-12 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml
 
 
@@ -23,30 +23,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/cli-exit-tools?label=PyPI%20Package
    :target: https://badge.fury.io/py/cli_exit_tools
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/cli_exit_tools
    :target: https://codecov.io/gh/bitranox/cli_exit_tools
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/cli_exit_tools?branch=master
-   :target: https://bettercodehub.com/results/bitranox/cli_exit_tools
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/cli_exit_tools?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/cli_exit_tools/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/cli_exit_tools?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/cli_exit_tools/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/cli_exit_tools?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/cli_exit_tools/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/cli_exit_tools
+.. |snyk| image:: https://snyk.io/test/github/bitranox/cli_exit_tools/badge.svg
    :target: https://snyk.io/test/github/bitranox/cli_exit_tools
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/cli-exit-tools
    :target: https://pypi.org/project/cli-exit-tools/
@@ -57,22 +54,22 @@
 - print the traceback information (can be set with commandline option)
 - get a proper exit code from the Exception
 - flush the streams, to make sure output is written in proper order
 - demo how to integrate into Your cli module (see usage)
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/cli_exit_tools>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/cli_exit_tools/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -124,15 +121,15 @@
         >>> info()
         Info for ...
 
         """
         __init__conf__.print_info()
 
 
-    @click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)
+    @click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)    # type: ignore
     @click.version_option(
         version=__init__conf__.version, prog_name=__init__conf__.shell_command, message=f"{__init__conf__.shell_command} version {__init__conf__.version}"
     )
     @click.option("--traceback/--no-traceback", is_flag=True, type=bool, default=None, help="return traceback information on cli")
     def cli_main(traceback: Optional[bool] = None) -> None:
         if traceback is not None:
             cli_exit_tools.config.traceback = traceback
@@ -143,15 +140,15 @@
         """get program informations"""
         info()
 
 
     # entry point if main
     if __name__ == "__main__":
         try:
-            cli_main()
+            cli_main()      # type: ignore
         except Exception as exc:
             cli_exit_tools.print_exception_message()
             sys.exit(cli_exit_tools.get_system_exit_code(exc))
         finally:
             cli_exit_tools.flush_streams()
 
 - get the system exit code
@@ -294,14 +291,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade cli_exit_tools
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade cli_exit_tools[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/cli_exit_tools.git
 
@@ -317,22 +321,22 @@
     # for the latest development version :
     cli_exit_tools @ git+https://github.com/bitranox/cli_exit_tools.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/cli_exit_tools.git
     $ cd cli_exit_tools
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -383,14 +387,27 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.2.4
+---------
+2023-07-12:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+
 v1.2.3.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v1.2.3.1
 --------
 2022-06-01: update github actions test matrix
```

### Comparing `cli_exit_tools-1.2.3.2/cli_exit_tools/__init__.py` & `cli_exit_tools-1.2.4/cli_exit_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cli_exit_tools-1.2.3.2/cli_exit_tools/cli_exit_tools.py` & `cli_exit_tools-1.2.4/cli_exit_tools/cli_exit_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             return exit_code
         except (AttributeError, TypeError):
             pass
 
     if "posix" in sys.builtin_module_names:
         exceptions = posix_exceptions
     else:
-        exceptions = windows_exceptions
+        exceptions = windows_exceptions     # pragma: no cover
 
     # Handle all other Exceptions
     for exception in exceptions:
         if isinstance(exc, exception):
             return exceptions[exception]
 
     # this should never happen
```

### Comparing `cli_exit_tools-1.2.3.2/cli_exit_tools/cli_exit_tools_cli.py` & `cli_exit_tools-1.2.4/cli_exit_tools/cli_exit_tools_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     >>> info()
     Info for ...
 
     """
     __init__conf__.print_info()
 
 
-@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)
+@click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)    # type: ignore
 @click.version_option(
     version=__init__conf__.version, prog_name=__init__conf__.shell_command, message=f"{__init__conf__.shell_command} version {__init__conf__.version}"
 )
 @click.option("--traceback/--no-traceback", is_flag=True, type=bool, default=None, help="return traceback information on cli")
 def cli_main(traceback: Optional[bool] = None) -> None:
     if traceback is not None:
         cli_exit_tools.config.traceback = traceback
@@ -42,14 +42,14 @@
     """get program informations"""
     info()
 
 
 # entry point if main
 if __name__ == "__main__":
     try:
-        cli_main()
+        cli_main()      # type: ignore
     except Exception as exc:
         cli_exit_tools.print_exception_message()
         sys.exit(cli_exit_tools.get_system_exit_code(exc))
     finally:
         cli_exit_tools.flush_streams()
 # example}}}
```

### Comparing `cli_exit_tools-1.2.3.2/cli_exit_tools.egg-info/PKG-INFO` & `cli_exit_tools-1.2.4/cli_exit_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: cli-exit-tools
-Version: 1.2.3.2
+Version: 1.2.4
 Summary: functions to exit an cli application properly
-Home-page: https://github.com/bitranox/cli_exit_tools
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/cli_exit_tools
+Project-URL: Documentation, https://github.com/bitranox/cli_exit_tools/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/cli_exit_tools.git
+Project-URL: Changelog, https://github.com/bitranox/cli_exit_tools/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 cli_exit_tools
 ==============
 
 
-Version v1.2.3.2 as of 2022-06-02 see `Changelog`_
+Version v1.2.4 as of 2023-07-12 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml
 
 
@@ -41,30 +45,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/cli-exit-tools?label=PyPI%20Package
    :target: https://badge.fury.io/py/cli_exit_tools
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/cli_exit_tools
    :target: https://codecov.io/gh/bitranox/cli_exit_tools
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/cli_exit_tools?branch=master
-   :target: https://bettercodehub.com/results/bitranox/cli_exit_tools
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/cli_exit_tools?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/cli_exit_tools/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/cli_exit_tools?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/cli_exit_tools/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/cli_exit_tools?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/cli_exit_tools/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/cli_exit_tools
+.. |snyk| image:: https://snyk.io/test/github/bitranox/cli_exit_tools/badge.svg
    :target: https://snyk.io/test/github/bitranox/cli_exit_tools
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/cli-exit-tools
    :target: https://pypi.org/project/cli-exit-tools/
@@ -75,22 +76,22 @@
 - print the traceback information (can be set with commandline option)
 - get a proper exit code from the Exception
 - flush the streams, to make sure output is written in proper order
 - demo how to integrate into Your cli module (see usage)
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/cli_exit_tools>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/cli_exit_tools/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/cli_exit_tools/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -142,15 +143,15 @@
         >>> info()
         Info for ...
 
         """
         __init__conf__.print_info()
 
 
-    @click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)
+    @click.group(help=__init__conf__.title, context_settings=CLICK_CONTEXT_SETTINGS)    # type: ignore
     @click.version_option(
         version=__init__conf__.version, prog_name=__init__conf__.shell_command, message=f"{__init__conf__.shell_command} version {__init__conf__.version}"
     )
     @click.option("--traceback/--no-traceback", is_flag=True, type=bool, default=None, help="return traceback information on cli")
     def cli_main(traceback: Optional[bool] = None) -> None:
         if traceback is not None:
             cli_exit_tools.config.traceback = traceback
@@ -161,15 +162,15 @@
         """get program informations"""
         info()
 
 
     # entry point if main
     if __name__ == "__main__":
         try:
-            cli_main()
+            cli_main()      # type: ignore
         except Exception as exc:
             cli_exit_tools.print_exception_message()
             sys.exit(cli_exit_tools.get_system_exit_code(exc))
         finally:
             cli_exit_tools.flush_streams()
 
 - get the system exit code
@@ -312,14 +313,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade cli_exit_tools
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade cli_exit_tools[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/cli_exit_tools.git
 
@@ -335,22 +343,22 @@
     # for the latest development version :
     cli_exit_tools @ git+https://github.com/bitranox/cli_exit_tools.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/cli_exit_tools.git
     $ cd cli_exit_tools
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -401,14 +409,27 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.2.4
+---------
+2023-07-12:
+    - introduce PEP517 packaging standard
+    - introduce pyproject.toml build-system
+    - remove mypy.ini
+    - remove pytest.ini
+    - remove setup.cfg
+    - remove setup.py
+    - remove .bettercodehub.yml
+    - remove .travis.yml
+    - update black config
+
 v1.2.3.2
 ---------
 2022-06-02: update to github actions checkout@v3 and setup-python@v3
 
 v1.2.3.1
 --------
 2022-06-01: update github actions test matrix
```


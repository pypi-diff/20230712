# Comparing `tmp/lib_programname-2.0.5.tar.gz` & `tmp/lib_programname-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_programname-2.0.5.tar", last modified: Thu Jun  2 15:10:56 2022, max compression
+gzip compressed data, was "lib_programname-2.0.6.tar", last modified: Wed Jul 12 15:50:50 2023, max compression
```

## Comparing `lib_programname-2.0.5.tar` & `lib_programname-2.0.6.tar`

### file list

```diff
@@ -1,23 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 15:10:56.195370 lib_programname-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-06-02 15:10:08.000000 lib_programname-2.0.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-06-02 15:10:08.000000 lib_programname-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-02 15:10:08.000000 lib_programname-2.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9188 2022-06-02 15:10:56.195370 lib_programname-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8525 2022-06-02 15:10:08.000000 lib_programname-2.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 15:10:56.195370 lib_programname-2.0.5/lib_programname/
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-06-02 15:10:08.000000 lib_programname-2.0.5/lib_programname/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-06-02 15:10:08.000000 lib_programname-2.0.5/lib_programname/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7266 2022-06-02 15:10:08.000000 lib_programname-2.0.5/lib_programname/lib_programname.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-06-02 15:10:08.000000 lib_programname-2.0.5/lib_programname/lib_programname_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-02 15:10:08.000000 lib_programname-2.0.5/lib_programname/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-02 15:10:56.195370 lib_programname-2.0.5/lib_programname.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9188 2022-06-02 15:10:55.000000 lib_programname-2.0.5/lib_programname.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-06-02 15:10:56.000000 lib_programname-2.0.5/lib_programname.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 15:10:55.000000 lib_programname-2.0.5/lib_programname.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-06-02 15:10:55.000000 lib_programname-2.0.5/lib_programname.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-02 15:10:53.000000 lib_programname-2.0.5/lib_programname.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-02 15:10:56.000000 lib_programname-2.0.5/lib_programname.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-02 15:10:56.000000 lib_programname-2.0.5/lib_programname.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-06-02 15:10:08.000000 lib_programname-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-02 15:10:56.195370 lib_programname-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4169 2022-06-02 15:10:08.000000 lib_programname-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.482601 lib_programname-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/badges_project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.474600 lib_programname-2.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-12 15:49:57.000000 lib_programname-2.0.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-12 15:49:57.000000 lib_programname-2.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-12 15:49:57.000000 lib_programname-2.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-12 15:49:57.000000 lib_programname-2.0.6/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-12 15:49:57.000000 lib_programname-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 15:49:57.000000 lib_programname-2.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-12 15:49:57.000000 lib_programname-2.0.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-07-12 15:50:50.482601 lib_programname-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-12 15:49:57.000000 lib_programname-2.0.6/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-12 15:49:57.000000 lib_programname-2.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-12 15:49:57.000000 lib_programname-2.0.6/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/lib_programname/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/lib_programname/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname/lib_programname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname/lib_programname_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/lib_programname.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-07-12 15:50:50.000000 lib_programname-2.0.6/lib_programname.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-12 15:50:50.000000 lib_programname-2.0.6/lib_programname.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:50:50.000000 lib_programname-2.0.6/lib_programname.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-12 15:50:50.000000 lib_programname-2.0.6/lib_programname.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-12 15:50:50.000000 lib_programname-2.0.6/lib_programname.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 15:50:50.000000 lib_programname-2.0.6/lib_programname.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-12 15:49:57.000000 lib_programname-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 15:49:57.000000 lib_programname-2.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-12 15:49:57.000000 lib_programname-2.0.6/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:50:50.482601 lib_programname-2.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/test_cli.py
```

### Comparing `lib_programname-2.0.5/CHANGES.rst` & `lib_programname-2.0.6/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.6
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
 v2.0.5
 --------
 2022-06-02: correct mypy type error
 
 v2.0.4.2
 --------
 2022-06-01: update to github actions checkout@v3 and setup-python@v3
```

### Comparing `lib_programname-2.0.5/LICENSE` & `lib_programname-2.0.6/LICENSE`

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

### Comparing `lib_programname-2.0.5/PKG-INFO` & `lib_programname-2.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: lib_programname
-Version: 2.0.5
+Version: 2.0.6
 Summary: get reliably the name of the executed script
-Home-page: https://github.com/bitranox/lib_programname
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_programname
+Project-URL: Documentation, https://github.com/bitranox/lib_programname/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_programname.git
+Project-URL: Changelog, https://github.com/bitranox/lib_programname/blob/master/CHANGES.rst
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
 
 lib_programname
 ===============
 
 
-Version v2.0.5 as of 2022-06-02 see `Changelog`_
+Version v2.0.6 as of 2023-07-12 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml
 
 
@@ -41,30 +45,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-programname?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_programname
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_programname
    :target: https://codecov.io/gh/bitranox/lib_programname
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_programname?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_programname
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_programname?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_programname/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_programname?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_programname/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_programname?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_programname/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_programname
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_programname/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_programname
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-programname
    :target: https://pypi.org/project/lib-programname/
@@ -81,22 +82,22 @@
     $> python -m pip install lib_programname
     $> python
     >>> import lib_programname
     >>> path_to_program = lib_programname.get_path_executed_script()    # type: pathlib.Path
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_programname>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_programname/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -156,14 +157,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_programname
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_programname[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_programname.git
 
@@ -179,22 +187,22 @@
     # for the latest development version :
     lib_programname @ git+https://github.com/bitranox/lib_programname.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_programname.git
     $ cd lib_programname
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -246,14 +254,27 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.6
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
 v2.0.5
 --------
 2022-06-02: correct mypy type error
 
 v2.0.4.2
 --------
 2022-06-01: update to github actions checkout@v3 and setup-python@v3
```

### Comparing `lib_programname-2.0.5/README.rst` & `lib_programname-2.0.6/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 lib_programname
 ===============
 
 
-Version v2.0.5 as of 2022-06-02 see `Changelog`_
+Version v2.0.6 as of 2023-07-12 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml
 
 
@@ -23,30 +23,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-programname?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_programname
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_programname
    :target: https://codecov.io/gh/bitranox/lib_programname
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_programname?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_programname
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_programname?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_programname/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_programname?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_programname/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_programname?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_programname/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_programname
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_programname/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_programname
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-programname
    :target: https://pypi.org/project/lib-programname/
@@ -63,22 +60,22 @@
     $> python -m pip install lib_programname
     $> python
     >>> import lib_programname
     >>> path_to_program = lib_programname.get_path_executed_script()    # type: pathlib.Path
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_programname>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_programname/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -138,14 +135,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_programname
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_programname[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_programname.git
 
@@ -161,22 +165,22 @@
     # for the latest development version :
     lib_programname @ git+https://github.com/bitranox/lib_programname.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_programname.git
     $ cd lib_programname
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -228,14 +232,27 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.6
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
 v2.0.5
 --------
 2022-06-02: correct mypy type error
 
 v2.0.4.2
 --------
 2022-06-01: update to github actions checkout@v3 and setup-python@v3
```

### Comparing `lib_programname-2.0.5/lib_programname/__init__.py` & `lib_programname-2.0.6/lib_programname/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.5/lib_programname/__init__conf__.py` & `lib_programname-2.0.6/lib_programname/__init__conf__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # CONF
 
-name = "lib_programname"
-title = "get reliably the name of the executed script"
-version = "v2.0.5"
-url = "https://github.com/bitranox/lib_programname"
-author = "Robert Nowotny"
-author_email = "bitranox@gmail.com"
-shell_command = "lib_programname"
+name = 'lib_programname'
+title = 'get reliably the name of the executed script'
+version = 'v2.0.6'
+url = 'https://github.com/bitranox/lib_programname'
+author = 'Robert Nowotny'
+author_email = 'bitranox@gmail.com'
+shell_command = 'lib_programname'
 
 
 def print_info() -> None:
-    print(
-        """\
+    print("""\
 
 Info for lib_programname:
 
     get reliably the name of the executed script
 
-    Version : v2.0.5
+    Version : v2.0.6
     Url     : https://github.com/bitranox/lib_programname
     Author  : Robert Nowotny
-    Email   : bitranox@gmail.com"""
-    )
+    Email   : bitranox@gmail.com""")
```

### Comparing `lib_programname-2.0.5/lib_programname/lib_programname.py` & `lib_programname-2.0.6/lib_programname/lib_programname.py`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.5/lib_programname/lib_programname_cli.py` & `lib_programname-2.0.6/lib_programname/lib_programname_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
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
@@ -44,13 +44,13 @@
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
```

### Comparing `lib_programname-2.0.5/lib_programname.egg-info/PKG-INFO` & `lib_programname-2.0.6/lib_programname.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: lib-programname
-Version: 2.0.5
+Version: 2.0.6
 Summary: get reliably the name of the executed script
-Home-page: https://github.com/bitranox/lib_programname
-Author: Robert Nowotny
-Author-email: bitranox@gmail.com
+Author-email: Robert Nowotny <bitranox@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/bitranox/lib_programname
+Project-URL: Documentation, https://github.com/bitranox/lib_programname/blob/master/README.rst
+Project-URL: Repository, https://github.com/bitranox/lib_programname.git
+Project-URL: Changelog, https://github.com/bitranox/lib_programname/blob/master/CHANGES.rst
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
 
 lib_programname
 ===============
 
 
-Version v2.0.5 as of 2022-06-02 see `Changelog`_
+Version v2.0.6 as of 2023-07-12 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
-|codecov| |better_code| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
+|codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
 .. |build_badge| image:: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml/badge.svg
    :target: https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml
 
 
@@ -41,30 +45,27 @@
 .. for the pypi status link note the dashes, not the underscore !
 .. |pypi| image:: https://img.shields.io/pypi/status/lib-programname?label=PyPI%20Package
    :target: https://badge.fury.io/py/lib_programname
 
 .. |codecov| image:: https://img.shields.io/codecov/c/github/bitranox/lib_programname
    :target: https://codecov.io/gh/bitranox/lib_programname
 
-.. |better_code| image:: https://bettercodehub.com/edge/badge/bitranox/lib_programname?branch=master
-   :target: https://bettercodehub.com/results/bitranox/lib_programname
-
 .. |cc_maintain| image:: https://img.shields.io/codeclimate/maintainability-percentage/bitranox/lib_programname?label=CC%20maintainability
    :target: https://codeclimate.com/github/bitranox/lib_programname/maintainability
    :alt: Maintainability
 
 .. |cc_issues| image:: https://img.shields.io/codeclimate/issues/bitranox/lib_programname?label=CC%20issues
    :target: https://codeclimate.com/github/bitranox/lib_programname/maintainability
    :alt: Maintainability
 
 .. |cc_coverage| image:: https://img.shields.io/codeclimate/coverage/bitranox/lib_programname?label=CC%20coverage
    :target: https://codeclimate.com/github/bitranox/lib_programname/test_coverage
    :alt: Code Coverage
 
-.. |snyk| image:: https://img.shields.io/snyk/vulnerabilities/github/bitranox/lib_programname
+.. |snyk| image:: https://snyk.io/test/github/bitranox/lib_programname/badge.svg
    :target: https://snyk.io/test/github/bitranox/lib_programname
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-programname
    :target: https://pypi.org/project/lib-programname/
@@ -81,22 +82,22 @@
     $> python -m pip install lib_programname
     $> python
     >>> import lib_programname
     >>> path_to_program = lib_programname.get_path_executed_script()    # type: pathlib.Path
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.6, 3.7, 3.8, 3.9, 3.10, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/lib_programname>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/lib_programname/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_programname/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -156,14 +157,21 @@
 
 - to install the latest release from PyPi via pip (recommended):
 
 .. code-block::
 
     python -m pip install --upgrade lib_programname
 
+
+- to install the latest release from PyPi via pip, including test dependencies:
+
+.. code-block::
+
+    python -m pip install --upgrade lib_programname[test]
+
 - to install the latest version from github via pip:
 
 
 .. code-block::
 
     python -m pip install --upgrade git+https://github.com/bitranox/lib_programname.git
 
@@ -179,22 +187,22 @@
     # for the latest development version :
     lib_programname @ git+https://github.com/bitranox/lib_programname.git
 
     # to install and upgrade all modules mentioned in requirements.txt:
     python -m pip install --upgrade -r /<path>/requirements.txt
 
 
-- to install the latest development version from source code:
+- to install the latest development version, including test dependencies from source code:
 
 .. code-block::
 
     # cd ~
     $ git clone https://github.com/bitranox/lib_programname.git
     $ cd lib_programname
-    python setup.py install
+    python -m pip install -e .[test]
 
 - via makefile:
   makefiles are a very convenient way to install. Here we can do much more,
   like installing virtual environments, clean caches and so on.
 
 .. code-block:: shell
 
@@ -246,14 +254,27 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.6
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
 v2.0.5
 --------
 2022-06-02: correct mypy type error
 
 v2.0.4.2
 --------
 2022-06-01: update to github actions checkout@v3 and setup-python@v3
```


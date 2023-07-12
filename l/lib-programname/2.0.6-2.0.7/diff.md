# Comparing `tmp/lib_programname-2.0.6.tar.gz` & `tmp/lib_programname-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_programname-2.0.6.tar", last modified: Wed Jul 12 15:50:50 2023, max compression
+gzip compressed data, was "lib_programname-2.0.7.tar", last modified: Wed Jul 12 19:23:37 2023, max compression
```

## Comparing `lib_programname-2.0.6.tar` & `lib_programname-2.0.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.482601 lib_programname-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/.docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/README_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/acknowledgment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/badges_project.rst
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/commandline_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/description.rst
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/installation_via_makefile.rst
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/installation_via_pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/licence_mit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/tested_under.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/try_in_jupyter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.474600 lib_programname-2.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-12 15:49:57.000000 lib_programname-2.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-12 15:49:57.000000 lib_programname-2.0.6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-12 15:49:57.000000 lib_programname-2.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-12 15:49:57.000000 lib_programname-2.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-12 15:49:57.000000 lib_programname-2.0.6/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-12 15:49:57.000000 lib_programname-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 15:49:57.000000 lib_programname-2.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-12 15:49:57.000000 lib_programname-2.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-07-12 15:50:50.482601 lib_programname-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-12 15:49:57.000000 lib_programname-2.0.6/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-07-12 15:49:57.000000 lib_programname-2.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-12 15:49:57.000000 lib_programname-2.0.6/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/lib_programname/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/lib_programname/3rd_party_stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname/3rd_party_stubs/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname/lib_programname.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname/lib_programname_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/lib_programname.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9799 2023-07-12 15:50:50.000000 lib_programname-2.0.6/lib_programname.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-12 15:50:50.000000 lib_programname-2.0.6/lib_programname.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:50:50.000000 lib_programname-2.0.6/lib_programname.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-12 15:50:50.000000 lib_programname-2.0.6/lib_programname.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-12 15:50:50.000000 lib_programname-2.0.6/lib_programname.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 15:50:50.000000 lib_programname-2.0.6/lib_programname.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-12 15:49:57.000000 lib_programname-2.0.6/lib_programname.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-12 15:49:57.000000 lib_programname-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 15:49:57.000000 lib_programname-2.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-12 15:49:57.000000 lib_programname-2.0.6/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:50:50.482601 lib_programname-2.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:50:50.478601 lib_programname-2.0.6/tests/local_testscripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/lib_bash_functions.sh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/run_clean.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/run_pytest.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/run_testloop.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/run_testloop_windows.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/shellcheck.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/local_testscripts/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-12 15:49:57.000000 lib_programname-2.0.6/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.101968 lib_programname-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.093968 lib_programname-2.0.7/.docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/README_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/acknowledgment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/badges_project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/commandline_help.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/description.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/installation_via_makefile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/installation_via_pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/licence_mit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/tested_under.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/try_in_jupyter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.085968 lib_programname-2.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.093968 lib_programname-2.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-12 19:22:50.000000 lib_programname-2.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-12 19:22:50.000000 lib_programname-2.0.7/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-12 19:22:50.000000 lib_programname-2.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-12 19:22:50.000000 lib_programname-2.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-12 19:22:50.000000 lib_programname-2.0.7/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-12 19:22:50.000000 lib_programname-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-12 19:22:50.000000 lib_programname-2.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-12 19:22:50.000000 lib_programname-2.0.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-12 19:23:37.101968 lib_programname-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-12 19:22:50.000000 lib_programname-2.0.7/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-12 19:23:24.000000 lib_programname-2.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-12 19:22:50.000000 lib_programname-2.0.7/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.097968 lib_programname-2.0.7/lib_programname/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.097968 lib_programname-2.0.7/lib_programname/3rd_party_stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname/3rd_party_stubs/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname/lib_programname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname/lib_programname_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.097968 lib_programname-2.0.7/lib_programname.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-07-12 19:23:37.000000 lib_programname-2.0.7/lib_programname.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-12 19:23:37.000000 lib_programname-2.0.7/lib_programname.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:23:37.000000 lib_programname-2.0.7/lib_programname.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-12 19:23:37.000000 lib_programname-2.0.7/lib_programname.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-12 19:23:37.000000 lib_programname-2.0.7/lib_programname.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 19:23:37.000000 lib_programname-2.0.7/lib_programname.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-12 19:22:50.000000 lib_programname-2.0.7/lib_programname.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-12 19:22:50.000000 lib_programname-2.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 19:22:50.000000 lib_programname-2.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-12 19:22:50.000000 lib_programname-2.0.7/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 19:23:37.101968 lib_programname-2.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.097968 lib_programname-2.0.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:23:37.101968 lib_programname-2.0.7/tests/local_testscripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/lib_bash_functions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/run_clean.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/run_pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/run_testloop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/run_testloop_windows.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/shellcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/local_testscripts/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-12 19:22:50.000000 lib_programname-2.0.7/tests/test_cli.py
```

### Comparing `lib_programname-2.0.6/.coveragerc` & `lib_programname-2.0.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/.docs/README_template.rst` & `lib_programname-2.0.7/.docs/README_template.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_programname
 ===============
 
 
-Version v2.0.6 as of 2023-07-12 see `Changelog`_
+Version v2.0.7 as of 2023-07-12 see `Changelog`_
 
 
 .. include:: ./badges.rst
 
 .. include:: ./description.rst
 
 ----
```

### Comparing `lib_programname-2.0.6/.docs/badges.rst` & `lib_programname-2.0.7/.docs/badges.rst`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/.docs/badges_project.rst` & `lib_programname-2.0.7/.docs/badges_project.rst`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/.docs/installation.rst` & `lib_programname-2.0.7/.docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/.github/workflows/codeql-analysis.yml` & `lib_programname-2.0.7/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/.github/workflows/python-package.yml` & `lib_programname-2.0.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/.gitignore` & `lib_programname-2.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/CHANGES.rst` & `lib_programname-2.0.7/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.7
+---------
+2023-07-12:
+    - also works now with symlinks
+    - also works now with scripts and symlinks which do not have a ``py`` extension
+    - clean ./tests/test_cli.py
+
 v2.0.6
 ---------
 2023-07-12:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove mypy.ini
     - remove pytest.ini
```

### Comparing `lib_programname-2.0.6/CODE_OF_CONDUCT.md` & `lib_programname-2.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/CONTRIBUTING.md` & `lib_programname-2.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/ISSUE_TEMPLATE.md` & `lib_programname-2.0.7/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/LICENSE` & `lib_programname-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/Makefile` & `lib_programname-2.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/PKG-INFO` & `lib_programname-2.0.7/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,12 @@
-Metadata-Version: 2.1
-Name: lib_programname
-Version: 2.0.6
-Summary: get reliably the name of the executed script
-Author-email: Robert Nowotny <bitranox@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/bitranox/lib_programname
-Project-URL: Documentation, https://github.com/bitranox/lib_programname/blob/master/README.rst
-Project-URL: Repository, https://github.com/bitranox/lib_programname.git
-Project-URL: Changelog, https://github.com/bitranox/lib_programname/blob/master/CHANGES.rst
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7.0
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-License-File: LICENSE
-
 lib_programname
 ===============
 
 
-Version v2.0.6 as of 2023-07-12 see `Changelog`_
+Version v2.0.7 as of 2023-07-12 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -67,27 +45,70 @@
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-programname
    :target: https://pypi.org/project/lib-programname/
    :alt: PyPI - Downloads
 
+This little Library returns the path of the executed Python Script.
+
 Finding the name of the program from which a Python module is running can be trickier than it would seem at first, so lets make it damned easy.
 This works under pycharm, pytest, pytest-docrunner, uwsgi, dreampie etc. correctly.
 
 You might dive into Dough Hellmans `article <https://doughellmann.com/posts/determining-the-name-of-a-process-from-python/>`_
 about that issue.
 
-.. code-block:: python
+.. code-block::
 
     $> python -m pip install lib_programname
     $> python
     >>> import lib_programname
     >>> path_to_program = lib_programname.get_path_executed_script()    # type: pathlib.Path
 
+
+This also works now if the script does not have any extension and if the scripts is symlinked.
+
+In case the script is called via a symlink, the actual script location is returned, not the symlink !
+
+.. code-block::
+
+    $ # the test script
+    $ cat test.py
+    #!/usr/bin/env python3
+    import lib_programname
+    # this returns the fully resolved path to the launched python program
+    path_to_program = lib_programname.get_path_executed_script()  # type: pathlib.Path
+    print(path_to_program)
+
+    $ # running the script directly works
+    $ ./test.py
+    /Users/tester/test.py
+
+    $ # running the script with a .py named symlink works
+    $ ln -s test.py link2test.py
+    $ ./link2test.py
+    /Users/tester/test.py
+    $ rm link2test.py
+
+    $ # running the script with a symlink without an extension works
+    $ ln -s test.py link2test
+    $ ./link2test
+    /Users/tester/test.py
+    $ rm link2test
+
+    $ # running the script directly also works if it has no extension
+    $ mv test.py testme
+    $ ./testme
+    /Users/tester/testme
+
+    $ # running the extension-less script with a .py named symlink works
+    $ ln -s testme link2test.py
+    $ ./link2test.py
+    /Users/tester/testme
+
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.7.0 or newer
 
@@ -117,15 +138,15 @@
 
 You might try it right away in Jupyter Notebook by using the "launch binder" badge, or click `here <https://mybinder.org/v2/gh/{{rst_include.
 repository_slug}}/master?filepath=lib_programname.ipynb>`_
 
 Usage
 -----------
 
-.. code-block:: py
+.. code-block:: python
 
     import lib_programname
     # this returns the fully resolved path to the launched python program
     path_to_program = lib_programname.get_path_executed_script()    # type: pathlib.Path
 
 Usage from Commandline
 ------------------------
@@ -254,14 +275,21 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.7
+---------
+2023-07-12:
+    - also works now with symlinks
+    - also works now with scripts and symlinks which do not have a ``py`` extension
+    - clean ./tests/test_cli.py
+
 v2.0.6
 ---------
 2023-07-12:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove mypy.ini
     - remove pytest.ini
```

### Comparing `lib_programname-2.0.6/PULL_REQUEST_TEMPLATE.md` & `lib_programname-2.0.7/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/lib_programname/3rd_party_stubs/readme.txt` & `lib_programname-2.0.7/lib_programname/3rd_party_stubs/readme.txt`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/lib_programname/__init__.py` & `lib_programname-2.0.7/lib_programname/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/lib_programname/__init__conf__.py` & `lib_programname-2.0.7/lib_programname/__init__conf__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # CONF
 
 name = 'lib_programname'
 title = 'get reliably the name of the executed script'
-version = 'v2.0.6'
+version = 'v2.0.7'
 url = 'https://github.com/bitranox/lib_programname'
 author = 'Robert Nowotny'
 author_email = 'bitranox@gmail.com'
 shell_command = 'lib_programname'
 
 
 def print_info() -> None:
     print("""\
 
 Info for lib_programname:
 
     get reliably the name of the executed script
 
-    Version : v2.0.6
+    Version : v2.0.7
     Url     : https://github.com/bitranox/lib_programname
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com""")
```

### Comparing `lib_programname-2.0.6/lib_programname/lib_programname.py` & `lib_programname-2.0.7/lib_programname/lib_programname.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,29 +26,29 @@
     >>> # Test via __main__.__file__
     >>> assert get_path_executed_script() == pathlib.Path(__file__).resolve()
 
 
     >>> ### TEST get it via sys.argv
     >>> # Setup
     >>> # force __main__.__file__ invalid
-    >>> __main__.__file__ = str((pathlib.Path(__file__).parent / 'invalid_file.py'))  # .resolve() seems not to work on a non existing file in python 3.5
+    >>> __main__.__file__ = str((pathlib.Path(__file__).parent / 'invalid_file.py'))
 
     >>> # force sys.argv valid
     >>> save_sys_argv = list(sys.argv)
     >>> valid_path = str((pathlib.Path(__file__).resolve()))
     >>> sys.argv = [valid_path]
 
     >>> # Test via sys.argv
     >>> assert get_path_executed_script() == pathlib.Path(__file__).resolve()
 
 
     >>> ### TEST get it via stack
     >>> # Setup
     >>> # force sys.argv invalid
-    >>> invalid_path = str((pathlib.Path(__file__).parent / 'invalid_file.py'))  # .resolve() seems not to work on a non existing file in python 3.5
+    >>> invalid_path = str((pathlib.Path(__file__).parent / 'invalid_file.py'))
     >>> sys.argv = [invalid_path]
 
 
     >>> assert get_path_executed_script()
 
     >>> # teardown
     >>> __main__.__file__ = save_main_file
@@ -101,15 +101,15 @@
     >>> # if (not is_pytest_main_in_sys_argv()) and is_doctest_running(): assert get_fullpath_from_sys_argv() == pathlib.Path(__file__).resolve()
     >>> if lib_detect_testenv.is_doctest_active() and not lib_detect_testenv.is_pytest_active():
     ...     assert get_fullpath_from_sys_argv() == pathlib.Path(__file__).resolve()
     >>> if not lib_detect_testenv.is_doctest_active(): assert get_fullpath_from_sys_argv() != pathlib.Path()
 
     >>> # force test invalid sys.path
     >>> save_sys_argv = list(sys.argv)
-    >>> invalid_path = str((pathlib.Path(__file__).parent / 'invalid_file.py'))  # .resolve() seems not to work on a non existing file in python 3.5
+    >>> invalid_path = str((pathlib.Path(__file__).parent / 'invalid_file.py'))
     >>> sys.argv = [invalid_path]
     >>> assert get_fullpath_from_sys_argv() == pathlib.Path()
     >>> sys.argv = list(save_sys_argv)
 
     >>> # force test valid sys.path
     >>> save_sys_path = list(sys.argv)
     >>> valid_path = str((pathlib.Path(__file__).resolve()))
@@ -143,29 +143,45 @@
                 return valid_executable_path
             levels_back += 1  # pragma: no cover
         except IndexError:  # pragma: no cover
             break  # pragma: no cover
     return empty_path  # pragma: no cover
 
 
-def get_valid_executable_path_or_empty_path(arg_string: str) -> pathlib.Path:
+def get_valid_executable_path_or_empty_path(arg_string: str, only_files_with_extension_py: bool = False) -> pathlib.Path:
     """
-    >>> if lib_detect_testenv.is_doctest_active(): assert get_valid_executable_path_or_empty_path(__main__.__file__) == empty_path
+    :returns
+        a valid path to the executable script, or empty_path
+
+    :parameter arg_string
+        the sysargs as string
+
+    :parameter only_files_with_extension_py
+        only return files with extension ".py" - the old behaviour
+
+    >>> ## normal execution
     >>> assert get_valid_executable_path_or_empty_path(__file__) == pathlib.Path(__file__).resolve()
+    >>> # docrunner.py or doctest.py active
+    >>> if lib_detect_testenv.is_doctest_active(): assert get_valid_executable_path_or_empty_path(__main__.__file__) == empty_path
+    >>> # doctest.py active
+    >>> assert get_valid_executable_path_or_empty_path("doctest.py") == empty_path
     """
 
     # if is_doctest_in_arg_string(arg_string):
     if lib_detect_testenv.is_doctest_active(arg_string):
         return empty_path
 
     arg_string = remove_doctest_and_docrunner_parameters(arg_string)
-    arg_string = add_python_extension_if_not_there(arg_string)
+
+    if only_files_with_extension_py:
+        arg_string = add_python_extension_if_not_there(arg_string)
+
     path = pathlib.Path(arg_string)
     if path.is_file():
-        path = path.resolve()  # .resolve does not work on a non existing file in python 3.5
+        path = path.resolve()
         return path
     else:
         return empty_path
 
 
 def remove_doctest_and_docrunner_parameters(arg_string: str) -> str:
     """
```

### Comparing `lib_programname-2.0.6/lib_programname/lib_programname_cli.py` & `lib_programname-2.0.7/lib_programname/lib_programname_cli.py`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/lib_programname.egg-info/PKG-INFO` & `lib_programname-2.0.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lib-programname
-Version: 2.0.6
+Name: lib_programname
+Version: 2.0.7
 Summary: get reliably the name of the executed script
 Author-email: Robert Nowotny <bitranox@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bitranox/lib_programname
 Project-URL: Documentation, https://github.com/bitranox/lib_programname/blob/master/README.rst
 Project-URL: Repository, https://github.com/bitranox/lib_programname.git
 Project-URL: Changelog, https://github.com/bitranox/lib_programname/blob/master/CHANGES.rst
@@ -20,15 +20,15 @@
 Provides-Extra: test
 License-File: LICENSE
 
 lib_programname
 ===============
 
 
-Version v2.0.6 as of 2023-07-12 see `Changelog`_
+Version v2.0.7 as of 2023-07-12 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -67,27 +67,70 @@
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/lib-programname
    :target: https://pypi.org/project/lib-programname/
    :alt: PyPI - Downloads
 
+This little Library returns the path of the executed Python Script.
+
 Finding the name of the program from which a Python module is running can be trickier than it would seem at first, so lets make it damned easy.
 This works under pycharm, pytest, pytest-docrunner, uwsgi, dreampie etc. correctly.
 
 You might dive into Dough Hellmans `article <https://doughellmann.com/posts/determining-the-name-of-a-process-from-python/>`_
 about that issue.
 
-.. code-block:: python
+.. code-block::
 
     $> python -m pip install lib_programname
     $> python
     >>> import lib_programname
     >>> path_to_program = lib_programname.get_path_executed_script()    # type: pathlib.Path
 
+
+This also works now if the script does not have any extension and if the scripts is symlinked.
+
+In case the script is called via a symlink, the actual script location is returned, not the symlink !
+
+.. code-block::
+
+    $ # the test script
+    $ cat test.py
+    #!/usr/bin/env python3
+    import lib_programname
+    # this returns the fully resolved path to the launched python program
+    path_to_program = lib_programname.get_path_executed_script()  # type: pathlib.Path
+    print(path_to_program)
+
+    $ # running the script directly works
+    $ ./test.py
+    /Users/tester/test.py
+
+    $ # running the script with a .py named symlink works
+    $ ln -s test.py link2test.py
+    $ ./link2test.py
+    /Users/tester/test.py
+    $ rm link2test.py
+
+    $ # running the script with a symlink without an extension works
+    $ ln -s test.py link2test
+    $ ./link2test
+    /Users/tester/test.py
+    $ rm link2test
+
+    $ # running the script directly also works if it has no extension
+    $ mv test.py testme
+    $ ./testme
+    /Users/tester/testme
+
+    $ # running the extension-less script with a .py named symlink works
+    $ ln -s testme link2test.py
+    $ ./link2test.py
+    /Users/tester/testme
+
 ----
 
 automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.7.0 or newer
 
@@ -117,15 +160,15 @@
 
 You might try it right away in Jupyter Notebook by using the "launch binder" badge, or click `here <https://mybinder.org/v2/gh/{{rst_include.
 repository_slug}}/master?filepath=lib_programname.ipynb>`_
 
 Usage
 -----------
 
-.. code-block:: py
+.. code-block:: python
 
     import lib_programname
     # this returns the fully resolved path to the launched python program
     path_to_program = lib_programname.get_path_executed_script()    # type: pathlib.Path
 
 Usage from Commandline
 ------------------------
@@ -254,14 +297,21 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.7
+---------
+2023-07-12:
+    - also works now with symlinks
+    - also works now with scripts and symlinks which do not have a ``py`` extension
+    - clean ./tests/test_cli.py
+
 v2.0.6
 ---------
 2023-07-12:
     - introduce PEP517 packaging standard
     - introduce pyproject.toml build-system
     - remove mypy.ini
     - remove pytest.ini
```

### Comparing `lib_programname-2.0.6/lib_programname.egg-info/SOURCES.txt` & `lib_programname-2.0.7/lib_programname.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/lib_programname.ipynb` & `lib_programname-2.0.7/lib_programname.ipynb`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/pyproject.toml` & `lib_programname-2.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,36 +26,36 @@
 # dependencies - former setup.cfg "install_requires"
 # see: https://setuptools.pypa.io/en/latest/userguide/dependency_management.html
 dependencies = [
     "click",
     "cli_exit_tools",
     "lib_detect_testenv",
 ]
-version = "v2.0.6"
+version = "v2.0.7"
 # seems to be not allowed anymore
 # zip-save = false
 
 [project.urls]
 Homepage = "https://github.com/bitranox/lib_programname"
 Documentation = "https://github.com/bitranox/lib_programname/blob/master/README.rst"
 Repository = "https://github.com/bitranox/lib_programname.git"
 Changelog = "https://github.com/bitranox/lib_programname/blob/master/CHANGES.rst"
 
 [project.optional-dependencies]
 test = [
-    "black ; platform_python_implementation != 'PyPy'",
-    "black==19.3b0 ; platform_python_implementation == 'PyPy'",
+    "black",
     "codecov",
     "coloredlogs",
     "coverage",
     "flake8",
     "mypy ; platform_python_implementation != 'PyPy'",
     "pytest",
     "pytest-cov",
     "pytest-runner",
+    "readme_renderer",
 ]
 
 [project.scripts]
     lib_programname = "lib_programname.lib_programname_cli:cli_main"
 
 [tool.setuptools.package-data]
 lib_programname = [
```

### Comparing `lib_programname-2.0.6/tests/local_testscripts/lib_bash_functions.sh` & `lib_programname-2.0.7/tests/local_testscripts/lib_bash_functions.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/tests/local_testscripts/run_pytest.sh` & `lib_programname-2.0.7/tests/local_testscripts/run_pytest.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/tests/local_testscripts/run_testloop.sh` & `lib_programname-2.0.7/tests/local_testscripts/run_testloop.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh` & `lib_programname-2.0.7/tests/local_testscripts/run_testloop_pytest_and_mypy_only_no_setup.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/tests/local_testscripts/run_testloop_windows.cmd` & `lib_programname-2.0.7/tests/local_testscripts/run_testloop_windows.cmd`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/tests/local_testscripts/shellcheck.sh` & `lib_programname-2.0.7/tests/local_testscripts/shellcheck.sh`

 * *Files identical despite different names*

### Comparing `lib_programname-2.0.6/tests/local_testscripts/testing_tools.py` & `lib_programname-2.0.7/tests/local_testscripts/testing_tools.py`

 * *Files identical despite different names*


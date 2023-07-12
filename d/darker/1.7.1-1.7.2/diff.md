# Comparing `tmp/darker-1.7.1.tar.gz` & `tmp/darker-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darker-1.7.1.tar", last modified: Sun Mar 26 10:30:06 2023, max compression
+gzip compressed data, was "darker-1.7.2.tar", last modified: Wed Jul 12 18:50:34 2023, max compression
```

## Comparing `darker-1.7.1.tar` & `darker-1.7.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 kaiant    (1000) users      (100)        0 2023-03-26 10:30:06.539685 darker-1.7.1/
--rw-rw-r--   0 kaiant    (1000) users      (100)     1556 2020-08-04 21:32:02.000000 darker-1.7.1/LICENSE.rst
--rw-r--r--   0 kaiant    (1000) users      (100)    37493 2023-03-26 10:30:06.540685 darker-1.7.1/PKG-INFO
--rw-r--r--   0 kaiant    (1000) users      (100)    75593 2023-03-26 10:29:35.000000 darker-1.7.1/README.rst
--rw-r--r--   0 kaiant    (1000) users      (100)      351 2023-01-06 22:36:53.000000 darker-1.7.1/pyproject.toml
--rw-r--r--   0 kaiant    (1000) users      (100)     2242 2023-03-26 10:30:06.540685 darker-1.7.1/setup.cfg
--rw-r--r--   0 kaiant    (1000) users      (100)     1792 2023-01-15 21:17:32.000000 darker-1.7.1/setup.py
-drwxr-xr-x   0 kaiant    (1000) users      (100)        0 2023-03-26 10:30:06.537685 darker-1.7.1/src/
-drwxr-xr-x   0 kaiant    (1000) users      (100)        0 2023-03-26 10:30:06.538685 darker-1.7.1/src/darker/
--rw-r--r--   0 kaiant    (1000) users      (100)        0 2023-02-09 12:28:35.000000 darker-1.7.1/src/darker/__init__.py
--rw-r--r--   0 kaiant    (1000) users      (100)    25625 2023-03-26 09:52:21.000000 darker-1.7.1/src/darker/__main__.py
--rw-r--r--   0 kaiant    (1000) users      (100)     3624 2023-02-09 12:28:35.000000 darker-1.7.1/src/darker/argparse_helpers.py
--rw-r--r--   0 kaiant    (1000) users      (100)      651 2023-02-09 12:28:35.000000 darker-1.7.1/src/darker/black_compat.py
--rw-r--r--   0 kaiant    (1000) users      (100)     8332 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/black_diff.py
--rw-r--r--   0 kaiant    (1000) users      (100)     2955 2023-02-09 12:28:35.000000 darker-1.7.1/src/darker/chooser.py
--rw-r--r--   0 kaiant    (1000) users      (100)     6243 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/command_line.py
--rw-r--r--   0 kaiant    (1000) users      (100)     2354 2023-02-09 12:28:35.000000 darker-1.7.1/src/darker/concurrency.py
--rw-r--r--   0 kaiant    (1000) users      (100)     7461 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/config.py
--rw-r--r--   0 kaiant    (1000) users      (100)     9106 2023-02-11 17:17:18.000000 darker-1.7.1/src/darker/diff.py
--rw-r--r--   0 kaiant    (1000) users      (100)      436 2023-02-12 20:44:59.000000 darker-1.7.1/src/darker/exceptions.py
--rw-r--r--   0 kaiant    (1000) users      (100)     2545 2023-03-25 19:32:04.000000 darker-1.7.1/src/darker/fstring.py
--rw-r--r--   0 kaiant    (1000) users      (100)    24531 2023-03-26 10:11:15.000000 darker-1.7.1/src/darker/git.py
--rw-r--r--   0 kaiant    (1000) users      (100)     5283 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/help.py
-drwxr-xr-x   0 kaiant    (1000) users      (100)        0 2023-03-26 10:30:06.538685 darker-1.7.1/src/darker/highlighting/
--rw-r--r--   0 kaiant    (1000) users      (100)     1869 2023-02-09 12:28:35.000000 darker-1.7.1/src/darker/highlighting/__init__.py
--rw-r--r--   0 kaiant    (1000) users      (100)     3105 2023-02-09 12:28:35.000000 darker-1.7.1/src/darker/highlighting/lexers.py
--rw-r--r--   0 kaiant    (1000) users      (100)     6330 2023-02-11 17:17:18.000000 darker-1.7.1/src/darker/import_sorting.py
--rw-r--r--   0 kaiant    (1000) users      (100)    20925 2023-03-26 10:11:15.000000 darker-1.7.1/src/darker/linting.py
--rw-r--r--   0 kaiant    (1000) users      (100)     2043 2023-02-09 12:28:35.000000 darker-1.7.1/src/darker/multiline_strings.py
-drwxr-xr-x   0 kaiant    (1000) users      (100)        0 2023-03-26 10:30:06.539685 darker-1.7.1/src/darker/tests/
--rw-r--r--   0 kaiant    (1000) users      (100)        0 2023-02-09 12:28:35.000000 darker-1.7.1/src/darker/tests/__init__.py
--rw-r--r--   0 kaiant    (1000) users      (100)     5489 2023-03-25 19:30:24.000000 darker-1.7.1/src/darker/tests/conftest.py
--rw-r--r--   0 kaiant    (1000) users      (100)     1044 2023-02-09 12:28:35.000000 darker-1.7.1/src/darker/tests/git_diff_example_output.py
--rw-r--r--   0 kaiant    (1000) users      (100)     3488 2023-02-11 17:17:18.000000 darker-1.7.1/src/darker/tests/helpers.py
--rw-r--r--   0 kaiant    (1000) users      (100)     3448 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/tests/test_argparse_helpers.py
--rw-r--r--   0 kaiant    (1000) users      (100)    11185 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/tests/test_black_diff.py
--rw-r--r--   0 kaiant    (1000) users      (100)     1105 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/tests/test_chooser.py
--rw-r--r--   0 kaiant    (1000) users      (100)    28886 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/tests/test_command_line.py
--rw-r--r--   0 kaiant    (1000) users      (100)     1479 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/tests/test_concurrency.py
--rw-r--r--   0 kaiant    (1000) users      (100)    20795 2023-03-26 09:52:21.000000 darker-1.7.1/src/darker/tests/test_config.py
--rw-r--r--   0 kaiant    (1000) users      (100)     9329 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/tests/test_diff.py
--rw-r--r--   0 kaiant    (1000) users      (100)     1625 2023-02-09 12:28:35.000000 darker-1.7.1/src/darker/tests/test_difflib.py
--rw-r--r--   0 kaiant    (1000) users      (100)     1767 2023-03-25 08:36:08.000000 darker-1.7.1/src/darker/tests/test_fstring.py
--rw-r--r--   0 kaiant    (1000) users      (100)    39137 2023-03-26 10:11:15.000000 darker-1.7.1/src/darker/tests/test_git.py
--rw-r--r--   0 kaiant    (1000) users      (100)    21585 2023-03-26 10:11:15.000000 darker-1.7.1/src/darker/tests/test_highlighting.py
--rw-r--r--   0 kaiant    (1000) users      (100)     9005 2023-03-25 19:30:24.000000 darker-1.7.1/src/darker/tests/test_import_sorting.py
--rw-r--r--   0 kaiant    (1000) users      (100)    19638 2023-03-26 09:52:21.000000 darker-1.7.1/src/darker/tests/test_linting.py
--rw-r--r--   0 kaiant    (1000) users      (100)    30010 2023-03-26 09:52:21.000000 darker-1.7.1/src/darker/tests/test_main.py
--rw-r--r--   0 kaiant    (1000) users      (100)     5747 2023-03-26 09:52:21.000000 darker-1.7.1/src/darker/tests/test_main_blacken_and_flynt_single_file.py
--rw-r--r--   0 kaiant    (1000) users      (100)     5014 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/tests/test_main_revision.py
--rw-r--r--   0 kaiant    (1000) users      (100)     5169 2023-03-26 09:52:21.000000 darker-1.7.1/src/darker/tests/test_main_stdin_filename.py
--rw-r--r--   0 kaiant    (1000) users      (100)     5300 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/tests/test_multiline_strings.py
--rw-r--r--   0 kaiant    (1000) users      (100)    14270 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/tests/test_utils.py
--rw-r--r--   0 kaiant    (1000) users      (100)     2221 2023-03-25 18:49:56.000000 darker-1.7.1/src/darker/tests/test_verification.py
--rw-r--r--   0 kaiant    (1000) users      (100)     9178 2023-02-09 12:28:35.000000 darker-1.7.1/src/darker/utils.py
--rw-r--r--   0 kaiant    (1000) users      (100)     3201 2023-02-09 12:28:35.000000 darker-1.7.1/src/darker/verification.py
--rw-r--r--   0 kaiant    (1000) users      (100)       84 2023-03-26 10:29:35.000000 darker-1.7.1/src/darker/version.py
-drwxr-xr-x   0 kaiant    (1000) users      (100)        0 2023-03-26 10:30:06.538685 darker-1.7.1/src/darker.egg-info/
--rw-rw-r--   0 kaiant    (1000) users      (100)    37493 2023-03-26 10:30:06.000000 darker-1.7.1/src/darker.egg-info/PKG-INFO
--rw-rw-r--   0 kaiant    (1000) users      (100)     1682 2023-03-26 10:30:06.000000 darker-1.7.1/src/darker.egg-info/SOURCES.txt
--rw-rw-r--   0 kaiant    (1000) users      (100)        1 2023-03-26 10:30:06.000000 darker-1.7.1/src/darker.egg-info/dependency_links.txt
--rw-rw-r--   0 kaiant    (1000) users      (100)      207 2023-03-26 10:30:06.000000 darker-1.7.1/src/darker.egg-info/entry_points.txt
--rw-rw-r--   0 kaiant    (1000) users      (100)      534 2023-03-26 10:30:06.000000 darker-1.7.1/src/darker.egg-info/requires.txt
--rw-rw-r--   0 kaiant    (1000) users      (100)        7 2023-03-26 10:30:06.000000 darker-1.7.1/src/darker.egg-info/top_level.txt
+drwxr-xr-x   0 kaiant    (1000) users      (100)        0 2023-07-12 18:50:34.008976 darker-1.7.2/
+-rw-rw-r--   0 kaiant    (1000) users      (100)     1556 2020-08-04 21:32:02.000000 darker-1.7.2/LICENSE.rst
+-rw-r--r--   0 kaiant    (1000) users      (100)    37590 2023-07-12 18:50:34.009976 darker-1.7.2/PKG-INFO
+-rw-r--r--   0 kaiant    (1000) users      (100)    78145 2023-07-12 18:50:22.000000 darker-1.7.2/README.rst
+-rw-r--r--   0 kaiant    (1000) users      (100)      351 2023-07-12 18:50:18.000000 darker-1.7.2/pyproject.toml
+-rw-r--r--   0 kaiant    (1000) users      (100)     2360 2023-07-12 18:50:34.009976 darker-1.7.2/setup.cfg
+-rw-r--r--   0 kaiant    (1000) users      (100)     1792 2023-01-15 21:17:32.000000 darker-1.7.2/setup.py
+drwxr-xr-x   0 kaiant    (1000) users      (100)        0 2023-07-12 18:50:34.005976 darker-1.7.2/src/
+drwxr-xr-x   0 kaiant    (1000) users      (100)        0 2023-07-12 18:50:34.007976 darker-1.7.2/src/darker/
+-rw-r--r--   0 kaiant    (1000) users      (100)        0 2023-02-09 12:28:35.000000 darker-1.7.2/src/darker/__init__.py
+-rw-r--r--   0 kaiant    (1000) users      (100)    25625 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/__main__.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     3624 2023-05-30 06:05:50.000000 darker-1.7.2/src/darker/argparse_helpers.py
+-rw-r--r--   0 kaiant    (1000) users      (100)      651 2023-02-09 12:28:35.000000 darker-1.7.2/src/darker/black_compat.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     8332 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/black_diff.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     2955 2023-06-30 18:58:38.000000 darker-1.7.2/src/darker/chooser.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     6243 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/command_line.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     2354 2023-02-09 12:28:35.000000 darker-1.7.2/src/darker/concurrency.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     7477 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/config.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     9106 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/diff.py
+-rw-r--r--   0 kaiant    (1000) users      (100)      436 2023-02-12 20:44:59.000000 darker-1.7.2/src/darker/exceptions.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     2545 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/fstring.py
+-rw-r--r--   0 kaiant    (1000) users      (100)    24537 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/git.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     5283 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/help.py
+drwxr-xr-x   0 kaiant    (1000) users      (100)        0 2023-07-12 18:50:34.007976 darker-1.7.2/src/darker/highlighting/
+-rw-r--r--   0 kaiant    (1000) users      (100)     1869 2023-02-09 12:28:35.000000 darker-1.7.2/src/darker/highlighting/__init__.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     3105 2023-02-09 12:28:35.000000 darker-1.7.2/src/darker/highlighting/lexers.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     6330 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/import_sorting.py
+-rw-r--r--   0 kaiant    (1000) users      (100)    20937 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/linting.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     2579 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/multiline_strings.py
+drwxr-xr-x   0 kaiant    (1000) users      (100)        0 2023-07-12 18:50:34.008976 darker-1.7.2/src/darker/tests/
+-rw-r--r--   0 kaiant    (1000) users      (100)        0 2023-02-09 12:28:35.000000 darker-1.7.2/src/darker/tests/__init__.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     5489 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/conftest.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     1044 2023-05-30 06:06:12.000000 darker-1.7.2/src/darker/tests/git_diff_example_output.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     3488 2023-02-11 17:17:18.000000 darker-1.7.2/src/darker/tests/helpers.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     3448 2023-05-30 06:06:12.000000 darker-1.7.2/src/darker/tests/test_argparse_helpers.py
+-rw-r--r--   0 kaiant    (1000) users      (100)    11185 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_black_diff.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     1105 2023-03-25 18:49:56.000000 darker-1.7.2/src/darker/tests/test_chooser.py
+-rw-r--r--   0 kaiant    (1000) users      (100)    28886 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_command_line.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     1479 2023-03-25 18:49:56.000000 darker-1.7.2/src/darker/tests/test_concurrency.py
+-rw-r--r--   0 kaiant    (1000) users      (100)    20795 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_config.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     9329 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_diff.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     1625 2023-02-09 12:28:35.000000 darker-1.7.2/src/darker/tests/test_difflib.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     1767 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_fstring.py
+-rw-r--r--   0 kaiant    (1000) users      (100)    39137 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_git.py
+-rw-r--r--   0 kaiant    (1000) users      (100)    21585 2023-06-07 20:34:17.000000 darker-1.7.2/src/darker/tests/test_highlighting.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     9005 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_import_sorting.py
+-rw-r--r--   0 kaiant    (1000) users      (100)    20851 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_linting.py
+-rw-r--r--   0 kaiant    (1000) users      (100)    30010 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_main.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     5747 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_main_blacken_and_flynt_single_file.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     5014 2023-03-25 18:49:56.000000 darker-1.7.2/src/darker/tests/test_main_revision.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     5390 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_main_stdin_filename.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     5306 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_multiline_strings.py
+-rw-r--r--   0 kaiant    (1000) users      (100)    14270 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_utils.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     2221 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/tests/test_verification.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     9178 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/utils.py
+-rw-r--r--   0 kaiant    (1000) users      (100)     3201 2023-07-12 18:50:18.000000 darker-1.7.2/src/darker/verification.py
+-rw-r--r--   0 kaiant    (1000) users      (100)       84 2023-07-12 18:50:22.000000 darker-1.7.2/src/darker/version.py
+drwxr-xr-x   0 kaiant    (1000) users      (100)        0 2023-07-12 18:50:34.007976 darker-1.7.2/src/darker.egg-info/
+-rw-rw-r--   0 kaiant    (1000) users      (100)    37590 2023-07-12 18:50:33.000000 darker-1.7.2/src/darker.egg-info/PKG-INFO
+-rw-rw-r--   0 kaiant    (1000) users      (100)     1682 2023-07-12 18:50:33.000000 darker-1.7.2/src/darker.egg-info/SOURCES.txt
+-rw-rw-r--   0 kaiant    (1000) users      (100)        1 2023-07-12 18:50:33.000000 darker-1.7.2/src/darker.egg-info/dependency_links.txt
+-rw-rw-r--   0 kaiant    (1000) users      (100)      207 2023-07-12 18:50:33.000000 darker-1.7.2/src/darker.egg-info/entry_points.txt
+-rw-rw-r--   0 kaiant    (1000) users      (100)      570 2023-07-12 18:50:33.000000 darker-1.7.2/src/darker.egg-info/requires.txt
+-rw-rw-r--   0 kaiant    (1000) users      (100)        7 2023-07-12 18:50:33.000000 darker-1.7.2/src/darker.egg-info/top_level.txt
```

### Comparing `darker-1.7.1/LICENSE.rst` & `darker-1.7.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/PKG-INFO` & `darker-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: darker
-Version: 1.7.1
+Version: 1.7.2
 Summary: Apply Black formatting only in regions changed since last commit
 Home-page: https://github.com/akaihola/darker
 Author: Antti Kaihola
 Author-email: 13725+akaihola@users.noreply.github.com
 License: BSD
 Project-URL: Source Code, https://github.com/akaihola/darker
 Project-URL: Change Log, https://github.com/akaihola/darker/blob/master/CHANGES.rst
+Project-URL: News, https://github.com/akaihola/darker/discussions/categories/announcements
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
@@ -43,17 +44,17 @@
 .. _downloads-badge: https://pepy.tech/project/darker
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
 .. _black-badge: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
 .. _changelog-badge: https://github.com/akaihola/darker/blob/master/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darker/23?color=red&label=release%201.7.2
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darker/21?color=red&label=release%201.8.0
    :alt: Next milestone
-.. _next-milestone: https://github.com/akaihola/darker/milestone/23
+.. _next-milestone: https://github.com/akaihola/darker/milestone/21
 
 
 What?
 =====
 
 This utility reformats and checks Python source code files.
 However, when run in a Git repository, it compares an old revision of the source tree
@@ -144,19 +145,19 @@
 .. _@ambv: https://github.com/ambv
 
 How?
 ====
 
 To install or upgrade, use::
 
-  pip install --upgrade darker~=1.7.1
+  pip install --upgrade darker~=1.7.2
 
 Or, if you're using Conda_ for package management::
 
-  conda install -c conda-forge darker~=1.7.1 isort
+  conda install -c conda-forge darker~=1.7.2 isort
   conda update -c conda-forge darker
 
 ..
 
     **Note:** It is recommended to use the '``~=``' "`compatible release`_" version
     specifier for Darker. See `Guarding against Black compatibility breakage`_ for more
     information.
@@ -380,16 +381,16 @@
 --skip-magic-trailing-comma
        Skip adding trailing commas to expressions that are split by comma where each
        element is on its own line. This includes function signatures. This can be used
        to override ``skip_magic_trailing_comma = true`` from a configuration file.
 -l LENGTH, --line-length LENGTH
        How many characters per line to allow [default: 88]
 -t VERSION, --target-version VERSION
-       [py33|py34|py35|py36|py37|py38|py39|py310|py311] Python versions that should be
-       supported by Black's output. [default: per-file auto-detection]
+       [py33|py34|py35|py36|py37|py38|py39|py310|py311|py312] Python versions that
+       should be supported by Black's output. [default: per-file auto-detection]
 -W WORKERS, --workers WORKERS
        How many parallel workers to allow, or ``0`` for one per core [default: 1]
 
 To change default values for these options for a given project,
 add a ``[tool.darker]`` or ``[tool.black]`` section to ``pyproject.toml`` in the
 project's root directory, or to a different TOML file specified using the ``-c`` /
 ``--config`` option. For example:
@@ -645,15 +646,15 @@
        pre-commit sample-config >.pre-commit-config.yaml
 
 3. Append to the created ``.pre-commit-config.yaml`` the following lines:
 
    .. code-block:: yaml
 
       - repo: https://github.com/akaihola/darker
-        rev: 1.7.1
+        rev: 1.7.2
         hooks:
           - id: darker
 
 4. install the Git hook scripts and update to the newest version::
 
        pre-commit install
        pre-commit autoupdate
@@ -664,15 +665,15 @@
 
 If you'd prefer to not update but keep a stable pre-commit setup, you can pin Black and
 other reformatter/linter tools you use to known compatible versions, for example:
 
 .. code-block:: yaml
 
    - repo: https://github.com/akaihola/darker
-     rev: 1.7.1
+     rev: 1.7.2
      hooks:
        - id: darker
          args:
            - --isort
            - --lint mypy
            - --lint flake8
            - --lint pylint
@@ -692,15 +693,15 @@
 
 You can provide arguments, such as enabling isort, by specifying ``args``.
 Note the inclusion of the isort Python package under ``additional_dependencies``:
 
 .. code-block:: yaml
 
    - repo: https://github.com/akaihola/darker
-     rev: 1.7.1
+     rev: 1.7.2
      hooks:
        - id: darker
          args: [--isort]
          additional_dependencies:
            - isort~=5.9
 
 
@@ -737,19 +738,19 @@
      lint:
        runs-on: ubuntu-latest
        steps:
          - uses: actions/checkout@v3
            with:
              fetch-depth: 0 
          - uses: actions/setup-python@v4
-         - uses: akaihola/darker@1.7.1
+         - uses: akaihola/darker@1.7.2
            with:
              options: "--check --diff --isort --color"
              src: "./src"
-             version: "~=1.7.1"
+             version: "~=1.7.2"
              lint: "flake8,pylint==2.13.1"
 
 There needs to be a working Python environment, set up using ``actions/setup-python``
 in the above example. Darker will be installed in an isolated virtualenv to prevent
 conflicts with other workflows.
 
 ``"uses:"`` specifies which Darker release to get the GitHub Action definition from.
```

### Comparing `darker-1.7.1/README.rst` & `darker-1.7.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 .. _downloads-badge: https://pepy.tech/project/darker
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
 .. _black-badge: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
 .. _changelog-badge: https://github.com/akaihola/darker/blob/master/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darker/23?color=red&label=release%201.7.2
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darker/21?color=red&label=release%201.8.0
    :alt: Next milestone
-.. _next-milestone: https://github.com/akaihola/darker/milestone/23
+.. _next-milestone: https://github.com/akaihola/darker/milestone/21
 
 
 What?
 =====
 
 This utility reformats and checks Python source code files.
 However, when run in a Git repository, it compares an old revision of the source tree
@@ -133,19 +133,19 @@
 .. _@ambv: https://github.com/ambv
 
 How?
 ====
 
 To install or upgrade, use::
 
-  pip install --upgrade darker~=1.7.1
+  pip install --upgrade darker~=1.7.2
 
 Or, if you're using Conda_ for package management::
 
-  conda install -c conda-forge darker~=1.7.1 isort
+  conda install -c conda-forge darker~=1.7.2 isort
   conda update -c conda-forge darker
 
 ..
 
     **Note:** It is recommended to use the '``~=``' "`compatible release`_" version
     specifier for Darker. See `Guarding against Black compatibility breakage`_ for more
     information.
@@ -369,16 +369,16 @@
 --skip-magic-trailing-comma
        Skip adding trailing commas to expressions that are split by comma where each
        element is on its own line. This includes function signatures. This can be used
        to override ``skip_magic_trailing_comma = true`` from a configuration file.
 -l LENGTH, --line-length LENGTH
        How many characters per line to allow [default: 88]
 -t VERSION, --target-version VERSION
-       [py33|py34|py35|py36|py37|py38|py39|py310|py311] Python versions that should be
-       supported by Black's output. [default: per-file auto-detection]
+       [py33|py34|py35|py36|py37|py38|py39|py310|py311|py312] Python versions that
+       should be supported by Black's output. [default: per-file auto-detection]
 -W WORKERS, --workers WORKERS
        How many parallel workers to allow, or ``0`` for one per core [default: 1]
 
 To change default values for these options for a given project,
 add a ``[tool.darker]`` or ``[tool.black]`` section to ``pyproject.toml`` in the
 project's root directory, or to a different TOML file specified using the ``-c`` /
 ``--config`` option. For example:
@@ -634,15 +634,15 @@
        pre-commit sample-config >.pre-commit-config.yaml
 
 3. Append to the created ``.pre-commit-config.yaml`` the following lines:
 
    .. code-block:: yaml
 
       - repo: https://github.com/akaihola/darker
-        rev: 1.7.1
+        rev: 1.7.2
         hooks:
           - id: darker
 
 4. install the Git hook scripts and update to the newest version::
 
        pre-commit install
        pre-commit autoupdate
@@ -653,15 +653,15 @@
 
 If you'd prefer to not update but keep a stable pre-commit setup, you can pin Black and
 other reformatter/linter tools you use to known compatible versions, for example:
 
 .. code-block:: yaml
 
    - repo: https://github.com/akaihola/darker
-     rev: 1.7.1
+     rev: 1.7.2
      hooks:
        - id: darker
          args:
            - --isort
            - --lint mypy
            - --lint flake8
            - --lint pylint
@@ -681,15 +681,15 @@
 
 You can provide arguments, such as enabling isort, by specifying ``args``.
 Note the inclusion of the isort Python package under ``additional_dependencies``:
 
 .. code-block:: yaml
 
    - repo: https://github.com/akaihola/darker
-     rev: 1.7.1
+     rev: 1.7.2
      hooks:
        - id: darker
          args: [--isort]
          additional_dependencies:
            - isort~=5.9
 
 
@@ -726,19 +726,19 @@
      lint:
        runs-on: ubuntu-latest
        steps:
          - uses: actions/checkout@v3
            with:
              fetch-depth: 0 
          - uses: actions/setup-python@v4
-         - uses: akaihola/darker@1.7.1
+         - uses: akaihola/darker@1.7.2
            with:
              options: "--check --diff --isort --color"
              src: "./src"
-             version: "~=1.7.1"
+             version: "~=1.7.2"
              lint: "flake8,pylint==2.13.1"
 
 There needs to be a working Python environment, set up using ``actions/setup-python``
 in the above example. Darker will be installed in an isolated virtualenv to prevent
 conflicts with other workflows.
 
 ``"uses:"`` specifies which Darker release to get the GitHub Action definition from.
@@ -1096,14 +1096,25 @@
              <b>Bharat Kunwar</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+reviewed-by%3Abrtknr" title="Reviewed Pull Requests">👀</a>
        </td>
        <td align="center">
+         <a href="https://github.com/bdperkin">
+           <img src="https://avatars.githubusercontent.com/u/3385145?v=3" width="100px;" alt="@bdperkin" />
+           <br />
+           <sub>
+             <b>Brandon Perkins</b>
+           </sub>
+         </a>
+         <br />
+         <a href="https://github.com/akaihola/darker/issues?q=author%3Abdperkin" title="Bug reports">🐛</a>
+       </td>
+       <td align="center">
          <a href="https://github.com/casio">
            <img src="https://avatars.githubusercontent.com/u/29784?v=3" width="100px;" alt="@casio" />
            <br />
            <sub>
              <b>Carsten Kraus</b>
            </sub>
          </a>
@@ -1118,27 +1129,27 @@
              <b>Chmouel Boudjnah</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+author%3Achmouel" title="Code">💻</a>
          <a href="https://github.com/akaihola/darker/issues?q=author%3Achmouel" title="Bug reports">🐛</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/cclauss">
            <img src="https://avatars.githubusercontent.com/u/3709715?v=3" width="100px;" alt="@cclauss" />
            <br />
            <sub>
              <b>Christian Clauss</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+author%3Acclauss" title="Code">💻</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/chrisdecker1201">
            <img src="https://avatars.githubusercontent.com/u/20707614?v=3" width="100px;" alt="@chrisdecker1201" />
            <br />
            <sub>
              <b>Christian Decker</b>
            </sub>
@@ -1189,28 +1200,28 @@
            <sub>
              <b>David Dreher</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3ADavidCDreher" title="Bug reports">🐛</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/shangxiao">
            <img src="https://avatars.githubusercontent.com/u/1845938?v=3" width="100px;" alt="@shangxiao" />
            <br />
            <sub>
              <b>David Sanders</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+author%3Ashangxiao" title="Code">💻</a>
          <a href="https://github.com/akaihola/darker/issues?q=author%3Ashangxiao" title="Bug reports">🐛</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/dhrvjha">
            <img src="https://avatars.githubusercontent.com/u/43818577?v=3" width="100px;" alt="@dhrvjha" />
            <br />
            <sub>
              <b>Dhruv Kumar Jha</b>
            </sub>
@@ -1259,27 +1270,27 @@
            <sub>
              <b>Eric Riddoch</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Aphitoduck" title="Bug reports">🐛</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/philipgian">
            <img src="https://avatars.githubusercontent.com/u/6884633?v=3" width="100px;" alt="@philipgian" />
            <br />
            <sub>
              <b>Filippos Giannakos</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+author%3Aphilipgian" title="Code">💻</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/foxwhite25">
            <img src="https://avatars.githubusercontent.com/u/39846845?v=3" width="100px;" alt="@foxwhite25" />
            <br />
            <sub>
              <b>Fox_white</b>
            </sub>
@@ -1328,27 +1339,27 @@
            <sub>
              <b>Hugo van Kemenade</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+author%3Ahugovk" title="Code">💻</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/irynahryshanovich">
            <img src="https://avatars.githubusercontent.com/u/62266480?v=3" width="100px;" alt="@irynahryshanovich" />
            <br />
            <sub>
              <b>Iryna</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Airynahryshanovich" title="Bug reports">🐛</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/yajo">
            <img src="https://avatars.githubusercontent.com/u/973709?v=3" width="100px;" alt="@yajo" />
            <br />
            <sub>
              <b>Jairo Llopis</b>
            </sub>
@@ -1397,27 +1408,27 @@
            <sub>
              <b>Kentaro Wada</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Awkentaro" title="Bug reports">🐛</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/Asuskf">
            <img src="https://avatars.githubusercontent.com/u/36687747?v=3" width="100px;" alt="@Asuskf" />
            <br />
            <sub>
              <b>Kevin David</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/discussions?discussions_q=author%3AAsuskf" title="Bug reports">🐛</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/Krischtopp">
            <img src="https://avatars.githubusercontent.com/u/56152637?v=3" width="100px;" alt="@Krischtopp" />
            <br />
            <sub>
              <b>Krischtopp</b>
            </sub>
@@ -1455,14 +1466,27 @@
              <b>Mark Davidoff</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Amarkddavidoff" title="Bug reports">🐛</a>
        </td>
        <td align="center">
+         <a href="https://github.com/dwt">
+           <img src="https://avatars.githubusercontent.com/u/57199?v=3" width="100px;" alt="@dwt" />
+           <br />
+           <sub>
+             <b>Martin Häcker</b>
+           </sub>
+         </a>
+         <br />
+         <a href="https://github.com/akaihola/darker/issues?q=author%3Adwt" title="Bug reports">🐛</a>
+       </td>
+     </tr>
+     <tr>
+       <td align="center">
          <a href="https://github.com/matclayton">
            <img src="https://avatars.githubusercontent.com/u/126218?v=3" width="100px;" alt="@matclayton" />
            <br />
            <sub>
              <b>Mat Clayton</b>
            </sub>
          </a>
@@ -1478,16 +1502,14 @@
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/commits?author=Carreau" title="Code">💻</a>
          <a href="https://github.com/akaihola/darker/commits?author=Carreau" title="Documentation">📖</a>
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+reviewed-by%3ACarreau" title="Reviewed Pull Requests">👀</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/MatthijsBurgh">
            <img src="https://avatars.githubusercontent.com/u/18014833?v=3" width="100px;" alt="@MatthijsBurgh" />
            <br />
            <sub>
              <b>Matthijs van der Burgh</b>
            </sub>
@@ -1503,26 +1525,39 @@
              <b>Min RK</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/conda-forge/darker-feedstock/search?q=darker+author%3Aminrk&type=issues" title="Code">💻</a>
        </td>
        <td align="center">
+         <a href="https://github.com/my-tien">
+           <img src="https://avatars.githubusercontent.com/u/3898364?v=3" width="100px;" alt="@my-tien" />
+           <br />
+           <sub>
+             <b>My-Tien Nguyen</b>
+           </sub>
+         </a>
+         <br />
+         <a href="https://github.com/akaihola/darker/issues?q=author%3Amy-tien" title="Bug reports">🐛</a>
+       </td>
+       <td align="center">
          <a href="https://github.com/Mystic-Mirage">
            <img src="https://avatars.githubusercontent.com/u/1079805?v=3" width="100px;" alt="@Mystic-Mirage" />
            <br />
            <sub>
              <b>Mystic-Mirage</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/commits?author=Mystic-Mirage" title="Code">💻</a>
          <a href="https://github.com/akaihola/darker/commits?author=Mystic-Mirage" title="Documentation">📖</a>
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+reviewed-by%3AMystic-Mirage" title="Reviewed Pull Requests">👀</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/njhuffman">
            <img src="https://avatars.githubusercontent.com/u/66969728?v=3" width="100px;" alt="@njhuffman" />
            <br />
            <sub>
              <b>Nathan Huffman</b>
            </sub>
@@ -1550,16 +1585,14 @@
              <b>Pacu2</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+author%3APacu2" title="Code">💻</a>
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+reviewed-by%3APacu2" title="Reviewed Pull Requests">👀</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/PatrickJordanCongenica">
            <img src="https://avatars.githubusercontent.com/u/85236670?v=3" width="100px;" alt="@PatrickJordanCongenica" />
            <br />
            <sub>
              <b>Patrick Jordan</b>
            </sub>
@@ -1577,14 +1610,27 @@
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/commits?author=ivanov" title="Code">💻</a>
          <a href="https://github.com/akaihola/darker/issues?q=author%3Aivanov" title="Bug reports">🐛</a>
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+reviewed-by%3Aivanov" title="Reviewed Pull Requests">👀</a>
        </td>
        <td align="center">
+         <a href="https://github.com/gesslerpd">
+           <img src="https://avatars.githubusercontent.com/u/11217948?v=3" width="100px;" alt="@gesslerpd" />
+           <br />
+           <sub>
+             <b>Peter Gessler</b>
+           </sub>
+         </a>
+         <br />
+         <a href="https://github.com/akaihola/darker/issues?q=author%3Agesslerpd" title="Bug reports">🐛</a>
+       </td>
+     </tr>
+     <tr>
+       <td align="center">
          <a href="https://github.com/flying-sheep">
            <img src="https://avatars.githubusercontent.com/u/291575?v=3" width="100px;" alt="@flying-sheep" />
            <br />
            <sub>
              <b>Philipp A.</b>
            </sub>
          </a>
@@ -1620,16 +1666,14 @@
            <sub>
              <b>Ronie Martinez</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Aroniemartinez" title="Bug reports">🐛</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/rossbar">
            <img src="https://avatars.githubusercontent.com/u/1268991?v=3" width="100px;" alt="@rossbar" />
            <br />
            <sub>
              <b>Ross Barnowski</b>
            </sub>
@@ -1644,14 +1688,16 @@
            <sub>
              <b>Sean Hammond</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+reviewed-by%3Asherbie" title="Reviewed Pull Requests">👀</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/hauntsaninja">
            <img src="https://avatars.githubusercontent.com/u/12621235?v=3" width="100px;" alt="@hauntsaninja" />
            <br />
            <sub>
              <b>Shantanu</b>
            </sub>
@@ -1678,37 +1724,48 @@
              <b>Stefaan Lippens</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/pulls?q=is%3Apr+author%3Asoxofaan" title="Documentation">📖</a>
        </td>
        <td align="center">
+         <a href="https://github.com/strzonnek">
+           <img src="https://avatars.githubusercontent.com/u/80001458?v=3" width="100px;" alt="@strzonnek" />
+           <br />
+           <sub>
+             <b>Stephan Trzonnek</b>
+           </sub>
+         </a>
+         <br />
+         <a href="https://github.com/akaihola/darker/issues?q=author%3Astrzonnek" title="Bug reports">🐛</a>
+       </td>
+       <td align="center">
          <a href="https://github.com/tkolleh">
            <img src="https://avatars.githubusercontent.com/u/3095197?v=3" width="100px;" alt="@tkolleh" />
            <br />
            <sub>
              <b>TJ Kolleh</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/issues?q=author%3Atkolleh" title="Bug reports">🐛</a>
        </td>
-     </tr>
-     <tr>
        <td align="center">
          <a href="https://github.com/talhajunaidd">
            <img src="https://avatars.githubusercontent.com/u/6547611?v=3" width="100px;" alt="@talhajunaidd" />
            <br />
            <sub>
              <b>Talha Juanid</b>
            </sub>
          </a>
          <br />
          <a href="https://github.com/akaihola/darker/commits?author=talhajunaidd" title="Code">💻</a>
        </td>
+     </tr>
+     <tr>
        <td align="center">
          <a href="https://github.com/guettli">
            <img src="https://avatars.githubusercontent.com/u/414336?v=3" width="100px;" alt="@guettli" />
            <br />
            <sub>
              <b>Thomas Güttler</b>
            </sub>
@@ -1723,14 +1780,25 @@
            <sub>
              <b>Tobias Diez</b>
            </sub>
          </a>
          <br />
        </td>
        <td align="center">
+         <a href="https://github.com/tapted">
+           <img src="https://avatars.githubusercontent.com/u/1721312?v=3" width="100px;" alt="@tapted" />
+           <br />
+           <sub>
+             <b>Trent Apted</b>
+           </sub>
+         </a>
+         <br />
+         <a href="https://github.com/akaihola/darker/issues?q=author%3Atapted" title="Bug reports">🐛</a>
+       </td>
+       <td align="center">
          <a href="https://github.com/tgross35">
            <img src="https://avatars.githubusercontent.com/u/13724985?v=3" width="100px;" alt="@tgross35" />
            <br />
            <sub>
              <b>Trevor Gross</b>
            </sub>
          </a>
```

### Comparing `darker-1.7.1/setup.cfg` & `darker-1.7.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 project_urls = 
 	Source Code = https://github.com/akaihola/darker
 	Change Log = https://github.com/akaihola/darker/blob/master/CHANGES.rst
+	News = https://github.com/akaihola/darker/discussions/categories/announcements
 url = https://github.com/akaihola/darker
 
 [options]
 include_package_data = True
 package_dir = 
 	=src
 packages = find:
@@ -50,14 +51,16 @@
 test = 
 	airium>=0.2.3
 	black>=21.7b1  # to prevent Mypy error about `gen_python_files`, see issue #189
 	cryptography>=3.3.2  # through twine, fixes CVE-2020-36242
 	defusedxml>=0.7.1
 	flynt>=0.76,<0.78
 	isort>=5.0.1
+	mypy>=0.990
+	pip-requirements-parser
 	pygments
 	pytest>=6.2.0
 	pytest-darker
 	pytest-kwparametrize>=0.0.3
 	regex>=2021.4.4
 	requests_cache>=0.7
 	ruamel.yaml>=0.17.21
```

### Comparing `darker-1.7.1/setup.py` & `darker-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/__main__.py` & `darker-1.7.2/src/darker/__main__.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/argparse_helpers.py` & `darker-1.7.2/src/darker/argparse_helpers.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/black_compat.py` & `darker-1.7.2/src/darker/black_compat.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/black_diff.py` & `darker-1.7.2/src/darker/black_diff.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/chooser.py` & `darker-1.7.2/src/darker/chooser.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/command_line.py` & `darker-1.7.2/src/darker/command_line.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/concurrency.py` & `darker-1.7.2/src/darker/concurrency.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/config.py` & `darker-1.7.2/src/darker/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     )
 
 
 def validate_stdin_src(stdin_filename: Optional[str], src: List[str]) -> None:
     """Make sure both ``stdin`` mode and paths/directories are specified"""
     if stdin_filename is None:
         return
-    if len(src) == 0:
+    if len(src) == 0 or src == ["-"]:
         return
     raise ConfigurationError(
         "No Python source files are allowed when using the `stdin-filename` option"
     )
 
 
 def override_color_with_environment(pyproject_config: DarkerConfig) -> DarkerConfig:
```

### Comparing `darker-1.7.1/src/darker/diff.py` & `darker-1.7.2/src/darker/diff.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/fstring.py` & `darker-1.7.2/src/darker/fstring.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/git.py` & `darker-1.7.2/src/darker/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,15 +559,15 @@
     :param context_lines: The number of lines to include before and after a change
     :return: Line numbers of lines changed between the revision and given content
 
     """
     old = git_get_content_at_revision(path_in_repo, rev1, root)
     # 2. diff the given revisions for the file
     edited_opcodes = diff_and_get_opcodes(old, content)
-    multiline_string_ranges = get_multiline_string_ranges(content)
+    multiline_string_ranges = list(get_multiline_string_ranges(content))
     # 3. extract line numbers in each edited to-file for changed lines
     return list(
         opcodes_to_edit_linenums(edited_opcodes, context_lines, multiline_string_ranges)
     )
 
 
 @lru_cache(maxsize=1)
```

### Comparing `darker-1.7.1/src/darker/help.py` & `darker-1.7.2/src/darker/help.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/highlighting/__init__.py` & `darker-1.7.2/src/darker/highlighting/__init__.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/highlighting/lexers.py` & `darker-1.7.2/src/darker/highlighting/lexers.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/import_sorting.py` & `darker-1.7.2/src/darker/import_sorting.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/linting.py` & `darker-1.7.2/src/darker/linting.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,15 +520,15 @@
     :param root: The root of the Git repository
     :param paths: The files and directories to check, relative to ``root``
     :param revision: The revision to check out
     :return: Linter messages
 
     """
     with TemporaryDirectory() as tmpdir:
-        tmp_path = Path(tmpdir) / "baseline-revision"
+        tmp_path = Path(tmpdir) / "baseline-revision" / root.name
         with git_clone_local(root, revision, tmp_path) as clone_root:
             rev1_commit = git_rev_parse(revision, root)
             result = _get_messages_from_linters(
                 linter_cmdlines,
                 clone_root,
                 paths,
                 make_linter_env(root, rev1_commit),
```

### Comparing `darker-1.7.1/src/darker/multiline_strings.py` & `darker-1.7.2/src/darker/multiline_strings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 """Helper functions for dealing with reformatting multi-line strings"""
-
+import sys
 from tokenize import STRING, tokenize
-from typing import List, Optional, Sequence, Tuple
+from typing import Generator, Optional, Sequence, Tuple
 
 from darker.utils import TextDocument
 
+if sys.version_info >= (3, 12):
+    from tokenize import FSTRING_END, FSTRING_START
+else:
+    FSTRING_START = FSTRING_END = -1
+
+
+MAX_LINES_IN_FILE = 2**64  # make it very unlikely to hit this limit
+
 
-def get_multiline_string_ranges(content: TextDocument) -> List[Tuple[int, int]]:
-    """Return the line ranges of multi-line strings found in the given Python source
+def get_multiline_string_ranges(
+    content: TextDocument,
+) -> Generator[Tuple[int, int], None, None]:
+    """Generate the line ranges of multi-line strings found in the given Python source
 
-    The returned data is 1-based, end-exclusive. In other words, each item is a 1-based
+    The yielded data is 1-based, end-exclusive. In other words, each item is a 1-based
     ``(start, end)`` tuple, ``end`` being the line number following the last line of the
     multi-line string.
 
-    :return: Line number ranges of multi-line strings
+    :param content: The Python source code to scan for multi-line strings
+    :return: Generates the line ranges of multi-line strings
 
     """
     readline = (f"{line}\n".encode(content.encoding) for line in content.lines).__next__
-    return [
-        (t.start[0], t.end[0] + 1)
-        for t in tokenize(readline)
-        if t.type == STRING and t.end[0] > t.start[0]
-    ]
+    token_start_line = MAX_LINES_IN_FILE
+    for token in tokenize(readline):
+        if token.type in {STRING, FSTRING_START}:
+            token_start_line = token.start[0]
+        if token.type in {STRING, FSTRING_END} and token.end[0] > token_start_line:
+            yield token_start_line, token.end[0] + 1
+            token_start_line = MAX_LINES_IN_FILE
 
 
 def find_overlap(
     start: int, end: int, ranges: Sequence[Tuple[int, int]]
 ) -> Optional[Tuple[int, int]]:
     """Return the convex hull of given ranges which overlap with given start and end
```

### Comparing `darker-1.7.1/src/darker/tests/conftest.py` & `darker-1.7.2/src/darker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/git_diff_example_output.py` & `darker-1.7.2/src/darker/tests/git_diff_example_output.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/helpers.py` & `darker-1.7.2/src/darker/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_argparse_helpers.py` & `darker-1.7.2/src/darker/tests/test_argparse_helpers.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_black_diff.py` & `darker-1.7.2/src/darker/tests/test_black_diff.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_chooser.py` & `darker-1.7.2/src/darker/tests/test_chooser.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_command_line.py` & `darker-1.7.2/src/darker/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_concurrency.py` & `darker-1.7.2/src/darker/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_config.py` & `darker-1.7.2/src/darker/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_diff.py` & `darker-1.7.2/src/darker/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_difflib.py` & `darker-1.7.2/src/darker/tests/test_difflib.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_fstring.py` & `darker-1.7.2/src/darker/tests/test_fstring.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_git.py` & `darker-1.7.2/src/darker/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_highlighting.py` & `darker-1.7.2/src/darker/tests/test_highlighting.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_import_sorting.py` & `darker-1.7.2/src/darker/tests/test_import_sorting.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_linting.py` & `darker-1.7.2/src/darker/tests/test_linting.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # pylint: disable=protected-access,too-many-arguments,use-dict-literal
 
 """Unit tests for :mod:`darker.linting`"""
 
 import os
 from pathlib import Path
+from subprocess import PIPE, Popen  # nosec
 from textwrap import dedent
-from typing import Dict, Iterable, List, Tuple, Union
+from typing import Any, Dict, Iterable, List, Tuple, Union
+from unittest.mock import patch
 
 import pytest
 
 from darker import linting
 from darker.git import WORKTREE, RevisionRange
 from darker.linting import (
     DiffLineMapping,
@@ -563,7 +565,39 @@
     a_py = Path("a.py")
     expect = {
         MessageLocation(a_py, 1): [LinterMessage("python", "First line")],
         MessageLocation(a_py, 2): [LinterMessage("python", "EMPTY")],
         MessageLocation(a_py, 3): [LinterMessage("python", "Third line")],
     }
     assert result == expect
+
+
+class AssertEmptyStderrPopen(
+    Popen  # type: ignore[type-arg]
+):  # pylint: disable=too-few-public-methods
+    # When support for Python 3.8 is dropped, inherit `Popen[str]` instead and remove
+    # the `type-arg` ignore above.
+    """A Popen to use for the following test; asserts that its stderr is empty"""
+
+    def __init__(self, args: List[str], **kwargs: Any):  # type: ignore[misc]
+        super().__init__(args, stderr=PIPE, **kwargs)
+        assert self.stderr is not None
+        assert self.stderr.read() == ""
+
+
+def test_get_messages_from_linters_for_baseline_no_mypy_errors(git_repo):
+    """Ensure Mypy does not fail early when ``__init__.py`` is at the repository root
+
+    Regression test for #498
+
+    """
+    git_repo.add({"__init__.py": ""}, commit="Initial commit")
+    initial = git_repo.get_hash()
+    with patch.object(linting, "Popen", AssertEmptyStderrPopen):
+        # end of test setup
+
+        _ = linting._get_messages_from_linters_for_baseline(
+            linter_cmdlines=["mypy"],
+            root=git_repo.root,
+            paths=[Path("__init__.py")],
+            revision=initial,
+        )
```

### Comparing `darker-1.7.1/src/darker/tests/test_main.py` & `darker-1.7.2/src/darker/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_main_blacken_and_flynt_single_file.py` & `darker-1.7.2/src/darker/tests/test_main_blacken_and_flynt_single_file.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_main_revision.py` & `darker-1.7.2/src/darker/tests/test_main_revision.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_main_stdin_filename.py` & `darker-1.7.2/src/darker/tests/test_main_stdin_filename.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,21 @@
             "No Python source files are allowed when using the `stdin-filename` option"
         ),
     ),
     dict(stdin_filename="a.py", expect_a_py='modified = "stdin"\n'),
     dict(
         stdin_filename="a.py", revision="..:STDIN:", expect_a_py='modified = "stdin"\n'
     ),
+    dict(src=["-"], stdin_filename="a.py", expect_a_py='modified = "stdin"\n'),
+    dict(
+        src=["-"],
+        stdin_filename="a.py",
+        revision="..:STDIN:",
+        expect_a_py='modified = "stdin"\n',
+    ),
     dict(
         stdin_filename="a.py",
         revision="..:WORKTREE:",
         expect=ValueError(
             "With --stdin-filename, rev2 in ..:WORKTREE: must be ':STDIN:', not"
             " ':WORKTREE:'"
         ),
```

### Comparing `darker-1.7.1/src/darker/tests/test_multiline_strings.py` & `darker-1.7.2/src/darker/tests/test_multiline_strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             (51, "   quoted"),
             (52, "   six-"),
             (53, "   line"),
             (54, '   string"""'),
         ]
     )
 
-    result = multiline_strings.get_multiline_string_ranges(content)
+    result = list(multiline_strings.get_multiline_string_ranges(content))
 
     assert result == [
         # 1-based, end-exclusive
         (13, 15),
         (15, 17),
         (17, 19),
         (19, 21),
```

### Comparing `darker-1.7.1/src/darker/tests/test_utils.py` & `darker-1.7.2/src/darker/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/tests/test_verification.py` & `darker-1.7.2/src/darker/tests/test_verification.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/utils.py` & `darker-1.7.2/src/darker/utils.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker/verification.py` & `darker-1.7.2/src/darker/verification.py`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker.egg-info/PKG-INFO` & `darker-1.7.2/src/darker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: darker
-Version: 1.7.1
+Version: 1.7.2
 Summary: Apply Black formatting only in regions changed since last commit
 Home-page: https://github.com/akaihola/darker
 Author: Antti Kaihola
 Author-email: 13725+akaihola@users.noreply.github.com
 License: BSD
 Project-URL: Source Code, https://github.com/akaihola/darker
 Project-URL: Change Log, https://github.com/akaihola/darker/blob/master/CHANGES.rst
+Project-URL: News, https://github.com/akaihola/darker/discussions/categories/announcements
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
@@ -43,17 +44,17 @@
 .. _downloads-badge: https://pepy.tech/project/darker
 .. |black-badge| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :alt: Source code formatted using Black
 .. _black-badge: https://github.com/psf/black
 .. |changelog-badge| image:: https://img.shields.io/badge/-change%20log-purple
    :alt: Change log
 .. _changelog-badge: https://github.com/akaihola/darker/blob/master/CHANGES.rst
-.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darker/23?color=red&label=release%201.7.2
+.. |next-milestone| image:: https://img.shields.io/github/milestones/progress/akaihola/darker/21?color=red&label=release%201.8.0
    :alt: Next milestone
-.. _next-milestone: https://github.com/akaihola/darker/milestone/23
+.. _next-milestone: https://github.com/akaihola/darker/milestone/21
 
 
 What?
 =====
 
 This utility reformats and checks Python source code files.
 However, when run in a Git repository, it compares an old revision of the source tree
@@ -144,19 +145,19 @@
 .. _@ambv: https://github.com/ambv
 
 How?
 ====
 
 To install or upgrade, use::
 
-  pip install --upgrade darker~=1.7.1
+  pip install --upgrade darker~=1.7.2
 
 Or, if you're using Conda_ for package management::
 
-  conda install -c conda-forge darker~=1.7.1 isort
+  conda install -c conda-forge darker~=1.7.2 isort
   conda update -c conda-forge darker
 
 ..
 
     **Note:** It is recommended to use the '``~=``' "`compatible release`_" version
     specifier for Darker. See `Guarding against Black compatibility breakage`_ for more
     information.
@@ -380,16 +381,16 @@
 --skip-magic-trailing-comma
        Skip adding trailing commas to expressions that are split by comma where each
        element is on its own line. This includes function signatures. This can be used
        to override ``skip_magic_trailing_comma = true`` from a configuration file.
 -l LENGTH, --line-length LENGTH
        How many characters per line to allow [default: 88]
 -t VERSION, --target-version VERSION
-       [py33|py34|py35|py36|py37|py38|py39|py310|py311] Python versions that should be
-       supported by Black's output. [default: per-file auto-detection]
+       [py33|py34|py35|py36|py37|py38|py39|py310|py311|py312] Python versions that
+       should be supported by Black's output. [default: per-file auto-detection]
 -W WORKERS, --workers WORKERS
        How many parallel workers to allow, or ``0`` for one per core [default: 1]
 
 To change default values for these options for a given project,
 add a ``[tool.darker]`` or ``[tool.black]`` section to ``pyproject.toml`` in the
 project's root directory, or to a different TOML file specified using the ``-c`` /
 ``--config`` option. For example:
@@ -645,15 +646,15 @@
        pre-commit sample-config >.pre-commit-config.yaml
 
 3. Append to the created ``.pre-commit-config.yaml`` the following lines:
 
    .. code-block:: yaml
 
       - repo: https://github.com/akaihola/darker
-        rev: 1.7.1
+        rev: 1.7.2
         hooks:
           - id: darker
 
 4. install the Git hook scripts and update to the newest version::
 
        pre-commit install
        pre-commit autoupdate
@@ -664,15 +665,15 @@
 
 If you'd prefer to not update but keep a stable pre-commit setup, you can pin Black and
 other reformatter/linter tools you use to known compatible versions, for example:
 
 .. code-block:: yaml
 
    - repo: https://github.com/akaihola/darker
-     rev: 1.7.1
+     rev: 1.7.2
      hooks:
        - id: darker
          args:
            - --isort
            - --lint mypy
            - --lint flake8
            - --lint pylint
@@ -692,15 +693,15 @@
 
 You can provide arguments, such as enabling isort, by specifying ``args``.
 Note the inclusion of the isort Python package under ``additional_dependencies``:
 
 .. code-block:: yaml
 
    - repo: https://github.com/akaihola/darker
-     rev: 1.7.1
+     rev: 1.7.2
      hooks:
        - id: darker
          args: [--isort]
          additional_dependencies:
            - isort~=5.9
 
 
@@ -737,19 +738,19 @@
      lint:
        runs-on: ubuntu-latest
        steps:
          - uses: actions/checkout@v3
            with:
              fetch-depth: 0 
          - uses: actions/setup-python@v4
-         - uses: akaihola/darker@1.7.1
+         - uses: akaihola/darker@1.7.2
            with:
              options: "--check --diff --isort --color"
              src: "./src"
-             version: "~=1.7.1"
+             version: "~=1.7.2"
              lint: "flake8,pylint==2.13.1"
 
 There needs to be a working Python environment, set up using ``actions/setup-python``
 in the above example. Darker will be installed in an isolated virtualenv to prevent
 conflicts with other workflows.
 
 ``"uses:"`` specifies which Darker release to get the GitHub Action definition from.
```

### Comparing `darker-1.7.1/src/darker.egg-info/SOURCES.txt` & `darker-1.7.2/src/darker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `darker-1.7.1/src/darker.egg-info/requires.txt` & `darker-1.7.2/src/darker.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 [test]
 airium>=0.2.3
 black>=21.7b1
 cryptography>=3.3.2
 defusedxml>=0.7.1
 flynt<0.78,>=0.76
 isort>=5.0.1
+mypy>=0.990
+pip-requirements-parser
 pygments
 pytest>=6.2.0
 pytest-darker
 pytest-kwparametrize>=0.0.3
 regex>=2021.4.4
 requests_cache>=0.7
 ruamel.yaml>=0.17.21
```


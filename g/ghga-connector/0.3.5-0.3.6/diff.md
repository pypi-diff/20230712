# Comparing `tmp/ghga_connector-0.3.5.tar.gz` & `tmp/ghga_connector-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_connector-0.3.5.tar", last modified: Fri Jun 23 14:27:12 2023, max compression
+gzip compressed data, was "ghga_connector-0.3.6.tar", last modified: Wed Jul 12 13:28:31 2023, max compression
```

## Comparing `ghga_connector-0.3.5.tar` & `ghga_connector-0.3.6.tar`

### file list

```diff
@@ -1,61 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.906450 ghga_connector-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-06-23 14:27:12.906450 ghga_connector-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.898450 ghga_connector-0.3.5/ghga_connector/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.902450 ghga_connector-0.3.5/ghga_connector/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.902450 ghga_connector-0.3.5/ghga_connector/core/api_calls/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/api_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/api_calls/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/api_calls/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/api_calls/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/api_calls/work_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/batch_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/http_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/message_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.898450 ghga_connector-0.3.5/ghga_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-23 14:27:12.910450 ghga_connector-0.3.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.894451 ghga_connector-0.3.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.902450 ghga_connector-0.3.5/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.902450 ghga_connector-0.3.5/tests/fixtures/mock_api/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/mock_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12445 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/mock_api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/mock_api/testcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.906450 ghga_connector-0.3.5/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.906450 ghga_connector-0.3.5/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/integration/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/integration/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/integration/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/integration/test_file_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.906450 ghga_connector-0.3.5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.906450 ghga_connector-0.3.5/tests/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/unit/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/unit/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/unit/test_api_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/unit/test_file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.915959 ghga_connector-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-07-12 13:28:31.915959 ghga_connector-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.907958 ghga_connector-0.3.6/ghga_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/ghga_connector/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/ghga_connector/core/api_calls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/api_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/api_calls/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/api_calls/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/api_calls/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/api_calls/work_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/batch_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/http_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/ghga_connector/core/message_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.907958 ghga_connector-0.3.6/ghga_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-12 13:28:31.000000 ghga_connector-0.3.6/ghga_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/get_package_name.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18568 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/license_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/scripts/script_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/script_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/script_utils/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4972 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/update_config_docs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6729 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/update_readme.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8499 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/scripts/update_template_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-12 13:28:31.915959 ghga_connector-0.3.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.907958 ghga_connector-0.3.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/endpoints_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/tests/fixtures/mock_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/mock_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/mock_api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/fixtures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/tests/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/integration/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/integration/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16085 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/integration/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/integration/test_file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.911958 ghga_connector-0.3.6/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:28:31.915959 ghga_connector-0.3.6/tests/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/unit/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/unit/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/unit/test_api_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-12 13:28:22.000000 ghga_connector-0.3.6/tests/unit/test_file_operations.py
```

### Comparing `ghga_connector-0.3.5/LICENSE` & `ghga_connector-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/PKG-INFO` & `ghga_connector-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_connector
-Version: 0.3.5
+Version: 0.3.6
 Summary: GHGA Connector - A CLI client application for interacting with the GHGA system.
 Home-page: https://github.com/ghga-de/ghga-connector
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -41,29 +41,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.5
+docker pull ghga/ghga-connector:0.3.6
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.5 .
+docker build -t ghga/ghga-connector:0.3.6 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.5 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.6 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_connector-0.3.5/README.md` & `ghga_connector-0.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,29 +24,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.5
+docker pull ghga/ghga-connector:0.3.6
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.5 .
+docker build -t ghga/ghga-connector:0.3.6 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.5 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.6 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_connector-0.3.5/ghga_connector/__init__.py` & `ghga_connector-0.3.6/ghga_connector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 CLI - Client to perform up- and download operations to and from a local ghga instance
 """
 
-__version__ = "0.3.5"
+__version__ = "0.3.6"
```

### Comparing `ghga_connector-0.3.5/ghga_connector/__main__.py` & `ghga_connector-0.3.6/ghga_connector/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/cli.py` & `ghga_connector-0.3.6/ghga_connector/cli.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/config.py` & `ghga_connector-0.3.6/ghga_connector/config.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/__init__.py` & `ghga_connector-0.3.6/ghga_connector/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/api_calls/__init__.py` & `ghga_connector-0.3.6/ghga_connector/core/api_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/api_calls/download.py` & `ghga_connector-0.3.6/ghga_connector/core/api_calls/download.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/api_calls/upload.py` & `ghga_connector-0.3.6/ghga_connector/core/api_calls/upload.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/api_calls/utils.py` & `ghga_connector-0.3.6/ghga_connector/core/api_calls/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/api_calls/work_package.py` & `ghga_connector-0.3.6/ghga_connector/core/api_calls/work_package.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/batch_processing.py` & `ghga_connector-0.3.6/ghga_connector/core/batch_processing.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/client.py` & `ghga_connector-0.3.6/ghga_connector/core/client.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/constants.py` & `ghga_connector-0.3.6/ghga_connector/core/constants.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/exceptions.py` & `ghga_connector-0.3.6/ghga_connector/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/file_operations.py` & `ghga_connector-0.3.6/ghga_connector/core/file_operations.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/http_translation.py` & `ghga_connector-0.3.6/ghga_connector/core/http_translation.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/main.py` & `ghga_connector-0.3.6/ghga_connector/core/main.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector/core/message_display.py` & `ghga_connector-0.3.6/ghga_connector/core/message_display.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/ghga_connector.egg-info/PKG-INFO` & `ghga_connector-0.3.6/ghga_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga-connector
-Version: 0.3.5
+Version: 0.3.6
 Summary: GHGA Connector - A CLI client application for interacting with the GHGA system.
 Home-page: https://github.com/ghga-de/ghga-connector
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -41,29 +41,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.5
+docker pull ghga/ghga-connector:0.3.6
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.5 .
+docker build -t ghga/ghga-connector:0.3.6 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.5 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.6 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_connector-0.3.5/ghga_connector.egg-info/SOURCES.txt` & `ghga_connector-0.3.6/ghga_connector.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -23,22 +23,30 @@
 ghga_connector/core/main.py
 ghga_connector/core/message_display.py
 ghga_connector/core/api_calls/__init__.py
 ghga_connector/core/api_calls/download.py
 ghga_connector/core/api_calls/upload.py
 ghga_connector/core/api_calls/utils.py
 ghga_connector/core/api_calls/work_package.py
+scripts/__init__.py
+scripts/get_package_name.py
+scripts/license_checker.py
+scripts/update_config_docs.py
+scripts/update_readme.py
+scripts/update_template_files.py
+scripts/script_utils/__init__.py
+scripts/script_utils/cli.py
 tests/fixtures/__init__.py
 tests/fixtures/config.py
+tests/fixtures/endpoints_handler.py
 tests/fixtures/s3.py
 tests/fixtures/state.py
 tests/fixtures/utils.py
 tests/fixtures/mock_api/__init__.py
 tests/fixtures/mock_api/app.py
-tests/fixtures/mock_api/testcontainer.py
 tests/integration/__init__.py
 tests/integration/test_cli.py
 tests/integration/test_file_operations.py
 tests/integration/fixtures/__init__.py
 tests/integration/fixtures/utils.py
 tests/unit/__init__.py
 tests/unit/test_api_calls.py
```

### Comparing `ghga_connector-0.3.5/setup.cfg` & `ghga_connector-0.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/setup.py` & `ghga_connector-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/fixtures/__init__.py` & `ghga_connector-0.3.6/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/fixtures/config.py` & `ghga_connector-0.3.6/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/fixtures/mock_api/__init__.py` & `ghga_connector-0.3.6/tests/fixtures/mock_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/fixtures/mock_api/app.py` & `ghga_connector-0.3.6/tests/fixtures/mock_api/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,30 +18,35 @@
 Runs a small fastapi mock server for testing purposes.
 All mocks work correclty with file_id == "1".
 The drs3 mock sends back a "wait 1 minute" for file_id == "1m"
 All other file_ids will fail
 """
 
 import base64
+import json
+import logging
 import os
-from datetime import datetime, timezone
+from datetime import datetime
 from enum import Enum
 from typing import List
 
 try:  # workaround for https://github.com/pydantic/pydantic/issues/5821
     from typing_extensions import Literal
 except ImportError:
     from typing import Literal  # type: ignore
 
-
-from fastapi import FastAPI, Header, HTTPException, Request, status
-from fastapi.responses import JSONResponse, Response
+import httpx
+from fastapi import HTTPException, status
+from ghga_service_commons.utils.utc_dates import now_as_utc
 from pydantic import BaseModel
 
-DEFAULT_PART_SIZE = 16 * 1024 * 1024
+from tests.fixtures.endpoints_handler import EndpointsHandler
+
+logger = logging.getLogger()
+logger.setLevel(logging.INFO)
 
 
 class UploadStatus(str, Enum):
     """
     Enum for the possible UploadStatus of a specific upload_id
     """
 
@@ -134,15 +139,15 @@
     size: int
     created_time: str
     updated_time: str
     checksums: List[Checksum]
     access_methods: List[AccessMethod]
 
 
-class HttpEnvelopeResponse(JSONResponse):
+class HttpEnvelopeResponse(httpx.Response):
     """Return base64 encoded envelope bytes"""
 
     response_id = "envelope"
 
     def __init__(self, *, envelope: str, status_code: int = 200):
         """Construct message and init the response."""
 
@@ -158,44 +163,46 @@
         self.status_code = status_code
         self.exception_id = exception_id
         self.description = description
         self.data = data
         super().__init__(description)
 
 
-app = FastAPI()
-
-
-@app.exception_handler(HttpyException)
-async def httpy_exception_handler(request: Request, exc: HttpyException):
+def httpy_exception_handler(exc: HttpyException):
     """Transform HttpException data into a proper response object"""
-    return JSONResponse(
+
+    return httpx.Response(
         status_code=exc.status_code,
-        content={
-            "exception_id": exc.exception_id,
-            "description": exc.description,
-            "data": exc.data,
-        },
+        content=json.dumps(
+            {
+                "exception_id": exc.exception_id,
+                "description": exc.description,
+                "data": exc.data,
+            }
+        ).encode("utf-8"),
     )
 
 
-@app.get("/ready", summary="readiness_probe")
-async def ready():
+@EndpointsHandler.get("/")
+def ready():
     """
     Readyness probe.
     """
-    return JSONResponse(None, status_code=status.HTTP_204_NO_CONTENT)
+    return httpx.Response(status_code=status.HTTP_204_NO_CONTENT)
 
 
-@app.get("/objects/{file_id}", summary="drs3_mock")
-async def drs3_objects(file_id: str, authorization=Header()):
+@EndpointsHandler.get("/objects/{file_id}")
+def drs3_objects(file_id: str, request: httpx.Request):
     """
     Mock for the drs3 /objects/{file_id} call
     """
 
+    # get authorization header
+    authorization = request.headers["authorization"]
+
     # simulate token authorization error
     if authorization == "Bearer authfail_normal":
         raise HTTPException(
             status_code=403, detail="This is not the token you're looking for."
         )
 
     # simulate token file_id/object_id mismatch
@@ -204,131 +211,149 @@
             status_code=403,
             exception_id="wrongFileAuthorizationError",
             description="Endpoint file ID did not match file ID announced in work order token.",
             data={},
         )
 
     if file_id == "retry":
-        return Response(
+        return httpx.Response(
             status_code=status.HTTP_202_ACCEPTED, headers={"Retry-After": "10"}
         )
 
     if file_id in ("downloadable", "big-downloadable", "envelope-missing"):
-        return DrsObjectServe(
-            file_id=file_id,
-            self_uri=f"drs://localhost:8080//{file_id}",
-            size=int(os.environ["S3_DOWNLOAD_FIELD_SIZE"]),
-            created_time=datetime.now(timezone.utc).isoformat(),
-            updated_time=datetime.now(timezone.utc).isoformat(),
-            checksums=[Checksum(checksum="1", type="md5")],
-            access_methods=[
-                AccessMethod(
-                    access_url=AccessURL(url=os.environ["S3_DOWNLOAD_URL"]), type="s3"
-                )
-            ],
+        return httpx.Response(
+            status_code=200,
+            content=DrsObjectServe(
+                file_id=file_id,
+                self_uri=f"drs://localhost:8080//{file_id}",
+                size=int(os.environ["S3_DOWNLOAD_FIELD_SIZE"]),
+                created_time=now_as_utc().isoformat(),
+                updated_time=now_as_utc().isoformat(),
+                checksums=[Checksum(checksum="1", type="md5")],
+                access_methods=[
+                    AccessMethod(
+                        access_url=AccessURL(url=os.environ["S3_DOWNLOAD_URL"]),
+                        type="s3",
+                    )
+                ],
+            ).json(),
         )
 
     raise HTTPException(
         status_code=404,
         detail=(f'The DRSObject with the id "{file_id}" does not exist.'),
     )
 
 
-@app.get("/objects/{file_id}/envelopes/{public_key}", summary="drs3_envelope_mock")
-async def drs3_objects_envelopes(file_id: str, public_key: str, authorization=Header()):
+@EndpointsHandler.get("/objects/{file_id}/envelopes/{public_key}")
+def drs3_objects_envelopes(file_id: str, public_key: str):
     """
     Mock for the dcs /objects/{file_id}/envelopes/{public_key} call
     """
 
     if file_id in ("downloadable", "big-downloadable"):
-        response_str = str.encode(os.environ["FAKE_HEADER_ENVELOPE"])
+        response_str = str.encode(os.environ["FAKE_ENVELOPE"])
         envelope = base64.b64encode(response_str).decode("utf-8")
         return HttpEnvelopeResponse(envelope=envelope)
 
     raise HttpyException(
         status_code=404,
         exception_id="noSuchObject",
         description=(f'The DRSObject with the id "{file_id}" does not exist.'),
         data={"file_id": file_id},
     )
 
 
-@app.get("/files/{file_id}", summary="ulc_get_files_mock", status_code=200)
-async def ulc_get_files(file_id: str):
+@EndpointsHandler.get("/files/{file_id}")
+def ulc_get_files(file_id: str):
     """
     Mock for the ulc GET /files/{file_id} call.
     """
 
     if file_id == "pending":
         return FileProperties(
             file_id=file_id,
             file_name=file_id,
             md5_checksum="",
             size=0,
             grouping_label="inbox",
-            creation_date=datetime.utcnow(),
-            update_date=datetime.utcnow(),
+            creation_date=now_as_utc().isoformat(),
+            update_date=now_as_utc().isoformat(),
             format="",
             current_upload_id="pending",
         )
 
     raise HttpyException(
         status_code=404,
         exception_id="fileNotRegistered",
         description=f'The file with the file_id "{file_id}" does not exist.',
         data={"file_id": file_id},
     )
 
 
-@app.get("/uploads/{upload_id}", summary="ulc_get_uploads_mock", status_code=200)
-async def ulc_get_uploads(upload_id: str):
+@EndpointsHandler.get("/uploads/{upload_id}")
+def ulc_get_uploads(upload_id: str):
     """
     Mock for the ulc GET /uploads/{upload_id} call.
     """
     if upload_id == "pending":
-        return UploadProperties(
-            upload_id="pending",
-            file_id="pending",
-            part_size=DEFAULT_PART_SIZE,
+        return httpx.Response(
+            status_code=200,
+            content=UploadProperties(
+                upload_id="pending",
+                file_id="pending",
+                part_size=int(os.environ["DEFAULT_PART_SIZE"]),
+            ).json(),
         )
 
     raise HttpyException(
         status_code=404,
         exception_id="noSuchUpload",
         description=f'The upload with the id "{upload_id}" does not exist.',
         data={"upload_id": upload_id},
     )
 
 
-@app.post("/uploads", summary="ulc_post_uploads_mock", status_code=200)
-async def ulc_post_files_uploads(state: StatePost):
+@EndpointsHandler.post("/uploads")
+def ulc_post_files_uploads(request: httpx.Request):
     """
     Mock for the ulc POST /uploads call.
     """
+    content = json.loads(request.content)
+    state: StatePost = StatePost(**content)
 
     file_id = state.file_id
 
     if file_id == "uploadable":
-        return UploadProperties(
-            upload_id="pending",
-            file_id=file_id,
-            part_size=DEFAULT_PART_SIZE,
+        return httpx.Response(
+            status_code=200,
+            content=UploadProperties(
+                upload_id="pending",
+                file_id=file_id,
+                part_size=int(os.environ["DEFAULT_PART_SIZE"]),
+            ).json(),
         )
     if file_id == "uploadable-16":
-        return UploadProperties(
-            upload_id="pending",
-            file_id=file_id,
-            part_size=16 * 1024 * 1024,
+        return httpx.Response(
+            status_code=200,
+            content=UploadProperties(
+                upload_id="pending",
+                file_id=file_id,
+                part_size=16 * 1024 * 1024,
+            ).json(),
         )
 
     if file_id == "uploadable-8":
-        return UploadProperties(
-            upload_id="pending",
-            file_id=file_id,
-            part_size=8 * 1024 * 1024,
+        return httpx.Response(
+            status_code=200,
+            content=UploadProperties(
+                upload_id="pending",
+                file_id=file_id,
+                part_size=8 * 1024 * 1024,
+            ).json(),
         )
     if file_id == "pending":
         raise HttpyException(
             status_code=403,
             exception_id="noFileAccess",
             description=f'Can`t start multipart upload for file with file id "{file_id}".',
             data={"file_id": file_id},
@@ -338,61 +363,58 @@
         status_code=400,
         exception_id="fileNotRegistered",
         description=f'The file with the file_id "{file_id}" does not exist.',
         data={"file_id": file_id},
     )
 
 
-@app.post(
-    "/uploads/{upload_id}/parts/{part_no}/signed_urls",
-    summary="ulc_post_uploads_parts_files_signed_urls_mock",
-    status_code=200,
-)
-async def ulc_post_uploads_parts_files_signed_posts(upload_id: str, part_no: int):
+@EndpointsHandler.post("/uploads/{upload_id}/parts/{part_no}/signed_urls")
+def ulc_post_uploads_parts_files_signed_posts(upload_id: str, part_no: int):
     """
     Mock for the ulc POST /uploads/{upload_id}/parts/{part_no}/signed_urls call.
     """
 
     if upload_id == "pending":
-        if part_no == 1:
-            url = os.environ["S3_UPLOAD_URL_1"]
-            return {"url": url}
-        if part_no == 2:
-            url = os.environ["S3_UPLOAD_URL_2"]
-            return {"url": url}
+        if part_no in (1, 2):
+            urls = (os.environ["S3_UPLOAD_URL_1"], os.environ["S3_UPLOAD_URL_2"])
+            return httpx.Response(
+                status_code=200, text=json.dumps({"url": urls[part_no - 1]})
+            )
 
     raise HttpyException(
         status_code=404,
         exception_id="noSuchUpload",
         description=f'The file with the upload id "{upload_id}" does not exist.',
         data={"upload_id": upload_id},
     )
 
 
-@app.patch("/uploads/{upload_id}", summary="ulc_patch_uploads_mock", status_code=204)
-async def ulc_patch_uploads(upload_id: str, state: StatePatch):
+@EndpointsHandler.patch("/uploads/{upload_id}")
+def ulc_patch_uploads(upload_id: str, request: httpx.Request):
     """
     Mock for the ulc PATCH /uploads/{upload_id} call
     """
+    content = json.loads(request.content)
+    state: StatePatch = StatePatch(**content)
     upload_status = state.status
 
     if upload_id == "uploaded":
         if upload_status == UploadStatus.CANCELLED:
-            return JSONResponse(None, status_code=status.HTTP_204_NO_CONTENT)
+            return httpx.Response(status_code=status.HTTP_204_NO_CONTENT)
 
         raise HttpyException(
             status_code=400,
             exception_id="uploadNotPending",
             description=f'The upload with id "{upload_id}" can`t be set to "{upload_status}"',
             data={"upload_id": upload_id, "current_upload_status": upload_id},
         )
 
     if upload_id == "pending":
         if upload_status == UploadStatus.UPLOADED:
-            return JSONResponse(None, status_code=status.HTTP_204_NO_CONTENT)
+            return httpx.Response(status_code=status.HTTP_204_NO_CONTENT)
 
         raise HttpyException(
             status_code=400,
             exception_id="uploadStatusChange",
             description=f'The upload with id "{upload_id}" can`t be set to "{upload_status}"',
             data={"upload_id": upload_id, "target_status": upload_status},
         )
@@ -409,17 +431,31 @@
         status_code=404,
         exception_id="noSuchUpload",
         description=f'The upload with id "{upload_id}" does not exist',
         data={"upload_id": upload_id},
     )
 
 
-@app.post(
-    "/work-packages/{package_id}/files/{file_id}/work-order-tokens", status_code=201
-)
-async def create_work_order_token(
-    package_id: str, file_id: str, authorization=Header()
-):
+@EndpointsHandler.post("/work-packages/{package_id}/files/{file_id}/work-order-tokens")
+def create_work_order_token(package_id: str, file_id: str):
     """Mock Work Order Token endpoint"""
 
     # has to be at least 48 chars long
-    return base64.b64encode(b"1234567890" * 5).decode()
+    return httpx.Response(
+        status_code=201, content=base64.b64encode(b"1234567890" * 5).decode()
+    )
+
+
+def handle_request(request: httpx.Request):
+    """
+    This is used as the callback function for the httpx_mock fixture in test_cli.py.
+    """
+    url = str(request.url)
+    logger.info("Received request for url: %s", url)
+    try:
+        endpoint_function = EndpointsHandler.build_loaded_endpoint_function(request)
+        return endpoint_function()
+    except HttpyException as exc:
+        return httpy_exception_handler(exc=exc)
+    except HTTPException as exc:
+        text = json.dumps({"detail": exc.detail})
+        return httpx.Response(status_code=exc.status_code, text=text)
```

### Comparing `ghga_connector-0.3.5/tests/fixtures/s3.py` & `ghga_connector-0.3.6/tests/fixtures/s3.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/fixtures/state.py` & `ghga_connector-0.3.6/tests/fixtures/state.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/fixtures/utils.py` & `ghga_connector-0.3.6/tests/fixtures/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utils for Fixture handling"""
 
-
 from pathlib import Path
 from typing import Any
 
 import crypt4gh.keys
 from ghga_service_commons.utils import crypt
 
 BASE_DIR = Path(__file__).parent.resolve()
```

### Comparing `ghga_connector-0.3.5/tests/integration/__init__.py` & `ghga_connector-0.3.6/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/integration/fixtures/__init__.py` & `ghga_connector-0.3.6/tests/integration/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/integration/fixtures/utils.py` & `ghga_connector-0.3.6/tests/integration/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/integration/test_cli.py` & `ghga_connector-0.3.6/tests/integration/test_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,55 +15,87 @@
 #
 
 """Tests for the up- and download functions of the cli"""
 
 import base64
 import os
 import pathlib
+import re
 from contextlib import nullcontext
 from filecmp import cmp
 from pathlib import Path
 from typing import Optional
 from unittest.mock import Mock, patch
 
 import crypt4gh.keys
+import httpx
 import pytest
 from ghga_service_commons.utils.temp_files import big_temp_file
+from pytest_httpx import HTTPXMock, httpx_mock  # noqa: F401
 
 from ghga_connector.cli import download, upload
 from ghga_connector.core import exceptions
 from ghga_connector.core.constants import DEFAULT_PART_SIZE
 from ghga_connector.core.file_operations import Crypt4GHEncryptor
 from tests.fixtures import state
 from tests.fixtures.config import get_test_config
-from tests.fixtures.mock_api.testcontainer import MockAPIContainer
+from tests.fixtures.mock_api.app import handle_request
 from tests.fixtures.s3 import S3Fixture, get_big_s3_object, s3_fixture  # noqa: F401
 from tests.fixtures.utils import PRIVATE_KEY_FILE, PUBLIC_KEY_FILE, mock_wps_token
 
+URL_PATTERN = re.compile(r"^http://127\.0\.0\.1.*")
+
+ENVIRON_DEFAULTS = {
+    "DEFAULT_PART_SIZE": str(16 * 1024 * 1024),
+    "S3_DOWNLOAD_URL": "test://download.url",
+    "S3_UPLOAD_URL_1": "test://upload.url",
+    "S3_UPLOAD_URL_2": "test://upload.url",
+    "S3_DOWNLOAD_FIELD_SIZE": str(146),
+    "FAKE_ENVELOPE": "Fake_envelope",
+}
+
+unintercepted_hosts: list[str] = []
+
+
+@pytest.fixture
+def non_mocked_hosts() -> list:
+    # Let requests go out to localstack/S3
+    return unintercepted_hosts
+
+
+@pytest.fixture
+def assert_all_responses_were_requested() -> bool:
+    return False
+
 
 @pytest.mark.parametrize(
     "file_size,part_size",
     [
         (6 * 1024 * 1024, 5 * 1024 * 1024),
         (12 * 1024 * 1024, 5 * 1024 * 1024),
         (20 * 1024 * 1024, 1 * 1024 * 1024),
         (20 * 1024 * 1024, 64 * 1024),
         (1 * 1024 * 1024, DEFAULT_PART_SIZE),
         (20 * 1024 * 1024, DEFAULT_PART_SIZE),
     ],
 )
 @pytest.mark.asyncio
 async def test_multipart_download(
+    httpx_mock: HTTPXMock,  # noqa: F811
     file_size: int,
     part_size: int,
     s3_fixture: S3Fixture,  # noqa F811
     tmp_path: pathlib.Path,
     monkeypatch,
 ):
     """Test the multipart download of a file"""
+    httpx_mock.add_callback(callback=handle_request)
+    for name, value in ENVIRON_DEFAULTS.items():
+        monkeypatch.setenv(name, value)
+
     big_object = await get_big_s3_object(s3_fixture, object_size=file_size)
 
     # The download function will ask the user for input.
     monkeypatch.setattr("ghga_connector.core.main.get_wps_token", mock_wps_token)
     monkeypatch.setattr(
         "ghga_connector.core.api_calls.work_package.WorkPackageAccessor.get_package_files",
         Mock(return_value=dict(zip([big_object.object_id], [""]))),
@@ -79,43 +111,44 @@
 
     # get s3 download url
     download_url = await s3_fixture.storage.get_object_download_url(
         bucket_id=big_object.bucket_id,
         object_id=big_object.object_id,
         expires_after=180,
     )
+    unintercepted_hosts.append(httpx.URL(download_url).host)
 
     fake_envelope = "Thisisafakeenvelope"
 
-    with MockAPIContainer(
-        s3_download_url=download_url,
-        s3_download_file_size=file_size_,
-        fake_envelope=fake_envelope,
-    ) as api:
-        api_url = api.get_connection_url()
-        with patch(
-            "ghga_connector.cli.CONFIG",
-            get_test_config(
-                download_api=api_url,
-                part_size=part_size,
-                wps_api_url=api.get_connection_url(),
-            ),
-        ):
-            download(
-                output_dir=tmp_path,
-                submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
-                submitter_private_key_path=Path(PRIVATE_KEY_FILE),
-            )
+    monkeypatch.setenv("S3_DOWNLOAD_URL", download_url)
+    monkeypatch.setenv("S3_DOWNLOAD_FIELD_SIZE", str(file_size_))
+    monkeypatch.setenv("FAKE_ENVELOPE", fake_envelope)
+
+    big_file_content = str.encode(fake_envelope)
+    big_file_content += big_object.content
+    api_url = "http://127.0.0.1"
+
+    with patch(
+        "ghga_connector.cli.CONFIG",
+        get_test_config(
+            download_api=api_url,
+            part_size=part_size,
+            wps_api_url=api_url,
+        ),
+    ):
+        download(
+            output_dir=tmp_path,
+            submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
+            submitter_private_key_path=Path(PRIVATE_KEY_FILE),
+        )
 
-        big_file_content = str.encode(fake_envelope)
-        big_file_content += big_object.content
-        with open(tmp_path / f"{big_object.object_id}.c4gh", "rb") as file:
-            observed_content = file.read()
+    with open(tmp_path / f"{big_object.object_id}.c4gh", "rb") as file:
+        observed_content = file.read()
 
-        assert observed_content == big_file_content
+    assert observed_content == big_file_content
 
 
 @pytest.mark.parametrize(
     "bad_url,bad_outdir,file_name,expected_exception,proceed_on_missing",
     [
         (True, False, "file_downloadable", exceptions.ApiNotReachableError, True),
         (False, False, "file_downloadable", None, True),
@@ -136,28 +169,34 @@
             exceptions.FileNotRegisteredError,
             True,
         ),
     ],
 )
 @pytest.mark.asyncio
 async def test_download(
+    httpx_mock: HTTPXMock,  # noqa: F811
     bad_url: bool,
     bad_outdir: bool,
     file_name: str,
     expected_exception: type[Optional[Exception]],
     s3_fixture: S3Fixture,  # noqa: F811
     tmp_path: pathlib.Path,
     proceed_on_missing: bool,
     monkeypatch,
 ):
     """Test the download of a file"""
     output_dir = Path("/non/existing/path") if bad_outdir else tmp_path
 
     file = state.FILES[file_name]
 
+    # Intercept requests sent with httpx
+    httpx_mock.add_callback(callback=handle_request, url=URL_PATTERN)
+    for name, value in ENVIRON_DEFAULTS.items():
+        monkeypatch.setenv(name, value)
+
     # The download function will ask the user for input.
     monkeypatch.setattr("ghga_connector.core.main.get_wps_token", mock_wps_token)
     monkeypatch.setattr(
         "ghga_connector.core.api_calls.work_package.WorkPackageAccessor.get_package_files",
         Mock(return_value=dict(zip([file.file_id], [""]))),
     )
     monkeypatch.setattr(
@@ -170,70 +209,70 @@
             bucket_id=file.grouping_label,
             object_id=file.file_id,
             expires_after=60,
         )
 
     else:
         download_url = ""
+    unintercepted_hosts.append(httpx.URL(download_url).host)
 
     fake_envelope = "Thisisafakeenvelope"
 
-    with MockAPIContainer(
-        s3_download_url=download_url,
-        s3_download_file_size=os.path.getsize(file.file_path),
-        fake_envelope=fake_envelope,
-    ) as api:
-        api_url = "http://bad_url" if bad_url else api.get_connection_url()
-
+    monkeypatch.setenv("S3_DOWNLOAD_URL", download_url)
+    monkeypatch.setenv("S3_DOWNLOAD_FIELD_SIZE", str(os.path.getsize(file.file_path)))
+    monkeypatch.setenv("FAKE_ENVELOPE", fake_envelope)
+
+    api_url = "http://bad_url" if bad_url else "http://127.0.0.1"
+
+    with patch(
+        "ghga_connector.cli.CONFIG",
+        get_test_config(download_api=api_url, wps_api_url=api_url),
+    ):
+        # needed to mock user input
         with patch(
-            "ghga_connector.cli.CONFIG",
-            get_test_config(download_api=api_url, wps_api_url=api.get_connection_url()),
+            "ghga_connector.core.batch_processing.CliInputHandler.get_input",
+            return_value="yes" if proceed_on_missing else "no",
         ):
-            # needed to mock user input
-            with patch(
-                "ghga_connector.core.batch_processing.CliInputHandler.get_input",
-                return_value="yes" if proceed_on_missing else "no",
-            ):
-                if file_name == "file_not_downloadable":
-                    # check both 403 scenarios
-                    with patch(
-                        "ghga_connector.core.api_calls.work_package._decrypt",
-                        lambda data, key: "authfail_normal",
+            if file_name == "file_not_downloadable":
+                # check both 403 scenarios
+                with patch(
+                    "ghga_connector.core.api_calls.work_package._decrypt",
+                    lambda data, key: "authfail_normal",
+                ):
+                    with pytest.raises(
+                        exceptions.UnauthorizedAPICallError,
+                        match="This is not the token you're looking for.",
                     ):
-                        with pytest.raises(
-                            exceptions.UnauthorizedAPICallError,
-                            match="This is not the token you're looking for.",
-                        ):
-                            download(
-                                output_dir=output_dir,
-                                submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
-                                submitter_private_key_path=Path(PRIVATE_KEY_FILE),
-                            )
-                    with patch(
-                        "ghga_connector.core.api_calls.work_package._decrypt",
-                        lambda data, key: "file_id_mismatch",
+                        download(
+                            output_dir=output_dir,
+                            submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
+                            submitter_private_key_path=Path(PRIVATE_KEY_FILE),
+                        )
+                with patch(
+                    "ghga_connector.core.api_calls.work_package._decrypt",
+                    lambda data, key: "file_id_mismatch",
+                ):
+                    with pytest.raises(
+                        exceptions.UnauthorizedAPICallError,
+                        match="Endpoint file ID did not match file ID announced in work order token.",
                     ):
-                        with pytest.raises(
-                            exceptions.UnauthorizedAPICallError,
-                            match="Endpoint file ID did not match file ID announced in work order token.",
-                        ):
-                            download(
-                                output_dir=output_dir,
-                                submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
-                                submitter_private_key_path=Path(PRIVATE_KEY_FILE),
-                            )
-                else:
-                    with pytest.raises(  # type: ignore
-                        expected_exception
-                    ) if expected_exception else nullcontext():
                         download(
                             output_dir=output_dir,
                             submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
                             submitter_private_key_path=Path(PRIVATE_KEY_FILE),
                         )
+            else:
+                with pytest.raises(  # type: ignore
+                    expected_exception
+                ) if expected_exception else nullcontext():
+                    download(
+                        output_dir=output_dir,
+                        submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
+                        submitter_private_key_path=Path(PRIVATE_KEY_FILE),
+                    )
 
         # BadResponseCode is no longer propagated and file at path does not exist
         if file_name == "file_not_downloadable":
             return
 
         tmp_file = tmp_path / "file_with_envelope"
 
@@ -256,22 +295,29 @@
         (False, "file_not_uploadable", exceptions.FileNotRegisteredError),
         (False, "file_with_bad_path", exceptions.FileDoesNotExistError),
         (False, "encrypted_file", exceptions.FileAlreadyEncryptedError),
     ],
 )
 @pytest.mark.asyncio
 async def test_upload(
+    httpx_mock: HTTPXMock,  # noqa: F811
     bad_url: bool,
     file_name: str,
     expected_exception: type[Optional[Exception]],
     s3_fixture: S3Fixture,  # noqa F811
+    monkeypatch,
 ):
     """Test the upload of a file, expects Abort, if the file was not found"""
     uploadable_file = state.FILES[file_name]
 
+    # Intercept requests sent with httpx
+    httpx_mock.add_callback(callback=handle_request, url=URL_PATTERN)
+    for name, value in ENVIRON_DEFAULTS.items():
+        monkeypatch.setenv(name, value)
+
     if file_name == "encrypted_file":
         # encrypt test file on the fly
         server_pubkey = base64.b64encode(
             crypt4gh.keys.get_public_key(PUBLIC_KEY_FILE)
         ).decode("utf-8")
         encryptor = Crypt4GHEncryptor(
             server_pubkey=server_pubkey, submitter_private_key_path=PRIVATE_KEY_FILE
@@ -286,66 +332,75 @@
 
     upload_url = await s3_fixture.storage.get_part_upload_url(
         bucket_id=uploadable_file.grouping_label,
         object_id=uploadable_file.file_id,
         upload_id=upload_id,
         part_number=1,
     )
+    unintercepted_hosts.append(httpx.URL(upload_url).host)
 
-    with MockAPIContainer(s3_upload_url_1=upload_url) as api:
-        api_url = "http://bad_url" if bad_url else api.get_connection_url()
+    monkeypatch.setenv("S3_UPLOAD_URL_1", upload_url)
 
-        with patch("ghga_connector.cli.CONFIG", get_test_config(upload_api=api_url)):
-            with pytest.raises(  # type: ignore
-                expected_exception
-            ) if expected_exception else nullcontext():
-                if file_name == "encrypted_file":
-                    upload(
-                        file_id=uploadable_file.file_id,
-                        file_path=Path(encrypted_path).resolve(),
-                        submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
-                        submitter_private_key_path=Path(PRIVATE_KEY_FILE),
-                    )
-                else:
-                    upload(
-                        file_id=uploadable_file.file_id,
-                        file_path=uploadable_file.file_path.resolve(),
-                        submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
-                        submitter_private_key_path=Path(PRIVATE_KEY_FILE),
-                    )
+    api_url = "http://bad_url" if bad_url else "http://127.0.0.1"
 
-                await s3_fixture.storage.complete_multipart_upload(
-                    upload_id=upload_id,
-                    bucket_id=uploadable_file.grouping_label,
-                    object_id=uploadable_file.file_id,
+    with patch("ghga_connector.cli.CONFIG", get_test_config(upload_api=api_url)):
+        with pytest.raises(  # type: ignore
+            expected_exception
+        ) if expected_exception else nullcontext():
+            if file_name == "encrypted_file":
+                upload(
+                    file_id=uploadable_file.file_id,
+                    file_path=Path(encrypted_path).resolve(),
+                    submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
+                    submitter_private_key_path=Path(PRIVATE_KEY_FILE),
                 )
-
-                assert await s3_fixture.storage.does_object_exist(
-                    bucket_id=uploadable_file.grouping_label,
-                    object_id=uploadable_file.file_id,
+            else:
+                upload(
+                    file_id=uploadable_file.file_id,
+                    file_path=uploadable_file.file_path.resolve(),
+                    submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
+                    submitter_private_key_path=Path(PRIVATE_KEY_FILE),
                 )
 
+            await s3_fixture.storage.complete_multipart_upload(
+                upload_id=upload_id,
+                bucket_id=uploadable_file.grouping_label,
+                object_id=uploadable_file.file_id,
+            )
+
+            assert await s3_fixture.storage.does_object_exist(
+                bucket_id=uploadable_file.grouping_label,
+                object_id=uploadable_file.file_id,
+            )
+
 
 @pytest.mark.parametrize(
     "file_size,anticipated_part_size",
     [
         (6 * 1024 * 1024, 8),
         (20 * 1024 * 1024, 16),
     ],
 )
 @pytest.mark.asyncio
 async def test_multipart_upload(
+    httpx_mock: HTTPXMock,  # noqa: F811
     file_size: int,
     anticipated_part_size: int,
     s3_fixture: S3Fixture,  # noqa F811
+    monkeypatch,
 ):
     """Test the upload of a file, expects Abort, if the file was not found"""
     bucket_id = s3_fixture.existing_buckets[0]
     file_id = "uploadable-" + str(anticipated_part_size)
 
+    # Intercept requests sent with httpx
+    httpx_mock.add_callback(callback=handle_request, url=URL_PATTERN)
+    for name, value in ENVIRON_DEFAULTS.items():
+        monkeypatch.setenv(name, value)
+
     anticipated_part_size = anticipated_part_size * 1024 * 1024
 
     anticipated_part_quantity = file_size // anticipated_part_size
 
     if anticipated_part_quantity * anticipated_part_size < file_size:
         anticipated_part_quantity += 1
 
@@ -358,47 +413,48 @@
     # create presigned url for upload part 1
     upload_url_1 = await s3_fixture.storage.get_part_upload_url(
         upload_id=upload_id,
         bucket_id=bucket_id,
         object_id=file_id,
         part_number=1,
     )
+    unintercepted_hosts.append(httpx.URL(upload_url_1).host)
 
     # create presigned url for upload part 2
     upload_url_2 = await s3_fixture.storage.get_part_upload_url(
         upload_id=upload_id,
         bucket_id=bucket_id,
         object_id=file_id,
         part_number=2,
     )
+    unintercepted_hosts.append(httpx.URL(upload_url_2).host)
 
-    with MockAPIContainer(
-        s3_upload_url_1=upload_url_1,
-        s3_upload_url_2=upload_url_2,
-    ) as api:
-        api_url = api.get_connection_url()
-
-        # create big temp file
-        with big_temp_file(file_size) as file:
-            with patch(
-                "ghga_connector.cli.CONFIG",
-                get_test_config(upload_api=api_url),
-            ):
-                upload(
-                    file_id=file_id,
-                    file_path=Path(file.name),
-                    submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
-                    submitter_private_key_path=Path(PRIVATE_KEY_FILE),
-                )
+    monkeypatch.setenv("S3_UPLOAD_URL_1", upload_url_1)
+    monkeypatch.setenv("S3_UPLOAD_URL_2", upload_url_2)
 
-        # confirm upload
-        await s3_fixture.storage.complete_multipart_upload(
-            upload_id=upload_id,
-            bucket_id=bucket_id,
-            object_id=file_id,
-            anticipated_part_quantity=anticipated_part_quantity,
-            anticipated_part_size=anticipated_part_size,
-        )
-        assert await s3_fixture.storage.does_object_exist(
-            bucket_id=bucket_id,
-            object_id=file_id,
-        )
+    api_url = "http://127.0.0.1"
+
+    # create big temp file
+    with big_temp_file(file_size) as file:
+        with patch(
+            "ghga_connector.cli.CONFIG",
+            get_test_config(upload_api=api_url),
+        ):
+            upload(
+                file_id=file_id,
+                file_path=Path(file.name),
+                submitter_pubkey_path=Path(PUBLIC_KEY_FILE),
+                submitter_private_key_path=Path(PRIVATE_KEY_FILE),
+            )
+
+    # confirm upload
+    await s3_fixture.storage.complete_multipart_upload(
+        upload_id=upload_id,
+        bucket_id=bucket_id,
+        object_id=file_id,
+        anticipated_part_quantity=anticipated_part_quantity,
+        anticipated_part_size=anticipated_part_size,
+    )
+    assert await s3_fixture.storage.does_object_exist(
+        bucket_id=bucket_id,
+        object_id=file_id,
+    )
```

### Comparing `ghga_connector-0.3.5/tests/integration/test_file_operations.py` & `ghga_connector-0.3.6/tests/integration/test_file_operations.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/unit/__init__.py` & `ghga_connector-0.3.6/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/unit/fixtures/__init__.py` & `ghga_connector-0.3.6/tests/unit/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/unit/fixtures/utils.py` & `ghga_connector-0.3.6/tests/unit/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/unit/test_api_calls.py` & `ghga_connector-0.3.6/tests/unit/test_api_calls.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     CantChangeUploadStatusError,
     ConnectionFailedError,
     InvalidWPSResponseError,
     MaxPartNoExceededError,
     NoWorkPackageAccessError,
     UploadNotRegisteredError,
 )
-from tests.fixtures.mock_api.testcontainer import MockAPIContainer
 from tests.fixtures.utils import mock_wps_token
 
 
 @pytest.mark.parametrize(
     "bad_url,upload_id,upload_status,expected_exception",
     [
         (False, "pending", UploadStatus.UPLOADED, None),
@@ -49,33 +48,56 @@
         (False, "pending", UploadStatus.CANCELLED, CantChangeUploadStatusError),
         (False, "uploadable", UploadStatus.UPLOADED, CantChangeUploadStatusError),
         (False, "not_uploadable", UploadStatus.UPLOADED, UploadNotRegisteredError),
         (True, "uploaded", UploadStatus.UPLOADED, ConnectionFailedError),
     ],
 )
 def test_patch_multipart_upload(
+    httpx_mock: HTTPXMock,
     bad_url: bool,
     upload_id: str,
     upload_status: UploadStatus,
     expected_exception: type[Optional[Exception]],
 ):
     """
     Test the patch_multipart_upload function
     """
-    with MockAPIContainer() as api:
-        api_url = "http://bad_url" if bad_url else api.get_connection_url()
 
-        with pytest.raises(  # type: ignore
-            expected_exception
-        ) if expected_exception else nullcontext():
-            patch_multipart_upload(
-                api_url=api_url,
-                upload_id=upload_id,
-                upload_status=upload_status,
+    api_url = "http://bad_url" if bad_url else "http://127.0.0.1"
+    if bad_url:
+        httpx_mock.add_exception(
+            exception=ConnectionFailedError(
+                url=f"{api_url}/uploads/{upload_id}", reason="Testing"
             )
+        )
+    elif expected_exception == CantChangeUploadStatusError:
+        httpx_mock.add_response(
+            status_code=400,
+            json={
+                "data": "",
+                "description": "",
+                "exception_id": "uploadNotPending",
+            },
+        )
+    elif expected_exception == UploadNotRegisteredError:
+        httpx_mock.add_response(
+            status_code=404,
+            json={"data": "", "description": "", "exception_id": "noSuchUpload"},
+        )
+    elif expected_exception is None:
+        httpx_mock.add_response(status_code=204)
+
+    with pytest.raises(  # type: ignore
+        expected_exception
+    ) if expected_exception else nullcontext():
+        patch_multipart_upload(
+            api_url=api_url,
+            upload_id=upload_id,
+            upload_status=upload_status,
+        )
 
 
 @pytest.mark.parametrize(
     "from_part, end_part, expected_exception",
     [
         (None, 10, None),
         (2, 10, None),
```

### Comparing `ghga_connector-0.3.5/tests/unit/test_core.py` & `ghga_connector-0.3.6/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.5/tests/unit/test_file_operations.py` & `ghga_connector-0.3.6/tests/unit/test_file_operations.py`

 * *Files identical despite different names*


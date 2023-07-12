# Comparing `tmp/fusion-engine-client-1.20.0rc5.tar.gz` & `tmp/fusion-engine-client-1.20.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-client-1.20.0rc5.tar", last modified: Wed Jul 12 13:44:06 2023, max compression
+gzip compressed data, was "fusion-engine-client-1.20.0rc6.tar", last modified: Wed Jul 12 14:53:01 2023, max compression
```

## Comparing `fusion-engine-client-1.20.0rc5.tar` & `fusion-engine-client-1.20.0rc6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.250827 fusion-engine-client-1.20.0rc5/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-12 13:44:06.250827 fusion-engine-client-1.20.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.242827 fusion-engine-client-1.20.0rc5/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/bin/p1_display
--rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/bin/p1_extract
--rwxr-xr-x   0 runner    (1001) docker     (123)    13937 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/bin/p1_print
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.242827 fusion-engine-client-1.20.0rc5/fusion_engine_client/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.242827 fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   114807 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/attitude.py
--rw-r--r--   0 runner    (1001) docker     (123)    41758 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.246827 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56721 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    25370 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    26231 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/fault_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/gnss_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/measurement_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    39947 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/ros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/signal_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35596 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.246827 fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22963 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    31146 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/mixed_log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.246827 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24860 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/time_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.242827 fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-12 13:44:06.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-12 13:44:06.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:44:06.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-12 13:44:06.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 13:44:06.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:44:06.250827 fusion-engine-client-1.20.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.250827 fusion-engine-client-1.20.0rc5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_mixed_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_time_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.255403 fusion-engine-client-1.20.0rc6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-12 14:53:01.255403 fusion-engine-client-1.20.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.239403 fusion-engine-client-1.20.0rc6/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/bin/p1_display
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/bin/p1_extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13937 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/bin/p1_print
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.239403 fusion-engine-client-1.20.0rc6/fusion_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.243403 fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   114807 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41758 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.247403 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56721 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25370 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26231 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/fault_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/gnss_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/measurement_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39947 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/ros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/signal_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35596 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.247403 fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22963 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31146 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/mixed_log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.251403 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24860 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.243403 fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-12 14:53:01.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-12 14:53:01.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:53:01.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-12 14:53:01.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 14:53:01.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:53:01.255403 fusion-engine-client-1.20.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.255403 fusion-engine-client-1.20.0rc6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_mixed_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_time_range.py
```

### Comparing `fusion-engine-client-1.20.0rc5/PKG-INFO` & `fusion-engine-client-1.20.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.20.0rc5
+Version: 1.20.0rc6
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.20.0rc5/README.md` & `fusion-engine-client-1.20.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/bin/p1_extract` & `fusion-engine-client-1.20.0rc6/bin/p1_extract`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/bin/p1_print` & `fusion-engine-client-1.20.0rc6/bin/p1_print`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/analyzer.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/attitude.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/attitude.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/data_loader.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/configuration.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/configuration.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/control.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/defs.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/device.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/device.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/fault_control.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/fault_control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/gnss_corrections.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/gnss_corrections.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/measurement_details.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/measurement_details.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/measurements.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/measurements.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/ros.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/ros.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/signal_defs.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/signal_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/solution.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/solution.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/timestamp.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/timestamp.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/decoder.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/encoder.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/file_index.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/mixed_log_reader.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/argument_parser.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/bin_utils.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/bin_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/construct_utils.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/enum_utils.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/log.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/log.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/numpy_utils.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/time_range.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/time_range.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/trace.py` & `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/PKG-INFO` & `fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.20.0rc5
+Version: 1.20.0rc6
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/SOURCES.txt` & `fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/setup.py` & `fusion-engine-client-1.20.0rc6/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/tests/test_config.py` & `fusion-engine-client-1.20.0rc6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/tests/test_construct_utils.py` & `fusion-engine-client-1.20.0rc6/tests/test_construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/tests/test_data_loader.py` & `fusion-engine-client-1.20.0rc6/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/tests/test_decoder.py` & `fusion-engine-client-1.20.0rc6/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/tests/test_encoder.py` & `fusion-engine-client-1.20.0rc6/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/tests/test_enum_utils.py` & `fusion-engine-client-1.20.0rc6/tests/test_enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/tests/test_file_index.py` & `fusion-engine-client-1.20.0rc6/tests/test_file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/tests/test_message_defs.py` & `fusion-engine-client-1.20.0rc6/tests/test_message_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/tests/test_mixed_log_reader.py` & `fusion-engine-client-1.20.0rc6/tests/test_mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc5/tests/test_time_range.py` & `fusion-engine-client-1.20.0rc6/tests/test_time_range.py`

 * *Files identical despite different names*


# Comparing `tmp/fusion-engine-client-1.20.0rc4.tar.gz` & `tmp/fusion-engine-client-1.20.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-client-1.20.0rc4.tar", last modified: Fri Jul  7 23:25:15 2023, max compression
+gzip compressed data, was "fusion-engine-client-1.20.0rc5.tar", last modified: Wed Jul 12 13:44:06 2023, max compression
```

## Comparing `fusion-engine-client-1.20.0rc4.tar` & `fusion-engine-client-1.20.0rc5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.148193 fusion-engine-client-1.20.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-07 23:25:15.148193 fusion-engine-client-1.20.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.144193 fusion-engine-client-1.20.0rc4/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/bin/p1_display
--rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/bin/p1_extract
--rwxr-xr-x   0 runner    (1001) docker     (123)    13937 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/bin/p1_print
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.144193 fusion-engine-client-1.20.0rc4/fusion_engine_client/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.144193 fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   114646 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/attitude.py
--rw-r--r--   0 runner    (1001) docker     (123)    41758 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.144193 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56721 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24157 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    26203 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/fault_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/gnss_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/measurement_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    39947 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/ros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/signal_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35596 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.144193 fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22963 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    31146 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/mixed_log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.148193 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24860 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/time_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.144193 fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-07 23:25:15.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-07 23:25:15.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:25:15.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-07 23:25:15.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 23:25:15.000000 fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 23:25:15.148193 fusion-engine-client-1.20.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:25:15.148193 fusion-engine-client-1.20.0rc4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_mixed_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-07-07 23:24:37.000000 fusion-engine-client-1.20.0rc4/tests/test_time_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.250827 fusion-engine-client-1.20.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-12 13:44:06.250827 fusion-engine-client-1.20.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.242827 fusion-engine-client-1.20.0rc5/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/bin/p1_display
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/bin/p1_extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13937 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/bin/p1_print
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.242827 fusion-engine-client-1.20.0rc5/fusion_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.242827 fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   114807 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41758 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.246827 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56721 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25370 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26231 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/fault_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/gnss_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/measurement_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39947 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/ros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/signal_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35596 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.246827 fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22963 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31146 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/mixed_log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.246827 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24860 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.242827 fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-12 13:44:06.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-12 13:44:06.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:44:06.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-12 13:44:06.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 13:44:06.000000 fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:44:06.250827 fusion-engine-client-1.20.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:44:06.250827 fusion-engine-client-1.20.0rc5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_mixed_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-07-12 13:43:29.000000 fusion-engine-client-1.20.0rc5/tests/test_time_range.py
```

### Comparing `fusion-engine-client-1.20.0rc4/PKG-INFO` & `fusion-engine-client-1.20.0rc5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.20.0rc4
+Version: 1.20.0rc5
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.20.0rc4/README.md` & `fusion-engine-client-1.20.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/bin/p1_extract` & `fusion-engine-client-1.20.0rc5/bin/p1_extract`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/bin/p1_print` & `fusion-engine-client-1.20.0rc5/bin/p1_print`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/analyzer.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -914,15 +914,15 @@
         num_traces = len(figure.data)
         buttons = [dict(label='All', method='restyle', args=['visible', [True] * num_traces])]
         for system, indices in sorted(indices_by_system.items()):
             if len(indices) == 0:
                 continue
             visible = np.full((num_traces,), False)
             visible[indices] = True
-            buttons.append(dict(label=str(system), method='restyle', args=['visible', list(visible)]))
+            buttons.append(dict(label=f'{str(system)} ({len(indices)})', method='restyle', args=['visible', visible]))
         figure['layout']['updatemenus'] = [{
             'type': 'buttons',
             'direction': 'left',
             'buttons': buttons,
             'x': 0.0,
             'xanchor': 'left',
             'y': 1.1,
@@ -1000,19 +1000,21 @@
                          5, 1)
 
         num_count_traces = len(figure.data)
 
         # Plot each satellite. Plot in reverse order so G01 is at the top of the Y axis.
         data_by_sv = GNSSSatelliteMessage.group_by_sv(data)
         svs = list(data_by_sv.keys())
+        svs_by_system = defaultdict(set)
         indices_by_system = defaultdict(list)
         for i, sv in enumerate(svs[::-1]):
             sv = int(sv)
             system = get_system(sv)
             name = satellite_to_string(sv, short=True)
+            svs_by_system[system].add(sv)
 
             sv_data = data_by_sv[sv]
             time = sv_data['p1_time'] - float(self.t0)
             is_used = np.bitwise_and(sv_data['flags'], SatelliteInfo.SATELLITE_USED).astype(bool)
 
             idx = is_used
             if np.any(idx):
@@ -1043,15 +1045,16 @@
         buttons = [dict(label='All', method='restyle', args=['visible', [True] * num_traces])]
         for system, indices in sorted(indices_by_system.items()):
             if len(indices) == 0:
                 continue
             visible = np.full((num_traces,), False)
             visible[:num_count_traces] = True
             visible[indices] = True
-            buttons.append(dict(label=str(system), method='restyle', args=['visible', list(visible)]))
+            buttons.append(dict(label=f'{str(system)} ({len(svs_by_system[system])})', method='restyle',
+                                args=['visible', visible]))
         figure['layout']['updatemenus'] = [{
             'type': 'buttons',
             'direction': 'left',
             'buttons': buttons,
             'x': 0.0,
             'xanchor': 'left',
             'y': 1.1,
```

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/attitude.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/attitude.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/analysis/data_loader.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/analysis/data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/configuration.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/configuration.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/control.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/control.py`

 * *Files 3% similar despite different names*

```diff
@@ -630,7 +630,44 @@
         return result
 
     def __str__(self):
         return 'Shutdown Request [flags=0x%016x]' % self.shutdown_flags
 
     def calcsize(self) -> int:
         return self.ShutdownRequestConstruct.sizeof()
+
+
+class StartupRequest(MessagePayload):
+    """!
+    @brief Perform a device startup.
+    """
+    MESSAGE_TYPE = MessageType.STARTUP_REQUEST
+    MESSAGE_VERSION = 0
+
+    StartupRequestConstruct = Struct(
+        "startup_flags" / Int64ul,
+        Padding(8),
+    )
+
+    def __init__(self, startup_flags = 0):
+        self.startup_flags = startup_flags
+
+    def pack(self, buffer: bytes = None, offset: int = 0, return_buffer: bool = True) -> (bytes, int):
+        values = vars(self)
+        packed_data = self.StartupRequestConstruct.build(values)
+        return PackedDataToBuffer(packed_data, buffer, offset, return_buffer)
+
+    def unpack(self, buffer: bytes, offset: int = 0, message_version: int = MessagePayload._UNSPECIFIED_VERSION) -> int:
+        parsed = self.StartupRequestConstruct.parse(buffer[offset:])
+        self.__dict__.update(parsed)
+        return parsed._io.tell()
+
+    def __repr__(self):
+        result = super().__repr__()[:-1]
+        result += f', flags=0x{self.startup_flags:016X}]'
+        return result
+
+    def __str__(self):
+        return 'Startup Request [flags=0x%016x]' % self.startup_flags
+
+    def calcsize(self) -> int:
+        return self.StartupRequestConstruct.sizeof()
```

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/defs.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,15 @@
     MESSAGE_REQUEST = 13001
     RESET_REQUEST = 13002
     VERSION_INFO = 13003
     EVENT_NOTIFICATION = 13004
     SHUTDOWN_REQUEST = 13005
     FAULT_CONTROL = 13006
     DEVICE_ID = 13007
+    STARTUP_REQUEST = 13008
 
     SET_CONFIG = 13100
     GET_CONFIG = 13101
     SAVE_CONFIG = 13102
     CONFIG_RESPONSE = 13103
 
     IMPORT_DATA = 13110
```

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/device.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/device.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/fault_control.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/fault_control.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 class FaultType(IntEnum):
     CLEAR_ALL = 0
     CRASH = 1
     FATAL_ERROR = 2
     COCOM = 3
     ENABLE_GNSS = 4
     REGION_BLACKOUT = 5
+    QUECTEL_TEST = 6
 
 
 class CoComType(IntEnum):
     NONE = 0
     ACCELERATION = 1
     SPEED = 2
     ALTITUDE = 3
@@ -152,14 +153,21 @@
     @_class_gen.create_payload_class(FaultType.REGION_BLACKOUT, _class_gen.BoolConstruct)
     class RegionBlackout(_class_gen.Bool):
         """!
         @brief Simulate a region blackout (intended for factory test purposes only).
         """
         pass
 
+    @_class_gen.create_payload_class(FaultType.QUECTEL_TEST, _class_gen.BoolConstruct)
+    class QuectelTest(_class_gen.Bool):
+        """!
+        @brief Enable/disable Quectel test features (intended for factory test purposes only).
+        """
+        pass
+
     FaultControlMessageConstruct = Struct(
         "fault_type" / AutoEnum(Int8ul, FaultType),
         Padding(15),
         "payload_length_bytes" / Int32ul,
         "payload" / Bytes(this.payload_length_bytes),
     )
```

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/gnss_corrections.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/gnss_corrections.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/measurement_details.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/measurement_details.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/measurements.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/measurements.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/ros.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/ros.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/signal_defs.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/signal_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/solution.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/solution.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/messages/timestamp.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/messages/timestamp.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/decoder.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/encoder.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/file_index.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/parsers/mixed_log_reader.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/parsers/mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/argument_parser.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/bin_utils.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/bin_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/construct_utils.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/enum_utils.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/log.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/log.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/numpy_utils.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/time_range.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/time_range.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client/utils/trace.py` & `fusion-engine-client-1.20.0rc5/fusion_engine_client/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/PKG-INFO` & `fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.20.0rc4
+Version: 1.20.0rc5
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.20.0rc4/fusion_engine_client.egg-info/SOURCES.txt` & `fusion-engine-client-1.20.0rc5/fusion_engine_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/setup.py` & `fusion-engine-client-1.20.0rc5/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/tests/test_config.py` & `fusion-engine-client-1.20.0rc5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/tests/test_construct_utils.py` & `fusion-engine-client-1.20.0rc5/tests/test_construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/tests/test_data_loader.py` & `fusion-engine-client-1.20.0rc5/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/tests/test_decoder.py` & `fusion-engine-client-1.20.0rc5/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/tests/test_encoder.py` & `fusion-engine-client-1.20.0rc5/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/tests/test_enum_utils.py` & `fusion-engine-client-1.20.0rc5/tests/test_enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/tests/test_file_index.py` & `fusion-engine-client-1.20.0rc5/tests/test_file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/tests/test_message_defs.py` & `fusion-engine-client-1.20.0rc5/tests/test_message_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/tests/test_mixed_log_reader.py` & `fusion-engine-client-1.20.0rc5/tests/test_mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc4/tests/test_time_range.py` & `fusion-engine-client-1.20.0rc5/tests/test_time_range.py`

 * *Files identical despite different names*


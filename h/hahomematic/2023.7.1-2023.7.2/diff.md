# Comparing `tmp/hahomematic-2023.7.1.tar.gz` & `tmp/hahomematic-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.7.1.tar", last modified: Tue Jul 11 11:07:04 2023, max compression
+gzip compressed data, was "hahomematic-2023.7.2.tar", last modified: Wed Jul 12 10:03:14 2023, max compression
```

## Comparing `hahomematic-2023.7.1.tar` & `hahomematic-2023.7.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.373333 hahomematic-2023.7.1/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/backport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.373333 hahomematic-2023.7.1/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    52761 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    46789 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14379 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.373333 hahomematic-2023.7.1/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    34412 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19878 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:07:04.373333 hahomematic-2023.7.1/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-11 11:07:03.000000 hahomematic-2023.7.1/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-11 11:07:04.000000 hahomematic-2023.7.1/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:07:03.000000 hahomematic-2023.7.1/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:07:02.000000 hahomematic-2023.7.1/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 11:07:04.000000 hahomematic-2023.7.1/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 11:07:04.000000 hahomematic-2023.7.1/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-11 11:06:32.000000 hahomematic-2023.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 11:07:04.377333 hahomematic-2023.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.695116 hahomematic-2023.7.2/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/backport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.695116 hahomematic-2023.7.2/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24363 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52761 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46789 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34412 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24980 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19878 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-12 10:02:40.000000 hahomematic-2023.7.2/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:03:14.695116 hahomematic-2023.7.2/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-12 10:03:14.000000 hahomematic-2023.7.2/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-12 10:03:14.000000 hahomematic-2023.7.2/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:03:14.000000 hahomematic-2023.7.2/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:03:12.000000 hahomematic-2023.7.2/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-12 10:03:14.000000 hahomematic-2023.7.2/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 10:03:14.000000 hahomematic-2023.7.2/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-07-12 10:02:41.000000 hahomematic-2023.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 10:03:14.699116 hahomematic-2023.7.2/setup.cfg
```

### Comparing `hahomematic-2023.7.1/LICENSE` & `hahomematic-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/PKG-INFO` & `hahomematic-2023.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.7.1/README.md` & `hahomematic-2023.7.2/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/__init__.py` & `hahomematic-2023.7.2/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/backport.py` & `hahomematic-2023.7.2/hahomematic/backport.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/caches/dynamic.py` & `hahomematic-2023.7.2/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/caches/persistent.py` & `hahomematic-2023.7.2/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/caches/visibility.py` & `hahomematic-2023.7.2/hahomematic/caches/visibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,43 +84,43 @@
     "WORKING",
 )
 
 # Parameters within the VALUES paramset for which we don't create entities.
 _IGNORED_PARAMETERS: Final[tuple[str, ...]] = (
     "ACCESS_AUTHORIZATION",
     "ACOUSTIC_NOTIFICATION_SELECTION",  # ro
-    "ADAPTION_DRIVE",  # ro"
+    "ADAPTION_DRIVE",  # ro
     "AES_KEY",
-    "ALARM_COUNT",  # ro"
-    "ALL_LEDS",  # ro"
-    "ARROW_DOWN",  # ro"
+    "ALARM_COUNT",  # ro
+    "ALL_LEDS",  # ro
+    "ARROW_DOWN",  # ro
     "ARROW_UP",  # ro
     "BACKLIGHT",  # ro
-    "BEEP",  # ro"
-    "BELL",  # ro"
-    "BLIND",  # ro"
+    "BEEP",  # ro
+    "BELL",  # ro
+    "BLIND",  # ro
     "BOOST_STATE",
     "BOOST_TIME",
     "BOOT",
-    "BULB",  # ro"
+    "BULB",  # ro
     "CLEAR_WINDOW_OPEN_SYMBOL",  # ro
-    "CLOCK",  # ro"
+    "CLOCK",  # ro
     "CONTROL_DIFFERENTIAL_TEMPERATURE",
     "DATE_TIME_UNKNOWN",
     "DECISION_VALUE",
     "DEVICE_IN_BOOTLOADER",
     "DISPLAY_DATA_ALIGNMENT",  # ro
     "DISPLAY_DATA_BACKGROUND_COLOR",  # ro
     "DISPLAY_DATA_COMMIT",  # ro
     "DISPLAY_DATA_ICON",  # ro
     "DISPLAY_DATA_ID",  # ro
     "DISPLAY_DATA_ID",  # ro
     "DISPLAY_DATA_STRING",  # ro
     "DISPLAY_DATA_TEXT_COLOR",  # ro
-    "DOOR",  # ro"
+    "DOOR",  # ro
     "EXTERNAL_CLOCK",
     "FROST_PROTECTION",
     "HUMIDITY_LIMITER",
     "IDENTIFICATION_MODE_KEY_VISUAL",
     "IDENTIFICATION_MODE_LCD_BACKLIGHT",
     "INCLUSION_UNSUPPORTED_DEVICE",
     "INHIBIT",
@@ -130,39 +130,39 @@
     "OLD_LEVEL",  # ro
     "OVERFLOW",
     "OVERRUN",
     "PARTY_SET_POINT_TEMPERATURE",
     "PARTY_TEMPERATURE",
     "PARTY_TIME_END",
     "PARTY_TIME_START",
-    "PHONE",  # ro"
+    "PHONE",  # ro
     "PROCESS",
     "QUICK_VETO_TIME",
     "RAMP_STOP",
     "RELOCK_DELAY",
-    "SCENE",  # ro"
+    "SCENE",  # ro
     "SELF_CALIBRATION",
-    "SERVICE_COUNT",  # ro"
+    "SERVICE_COUNT",  # ro
     "SET_SYMBOL_FOR_HEATING_PHASE",
     "SHADING_SPEED",  # ro
-    "SHEV_POS",  # ro"
-    "SPEED",  # ro"
+    "SHEV_POS",  # ro
+    "SPEED",  # ro
     "STATE_UNCERTAIN",
     "SUBMIT",
     "SWITCH_POINT_OCCURED",
     "TEMPERATURE_LIMITER",
     "TEMPERATURE_OUT_OF_RANGE",
     "TEXT",
     "TIME_OF_OPERATION",
-    "USER_COLOR",  # ro"
-    "USER_PROGRAM",  # ro"
+    "USER_COLOR",  # ro
+    "USER_PROGRAM",  # ro
     "VALVE_ADAPTION",
     "WINDOW",  # ro
     "WIN_RELEASE",
-    "WIN_RELEASE_ACT",  # ro"
+    "WIN_RELEASE_ACT",  # ro
 )
 
 # Ignore Parameter that end with
 _IGNORED_PARAMETERS_WILDCARDS_END: Final[tuple[str, ...]] = (
     "_OVERFLOW",
     "_OVERRUN",
     "_REPORTING",
```

### Comparing `hahomematic-2023.7.1/hahomematic/central_unit.py` & `hahomematic-2023.7.2/hahomematic/central_unit.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/client.py` & `hahomematic-2023.7.2/hahomematic/client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/const.py` & `hahomematic-2023.7.2/hahomematic/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,18 +74,20 @@
 EVENT_CONFIG_PENDING: Final = "CONFIG_PENDING"
 EVENT_ERROR: Final = "ERROR"
 EVENT_UPDATE_PENDING: Final = "UPDATE_PENDING"
 
 EVENT_PONG: Final = "PONG"
 EVENT_PRESS: Final = "PRESS"
 EVENT_PRESS_CONT: Final = "PRESS_CONT"
+EVENT_PRESS_LOCK: Final = "PRESS_LOCK"
 EVENT_PRESS_LONG: Final = "PRESS_LONG"
 EVENT_PRESS_LONG_RELEASE: Final = "PRESS_LONG_RELEASE"
 EVENT_PRESS_LONG_START: Final = "PRESS_LONG_START"
 EVENT_PRESS_SHORT: Final = "PRESS_SHORT"
+EVENT_PRESS_UNLOCK: Final = "PRESS_UNLOCK"
 EVENT_SEQUENCE_OK: Final = "SEQUENCE_OK"
 EVENT_STICKY_UN_REACH: Final = "STICKY_UNREACH"
 EVENT_UN_REACH: Final = "UNREACH"
 
 FILE_CUSTOM_UN_IGNORE_PARAMETERS: Final = "unignore"
 FILE_DEVICES: Final = "homematic_devices.json"
 FILE_PARAMSETS: Final = "homematic_paramsets.json"
@@ -205,18 +207,20 @@
     EVENT_PRESS_LONG_START: ("KEY_BEHAVIOR", "SWITCH_BEHAVIOR"),
     EVENT_PRESS_SHORT: ("KEY_BEHAVIOR", "SWITCH_BEHAVIOR"),
 }
 
 CLICK_EVENTS: Final[tuple[str, ...]] = (
     EVENT_PRESS,
     EVENT_PRESS_CONT,
+    EVENT_PRESS_LOCK,
     EVENT_PRESS_LONG,
     EVENT_PRESS_LONG_RELEASE,
     EVENT_PRESS_LONG_START,
     EVENT_PRESS_SHORT,
+    EVENT_PRESS_UNLOCK,
 )
 
 DEVICE_ERROR_EVENTS: Final[tuple[str, ...]] = ("ERROR", "SENSOR_ERROR")
 
 IMPULSE_EVENTS: Final[tuple[str, ...]] = (EVENT_SEQUENCE_OK,)
 
 BUTTON_ACTIONS: Final[tuple[str, ...]] = ("RESET_MOTION", "RESET_PRESENCE")
```

### Comparing `hahomematic-2023.7.1/hahomematic/decorators.py` & `hahomematic-2023.7.2/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/exceptions.py` & `hahomematic-2023.7.2/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/exporter.py` & `hahomematic-2023.7.2/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/hmcli.py` & `hahomematic-2023.7.2/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/json_rpc_client.py` & `hahomematic-2023.7.2/hahomematic/json_rpc_client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/__init__.py` & `hahomematic-2023.7.2/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.7.2/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.7.2/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/custom/const.py` & `hahomematic-2023.7.2/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.7.2/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.7.2/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.7.2/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/custom/light.py` & `hahomematic-2023.7.2/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.7.2/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.7.2/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/custom/support.py` & `hahomematic-2023.7.2/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.7.2/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/device.py` & `hahomematic-2023.7.2/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/entity.py` & `hahomematic-2023.7.2/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/event.py` & `hahomematic-2023.7.2/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.7.2/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/generic/action.py` & `hahomematic-2023.7.2/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.7.2/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/generic/button.py` & `hahomematic-2023.7.2/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.7.2/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/generic/number.py` & `hahomematic-2023.7.2/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/generic/select.py` & `hahomematic-2023.7.2/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.7.2/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.7.2/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.7.2/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.7.2/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/hub/button.py` & `hahomematic-2023.7.2/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.7.2/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/hub/number.py` & `hahomematic-2023.7.2/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/hub/select.py` & `hahomematic-2023.7.2/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.7.2/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/hub/text.py` & `hahomematic-2023.7.2/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/support.py` & `hahomematic-2023.7.2/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/platforms/update.py` & `hahomematic-2023.7.2/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.7.2/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.7.2/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.7.2/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/support.py` & `hahomematic-2023.7.2/hahomematic/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.7.2/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic/xml_rpc_server.py` & `hahomematic-2023.7.2/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.7.2/hahomematic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.7.1/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.7.2/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.7.1/pyproject.toml` & `hahomematic-2023.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.7.1"
+version     = "2023.7.2"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```


# Comparing `tmp/dashio-3.3.6.tar.gz` & `tmp/dashio-3.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashio-3.3.6.tar", last modified: Wed Apr 26 04:43:05 2023, max compression
+gzip compressed data, was "dashio-3.3.7.tar", last modified: Tue Jul 11 22:05:24 2023, max compression
```

## Comparing `dashio-3.3.6.tar` & `dashio-3.3.7.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.631092 dashio-3.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 04:42:55.000000 dashio-3.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-26 04:43:05.631092 dashio-3.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-26 04:42:55.000000 dashio-3.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.623092 dashio-3.3.6/dashio/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.627092 dashio-3.3.6/dashio/action_station_services/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/action_station_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/as_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/clock_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/modbus_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/timer_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/bleconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.627092 dashio-3.3.6/dashio/iotcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/audio_visual_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/knob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/ring_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/mqttconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/serialconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/zeroconf_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/zmqconnection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.627092 dashio-3.3.6/dashio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-26 04:43:05.000000 dashio-3.3.6/dashio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-26 04:43:05.000000 dashio-3.3.6/dashio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:43:05.000000 dashio-3.3.6/dashio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:43:05.000000 dashio-3.3.6/dashio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-26 04:43:05.000000 dashio-3.3.6/dashio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 04:43:05.000000 dashio-3.3.6/dashio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-26 04:42:55.000000 dashio-3.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-26 04:43:05.631092 dashio-3.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-26 04:42:55.000000 dashio-3.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.631092 dashio-3.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_dashdevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_knob.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_mqttconntection.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_zqmconnection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.631092 dashio-3.3.6/utilities/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-04-26 04:42:55.000000 dashio-3.3.6/utilities/c64_decode
--rwxr-xr-x   0 runner    (1001) docker     (123)     1709 2023-04-26 04:42:55.000000 dashio-3.3.6/utilities/c64_encode
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.647575 dashio-3.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 22:05:15.000000 dashio-3.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-11 22:05:24.647575 dashio-3.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-07-11 22:05:15.000000 dashio-3.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.639575 dashio-3.3.7/dashio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.639575 dashio-3.3.7/dashio/action_station_services/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/action_station_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/as_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/clock_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/modbus_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/action_station_services/timer_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/bleconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.643575 dashio-3.3.7/dashio/iotcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/audio_visual_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/ring_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/iotcontrol/time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/mqttconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/serialconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/zeroconf_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-11 22:05:15.000000 dashio-3.3.7/dashio/zmqconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.639575 dashio-3.3.7/dashio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-11 22:05:24.000000 dashio-3.3.7/dashio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-11 22:05:24.000000 dashio-3.3.7/dashio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:05:24.000000 dashio-3.3.7/dashio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:05:24.000000 dashio-3.3.7/dashio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 22:05:24.000000 dashio-3.3.7/dashio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 22:05:24.000000 dashio-3.3.7/dashio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-11 22:05:15.000000 dashio-3.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-11 22:05:24.647575 dashio-3.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-11 22:05:15.000000 dashio-3.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.647575 dashio-3.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_dashdevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_mqttconntection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:15.000000 dashio-3.3.7/tests/test_zqmconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:05:24.647575 dashio-3.3.7/utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-07-11 22:05:15.000000 dashio-3.3.7/utilities/c64_decode
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1726 2023-07-11 22:05:15.000000 dashio-3.3.7/utilities/c64_encode
```

### Comparing `dashio-3.3.6/LICENSE` & `dashio-3.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/PKG-INFO` & `dashio-3.3.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashio
-Version: 3.3.6
+Version: 3.3.7
 Summary: DashIO interface library
 Home-page: https://dashio.io
 Download-URL: https://github.com/dashio-connect/python-dashio
 Author: James Boulton
 Author-email: james@dashio.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
@@ -14,19 +14,29 @@
 Provides-Extra: testing
 License-File: LICENSE
 
 # python-dashio
 
 ![Tests](https://github.com/dashio-connect/python-dashio/actions/workflows/tests.yml/badge.svg)
 
-[**python-dashio**](http://www.dashio.io) - It is a quick effortless way to connect your IoT device to your phone, tablet or iPad using the free **Dash** app. It allows easy setup of controls such as Dials, Text Boxes, Charts, Graphs, Notifications..., from your IoT device. You can define the look and layout of the controls on your phone from your IoT device. There are three methods to connect to your phone; Bluetooth Low Energy (BLE), TCP or MQTT.
+[**python-dashio**](http://dashio.io) - Create beautiful mobile dashboards for your python project. It is a quick effortless way to connect your python code to your phone, tablet or iPad using the free [**Dash**](https://apps.apple.com/us/app/dash-iot/id1574116689) app. It allows easy setup of controls such as Dials, Text Boxes, Charts, Graphs, Notifications..., from your IoT device. You can define the look and layout of the controls on your phone from your python code. There are three methods to connect to your phone; Bluetooth Low Energy (BLE - on supported platforms), TCP, and MQTT via the dash.dashio.io server.
 
 ## Getting Started
 
-For the big picture on **DashIO**, take a look at our website: <a href="https://dashio.io">dashio.io</a>
+* For the big picture on **DashIO**, take a look at our website: <a href="https://dashio.io">dashio.io</a>
+
+* Create an account on <a href="https://dashio.io/account-create/">dash.dashio.io</a>
+
+* Get the App:
+
+[<img src=https://raw.githubusercontent.com/dashio-connect/python-dashio/master/Documents/download-on-the-app-store.svg>](<https://apps.apple.com/us/app/dash-iot/id1574116689>)
+
+Android coming soon. If you would like to help us test the android version email to [info@dashio.io](mailto:info@dashio.io) with "Android Beta Tester" in the title.
+
+<img src="https://raw.githubusercontent.com/dashio-connect/python-dashio/master/Documents/Google_Play_Store_badge_EN.svg" width="120"/> 
 
 ## Documentation
 
 For all documentation and software guides: <a href="https://dashio.io/documents">dashio.io/documents</a>
 
 For the **DashIO** Python guide: <a href="https://dashio.io/guide-python">dashio.io/guide-python</a>
 
@@ -191,7 +201,44 @@
 aknob.add_receive_message_callback(knob_event_handler)
 
 while True:
     time.sleep(1)
 ```
 
 We've added the cfg64 string. Then decoded it with *dashio.decode_cfg64(cfg64)*. This function returns a dictionary that we can pass into Device so that it can to instantiate and add the controls.
+
+Included in the library are two commandline utilities to encode and decode cfg64 files.
+
+```sh
+$ c64_decode -h
+usage: c64_decode [-h] [-p] [-o OUT_FILE] [-i INDENT] file
+
+positional arguments:
+  file                  Input file name.
+
+options:
+  -h, --help            show this help message and exit
+  -p, --print           Print output.
+  -o OUT_FILE, --out OUT_FILE
+                        output filename.
+  -i INDENT, --indent INDENT
+                        Indent depth (Default 4).
+```
+
+And
+
+```sh
+$ c64_encode -h
+usage: c64_encode [-h] [-f FORMAT] [-o OUT_FILE] [-w WIDTH] file
+
+positional arguments:
+  file                  Input file name.
+
+options:
+  -h, --help            show this help message and exit
+  -f FORMAT, --format FORMAT
+                        Format output. Options: 'None', 'C', 'Python'.
+  -o OUT_FILE, --out OUT_FILE
+                        output filename.
+  -w WIDTH, --width WIDTH
+                        Width of formatted output (Default 80).
+```
```

### Comparing `dashio-3.3.6/README.md` & `dashio-3.3.7/dashio.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,42 @@
+Metadata-Version: 2.1
+Name: dashio
+Version: 3.3.7
+Summary: DashIO interface library
+Home-page: https://dashio.io
+Download-URL: https://github.com/dashio-connect/python-dashio
+Author: James Boulton
+Author-email: james@dashio.com
+License: MIT
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Operating System :: OS Independent
+Requires-Python: >3.6.0
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+
 # python-dashio
 
 ![Tests](https://github.com/dashio-connect/python-dashio/actions/workflows/tests.yml/badge.svg)
 
-[**python-dashio**](http://www.dashio.io) - It is a quick effortless way to connect your IoT device to your phone, tablet or iPad using the free **Dash** app. It allows easy setup of controls such as Dials, Text Boxes, Charts, Graphs, Notifications..., from your IoT device. You can define the look and layout of the controls on your phone from your IoT device. There are three methods to connect to your phone; Bluetooth Low Energy (BLE), TCP or MQTT.
+[**python-dashio**](http://dashio.io) - Create beautiful mobile dashboards for your python project. It is a quick effortless way to connect your python code to your phone, tablet or iPad using the free [**Dash**](https://apps.apple.com/us/app/dash-iot/id1574116689) app. It allows easy setup of controls such as Dials, Text Boxes, Charts, Graphs, Notifications..., from your IoT device. You can define the look and layout of the controls on your phone from your python code. There are three methods to connect to your phone; Bluetooth Low Energy (BLE - on supported platforms), TCP, and MQTT via the dash.dashio.io server.
 
 ## Getting Started
 
-For the big picture on **DashIO**, take a look at our website: <a href="https://dashio.io">dashio.io</a>
+* For the big picture on **DashIO**, take a look at our website: <a href="https://dashio.io">dashio.io</a>
+
+* Create an account on <a href="https://dashio.io/account-create/">dash.dashio.io</a>
+
+* Get the App:
+
+[<img src=https://raw.githubusercontent.com/dashio-connect/python-dashio/master/Documents/download-on-the-app-store.svg>](<https://apps.apple.com/us/app/dash-iot/id1574116689>)
+
+Android coming soon. If you would like to help us test the android version email to [info@dashio.io](mailto:info@dashio.io) with "Android Beta Tester" in the title.
+
+<img src="https://raw.githubusercontent.com/dashio-connect/python-dashio/master/Documents/Google_Play_Store_badge_EN.svg" width="120"/> 
 
 ## Documentation
 
 For all documentation and software guides: <a href="https://dashio.io/documents">dashio.io/documents</a>
 
 For the **DashIO** Python guide: <a href="https://dashio.io/guide-python">dashio.io/guide-python</a>
 
@@ -175,7 +201,44 @@
 aknob.add_receive_message_callback(knob_event_handler)
 
 while True:
     time.sleep(1)
 ```
 
 We've added the cfg64 string. Then decoded it with *dashio.decode_cfg64(cfg64)*. This function returns a dictionary that we can pass into Device so that it can to instantiate and add the controls.
+
+Included in the library are two commandline utilities to encode and decode cfg64 files.
+
+```sh
+$ c64_decode -h
+usage: c64_decode [-h] [-p] [-o OUT_FILE] [-i INDENT] file
+
+positional arguments:
+  file                  Input file name.
+
+options:
+  -h, --help            show this help message and exit
+  -p, --print           Print output.
+  -o OUT_FILE, --out OUT_FILE
+                        output filename.
+  -i INDENT, --indent INDENT
+                        Indent depth (Default 4).
+```
+
+And
+
+```sh
+$ c64_encode -h
+usage: c64_encode [-h] [-f FORMAT] [-o OUT_FILE] [-w WIDTH] file
+
+positional arguments:
+  file                  Input file name.
+
+options:
+  -h, --help            show this help message and exit
+  -f FORMAT, --format FORMAT
+                        Format output. Options: 'None', 'C', 'Python'.
+  -o OUT_FILE, --out OUT_FILE
+                        output filename.
+  -w WIDTH, --width WIDTH
+                        Width of formatted output (Default 80).
+```
```

### Comparing `dashio-3.3.6/dashio/__init__.py` & `dashio-3.3.7/dashio/__init__.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/action_station.py` & `dashio-3.3.7/dashio/action_station.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/action_station_services/action_station_service_config.py` & `dashio-3.3.7/dashio/action_station_services/action_station_service_config.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/action_station_services/as_servicel.py` & `dashio-3.3.7/dashio/action_station_services/as_servicel.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/action_station_services/clock_servicel.py` & `dashio-3.3.7/dashio/action_station_services/clock_servicel.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/action_station_services/modbus_service.py` & `dashio-3.3.7/dashio/action_station_services/modbus_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/action_station_services/task_service.py` & `dashio-3.3.7/dashio/action_station_services/task_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/action_station_services/timer_service.py` & `dashio-3.3.7/dashio/action_station_services/timer_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/bleconnection.py` & `dashio-3.3.7/dashio/bleconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/constants.py` & `dashio-3.3.7/dashio/constants.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/dashconnection.py` & `dashio-3.3.7/dashio/dashconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/device.py` & `dashio-3.3.7/dashio/device.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/__init__.py` & `dashio-3.3.7/dashio/iotcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/alarm.py` & `dashio-3.3.7/dashio/iotcontrol/alarm.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/audio_visual_display.py` & `dashio-3.3.7/dashio/iotcontrol/audio_visual_display.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/button.py` & `dashio-3.3.7/dashio/iotcontrol/button.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/button_group.py` & `dashio-3.3.7/dashio/iotcontrol/button_group.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/chart.py` & `dashio-3.3.7/dashio/iotcontrol/chart.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/color_picker.py` & `dashio-3.3.7/dashio/iotcontrol/color_picker.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/control.py` & `dashio-3.3.7/dashio/iotcontrol/control.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/device_view.py` & `dashio-3.3.7/dashio/iotcontrol/device_view.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/dial.py` & `dashio-3.3.7/dashio/iotcontrol/dial.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/direction.py` & `dashio-3.3.7/dashio/iotcontrol/direction.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/enums.py` & `dashio-3.3.7/dashio/iotcontrol/enums.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/event.py` & `dashio-3.3.7/dashio/iotcontrol/event.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/event_log.py` & `dashio-3.3.7/dashio/iotcontrol/event_log.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/knob.py` & `dashio-3.3.7/dashio/iotcontrol/knob.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/label.py` & `dashio-3.3.7/dashio/iotcontrol/label.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/map.py` & `dashio-3.3.7/dashio/iotcontrol/map.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/menu.py` & `dashio-3.3.7/dashio/iotcontrol/menu.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/ring_buffer.py` & `dashio-3.3.7/dashio/iotcontrol/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/selector.py` & `dashio-3.3.7/dashio/iotcontrol/selector.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/slider.py` & `dashio-3.3.7/dashio/iotcontrol/slider.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/textbox.py` & `dashio-3.3.7/dashio/iotcontrol/textbox.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/iotcontrol/time_graph.py` & `dashio-3.3.7/dashio/iotcontrol/time_graph.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/ip.py` & `dashio-3.3.7/dashio/ip.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/load_config.py` & `dashio-3.3.7/dashio/load_config.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/mqttconnection.py` & `dashio-3.3.7/dashio/mqttconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/serialconnection.py` & `dashio-3.3.7/dashio/serialconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/tcpconnection.py` & `dashio-3.3.7/dashio/tcpconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/zeroconf_service.py` & `dashio-3.3.7/dashio/zeroconf_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio/zmqconnection.py` & `dashio-3.3.7/dashio/zmqconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/dashio.egg-info/PKG-INFO` & `dashio-3.3.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-Metadata-Version: 2.1
-Name: dashio
-Version: 3.3.6
-Summary: DashIO interface library
-Home-page: https://dashio.io
-Download-URL: https://github.com/dashio-connect/python-dashio
-Author: James Boulton
-Author-email: james@dashio.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Operating System :: OS Independent
-Requires-Python: >3.6.0
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 # python-dashio
 
 ![Tests](https://github.com/dashio-connect/python-dashio/actions/workflows/tests.yml/badge.svg)
 
-[**python-dashio**](http://www.dashio.io) - It is a quick effortless way to connect your IoT device to your phone, tablet or iPad using the free **Dash** app. It allows easy setup of controls such as Dials, Text Boxes, Charts, Graphs, Notifications..., from your IoT device. You can define the look and layout of the controls on your phone from your IoT device. There are three methods to connect to your phone; Bluetooth Low Energy (BLE), TCP or MQTT.
+[**python-dashio**](http://dashio.io) - Create beautiful mobile dashboards for your python project. It is a quick effortless way to connect your python code to your phone, tablet or iPad using the free [**Dash**](https://apps.apple.com/us/app/dash-iot/id1574116689) app. It allows easy setup of controls such as Dials, Text Boxes, Charts, Graphs, Notifications..., from your IoT device. You can define the look and layout of the controls on your phone from your python code. There are three methods to connect to your phone; Bluetooth Low Energy (BLE - on supported platforms), TCP, and MQTT via the dash.dashio.io server.
 
 ## Getting Started
 
-For the big picture on **DashIO**, take a look at our website: <a href="https://dashio.io">dashio.io</a>
+* For the big picture on **DashIO**, take a look at our website: <a href="https://dashio.io">dashio.io</a>
+
+* Create an account on <a href="https://dashio.io/account-create/">dash.dashio.io</a>
+
+* Get the App:
+
+[<img src=https://raw.githubusercontent.com/dashio-connect/python-dashio/master/Documents/download-on-the-app-store.svg>](<https://apps.apple.com/us/app/dash-iot/id1574116689>)
+
+Android coming soon. If you would like to help us test the android version email to [info@dashio.io](mailto:info@dashio.io) with "Android Beta Tester" in the title.
+
+<img src="https://raw.githubusercontent.com/dashio-connect/python-dashio/master/Documents/Google_Play_Store_badge_EN.svg" width="120"/> 
 
 ## Documentation
 
 For all documentation and software guides: <a href="https://dashio.io/documents">dashio.io/documents</a>
 
 For the **DashIO** Python guide: <a href="https://dashio.io/guide-python">dashio.io/guide-python</a>
 
@@ -191,7 +185,44 @@
 aknob.add_receive_message_callback(knob_event_handler)
 
 while True:
     time.sleep(1)
 ```
 
 We've added the cfg64 string. Then decoded it with *dashio.decode_cfg64(cfg64)*. This function returns a dictionary that we can pass into Device so that it can to instantiate and add the controls.
+
+Included in the library are two commandline utilities to encode and decode cfg64 files.
+
+```sh
+$ c64_decode -h
+usage: c64_decode [-h] [-p] [-o OUT_FILE] [-i INDENT] file
+
+positional arguments:
+  file                  Input file name.
+
+options:
+  -h, --help            show this help message and exit
+  -p, --print           Print output.
+  -o OUT_FILE, --out OUT_FILE
+                        output filename.
+  -i INDENT, --indent INDENT
+                        Indent depth (Default 4).
+```
+
+And
+
+```sh
+$ c64_encode -h
+usage: c64_encode [-h] [-f FORMAT] [-o OUT_FILE] [-w WIDTH] file
+
+positional arguments:
+  file                  Input file name.
+
+options:
+  -h, --help            show this help message and exit
+  -f FORMAT, --format FORMAT
+                        Format output. Options: 'None', 'C', 'Python'.
+  -o OUT_FILE, --out OUT_FILE
+                        output filename.
+  -w WIDTH, --width WIDTH
+                        Width of formatted output (Default 80).
+```
```

### Comparing `dashio-3.3.6/dashio.egg-info/SOURCES.txt` & `dashio-3.3.7/dashio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/setup.cfg` & `dashio-3.3.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/setup.py` & `dashio-3.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="dashio",
-    version="3.3.6",
+    version="3.3.7",
     description="DashIO interface library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="James Boulton",
     author_email="james@dashio.com",
     url="https://dashio.io",
     download_url="https://github.com/dashio-connect/python-dashio",
```

### Comparing `dashio-3.3.6/tests/test_button.py` & `dashio-3.3.7/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_button_group.py` & `dashio-3.3.7/tests/test_button_group.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_chart.py` & `dashio-3.3.7/tests/test_chart.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_dashdevice.py` & `dashio-3.3.7/tests/test_dashdevice.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_device_view.py` & `dashio-3.3.7/tests/test_device_view.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_dial.py` & `dashio-3.3.7/tests/test_dial.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_direction.py` & `dashio-3.3.7/tests/test_direction.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_event_log.py` & `dashio-3.3.7/tests/test_event_log.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_knob.py` & `dashio-3.3.7/tests/test_knob.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_label.py` & `dashio-3.3.7/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_map.py` & `dashio-3.3.7/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_menu.py` & `dashio-3.3.7/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_selector.py` & `dashio-3.3.7/tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_slider.py` & `dashio-3.3.7/tests/test_slider.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_textbox.py` & `dashio-3.3.7/tests/test_textbox.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/tests/test_time_graph.py` & `dashio-3.3.7/tests/test_time_graph.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/utilities/c64_decode` & `dashio-3.3.7/utilities/c64_decode`

 * *Files identical despite different names*

### Comparing `dashio-3.3.6/utilities/c64_encode` & `dashio-3.3.7/utilities/c64_encode`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     )
     new_s = '"\\\n"'.join(new_l)
     return '"' + new_s + '"'
 
 def parse_commandline_arguments():
     parser = argparse.ArgumentParser()
     parser.add_argument('file', help="Input file name.")
-    parser.add_argument("-f", "--format", dest="format", default="None", help="Format output. Options: 'None', 'C', 'Python'.")
+    parser.add_argument("-f", "--format", dest="format", default="None", help="Format output. Options: 'None', 'C', 'Python' (Default 'None').")
     parser.add_argument("-o", "--out", dest="out_file", help="output filename.")
     parser.add_argument("-w", "--width", dest="width", default=80, type=int, help="Width of formatted output (Default 80).")
     args = parser.parse_args()
     return args
 
 def main():
     args = parse_commandline_arguments()
```


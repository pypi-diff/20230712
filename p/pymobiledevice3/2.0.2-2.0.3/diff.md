# Comparing `tmp/pymobiledevice3-2.0.2.tar.gz` & `tmp/pymobiledevice3-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymobiledevice3-2.0.2.tar", last modified: Mon Jun 19 10:22:57 2023, max compression
+gzip compressed data, was "pymobiledevice3-2.0.3.tar", last modified: Wed Jul 12 05:36:52 2023, max compression
```

## Comparing `pymobiledevice3-2.0.2.tar` & `pymobiledevice3-2.0.3.tar`

### file list

```diff
@@ -1,149 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:57.476351 pymobiledevice3-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    57629 2023-06-19 10:22:57.472351 pymobiledevice3-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:57.456351 pymobiledevice3-2.0.2/pymobiledevice3/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/bonjour.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/ca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:57.460351 pymobiledevice3-2.0.2/pymobiledevice3/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/afc.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/amfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/bonjour.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/cli_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/companion_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/crash.py
--rw-r--r--   0 runner    (1001) docker     (123)    34760 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/developer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/mounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/power_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/provision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/springboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/cli/webinspector.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/irecv.py
--rw-r--r--   0 runner    (1001) docker     (123)    32198 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/irecv_devices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27360 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/pair_records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:57.464351 pymobiledevice3-2.0.2/pymobiledevice3/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1023280 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/dsc_uuid_map.json
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/dsc_uuid_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/firmware_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    25467 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/notifications.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:57.464351 pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/element_attribute.js
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/element_clear.js
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/enter_fullscreen.js
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/find_nodes.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/focus.js
--rw-r--r--   0 runner    (1001) docker     (123)    42234 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/get_attribute.js
--rw-r--r--   0 runner    (1001) docker     (123)    43072 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/is_displayed.js
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/is_editable.js
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/is_enabled.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:57.468351 pymobiledevice3-2.0.2/pymobiledevice3/restore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/restore/asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/restore/base_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/restore/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/restore/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/restore/fdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/restore/ftab.py
--rw-r--r--   0 runner    (1001) docker     (123)    16325 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/restore/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    49812 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/restore/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/restore/restore_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/restore/restored_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/restore/tss.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6768 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/service_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:57.472351 pymobiledevice3-2.0.2/pymobiledevice3/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/accessibilityaudit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31043 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/afc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/amfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/base_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/companion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/crash_reports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/debugserver_applist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/device_arbitration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/device_link.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6154 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/diagnostics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1441 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dtfetchsymbols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:57.472351 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:57.472351 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/application_listing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/condition_inducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/device_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/energy_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/network_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/process_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/sysmontap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/file_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/heartbeat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/house_arrest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/installation_proxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/misagent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3410 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/mobile_activation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3322 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/mobile_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10734 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/mobile_image_mounter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16752 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/mobilebackup2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1544 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/notification_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/os_trace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9223 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/pcapd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/power_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/preboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/remote_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1270 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/screenshot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1790 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/simulate_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/springboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/syslog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:57.472351 pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/automation_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/cdp_screencast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/cdp_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    32080 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/cdp_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/inspector_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/selenium_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/session_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/switch_to.py
--rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/services/webinspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/tcp_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/usbmux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pymobiledevice3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:57.460351 pymobiledevice3-2.0.2/pymobiledevice3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    57629 2023-06-19 10:22:57.000000 pymobiledevice3-2.0.2/pymobiledevice3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-06-19 10:22:57.000000 pymobiledevice3-2.0.2/pymobiledevice3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:22:57.000000 pymobiledevice3-2.0.2/pymobiledevice3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-19 10:22:57.000000 pymobiledevice3-2.0.2/pymobiledevice3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-19 10:22:57.000000 pymobiledevice3-2.0.2/pymobiledevice3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 10:22:57.000000 pymobiledevice3-2.0.2/pymobiledevice3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 10:22:57.476351 pymobiledevice3-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:22:57.472351 pymobiledevice3-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-19 10:22:41.000000 pymobiledevice3-2.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:52.699082 pymobiledevice3-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    57629 2023-07-12 05:36:52.699082 pymobiledevice3-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:52.679082 pymobiledevice3-2.0.3/pymobiledevice3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/bonjour.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/ca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:52.683082 pymobiledevice3-2.0.3/pymobiledevice3/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/afc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/bonjour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/cli_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/companion_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/crash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34762 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/developer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/mounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/power_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/provision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/springboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11630 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/cli/webinspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/irecv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32198 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/irecv_devices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29015 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/pair_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:52.683082 pymobiledevice3-2.0.3/pymobiledevice3/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/remote/bonjour.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20346 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/remote/core_device_tunnel_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/remote/remote_service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/remote/remotexpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/remote/xpc_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:52.687082 pymobiledevice3-2.0.3/pymobiledevice3/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1023280 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/dsc_uuid_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/dsc_uuid_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/firmware_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25467 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/notifications.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:52.687082 pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/element_attribute.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/element_clear.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/enter_fullscreen.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/find_nodes.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/focus.js
+-rw-r--r--   0 runner    (1001) docker     (123)    42234 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/get_attribute.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43072 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/is_displayed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/is_editable.js
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/is_enabled.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:52.687082 pymobiledevice3-2.0.3/pymobiledevice3/restore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/restore/asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/restore/base_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/restore/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/restore/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/restore/fdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/restore/ftab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16325 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/restore/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49812 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/restore/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/restore/restore_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/restore/restored_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/restore/tss.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6768 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/service_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:52.695082 pymobiledevice3-2.0.3/pymobiledevice3/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/accessibilityaudit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31043 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/afc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/companion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/crash_reports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/debugserver_applist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1153 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/device_arbitration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/device_link.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6154 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/diagnostics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1441 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dtfetchsymbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:52.695082 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:52.695082 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/application_listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/condition_inducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/energy_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/network_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/process_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/sysmontap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/file_relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/heartbeat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/house_arrest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/installation_proxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1894 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/misagent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3410 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/mobile_activation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4517 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/mobile_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13592 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/mobile_image_mounter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16752 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/mobilebackup2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1544 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/notification_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/os_trace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9223 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/pcapd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/power_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/preboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/remote_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1270 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/screenshot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1790 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/simulate_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/springboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/syslog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:52.699082 pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/automation_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/cdp_screencast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/cdp_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32080 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/cdp_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/inspector_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/selenium_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/session_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/switch_to.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/services/webinspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/tcp_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pymobiledevice3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:52.679082 pymobiledevice3-2.0.3/pymobiledevice3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    57629 2023-07-12 05:36:52.000000 pymobiledevice3-2.0.3/pymobiledevice3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-12 05:36:52.000000 pymobiledevice3-2.0.3/pymobiledevice3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 05:36:52.000000 pymobiledevice3-2.0.3/pymobiledevice3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-12 05:36:52.000000 pymobiledevice3-2.0.3/pymobiledevice3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-12 05:36:52.000000 pymobiledevice3-2.0.3/pymobiledevice3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 05:36:52.000000 pymobiledevice3-2.0.3/pymobiledevice3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 05:36:52.699082 pymobiledevice3-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:36:52.699082 pymobiledevice3-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-12 05:36:36.000000 pymobiledevice3-2.0.3/tests/test_utils.py
```

### Comparing `pymobiledevice3-2.0.2/LICENSE` & `pymobiledevice3-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/PKG-INFO` & `pymobiledevice3-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymobiledevice3
-Version: 2.0.2
+Version: 2.0.3
 Summary: Pure python3 implementation for working with iDevices (iPhone, etc...)
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `pymobiledevice3-2.0.2/README.md` & `pymobiledevice3-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/__main__.py` & `pymobiledevice3-2.0.3/pymobiledevice3/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,42 +19,46 @@
 from pymobiledevice3.cli.mounter import cli as mounter_cli
 from pymobiledevice3.cli.notification import cli as notification_cli
 from pymobiledevice3.cli.pcap import cli as pcap_cli
 from pymobiledevice3.cli.power_assertion import cli as power_assertion_cli
 from pymobiledevice3.cli.processes import cli as ps_cli
 from pymobiledevice3.cli.profile import cli as profile_cli
 from pymobiledevice3.cli.provision import cli as provision_cli
+from pymobiledevice3.cli.remote import cli as remote_cli
 from pymobiledevice3.cli.restore import cli as restore_cli
 from pymobiledevice3.cli.springboard import cli as springboard_cli
 from pymobiledevice3.cli.syslog import cli as syslog_cli
 from pymobiledevice3.cli.usbmux import cli as usbmux_cli
 from pymobiledevice3.cli.webinspector import cli as webinspector_cli
 from pymobiledevice3.exceptions import ConnectionFailedError, DeveloperModeError, DeveloperModeIsNotEnabledError, \
     DeviceHasPasscodeSetError, InternalError, InvalidServiceError, MessageNotSupportedError, MissingValueError, \
     NoDeviceConnectedError, NoDeviceSelectedError, NotPairedError, PairingDialogResponsePendingError, \
     PasswordRequiredError, SetProhibitedError, UserDeniedPairingError
 
 coloredlogs.install(level=logging.INFO)
 
+logging.getLogger('quic').disabled = True
 logging.getLogger('asyncio').disabled = True
+logging.getLogger('zeroconf').disabled = True
 logging.getLogger('parso.cache').disabled = True
 logging.getLogger('parso.cache.pickle').disabled = True
 logging.getLogger('parso.python.diff').disabled = True
 logging.getLogger('humanfriendly.prompts').disabled = True
 logging.getLogger('blib2to3.pgen2.driver').disabled = True
 logging.getLogger('urllib3.connectionpool').disabled = True
 
 logger = logging.getLogger(__name__)
 
 
 def cli():
     cli_commands = click.CommandCollection(sources=[
         developer_cli, mounter_cli, apps_cli, profile_cli, lockdown_cli, diagnostics_cli, syslog_cli, pcap_cli,
         crash_cli, afc_cli, ps_cli, notification_cli, usbmux_cli, power_assertion_cli, springboard_cli,
-        provision_cli, backup_cli, restore_cli, activation_cli, companion_cli, webinspector_cli, amfi_cli, bonjour_cli
+        provision_cli, backup_cli, restore_cli, activation_cli, companion_cli, webinspector_cli, amfi_cli, bonjour_cli,
+        remote_cli
     ])
     cli_commands.context_settings = dict(help_option_names=['-h', '--help'])
     try:
         cli_commands()
     except NoDeviceConnectedError:
         logger.error('Device is not connected')
     except ConnectionAbortedError:
```

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/bonjour.py` & `pymobiledevice3-2.0.3/pymobiledevice3/bonjour.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/ca.py` & `pymobiledevice3-2.0.3/pymobiledevice3/ca.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/activation.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/activation.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/afc.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/afc.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/amfi.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/amfi.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/apps.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/apps.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/backup.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/backup.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/bonjour.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/bonjour.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/cli_common.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/cli_common.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import datetime
 import json
 import logging
 import os
 import uuid
+from typing import List, Optional
 
 import click
 import coloredlogs
 import hexdump
-import inquirer
-from inquirer.themes import GreenPassion
+import inquirer3
+from inquirer3.themes import GreenPassion
 from pygments import formatters, highlight, lexers
 
 from pymobiledevice3.exceptions import NoDeviceSelectedError
 from pymobiledevice3.lockdown import LockdownClient, create_using_usbmux
 from pymobiledevice3.usbmux import select_devices_by_connection_type
 
 
@@ -51,63 +52,47 @@
 def wait_return():
     input('> Hit RETURN to exit')
 
 
 UDID_ENV_VAR = 'PYMOBILEDEVICE3_UDID'
 
 
-class DeviceInfo:
-    def __init__(self, lockdown_client: LockdownClient):
-        self.lockdown_client = lockdown_client
-        self.product_version = self.lockdown_client.product_version
-        self.serial = self.lockdown_client.identifier
-        self.display_name = self.lockdown_client.display_name
-
-    def __str__(self):
-        if self.display_name is None:
-            return f'Unknown device, ios version: {self.product_version}, serial: {self.serial}'
-        else:
-            return f'{self.display_name}, ios version: {self.product_version}, serial: {self.serial}'
+def prompt_device_list(device_list: List):
+    device_question = [inquirer3.List('device', message='choose device', choices=device_list, carousel=True)]
+    try:
+        result = inquirer3.prompt(device_question, theme=GreenPassion(), raise_keyboard_interrupt=True)
+        return result['device']
+    except KeyboardInterrupt:
+        raise NoDeviceSelectedError()
 
 
 class Command(click.Command):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.params[:0] = [
             click.Option(('lockdown', '--udid'), envvar=UDID_ENV_VAR, callback=self.udid,
                          help=f'Device unique identifier. You may pass {UDID_ENV_VAR} environment variable to pass this'
                               f' option as well'),
             click.Option(('verbosity', '-v', '--verbose'), count=True, callback=set_verbosity, expose_value=False),
         ]
 
     @staticmethod
-    def udid(ctx, param, value):
+    def udid(ctx, param: str, value: str) -> Optional[LockdownClient]:
         if '_PYMOBILEDEVICE3_COMPLETE' in os.environ:
             # prevent lockdown connection establishment when in autocomplete mode
             return
 
         if value is not None:
             return create_using_usbmux(serial=value)
 
         devices = select_devices_by_connection_type(connection_type='USB')
         if len(devices) <= 1:
             return create_using_usbmux()
 
-        devices_options = []
-        for device in devices:
-            lockdown_client = create_using_usbmux(serial=device.serial)
-            device_info = DeviceInfo(lockdown_client)
-            devices_options.append(device_info)
-
-        device_question = [inquirer.List('device', message='choose device', choices=devices_options, carousel=True)]
-        try:
-            result = inquirer.prompt(device_question, theme=GreenPassion(), raise_keyboard_interrupt=True)
-            return result['device'].lockdown_client
-        except KeyboardInterrupt as e:
-            raise NoDeviceSelectedError from e
+        return prompt_device_list([create_using_usbmux(serial=device.serial) for device in devices])
 
 
 class CommandWithoutAutopair(Command):
     @staticmethod
     def udid(ctx, param, value):
         if '_PYMOBILEDEVICE3_COMPLETE' in os.environ:
             # prevent lockdown connection establishment when in autocomplete mode
```

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/companion_proxy.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/companion_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/crash.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/crash.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/developer.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/developer.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,16 +218,16 @@
 def netstat(lockdown: LockdownClient):
     """ Print information about current network activity. """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
         with NetworkMonitor(dvt) as monitor:
             for event in monitor:
                 if isinstance(event, ConnectionDetectionEvent):
                     logger.info(
-                        f'Connection detected: {event.local_address.data.address}:{event.local_address.port} -> '
-                        f'{event.remote_address.data.address}:{event.remote_address.port}')
+                        f'Connection detected: {event.local_address.data.hostname}:{event.local_address.port} -> '
+                        f'{event.remote_address.data.hostname}:{event.remote_address.port}')
 
 
 @dvt.command('screenshot', cls=Command)
 @click.argument('out', type=click.File('wb'))
 def screenshot(lockdown: LockdownClient, out):
     """ get device screenshot """
     with DvtSecureSocketProxyService(lockdown=lockdown) as dvt:
```

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/diagnostics.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/diagnostics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/lockdown.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/lockdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,17 +68,18 @@
 @click.option('--color/--no-color', default=True)
 def lockdown_remove(lockdown: LockdownClient, domain, key, color):
     """ remove a domain/key pair """
     print_json(lockdown.remove_value(domain=domain, key=key), colored=color)
 
 
 @lockdown_group.command('unpair', cls=CommandWithoutAutopair)
-def lockdown_unpair(lockdown: LockdownClient):
+@click.argument('host_id', required=False)
+def lockdown_unpair(lockdown: LockdownClient, host_id: str = None):
     """ unpair from connected device """
-    lockdown.unpair()
+    lockdown.unpair(host_id=host_id)
 
 
 @lockdown_group.command('pair', cls=CommandWithoutAutopair)
 def lockdown_pair(lockdown: LockdownClient):
     """ pair device """
     lockdown.pair()
```

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/notification.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/notification.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/pcap.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/pcap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/power_assertion.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/power_assertion.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/processes.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/processes.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/profile.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/profile.py`

 * *Files 25% similar despite different names*

```diff
@@ -33,14 +33,29 @@
     """ install given profiles """
     service = MobileConfigService(lockdown=lockdown)
     for profile in profiles:
         logger.info(f'installing {profile.name}')
         service.install_profile(profile.read())
 
 
+@profile_group.command('install-silent', cls=Command)
+@click.option('--keystore', type=click.File('rb'), required=True,
+              help="A PKCS#12 keystore containing the certificate and private key which can supervise the device.")
+@click.option('--keystore-password', prompt=True, required=True, hide_input=True,
+              help="The password for the PKCS#12 keystore.")
+@click.argument('profiles', nargs=-1, type=click.File('rb'))
+def profile_install_silent(lockdown: LockdownClient, profiles, keystore, keystore_password):
+    """ install given profiles without user interaction (requires the device to be supervised) """
+    service = MobileConfigService(lockdown=lockdown)
+    for profile in profiles:
+        logger.info(f'installing {profile.name}')
+        service.install_profile_silent(
+            profile.read(), keystore.read(), keystore_password)
+
+
 @profile_group.command('cloud-configuration', cls=Command)
 @click.option('--color/--no-color', default=True)
 def profile_cloud_configuration(lockdown: LockdownClient, color):
     """ get cloud configuration """
     print_json(MobileConfigService(lockdown=lockdown).get_cloud_configuration(), colored=color)
```

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/provision.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/provision.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/restore.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/restore.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/springboard.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/springboard.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/syslog.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/syslog.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/usbmux.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/usbmux.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/cli/webinspector.py` & `pymobiledevice3-2.0.3/pymobiledevice3/cli/webinspector.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import logging
 from abc import ABC, abstractmethod
 from contextlib import asynccontextmanager
 from functools import update_wrapper
 from typing import Optional, Type
 
 import click
-import inquirer
+import inquirer3
 import IPython
 import uvicorn
-from inquirer.themes import GreenPassion
+from inquirer3.themes import GreenPassion
 from prompt_toolkit import HTML, PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.lexers import PygmentsLexer
 from prompt_toolkit.patch_stdout import patch_stdout
 from prompt_toolkit.styles import style_from_pygments_cls
 from pygments import formatters, highlight, lexers
@@ -332,16 +332,16 @@
     def query_page(inspector: WebinspectorService) -> Optional[Page]:
         reload_pages(inspector)
         available_pages = list(inspector.get_open_pages().get('Safari', []))
         if not available_pages:
             logger.error('Unable to find available pages (try to unlock device)')
             return
 
-        page_query = [inquirer.List('page', message='choose page', choices=available_pages, carousel=True)]
-        page = inquirer.prompt(page_query, theme=GreenPassion(), raise_keyboard_interrupt=True)['page']
+        page_query = [inquirer3.List('page', message='choose page', choices=available_pages, carousel=True)]
+        page = inquirer3.prompt(page_query, theme=GreenPassion(), raise_keyboard_interrupt=True)['page']
         return page
 
 
 async def run_js_shell(js_shell_class: Type[JsShell], lockdown: LockdownClient,
                        timeout: float, url: str):
     async with js_shell_class.create(lockdown, timeout, SAFARI) as js_shell_instance:
         await js_shell_instance.start(url)
```

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/exceptions.py` & `pymobiledevice3-2.0.3/pymobiledevice3/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,19 @@
 
 
 class ConnectionTerminatedError(PyMobileDevice3Exception):
     """ Raise when a connection is terminated abruptly. """
     pass
 
 
+class StreamClosedError(ConnectionTerminatedError):
+    """ Raise when trying to send a message on a closed stream. """
+    pass
+
+
 class WebInspectorNotEnabledError(PyMobileDevice3Exception):
     """ Raise when Web Inspector is not enabled. """
     pass
 
 
 class RemoteAutomationNotEnabledError(PyMobileDevice3Exception):
     """ Raise when Web Inspector remote automation is not enabled. """
@@ -183,14 +188,19 @@
 
 
 class DeveloperModeIsNotEnabledError(PyMobileDevice3Exception):
     """ Raise when mounting failed because developer mode is not enabled. """
     pass
 
 
+class DeveloperDiskImageNotFoundError(PyMobileDevice3Exception):
+    """ Failed to locate the correct DeveloperDiskImage.dmg """
+    pass
+
+
 class DeveloperModeError(PyMobileDevice3Exception):
     """ Raise when amfid failed to enable developer mode. """
     pass
 
 
 class LockdownError(PyMobileDevice3Exception):
     """ lockdown general error """
```

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/irecv.py` & `pymobiledevice3-2.0.3/pymobiledevice3/irecv.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/irecv_devices.py` & `pymobiledevice3-2.0.3/pymobiledevice3/irecv_devices.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/lockdown.py` & `pymobiledevice3-2.0.3/pymobiledevice3/lockdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -662,7 +662,39 @@
     """
     service = ServiceConnection.create_using_tcp(hostname, port)
     client = TcpLockdownClient.create(
         service, identifier=identifier, label=label, local_hostname=local_hostname, pair_record=pair_record,
         pairing_records_cache_folder=pairing_records_cache_folder, pair_timeout=pair_timeout, autopair=autopair,
         port=port, hostname=hostname)
     return client
+
+
+def create_using_remote(hostname: str, identifier: str = None, label: str = DEFAULT_LABEL, autopair: bool = True,
+                        pair_timeout: int = None, local_hostname: str = None, pair_record: Mapping = None,
+                        pairing_records_cache_folder: Path = None,
+                        port: int = SERVICE_PORT) -> TcpLockdownClient:
+    """
+    Create a TcpLockdownClient instance over RSD
+
+    :param hostname: The target device hostname
+    :param identifier: Used as an identifier to look for the device pair record
+    :param label: lockdownd user-agent
+    :param autopair: Attempt to pair with device (blocking) if not already paired
+    :param pair_timeout: Timeout for autopair
+    :param local_hostname: Used as a seed to generate the HostID
+    :param pair_record: Use this pair record instead of the default behavior (search in host/create our own)
+    :param pairing_records_cache_folder: Use the following location to search and save pair records
+    :param port: lockdownd service port
+    :return: TcpLockdownClient instance
+    """
+    service = ServiceConnection.create_using_tcp(hostname, port)
+    service.send_plist({'Label': label, 'ProtocolVersion': '2', 'Request': 'RSDCheckin'})
+
+    # we expect two responses after the first request
+    service.recv_plist()
+    service.recv_plist()
+
+    client = TcpLockdownClient.create(
+        service, identifier=identifier, label=label, local_hostname=local_hostname, pair_record=pair_record,
+        pairing_records_cache_folder=pairing_records_cache_folder, pair_timeout=pair_timeout, autopair=autopair,
+        port=port, hostname=hostname)
+    return client
```

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/pair_records.py` & `pymobiledevice3-2.0.3/pymobiledevice3/pair_records.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/resources/dsc_uuid_map.json` & `pymobiledevice3-2.0.3/pymobiledevice3/resources/dsc_uuid_map.json`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/resources/dsc_uuid_map.py` & `pymobiledevice3-2.0.3/pymobiledevice3/resources/dsc_uuid_map.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/resources/firmware_notifications.py` & `pymobiledevice3-2.0.3/pymobiledevice3/resources/firmware_notifications.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/resources/notifications.txt` & `pymobiledevice3-2.0.3/pymobiledevice3/resources/notifications.txt`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/element_clear.js` & `pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/element_clear.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/enter_fullscreen.js` & `pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/enter_fullscreen.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/find_nodes.js` & `pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/find_nodes.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/get_attribute.js` & `pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/get_attribute.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/is_displayed.js` & `pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/is_displayed.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/is_editable.js` & `pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/is_editable.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/resources/webinspector/is_enabled.js` & `pymobiledevice3-2.0.3/pymobiledevice3/resources/webinspector/is_enabled.js`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/restore/asr.py` & `pymobiledevice3-2.0.3/pymobiledevice3/restore/asr.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/restore/base_restore.py` & `pymobiledevice3-2.0.3/pymobiledevice3/restore/base_restore.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/restore/consts.py` & `pymobiledevice3-2.0.3/pymobiledevice3/restore/consts.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/restore/device.py` & `pymobiledevice3-2.0.3/pymobiledevice3/restore/device.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/restore/fdr.py` & `pymobiledevice3-2.0.3/pymobiledevice3/restore/fdr.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/restore/ftab.py` & `pymobiledevice3-2.0.3/pymobiledevice3/restore/ftab.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/restore/recovery.py` & `pymobiledevice3-2.0.3/pymobiledevice3/restore/recovery.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/restore/restore.py` & `pymobiledevice3-2.0.3/pymobiledevice3/restore/restore.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/restore/restore_options.py` & `pymobiledevice3-2.0.3/pymobiledevice3/restore/restore_options.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/restore/restored_client.py` & `pymobiledevice3-2.0.3/pymobiledevice3/restore/restored_client.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/restore/tss.py` & `pymobiledevice3-2.0.3/pymobiledevice3/restore/tss.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/service_connection.py` & `pymobiledevice3-2.0.3/pymobiledevice3/service_connection.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/accessibilityaudit.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/accessibilityaudit.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/afc.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/afc.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/amfi.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/amfi.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/base_service.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/base_service.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/companion.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/companion.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/crash_reports.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/crash_reports.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/debugserver_applist.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/debugserver_applist.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/device_arbitration.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/device_arbitration.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/device_link.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/device_link.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/diagnostics.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/diagnostics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/dtfetchsymbols.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/dtfetchsymbols.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/application_listing.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/application_listing.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/condition_inducer.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/condition_inducer.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/device_info.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/device_info.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/energy_monitor.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/energy_monitor.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/graphics.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/graphics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/network_monitor.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/network_monitor.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/notifications.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/notifications.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/process_control.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/process_control.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/dvt/instruments/sysmontap.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/dvt/instruments/sysmontap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/file_relay.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/file_relay.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/heartbeat.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/house_arrest.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/house_arrest.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/installation_proxy.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/installation_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/misagent.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/misagent.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/mobile_activation.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/mobile_activation.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/mobile_image_mounter.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/mobile_image_mounter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import hashlib
 import plistlib
 from pathlib import Path
 from typing import List, Mapping
 
-from pymobiledevice3.exceptions import AlreadyMountedError, DeveloperModeIsNotEnabledError, InternalError, \
-    MessageNotSupportedError, MissingManifestError, NotMountedError, PyMobileDevice3Exception, \
-    UnsupportedCommandError
+from developer_disk_image.repo import DeveloperDiskImageRepository
+from packaging.version import Version
+
+from pymobiledevice3.common import get_home_folder
+from pymobiledevice3.exceptions import AlreadyMountedError, DeveloperDiskImageNotFoundError, \
+    DeveloperModeIsNotEnabledError, InternalError, MessageNotSupportedError, MissingManifestError, NotMountedError, \
+    PyMobileDevice3Exception, UnsupportedCommandError
 from pymobiledevice3.lockdown import LockdownClient
 from pymobiledevice3.restore.tss import TSSRequest
 from pymobiledevice3.services.base_service import BaseService
 
 
 class MobileImageMounterService(BaseService):
     # implemented in /usr/libexec/mobile_storage_proxy
@@ -273,7 +277,73 @@
             if manifest_entry.get('Digest') is None:
                 tss_entry['Digest'] = bytes()
 
             request.update({key: tss_entry})
 
         response = request.send_receive()
         return response['ApImg4Ticket']
+
+
+def auto_mount_developer(lockdown: LockdownClient, xcode: str = None, version: str = None) -> None:
+    """ auto-detect correct DeveloperDiskImage and mount it """
+    if xcode is None:
+        # avoid "default"-ing this option, because Windows and Linux won't have this path
+        xcode = Path('/Applications/Xcode.app')
+        if not (xcode.exists()):
+            xcode = get_home_folder() / 'Xcode.app'
+            xcode.mkdir(parents=True, exist_ok=True)
+
+    image_mounter = DeveloperDiskImageMounter(lockdown=lockdown)
+    if image_mounter.is_image_mounted('Developer'):
+        raise AlreadyMountedError()
+
+    if version is None:
+        version = lockdown.sanitized_ios_version
+    image_dir = f'{xcode}/Contents/Developer/Platforms/iPhoneOS.platform/DeviceSupport/{version}'
+    image_path = f'{image_dir}/DeveloperDiskImage.dmg'
+    signature = f'{image_path}.signature'
+    developer_disk_image_dir = Path(image_path).parent
+
+    image_path = Path(image_path)
+    signature = Path(signature)
+
+    if not image_path.exists():
+        # download the DeveloperDiskImage from our repository
+        repo = DeveloperDiskImageRepository.create()
+        developer_disk_image = repo.get_developer_disk_image(version)
+
+        if developer_disk_image is None:
+            raise DeveloperDiskImageNotFoundError()
+
+        # write it filesystem
+        developer_disk_image_dir.mkdir(exist_ok=True, parents=True)
+        image_path.write_bytes(developer_disk_image.image)
+        signature.write_bytes(developer_disk_image.signature)
+
+    image_mounter.mount(image_path, signature)
+
+
+def auto_mount_personalized(lockdown: LockdownClient) -> None:
+    local_path = get_home_folder() / 'Xcode_iOS_DDI_Personalized'
+    local_path.mkdir(parents=True, exist_ok=True)
+
+    image = local_path / 'Image.dmg'
+    build_manifest = local_path / 'BuildManifest.plist'
+    trustcache = local_path / 'Image.trustcache'
+
+    if not image.exists():
+        # download the Personalized image from our repository
+        repo = DeveloperDiskImageRepository.create()
+        personalized_image = repo.get_personalized_disk_image()
+
+        image.write_bytes(personalized_image.image)
+        build_manifest.write_bytes(personalized_image.build_manifest)
+        trustcache.write_bytes(personalized_image.trustcache)
+
+    PersonalizedImageMounter(lockdown=lockdown).mount(image, build_manifest, trustcache)
+
+
+def auto_mount(lockdown: LockdownClient, xcode: str = None, version: str = None) -> None:
+    if Version(lockdown.product_version) < Version('17.0'):
+        auto_mount_developer(lockdown, xcode=xcode, version=version)
+    else:
+        auto_mount_personalized(lockdown)
```

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/mobilebackup2.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/mobilebackup2.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/notification_proxy.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/notification_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/os_trace.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/os_trace.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/pcapd.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/pcapd.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/power_assertion.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/power_assertion.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/preboard.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/preboard.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/remote_server.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/remote_server.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/screenshot.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/screenshot.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/simulate_location.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/simulate_location.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/springboard.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/springboard.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/syslog.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/syslog.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/alert.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/alert.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/automation_session.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/automation_session.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/cdp_screencast.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/cdp_screencast.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/cdp_server.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/cdp_server.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/cdp_target.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/cdp_target.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/driver.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/driver.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/element.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/element.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/inspector_session.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/inspector_session.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/selenium_api.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/selenium_api.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/session_protocol.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/session_protocol.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/web_protocol/switch_to.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/web_protocol/switch_to.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/services/webinspector.py` & `pymobiledevice3-2.0.3/pymobiledevice3/services/webinspector.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/tcp_forwarder.py` & `pymobiledevice3-2.0.3/pymobiledevice3/tcp_forwarder.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/usbmux.py` & `pymobiledevice3-2.0.3/pymobiledevice3/usbmux.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3/utils.py` & `pymobiledevice3-2.0.3/pymobiledevice3/utils.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3.egg-info/PKG-INFO` & `pymobiledevice3-2.0.3/pymobiledevice3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymobiledevice3
-Version: 2.0.2
+Version: 2.0.3
 Summary: Pure python3 implementation for working with iDevices (iPhone, etc...)
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `pymobiledevice3-2.0.2/pymobiledevice3.egg-info/SOURCES.txt` & `pymobiledevice3-2.0.3/pymobiledevice3.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,26 @@
 pymobiledevice3/cli/mounter.py
 pymobiledevice3/cli/notification.py
 pymobiledevice3/cli/pcap.py
 pymobiledevice3/cli/power_assertion.py
 pymobiledevice3/cli/processes.py
 pymobiledevice3/cli/profile.py
 pymobiledevice3/cli/provision.py
+pymobiledevice3/cli/remote.py
 pymobiledevice3/cli/restore.py
 pymobiledevice3/cli/springboard.py
 pymobiledevice3/cli/syslog.py
 pymobiledevice3/cli/usbmux.py
 pymobiledevice3/cli/webinspector.py
+pymobiledevice3/remote/__init__.py
+pymobiledevice3/remote/bonjour.py
+pymobiledevice3/remote/core_device_tunnel_service.py
+pymobiledevice3/remote/remote_service_discovery.py
+pymobiledevice3/remote/remotexpc.py
+pymobiledevice3/remote/xpc_message.py
 pymobiledevice3/resources/__init__.py
 pymobiledevice3/resources/dsc_uuid_map.json
 pymobiledevice3/resources/dsc_uuid_map.py
 pymobiledevice3/resources/firmware_notifications.py
 pymobiledevice3/resources/notifications.txt
 pymobiledevice3/resources/webinspector/element_attribute.js
 pymobiledevice3/resources/webinspector/element_clear.js
```

### Comparing `pymobiledevice3-2.0.2/pyproject.toml` & `pymobiledevice3-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymobiledevice3"
-version = "2.0.2"
+version = "2.0.3"
 description = "Pure python3 implementation for working with iDevices (iPhone, etc...)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["ios", "protocol", "lockdownd", "instruments", "automation", "cli", "afc"]
 authors = [
     { name = "doronz88", email = "doron88@gmail.com" },
```


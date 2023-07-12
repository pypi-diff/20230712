# Comparing `tmp/bssenv-2.8.0.tar.gz` & `tmp/bssenv-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bssenv-2.8.0.tar", last modified: Fri Jul  7 10:02:38 2023, max compression
+gzip compressed data, was "bssenv-2.8.1.tar", last modified: Wed Jul 12 06:17:28 2023, max compression
```

## Comparing `bssenv-2.8.0.tar` & `bssenv-2.8.1.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.999047 bssenv-2.8.0/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1238 2023-07-07 10:02:37.999047 bssenv-2.8.0/PKG-INFO
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      287 2023-07-07 10:02:31.000000 bssenv-2.8.0/README.rst
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.975047 bssenv-2.8.0/bssenv.egg-info/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1238 2023-07-07 10:02:37.000000 bssenv-2.8.0/bssenv.egg-info/PKG-INFO
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     7839 2023-07-07 10:02:37.000000 bssenv-2.8.0/bssenv.egg-info/SOURCES.txt
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        1 2023-07-07 10:02:37.000000 bssenv-2.8.0/bssenv.egg-info/dependency_links.txt
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       57 2023-07-07 10:02:37.000000 bssenv-2.8.0/bssenv.egg-info/entry_points.txt
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        8 2023-07-07 10:02:37.000000 bssenv-2.8.0/bssenv.egg-info/top_level.txt
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1548 2023-07-07 09:53:23.000000 bssenv-2.8.0/pyproject.toml
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       38 2023-07-07 10:02:37.999047 bssenv-2.8.0/setup.cfg
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5484 2023-05-23 18:11:05.000000 bssenv-2.8.0/setup.py
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.971047 bssenv-2.8.0/src/
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.971047 bssenv-2.8.0/src/comarch/
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.971047 bssenv-2.8.0/src/comarch/bss/
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.975047 bssenv-2.8.0/src/comarch/bss/bssenv/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/__init__.py
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     8368 2023-03-30 15:31:59.000000 bssenv-2.8.0/src/comarch/bss/bssenv/bssenv.py
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.975047 bssenv-2.8.0/src/comarch/bss/bssenv/data/
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.979047 bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1833 2020-11-02 14:43:23.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/12125d03.0
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1983 2020-11-02 14:43:48.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/66808c77.0
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1833 2020-11-02 14:43:23.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/7605dfdf.0
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       11 2021-03-12 10:01:21.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/README
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1833 2020-11-02 14:43:23.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/comarch_root.crt
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1983 2020-11-02 14:43:48.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/comarch_servers.crt
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1983 2020-11-02 14:43:48.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/da3b64ee.0
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.971047 bssenv-2.8.0/src/comarch/bss/bssenv/data/composefiles/
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.979047 bssenv-2.8.0/src/comarch/bss/bssenv/data/composefiles/commands/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/composefiles/commands/.gitkeep
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.979047 bssenv-2.8.0/src/comarch/bss/bssenv/data/composefiles/data_providers/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/composefiles/data_providers/.gitkeep
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.979047 bssenv-2.8.0/src/comarch/bss/bssenv/data/config/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2021-03-16 14:37:44.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/config/.gitkeep
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.979047 bssenv-2.8.0/src/comarch/bss/bssenv/data/python_site_packages/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1372 2023-05-10 17:56:41.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/python_site_packages/requirements.txt
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.979047 bssenv-2.8.0/src/comarch/bss/bssenv/data/resources/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3747 2023-04-25 06:30:33.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/resources/info
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    12083 2023-07-03 05:28:34.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/resources/info2
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      179 2021-04-08 16:40:03.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/resources/post_create_environment_from_snap_info
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      217 2021-04-08 16:39:33.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/resources/post_create_environment_info
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.975047 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.979047 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/autocompletion/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    16254 2023-04-24 20:05:39.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/autocompletion/autocomplete.install
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1821 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/autocompletion/autocomplete.uninstall
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.983047 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    21896 2023-07-05 16:44:10.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/activate
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5440 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/clean
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5634 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/cmd
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2486 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/configMaps
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5454 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/debug
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     9778 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/describe
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5394 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/dns
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2622 2022-01-21 08:07:57.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/enter
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5072 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/exp
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1246 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/fullInstall
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1272 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/fullUpdate
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3224 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/images
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3070 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/init
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    34193 2023-07-03 08:36:45.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/install
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2859 2022-01-21 08:07:39.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/logs
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2631 2022-01-21 08:07:32.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/pause
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    13368 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/ports
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2669 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/retagStableDescriptorForImage
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4034 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/services
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    15430 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/snapshot
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2644 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/start
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1346 2022-01-21 08:07:06.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/stats
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4930 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/status
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2667 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/stop
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     6993 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/switch
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     8957 2023-06-26 17:44:39.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/test
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3477 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/top
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4833 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/uninstall
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2725 2022-01-21 08:06:28.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/unpause
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2255 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/update
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3606 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/versions
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5790 2022-01-21 09:05:26.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/waiton
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.987047 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.991047 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1598 2023-04-19 16:44:41.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/completeExp
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1387 2022-01-19 09:18:24.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listAvailableCommands
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      950 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listDnsMappings
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1063 2023-04-24 19:06:40.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listEntityNames
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      723 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listEnvironmentLocalSnapshots
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      724 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listEnvironmentRemoteSnapshots
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1150 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listLocalSnapshots
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1151 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listRemoteSnapshots
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      822 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNames
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2034 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommands
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1641 2022-01-19 09:54:35.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommandsWithExistingContainers
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1718 2022-01-19 11:02:19.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommandsWithPausedContainers
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1631 2022-01-19 09:23:31.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommandsWithRunningContainers
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1115 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesToClean
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      866 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesToDebug
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      859 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesToInit
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      864 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesWithPorts
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      814 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceSwitches
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3258 2022-01-21 08:33:07.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/createGuardContainers
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      749 2021-05-05 16:40:26.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/destroy
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      311 2022-12-23 10:21:59.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/setOwnerAndPrivilegesForEnvFiles
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1436 2023-04-27 05:18:14.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/updateComposeFilesAfterCreateFromSnap
--rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4004 2023-04-27 05:45:31.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/updateSnapshotImages
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.991047 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.991047 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/gui/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-05-18 08:42:06.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/gui/__init__.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1075 2023-05-18 08:54:56.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/gui/authentication.py
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.991047 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/gui/pages/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       61 2023-05-18 08:29:58.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/gui/pages/__init__.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2008 2023-05-18 08:45:08.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/gui/pages/home.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1112 2023-05-18 14:35:28.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/gui/pages/login.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      565 2023-05-18 07:39:52.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/gui/session.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      315 2023-05-18 08:52:58.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/main.py
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.975047 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.975047 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.995047 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2021-04-07 06:50:54.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/__init__.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    11809 2023-07-07 09:46:44.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/bssenv.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5097 2022-01-13 17:58:49.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/cache.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3848 2021-04-08 16:28:12.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/clean.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      910 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/commandline.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    15871 2023-04-21 06:02:21.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/commands.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4814 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/composefile.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1233 2023-07-07 06:30:18.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/config.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      931 2023-05-11 19:34:11.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/const.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2514 2023-07-07 09:46:23.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/daemons.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4625 2023-04-21 06:07:23.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/data_providers.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1696 2022-01-10 12:46:27.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/dns.py
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.999047 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    10941 2023-07-03 08:02:23.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/__init__.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    19182 2023-05-10 07:05:53.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/dockerClient.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2050 2023-04-21 11:29:13.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/dockerCompose.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    39311 2023-04-28 17:48:51.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/dockerRegistry.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    17185 2023-04-13 18:54:58.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/entities.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1739 2021-05-05 17:05:54.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/env.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1998 2021-04-08 16:29:32.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/export.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3833 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/init.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    35567 2023-07-07 09:44:05.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/install.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      709 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/itertools.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4354 2023-03-28 17:02:24.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/lazy.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3385 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/logging.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5926 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/os.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3663 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/paths.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4401 2022-01-10 12:46:27.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/ports.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       72 2021-03-10 18:17:51.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/regex.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    29145 2023-04-21 11:30:13.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/services.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    25189 2023-05-10 09:31:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/snapshots.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4168 2022-01-10 12:46:27.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/switches.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     7438 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/terminal.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1903 2023-04-17 06:23:40.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/threading.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1395 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/tmp.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      420 2022-12-23 11:55:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/types.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    11550 2023-04-24 06:51:50.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/uninstall.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1039 2023-07-03 08:00:15.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/yaml.py
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.999047 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/sys/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5582 2021-03-08 18:14:56.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/sys/bssenv.autocomplete
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.975047 bssenv-2.8.0/src/comarch/bss/bssenv/data/templates/
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.999047 bssenv-2.8.0/src/comarch/bss/bssenv/data/templates/composefiles/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       95 2023-04-20 07:02:56.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/templates/composefiles/template.yml
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.999047 bssenv-2.8.0/src/comarch/bss/bssenv/data/templates/shell/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1236 2022-01-10 15:00:08.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/templates/shell/command.py
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1358 2022-01-19 18:34:55.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/templates/shell/serviceCommand.py
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.999047 bssenv-2.8.0/src/comarch/bss/bssenv/data/tools/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2020-09-28 12:16:37.000000 bssenv-2.8.0/src/comarch/bss/bssenv/data/tools/.gitkeep
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.975047 bssenv-2.8.0/src/comarch/bss/bssenv/internal/
-drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-07 10:02:37.999047 bssenv-2.8.0/src/comarch/bss/bssenv/internal/config/
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       56 2021-04-06 14:31:49.000000 bssenv-2.8.0/src/comarch/bss/bssenv/internal/config/concurrency.yml
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      587 2023-05-10 09:44:38.000000 bssenv-2.8.0/src/comarch/bss/bssenv/internal/config/docker.yml
--rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       25 2021-04-01 06:12:17.000000 bssenv-2.8.0/src/comarch/bss/bssenv/internal/config/timeouts.yml
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.144212 bssenv-2.8.1/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4775 2023-07-12 06:17:28.144212 bssenv-2.8.1/PKG-INFO
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3824 2023-07-12 05:37:37.000000 bssenv-2.8.1/README.rst
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.124212 bssenv-2.8.1/bssenv.egg-info/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4775 2023-07-12 06:17:28.000000 bssenv-2.8.1/bssenv.egg-info/PKG-INFO
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     7839 2023-07-12 06:17:28.000000 bssenv-2.8.1/bssenv.egg-info/SOURCES.txt
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        1 2023-07-12 06:17:28.000000 bssenv-2.8.1/bssenv.egg-info/dependency_links.txt
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       57 2023-07-12 06:17:28.000000 bssenv-2.8.1/bssenv.egg-info/entry_points.txt
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        8 2023-07-12 06:17:28.000000 bssenv-2.8.1/bssenv.egg-info/top_level.txt
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1547 2023-07-12 06:17:04.000000 bssenv-2.8.1/pyproject.toml
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       38 2023-07-12 06:17:28.144212 bssenv-2.8.1/setup.cfg
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5484 2023-05-23 18:11:05.000000 bssenv-2.8.1/setup.py
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.120212 bssenv-2.8.1/src/
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.120212 bssenv-2.8.1/src/comarch/
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.120212 bssenv-2.8.1/src/comarch/bss/
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.124212 bssenv-2.8.1/src/comarch/bss/bssenv/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/__init__.py
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     8368 2023-03-30 15:31:59.000000 bssenv-2.8.1/src/comarch/bss/bssenv/bssenv.py
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.120212 bssenv-2.8.1/src/comarch/bss/bssenv/data/
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.124212 bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1833 2020-11-02 14:43:23.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/12125d03.0
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1983 2020-11-02 14:43:48.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/66808c77.0
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1833 2020-11-02 14:43:23.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/7605dfdf.0
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       11 2021-03-12 10:01:21.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/README
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1833 2020-11-02 14:43:23.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/comarch_root.crt
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1983 2020-11-02 14:43:48.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/comarch_servers.crt
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1983 2020-11-02 14:43:48.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/da3b64ee.0
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.120212 bssenv-2.8.1/src/comarch/bss/bssenv/data/composefiles/
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.124212 bssenv-2.8.1/src/comarch/bss/bssenv/data/composefiles/commands/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/composefiles/commands/.gitkeep
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.124212 bssenv-2.8.1/src/comarch/bss/bssenv/data/composefiles/data_providers/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/composefiles/data_providers/.gitkeep
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.124212 bssenv-2.8.1/src/comarch/bss/bssenv/data/config/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2021-03-16 14:37:44.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/config/.gitkeep
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.124212 bssenv-2.8.1/src/comarch/bss/bssenv/data/python_site_packages/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1347 2023-07-12 05:45:46.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/python_site_packages/requirements.txt
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.128212 bssenv-2.8.1/src/comarch/bss/bssenv/data/resources/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3747 2023-04-25 06:30:33.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/resources/info
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    12083 2023-07-03 05:28:34.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/resources/info2
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      179 2021-04-08 16:40:03.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/resources/post_create_environment_from_snap_info
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      217 2021-04-08 16:39:33.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/resources/post_create_environment_info
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.120212 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.128212 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/autocompletion/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    16254 2023-04-24 20:05:39.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/autocompletion/autocomplete.install
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1821 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/autocompletion/autocomplete.uninstall
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.132212 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    21896 2023-07-05 16:44:10.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/activate
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5440 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/clean
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5634 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/cmd
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2486 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/configMaps
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5454 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/debug
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     9778 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/describe
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5394 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/dns
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2622 2022-01-21 08:07:57.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/enter
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5072 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/exp
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1246 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/fullInstall
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1272 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/fullUpdate
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3224 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/images
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3070 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/init
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    34193 2023-07-03 08:36:45.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/install
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2859 2022-01-21 08:07:39.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/logs
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2631 2022-01-21 08:07:32.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/pause
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    13368 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/ports
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2669 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/retagStableDescriptorForImage
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4034 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/services
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    15430 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/snapshot
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2644 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/start
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1346 2022-01-21 08:07:06.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/stats
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4930 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/status
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2667 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/stop
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     6993 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/switch
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     8957 2023-06-26 17:44:39.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/test
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3477 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/top
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4833 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/uninstall
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2725 2022-01-21 08:06:28.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/unpause
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2255 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/update
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3606 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/versions
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5790 2022-01-21 09:05:26.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/waiton
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.132212 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.136212 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1598 2023-04-19 16:44:41.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/completeExp
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1387 2022-01-19 09:18:24.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listAvailableCommands
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      950 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listDnsMappings
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1063 2023-04-24 19:06:40.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listEntityNames
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      723 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listEnvironmentLocalSnapshots
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      724 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listEnvironmentRemoteSnapshots
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1150 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listLocalSnapshots
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1151 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listRemoteSnapshots
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      822 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNames
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2034 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommands
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1641 2022-01-19 09:54:35.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommandsWithExistingContainers
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1718 2022-01-19 11:02:19.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommandsWithPausedContainers
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1631 2022-01-19 09:23:31.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommandsWithRunningContainers
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1115 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesToClean
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      866 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesToDebug
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      859 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesToInit
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      864 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesWithPorts
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      814 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceSwitches
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3258 2022-01-21 08:33:07.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/createGuardContainers
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      749 2021-05-05 16:40:26.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/destroy
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      311 2022-12-23 10:21:59.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/setOwnerAndPrivilegesForEnvFiles
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1436 2023-04-27 05:18:14.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/updateComposeFilesAfterCreateFromSnap
+-rwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4004 2023-04-27 05:45:31.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/updateSnapshotImages
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.136212 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.136212 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/gui/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-05-18 08:42:06.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/gui/__init__.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1075 2023-05-18 08:54:56.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/gui/authentication.py
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.136212 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/gui/pages/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       61 2023-05-18 08:29:58.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/gui/pages/__init__.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2008 2023-05-18 08:45:08.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/gui/pages/home.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1112 2023-05-18 14:35:28.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/gui/pages/login.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      565 2023-05-18 07:39:52.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/gui/session.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      315 2023-05-18 08:52:58.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/main.py
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.120212 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.120212 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.140212 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2021-04-07 06:50:54.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/__init__.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    11809 2023-07-07 09:46:44.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/bssenv.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5097 2022-01-13 17:58:49.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/cache.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3848 2021-04-08 16:28:12.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/clean.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      910 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/commandline.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    15871 2023-04-21 06:02:21.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/commands.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4814 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/composefile.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1233 2023-07-07 06:30:18.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/config.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      931 2023-05-11 19:34:11.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/const.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2514 2023-07-07 09:46:23.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/daemons.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4625 2023-04-21 06:07:23.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/data_providers.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1696 2022-01-10 12:46:27.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/dns.py
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.144212 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    10941 2023-07-03 08:02:23.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/__init__.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    19182 2023-05-10 07:05:53.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/dockerClient.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     2050 2023-04-21 11:29:13.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/dockerCompose.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    39311 2023-04-28 17:48:51.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/dockerRegistry.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    17185 2023-04-13 18:54:58.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/entities.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1739 2021-05-05 17:05:54.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/env.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1998 2021-04-08 16:29:32.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/export.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3833 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/init.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    35567 2023-07-07 09:44:05.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/install.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      709 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/itertools.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4354 2023-03-28 17:02:24.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/lazy.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3385 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/logging.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5926 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/os.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     3663 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/paths.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4401 2022-01-10 12:46:27.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/ports.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       72 2021-03-10 18:17:51.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/regex.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    29145 2023-04-21 11:30:13.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/services.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    25189 2023-05-10 09:31:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/snapshots.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     4168 2022-01-10 12:46:27.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/switches.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     7438 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/terminal.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1903 2023-04-17 06:23:40.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/threading.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1395 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/tmp.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      420 2022-12-23 11:55:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/types.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)    11550 2023-04-24 06:51:50.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/uninstall.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1039 2023-07-03 08:00:15.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/yaml.py
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.144212 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/sys/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     5582 2021-03-08 18:14:56.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/sys/bssenv.autocomplete
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.120212 bssenv-2.8.1/src/comarch/bss/bssenv/data/templates/
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.144212 bssenv-2.8.1/src/comarch/bss/bssenv/data/templates/composefiles/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       95 2023-04-20 07:02:56.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/templates/composefiles/template.yml
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.144212 bssenv-2.8.1/src/comarch/bss/bssenv/data/templates/shell/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1236 2022-01-10 15:00:08.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/templates/shell/command.py
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)     1358 2022-01-19 18:34:55.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/templates/shell/serviceCommand.py
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.144212 bssenv-2.8.1/src/comarch/bss/bssenv/data/tools/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2020-09-28 12:16:37.000000 bssenv-2.8.1/src/comarch/bss/bssenv/data/tools/.gitkeep
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.124212 bssenv-2.8.1/src/comarch/bss/bssenv/internal/
+drwxrwxr-x   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)        0 2023-07-12 06:17:28.144212 bssenv-2.8.1/src/comarch/bss/bssenv/internal/config/
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       56 2021-04-06 14:31:49.000000 bssenv-2.8.1/src/comarch/bss/bssenv/internal/config/concurrency.yml
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)      587 2023-05-10 09:44:38.000000 bssenv-2.8.1/src/comarch/bss/bssenv/internal/config/docker.yml
+-rw-rw-r--   0 hubert_tarnacki  (1000) hubert_tarnacki  (1000)       25 2021-04-01 06:12:17.000000 bssenv-2.8.1/src/comarch/bss/bssenv/internal/config/timeouts.yml
```

### Comparing `bssenv-2.8.0/bssenv.egg-info/SOURCES.txt` & `bssenv-2.8.1/bssenv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/pyproject.toml` & `bssenv-2.8.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bssenv"
-version = "2.8.0"
+version = "2.8.1"
 description = "A project for managing bss local, dockerized environments"
 
 authors = [
   { name = "Hubert Tarnacki", email = "hubert.tarnacki@comarch.com" }
 ]
 maintainers = [
   { name = "Hubert Tarnacki", email = "hubert.tarnacki@comarch.com" }
@@ -22,18 +22,18 @@
     'Programming Language :: Python :: 3',
     'Programming Language :: Unix Shell'
 ]
 
 requires-python = ">=3.8"
 
 [project.urls]
-documentation = "https://wiki.comarch/display/BSSRND/bssenv"
-repository = "http://r7.krakow.comarch:8000/Aurel/bssenv"
-bug-reports = "https://tapir.krakow.comarch/jira/projects/BSSREL"
-Home-Page = "https://wiki.comarch/display/BSSRND/bssenv"
+Homepage = "https://wiki.comarch/display/BSSRND/bssenv"
+Documentation = "https://wiki.comarch/display/BSSRND/bssenv"
+Repository = "http://r7.krakow.comarch:8000/Aurel/bssenv"
+Bug-Reports = "https://tapir.krakow.comarch/jira/projects/BSSREL"
 
 [project.scripts]
 bssenv = "comarch.bss.bssenv.bssenv:run"
 
 [build-system]
 requires = ["setuptools", "pip"]
 build-backend = "setuptools.build_meta"
```

### Comparing `bssenv-2.8.0/setup.py` & `bssenv-2.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/bssenv.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/bssenv.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/12125d03.0` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/12125d03.0`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/66808c77.0` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/66808c77.0`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/7605dfdf.0` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/7605dfdf.0`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/comarch_root.crt` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/comarch_root.crt`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/comarch_servers.crt` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/comarch_servers.crt`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/certificates/da3b64ee.0` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/certificates/da3b64ee.0`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/python_site_packages/requirements.txt` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/python_site_packages/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 blessed==1.19.1
 bracex==2.3.post1 ; python_version >= '3.7'
 certifi==2023.5.7 ; python_version >= '3.6'
 cffi==1.15.1
 charset-normalizer==2.1.1 ; python_full_version >= '3.6.0'
 cloudpickle==2.2.1 ; python_version >= '3.6'
 commonmark==0.9.1
-cryptography==40.0.2 ; python_version >= '3.6'
+cryptography==41.0.2 ; python_version >= '3.7'
 dask==2022.06.1
 deepdiff==5.8.1
 docker==5.0.3
-fsspec==2023.5.0 ; python_version >= '3.8'
+fsspec==2023.6.0 ; python_version >= '3.8'
 humanize==4.2.3
 idna==3.4 ; python_version >= '3.5'
 jeepney==0.8.0 ; python_version >= '3.7'
 locket==1.0.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 ordered-set==4.1.0 ; python_version >= '3.7'
 packaging==23.1 ; python_version >= '3.7'
 partd==1.4.0 ; python_version >= '3.7'
@@ -29,12 +29,12 @@
 pyyaml==5.4.1
 requests==2.28.1
 rich==12.4.4
 secretstorage==3.3.3
 six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 toml==0.10.2
 toolz==0.12.0 ; python_version >= '3.5'
-typing-extensions==4.5.0 ; python_version < '3.9'
-urllib3==1.26.15 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
+typing-extensions==4.5.0
+urllib3==1.26.16 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
 wcmatch==8.4
 wcwidth==0.2.6
-websocket-client==1.5.1 ; python_version >= '3.7'
+websocket-client==1.6.1 ; python_version >= '3.7'
```

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/resources/info` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/resources/info`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/resources/info2` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/resources/info2`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/autocompletion/autocomplete.install` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/autocompletion/autocomplete.install`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/autocompletion/autocomplete.uninstall` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/autocompletion/autocomplete.uninstall`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/activate` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/activate`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/clean` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/clean`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/cmd` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/cmd`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/configMaps` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/configMaps`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/debug` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/debug`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/describe` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/describe`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/dns` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/dns`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/enter` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/enter`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/exp` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/exp`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/fullInstall` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/fullInstall`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/fullUpdate` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/fullUpdate`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/images` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/images`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/init` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/init`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/install` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/install`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/logs` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/logs`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/pause` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/pause`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/ports` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/ports`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/retagStableDescriptorForImage` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/retagStableDescriptorForImage`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/services` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/services`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/snapshot` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/snapshot`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/start` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/start`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/stats` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/stats`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/status` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/status`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/stop` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/stop`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/switch` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/switch`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/test` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/test`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/top` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/top`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/uninstall` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/uninstall`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/unpause` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/unpause`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/update` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/update`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/versions` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/versions`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin/waiton` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin/waiton`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/completeExp` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/completeExp`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listAvailableCommands` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listAvailableCommands`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listDnsMappings` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listDnsMappings`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listEntityNames` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listEntityNames`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listEnvironmentLocalSnapshots` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listEnvironmentLocalSnapshots`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listEnvironmentRemoteSnapshots` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listEnvironmentRemoteSnapshots`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listLocalSnapshots` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listLocalSnapshots`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listRemoteSnapshots` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listRemoteSnapshots`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNames` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNames`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommands` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommands`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommandsWithExistingContainers` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommandsWithExistingContainers`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommandsWithPausedContainers` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommandsWithPausedContainers`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommandsWithRunningContainers` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesAndCommandsWithRunningContainers`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesToClean` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesToClean`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesToDebug` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesToDebug`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesToInit` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesToInit`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesWithPorts` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceNamesWithPorts`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceSwitches` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/autocompletions/listServiceSwitches`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/createGuardContainers` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/createGuardContainers`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/destroy` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/destroy`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/updateComposeFilesAfterCreateFromSnap` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/updateComposeFilesAfterCreateFromSnap`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/bin2/updateSnapshotImages` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/bin2/updateSnapshotImages`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/gui/authentication.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/gui/authentication.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/gui/pages/home.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/gui/pages/home.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/gui/pages/login.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/gui/pages/login.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/gui/gui/session.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/gui/gui/session.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/bssenv.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/bssenv.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/cache.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/cache.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/clean.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/clean.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/commandline.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/commandline.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/commands.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/commands.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/composefile.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/composefile.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/config.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/config.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/const.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/const.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/daemons.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/daemons.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/data_providers.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/data_providers.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/dns.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/dns.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/__init__.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/dockerClient.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/dockerClient.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/dockerCompose.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/dockerCompose.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/dockerRegistry.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/docker/dockerRegistry.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/entities.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/entities.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/env.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/env.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/export.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/export.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/init.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/init.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/install.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/install.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/itertools.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/itertools.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/lazy.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/lazy.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/logging.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/logging.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/os.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/os.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/paths.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/paths.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/ports.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/ports.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/services.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/services.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/snapshots.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/snapshots.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/switches.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/switches.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/terminal.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/terminal.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/threading.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/threading.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/tmp.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/tmp.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/uninstall.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/uninstall.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/lib/python/local/yaml.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/lib/python/local/yaml.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/scripts/sys/bssenv.autocomplete` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/scripts/sys/bssenv.autocomplete`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/templates/shell/command.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/templates/shell/command.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/data/templates/shell/serviceCommand.py` & `bssenv-2.8.1/src/comarch/bss/bssenv/data/templates/shell/serviceCommand.py`

 * *Files identical despite different names*

### Comparing `bssenv-2.8.0/src/comarch/bss/bssenv/internal/config/docker.yml` & `bssenv-2.8.1/src/comarch/bss/bssenv/internal/config/docker.yml`

 * *Files identical despite different names*


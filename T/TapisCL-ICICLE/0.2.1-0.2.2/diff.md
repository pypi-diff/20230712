# Comparing `tmp/TapisCL-ICICLE-0.2.1.tar.gz` & `tmp/TapisCL-ICICLE-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.2.1.tar", last modified: Fri Jul  7 17:27:11 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.2.2.tar", last modified: Tue Jul 11 23:32:52 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.2.1.tar` & `TapisCL-ICICLE-0.2.2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 17:27:11.250585 TapisCL-ICICLE-0.2.1/
--rw-rw-rw-   0        0        0    35823 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.1/LICENSE
--rw-rw-rw-   0        0        0    44898 2023-07-07 17:27:11.249590 TapisCL-ICICLE-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3015 2023-06-27 20:45:47.000000 TapisCL-ICICLE-0.2.1/README.md
--rw-rw-rw-   0        0        0     1203 2023-07-07 17:26:21.000000 TapisCL-ICICLE-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 17:27:11.251584 TapisCL-ICICLE-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-07 17:27:11.020367 TapisCL-ICICLE-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-07 17:27:11.031464 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      321 2023-06-28 16:15:55.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:27:11.049385 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0       84 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0    10068 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0    10189 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/client/handlers.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:27:11.132468 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/__init__.py
--rw-rw-rw-   0        0        0    10762 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/appCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:27:11.143125 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/arguments/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/arguments/__init__.py
--rw-rw-rw-   0        0        0     7175 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/arguments/argument.py
--rw-rw-rw-   0        0        0    17471 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0    10393 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     2190 2023-06-30 23:43:06.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/commandOpts.py
--rw-rw-rw-   0        0        0     1616 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     4947 2023-07-07 17:17:32.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/decorators.py
--rw-rw-rw-   0        0        0    11359 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     6205 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/jobCommands.py
--rw-rw-rw-   0        0        0     9081 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:27:11.159173 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1250 2023-06-30 18:18:14.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      871 2023-06-22 18:14:57.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     4010 2023-07-07 16:41:01.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0    20776 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/systemCommands.py
--rw-rw-rw-   0        0        0     8018 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/volumeCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:27:11.183823 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0    11007 2023-07-07 17:05:35.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/server/auth.py
--rw-rw-rw-   0        0        0    10202 2023-07-07 16:36:44.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0     2044 2023-07-07 17:02:35.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/server/userFileManager.py
--rw-rw-rw-   0        0        0      290 2023-07-03 18:17:51.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:27:11.198498 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/socketopts/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/socketopts/__init__.py
--rw-rw-rw-   0        0        0     2190 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/socketopts/schemas.py
--rw-rw-rw-   0        0        0     4439 2023-07-06 15:43:36.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/socketopts/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:27:11.225261 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2457 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1044 2023-06-22 17:11:48.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0     1961 2023-07-06 18:19:25.000000 TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/utilities/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-07 17:27:11.244336 TapisCL-ICICLE-0.2.1/src/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44898 2023-07-07 17:27:10.000000 TapisCL-ICICLE-0.2.1/src/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1722 2023-07-07 17:27:11.000000 TapisCL-ICICLE-0.2.1/src/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 17:27:10.000000 TapisCL-ICICLE-0.2.1/src/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-07 17:27:10.000000 TapisCL-ICICLE-0.2.1/src/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 17:27:10.000000 TapisCL-ICICLE-0.2.1/src/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-07 17:27:10.000000 TapisCL-ICICLE-0.2.1/src/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-27 23:09:19.000000 TapisCL-ICICLE-0.2.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.474839 TapisCL-ICICLE-0.2.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    44898 2023-07-11 23:32:52.474336 TapisCL-ICICLE-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3015 2023-06-29 16:14:59.000000 TapisCL-ICICLE-0.2.2/README.md
+-rw-rw-rw-   0        0        0     1222 2023-07-11 23:32:32.000000 TapisCL-ICICLE-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 23:32:52.474839 TapisCL-ICICLE-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.445412 TapisCL-ICICLE-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.446807 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      321 2023-06-29 16:14:59.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.449804 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0       84 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0    10294 2023-07-11 22:01:19.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0    13905 2023-07-11 23:10:26.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/client/handlers.py
+drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.458433 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/__init__.py
+-rw-rw-rw-   0        0        0    14439 2023-07-11 22:55:10.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/appCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.460425 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/arguments/
+-rw-rw-rw-   0        0        0        0 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/arguments/__init__.py
+-rw-rw-rw-   0        0        0     7310 2023-07-11 22:55:48.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/arguments/argument.py
+-rw-rw-rw-   0        0        0    20538 2023-07-11 22:05:10.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0    10475 2023-07-11 17:43:00.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2190 2023-06-21 21:26:22.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/commandOpts.py
+-rw-rw-rw-   0        0        0     1757 2023-07-08 04:38:18.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     4947 2023-07-10 21:26:23.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/decorators.py
+-rw-rw-rw-   0        0        0    11359 2023-07-06 00:05:20.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     6692 2023-07-11 21:52:39.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/jobCommands.py
+-rw-rw-rw-   0        0        0    10586 2023-07-11 20:26:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.462418 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1615 2023-07-11 17:42:26.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      871 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     4414 2023-07-08 04:38:18.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0    25444 2023-07-11 23:15:25.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/systemCommands.py
+-rw-rw-rw-   0        0        0     8018 2023-07-05 23:06:02.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/volumeCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.464411 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0    10928 2023-07-06 00:52:04.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/server/auth.py
+-rw-rw-rw-   0        0        0    10250 2023-07-11 21:49:02.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      290 2023-07-05 15:04:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.465585 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/socketopts/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/socketopts/__init__.py
+-rw-rw-rw-   0        0        0     2233 2023-07-10 21:26:16.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/socketopts/schemas.py
+-rw-rw-rw-   0        0        0     4404 2023-07-08 04:38:18.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/socketopts/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.468850 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-16 02:31:56.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1044 2023-06-29 21:33:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0     2328 2023-07-08 04:38:18.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.471840 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44898 2023-07-11 23:32:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1692 2023-07-11 23:32:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 23:32:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-11 23:32:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 23:32:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-11 23:32:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-29 16:14:59.000000 TapisCL-ICICLE-0.2.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.472837 TapisCL-ICICLE-0.2.2/tests/
+-rw-rw-rw-   0        0        0      191 2023-07-10 17:51:41.000000 TapisCL-ICICLE-0.2.2/tests/test.py
```

### Comparing `TapisCL-ICICLE-0.2.1/LICENSE` & `TapisCL-ICICLE-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.1/PKG-INFO` & `TapisCL-ICICLE-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.2.1
+Version: 0.2.2
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.2.1/README.md` & `TapisCL-ICICLE-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.1/pyproject.toml` & `TapisCL-ICICLE-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "poetry-core>=1.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.2.1"
+version = "0.2.2"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "m.ray37990@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
@@ -26,14 +26,15 @@
 pyperclip = "*"
 py2neo = "*"
 psycopg2-binary = "*"
 blessed = "*"
 prompt_toolkit = "*"
 TapisFederatedAuthClientAPI = "*"
 requests = "*"
+pyreadline3 = "*"
 
 [project.optional-dependencies]
 dev = []
 
 [project.urls]
 Homepage = "https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE"
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/client/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,18 @@
             self.connection.send(handled_response)
 
     def terminal_cli(self):
         try:
             kwargs = self.parser.parse_args()
             kwargs = vars(kwargs)
             self.interface(kwargs)
+            kwargs = vars(self.parser.parse_args(['exit']))
+            response_message = schemas.CommandData(request_content=kwargs)
+            self.connection.send(response_message)
+            self.connection.close()
         except Exception as e:
             print(e)
         finally:
             sys.exit(0)
 
     def cli_window(self):
         title = pyfiglet.figlet_format("-----------\nTapisCLICICLE\n-----------", font="slant") # print the title when CLI is accessed
@@ -199,33 +203,33 @@
             try:
                 time.sleep(0.01)
                 kwargs: dict = vars(self.parser.parse_args(str(input(f"[{self.username}@{self.url}][{self.current_system}]{self.pwd} ")).split(" ")))
                 self.interface(kwargs)
             except KeyboardInterrupt:
                 continue
             except exceptions.Shutdown:
-                print("Server shutdown, exiting")
+                print("Exit initiated by user")
                 kwargs = vars(self.parser.parse_args(['shutdown']))
                 response_message = schemas.CommandData(request_content=kwargs)
                 self.connection.send(response_message)
                 self.connection.close()
                 break
             except (ConnectionAbortedError, ConnectionResetError):
-                print("Server shutdown, exiting")
+                print("Server shutdown, exiting (SF)")
                 self.connection.close()
                 break
             except (TypeError, argparse.ArgumentError, argparse.ArgumentTypeError) as e:
                 print(e)
                 error_str = traceback.format_exc()
                 print(error_str)
                 print("Invalid command")
             except Exception as e:
                 error_str = traceback.format_exc()
-                if self.debug:
-                    print(error_str)
+                #if self.debug:
+                print(error_str)
                 print(e)
                 error_message = schemas.ResponseData(error=str(e))
                 self.connection.send(error_message)
         
 
     def main(self):
         if len(sys.argv) > 1: # checks if any command line arguments were provided. Does not open CLI
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/client/handlers.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/client/handlers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from getpass import getpass
 import os
 import json
+import pprint
+import time
+import pyreadline3
 
 from prompt_toolkit.validation import Validator, ValidationError
 from prompt_toolkit.completion import word_completer, WordCompleter
 from prompt_toolkit import prompt
 from blessed import Terminal
 
+
 if __name__ != "__main__":
     from ..socketopts import schemas
 
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(f"{__file__}")))
 saved_command = os.path.join(__location__, r'entered_command.json')
 
 
+LINE_READER = base_read_line = pyreadline3.BaseReadline()
+
+
 class Formatters:
     """
     Format received dictionaries in the client code
     """
     def print_response(self, input_data, depth: int=0):
         if isinstance(input_data, (list, set, tuple)):
             for data in input_data:
@@ -30,15 +37,15 @@
             for name, data in input_data.items():
                 if isinstance(data, (int, str)):
                     print(("  " * depth) + f"{name}: {data}")
                     continue
                 print(("  " * depth) + f"{name}: ")
                 self.print_response(data, depth=depth+1)
         elif isinstance(input_data, (int, str)):
-            print(input_data)
+            print(f"{depth * '  '}{input_data}")
         if depth == 0:
             print("\n")
 
 
 class ParserTypeLenEnforcer:
         def __init__(self, name: str=str(), size: tuple=(0, 0), data_type: str='string', choices: list=list()):
             self.arg_name = name
@@ -75,16 +82,16 @@
     def __init__(self):
         super().__init__()
         self.enforcer = ParserTypeLenEnforcer()
 
     def validate(self, document):
         text = document.text
         self.enforcer(text)
-            
 
+        
 class Handlers(Formatters):
     def __init__(self):
         self.validator = ResponseValidator()
 
     def __expression_input(self) -> str: 
         """
         Input an expression as requested by the server for something like cypher queries
@@ -95,104 +102,171 @@
         while line != 'exit': 
             line = str(input("> "))
             if line != 'exit':
                 expression += line
         return expression
     
     def confirmation_handler(self, argument):
+        if 'description' in argument and argument['description']:
+            print(argument['description'])
         print(argument['name'])
         while True:
             decision = str(input("(y/n)"))
             if decision == 'y':
                 decision = True
                 break
             elif decision == 'n':
                 decision = False
                 break
             else:
                 print("Enter valid response")
         return decision
     
-    def input_dict_handler(self, term: Terminal, attrs: dict):
+    def input_dict_handler(self, term: Terminal, attrs: dict, default=None):
         mode = 'create'
-        answer = dict()
+        if not default:
+            default = dict()
+        answer = default
         default_name = attrs['data_type']['name']
         with term.fullscreen():
             print(f"You are now entering data for {attrs['name']}")
             while True:
-                print(f"{term.clear}{attrs['name']}\nreserved names: create, delete, exit (enter these for special action)\n{answer}\nmode: {mode}")
+                print(f"{term.clear}now editing the map: {attrs['name']}\nreserved names: create, delete, exit (enter these for special action)\nmode: {mode}")
+                print(json.dumps(answer, indent=4))
                 attrs['data_type']['name'] = default_name
                 name = str(input(f"enter the name for the instance of your {attrs['data_type']['name']}: "))
                 if name.lower() in ('delete', 'create'):
                     mode = name
                     continue
                 if name.lower() == 'exit':
                     return answer
                 if mode == 'create':
                     mode = 'create'
                     attrs['data_type']['name'] = name
-                    sub_answer = self.form_handler({name:attrs['data_type']}, term)
+                    if name in answer:
+                        default_value = answer#[name]
+                    else:
+                        default_value = None
+                    pprint.pprint({name:attrs['data_type']})
+                    sub_answer = self.advanced_input_handler({name:attrs['data_type']}, term, default=default_value)
                     answer.update(**sub_answer)
                 elif mode == 'delete':
                     mode = 'delete'
                     try:
                         answer.pop(name)
                     except KeyError:
                         pass
 
-    def input_list(self, term: Terminal, attrs: dict):
-        answer = []
+    def input_list(self, term: Terminal, attrs: dict, default=None):
+        if not default:
+            default = list()
+        answer = default
         with term.fullscreen():
             print(f"You are now entering data for {attrs['name']}")
+            mode = 'modify'
             while True:
+                sub_answer = None
                 presentable_dict = {str(index+1):value for index, value in enumerate(answer)}
-                print(f"{term.clear}{attrs['name']}\nreserved names: exit, new (enter these for special action). Enter index of an existing variable name to delete it\n{presentable_dict}")
+                print(rf"""{term.clear}now editing the list: {attrs['name']}
+                      Enter exit to submit list, or new to create new list element.
+                      Modes: to change mode, enter the mode you want to use. 
+                        Delete: when you enter an index the index is deleted. 
+                        Modify: when you enter an index you will re-enter the element to modify it
+                      mode: {mode}""")
+                print(json.dumps(presentable_dict, indent=4))
                 decision = input("Enter 'new' or 'exit': ")
                 if decision.lower() == 'exit':
                     return answer
                 elif decision.lower() == 'new':
                     pass
-                elif decision.isdigit():
+                elif decision.lower() in ('modify', 'delete'):
+                    mode = decision
+                    continue
+                elif decision.isdigit() and mode == 'delete':
                     try:
                         answer.pop(int(decision)-1)
                     except IndexError:
                         continue
                     continue
+                elif decision.isdigit() and mode == 'modify':
+                    try:
+                        print({f"{attrs['name']}_{str(decision)}":answer[int(decision)-1]})
+                        time.sleep(5)
+                        sub_answer = self.advanced_input_handler({f"{attrs['name']}_{str(decision)}":attrs['data_type']}, term, default={f"{attrs['name']}_{str(decision)}":answer[int(decision)-1]})
+                        answer[int(decision)-1] = sub_answer[f"{attrs['name']}_{str(decision)}"]
+                    except IndexError:
+                        continue
+                    continue
                 else:
                     continue
-                sub_answer = self.form_handler({str(len(answer)+1):attrs['data_type']}, term)
+                sub_answer = self.advanced_input_handler({f"{attrs['name']}_{str(len(answer)+1)}":attrs['data_type']}, term)
                 index, value = list(sub_answer.items())[0]
                 answer.append(value)
+
+    def form_handler(self, term: Terminal, attrs: dict, form_name, default=None):
+        form_options = attrs['arguments_list']
+        completer = WordCompleter(list(form_options.keys()))
+        if not default:
+            form_input = dict()
+            for name, command_metadata in form_options.items():
+                if command_metadata['default_value']:
+                    form_input[name] = command_metadata['default_value']
+                    continue
+                form_input[name] = ''
+        else:
+            form_input = {arg_name:arg_default_value for arg_name, arg_default_value in default.items() if arg_name in form_options}
+        while True:
+            print(f"{term.clear}now editing the form: {form_name}")
+            print(json.dumps(form_input, indent=3))
+            field = prompt('Enter the field you want to modify. Enter exit to complete: ', completer=completer)
+            if field.lower() == 'exit':
+                return form_input
+            elif field not in form_options:
+                continue
+            result = self.advanced_input_handler({field:form_options[field]}, term, default=form_input)
+            form_input[field] = result[field]
+            
+    def str_input(self, attrs):
+        completer = None
+        if 'choices' in attrs and attrs['choices']:
+            completer = WordCompleter(attrs['choices'])
+        answer = prompt(f"{attrs['name']}: ", validator=self.validator, wrap_lines=True, completer=completer)
+        return answer
     
-    def form_handler(self, form_request: dict, term: Terminal):
+    def advanced_input_handler(self, form_request: dict, term: Terminal, default=None):
         response = dict()
         for field, attrs in form_request.items():
             arg_type = attrs['arg_type']
             self.validator.enforcer.update_constraints(**attrs)
+            if 'description' in attrs and attrs['description']:
+                print(attrs['description'])
+            # pprint.pprint(form_request)
+            # print(field)
+            if default:
+                default_selection = default[field]
+            else:
+                default_selection = None
             try:
                 match arg_type:
                     case 'secure':
                         answer = prompt(f"{attrs['name']}: ", validator=self.validator, is_password=True)
                     case 'expression':
                         with term.fullscreen():
                             print(f"Enter expression input for the {attrs['name']} argument.")
                             answer = self.__expression_input()
                     case 'form':
-                        answer = self.form_handler(attrs['arguments_list'], term)
+                        answer = self.form_handler(term, attrs, field, default=default_selection)
                     case 'input_list':
-                        answer = self.input_list(term, attrs)
+                        answer = self.input_list(term, attrs, default=default_selection)
                     case 'input_dict':
-                        answer = self.input_dict_handler(term, attrs)
+                        answer = self.input_dict_handler(term, attrs, default=default_selection)
                     case 'str_input':
-                        completer = None
-                        if 'description' in attrs and attrs['description']:
-                            print(attrs['description'])
-                        if 'choices' in attrs and attrs['choices']:
-                            completer = WordCompleter(attrs['choices'])
-                        answer = prompt(f"{attrs['name']}: ", validator=self.validator, wrap_lines=True, completer=completer)
+                        answer = self.str_input(attrs)
+                    case 'standard':
+                        answer = self.str_input(attrs)
                     case 'confirmation':
                         answer = self.confirmation_handler(attrs)
                     case 'silent':
                         continue
                     case _:
                         raise AttributeError(f"There is not argument type {arg_type}")
                 response[field] = answer
@@ -206,15 +280,19 @@
         return response
     
     def universal_message_handler(self, message: schemas.BaseSchema, term: Terminal):
         self.print_response(message.message)
         if message.error:
             self.print_response(message.error)
         if message.request_content:
-            filled_form = self.form_handler(message.request_content, term)
+            try:
+                default = message.existing_data
+            except:
+                default = None
+            filled_form = self.advanced_input_handler(message.request_content, term, default=default)
             return filled_form
         return None
         
     def environment_cli_response_stream_handler(self, response):
         if response.schema_type == 'ResponseData' and response.exit_status: # if the command was a shutdown or exit, close the program
             self.print_response(response.response_message)
             os._exit(0)
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/appCommands.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/volumeCommands.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,258 +1,249 @@
-import json
+from tapipy.tapis import errors as TapisErrors
 
 
 if __name__ != "__main__":
     from . import baseCommand, decorators
     from .arguments import argument
+    from . import commandOpts
     Argument = argument.Argument
 
 
-class create_app(baseCommand.BaseCommand):
+class get_volumes(baseCommand.BaseCommand):
     """
-    @help: create an app. You must have a properly configured app config file. 
-    See a template at https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/tapis-config-files/app-config.json
+    @help: get a list of volumes registered to your account
+    """
+    async def run(self, *args, **kwargs):
+        return self.t.pods.get_volumes()
+    
+
+class create_volume(baseCommand.BaseCommand):
+    """
+    @help: create a new volume on which to store files to be used by Tapis pods. This allows several pods to share the same persistent files
     """
     supports_config_file=True
     required_arguments = [
-        Argument('id', positional=True),
-        Argument('version', positional=True),
-        Argument('containerImage')
+        Argument('volume_id', positional=True)
     ]
     optional_arguments = [
         Argument('description', arg_type='str_input'),
-        Argument('owner', default_value=r"${apiUserId}"),
-        Argument('enabled', action='store_true'),
-        Argument('runtime', choices=['SINGULARITY', 'DOCKER']),
-        Argument('runtimeVersion'),
-        Argument('runtimeOptions', choices=['NONE', 'SINGULARITY_START', 'SINGULARITY_RUN']),
-        Argument('jobType', choices=['BATCH', 'FORK']),
-        Argument('maxJobs', data_type='int'),
-        Argument('maxJobsPerUser', data_type='int'),
-        Argument("strictFileInputs", action='store_true'),
-        Argument('tags', arg_type='input_list', data_type=Argument('tag', size_limit=(1, 128))),
+        Argument('size_limit', data_type='int', default_value=1024)
     ]
-    async def run(self, *args, **kwargs) -> str: # create a tapis app taking a json descriptor file path
-        url = self.t.apps.createAppVersion(**kwargs)
-        return f"App created successfully\nID: {kwargs['id']}\nVersion: {kwargs['version']}\nURL: {url}\n"
+    async def run(self, *args, **kwargs):
+        return self.t.pods.create_volume(**kwargs)
     
 
-class update_app(create_app):
+class get_volume(baseCommand.BaseCommand):
     """
-    @help: update app with the select attributes
+    @help: get information on a specific volume
     """
-    supports_config_file = True
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
     required_arguments = [
-        Argument('appId', size_limit=(1, 80), positional=True),
-        Argument('appVersion', size_limit=(1, 64), positional=True)
+        Argument('volume_id', positional=True)
     ]
     async def run(self, *args, **kwargs):
-        self.t.apps.patchApp(**kwargs)
-        return f'updated app {kwargs["appId"]} successfully'
-
+        return self.t.pods.get_volume(**kwargs)
+    
 
-class assign_default_job_attributes(baseCommand.BaseCommand):
+class volume(baseCommand.BaseCommand):
     """
-    @help: assign a default set of job attributes for this app, if you decide to run it as a job
+    @help: enter the volume to interact with its files more directly
     """
-    supports_config_file=True
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
     required_arguments = [
-        Argument('appId', size_limit=(1, 80), positional=True),
-        Argument('appVersion', size_limit=(1, 64), positional=True)
+        Argument('volume_id', positional=True)
     ]
-    optional_arguments = [
-        Argument('description', arg_type='str_input'),
-        Argument('dynamicExecSystem', arg_type='confirmation', description="System is dynamic?"),
-        Argument('execSystemConstraints', arg_type='input_list', data_type=Argument('constraint', size_limit=(3, 4096))),
-        Argument('execSystemId', size_limit=(1, 80)),
-        Argument('execSystemExecDir', size_limit=(1, 4096)),
-        Argument('execSystemInputDir', size_limit=(1, 4096)),
-        Argument('execSystemOutputDir', size_limit=(1, 4096)),
-        Argument('execSystemLogicalQueue', size_limit=(1, 128)),
-        Argument('archiveSystemId', size_limit=(1, 80)),
-        Argument('archivesystemDir', size_limit=(1, 4096)),
-        Argument('archiveOnAppError', arg_type='confirmation', description='archive on error?'),
-        Argument("isMpi", arg_type='confirmation', description="is mpi?"),
-        Argument('mpiCmd', size_limit=(1, 126), arg_type='str_input'),
-        Argument('cmdPrefix', size_limit=(1, 126)),
-        argument.Form('parameterSet', arguments_list=[
-            Argument('appArgs', arg_type='input_list', data_type=argument.Form('appArg', arguments_list=[
-                Argument('name', size_limit=(1, 80)),
-                Argument('description', size_limit=(1, 8096)),
-                Argument('inputMode', choices=['REQUIRED', "FIXED", "INCLUDE_ON_DEMAND", "INCLUDE_BY_DEFAULT"]),
-                Argument('arg')]
-            )),
-            Argument('containerArgs', arg_type='input_list', data_type=argument.Form('containerArg', arguments_list=[
-                Argument('name', size_limit=(1, 80)),
-                Argument('description', size_limit=(1, 8096)),
-                Argument('inputMode', choices=['REQUIRED', "FIXED", "INCLUDE_ON_DEMAND", "INCLUDE_BY_DEFAULT"]),
-                Argument('arg')
-            ])),
-            Argument('schedulerOptions', arg_type='input_list', data_type=argument.Form('schedulerOption', arguments_list=[
-                Argument('name', size_limit=(1, 80)),
-                Argument('description', size_limit=(1, 8096)),
-                Argument('inputMode', choices=['REQUIRED', "FIXED", "INCLUDE_ON_DEMAND", "INCLUDE_BY_DEFAULT"]),
-                Argument('arg')
-            ])),
-            Argument('envVariables', arg_type='input_list', data_type=argument.Form('environment_variable', arguments_list=[
-                Argument('key'),
-                Argument('value'),
-                Argument('description', size_limit=(1, 2048))
-            ]))
-        ]),
-        Argument('fileInputs', arg_type='input_list', data_type=argument.Form('fileInput', arguments_list=[
-            Argument('name', size_limit=(1, 80)),
-            Argument('description', size_limit=(1, 8096)),
-            Argument('inputMode', choices=['REQUIRED', 'OPTIONAL', 'FIXED']),
-            Argument('autoMountLocal', arg_type='confirmation', description='auto mount to local?'),
-            Argument('sourceUrl'),
-            Argument('targetPath')
-        ])),
-        Argument('fileInputArrays', arg_type='input_list', data_type=argument.Form('fileInput', arguments_list=[
-            Argument('name', size_limit=(1, 80)),
-            Argument('description', size_limit=(1, 8096)),
-            Argument('inputMode', choices=['REQUIRED', 'OPTIONAL', 'FIXED']),
-            Argument('sourceUrls', arg_type='input_list', data_type=Argument('sourceUrl')),
-            Argument('targetPath')
-        ])),
-        Argument('nodeCount', data_type='int'),
-        Argument('coresPerNode', data_type='int'),
-        Argument('memoryMB', data_type='int'),
-        Argument('maxMinutes', data_type='int'),
-        Argument('subscriptions', arg_type='input_list', data_type=argument.Form('subscription', arguments_list=[
-            Argument('description'),
-            Argument('enabled', arg_type='confirmation', description='enable subscription?'),
-            Argument('jobEventCategoryFilter', choices=['ALL', 'JOB_NEW_STATUS', 'JOB_INPUT_TRANSACTION_ID', 'JOB_ARCHIVE_TRANSACTION_ID', 'JOB_ERROR_MESSAGE', 'JOB_SUBSCRIPTION']),
-            Argument('ttlMinutes', data_type='int'),
-            Argument('deliveryTargets', arg_type='input_list', data_type=argument.Form('deliveryTarget', arguments_list=[
-                Argument('deliveryMethod', choices=['WEBHOOK', 'EMAIL']),
-                Argument('deliveryAddress')
-            ]))
-        ]))
-    ]
-    async def run(self, *args, **kwargs):
-        appId = kwargs.pop('appId')
-        appVersion = kwargs.pop('appVersion')
-        self.t.apps.patchApp(appId=appId, appVersion=appVersion, jobAttributes=kwargs)
-        return 'updated job attributes successfully'
+    async def run(self, *args, **kwargs):
+        volume_info = self.t.pods.get_volume(volume_id=kwargs['volume_id'])
+        kwargs['connection'].system = volume_info.volume_id
+        kwargs['connection'].pwd = "/"
+        return f"successfully entered the volume {kwargs['connection'].system}"
     
 
-class get_apps(baseCommand.BaseCommand):
+class exit_volume(baseCommand.BaseCommand):
     """
-    @help: get a list of all available apps
+    @help: exit the volume you are currently in 
     """
-    return_fields = ['id', 'version' 'runtime', 'containerImage']
-    optional_arguments = [
-        Argument('listType', choices=[
-            'OWNED',
-            'SHARED_PUBLIC',
-            'SHARED_DIRECT',
-            'READ_PERM', 
-            'MINE',
-            'ALL'
-        ])
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
+    required_arguments = [
+        Argument('volume_id', positional=True)
     ]
     async def run(self, *args, **kwargs):
-        return self.t.apps.getApps(**kwargs)
+        kwargs['connection'].system = ""
+        kwargs['connection'].pwd = ""
+        return f"successfully exited the volume {kwargs['volume_id']}"
     
 
-class get_app(baseCommand.BaseCommand):
+class update_volume(create_volume):
     """
-    @help: get a specific app
+    @help: update a volume's information
     """
-    return_fields = ['id', 'version' 'runtime', 'containerImage']
+    supports_config_file=True
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
+    async def run(self, *args, **kwargs):
+        return self.t.pods.update_volume(**kwargs)
+    
+
+class delete_volume(baseCommand.BaseCommand):
+    """
+    @help: delete a volume
+    """
+    decorator=decorators.NeedsConfirmation()
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
     required_arguments = [
-        Argument('appId', size_limit=(1, 80), positional=True),
+        Argument('volume_id', positional=True)
     ]
-    optional_arguments = [
-        Argument('appVersion', size_limit=(1, 64))
+    async def run(self, *args, **kwargs):
+        return self.t.pods.delete_volume_files(**kwargs)
+
+
+class dir(baseCommand.BaseCommand):
+    """
+    @help: list all files in the selected volume
+    """
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
+    required_arguments = [
+        Argument('volume_id', positional=True)
     ]
     async def run(self, *args, **kwargs):
-        if 'appVersion' not in kwargs:
-            version = self.t.apps.getAppLatestVersion(**kwargs).version
-            kwargs['appVersion'] = version
-        return self.t.apps.getApp(**kwargs)
+        return self.t.pods.list_volume_files(**kwargs)
     
 
-class is_app_enabled(baseCommand.BaseCommand):
+class upload_volume(baseCommand.BaseCommand):
     """
-    @help: check if the app is enabled
+    @help: upload a file from your local machine to the volume
     """
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id'), commandOpts.CHECK_PWD('path',)]
     required_arguments = [
-        Argument('appId', size_limit=(1, 80), positional=True),
+        Argument('volume_id', positional=True),
+        Argument('path'),
+        Argument('file')
     ]
     async def run(self, *args, **kwargs):
-        return self.t.apps.isEnabled(**kwargs)
+        return self.t.pods.upload_to_volume(**kwargs)
     
 
-class enable_app(is_app_enabled):
+class set_volume_permission(baseCommand.BaseCommand):
     """
-    @help: enable the app
+    @help: set the permission for a user on a volume
     """
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
+    required_arguments = [
+        Argument('volume_id', positional=True),
+        Argument('username'),
+        Argument('level')
+    ]
     async def run(self, *args, **kwargs):
-        return self.t.apps.enableApp(**kwargs)
-    
+        user = kwargs.pop('username')
+        kwargs['user'] = user
+        return self.t.pods.set_volume_permission(**kwargs)
+
 
-class disable_app(is_app_enabled):
+class get_volume_permissions(baseCommand.BaseCommand):
     """
-    @help: disable the app
+    @help: set the permission for a user on a volume
     """
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
+    required_arguments = [
+        Argument('volume_id', positional=True),
+    ]
     async def run(self, *args, **kwargs):
-        return self.t.apps.disableApp(**kwargs)
+        return self.t.pods.get_volume_permission(**kwargs)
     
 
-class delete_app(is_app_enabled):
+class delete_volume_permission(baseCommand.BaseCommand):
     """
-    @help: delete the app
+    @help: delete the persmission for a user on a volume
     """
     decorator=decorators.NeedsConfirmation()
+    required_arguments = [
+        Argument('volume_id', positional=True),
+        Argument('username'),
+        Argument('level')
+    ]
     async def run(self, *args, **kwargs):
-        return self.t.apps.disableApp(**kwargs)
+        user = kwargs.pop('username')
+        kwargs['user'] = user
+        return self.t.pods.delete_volume_permission(**kwargs)
     
 
-class undelete_app(is_app_enabled):
+class get_snapshots(baseCommand.BaseCommand):
     """
-    @help: undo a deletion of an app
+    @help: get a list of snapshots on the tenant you have access to
     """
     async def run(self, *args, **kwargs):
-        return self.t.apps.undeleteApp(**kwargs)
+        return self.t.pods.get_snapshots()
+    
+
+class create_snapshot(baseCommand.BaseCommand):
+    """
+    @help: create a backup of the volume selected or specific files in the volume
+    """
+    supports_config_file=True
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('source_volume_id'), commandOpts.CHECK_PWD(('source_volume_path', 'destination_path'))]
+    required_arguments = [
+        Argument('snapshot_id', positional=True),
+        Argument('source_volume_id', positional=True),
+        Argument('source_volume_path')
+    ]
+    optional_arguments = [
+        Argument('destination_path', description="Required if your snapshot is of a single file"),
+        Argument('description', arg_type='str_input'),
+        Argument('size_limit', data_type='int', description='maximum size in megabytes of the snapshot'),
+        Argument('cron'),
+        Argument('retention_policy')
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.pods.create_snapshot(**kwargs)
     
 
-class get_app_history(is_app_enabled):
+class get_snapshot(baseCommand.BaseCommand):
     """
-    @help: get the history of changes to an application
+    @help: get snapshot information
     """
+    required_arguments = [
+        Argument('snapshot_id', positional=True)
+    ]
     async def run(self, *args, **kwargs):
-        return str(self.t.apps.getAppHistory(**kwargs))
+        return self.t.pods.get_snapshot(**kwargs)
     
 
-class get_app_user_perms(baseCommand.BaseCommand):
+class update_snapshot(baseCommand.BaseCommand):
     """
-    @help: get list of user permissions for the app
+    @help: update snapshot information
     """
+    supports_config_file=True
     required_arguments = [
-        Argument('appId', size_limit=(1, 80), positional=True),
-        Argument('userName', size_limit=(1, 80))
+        Argument('snapshot_id', positional=True)
+    ]
+    optional_arguments = [
+        Argument('description', arg_type='str_input'),
+        Argument('size_limit', data_type='int'),
+        Argument('cron'),
+        Argument('retention_policy')
     ]
     async def run(self, *args, **kwargs):
-        return str(self.t.apps.getUserPerms)
+        return self.t.pods.update_snapshot(**kwargs)
     
 
-class grant_app_user_perms(baseCommand.BaseCommand):
+class delete_snapshot(baseCommand.BaseCommand):
     """
-    @help: grant user perms for a specific user on an app
+    @help: delete snapshot information
     """
+    decorator=decorators.NeedsConfirmation()
     required_arguments = [
-        Argument('appId', size_limit=(1, 80), positional=True),
-        Argument('userName', size_limit=(1, 80)),
-        Argument('permissions', arg_type='input_list', data_type=Argument('permission', choices=['READ', 'MODIFY', 'EXECUTE']))
+        Argument('snapshot_id', positional=True)
     ]
     async def run(self, *args, **kwargs):
-        return self.t.apps.grantUserPerms(**kwargs)
+        return self.t.pods.delete_snapshot(**kwargs)
     
 
-class revoke_app_user_perms(grant_app_user_perms):
+class list_snapshot_files(baseCommand.BaseCommand):
     """
-    @help: revoke perms for a specific user on an app
+    @help: list the files in a snapshot
     """
+    required_arguments = [
+        Argument('snapshot_id', positional=True)
+    ]
     async def run(self, *args, **kwargs):
-        return self.t.apps.revokeUserPerms(**kwargs)
+        return self.t.pods.list_snapshot_files(**kwargs)
+
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/arguments/argument.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/arguments/argument.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
                  data_type: ALLOWED_DATA_TYPES | typing.Type[AbstractArgument] = 'string',
                  arg_type: ALLOWED_ARG_TYPES | typing.Literal['standard']='standard',
                  choices: list | typing.Type[DynamicChoiceList] | None=None, 
                  action: typing.Literal['store', 'store_true', 'store_false']="store", 
                  description: str="",
                  positional: bool=False,
                  default_value=None,
+                 depends_on: list = [],
                  size_limit: tuple=(0,4096)):
         if arg_type not in typing.get_args(ALLOWED_ARG_TYPES) and arg_type != 'standard':
             raise ValueError(f"The arg type parameter in the argument {self.__class__.__name__} must be in the list {ALLOWED_ARG_TYPES}. Got arg type {arg_type}")
         if data_type not in typing.get_args(ALLOWED_DATA_TYPES) and not issubclass(data_type.__class__, AbstractArgument):
             raise ValueError(f"The data type argument provided to the argument {self.__class__.__name__} must be in the list {ALLOWED_DATA_TYPES}, or must be a subclass of AbstractArgument")
         if action not in typing.get_args(ALLOWED_ACTIONS):
             raise ValueError(f"Action {action} not in the list {ALLOWED_ACTIONS}, in argument {self.__class__.__name__}")
@@ -61,14 +62,15 @@
         if self.arg_type != 'standard':
             action = 'store_true'
         self.action = action
         self.description = description
         self.positional = positional
         self.default_value = default_value
         self.size_limit=size_limit
+        self.depends_on = depends_on
 
         self.truncated_arg = None
         self.full_arg = f"--{self.argument}"
 
     def verify_standard_value(self, value):
         if self.arg_type == "standard":
             #print(f"ARGUMENT NAME: {self.argument}\nARGUMENT VALUE: {value}\n")
@@ -84,16 +86,14 @@
                 raise ValueError(f"The argument {self.argument} requires a datatype {self.data_type}")
             if type(value) == int:
                 if value >= max_ or value < min_:
                     raise ValueError(f"The argument {self.argument} must be a value in the range {self.size_limit}")
             elif type(value) == str and (len(value) >= max_ or len(value) < min_):
                 raise ValueError(f"The argument {self.argument} must be between the sizes {self.size_limit}")
             elif self.choices and value not in self.choices:
-                print(value)
-                print(self.choices)
                 raise ValueError(f"The value for argument {self.argument} must be in the list {self.choices}")
             elif value == None and self.default_value:
                 value = self.default_value
         return value
 
     def json(self):
         json = {
@@ -103,26 +103,27 @@
             'choices':self.choices,
             'action':self.action,
             'description':self.description,
             'positional':self.positional,
             'default_value':self.default_value,
             'size_limit':self.size_limit,
             'truncated_arg':self.truncated_arg,
-            'full_arg':self.full_arg
+            'full_arg':self.full_arg,
+            'depends_on':self.depends_on
         }
         if self.data_type in ('string', 'int', 'bool'):
             json['data_type'] = self.data_type
         else:
             json['data_type'] = self.data_type.json()
         return json
     
     def help_message(self):
         help = {"name":self.argument,
                 "description":f"{self.description}"}
-        if self.choices:
+        if self.choices and isinstance(self.choices, list):
             help['choices'] = self.choices
         if self.positional:
             help['syntax'] = f"<{self.argument}>"
         elif self.action == 'store':
             help['syntax'] = f"{self.truncated_arg}/{self.full_arg} <{self.argument}>"
         else:
             help['syntax'] = f"{self.truncated_arg}/{self.full_arg}"
@@ -139,21 +140,21 @@
     def str(self):
         help_str = f"{self.truncated_arg}/{self.full_arg} "
         if self.positional:
             help_str = f"<{self.argument}> "
         elif self.action == 'store':
             help_str += f"<{self.argument}> "
         if self.arg_type != 'standard':
-            help_str += ' (f)'
+            help_str += ' (f)\t'
         return help_str
 
 
 class Form(Argument):
-    def __init__(self, form_name, arguments_list):
-        super().__init__(form_name, arg_type='form')
+    def __init__(self, form_name, arguments_list, description=None):
+        super().__init__(form_name, arg_type='form', description=description)
         for argument in arguments_list:
             if argument.arg_type == 'standard':
                 argument.arg_type = 'str_input'
         self.arguments_list = {argument.argument:argument for argument in arguments_list}
 
     def json(self):
         fields = {argument_name:argument.json() for argument_name, argument in self.arguments_list.items()}
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/baseCommand.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/baseCommand.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 import ast
 import json
 from typing import Type
 import typing
 from abc import abstractmethod, ABC
 import os
 from pprint import pprint
+from datetime import datetime
 
 from commands import decorators # I finally understand. Imported at the top level by serverRun, so it can only see packages from that vantage point
 from utilities import exceptions
 from commands.arguments.argument import Argument, DynamicChoiceList, ALLOWED_ARG_TYPES
 from socketopts import schemas
 from commands import dataFormatters
 
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(f"{__file__}")))
-saved_command = os.path.join(__location__, r'entered_command.json')
+saved_command_root_dir = os.path.join(__location__, r'..\user_files')
 
 
 def get_kwargs(function):
     sig = inspect.signature(function)
     keyword_args = [param.name for param in sig.parameters.values() if param.default != inspect.Parameter.empty]
     return keyword_args
 
@@ -80,14 +81,20 @@
     def __check_decorator(self, name, attrs):
         if 'decorator' in list(attrs.keys()) and type(attrs['decorator']) not in decorators.DECORATOR_LIST:
             raise TypeError(f"The decorator parameter of the command {name} is invalid. Must be set to None or to a decorator type. Currently is {type(attrs['decorator'])}")
         
     def __check_command_opt(self, name, attrs):
         if 'command_opt' in list(attrs.keys()) and type((attrs['command_opt'])) != list:
             raise TypeError(f"The command opt attribute of the command {name} must be a list!")
+        
+
+class UpdatableFormRetriever(abc.ABC):
+    @abc.abstractmethod
+    def __call__(self, tapis_instance, **kwargs):
+        pass
 
 
 class HelpMenu:
     def __init__(self, required_arguments: dict[str, Argument], optional_arguments: dict[str, Argument]):
         self.required_arguments = required_arguments
         self.optional_arguments = optional_arguments
         self.arguments = {**required_arguments, **optional_arguments}
@@ -108,179 +115,242 @@
 class BaseCommand(ABC, HelpStringRetriever, metaclass=CommandMetaClass):
     decorator = None
     return_fields: list = []
     command_opt: list = None
     supports_config_file: bool = False
     required_arguments: list[Argument] | dict = list()
     optional_arguments: list[Argument] | dict = list()
+    updateable_form_retriever: UpdatableFormRetriever = None
     def __init__(self):
         self.t = None
         self.username = None
         self.password = None
         self.server = None
         self.arguments = dict()
         self.return_formatter: dataFormatters.BaseDataFormatter = dataFormatters.BaseDataFormatter(self.return_fields)
-        self.default_commands()
+        self.default_arguments()
         if self.supports_config_file:
             self.optional_arguments.append(Argument('file'))
         if isinstance(self.required_arguments, list):
             self.required_arguments = {argument.argument:argument for argument in self.required_arguments}
             self.arguments.update(**self.required_arguments)
         if isinstance(self.optional_arguments, list):  
             self.optional_arguments = {argument.argument:argument for argument in self.optional_arguments}
             self.arguments.update(**self.optional_arguments)
         self.positional_arguments = [arg_name for arg_name, arg in self.required_arguments.items() if arg.positional]
         self.form_arguments = [arg_name for arg_name, arg in self.arguments.items() if arg.arg_type not in  ('standard', 'silent')]
         self.help: dict[dict[str, list[dict[str, str]]]] = dict()
 
         self.command_execution_sequence = []
-        if self.supports_config_file:
-            self.command_execution_sequence.append(self.handle_config_file)
         if self.positional_arguments:
             self.command_execution_sequence.append(self.check_for_positionals)
         if self.command_opt:
             self.command_execution_sequence.append(self.handle_arg_opts)
         self.command_execution_sequence.append(self.verify_argument_rules_followed)
         if self.form_arguments:
             self.command_execution_sequence.append(self.handle_form_input)
         self.command_execution_sequence.append(self.verify_argument_rules_followed)
         self.command_execution_sequence.append(self.filter_kwargs)
 
-    def default_commands(self):
-        default_commands = [Argument('connection', arg_type='silent'),
+    def default_arguments(self):
+        """
+        these are pseudarguments that allow some non-argument data to be passed to the command. This is a bit hacky, but its programatically necessary in the context of this framework
+        """
+        default_arguments = [Argument('connection', arg_type='silent'),
                             Argument('verbose', arg_type='silent'),
                             Argument('help', arg_type='silent'),
                             Argument('positionals', arg_type='silent')]
         
-        for command in default_commands:
+        for command in default_arguments:
             self.required_arguments.append(command)
 
     async def verify_argument_rules_followed(self, kwargs):
-        print("ACTIVATED THE ARGUMENT RULES TESTER")
+        """
+        verify that the rules for each argument are followed, this is the argument validation
+        """
         for name, value in self.arguments.items():
             if name in self.required_arguments and kwargs[name] == None:
                 raise Exception(f"The argument {name} is required by the command {self.__class__.__name__}")
             elif name in kwargs and name in self.required_arguments and name not in self.form_arguments:
                 kwargs[name] = self.required_arguments[name].verify_standard_value(kwargs[name])
             elif name in kwargs and name in self.optional_arguments and name not in self.form_arguments:
                 kwargs[name] = self.optional_arguments[name].verify_standard_value(kwargs[name])
+            if kwargs[name] and value.depends_on:
+                for dependency in value.depends_on:
+                    if not kwargs[dependency]:
+                        raise Exception(f"The argument {name} requires the arguments {value.depends_on}")
         return kwargs
 
     async def filter_kwargs(self, kwargs):
+        """
+        filters out kwargs that have None value, Tapis breaks if I dont do this
+        """
         filtered_kwargs = dict()
         for arg, value in kwargs.items():
             if arg in self.arguments and value or arg in self.required_arguments or (value == False and arg in self.arguments and self.arguments[arg].arg_type == 'standard'):
                 filtered_kwargs[arg] = value
         return filtered_kwargs
 
     async def handle_config_file(self, kwargs):
+        """
+        when there is a config file submitted, that config file overrides all the other received kwargs
+        """
         if kwargs['file']:
             with open(kwargs['file'], 'r') as f:
-                kwargs = json.loads(f.read)
+                kwargs = json.load(f)
+            if 'error' in kwargs:
+                kwargs.pop('error')
         return kwargs
     
-    async def handle_form_input(self, kwargs):
+    async def handle_form_input(self, kwargs, complex_args_flag=True):
+        """
+        handles forms when the user selects to fill them out
+        """
+        existing_values = dict()
+        if self.updateable_form_retriever:
+            existing_values = self.return_formatter.obj_to_dict(self.updateable_form_retriever(self.t, **kwargs))
         for arg_name in self.form_arguments:
             if kwargs[arg_name] or arg_name in self.required_arguments:
-                request = schemas.FormRequest(request_content={arg_name:self.arguments[arg_name] for arg_name in self.form_arguments if kwargs[arg_name] or arg_name in self.required_arguments})
+                request = schemas.FormRequest(request_content={arg_name:self.arguments[arg_name]}, existing_data=existing_values)
                 await kwargs['connection'].send(request)
                 response: schemas.FormResponse = await kwargs['connection'].receive()
                 kwargs.update(**response.request_content)
         return kwargs
-    
+
     async def handle_arg_opts(self, kwargs):
+        """
+        arg opts handle special operations, like supporting relative file paths, and system entry
+        """
         for opt in self.command_opt:
             kwargs = opt(kwargs)
         return kwargs
     
     async def check_for_positionals(self, kwargs):
+        """
+        some commands contain positional arguments. This function handles that circumstance
+        """
         for arg_name, value in zip(self.positional_arguments, kwargs['positionals']):
             kwargs[arg_name] = value
         return kwargs
 
     def set_t_and_creds(self, t, username, password, server):
+        """
+        whenever the tenant or user changes, the new tapis object with the new credentials must be passed to each command to ensure they are operating on the currect user
+        """
         self.t = t
         self.username = username
         self.password = password
         self.server = server
         for key, arg in self.optional_arguments.items():
             if issubclass(arg.choices.__class__, DynamicChoiceList):
                 arg.choices = arg.choices(self.t)
 
     def update_args_with_truncated(self, truncated_args_dict):
+        """
+        when the command group finishes processing all the truncated arguments, they get passed back here to be processed and assigned
+        """
         try:
             for key in self.required_arguments:
                 self.required_arguments[key].truncated_arg = f"-{truncated_args_dict[key]}"
             for key in self.optional_arguments:
                 self.optional_arguments[key].truncated_arg = f"-{truncated_args_dict[key]}"
             self.help['required'] = self.__argument_help_compiler(self.required_arguments)
             self.help['optional'] = self.__argument_help_compiler(self.optional_arguments)
         except Exception as e:
             print(self.__class__.__name__)
             raise e
         
     def __argument_help_compiler(self, arg_dict: dict[str, Argument]):
+        """
+        compile the help menus based on stored command metadata
+        """
         verbose_dict = dict()
         standard_str = str()
         for name, argument in arg_dict.items():
             if not (name in self.required_arguments and name in self.form_arguments) and argument.arg_type != 'silent':
                 verbose_dict[name] = argument.help_message()
                 standard_str += argument.str()
         return {'verbose':verbose_dict, 'standard':standard_str}
 
     def __get_help(self, verbose):
+        """
+        return the compiled help menus
+        """
         help_dict = {"Command":self.__class__.__name__,
                     "Description":self.help_string_retriever()}
         if not verbose:
             help_dict.update(**{
                 "Syntax":f"{self.__class__.__name__} {self.help['required']['standard']}\n(Optional Arguments) {self.help['optional']['standard']}"})
         else:
             help_dict.update(**{
                 "Syntax":f"{self.__class__.__name__}",
                 "Required Arguments":self.help['required']['verbose'],
                 "Optional Arguments":self.help['optional']['verbose']})
         return help_dict
     
     def brief_help(self):
+        """
+        return non verbose help
+        """
         return {"Command":self.__class__.__name__,
                 "Description":self.help_string_retriever()}
     
     @abstractmethod
     async def run(self, *args, **kwargs):
+        """
+        contains the actual command information at command definition
+        """
         pass
 
     async def __call__(self, **kwargs):
-        pprint(kwargs)
-        if self.decorator:
-            try:
-                return_value = await self.decorator(input_command=self, **kwargs)
-            except (ValueError, exceptions.NoConfirmationError) as e:
-                return f"Command execution failed due to {e}"
-
-        if kwargs['help']:
-            return self.__get_help(verbose=kwargs['verbose'])
-        for handler in self.command_execution_sequence:
-            print(f"EXECUTING: {handler.__name__}")
-            kwargs = await handler(kwargs)
-            pprint(f"{kwargs}\n")
+        """
+        runs all command meta-operations
+        """
+        if self.supports_config_file and kwargs['file']:
+            new_kwargs = await self.handle_config_file(kwargs)
+            for arg_name, arg in kwargs.items():
+                if arg_name in ('connection', 'positionals', 'verbose', 'help'):
+                    new_kwargs[arg_name] = arg
+            kwargs = new_kwargs
         else:
-            try:
-                return_value = await self.run(**kwargs)
-            except exceptions.Shutdown as e:
-                raise e
-            except Exception as e:
-                with open(saved_command, 'a') as f:
+            if self.decorator:
+                try:
+                    return_value = await self.decorator(input_command=self, **kwargs)
+                except (ValueError, exceptions.NoConfirmationError) as e:
+                    return f"Command execution failed due to {e}"
+
+            if kwargs['help']:
+                return self.__get_help(verbose=kwargs['verbose'])
+            for handler in self.command_execution_sequence:
+                kwargs = await handler(kwargs)
+        try:
+            return_value = await self.run(**kwargs)
+        except (exceptions.Shutdown, exceptions.Exit) as e:
+            raise e
+        except Exception as e:
+            if self.supports_config_file:
+                current_date = datetime.now()
+                formatted_date = current_date.strftime("%m-%d-%y")
+                main_save_path = f"{saved_command_root_dir}\\{formatted_date}"
+                try:
+                    os.listdir(main_save_path)
+                except:
+                    os.makedirs(main_save_path)
+                number = len(os.listdir(main_save_path))
+                file_save_path = f"{main_save_path}\\{self.__class__.__name__}_{number}.json"
+                with open(file_save_path, 'w') as f:
                     kwargs.pop('connection')
-                    f.write(json.dumps(kwargs))
-                    print(f"Argument input failure, command data written to file {saved_command}")
-                    raise e
-        if self.return_formatter:
-            return_value = self.return_formatter(return_value, kwargs['verbose'])
-        else:
-            return_value = str(return_value)
+                    kwargs.pop('positionals')
+                    kwargs.pop('verbose')
+                    kwargs.pop('help')
+                    kwargs['error'] = str(e)
+                    json.dump(kwargs, f, indent=4)
+                    raise Exception(e, f"Argument input failure, command data written to file {file_save_path}")
+            raise e
+        return_value = self.return_formatter(return_value, kwargs['verbose'])
         return return_value
     
 
 class BaseQuery(BaseCommand):
     def get_pod_credentials(self, id):
         uname, pword = self.t.pods.get_pod_credentials(pod_id=id).user_username, self.t.pods.get_pod_credentials(pod_id=id).user_password
         return uname, pword
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/commandMap.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/commandMap.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,16 @@
 
 class Query(baseCommand.BaseCommandMap):
     """
     @help: run integrated query CLIs
     """
     command_map = {
         'postgres': postgres.postgres(),
-        'neo4j': neo4j.neo4j()
+        'neo4j': neo4j.neo4j(),
+        'get_neo4j_pod_uri':neo4j.get_neo4j_pod_uri(),
     }
 
 
 class ArgsGenerator:
     def generate_truncated_arguments(self, arg_dict: dict) -> dict:
         truncation_dict = dict()
         for argument_name in arg_dict.keys():
@@ -205,15 +206,16 @@
     groups = {
         'Systems': Systems(),
         'General': General(),
         'Pods': Pods(),
         'Files': Files(),
         'Apps': Apps(),
         'Query': Query(),
-        'Volumes':Volumes()
+        'Volumes':Volumes(),
+        'Jobs': Jobs()
     }
     def __init__(self):
         truncated_arguments = self.generate_truncated_arguments(self.arguments)
         for command in self.aggregate_command_map.values():
             command.update_args_with_truncated(truncated_arguments)
         for name, argument in self.arguments.items():
             argument.truncated_arg = truncated_arguments[name]
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/commandOpts.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/commandOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/dataFormatters.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/dataFormatters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import pprint
+
+
 class BaseDataFormatter:
     def __init__(self, non_verbose_fields: list[list | str] = []):
         self.non_verbose_fields = non_verbose_fields
 
     def obj_to_dict(self, obj):
         if isinstance(obj, (int, float, str, bool)):
             return obj 
@@ -11,31 +14,34 @@
             return type(obj)(self.obj_to_dict(item) for item in obj) 
         elif obj == None:
             return None
         elif isinstance(obj, object):
             return self.obj_to_dict(obj.__dict__) 
         return None 
     
-    def non_verbose_formatter(self, serialized_data, formatted=dict()):
+    def non_verbose_formatter(self, serialized_data):
+        formatted = dict()
         if self.non_verbose_fields:
             for field in self.non_verbose_fields:
                 if isinstance(field, str):
                     formatted[field] = serialized_data[field]
+                    print(serialized_data[field])
                 elif isinstance(field, list):
                     formatted[field] = self.non_verbose_formatter(serialized_data[field])
             return formatted
         else:
             return serialized_data
     
     def __call__(self, data, verbose):
         serialized = self.obj_to_dict(data)
         if verbose:
             return serialized
         if isinstance(serialized, list) and self.non_verbose_fields:
             return_data = list()
             for fragment in serialized:
-                return_data.append(self.non_verbose_formatter(fragment))
+                non_verbose_fragment = self.non_verbose_formatter(fragment)
+                return_data.append(non_verbose_fragment)
             return return_data
         return self.non_verbose_formatter(serialized)
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/decorators.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/fileCommands.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/fileCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/jobCommands.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/jobCommands.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 if __name__ != "__main__":
     from . import baseCommand, decorators
     from .arguments import argument
     from . import appCommands
+    from commands import commandOpts
     Argument = argument.Argument
 
 
 class hide_job(baseCommand.BaseCommand):
     """
     @help: hide a job if its already completed
     """
@@ -51,15 +52,15 @@
         Argument('limit', data_type='int'),
         Argument('skip', data_type='int'),
     ]
     async def run(self, *args, **kwargs):
         return self.t.jobs.getJobHistory(**kwargs)
     
 
-class get_jobs(hide_job):
+class get_jobs(baseCommand.BaseCommand):
     """
     @help: list all available jobs on the system
     """
     return_fileds = ['appId', 'appVersion', 'execSystemId', 'uuid']
     async def run(self, *args, **kwargs):
         return self.t.jobs.getJobList()
     
@@ -77,40 +78,48 @@
         Argument('format', description='something like zip or tar')
     ]
     async def run(self, *args, **kwargs):
         self.t.jobs.getJobOutputDownload(**kwargs)
         return f"job {kwargs['jobUuid']} output successfully downloaded"
     
 
-class get_job_status:
+class get_job_status(baseCommand.BaseCommand):
     """
     @help: retrieve the status of a job
     """
     required_arguments = [
         Argument('jobUuid')
     ]
     async def run(self, *args, **kwargs):
         return self.t.jobs.getJobStatus(**kwargs)
     
 
 class resubmit_job(baseCommand.BaseCommand):
     """
     @help: resubmit a job with the same arguments as the original submission
     """
+    return_fields = ['name', 'status', 'uuid', 'appId', 'execSystemId']
     required_arguments = [
         Argument('jobUuid'),
     ]
     async def run(self, *args, **kwargs):
         return self.t.jobs.resubmitJob(**kwargs)
     
 
 class submit_job(appCommands.assign_default_job_attributes):
     """
     @help: submit a job to be run on the select system based on a pre-existing app
     """
+    return_fields = ['name', 'status', 'uuid', 'appId', 'execSystemId']
+    command_opt = [commandOpts.CHECK_EXPLICIT_ID('execSystemId')]
+    required_arguments = [
+        Argument('appId', size_limit=(1, 80), positional=True),
+        Argument('appVersion', size_limit=(1, 64)),
+        Argument('name', positional=True)
+    ]
     async def run(self, *args, **kwargs):
         return self.t.jobs.submitJob(**kwargs)
     
 
 class share_job(baseCommand.BaseCommand):
     """
     @help: share a job with the select grantee user
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/podCommands.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/podCommands.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,62 +40,80 @@
     supports_config_file=True
     required_arguments=[
         Argument('pod_id', positional=True),
         Argument('pod_template', positional=True)
     ]
     optional_arguments=[
         Argument('description', arg_type='str_input', size_limit=(0, 2048)),
-        Argument('command', arg_type='input_list', data_type=argument.Argument('command', arg_type='str_input')),
+        Argument('command', arg_type='input_list', data_type=argument.Argument('command', arg_type='str_input'), description="Command to run in the pod"),
         Argument('environment_variables', arg_type='input_dict', data_type=argument.Argument('environment_variable', arg_type='str_input')),
-        Argument('data_request', arg_type='input_list', data_type=argument.Argument('data_request', arg_type='str_input')),
-        Argument('roles_required', arg_type='input_list', data_type=argument.Argument('required_role', arg_type='str_input')),
+        Argument('roles_required', arg_type='input_list', data_type=argument.Argument('required_role', arg_type='str_input'), description='what role is required by the user to access this pod?'),
         Argument('time_to_stop_default', data_type='int'),
         Argument('time_to_stop_instance', data_type='int'),
         Argument('volume_mounts', arg_type='input_dict', data_type=argument.Form(
             'volume_mount', arguments_list = [
                 Argument('type', choices=['tapisvolume', 'tapissnapshot', 'pvc']),
-                Argument("mount_path"),
-                Argument('sub_path')
+                Argument("mount_path", description='This is top level path you want to mount the volume on inside the pod. This is something like <neo4j-home>\data for a neo4j pod. Data from that path will load to the mount and become persistent'),
+                Argument('sub_path', description='If you want to only load a single file, like file.txt (which is inside the parent mount path) you can specify here')
             ]
-        )),
+        ), description="Used to attach the pod to an existing kubernetes volume to provide pod persistence (in case of crash). Each key is the volume_id"),
         Argument('networking', arg_type='input_dict', data_type=argument.Form(
             'network', arguments_list = [
-                Argument('protocol'),
+                Argument('protocol', description='Something like https'),
                 Argument('port', data_type='int'),
                 Argument('url')
             ]
-        )),
+        ), description='Important networking configuration. You probably shouldnt touch this, but I wont stop you'),
         argument.Form(
             'resources', arguments_list = [
                 Argument('cpu_request', data_type='int'),
                 Argument('cpu_limit', data_type='int'),
                 Argument('mem_request', data_type='int'),
                 Argument('mem_limit', data_type='int'),
             ]
         )
     ]
     async def run(self, *args, **kwargs) -> str:
         template_name = kwargs['pod_template']
         template_formats = (f"template/{template_name}", f"{self.username}/{template_name}", template_name)
+        if 'volume_mounts' in kwargs and kwargs['volume_mounts']:
+            for mount_name, mount in kwargs['volume_mounts'].items():
+                if mount['type'] == 'tapisvolume':
+                    try:
+                        self.t.pods.get_volume(volume_id=mount_name)
+                    except:
+                        self.t.pods.create_volume(volume_id=mount_name)
+                elif mount['type'] == 'tapissnapshot':
+                    try:
+                        self.t.pods.get_snapshot(snapshot_id=mount_name)
+                    except:
+                        raise Exception('snapshot not found')
         for template_format in template_formats:
             try:
                 kwargs['pod_template'] = template_format
-                pod_information = self.t.pods.create_pod(**kwargs)
+                results = self.t.pods.create_pod(**kwargs)
                 break
             except TapisErrors.BadRequestError as e:
                 if template_format != template_formats[-1]:
                     continue
                 raise ValueError(f"Failed to execute pod creation due to {str(e)}")
-        return pod_information
+        return results
+    
+
+class PodUpdatingRetriever(baseCommand.UpdatableFormRetriever):
+    def __call__(self, tapis_instance, **kwargs):
+        pod_data = tapis_instance.pods.get_pod(pod_id=kwargs["pod_id"])
+        return pod_data
     
 
 class update_pod(create_pod): # make it so the command retrieves current settings and sends them over so forms can append and edit instead of just overwrite
     """
     @help: update a pod. Must be restarted to stage changes
     """
+    updateable_form_retriever=PodUpdatingRetriever()
     return_fields = ['pod_id', 'pod_template', 'status']
     required_arguments=[
         Argument('pod_id', positional=True),
     ]
     async def run(self, *args, **kwargs):
         print(kwargs)
         pod_information = self.t.pods.update_pod(**kwargs)
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/query/neo4j.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,8 +21,19 @@
         return_value = graph.run(kwargs['expression'])
         print(type(return_value))
         if str(return_value) == '(No data)' and 'create' in kwargs['expression'].lower(): # if no data is returned (mostly if something is created) then just say 'success'
             return f'[+][{kwargs["id"]}@pods.{self.t.base_url.split("https://")[1]}:443] Success'
         elif str(return_value) == '(No data)':
             return f'[-][{kwargs["id"]}@pods.{self.t.base_url.split("https://")[1]}:443] KG is empty'
 
-        return return_value
+        return return_value
+    
+
+class get_neo4j_pod_uri(baseCommand.BaseCommand):
+    """
+    @help: get the uri for a neo4j pod to use in external database software
+    """
+    required_arguments = [
+        argument.Argument('id')
+    ]
+    async def run(self, *args, **kwargs) -> str:
+        return f"bolt+ssc://{kwargs['id']}.pods.{self.t.base_url.split('https://')[1]}:443"
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/query/postgres.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/query/postgres.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/serverCommands.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,26 @@
 
 if __name__ != "__main__":
     from . import baseCommand, decorators
     from utilities import exceptions
     from commands.arguments.argument import Argument
 
 
+class ServiceChecker:
+    def __init__(self, available_services: list):
+        self.available_services = available_services
+
+    def check_services(self, t):
+        tenant = t.tenants.get_tenant(tenant_id=t.tenant_id)
+        site_id = tenant.site_id
+        supported_services = t.tenants.get_site(site_id=site_id).services
+        filtered_supported_services = [service for service in supported_services if service in self.available_services]
+        return filtered_supported_services
+
+
 class get_tenants(baseCommand.BaseCommand):
     """
     @help: get a list of available tenants to authenticate with
     """
     async def run(self, *args, **kwargs):
         return_data = dict()
         tenants = self.t.tenants.list_tenants()
@@ -52,15 +64,14 @@
             results = await self.server.device_code_grant(tenant_uri, kwargs['connection'])
         elif auth == "federated":
             results = await self.server.federated_grant(tenant_uri, kwargs['connection'])
         else:
             results = None
         self.server.configure_decorators(self.server.username, self.server.password)
         self.server.update_credentials(self.server.t, self.server.username, self.server.password)
-        self.server.available_services = self.server.service_checker.check_services(self.server.t)
         return results
       
 
 class exit(baseCommand.BaseCommand):
     """
     @help: exit the CLI without shutting down the service
     """
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/commands/systemCommands.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/systemCommands.py`

 * *Files 27% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     
 
 class get_systems(baseCommand.BaseCommand):
     """
     @help: Gets and returns the list of systems the current Tapis service and account have access to
     @doc: this is an example of the doc segment of the docstring. not included in help message
     """
-    return_fields = ['id', 'systemType', 'host', 'enabled']
+    return_fields = ['id', 'systemType', 'host']
     optional_arguments = [
         Argument('listType', choices=['OWNED', 'SHARED_PUBLIC', 'ALL'])
     ]
     async def run(self, *args, **kwargs):
         systems = self.t.systems.getSystems(**kwargs)
         return systems
     
@@ -122,51 +122,51 @@
     this command will automatically create and upload the ssh keys
     """
     supports_config_file=True
     required_arguments=[
         Argument('id', size_limit=(1, 80), positional=True),
         Argument('systemType', choices=["LINUX", "S3", "IRODS", "GLOBUS"], description=
                                     """LINUX is a standard linux kernel
-                                    S3 refers to an AWS S3 Bucket
-                                    IRODS refers to an IRODS data management system
-                                    GLOBUS refers to a GLOBUS file system"""),
+S3 refers to an AWS S3 Bucket
+IRODS refers to an IRODS data management system
+GLOBUS refers to a GLOBUS file system"""),
         Argument('host', size_limit=(1, 256), description="In the case of Linux this is the hostname or IP of the HPC system you want to connect to. For S3, this is the AWS bucket URL"),
         Argument('defaultAuthnMethod', choices=['PASSWORD', "PKI_KEYS", "ACCESS_KEY", "TOKEN", "CERT"], description=
                                     """Depending on your systemType, you will be restricted to certain options.
-                                    Linux: PASSWORD, PKI_KEYS
-                                    S3: ACCESS_KEY
-                                    GLOBUS: TOKEN
-                                    IRODS: TOKEN
-                                    In the case you choose password, your username and password will either be your TACC account info, or the login info you used with federated/device_code grant"""),
+Linux: PASSWORD, PKI_KEYS
+S3: ACCESS_KEY
+GLOBUS: TOKEN
+IRODS: TOKEN
+In the case you choose password, your username and password will either be your TACC account info, or the login info you used with federated/device_code grant"""),
     ]
     optional_arguments=[
-        Argument('canExec', action='store_true', default_value=False),
+        Argument('canExec', action='store_true', default_value=False, depends_on=['jobRuntimes']),
         Argument('description', arg_type='str_input', size_limit=(0, 2048)),
         Argument('owner'),
         Argument('enabled', action='store_true'),
         Argument('effectiveUserId', default_value=r"${apiUserId}", size_limit=(0, 60)),
         Argument('bucketName'),
         Argument('rootDir', default_value='/', size_limit=(0, 4096)),
         Argument('port', data_type='int'),
         Argument('useProxy', action='store_true'),
         Argument('proxyHost', size_limit=(0, 256)),
         Argument('proxyPort', data_type='int'),
-        Argument('isDtn', action='store_true'),
+        Argument('isDtn', action='store_true', depends_on=['rootDir']),
         Argument('dtnSystemId', size_limit=(0, 80)),
         Argument('dtnMountPoint'),
-        Argument('canRunBatch', action='store_true'),
+        Argument('canRunBatch', action='store_true', depends_on=['batchScheduler', 'batchLogicalQueues', 'batchLogicalDefaultQueue']),
         Argument('enableCmdPrefix', action='store_true'),
         Argument('mpiCmd', size_limit=(0, 126), arg_type='str_input'),
         Argument('jobRuntimes', arg_type='input_list', data_type=argument.Form(
             'jobRuntime', arguments_list = [
                 Argument('runtimeType', choices=['DOCKER', 'SINGULARITY']), 
                 Argument('version')
                 ]
             )),
-        Argument('jobWorkingDir', default_value=r"HOST_EVAL($WORK2)", size_limit=(0, 4096)),
+        Argument('jobWorkingDir', default_value=r"HOST_EVAL($WORK2)", size_limit=(0, 4096), description='Where on this hpc system are jobs run?'),
         Argument('jobEnvVariables', arg_type='input_list', data_type=argument.Form(
             'jobEnvironmentVariable', arguments_list = [
                 Argument('key'),
                 Argument('value', default_value=''),
                 Argument('description', size_limit=(0, 2048), arg_type='str_input')
             ]
         )),
@@ -300,24 +300,105 @@
         system_info = self.t.systems.getSystem(systemId=kwargs['id'])
         kwargs['systemType'] = system_info.systemType
         kwargs['defaultAuthnMethod'] = system_info.defaultAuthnMethod
         return_info = await self.authenticate(kwargs)
         return return_info
     
 
+class SystemUpdatingRetriever(baseCommand.UpdatableFormRetriever):
+    def __call__(self, tapis_instance, **kwargs):
+        system_data = tapis_instance.systems.getSystem(systemId=kwargs["systemId"])
+        return system_data
+    
+
 class update_system(create_system):
     """
     @help: update a system with new information
     """
+    updateable_form_retriever = SystemUpdatingRetriever()
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('systemId')]
-    required_arguments = [
-        Argument('systemId', size_limit=(1, 80), positional=True)
+    required_arguments=[
+        Argument('systemId', size_limit=(1, 80), positional=True),
+    ]
+    optional_arguments=[
+        Argument('defaultAuthnMethod', choices=['PASSWORD', "PKI_KEYS", "ACCESS_KEY", "TOKEN", "CERT"], description=
+                                    """Depending on your systemType, you will be restricted to certain options.
+                                    Linux: PASSWORD, PKI_KEYS
+                                    S3: ACCESS_KEY
+                                    GLOBUS: TOKEN
+                                    IRODS: TOKEN
+                                    In the case you choose password, your username and password will either be your TACC account info, or the login info you used with federated/device_code grant"""),
+        Argument('host', size_limit=(1, 256), description="In the case of Linux this is the hostname or IP of the HPC system you want to connect to. For S3, this is the AWS bucket URL"),
+        Argument('description', arg_type='str_input', size_limit=(0, 2048)),
+        Argument('effectiveUserId', default_value=r"${apiUserId}", size_limit=(0, 60)),
+        Argument('port', data_type='int'),
+        Argument('useProxy', action='store_true'),
+        Argument('proxyHost', size_limit=(0, 256)),
+        Argument('proxyPort', data_type='int'),
+        Argument('dtnSystemId', size_limit=(0, 80)),
+        Argument('dtnMountPoint'),
+        Argument('canRunBatch', action='store_true'),
+        Argument('enableCmdPrefix', action='store_true'),
+        Argument('mpiCmd', size_limit=(0, 126), arg_type='str_input'),
+        Argument('jobRuntimes', arg_type='input_list', data_type=argument.Form(
+            'jobRuntime', arguments_list = [
+                Argument('runtimeType', choices=['DOCKER', 'SINGULARITY']), 
+                Argument('version')
+                ]
+            )),
+        Argument('jobWorkingDir', default_value=r"HOST_EVAL($WORK2)", size_limit=(0, 4096)),
+        Argument('jobEnvVariables', arg_type='input_list', data_type=argument.Form(
+            'jobEnvironmentVariable', arguments_list = [
+                Argument('key'),
+                Argument('value', default_value=''),
+                Argument('description', size_limit=(0, 2048), arg_type='str_input')
+            ]
+        )),
+        Argument('jobMaxJobs', data_type='int'),
+        Argument('jobMaxJobsPerUser', data_type='int'),
+        Argument('batchScheduler', choices=['SLURM', "CONDOR", "PBS", "SGE", "UGE", "TORQUE"]),
+        Argument('batchLogicalQueues', arg_type='input_list', data_type=argument.Form(
+            'batchLogicalQueue', arguments_list = [
+                Argument('name', size_limit=(1, 128)),
+                Argument('hpcQueueName', size_limit=(1, 128)),
+                Argument('maxJobs', data_type='int'),
+                Argument('maxJobsPerUser', data_type='int'),
+                Argument('minNodeCount', data_type='int'),
+                Argument('maxNodeCount', data_type='int'),
+                Argument('minCoresPerNode', data_type='int'),
+                Argument('maxCoresPerNode', data_type='int'),
+                Argument('minMemoryMB', data_type='int'),
+                Argument('maxMemoryMB', data_type='int'),
+                Argument('minMinutes', data_type='int'),
+                Argument('maxMinutes', data_type='int')
+            ]
+        )),
+        Argument('batchDefaultLoginQueue', size_limit=(1, 128)),
+        Argument('batchSchedulerProfile', choices=get_scheduler_profiles_choices()),
+        Argument('jobCapabilities', arg_type='input_list', data_type=argument.Form(
+            'jobCapability', arguments_list=[
+                Argument('category', choices=['SCHEUDLER', 
+                                              'OS', 'HARDWARE', 
+                                              'SOFTWARE', 'JOB', 
+                                              'CONTAINER', 'MISC', 
+                                              'CUSTOM']),
+                Argument('name', size_limit=(1, 128)),
+                Argument('datatype', choices=['STRING', 'INTEGER', 
+                                              'BOOLEAN', 'NUMBER', 
+                                              'TIMESTAMP']),
+                Argument('precedence', data_type='int'),
+                Argument('value')
+            ]
+        )),
+        Argument('tags', arg_type='input_list', data_type=Argument('tag', arg_type='str_input')),
+        Argument('notes', arg_type='str_input'),
+        Argument('importRefId')
     ]
     async def run(self, *args, **kwargs):
-        result = self.t.systems.putSystem(**kwargs)
+        result = self.t.systems.patchSystem(**kwargs)
         return result
     
 
 class is_system_enabled(baseCommand.BaseCommand):
     """
     @help: check to see if a system is enabled
     """
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/server/auth.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/server/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,11 +197,10 @@
                 continue
         success_message = schemas.AuthRequest(auth_request_type="success", message={
             "message":f"Successfully authenticated with {auth_type} authentication",
             "username":self.username,
             "url":link})
         self.configure_decorators(self.username, self.password)
         self.update_credentials(self.t, self.username, self.password)
-        self.available_services = self.service_checker.check_services(self.t)
         await connection.send(success_message)
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/server/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 import time
 import socket
 import asyncio
 import traceback
+import typing
+import os
+import json
 
 from tapipy.tapis import Tapis
 
-if __name__ != "__main__":
-    from commands import commandMap, decorators
-    from utilities import logger, exceptions
-    from socketopts import schemas, socketOpts
-    from server import auth
-else:
-    import commands.commandMap as commandMap
-
-
-class ServiceChecker:
-    def __init__(self, available_services: list):
-        self.available_services = available_services
-
-    def check_services(self, t):
-        tenant = t.tenants.get_tenant(tenant_id=t.tenant_id)
-        site_id = tenant.site_id
-        supported_services = t.tenants.get_site(site_id=site_id).services
-        filtered_supported_services = [service for service in supported_services if service in self.available_services]
-        return filtered_supported_services
+from commands import commandMap, decorators
+from utilities import logger, exceptions
+from socketopts import schemas, socketOpts
+from server import auth
 
 
 class ServerConnection(socketOpts.ServerSocketOpts):
     """
     connection object to wrap around async reader and writer to make work easier
     """
     def __init__(self, name, reader, writer, connection_list, debug=False):
@@ -42,35 +30,40 @@
 
     def set_status_device_authenticating(self):
         self.status = 'DEVICE_CODE_AUTH'
 
     def set_status_closed(self):
         self.status = 'CLOSED'
 
+    def set_status_exiting(self):
+        self.status = 'EXITING'
+
     def set_task(self, task: asyncio.Task):
         self.task = task
-        self.status == 'OPEN'
+        self.status = 'OPEN'
 
-    async def close(self):
+    async def close(self, connection_list_lock: asyncio.Lock):
         self.logger.info('ATTEMPTING TO CLOSE')
-        if self.status == 'OPEN':
-            self.task.cancel()
-            self.logger.info(self.task.result())
+        if self.status in ('OPEN', 'EXITING'):
+            result = self.task.cancel()
+            self.logger.info("successfully cancelled task")
             await self.send(self.shutdown_message)
             self.writer.close()
             await self.writer.wait_closed()
             self.status = 'CLOSED'
-            self.connection_list.remove(self)
-        elif self.status == 'DEVICE_CODE_AUTH':
+        elif self.status == 'DEVICE_CODE_AUTH': # only in the auth file
             await self.send(schemas.AuthRequest(error='cancelled authentication during device_code grant', auth_request_type='device_code'))
             self.writer.close()
             await self.writer.wait_closed()
         else:
             self.writer.close()
             await self.writer.wait_closed()
+        async with connection_list_lock:
+            self.connection_list.remove(self)
+        print(self.connection_list)
         self.logger.info('SUCCESSFULLY CLOSED')
 
 
 class Server(commandMap.AggregateCommandMap, logger.ServerLogger, decorators.DecoratorSetup, auth.ServerSideAuth):
     """
     Receives commands from the client and executes Tapis operations
     """
@@ -84,17 +77,14 @@
         self.t = None
         self.url = None
         self.access_token = None
         self.username = None
         self.password = None
         self.auth_type = None
 
-        self.service_checker = ServiceChecker(available_services=list(self.groups.keys()))
-        self.available_services = []
-
         self.__name__ = "Server"
         self.initialize_logger(self.__name__)
         # setting up socket server
         self.ip, self.port = IP, PORT
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.sock.setblocking(False)
         self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
@@ -104,19 +94,20 @@
         self.end_time = time.time() + self.SESSION_TIME # start the countdown on the timeout
 
         self.connections_list: list[ServerConnection] = []
 
         self.server = None
         self.num_connections = 0
 
+        self.connection_list_lock = asyncio.Lock()
         self.logger.info('initialization complete')
 
     async def close_connections(self):
-        for connection in self.connections_list:
-            await connection.close()
+        print([connection.status for connection in self.connections_list])
+        return await asyncio.gather(*[connection.close(self.connection_list_lock) for connection in self.connections_list])
 
     async def close(self):
         await self.close_connections()
         self.server.close()
         raise exceptions.Shutdown()
 
     async def check_timeout(self):
@@ -126,14 +117,17 @@
                 self.running = False
                 return 'server timed out'
             await asyncio.sleep(3)
     
     async def check_shutdown(self):
         while self.running:
             await asyncio.sleep(3)
+            for connection in self.connections_list:
+                if connection.status == 'EXITING':
+                    await connection.close(self.connection_list_lock)
         await self.close()
         self.logger.info("The server shutdown.")
         return None
 
     async def handshake(self, connection):
         self.logger.info("Handshake starting")
         if self.initial:  # if this is the first time in the session that the cli is connecting
@@ -155,36 +149,37 @@
         connection = ServerConnection(f"CON-{self.num_connections}", reader=reader, writer=writer, connection_list=self.connections_list, debug=self.debug)
         ip, port = writer.transport.get_extra_info('socket').getsockname()
         self.logger.info("Received connection request")
         try:
             await self.handshake(connection)
         except exceptions.InvalidCredentialsReceived as e:
             self.logger.warning("invalid credentials entered too many times. Cancelling request")
-            await connection.close()
+            await connection.close(self.connection_list_lock)
             return
         except exceptions.ClientSideError as e:
             self.logger.warning(f"Encountered client side error during startup handshake. {e}")
-            await connection.close()
+            await connection.close(self.connection_list_lock)
             return
         except Exception as e:
             self.logger.warning(e)
-            await connection.close()
+            await connection.close(self.connection_list_lock)
             return
         self.logger.info("connection is running now")
         await connection.send(schemas.ResponseData(request_content={name:argument.json() for name, argument in self.arguments.items()}))
         
         setup_response: schemas.ResponseData = await connection.receive()
         if not setup_response.request_content['setup_success']:
             self.logger.warning(f"The setup of the connection {connection.name} failed")
             return
 
         loop = asyncio.get_event_loop()
         task: asyncio.Task = loop.create_task(self.receive_and_execute(connection))
         connection.set_task(task)
         self.connections_list.append(connection)
+        print([connection.status for connection in self.connections_list])
 
     async def receive_and_execute(self, connection: ServerConnection):
         """
         receive and process commands
         """
         self.logger.info(f"{connection.name} is now running")
         while self.running:
@@ -198,28 +193,28 @@
                 self.end_time = time.time() + self.SESSION_TIME 
                 await connection.send(response)
                 self.logger.info(message.schema_type)
             except exceptions.ClientSideError as e:
                 self.logger.warning(e)
                 continue
             except (exceptions.TimeoutError, exceptions.Shutdown) as e:
-                error_response = schemas.ResponseData(error=str(e), exit_status=1, url=self.url, active_username=self.username)
-                await connection.send(error_response)
+                #error_response = schemas.ResponseData(error=str(e), url=self.url, active_username=self.username, exit_status=1)
+                #await connection.send(error_response)
                 self.logger.warning(str(e))
                 self.running = False
-                return 'shutdown initiated, closing'
+                return
             except exceptions.Exit as e:
                 self.logger.info("user exit initiated")
-                error_response = schemas.ResponseData(error=str(e), exit_status=1, url=self.url, active_username=self.username)
-                await connection.send(error_response)
-                await connection.close()
+                # error_response = schemas.ResponseData(error=str(e), exit_status=1, url=self.url, active_username=self.username)
+                # await connection.send(error_response)
+                connection.set_status_exiting()
                 return
             except OSError:
                 self.logger.info("connection was lost, waiting to reconnect")
-                await connection.close()
+                await connection.close(self.connection_list_lock)
             except asyncio.CancelledError:
                 return 'task was cancelled'
             except (exceptions.CommandNotFoundError, exceptions.NoConfirmationError, exceptions.InvalidCredentialsReceived, Exception) as e:
                 error_str = traceback.format_exc()
                 error_response = schemas.ResponseData(error=str(e), url=self.url, active_username=self.username)
                 await connection.send(error_response)
                 self.logger.warning(f"{error_str}")
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/socketopts/schemas.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/socketopts/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     
 
 class FormRequest(BaseSchema):
     """
     Request seperate input for some command parameters. If the arguments_list is empty, this will be interpreted as an expression request for something like neo4j
     """
     schema_type: str = 'FormRequest'
+    existing_data: dict | object = dict()
 
 
 class FormResponse(BaseSchema):
     """
     respond to a form request with proper data
     """
     schema_type: str = 'FormResponse'
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/socketopts/socketOpts.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/socketopts/socketOpts.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,16 @@
         self.initialize_logger(f"{name} LOGGER")
         self.debug_state = debug
 
     def debug(self, operation: typing.Literal["SENDING", "RECEIVED", "WAITING"], message: str | typing.Type[schemas.BaseSchema]):
         if self.debug_state:
             if not isinstance(message, str):
                 self.logger.info(f"""{operation}: {message.schema_type}
-                                    MESSAGE CONTENT:{pformat(message.request_content)}
                                     MESSAGE: {pformat(message.message)}
-                                    ERROR: {pformat(message.error)}""")
+                                    ERROR: {pformat(message.error)}""") # MESSAGE CONTENT:{pformat(message.request_content)}
             else:
                 self.logger.info(message)
 
 
 class ClientSocketOpts(BaseSocketOpts):
     """
     synchronous sockets to be used by clients
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/killableThread.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import sys
+import typing
 
 
 class ServerLogger:
     def initialize_logger(self, name):
         self.logger = logging.getLogger(name)
         self.logger.setLevel(logging.INFO)
         stream_handler = logging.StreamHandler(stream=sys.stdout)
@@ -39,18 +40,28 @@
             '%(name)s - %(levelname)s - %(message)s')
         stream_handler.setFormatter(stream_format)
         self.logger.addHandler(stream_handler)
         self.logger.disabled = False
 
 
 class ServiceLogger:
+    levels_map = {
+        'info':logging.INFO,
+        'warning':logging.WARNING,
+        'error':logging.ERROR
+    }
     def __init__(self, name, log_path):
         self.logger = logging.getLogger(name)
         self.logger.setLevel(logging.INFO)
-        file_handler = file_handler = logging.FileHandler(
+        self.file_handler = logging.FileHandler(
             log_path, mode='a')
-        file_handler.setLevel(logging.INFO)
+        self.file_handler.setLevel(logging.INFO)
         file_format = logging.Formatter(
             '%(name)s - %(levelname)s - %(message)s')
-        file_handler.setFormatter(file_format)
-        self.logger.addHandler(file_handler)
-        self.logger.disabled = False
+        self.file_handler.setFormatter(file_format)
+        self.logger.addHandler(self.file_handler)
+        self.logger.disabled = False
+
+    def log(self, data, level: typing.Literal['info', 'warning', 'error'], filename: str):
+        self.file_handler.baseFilename = filename
+        level = self.levels_map[level]
+        self.logger.log(level, data)
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.2.1
+Version: 0.2.2
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.2.1/src/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 src/TapisCLICICLE/commands/arguments/argument.py
 src/TapisCLICICLE/commands/query/__init__.py
 src/TapisCLICICLE/commands/query/neo4j.py
 src/TapisCLICICLE/commands/query/postgres.py
 src/TapisCLICICLE/server/__init__.py
 src/TapisCLICICLE/server/auth.py
 src/TapisCLICICLE/server/server.py
-src/TapisCLICICLE/server/userFileManager.py
 src/TapisCLICICLE/socketopts/__init__.py
 src/TapisCLICICLE/socketopts/schemas.py
 src/TapisCLICICLE/socketopts/socketOpts.py
 src/TapisCLICICLE/utilities/__init__.py
 src/TapisCLICICLE/utilities/exceptions.py
 src/TapisCLICICLE/utilities/killableThread.py
 src/TapisCLICICLE/utilities/logger.py
 src/TapisCL_ICICLE.egg-info/PKG-INFO
 src/TapisCL_ICICLE.egg-info/SOURCES.txt
 src/TapisCL_ICICLE.egg-info/dependency_links.txt
 src/TapisCL_ICICLE.egg-info/entry_points.txt
 src/TapisCL_ICICLE.egg-info/requires.txt
-src/TapisCL_ICICLE.egg-info/top_level.txt
+src/TapisCL_ICICLE.egg-info/top_level.txt
+tests/test.py
```


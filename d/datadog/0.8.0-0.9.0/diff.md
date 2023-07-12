# Comparing `tmp/datadog-0.8.0.tar.gz` & `tmp/datadog-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datadog-0.8.0.tar", last modified: Thu Jul 30 14:00:08 2015, max compression
+gzip compressed data, was "dist/datadog-0.9.0.tar", last modified: Mon Aug 31 17:10:24 2015, max compression
```

## Comparing `datadog-0.8.0.tar` & `datadog-0.9.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-07-30 14:00:08.000000 datadog-0.8.0/
-drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-07-30 14:00:08.000000 datadog-0.8.0/datadog/
--rw-r--r--   0 yannmahe   (501) staff       (20)     2747 2015-07-27 20:25:45.000000 datadog-0.8.0/datadog/__init__.py
-drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-07-30 14:00:08.000000 datadog-0.8.0/datadog/api/
--rw-r--r--   0 yannmahe   (501) staff       (20)      824 2015-07-30 13:56:20.000000 datadog-0.8.0/datadog/api/__init__.py
--rw-r--r--   0 yannmahe   (501) staff       (20)    14964 2015-07-27 20:25:45.000000 datadog-0.8.0/datadog/api/base.py
--rw-r--r--   0 yannmahe   (501) staff       (20)      324 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/api/comments.py
--rw-r--r--   0 yannmahe   (501) staff       (20)      130 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/api/constants.py
--rw-r--r--   0 yannmahe   (501) staff       (20)      377 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/api/downtimes.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     2664 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/api/events.py
--rw-r--r--   0 yannmahe   (501) staff       (20)      657 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/api/exceptions.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     2408 2015-07-30 13:56:20.000000 datadog-0.8.0/datadog/api/graphs.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     1107 2015-06-16 21:14:00.000000 datadog-0.8.0/datadog/api/hosts.py
--rw-r--r--   0 yannmahe   (501) staff       (20)      537 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/api/infrastructure.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     3700 2015-07-01 14:04:01.000000 datadog-0.8.0/datadog/api/metrics.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     3091 2015-07-01 14:04:01.000000 datadog-0.8.0/datadog/api/monitors.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     1152 2015-07-01 14:04:01.000000 datadog-0.8.0/datadog/api/screenboards.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     1290 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/api/service_checks.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     1383 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/api/tags.py
--rw-r--r--   0 yannmahe   (501) staff       (20)      466 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/api/timeboards.py
--rw-r--r--   0 yannmahe   (501) staff       (20)      799 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/api/users.py
-drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-07-30 14:00:08.000000 datadog-0.8.0/datadog/dogshell/
--rw-r--r--   0 yannmahe   (501) staff       (20)     3098 2015-05-19 13:52:03.000000 datadog-0.8.0/datadog/dogshell/__init__.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     7192 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/dogshell/comment.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     3601 2015-04-23 21:21:27.000000 datadog-0.8.0/datadog/dogshell/common.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     4618 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/dogshell/downtime.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     6792 2015-04-23 21:21:27.000000 datadog-0.8.0/datadog/dogshell/event.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     2054 2015-06-16 21:14:00.000000 datadog-0.8.0/datadog/dogshell/host.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     1913 2015-06-30 15:18:44.000000 datadog-0.8.0/datadog/dogshell/metric.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     8490 2015-07-01 14:04:01.000000 datadog-0.8.0/datadog/dogshell/monitor.py
--rw-r--r--   0 yannmahe   (501) staff       (20)    12141 2015-07-01 14:04:01.000000 datadog-0.8.0/datadog/dogshell/screenboard.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     1386 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/dogshell/search.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     1671 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/dogshell/service_check.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     4134 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/dogshell/tag.py
--rw-r--r--   0 yannmahe   (501) staff       (20)    13603 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/dogshell/timeboard.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     9946 2015-04-24 18:03:42.000000 datadog-0.8.0/datadog/dogshell/wrap.py
-drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-07-30 14:00:08.000000 datadog-0.8.0/datadog/dogstatsd/
--rw-r--r--   0 yannmahe   (501) staff       (20)       50 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/dogstatsd/__init__.py
--rw-r--r--   0 yannmahe   (501) staff       (20)    10495 2015-07-27 20:25:45.000000 datadog-0.8.0/datadog/dogstatsd/base.py
-drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-07-30 14:00:08.000000 datadog-0.8.0/datadog/threadstats/
--rw-r--r--   0 yannmahe   (501) staff       (20)       57 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/threadstats/__init__.py
--rw-r--r--   0 yannmahe   (501) staff       (20)    14015 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/threadstats/base.py
--rw-r--r--   0 yannmahe   (501) staff       (20)      282 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/threadstats/constants.py
--rw-r--r--   0 yannmahe   (501) staff       (20)      479 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/threadstats/events.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     4410 2015-04-17 15:12:50.000000 datadog-0.8.0/datadog/threadstats/metrics.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     1325 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/threadstats/periodic_timer.py
--rw-r--r--   0 yannmahe   (501) staff       (20)      433 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/threadstats/reporters.py
-drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-07-30 14:00:08.000000 datadog-0.8.0/datadog/util/
--rw-r--r--   0 yannmahe   (501) staff       (20)        0 2015-03-11 15:50:47.000000 datadog-0.8.0/datadog/util/__init__.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     1131 2015-04-03 14:41:52.000000 datadog-0.8.0/datadog/util/compat.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     3316 2015-06-22 22:19:57.000000 datadog-0.8.0/datadog/util/config.py
--rw-r--r--   0 yannmahe   (501) staff       (20)     9602 2015-05-27 15:52:58.000000 datadog-0.8.0/datadog/util/hostname.py
-drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-07-30 14:00:08.000000 datadog-0.8.0/datadog.egg-info/
--rw-r--r--   0 yannmahe   (501) staff       (20)        1 2015-07-30 14:00:08.000000 datadog-0.8.0/datadog.egg-info/dependency_links.txt
--rw-r--r--   0 yannmahe   (501) staff       (20)       84 2015-07-30 14:00:08.000000 datadog-0.8.0/datadog.egg-info/entry_points.txt
--rw-rw-r--   0 yannmahe   (501) staff       (20)       47 2015-05-22 19:28:30.000000 datadog-0.8.0/datadog.egg-info/pbr.json
--rw-r--r--   0 yannmahe   (501) staff       (20)      619 2015-07-30 14:00:08.000000 datadog-0.8.0/datadog.egg-info/PKG-INFO
--rw-r--r--   0 yannmahe   (501) staff       (20)       51 2015-07-30 14:00:08.000000 datadog-0.8.0/datadog.egg-info/requires.txt
--rw-r--r--   0 yannmahe   (501) staff       (20)     1421 2015-07-30 14:00:08.000000 datadog-0.8.0/datadog.egg-info/SOURCES.txt
--rw-r--r--   0 yannmahe   (501) staff       (20)        8 2015-07-30 14:00:08.000000 datadog-0.8.0/datadog.egg-info/top_level.txt
--rw-r--r--   0 yannmahe   (501) staff       (20)      619 2015-07-30 14:00:08.000000 datadog-0.8.0/PKG-INFO
--rw-r--r--   0 yannmahe   (501) staff       (20)       59 2015-07-30 14:00:08.000000 datadog-0.8.0/setup.cfg
--rw-r--r--   0 yannmahe   (501) staff       (20)     1416 2015-07-30 13:56:20.000000 datadog-0.8.0/setup.py
+drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-08-31 17:10:24.000000 datadog-0.9.0/
+drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-08-31 17:10:24.000000 datadog-0.9.0/datadog/
+-rw-r--r--   0 yannmahe   (501) staff       (20)     3031 2015-08-31 17:00:06.000000 datadog-0.9.0/datadog/__init__.py
+drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-08-31 17:10:24.000000 datadog-0.9.0/datadog/api/
+-rw-r--r--   0 yannmahe   (501) staff       (20)      821 2015-08-25 19:44:23.000000 datadog-0.9.0/datadog/api/__init__.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)    15064 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/api/base.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)      324 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/api/comments.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)      130 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/api/constants.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)      377 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/api/downtimes.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     2664 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/api/events.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)      657 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/api/exceptions.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     2408 2015-08-25 19:44:23.000000 datadog-0.9.0/datadog/api/graphs.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     1107 2015-06-16 21:14:00.000000 datadog-0.9.0/datadog/api/hosts.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)      537 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/api/infrastructure.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     3700 2015-07-01 14:04:01.000000 datadog-0.9.0/datadog/api/metrics.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     3091 2015-07-01 14:04:01.000000 datadog-0.9.0/datadog/api/monitors.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     1152 2015-07-01 14:04:01.000000 datadog-0.9.0/datadog/api/screenboards.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     1290 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/api/service_checks.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     1383 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/api/tags.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)      466 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/api/timeboards.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)      799 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/api/users.py
+drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-08-31 17:10:24.000000 datadog-0.9.0/datadog/dogshell/
+-rw-r--r--   0 yannmahe   (501) staff       (20)     3122 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/__init__.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     7206 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/comment.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     3620 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/common.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     4622 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/downtime.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     6806 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/event.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     2059 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/host.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     1923 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/metric.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     8495 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/monitor.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)    12155 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/screenboard.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     1391 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/search.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     1676 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/service_check.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     4139 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/tag.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)    13617 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/timeboard.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     9964 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/dogshell/wrap.py
+drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-08-31 17:10:24.000000 datadog-0.9.0/datadog/dogstatsd/
+-rw-r--r--   0 yannmahe   (501) staff       (20)       50 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/dogstatsd/__init__.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)    11028 2015-08-25 19:44:23.000000 datadog-0.9.0/datadog/dogstatsd/base.py
+drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-08-31 17:10:24.000000 datadog-0.9.0/datadog/threadstats/
+-rw-r--r--   0 yannmahe   (501) staff       (20)       57 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/threadstats/__init__.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)    14015 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/threadstats/base.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)      282 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/threadstats/constants.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)      479 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/threadstats/events.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     4410 2015-04-17 15:12:50.000000 datadog-0.9.0/datadog/threadstats/metrics.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     1325 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/threadstats/periodic_timer.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)      433 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/threadstats/reporters.py
+drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-08-31 17:10:24.000000 datadog-0.9.0/datadog/util/
+-rw-r--r--   0 yannmahe   (501) staff       (20)        0 2015-03-11 15:50:47.000000 datadog-0.9.0/datadog/util/__init__.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     1008 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/util/compat.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     3316 2015-06-22 22:19:57.000000 datadog-0.9.0/datadog/util/config.py
+-rw-r--r--   0 yannmahe   (501) staff       (20)     9647 2015-08-31 17:04:19.000000 datadog-0.9.0/datadog/util/hostname.py
+drwxr-xr-x   0 yannmahe   (501) staff       (20)        0 2015-08-31 17:10:24.000000 datadog-0.9.0/datadog.egg-info/
+-rw-r--r--   0 yannmahe   (501) staff       (20)        1 2015-08-31 17:10:24.000000 datadog-0.9.0/datadog.egg-info/dependency_links.txt
+-rw-r--r--   0 yannmahe   (501) staff       (20)       84 2015-08-31 17:10:24.000000 datadog-0.9.0/datadog.egg-info/entry_points.txt
+-rw-rw-r--   0 yannmahe   (501) staff       (20)       47 2015-08-25 19:57:58.000000 datadog-0.9.0/datadog.egg-info/pbr.json
+-rw-r--r--   0 yannmahe   (501) staff       (20)      619 2015-08-31 17:10:24.000000 datadog-0.9.0/datadog.egg-info/PKG-INFO
+-rw-r--r--   0 yannmahe   (501) staff       (20)       51 2015-08-31 17:10:24.000000 datadog-0.9.0/datadog.egg-info/requires.txt
+-rw-r--r--   0 yannmahe   (501) staff       (20)     1421 2015-08-31 17:10:24.000000 datadog-0.9.0/datadog.egg-info/SOURCES.txt
+-rw-r--r--   0 yannmahe   (501) staff       (20)        8 2015-08-31 17:10:24.000000 datadog-0.9.0/datadog.egg-info/top_level.txt
+-rw-r--r--   0 yannmahe   (501) staff       (20)      619 2015-08-31 17:10:24.000000 datadog-0.9.0/PKG-INFO
+-rw-r--r--   0 yannmahe   (501) staff       (20)       59 2015-08-31 17:10:24.000000 datadog-0.9.0/setup.cfg
+-rw-r--r--   0 yannmahe   (501) staff       (20)     1425 2015-08-31 17:04:19.000000 datadog-0.9.0/setup.py
```

### Comparing `datadog-0.8.0/datadog/__init__.py` & `datadog-0.9.0/datadog/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 It contains:
 * datadog.api: a Python client for Datadog REST API.
 * datadog.dogstatsd: a DogStatsd Python client.
 * datadog.threadstats: an alternative tool to DogStatsd client for collecting application metrics
 without hindering performance.
 * datadog.dogshell: a command-line tool, wrapping datadog.api, to interact with Datadog REST API.
 """
+# stdlib
 from pkg_resources import get_distribution, DistributionNotFound
 import os
 import os.path
 
+# datadog
 from datadog import api
 from datadog.dogstatsd import statsd
 from datadog.threadstats import ThreadStats  # noqa
 from datadog.util.hostname import get_hostname
+from datadog.util.compat import iteritems
 
 
 try:
     _dist = get_distribution("datadog")
     # Normalize case for Windows systems
     dist_loc = os.path.normcase(_dist.location)
     here = os.path.normcase(__file__)
@@ -28,15 +31,15 @@
 except DistributionNotFound:
     __version__ = 'Please install datadog with setup.py'
 else:
     __version__ = _dist.version
 
 
 def initialize(api_key=None, app_key=None, host_name=None, api_host=None,
-               proxies=None, statsd_host=None, statsd_port=None, cacert=True):
+               statsd_host=None, statsd_port=None, **kwargs):
     """
     Initialize and configure Datadog.api and Datadog.statsd modules
 
     :param api_key: Datadog API key
     :type api_key: string
 
     :param app_key: Datadog application key
@@ -50,25 +53,31 @@
 
     :param statsd_host: Host of DogStatsd server or statsd daemon
     :type statsd_host: address
 
     :param statsd_port: Port of DogStatsd server or statsd daemon
     :type statsd_port: port
 
-    :param cacert: Path to local certificate file used to verify SSL
-    certificates. Can also be set to True (default) to use the systems
-    certificate store, or False to skip SSL verification
+    :param cacert: Path to local certificate file used to verify SSL \
+        certificates. Can also be set to True (default) to use the systems \
+        certificate store, or False to skip SSL verification
     :type cacert: path or boolean
+
+    :param mute: Mute any exceptions before they escape from the library (default: True).
+    :type mute: boolean
     """
-    # Configure api
+    # API configuration
     api._api_key = api_key if api_key is not None else os.environ.get('DATADOG_API_KEY')
     api._application_key = app_key if app_key is not None else os.environ.get('DATADOG_APP_KEY')
     api._host_name = host_name if host_name is not None else get_hostname()
     api._api_host = api_host if api_host is not None else \
         os.environ.get('DATADOG_HOST', 'https://app.datadoghq.com')
-    api._proxies = proxies
-    api._cacert = cacert
 
-    # Given statsd_host and statsd_port, overrides statsd instance
+    # Statsd configuration -overrides default statsd instance attributes-
     if statsd_host and statsd_port:
         statsd.host = statsd_host
         statsd.port = int(statsd_port)
+
+    # HTTP client and API options
+    for key, value in iteritems(kwargs):
+        attribute = "_{0}".format(key)
+        setattr(api, attribute, value)
```

### Comparing `datadog-0.8.0/datadog/api/__init__.py` & `datadog-0.9.0/datadog/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # HTTP(S) settings
 _proxies = None
 _timeout = 3
 _max_timeouts = 3
 _max_retries = 3
 _backoff_period = 300
-_swallow = True
+_mute = True
 
 # Resources
 from datadog.api.comments import Comment
 from datadog.api.downtimes import Downtime
 from datadog.api.timeboards import Timeboard
 from datadog.api.events import Event
 from datadog.api.infrastructure import Infrastructure
```

### Comparing `datadog-0.8.0/datadog/api/base.py` & `datadog-0.9.0/datadog/api/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # stdlib
 import time
 import logging
 import requests
 
+# 3p
+import simplejson as json
+
 # datadog
 from datadog.api.exceptions import ClientError, ApiError, HttpBackoff, \
     HttpTimeout, ApiNotInitialized
 from datadog.api import _api_version, _max_timeouts, _backoff_period
-from datadog.util.compat import json, is_p3k
+from datadog.util.compat import is_p3k
 
 log = logging.getLogger('dd.datadogpy')
 
 
 class HTTPClient(object):
     """
     HTTP client based on Requests library for Datadog API calls
@@ -57,15 +60,15 @@
             # Check if it's ok to submit
             if not cls._should_submit():
                 raise HttpBackoff("Too many timeouts. Won't try again for {1} seconds."
                                   .format(*cls._backoff_status()))
 
             # Import API, User and HTTP settings
             from datadog.api import _api_key, _application_key, _api_host, \
-                _swallow, _host_name, _proxies, _max_retries, _timeout, \
+                _mute, _host_name, _proxies, _max_retries, _timeout, \
                 _cacert
 
             # Check keys and add then to params
             if _api_key is None:
                 raise ApiNotInitialized("API key is not set."
                                         " Please run 'initialize' method first.")
             params['api_key'] = _api_key
@@ -120,14 +123,15 @@
             except requests.ConnectionError as e:
                 raise ClientError("Could not request %s %s%s: %s" % (method, _api_host, url, e))
             except requests.exceptions.Timeout as e:
                 cls._timeout_counter += 1
                 raise HttpTimeout('%s %s timed out after %d seconds.' % (method, url, _timeout))
             except requests.exceptions.HTTPError as e:
                 if e.response.status_code in (400, 403, 404):
+                    # This gets caught afterwards and raises an ApiError exception
                     pass
                 else:
                     raise
             except TypeError as e:
                 raise TypeError(
                     "Your installed version of 'requests' library seems not compatible with"
                     "Datadog's usage. We recommand upgrading it ('pip install -U requests')."
@@ -156,24 +160,24 @@
                 response_obj = None
             if response_formatter is None:
                 return response_obj
             else:
                 return response_formatter(response_obj)
 
         except ClientError as e:
-            if _swallow:
+            if _mute:
                 log.error(str(e))
                 if error_formatter is None:
                     return {'errors': e.args[0]}
                 else:
                     return error_formatter({'errors': e.args[0]})
             else:
                 raise
         except ApiError as e:
-            if _swallow:
+            if _mute:
                 for error in e.args[0]['errors']:
                     log.error(str(error))
                 if error_formatter is None:
                     return e.args[0]
                 else:
                     return error_formatter(e.args[0])
             else:
```

### Comparing `datadog-0.8.0/datadog/api/events.py` & `datadog-0.9.0/datadog/api/events.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/api/exceptions.py` & `datadog-0.9.0/datadog/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/api/graphs.py` & `datadog-0.9.0/datadog/api/graphs.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/api/hosts.py` & `datadog-0.9.0/datadog/api/hosts.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/api/infrastructure.py` & `datadog-0.9.0/datadog/api/infrastructure.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/api/metrics.py` & `datadog-0.9.0/datadog/api/metrics.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/api/monitors.py` & `datadog-0.9.0/datadog/api/monitors.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/api/screenboards.py` & `datadog-0.9.0/datadog/api/screenboards.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/api/service_checks.py` & `datadog-0.9.0/datadog/api/service_checks.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/api/tags.py` & `datadog-0.9.0/datadog/api/tags.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/api/users.py` & `datadog-0.9.0/datadog/api/users.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/dogshell/__init__.py` & `datadog-0.9.0/datadog/dogshell/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-import argparse
+# stdlib
+import logging
 import os
 import pkg_resources as pkg
 
-import logging
+# 3p
+import argparse
 
-from datadog.dogshell.common import DogshellConfig
+# datadog
+from datadog import initialize
 from datadog.dogshell.comment import CommentClient
-from datadog.dogshell.search import SearchClient
-from datadog.dogshell.metric import MetricClient
-from datadog.dogshell.tag import TagClient
+from datadog.dogshell.common import DogshellConfig
+from datadog.dogshell.downtime import DowntimeClient
 from datadog.dogshell.event import EventClient
+from datadog.dogshell.host import HostClient
+from datadog.dogshell.metric import MetricClient
 from datadog.dogshell.monitor import MonitorClient
-from datadog.dogshell.downtime import DowntimeClient
 from datadog.dogshell.screenboard import ScreenboardClient
-from datadog.dogshell.timeboard import TimeboardClient
-from datadog.dogshell.host import HostClient
+from datadog.dogshell.search import SearchClient
 from datadog.dogshell.service_check import ServiceCheckClient
-from datadog import initialize
+from datadog.dogshell.tag import TagClient
+from datadog.dogshell.timeboard import TimeboardClient
 
 logging.getLogger('dd.datadogpy').setLevel(logging.CRITICAL)
 
 
 def main():
 
     parser = argparse.ArgumentParser(description="Interact with the Datadog API",
```

### Comparing `datadog-0.8.0/datadog/dogshell/comment.py` & `datadog-0.9.0/datadog/dogshell/comment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+# stdlib
 import sys
 
+# 3p
+import simplejson as json
+
+# datadog
 from datadog.dogshell.common import report_errors, report_warnings
 from datadog import api
-from datadog.util.compat import json
 
 
 class CommentClient(object):
 
     @classmethod
     def setup_parser(cls, subparsers):
         parser = subparsers.add_parser('comment', help="Post, update, and delete comments.")
```

### Comparing `datadog-0.8.0/datadog/dogshell/common.py` & `datadog-0.9.0/datadog/dogshell/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+# stdlib
 from __future__ import print_function
 import os
 import sys
 import logging
 import socket
 
+# datadog
 from datadog.util.compat import is_p3k, configparser, IterableUserDict,\
     get_input
 
 log = logging.getLogger('dd.datadogpy')
 
 
 def print_err(msg):
```

### Comparing `datadog-0.8.0/datadog/dogshell/downtime.py` & `datadog-0.9.0/datadog/dogshell/downtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from datadog.util.compat import json
-from datadog.dogshell.common import report_errors, report_warnings
+# 3p
+import simplejson as json
 
+# datadog
 from datadog import api
+from datadog.dogshell.common import report_errors, report_warnings
 
 
 class DowntimeClient(object):
     @classmethod
     def setup_parser(cls, subparsers):
         parser = subparsers.add_parser('downtime', help="Create, edit, and delete downtimes")
         parser.add_argument('--string_ids', action='store_true', dest='string_ids',
```

### Comparing `datadog-0.8.0/datadog/dogshell/event.py` & `datadog-0.9.0/datadog/dogshell/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+# stdlib
 import datetime
 import time
 import re
 import sys
 
-from datadog.util.compat import json
-from datadog.dogshell.common import report_errors, report_warnings
+# 3p
+import simplejson as json
+
+# datadog
 from datadog import api
+from datadog.dogshell.common import report_errors, report_warnings
 
 
 def prettyprint_event(event):
     title = event['title'] or ''
     text = event.get('text', '') or ''
     handle = event.get('handle', '') or ''
     date = event['date_happened']
```

### Comparing `datadog-0.8.0/datadog/dogshell/host.py` & `datadog-0.9.0/datadog/dogshell/host.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from datadog.dogshell.common import report_errors, report_warnings
-from datadog.util.compat import json
+# 3p
+import simplejson as json
+
+# datadog
 from datadog import api
+from datadog.dogshell.common import report_errors, report_warnings
 
 
 class HostClient(object):
     @classmethod
     def setup_parser(cls, subparsers):
         parser = subparsers.add_parser('host', help='Mute, unmute hosts')
         verb_parsers = parser.add_subparsers(title='Verbs')
```

### Comparing `datadog-0.8.0/datadog/dogshell/metric.py` & `datadog-0.9.0/datadog/dogshell/metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from datadog.dogshell.common import report_errors, report_warnings, find_localhost
+# datadog
 from datadog import api
+from datadog.dogshell.common import report_errors, report_warnings, find_localhost
 
 
 class MetricClient(object):
 
     @classmethod
     def setup_parser(cls, subparsers):
         parser = subparsers.add_parser('metric', help="Post metrics.")
```

### Comparing `datadog-0.8.0/datadog/dogshell/monitor.py` & `datadog-0.9.0/datadog/dogshell/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from datadog.util.compat import json
-from datadog.dogshell.common import report_errors, report_warnings
+# 3p
+import simplejson as json
+
+# datadog
 from datadog import api
+from datadog.dogshell.common import report_errors, report_warnings
 
 
 class MonitorClient(object):
     @classmethod
     def setup_parser(cls, subparsers):
         parser = subparsers.add_parser('monitor', help="Create, edit, and delete monitors")
         parser.add_argument('--string_ids', action='store_true', dest='string_ids',
```

### Comparing `datadog-0.8.0/datadog/dogshell/screenboard.py` & `datadog-0.9.0/datadog/dogshell/screenboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+# stdlib
 import argparse
 import sys
 import platform
 import webbrowser
 
-from datetime import datetime
-from datadog.util.compat import json
-from datadog.dogshell.common import report_errors, report_warnings, print_err
+# 3p
+import simplejson as json
+
+# datadog
 from datadog import api
+from datadog.dogshell.common import report_errors, report_warnings, print_err
+from datetime import datetime
 
 
 class ScreenboardClient(object):
 
     @classmethod
     def setup_parser(cls, subparsers):
         parser = subparsers.add_parser('screenboard', help="Create, edit, and delete screenboards.")
```

### Comparing `datadog-0.8.0/datadog/dogshell/search.py` & `datadog-0.9.0/datadog/dogshell/search.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from datadog.util.compat import json
-from datadog.dogshell.common import report_errors, report_warnings
+# 3p
+import simplejson as json
+
+# datadog
 from datadog import api
+from datadog.dogshell.common import report_errors, report_warnings
 
 
 # TODO IS there a test ?
 class SearchClient(object):
 
     @classmethod
     def setup_parser(cls, subparsers):
```

### Comparing `datadog-0.8.0/datadog/dogshell/service_check.py` & `datadog-0.9.0/datadog/dogshell/service_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from datadog.util.compat import json
-from datadog.dogshell.common import report_errors, report_warnings
+# 3p
+import simplejson as json
+
+# datadog
 from datadog import api
+from datadog.dogshell.common import report_errors, report_warnings
 
 
 class ServiceCheckClient(object):
     @classmethod
     def setup_parser(cls, subparsers):
         parser = subparsers.add_parser('service_check', help="Perform service checks")
         verb_parsers = parser.add_subparsers(title='Verbs')
```

### Comparing `datadog-0.8.0/datadog/dogshell/tag.py` & `datadog-0.9.0/datadog/dogshell/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from datadog.util.compat import json
-from datadog.dogshell.common import report_errors, report_warnings
+# 3p
+import simplejson as json
+
+# datadog
 from datadog import api
+from datadog.dogshell.common import report_errors, report_warnings
 
 
 class TagClient(object):
 
     @classmethod
     def setup_parser(cls, subparsers):
         parser = subparsers.add_parser('tag', help="View and modify host tags.")
```

### Comparing `datadog-0.8.0/datadog/dogshell/timeboard.py` & `datadog-0.9.0/datadog/dogshell/timeboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-import argparse
+# stdlib
 import os.path
 import platform
 import sys
 import webbrowser
 
-from datetime import datetime
-from datadog.util.compat import json
-from datadog.dogshell.common import report_errors, report_warnings, print_err
+# 3p
+import argparse
+import simplejson as json
+
+# datadog
 from datadog import api
+from datadog.dogshell.common import report_errors, report_warnings, print_err
+from datetime import datetime
 
 
 class TimeboardClient(object):
 
     @classmethod
     def setup_parser(cls, subparsers):
         parser = subparsers.add_parser('timeboard', help="Create, edit, and delete timeboards")
```

### Comparing `datadog-0.8.0/datadog/dogshell/wrap.py` & `datadog-0.9.0/datadog/dogshell/wrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 dogwrap -n test-job -k $API_KEY --submit_mode errors "ls -lah"
 
 And you can give the command a timeout too:
 
 dogwrap -n test-job -k $API_KEY --timeout=1 "sleep 3"
 
 '''
-
-import sys
-import time
+# stdlib
 import optparse
-import threading
-import subprocess
 import pkg_resources as pkg
+import subprocess
+import sys
+import threading
+import time
 
+# datadog
 from datadog import initialize, api
 
 
 SUCCESS = 'success'
 ERROR = 'error'
```

### Comparing `datadog-0.8.0/datadog/dogstatsd/base.py` & `datadog-0.9.0/datadog/dogstatsd/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,33 +17,45 @@
 
 log = logging.getLogger('dogstatsd')
 
 
 class DogStatsd(object):
     OK, WARNING, CRITICAL, UNKNOWN = (0, 1, 2, 3)
 
-    def __init__(self, host='localhost', port=8125, max_buffer_size=50, constant_tags=None):
+    def __init__(self, host='localhost', port=8125, max_buffer_size=50,
+                 constant_tags=None, use_ms=False):
         """
         Initialize a DogStatsd object.
 
         >>> statsd = DogStatsd()
 
         :param host: the host of the DogStatsd server.
+        :type host: string
+
         :param port: the port of the DogStatsd server.
-        :param max_buffer_size: Maximum number of metric to buffer before sending to the server
-            if sending metrics in batch
-        :param constant_tags: A list of strings to attach to every metric reported by this client
+        :type port: integer
+
+        :param max_buffer_size: Maximum number of metrics to buffer before sending to the server
+        if sending metrics in batch
+        :type max_buffer_size: integer
+
+        :param constant_tags: Tags to attach to every metric reported by this client
+        :type constant_tags: list of strings
+
+        :param use_ms: Report timed values in milliseconds instead of seconds (default False)
+        :type use_ms: boolean
         """
         self.host = host
         self.port = int(port)
         self.socket = None
         self.max_buffer_size = max_buffer_size
         self._send = self._send_to_server
         self.encoding = 'utf-8'
         self.constant_tags = constant_tags
+        self.use_ms = use_ms
 
     def __enter__(self):
         self.open_buffer(self.max_buffer_size)
         return self
 
     def __exit__(self, type, value, traceback):
         self.close_buffer()
@@ -131,19 +143,20 @@
 
     class _TimedContextManagerDecorator(object):
         """
         A context manager and a decorator which will report the elapsed time in
         the context OR in a function call.
         """
 
-        def __init__(self, statsd, metric=None, tags=None, sample_rate=1):
+        def __init__(self, statsd, metric=None, tags=None, sample_rate=1, use_ms=None):
             self.statsd = statsd
             self.metric = metric
             self.tags = tags
             self.sample_rate = sample_rate
+            self.use_ms = use_ms
 
         def __call__(self, func):
             """Decorator which returns the elapsed time of the function call."""
             # Default to the function name if metric was not provided.
             if not self.metric:
                 self.metric = '%s.%s' % (func.__module__, func.__name__)
 
@@ -156,18 +169,20 @@
         def __enter__(self):
             if not self.metric:
                 raise TypeError("Cannot used timed without a metric!")
             self.start = time()
 
         def __exit__(self, type, value, traceback):
             # Report the elapsed time of the context manager.
-            self.statsd.timing(self.metric, time() - self.start,
-                               self.tags, self.sample_rate)
+            elapsed = time() - self.start
+            use_ms = self.use_ms if self.use_ms is not None else self.statsd.use_ms
+            elapsed = int(round(1000 * elapsed)) if use_ms else elapsed
+            self.statsd.timing(self.metric, elapsed, self.tags, self.sample_rate)
 
-    def timed(self, metric=None, tags=None, sample_rate=1):
+    def timed(self, metric=None, tags=None, sample_rate=1, use_ms=None):
         """
         A decorator or context manager that will measure the distribution of a
         function's/context's run time. Optionally specify a list of tags or a
         sample rate. If the metric is not defined as a decorator, the module
         name and function name will be used. The metric is required as a context
         manager.
         ::
@@ -185,15 +200,15 @@
             # Is equivalent to ...
             start = time.time()
             try:
                 get_user(user_id)
             finally:
                 statsd.timing('user.query.time', time.time() - start)
         """
-        return self._TimedContextManagerDecorator(self, metric, tags, sample_rate)
+        return self._TimedContextManagerDecorator(self, metric, tags, sample_rate, use_ms)
 
     def set(self, metric, value, tags=None, sample_rate=1):
         """
         Sample a set value.
 
         >>> statsd.set('visitors.uniques', 999)
         """
```

### Comparing `datadog-0.8.0/datadog/threadstats/base.py` & `datadog-0.9.0/datadog/threadstats/base.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/threadstats/metrics.py` & `datadog-0.9.0/datadog/threadstats/metrics.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/threadstats/periodic_timer.py` & `datadog-0.9.0/datadog/threadstats/periodic_timer.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/util/compat.py` & `datadog-0.9.0/datadog/util/compat.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,13 +47,7 @@
 except ImportError:
     from ConfigParser import ConfigParser
 
 try:
     from urllib.parse import urlparse
 except ImportError:
     from urlparse import urlparse
-
-# prefer simplejson but fall back to stdlib python
-try:
-    import simplejson as json
-except ImportError:
-    import json
```

### Comparing `datadog-0.8.0/datadog/util/config.py` & `datadog-0.9.0/datadog/util/config.py`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/datadog/util/hostname.py` & `datadog-0.9.0/datadog/util/hostname.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+# stdlib
 import socket
 import re
 import logging
 import subprocess
 import types
 
-from datadog.util.compat import url_lib, is_p3k, iteritems, json
+# 3p
+import simplejson as json
+
+# datadog
+from datadog.util.compat import url_lib, is_p3k, iteritems
 from datadog.util.config import get_config, get_os, CfgNotFound
 
 VALID_HOSTNAME_RFC_1123_PATTERN = re.compile(r"^(([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9\-]*[a-zA-Z0-9])\.)*([A-Za-z0-9]|[A-Za-z0-9][A-Za-z0-9\-]*[A-Za-z0-9])$")  # noqa
 MAX_HOSTNAME_LEN = 255
 
 log = logging.getLogger('dd.datadogpy')
```

### Comparing `datadog-0.8.0/datadog.egg-info/PKG-INFO` & `datadog-0.9.0/datadog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: datadog
-Version: 0.8.0
+Version: 0.9.0
 Summary: The Datadog Python library
 Home-page: http://www.datadoghq.com
 Author: Datadog, Inc.
 Author-email: dev@datadoghq.com
 License: BSD
 Description: UNKNOWN
 Keywords: datadog data
```

### Comparing `datadog-0.8.0/datadog.egg-info/SOURCES.txt` & `datadog-0.9.0/datadog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datadog-0.8.0/PKG-INFO` & `datadog-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: datadog
-Version: 0.8.0
+Version: 0.9.0
 Summary: The Datadog Python library
 Home-page: http://www.datadoghq.com
 Author: Datadog, Inc.
 Author-email: dev@datadoghq.com
 License: BSD
 Description: UNKNOWN
 Keywords: datadog data
```

### Comparing `datadog-0.8.0/setup.py` & `datadog-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from setuptools import setup
 import sys
 
 install_reqs = [
     "decorator>=3.3.2",
     "requests>=2.6.0",
 ]
+
 if sys.version_info[0] == 2:
-    # simplejson is not python3 compatible
     install_reqs.append("simplejson>=2.0.9")
+else:
+    install_reqs.append("simplejson>=3.0.0")
 
 if [sys.version_info[0], sys.version_info[1]] < [2, 7]:
     install_reqs.append("argparse>=1.2")
 
 setup(
     name="datadog",
-    version="0.8.0",
+    version="0.9.0",
     install_requires=install_reqs,
     tests_require=["tox", "nose", "mock", "six", "pillow"],
     packages=[
         'datadog',
         'datadog.api',
         'datadog.dogstatsd',
         'datadog.threadstats',
```


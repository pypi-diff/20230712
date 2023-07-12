# Comparing `tmp/ytsaurus-spyt-1.70.1b456.post18771733.dev24.tar.gz` & `tmp/ytsaurus-spyt-1.70.1b456.post7419714.dev25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ytsaurus-spyt-1.70.1b456.post18771733.dev24.tar", last modified: Wed Jul 12 10:29:01 2023, max compression
+gzip compressed data, was "dist/ytsaurus-spyt-1.70.1b456.post7419714.dev25.tar", last modified: Wed Jul 12 10:53:07 2023, max compression
```

## Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24.tar` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-07-12 10:29:01.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-07-12 10:29:01.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-07-12 10:29:01.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/bin/
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-07-12 10:29:00.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/bin/spark-discovery-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11888 2023-07-12 10:29:00.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/bin/spark-launch-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2298 2023-07-12 10:29:00.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/bin/spark-manage-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-07-12 10:29:00.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/bin/spark-shell-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-07-12 10:29:00.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/bin/spark-submit-yt
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-07-12 10:29:01.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/jars/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798359 2023-07-12 10:29:00.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/jars/spark-yt-submit.jar
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-07-12 10:29:01.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/__init__.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/client.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/common.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7357 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/conf.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/dependency_utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4258 2023-07-12 09:34:53.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/enabler.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    37225 2023-07-12 09:34:53.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/standalone.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/submit.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/types.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      183 2023-07-12 10:28:10.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/version.py
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-07-12 10:29:01.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/ytsaurus_spyt.egg-info/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      773 2023-07-12 10:29:01.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/ytsaurus_spyt.egg-info/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      550 2023-07-12 10:29:01.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/ytsaurus_spyt.egg-info/SOURCES.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-07-12 10:29:01.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/ytsaurus_spyt.egg-info/dependency_links.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-07-12 10:29:01.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/ytsaurus_spyt.egg-info/requires.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-07-12 10:29:01.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/ytsaurus_spyt.egg-info/top_level.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/MANIFEST.in
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      347 2023-07-12 09:34:53.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/README.md
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1161 2023-07-12 09:34:53.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/setup.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      773 2023-07-12 10:29:01.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-07-12 10:29:01.000000 ytsaurus-spyt-1.70.1b456.post18771733.dev24/setup.cfg
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/bin/
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/bin/spark-discovery-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11888 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/bin/spark-launch-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2298 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/bin/spark-manage-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/bin/spark-shell-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/bin/spark-submit-yt
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/jars/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798359 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/jars/spark-yt-submit.jar
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/__init__.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/client.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/common.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7357 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/conf.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/dependency_utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4258 2023-07-12 09:34:53.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/enabler.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    37225 2023-07-12 09:34:53.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/standalone.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/submit.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/types.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-05-11 12:57:25.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      181 2023-07-12 10:51:58.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/version.py
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/ytsaurus_spyt.egg-info/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      772 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/ytsaurus_spyt.egg-info/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      550 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/ytsaurus_spyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/ytsaurus_spyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/ytsaurus_spyt.egg-info/requires.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/ytsaurus_spyt.egg-info/top_level.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/MANIFEST.in
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      347 2023-07-12 09:34:53.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/README.md
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1161 2023-07-12 09:34:53.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/setup.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      772 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-07-12 10:53:07.000000 ytsaurus-spyt-1.70.1b456.post7419714.dev25/setup.cfg
```

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/bin/spark-discovery-yt` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/bin/spark-discovery-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/bin/spark-launch-yt` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/bin/spark-launch-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/bin/spark-manage-yt` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/bin/spark-manage-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/bin/spark-shell-yt` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/bin/spark-shell-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/bin/spark-submit-yt` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/bin/spark-submit-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/deps/jars/spark-yt-submit.jar` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/deps/jars/spark-yt-submit.jar`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/client.py` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/client.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/common.py` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/common.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/conf.py` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/conf.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/enabler.py` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/enabler.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/standalone.py` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/standalone.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/submit.py` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/submit.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/types.py` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/types.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/spyt/utils.py` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/spyt/utils.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/ytsaurus_spyt.egg-info/PKG-INFO` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/ytsaurus_spyt.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: ytsaurus-spyt
-Version: 1.70.1b456.post18771733.dev24
+Version: 1.70.1b456.post7419714.dev25
 Summary: YTsaurus SPYT high-level client
 Home-page: https://github.com/ytsaurus/ytsaurus/tree/main/yt/spark/spark-over-yt
 Author: YTsaurus
 Author-email: dev@ytsaurus.tech
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: # YTsaurus SPYT
```

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/ytsaurus_spyt.egg-info/SOURCES.txt` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/ytsaurus_spyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/setup.py` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/setup.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.70.1b456.post18771733.dev24/PKG-INFO` & `ytsaurus-spyt-1.70.1b456.post7419714.dev25/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: ytsaurus-spyt
-Version: 1.70.1b456.post18771733.dev24
+Version: 1.70.1b456.post7419714.dev25
 Summary: YTsaurus SPYT high-level client
 Home-page: https://github.com/ytsaurus/ytsaurus/tree/main/yt/spark/spark-over-yt
 Author: YTsaurus
 Author-email: dev@ytsaurus.tech
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: # YTsaurus SPYT
```


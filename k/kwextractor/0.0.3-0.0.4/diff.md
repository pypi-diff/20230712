# Comparing `tmp/kwextractor-0.0.3.tar.gz` & `tmp/kwextractor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwextractor-0.0.3.tar", last modified: Wed Jul 12 12:53:51 2023, max compression
+gzip compressed data, was "kwextractor-0.0.4.tar", last modified: Wed Jul 12 12:57:23 2023, max compression
```

## Comparing `kwextractor-0.0.3.tar` & `kwextractor-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 12:53:51.176279 kwextractor-0.0.3/
--rw-rw-rw-   0        0        0      188 2023-07-12 12:53:51.174276 kwextractor-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4648 2022-12-15 02:51:31.000000 kwextractor-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 12:53:51.116279 kwextractor-0.0.3/kwextractor/
--rw-rw-rw-   0        0        0        0 2022-11-11 03:30:05.000000 kwextractor-0.0.3/kwextractor/__init__.py
--rw-rw-rw-   0        0        0      367 2022-11-11 03:10:14.000000 kwextractor-0.0.3/kwextractor/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:53:51.149277 kwextractor-0.0.3/kwextractor/data/
--rw-rw-rw-   0        0        0      911 2022-11-11 03:10:14.000000 kwextractor-0.0.3/kwextractor/data/data_emotion_words.txt
--rw-rw-rw-   0        0        0   159440 2022-12-01 04:00:09.000000 kwextractor-0.0.3/kwextractor/data/data_full_allkeywords.txt
--rw-rw-rw-   0        0        0    23149 2022-12-15 02:41:27.000000 kwextractor-0.0.3/kwextractor/data/stop_words_vn_tokenized.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 12:53:51.162279 kwextractor-0.0.3/kwextractor/process/
--rw-rw-rw-   0        0        0        0 2022-11-11 03:10:14.000000 kwextractor-0.0.3/kwextractor/process/__init__.py
--rw-rw-rw-   0        0        0    10753 2022-12-15 03:03:00.000000 kwextractor-0.0.3/kwextractor/process/extract_keywords.py
--rw-rw-rw-   0        0        0      899 2022-11-11 03:32:31.000000 kwextractor-0.0.3/kwextractor/process/extract_numverse.py
--rw-rw-rw-   0        0        0     1494 2022-12-14 15:19:21.000000 kwextractor-0.0.3/kwextractor/process/replacing_w2n.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:53:51.167279 kwextractor-0.0.3/kwextractor/utils/
--rw-rw-rw-   0        0        0        0 2022-11-11 03:30:05.000000 kwextractor-0.0.3/kwextractor/utils/__init__.py
--rw-rw-rw-   0        0        0     3518 2022-12-15 02:26:46.000000 kwextractor-0.0.3/kwextractor/utils/process_kw.py
--rw-rw-rw-   0        0        0       82 2023-07-12 12:31:13.000000 kwextractor-0.0.3/kwextractor/version.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:53:51.139276 kwextractor-0.0.3/kwextractor.egg-info/
--rw-rw-rw-   0        0        0      188 2023-07-12 12:53:50.000000 kwextractor-0.0.3/kwextractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      629 2023-07-12 12:53:50.000000 kwextractor-0.0.3/kwextractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 12:53:50.000000 kwextractor-0.0.3/kwextractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-12 12:53:50.000000 kwextractor-0.0.3/kwextractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-12 12:53:50.000000 kwextractor-0.0.3/kwextractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 12:53:51.176279 kwextractor-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      760 2022-11-11 08:43:25.000000 kwextractor-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:53:51.171279 kwextractor-0.0.3/tests/
--rw-rw-rw-   0        0        0     1308 2022-12-15 03:04:53.000000 kwextractor-0.0.3/tests/test_kwextractor.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:57:23.060550 kwextractor-0.0.4/
+-rw-rw-rw-   0        0        0      188 2023-07-12 12:57:23.060550 kwextractor-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4648 2022-12-15 02:51:31.000000 kwextractor-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 12:57:22.964989 kwextractor-0.0.4/kwextractor/
+-rw-rw-rw-   0        0        0        0 2022-11-11 03:30:05.000000 kwextractor-0.0.4/kwextractor/__init__.py
+-rw-rw-rw-   0        0        0      367 2022-11-11 03:10:14.000000 kwextractor-0.0.4/kwextractor/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:57:23.029020 kwextractor-0.0.4/kwextractor/data/
+-rw-rw-rw-   0        0        0      911 2022-11-11 03:10:14.000000 kwextractor-0.0.4/kwextractor/data/data_emotion_words.txt
+-rw-rw-rw-   0        0        0   159440 2022-12-01 04:00:09.000000 kwextractor-0.0.4/kwextractor/data/data_full_allkeywords.txt
+-rw-rw-rw-   0        0        0    23149 2022-12-15 02:41:27.000000 kwextractor-0.0.4/kwextractor/data/stop_words_vn_tokenized.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 12:57:23.042020 kwextractor-0.0.4/kwextractor/process/
+-rw-rw-rw-   0        0        0        0 2022-11-11 03:10:14.000000 kwextractor-0.0.4/kwextractor/process/__init__.py
+-rw-rw-rw-   0        0        0    10753 2022-12-15 03:03:00.000000 kwextractor-0.0.4/kwextractor/process/extract_keywords.py
+-rw-rw-rw-   0        0        0      899 2022-11-11 03:32:31.000000 kwextractor-0.0.4/kwextractor/process/extract_numverse.py
+-rw-rw-rw-   0        0        0     1494 2022-12-14 15:19:21.000000 kwextractor-0.0.4/kwextractor/process/replacing_w2n.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:57:23.048021 kwextractor-0.0.4/kwextractor/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-11 03:30:05.000000 kwextractor-0.0.4/kwextractor/utils/__init__.py
+-rw-rw-rw-   0        0        0     3518 2022-12-15 02:26:46.000000 kwextractor-0.0.4/kwextractor/utils/process_kw.py
+-rw-rw-rw-   0        0        0       82 2023-07-12 12:57:16.000000 kwextractor-0.0.4/kwextractor/version.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:57:23.016490 kwextractor-0.0.4/kwextractor.egg-info/
+-rw-rw-rw-   0        0        0      188 2023-07-12 12:57:22.000000 kwextractor-0.0.4/kwextractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      639 2023-07-12 12:57:22.000000 kwextractor-0.0.4/kwextractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:57:22.000000 kwextractor-0.0.4/kwextractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-12 12:57:22.000000 kwextractor-0.0.4/kwextractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 12:57:22.000000 kwextractor-0.0.4/kwextractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-12 12:57:23.065551 kwextractor-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      760 2022-11-11 08:43:25.000000 kwextractor-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:57:23.052020 kwextractor-0.0.4/tests/
+-rw-rw-rw-   0        0        0     1308 2022-12-15 03:04:53.000000 kwextractor-0.0.4/tests/test_kwextractor.py
```

### Comparing `kwextractor-0.0.3/README.md` & `kwextractor-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.3/kwextractor/data/data_emotion_words.txt` & `kwextractor-0.0.4/kwextractor/data/data_emotion_words.txt`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.3/kwextractor/data/data_full_allkeywords.txt` & `kwextractor-0.0.4/kwextractor/data/data_full_allkeywords.txt`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.3/kwextractor/data/stop_words_vn_tokenized.txt` & `kwextractor-0.0.4/kwextractor/data/stop_words_vn_tokenized.txt`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.3/kwextractor/process/extract_keywords.py` & `kwextractor-0.0.4/kwextractor/process/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.3/kwextractor/process/extract_numverse.py` & `kwextractor-0.0.4/kwextractor/process/extract_numverse.py`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.3/kwextractor/process/replacing_w2n.py` & `kwextractor-0.0.4/kwextractor/process/replacing_w2n.py`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.3/kwextractor/utils/process_kw.py` & `kwextractor-0.0.4/kwextractor/utils/process_kw.py`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.3/kwextractor.egg-info/SOURCES.txt` & `kwextractor-0.0.4/kwextractor.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.md
+setup.cfg
 setup.py
 kwextractor/__init__.py
 kwextractor/constants.py
 kwextractor/version.py
 kwextractor.egg-info/PKG-INFO
 kwextractor.egg-info/SOURCES.txt
 kwextractor.egg-info/dependency_links.txt
```

### Comparing `kwextractor-0.0.3/setup.py` & `kwextractor-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.3/tests/test_kwextractor.py` & `kwextractor-0.0.4/tests/test_kwextractor.py`

 * *Files identical despite different names*


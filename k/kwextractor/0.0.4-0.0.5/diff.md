# Comparing `tmp/kwextractor-0.0.4.tar.gz` & `tmp/kwextractor-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwextractor-0.0.4.tar", last modified: Wed Jul 12 12:57:23 2023, max compression
+gzip compressed data, was "kwextractor-0.0.5.tar", last modified: Wed Jul 12 13:05:30 2023, max compression
```

## Comparing `kwextractor-0.0.4.tar` & `kwextractor-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 12:57:23.060550 kwextractor-0.0.4/
--rw-rw-rw-   0        0        0      188 2023-07-12 12:57:23.060550 kwextractor-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4648 2022-12-15 02:51:31.000000 kwextractor-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 12:57:22.964989 kwextractor-0.0.4/kwextractor/
--rw-rw-rw-   0        0        0        0 2022-11-11 03:30:05.000000 kwextractor-0.0.4/kwextractor/__init__.py
--rw-rw-rw-   0        0        0      367 2022-11-11 03:10:14.000000 kwextractor-0.0.4/kwextractor/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:57:23.029020 kwextractor-0.0.4/kwextractor/data/
--rw-rw-rw-   0        0        0      911 2022-11-11 03:10:14.000000 kwextractor-0.0.4/kwextractor/data/data_emotion_words.txt
--rw-rw-rw-   0        0        0   159440 2022-12-01 04:00:09.000000 kwextractor-0.0.4/kwextractor/data/data_full_allkeywords.txt
--rw-rw-rw-   0        0        0    23149 2022-12-15 02:41:27.000000 kwextractor-0.0.4/kwextractor/data/stop_words_vn_tokenized.txt
-drwxrwxrwx   0        0        0        0 2023-07-12 12:57:23.042020 kwextractor-0.0.4/kwextractor/process/
--rw-rw-rw-   0        0        0        0 2022-11-11 03:10:14.000000 kwextractor-0.0.4/kwextractor/process/__init__.py
--rw-rw-rw-   0        0        0    10753 2022-12-15 03:03:00.000000 kwextractor-0.0.4/kwextractor/process/extract_keywords.py
--rw-rw-rw-   0        0        0      899 2022-11-11 03:32:31.000000 kwextractor-0.0.4/kwextractor/process/extract_numverse.py
--rw-rw-rw-   0        0        0     1494 2022-12-14 15:19:21.000000 kwextractor-0.0.4/kwextractor/process/replacing_w2n.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:57:23.048021 kwextractor-0.0.4/kwextractor/utils/
--rw-rw-rw-   0        0        0        0 2022-11-11 03:30:05.000000 kwextractor-0.0.4/kwextractor/utils/__init__.py
--rw-rw-rw-   0        0        0     3518 2022-12-15 02:26:46.000000 kwextractor-0.0.4/kwextractor/utils/process_kw.py
--rw-rw-rw-   0        0        0       82 2023-07-12 12:57:16.000000 kwextractor-0.0.4/kwextractor/version.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:57:23.016490 kwextractor-0.0.4/kwextractor.egg-info/
--rw-rw-rw-   0        0        0      188 2023-07-12 12:57:22.000000 kwextractor-0.0.4/kwextractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      639 2023-07-12 12:57:22.000000 kwextractor-0.0.4/kwextractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 12:57:22.000000 kwextractor-0.0.4/kwextractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-12 12:57:22.000000 kwextractor-0.0.4/kwextractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-12 12:57:22.000000 kwextractor-0.0.4/kwextractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-12 12:57:23.065551 kwextractor-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      760 2022-11-11 08:43:25.000000 kwextractor-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:57:23.052020 kwextractor-0.0.4/tests/
--rw-rw-rw-   0        0        0     1308 2022-12-15 03:04:53.000000 kwextractor-0.0.4/tests/test_kwextractor.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:05:30.508204 kwextractor-0.0.5/
+-rw-rw-rw-   0        0        0     4879 2023-07-12 13:05:30.501231 kwextractor-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4648 2022-12-15 02:51:31.000000 kwextractor-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 13:05:30.444217 kwextractor-0.0.5/kwextractor/
+-rw-rw-rw-   0        0        0        0 2022-11-11 03:30:05.000000 kwextractor-0.0.5/kwextractor/__init__.py
+-rw-rw-rw-   0        0        0      367 2022-11-11 03:10:14.000000 kwextractor-0.0.5/kwextractor/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:05:30.475205 kwextractor-0.0.5/kwextractor/data/
+-rw-rw-rw-   0        0        0      911 2022-11-11 03:10:14.000000 kwextractor-0.0.5/kwextractor/data/data_emotion_words.txt
+-rw-rw-rw-   0        0        0   159440 2022-12-01 04:00:09.000000 kwextractor-0.0.5/kwextractor/data/data_full_allkeywords.txt
+-rw-rw-rw-   0        0        0    23149 2022-12-15 02:41:27.000000 kwextractor-0.0.5/kwextractor/data/stop_words_vn_tokenized.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 13:05:30.488210 kwextractor-0.0.5/kwextractor/process/
+-rw-rw-rw-   0        0        0        0 2022-11-11 03:10:14.000000 kwextractor-0.0.5/kwextractor/process/__init__.py
+-rw-rw-rw-   0        0        0    10753 2022-12-15 03:03:00.000000 kwextractor-0.0.5/kwextractor/process/extract_keywords.py
+-rw-rw-rw-   0        0        0      899 2022-11-11 03:32:31.000000 kwextractor-0.0.5/kwextractor/process/extract_numverse.py
+-rw-rw-rw-   0        0        0     1494 2022-12-14 15:19:21.000000 kwextractor-0.0.5/kwextractor/process/replacing_w2n.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:05:30.494209 kwextractor-0.0.5/kwextractor/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-11 03:30:05.000000 kwextractor-0.0.5/kwextractor/utils/__init__.py
+-rw-rw-rw-   0        0        0     3518 2022-12-15 02:26:46.000000 kwextractor-0.0.5/kwextractor/utils/process_kw.py
+-rw-rw-rw-   0        0        0       82 2023-07-12 13:02:26.000000 kwextractor-0.0.5/kwextractor/version.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:05:30.465218 kwextractor-0.0.5/kwextractor.egg-info/
+-rw-rw-rw-   0        0        0     4879 2023-07-12 13:05:30.000000 kwextractor-0.0.5/kwextractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-07-12 13:05:30.000000 kwextractor-0.0.5/kwextractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 13:05:30.000000 kwextractor-0.0.5/kwextractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-12 13:05:30.000000 kwextractor-0.0.5/kwextractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 13:05:30.000000 kwextractor-0.0.5/kwextractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 13:05:30.509210 kwextractor-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      985 2023-07-12 13:03:32.000000 kwextractor-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:05:30.497207 kwextractor-0.0.5/tests/
+-rw-rw-rw-   0        0        0     1308 2022-12-15 03:04:53.000000 kwextractor-0.0.5/tests/test_kwextractor.py
```

### Comparing `kwextractor-0.0.4/README.md` & `kwextractor-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.4/kwextractor/data/data_emotion_words.txt` & `kwextractor-0.0.5/kwextractor/data/data_emotion_words.txt`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.4/kwextractor/data/data_full_allkeywords.txt` & `kwextractor-0.0.5/kwextractor/data/data_full_allkeywords.txt`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.4/kwextractor/data/stop_words_vn_tokenized.txt` & `kwextractor-0.0.5/kwextractor/data/stop_words_vn_tokenized.txt`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.4/kwextractor/process/extract_keywords.py` & `kwextractor-0.0.5/kwextractor/process/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.4/kwextractor/process/extract_numverse.py` & `kwextractor-0.0.5/kwextractor/process/extract_numverse.py`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.4/kwextractor/process/replacing_w2n.py` & `kwextractor-0.0.5/kwextractor/process/replacing_w2n.py`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.4/kwextractor/utils/process_kw.py` & `kwextractor-0.0.5/kwextractor/utils/process_kw.py`

 * *Files identical despite different names*

### Comparing `kwextractor-0.0.4/kwextractor.egg-info/SOURCES.txt` & `kwextractor-0.0.5/kwextractor.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 README.md
-setup.cfg
 setup.py
 kwextractor/__init__.py
 kwextractor/constants.py
 kwextractor/version.py
 kwextractor.egg-info/PKG-INFO
 kwextractor.egg-info/SOURCES.txt
 kwextractor.egg-info/dependency_links.txt
```

### Comparing `kwextractor-0.0.4/setup.py` & `kwextractor-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-import os
+from pathlib import Path
 from kwextractor.version import get_kwextractor_version
 from setuptools import setup, find_packages
 
+this_directory = Path(__file__).parent
+long_description = (this_directory/"README.md").read_text(encoding='utf-8')
+
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="kwextractor",
     version=get_kwextractor_version(),
     packages=find_packages(
@@ -19,8 +22,10 @@
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     test_suite='tests',
     description="Extract keywords for vietnamese text.",
     author="Trinh Do Duy Hung",
     author_email="trinhhungsss492@gmail.com",
     license="MIT",
+    long_description=long_description,
+    long_description_content_type='text/markdown'
 )
```

### Comparing `kwextractor-0.0.4/tests/test_kwextractor.py` & `kwextractor-0.0.5/tests/test_kwextractor.py`

 * *Files identical despite different names*


# Comparing `tmp/interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1.tar.gz` & `tmp/interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1.tar", last modified: Tue Jul 11 17:18:03 2023, max compression
+gzip compressed data, was "interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2.tar", last modified: Wed Jul 12 13:00:03 2023, max compression
```

## Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1.tar` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 17:18:03.364354 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 17:18:03.360355 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/.github/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 17:18:03.360355 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/.github/workflows/
--rw-rw-r--   0 alex      (1000) alex      (1000)      569 2023-07-11 17:15:18.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/.github/workflows/tests.yml
--rw-rw-r--   0 alex      (1000) alex      (1000)     1393 2023-07-11 17:02:47.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/.gitignore
--rw-rw-r--   0 alex      (1000) alex      (1000)      381 2023-07-10 19:26:02.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/.pre-commit-config.yaml
--rw-rw-r--   0 alex      (1000) alex      (1000)     1066 2023-07-11 17:00:06.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/LICENSE.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      741 2023-07-11 17:18:03.364354 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      105 2023-07-10 15:16:42.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/README.md
--rw-rw-r--   0 alex      (1000) alex      (1000)       53 2023-07-10 15:16:42.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/design.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 17:18:03.364354 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)      741 2023-07-11 17:18:03.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      892 2023-07-11 17:18:03.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-11 17:18:03.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-11 17:10:17.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1000) alex      (1000)       44 2023-07-11 17:18:03.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-11 17:18:03.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/top_level.txt
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 17:18:03.364354 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/lotr_sdk/
--rw-rw-r--   0 alex      (1000) alex      (1000)      200 2023-07-11 17:04:05.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/lotr_sdk/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3439 2023-07-11 16:37:26.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/lotr_sdk/client.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2045 2023-07-11 16:34:22.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/lotr_sdk/resources.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      261 2023-07-10 19:29:18.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/lotr_sdk/utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-11 17:18:03.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/lotr_sdk/version.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      622 2023-07-10 15:16:42.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/pull_request_template.md
--rw-rw-r--   0 alex      (1000) alex      (1000)      231 2023-07-11 17:02:47.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/pyproject.toml
--rwxrwxr-x   0 alex      (1000) alex      (1000)      596 2022-12-20 12:53:52.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/release.sh
--rw-rw-r--   0 alex      (1000) alex      (1000)      859 2023-07-11 17:18:03.368355 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/setup.cfg
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 17:18:03.364354 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/tests/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-10 17:56:59.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/tests/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 17:18:03.364354 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/tests/recorded_responses/
--rw-rw-r--   0 alex      (1000) alex      (1000)     4664 2023-07-11 16:38:34.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/tests/recorded_responses/test_movie_by_id.yml
--rw-rw-r--   0 alex      (1000) alex      (1000)     4668 2023-07-11 16:40:52.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/tests/recorded_responses/test_movies_collection.yml
--rw-rw-r--   0 alex      (1000) alex      (1000)      501 2023-07-11 16:38:34.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/tests/recorded_responses/test_quote_by_id.yml
--rw-rw-r--   0 alex      (1000) alex      (1000)     1514 2023-07-11 16:38:34.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/tests/recorded_responses/test_quotes_collection.yml
--rw-rw-r--   0 alex      (1000) alex      (1000)     3533 2023-07-11 16:40:46.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/tests/test_client.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      105 2023-07-11 17:09:57.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/tox.ini
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-12 13:00:03.340534 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-12 13:00:03.336534 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/.github/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-12 13:00:03.340534 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/.github/workflows/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      569 2023-07-11 17:15:18.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/.github/workflows/tests.yml
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1393 2023-07-11 17:02:47.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/.gitignore
+-rw-rw-r--   0 alex      (1000) alex      (1000)      381 2023-07-10 19:26:02.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/.pre-commit-config.yaml
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1066 2023-07-11 17:00:06.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/LICENSE.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      741 2023-07-12 13:00:03.340534 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3269 2023-07-11 18:21:25.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/README.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3603 2023-07-11 19:32:19.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/design.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-12 13:00:03.340534 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      741 2023-07-12 13:00:03.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      932 2023-07-12 13:00:03.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-12 13:00:03.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-11 17:10:17.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1000) alex      (1000)       44 2023-07-12 13:00:03.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-12 13:00:03.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/top_level.txt
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-12 13:00:03.340534 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/lotr_sdk/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      200 2023-07-11 17:04:05.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/lotr_sdk/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4357 2023-07-11 20:39:29.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/lotr_sdk/client.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2054 2023-07-11 20:34:50.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/lotr_sdk/resources.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      261 2023-07-10 19:29:18.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/lotr_sdk/utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-12 13:00:03.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/lotr_sdk/version.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      622 2023-07-10 15:16:42.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/pull_request_template.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)      231 2023-07-11 17:02:47.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/pyproject.toml
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      596 2022-12-20 12:53:52.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/release.sh
+-rw-rw-r--   0 alex      (1000) alex      (1000)      859 2023-07-12 13:00:03.340534 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-12 13:00:03.340534 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tests/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-10 17:56:59.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tests/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-12 13:00:03.340534 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tests/recorded_responses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      602 2023-07-11 20:20:58.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tests/recorded_responses/test_close.yml
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4664 2023-07-11 16:38:34.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tests/recorded_responses/test_movie_by_id.yml
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4668 2023-07-11 16:40:52.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tests/recorded_responses/test_movies_collection.yml
+-rw-rw-r--   0 alex      (1000) alex      (1000)      501 2023-07-11 16:38:34.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tests/recorded_responses/test_quote_by_id.yml
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1514 2023-07-11 16:38:34.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tests/recorded_responses/test_quotes_collection.yml
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3910 2023-07-11 20:38:47.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tests/test_client.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      105 2023-07-11 17:09:57.000000 interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tox.ini
```

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/.github/workflows/tests.yml` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/.gitignore` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/LICENSE.txt` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/PKG-INFO` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interview_6823bb0acd1b4ca8a37a2e052ac5dce2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Interview task that I don't want to be too easy to find
 Home-page: https://github.com/hatchways-community/6823bb0acd1b4ca8a37a2e052ac5dce2
 Author: Alex Hall
 Author-email: alex.mojaki@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/PKG-INFO` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interview-6823bb0acd1b4ca8a37a2e052ac5dce2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Interview task that I don't want to be too easy to find
 Home-page: https://github.com/hatchways-community/6823bb0acd1b4ca8a37a2e052ac5dce2
 Author: Alex Hall
 Author-email: alex.mojaki@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/SOURCES.txt` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/interview_6823bb0acd1b4ca8a37a2e052ac5dce2.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,11 +18,12 @@
 lotr_sdk/__init__.py
 lotr_sdk/client.py
 lotr_sdk/resources.py
 lotr_sdk/utils.py
 lotr_sdk/version.py
 tests/__init__.py
 tests/test_client.py
+tests/recorded_responses/test_close.yml
 tests/recorded_responses/test_movie_by_id.yml
 tests/recorded_responses/test_movies_collection.yml
 tests/recorded_responses/test_quote_by_id.yml
 tests/recorded_responses/test_quotes_collection.yml
```

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/lotr_sdk/resources.py` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/lotr_sdk/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,9 +67,9 @@
     def movie_id(self) -> str:
         return self.raw_data["movie"]
 
     @property
     def character_id(self) -> str:
         return self.raw_data["character"]
 
-    def movie(self):
+    def movie(self) -> Movie:
         return self._client.movie(self.movie_id)
```

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/pull_request_template.md` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/release.sh` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/release.sh`

 * *Files identical despite different names*

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/setup.cfg` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/tests/recorded_responses/test_movie_by_id.yml` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tests/recorded_responses/test_movie_by_id.yml`

 * *Files identical despite different names*

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/tests/recorded_responses/test_movies_collection.yml` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tests/recorded_responses/test_movies_collection.yml`

 * *Files identical despite different names*

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/tests/recorded_responses/test_quotes_collection.yml` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tests/recorded_responses/test_quotes_collection.yml`

 * *Files identical despite different names*

### Comparing `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.1/tests/test_client.py` & `interview_6823bb0acd1b4ca8a37a2e052ac5dce2-0.0.2/tests/test_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import functools
 import itertools
 import os
+import unittest.mock
 from pathlib import Path
 
 import responses
 import responses._recorder
 
 from lotr_sdk import Client
 
-client = Client(os.environ.get("THE_ONE_API_KEY"))
+client = Client(os.environ.get("THE_ONE_API_KEY", ""))
 
 RESPONSES_MODE = os.environ.get("RECORD_RESPONSES_MODE", "replay")
 
 
 def record_responses(func):
     path = Path(__file__).parent / "recorded_responses" / f"{func.__name__}.yml"
     if RESPONSES_MODE == "replay":
@@ -57,17 +58,17 @@
     lst = list(collection)
     assert len(lst) == len(set(lst)) == size == 8
     assert list(collection) == []
 
     for movie in lst:
         check_movie(movie)
 
-    if collection.paginator.params.sort == "name:asc":
+    if collection._paginator.params.sort == "name:asc":
         assert lst == sorted(lst, key=lambda m: m.name)
-    elif collection.paginator.params.sort == "name:desc":
+    elif collection._paginator.params.sort == "name:desc":
         assert lst == sorted(lst, key=lambda m: m.name, reverse=True)
     return lst
 
 
 def check_quotes_collection(collection):
     size = len(collection)
     max_items = 5
@@ -118,7 +119,17 @@
         "_id": quote_id,
         "id": quote_id,
         "character": "5cd99d4bde30eff6ebccfea0",
         "dialog": "Fool of a Took! Throw yourself in next time, and rid us of your "
         "stupidity!",
         "movie": "5cd95395de30eff6ebccde5c",
     }
+
+
+@record_responses
+def test_close():
+    temp_client = Client("")
+    # requests.Session.close surprisingly has no easily testable effect
+    temp_client.session.close = unittest.mock.Mock()  # type: ignore
+    with temp_client:
+        assert temp_client.session.get("https://httpbin.org/get").ok
+    temp_client.session.close.assert_called_once()
```


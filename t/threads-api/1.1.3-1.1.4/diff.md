# Comparing `tmp/threads-api-1.1.3.tar.gz` & `tmp/threads-api-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.1.3.tar", last modified: Wed Jul 12 16:49:12 2023, max compression
+gzip compressed data, was "threads-api-1.1.4.tar", last modified: Wed Jul 12 20:15:23 2023, max compression
```

## Comparing `threads-api-1.1.3.tar` & `threads-api-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 16:49:12.653453 threads-api-1.1.3/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.3/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    13376 2023-07-12 16:49:12.653453 threads-api-1.1.3/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    12846 2023-07-12 15:14:47.000000 threads-api-1.1.3/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      452 2023-07-12 16:45:24.000000 threads-api-1.1.3/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-12 16:49:12.653453 threads-api-1.1.3/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      768 2023-07-12 16:37:50.000000 threads-api-1.1.3/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 16:49:12.641453 threads-api-1.1.3/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.3/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 16:49:12.645453 threads-api-1.1.3/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.3/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    29672 2023-07-12 16:36:59.000000 threads-api-1.1.3/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 16:49:12.645453 threads-api-1.1.3/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.3/threads_api/tests/__init__.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      406 2023-07-11 20:05:14.000000 threads-api-1.1.3/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 16:49:12.641453 threads-api-1.1.3/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    13376 2023-07-12 16:49:12.000000 threads-api-1.1.3/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-12 16:49:12.000000 threads-api-1.1.3/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-12 16:49:12.000000 threads-api-1.1.3/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-12 16:49:12.000000 threads-api-1.1.3/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-12 16:49:12.000000 threads-api-1.1.3/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:15:23.084892 threads-api-1.1.4/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.4/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    13446 2023-07-12 20:15:23.084892 threads-api-1.1.4/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    12916 2023-07-12 20:11:18.000000 threads-api-1.1.4/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      452 2023-07-12 20:11:18.000000 threads-api-1.1.4/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-12 20:15:23.084892 threads-api-1.1.4/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      768 2023-07-12 20:11:18.000000 threads-api-1.1.4/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:15:23.084892 threads-api-1.1.4/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.4/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:15:23.084892 threads-api-1.1.4/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.4/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    29835 2023-07-12 20:11:18.000000 threads-api-1.1.4/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:15:23.084892 threads-api-1.1.4/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.4/threads_api/tests/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      305 2023-07-12 19:46:32.000000 threads-api-1.1.4/threads_api/tests/get_post_id_test.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      370 2023-07-12 20:11:18.000000 threads-api-1.1.4/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:15:23.084892 threads-api-1.1.4/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    13446 2023-07-12 20:15:23.000000 threads-api-1.1.4/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      404 2023-07-12 20:15:23.000000 threads-api-1.1.4/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-12 20:15:23.000000 threads-api-1.1.4/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-12 20:15:23.000000 threads-api-1.1.4/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-12 20:15:23.000000 threads-api-1.1.4/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.1.3/LICENSE` & `threads-api-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.3/PKG-INFO` & `threads-api-1.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: threads-api
-Version: 1.1.3
-Summary: Unofficial Python client for Meta Threads.net API
-Home-page: https://github.com/danie1/threads-api
-Author: Danie1
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # [<img src="https://raw.githubusercontent.com/danie1/threads-api/main/.github/logo.jpg" width="36" height="36" />](https://github.com/danie1) Meta's Threads.net API
 
 [![Downdloads](https://pepy.tech/badge/threads-api)](https://pypi.org/project/threads-api/)
 [![Version](https://img.shields.io/pypi/v/threads-api.svg?style=flat)](https://pypi.org/project/threads-api/)
 [![Python](https://img.shields.io/pypi/pyversions/threads-api.svg)](https://pypi.org/project/threads-api/) [![MIT License](https://img.shields.io/pypi/l/threads-api.svg?style=flat)](https://github.com/Danie1/threads-api/blob/main/LICENSE) 
 
 > Unofficial, Reverse-Engineered Python client for Meta's [Threads](https://threads.net).
@@ -27,14 +10,16 @@
 
 # Threads API - Python
 
 Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to login, read and publish posts, view who liked a post, retrieve user profile information, follow/unfollow and much more.
 
 It is built using `aiohttp` to ease asynchronous execution of the API, for ⚡ super-fast ⚡ results.
 
+> Note: Since v1.1.3 we are using ```instagrapi``` package to login.
+
 Table of content:
 
 * [Demo](#demo)
 * [Getting started](#getting-started)
   * [Installation](#Installation)
 * [Usage Examples](#usage-examples)
 * [Roadmap](#📌-roadmap)
@@ -381,9 +366,7 @@
 - [x] ✅  CI/CD
   - [x] ✅  GitHub Actions Pipeline
   - [ ] 🚧  Pytest
 
 
 # License
 This project is licensed under the MIT license.
-
-
```

### Comparing `threads-api-1.1.3/README.md` & `threads-api-1.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: threads-api
+Version: 1.1.4
+Summary: Unofficial Python client for Meta Threads.net API
+Home-page: https://github.com/danie1/threads-api
+Author: Danie1
+Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # [<img src="https://raw.githubusercontent.com/danie1/threads-api/main/.github/logo.jpg" width="36" height="36" />](https://github.com/danie1) Meta's Threads.net API
 
 [![Downdloads](https://pepy.tech/badge/threads-api)](https://pypi.org/project/threads-api/)
 [![Version](https://img.shields.io/pypi/v/threads-api.svg?style=flat)](https://pypi.org/project/threads-api/)
 [![Python](https://img.shields.io/pypi/pyversions/threads-api.svg)](https://pypi.org/project/threads-api/) [![MIT License](https://img.shields.io/pypi/l/threads-api.svg?style=flat)](https://github.com/Danie1/threads-api/blob/main/LICENSE) 
 
 > Unofficial, Reverse-Engineered Python client for Meta's [Threads](https://threads.net).
@@ -10,14 +27,16 @@
 
 # Threads API - Python
 
 Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to login, read and publish posts, view who liked a post, retrieve user profile information, follow/unfollow and much more.
 
 It is built using `aiohttp` to ease asynchronous execution of the API, for ⚡ super-fast ⚡ results.
 
+> Note: Since v1.1.3 we are using ```instagrapi``` package to login.
+
 Table of content:
 
 * [Demo](#demo)
 * [Getting started](#getting-started)
   * [Installation](#Installation)
 * [Usage Examples](#usage-examples)
 * [Roadmap](#📌-roadmap)
@@ -364,7 +383,9 @@
 - [x] ✅  CI/CD
   - [x] ✅  GitHub Actions Pipeline
   - [ ] 🚧  Pytest
 
 
 # License
 This project is licensed under the MIT license.
+
+
```

### Comparing `threads-api-1.1.3/setup.py` & `threads-api-1.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='threads-api',
-    version='1.1.3',
+    version='1.1.4',
     description='Unofficial Python client for Meta Threads.net API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Danie1',
     author_email='',
     url='https://github.com/danie1/threads-api',
     packages=find_packages(),
```

### Comparing `threads-api-1.1.3/threads_api/src/threads_api.py` & `threads-api-1.1.4/threads_api/src/threads_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -489,21 +489,25 @@
             post_url (str): The URL of the post.
         Returns:
             str: The post ID if found, or None if the post ID is not found.
 
         Raises:
             Exception: If an error occurs during the post ID retrieval process.
         """        
-        async with aiohttp.ClientSession() as session:
-            async with session.get(post_url, headers=await self._get_public_headers()) as response:
-                text = await response.text()
-
-        text = text.replace('\\s', "").replace('\\n', "")
-        post_id = re.search(r'"props":{"post_id":"(\d+)"},', text)
-        return post_id.group(1)
+        if "https://" in post_url and "/@" in post_url:
+            raise Exception(f"Argument {post_url} is not a valid URL")
+        elif "https://" in post_url and "/t" in post_url:
+            shortcode = post_url.split("/t/")[-1].split("/")[0]
+        elif len(post_url) == 11:
+            shortcode = post_url
+        alphabet = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789-_"
+        id = 0
+        for char in shortcode:
+            id = (id * 64) + alphabet.index(char)
+        return str(id)
 
     async def get_post(self, post_id: str):
         """
         Retrieves the post information for a given post ID.
 
         Args:
             post_id (str): The ID of the post.
```

### Comparing `threads-api-1.1.3/threads_api.egg-info/PKG-INFO` & `threads-api-1.1.4/threads_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.1.3
+Version: 1.1.4
 Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -27,14 +27,16 @@
 
 # Threads API - Python
 
 Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to login, read and publish posts, view who liked a post, retrieve user profile information, follow/unfollow and much more.
 
 It is built using `aiohttp` to ease asynchronous execution of the API, for ⚡ super-fast ⚡ results.
 
+> Note: Since v1.1.3 we are using ```instagrapi``` package to login.
+
 Table of content:
 
 * [Demo](#demo)
 * [Getting started](#getting-started)
   * [Installation](#Installation)
 * [Usage Examples](#usage-examples)
 * [Roadmap](#📌-roadmap)
```


# Comparing `tmp/developer_disk_image-0.0.1.tar.gz` & `tmp/developer_disk_image-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "developer_disk_image-0.0.1.tar", last modified: Tue Jul 11 17:14:49 2023, max compression
+gzip compressed data, was "developer_disk_image-0.0.2.tar", last modified: Wed Jul 12 05:21:29 2023, max compression
```

## Comparing `developer_disk_image-0.0.1.tar` & `developer_disk_image-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:14:49.379047 developer_disk_image-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-11 17:14:49.379047 developer_disk_image-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-11 17:14:29.000000 developer_disk_image-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:14:49.379047 developer_disk_image-0.0.1/developer_disk_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:14:29.000000 developer_disk_image-0.0.1/developer_disk_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-11 17:14:29.000000 developer_disk_image-0.0.1/developer_disk_image/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:14:49.379047 developer_disk_image-0.0.1/developer_disk_image.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-11 17:14:49.000000 developer_disk_image-0.0.1/developer_disk_image.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-11 17:14:49.000000 developer_disk_image-0.0.1/developer_disk_image.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:14:49.000000 developer_disk_image-0.0.1/developer_disk_image.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 17:14:49.000000 developer_disk_image-0.0.1/developer_disk_image.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 17:14:49.000000 developer_disk_image-0.0.1/developer_disk_image.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 17:14:49.000000 developer_disk_image-0.0.1/developer_disk_image.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-11 17:14:29.000000 developer_disk_image-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 17:14:29.000000 developer_disk_image-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:14:49.379047 developer_disk_image-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:14:49.379047 developer_disk_image-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-11 17:14:29.000000 developer_disk_image-0.0.1/tests/test_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:21:29.849850 developer_disk_image-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-12 05:21:29.849850 developer_disk_image-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-12 05:21:12.000000 developer_disk_image-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:21:29.849850 developer_disk_image-0.0.2/developer_disk_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:21:12.000000 developer_disk_image-0.0.2/developer_disk_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 05:21:12.000000 developer_disk_image-0.0.2/developer_disk_image/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-12 05:21:12.000000 developer_disk_image-0.0.2/developer_disk_image/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:21:29.849850 developer_disk_image-0.0.2/developer_disk_image.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-12 05:21:29.000000 developer_disk_image-0.0.2/developer_disk_image.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-12 05:21:29.000000 developer_disk_image-0.0.2/developer_disk_image.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 05:21:29.000000 developer_disk_image-0.0.2/developer_disk_image.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-12 05:21:29.000000 developer_disk_image-0.0.2/developer_disk_image.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 05:21:29.000000 developer_disk_image-0.0.2/developer_disk_image.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-12 05:21:29.000000 developer_disk_image-0.0.2/developer_disk_image.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-12 05:21:12.000000 developer_disk_image-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 05:21:12.000000 developer_disk_image-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 05:21:29.849850 developer_disk_image-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:21:29.849850 developer_disk_image-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-12 05:21:12.000000 developer_disk_image-0.0.2/tests/test_repo.py
```

### Comparing `developer_disk_image-0.0.1/PKG-INFO` & `developer_disk_image-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developer_disk_image
-Version: 0.0.1
+Version: 0.0.2
 Summary: Download DeveloperDiskImage ans Personalized images from GitHub
 Author-email: doronz88 <doron88@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>
 Project-URL: Homepage, https://github.com/doronz88/DeveloperDiskImage
 Project-URL: Bug Reports, https://github.com/doronz88/DeveloperDiskImage/issues
 Keywords: ios,DeveloperDiskImage
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,35 +15,37 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
+[![Pypi version](https://img.shields.io/pypi/v/developer_disk_image.svg)](https://pypi.org/project/developer_disk_image/ "PyPi package")
+
 # Overview
 
 Store both types of Apple's DeveloperDiskImage files:
 
 - `DeveloperDiskImage.dmg` & `DeveloperDiskImage.dmg.signature`
     - Used for each iOS version < 17.0
 - The new Personalized images, but splitted to:
     - APFS
     - `BuildManifest.plist`
     - Trustcache
 
-The split of the new format is requires for OS* other then macOS then will have trouble mounting the original APFS image
-inside: `~/Library/Developer/DeveloperDiskImages`.
+The split of the new format is requires for OS* other than macOS that will have trouble extracting the original APFS
+image inside: `~/Library/Developer/DeveloperDiskImages`.
 
 # Python package
 
 Additionally, this repo provides a python API for accessing this repository.
 You can install it as follows:
 
 ```shell
-python3 -m pip install developer_disk_image
+python3 -m pip install -U developer_disk_image
 ```
 
 ## Example usage
 
 ```python
 from developer_disk_image.repo import DeveloperDiskImageRepository
```

### Comparing `developer_disk_image-0.0.1/README.md` & `developer_disk_image-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+[![Pypi version](https://img.shields.io/pypi/v/developer_disk_image.svg)](https://pypi.org/project/developer_disk_image/ "PyPi package")
+
 # Overview
 
 Store both types of Apple's DeveloperDiskImage files:
 
 - `DeveloperDiskImage.dmg` & `DeveloperDiskImage.dmg.signature`
     - Used for each iOS version < 17.0
 - The new Personalized images, but splitted to:
     - APFS
     - `BuildManifest.plist`
     - Trustcache
 
-The split of the new format is requires for OS* other then macOS then will have trouble mounting the original APFS image
-inside: `~/Library/Developer/DeveloperDiskImages`.
+The split of the new format is requires for OS* other than macOS that will have trouble extracting the original APFS
+image inside: `~/Library/Developer/DeveloperDiskImages`.
 
 # Python package
 
 Additionally, this repo provides a python API for accessing this repository.
 You can install it as follows:
 
 ```shell
-python3 -m pip install developer_disk_image
+python3 -m pip install -U developer_disk_image
 ```
 
 ## Example usage
 
 ```python
 from developer_disk_image.repo import DeveloperDiskImageRepository
```

### Comparing `developer_disk_image-0.0.1/developer_disk_image/repo.py` & `developer_disk_image-0.0.2/developer_disk_image/repo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import base64
 import dataclasses
 import json
 from typing import Mapping, Optional
 
 import requests
 
+from developer_disk_image.exceptions import GithubRateLimitExceededError
+
 DEVELOPER_DISK_IMAGE_REPO_TREE_URL = \
     'https://api.github.com/repos/doronz88/DeveloperDiskImage/git/trees/main?recursive=true'
 
 
 @dataclasses.dataclass
 class DeveloperDiskImage:
     image: bytes
@@ -19,17 +21,17 @@
 class PersonalizedImage:
     image: bytes
     build_manifest: bytes
     trustcache: bytes
 
 
 class DeveloperDiskImageRepository:
-    @staticmethod
-    def create() -> 'DeveloperDiskImageRepository':
-        return DeveloperDiskImageRepository(json.loads(requests.get(DEVELOPER_DISK_IMAGE_REPO_TREE_URL).text)['tree'])
+    @classmethod
+    def create(cls) -> 'DeveloperDiskImageRepository':
+        return cls(cls._query(DEVELOPER_DISK_IMAGE_REPO_TREE_URL)['tree'])
 
     def __init__(self, tree: Mapping):
         self._path_urls = {}
         for node in tree:
             self._path_urls[node['path']] = node
 
     def get_developer_disk_image(self, version: str) -> Optional[DeveloperDiskImage]:
@@ -48,8 +50,15 @@
             'PersonalizedImages/Xcode_iOS_DDI_Personalized/Image.dmg.trustcache')
         return PersonalizedImage(image=image, build_manifest=build_manifest, trustcache=trustcache)
 
     def _get_blob(self, path: str) -> Optional[bytes]:
         url = self._path_urls.get(path, {}).get('url')
         if url is None:
             return None
-        return base64.b64decode(json.loads(requests.get(url).text)['content'])
+        return base64.b64decode(self._query(url)['content'])
+
+    @staticmethod
+    def _query(url: str) -> Mapping:
+        response = json.loads(requests.get(url).text)
+        if response.get('message', '').startswith('API rate limit exceeded'):
+            raise GithubRateLimitExceededError()
+        return response
```

### Comparing `developer_disk_image-0.0.1/developer_disk_image.egg-info/PKG-INFO` & `developer_disk_image-0.0.2/developer_disk_image.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: developer-disk-image
-Version: 0.0.1
+Version: 0.0.2
 Summary: Download DeveloperDiskImage ans Personalized images from GitHub
 Author-email: doronz88 <doron88@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>
 Project-URL: Homepage, https://github.com/doronz88/DeveloperDiskImage
 Project-URL: Bug Reports, https://github.com/doronz88/DeveloperDiskImage/issues
 Keywords: ios,DeveloperDiskImage
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,35 +15,37 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
+[![Pypi version](https://img.shields.io/pypi/v/developer_disk_image.svg)](https://pypi.org/project/developer_disk_image/ "PyPi package")
+
 # Overview
 
 Store both types of Apple's DeveloperDiskImage files:
 
 - `DeveloperDiskImage.dmg` & `DeveloperDiskImage.dmg.signature`
     - Used for each iOS version < 17.0
 - The new Personalized images, but splitted to:
     - APFS
     - `BuildManifest.plist`
     - Trustcache
 
-The split of the new format is requires for OS* other then macOS then will have trouble mounting the original APFS image
-inside: `~/Library/Developer/DeveloperDiskImages`.
+The split of the new format is requires for OS* other than macOS that will have trouble extracting the original APFS
+image inside: `~/Library/Developer/DeveloperDiskImages`.
 
 # Python package
 
 Additionally, this repo provides a python API for accessing this repository.
 You can install it as follows:
 
 ```shell
-python3 -m pip install developer_disk_image
+python3 -m pip install -U developer_disk_image
 ```
 
 ## Example usage
 
 ```python
 from developer_disk_image.repo import DeveloperDiskImageRepository
```

### Comparing `developer_disk_image-0.0.1/pyproject.toml` & `developer_disk_image-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "developer_disk_image"
-version = "0.0.1"
+version = "0.0.2"
 description = "Download DeveloperDiskImage ans Personalized images from GitHub"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["ios", "DeveloperDiskImage"]
 authors = [
     { name = "doronz88", email = "doron88@gmail.com" }
```


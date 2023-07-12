# Comparing `tmp/labkey-2.5.0.tar.gz` & `tmp/labkey-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labkey-2.5.0.tar", last modified: Thu Jul  6 20:36:04 2023, max compression
+gzip compressed data, was "labkey-2.5.1.tar", last modified: Wed Jul 12 18:53:29 2023, max compression
```

## Comparing `labkey-2.5.0.tar` & `labkey-2.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 alanvezina   (502) staff       (20)        0 2023-07-06 20:36:04.739961 labkey-2.5.0/
--rw-r--r--   0 alanvezina   (502) staff       (20)     9665 2023-07-06 20:35:36.000000 labkey-2.5.0/CHANGE.txt
--rw-r--r--   0 alanvezina   (502) staff       (20)    11358 2021-03-01 23:06:47.000000 labkey-2.5.0/LICENSE.txt
--rw-r--r--   0 alanvezina   (502) staff       (20)       62 2021-03-01 23:06:47.000000 labkey-2.5.0/MANIFEST.in
--rw-r--r--   0 alanvezina   (502) staff       (20)      892 2023-07-06 20:36:04.740110 labkey-2.5.0/PKG-INFO
--rw-r--r--   0 alanvezina   (502) staff       (20)     5713 2022-10-04 16:43:32.000000 labkey-2.5.0/README.md
--rw-r--r--   0 alanvezina   (502) staff       (20)     3084 2022-02-22 02:02:44.000000 labkey-2.5.0/download_file_example.txt
-drwxr-xr-x   0 alanvezina   (502) staff       (20)        0 2023-07-06 20:36:04.737418 labkey-2.5.0/labkey/
--rw-r--r--   0 alanvezina   (502) staff       (20)      695 2023-07-06 20:35:36.000000 labkey-2.5.0/labkey/__init__.py
--rw-r--r--   0 alanvezina   (502) staff       (20)     1351 2022-10-04 16:43:32.000000 labkey-2.5.0/labkey/api_wrapper.py
--rw-r--r--   0 alanvezina   (502) staff       (20)     5497 2023-07-06 20:35:36.000000 labkey-2.5.0/labkey/container.py
--rw-r--r--   0 alanvezina   (502) staff       (20)    22486 2022-05-11 22:16:02.000000 labkey-2.5.0/labkey/domain.py
--rw-r--r--   0 alanvezina   (502) staff       (20)     2929 2021-03-01 23:06:47.000000 labkey-2.5.0/labkey/exceptions.py
--rw-r--r--   0 alanvezina   (502) staff       (20)     8804 2021-05-12 17:28:18.000000 labkey-2.5.0/labkey/experiment.py
--rw-r--r--   0 alanvezina   (502) staff       (20)    17641 2022-06-27 21:06:06.000000 labkey-2.5.0/labkey/query.py
--rw-r--r--   0 alanvezina   (502) staff       (20)    15284 2021-05-12 17:28:18.000000 labkey-2.5.0/labkey/security.py
--rw-r--r--   0 alanvezina   (502) staff       (20)     6957 2022-10-24 16:02:28.000000 labkey-2.5.0/labkey/server_context.py
--rw-r--r--   0 alanvezina   (502) staff       (20)     6144 2023-07-06 19:01:12.000000 labkey-2.5.0/labkey/storage.py
--rw-r--r--   0 alanvezina   (502) staff       (20)     2651 2023-07-06 20:35:36.000000 labkey-2.5.0/labkey/utils.py
-drwxr-xr-x   0 alanvezina   (502) staff       (20)        0 2023-07-06 20:36:04.739621 labkey-2.5.0/labkey.egg-info/
--rw-r--r--   0 alanvezina   (502) staff       (20)      892 2023-07-06 20:36:04.000000 labkey-2.5.0/labkey.egg-info/PKG-INFO
--rw-r--r--   0 alanvezina   (502) staff       (20)      552 2023-07-06 20:36:04.000000 labkey-2.5.0/labkey.egg-info/SOURCES.txt
--rw-r--r--   0 alanvezina   (502) staff       (20)        1 2023-07-06 20:36:04.000000 labkey-2.5.0/labkey.egg-info/dependency_links.txt
--rw-r--r--   0 alanvezina   (502) staff       (20)       49 2023-07-06 20:36:04.000000 labkey-2.5.0/labkey.egg-info/requires.txt
--rw-r--r--   0 alanvezina   (502) staff       (20)        7 2023-07-06 20:36:04.000000 labkey-2.5.0/labkey.egg-info/top_level.txt
--rw-r--r--   0 alanvezina   (502) staff       (20)      450 2022-04-07 18:55:06.000000 labkey-2.5.0/lundbeck_file_download_notes.txt
--rw-r--r--   0 alanvezina   (502) staff       (20)     1114 2022-06-21 20:18:12.000000 labkey-2.5.0/perf_testing_notes.txt
--rw-r--r--   0 alanvezina   (502) staff       (20)     1785 2021-09-27 20:09:56.000000 labkey-2.5.0/playground.py.txt
--rw-r--r--   0 alanvezina   (502) staff       (20)       31 2021-03-01 23:06:47.000000 labkey-2.5.0/pyproject.toml
--rw-r--r--   0 alanvezina   (502) staff       (20)      161 2021-03-01 23:06:47.000000 labkey-2.5.0/pytest.ini
--rw-r--r--   0 alanvezina   (502) staff       (20)      193 2023-07-06 20:36:04.740734 labkey-2.5.0/setup.cfg
--rw-r--r--   0 alanvezina   (502) staff       (20)     2249 2021-03-01 23:06:47.000000 labkey-2.5.0/setup.py
+drwxr-xr-x   0 alanvezina   (502) staff       (20)        0 2023-07-12 18:53:29.986414 labkey-2.5.1/
+-rw-r--r--   0 alanvezina   (502) staff       (20)     9665 2023-07-06 20:35:36.000000 labkey-2.5.1/CHANGE.txt
+-rw-r--r--   0 alanvezina   (502) staff       (20)    11358 2021-03-01 23:06:47.000000 labkey-2.5.1/LICENSE.txt
+-rw-r--r--   0 alanvezina   (502) staff       (20)       62 2021-03-01 23:06:47.000000 labkey-2.5.1/MANIFEST.in
+-rw-r--r--   0 alanvezina   (502) staff       (20)      892 2023-07-12 18:53:29.986560 labkey-2.5.1/PKG-INFO
+-rw-r--r--   0 alanvezina   (502) staff       (20)     5713 2022-10-04 16:43:32.000000 labkey-2.5.1/README.md
+-rw-r--r--   0 alanvezina   (502) staff       (20)     3084 2022-02-22 02:02:44.000000 labkey-2.5.1/download_file_example.txt
+drwxr-xr-x   0 alanvezina   (502) staff       (20)        0 2023-07-12 18:53:29.983972 labkey-2.5.1/labkey/
+-rw-r--r--   0 alanvezina   (502) staff       (20)      695 2023-07-12 18:53:14.000000 labkey-2.5.1/labkey/__init__.py
+-rw-r--r--   0 alanvezina   (502) staff       (20)     1351 2022-10-04 16:43:32.000000 labkey-2.5.1/labkey/api_wrapper.py
+-rw-r--r--   0 alanvezina   (502) staff       (20)     5497 2023-07-06 20:35:36.000000 labkey-2.5.1/labkey/container.py
+-rw-r--r--   0 alanvezina   (502) staff       (20)    22486 2022-05-11 22:16:02.000000 labkey-2.5.1/labkey/domain.py
+-rw-r--r--   0 alanvezina   (502) staff       (20)     2929 2021-03-01 23:06:47.000000 labkey-2.5.1/labkey/exceptions.py
+-rw-r--r--   0 alanvezina   (502) staff       (20)     8804 2021-05-12 17:28:18.000000 labkey-2.5.1/labkey/experiment.py
+-rw-r--r--   0 alanvezina   (502) staff       (20)    17641 2022-06-27 21:06:06.000000 labkey-2.5.1/labkey/query.py
+-rw-r--r--   0 alanvezina   (502) staff       (20)    15284 2021-05-12 17:28:18.000000 labkey-2.5.1/labkey/security.py
+-rw-r--r--   0 alanvezina   (502) staff       (20)     6950 2023-07-12 18:53:14.000000 labkey-2.5.1/labkey/server_context.py
+-rw-r--r--   0 alanvezina   (502) staff       (20)     6144 2023-07-06 19:01:12.000000 labkey-2.5.1/labkey/storage.py
+-rw-r--r--   0 alanvezina   (502) staff       (20)     2651 2023-07-06 20:35:36.000000 labkey-2.5.1/labkey/utils.py
+drwxr-xr-x   0 alanvezina   (502) staff       (20)        0 2023-07-12 18:53:29.986115 labkey-2.5.1/labkey.egg-info/
+-rw-r--r--   0 alanvezina   (502) staff       (20)      892 2023-07-12 18:53:29.000000 labkey-2.5.1/labkey.egg-info/PKG-INFO
+-rw-r--r--   0 alanvezina   (502) staff       (20)      552 2023-07-12 18:53:29.000000 labkey-2.5.1/labkey.egg-info/SOURCES.txt
+-rw-r--r--   0 alanvezina   (502) staff       (20)        1 2023-07-12 18:53:29.000000 labkey-2.5.1/labkey.egg-info/dependency_links.txt
+-rw-r--r--   0 alanvezina   (502) staff       (20)       49 2023-07-12 18:53:29.000000 labkey-2.5.1/labkey.egg-info/requires.txt
+-rw-r--r--   0 alanvezina   (502) staff       (20)        7 2023-07-12 18:53:29.000000 labkey-2.5.1/labkey.egg-info/top_level.txt
+-rw-r--r--   0 alanvezina   (502) staff       (20)      450 2022-04-07 18:55:06.000000 labkey-2.5.1/lundbeck_file_download_notes.txt
+-rw-r--r--   0 alanvezina   (502) staff       (20)     1114 2022-06-21 20:18:12.000000 labkey-2.5.1/perf_testing_notes.txt
+-rw-r--r--   0 alanvezina   (502) staff       (20)     1785 2021-09-27 20:09:56.000000 labkey-2.5.1/playground.py.txt
+-rw-r--r--   0 alanvezina   (502) staff       (20)       31 2021-03-01 23:06:47.000000 labkey-2.5.1/pyproject.toml
+-rw-r--r--   0 alanvezina   (502) staff       (20)      161 2021-03-01 23:06:47.000000 labkey-2.5.1/pytest.ini
+-rw-r--r--   0 alanvezina   (502) staff       (20)      193 2023-07-12 18:53:29.987137 labkey-2.5.1/setup.cfg
+-rw-r--r--   0 alanvezina   (502) staff       (20)     2249 2021-03-01 23:06:47.000000 labkey-2.5.1/setup.py
```

### Comparing `labkey-2.5.0/CHANGE.txt` & `labkey-2.5.1/CHANGE.txt`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/LICENSE.txt` & `labkey-2.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/PKG-INFO` & `labkey-2.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labkey
-Version: 2.5.0
+Version: 2.5.1
 Summary: Python client API for LabKey Server
 Home-page: https://github.com/LabKey/labkey-api-python
 Author: LabKey
 Author-email: alanv@labkey.com
 Maintainer: Alan Vezina
 Maintainer-email: alanv@labkey.com
 License: Apache License 2.0
```

### Comparing `labkey-2.5.0/README.md` & `labkey-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/download_file_example.txt` & `labkey-2.5.1/download_file_example.txt`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/labkey/__init__.py` & `labkey-2.5.1/labkey/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __title__ = "labkey"
-__version__ = "2.5.0"
+__version__ = "2.5.1"
 __author__ = "LabKey"
 __license__ = "Apache License 2.0"
```

### Comparing `labkey-2.5.0/labkey/api_wrapper.py` & `labkey-2.5.1/labkey/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/labkey/container.py` & `labkey-2.5.1/labkey/container.py`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/labkey/domain.py` & `labkey-2.5.1/labkey/domain.py`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/labkey/exceptions.py` & `labkey-2.5.1/labkey/exceptions.py`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/labkey/experiment.py` & `labkey-2.5.1/labkey/experiment.py`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/labkey/query.py` & `labkey-2.5.1/labkey/query.py`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/labkey/security.py` & `labkey-2.5.1/labkey/security.py`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/labkey/server_context.py` & `labkey-2.5.1/labkey/server_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
         options = {
             "webdav_hostname": self.base_url,
         }
 
         if self._api_key is not None:
             options["webdav_login"] = "apikey"
-            options["webdav_password"] = f"apikey|{self._api_key}"
+            options["webdav_password"] = f"{self._api_key}"
 
         if webdav_options is not None:
             options = {
                 **options,
                 **webdav_options,
             }
```

### Comparing `labkey-2.5.0/labkey/storage.py` & `labkey-2.5.1/labkey/storage.py`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/labkey/utils.py` & `labkey-2.5.1/labkey/utils.py`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/labkey.egg-info/PKG-INFO` & `labkey-2.5.1/labkey.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labkey
-Version: 2.5.0
+Version: 2.5.1
 Summary: Python client API for LabKey Server
 Home-page: https://github.com/LabKey/labkey-api-python
 Author: LabKey
 Author-email: alanv@labkey.com
 Maintainer: Alan Vezina
 Maintainer-email: alanv@labkey.com
 License: Apache License 2.0
```

### Comparing `labkey-2.5.0/labkey.egg-info/SOURCES.txt` & `labkey-2.5.1/labkey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/perf_testing_notes.txt` & `labkey-2.5.1/perf_testing_notes.txt`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/playground.py.txt` & `labkey-2.5.1/playground.py.txt`

 * *Files identical despite different names*

### Comparing `labkey-2.5.0/setup.py` & `labkey-2.5.1/setup.py`

 * *Files identical despite different names*


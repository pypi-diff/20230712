# Comparing `tmp/tencentcloud-sdk-python-cpdp-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-cpdp-3.0.933.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cpdp-3.0.931.tar", last modified: Mon Jul 10 00:37:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cpdp-3.0.933.tar", last modified: Wed Jul 12 00:23:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cpdp-3.0.931.tar` & `tencentcloud-sdk-python-cpdp-3.0.933.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud_sdk_python_cpdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud_sdk_python_cpdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud_sdk_python_cpdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud_sdk_python_cpdp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud/cpdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud/cpdp/v20190820/
--rw-r--r--   0 root         (0) root         (0)    19183 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud/cpdp/v20190820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  2040467 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud/cpdp/v20190820/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud/cpdp/v20190820/__init__.py
--rw-r--r--   0 root         (0) root         (0)   210732 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud/cpdp/v20190820/cpdp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud/cpdp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:37:40.000000 tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud/cpdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud/cpdp/v20190820/
+-rw-r--r--   0 root         (0) root         (0)   210732 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud/cpdp/v20190820/cpdp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud/cpdp/v20190820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19183 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud/cpdp/v20190820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  2040467 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud/cpdp/v20190820/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud/cpdp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud_sdk_python_cpdp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud_sdk_python_cpdp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud_sdk_python_cpdp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:23:53.000000 tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud_sdk_python_cpdp.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.931/setup.py` & `tencentcloud-sdk-python-cpdp-3.0.933/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-cpdp-3.0.933/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cpdp
-Version: 3.0.931
+Version: 3.0.933
 Summary: Tencent Cloud Cpdp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cpdp
-Version: 3.0.931
+Version: 3.0.933
 Summary: Tencent Cloud Cpdp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.931/README.rst` & `tencentcloud-sdk-python-cpdp-3.0.933/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud/cpdp/v20190820/errorcodes.py` & `tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud/cpdp/v20190820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud/cpdp/v20190820/models.py` & `tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud/cpdp/v20190820/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud/cpdp/v20190820/cpdp_client.py` & `tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud/cpdp/v20190820/cpdp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cpdp-3.0.933/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.931'
+__version__ = '3.0.933'
```


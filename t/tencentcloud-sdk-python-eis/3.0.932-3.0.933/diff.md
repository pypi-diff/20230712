# Comparing `tmp/tencentcloud-sdk-python-eis-3.0.932.tar.gz` & `tmp/tencentcloud-sdk-python-eis-3.0.933.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-eis-3.0.932.tar", last modified: Tue Jul 11 00:43:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-eis-3.0.933.tar", last modified: Wed Jul 12 00:29:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-eis-3.0.932.tar` & `tencentcloud-sdk-python-eis-3.0.933.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud_sdk_python_eis.egg-info/
--rw-r--r--   0 root         (0) root         (0)      603 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud_sdk_python_eis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud_sdk_python_eis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud_sdk_python_eis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20200715/
--rw-r--r--   0 root         (0) root         (0)     1197 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20200715/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    17929 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20200715/models.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20200715/eis_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20200715/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20210601/
--rw-r--r--   0 root         (0) root         (0)     2977 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20210601/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    39966 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20210601/models.py
--rw-r--r--   0 root         (0) root         (0)     5846 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20210601/eis_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:09.000000 tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20210601/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud_sdk_python_eis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud_sdk_python_eis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud_sdk_python_eis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud_sdk_python_eis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20210601/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20210601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5846 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20210601/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20210601/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    39966 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20210601/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20200715/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20200715/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20200715/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20200715/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    17929 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20200715/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:29:29.000000 tencentcloud-sdk-python-eis-3.0.933/README.rst
```

### Comparing `tencentcloud-sdk-python-eis-3.0.932/setup.py` & `tencentcloud-sdk-python-eis-3.0.933/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.932/PKG-INFO` & `tencentcloud-sdk-python-eis-3.0.933/tencentcloud_sdk_python_eis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eis
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Eis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eis-3.0.932/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-eis-3.0.933/tencentcloud_sdk_python_eis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.932/tencentcloud_sdk_python_eis.egg-info/PKG-INFO` & `tencentcloud-sdk-python-eis-3.0.933/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-eis
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Eis SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-eis-3.0.932/README.rst` & `tencentcloud-sdk-python-eis-3.0.933/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.932/tencentcloud/__init__.py` & `tencentcloud-sdk-python-eis-3.0.933/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.932'
+__version__ = '3.0.933'
```

### Comparing `tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20200715/errorcodes.py` & `tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20200715/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20200715/models.py` & `tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20200715/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20200715/eis_client.py` & `tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20200715/eis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20210601/errorcodes.py` & `tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20210601/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20210601/models.py` & `tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20210601/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-eis-3.0.932/tencentcloud/eis/v20210601/eis_client.py` & `tencentcloud-sdk-python-eis-3.0.933/tencentcloud/eis/v20210601/eis_client.py`

 * *Files identical despite different names*


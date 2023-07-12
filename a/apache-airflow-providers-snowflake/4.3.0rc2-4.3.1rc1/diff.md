# Comparing `tmp/apache-airflow-providers-snowflake-4.3.0rc2.tar.gz` & `tmp/apache-airflow-providers-snowflake-4.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-snowflake-4.3.0rc2.tar", last modified: Thu Jul  6 04:51:33 2023, max compression
+gzip compressed data, was "apache-airflow-providers-snowflake-4.3.1rc1.tar", last modified: Wed Jul 12 19:13:35 2023, max compression
```

## Comparing `apache-airflow-providers-snowflake-4.3.0rc2.tar` & `apache-airflow-providers-snowflake-4.3.1rc1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.382175 apache-airflow-providers-snowflake-4.3.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:51:32.000000 apache-airflow-providers-snowflake-4.3.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5873 2023-07-06 04:51:33.382708 apache-airflow-providers-snowflake-4.3.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4174 2023-07-06 04:51:32.000000 apache-airflow-providers-snowflake-4.3.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.267934 apache-airflow-providers-snowflake-4.3.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.269026 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.309311 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-07-06 04:42:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4949 2023-07-06 04:51:32.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.319211 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17859 2023-06-05 12:50:36.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/snowflake.py
--rw-r--r--   0 root         (0) root         (0)    12676 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/snowflake_sql_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.325917 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24666 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.338441 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5786 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/s3_to_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     5078 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/snowflake_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.344467 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4306 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/snowflake_trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.354559 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/common.py
--rw-r--r--   0 root         (0) root         (0)     6878 2023-06-01 07:44:14.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.379560 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5873 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1299 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      227 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-snowflake-4.3.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2059 2023-07-06 04:51:33.384605 apache-airflow-providers-snowflake-4.3.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1789 2023-07-06 04:51:32.000000 apache-airflow-providers-snowflake-4.3.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.488646 apache-airflow-providers-snowflake-4.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-12 19:13:34.000000 apache-airflow-providers-snowflake-4.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5873 2023-07-12 19:13:35.489212 apache-airflow-providers-snowflake-4.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4174 2023-07-12 19:13:34.000000 apache-airflow-providers-snowflake-4.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.381882 apache-airflow-providers-snowflake-4.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.383080 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.419481 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-07-12 19:08:31.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4970 2023-07-12 19:13:34.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.428181 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18283 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)    12677 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.437071 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24724 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/operators/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.448706 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5765 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     5083 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.454531 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.462898 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/common.py
+-rw-r--r--   0 root         (0) root         (0)     6889 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:35.486050 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5873 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:13:35.000000 apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-snowflake-4.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-07-12 19:13:35.491041 apache-airflow-providers-snowflake-4.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-07-12 19:13:34.000000 apache-airflow-providers-snowflake-4.3.1rc1/setup.py
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/LICENSE` & `apache-airflow-providers-snowflake-4.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/MANIFEST.in` & `apache-airflow-providers-snowflake-4.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/PKG-INFO` & `apache-airflow-providers-snowflake-4.3.1rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.3.0rc2
+Version: 4.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -68,28 +68,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.3.0rc2``
+Release: ``4.3.1rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -126,8 +126,8 @@
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 `apache-airflow-providers-slack <https://airflow.apache.org/docs/apache-airflow-providers-slack>`_            ``slack``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/README.rst` & `apache-airflow-providers-snowflake-4.3.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.3.0rc2``
+Release: ``4.3.1rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -90,8 +90,8 @@
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 `apache-airflow-providers-slack <https://airflow.apache.org/docs/apache-airflow-providers-slack>`_            ``slack``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/__init__.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.3.0"
+__version__ = "4.3.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/get_provider_info.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-snowflake",
         "name": "Snowflake",
         "description": "`Snowflake <https://www.snowflake.com/>`__\n",
         "suspended": False,
         "versions": [
+            "4.3.1",
             "4.3.0",
             "4.2.0",
             "4.1.0",
             "4.0.5",
             "4.0.4",
             "4.0.3",
             "4.0.2",
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/__init__.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/snowflake.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files 4% similar despite different names*

```diff
@@ -244,15 +244,20 @@
         private_key_pem = None
         if private_key_content and private_key_file:
             raise AirflowException(
                 "The private_key_file and private_key_content extra fields are mutually exclusive. "
                 "Please remove one."
             )
         elif private_key_file:
-            private_key_pem = Path(private_key_file).read_bytes()
+            private_key_file_path = Path(private_key_file)
+            if not private_key_file_path.is_file() or private_key_file_path.stat().st_size == 0:
+                raise ValueError("The private_key_file path points to an empty or invalid file.")
+            if private_key_file_path.stat().st_size > 4096:
+                raise ValueError("The private_key_file size is too big. Please keep it less than 4 KB.")
+            private_key_pem = Path(private_key_file_path).read_bytes()
         elif private_key_content:
             private_key_pem = private_key_content.encode()
 
         if private_key_pem:
             passphrase = None
             if conn.password:
                 passphrase = conn.password.strip().encode()
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/snowflake_sql_api.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 from airflow import AirflowException
 from airflow.providers.snowflake.hooks.snowflake import SnowflakeHook
 from airflow.providers.snowflake.utils.sql_api_generate_jwt import JWTGenerator
 
 
 class SnowflakeSqlApiHook(SnowflakeHook):
     """
-    A client to interact with Snowflake using SQL API  and allows submitting
-    multiple SQL statements in a single request. In combination with aiohttp, make post request to submit SQL
-    statements for execution, poll to check the status of the execution of a statement. Fetch query results
-    asynchronously.
+    A client to interact with Snowflake using SQL API and submit multiple SQL statements in a single request.
+
+    In combination with aiohttp, make post request to submit SQL statements for execution,
+    poll to check the status of the execution of a statement. Fetch query results asynchronously.
 
     This hook requires the snowflake_conn_id connection. This hooks mainly uses account, schema, database,
      warehouse, private_key_file or private_key_content field must be setup in the connection. Other inputs
       can be defined in the connection or hook instantiation.
 
     :param snowflake_conn_id: Reference to
         :ref:`Snowflake connection id<howto/connection:snowflake>`
@@ -133,15 +133,18 @@
         :param bindings: (Optional) Values of bind variables in the SQL statement.
             When executing the statement, Snowflake replaces placeholders (? and :name) in
             the statement with these specified values.
         """
         conn_config = self._get_conn_params()
 
         req_id = uuid.uuid4()
-        url = f"https://{conn_config['account']}.{conn_config['region']}.snowflakecomputing.com/api/v2/statements"
+        url = (
+            f"https://{conn_config['account']}.{conn_config['region']}"
+            f".snowflakecomputing.com/api/v2/statements"
+        )
         params: dict[str, Any] | None = {"requestId": str(req_id), "async": True, "pageSize": 10}
         headers = self.get_headers()
         if bindings is None:
             bindings = {}
         data = {
             "statement": sql,
             "resultSetMetaData": {"format": "json"},
@@ -167,17 +170,15 @@
         elif "statementHandle" in json_response:
             self.query_ids.append(json_response["statementHandle"])
         else:
             raise AirflowException("No statementHandle/statementHandles present in response")
         return self.query_ids
 
     def get_headers(self) -> dict[str, Any]:
-        """Based on the private key, and with connection details JWT Token is generated and header
-        is formed.
-        """
+        """Form JWT Token and header based on the private key, and connection details."""
         if not self.private_key:
             self.get_private_key()
         conn_config = self._get_conn_params()
 
         # Get the JWT token from the connection details and the private key
         token = JWTGenerator(
             conn_config["account"],  # type: ignore[arg-type]
@@ -202,21 +203,23 @@
 
         :param query_id: statement handles query ids for the individual statements.
         """
         conn_config = self._get_conn_params()
         req_id = uuid.uuid4()
         header = self.get_headers()
         params = {"requestId": str(req_id)}
-        url = f"https://{conn_config['account']}.{conn_config['region']}.snowflakecomputing.com/api/v2/statements/{query_id}"
+        url = (
+            f"https://{conn_config['account']}.{conn_config['region']}"
+            f".snowflakecomputing.com/api/v2/statements/{query_id}"
+        )
         return header, params, url
 
     def check_query_output(self, query_ids: list[str]) -> None:
         """
-        Based on the query ids passed as the parameter make HTTP request to snowflake SQL API and logs
-        the response.
+        Make HTTP request to snowflake SQL API based on the provided query ids and log the response.
 
         :param query_ids: statement handles query id for the individual statements.
         """
         for query_id in query_ids:
             header, params, url = self.get_request_url_header_params(query_id)
             try:
                 response = requests.get(url, headers=header, params=params)
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/__init__.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/snowflake.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/operators/snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,24 +19,23 @@
 
 import time
 import warnings
 from datetime import timedelta
 from typing import TYPE_CHECKING, Any, Iterable, List, Mapping, Sequence, SupportsAbs, cast
 
 from airflow import AirflowException
+from airflow.configuration import conf
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.common.sql.operators.sql import (
     SQLCheckOperator,
     SQLExecuteQueryOperator,
     SQLIntervalCheckOperator,
     SQLValueCheckOperator,
 )
-from airflow.providers.snowflake.hooks.snowflake_sql_api import (
-    SnowflakeSqlApiHook,
-)
+from airflow.providers.snowflake.hooks.snowflake_sql_api import SnowflakeSqlApiHook
 from airflow.providers.snowflake.triggers.snowflake_trigger import SnowflakeSqlApiTrigger
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SnowflakeOperator(SQLExecuteQueryOperator):
@@ -131,18 +130,19 @@
                 current_processed_result.append(dict_result)
             returned_results.append(current_processed_result)
         return returned_results
 
 
 class SnowflakeCheckOperator(SQLCheckOperator):
     """
-    Performs a check against Snowflake. The ``SnowflakeCheckOperator`` expects
-    a sql query that will return a single row. Each value on that
-    first row is evaluated using python ``bool`` casting. If any of the
-    values return ``False`` the check is failed and errors out.
+    Performs a check against Snowflake.
+
+    The ``SnowflakeCheckOperator`` expects a sql query that will return a single row. Each
+    value on that first row is evaluated using python ``bool`` casting. If any of the values
+    return ``False`` the check is failed and errors out.
 
     Note that Python bool casting evals the following as ``False``:
 
     * ``False``
     * ``0``
     * Empty string (``""``)
     * Empty list (``[]``)
@@ -221,16 +221,15 @@
         self.authenticator = authenticator
         self.session_parameters = session_parameters
         self.query_ids: list[str] = []
 
 
 class SnowflakeValueCheckOperator(SQLValueCheckOperator):
     """
-    Performs a simple check using sql code against a specified value, within a
-    certain level of tolerance.
+    Performs a simple check using sql code against a specified value, within a certain level of tolerance.
 
     :param sql: the sql to be executed
     :param pass_value: the value to check against
     :param tolerance: (optional) the tolerance allowed to accept the query as
         passing
     :param snowflake_conn_id: Reference to
         :ref:`Snowflake connection id<howto/connection:snowflake>`
@@ -289,16 +288,15 @@
         self.authenticator = authenticator
         self.session_parameters = session_parameters
         self.query_ids: list[str] = []
 
 
 class SnowflakeIntervalCheckOperator(SQLIntervalCheckOperator):
     """
-    Checks that the values of metrics given as SQL expressions are within
-    a certain tolerance of the ones from days_back before.
+    Checks that the metrics given as SQL expressions are within tolerance of the ones from days_back before.
 
     This method constructs a query like so ::
 
         SELECT {metrics_threshold_dict_key} FROM {table}
         WHERE {date_filter_column}=<date>
 
     :param table: the table name
@@ -448,15 +446,15 @@
         authenticator: str | None = None,
         session_parameters: dict[str, Any] | None = None,
         poll_interval: int = 5,
         statement_count: int = 0,
         token_life_time: timedelta = LIFETIME,
         token_renewal_delta: timedelta = RENEWAL_DELTA,
         bindings: dict[str, Any] | None = None,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs: Any,
     ) -> None:
         self.snowflake_conn_id = snowflake_conn_id
         self.poll_interval = poll_interval
         self.statement_count = statement_count
         self.token_life_time = token_life_time
         self.token_renewal_delta = token_renewal_delta
@@ -475,14 +473,15 @@
                 **hook_params,
             }
         super().__init__(conn_id=snowflake_conn_id, **kwargs)  # pragma: no cover
 
     def execute(self, context: Context) -> None:
         """
         Make a POST API request to snowflake by using SnowflakeSQL and execute the query to get the ids.
+
         By deferring the SnowflakeSqlApiTrigger class passed along with query ids.
         """
         self.log.info("Executing: %s", self.sql)
         self._hook = SnowflakeSqlApiHook(
             snowflake_conn_id=self.snowflake_conn_id,
             token_life_time=self.token_life_time,
             token_renewal_delta=self.token_renewal_delta,
@@ -535,16 +534,16 @@
                 queries_in_progress.remove(query_id)
             time.sleep(self.poll_interval)
         return {"success": statement_success_status, "error": statement_error_status}
 
     def execute_complete(self, context: Context, event: dict[str, str | list[str]] | None = None) -> None:
         """
         Callback for when the trigger fires - returns immediately.
-        Relies on trigger to throw an exception, otherwise it assumes execution was
-        successful.
+
+        Relies on trigger to throw an exception, otherwise it assumes execution was successful.
         """
         if event:
             if "status" in event and event["status"] == "error":
                 msg = f"{event['status']}: {event['message']}"
                 raise AirflowException(msg)
             elif "status" in event and event["status"] == "success":
                 hook = SnowflakeSqlApiHook(snowflake_conn_id=self.snowflake_conn_id)
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/__init__.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""
-This module contains abstract operator that child classes
-implement "COPY INTO <TABLE> SQL in Snowflake".
-"""
+"""Abstract operator that child classes implement ``COPY INTO <TABLE> SQL in Snowflake``."""
 from __future__ import annotations
 
 from typing import Any, Sequence
 
 from airflow.models import BaseOperator
 from airflow.providers.snowflake.hooks.snowflake import SnowflakeHook
 from airflow.providers.snowflake.utils.common import enclose_param
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/s3_to_snowflake.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/snowflake_to_slack.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,20 +21,22 @@
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.slack.transfers.sql_to_slack import SqlToSlackOperator
 
 
 class SnowflakeToSlackOperator(SqlToSlackOperator):
     """
-    Executes an SQL statement in Snowflake and sends the results to Slack. The results of the query are
-    rendered into the 'slack_message' parameter as a Pandas dataframe using a JINJA variable called '{{
-    results_df }}'. The 'results_df' variable name can be changed by specifying a different
-    'results_df_name' parameter. The Tabulate library is added to the JINJA environment as a filter to
-    allow the dataframe to be rendered nicely. For example, set 'slack_message' to {{ results_df |
-    tabulate(tablefmt="pretty", headers="keys") }} to send the results to Slack as an ascii rendered table.
+    Executes an SQL statement in Snowflake and sends the results to Slack.
+
+    The results of the query are rendered into the 'slack_message' parameter as a Pandas dataframe
+    using a Jinja variable called '{{ results_df }}'. The 'results_df' variable name can be changed
+    by specifying a different 'results_df_name' parameter. The Tabulate library is added to the
+    Jinja environment as a filter to allow the dataframe to be rendered nicely. For example, set
+    'slack_message' to {{ results_df | tabulate(tablefmt="pretty", headers="keys") }} to send the
+    results to Slack as an ASCII rendered table.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SnowflakeToSlackOperator`
 
     :param sql: The SQL statement to execute on Snowflake (templated)
     :param slack_message: The templated Slack message to send with the data returned from Snowflake.
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/__init__.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/snowflake_trigger.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,19 +89,15 @@
                     "statement_query_ids": statement_query_ids,
                 }
             )
         except Exception as e:
             yield TriggerEvent({"status": "error", "message": str(e)})
 
     async def get_query_status(self, query_id: str) -> dict[str, Any]:
-        """
-        Async function to check whether the query statement submitted via SQL API is still
-        running state and returns True if it is still running else
-        return False.
-        """
+        """Return True if the SQL query is still running otherwise return False."""
         hook = SnowflakeSqlApiHook(
             self.snowflake_conn_id,
             self.token_life_time,
             self.token_renewal_delta,
         )
         return await hook.get_sql_api_query_status_async(query_id)
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/__init__.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/common.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/sql_api_generate_jwt.py` & `apache-airflow-providers-snowflake-4.3.1rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 # the passphrase for decrypting your private key. As an example, this function
 # prompts the user for the passphrase.
 
 
 class JWTGenerator:
     """
     Creates and signs a JWT with the specified private key file, username, and account identifier.
+
     The JWTGenerator keeps the generated token and only regenerates the token if a specified period
     of time has passed.
 
     Creates an object that generates JWTs for the specified user, account identifier, and private key
 
     :param account: Your Snowflake account identifier.
         See https://docs.snowflake.com/en/user-guide/admin-account-identifier.html. Note that if you are using
@@ -88,14 +89,15 @@
         self.private_key = private_key
         self.renew_time = datetime.now(timezone.utc)
         self.token: str | None = None
 
     def prepare_account_name_for_jwt(self, raw_account: str) -> str:
         """
         Prepare the account identifier for use in the JWT.
+
         For the JWT, the account identifier must not include the subdomain or any region or cloud provider
         information.
 
         :param raw_account: The specified account identifier.
         """
         account = raw_account
         if ".global" not in account:
@@ -109,15 +111,17 @@
             if idx > 0:
                 account = account[0:idx]  # pragma: no cover
         # Use uppercase for the account identifier.
         return account.upper()
 
     def get_token(self) -> str | None:
         """
-        Generates a new JWT. If a JWT has been already been generated earlier, return the previously
+        Generates a new JWT.
+
+        If a JWT has been already been generated earlier, return the previously
         generated token unless the specified renewal time has passed.
         """
         now = datetime.now(timezone.utc)  # Fetch the current time
 
         # If the token has expired or doesn't exist, regenerate the token.
         if self.token is None or self.renew_time <= now:
             logger.info(
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/PKG-INFO` & `apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.3.0rc2
+Version: 4.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -68,28 +68,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.3.0rc2``
+Release: ``4.3.1rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -126,8 +126,8 @@
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 `apache-airflow-providers-slack <https://airflow.apache.org/docs/apache-airflow-providers-slack>`_            ``slack``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/SOURCES.txt` & `apache-airflow-providers-snowflake-4.3.1rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/pyproject.toml` & `apache-airflow-providers-snowflake-4.3.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/setup.cfg` & `apache-airflow-providers-snowflake-4.3.1rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.1/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -56,10 +56,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.snowflake.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.snowflake
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-snowflake-4.3.0rc2/setup.py` & `apache-airflow-providers-snowflake-4.3.1rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-snowflake package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.3.0"
+version = "4.3.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-snowflake setup."""
     setup(
         version=version,
         extras_require={
```


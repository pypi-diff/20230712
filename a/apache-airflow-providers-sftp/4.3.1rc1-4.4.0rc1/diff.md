# Comparing `tmp/apache-airflow-providers-sftp-4.3.1rc1.tar.gz` & `tmp/apache-airflow-providers-sftp-4.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sftp-4.3.1rc1.tar", last modified: Tue Jun 20 11:43:08 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sftp-4.4.0rc1.tar", last modified: Wed Jul 12 19:13:33 2023, max compression
```

## Comparing `apache-airflow-providers-sftp-4.3.1rc1.tar` & `apache-airflow-providers-sftp-4.4.0rc1.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.517921 apache-airflow-providers-sftp-4.3.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.3.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:07.000000 apache-airflow-providers-sftp-4.3.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.3.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14383 2023-06-20 11:43:08.518966 apache-airflow-providers-sftp-4.3.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12841 2023-06-20 11:43:07.000000 apache-airflow-providers-sftp-4.3.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.433826 apache-airflow-providers-sftp-4.3.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.434921 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.468802 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3055 2023-06-20 11:43:07.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.474511 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14745 2023-06-05 12:50:36.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/hooks/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.481711 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8461 2023-06-02 11:31:21.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/operators/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.490618 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3543 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/sensors/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.515320 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14383 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      768 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-sftp-4.3.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1859 2023-06-20 11:43:08.521036 apache-airflow-providers-sftp-4.3.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1665 2023-06-20 11:43:07.000000 apache-airflow-providers-sftp-4.3.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.597969 apache-airflow-providers-sftp-4.4.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.4.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-12 19:13:32.000000 apache-airflow-providers-sftp-4.4.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.4.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5472 2023-07-12 19:13:33.598522 apache-airflow-providers-sftp-4.4.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3822 2023-07-12 19:13:32.000000 apache-airflow-providers-sftp-4.4.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.504568 apache-airflow-providers-sftp-4.4.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.505728 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.546449 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-07-12 19:08:31.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.549508 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.555289 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-07-12 19:13:32.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.560953 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14745 2023-06-05 12:50:36.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.566531 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8458 2023-07-06 04:42:33.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/operators/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.572295 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.595702 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5472 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      918 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-sftp-4.4.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-07-12 19:13:33.600765 apache-airflow-providers-sftp-4.4.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-12 19:13:32.000000 apache-airflow-providers-sftp-4.4.0rc1/setup.py
```

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/LICENSE` & `apache-airflow-providers-sftp-4.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/MANIFEST.in` & `apache-airflow-providers-sftp-4.4.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/__init__.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.3.1"
+__version__ = "4.4.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/get_provider_info.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/get_provider_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-sftp",
         "name": "SFTP",
         "description": "`SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__\n",
         "suspended": False,
         "versions": [
+            "4.4.0",
             "4.3.1",
             "4.3.0",
             "4.2.4",
             "4.2.3",
             "4.2.2",
             "4.2.1",
             "4.2.0",
@@ -69,20 +70,29 @@
                 "integration-name": "SSH File Transfer Protocol (SFTP)",
                 "python-modules": ["airflow.providers.sftp.operators.sftp"],
             }
         ],
         "sensors": [
             {
                 "integration-name": "SSH File Transfer Protocol (SFTP)",
-                "python-modules": ["airflow.providers.sftp.sensors.sftp"],
+                "python-modules": [
+                    "airflow.providers.sftp.sensors.sftp",
+                    "airflow.providers.sftp.decorators.sensors.sftp",
+                ],
             }
         ],
         "hooks": [
             {
                 "integration-name": "SSH File Transfer Protocol (SFTP)",
                 "python-modules": ["airflow.providers.sftp.hooks.sftp"],
             }
         ],
         "connection-types": [
             {"hook-class-name": "airflow.providers.sftp.hooks.sftp.SFTPHook", "connection-type": "sftp"}
         ],
+        "task-decorators": [
+            {
+                "class-name": "airflow.providers.sftp.decorators.sensors.sftp.sftp_sensor_task",
+                "name": "sftp_sensor",
+            }
+        ],
     }
```

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/hooks/__init__.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/hooks/sftp.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/operators/__init__.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/operators/sftp.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/operators/sftp.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     PUT = "put"
     GET = "get"
 
 
 class SFTPOperator(BaseOperator):
     """
     SFTPOperator for transferring files from remote host to local or vice a versa.
-    This operator uses sftp_hook to open sftp transport channel that serve as basis
-    for file transfer.
+
+    This operator uses sftp_hook to open sftp transport channel that serve as basis for file transfer.
 
     :param ssh_conn_id: :ref:`ssh connection id<howto/connection:ssh>`
         from airflow Connections. `ssh_conn_id` will be ignored if `ssh_hook`
         or `sftp_hook` is provided.
     :param sftp_hook: predefined SFTPHook to use
         Either `sftp_hook` or `ssh_conn_id` needs to be provided.
     :param ssh_hook: Deprecated - predefined SSHHook to use for remote execution
```

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/sensors/__init__.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/sensors/sftp.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/sftp.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 # specific language governing permissions and limitations
 # under the License.
 """This module contains SFTP sensor."""
 from __future__ import annotations
 
 import os
 from datetime import datetime
-from typing import TYPE_CHECKING, Sequence
+from typing import TYPE_CHECKING, Any, Callable, Sequence
 
 from paramiko.sftp import SFTP_NO_SUCH_FILE
 
 from airflow.providers.sftp.hooks.sftp import SFTPHook
-from airflow.sensors.base import BaseSensorOperator
+from airflow.sensors.base import BaseSensorOperator, PokeReturnValue
 from airflow.utils.timezone import convert_to_utc
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SFTPSensor(BaseSensorOperator):
@@ -50,26 +50,33 @@
     def __init__(
         self,
         *,
         path: str,
         file_pattern: str = "",
         newer_than: datetime | None = None,
         sftp_conn_id: str = "sftp_default",
+        python_callable: Callable | None = None,
+        op_args: list | None = None,
+        op_kwargs: dict[str, Any] | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.path = path
         self.file_pattern = file_pattern
         self.hook: SFTPHook | None = None
         self.sftp_conn_id = sftp_conn_id
         self.newer_than: datetime | None = newer_than
+        self.python_callable: Callable | None = python_callable
+        self.op_args = op_args or []
+        self.op_kwargs = op_kwargs or {}
 
-    def poke(self, context: Context) -> bool:
+    def poke(self, context: Context) -> PokeReturnValue | bool:
         self.hook = SFTPHook(self.sftp_conn_id)
         self.log.info("Poking for %s, with pattern %s", self.path, self.file_pattern)
+        files_found = []
 
         if self.file_pattern:
             files_from_pattern = self.hook.get_files_by_pattern(self.path, self.file_pattern)
             if files_from_pattern:
                 actual_files_to_check = [
                     os.path.join(self.path, file_from_pattern) for file_from_pattern in files_from_pattern
                 ]
@@ -85,12 +92,22 @@
                 if e.errno != SFTP_NO_SUCH_FILE:
                     raise e
                 continue
             if self.newer_than:
                 _mod_time = convert_to_utc(datetime.strptime(mod_time, "%Y%m%d%H%M%S"))
                 _newer_than = convert_to_utc(self.newer_than)
                 if _newer_than <= _mod_time:
-                    return True
+                    files_found.append(actual_file_to_check)
             else:
-                return True
+                files_found.append(actual_file_to_check)
         self.hook.close_conn()
-        return False
+        if not len(files_found):
+            return False
+        if self.python_callable is not None:
+            if self.op_kwargs:
+                self.op_kwargs["files_found"] = files_found
+            callable_return = self.python_callable(*self.op_args, **self.op_kwargs)
+            return PokeReturnValue(
+                is_done=True,
+                xcom_value={"files_found": files_found, "decorator_return_value": callable_return},
+            )
+        return True
```

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/SOURCES.txt` & `apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 NOTICE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 airflow/providers/sftp/__init__.py
 airflow/providers/sftp/get_provider_info.py
+airflow/providers/sftp/decorators/__init__.py
+airflow/providers/sftp/decorators/sensors/__init__.py
+airflow/providers/sftp/decorators/sensors/sftp.py
 airflow/providers/sftp/hooks/__init__.py
 airflow/providers/sftp/hooks/sftp.py
 airflow/providers/sftp/operators/__init__.py
 airflow/providers/sftp/operators/sftp.py
 airflow/providers/sftp/sensors/__init__.py
 airflow/providers/sftp/sensors/sftp.py
 apache_airflow_providers_sftp.egg-info/PKG-INFO
```

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/pyproject.toml` & `apache-airflow-providers-sftp-4.4.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 [tool.black]
 line-length = 110
 target-version = ['py37', 'py38', 'py39', 'py310']
-# The build system section is needed in order to workaround the side-effect introduced by recent
-# setup tools version. The recent setuptools version update (64.0.0) broke paths of editable installations
-# and we have to pin it to 63.4.3 version
-# The problem is tracked (and this limitation might be removed if it is solved) in:
-# https://github.com/pypa/setuptools/issues/3548
+
+# Editable installs are currently broken using setuptools 64.0.0 and above. The problem is tracked in
+# https://github.com/pypa/setuptools/issues/3548. We're also discussing how we could potentially fix
+# this problem on our end in issue https://github.com/apache/airflow/issues/30764. Until then we need
+# to use one of the following workarounds locally for editable installs:
+# 1) Pin setuptools <= 63.4.3 below in the [build-system] section.
+# 2) Include your airflow source code directory in PYTHONPATH.
 [build-system]
 requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">=3.8"
```

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/setup.cfg` & `apache-airflow-providers-sftp-4.4.0rc1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.3.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-sftp-4.3.1rc1/setup.py` & `apache-airflow-providers-sftp-4.4.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-sftp package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.3.1"
+version = "4.4.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-sftp setup."""
     setup(
         version=version,
         extras_require={"ssh": ["apache-airflow-providers-ssh"]},
```


# Comparing `tmp/apache-airflow-providers-http-4.4.2rc1.tar.gz` & `tmp/apache-airflow-providers-http-4.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-http-4.4.2rc1.tar", last modified: Tue Jun 20 11:42:18 2023, max compression
+gzip compressed data, was "apache-airflow-providers-http-4.5.0rc1.tar", last modified: Wed Jul 12 19:13:29 2023, max compression
```

## Comparing `apache-airflow-providers-http-4.4.2rc1.tar` & `apache-airflow-providers-http-4.5.0rc1.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.277746 apache-airflow-providers-http-4.4.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-http-4.4.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:17.000000 apache-airflow-providers-http-4.4.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-http-4.4.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12757 2023-06-20 11:42:18.278886 apache-airflow-providers-http-4.4.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11235 2023-06-20 11:42:17.000000 apache-airflow-providers-http-4.4.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.184744 apache-airflow-providers-http-4.4.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.185980 apache-airflow-providers-http-4.4.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.228034 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3088 2023-06-20 11:42:17.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.234411 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16171 2023-06-05 12:50:36.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/hooks/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.241051 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5829 2023-06-02 11:31:21.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/operators/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.247280 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5885 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/sensors/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.275094 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12757 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      768 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       78 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-http-4.4.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1872 2023-06-20 11:42:18.280969 apache-airflow-providers-http-4.4.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-06-20 11:42:17.000000 apache-airflow-providers-http-4.4.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.266460 apache-airflow-providers-http-4.5.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-http-4.5.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-12 19:13:28.000000 apache-airflow-providers-http-4.5.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-http-4.5.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4480 2023-07-12 19:13:29.267642 apache-airflow-providers-http-4.5.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-07-12 19:13:28.000000 apache-airflow-providers-http-4.5.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.180504 apache-airflow-providers-http-4.5.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.181594 apache-airflow-providers-http-4.5.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.215986 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-07-12 19:08:31.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3320 2023-07-12 19:13:28.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.221668 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16172 2023-07-09 14:40:47.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/hooks/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.227193 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7470 2023-07-10 18:20:09.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/operators/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.232834 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5864 2023-07-05 07:19:39.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/sensors/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.238574 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-10 18:20:09.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4988 2023-07-10 18:20:09.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/triggers/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.262194 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4480 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      852 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-http-4.5.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-07-12 19:13:29.269949 apache-airflow-providers-http-4.5.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-07-12 19:13:27.000000 apache-airflow-providers-http-4.5.0rc1/setup.py
```

### Comparing `apache-airflow-providers-http-4.4.2rc1/LICENSE` & `apache-airflow-providers-http-4.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2rc1/MANIFEST.in` & `apache-airflow-providers-http-4.5.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/__init__.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.4.2"
+__version__ = "4.5.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/get_provider_info.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-http",
         "name": "Hypertext Transfer Protocol (HTTP)",
         "description": "`Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__\n",
         "suspended": False,
         "versions": [
+            "4.5.0",
             "4.4.2",
             "4.4.1",
             "4.4.0",
             "4.3.0",
             "4.2.0",
             "4.1.1",
             "4.1.0",
@@ -79,11 +80,17 @@
         ],
         "hooks": [
             {
                 "integration-name": "Hypertext Transfer Protocol (HTTP)",
                 "python-modules": ["airflow.providers.http.hooks.http"],
             }
         ],
+        "triggers": [
+            {
+                "integration-name": "Hypertext Transfer Protocol (HTTP)",
+                "python-modules": ["airflow.providers.http.triggers.http"],
+            }
+        ],
         "connection-types": [
             {"hook-class-name": "airflow.providers.http.hooks.http.HttpHook", "connection-type": "http"}
         ],
     }
```

### Comparing `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/hooks/__init__.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/hooks/http.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/hooks/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
             attempt_num = 1
             while True:
                 response = await request_func(
                     url,
                     json=data if self.method in ("POST", "PATCH") else None,
                     params=data if self.method == "GET" else None,
-                    headers=headers,
+                    headers=_headers,
                     auth=auth,
                     **extra_options,
                 )
                 try:
                     response.raise_for_status()
                     return response
                 except ClientResponseError as e:
```

### Comparing `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/operators/__init__.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/operators/http.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/sensors/http.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,121 +15,124 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, Sequence
 
-from requests.auth import AuthBase
-
 from airflow.exceptions import AirflowException
-from airflow.models import BaseOperator
 from airflow.providers.http.hooks.http import HttpHook
+from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
-class SimpleHttpOperator(BaseOperator):
+class HttpSensor(BaseSensorOperator):
     """
-    Calls an endpoint on an HTTP system to execute an action.
+    Execute HTTP GET statement; return False on failure 404 Not Found or `response_check` returning False.
+
+    HTTP Error codes other than 404 (like 403) or Connection Refused Error
+    would raise an exception and fail the sensor itself directly (no more poking).
+    To avoid failing the task for other codes than 404, the argument ``extra_option``
+    can be passed with the value ``{'check_response': False}``. It will make the ``response_check``
+    be execute for any http status code.
+
+    The response check can access the template context to the operator:
+
+    .. code-block:: python
+
+        def response_check(response, task_instance):
+            # The task_instance is injected, so you can pull data form xcom
+            # Other context variables such as dag, ds, execution_date are also available.
+            xcom_data = task_instance.xcom_pull(task_ids="pushing_task")
+            # In practice you would do something more sensible with this data..
+            print(xcom_data)
+            return True
+
+
+        HttpSensor(task_id="my_http_sensor", ..., response_check=response_check)
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
-        :ref:`howto/operator:SimpleHttpOperator`
+        :ref:`howto/operator:HttpSensor`
 
-    :param http_conn_id: The :ref:`http connection<howto/connection:http>` to run
-        the operator against
-    :param endpoint: The relative part of the full url. (templated)
-    :param method: The HTTP method to use, default = "POST"
-    :param data: The data to pass. POST-data in POST/PUT and params
-        in the URL for a GET request. (templated)
+    :param http_conn_id: The :ref:`http connection<howto/connection:http>` to run the
+        sensor against
+    :param method: The HTTP request method to use
+    :param endpoint: The relative part of the full url
+    :param request_params: The parameters to be added to the GET url
     :param headers: The HTTP headers to be added to the GET request
     :param response_check: A check against the 'requests' response object.
         The callable takes the response object as the first positional argument
         and optionally any number of keyword arguments available in the context dictionary.
         It should return True for 'pass' and False otherwise.
-    :param response_filter: A function allowing you to manipulate the response
-        text. e.g response_filter=lambda response: json.loads(response.text).
-        The callable takes the response object as the first positional argument
-        and optionally any number of keyword arguments available in the context dictionary.
     :param extra_options: Extra options for the 'requests' library, see the
         'requests' documentation (options to modify timeout, ssl, etc.)
-    :param log_response: Log the response (default: False)
-    :param auth_type: The auth type for the service
     :param tcp_keep_alive: Enable TCP Keep Alive for the connection.
     :param tcp_keep_alive_idle: The TCP Keep Alive Idle parameter (corresponds to ``socket.TCP_KEEPIDLE``).
     :param tcp_keep_alive_count: The TCP Keep Alive count parameter (corresponds to ``socket.TCP_KEEPCNT``)
     :param tcp_keep_alive_interval: The TCP Keep Alive interval parameter (corresponds to
         ``socket.TCP_KEEPINTVL``)
     """
 
-    template_fields: Sequence[str] = (
-        "endpoint",
-        "data",
-        "headers",
-    )
-    template_fields_renderers = {"headers": "json", "data": "py"}
-    template_ext: Sequence[str] = ()
-    ui_color = "#f4a460"
+    template_fields: Sequence[str] = ("endpoint", "request_params", "headers")
 
     def __init__(
         self,
         *,
-        endpoint: str | None = None,
-        method: str = "POST",
-        data: Any = None,
-        headers: dict[str, str] | None = None,
+        endpoint: str,
+        http_conn_id: str = "http_default",
+        method: str = "GET",
+        request_params: dict[str, Any] | None = None,
+        headers: dict[str, Any] | None = None,
         response_check: Callable[..., bool] | None = None,
-        response_filter: Callable[..., Any] | None = None,
         extra_options: dict[str, Any] | None = None,
-        http_conn_id: str = "http_default",
-        log_response: bool = False,
-        auth_type: type[AuthBase] | None = None,
         tcp_keep_alive: bool = True,
         tcp_keep_alive_idle: int = 120,
         tcp_keep_alive_count: int = 20,
         tcp_keep_alive_interval: int = 30,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
+        self.endpoint = endpoint
         self.http_conn_id = http_conn_id
         self.method = method
-        self.endpoint = endpoint
+        self.request_params = request_params or {}
         self.headers = headers or {}
-        self.data = data or {}
-        self.response_check = response_check
-        self.response_filter = response_filter
         self.extra_options = extra_options or {}
-        self.log_response = log_response
-        self.auth_type = auth_type
+        self.response_check = response_check
         self.tcp_keep_alive = tcp_keep_alive
         self.tcp_keep_alive_idle = tcp_keep_alive_idle
         self.tcp_keep_alive_count = tcp_keep_alive_count
         self.tcp_keep_alive_interval = tcp_keep_alive_interval
 
-    def execute(self, context: Context) -> Any:
+    def poke(self, context: Context) -> bool:
         from airflow.utils.operator_helpers import determine_kwargs
 
-        http = HttpHook(
-            self.method,
+        hook = HttpHook(
+            method=self.method,
             http_conn_id=self.http_conn_id,
-            auth_type=self.auth_type,
             tcp_keep_alive=self.tcp_keep_alive,
             tcp_keep_alive_idle=self.tcp_keep_alive_idle,
             tcp_keep_alive_count=self.tcp_keep_alive_count,
             tcp_keep_alive_interval=self.tcp_keep_alive_interval,
         )
 
-        self.log.info("Calling HTTP method")
+        self.log.info("Poking: %s", self.endpoint)
+        try:
+            response = hook.run(
+                self.endpoint,
+                data=self.request_params,
+                headers=self.headers,
+                extra_options=self.extra_options,
+            )
+            if self.response_check:
+                kwargs = determine_kwargs(self.response_check, [response], context)
+                return self.response_check(response, **kwargs)
+        except AirflowException as exc:
+            if str(exc).startswith("404"):
+                return False
+
+            raise exc
 
-        response = http.run(self.endpoint, self.data, self.headers, self.extra_options)
-        if self.log_response:
-            self.log.info(response.text)
-        if self.response_check:
-            kwargs = determine_kwargs(self.response_check, [response], context)
-            if not self.response_check(response, **kwargs):
-                raise AirflowException("Response check returned False.")
-        if self.response_filter:
-            kwargs = determine_kwargs(self.response_filter, [response], context)
-            return self.response_filter(response, **kwargs)
-        return response.text
+        return True
```

### Comparing `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/sensors/__init__.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/sensors/http.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/operators/http.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,127 +13,161 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+import base64
+import pickle
 from typing import TYPE_CHECKING, Any, Callable, Sequence
 
+from requests import Response
+from requests.auth import AuthBase
+
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException
+from airflow.models import BaseOperator
 from airflow.providers.http.hooks.http import HttpHook
-from airflow.sensors.base import BaseSensorOperator
+from airflow.providers.http.triggers.http import HttpTrigger
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
-class HttpSensor(BaseSensorOperator):
+class SimpleHttpOperator(BaseOperator):
     """
-    Executes a HTTP GET statement and returns False on failure caused by
-    404 Not Found or `response_check` returning False.
-
-    HTTP Error codes other than 404 (like 403) or Connection Refused Error
-    would raise an exception and fail the sensor itself directly (no more poking).
-    To avoid failing the task for other codes than 404, the argument ``extra_option``
-    can be passed with the value ``{'check_response': False}``. It will make the ``response_check``
-    be execute for any http status code.
-
-    The response check can access the template context to the operator:
-
-    .. code-block:: python
-
-        def response_check(response, task_instance):
-            # The task_instance is injected, so you can pull data form xcom
-            # Other context variables such as dag, ds, execution_date are also available.
-            xcom_data = task_instance.xcom_pull(task_ids="pushing_task")
-            # In practice you would do something more sensible with this data..
-            print(xcom_data)
-            return True
-
-
-        HttpSensor(task_id="my_http_sensor", ..., response_check=response_check)
+    Calls an endpoint on an HTTP system to execute an action.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
-        :ref:`howto/operator:HttpSensor`
+        :ref:`howto/operator:SimpleHttpOperator`
 
-    :param http_conn_id: The :ref:`http connection<howto/connection:http>` to run the
-        sensor against
-    :param method: The HTTP request method to use
-    :param endpoint: The relative part of the full url
-    :param request_params: The parameters to be added to the GET url
+    :param http_conn_id: The :ref:`http connection<howto/connection:http>` to run
+        the operator against
+    :param endpoint: The relative part of the full url. (templated)
+    :param method: The HTTP method to use, default = "POST"
+    :param data: The data to pass. POST-data in POST/PUT and params
+        in the URL for a GET request. (templated)
     :param headers: The HTTP headers to be added to the GET request
     :param response_check: A check against the 'requests' response object.
         The callable takes the response object as the first positional argument
         and optionally any number of keyword arguments available in the context dictionary.
         It should return True for 'pass' and False otherwise.
+    :param response_filter: A function allowing you to manipulate the response
+        text. e.g response_filter=lambda response: json.loads(response.text).
+        The callable takes the response object as the first positional argument
+        and optionally any number of keyword arguments available in the context dictionary.
     :param extra_options: Extra options for the 'requests' library, see the
         'requests' documentation (options to modify timeout, ssl, etc.)
+    :param log_response: Log the response (default: False)
+    :param auth_type: The auth type for the service
     :param tcp_keep_alive: Enable TCP Keep Alive for the connection.
     :param tcp_keep_alive_idle: The TCP Keep Alive Idle parameter (corresponds to ``socket.TCP_KEEPIDLE``).
     :param tcp_keep_alive_count: The TCP Keep Alive count parameter (corresponds to ``socket.TCP_KEEPCNT``)
     :param tcp_keep_alive_interval: The TCP Keep Alive interval parameter (corresponds to
         ``socket.TCP_KEEPINTVL``)
+    :param deferrable: Run operator in the deferrable mode
     """
 
-    template_fields: Sequence[str] = ("endpoint", "request_params", "headers")
+    template_fields: Sequence[str] = (
+        "endpoint",
+        "data",
+        "headers",
+    )
+    template_fields_renderers = {"headers": "json", "data": "py"}
+    template_ext: Sequence[str] = ()
+    ui_color = "#f4a460"
 
     def __init__(
         self,
         *,
-        endpoint: str,
-        http_conn_id: str = "http_default",
-        method: str = "GET",
-        request_params: dict[str, Any] | None = None,
-        headers: dict[str, Any] | None = None,
+        endpoint: str | None = None,
+        method: str = "POST",
+        data: Any = None,
+        headers: dict[str, str] | None = None,
         response_check: Callable[..., bool] | None = None,
+        response_filter: Callable[..., Any] | None = None,
         extra_options: dict[str, Any] | None = None,
+        http_conn_id: str = "http_default",
+        log_response: bool = False,
+        auth_type: type[AuthBase] | None = None,
         tcp_keep_alive: bool = True,
         tcp_keep_alive_idle: int = 120,
         tcp_keep_alive_count: int = 20,
         tcp_keep_alive_interval: int = 30,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
-        self.endpoint = endpoint
         self.http_conn_id = http_conn_id
         self.method = method
-        self.request_params = request_params or {}
+        self.endpoint = endpoint
         self.headers = headers or {}
-        self.extra_options = extra_options or {}
+        self.data = data or {}
         self.response_check = response_check
+        self.response_filter = response_filter
+        self.extra_options = extra_options or {}
+        self.log_response = log_response
+        self.auth_type = auth_type
         self.tcp_keep_alive = tcp_keep_alive
         self.tcp_keep_alive_idle = tcp_keep_alive_idle
         self.tcp_keep_alive_count = tcp_keep_alive_count
         self.tcp_keep_alive_interval = tcp_keep_alive_interval
+        self.deferrable = deferrable
 
-    def poke(self, context: Context) -> bool:
-        from airflow.utils.operator_helpers import determine_kwargs
-
-        hook = HttpHook(
-            method=self.method,
-            http_conn_id=self.http_conn_id,
-            tcp_keep_alive=self.tcp_keep_alive,
-            tcp_keep_alive_idle=self.tcp_keep_alive_idle,
-            tcp_keep_alive_count=self.tcp_keep_alive_count,
-            tcp_keep_alive_interval=self.tcp_keep_alive_interval,
-        )
-
-        self.log.info("Poking: %s", self.endpoint)
-        try:
-            response = hook.run(
-                self.endpoint,
-                data=self.request_params,
-                headers=self.headers,
-                extra_options=self.extra_options,
+    def execute(self, context: Context) -> Any:
+        if self.deferrable:
+            self.defer(
+                trigger=HttpTrigger(
+                    http_conn_id=self.http_conn_id,
+                    auth_type=self.auth_type,
+                    method=self.method,
+                    endpoint=self.endpoint,
+                    headers=self.headers,
+                    data=self.data,
+                    extra_options=self.extra_options,
+                ),
+                method_name="execute_complete",
+            )
+        else:
+            http = HttpHook(
+                self.method,
+                http_conn_id=self.http_conn_id,
+                auth_type=self.auth_type,
+                tcp_keep_alive=self.tcp_keep_alive,
+                tcp_keep_alive_idle=self.tcp_keep_alive_idle,
+                tcp_keep_alive_count=self.tcp_keep_alive_count,
+                tcp_keep_alive_interval=self.tcp_keep_alive_interval,
             )
-            if self.response_check:
-                kwargs = determine_kwargs(self.response_check, [response], context)
-                return self.response_check(response, **kwargs)
-        except AirflowException as exc:
-            if str(exc).startswith("404"):
-                return False
 
-            raise exc
+            self.log.info("Calling HTTP method")
+
+            response = http.run(self.endpoint, self.data, self.headers, self.extra_options)
+            return self.process_response(context=context, response=response)
+
+    def process_response(self, context: Context, response: Response) -> str:
+        """Process the response."""
+        from airflow.utils.operator_helpers import determine_kwargs
 
-        return True
+        if self.log_response:
+            self.log.info(response.text)
+        if self.response_check:
+            kwargs = determine_kwargs(self.response_check, [response], context)
+            if not self.response_check(response, **kwargs):
+                raise AirflowException("Response check returned False.")
+        if self.response_filter:
+            kwargs = determine_kwargs(self.response_filter, [response], context)
+            return self.response_filter(response, **kwargs)
+        return response.text
+
+    def execute_complete(self, context: Context, event: dict):
+        """
+        Callback for when the trigger fires - returns immediately.
+
+        Relies on trigger to throw an exception, otherwise it assumes execution was successful.
+        """
+        if event["status"] == "success":
+            response = pickle.loads(base64.standard_b64decode(event["response"]))
+            return self.process_response(context=context, response=response)
+        else:
+            raise AirflowException(f"Unexpected error in the operation: {event['message']}")
```

### Comparing `apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/SOURCES.txt` & `apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 airflow/providers/http/get_provider_info.py
 airflow/providers/http/hooks/__init__.py
 airflow/providers/http/hooks/http.py
 airflow/providers/http/operators/__init__.py
 airflow/providers/http/operators/http.py
 airflow/providers/http/sensors/__init__.py
 airflow/providers/http/sensors/http.py
+airflow/providers/http/triggers/__init__.py
+airflow/providers/http/triggers/http.py
 apache_airflow_providers_http.egg-info/PKG-INFO
 apache_airflow_providers_http.egg-info/SOURCES.txt
 apache_airflow_providers_http.egg-info/dependency_links.txt
 apache_airflow_providers_http.egg-info/entry_points.txt
 apache_airflow_providers_http.egg-info/not-zip-safe
 apache_airflow_providers_http.egg-info/requires.txt
 apache_airflow_providers_http.egg-info/top_level.txt
```

### Comparing `apache-airflow-providers-http-4.4.2rc1/pyproject.toml` & `apache-airflow-providers-http-4.5.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-http-4.4.2rc1/setup.cfg` & `apache-airflow-providers-http-4.5.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.2/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-http/4.5.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-http/4.5.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-http-4.4.2rc1/setup.py` & `apache-airflow-providers-http-4.5.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-http package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.4.2"
+version = "4.5.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-http setup."""
     setup(
         version=version,
         extras_require={},
```


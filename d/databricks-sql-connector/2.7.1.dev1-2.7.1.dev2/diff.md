# Comparing `tmp/databricks_sql_connector-2.7.1.dev1.tar.gz` & `tmp/databricks_sql_connector-2.7.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sql_connector-2.7.1.dev1.tar", max compression
+gzip compressed data, was "databricks_sql_connector-2.7.1.dev2.tar", max compression
```

## Comparing `databricks_sql_connector-2.7.1.dev1.tar` & `databricks_sql_connector-2.7.1.dev2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     4821 2023-07-10 22:01:30.910556 databricks_sql_connector-2.7.1.dev1/CHANGELOG.md
--rw-r--r--   0        0        0    11346 2023-06-14 20:24:08.166793 databricks_sql_connector-2.7.1.dev1/LICENSE
--rw-r--r--   0        0        0     2723 2023-06-14 20:24:08.167012 databricks_sql_connector-2.7.1.dev1/README.md
--rw-r--r--   0        0        0     1593 2023-07-10 22:04:02.434540 databricks_sql_connector-2.7.1.dev1/pyproject.toml
--rw-r--r--   0        0        0      295 2023-06-14 20:24:08.170343 databricks_sql_connector-2.7.1.dev1/src/databricks/__init__.py
--rw-r--r--   0        0        0     1274 2023-07-10 22:04:13.555138 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 20:24:08.170890 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/__init__.py
--rw-r--r--   0        0        0     4421 2023-06-26 20:08:27.727475 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/auth.py
--rw-r--r--   0        0        0     6192 2023-06-26 20:08:27.727986 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/authenticators.py
--rw-r--r--   0        0        0     3790 2023-06-26 20:08:27.728260 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/endpoint.py
--rw-r--r--   0        0        0     9499 2023-06-26 20:08:27.728679 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/oauth.py
--rw-r--r--   0        0        0     1201 2023-06-14 20:24:08.171709 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/oauth_http_handler.py
--rw-r--r--   0        0        0     5949 2023-06-22 16:18:22.936813 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/thrift_http_client.py
--rw-r--r--   0        0        0    37992 2023-07-10 15:14:36.220919 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/client.py
--rw-r--r--   0        0        0     6547 2023-07-10 15:14:36.221186 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/cloudfetch/download_manager.py
--rw-r--r--   0        0        0     6374 2023-07-10 15:14:36.221386 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/cloudfetch/downloader.py
--rw-r--r--   0        0        0     2423 2023-06-14 20:24:08.172576 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/exc.py
--rw-r--r--   0        0        0        0 2023-06-14 20:24:08.172808 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/experimental/__init__.py
--rw-r--r--   0        0        0     2543 2023-06-26 20:08:27.729586 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/experimental/oauth_persistence.py
--rwxr-xr-x   0        0        0     8062 2023-06-14 20:24:08.173439 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
--rw-r--r--   0        0        0   136849 2023-06-14 20:24:08.175895 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
--rw-r--r--   0        0        0       49 2023-06-14 20:24:08.176090 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/__init__.py
--rw-r--r--   0        0        0     1307 2023-06-14 20:24:08.176221 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/constants.py
--rw-r--r--   0        0        0  2077276 2023-06-14 20:24:08.177855 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/ttypes.py
--rw-r--r--   0        0        0        0 2023-06-14 20:24:08.178096 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/__init__.py
--rw-r--r--   0        0        0    40111 2023-07-10 15:14:36.221836 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_backend.py
--rw-r--r--   0        0        0     6771 2023-06-14 20:24:08.178634 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/types.py
--rw-r--r--   0        0        0    17993 2023-07-10 15:14:36.222244 databricks_sql_connector-2.7.1.dev1/src/databricks/sql/utils.py
--rw-r--r--   0        0        0       60 2023-06-14 20:24:08.179003 databricks_sql_connector-2.7.1.dev1/src/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    10562 2023-07-10 21:41:38.369013 databricks_sql_connector-2.7.1.dev1/src/databricks/sqlalchemy/dialect/__init__.py
--rw-r--r--   0        0        0      494 2023-06-14 20:24:08.179360 databricks_sql_connector-2.7.1.dev1/src/databricks/sqlalchemy/dialect/base.py
--rw-r--r--   0        0        0      792 2023-06-14 20:24:08.179497 databricks_sql_connector-2.7.1.dev1/src/databricks/sqlalchemy/dialect/compiler.py
--rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 databricks_sql_connector-2.7.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0     5070 2023-07-12 01:05:48.311672 databricks_sql_connector-2.7.1.dev2/CHANGELOG.md
+-rw-r--r--   0        0        0    11346 2023-06-14 20:24:08.166793 databricks_sql_connector-2.7.1.dev2/LICENSE
+-rw-r--r--   0        0        0     2723 2023-06-14 20:24:08.167012 databricks_sql_connector-2.7.1.dev2/README.md
+-rw-r--r--   0        0        0     1593 2023-07-12 13:58:42.950327 databricks_sql_connector-2.7.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0      295 2023-06-14 20:24:08.170343 databricks_sql_connector-2.7.1.dev2/src/databricks/__init__.py
+-rw-r--r--   0        0        0     1274 2023-07-12 13:58:37.675891 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:24:08.170890 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/__init__.py
+-rw-r--r--   0        0        0     4421 2023-07-11 02:39:13.117511 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/auth.py
+-rw-r--r--   0        0        0     6192 2023-07-11 02:39:13.117899 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/authenticators.py
+-rw-r--r--   0        0        0     3790 2023-07-11 02:39:13.118139 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/endpoint.py
+-rw-r--r--   0        0        0     9989 2023-07-12 01:04:46.051969 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/oauth.py
+-rw-r--r--   0        0        0     1201 2023-06-14 20:24:08.171709 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/oauth_http_handler.py
+-rw-r--r--   0        0        0     6036 2023-07-12 01:04:46.052362 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/thrift_http_client.py
+-rw-r--r--   0        0        0    37992 2023-07-12 00:32:42.468464 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/client.py
+-rw-r--r--   0        0        0     6547 2023-07-12 00:32:42.468765 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/cloudfetch/download_manager.py
+-rw-r--r--   0        0        0     6374 2023-07-12 00:32:42.469030 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/cloudfetch/downloader.py
+-rw-r--r--   0        0        0     2423 2023-06-14 20:24:08.172576 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:24:08.172808 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/experimental/__init__.py
+-rw-r--r--   0        0        0     2543 2023-07-11 02:39:13.120777 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/experimental/oauth_persistence.py
+-rwxr-xr-x   0        0        0     8062 2023-06-14 20:24:08.173439 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
+-rw-r--r--   0        0        0   136849 2023-06-14 20:24:08.175895 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
+-rw-r--r--   0        0        0       49 2023-06-14 20:24:08.176090 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/__init__.py
+-rw-r--r--   0        0        0     1307 2023-06-14 20:24:08.176221 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/constants.py
+-rw-r--r--   0        0        0  2077276 2023-06-14 20:24:08.177855 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/ttypes.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:24:08.178096 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/__init__.py
+-rw-r--r--   0        0        0    40111 2023-07-12 00:32:42.469577 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_backend.py
+-rw-r--r--   0        0        0     6771 2023-06-14 20:24:08.178634 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/types.py
+-rw-r--r--   0        0        0    17993 2023-07-12 00:32:42.470095 databricks_sql_connector-2.7.1.dev2/src/databricks/sql/utils.py
+-rw-r--r--   0        0        0       60 2023-06-14 20:24:08.179003 databricks_sql_connector-2.7.1.dev2/src/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    10687 2023-07-12 01:04:46.082556 databricks_sql_connector-2.7.1.dev2/src/databricks/sqlalchemy/dialect/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-14 20:24:08.179360 databricks_sql_connector-2.7.1.dev2/src/databricks/sqlalchemy/dialect/base.py
+-rw-r--r--   0        0        0      792 2023-06-14 20:24:08.179497 databricks_sql_connector-2.7.1.dev2/src/databricks/sqlalchemy/dialect/compiler.py
+-rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 databricks_sql_connector-2.7.1.dev2/PKG-INFO
```

### Comparing `databricks_sql_connector-2.7.1.dev1/CHANGELOG.md` & `databricks_sql_connector-2.7.1.dev2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Release History
 
 ## 2.7.x (Unreleased)
 
+- Add support for Cloud Fetch
+- SQLAlchemy has_table function now honours schema= argument and adds catalog= argument
 - Fix: Revised SQLAlchemy dialect and examples for compatibility with SQLAlchemy==1.3.x
+- Fix: oauth would fail if expired credentials appeared in ~/.netrc
+- Fix: Python HTTP proxies were broken after switch to urllib3
 
 ## 2.7.0 (2023-06-26)
 
 - Fix: connector raised exception when calling close() on a closed Thrift session
 - Improve e2e test development ergonomics
 - Redact logged thrift responses by default
 - Add support for OAuth on Databricks Azure
```

### Comparing `databricks_sql_connector-2.7.1.dev1/LICENSE` & `databricks_sql_connector-2.7.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/README.md` & `databricks_sql_connector-2.7.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/pyproject.toml` & `databricks_sql_connector-2.7.1.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-sql-connector"
-version = "2.7.1.dev1"
+version = "2.7.1.dev2"
 description = "Databricks SQL Connector for Python"
 authors = ["Databricks <databricks-sql-connector-maintainers@databricks.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "databricks", from = "src"}]
 include = ["CHANGELOG.md"]
```

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/__init__.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 NUMBER = DBAPITypeObject(
     "boolean", "tinyint", "smallint", "int", "bigint", "float", "double", "decimal"
 )
 DATETIME = DBAPITypeObject("timestamp")
 DATE = DBAPITypeObject("date")
 ROWID = DBAPITypeObject()
 
-__version__ = "2.7.1.dev1"
+__version__ = "2.7.1.dev2"
 USER_AGENT_NAME = "PyDatabricksSqlConnector"
 
 # These two functions are pyhive legacy
 Date = datetime.date
 Timestamp = datetime.datetime
```

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/auth.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/auth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/authenticators.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/authenticators.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/endpoint.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/endpoint.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/oauth.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/oauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,30 @@
 
 from databricks.sql.auth.oauth_http_handler import OAuthHttpSingleRequestHandler
 from databricks.sql.auth.endpoint import OAuthEndpointCollection
 
 logger = logging.getLogger(__name__)
 
 
+class IgnoreNetrcAuth(requests.auth.AuthBase):
+    """This auth method is a no-op.
+
+    We use it to force requestslib to not use .netrc to write auth headers
+    when making .post() requests to the oauth token endpoints, since these
+    don't require authentication.
+
+    In cases where .netrc is outdated or corrupt, these requests will fail.
+
+    See issue #121
+    """
+
+    def __call__(self, r):
+        return r
+
+
 class OAuthManager:
     def __init__(
         self,
         port_range: List[int],
         client_id: str,
         idp_endpoint: OAuthEndpointCollection,
     ):
@@ -39,15 +55,15 @@
     def __get_redirect_url(redirect_port: int):
         return f"http://localhost:{redirect_port}"
 
     def __fetch_well_known_config(self, hostname: str):
         known_config_url = self.idp_endpoint.get_openid_config_url(hostname)
 
         try:
-            response = requests.get(url=known_config_url)
+            response = requests.get(url=known_config_url, auth=IgnoreNetrcAuth())
         except RequestException as e:
             logger.error(
                 f"Unable to fetch OAuth configuration from {known_config_url}.\n"
                 "Verify it is a valid workspace URL and that OAuth is "
                 "enabled on this account."
             )
             raise e
@@ -145,15 +161,17 @@
 
     @staticmethod
     def __send_token_request(token_request_url, data):
         headers = {
             "Accept": "application/json",
             "Content-Type": "application/x-www-form-urlencoded",
         }
-        response = requests.post(url=token_request_url, data=data, headers=headers)
+        response = requests.post(
+            url=token_request_url, data=data, headers=headers, auth=IgnoreNetrcAuth()
+        )
         return response.json()
 
     def __send_refresh_token_request(self, hostname, refresh_token):
         oauth_config = self.__fetch_well_known_config(hostname)
         token_request_url = oauth_config["token_endpoint"]
         client = oauthlib.oauth2.WebApplicationClient(self.client_id)
         token_request_body = client.prepare_refresh_body(
```

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/oauth_http_handler.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/oauth_http_handler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/auth/thrift_http_client.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/auth/thrift_http_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,18 @@
         if self.using_proxy():
             proxy_manager = ProxyManager(
                 self.proxy_uri,
                 num_pools=1,
                 headers={"Proxy-Authorization": self.proxy_auth},
             )
             self.__pool = proxy_manager.connection_from_host(
-                self.host, self.port, pool_kwargs=_pool_kwargs
+                host=self.realhost,
+                port=self.realport,
+                scheme=self.scheme,
+                pool_kwargs=_pool_kwargs,
             )
         else:
             self.__pool = pool_class(self.host, self.port, **_pool_kwargs)
 
     def close(self):
         self.__resp and self.__resp.drain_conn()
         self.__resp and self.__resp.release_conn()
```

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/client.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/client.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/cloudfetch/download_manager.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/cloudfetch/download_manager.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/cloudfetch/downloader.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/cloudfetch/downloader.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/exc.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/exc.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/experimental/oauth_persistence.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/experimental/oauth_persistence.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/constants.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_api/TCLIService/ttypes.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_api/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/thrift_backend.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/thrift_backend.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/types.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/types.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sql/utils.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sql/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sqlalchemy/dialect/__init__.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sqlalchemy/dialect/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,25 +263,30 @@
 
         return _tables
 
     def do_rollback(self, dbapi_connection):
         # Databricks SQL Does not support transactions
         pass
 
-    def has_table(self, connection, table_name, schema=None, **kwargs) -> bool:
+    def has_table(
+        self, connection, table_name, schema=None, catalog=None, **kwargs
+    ) -> bool:
         """SQLAlchemy docstrings say dialect providers must implement this method"""
 
-        schema = schema or "default"
+        _schema = schema or self.schema
+        _catalog = catalog or self.catalog
 
         # DBR >12.x uses underscores in error messages
         DBR_LTE_12_NOT_FOUND_STRING = "Table or view not found"
         DBR_GT_12_NOT_FOUND_STRING = "TABLE_OR_VIEW_NOT_FOUND"
 
         try:
-            res = connection.execute(f"DESCRIBE TABLE {table_name}")
+            res = connection.execute(
+                f"DESCRIBE TABLE {_catalog}.{_schema}.{table_name}"
+            )
             return True
         except DatabaseError as e:
             if DBR_GT_12_NOT_FOUND_STRING in str(
                 e
             ) or DBR_LTE_12_NOT_FOUND_STRING in str(e):
                 return False
             else:
```

### Comparing `databricks_sql_connector-2.7.1.dev1/src/databricks/sqlalchemy/dialect/compiler.py` & `databricks_sql_connector-2.7.1.dev2/src/databricks/sqlalchemy/dialect/compiler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.7.1.dev1/PKG-INFO` & `databricks_sql_connector-2.7.1.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sql-connector
-Version: 2.7.1.dev1
+Version: 2.7.1.dev2
 Summary: Databricks SQL Connector for Python
 License: Apache-2.0
 Author: Databricks
 Author-email: databricks-sql-connector-maintainers@databricks.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


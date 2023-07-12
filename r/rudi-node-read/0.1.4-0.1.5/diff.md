# Comparing `tmp/rudi-node-read-0.1.4.tar.gz` & `tmp/rudi-node-read-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudi-node-read-0.1.4.tar", last modified: Tue Jul 11 13:35:58 2023, max compression
+gzip compressed data, was "rudi-node-read-0.1.5.tar", last modified: Wed Jul 12 09:57:31 2023, max compression
```

## Comparing `rudi-node-read-0.1.4.tar` & `rudi-node-read-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.590342 rudi-node-read-0.1.4/
--rw-rw-r--   0 omartine (660741) dept-aac (29120)    13840 2022-03-30 12:00:55.000000 rudi-node-read-0.1.4/LICENCE.md
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     2144 2023-07-11 13:35:58.590048 rudi-node-read-0.1.4/PKG-INFO
--rw-rw-r--   0 omartine (660741) dept-aac (29120)      940 2023-07-07 15:06:14.000000 rudi-node-read-0.1.4/README.md
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     1818 2023-07-11 13:35:29.000000 rudi-node-read-0.1.4/pyproject.toml
--rw-rw-r--   0 omartine (660741) dept-aac (29120)       38 2023-07-11 13:35:58.590448 rudi-node-read-0.1.4/setup.cfg
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.577826 rudi-node-read-0.1.4/src/
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.580221 rudi-node-read-0.1.4/src/rudi_node_read/
--rw-r--r--   0 omartine (660741) dept-aac (29120)        0 2023-07-07 13:29:00.000000 rudi-node-read-0.1.4/src/rudi_node_read/__init_.py
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.583363 rudi-node-read-0.1.4/src/rudi_node_read/connectors/
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     5302 2023-07-10 15:15:15.000000 rudi-node-read-0.1.4/src/rudi_node_read/connectors/io_connector.py
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     4137 2023-07-10 14:57:09.000000 rudi-node-read-0.1.4/src/rudi_node_read/connectors/io_rudi_node_read.py
--rw-rw-r--   0 omartine (660741) dept-aac (29120)    20460 2023-07-10 14:57:04.000000 rudi-node-read-0.1.4/src/rudi_node_read/rudi_node_reader.py
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.588631 rudi-node-read-0.1.4/src/rudi_node_read/utils/
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     2115 2023-07-07 15:12:22.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/err.py
--rw-rw-r--   0 omartine (660741) dept-aac (29120)      864 2023-07-07 15:12:22.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/jwt.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     1355 2023-07-07 15:12:22.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/log.py
--rw-rw-r--   0 omartine (660741) dept-aac (29120)      302 2023-07-07 12:48:49.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/serializable.py
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     5138 2023-07-10 14:58:48.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/type_dict.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)      784 2023-07-07 15:12:22.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/type_misc.py
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     1631 2023-07-10 14:58:16.000000 rudi-node-read-0.1.4/src/rudi_node_read/utils/type_string.py
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.582431 rudi-node-read-0.1.4/src/rudi_node_read.egg-info/
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     2144 2023-07-11 13:35:58.000000 rudi-node-read-0.1.4/src/rudi_node_read.egg-info/PKG-INFO
--rw-rw-r--   0 omartine (660741) dept-aac (29120)      694 2023-07-11 13:35:58.000000 rudi-node-read-0.1.4/src/rudi_node_read.egg-info/SOURCES.txt
--rw-rw-r--   0 omartine (660741) dept-aac (29120)        1 2023-07-11 13:35:58.000000 rudi-node-read-0.1.4/src/rudi_node_read.egg-info/dependency_links.txt
--rw-rw-r--   0 omartine (660741) dept-aac (29120)       81 2023-07-11 13:35:58.000000 rudi-node-read-0.1.4/src/rudi_node_read.egg-info/requires.txt
--rw-rw-r--   0 omartine (660741) dept-aac (29120)       15 2023-07-11 13:35:58.000000 rudi-node-read-0.1.4/src/rudi_node_read.egg-info/top_level.txt
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-11 13:35:58.589284 rudi-node-read-0.1.4/tests/
--rw-r--r--   0 omartine (660741) dept-aac (29120)     3171 2023-07-07 15:12:22.000000 rudi-node-read-0.1.4/tests/test_rudi_node_reader.py
+drwxr-xr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-12 09:57:31.240890 rudi-node-read-0.1.5/
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)    13840 2022-03-30 12:00:55.000000 rudi-node-read-0.1.5/LICENCE.md
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     2144 2023-07-12 09:57:31.240522 rudi-node-read-0.1.5/PKG-INFO
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)      940 2023-07-07 15:06:14.000000 rudi-node-read-0.1.5/README.md
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     2354 2023-07-12 09:57:12.000000 rudi-node-read-0.1.5/pyproject.toml
+-rw-r--r--   0 omartine (660741) dept-aac (29120)       38 2023-07-12 09:57:31.240988 rudi-node-read-0.1.5/setup.cfg
+drwxr-xr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-12 09:57:31.226066 rudi-node-read-0.1.5/src/
+drwxr-xr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-12 09:57:31.229250 rudi-node-read-0.1.5/src/rudi_node_read/
+-rw-r--r--   0 omartine (660741) dept-aac (29120)        0 2023-07-07 13:29:00.000000 rudi-node-read-0.1.5/src/rudi_node_read/__init_.py
+drwxr-xr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-12 09:57:31.233416 rudi-node-read-0.1.5/src/rudi_node_read/connectors/
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     5755 2023-07-12 09:38:19.000000 rudi-node-read-0.1.5/src/rudi_node_read/connectors/io_connector.py
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     5175 2023-07-12 09:46:56.000000 rudi-node-read-0.1.5/src/rudi_node_read/connectors/io_rudi_node_read.py
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)    20849 2023-07-12 09:55:59.000000 rudi-node-read-0.1.5/src/rudi_node_read/rudi_node_reader.py
+drwxr-xr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-12 09:57:31.239011 rudi-node-read-0.1.5/src/rudi_node_read/utils/
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     2115 2023-07-07 15:12:22.000000 rudi-node-read-0.1.5/src/rudi_node_read/utils/err.py
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)      864 2023-07-07 15:12:22.000000 rudi-node-read-0.1.5/src/rudi_node_read/utils/jwt.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     1401 2023-07-12 09:42:46.000000 rudi-node-read-0.1.5/src/rudi_node_read/utils/log.py
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)      302 2023-07-07 12:48:49.000000 rudi-node-read-0.1.5/src/rudi_node_read/utils/serializable.py
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     5138 2023-07-10 14:58:48.000000 rudi-node-read-0.1.5/src/rudi_node_read/utils/type_dict.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)      784 2023-07-07 15:12:22.000000 rudi-node-read-0.1.5/src/rudi_node_read/utils/type_misc.py
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     1631 2023-07-10 14:58:16.000000 rudi-node-read-0.1.5/src/rudi_node_read/utils/type_string.py
+drwxr-xr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-12 09:57:31.232414 rudi-node-read-0.1.5/src/rudi_node_read.egg-info/
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     2144 2023-07-12 09:57:31.000000 rudi-node-read-0.1.5/src/rudi_node_read.egg-info/PKG-INFO
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)      694 2023-07-12 09:57:31.000000 rudi-node-read-0.1.5/src/rudi_node_read.egg-info/SOURCES.txt
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)        1 2023-07-12 09:57:31.000000 rudi-node-read-0.1.5/src/rudi_node_read.egg-info/dependency_links.txt
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)       81 2023-07-12 09:57:31.000000 rudi-node-read-0.1.5/src/rudi_node_read.egg-info/requires.txt
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)       15 2023-07-12 09:57:31.000000 rudi-node-read-0.1.5/src/rudi_node_read.egg-info/top_level.txt
+drwxr-xr-x   0 omartine (660741) dept-aac (29120)        0 2023-07-12 09:57:31.239763 rudi-node-read-0.1.5/tests/
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     3171 2023-07-07 15:12:22.000000 rudi-node-read-0.1.5/tests/test_rudi_node_reader.py
```

### Comparing `rudi-node-read-0.1.4/LICENCE.md` & `rudi-node-read-0.1.5/LICENCE.md`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.4/PKG-INFO` & `rudi-node-read-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudi-node-read
-Version: 0.1.4
+Version: 0.1.5
 Summary: Use the external API of a RUDI Producer node
 Author-email: Olivier Martineau <olivier.martineau@irisa.fr>
 Maintainer-email: Olivier Martineau <olivier.martineau@irisa.fr>
 License: EUPL-1.2
 Project-URL: Homepage, https://github.com/OlivierMartineau/rudi-node-read
 Project-URL: Documentation, https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER
 Project-URL: Changelog, https://github.com/OlivierMartineau/rudi-node-read/blob/release/CHANGELOG.md
```

### Comparing `rudi-node-read-0.1.4/README.md` & `rudi-node-read-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.4/src/rudi_node_read/connectors/io_connector.py` & `rudi-node-read-0.1.5/src/rudi_node_read/connectors/io_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from rudi_node_read.utils.log import log_d_if, log_e, log_d
 from rudi_node_read.utils.serializable import Serializable
 from rudi_node_read.utils.type_string import slash_join
 
 HttpRequestMethod = Literal["GET", "PUT", "DEL", "POST"]
 HTTP_REQUEST_METHODS = get_args(HttpRequestMethod)
 
+STATUS = "status"
+REDIRECTION = "redirection"
+
 
 def https_download(resource_url: str, should_show_debug_line: bool = False):
     fun = "https_download"
     (scheme, netloc, path, query, fragment) = urlsplit(resource_url)
     if scheme != "https":
         raise NotImplementedError("only HTTPS protocol is supported")
     connection = HTTPSConnection(netloc)
@@ -31,22 +34,28 @@
         return data
 
 
 class Connector(Serializable):
     _default_connector = None
 
     def __init__(self, server_url: str):
+        self.scheme = None
+        self.host = None
+        self.path = None
+        self.base_url = None
+        self._set_url(server_url)
+
+    def _set_url(self, server_url: str):
         (scheme, netloc, path, query, fragment) = urlsplit(server_url)
         if scheme != "http" and scheme != "https":
             raise NotImplementedError("only http and https are supported")
         self.scheme = scheme
         self.host = netloc
         self.path = path
         self.base_url = slash_join(f"{self.scheme}://{self.host}", self.path)
-
         log_d("Connector", "base_url", self.base_url)
 
     def full_url(self, url: str = "/"):
         return slash_join(self.base_url, url)
 
     def full_path(self, url: str = "/"):
         return slash_join("/", self.path, url)
@@ -94,14 +103,17 @@
         headers: dict,
         body: dict,
         should_log_response: bool = True,
     ):
         """Basic parsing of the result"""
         fun = f"{self.__class__.__name__}.parse_response"
         response = connection.getresponse()
+        # log_d(fun, "Response", response.getcode(), response.getheaders(), response.info())
+        if response.status in [301, 302]:
+            return {STATUS: response.status, REDIRECTION: response.getheader("location")}
         if (
             response.status not in [200, 500, 501]
             and not (530 <= response.status < 540)
             and not (400 <= response.status < 500)
         ):
             return None
```

### Comparing `rudi-node-read-0.1.4/src/rudi_node_read/connectors/io_rudi_node_read.py` & `rudi-node-read-0.1.5/src/rudi_node_read/connectors/io_rudi_node_read.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from rudi_node_read.connectors.io_connector import Connector
+from rudi_node_read.connectors.io_connector import Connector, STATUS, REDIRECTION
 from rudi_node_read.utils.log import log_d, log_e
+from rudi_node_read.utils.type_dict import is_dict
 from rudi_node_read.utils.type_string import slash_join
 
 REQ_LIMIT = 500
 
 
 class RudiNodeConnector(Connector):
     def __init__(self, server_url: str, headers_user_agent: str = "RudiNodeConnector"):
         """
         Creates a connector to the API/proxy module of a RUDI Node
         :param server_url: the URL of the RUDI Node
         :param headers_user_agent: (optional) identifies the user launching the request (or at least the module)
         in the request headers, for logging purpose.
         """
+        fun = "RudiNodeConnector.__init__"
 
         super().__init__(server_url)
 
-        log_d("RudiNodeConnector", "attributes", self)
+        # log_d("RudiNodeConnector", "attributes", self)
         self.test_rudi_api_connection()
         self._headers = {
             "User-Agent": headers_user_agent,
             "Content-type": "text/plain",
             "Accept": "application/json",
         }
 
@@ -29,17 +31,31 @@
         Performs an identified GET request through /api/v1 path
         :param url: part of the URL that comes after /api/admin
         :return: a JSON
         """
         return self.request(url=slash_join("api/v1", url), req_method="GET", headers=self._headers)
 
     def test_rudi_api_connection(self):
-        test = self.request("api/admin/hash")
+        test_path = "api/admin/hash"
+        test = self.request(test_path)
         if test is None:
             log_e("RudiNodeConnector", f"!! Node '{self.host}'", "no connection!")
+            raise ConnectionError(f"Connection failed to node '{self.host}'")
+        if is_dict(test) and test.get(STATUS) in [301, 302]:
+            server_url = str(test.get(REDIRECTION))
+            if not server_url.endswith(test_path):
+                log_e("RudiNodeConnector", f"!! Node '{self.host}'", "redirection incorrect!")
+                raise ConnectionError(f"Connection failed to node '{self.host}'")
+            self._set_url(server_url.replace(f"/{test_path}", ""))
+            test = self.request(test_path)
+            if test is None:
+                log_e("RudiNodeConnector", f"!! Node '{self.host}'", "redirection failed!")
+                raise ConnectionError(f"Connection failed to node '{self.host}'")
+            log_d("RudiNodeConnector", f"Node '{self.host}'", "redirection OK")
+
         else:
             log_d("RudiNodeConnector", f"Node '{self.host}'", "connection OK")
 
     def get_metadata_with_uuid(self, metadata_uuid: str):
         return self.get_api(f"resources/{metadata_uuid}")
 
     def get_metadata_with_filter(self, rudi_fields_filter: dict):
@@ -85,16 +101,17 @@
                     "id": media["media_id"],
                 }
             )
         return media_list_final
 
 
 if __name__ == "__main__":
-    rudi_node_connector = RudiNodeConnector("https://bacasable.fenix.rudi-univ-rennes1.fr")
+    # rudi_node_connector = RudiNodeConnector("https://bacasable.fenix.rudi-univ-rennes1.fr")
+    rudi_node_connector = RudiNodeConnector("https://audiar.rudi.irisa.fr")
     log_d("RudiNodeConnector", "metadata nb", rudi_node_connector.get_metadata_count())
     log_d("RudiNodeConnector", "metadata_ids", rudi_node_connector.get_metadata_ids())
-    meta1 = rudi_node_connector.get_metadata_list()[1]
+    meta1 = rudi_node_connector.get_metadata_list()[0]
     meta1_id = meta1["global_id"]
     rudi_node_connector.get_metadata_with_uuid(meta1_id)
     log_d("RudiNodeConnector", "meta1", meta1_id)
     meta1_media = rudi_node_connector.get_list_media_for_metadata(meta1_id)
     log_d("RudiNodeConnector", "meta1 media", meta1_media)
```

### Comparing `rudi-node-read-0.1.4/src/rudi_node_read/rudi_node_reader.py` & `rudi-node-read-0.1.5/src/rudi_node_read/rudi_node_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,20 @@
 _STATUS_DOWNLOADED = "downloaded"
 
 
 class RudiNodeReader:
     _default_getter = None
 
     def __init__(self, server_url: str, headers_user_agent: str = "RudiNodeReader"):
+        fun = "RudiNodeReader.__init__"
         self._server_url = server_url
         self._headers_user_agent = headers_user_agent
-
-        self._connector = None
+        log_d(fun, "connecting")
+        self._connector = RudiNodeConnector(self._server_url, self._headers_user_agent)
+        log_d(fun, self._connector)
 
         self._meta_list = None
         self._meta_list_available = None
         self._meta_count = 0
         self._org_list = None
         self._org_names = None
         self._contact_list = None
@@ -425,15 +427,17 @@
         file_path = abspath(slash_join(local_download_dir, file_name))
         json_str = dumps(obj=self.metadata_list, ensure_ascii=False, indent=2).encode("utf-8")
         open(file_path, "wb").write(json_str)
 
 
 if __name__ == "__main__":
     rudi_node_info = RudiNodeReader("https://bacasable.fenix.rudi-univ-rennes1.fr")
+    # rudi_node_info = RudiNodeReader("https://audiar.rudi.irisa.fr")
     info_tag = "RudiNode info"
+
     log_d(info_tag, "metadata nb", rudi_node_info.metadata_count)
     log_d(info_tag, "metadata list nb", len(rudi_node_info.metadata_list))
     log_d(info_tag, "organizations", rudi_node_info.organization_list)
     log_d(info_tag, "organization names", rudi_node_info.organization_names)
 
     log_d(info_tag, "contact names", rudi_node_info.contact_names)
     log_d(info_tag, "themes", rudi_node_info.themes)
@@ -524,7 +528,10 @@
     log_d(
         dwnld_tag,
         f"media with name '{f_name}'",
         rudi_node_info.download_file_with_name(f_name, dwnld_dir),
     )
 
     rudi_node_info.save_metadata_to_file(dwnld_dir)
+
+    rudi_node_with_redirect = RudiNodeReader("https://audiar.rudi.irisa.fr")
+    log_d(info_tag, "metadata nb", rudi_node_with_redirect.metadata_count)
```

### Comparing `rudi-node-read-0.1.4/src/rudi_node_read/utils/err.py` & `rudi-node-read-0.1.5/src/rudi_node_read/utils/err.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.4/src/rudi_node_read/utils/jwt.py` & `rudi-node-read-0.1.5/src/rudi_node_read/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.4/src/rudi_node_read/utils/log.py` & `rudi-node-read-0.1.5/src/rudi_node_read/utils/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime
+from os import getenv
 from time import time
 
-SHOULD_LOG = False
+SHOULD_LOG = bool(getenv("RUDI_NODE_DEV"))
 
 
 def log(*args):
     if SHOULD_LOG:
         if len(args) < 2:
             print(f"D {now()}")
         elif len(args) == 2:
```

### Comparing `rudi-node-read-0.1.4/src/rudi_node_read/utils/type_dict.py` & `rudi-node-read-0.1.5/src/rudi_node_read/utils/type_dict.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.4/src/rudi_node_read/utils/type_misc.py` & `rudi-node-read-0.1.5/src/rudi_node_read/utils/type_misc.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.4/src/rudi_node_read/utils/type_string.py` & `rudi-node-read-0.1.5/src/rudi_node_read/utils/type_string.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.4/src/rudi_node_read.egg-info/PKG-INFO` & `rudi-node-read-0.1.5/src/rudi_node_read.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudi-node-read
-Version: 0.1.4
+Version: 0.1.5
 Summary: Use the external API of a RUDI Producer node
 Author-email: Olivier Martineau <olivier.martineau@irisa.fr>
 Maintainer-email: Olivier Martineau <olivier.martineau@irisa.fr>
 License: EUPL-1.2
 Project-URL: Homepage, https://github.com/OlivierMartineau/rudi-node-read
 Project-URL: Documentation, https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER
 Project-URL: Changelog, https://github.com/OlivierMartineau/rudi-node-read/blob/release/CHANGELOG.md
```

### Comparing `rudi-node-read-0.1.4/src/rudi_node_read.egg-info/SOURCES.txt` & `rudi-node-read-0.1.5/src/rudi_node_read.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.4/tests/test_rudi_node_reader.py` & `rudi-node-read-0.1.5/tests/test_rudi_node_reader.py`

 * *Files identical despite different names*


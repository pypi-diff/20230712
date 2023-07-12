# Comparing `tmp/papertronics-sdk-0.0.34.tar.gz` & `tmp/papertronics-sdk-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papertronics-sdk-0.0.34.tar", last modified: Tue Jul 11 14:49:59 2023, max compression
+gzip compressed data, was "papertronics-sdk-0.0.35.tar", last modified: Wed Jul 12 08:46:40 2023, max compression
```

## Comparing `papertronics-sdk-0.0.34.tar` & `papertronics-sdk-0.0.35.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:59.050178 papertronics-sdk-0.0.34/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-11 14:49:59.050178 papertronics-sdk-0.0.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:59.046178 papertronics-sdk-0.0.34/papertronics_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:59.046178 papertronics-sdk-0.0.34/papertronics_sdk/lab/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/lab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/lab/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/lab/base_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:59.046178 papertronics-sdk-0.0.34/papertronics_sdk/lab/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/lab/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/lab/exceptions/status_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:59.050178 papertronics-sdk-0.0.34/papertronics_sdk/lab/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/lab/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/lab/models/admin_cloud_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/lab/models/cloud_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/lab/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/lab/models/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/lab/models/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/lab/models/station_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/papertronics_sdk/lab/user_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:49:59.046178 papertronics-sdk-0.0.34/papertronics_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-11 14:49:59.000000 papertronics-sdk-0.0.34/papertronics_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-11 14:49:59.000000 papertronics-sdk-0.0.34/papertronics_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:49:59.000000 papertronics-sdk-0.0.34/papertronics_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-11 14:49:59.000000 papertronics-sdk-0.0.34/papertronics_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 14:49:59.000000 papertronics-sdk-0.0.34/papertronics_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:49:58.000000 papertronics-sdk-0.0.34/papertronics_sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 14:49:47.000000 papertronics-sdk-0.0.34/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-11 14:49:59.050178 papertronics-sdk-0.0.34/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:40.490350 papertronics-sdk-0.0.35/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-12 08:46:40.494350 papertronics-sdk-0.0.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:40.486349 papertronics-sdk-0.0.35/papertronics_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:40.490350 papertronics-sdk-0.0.35/papertronics_sdk/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/base_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:40.490350 papertronics-sdk-0.0.35/papertronics_sdk/lab/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/exceptions/status_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:40.490350 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/admin_cloud_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/cloud_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/models/station_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/papertronics_sdk/lab/user_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:46:40.490350 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-12 08:46:40.000000 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-12 08:46:40.000000 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:46:40.000000 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 08:46:40.000000 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 08:46:40.000000 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:46:40.000000 papertronics-sdk-0.0.35/papertronics_sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-12 08:46:26.000000 papertronics-sdk-0.0.35/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-12 08:46:40.494350 papertronics-sdk-0.0.35/setup.cfg
```

### Comparing `papertronics-sdk-0.0.34/PKG-INFO` & `papertronics-sdk-0.0.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.34
+Version: 0.0.35
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.34/README.md` & `papertronics-sdk-0.0.35/README.md`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.34/papertronics_sdk/lab/admin_client.py` & `papertronics-sdk-0.0.35/papertronics_sdk/lab/admin_client.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.34/papertronics_sdk/lab/base_client.py` & `papertronics-sdk-0.0.35/papertronics_sdk/lab/base_client.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.34/papertronics_sdk/lab/models/cloud_models.py` & `papertronics-sdk-0.0.35/papertronics_sdk/lab/models/cloud_models.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.34/papertronics_sdk/lab/models/database.py` & `papertronics-sdk-0.0.35/papertronics_sdk/lab/models/database.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.34/papertronics_sdk/lab/models/generic.py` & `papertronics-sdk-0.0.35/papertronics_sdk/lab/models/generic.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.34/papertronics_sdk/lab/models/station_protocol.py` & `papertronics-sdk-0.0.35/papertronics_sdk/lab/models/station_protocol.py`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.34/papertronics_sdk/lab/user_client.py` & `papertronics-sdk-0.0.35/papertronics_sdk/lab/user_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -65,33 +65,46 @@
 
     def get_protocol(self,
                      protocol_id: Optional[uuid.UUID] = None,
                      protocol_test_type: Optional[str] = None,
                      page_size: Optional[int] = None,
                      page: Optional[int] = None,
                      valid: Optional[bool] = True) -> Union[ProtocolModel, List[ProtocolModel]]:
+        params = {}
+        if protocol_id:
+            params["protocol_id"] = protocol_id
+        if protocol_test_type:
+            params["protocol_test_type"] = protocol_test_type
+        if page_size is not None:
+            params["page_size"] = page_size
+        if page is not None:
+            params["page"] = page
+        if valid is not None:
+            params["valid"] = valid
+
         response = self.get(f"/protocol",
                             headers={"Authorization": f"Bearer {self.token}"},
-                            params=dict(protocol_id=protocol_id,
-                                        protocol_test_type=protocol_test_type,
-                                        page_size=page_size,
-                                        page=page,
-                                        valid=valid))
+                            params=params)
         if type(response.json()) == list:
             return [ProtocolModel.parse_obj(r) for r in response.json()]
         else:
             return ProtocolModel.parse_obj(response.json())
 
     def count_protocol(self,
                        protocol_test_type: Optional[str] = None,
                        valid: Optional[bool] = True) -> int:
+        params = {}
+        if protocol_test_type:
+            params["protocol_test_type"] = protocol_test_type
+        if valid is not None:
+            params["valid"] = valid
+
         response = self.get(f"/protocol/count",
                             headers={"Authorization": f"Bearer {self.token}"},
-                            params=dict(protocol_test_type=protocol_test_type,
-                                        valid=valid))
+                            params=params)
         return int(response.text)
 
     def get_protocol_test_def(self, protocol_id: uuid.UUID) -> Union[ProtocolTestResponse, str]:
         response = self.get(f"/protocol/test",
                             headers={"Authorization": f"Bearer {self.token}"},
                             params={"protocol_id": protocol_id})
         if type(response.json()) == str:
@@ -123,35 +136,48 @@
                         device_id: Optional[uuid.UUID] = None,
                         order_by: str = "start_time",
                         ascending_order: bool = False,
                         page_size: Optional[int] = None,
                         page: Optional[int] = None,
                         valid: Optional[bool] = None,
                         first=True) -> Union[List[ExperimentModel], ExperimentModel]:
+        params = {"order_by": order_by,
+                  "ascending_order": ascending_order,
+                  "first": first}
+        if experiment_id:
+            params["experiment_id"] = experiment_id
+        if device_id:
+            params["device_id"] = device_id
+        if page_size is not None:
+            params["page_size"] = page_size
+        if page is not None:
+            params["page"] = page
+        if valid is not None:
+            params["valid"] = valid
+
         response = self.get(f"/experiment",
                             headers={"Authorization": f"Bearer {self.token}"},
-                            params=dict(experiment_id=experiment_id,
-                                        device_id=device_id,
-                                        order_by=order_by,
-                                        ascending_order=ascending_order,
-                                        page_size=page_size,
-                                        page=page,
-                                        valid=valid))
+                            params=params)
         if first:
             return ExperimentModel.parse_obj(response.json()[0])
         else:
             return [ExperimentModel.parse_obj(r) for r in response.json()]
 
     def count_experiments(self,
                           valid: Optional[bool] = None,
                           device_id: Optional[uuid.UUID] = None) -> int:
+        params = {}
+        if valid is not None:
+            params["valid"] = valid
+        if device_id is not None:
+            params["device_id"] = device_id
+
         response = self.get(f"/experiment/count",
                             headers={"Authorization": f"Bearer {self.token}"},
-                            params=dict(device_id=device_id,
-                                        valid=valid))
+                            params=params)
         return int(response.text)
 
     def edit_experiment_by_id(self,
                               experiment_id: uuid.UUID,
                               experiment_edit_request: ExperimentEditRequest):
         response = self.post(f"/experiment/edit",
                              headers={"Authorization": f"Bearer {self.token}"},
```

### Comparing `papertronics-sdk-0.0.34/papertronics_sdk.egg-info/PKG-INFO` & `papertronics-sdk-0.0.35/papertronics_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papertronics-sdk
-Version: 0.0.34
+Version: 0.0.35
 Summary: A collection of pydantic models and shared utility functions for SG Papertronics projects
 Home-page: https://github.com/SG-Papertronics/shared
 Author: Job Heersink
 Author-email: j.g.heersink@sgpapertronics.com
 License: private
 Keywords: beer-o-meter,lab-app,setuptools
 Classifier: Programming Language :: Python :: 3
```

### Comparing `papertronics-sdk-0.0.34/papertronics_sdk.egg-info/SOURCES.txt` & `papertronics-sdk-0.0.35/papertronics_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `papertronics-sdk-0.0.34/setup.cfg` & `papertronics-sdk-0.0.35/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = papertronics-sdk
-version = 0.0.34
+version = 0.0.35
 author = Job Heersink
 author_email = j.g.heersink@sgpapertronics.com
 url = https://github.com/SG-Papertronics/shared
 description = A collection of pydantic models and shared utility functions for SG Papertronics projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = beer-o-meter, lab-app, setuptools
```


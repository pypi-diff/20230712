# Comparing `tmp/benchling_wrapper-0.1.2.tar.gz` & `tmp/benchling_wrapper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchling_wrapper-0.1.2.tar", last modified: Wed Apr  5 16:34:04 2023, max compression
+gzip compressed data, was "benchling_wrapper-0.2.1.tar", last modified: Wed Jul 12 10:09:33 2023, max compression
```

## Comparing `benchling_wrapper-0.1.2.tar` & `benchling_wrapper-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-04-05 16:34:04.332654 benchling_wrapper-0.1.2/
--rw-r--r--   0 bostongene   (503) staff       (20)     1074 2023-04-04 09:25:52.000000 benchling_wrapper-0.1.2/LICENSE
--rw-r--r--   0 bostongene   (503) staff       (20)      735 2023-04-05 16:34:04.332791 benchling_wrapper-0.1.2/PKG-INFO
--rw-r--r--   0 bostongene   (503) staff       (20)      565 2023-04-04 09:20:37.000000 benchling_wrapper-0.1.2/README.md
--rw-r--r--   0 bostongene   (503) staff       (20)      103 2023-04-05 16:34:04.333251 benchling_wrapper-0.1.2/setup.cfg
--rw-r--r--   0 bostongene   (503) staff       (20)     1423 2023-04-05 16:33:06.000000 benchling_wrapper-0.1.2/setup.py
-drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-04-05 16:34:04.328564 benchling_wrapper-0.1.2/src/
-drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-04-05 16:34:04.330936 benchling_wrapper-0.1.2/src/benchling_wrapper/
--rw-r--r--   0 bostongene   (503) staff       (20)        0 2023-04-04 11:26:30.000000 benchling_wrapper-0.1.2/src/benchling_wrapper/__init__.py
--rw-r--r--   0 bostongene   (503) staff       (20)    15428 2023-04-04 10:21:24.000000 benchling_wrapper-0.1.2/src/benchling_wrapper/benchling_wrapper.py
-drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-04-05 16:34:04.332409 benchling_wrapper-0.1.2/src/benchling_wrapper.egg-info/
--rw-r--r--   0 bostongene   (503) staff       (20)      735 2023-04-05 16:34:04.000000 benchling_wrapper-0.1.2/src/benchling_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 bostongene   (503) staff       (20)      337 2023-04-05 16:34:04.000000 benchling_wrapper-0.1.2/src/benchling_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 bostongene   (503) staff       (20)        1 2023-04-05 16:34:04.000000 benchling_wrapper-0.1.2/src/benchling_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 bostongene   (503) staff       (20)       57 2023-04-05 16:34:04.000000 benchling_wrapper-0.1.2/src/benchling_wrapper.egg-info/requires.txt
--rw-r--r--   0 bostongene   (503) staff       (20)       18 2023-04-05 16:34:04.000000 benchling_wrapper-0.1.2/src/benchling_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-07-12 10:09:33.138625 benchling_wrapper-0.2.1/
+-rw-r--r--   0 bostongene   (503) staff       (20)     1074 2023-04-04 09:25:52.000000 benchling_wrapper-0.2.1/LICENSE
+-rw-r--r--   0 bostongene   (503) staff       (20)      735 2023-07-12 10:09:33.139174 benchling_wrapper-0.2.1/PKG-INFO
+-rw-r--r--   0 bostongene   (503) staff       (20)      565 2023-04-04 09:20:37.000000 benchling_wrapper-0.2.1/README.md
+-rw-r--r--   0 bostongene   (503) staff       (20)      103 2023-07-12 10:09:33.140694 benchling_wrapper-0.2.1/setup.cfg
+-rw-r--r--   0 bostongene   (503) staff       (20)     1423 2023-07-12 10:07:56.000000 benchling_wrapper-0.2.1/setup.py
+drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-07-12 10:09:33.127140 benchling_wrapper-0.2.1/src/
+drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-07-12 10:09:33.133128 benchling_wrapper-0.2.1/src/benchling_wrapper/
+-rw-r--r--   0 bostongene   (503) staff       (20)        0 2023-04-04 11:26:30.000000 benchling_wrapper-0.2.1/src/benchling_wrapper/__init__.py
+-rw-r--r--   0 bostongene   (503) staff       (20)    16754 2023-07-12 10:06:15.000000 benchling_wrapper-0.2.1/src/benchling_wrapper/benchling_wrapper.py
+drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-07-12 10:09:33.137332 benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/
+-rw-r--r--   0 bostongene   (503) staff       (20)      735 2023-07-12 10:09:33.000000 benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 bostongene   (503) staff       (20)      337 2023-07-12 10:09:33.000000 benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 bostongene   (503) staff       (20)        1 2023-07-12 10:09:33.000000 benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 bostongene   (503) staff       (20)       57 2023-07-12 10:09:33.000000 benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/requires.txt
+-rw-r--r--   0 bostongene   (503) staff       (20)       18 2023-07-12 10:09:33.000000 benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/top_level.txt
```

### Comparing `benchling_wrapper-0.1.2/LICENSE` & `benchling_wrapper-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `benchling_wrapper-0.1.2/PKG-INFO` & `benchling_wrapper-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchling_wrapper
-Version: 0.1.2
+Version: 0.2.1
 Summary: To make integrations with Benchling easier we prepared a wrapper with the most used API functions.
 Home-page: https://bitbucket.org/egor-yatsishin/benchling-wrapper
 Author: Ivan Ivanov
 Author-email: 300899@gmail.com
 License: MIT
 Keywords: benchling wrapper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `benchling_wrapper-0.1.2/README.md` & `benchling_wrapper-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `benchling_wrapper-0.1.2/setup.py` & `benchling_wrapper-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='benchling_wrapper',
-    version='0.1.2',
+    version='0.2.1',
     license='MIT',
     author="Ivan Ivanov",
     author_email='300899@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://bitbucket.org/egor-yatsishin/benchling-wrapper',
     keywords='benchling wrapper',
```

### Comparing `benchling_wrapper-0.1.2/src/benchling_wrapper/benchling_wrapper.py` & `benchling_wrapper-0.2.1/src/benchling_wrapper/benchling_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Benchling Wrapper main module.
+"""
 from benchling_api_client.v2.stable.models.dna_sequence import DnaSequence
 from benchling_sdk.auth.client_credentials_oauth2 import ClientCredentialsOAuth2
 from benchling_api_client.models.naming_strategy import NamingStrategy
 from benchling_sdk.helpers.pagination_helpers import PageIterator
 from benchling_sdk.helpers.serialization_helpers import fields
 from benchling_sdk.helpers.retry_helpers import RetryStrategy
 from benchling_sdk.benchling import Benchling
@@ -16,14 +19,20 @@
 _RETRY_STRATEGY_MAX_TRIES = 17  # 65535.5 secs
 _REQUEST_STEP_BASE_DELAY = 60
 REQUESTS_RETRY_COUNT = 623  # 23:58:05
 
 
 def _with_retry(func: Callable) -> Callable:
     def wrapper(*args, **kwargs) -> Any:
+        """
+        Retry decorator for Benchling SDK methods.
+        :param args:
+        :param kwargs:
+        :return:
+        """
         for i in range(REQUESTS_RETRY_COUNT + 1):
             try:
                 return func(*args, **kwargs)
 
             # TransportError: decorate Benchling Limitation
             except TransportError as e:
                 if i == REQUESTS_RETRY_COUNT:
@@ -98,29 +107,32 @@
 
         :param: entity_name - name of the entity.
         :return: entity - entity for the given entity name
         """
         return self.benchling.custom_entities.list(name=entity_name).first()
 
     @_with_retry
-    def get_entities_by_names(self, entity_names: list[str]) -> PageIterator[CustomEntity]:
+    def get_entities_by_names(self, entity_names: list[str]) -> list[CustomEntity]:
         """
-        Get the entity for the given list of entity names.
+        Get the entities for the given list of entity names.
 
-        :param: entity_names - name of the entity.
+        :param: entity_name - name of the entity.
         :return: entity - entity for the given entity name
         """
-        return self.benchling.custom_entities.list(names_any_of=entity_names)
+        result = []
+        for chunk in chunking(entity_names):
+            result.extend(*self.benchling.custom_entities.list(names_any_of=chunk, page_size=100))
+        return result
 
     @_with_retry
     def get_entity_by_id(self, entity_id: str) -> CustomEntity:
         """
         Get the entity for the given entity id.
 
-        :param: entity_id - id of the entity
+        :param: entity_id - id of the entity.
         :return: entity - entity for the given entity id
         """
         return self.benchling.custom_entities.get_by_id(entity_id)
 
     @_with_retry
     def get_entities_by_ids(self,
                             entity_ids: list[str]) -> PageIterator[CustomEntity]:
@@ -131,19 +143,19 @@
         :return: page iterator with entities - list of entities for the given registry ids
         """
         registry_id = self.benchling_registry_id
         return self.benchling.custom_entities.list(registry_id=registry_id,
                                                    entity_registry_ids_any_of=entity_ids)
 
     @_with_retry
-    def get_sequence_by_name(self, entity_name: str) -> CustomEntity:
+    def get_sequence_by_name(self, entity_name: str) -> DnaSequence | None:
         """
         Get the entity for the given entity name.
 
-        :param: entity_name - name of the entity
+        :param: entity_name - name of the entity.
         :return: entity - entity for the given entity name
         """
         return self.benchling.dna_sequences.list(name=entity_name).first()
 
     @_with_retry
     def get_sequence_by_id(self, entity_id: str) -> DnaSequence:
         """
@@ -151,24 +163,43 @@
 
         :param: entity_id - id of the entity.
         :return: entity - entity for the given entity id
         """
         return self.benchling.dna_sequences.get_by_id(entity_id)
 
     @_with_retry
-    def get_sequences_by_ids(self, entity_ids: list[str]) -> PageIterator[DnaSequence]:
+    def get_sequences_by_ids(self, entity_ids: list[str]) -> list[DnaSequence]:
         """
         Get the entity for the given entity id.
 
         :param: entity_id - id of the entity.
         :return: entity - entity for the given entity id
         """
         registry_id = self.benchling_registry_id
-        return self.benchling.dna_sequences.list(registry_id=registry_id,
-                                                 entity_registry_ids_any_of=entity_ids)
+        result = []
+        for chunk in chunking(entity_ids):
+            result.extend(*self.benchling.dna_sequences.list(registry_id=registry_id,
+                                                             entity_registry_ids_any_of=chunk))
+        return result
+
+    @_with_retry
+    def get_entities_by_ids(self,
+                            entity_ids: list[str]) -> list[CustomEntity]:
+        """
+        Get the entity by the registry ids.
+
+        :param: entity_registry_ids_any_of - list of registry ids
+        :return: page iterator with entities - list of entities for the given registry ids
+        """
+        registry_id = self.benchling_registry_id
+        result = []
+        for chunk in chunking(entity_ids):
+            result.extend(*self.benchling.custom_entities.list(registry_id=registry_id,
+                                                               entity_registry_ids_any_of=chunk))
+        return result
 
     @_with_retry
     def get_entity_by_modified(self, schema_id: str, modified_at: str) -> PageIterator[CustomEntity]:
         """
         Get the entity by the modified_at entity attribute.
 
         :param: schema_id - id of the schema
@@ -248,17 +279,18 @@
     def unregister_entities(self, entity_ids: list[str], folder_id: str) -> None:
         """
         Unregister the entity in Benchling.
         :param: entity_id - id of the entity to unregister
         :return: None
         """
         registry_id = self.benchling_registry_id
-        self.benchling.registry.unregister(registry_id=registry_id,
-                                           entity_ids=entity_ids,
-                                           folder_id=folder_id)
+        for chunk in chunking(entity_ids):
+            self.benchling.registry.unregister(registry_id=registry_id,
+                                               entity_ids=chunk,
+                                               folder_id=folder_id)
 
     @_with_retry
     def get_dropdown_options(self, dropdown: models.Dropdown) -> dict:
         """
         Get dropdown variants by dropdown id.
         :param dropdown: dropdown object.
         :type dropdown: models.Dropdown.
@@ -293,63 +325,64 @@
     @_with_retry
     def register_assay_results(self, assay_results: list[models.AssayResultCreate]) -> None:
         """
         Register the assay result in Benchling.
         :param: assay_result - assay result to register - accepts a list
         :return: None
         """
-        self.benchling.assay_results.create(assay_results=assay_results)
+        for chunk in chunking(assay_results):
+            self.benchling.assay_results.create(assay_results=chunk)
 
 
 def get_entity_name(entity: CustomEntity) -> str:
     """
     Get the name of the entity.
 
-    :param: entity - benchling entity
+    :param: entity - benchling entity.
     :return: entity name - name of the entity
     """
     try:
         return entity.name
     except IndexError:
         raise ValueError("Can not get entity name")
 
 
 def get_entity_id(entity: CustomEntity) -> str:
     """
     Get the entity id of the entity.
 
-    :param: entity - benchling entity
+    :param: entity - benchling entity.
     :return: entity id - entity id of the entity
     """
     try:
         return entity.id
     except IndexError:
         raise ValueError("Can not get entity id")
 
 
 def get_field_value(entity: CustomEntity, field_name: str) -> str:
     """
     Get the value of the field with the given name.
 
     :param: entity - benchling entity
-    :param: field_name - name of the field
+    :param: field_name - name of the field.
     :return: field value - value of the field with the given name
     """
     try:
         return entity.fields[field_name].value
     except IndexError:
         raise ValueError(f"Can not get field value for {field_name}")
 
 
 def get_display_field_value(entity: CustomEntity, field_name: str) -> str:
     """
     Get the display value of the field with the given name.
 
     :param: entity - benchling entity
-    :param: field_name - name of the field
+    :param: field_name - name of the field.
     :return: field display value - display value of the field with the given name
     """
     try:
         return entity.fields[field_name].display_value
     except IndexError:
         raise ValueError(f"Can not get field display value for {field_name}")
 
@@ -407,7 +440,16 @@
     """
     assay_result = models.AssayResultCreate(
         schema_id=schema_id,
         fields=fields(fields_dict_converter(fields_dict)),
         project_id=project_id
     )
     return assay_result
+
+
+def chunking(lst: list):
+    """
+    Chunking the list into chunks of 100 elements.
+    :param lst:
+    """
+    for i in range(0, len(lst), 100):
+        yield lst[i:i + 100]
```

### Comparing `benchling_wrapper-0.1.2/src/benchling_wrapper.egg-info/PKG-INFO` & `benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchling-wrapper
-Version: 0.1.2
+Version: 0.2.1
 Summary: To make integrations with Benchling easier we prepared a wrapper with the most used API functions.
 Home-page: https://bitbucket.org/egor-yatsishin/benchling-wrapper
 Author: Ivan Ivanov
 Author-email: 300899@gmail.com
 License: MIT
 Keywords: benchling wrapper
 Classifier: Development Status :: 3 - Alpha
```


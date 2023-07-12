# Comparing `tmp/benchling_wrapper-0.2.1.tar.gz` & `tmp/benchling_wrapper-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchling_wrapper-0.2.1.tar", last modified: Wed Jul 12 10:09:33 2023, max compression
+gzip compressed data, was "benchling_wrapper-0.2.2.tar", last modified: Wed Jul 12 11:46:40 2023, max compression
```

## Comparing `benchling_wrapper-0.2.1.tar` & `benchling_wrapper-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-07-12 10:09:33.138625 benchling_wrapper-0.2.1/
--rw-r--r--   0 bostongene   (503) staff       (20)     1074 2023-04-04 09:25:52.000000 benchling_wrapper-0.2.1/LICENSE
--rw-r--r--   0 bostongene   (503) staff       (20)      735 2023-07-12 10:09:33.139174 benchling_wrapper-0.2.1/PKG-INFO
--rw-r--r--   0 bostongene   (503) staff       (20)      565 2023-04-04 09:20:37.000000 benchling_wrapper-0.2.1/README.md
--rw-r--r--   0 bostongene   (503) staff       (20)      103 2023-07-12 10:09:33.140694 benchling_wrapper-0.2.1/setup.cfg
--rw-r--r--   0 bostongene   (503) staff       (20)     1423 2023-07-12 10:07:56.000000 benchling_wrapper-0.2.1/setup.py
-drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-07-12 10:09:33.127140 benchling_wrapper-0.2.1/src/
-drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-07-12 10:09:33.133128 benchling_wrapper-0.2.1/src/benchling_wrapper/
--rw-r--r--   0 bostongene   (503) staff       (20)        0 2023-04-04 11:26:30.000000 benchling_wrapper-0.2.1/src/benchling_wrapper/__init__.py
--rw-r--r--   0 bostongene   (503) staff       (20)    16754 2023-07-12 10:06:15.000000 benchling_wrapper-0.2.1/src/benchling_wrapper/benchling_wrapper.py
-drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-07-12 10:09:33.137332 benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/
--rw-r--r--   0 bostongene   (503) staff       (20)      735 2023-07-12 10:09:33.000000 benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 bostongene   (503) staff       (20)      337 2023-07-12 10:09:33.000000 benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 bostongene   (503) staff       (20)        1 2023-07-12 10:09:33.000000 benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 bostongene   (503) staff       (20)       57 2023-07-12 10:09:33.000000 benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/requires.txt
--rw-r--r--   0 bostongene   (503) staff       (20)       18 2023-07-12 10:09:33.000000 benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-07-12 11:46:40.047262 benchling_wrapper-0.2.2/
+-rw-r--r--   0 bostongene   (503) staff       (20)     1074 2023-04-04 09:25:52.000000 benchling_wrapper-0.2.2/LICENSE
+-rw-r--r--   0 bostongene   (503) staff       (20)      735 2023-07-12 11:46:40.047501 benchling_wrapper-0.2.2/PKG-INFO
+-rw-r--r--   0 bostongene   (503) staff       (20)      565 2023-04-04 09:20:37.000000 benchling_wrapper-0.2.2/README.md
+-rw-r--r--   0 bostongene   (503) staff       (20)      103 2023-07-12 11:46:40.048323 benchling_wrapper-0.2.2/setup.cfg
+-rw-r--r--   0 bostongene   (503) staff       (20)     1423 2023-07-12 11:46:27.000000 benchling_wrapper-0.2.2/setup.py
+drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-07-12 11:46:40.042123 benchling_wrapper-0.2.2/src/
+drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-07-12 11:46:40.044524 benchling_wrapper-0.2.2/src/benchling_wrapper/
+-rw-r--r--   0 bostongene   (503) staff       (20)        0 2023-04-04 11:26:30.000000 benchling_wrapper-0.2.2/src/benchling_wrapper/__init__.py
+-rw-r--r--   0 bostongene   (503) staff       (20)    16179 2023-07-12 11:45:16.000000 benchling_wrapper-0.2.2/src/benchling_wrapper/benchling_wrapper.py
+drwxr-xr-x   0 bostongene   (503) staff       (20)        0 2023-07-12 11:46:40.046757 benchling_wrapper-0.2.2/src/benchling_wrapper.egg-info/
+-rw-r--r--   0 bostongene   (503) staff       (20)      735 2023-07-12 11:46:39.000000 benchling_wrapper-0.2.2/src/benchling_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 bostongene   (503) staff       (20)      337 2023-07-12 11:46:39.000000 benchling_wrapper-0.2.2/src/benchling_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 bostongene   (503) staff       (20)        1 2023-07-12 11:46:39.000000 benchling_wrapper-0.2.2/src/benchling_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 bostongene   (503) staff       (20)       57 2023-07-12 11:46:39.000000 benchling_wrapper-0.2.2/src/benchling_wrapper.egg-info/requires.txt
+-rw-r--r--   0 bostongene   (503) staff       (20)       18 2023-07-12 11:46:39.000000 benchling_wrapper-0.2.2/src/benchling_wrapper.egg-info/top_level.txt
```

### Comparing `benchling_wrapper-0.2.1/LICENSE` & `benchling_wrapper-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `benchling_wrapper-0.2.1/PKG-INFO` & `benchling_wrapper-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchling_wrapper
-Version: 0.2.1
+Version: 0.2.2
 Summary: To make integrations with Benchling easier we prepared a wrapper with the most used API functions.
 Home-page: https://bitbucket.org/egor-yatsishin/benchling-wrapper
 Author: Ivan Ivanov
 Author-email: 300899@gmail.com
 License: MIT
 Keywords: benchling wrapper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `benchling_wrapper-0.2.1/README.md` & `benchling_wrapper-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `benchling_wrapper-0.2.1/setup.py` & `benchling_wrapper-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='benchling_wrapper',
-    version='0.2.1',
+    version='0.2.2',
     license='MIT',
     author="Ivan Ivanov",
     author_email='300899@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://bitbucket.org/egor-yatsishin/benchling-wrapper',
     keywords='benchling wrapper',
```

### Comparing `benchling_wrapper-0.2.1/src/benchling_wrapper/benchling_wrapper.py` & `benchling_wrapper-0.2.2/src/benchling_wrapper/benchling_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,24 +131,27 @@
         :param: entity_id - id of the entity.
         :return: entity - entity for the given entity id
         """
         return self.benchling.custom_entities.get_by_id(entity_id)
 
     @_with_retry
     def get_entities_by_ids(self,
-                            entity_ids: list[str]) -> PageIterator[CustomEntity]:
+                            entity_ids: list[str]) -> list[CustomEntity]:
         """
         Get the entity by the registry ids.
 
         :param: entity_registry_ids_any_of - list of registry ids
         :return: page iterator with entities - list of entities for the given registry ids
         """
         registry_id = self.benchling_registry_id
-        return self.benchling.custom_entities.list(registry_id=registry_id,
-                                                   entity_registry_ids_any_of=entity_ids)
+        result = []
+        for chunk in chunking(entity_ids):
+            result.extend(*self.benchling.custom_entities.list(registry_id=registry_id,
+                                                               entity_registry_ids_any_of=chunk))
+        return result
 
     @_with_retry
     def get_sequence_by_name(self, entity_name: str) -> DnaSequence | None:
         """
         Get the entity for the given entity name.
 
         :param: entity_name - name of the entity.
@@ -178,30 +181,14 @@
         result = []
         for chunk in chunking(entity_ids):
             result.extend(*self.benchling.dna_sequences.list(registry_id=registry_id,
                                                              entity_registry_ids_any_of=chunk))
         return result
 
     @_with_retry
-    def get_entities_by_ids(self,
-                            entity_ids: list[str]) -> list[CustomEntity]:
-        """
-        Get the entity by the registry ids.
-
-        :param: entity_registry_ids_any_of - list of registry ids
-        :return: page iterator with entities - list of entities for the given registry ids
-        """
-        registry_id = self.benchling_registry_id
-        result = []
-        for chunk in chunking(entity_ids):
-            result.extend(*self.benchling.custom_entities.list(registry_id=registry_id,
-                                                               entity_registry_ids_any_of=chunk))
-        return result
-
-    @_with_retry
     def get_entity_by_modified(self, schema_id: str, modified_at: str) -> PageIterator[CustomEntity]:
         """
         Get the entity by the modified_at entity attribute.
 
         :param: schema_id - id of the schema
         :param: modified_at - modified_at attribute of the entity (datetime, RFC 3339 format)
         :return: page iterator with entities - list entity for the given (field name, field value) pair
```

### Comparing `benchling_wrapper-0.2.1/src/benchling_wrapper.egg-info/PKG-INFO` & `benchling_wrapper-0.2.2/src/benchling_wrapper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchling-wrapper
-Version: 0.2.1
+Version: 0.2.2
 Summary: To make integrations with Benchling easier we prepared a wrapper with the most used API functions.
 Home-page: https://bitbucket.org/egor-yatsishin/benchling-wrapper
 Author: Ivan Ivanov
 Author-email: 300899@gmail.com
 License: MIT
 Keywords: benchling wrapper
 Classifier: Development Status :: 3 - Alpha
```


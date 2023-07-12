# Comparing `tmp/idds-workflow-1.2.9.tar.gz` & `tmp/idds-workflow-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-workflow-1.2.9.tar", last modified: Sat Apr 29 19:24:58 2023, max compression
+gzip compressed data, was "idds-workflow-1.3.0.tar", last modified: Wed Jul 12 16:01:39 2023, max compression
```

## Comparing `idds-workflow-1.2.9.tar` & `idds-workflow-1.3.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:58.939656 idds-workflow-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-29 19:24:58.939656 idds-workflow-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:58.939656 idds-workflow-1.2.9/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:58.939656 idds-workflow-1.2.9/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:58.939656 idds-workflow-1.2.9/lib/idds/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflow/datawork.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflow/processingwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 19:24:53.000000 idds-workflow-1.2.9/lib/idds/workflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    80253 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflow/work.py
--rw-r--r--   0 runner    (1001) docker     (123)    90930 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:58.939656 idds-workflow-1.2.9/lib/idds/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflowv2/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflowv2/datawork.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflowv2/processingwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflowv2/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflowv2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    81692 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflowv2/work.py
--rw-r--r--   0 runner    (1001) docker     (123)   103034 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/lib/idds/workflowv2/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:58.939656 idds-workflow-1.2.9/lib/idds_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-29 19:24:58.000000 idds-workflow-1.2.9/lib/idds_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-29 19:24:58.000000 idds-workflow-1.2.9/lib/idds_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 19:24:58.000000 idds-workflow-1.2.9/lib/idds_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 19:24:58.000000 idds-workflow-1.2.9/lib/idds_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 19:24:58.000000 idds-workflow-1.2.9/lib/idds_workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-29 19:24:58.939656 idds-workflow-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-29 19:24:44.000000 idds-workflow-1.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:58.939656 idds-workflow-1.2.9/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:58.939656 idds-workflow-1.2.9/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-29 19:24:53.000000 idds-workflow-1.2.9/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.045985 idds-workflow-1.3.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.045985 idds-workflow-1.3.0/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/lib/idds/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/datawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/processingwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-12 16:01:34.000000 idds-workflow-1.3.0/lib/idds/workflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80453 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/work.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90930 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/lib/idds/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/datawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/processingwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81884 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/work.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103065 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/lib/idds_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-12 16:01:39.000000 idds-workflow-1.3.0/lib/idds_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-12 16:01:39.000000 idds-workflow-1.3.0/lib/idds_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:01:39.000000 idds-workflow-1.3.0/lib/idds_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 16:01:39.000000 idds-workflow-1.3.0/lib/idds_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 16:01:39.000000 idds-workflow-1.3.0/lib/idds_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.045985 idds-workflow-1.3.0/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 16:01:34.000000 idds-workflow-1.3.0/tools/env/environment.yml
```

### Comparing `idds-workflow-1.2.9/LICENSE.rst` & `idds-workflow-1.3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.9/PKG-INFO` & `idds-workflow-1.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-workflow
-Version: 1.2.9
+Version: 1.3.0
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-workflow-1.2.9/lib/idds/workflow/base.py` & `idds-workflow-1.3.0/lib/idds/workflow/base.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.9/lib/idds/workflow/datawork.py` & `idds-workflow-1.3.0/lib/idds/workflow/datawork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.9/lib/idds/workflow/processingwork.py` & `idds-workflow-1.3.0/lib/idds/workflow/processingwork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.9/lib/idds/workflow/utils.py` & `idds-workflow-1.3.0/lib/idds/workflow/utils.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.9/lib/idds/workflow/work.py` & `idds-workflow-1.3.0/lib/idds/workflow/work.py`

 * *Files 0% similar despite different names*

```diff
@@ -817,14 +817,17 @@
         if self._collections:
             for k in self._collections:
                 coll = self._collections[k]
                 if type(coll) in [Collection]:
                     coll_metadata[k] = {'coll_id': coll.coll_id}
         self.add_metadata_item('collections', coll_metadata)
 
+    def with_sub_map_id(self):
+        return False
+
     @property
     def processings(self):
         return self._processings
 
     @processings.setter
     def processings(self, value):
         self._processings = value
@@ -1824,14 +1827,17 @@
         *** Function called by Transformer agent.
         """
         return False
 
     def require_ext_contents(self):
         return False
 
+    def has_external_content_id(self):
+        return False
+
     def set_work_name_to_coll_map(self, work_name_to_coll_map):
         self.work_name_to_coll_map = work_name_to_coll_map
 
     def get_work_name_to_coll_map(self):
         return self.work_name_to_coll_map
 
     def add_processing_to_processings(self, processing):
@@ -2256,7 +2262,10 @@
             os.environ['X509_USER_PROXY'] = user_proxy
 
     def unset_user_proxy(self):
         if self.original_proxy:
             os.environ['X509_USER_PROXY'] = self.original_proxy
         else:
             del os.environ['X509_USER_PROXY']
+
+    def get_external_content_ids(self, processing, log_prefix=''):
+        return []
```

### Comparing `idds-workflow-1.2.9/lib/idds/workflow/workflow.py` & `idds-workflow-1.3.0/lib/idds/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.9/lib/idds/workflowv2/base.py` & `idds-workflow-1.3.0/lib/idds/workflowv2/base.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.9/lib/idds/workflowv2/datawork.py` & `idds-workflow-1.3.0/lib/idds/workflowv2/datawork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.9/lib/idds/workflowv2/processingwork.py` & `idds-workflow-1.3.0/lib/idds/workflowv2/processingwork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.9/lib/idds/workflowv2/utils.py` & `idds-workflow-1.3.0/lib/idds/workflowv2/utils.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.2.9/lib/idds/workflowv2/work.py` & `idds-workflow-1.3.0/lib/idds/workflowv2/work.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0OA
 #
 # Authors:
-# - Wen Guan, <wen.guan@cern.ch>, 2020 - 2021
+# - Wen Guan, <wen.guan@cern.ch>, 2020 - 2023
 
 import copy
 import datetime
 import logging
 import os
 import stat
 import uuid
@@ -846,14 +846,17 @@
         if self._collections:
             for k in self._collections:
                 coll = self._collections[k]
                 if type(coll) in [Collection]:
                     coll_metadata[k] = {'coll_id': coll.coll_id}
         self.add_metadata_item('collections', coll_metadata)
 
+    def with_sub_map_id(self):
+        return False
+
     @property
     def processings(self):
         return self._processings
 
     @processings.setter
     def processings(self, value):
         self._processings = value
@@ -1281,17 +1284,17 @@
         self.old_processings = []
         self.terminated_msg = ""
         self.output_data = {}
         self.parameters_for_next_task = None
         self.last_updated_at = datetime.datetime.utcnow()
 
     def set_agent_attributes(self, attrs, req_attributes=None):
+        if self.agent_attributes is None:
+            self.agent_attributes = {}
         if attrs and self.class_name in attrs:
-            if self.agent_attributes is None:
-                self.agent_attributes = {}
             for key, value in attrs[self.class_name].items():
                 self.agent_attributes[key] = value
         self.logger.info("agent_attributes: %s" % self.agent_attributes)
 
     def get_agent_attributes(self):
         return self.agent_attributes
 
@@ -1859,14 +1862,17 @@
         *** Function called by Transformer agent.
         """
         return False
 
     def require_ext_contents(self):
         return False
 
+    def has_external_content_id(self):
+        return False
+
     def set_work_name_to_coll_map(self, work_name_to_coll_map):
         self.work_name_to_coll_map = work_name_to_coll_map
 
     def get_work_name_to_coll_map(self):
         return self.work_name_to_coll_map
 
     def add_processing_to_processings(self, processing):
@@ -2291,7 +2297,10 @@
             os.environ['X509_USER_PROXY'] = user_proxy
 
     def unset_user_proxy(self):
         if self.original_proxy:
             os.environ['X509_USER_PROXY'] = self.original_proxy
         else:
             del os.environ['X509_USER_PROXY']
+
+    def get_external_content_ids(self, processing, log_prefix=''):
+        return []
```

### Comparing `idds-workflow-1.2.9/lib/idds/workflowv2/workflow.py` & `idds-workflow-1.3.0/lib/idds/workflowv2/workflow.py`

 * *Files identical despite different names*

```diff
@@ -1889,15 +1889,15 @@
                 return True
         return False
 
     def is_finished(self, synchronize=True):
         """
         *** Function called by Marshaller agent.
         """
-        return self.is_terminated(synchronize=synchronize) and self.num_finished_works == self.num_total_works
+        return self.is_terminated(synchronize=synchronize) and self.num_finished_works == self.num_total_works and (self.num_total_works > 0)
 
     def is_subfinished(self, synchronize=True):
         """
         *** Function called by Marshaller agent.
         """
         return self.is_terminated(synchronize=synchronize) and (self.num_finished_works + self.num_subfinished_works > 0 and self.num_finished_works + self.num_subfinished_works <= self.num_total_works)
```

### Comparing `idds-workflow-1.2.9/lib/idds_workflow.egg-info/PKG-INFO` & `idds-workflow-1.3.0/lib/idds_workflow.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-workflow
-Version: 1.2.9
+Version: 1.3.0
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-workflow-1.2.9/lib/idds_workflow.egg-info/SOURCES.txt` & `idds-workflow-1.3.0/lib/idds_workflow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 lib/idds/workflow/version.py
 lib/idds/workflow/work.py
 lib/idds/workflow/workflow.py
 lib/idds/workflowv2/__init__.py
 lib/idds/workflowv2/base.py
 lib/idds/workflowv2/datawork.py
 lib/idds/workflowv2/processingwork.py
+lib/idds/workflowv2/tree.py
 lib/idds/workflowv2/utils.py
 lib/idds/workflowv2/version.py
 lib/idds/workflowv2/work.py
 lib/idds/workflowv2/workflow.py
 lib/idds_workflow.egg-info/PKG-INFO
 lib/idds_workflow.egg-info/SOURCES.txt
 lib/idds_workflow.egg-info/dependency_links.txt
```

### Comparing `idds-workflow-1.2.9/setup.py` & `idds-workflow-1.3.0/setup.py`

 * *Files identical despite different names*


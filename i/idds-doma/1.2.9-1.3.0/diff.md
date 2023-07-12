# Comparing `tmp/idds-doma-1.2.9.tar.gz` & `tmp/idds-doma-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-doma-1.2.9.tar", last modified: Sat Apr 29 19:24:59 2023, max compression
+gzip compressed data, was "idds-doma-1.3.0.tar", last modified: Wed Jul 12 16:01:39 2023, max compression
```

## Comparing `idds-doma-1.2.9.tar` & `idds-doma-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-29 19:24:44.000000 idds-doma-1.2.9/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-29 19:24:59.595692 idds-doma-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-29 19:24:44.000000 idds-doma-1.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-04-29 19:24:44.000000 idds-doma-1.2.9/bin/setup_panda_token
--rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-04-29 19:24:44.000000 idds-doma-1.2.9/bin/setup_panda_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-doma-1.2.9/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/lib/idds/doma/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-doma-1.2.9/lib/idds/doma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 19:24:53.000000 idds-doma-1.2.9/lib/idds/doma/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/lib/idds/doma/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-doma-1.2.9/lib/idds/doma/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-04-29 19:24:44.000000 idds-doma-1.2.9/lib/idds/doma/workflow/domapandawork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/lib/idds/doma/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 19:24:44.000000 idds-doma-1.2.9/lib/idds/doma/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68326 2023-04-29 19:24:44.000000 idds-doma-1.2.9/lib/idds/doma/workflowv2/domapandawork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/lib/idds_doma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-29 19:24:59.000000 idds-doma-1.2.9/lib/idds_doma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-29 19:24:59.000000 idds-doma-1.2.9/lib/idds_doma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 19:24:59.000000 idds-doma-1.2.9/lib/idds_doma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-29 19:24:59.000000 idds-doma-1.2.9/lib/idds_doma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 19:24:59.000000 idds-doma-1.2.9/lib/idds_doma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-29 19:24:59.595692 idds-doma-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-29 19:24:44.000000 idds-doma-1.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 19:24:59.595692 idds-doma-1.2.9/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-29 19:24:53.000000 idds-doma-1.2.9/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-12 16:01:25.000000 idds-doma-1.3.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-12 16:01:39.786002 idds-doma-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-12 16:01:25.000000 idds-doma-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-07-12 16:01:25.000000 idds-doma-1.3.0/bin/setup_panda_token
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-07-12 16:01:25.000000 idds-doma-1.3.0/bin/setup_panda_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.782002 idds-doma-1.3.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/lib/idds/doma/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-12 16:01:34.000000 idds-doma-1.3.0/lib/idds/doma/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/lib/idds/doma/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflow/domapandawork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/lib/idds/doma/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflowv2/domaeventmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39387 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflowv2/domapandaeswork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59948 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflowv2/domapandawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-07-12 16:01:25.000000 idds-doma-1.3.0/lib/idds/doma/workflowv2/domatree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/lib/idds_doma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-12 16:01:39.000000 idds-doma-1.3.0/lib/idds_doma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-12 16:01:39.000000 idds-doma-1.3.0/lib/idds_doma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:01:39.000000 idds-doma-1.3.0/lib/idds_doma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-12 16:01:39.000000 idds-doma-1.3.0/lib/idds_doma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 16:01:39.000000 idds-doma-1.3.0/lib/idds_doma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 16:01:39.786002 idds-doma-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-12 16:01:25.000000 idds-doma-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.786002 idds-doma-1.3.0/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-12 16:01:34.000000 idds-doma-1.3.0/tools/env/environment.yml
```

### Comparing `idds-doma-1.2.9/LICENSE.rst` & `idds-doma-1.3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.9/PKG-INFO` & `idds-doma-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
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

### Comparing `idds-doma-1.2.9/bin/setup_panda_token` & `idds-doma-1.3.0/bin/setup_panda_token`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.9/bin/setup_panda_token.py` & `idds-doma-1.3.0/bin/setup_panda_token.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.9/lib/idds/doma/workflow/domapandawork.py` & `idds-doma-1.3.0/lib/idds/doma/workflow/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.9/lib/idds/doma/workflowv2/domapandawork.py` & `idds-doma-1.3.0/lib/idds/doma/workflowv2/domapandawork.py`

 * *Files 9% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         self.dependency_map = dependency_map
         if self.dependency_map is None:
             self.dependency_map = {}
         self.dependency_map_deleted = []
         # self.logger.setLevel(logging.DEBUG)
 
         self.task_name = task_name
+        self.orig_task_name = self.task_name
         self.real_task_name = None
         self.set_work_name(task_name)
         self.task_queue = task_queue
         self.queue = queue
         self.dep_tasks_id_names_map = {}
         self.executable = executable
         self.processingType = processing_type
@@ -206,15 +207,15 @@
                 self.panda_auth_vo = panda_config.get('panda', 'panda_auth_vo')
                 os.environ['PANDA_AUTH_VO'] = self.panda_auth_vo
             if 'PANDA_CONFIG_ROOT' not in os.environ and panda_config.has_option('panda', 'panda_config_root'):
                 self.panda_config_root = panda_config.get('panda', 'panda_config_root')
                 os.environ['PANDA_CONFIG_ROOT'] = self.panda_config_root
 
     def set_agent_attributes(self, attrs, req_attributes=None):
-        if 'life_time' not in attrs[self.class_name] or int(attrs[self.class_name]['life_time']) <= 0:
+        if self.class_name in attrs and ('life_time' not in attrs[self.class_name] or int(attrs[self.class_name]['life_time']) <= 0):
             attrs['life_time'] = None
         super(DomaPanDAWork, self).set_agent_attributes(attrs)
         if 'num_retries' in self.agent_attributes and self.agent_attributes['num_retries']:
             self.num_retries = int(self.agent_attributes['num_retries'])
         if 'poll_panda_jobs_chunk_size' in self.agent_attributes and self.agent_attributes['poll_panda_jobs_chunk_size']:
             self.poll_panda_jobs_chunk_size = int(self.agent_attributes['poll_panda_jobs_chunk_size'])
 
@@ -529,25 +530,29 @@
         task_param_map['noWaitParent'] = True
         task_param_map['taskType'] = self.task_type
         task_param_map['coreCount'] = self.core_count
         task_param_map['skipScout'] = True
         task_param_map['cloud'] = self.task_cloud
         task_param_map['PandaSite'] = self.task_site
         if self.task_rss and self.task_rss > 0:
-            task_param_map['ramCount'] = self.task_rss
+            task_param_map['ramCount'] = self.task_rss / self.core_count if self.core_count else self.task_rss
             # task_param_map['ramUnit'] = 'MB'
             task_param_map['ramUnit'] = 'MBPerCoreFixed'
 
         # task_param_map['inputPreStaging'] = True
         task_param_map['prestagingRuleID'] = 123
         task_param_map['nChunksToWait'] = 1
         task_param_map['maxCpuCount'] = self.core_count
         task_param_map['maxWalltime'] = self.maxWalltime
         task_param_map['maxFailure'] = self.maxAttempt if self.maxAttempt else 5
         task_param_map['maxAttempt'] = self.maxAttempt if self.maxAttempt else 5
+        if task_param_map['maxAttempt'] < self.num_retries:
+            task_param_map['maxAttempt'] = self.num_retries
+        if task_param_map['maxFailure'] < self.num_retries:
+            task_param_map['maxFailure'] = self.num_retries
         task_param_map['log'] = self.task_log
         task_param_map['jobParameters'] = [
             {'type': 'constant',
              'value': executable,  # noqa: E501
              },
         ]
 
@@ -669,17 +674,20 @@
         elif task_status in ['running', 'toretry', 'toincexec', 'throttled']:
             processing_status = ProcessingStatus.Running
         elif task_status in ['done']:
             processing_status = ProcessingStatus.Finished
         elif task_status in ['finished', 'paused']:
             # finished, finishing, waiting it to be done
             processing_status = ProcessingStatus.SubFinished
-        elif task_status in ['failed', 'aborted', 'exhausted']:
+        elif task_status in ['failed', 'exhausted']:
             # aborting, tobroken
             processing_status = ProcessingStatus.Failed
+        elif task_status in ['aborted']:
+            # aborting, tobroken
+            processing_status = ProcessingStatus.Cancelled
         elif task_status in ['broken']:
             processing_status = ProcessingStatus.Broken
         else:
             # finished, finishing, aborting, topreprocess, preprocessing, tobroken
             # toretry, toincexec, rerefine, paused, throttled, passed
             processing_status = ProcessingStatus.Submitted
         return processing_status
@@ -722,59 +730,14 @@
                     if content['status'] not in [ContentStatus.Available]:
                         update_content = {'content_id': content['content_id'],
                                           'status': ContentStatus.New,
                                           'substatus': ContentStatus.New}
                         updated_contents.append(update_content)
         return updated_contents
 
-    def sort_panda_jobids(self, input_output_maps):
-        panda_job_ids = {}
-        panda_id_to_map_ids = {}
-        map_id_without_panda_ids = []
-        for map_id in input_output_maps:
-            outputs = input_output_maps[map_id]['outputs']
-            for content in outputs:
-                if content['status'] not in panda_job_ids:
-                    panda_job_ids[content['status']] = []
-
-                if 'panda_id' in content['content_metadata']:
-                    panda_job_ids[content['status']].append(content['content_metadata']['panda_id'])
-                    panda_id_to_map_ids[content['content_metadata']['panda_id']] = map_id
-                else:
-                    map_id_without_panda_ids.append(map_id)
-
-        return panda_job_ids, map_id_without_panda_ids, panda_id_to_map_ids
-
-    def get_registered_panda_jobids(self, input_output_maps):
-        panda_job_ids, map_id_without_panda_ids, panda_id_to_map_ids = self.sort_panda_jobids(input_output_maps)
-        unterminated_panda_ids = []
-        finished_panda_ids = []
-        failed_panda_ids = []
-        for key in panda_job_ids:
-            if key in [ContentStatus.Available]:
-                finished_panda_ids += panda_job_ids[key]
-            elif key in [ContentStatus.Failed, ContentStatus.FinalFailed,
-                         ContentStatus.Lost, ContentStatus.Deleted,
-                         ContentStatus.Missing]:
-                failed_panda_ids += panda_job_ids[key]
-            else:
-                unterminated_panda_ids += panda_job_ids[key]
-        return finished_panda_ids + failed_panda_ids, unterminated_panda_ids, map_id_without_panda_ids, panda_id_to_map_ids
-
-    def get_map_id_from_input(self, input_output_maps, input_file):
-        map_keys = list(input_output_maps.keys())
-        map_keys.reverse()
-        for map_id in map_keys:
-            inputs = input_output_maps[map_id]['inputs']
-            # outputs = input_output_maps[map_id]['outputs']
-            for content in inputs:
-                if content['name'] == input_file:
-                    return map_id
-        return None
-
     def get_content_status_from_panda_status(self, job_info):
         if job_info is None:
             return ContentStatus.Processing
 
         jobstatus = job_info.jobStatus
         if jobstatus in ['finished', 'merging']:
             return ContentStatus.Available
@@ -782,40 +745,61 @@
             attempt_nr = int(job_info.attemptNr) if job_info.attemptNr else 0
             max_attempt = int(job_info.maxAttempt) if job_info.maxAttempt else 0
             self_maxAttempt = int(self.maxAttempt) if self.maxAttempt else 0
             if (attempt_nr >= max_attempt) and (attempt_nr >= self_maxAttempt):
                 return ContentStatus.FinalFailed
             else:
                 return ContentStatus.Failed
+        elif jobstatus in ['activated']:
+            return ContentStatus.Activated
         else:
             return ContentStatus.Processing
 
-    def get_update_contents_from_map_id(self, map_id, input_output_maps, job_info):
-        outputs = input_output_maps[map_id]['outputs']
-        update_contents = []
-        for content in outputs:
-            status = self.get_content_status_from_panda_status(job_info)
-            content['substatus'] = status
-
-            if 'panda_id' in content['content_metadata'] and content['content_metadata']['panda_id']:
-                # if content['content_metadata']['panda_id'] != job_info.PandaID:
-                if content['content_metadata']['panda_id'] < job_info.PandaID:
-                    # new panda id is the bigger one.
-                    if 'old_panda_id' not in content['content_metadata']:
-                        content['content_metadata']['old_panda_id'] = []
-                    if content['content_metadata']['panda_id'] not in content['content_metadata']['old_panda_id']:
-                        content['content_metadata']['old_panda_id'].append(content['content_metadata']['panda_id'])
-            content['content_metadata']['panda_id'] = job_info.PandaID
-
-            update_contents.append(content)
-        return update_contents
-
-    def get_panda_job_status(self, jobids):
-        jobids = list(jobids)
-        self.logger.debug("get_panda_job_status, jobids[:10]: %s" % str(jobids[:10]))
+    def get_unterminated_jobs(self, all_jobs_ids, input_output_maps, contents_ext):
+        finished_jobs, failed_jobs = [], []
+
+        contents_ext_dict = {content['content_id']: content for content in contents_ext}
+
+        for map_id in input_output_maps:
+            outputs = input_output_maps[map_id]['outputs']
+            for content in outputs:
+                if content['substatus'] in [ContentStatus.Available]:
+                    if 'panda_id' in content['content_metadata']:
+                        panda_id = content['content_metadata']['panda_id']
+                        if content['content_id'] not in contents_ext_dict:
+                            continue
+
+                        content_ext = contents_ext_dict[content['content_id']]
+                        if content['substatus'] != content_ext['status'] or panda_id != content_ext['panda_id']:
+                            continue
+
+                        if panda_id not in finished_jobs:
+                            finished_jobs.append(panda_id)
+                elif content['substatus'] in [ContentStatus.FinalFailed,
+                                              ContentStatus.Lost, ContentStatus.Deleted,
+                                              ContentStatus.Missing]:
+                    if 'panda_id' in content['content_metadata']:
+                        panda_id = content['content_metadata']['panda_id']
+                        if content['content_id'] not in contents_ext_dict:
+                            continue
+
+                        content_ext = contents_ext_dict[content['content_id']]
+                        if content['substatus'] != content_ext['status'] or panda_id != content_ext['panda_id']:
+                            continue
+
+                        if panda_id not in failed_jobs:
+                            failed_jobs.append(panda_id)
+
+        all_jobs_ids = set(all_jobs_ids)
+        terminated_jobs = set(finished_jobs + failed_jobs)
+        unterminated_jobs = all_jobs_ids - terminated_jobs
+        return list(unterminated_jobs)
+
+    def get_panda_job_status(self, jobids, log_prefix=''):
+        self.logger.debug(log_prefix + "get_panda_job_status, jobids[:10]: %s" % str(jobids[:10]))
         try:
             from pandaclient import Client
             ret = Client.getJobStatus(jobids, verbose=0)
             if ret[0] == 0:
                 left_jobids = []
                 ret_jobs = []
                 jobs_list = ret[1]
@@ -830,296 +814,158 @@
                         if ret1[0] == 0:
                             left_jobs_list = ret1[1]
                         ret_jobs = ret_jobs + left_jobs_list
                     except Exception as ex:
                         self.logger.error(str(ex))
                         self.logger.error(traceback.format_exc())
                 return ret_jobs
+            else:
+                self.logger.warn(log_prefix + "get_panda_job_status failed: %s" % str(ret))
+                return []
         except Exception as ex:
             self.logger.error(str(ex))
             self.logger.error(traceback.format_exc())
         return []
 
-    def map_panda_ids(self, unregistered_job_ids, input_output_maps):
-        self.logger.debug("map_panda_ids, unregistered_job_ids[:10]: %s" % str(unregistered_job_ids[:10]))
-
-        # updated_map_ids = []
-        full_update_contents = []
-        chunksize = 2000
-        chunks = [unregistered_job_ids[i:i + chunksize] for i in range(0, len(unregistered_job_ids), chunksize)]
-        for chunk in chunks:
-            # jobs_list = Client.getJobStatus(chunk, verbose=0)[1]
-            jobs_list = self.get_panda_job_status(chunk)
-            for job_info in jobs_list:
-                if job_info and job_info.Files and len(job_info.Files) > 0:
-                    for job_file in job_info.Files:
-                        # if job_file.type in ['log']:
-                        if job_file.type not in ['pseudo_input']:
-                            continue
-                        if ':' in job_file.lfn:
-                            pos = job_file.lfn.find(":")
-                            input_file = job_file.lfn[pos + 1:]
-                            # input_file = job_file.lfn.split(':')[1]
-                        else:
-                            input_file = job_file.lfn
-                        map_id = self.get_map_id_from_input(input_output_maps, input_file)
-                        if map_id:
-                            update_contents = self.get_update_contents_from_map_id(map_id, input_output_maps, job_info)
-                            full_update_contents += update_contents
-        return full_update_contents
-
-    def get_status_changed_contents(self, unterminated_job_ids, input_output_maps, panda_id_to_map_ids):
-        self.logger.debug("get_status_changed_contents, unterminated_job_ids[:10]: %s" % str(unterminated_job_ids[:10]))
-
-        full_update_contents = []
-        chunksize = 2000
-        chunks = [unterminated_job_ids[i:i + chunksize] for i in range(0, len(unterminated_job_ids), chunksize)]
-        for chunk in chunks:
-            # jobs_list = Client.getJobStatus(chunk, verbose=0)[1]
-            jobs_list = self.get_panda_job_status(chunk)
-            for job_info in jobs_list:
-                panda_id = job_info.PandaID
-                map_id = panda_id_to_map_ids[panda_id]
-                update_contents = self.get_update_contents_from_map_id(map_id, input_output_maps, job_info)
-                full_update_contents += update_contents
-        return full_update_contents
-
-    def get_final_update_contents(self, input_output_maps):
-        update_contents = []
-        for map_id in input_output_maps:
-            outputs = input_output_maps[map_id]['outputs'] if 'outputs' in input_output_maps[map_id] else []
-            for content in outputs:
-                if (content['substatus'] not in [ContentStatus.Available, ContentStatus.FakeAvailable, ContentStatus.FinalFailed]):
-                    content['content_metadata']['old_final_status'] = content['substatus']
-                    content['substatus'] = ContentStatus.FinalFailed
-                    update_contents.append(content)
-
-        return update_contents
-
-    def poll_panda_jobs(self, job_ids):
-        job_ids = list(job_ids)
-        self.logger.debug("poll_panda_jobs, poll_panda_jobs_chunk_size: %s, job_ids[:10]: %s" % (self.poll_panda_jobs_chunk_size, str(job_ids[:10])))
-
-        # updated_map_ids = []
-        inputname_jobid_map = {}
+    def poll_panda_jobs(self, job_ids, log_prefix=''):
+        job_status_info = {}
+        self.logger.debug(log_prefix + "poll_panda_jobs, poll_panda_jobs_chunk_size: %s, job_ids[:10]: %s" % (self.poll_panda_jobs_chunk_size, str(job_ids[:10])))
         chunksize = self.poll_panda_jobs_chunk_size
         chunks = [job_ids[i:i + chunksize] for i in range(0, len(job_ids), chunksize)]
         for chunk in chunks:
             # jobs_list = Client.getJobStatus(chunk, verbose=0)[1]
-            jobs_list = self.get_panda_job_status(chunk)
+            jobs_list = self.get_panda_job_status(chunk, log_prefix=log_prefix)
             if jobs_list:
-                self.logger.debug("poll_panda_jobs, input jobs: %s, output_jobs: %s" % (len(chunk), len(jobs_list)))
+                self.logger.debug(log_prefix + "poll_panda_jobs, input jobs: %s, output_jobs: %s" % (len(chunk), len(jobs_list)))
                 for job_info in jobs_list:
                     job_status = self.get_content_status_from_panda_status(job_info)
                     if job_info and job_info.Files and len(job_info.Files) > 0:
                         for job_file in job_info.Files:
                             # if job_file.type in ['log']:
                             if job_file.type not in ['pseudo_input']:
                                 continue
                             if ':' in job_file.lfn:
                                 pos = job_file.lfn.find(":")
                                 input_file = job_file.lfn[pos + 1:]
                                 # input_file = job_file.lfn.split(':')[1]
                             else:
                                 input_file = job_file.lfn
-                            inputname_jobid_map[input_file] = {'panda_id': job_info.PandaID, 'status': job_status, 'job_info': job_info}
+                            job_status_info[input_file] = {'panda_id': job_info.PandaID, 'status': job_status, 'job_info': job_info}
             else:
-                self.logger.warn("poll_panda_jobs, input jobs: %s, output_jobs: %s" % (len(chunk), jobs_list))
-        return inputname_jobid_map
+                self.logger.warn(log_prefix + "poll_panda_jobs, input jobs: %s, output_jobs: %s" % (len(chunk), jobs_list))
+        return job_status_info
 
-    def get_job_maps(self, input_output_maps):
-        inputname_mapid_map = {}
-        finished_jobs, failed_jobs = [], []
+    def get_update_contents(self, unterminated_jobs_status, input_output_maps, contents_ext, job_info_maps, abort=False, log_prefix=''):
+        inputname_to_map_id_outputs = {}
         for map_id in input_output_maps:
             inputs = input_output_maps[map_id]['inputs']
             outputs = input_output_maps[map_id]['outputs']
-            for content in outputs:
-                if content['substatus'] in [ContentStatus.Available]:
-                    if 'panda_id' in content['content_metadata']:
-                        finished_jobs.append(content['content_metadata']['panda_id'])
-                elif content['substatus'] in [ContentStatus.FinalFailed,
-                                              ContentStatus.Lost, ContentStatus.Deleted,
-                                              ContentStatus.Missing]:
-                    if 'panda_id' in content['content_metadata']:
-                        failed_jobs.append(content['content_metadata']['panda_id'])
             for content in inputs:
-                inputname_mapid_map[content['name']] = {'map_id': map_id,
-                                                        'outputs': outputs}
-        return finished_jobs + failed_jobs, inputname_mapid_map
-
-    def get_update_contents(self, inputnames, inputname_mapid_map, inputname_jobid_map):
-        self.logger.debug("get_update_contents, inputnames[:5]: %s" % str(inputnames[:5]))
-        # self.logger.debug("get_update_contents, inputname_mapid_map[:5]: %s" % str({k: inputname_mapid_map[k] for k in inputnames[:5]}))
-        self.logger.debug("get_update_contents, inputname_jobid_map[:3]: %s" % str({k: inputname_jobid_map[k] for k in inputnames[:3]}))
+                inputname_to_map_id_outputs[content['name']] = {'map_id': map_id, 'outputs': outputs}
 
-        update_contents = []
-        update_contents_full = []
-        contents_ext_full = {}
-        num_updated_contents, num_unupdated_contents = 0, 0
-        for inputname in inputnames:
-            panda_id_status = inputname_jobid_map[inputname]
-            panda_id = panda_id_status['panda_id']
-            panda_status = panda_id_status['status']
-            job_info = panda_id_status['job_info']
-            map_id_contents = inputname_mapid_map[inputname]
-            contents = map_id_contents['outputs']
-            for content in contents:
-                if content['substatus'] != panda_status:
-                    # content['status'] = panda_status
-                    content['substatus'] = panda_status
-                    update_contents_full.append(content)
-                    update_content = {'content_id': content['content_id'],
-                                      # 'status': panda_status,
-                                      'substatus': panda_status}
-                    # 'content_metadata': content['content_metadata']
-                    if 'panda_id' in content['content_metadata'] and content['content_metadata']['panda_id']:
-                        # if content['content_metadata']['panda_id'] != job_info.PandaID:
-                        if content['content_metadata']['panda_id'] < panda_id:
-                            # new panda id is the bigger one.
-                            if 'old_panda_id' not in content['content_metadata']:
-                                content['content_metadata']['old_panda_id'] = []
-                            if content['content_metadata']['panda_id'] not in content['content_metadata']['old_panda_id']:
-                                content['content_metadata']['old_panda_id'].append(content['content_metadata']['panda_id'])
-                            content['content_metadata']['panda_id'] = panda_id
-                            # content['status'] = panda_status
-                            content['substatus'] = panda_status
-                            update_content['content_metadata'] = content['content_metadata']
-                        elif content['content_metadata']['panda_id'] > panda_id:
-                            if 'old_panda_id' not in content['content_metadata']:
-                                content['content_metadata']['old_panda_id'] = []
-                            if panda_id not in content['content_metadata']['old_panda_id']:
-                                content['content_metadata']['old_panda_id'].append(panda_id)
-                            # content['content_metadata']['panda_id'] = content['content_metadata']['panda_id']
-                            # content['substatus'] = panda_status
-                            update_content['content_metadata'] = content['content_metadata']
-                        else:
-                            pass
-                            # content['content_metadata']['panda_id'] = panda_id
-                            content['substatus'] = panda_status
-                    else:
+        contents_ext_dict = {content['content_id']: content for content in contents_ext}
+
+        update_contents, update_contents_full = [], []
+        new_contents_ext, update_contents_ext = [], []
+        update_contents_dict, new_contents_ext_dict = {}, {}
+        for input_file in unterminated_jobs_status:
+            panda_job_status = unterminated_jobs_status[input_file]
+            panda_id = panda_job_status['panda_id']
+            panda_status = panda_job_status['status']
+            job_info = panda_job_status['job_info']
+
+            output_contents = inputname_to_map_id_outputs[input_file]['outputs']
+            for content in output_contents:
+                content['substatus'] = panda_status
+                update_contents_full.append(content)
+                update_content = {'content_id': content['content_id'],
+                                  # 'status': panda_status,
+                                  'substatus': panda_status}
+
+                if 'panda_id' in content['content_metadata'] and content['content_metadata']['panda_id']:
+                    if content['content_metadata']['panda_id'] < panda_id:
+                        # new panda id is the bigger one.
+                        if 'old_panda_id' not in content['content_metadata']:
+                            content['content_metadata']['old_panda_id'] = []
+                        if content['content_metadata']['panda_id'] not in content['content_metadata']['old_panda_id']:
+                            content['content_metadata']['old_panda_id'].append(content['content_metadata']['panda_id'])
                         content['content_metadata']['panda_id'] = panda_id
-                        content['substatus'] = panda_status
                         update_content['content_metadata'] = content['content_metadata']
-
-                    update_contents.append(update_content)
-                    num_updated_contents += 1
+                    elif content['content_metadata']['panda_id'] > panda_id:
+                        if 'old_panda_id' not in content['content_metadata']:
+                            content['content_metadata']['old_panda_id'] = []
+                        if panda_id not in content['content_metadata']['old_panda_id']:
+                            content['content_metadata']['old_panda_id'].append(panda_id)
+                        # content['content_metadata']['panda_id'] = content['content_metadata']['panda_id']
+                        # content['substatus'] = panda_status
+                        update_content['content_metadata'] = content['content_metadata']
+                    else:
+                        pass
                 else:
-                    # num_unupdated_contents += 1
-                    pass
+                    content['content_metadata']['panda_id'] = panda_id
+                    update_content['content_metadata'] = content['content_metadata']
+
+                update_contents.append(update_content)
+                update_contents_dict[update_content['content_id']] = update_content
 
                 if panda_status in [ContentStatus.Available, ContentStatus.Failed, ContentStatus.FinalFailed,
                                     ContentStatus.Lost, ContentStatus.Deleted, ContentStatus.Missing]:
-                    contents_ext_full[content['content_id']] = {'content': content, 'job_info': job_info}
-
-        self.logger.debug("get_update_contents, num_updated_contents: %s, num_unupdated_contents: %s" % (num_updated_contents, num_unupdated_contents))
-        self.logger.debug("get_update_contents, update_contents[:3]: %s" % (str(update_contents[:3])))
-        self.logger.debug("get_update_contents, contents_ext_full[:3]: %s" % (str({k: contents_ext_full[k] for k in list(contents_ext_full.keys())[:3]})))
-        return update_contents, update_contents_full, contents_ext_full
-
-    def get_contents_ext_detail(self, new_contents_ext, update_contents_ext, job_info_maps={}):
-        new_contents_ext_d, update_contents_ext_d = [], []
-
-        for content_id in new_contents_ext:
-            content = new_contents_ext[content_id]['content']
-            job_info = new_contents_ext[content_id]['job_info']
-            new_content_ext_d = {'content_id': content['content_id'],
-                                 'request_id': content['request_id'],
-                                 'transform_id': content['transform_id'],
-                                 'workload_id': content['workload_id'],
-                                 'coll_id': content['coll_id'],
-                                 'map_id': content['map_id'],
-                                 'status': content['status']}
-            for job_info_item in job_info_maps:
-                new_content_ext_d[job_info_item] = getattr(job_info, job_info_maps[job_info_item])
-                if new_content_ext_d[job_info_item] == 'NULL':
-                    new_content_ext_d[job_info_item] = None
-                if new_content_ext_d[job_info_item] is None:
-                    del new_content_ext_d[job_info_item]
-
-            new_contents_ext_d.append(new_content_ext_d)
-
-        for content_id in update_contents_ext:
-            content = update_contents_ext[content_id]['content']
-            job_info = update_contents_ext[content_id]['job_info']
-            update_content_ext_d = {'content_id': content['content_id'],
-                                    'status': content['status']}
-            for job_info_item in job_info_maps:
-                update_content_ext_d[job_info_item] = getattr(job_info, job_info_maps[job_info_item])
-                if update_content_ext_d[job_info_item] == 'NULL':
-                    update_content_ext_d[job_info_item] = None
-                if update_content_ext_d[job_info_item] is None:
-                    del update_content_ext_d[job_info_item]
-
-            update_contents_ext_d.append(update_content_ext_d)
-
-        return new_contents_ext_d, update_contents_ext_d
-
-    def get_contents_ext(self, input_output_maps, contents_ext, contents_ext_full, job_info_maps={}):
-        self.logger.debug("get_contents_ext, len(contents_ext): %s" % (str(len(contents_ext))))
-        self.logger.debug("get_contents_ext, contents_ext[:3]: %s" % (str(contents_ext[:3])))
-
-        contents_ext_dict = {content['content_id']: content for content in contents_ext}
-
-        left_contents = []
-        to_check_panda_ids = {}
-        new_contents_ext, update_contents_ext = {}, {}
-        new_need_poll_contents_ext, update_need_poll_contents_ext = {}, {}
-
-        for map_id in input_output_maps:
-            # inputs = input_output_maps[map_id]['inputs']
-            outputs = input_output_maps[map_id]['outputs']
-
-            for content in outputs:
-                if content['substatus'] in [ContentStatus.Available, ContentStatus.Failed, ContentStatus.FinalFailed,
-                                            ContentStatus.Lost, ContentStatus.Deleted, ContentStatus.Missing]:
                     if content['content_id'] not in contents_ext_dict:
-                        if content['content_id'] in contents_ext_full:
-                            new_contents_ext[content['content_id']] = contents_ext_full[content['content_id']]
-                        else:
-                            new_need_poll_contents_ext[content['content_id']] = content
-                            if content['content_metadata'] and 'panda_id' in content['content_metadata']:
-                                to_check_panda_ids[content['content_metadata']['panda_id']] = content['content_id']
+                        new_content_ext = {'content_id': content['content_id'],
+                                           'request_id': content['request_id'],
+                                           'transform_id': content['transform_id'],
+                                           'workload_id': content['workload_id'],
+                                           'coll_id': content['coll_id'],
+                                           'map_id': content['map_id'],
+                                           'status': panda_status}
+                        for job_info_item in job_info_maps:
+                            new_content_ext[job_info_item] = getattr(job_info, job_info_maps[job_info_item])
+                            if new_content_ext[job_info_item] == 'NULL':
+                                new_content_ext[job_info_item] = None
+                            if new_content_ext[job_info_item] is None:
+                                del new_content_ext[job_info_item]
+                        new_contents_ext.append(new_content_ext)
+                        new_contents_ext_dict[new_content_ext['content_id']] = new_content_ext
                     else:
-                        content_ext = contents_ext_dict[content['content_id']]
-                        panda_id = None
-                        if content['content_metadata'] and 'panda_id' in content['content_metadata']:
-                            panda_id = content['content_metadata']['panda_id']
-                        if content['substatus'] != content_ext['status'] or panda_id != content_ext['panda_id']:
-                            if content['content_id'] in contents_ext_full:
-                                update_contents_ext[content['content_id']] = contents_ext_full[content['content_id']]
-                            else:
-                                update_need_poll_contents_ext[content['content_id']] = content
-                                if panda_id:
-                                    to_check_panda_ids[panda_id] = content['content_id']
-                else:
-                    left_contents.append(content)
+                        update_content_ext = {'content_id': content['content_id'],
+                                              'status': panda_status}
+                        for job_info_item in job_info_maps:
+                            update_content_ext[job_info_item] = getattr(job_info, job_info_maps[job_info_item])
+                            if update_content_ext[job_info_item] == 'NULL':
+                                update_content_ext[job_info_item] = None
+                            if update_content_ext[job_info_item] is None:
+                                del update_content_ext[job_info_item]
+                        update_contents_ext.append(update_content_ext)
+
+        if abort:
+            for map_id in input_output_maps:
+                outputs = input_output_maps[map_id]['outputs']
+                for content in outputs:
+                    if content['substatus'] not in [ContentStatus.Available, ContentStatus.Failed, ContentStatus.FinalFailed,
+                                                    ContentStatus.Lost, ContentStatus.Deleted, ContentStatus.Missing]:
+                        if content['content_id'] not in update_contents_dict:
+                            update_content = {'content_id': content['content_id'],
+                                              'substatus': ContentStatus.Missing}
+                            update_contents.append(update_content)
+                        if content['content_id'] not in contents_ext_dict and content['content_id'] not in new_contents_ext_dict:
+                            new_content_ext = {'content_id': content['content_id'],
+                                               'request_id': content['request_id'],
+                                               'transform_id': content['transform_id'],
+                                               'workload_id': content['workload_id'],
+                                               'coll_id': content['coll_id'],
+                                               'map_id': content['map_id'],
+                                               'status': ContentStatus.Missing}
+                            new_contents_ext.append(new_content_ext)
 
-        if to_check_panda_ids:
-            to_check_panda_ids_list = list(to_check_panda_ids.keys())
-            ret_job_infos = self.get_panda_job_status(to_check_panda_ids_list)
-            for job_info in ret_job_infos:
-                content_id = to_check_panda_ids[job_info.PandaID]
-                del to_check_panda_ids[job_info.PandaID]
-                if content_id in new_need_poll_contents_ext:
-                    new_contents_ext[content_id] = {'content': new_need_poll_contents_ext[content_id], 'job_info': job_info}
-                    del new_need_poll_contents_ext[content_id]
-                else:
-                    update_contents_ext[content_id] = {'content': update_need_poll_contents_ext[content_id], 'job_info': job_info}
-                    del update_need_poll_contents_ext[content_id]
-        for content_id in new_need_poll_contents_ext:
-            left_contents.append(new_need_poll_contents_ext[content_id])
-        for content_id in update_need_poll_contents_ext:
-            left_contents.append(update_need_poll_contents_ext[content_id])
-
-        new_contents_ext_d, update_contents_ext_d = self.get_contents_ext_detail(new_contents_ext, update_contents_ext, job_info_maps)
-
-        self.logger.debug("get_contents_ext, new_contents_ext_d[:1]: %s" % (str(new_contents_ext_d[:1])))
-        self.logger.debug("get_contents_ext, update_contents_ext_d[:1]: %s" % (str(update_contents_ext_d[:1])))
-        self.logger.debug("get_contents_ext, left_contents[:1]: %s" % (str(left_contents[:3])))
-        return new_contents_ext_d, update_contents_ext_d, left_contents
+        self.logger.debug("get_update_contents, num_update_contents: %s" % (len(update_contents)))
+        self.logger.debug("get_update_contents, update_contents[:3]: %s" % (str(update_contents[:3])))
+        self.logger.debug("get_update_contents, new_contents_ext[:1]: %s" % (str(new_contents_ext[:1])))
+        self.logger.debug("get_update_contents, update_contents_ext[:1]: %s" % (str(update_contents_ext[:1])))
+
+        return update_contents, update_contents_full, new_contents_ext, update_contents_ext
 
     def poll_panda_task(self, processing=None, input_output_maps=None, contents_ext=None, job_info_maps={}, log_prefix=''):
         task_id = None
         try:
             from pandaclient import Client
 
             if processing:
@@ -1140,32 +986,23 @@
                     task_info = task_info[1]
 
                     processing_status = self.get_processing_status_from_panda_status(task_info["status"])
                     self.logger.info(log_prefix + "poll_panda_task processing_status: %s" % processing_status)
 
                     all_jobs_ids = task_info['PandaID']
 
-                    terminated_jobs, inputname_mapid_map = self.get_job_maps(input_output_maps)
-                    self.logger.debug(log_prefix + "poll_panda_task, task_id: %s, all jobs: %s, terminated_jobs: %s" % (str(task_id), len(all_jobs_ids), len(terminated_jobs)))
+                    unterminated_jobs = self.get_unterminated_jobs(all_jobs_ids, input_output_maps, contents_ext)
+                    self.logger.debug(log_prefix + "poll_panda_task, task_id: %s, all jobs: %s, unterminated_jobs: %s" % (str(task_id), len(all_jobs_ids), len(unterminated_jobs)))
 
-                    all_jobs_ids = set(all_jobs_ids)
-                    terminated_jobs = set(terminated_jobs)
-                    unterminated_jobs = all_jobs_ids - terminated_jobs
-
-                    inputname_jobid_map = self.poll_panda_jobs(unterminated_jobs)
-                    intersection_keys = set(inputname_mapid_map.keys()) & set(inputname_jobid_map.keys())
-
-                    updated_contents, update_contents_full, contents_ext_full = self.get_update_contents(list(intersection_keys),
-                                                                                                         inputname_mapid_map,
-                                                                                                         inputname_jobid_map)
-
-                    new_contents_ext, update_contents_ext, left_contents = self.get_contents_ext(input_output_maps, contents_ext,
-                                                                                                 contents_ext_full, job_info_maps)
-                    # if left_jobs:
-                    #     processing_status = ProcessingStatus.Running
+                    unterminated_jobs_status = self.poll_panda_jobs(unterminated_jobs, log_prefix=log_prefix)
+                    abort_status = False
+                    if processing_status in [ProcessingStatus.Cancelled]:
+                        abort_status = True
+                    ret_contents = self.get_update_contents(unterminated_jobs_status, input_output_maps, contents_ext, job_info_maps, abort=abort_status, log_prefix=log_prefix)
+                    updated_contents, update_contents_full, new_contents_ext, update_contents_ext = ret_contents
 
                     return processing_status, updated_contents, update_contents_full, new_contents_ext, update_contents_ext
                 else:
                     self.logger.error("poll_panda_task, task_id (%s) cannot be found" % task_id)
                     return ProcessingStatus.Failed, [], [], [], []
         except Exception as ex:
             msg = "Failed to check the processing (%s) status: %s" % (str(processing['processing_id']), str(ex))
@@ -1242,14 +1079,27 @@
 
     def resume_processing(self, processing, log_prefix=''):
         self.reactivate_processing(processing, log_prefix=log_prefix)
 
     def require_ext_contents(self):
         return True
 
+    def has_external_content_id(self):
+        return True
+
+    def get_external_content_ids(self, processing, log_prefix=''):
+        if processing:
+            from pandaclient import Client
+            proc = processing['processing_metadata']['processing']
+            task_id = proc.workload_id
+            status, output = Client.get_files_in_datasets(task_id, verbose=False)
+            if status == 0:
+                return output
+        return []
+
     def poll_processing_updates(self, processing, input_output_maps, contents_ext=None, job_info_maps={}, log_prefix=''):
         """
         *** Function called by Carrier agent.
         """
         update_contents = []
         update_contents_full = []
         self.logger.debug(log_prefix + "poll_processing_updates, input_output_maps.keys[:3]: %s" % str(list(input_output_maps.keys())[:3]))
```

### Comparing `idds-doma-1.2.9/lib/idds_doma.egg-info/PKG-INFO` & `idds-doma-1.3.0/lib/idds_doma.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
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

### Comparing `idds-doma-1.2.9/lib/idds_doma.egg-info/SOURCES.txt` & `idds-doma-1.3.0/lib/idds_doma.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 bin/setup_panda_token.py
 lib/idds/__init__.py
 lib/idds/doma/__init__.py
 lib/idds/doma/version.py
 lib/idds/doma/workflow/__init__.py
 lib/idds/doma/workflow/domapandawork.py
 lib/idds/doma/workflowv2/__init__.py
+lib/idds/doma/workflowv2/domaeventmap.py
+lib/idds/doma/workflowv2/domapandaeswork.py
 lib/idds/doma/workflowv2/domapandawork.py
+lib/idds/doma/workflowv2/domatree.py
 lib/idds_doma.egg-info/PKG-INFO
 lib/idds_doma.egg-info/SOURCES.txt
 lib/idds_doma.egg-info/dependency_links.txt
 lib/idds_doma.egg-info/requires.txt
 lib/idds_doma.egg-info/top_level.txt
 tools/env/environment.yml
```

### Comparing `idds-doma-1.2.9/setup.py` & `idds-doma-1.3.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/prophecy-build-tool-1.1.3.tar.gz` & `tmp/prophecy-build-tool-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prophecy-build-tool/prophecy-build-tool/dist/.tmp-2mqlfswu/prophecy-build-tool-1.1.3.tar", last modified: Tue Jun 27 07:26:51 2023, max compression
+gzip compressed data, was "/home/runner/work/prophecy-build-tool/prophecy-build-tool/dist/.tmp-5mvmk7l4/prophecy-build-tool-1.1.4.tar", last modified: Wed Jul 12 16:16:39 2023, max compression
```

## Comparing `prophecy-build-tool-1.1.3.tar` & `prophecy-build-tool-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/pbt/
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/src/pbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/src/pbt/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    39198 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/src/pbt/prophecy_build_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:26:51.000000 prophecy-build-tool-1.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-27 07:21:52.000000 prophecy-build-tool-1.1.3/test/test_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:16:39.000000 prophecy-build-tool-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 16:12:05.000000 prophecy-build-tool-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-12 16:16:39.000000 prophecy-build-tool-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-12 16:12:05.000000 prophecy-build-tool-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-12 16:12:05.000000 prophecy-build-tool-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-12 16:16:39.000000 prophecy-build-tool-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-12 16:12:05.000000 prophecy-build-tool-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:16:39.000000 prophecy-build-tool-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:16:39.000000 prophecy-build-tool-1.1.4/src/pbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-12 16:12:05.000000 prophecy-build-tool-1.1.4/src/pbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-12 16:12:05.000000 prophecy-build-tool-1.1.4/src/pbt/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39366 2023-07-12 16:12:05.000000 prophecy-build-tool-1.1.4/src/pbt/prophecy_build_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:16:39.000000 prophecy-build-tool-1.1.4/src/prophecy_build_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-12 16:16:39.000000 prophecy-build-tool-1.1.4/src/prophecy_build_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-12 16:16:39.000000 prophecy-build-tool-1.1.4/src/prophecy_build_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:16:39.000000 prophecy-build-tool-1.1.4/src/prophecy_build_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-12 16:16:39.000000 prophecy-build-tool-1.1.4/src/prophecy_build_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-12 16:16:39.000000 prophecy-build-tool-1.1.4/src/prophecy_build_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-12 16:16:39.000000 prophecy-build-tool-1.1.4/src/prophecy_build_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:16:39.000000 prophecy-build-tool-1.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-12 16:12:05.000000 prophecy-build-tool-1.1.4/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-12 16:12:05.000000 prophecy-build-tool-1.1.4/test/test_deploy.py
```

### Comparing `prophecy-build-tool-1.1.3/LICENSE` & `prophecy-build-tool-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.3/PKG-INFO` & `prophecy-build-tool-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.1.3
+Version: 1.1.4
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.1.3/README.md` & `prophecy-build-tool-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.3/setup.py` & `prophecy-build-tool-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as _in:
     long_description = _in.read()
 
 setuptools.setup(
     name="prophecy-build-tool",
-    version="1.1.3",
+    version="1.1.4",
     author="Prophecy",
     author_email="maciej@prophecy.io",
     description="Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the "
     "Prophecy IDE.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SimpleDataLabsInc/prophecy-build-tool",
```

### Comparing `prophecy-build-tool-1.1.3/src/pbt/__init__.py` & `prophecy-build-tool-1.1.4/src/pbt/__init__.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.3/src/pbt/process.py` & `prophecy-build-tool-1.1.4/src/pbt/process.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.3/src/pbt/prophecy_build_tool.py` & `prophecy-build-tool-1.1.4/src/pbt/prophecy_build_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
                 self.dependent_projects[dirname(dependent_project)] = ProphecyBuildTool(dirname(dependent_project))
         self.dbfs_service = None
         self.jobs_service = None
         self.api_client = None
         self.python_cmd, self.pip_cmd = self.get_python_commands(path_root)
         self.pipelines_build_path = {}
         self.dependent_pipelines_build_path = {}
+        self.uploaded_target_paths = set()
         self.project_release = (
             release_version
             if release_version
             else os.getenv(
                 "PROJECT_RELEASE_VERSION_PLACEHOLDER",
                 "__PROJECT_RELEASE_VERSION_PLACEHOLDER__",
             )
@@ -436,26 +437,27 @@
                         pipelines_build_path = (
                             self.pipelines_build_path
                             if pipeline_id in self.pipelines_build_path
                             else self.dependent_pipelines_build_path
                         )
                         source_path = pipelines_build_path[pipeline_id]["source_absolute"]
                         target_path = component["PipelineComponent"]["path"]
-                        if not pipelines_build_path[pipeline_id]["uploaded"]:
+                        if not pipelines_build_path[pipeline_id]["uploaded"] or target_path not in self.uploaded_target_paths:
                             print(
                                 "    Uploading %s to %s"
                                 % (
                                     pipelines_build_path[pipeline_id]["source"],
                                     target_path,
                                 )
                             )
 
                             try:
                                 self.dbfs_service.put(target_path, overwrite=True, src_path=source_path)
                                 pipelines_build_path[pipeline_id]["uploaded"] = True
+                                self.uploaded_target_paths.add(target_path)
                             except HTTPError as e:
                                 pipelines_upload_failures_job[pipeline_id].append(e.response.text)
                                 pipelines_upload_failures[pipeline_id].append(e.response.text)
                             except Exception as ex:
                                 pipelines_build_path[pipeline_id]["uploaded"] = False
                                 pipelines_upload_failures_job[pipeline_id].append(str(ex))
                                 pipelines_upload_failures[pipeline_id].append(str(ex))
```

### Comparing `prophecy-build-tool-1.1.3/src/prophecy_build_tool.egg-info/PKG-INFO` & `prophecy-build-tool-1.1.4/src/prophecy_build_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.1.3
+Version: 1.1.4
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.1.3/test/test_build.py` & `prophecy-build-tool-1.1.4/test/test_build.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.3/test/test_deploy.py` & `prophecy-build-tool-1.1.4/test/test_deploy.py`

 * *Files identical despite different names*


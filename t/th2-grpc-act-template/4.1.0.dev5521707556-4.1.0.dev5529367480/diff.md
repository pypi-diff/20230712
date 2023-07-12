# Comparing `tmp/th2_grpc_act_template-4.1.0.dev5521707556.tar.gz` & `tmp/th2_grpc_act_template-4.1.0.dev5529367480.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_act_template-4.1.0.dev5521707556.tar", last modified: Tue Jul 11 15:11:56 2023, max compression
+gzip compressed data, was "dist/th2_grpc_act_template-4.1.0.dev5529367480.tar", last modified: Wed Jul 12 08:33:43 2023, max compression
```

## Comparing `th2_grpc_act_template-4.1.0.dev5521707556.tar` & `th2_grpc_act_template-4.1.0.dev5529367480.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/
--rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3908 2023-07-11 15:10:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-11 15:10:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-07-11 15:10:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-07-11 15:11:34.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_service.py
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-11 15:10:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)     5529 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    20820 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-11 15:11:56.000000 th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/
+-rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3908 2023-07-12 08:32:44.000000 th2_grpc_act_template-4.1.0.dev5529367480/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-07-12 08:32:45.000000 th2_grpc_act_template-4.1.0.dev5529367480/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-07-12 08:32:44.000000 th2_grpc_act_template-4.1.0.dev5529367480/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2128 2023-07-12 08:33:21.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template/act_service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-12 08:32:44.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template/act_template.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template/act_template_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5529 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template/act_template_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    20820 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template/act_template_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-12 08:33:43.000000 th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template.egg-info/top_level.txt
```

### Comparing `th2_grpc_act_template-4.1.0.dev5521707556/PKG-INFO` & `th2_grpc_act_template-4.1.0.dev5529367480/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_act_template
-Version: 4.1.0.dev5521707556
+Version: 4.1.0.dev5529367480
 Summary: th2_grpc_act_template
 Home-page: https://github.com/th2-net/th2-grpc-act-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC act template library (4.0.1)
```

### Comparing `th2_grpc_act_template-4.1.0.dev5521707556/README.md` & `th2_grpc_act_template-4.1.0.dev5529367480/README.md`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.1.0.dev5521707556/setup.py` & `th2_grpc_act_template-4.1.0.dev5529367480/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.strict_mode = False
 
     def finalize_options(self):
         pass
 
     def run(self):
         proto_path = os.path.abspath('src/main/proto')
-        gen_path = os.path.abspath('src/gen/main/python')
+        gen_path = os.path.abspath('build/generated/source/proto/main/services/python')
 
         if not os.path.exists(gen_path):
             os.makedirs(gen_path)
 
         proto_files = []
         for root, _, files in os.walk(proto_path):
             for filename in files:
@@ -68,16 +68,15 @@
 
 
 class CustomDist(sdist):
 
     def run(self):
         copy_tree(f'src/main/proto/{package_name}', package_name)
 
-        copy_tree(f'src/gen/main/python/{package_name}', package_name)
-        copy_tree(f'src/gen/main/services/python/{package_name}', package_name)
+        copy_tree(f'build/generated/source/proto/main/services/python/{package_name}', package_name)
         Path(f'{package_name}/__init__.py').touch()
         Path(f'{package_name}/py.typed').touch()
 
         def make_packages(root_dir):
             for path in Path(root_dir).iterdir():
                 if path.is_dir():
                     path.joinpath('__init__.py').touch()
```

### Comparing `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_service.py` & `th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template/act_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template.proto` & `th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template/act_template.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template_pb2.py` & `th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template/act_template_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template_pb2.pyi` & `th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template/act_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template/act_template_pb2_grpc.py` & `th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template/act_template_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/PKG-INFO` & `th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-act-template
-Version: 4.1.0.dev5521707556
+Version: 4.1.0.dev5529367480
 Summary: th2_grpc_act_template
 Home-page: https://github.com/th2-net/th2-grpc-act-template
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # th2 gRPC act template library (4.0.1)
```

### Comparing `th2_grpc_act_template-4.1.0.dev5521707556/th2_grpc_act_template.egg-info/SOURCES.txt` & `th2_grpc_act_template-4.1.0.dev5529367480/th2_grpc_act_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*


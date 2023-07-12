# Comparing `tmp/cubetools-0.4.6.tar.gz` & `tmp/cubetools-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubetools-0.4.6.tar", last modified: Mon Jun 26 09:13:10 2023, max compression
+gzip compressed data, was "dist/cubetools-0.4.7.tar", last modified: Wed Jul 12 06:51:44 2023, max compression
```

## Comparing `cubetools-0.4.6.tar` & `cubetools-0.4.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-06-26 09:13:10.000000 cubetools-0.4.6/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2340 2023-06-26 09:13:10.000000 cubetools-0.4.6/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1232 2023-06-19 07:55:29.000000 cubetools-0.4.6/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-06-26 09:13:10.000000 cubetools-0.4.6/cubetools/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.4.6/cubetools/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3047 2023-06-19 07:55:29.000000 cubetools-0.4.6/cubetools/download_model.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.4.6/cubetools/image_tools.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.4.6/cubetools/mindspore_lite_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.4.6/cubetools/onnx_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.4.6/cubetools/openvino_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.4.6/cubetools/paddle_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2394 2023-05-23 12:05:30.000000 cubetools-0.4.6/cubetools/python_chat_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    15694 2023-05-25 10:46:59.000000 cubetools-0.4.6/cubetools/python_video_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2137 2023-06-26 09:12:56.000000 cubetools-0.4.6/cubetools/pytorch_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.4.6/cubetools/video_capture.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3799 2023-05-25 10:06:04.000000 cubetools-0.4.6/cubetools/video_predict.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-06-26 09:13:10.000000 cubetools-0.4.6/cubetools.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2340 2023-06-26 09:13:10.000000 cubetools-0.4.6/cubetools.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      565 2023-06-26 09:13:10.000000 cubetools-0.4.6/cubetools.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-06-26 09:13:10.000000 cubetools-0.4.6/cubetools.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       88 2023-06-26 09:13:10.000000 cubetools-0.4.6/cubetools.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       32 2023-06-26 09:13:10.000000 cubetools-0.4.6/cubetools.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-06-26 09:13:10.000000 cubetools-0.4.6/cubetools.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-06-26 09:13:10.000000 cubetools-0.4.6/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2291 2023-06-26 09:12:56.000000 cubetools-0.4.6/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-07-12 06:51:44.000000 cubetools-0.4.7/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2340 2023-07-12 06:51:44.000000 cubetools-0.4.7/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1232 2023-06-19 07:55:29.000000 cubetools-0.4.7/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.4.7/cubetools/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3047 2023-06-19 07:55:29.000000 cubetools-0.4.7/cubetools/download_model.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.4.7/cubetools/image_tools.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.4.7/cubetools/mindspore_lite_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.4.7/cubetools/onnx_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.4.7/cubetools/openvino_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.4.7/cubetools/paddle_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2394 2023-05-23 12:05:30.000000 cubetools-0.4.7/cubetools/python_chat_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    15694 2023-05-25 10:46:59.000000 cubetools-0.4.7/cubetools/python_video_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2628 2023-07-12 06:51:33.000000 cubetools-0.4.7/cubetools/pytorch_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.4.7/cubetools/video_capture.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3799 2023-05-25 10:06:04.000000 cubetools-0.4.7/cubetools/video_predict.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2340 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      565 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       88 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       32 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-07-12 06:51:44.000000 cubetools-0.4.7/cubetools.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-07-12 06:51:44.000000 cubetools-0.4.7/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2291 2023-07-12 06:51:33.000000 cubetools-0.4.7/setup.py
```

### Comparing `cubetools-0.4.6/PKG-INFO` & `cubetools-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.4.6
+Version: 0.4.7
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
```

### Comparing `cubetools-0.4.6/README.md` & `cubetools-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.6/cubetools/download_model.py` & `cubetools-0.4.7/cubetools/download_model.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.6/cubetools/image_tools.py` & `cubetools-0.4.7/cubetools/image_tools.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.6/cubetools/mindspore_lite_predict.py` & `cubetools-0.4.7/cubetools/mindspore_lite_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.6/cubetools/onnx_predict.py` & `cubetools-0.4.7/cubetools/onnx_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.6/cubetools/openvino_predict.py` & `cubetools-0.4.7/cubetools/openvino_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.6/cubetools/paddle_predict.py` & `cubetools-0.4.7/cubetools/paddle_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.6/cubetools/python_chat_frontend.py` & `cubetools-0.4.7/cubetools/python_chat_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.6/cubetools/python_video_frontend.py` & `cubetools-0.4.7/cubetools/python_video_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.6/cubetools/pytorch_predict.py` & `cubetools-0.4.7/cubetools/pytorch_predict.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,40 +2,47 @@
 import gc
 import torch
 from copy import deepcopy
 
 
 # 通用PyTorch推理框架
 class Model(object):
-    def __init__(self, net, model_path, param_key=None, strict=True, cudnn_benchmark=True):
+    def __init__(self, net, model_path, param_key=None, extra_key_prefix=None, strict=True, cudnn_benchmark=True):
         if cudnn_benchmark:
             import torch.backends.cudnn as cudnn
             cudnn.benchmark = True
         self.device = torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
         self.cpu_device = torch.device('cpu')
 
-        net_params = torch.load(model_path, map_location=self.cpu_device)
-        if param_key is not None and param_key in net_params:
-                net_params = net_params[param_key]
-
-        # remove unnecessary 'module.' or 'model.'
-        for k, v in deepcopy(net_params).items():
-            if k.startswith('module.model.'):
-                net_params[k[13:]] = v
-                net_params.pop(k)
-            elif k.startswith('module.'):
-                net_params[k[7:]] = v
-                net_params.pop(k)
-            elif k.startswith('model.'):
-                net_params[k[6:]] = v
-                net_params.pop(k)
+        if net is not None:
+            net_params = torch.load(model_path, map_location=self.cpu_device)
+            if param_key is not None and param_key in net_params:
+                    net_params = net_params[param_key]
+
+            # remove unnecessary 'module.' or 'model.'
+            for k, v in deepcopy(net_params).items():
+                if k.startswith('module.model.'):
+                    net_params[k[13:]] = v
+                    net_params.pop(k)
+                elif k.startswith('module.'):
+                    net_params[k[7:]] = v
+                    net_params.pop(k)
+                elif k.startswith('model.'):
+                    net_params[k[6:]] = v
+                    net_params.pop(k)
+                elif extra_key_prefix and k.startswith(extra_key_prefix):
+                    # extra_key_prefix 应为以“.”结尾的字符串，例如： 'module.', 'model.'
+                    net_params[k[len(extra_key_prefix):]] = v
+                    net_params.pop(k)
+
+            net.load_state_dict(net_params, strict=strict)
+            self.model = net
+        else:
+            self.model = torch.jit.load(model_path, map_location=self.cpu_device)
 
-        net.load_state_dict(net_params, strict=strict)
-
-        self.model = net
         self.model.eval()
         self.model = self.model.to(self.device)
 
     def predict(self, inputs):
         inputs = to_device(inputs, self.device)
 
         with torch.no_grad():
```

### Comparing `cubetools-0.4.6/cubetools/video_capture.py` & `cubetools-0.4.7/cubetools/video_capture.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.6/cubetools/video_predict.py` & `cubetools-0.4.7/cubetools/video_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.6/cubetools.egg-info/PKG-INFO` & `cubetools-0.4.7/cubetools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.4.6
+Version: 0.4.7
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
```

### Comparing `cubetools-0.4.6/cubetools.egg-info/SOURCES.txt` & `cubetools-0.4.7/cubetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubetools-0.4.6/setup.py` & `cubetools-0.4.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='cubetools',
-    version='0.4.6',
+    version='0.4.7',
     author='cubeai',
     author_email='cubeai@163.com',
     description='CubeAI模型开发常用工具集',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```


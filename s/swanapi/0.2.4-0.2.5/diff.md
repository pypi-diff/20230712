# Comparing `tmp/swanapi-0.2.4-py3-none-any.whl.zip` & `tmp/swanapi-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 17399 bytes, number of entries: 18
+Zip file size: 17480 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      157 b- defN 23-Jul-11 00:16 swanapi/__init__.py
--rw-r--r--  2.0 unx     8931 b- defN 23-Jul-11 01:15 swanapi/base_inference.py
+-rw-r--r--  2.0 unx     9066 b- defN 23-Jul-12 09:02 swanapi/base_inference.py
 -rw-r--r--  2.0 unx     1831 b- defN 23-Jul-11 00:57 swanapi/base_requests.py
 -rw-r--r--  2.0 unx      863 b- defN 23-Jul-09 17:55 swanapi/make_build.py
 -rw-r--r--  2.0 unx     2746 b- defN 23-Jul-11 03:40 swanapi/server.py
 -rw-r--r--  2.0 unx      562 b- defN 23-Jul-10 19:06 swanapi/swan_types.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 09:38 swanapi/docker_builder/__init__.py
 -rw-r--r--  2.0 unx     3953 b- defN 23-Jul-11 07:06 swanapi/docker_builder/config.py
 -rw-r--r--  2.0 unx     4689 b- defN 23-Jul-11 13:47 swanapi/docker_builder/cuda_container.py
 -rw-r--r--  2.0 unx     3348 b- defN 23-Jul-09 18:53 swanapi/docker_builder/generate_dockerfile.py
 -rw-r--r--  2.0 unx     1901 b- defN 23-Jul-11 07:25 swanapi/docker_builder/runner.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 01:19 swanapi/utils/__init__.py
--rw-r--r--  2.0 unx    15239 b- defN 23-Jul-11 00:31 swanapi/utils/utils.py
--rw-r--r--  2.0 unx      368 b- defN 23-Jul-11 14:18 swanapi-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 14:18 swanapi-0.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Jul-11 14:18 swanapi-0.2.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-11 14:18 swanapi-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1481 b- defN 23-Jul-11 14:18 swanapi-0.2.4.dist-info/RECORD
-18 files, 46219 bytes uncompressed, 14959 bytes compressed:  67.6%
+-rw-r--r--  2.0 unx    15334 b- defN 23-Jul-12 09:03 swanapi/utils/utils.py
+-rw-r--r--  2.0 unx      368 b- defN 23-Jul-12 09:10 swanapi-0.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 09:10 swanapi-0.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-12 09:10 swanapi-0.2.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-12 09:10 swanapi-0.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1481 b- defN 23-Jul-12 09:10 swanapi-0.2.5.dist-info/RECORD
+18 files, 46449 bytes uncompressed, 15040 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: swanapi/utils/__init__.py
 Comment: 
 
 Filename: swanapi/utils/utils.py
 Comment: 
 
-Filename: swanapi-0.2.4.dist-info/METADATA
+Filename: swanapi-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: swanapi-0.2.4.dist-info/WHEEL
+Filename: swanapi-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: swanapi-0.2.4.dist-info/entry_points.txt
+Filename: swanapi-0.2.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: swanapi-0.2.4.dist-info/top_level.txt
+Filename: swanapi-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: swanapi-0.2.4.dist-info/RECORD
+Filename: swanapi-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swanapi/base_inference.py

```diff
@@ -23,14 +23,15 @@
             "dict": dict,
         }
         self.types_list = list(self.TYPES.keys())
         self.outputs_typing = None
         self.requests_inputs = None
         self.requests_inputs_param_names = None
         self.requests_outputs_variables_num = None
+        self.description = None
 
     def backbone_type_checker(self) -> None:
         # 如果fn是列表，报错
         if isinstance(self.fn, list):
             raise DeprecationWarning(
                 "The `fn` parameter only accepts a single function, support for a list "
                 "of functions has been deprecated."
@@ -90,15 +91,16 @@
         # self.requests_inputs - 用户输入的完整json字典
         self.requests_inputs = requests_inputs
         # 获取网络请求的参数个数
         self.requests_inputs_param_names = list(self.requests_inputs.keys())
         # 判断网络请求输入的参数的个数是否与inputs定义的个数一致
         assert len(self.requests_inputs_param_names) == len(self.backbone_inputs), "请求传入的参数数量与inputs定义的不一致"
         # 判断网络请求输入的参数名是否与fn定义的一致
-        assert utils.check_elements_in_list(self.requests_inputs_param_names, self.fn_param_names), "请求传入的参数key与fn定义的不一致"
+        assert utils.check_elements_in_list(self.requests_inputs_param_names,
+                                            self.fn_param_names), "请求传入的参数key与fn定义的不一致"
 
     def requests_input_converter(self) -> None:
         # 对于每一个requests内容的输入类型，做相应的转换
         for iter, param_name in enumerate(self.fn_param_names):
             # param_name : 'input_image', 'custom_size_height', 'custom_size_width'
             # 获取内容values
             values = self.requests_inputs[param_name]
@@ -173,19 +175,21 @@
                 assert isinstance(result[iter], str)
                 result_json[iter] = {"content": result[iter]}
 
             elif backbone_output == "number":
                 assert isinstance(result[iter], (int, float))
                 result_json[iter] = {"content": result[iter]}
 
-            elif backbone_output == ["dict"]:
+            elif backbone_output == "dict":
                 assert isinstance(result, dict)
                 result_json[iter] = {"content": result[iter]}
 
-            elif backbone_output == ["list"]:
+            elif backbone_output == "list":
                 assert isinstance(result, list)
                 result_json[iter] = {"content": result[iter]}
-
             else:
                 raise TypeError("类型检查模块存在Bug")
 
         return result_json
+
+    def get_description(self):
+        return self.description
```

## swanapi/utils/utils.py

```diff
@@ -426,9 +426,14 @@
     if is_valid_url(path):
         return encode_url_to_base64(path)
     else:
         return encode_file_to_base64(path)
 
 
 def bytes_to_array(bytes_data):
+    """
+    将字节流解码成PIL风格的numpy
+    :param bytes_data:
+    :return:
+    """
     im = _Image.open(BytesIO(bytes_data))
     return np.array(im)
```

## Comparing `swanapi-0.2.4.dist-info/RECORD` & `swanapi-0.2.5.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 swanapi/__init__.py,sha256=2N4vWNDaCYewP1euHTVKHE1zmtStmsi0af6S-lu8Bs0,157
-swanapi/base_inference.py,sha256=QlWvZI1rpff8pdcMLQ-AKDBHbAIKulXDXJd2I6TAnJw,8931
+swanapi/base_inference.py,sha256=xCTcBAWeztnZWoscBqvYMk9WjrAw7vqie5o5fEMerbY,9066
 swanapi/base_requests.py,sha256=kpGxsP26WgZG7SroPCoDZl_7fjsgHmXOSFHGKbCnozc,1831
 swanapi/make_build.py,sha256=P4WsA52pftJyNLrU986UKkYPY88VLzRMgQJ6s_UUTY0,863
 swanapi/server.py,sha256=AuVDQd_AJbBejrYT5MY5R0NIM64_9QWMCUhqzfUH0Vw,2746
 swanapi/swan_types.py,sha256=6rjoLVOqyahSQXilAVtMVS4e50MNeCMEBinPu3jR_JE,562
 swanapi/docker_builder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swanapi/docker_builder/config.py,sha256=oMHdFbV8zGzlsIfMjPT1PimM1t6LLnkEIuKxEpjiANM,3953
 swanapi/docker_builder/cuda_container.py,sha256=HBVrWfq7_SkUrC_L9D9oCCCDHChuw-GV09AasrCDGlE,4689
 swanapi/docker_builder/generate_dockerfile.py,sha256=bbd2u94MgyZq883WrTtk936TM-6eUYTuc1ZqgVdgM90,3348
 swanapi/docker_builder/runner.py,sha256=rHLlSWqyJkXfWbSIBJGTWfiqtzsOdXYQZrHR0OoUAh8,1901
 swanapi/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-swanapi/utils/utils.py,sha256=jx9anz_ty9T1FAJRAT8eLlsKoCOGha4CsPzKa2plK50,15239
-swanapi-0.2.4.dist-info/METADATA,sha256=RG26okDn3ifK611GQf6mkWLJ4g9daXQHESAGejOP4xg,368
-swanapi-0.2.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swanapi-0.2.4.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
-swanapi-0.2.4.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
-swanapi-0.2.4.dist-info/RECORD,,
+swanapi/utils/utils.py,sha256=Q2UVZ4g0n9o42mflHpylBvXooIqun8HbJj-xTmIoUHc,15334
+swanapi-0.2.5.dist-info/METADATA,sha256=UlH8PsyF91nl5lOylFK2hsy2mdXTjskzMqzKHecGyPE,368
+swanapi-0.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swanapi-0.2.5.dist-info/entry_points.txt,sha256=jqLTkbNqH1FcP_Fdt51ZEiZlGVYxBb-spukW4iHwPzo,50
+swanapi-0.2.5.dist-info/top_level.txt,sha256=IMPJQB4d-hjWaRE7hQcOckZuFdbQoEWWXL29rxE1b0Y,8
+swanapi-0.2.5.dist-info/RECORD,,
```


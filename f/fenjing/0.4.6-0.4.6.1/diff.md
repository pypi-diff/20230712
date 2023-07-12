# Comparing `tmp/fenjing-0.4.6.tar.gz` & `tmp/fenjing-0.4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.4.6.tar", last modified: Wed Jul 12 09:49:22 2023, max compression
+gzip compressed data, was "fenjing-0.4.6.1.tar", last modified: Wed Jul 12 09:55:53 2023, max compression
```

## Comparing `fenjing-0.4.6.tar` & `fenjing-0.4.6.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:49:22.213267 fenjing-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-12 09:49:12.000000 fenjing-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-12 09:49:12.000000 fenjing-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-12 09:49:22.213267 fenjing-0.4.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6735 2023-07-12 09:49:12.000000 fenjing-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 09:49:12.000000 fenjing-0.4.6/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:49:22.209267 fenjing-0.4.6/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7473 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    32506 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:49:22.213267 fenjing-0.4.6/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-07-12 09:49:13.000000 fenjing-0.4.6/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:49:22.213267 fenjing-0.4.6/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-12 09:49:22.000000 fenjing-0.4.6/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-12 09:49:22.000000 fenjing-0.4.6/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:49:22.000000 fenjing-0.4.6/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 09:49:22.000000 fenjing-0.4.6/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 09:49:22.000000 fenjing-0.4.6/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 09:49:13.000000 fenjing-0.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:49:22.213267 fenjing-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-12 09:49:13.000000 fenjing-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:49:22.213267 fenjing-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-12 09:49:13.000000 fenjing-0.4.6/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-12 09:49:13.000000 fenjing-0.4.6/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6735 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7473 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32560 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-12 09:55:53.000000 fenjing-0.4.6.1/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-12 09:55:53.000000 fenjing-0.4.6.1/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:55:53.000000 fenjing-0.4.6.1/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 09:55:53.000000 fenjing-0.4.6.1/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 09:55:53.000000 fenjing-0.4.6.1/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:55:53.059677 fenjing-0.4.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-12 09:55:41.000000 fenjing-0.4.6.1/tests/test_payload_gen.py
```

### Comparing `fenjing-0.4.6/LICENSE` & `fenjing-0.4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/PKG-INFO` & `fenjing-0.4.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.6
+Version: 0.4.6.1
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.4.6/README.md` & `fenjing-0.4.6.1/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/cli.py` & `fenjing-0.4.6.1/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/colorize.py` & `fenjing-0.4.6.1/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/config_payload.py` & `fenjing-0.4.6.1/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/const.py` & `fenjing-0.4.6.1/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/context_vars.py` & `fenjing-0.4.6.1/fenjing/context_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/form.py` & `fenjing-0.4.6.1/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/form_cracker.py` & `fenjing-0.4.6.1/fenjing/form_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/full_payload_gen.py` & `fenjing-0.4.6.1/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/payload_gen.py` & `fenjing-0.4.6.1/fenjing/payload_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1215,44 +1215,54 @@
             (ATTRIBUTE, "__dict__"),
             (ITEM, "_TemplateReference__context"),
             (ITEM, "config"),
         )
     ]
 
 
-@req_gen
-def gen_config_request(context):
-    return [
-        (
-            CHAINED_ATTRIBUTE_ITEM,
-            (LITERAL, "request"),
-            (ATTRIBUTE, "application"),
-            (ATTRIBUTE, "__self__"),
-            (ATTRIBUTE, "json_module"),
-            (ATTRIBUTE, "JSONEncoder"),
-            (ATTRIBUTE, "default"),
-            (ATTRIBUTE, "__globals__"),
-            (ITEM, "current_app"),
-            (ATTRIBUTE, "config"),
-        )
-    ]
+# @req_gen
+# def gen_config_request(context):
+#     return [
+#         (
+#             CHAINED_ATTRIBUTE_ITEM,
+#             (LITERAL, "request"),
+#             (ATTRIBUTE, "application"),
+#             (ATTRIBUTE, "__self__"),
+#             (ATTRIBUTE, "json_module"),
+#             (ATTRIBUTE, "JSONEncoder"),
+#             (ATTRIBUTE, "default"),
+#             (ATTRIBUTE, "__globals__"),
+#             (ITEM, "current_app"),
+#             (ATTRIBUTE, "config"),
+#         )
+#     ]
 
 
 # ---
 
 
+# @req_gen
+# def gen_module_os_urlfor(context):
+#     return [
+#         (
+#             CHAINED_ATTRIBUTE_ITEM,
+#             (LITERAL, "url_for"),
+#             (ATTRIBUTE, "__globals__"),
+#             (ITEM, "os"),
+#         )
+#     ]
+
+
 @req_gen
-def gen_module_os_urlfor(context):
+def gen_module_os_eval(context):
     return [
-        (
-            CHAINED_ATTRIBUTE_ITEM,
-            (LITERAL, "url_for"),
-            (ATTRIBUTE, "__globals__"),
-            (ITEM, "os"),
-        )
+        (EVAL, "__import__"),
+        (LITERAL, "("),
+        (STRING, "os"),
+        (LITERAL, ")"),
     ]
 
 
 @req_gen
 def gen_module_os_config(context):
     return [
         (
@@ -1261,22 +1271,14 @@
             (CLASS_ATTRIBUTE, "__init__"),
             (ATTRIBUTE, "__globals__"),
             (ITEM, "os"),
         )
     ]
 
 
-@req_gen
-def gen_module_os_eval(context):
-    return [
-        (EVAL, "__import__"),
-        (LITERAL, "("),
-        (STRING, "os"),
-        (LITERAL, ")"),
-    ]
 
 # ---
 
 
 
 @req_gen
 def gen_os_popen_obj_normal(context, cmd):
```

### Comparing `fenjing-0.4.6/fenjing/requester.py` & `fenjing-0.4.6.1/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/scan_url.py` & `fenjing-0.4.6.1/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/shell_payload.py` & `fenjing-0.4.6.1/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/templates/index.html` & `fenjing-0.4.6.1/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/waf_func_gen.py` & `fenjing-0.4.6.1/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing/webui.py` & `fenjing-0.4.6.1/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/fenjing.egg-info/PKG-INFO` & `fenjing-0.4.6.1/fenjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.6
+Version: 0.4.6.1
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.4.6/fenjing.egg-info/SOURCES.txt` & `fenjing-0.4.6.1/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/setup.py` & `fenjing-0.4.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/tests/test_full_payload_gen.py` & `fenjing-0.4.6.1/tests/test_full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.6/tests/test_payload_gen.py` & `fenjing-0.4.6.1/tests/test_payload_gen.py`

 * *Files identical despite different names*


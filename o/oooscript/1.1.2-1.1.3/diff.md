# Comparing `tmp/oooscript-1.1.2.tar.gz` & `tmp/oooscript-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oooscript-1.1.2.tar", max compression
+gzip compressed data, was "oooscript-1.1.3.tar", max compression
```

## Comparing `oooscript-1.1.2.tar` & `oooscript-1.1.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rwxr-xr-x   0        0        0      316 2023-07-12 17:21:58.356350 oooscript-1.1.2/README.md
--rwxr-xr-x   0        0        0       71 2023-07-12 17:21:58.361276 oooscript-1.1.2/oooscript/.oooscript_root
--rwxr-xr-x   0        0        0      165 2022-10-01 21:39:16.817180 oooscript-1.1.2/oooscript/__init__.py
--rwxr-xr-x   0        0        0        0 2022-09-12 18:03:39.994876 oooscript-1.1.2/oooscript/build/__init__.py
--rwxr-xr-x   0        0        0     8017 2023-07-12 17:57:46.185749 oooscript-1.1.2/oooscript/build/build.py
--rwxr-xr-x   0        0        0      423 2022-09-26 16:21:12.331358 oooscript-1.1.2/oooscript/build/build_util.py
--rwxr-xr-x   0        0        0     3691 2022-10-01 21:39:16.819366 oooscript-1.1.2/oooscript/build/copy_resource.py
--rwxr-xr-x   0        0        0     5521 2023-07-12 17:58:10.477781 oooscript-1.1.2/oooscript/build/embed_py_script.py
--rwxr-xr-x   0        0        0     4659 2022-10-01 22:51:52.055266 oooscript-1.1.2/oooscript/build/manifest_script.py
--rwxr-xr-x   0        0        0      209 2022-09-26 16:21:12.336634 oooscript-1.1.2/oooscript/build/tmp_dir.py
--rwxr-xr-x   0        0        0        0 2022-09-13 16:08:22.450751 oooscript-1.1.2/oooscript/cfg/__init__.py
--rwxr-xr-x   0        0        0     3203 2023-07-06 20:15:59.696122 oooscript-1.1.2/oooscript/cfg/config.py
--rwxr-xr-x   0        0        0        0 2022-10-01 21:38:58.799643 oooscript-1.1.2/oooscript/cli/__init__.py
--rwxr-xr-x   0        0        0     2854 2023-07-12 17:21:58.367211 oooscript-1.1.2/oooscript/cli/main.py
--rwxr-xr-x   0        0        0        0 2022-09-12 18:26:31.865907 oooscript-1.1.2/oooscript/lib/__init__.py
--rwxr-xr-x   0        0        0      376 2022-09-12 18:26:59.276746 oooscript-1.1.2/oooscript/lib/enums.py
--rwxr-xr-x   0        0        0       40 2022-10-01 21:38:58.805512 oooscript-1.1.2/oooscript/lib/ex.py
--rwxr-xr-x   0        0        0        0 2022-09-12 18:24:13.737439 oooscript-1.1.2/oooscript/models/__init__.py
--rwxr-xr-x   0        0        0        0 2022-09-26 16:21:12.338808 oooscript-1.1.2/oooscript/models/script_cfg/__init__.py
--rwxr-xr-x   0        0        0      522 2022-10-01 21:39:16.823315 oooscript-1.1.2/oooscript/models/script_cfg/args.py
--rwxr-xr-x   0        0        0      640 2022-10-01 21:39:16.824695 oooscript-1.1.2/oooscript/models/script_cfg/model_script_cfg.py
--rwxr-xr-x   0        0        0      533 2022-09-12 18:24:13.773946 oooscript-1.1.2/oooscript/models/validators.py
--rwxr-xr-x   0        0        0       83 2022-09-13 15:24:25.505568 oooscript-1.1.2/oooscript/res/__init__.py
--rwxr-xr-x   0        0        0       88 2022-09-13 15:24:14.808773 oooscript-1.1.2/oooscript/res/docs/__init__.py
--rwxr-xr-x   0        0        0     3996 2022-09-26 16:21:12.342560 oooscript-1.1.2/oooscript/res/docs/blank.odf
--rwxr-xr-x   0        0        0     7979 2022-09-26 16:21:12.343538 oooscript-1.1.2/oooscript/res/docs/blank.odg
--rwxr-xr-x   0        0        0    15064 2022-09-26 16:21:12.344729 oooscript-1.1.2/oooscript/res/docs/blank.odp
--rwxr-xr-x   0        0        0     6968 2022-09-26 16:21:12.345631 oooscript-1.1.2/oooscript/res/docs/blank.ods
--rwxr-xr-x   0        0        0     8193 2022-09-13 15:18:46.583474 oooscript-1.1.2/oooscript/res/docs/blank.odt
--rwxr-xr-x   0        0        0        0 2022-09-12 18:04:27.526867 oooscript-1.1.2/oooscript/utils/__init__.py
--rwxr-xr-x   0        0        0     1155 2022-09-14 13:46:13.153083 oooscript-1.1.2/oooscript/utils/enum_util.py
--rwxr-xr-x   0        0        0    10031 2022-10-01 21:39:16.826146 oooscript-1.1.2/oooscript/utils/paths.py
--rwxr-xr-x   0        0        0     1866 2023-07-12 17:40:55.942177 oooscript-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 oooscript-1.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0      316 2023-07-12 17:21:58.356350 oooscript-1.1.3/README.md
+-rwxr-xr-x   0        0        0       71 2023-07-12 17:21:58.361276 oooscript-1.1.3/oooscript/.oooscript_root
+-rwxr-xr-x   0        0        0      165 2022-10-01 21:39:16.817180 oooscript-1.1.3/oooscript/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:03:39.994876 oooscript-1.1.3/oooscript/build/__init__.py
+-rwxr-xr-x   0        0        0     8011 2023-07-12 18:43:45.827916 oooscript-1.1.3/oooscript/build/build.py
+-rwxr-xr-x   0        0        0      423 2022-09-26 16:21:12.331358 oooscript-1.1.3/oooscript/build/build_util.py
+-rwxr-xr-x   0        0        0     3691 2022-10-01 21:39:16.819366 oooscript-1.1.3/oooscript/build/copy_resource.py
+-rwxr-xr-x   0        0        0     5521 2023-07-12 18:34:46.017444 oooscript-1.1.3/oooscript/build/embed_py_script.py
+-rwxr-xr-x   0        0        0     4659 2022-10-01 22:51:52.055266 oooscript-1.1.3/oooscript/build/manifest_script.py
+-rwxr-xr-x   0        0        0      209 2022-09-26 16:21:12.336634 oooscript-1.1.3/oooscript/build/tmp_dir.py
+-rwxr-xr-x   0        0        0        0 2022-09-13 16:08:22.450751 oooscript-1.1.3/oooscript/cfg/__init__.py
+-rwxr-xr-x   0        0        0     3203 2023-07-06 20:15:59.696122 oooscript-1.1.3/oooscript/cfg/config.py
+-rwxr-xr-x   0        0        0        0 2022-10-01 21:38:58.799643 oooscript-1.1.3/oooscript/cli/__init__.py
+-rwxr-xr-x   0        0        0     2852 2023-07-12 18:49:42.567227 oooscript-1.1.3/oooscript/cli/main.py
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:26:31.865907 oooscript-1.1.3/oooscript/lib/__init__.py
+-rwxr-xr-x   0        0        0      376 2022-09-12 18:26:59.276746 oooscript-1.1.3/oooscript/lib/enums.py
+-rwxr-xr-x   0        0        0       40 2022-10-01 21:38:58.805512 oooscript-1.1.3/oooscript/lib/ex.py
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:24:13.737439 oooscript-1.1.3/oooscript/models/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-09-26 16:21:12.338808 oooscript-1.1.3/oooscript/models/script_cfg/__init__.py
+-rwxr-xr-x   0        0        0      522 2022-10-01 21:39:16.823315 oooscript-1.1.3/oooscript/models/script_cfg/args.py
+-rwxr-xr-x   0        0        0      640 2022-10-01 21:39:16.824695 oooscript-1.1.3/oooscript/models/script_cfg/model_script_cfg.py
+-rwxr-xr-x   0        0        0      533 2022-09-12 18:24:13.773946 oooscript-1.1.3/oooscript/models/validators.py
+-rwxr-xr-x   0        0        0       83 2022-09-13 15:24:25.505568 oooscript-1.1.3/oooscript/res/__init__.py
+-rwxr-xr-x   0        0        0       88 2022-09-13 15:24:14.808773 oooscript-1.1.3/oooscript/res/docs/__init__.py
+-rwxr-xr-x   0        0        0     3996 2022-09-26 16:21:12.342560 oooscript-1.1.3/oooscript/res/docs/blank.odf
+-rwxr-xr-x   0        0        0     7979 2022-09-26 16:21:12.343538 oooscript-1.1.3/oooscript/res/docs/blank.odg
+-rwxr-xr-x   0        0        0    15064 2022-09-26 16:21:12.344729 oooscript-1.1.3/oooscript/res/docs/blank.odp
+-rwxr-xr-x   0        0        0     6968 2022-09-26 16:21:12.345631 oooscript-1.1.3/oooscript/res/docs/blank.ods
+-rwxr-xr-x   0        0        0     8193 2022-09-13 15:18:46.583474 oooscript-1.1.3/oooscript/res/docs/blank.odt
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:04:27.526867 oooscript-1.1.3/oooscript/utils/__init__.py
+-rwxr-xr-x   0        0        0     1155 2022-09-14 13:46:13.153083 oooscript-1.1.3/oooscript/utils/enum_util.py
+-rwxr-xr-x   0        0        0    10031 2022-10-01 21:39:16.826146 oooscript-1.1.3/oooscript/utils/paths.py
+-rwxr-xr-x   0        0        0     1866 2023-07-12 18:48:43.155944 oooscript-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 oooscript-1.1.3/PKG-INFO
```

### Comparing `oooscript-1.1.2/oooscript/build/build.py` & `oooscript-1.1.3/oooscript/build/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,26 +134,24 @@
             return self._res_path / "docs" / "blank.odf"
         elif t == AppTypeEnum.WRITER:
             return self._res_path / "docs" / "blank.odt"
         else:
             # base is not currently supported
             return None
 
-    def _embed_script(self) -> None:
+    def _embed_script(self, build_dir: Path) -> None:
         if self._embed_doc is None:
             # src_doc = self._config.app_res_blank_odt
             src_doc = self._get_blank_embed_doc()
             if src_doc is None:
                 return None
         else:
             src_doc = paths.get_path(self._embed_doc)
         cp = CopyResource(src=src_doc, dst=None, clear_prev=False, src_is_res=self._embed_doc is None)
-        emb = EmbedScriptPy(
-            src=self._dest_file, doc_path=cp.src_path, model=self._model, build_dir=self._builder_args.build_dir
-        )
+        emb = EmbedScriptPy(src=self._dest_file, doc_path=cp.src_path, model=self._model, build_dir=build_dir)
         emb.embed()
 
     # region Public Methods
     def build(self) -> bool:
         """
         Builds the plugin into the dist folder outlined in settings.json
         @return: `True` of the build is a success; Otherwise, `False`
@@ -209,15 +207,15 @@
         # region Report
         if self.allow_print == True and os.path.exists(self._dest_file):
             print("Generated File: " + self._dest_file)
         # endregion Report
         if self._model.args.single_script is False:
             self._append_g_exported()
         if self._embed:
-            self._embed_script()
+            self._embed_script(build_dir=dist_dir)
         return True
 
     # endregion Public Methods
 
     @property
     def site_pkg_dir(self):
         if self._site_pkg_dir is None:
```

### Comparing `oooscript-1.1.2/oooscript/build/copy_resource.py` & `oooscript-1.1.3/oooscript/build/copy_resource.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/oooscript/build/embed_py_script.py` & `oooscript-1.1.3/oooscript/build/embed_py_script.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/oooscript/build/manifest_script.py` & `oooscript-1.1.3/oooscript/build/manifest_script.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/oooscript/cfg/config.py` & `oooscript-1.1.3/oooscript/cfg/config.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/oooscript/cli/main.py` & `oooscript-1.1.3/oooscript/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         help="Optional, LibreOffice document to embed script into.",
     )
     parser.add_argument(
         "-b",
         "--build-dir",
         default=None,
         dest="build_dir",
-        help="Optional, build directory to place compiled script. Can be relative or absolute path. Will override the build directory set by environment and config.json.",
+        help="Optional, build directory to place compiled script. Can be relative or absolute path. Will override the build directory set by environment and .env file.",
     )
 
 
 # endregion  parser setup
 
 
 # region        process arg command
```

### Comparing `oooscript-1.1.2/oooscript/models/script_cfg/args.py` & `oooscript-1.1.3/oooscript/models/script_cfg/args.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/oooscript/models/script_cfg/model_script_cfg.py` & `oooscript-1.1.3/oooscript/models/script_cfg/model_script_cfg.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/oooscript/models/validators.py` & `oooscript-1.1.3/oooscript/models/validators.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/oooscript/res/docs/blank.odf` & `oooscript-1.1.3/oooscript/res/docs/blank.odf`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/oooscript/res/docs/blank.odg` & `oooscript-1.1.3/oooscript/res/docs/blank.odg`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/oooscript/res/docs/blank.odp` & `oooscript-1.1.3/oooscript/res/docs/blank.odp`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/oooscript/res/docs/blank.ods` & `oooscript-1.1.3/oooscript/res/docs/blank.ods`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/oooscript/res/docs/blank.odt` & `oooscript-1.1.3/oooscript/res/docs/blank.odt`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/oooscript/utils/enum_util.py` & `oooscript-1.1.3/oooscript/utils/enum_util.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/oooscript/utils/paths.py` & `oooscript-1.1.3/oooscript/utils/paths.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.2/pyproject.toml` & `oooscript-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oooscript"
-version = "1.1.2"
+version = "1.1.3"
 description = "Compiles several python scripts into a single script that can be eaisly used by LibreOffice as a macro."
 authors = [":Barry-Thomas-Paul: Moss <vibrationoflife@protonmail.com>"]
 homepage = "https://github.com/Amourspirit/python_libreoffice_oooscript"
 documentation = "https://oooscript.readthedocs.io/en/latest/"
 repository = "https://github.com/Amourspirit/python_libreoffice_oooscript"
 license = "MIT"
 readme = "README.md"
```

### Comparing `oooscript-1.1.2/PKG-INFO` & `oooscript-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oooscript
-Version: 1.1.2
+Version: 1.1.3
 Summary: Compiles several python scripts into a single script that can be eaisly used by LibreOffice as a macro.
 Home-page: https://github.com/Amourspirit/python_libreoffice_oooscript
 License: MIT
 Keywords: ooouno,libreoffice,stickytape,uno,pyuno,macro
 Author: :Barry-Thomas-Paul: Moss
 Author-email: vibrationoflife@protonmail.com
 Requires-Python: >=3.8,<4.0
```


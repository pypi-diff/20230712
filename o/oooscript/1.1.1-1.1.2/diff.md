# Comparing `tmp/oooscript-1.1.1.tar.gz` & `tmp/oooscript-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oooscript-1.1.1.tar", max compression
+gzip compressed data, was "oooscript-1.1.2.tar", max compression
```

## Comparing `oooscript-1.1.1.tar` & `oooscript-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rwxr-xr-x   0        0        0      316 2023-07-12 17:11:29.592501 oooscript-1.1.1/README.md
--rwxr-xr-x   0        0        0       71 2023-07-12 17:11:29.593500 oooscript-1.1.1/oooscript/.oooscript_root
--rwxr-xr-x   0        0        0      165 2022-10-01 21:39:16.817180 oooscript-1.1.1/oooscript/__init__.py
--rwxr-xr-x   0        0        0        0 2022-09-12 18:03:39.994876 oooscript-1.1.1/oooscript/build/__init__.py
--rwxr-xr-x   0        0        0     7955 2023-07-12 17:11:29.595534 oooscript-1.1.1/oooscript/build/build.py
--rwxr-xr-x   0        0        0      423 2022-09-26 16:21:12.331358 oooscript-1.1.1/oooscript/build/build_util.py
--rwxr-xr-x   0        0        0     3691 2022-10-01 21:39:16.819366 oooscript-1.1.1/oooscript/build/copy_resource.py
--rwxr-xr-x   0        0        0     5271 2022-10-01 21:38:58.797077 oooscript-1.1.1/oooscript/build/embed_py_script.py
--rwxr-xr-x   0        0        0     4659 2022-10-01 22:51:52.055266 oooscript-1.1.1/oooscript/build/manifest_script.py
--rwxr-xr-x   0        0        0      209 2022-09-26 16:21:12.336634 oooscript-1.1.1/oooscript/build/tmp_dir.py
--rwxr-xr-x   0        0        0        0 2022-09-13 16:08:22.450751 oooscript-1.1.1/oooscript/cfg/__init__.py
--rwxr-xr-x   0        0        0     3203 2023-07-06 20:15:59.696122 oooscript-1.1.1/oooscript/cfg/config.py
--rwxr-xr-x   0        0        0        0 2022-10-01 21:38:58.799643 oooscript-1.1.1/oooscript/cli/__init__.py
--rwxr-xr-x   0        0        0     2854 2023-07-12 17:11:29.596405 oooscript-1.1.1/oooscript/cli/main.py
--rwxr-xr-x   0        0        0        0 2022-09-12 18:26:31.865907 oooscript-1.1.1/oooscript/lib/__init__.py
--rwxr-xr-x   0        0        0      376 2022-09-12 18:26:59.276746 oooscript-1.1.1/oooscript/lib/enums.py
--rwxr-xr-x   0        0        0       40 2022-10-01 21:38:58.805512 oooscript-1.1.1/oooscript/lib/ex.py
--rwxr-xr-x   0        0        0        0 2022-09-12 18:24:13.737439 oooscript-1.1.1/oooscript/models/__init__.py
--rwxr-xr-x   0        0        0        0 2022-09-26 16:21:12.338808 oooscript-1.1.1/oooscript/models/script_cfg/__init__.py
--rwxr-xr-x   0        0        0      522 2022-10-01 21:39:16.823315 oooscript-1.1.1/oooscript/models/script_cfg/args.py
--rwxr-xr-x   0        0        0      640 2022-10-01 21:39:16.824695 oooscript-1.1.1/oooscript/models/script_cfg/model_script_cfg.py
--rwxr-xr-x   0        0        0      533 2022-09-12 18:24:13.773946 oooscript-1.1.1/oooscript/models/validators.py
--rwxr-xr-x   0        0        0       83 2022-09-13 15:24:25.505568 oooscript-1.1.1/oooscript/res/__init__.py
--rwxr-xr-x   0        0        0       88 2022-09-13 15:24:14.808773 oooscript-1.1.1/oooscript/res/docs/__init__.py
--rwxr-xr-x   0        0        0     3996 2022-09-26 16:21:12.342560 oooscript-1.1.1/oooscript/res/docs/blank.odf
--rwxr-xr-x   0        0        0     7979 2022-09-26 16:21:12.343538 oooscript-1.1.1/oooscript/res/docs/blank.odg
--rwxr-xr-x   0        0        0    15064 2022-09-26 16:21:12.344729 oooscript-1.1.1/oooscript/res/docs/blank.odp
--rwxr-xr-x   0        0        0     6968 2022-09-26 16:21:12.345631 oooscript-1.1.1/oooscript/res/docs/blank.ods
--rwxr-xr-x   0        0        0     8193 2022-09-13 15:18:46.583474 oooscript-1.1.1/oooscript/res/docs/blank.odt
--rwxr-xr-x   0        0        0        0 2022-09-12 18:04:27.526867 oooscript-1.1.1/oooscript/utils/__init__.py
--rwxr-xr-x   0        0        0     1155 2022-09-14 13:46:13.153083 oooscript-1.1.1/oooscript/utils/enum_util.py
--rwxr-xr-x   0        0        0    10031 2022-10-01 21:39:16.826146 oooscript-1.1.1/oooscript/utils/paths.py
--rwxr-xr-x   0        0        0     1866 2023-07-12 17:11:29.597082 oooscript-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 oooscript-1.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      316 2023-07-12 17:21:58.356350 oooscript-1.1.2/README.md
+-rwxr-xr-x   0        0        0       71 2023-07-12 17:21:58.361276 oooscript-1.1.2/oooscript/.oooscript_root
+-rwxr-xr-x   0        0        0      165 2022-10-01 21:39:16.817180 oooscript-1.1.2/oooscript/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:03:39.994876 oooscript-1.1.2/oooscript/build/__init__.py
+-rwxr-xr-x   0        0        0     8017 2023-07-12 17:57:46.185749 oooscript-1.1.2/oooscript/build/build.py
+-rwxr-xr-x   0        0        0      423 2022-09-26 16:21:12.331358 oooscript-1.1.2/oooscript/build/build_util.py
+-rwxr-xr-x   0        0        0     3691 2022-10-01 21:39:16.819366 oooscript-1.1.2/oooscript/build/copy_resource.py
+-rwxr-xr-x   0        0        0     5521 2023-07-12 17:58:10.477781 oooscript-1.1.2/oooscript/build/embed_py_script.py
+-rwxr-xr-x   0        0        0     4659 2022-10-01 22:51:52.055266 oooscript-1.1.2/oooscript/build/manifest_script.py
+-rwxr-xr-x   0        0        0      209 2022-09-26 16:21:12.336634 oooscript-1.1.2/oooscript/build/tmp_dir.py
+-rwxr-xr-x   0        0        0        0 2022-09-13 16:08:22.450751 oooscript-1.1.2/oooscript/cfg/__init__.py
+-rwxr-xr-x   0        0        0     3203 2023-07-06 20:15:59.696122 oooscript-1.1.2/oooscript/cfg/config.py
+-rwxr-xr-x   0        0        0        0 2022-10-01 21:38:58.799643 oooscript-1.1.2/oooscript/cli/__init__.py
+-rwxr-xr-x   0        0        0     2854 2023-07-12 17:21:58.367211 oooscript-1.1.2/oooscript/cli/main.py
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:26:31.865907 oooscript-1.1.2/oooscript/lib/__init__.py
+-rwxr-xr-x   0        0        0      376 2022-09-12 18:26:59.276746 oooscript-1.1.2/oooscript/lib/enums.py
+-rwxr-xr-x   0        0        0       40 2022-10-01 21:38:58.805512 oooscript-1.1.2/oooscript/lib/ex.py
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:24:13.737439 oooscript-1.1.2/oooscript/models/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-09-26 16:21:12.338808 oooscript-1.1.2/oooscript/models/script_cfg/__init__.py
+-rwxr-xr-x   0        0        0      522 2022-10-01 21:39:16.823315 oooscript-1.1.2/oooscript/models/script_cfg/args.py
+-rwxr-xr-x   0        0        0      640 2022-10-01 21:39:16.824695 oooscript-1.1.2/oooscript/models/script_cfg/model_script_cfg.py
+-rwxr-xr-x   0        0        0      533 2022-09-12 18:24:13.773946 oooscript-1.1.2/oooscript/models/validators.py
+-rwxr-xr-x   0        0        0       83 2022-09-13 15:24:25.505568 oooscript-1.1.2/oooscript/res/__init__.py
+-rwxr-xr-x   0        0        0       88 2022-09-13 15:24:14.808773 oooscript-1.1.2/oooscript/res/docs/__init__.py
+-rwxr-xr-x   0        0        0     3996 2022-09-26 16:21:12.342560 oooscript-1.1.2/oooscript/res/docs/blank.odf
+-rwxr-xr-x   0        0        0     7979 2022-09-26 16:21:12.343538 oooscript-1.1.2/oooscript/res/docs/blank.odg
+-rwxr-xr-x   0        0        0    15064 2022-09-26 16:21:12.344729 oooscript-1.1.2/oooscript/res/docs/blank.odp
+-rwxr-xr-x   0        0        0     6968 2022-09-26 16:21:12.345631 oooscript-1.1.2/oooscript/res/docs/blank.ods
+-rwxr-xr-x   0        0        0     8193 2022-09-13 15:18:46.583474 oooscript-1.1.2/oooscript/res/docs/blank.odt
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:04:27.526867 oooscript-1.1.2/oooscript/utils/__init__.py
+-rwxr-xr-x   0        0        0     1155 2022-09-14 13:46:13.153083 oooscript-1.1.2/oooscript/utils/enum_util.py
+-rwxr-xr-x   0        0        0    10031 2022-10-01 21:39:16.826146 oooscript-1.1.2/oooscript/utils/paths.py
+-rwxr-xr-x   0        0        0     1866 2023-07-12 17:40:55.942177 oooscript-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 oooscript-1.1.2/PKG-INFO
```

### Comparing `oooscript-1.1.1/oooscript/build/build.py` & `oooscript-1.1.2/oooscript/build/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,17 @@
             # src_doc = self._config.app_res_blank_odt
             src_doc = self._get_blank_embed_doc()
             if src_doc is None:
                 return None
         else:
             src_doc = paths.get_path(self._embed_doc)
         cp = CopyResource(src=src_doc, dst=None, clear_prev=False, src_is_res=self._embed_doc is None)
-        emb = EmbedScriptPy(src=self._dest_file, doc_path=cp.src_path, model=self._model)
+        emb = EmbedScriptPy(
+            src=self._dest_file, doc_path=cp.src_path, model=self._model, build_dir=self._builder_args.build_dir
+        )
         emb.embed()
 
     # region Public Methods
     def build(self) -> bool:
         """
         Builds the plugin into the dist folder outlined in settings.json
         @return: `True` of the build is a success; Otherwise, `False`
```

### Comparing `oooscript-1.1.1/oooscript/build/copy_resource.py` & `oooscript-1.1.2/oooscript/build/copy_resource.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/oooscript/build/embed_py_script.py` & `oooscript-1.1.2/oooscript/build/embed_py_script.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 # coding: utf-8
 """
-Manages embeding a script into a LibreOffice Document
+Manages embedding a script into a LibreOffice Document
 
-Copies new docment into predefined build directory.
+Copies new document into predefined build directory.
 """
 from __future__ import annotations
 import os
 import zipfile
 import shutil
-from typing import List
+from typing import List, Union
 from pathlib import Path
 from .tmp_dir import tmpdir
 from .copy_resource import CopyResource
 from .manifest_script import ManifestScript
 from ..utils import paths
 from ..cfg import config
 from ..models.script_cfg.model_script_cfg import ModelScriptCfg as Model
 from . import build_util
 
 
 class EmbedScriptPy:
-    def __init__(self, src: str | Path | List[str], doc_path: str | Path | List[str], model: Model) -> None:
+    def __init__(
+        self,
+        src: str | Path | List[str],
+        doc_path: str | Path | List[str],
+        model: Model,
+        build_dir: Union[str, Path, None] = None,
+    ) -> None:
         """
         Constructor
 
         Args:
             src (Union[str, Path, List[str]]): Source File, this is usually is a file from build dir.
             doc_path (Union[str, Path, List[str]]): Path to resource LibreOffice document.
             model (ModelScriptCfg): Model for example.
         """
         self._src = paths.get_path(src, ensure_absolute=True)
         self._doc_path = paths.get_path(doc_path, ensure_absolute=True)
         self._model = model
         self._config = config.get_app_cfg()
+        self._build_dir = build_dir
 
     def embed(self) -> None:
         """
         Embeds python script in a LibreOffice Document and places doc in build dir.
         """
+
         # LO documents are zip file so this method unzip, adds script, updated manifest, rezips
         # and copies into build dir.
         def unzip(source: Path, dest: Path) -> None:
             with zipfile.ZipFile(str(source), "r") as zip_ref:
                 zip_ref.extractall(str(dest))
 
         def zipdir(unzipped_path: Path, ziph: zipfile.ZipFile):
@@ -58,39 +66,41 @@
                     ziph.write(
                         os.path.join(root, file),
                         os.path.relpath(os.path.join(root, file), os.path.join(unzipped_path, "..")),
                     )
 
         def zip_dir(unzipped_path: Path, dst_zip: Path) -> None:
             # https://ask.libreoffice.org/t/libreoffice-6-0-unzip-zip-open-document-file/40028
-            # mimefile must be first file in zip.
+            # mime file must be first file in zip.
             files = [p for p in unzipped_path.iterdir() if p.is_file()]
             subdirs = [p for p in unzipped_path.iterdir() if p.is_dir()]
-            with zipfile.ZipFile(dst_zip, "w", zipfile.ZIP_DEFLATED) as zipf:
+            with zipfile.ZipFile(dst_zip, "w", zipfile.ZIP_DEFLATED) as zip_f:
                 for file in files:
-
-                    pfile = file
-                    zipf.write(pfile, pfile.relative_to(unzipped_path))
+                    p_file = file
+                    zip_f.write(p_file, p_file.relative_to(unzipped_path))
                 for d in subdirs:
-                    zipdir(unzipped_path=d, ziph=zipf)
+                    zipdir(unzipped_path=d, ziph=zip_f)
 
         def get_odt_dest_path(tmp_dir: Path) -> Path:
             # path in tmpdir to zib version of LO document.
             src = self._doc_path
             dst = Path(tmp_dir, f"{src.stem}.zip")
             return dst
 
         def copy_script_to_unzipped(script_src: Path, zip_extract_dst: Path) -> None:
             p_script = zip_extract_dst / "Scripts" / "python"
             dst = Path(p_script, script_src.name)
             paths.mkdirp(p_script)
             shutil.copy2(script_src, dst)
 
         def copy_zipped_to_build(zip_file: Path) -> None:
-            build_path = build_util.get_build_path()
+            if self._build_dir is None:
+                build_path = build_util.get_build_path()
+            else:
+                build_path = self._build_dir
             paths.mkdirp(build_path)
             build_dest = Path(build_path, f"{self._model.args.output_name}{self._doc_path.suffix}")
             shutil.copy2(zip_file, build_dest)
 
         self._validate()
         with tmpdir() as temp_dir:
             p_tmp = Path(temp_dir)
@@ -104,26 +114,26 @@
             )
             cp.copy()
 
             zip_path = cp.dst_path
             zip_extract_dst = Path(p_tmp, zip_path.stem)
             unzip(source=zip_path, dest=zip_extract_dst)
 
-            # update manifest in unziped dir
+            # update manifest in unzipped dir
             manifest_path = zip_extract_dst / "META-INF" / "manifest.xml"
             mfs = ManifestScript(manifest_path=manifest_path, script_name=self._src.name)
             mfs.write(verify=True)
 
             # remove zip file in tmp dir.
             if zip_path.exists():
                 os.remove(zip_path)
 
             copy_script_to_unzipped(script_src=self._src, zip_extract_dst=zip_extract_dst)
 
-            # zip unzipped dir with the new embeded script files
+            # zip unzipped dir with the new embedded script files
             zip_dest = cp.dst_path.parent / f"{self._model.args.output_name}.zip"
             # zip_dir(unzipped_path=zip_extract_dst, dst_zip=cp.dst_path)
             zip_dir(unzipped_path=zip_extract_dst, dst_zip=zip_dest)
 
             copy_zipped_to_build(zip_dest)
             # tmp dir will not del.
```

### Comparing `oooscript-1.1.1/oooscript/build/manifest_script.py` & `oooscript-1.1.2/oooscript/build/manifest_script.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/oooscript/cfg/config.py` & `oooscript-1.1.2/oooscript/cfg/config.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/oooscript/cli/main.py` & `oooscript-1.1.2/oooscript/cli/main.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/oooscript/models/script_cfg/args.py` & `oooscript-1.1.2/oooscript/models/script_cfg/args.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/oooscript/models/script_cfg/model_script_cfg.py` & `oooscript-1.1.2/oooscript/models/script_cfg/model_script_cfg.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/oooscript/models/validators.py` & `oooscript-1.1.2/oooscript/models/validators.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/oooscript/res/docs/blank.odf` & `oooscript-1.1.2/oooscript/res/docs/blank.odf`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/oooscript/res/docs/blank.odg` & `oooscript-1.1.2/oooscript/res/docs/blank.odg`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/oooscript/res/docs/blank.odp` & `oooscript-1.1.2/oooscript/res/docs/blank.odp`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/oooscript/res/docs/blank.ods` & `oooscript-1.1.2/oooscript/res/docs/blank.ods`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/oooscript/res/docs/blank.odt` & `oooscript-1.1.2/oooscript/res/docs/blank.odt`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/oooscript/utils/enum_util.py` & `oooscript-1.1.2/oooscript/utils/enum_util.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/oooscript/utils/paths.py` & `oooscript-1.1.2/oooscript/utils/paths.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.1/pyproject.toml` & `oooscript-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oooscript"
-version = "1.1.1"
+version = "1.1.2"
 description = "Compiles several python scripts into a single script that can be eaisly used by LibreOffice as a macro."
 authors = [":Barry-Thomas-Paul: Moss <vibrationoflife@protonmail.com>"]
 homepage = "https://github.com/Amourspirit/python_libreoffice_oooscript"
 documentation = "https://oooscript.readthedocs.io/en/latest/"
 repository = "https://github.com/Amourspirit/python_libreoffice_oooscript"
 license = "MIT"
 readme = "README.md"
```

### Comparing `oooscript-1.1.1/PKG-INFO` & `oooscript-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oooscript
-Version: 1.1.1
+Version: 1.1.2
 Summary: Compiles several python scripts into a single script that can be eaisly used by LibreOffice as a macro.
 Home-page: https://github.com/Amourspirit/python_libreoffice_oooscript
 License: MIT
 Keywords: ooouno,libreoffice,stickytape,uno,pyuno,macro
 Author: :Barry-Thomas-Paul: Moss
 Author-email: vibrationoflife@protonmail.com
 Requires-Python: >=3.8,<4.0
```


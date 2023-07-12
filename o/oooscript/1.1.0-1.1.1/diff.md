# Comparing `tmp/oooscript-1.1.0.tar.gz` & `tmp/oooscript-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oooscript-1.1.0.tar", max compression
+gzip compressed data, was "oooscript-1.1.1.tar", max compression
```

## Comparing `oooscript-1.1.0.tar` & `oooscript-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rwxr-xr-x   0        0        0      316 2022-10-01 22:51:52.046019 oooscript-1.1.0/README.md
--rwxr-xr-x   0        0        0       71 2022-09-26 16:21:12.329300 oooscript-1.1.0/oooscript/.oooscript_root
--rwxr-xr-x   0        0        0      165 2022-10-01 21:39:16.817180 oooscript-1.1.0/oooscript/__init__.py
--rwxr-xr-x   0        0        0        0 2022-09-12 18:03:39.994876 oooscript-1.1.0/oooscript/build/__init__.py
--rwxr-xr-x   0        0        0     7573 2022-10-01 21:39:16.818438 oooscript-1.1.0/oooscript/build/build.py
--rwxr-xr-x   0        0        0      423 2022-09-26 16:21:12.331358 oooscript-1.1.0/oooscript/build/build_util.py
--rwxr-xr-x   0        0        0     3691 2022-10-01 21:39:16.819366 oooscript-1.1.0/oooscript/build/copy_resource.py
--rwxr-xr-x   0        0        0     5271 2022-10-01 21:38:58.797077 oooscript-1.1.0/oooscript/build/embed_py_script.py
--rwxr-xr-x   0        0        0     4659 2022-10-01 22:51:52.055266 oooscript-1.1.0/oooscript/build/manifest_script.py
--rwxr-xr-x   0        0        0      209 2022-09-26 16:21:12.336634 oooscript-1.1.0/oooscript/build/tmp_dir.py
--rwxr-xr-x   0        0        0        0 2022-09-13 16:08:22.450751 oooscript-1.1.0/oooscript/cfg/__init__.py
--rwxr-xr-x   0        0        0     3203 2023-07-06 20:04:39.651893 oooscript-1.1.0/oooscript/cfg/config.py
--rwxr-xr-x   0        0        0        0 2022-10-01 21:38:58.799643 oooscript-1.1.0/oooscript/cli/__init__.py
--rwxr-xr-x   0        0        0     2446 2022-10-01 21:39:16.821586 oooscript-1.1.0/oooscript/cli/main.py
--rwxr-xr-x   0        0        0        0 2022-09-12 18:26:31.865907 oooscript-1.1.0/oooscript/lib/__init__.py
--rwxr-xr-x   0        0        0      376 2022-09-12 18:26:59.276746 oooscript-1.1.0/oooscript/lib/enums.py
--rwxr-xr-x   0        0        0       40 2022-10-01 21:38:58.805512 oooscript-1.1.0/oooscript/lib/ex.py
--rwxr-xr-x   0        0        0        0 2022-09-12 18:24:13.737439 oooscript-1.1.0/oooscript/models/__init__.py
--rwxr-xr-x   0        0        0        0 2022-09-26 16:21:12.338808 oooscript-1.1.0/oooscript/models/script_cfg/__init__.py
--rwxr-xr-x   0        0        0      522 2022-10-01 21:39:16.823315 oooscript-1.1.0/oooscript/models/script_cfg/args.py
--rwxr-xr-x   0        0        0      640 2022-10-01 21:39:16.824695 oooscript-1.1.0/oooscript/models/script_cfg/model_script_cfg.py
--rwxr-xr-x   0        0        0      533 2022-09-12 18:24:13.773946 oooscript-1.1.0/oooscript/models/validators.py
--rwxr-xr-x   0        0        0       83 2022-09-13 15:24:25.505568 oooscript-1.1.0/oooscript/res/__init__.py
--rwxr-xr-x   0        0        0       88 2022-09-13 15:24:14.808773 oooscript-1.1.0/oooscript/res/docs/__init__.py
--rwxr-xr-x   0        0        0     3996 2022-09-26 16:21:12.342560 oooscript-1.1.0/oooscript/res/docs/blank.odf
--rwxr-xr-x   0        0        0     7979 2022-09-26 16:21:12.343538 oooscript-1.1.0/oooscript/res/docs/blank.odg
--rwxr-xr-x   0        0        0    15064 2022-09-26 16:21:12.344729 oooscript-1.1.0/oooscript/res/docs/blank.odp
--rwxr-xr-x   0        0        0     6968 2022-09-26 16:21:12.345631 oooscript-1.1.0/oooscript/res/docs/blank.ods
--rwxr-xr-x   0        0        0     8193 2022-09-13 15:18:46.583474 oooscript-1.1.0/oooscript/res/docs/blank.odt
--rwxr-xr-x   0        0        0        0 2022-09-12 18:04:27.526867 oooscript-1.1.0/oooscript/utils/__init__.py
--rwxr-xr-x   0        0        0     1155 2022-09-14 13:46:13.153083 oooscript-1.1.0/oooscript/utils/enum_util.py
--rwxr-xr-x   0        0        0    10031 2022-10-01 21:39:16.826146 oooscript-1.1.0/oooscript/utils/paths.py
--rwxr-xr-x   0        0        0     1866 2023-07-06 20:04:39.658628 oooscript-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 oooscript-1.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0      316 2023-07-12 17:11:29.592501 oooscript-1.1.1/README.md
+-rwxr-xr-x   0        0        0       71 2023-07-12 17:11:29.593500 oooscript-1.1.1/oooscript/.oooscript_root
+-rwxr-xr-x   0        0        0      165 2022-10-01 21:39:16.817180 oooscript-1.1.1/oooscript/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:03:39.994876 oooscript-1.1.1/oooscript/build/__init__.py
+-rwxr-xr-x   0        0        0     7955 2023-07-12 17:11:29.595534 oooscript-1.1.1/oooscript/build/build.py
+-rwxr-xr-x   0        0        0      423 2022-09-26 16:21:12.331358 oooscript-1.1.1/oooscript/build/build_util.py
+-rwxr-xr-x   0        0        0     3691 2022-10-01 21:39:16.819366 oooscript-1.1.1/oooscript/build/copy_resource.py
+-rwxr-xr-x   0        0        0     5271 2022-10-01 21:38:58.797077 oooscript-1.1.1/oooscript/build/embed_py_script.py
+-rwxr-xr-x   0        0        0     4659 2022-10-01 22:51:52.055266 oooscript-1.1.1/oooscript/build/manifest_script.py
+-rwxr-xr-x   0        0        0      209 2022-09-26 16:21:12.336634 oooscript-1.1.1/oooscript/build/tmp_dir.py
+-rwxr-xr-x   0        0        0        0 2022-09-13 16:08:22.450751 oooscript-1.1.1/oooscript/cfg/__init__.py
+-rwxr-xr-x   0        0        0     3203 2023-07-06 20:15:59.696122 oooscript-1.1.1/oooscript/cfg/config.py
+-rwxr-xr-x   0        0        0        0 2022-10-01 21:38:58.799643 oooscript-1.1.1/oooscript/cli/__init__.py
+-rwxr-xr-x   0        0        0     2854 2023-07-12 17:11:29.596405 oooscript-1.1.1/oooscript/cli/main.py
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:26:31.865907 oooscript-1.1.1/oooscript/lib/__init__.py
+-rwxr-xr-x   0        0        0      376 2022-09-12 18:26:59.276746 oooscript-1.1.1/oooscript/lib/enums.py
+-rwxr-xr-x   0        0        0       40 2022-10-01 21:38:58.805512 oooscript-1.1.1/oooscript/lib/ex.py
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:24:13.737439 oooscript-1.1.1/oooscript/models/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-09-26 16:21:12.338808 oooscript-1.1.1/oooscript/models/script_cfg/__init__.py
+-rwxr-xr-x   0        0        0      522 2022-10-01 21:39:16.823315 oooscript-1.1.1/oooscript/models/script_cfg/args.py
+-rwxr-xr-x   0        0        0      640 2022-10-01 21:39:16.824695 oooscript-1.1.1/oooscript/models/script_cfg/model_script_cfg.py
+-rwxr-xr-x   0        0        0      533 2022-09-12 18:24:13.773946 oooscript-1.1.1/oooscript/models/validators.py
+-rwxr-xr-x   0        0        0       83 2022-09-13 15:24:25.505568 oooscript-1.1.1/oooscript/res/__init__.py
+-rwxr-xr-x   0        0        0       88 2022-09-13 15:24:14.808773 oooscript-1.1.1/oooscript/res/docs/__init__.py
+-rwxr-xr-x   0        0        0     3996 2022-09-26 16:21:12.342560 oooscript-1.1.1/oooscript/res/docs/blank.odf
+-rwxr-xr-x   0        0        0     7979 2022-09-26 16:21:12.343538 oooscript-1.1.1/oooscript/res/docs/blank.odg
+-rwxr-xr-x   0        0        0    15064 2022-09-26 16:21:12.344729 oooscript-1.1.1/oooscript/res/docs/blank.odp
+-rwxr-xr-x   0        0        0     6968 2022-09-26 16:21:12.345631 oooscript-1.1.1/oooscript/res/docs/blank.ods
+-rwxr-xr-x   0        0        0     8193 2022-09-13 15:18:46.583474 oooscript-1.1.1/oooscript/res/docs/blank.odt
+-rwxr-xr-x   0        0        0        0 2022-09-12 18:04:27.526867 oooscript-1.1.1/oooscript/utils/__init__.py
+-rwxr-xr-x   0        0        0     1155 2022-09-14 13:46:13.153083 oooscript-1.1.1/oooscript/utils/enum_util.py
+-rwxr-xr-x   0        0        0    10031 2022-10-01 21:39:16.826146 oooscript-1.1.1/oooscript/utils/paths.py
+-rwxr-xr-x   0        0        0     1866 2023-07-12 17:11:29.597082 oooscript-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 oooscript-1.1.1/PKG-INFO
```

### Comparing `oooscript-1.1.0/oooscript/build/build.py` & `oooscript-1.1.1/oooscript/build/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 from __future__ import annotations
 import json
 from pathlib import Path
 import scriptmerge
 import os
 from dataclasses import dataclass
-from typing import List, Optional
+from typing import List, Optional, Union
 from distutils.sysconfig import get_python_lib
 from .embed_py_script import EmbedScriptPy
 from .copy_resource import CopyResource
 from ..utils import paths
 from ..cfg import config
 from ..models.script_cfg.model_script_cfg import ModelScriptCfg
 from ..lib.enums import AppTypeEnum
@@ -23,25 +23,29 @@
     """
     allow_print: bool = False
     """
     If True some print statements will be made in the terminal
     """
     embed_in_doc: bool = False
     """
-    If True then an odt file with embeded script is generated
+    If True then an odt file with embedded script is generated
     """
     embed_doc: Optional[str] = None
     """
     The document to embed compile script into.
     
     Requires ``embed_in_doc`` be ``True``.
     
     If ``embed_in_doc`` be ``True`` then the default used document to embed
     is internal .odt file.
     """
+    build_dir: Union[str, Path, None] = None
+    """
+    Build directory to place compiled script. Will override the build directory set by environment and config.json.
+    """
 
 
 class Builder:
     """Builder Class"""
 
     # region Constructor
     def __init__(self, args: BuilderArgs):
@@ -51,23 +55,24 @@
         Arguments:
             args (BuilderArgs): Builder Args
         """
         self._config = config.get_app_cfg()
         self._allow_print = args.allow_print
         self._embed = args.embed_in_doc
         self._embed_doc = args.embed_doc
+        self._builder_args = args
         self._dest_file = ""
         self._json_cfg = paths.get_path(path=args.config_json, ensure_absolute=True)
         # self._json_cfg = paths.get_path_from_lst(
         #     "src/examples/message_box/config.json".split("/"), ensure_absolute=True
         # )
         self._src_path = self._json_cfg.parent
         self._site_pkg_dir = None
-        jdata = json.loads(self._json_cfg.read_text())
-        self._model = ModelScriptCfg(**jdata)
+        j_data = json.loads(self._json_cfg.read_text())
+        self._model = ModelScriptCfg(**j_data)
         self._src_file = self._get_src_file()
         self._res_path = paths.get_pkg_res_path()
 
     # endregion Constructor
 
     def _get_src_file(self) -> Path:
         parts = self._model.args.src_file.replace("\\", "/").split("/")
@@ -129,15 +134,14 @@
             return self._res_path / "docs" / "blank.odf"
         elif t == AppTypeEnum.WRITER:
             return self._res_path / "docs" / "blank.odt"
         else:
             # base is not currently supported
             return None
 
-
     def _embed_script(self) -> None:
         if self._embed_doc is None:
             # src_doc = self._config.app_res_blank_odt
             src_doc = self._get_blank_embed_doc()
             if src_doc is None:
                 return None
         else:
@@ -148,53 +152,55 @@
 
     # region Public Methods
     def build(self) -> bool:
         """
         Builds the plugin into the dist folder outlined in settings.json
         @return: `True` of the build is a success; Otherwise, `False`
         """
-
-        dist_dir = paths.get_path(self._config.app_build_dir, ensure_absolute=True)
+        if self._builder_args.build_dir is not None:
+            dist_dir = paths.get_path(self._builder_args.build_dir, ensure_absolute=True)
+        else:
+            dist_dir = paths.get_path(self._config.app_build_dir, ensure_absolute=True)
         dest_file = dist_dir / f"{self._model.args.output_name}{self._src_file.suffix}"
         self._dest_file = str(dest_file)
 
         if not os.path.exists(dist_dir):
             os.makedirs(dist_dir)
             if self.allow_print:
                 print("Made Dir: " + dist_dir)
 
         if os.path.exists(self._dest_file):
             os.remove(self._dest_file)
             if self.allow_print:
                 print("Deleted File: " + self._dest_file)
         # region Make file using scriptmerge
-        # processer = "scriptmerge"
+        # processor = "scriptmerge"
         # site_inc_path = self._get_site_include_path()
         # params = f"'{self._src_file}' {site_inc_path} --output-file {self._dest_file!r}".replace(
         #     "  ", " "
         # ).strip()
-        # cmd = f"{processer} {params}"
+        # cmd = f"{processor} {params}"
         # if self.allow_print:
         #     print(cmd)
 
         # os.system(cmd)
 
         # sys.exit()
         if self._model.args.single_script:
-            with open(self._src_file, "r") as sfile:
-                output = sfile.read()
+            with open(self._src_file, "r") as s_file:
+                output = s_file.read()
         else:
-            # get exclude modules, don't worrie about duplicates, scriptmereg handles it.
+            # get exclude modules, don't worry about duplicates, scriptmerge handles it.
             exclude_modules = self._model.args.exclude_modules + self._config.build_exclude_modules
             output = scriptmerge.script(
                 path=str(self._src_file),
                 add_python_modules=[],
                 add_python_paths=self._get_include_paths(),
                 exclude_python_modules=exclude_modules,
-                clean=self._model.args.clean
+                clean=self._model.args.clean,
             )
         with open(self._dest_file, "w") as output_file:
             output_file.write(output)
         # endregion Make file using scriptmerge
         # region Append Global Exports
 
         # endregion Append Global Exports
```

### Comparing `oooscript-1.1.0/oooscript/build/copy_resource.py` & `oooscript-1.1.1/oooscript/build/copy_resource.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/oooscript/build/embed_py_script.py` & `oooscript-1.1.1/oooscript/build/embed_py_script.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/oooscript/build/manifest_script.py` & `oooscript-1.1.1/oooscript/build/manifest_script.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/oooscript/cfg/config.py` & `oooscript-1.1.1/oooscript/cfg/config.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/oooscript/cli/main.py` & `oooscript-1.1.1/oooscript/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 # region imports
 import sys
 import argparse
 
 from oooscript.build.build import Builder
 from oooscript.build.build import BuilderArgs
 from oooscript import __version__
+
 # endregion imports
 
 # region Parser
 
+
 # region    parser setup
 def _create_parser(name: str) -> argparse.ArgumentParser:
     return argparse.ArgumentParser(description=name)
 
 
 def _parse_args(parser: argparse.ArgumentParser):
     parser = _create_parser("main")
@@ -35,21 +37,39 @@
     parser.add_argument(
         "-e",
         "--embed",
         action="store_true",
         default=False,
         help="Determines if script is embedded in a LibreOffice Document",
     )
-    parser.add_argument("-d", "--embed-doc", type=str, default=None, help="Opional, LibreOffice document to embed script into.")
+    parser.add_argument(
+        "-d",
+        "--embed-doc",
+        type=str,
+        default=None,
+        dest="embed_doc",
+        help="Optional, LibreOffice document to embed script into.",
+    )
+    parser.add_argument(
+        "-b",
+        "--build-dir",
+        default=None,
+        dest="build_dir",
+        help="Optional, build directory to place compiled script. Can be relative or absolute path. Will override the build directory set by environment and config.json.",
+    )
+
 
 # endregion  parser setup
 
+
 # region        process arg command
 def _args_action_compile(a_parser: argparse.ArgumentParser, args: argparse.Namespace) -> None:
-    args = BuilderArgs(config_json=args.config, embed_in_doc=args.embed, embed_doc=args.embed_doc)
+    args = BuilderArgs(
+        config_json=args.config, embed_in_doc=args.embed, embed_doc=args.embed_doc, build_dir=args.build_dir
+    )
     builder = Builder(args)
     builder.build()
 
 
 def _args_action_version(a_parser: argparse.ArgumentParser, args: argparse.Namespace) -> None:
     print(__version__)
 
@@ -66,19 +86,20 @@
         a_parser.print_help()
 
 
 # endregion     process arg command
 
 # endregion Parser
 
+
 # region Main
 def main():
     parser = argparse.ArgumentParser()
     args = _parse_args(parser)
     _args_process_cmd(a_parser=parser, args=args)
     return 0
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
 
-# endregion Main
+# endregion Main
```

### Comparing `oooscript-1.1.0/oooscript/models/script_cfg/args.py` & `oooscript-1.1.1/oooscript/models/script_cfg/args.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/oooscript/models/script_cfg/model_script_cfg.py` & `oooscript-1.1.1/oooscript/models/script_cfg/model_script_cfg.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/oooscript/models/validators.py` & `oooscript-1.1.1/oooscript/models/validators.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/oooscript/res/docs/blank.odf` & `oooscript-1.1.1/oooscript/res/docs/blank.odf`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/oooscript/res/docs/blank.odg` & `oooscript-1.1.1/oooscript/res/docs/blank.odg`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/oooscript/res/docs/blank.odp` & `oooscript-1.1.1/oooscript/res/docs/blank.odp`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/oooscript/res/docs/blank.ods` & `oooscript-1.1.1/oooscript/res/docs/blank.ods`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/oooscript/res/docs/blank.odt` & `oooscript-1.1.1/oooscript/res/docs/blank.odt`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/oooscript/utils/enum_util.py` & `oooscript-1.1.1/oooscript/utils/enum_util.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/oooscript/utils/paths.py` & `oooscript-1.1.1/oooscript/utils/paths.py`

 * *Files identical despite different names*

### Comparing `oooscript-1.1.0/pyproject.toml` & `oooscript-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oooscript"
-version = "1.1.0"
+version = "1.1.1"
 description = "Compiles several python scripts into a single script that can be eaisly used by LibreOffice as a macro."
 authors = [":Barry-Thomas-Paul: Moss <vibrationoflife@protonmail.com>"]
 homepage = "https://github.com/Amourspirit/python_libreoffice_oooscript"
 documentation = "https://oooscript.readthedocs.io/en/latest/"
 repository = "https://github.com/Amourspirit/python_libreoffice_oooscript"
 license = "MIT"
 readme = "README.md"
```

### Comparing `oooscript-1.1.0/PKG-INFO` & `oooscript-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oooscript
-Version: 1.1.0
+Version: 1.1.1
 Summary: Compiles several python scripts into a single script that can be eaisly used by LibreOffice as a macro.
 Home-page: https://github.com/Amourspirit/python_libreoffice_oooscript
 License: MIT
 Keywords: ooouno,libreoffice,stickytape,uno,pyuno,macro
 Author: :Barry-Thomas-Paul: Moss
 Author-email: vibrationoflife@protonmail.com
 Requires-Python: >=3.8,<4.0
@@ -31,9 +31,9 @@
 
 # oooscript
 
 ![Tests](https://github.com/Amourspirit/python_libreoffice_oooscript/actions/workflows/tests.yml/badge.svg)
 
 Compiles one or more python scripts into a single script that can easily used as a LibreOffice macro.
 
-Documentation can be founc on [Read the Docs](https://oooscript.readthedocs.io/en/latest/)
+Documentation can be found on [Read the Docs](https://oooscript.readthedocs.io/en/latest/)
```


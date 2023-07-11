# Comparing `tmp/dapperdata-0.3.0.tar.gz` & `tmp/dapperdata-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapperdata-0.3.0.tar", last modified: Mon Jan 30 20:29:35 2023, max compression
+gzip compressed data, was "dapperdata-0.4.0.tar", last modified: Tue Jul 11 23:35:56 2023, max compression
```

## Comparing `dapperdata-0.3.0.tar` & `dapperdata-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:29:35.469142 dapperdata-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-30 20:29:08.000000 dapperdata-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-01-30 20:29:35.473142 dapperdata-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-30 20:29:08.000000 dapperdata-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:29:35.473142 dapperdata-0.3.0/dapperdata/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-30 20:29:08.000000 dapperdata-0.3.0/dapperdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-30 20:29:35.473142 dapperdata-0.3.0/dapperdata/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-01-30 20:29:08.000000 dapperdata-0.3.0/dapperdata/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:29:35.469142 dapperdata-0.3.0/dapperdata/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 20:29:08.000000 dapperdata-0.3.0/dapperdata/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-01-30 20:29:08.000000 dapperdata-0.3.0/dapperdata/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:29:35.469142 dapperdata-0.3.0/dapperdata/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 20:29:08.000000 dapperdata-0.3.0/dapperdata/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-30 20:29:08.000000 dapperdata-0.3.0/dapperdata/formatters/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-01-30 20:29:08.000000 dapperdata-0.3.0/dapperdata/formatters/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-30 20:29:08.000000 dapperdata-0.3.0/dapperdata/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:29:35.469142 dapperdata-0.3.0/dapperdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-01-30 20:29:35.000000 dapperdata-0.3.0/dapperdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-01-30 20:29:35.000000 dapperdata-0.3.0/dapperdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 20:29:35.000000 dapperdata-0.3.0/dapperdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-30 20:29:35.000000 dapperdata-0.3.0/dapperdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-30 20:29:35.000000 dapperdata-0.3.0/dapperdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-30 20:29:35.000000 dapperdata-0.3.0/dapperdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-30 20:29:08.000000 dapperdata-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-01-30 20:29:35.473142 dapperdata-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-01-30 20:29:08.000000 dapperdata-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:29:35.469142 dapperdata-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 20:29:08.000000 dapperdata-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-01-30 20:29:08.000000 dapperdata-0.3.0/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-01-30 20:29:08.000000 dapperdata-0.3.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-01-30 20:29:08.000000 dapperdata-0.3.0/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:35:56.874727 dapperdata-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 23:35:15.000000 dapperdata-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-11 23:35:56.874727 dapperdata-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-11 23:35:15.000000 dapperdata-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:35:56.874727 dapperdata-0.4.0/dapperdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 23:35:15.000000 dapperdata-0.4.0/dapperdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-11 23:35:56.878727 dapperdata-0.4.0/dapperdata/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-11 23:35:15.000000 dapperdata-0.4.0/dapperdata/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:35:56.874727 dapperdata-0.4.0/dapperdata/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 23:35:15.000000 dapperdata-0.4.0/dapperdata/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-11 23:35:15.000000 dapperdata-0.4.0/dapperdata/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:35:56.874727 dapperdata-0.4.0/dapperdata/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 23:35:15.000000 dapperdata-0.4.0/dapperdata/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-11 23:35:15.000000 dapperdata-0.4.0/dapperdata/formatters/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-11 23:35:15.000000 dapperdata-0.4.0/dapperdata/formatters/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 23:35:15.000000 dapperdata-0.4.0/dapperdata/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:35:56.874727 dapperdata-0.4.0/dapperdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-11 23:35:56.000000 dapperdata-0.4.0/dapperdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-11 23:35:56.000000 dapperdata-0.4.0/dapperdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 23:35:56.000000 dapperdata-0.4.0/dapperdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-11 23:35:56.000000 dapperdata-0.4.0/dapperdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 23:35:56.000000 dapperdata-0.4.0/dapperdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 23:35:56.000000 dapperdata-0.4.0/dapperdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-11 23:35:15.000000 dapperdata-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-11 23:35:56.878727 dapperdata-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 23:35:15.000000 dapperdata-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 23:35:56.874727 dapperdata-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 23:35:15.000000 dapperdata-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-11 23:35:15.000000 dapperdata-0.4.0/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 23:35:15.000000 dapperdata-0.4.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-11 23:35:15.000000 dapperdata-0.4.0/tests/test_yaml.py
```

### Comparing `dapperdata-0.3.0/LICENSE` & `dapperdata-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dapperdata-0.3.0/PKG-INFO` & `dapperdata-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapperdata
-Version: 0.3.0
+Version: 0.4.0
 Summary: An opinionated formatter for configuration files.
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # DapperData
```

### Comparing `dapperdata-0.3.0/README.md` & `dapperdata-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dapperdata-0.3.0/dapperdata/cli.py` & `dapperdata-0.4.0/dapperdata/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,72 +52,68 @@
 def format_directory(dirname: str, dry_run: bool = True, excluded_paths: Set[str] = set([])) -> Set[str]:
     changed_files = set([])
     excluded_paths = set([x.strip("/") for x in excluded_paths])
 
     # Pretty much never want to go into git management directories.
     excluded_paths.add(".git")
 
-    for (root, dirs, files) in os.walk(dirname, topdown=True):
-
+    for root, dirs, files in os.walk(dirname, topdown=True):
         if root.startswith("./"):
             root = root[2:]
 
         exclude_root = False
         for excluded_path in excluded_paths:
             if root == excluded_path:
                 exclude_root = True
                 break
 
         if exclude_root:
             # Remove directories to prevent them from being crawled.
             # This only works when `topdown` is True on the os.walk call.
-            for dir in dirs:
-                dirs.remove(dir)
+            dirs[:] = []
             continue
 
         for dir in dirs:
+            if dir.startswith("./"):
+                normalized_dir = dir[2:]
+            else:
+                normalized_dir = dir
             for excluded_path in excluded_paths:
-                if dir.startswith("./"):
-                    normalized_dir = dir[2:]
-                else:
-                    normalized_dir = dir
-                if normalized_dir == excluded_path:
+                if normalized_dir.startswith(excluded_path):
                     dirs.remove(dir)
+                    break
 
         for path in files:
             file_path = f"{root}/{path}"
-
             if file_path in excluded_paths:
                 continue
 
             if format_file(file_path, dry_run=dry_run):
                 changed_files.add(file_path)
 
     return changed_files
 
 
-@app.command()
+@app.command()  # type: ignore
 @click.argument("filename", type=click.Path(exists=True, file_okay=True, dir_okay=False))
 @click.option("-d", "--dry-run", default=True)
 def format(filename: str, dry_run: bool = True):
     print(f"Formatting {filename}")
     if format_file(filename, dry_run=dry_run):
         print("Changes detected.")
     else:
         print("No changes detected.")
 
 
-@app.command()
+@app.command()  # type: ignore
 @click.argument("dirname", type=click.Path(exists=True, file_okay=False, dir_okay=True))
 @click.option("--dry-run", "-d", default=True)
 def pretty(dirname: str, dry_run: bool = True):
-
     if dry_run:
         typer.echo("Dry Run- No changes will be made.")
-
     changed_files = format_directory(dirname, dry_run, excluded_paths=settings.exclude_paths)
 
     if len(changed_files):
         if dry_run:
             typer.echo("Changes needed in the following files:")
             for file in changed_files:
                 typer.echo(f"{TYPER_FAILURE} {file}")
```

### Comparing `dapperdata-0.3.0/dapperdata/conf/settings.py` & `dapperdata-0.4.0/dapperdata/conf/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 from typing import List, Set
 
-from pydantic import BaseSettings
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
 
 default_data = {}
@@ -32,15 +32,13 @@
                 continue
             gitignore_directories.add(line_string)
     if len(gitignore_directories) > 0:
         default_data["exclude_paths"] = set(default_data.get("exclude_paths", [])) | gitignore_directories
 
 
 class Settings(BaseSettings):
-
     project_name: str = "pretty-config"
     debug: bool = False
 
     exclude_paths: Set[str] = default_data.get("exclude_paths", [])
 
-    class Config:
-        env_prefix = "dapperdata_"
+    model_config = SettingsConfigDict(env_prefix="dapperdata_")
```

### Comparing `dapperdata-0.3.0/dapperdata/formatters/yaml.py` & `dapperdata-0.4.0/dapperdata/formatters/yaml.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 #
 # Overload the comment writer to remove superfluous newlines.
 #
 
 # Save the original comment writer so our extended version can use it.
 ruamel.yaml.emitter.Emitter.write_comment_original = ruamel.yaml.emitter.Emitter.write_comment  # type: ignore
 
+
 # Create the new comment writer.
 def strip_empty_lines_write_comment(self, comment: Any, pre: bool = False) -> None:
     # Check if comment is nothing but newlines.
     # Then replace with a single new line.
     string_check = comment.value.replace("\n", "")
     if len(string_check) == 0:
         comment.value = "\n"
```

### Comparing `dapperdata-0.3.0/dapperdata.egg-info/PKG-INFO` & `dapperdata-0.4.0/dapperdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapperdata
-Version: 0.3.0
+Version: 0.4.0
 Summary: An opinionated formatter for configuration files.
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # DapperData
```

### Comparing `dapperdata-0.3.0/dapperdata.egg-info/SOURCES.txt` & `dapperdata-0.4.0/dapperdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dapperdata-0.3.0/pyproject.toml` & `dapperdata-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dapperdata-0.3.0/setup.cfg` & `dapperdata-0.4.0/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -21,28 +21,29 @@
 00000140: 6566 6978 203d 2076 0a70 6172 656e 7464  efix = v.parentd
 00000150: 6972 5f70 7265 6669 7820 3d20 0a0a 5b6f  ir_prefix = ..[o
 00000160: 7074 696f 6e73 5d0a 7061 636b 6167 6573  ptions].packages
 00000170: 203d 2066 696e 643a 0a69 6e63 6c75 6465   = find:.include
 00000180: 5f70 6163 6b61 6765 5f64 6174 6120 3d20  _package_data = 
 00000190: 5472 7565 0a69 6e73 7461 6c6c 5f72 6571  True.install_req
 000001a0: 7569 7265 7320 3d20 0a09 7079 6461 6e74  uires = ..pydant
-000001b0: 6963 0a09 7479 7065 720a 0972 7561 6d65  ic..typer..ruame
-000001c0: 6c2e 7961 6d6c 0a09 746f 6d6c 693e 3d31  l.yaml..tomli>=1
-000001d0: 2e31 2e30 3b70 7974 686f 6e5f 7665 7273  .1.0;python_vers
-000001e0: 696f 6e3c 2733 2e31 3127 0a0a 5b6f 7074  ion<'3.11'..[opt
-000001f0: 696f 6e73 2e65 7874 7261 735f 7265 7175  ions.extras_requ
-00000200: 6972 655d 0a64 6576 203d 200a 0962 6c61  ire].dev = ..bla
-00000210: 636b 0a09 6275 696c 640a 0967 6c6f 6d0a  ck..build..glom.
-00000220: 0969 736f 7274 0a09 6d79 7079 0a09 7069  .isort..mypy..pi
-00000230: 702d 746f 6f6c 730a 0970 7974 6573 740a  p-tools..pytest.
-00000240: 0970 7974 6573 742d 636f 760a 0970 7974  .pytest-cov..pyt
-00000250: 6573 742d 7072 6574 7479 0a0a 5b6f 7074  est-pretty..[opt
-00000260: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
-00000270: 615d 0a64 6170 7065 7264 6174 6120 3d20  a].dapperdata = 
-00000280: 7079 2e74 7970 6564 0a0a 5b6f 7074 696f  py.typed..[optio
-00000290: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-000002a0: 0a63 6f6e 736f 6c65 5f73 6372 6970 7473  .console_scripts
-000002b0: 203d 200a 0964 6170 7065 7264 6174 6120   = ..dapperdata 
-000002c0: 3d20 6461 7070 6572 6461 7461 2e63 6c69  = dapperdata.cli
-000002d0: 3a61 7070 0a0a 5b65 6767 5f69 6e66 6f5d  :app..[egg_info]
-000002e0: 0a74 6167 5f62 7569 6c64 203d 200a 7461  .tag_build = .ta
-000002f0: 675f 6461 7465 203d 2030 0a0a            g_date = 0..
+000001b0: 6963 0a09 7079 6461 6e74 6963 2d73 6574  ic..pydantic-set
+000001c0: 7469 6e67 730a 0974 7970 6572 0a09 7275  tings..typer..ru
+000001d0: 616d 656c 2e79 616d 6c0a 0974 6f6d 6c69  amel.yaml..tomli
+000001e0: 3e3d 312e 312e 303b 7079 7468 6f6e 5f76  >=1.1.0;python_v
+000001f0: 6572 7369 6f6e 3c27 332e 3131 270a 0a5b  ersion<'3.11'..[
+00000200: 6f70 7469 6f6e 732e 6578 7472 6173 5f72  options.extras_r
+00000210: 6571 7569 7265 5d0a 6465 7620 3d20 0a09  equire].dev = ..
+00000220: 626c 6163 6b0a 0962 7569 6c64 0a09 676c  black..build..gl
+00000230: 6f6d 0a09 6973 6f72 740a 096d 7970 790a  om..isort..mypy.
+00000240: 0970 6970 2d74 6f6f 6c73 0a09 7079 7465  .pip-tools..pyte
+00000250: 7374 0a09 7079 7465 7374 2d63 6f76 0a09  st..pytest-cov..
+00000260: 7079 7465 7374 2d70 7265 7474 790a 0a5b  pytest-pretty..[
+00000270: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
+00000280: 6461 7461 5d0a 6461 7070 6572 6461 7461  data].dapperdata
+00000290: 203d 2070 792e 7479 7065 640a 0a5b 6f70   = py.typed..[op
+000002a0: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+000002b0: 7473 5d0a 636f 6e73 6f6c 655f 7363 7269  ts].console_scri
+000002c0: 7074 7320 3d20 0a09 6461 7070 6572 6461  pts = ..dapperda
+000002d0: 7461 203d 2064 6170 7065 7264 6174 612e  ta = dapperdata.
+000002e0: 636c 693a 6170 700a 0a5b 6567 675f 696e  cli:app..[egg_in
+000002f0: 666f 5d0a 7461 675f 6275 696c 6420 3d20  fo].tag_build = 
+00000300: 0a74 6167 5f64 6174 6520 3d20 300a 0a    .tag_date = 0..
```


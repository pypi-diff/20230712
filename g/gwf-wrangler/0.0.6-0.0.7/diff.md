# Comparing `tmp/gwf_wrangler-0.0.6.tar.gz` & `tmp/gwf_wrangler-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwf_wrangler-0.0.6.tar", last modified: Sun Jul  9 04:08:06 2023, max compression
+gzip compressed data, was "gwf_wrangler-0.0.7.tar", last modified: Wed Jul 12 19:37:06 2023, max compression
```

## Comparing `gwf_wrangler-0.0.6.tar` & `gwf_wrangler-0.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-09 04:08:06.848002 gwf_wrangler-0.0.6/
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1052 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.6/LICENSE
--rw-rw-r--   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.6/MANIFEST.in
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     4774 2023-07-09 04:08:06.848002 gwf_wrangler-0.0.6/PKG-INFO
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     3031 2023-07-09 04:04:17.000000 gwf_wrangler-0.0.6/README.md
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-09 04:08:06.844001 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     4774 2023-07-09 04:08:06.000000 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/PKG-INFO
--rw-rw-r--   0 rlong     (1000) rlong     (1000)      647 2023-07-09 04:08:06.000000 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/SOURCES.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)        1 2023-07-09 04:08:06.000000 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/dependency_links.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)       47 2023-07-09 04:08:06.000000 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/entry_points.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)       63 2023-07-09 04:08:06.000000 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/requires.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)       29 2023-07-09 04:08:06.000000 gwf_wrangler-0.0.6/gwf_wrangler.egg-info/top_level.txt
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1255 2023-07-09 04:07:56.000000 gwf_wrangler-0.0.6/pyproject.toml
--rw-rw-r--   0 rlong     (1000) rlong     (1000)       38 2023-07-09 04:08:06.848002 gwf_wrangler-0.0.6/setup.cfg
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-09 04:08:06.844001 gwf_wrangler-0.0.6/src/
--rw-rw-r--   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.6/src/__init__.py
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     3848 2023-07-09 03:53:20.000000 gwf_wrangler-0.0.6/src/__main__.py
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1435 2023-07-09 03:08:58.000000 gwf_wrangler-0.0.6/src/cli.py
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     2014 2023-07-09 02:43:34.000000 gwf_wrangler-0.0.6/src/mapper.py
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1200 2023-07-09 02:56:07.000000 gwf_wrangler-0.0.6/src/script.py
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-09 04:08:06.844001 gwf_wrangler-0.0.6/tests/
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1087 2023-07-09 03:51:36.000000 gwf_wrangler-0.0.6/tests/test_main.py
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-09 04:08:06.844001 gwf_wrangler-0.0.6/venv/
-drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-09 04:08:06.848002 gwf_wrangler-0.0.6/venv/bin/
--rw-rw-r--   0 rlong     (1000) rlong     (1000)     1176 2023-07-01 20:23:27.000000 gwf_wrangler-0.0.6/venv/bin/activate_this.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      631 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2html.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      753 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2html4.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)     1088 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2html5.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      830 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2latex.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      653 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2man.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      819 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2odt.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      625 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      638 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      674 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2s5.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      910 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2xetex.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      639 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rst2xml.py
--rwxrwxr-x   0 rlong     (1000) rlong     (1000)      707 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.6/venv/bin/rstpep2html.py
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-12 19:37:06.877118 gwf_wrangler-0.0.7/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1052 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.7/LICENSE
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.7/MANIFEST.in
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     4774 2023-07-12 19:37:06.877118 gwf_wrangler-0.0.7/PKG-INFO
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     3031 2023-07-12 19:35:55.000000 gwf_wrangler-0.0.7/README.md
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-12 19:37:06.869118 gwf_wrangler-0.0.7/gwf_wrangler.egg-info/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     4774 2023-07-12 19:37:06.000000 gwf_wrangler-0.0.7/gwf_wrangler.egg-info/PKG-INFO
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)      647 2023-07-12 19:37:06.000000 gwf_wrangler-0.0.7/gwf_wrangler.egg-info/SOURCES.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)        1 2023-07-12 19:37:06.000000 gwf_wrangler-0.0.7/gwf_wrangler.egg-info/dependency_links.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)       47 2023-07-12 19:37:06.000000 gwf_wrangler-0.0.7/gwf_wrangler.egg-info/entry_points.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)       63 2023-07-12 19:37:06.000000 gwf_wrangler-0.0.7/gwf_wrangler.egg-info/requires.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)       29 2023-07-12 19:37:06.000000 gwf_wrangler-0.0.7/gwf_wrangler.egg-info/top_level.txt
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1255 2023-07-12 19:35:55.000000 gwf_wrangler-0.0.7/pyproject.toml
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)       38 2023-07-12 19:37:06.877118 gwf_wrangler-0.0.7/setup.cfg
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-12 19:37:06.873118 gwf_wrangler-0.0.7/src/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)        0 2023-07-01 20:09:07.000000 gwf_wrangler-0.0.7/src/__init__.py
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     3849 2023-07-12 19:30:49.000000 gwf_wrangler-0.0.7/src/__main__.py
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1435 2023-07-09 03:08:58.000000 gwf_wrangler-0.0.7/src/cli.py
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     2014 2023-07-09 02:43:34.000000 gwf_wrangler-0.0.7/src/mapper.py
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1200 2023-07-09 02:56:07.000000 gwf_wrangler-0.0.7/src/script.py
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-12 19:37:06.873118 gwf_wrangler-0.0.7/tests/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1087 2023-07-09 03:51:36.000000 gwf_wrangler-0.0.7/tests/test_main.py
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-12 19:37:06.869118 gwf_wrangler-0.0.7/venv/
+drwxrwxr-x   0 rlong     (1000) rlong     (1000)        0 2023-07-12 19:37:06.873118 gwf_wrangler-0.0.7/venv/bin/
+-rw-rw-r--   0 rlong     (1000) rlong     (1000)     1176 2023-07-01 20:23:27.000000 gwf_wrangler-0.0.7/venv/bin/activate_this.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      631 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.7/venv/bin/rst2html.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      753 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.7/venv/bin/rst2html4.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)     1088 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.7/venv/bin/rst2html5.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      830 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.7/venv/bin/rst2latex.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      653 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.7/venv/bin/rst2man.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      819 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.7/venv/bin/rst2odt.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      625 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.7/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      638 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.7/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      674 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.7/venv/bin/rst2s5.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      910 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.7/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      639 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.7/venv/bin/rst2xml.py
+-rwxrwxr-x   0 rlong     (1000) rlong     (1000)      707 2023-07-01 21:11:13.000000 gwf_wrangler-0.0.7/venv/bin/rstpep2html.py
```

### Comparing `gwf_wrangler-0.0.6/LICENSE` & `gwf_wrangler-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/PKG-INFO` & `gwf_wrangler-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwf_wrangler
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python package to convert yaml files to lua scripts for the Global Workflow Project.
 Author-email: Ryan Long <ryan.long@noaa.gov>
 License: Copyright 2023 NOAA
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-# Wrangler (0.0.5)
+# Wrangler (0.0.7)
 
 ## Logging
 
 ### Use the Correct Levels When Logging
 
 It might be difficult to decide which level to assign each event. Fortunately, the Python logging module presents fewer levels than other logging libraries. This makes things easier by eliminating some potential ambiguity. When it comes to Python levels, here are the general guidelines:
```

### Comparing `gwf_wrangler-0.0.6/README.md` & `gwf_wrangler-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# Wrangler (0.0.5)
+# Wrangler (0.0.7)
 
 ## Logging
 
 ### Use the Correct Levels When Logging
 
 It might be difficult to decide which level to assign each event. Fortunately, the Python logging module presents fewer levels than other logging libraries. This makes things easier by eliminating some potential ambiguity. When it comes to Python levels, here are the general guidelines:
```

### Comparing `gwf_wrangler-0.0.6/gwf_wrangler.egg-info/PKG-INFO` & `gwf_wrangler-0.0.7/gwf_wrangler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwf-wrangler
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python package to convert yaml files to lua scripts for the Global Workflow Project.
 Author-email: Ryan Long <ryan.long@noaa.gov>
 License: Copyright 2023 NOAA
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
-# Wrangler (0.0.5)
+# Wrangler (0.0.7)
 
 ## Logging
 
 ### Use the Correct Levels When Logging
 
 It might be difficult to decide which level to assign each event. Fortunately, the Python logging module presents fewer levels than other logging libraries. This makes things easier by eliminating some potential ambiguity. When it comes to Python levels, here are the general guidelines:
```

### Comparing `gwf_wrangler-0.0.6/gwf_wrangler.egg-info/SOURCES.txt` & `gwf_wrangler-0.0.7/gwf_wrangler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/pyproject.toml` & `gwf_wrangler-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "versioneer[toml]"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gwf_wrangler"
 description = "A python package to convert yaml files to lua scripts for the Global Workflow Project."
 readme = "README.md"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = ["PyYAML"]
 authors = [{ name = "Ryan Long", email = "ryan.long@noaa.gov" }]
 keywords = ["globalworkflow", "global workflow", "esmf"]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
@@ -29,15 +29,15 @@
 "Homepage" = "https://github.com/pypa/gwf-wrangler"
 "Bug Tracker" = "https://github.com/pypa/gwf-wrangler/issues"
 
 [tool.setuptools.packages]
 find = {} # Scan the project directory with the default parameters
 
 [tool.bumpver]
-current_version = "0.0.4"
+current_version = "0.0.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `gwf_wrangler-0.0.6/src/__main__.py` & `gwf_wrangler-0.0.7/src/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     except ScriptNotFound:
         return []
 
 
 def get_postpend_script(scripts):
     """returns the lua content of a postpend script if it exists"""
     try:
-        return get_content(find_script("^pre", scripts))
+        return get_content(find_script("^post", scripts))
     except ScriptNotFound:
         return []
 
 
 def get_bookend_scripts_content(scripts: list[Script]) -> Tuple[list[str], ...]:
     """returns the prepend and postpend scripts if thy exist"""
     return (get_prepend_script(scripts), get_postpend_script(scripts))
@@ -87,16 +87,16 @@
         Path(output_path / Path(f"{script.name}.lua")), "w", encoding="utf-8"
     ) as _output:
         _output.writelines(script.get_as_lua("help"))
         _output.writelines(prepend_script)
         _output.writelines(script.get_as_lua("modulepaths"))
         _output.writelines(script.get_as_lua("modules"))
         _output.writelines(script.get_as_lua("environment"))
-        _output.writelines(script.get_as_lua("^extra"))
         _output.writelines(postpend_script)
+        _output.writelines(script.get_as_lua("^extra"))
         _output.writelines(script.get_as_lua("whatis"))
 
 
 def scripts_to_process(scripts) -> list[Script]:
     """returns list of scripts to process excluding those
     denoted with a special character"""
     return [x for x in scripts if KEYWORD_INDICATOR not in x.name]
```

### Comparing `gwf_wrangler-0.0.6/src/cli.py` & `gwf_wrangler-0.0.7/src/cli.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/src/mapper.py` & `gwf_wrangler-0.0.7/src/mapper.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/src/script.py` & `gwf_wrangler-0.0.7/src/script.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/tests/test_main.py` & `gwf_wrangler-0.0.7/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/venv/bin/activate_this.py` & `gwf_wrangler-0.0.7/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/venv/bin/rst2html.py` & `gwf_wrangler-0.0.7/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/venv/bin/rst2html4.py` & `gwf_wrangler-0.0.7/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/venv/bin/rst2html5.py` & `gwf_wrangler-0.0.7/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/venv/bin/rst2latex.py` & `gwf_wrangler-0.0.7/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/venv/bin/rst2man.py` & `gwf_wrangler-0.0.7/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/venv/bin/rst2odt.py` & `gwf_wrangler-0.0.7/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/venv/bin/rst2odt_prepstyles.py` & `gwf_wrangler-0.0.7/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/venv/bin/rst2pseudoxml.py` & `gwf_wrangler-0.0.7/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/venv/bin/rst2s5.py` & `gwf_wrangler-0.0.7/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/venv/bin/rst2xetex.py` & `gwf_wrangler-0.0.7/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/venv/bin/rst2xml.py` & `gwf_wrangler-0.0.7/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `gwf_wrangler-0.0.6/venv/bin/rstpep2html.py` & `gwf_wrangler-0.0.7/venv/bin/rstpep2html.py`

 * *Files identical despite different names*


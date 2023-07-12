# Comparing `tmp/click_schema_config-0.2.0.tar.gz` & `tmp/click_schema_config-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_schema_config-0.2.0.tar", max compression
+gzip compressed data, was "click_schema_config-0.2.1.tar", max compression
```

## Comparing `click_schema_config-0.2.0.tar` & `click_schema_config-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1069 2023-07-12 09:20:50.939061 click_schema_config-0.2.0/LICENSE
--rwxr-xr-x   0        0        0     5255 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/README.md
--rwxr-xr-x   0        0        0      150 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/__init__.py
--rwxr-xr-x   0        0        0     2318 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/click.py
--rw-r--r--   0        0        0     3320 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/commands/codegen.py
--rw-r--r--   0        0        0       69 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/commands/templates/__init__.py.jinja
--rw-r--r--   0        0        0      768 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/commands/templates/dataclass.py.jinja
--rw-r--r--   0        0        0        0 2023-07-12 09:20:50.947061 click_schema_config-0.2.0/click_schema_config/py.typed
--rwxr-xr-x   0        0        0     3585 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/read_config.py
--rw-r--r--   0        0        0      408 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/click_schema_config/types.py
--rwxr-xr-x   0        0        0      681 2023-07-12 09:20:50.955062 click_schema_config-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5844 1970-01-01 00:00:00.000000 click_schema_config-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-07-12 10:09:59.473612 click_schema_config-0.2.1/LICENSE
+-rwxr-xr-x   0        0        0     5255 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/README.md
+-rwxr-xr-x   0        0        0      150 2023-07-12 10:09:59.477612 click_schema_config-0.2.1/click_schema_config/__init__.py
+-rwxr-xr-x   0        0        0     2318 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/click_schema_config/click.py
+-rw-r--r--   0        0        0     3320 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/click_schema_config/commands/codegen.py
+-rw-r--r--   0        0        0       69 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/click_schema_config/commands/templates/__init__.py.jinja
+-rw-r--r--   0        0        0      768 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/click_schema_config/commands/templates/dataclass.py.jinja
+-rw-r--r--   0        0        0        0 2023-07-12 10:09:59.473612 click_schema_config-0.2.1/click_schema_config/py.typed
+-rwxr-xr-x   0        0        0     3585 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/click_schema_config/read_config.py
+-rw-r--r--   0        0        0      408 2023-07-12 10:09:59.481612 click_schema_config-0.2.1/click_schema_config/types.py
+-rwxr-xr-x   0        0        0      698 2023-07-12 10:09:59.485612 click_schema_config-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5883 1970-01-01 00:00:00.000000 click_schema_config-0.2.1/PKG-INFO
```

### Comparing `click_schema_config-0.2.0/LICENSE` & `click_schema_config-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.0/README.md` & `click_schema_config-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.0/click_schema_config/click.py` & `click_schema_config-0.2.1/click_schema_config/click.py`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.0/click_schema_config/commands/codegen.py` & `click_schema_config-0.2.1/click_schema_config/commands/codegen.py`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.0/click_schema_config/commands/templates/dataclass.py.jinja` & `click_schema_config-0.2.1/click_schema_config/commands/templates/dataclass.py.jinja`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.0/click_schema_config/read_config.py` & `click_schema_config-0.2.1/click_schema_config/read_config.py`

 * *Files identical despite different names*

### Comparing `click_schema_config-0.2.0/pyproject.toml` & `click_schema_config-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "click-schema-config"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Joy Void Joy <joy.void.joy@gmail.com>"]
 readme = "README.md"
 packages = [{include = "click_schema_config"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.4"
 pyyaml = "^6.0"
 pydantic = "^2.0.2"
 jinja2 = "^3.1.2"
 black = {version = "^22.8.0", allow-prereleases = true}
 types-click = "^7.1.8"
+halo = "^0.0.31"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 ipython = "^8.14.0"
 halo = "^0.0.31"
 types-pyyaml = "^6.0.12.10"
```

### Comparing `click_schema_config-0.2.0/PKG-INFO` & `click_schema_config-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: click-schema-config
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Joy Void Joy
 Author-email: joy.void.joy@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=22.8.0,<23.0.0)
 Requires-Dist: click (>=8.1.4,<9.0.0)
+Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: types-click (>=7.1.8,<8.0.0)
 Description-Content-Type: text/markdown
 
 # click-schema-config
```


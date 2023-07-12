# Comparing `tmp/utilki-0.6.1.tar.gz` & `tmp/utilki-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.6.1.tar", max compression
+gzip compressed data, was "utilki-0.6.2.tar", max compression
```

## Comparing `utilki-0.6.1.tar` & `utilki-0.6.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-28 16:08:26.749752 utilki-0.6.1/README.md
--rw-r--r--   0        0        0      525 2023-06-28 16:08:26.749752 utilki-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-28 16:08:26.749752 utilki-0.6.1/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-06-28 16:08:26.749752 utilki-0.6.1/utilki/cli.py
--rw-r--r--   0        0        0     6761 2023-06-28 16:08:26.749752 utilki-0.6.1/utilki/log_utils.py
--rw-r--r--   0        0        0     7325 2023-06-28 16:08:26.749752 utilki-0.6.1/utilki/task_mixin.py
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 utilki-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-12 02:38:23.539777 utilki-0.6.2/README.md
+-rw-r--r--   0        0        0      525 2023-07-12 02:38:23.539777 utilki-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-07-12 02:38:23.539777 utilki-0.6.2/utilki/__init__.py
+-rw-r--r--   0        0        0     2257 2023-07-12 02:38:23.539777 utilki-0.6.2/utilki/cli.py
+-rw-r--r--   0        0        0     6761 2023-07-12 02:38:23.539777 utilki-0.6.2/utilki/log_utils.py
+-rw-r--r--   0        0        0     7325 2023-07-12 02:38:23.539777 utilki-0.6.2/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 utilki-0.6.2/PKG-INFO
```

### Comparing `utilki-0.6.1/README.md` & `utilki-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.6.1/pyproject.toml` & `utilki-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utilki"
-version = "0.6.1"
+version = "0.6.2"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 click = "^8.1.3"
```

### Comparing `utilki-0.6.1/utilki/cli.py` & `utilki-0.6.2/utilki/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     res = subprocess.run(
         ["pyenv", "install", "--list"],
         capture_output=True,
         text=True,
     )
     if res.returncode != 0:
         click.echo(res.stderr)
-        return
+        return []
     versions = res.stdout.splitlines()
     return [version.strip() for version in versions[1:]]
 
 
 @click.group(name="utilki")
 def cli():
     pass
@@ -24,14 +24,15 @@
 @click.argument(
     "python_version",
     type=click.Choice(get_list_of_python_versions()),
     default="3.8.10",
 )
 def venv(python_version):
     # Create the virtual environment with the given name and Python version
+    click.echo(f"Creating venv with Python version {python_version}")
     venv_name = click.prompt("Enter venv name", type=str)
     res = subprocess.run(
         ["pyenv", "virtualenv", python_version, venv_name],
         capture_output=True,
         text=True,
     )
     if res.returncode != 0:
```

### Comparing `utilki-0.6.1/utilki/log_utils.py` & `utilki-0.6.2/utilki/log_utils.py`

 * *Files identical despite different names*

### Comparing `utilki-0.6.1/utilki/task_mixin.py` & `utilki-0.6.2/utilki/task_mixin.py`

 * *Files identical despite different names*

### Comparing `utilki-0.6.1/PKG-INFO` & `utilki-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.6.1
+Version: 0.6.2
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```


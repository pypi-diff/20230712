# Comparing `tmp/app_confetti-0.2.0.tar.gz` & `tmp/app_confetti-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_confetti-0.2.0.tar", max compression
+gzip compressed data, was "app_confetti-0.3.0.tar", max compression
```

## Comparing `app_confetti-0.2.0.tar` & `app_confetti-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1849 2023-02-19 13:08:09.666085 app_confetti-0.2.0/README.md
--rw-r--r--   0        0        0       44 2023-02-19 13:08:09.666085 app_confetti-0.2.0/app_confetti/__init__.py
--rw-r--r--   0        0        0       84 2023-02-19 13:04:02.348294 app_confetti-0.2.0/app_confetti/fetch/__init__.py
--rw-r--r--   0        0        0     3116 2023-02-19 13:04:59.307699 app_confetti-0.2.0/app_confetti/fetch/aws.py
--rw-r--r--   0        0        0      431 2023-02-19 13:02:25.982469 app_confetti-0.2.0/app_confetti/fetch/dotenv.py
--rw-r--r--   0        0        0     1506 2023-02-19 13:04:02.351294 app_confetti-0.2.0/app_confetti/util.py
--rw-r--r--   0        0        0     2035 2023-02-19 13:08:09.665085 app_confetti-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2935 1970-01-01 00:00:00.000000 app_confetti-0.2.0/setup.py
--rw-r--r--   0        0        0     2733 1970-01-01 00:00:00.000000 app_confetti-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2449 2023-07-12 10:55:47.996430 app_confetti-0.3.0/README.md
+-rw-r--r--   0        0        0       44 2023-07-12 10:55:47.996430 app_confetti-0.3.0/app_confetti/__init__.py
+-rw-r--r--   0        0        0       84 2023-02-19 13:04:02.348294 app_confetti-0.3.0/app_confetti/fetch/__init__.py
+-rw-r--r--   0        0        0     3116 2023-02-19 13:04:59.307699 app_confetti-0.3.0/app_confetti/fetch/aws.py
+-rw-r--r--   0        0        0      431 2023-02-19 13:02:25.982469 app_confetti-0.3.0/app_confetti/fetch/dotenv.py
+-rw-r--r--   0        0        0     1503 2023-07-12 10:52:46.378496 app_confetti-0.3.0/app_confetti/util.py
+-rw-r--r--   0        0        0     2039 2023-07-12 10:55:47.996430 app_confetti-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3331 1970-01-01 00:00:00.000000 app_confetti-0.3.0/PKG-INFO
```

### Comparing `app_confetti-0.2.0/app_confetti/fetch/aws.py` & `app_confetti-0.3.0/app_confetti/fetch/aws.py`

 * *Files identical despite different names*

### Comparing `app_confetti-0.2.0/app_confetti/util.py` & `app_confetti-0.3.0/app_confetti/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,11 +36,11 @@
                 value = default
             else:
                 raise KeyError(key)
 
         try:
             return convert(value)
         except ValueError as e:
-            msg = f"{key} {str(e)}"
+            msg = f"{key} {e!s}"
             raise ValueError(msg) from e
 
     return dataclasses.field(default_factory=default_factory, **kwargs)
```

### Comparing `app_confetti-0.2.0/pyproject.toml` & `app_confetti-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "app_confetti"
-version = "0.2.0"
+version = "0.3.0"
 description = "Environment application configuration"
 authors = ["Daniel Edgecombe <edgy.edgemond@gmail.com>"]
 license = "Apache-2.0"
 repository="https://github.com/EdgyEdgemond/app-confetti/"
 homepage="https://github.com/EdgyEdgemond/app-confetti/"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
-python-dotenv = "^0.15.0"
+python-dotenv = "^1.0.0"
 boto3 = { version = "^1.14.49", optional = true }
 ec2-metadata  = { version = "^2.2.0", optional = true }
 
 [tool.poetry.extras]
 aws = ["boto3", "ec2-metadata"]
 
 [tool.poetry.dev-dependencies]
@@ -76,22 +76,22 @@
     "D",
     "FBT",  # boolean trap? no documentation
     "S",  # bandit is run as a full commit hook
 ]
 
 [tool.ruff.per-file-ignores]
 "tasks.py" = ["ANN", "E501", "INP001"]
-"tests/*" = ["ANN", "D"]
+"tests/*" = ["ANN", "D", "RUF009"]
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.poetry.scripts]
 changelog-gen = "changelog_gen.cli.command:gen"
 changelog-init = "changelog_gen.cli.command:init"
 
 [build-system]
-requires = ["poetry-core>=1.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```


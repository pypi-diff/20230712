# Comparing `tmp/dbt_copilot_python-0.1.1.tar.gz` & `tmp/dbt_copilot_python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_copilot_python-0.1.1.tar", max compression
+gzip compressed data, was "dbt_copilot_python-0.1.2.tar", max compression
```

## Comparing `dbt_copilot_python-0.1.1.tar` & `dbt_copilot_python-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1090 2023-06-30 08:44:11.359787 dbt_copilot_python-0.1.1/LICENSE
--rw-r--r--   0        0        0     1309 2023-07-10 14:34:46.022458 dbt_copilot_python-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-03 11:33:07.684277 dbt_copilot_python-0.1.1/dbt_copilot_python/__init__.py
--rw-r--r--   0        0        0     1225 2023-07-11 11:36:47.245860 dbt_copilot_python-0.1.1/dbt_copilot_python/database.py
--rw-r--r--   0        0        0      692 2023-07-03 11:33:07.684778 dbt_copilot_python-0.1.1/dbt_copilot_python/network.py
--rw-r--r--   0        0        0      128 2023-07-03 11:33:07.684860 dbt_copilot_python-0.1.1/dbt_copilot_python/utility.py
--rw-r--r--   0        0        0      582 2023-07-11 11:37:29.616935 dbt_copilot_python-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1866 1970-01-01 00:00:00.000000 dbt_copilot_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-30 08:44:11.359787 dbt_copilot_python-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1927 2023-07-12 14:55:42.747641 dbt_copilot_python-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 11:33:07.684277 dbt_copilot_python-0.1.2/dbt_copilot_python/__init__.py
+-rw-r--r--   0        0        0     1225 2023-07-12 14:31:03.709428 dbt_copilot_python-0.1.2/dbt_copilot_python/database.py
+-rw-r--r--   0        0        0      692 2023-07-03 11:33:07.684778 dbt_copilot_python-0.1.2/dbt_copilot_python/network.py
+-rw-r--r--   0        0        0      128 2023-07-03 11:33:07.684860 dbt_copilot_python-0.1.2/dbt_copilot_python/utility.py
+-rw-r--r--   0        0        0      582 2023-07-12 14:52:43.164507 dbt_copilot_python-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 dbt_copilot_python-0.1.2/PKG-INFO
```

### Comparing `dbt_copilot_python-0.1.1/LICENSE` & `dbt_copilot_python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_copilot_python-0.1.1/README.md` & `dbt_copilot_python-0.1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -10,32 +10,54 @@
 
 ```
 pip install dbt-copilot-python
 ```
 
 ### Usage
 
-In `settings.py`:
+In `settings.py`...
 
-1. Add the ECS container IP to `ALLOWED_HOSTS` so that the Application Load Balancer (ALB) healthcheck will succeed:
+#### ALLOWED_HOSTS
+
+Add the ECS container IP to `ALLOWED_HOSTS` so that the Application Load Balancer (ALB) healthcheck will succeed:
+
+```
+from dbt_copilot_python.network import setup_allowed_hosts
+
+ALLOWED_HOSTS = [...]
+
+ALLOWED_HOSTS = setup_allowed_hosts(ALLOWED_HOSTS)
+```
+
+#### DATABASES
+
+To configure the `DATABASES` setting from an RDS JSON object stored in AWS Secrets Manager, there are two options.
+
+1. Configure the `DATABASES` setting to use a database URL (recommended):
+
+    Note: This is dependent on the [`dj-database-url`](https://pypi.org/project/dj-database-url/) package which can be installed via `pip install dj-database-url`.
 
     ```
-    from dbt_copilot_python.network import setup_allowed_hosts
-    
-    ALLOWED_HOSTS = [...]
-    
-    ALLOWED_HOSTS = setup_allowed_hosts(ALLOWED_HOSTS)
+    import dj_database_url
+
+    from dbt_copilot_python.database import database_url_from_env
+   
+    DATABASES = {
+        "default": dj_database_url.config(
+            default=database_url_from_env("DATABASE_ENV_VAR_KEY")
+        )
+    }
     ```
 
-2. Configure the `DATABASES` setting from an RDS JSON object stored in SSM Parameter Store:
+2. Configure the `DATABASES` setting to use a dictionary containing the settings:
 
     ```
-    from dbt-copilot-python import aws_database_config
-   
-    DATABASES = aws_database_config("ENVIRONMENT_KEY")
+    from dbt-copilot-python.database import database_from_env
+
+    DATABASES = database_from_env("DATABASE_ENV_VAR_KEY")
     ```
 
 ## Contributing to `dbt-copilot-python`
 
 ### Requirements
 
 - [Poetry](https://python-poetry.org/); `pip install poetry`
```

### Comparing `dbt_copilot_python-0.1.1/dbt_copilot_python/database.py` & `dbt_copilot_python-0.1.2/dbt_copilot_python/database.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_python-0.1.1/dbt_copilot_python/network.py` & `dbt_copilot_python-0.1.2/dbt_copilot_python/network.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_python-0.1.1/pyproject.toml` & `dbt_copilot_python-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-copilot-python"
-version = "0.1.1"
+version = "0.1.2"
 description = "Helper functions to run Django and Flask applications in AWS Copilot/ECS."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 readme = "README.md"
 packages = [{ include = "dbt_copilot_python" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dbt_copilot_python-0.1.1/PKG-INFO` & `dbt_copilot_python-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-copilot-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: Helper functions to run Django and Flask applications in AWS Copilot/ECS.
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -24,32 +24,54 @@
 
 ```
 pip install dbt-copilot-python
 ```
 
 ### Usage
 
-In `settings.py`:
+In `settings.py`...
 
-1. Add the ECS container IP to `ALLOWED_HOSTS` so that the Application Load Balancer (ALB) healthcheck will succeed:
+#### ALLOWED_HOSTS
+
+Add the ECS container IP to `ALLOWED_HOSTS` so that the Application Load Balancer (ALB) healthcheck will succeed:
+
+```
+from dbt_copilot_python.network import setup_allowed_hosts
+
+ALLOWED_HOSTS = [...]
+
+ALLOWED_HOSTS = setup_allowed_hosts(ALLOWED_HOSTS)
+```
+
+#### DATABASES
+
+To configure the `DATABASES` setting from an RDS JSON object stored in AWS Secrets Manager, there are two options.
+
+1. Configure the `DATABASES` setting to use a database URL (recommended):
+
+    Note: This is dependent on the [`dj-database-url`](https://pypi.org/project/dj-database-url/) package which can be installed via `pip install dj-database-url`.
 
     ```
-    from dbt_copilot_python.network import setup_allowed_hosts
-    
-    ALLOWED_HOSTS = [...]
-    
-    ALLOWED_HOSTS = setup_allowed_hosts(ALLOWED_HOSTS)
+    import dj_database_url
+
+    from dbt_copilot_python.database import database_url_from_env
+   
+    DATABASES = {
+        "default": dj_database_url.config(
+            default=database_url_from_env("DATABASE_ENV_VAR_KEY")
+        )
+    }
     ```
 
-2. Configure the `DATABASES` setting from an RDS JSON object stored in SSM Parameter Store:
+2. Configure the `DATABASES` setting to use a dictionary containing the settings:
 
     ```
-    from dbt-copilot-python import aws_database_config
-   
-    DATABASES = aws_database_config("ENVIRONMENT_KEY")
+    from dbt-copilot-python.database import database_from_env
+
+    DATABASES = database_from_env("DATABASE_ENV_VAR_KEY")
     ```
 
 ## Contributing to `dbt-copilot-python`
 
 ### Requirements
 
 - [Poetry](https://python-poetry.org/); `pip install poetry`
```


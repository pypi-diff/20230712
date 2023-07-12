# Comparing `tmp/astronomer_cosmos-0.7.4.tar.gz` & `tmp/astronomer_cosmos-0.7.5.tar.gz`

## Comparing `astronomer_cosmos-0.7.4.tar` & `astronomer_cosmos-0.7.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/__init__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/constants.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/dag.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/dataset.py
--rw-r--r--   0        0        0    11460 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/render.py
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/core/__init__.py
--rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/dbt/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/dbt/parser/__init__.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/dbt/parser/output.py
--rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/dbt/parser/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/hooks/__init__.py
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/hooks/subprocess.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/operators/__init__.py
--rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/operators/base.py
--rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/operators/docker.py
--rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/operators/kubernetes.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/operators/lazy_load.py
--rw-r--r--   0        0        0    19302 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/operators/local.py
--rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/operators/virtualenv.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/__init__.py
--rw-r--r--   0        0        0     5525 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/base.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/databricks/token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/spark/thrift.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/trino/base.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/cosmos/profiles/trino/ldap.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/LICENSE
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/README.rst
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/__init__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/constants.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/dag.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/dataset.py
+-rw-r--r--   0        0        0    11460 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/render.py
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/dbt/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/dbt/parser/__init__.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/dbt/parser/output.py
+-rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/dbt/parser/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/hooks/__init__.py
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/hooks/subprocess.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/__init__.py
+-rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/base.py
+-rw-r--r--   0        0        0     5057 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/docker.py
+-rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/kubernetes.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/lazy_load.py
+-rw-r--r--   0        0        0    19892 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/local.py
+-rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/operators/virtualenv.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/__init__.py
+-rw-r--r--   0        0        0     5525 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/base.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/databricks/token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/spark/thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/trino/base.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/cosmos/profiles/trino/ldap.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/LICENSE
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/README.rst
+-rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     7004 2020-02-02 00:00:00.000000 astronomer_cosmos-0.7.5/PKG-INFO
```

### Comparing `astronomer_cosmos-0.7.4/cosmos/__init__.py` & `astronomer_cosmos-0.7.5/cosmos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Astronomer Cosmos is a library for rendering dbt workflows in Airflow.
 
 Contains dags, task groups, and operators.
 """
 
-__version__ = "0.7.4"
+__version__ = "0.7.5"
 
 from cosmos.dataset import get_dbt_dataset
 
 # re-export the dag and task group
 from cosmos.dag import DbtDag
 from cosmos.task_group import DbtTaskGroup
```

### Comparing `astronomer_cosmos-0.7.4/cosmos/dag.py` & `astronomer_cosmos-0.7.5/cosmos/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/dataset.py` & `astronomer_cosmos-0.7.5/cosmos/dataset.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/render.py` & `astronomer_cosmos-0.7.5/cosmos/render.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/task_group.py` & `astronomer_cosmos-0.7.5/cosmos/task_group.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/core/airflow.py` & `astronomer_cosmos-0.7.5/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/core/graph/entities.py` & `astronomer_cosmos-0.7.5/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/dbt/parser/output.py` & `astronomer_cosmos-0.7.5/cosmos/dbt/parser/output.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/dbt/parser/project.py` & `astronomer_cosmos-0.7.5/cosmos/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/hooks/subprocess.py` & `astronomer_cosmos-0.7.5/cosmos/hooks/subprocess.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/operators/__init__.py` & `astronomer_cosmos-0.7.5/cosmos/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/operators/base.py` & `astronomer_cosmos-0.7.5/cosmos/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/operators/docker.py` & `astronomer_cosmos-0.7.5/cosmos/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/operators/kubernetes.py` & `astronomer_cosmos-0.7.5/cosmos/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/operators/local.py` & `astronomer_cosmos-0.7.5/cosmos/operators/local.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,36 +36,41 @@
 
     :param profile_args: Arguments to pass to the profile. See
         :py:class:`cosmos.providers.dbt.core.profiles.BaseProfileMapping`.
     :param profile_name: A name to use for the dbt profile. If not provided, and no profile target is found
         in your project's dbt_project.yml, "cosmos_profile" is used.
     :param install_deps: If true, install dependencies before running the command
     :param callback: A callback function called on after a dbt run with a path to the dbt project directory.
+    :param target_name: A name to use for the dbt target. If not provided, and no target is found
+        in your project's dbt_project.yml, "cosmos_target" is used.
+    :param should_store_compiled_sql: If true, store the compiled SQL in the compiled_sql rendered template.
     """
 
     template_fields: Sequence[str] = DbtBaseOperator.template_fields + ("compiled_sql",)
     template_fields_renderers = {
         "compiled_sql": "sql",
     }
 
     def __init__(
         self,
         install_deps: bool = False,
         callback: Optional[Callable[[str], None]] = None,
         profile_args: dict[str, str] = {},
         profile_name: str | None = None,
         target_name: str | None = None,
+        should_store_compiled_sql: bool = True,
         **kwargs,
     ) -> None:
         self.install_deps = install_deps
         self.profile_args = profile_args
         self.callback = callback
         self.profile_name = profile_name
         self.target_name = target_name
         self.compiled_sql = ""
+        self.should_store_compiled_sql = should_store_compiled_sql
         super().__init__(**kwargs)
 
     @cached_property
     def subprocess_hook(self):
         """Returns hook for running the bash command."""
         return FullOutputSubprocessHook()
 
@@ -80,24 +85,29 @@
 
     @provide_session
     def store_compiled_sql(self, tmp_project_dir: str, context: Context, session: Session = NEW_SESSION) -> None:
         """
         Takes the compiled SQL files from the dbt run and stores them in the compiled_sql rendered template.
         Gets called after every dbt run.
         """
+        if not self.should_store_compiled_sql:
+            return
+
         compiled_queries = {}
         # dbt compiles sql files and stores them in the target directory
-        for root, _, files in os.walk(os.path.join(tmp_project_dir, "target")):
-            for file in files:
-                if not file.endswith(".sql"):
+        for folder_path, _, file_paths in os.walk(os.path.join(tmp_project_dir, "target")):
+            for file_path in file_paths:
+                if not file_path.endswith(".sql"):
                     continue
 
-                compiled_sql_path = Path(os.path.join(root, file))
+                compiled_sql_path = Path(os.path.join(folder_path, file_path))
                 compiled_sql = compiled_sql_path.read_text(encoding="utf-8")
-                compiled_queries[file] = compiled_sql.strip()
+
+                relative_path = str(compiled_sql_path.relative_to(tmp_project_dir))
+                compiled_queries[relative_path] = compiled_sql.strip()
 
         for name, query in compiled_queries.items():
             self.compiled_sql += f"-- {name}\n{query}\n\n"
 
         self.compiled_sql = self.compiled_sql.strip()
 
         # need to refresh the rendered task field record in the db because Airflow only does this
```

### Comparing `astronomer_cosmos-0.7.4/cosmos/operators/virtualenv.py` & `astronomer_cosmos-0.7.5/cosmos/operators/virtualenv.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/profiles/__init__.py` & `astronomer_cosmos-0.7.5/cosmos/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/profiles/base.py` & `astronomer_cosmos-0.7.5/cosmos/profiles/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-0.7.5/cosmos/profiles/bigquery/service_account_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/profiles/databricks/token.py` & `astronomer_cosmos-0.7.5/cosmos/profiles/databricks/token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/profiles/exasol/user_pass.py` & `astronomer_cosmos-0.7.5/cosmos/profiles/exasol/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/profiles/postgres/user_pass.py` & `astronomer_cosmos-0.7.5/cosmos/profiles/postgres/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/profiles/redshift/user_pass.py` & `astronomer_cosmos-0.7.5/cosmos/profiles/redshift/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/profiles/snowflake/user_pass.py` & `astronomer_cosmos-0.7.5/cosmos/profiles/snowflake/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/profiles/spark/thrift.py` & `astronomer_cosmos-0.7.5/cosmos/profiles/spark/thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/profiles/trino/base.py` & `astronomer_cosmos-0.7.5/cosmos/profiles/trino/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/profiles/trino/certificate.py` & `astronomer_cosmos-0.7.5/cosmos/profiles/trino/certificate.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/profiles/trino/jwt.py` & `astronomer_cosmos-0.7.5/cosmos/profiles/trino/jwt.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/cosmos/profiles/trino/ldap.py` & `astronomer_cosmos-0.7.5/cosmos/profiles/trino/ldap.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/.gitignore` & `astronomer_cosmos-0.7.5/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/LICENSE` & `astronomer_cosmos-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/README.rst` & `astronomer_cosmos-0.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-0.7.4/PKG-INFO` & `astronomer_cosmos-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 0.7.4
+Version: 0.7.5
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Requires-Dist: apache-airflow>=2.3.0
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: jinja2>=3.0.0
+Requires-Dist: pydantic<2.0.0,>=1.10.0
 Requires-Dist: typing-extensions; python_version < '3.8'
 Requires-Dist: virtualenv
 Provides-Extra: all
 Requires-Dist: astronomer-cosmos[dbt-all]; extra == 'all'
 Provides-Extra: dbt-all
 Requires-Dist: astronomer-cosmos[dbt-openlineage]; extra == 'dbt-all'
 Requires-Dist: dbt-bigquery; extra == 'dbt-all'
```


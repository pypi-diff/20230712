# Comparing `tmp/tableau-helpers-2.0.5.dev4.tar.gz` & `tmp/tableau-helpers-2.0.5.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableau-helpers-2.0.5.dev4.tar", last modified: Tue Jun 27 17:52:14 2023, max compression
+gzip compressed data, was "tableau-helpers-2.0.5.dev5.tar", last modified: Wed Jul 12 14:17:11 2023, max compression
```

## Comparing `tableau-helpers-2.0.5.dev4.tar` & `tableau-helpers-2.0.5.dev5.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.509108 tableau-helpers-2.0.5.dev4/
--rw-rw-rw-   0        0        0      122 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev4/.env.sample
--rw-rw-rw-   0        0        0      376 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev4/.gitignore
--rw-rw-rw-   0        0        0     1088 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev4/LICENSE
--rw-rw-rw-   0        0        0     1914 2023-06-27 17:52:14.509108 tableau-helpers-2.0.5.dev4/PKG-INFO
--rw-rw-rw-   0        0        0     1617 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev4/README.md
--rw-rw-rw-   0        0        0     1237 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-27 17:52:14.509108 tableau-helpers-2.0.5.dev4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.248654 tableau-helpers-2.0.5.dev4/tableau_helpers/
--rw-rw-rw-   0        0        0      191 2023-06-27 17:51:43.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.342637 tableau-helpers-2.0.5.dev4/tableau_helpers/cli/
--rw-rw-rw-   0        0        0        0 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/cli/__init__.py
--rw-rw-rw-   0        0        0     2533 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/cli/csv_to_hyper.py
--rw-rw-rw-   0        0        0     1114 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/cli/upload_hyper.py
--rw-rw-rw-   0        0        0     7794 2023-06-27 17:51:06.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/hyper.py
--rw-rw-rw-   0        0        0     7998 2023-06-27 17:51:06.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/server.py
--rw-rw-rw-   0        0        0     1142 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tableau_helpers/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.310814 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/
--rw-rw-rw-   0        0        0     1914 2023-06-27 17:52:13.000000 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1013 2023-06-27 17:52:14.000000 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 17:52:13.000000 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-06-27 17:52:13.000000 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      183 2023-06-27 17:52:13.000000 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-27 17:52:13.000000 tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.373904 tableau-helpers-2.0.5.dev4/tests/
--rw-rw-rw-   0        0        0        0 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.405573 tableau-helpers-2.0.5.dev4/tests/cli/
--rw-rw-rw-   0        0        0        0 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/cli/__init__.py
--rw-rw-rw-   0        0        0      881 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/cli/test_csv_to_hyper.py
--rw-rw-rw-   0        0        0      696 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/cli/test_upload_hyper.py
--rw-rw-rw-   0        0        0     1838 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-06-27 17:52:14.488824 tableau-helpers-2.0.5.dev4/tests/resources/
--rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_default_format.csv
--rw-rw-rw-   0        0        0    65536 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_default_format.hyper
--rw-rw-rw-   0        0        0       34 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_default_format.tab
--rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_default_format2.csv
--rw-rw-rw-   0        0        0      378 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_default_format_table_def.json
--rw-rw-rw-   0        0        0      887 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_join_table_def.json
--rw-rw-rw-   0        0        0       52 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_left.csv
--rw-rw-rw-   0        0        0       56 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/resources/good_right.csv
--rw-rw-rw-   0        0        0    65536 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/resources/joined.hyper
--rw-rw-rw-   0        0        0     3902 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/test_hyper.py
--rw-rw-rw-   0        0        0     1128 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tests/test_server.py
--rw-rw-rw-   0        0        0      564 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev4/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-12 14:17:11.367029 tableau-helpers-2.0.5.dev5/
+-rw-rw-rw-   0        0        0      122 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev5/.env.sample
+-rw-rw-rw-   0        0        0      376 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev5/.gitignore
+-rw-rw-rw-   0        0        0     1088 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev5/LICENSE
+-rw-rw-rw-   0        0        0     1914 2023-07-12 14:17:11.367029 tableau-helpers-2.0.5.dev5/PKG-INFO
+-rw-rw-rw-   0        0        0     1617 2022-11-10 13:11:45.000000 tableau-helpers-2.0.5.dev5/README.md
+-rw-rw-rw-   0        0        0     1237 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 14:17:11.367029 tableau-helpers-2.0.5.dev5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 14:17:11.074722 tableau-helpers-2.0.5.dev5/tableau_helpers/
+-rw-rw-rw-   0        0        0      191 2023-07-05 18:52:03.000000 tableau-helpers-2.0.5.dev5/tableau_helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:17:11.174792 tableau-helpers-2.0.5.dev5/tableau_helpers/cli/
+-rw-rw-rw-   0        0        0        0 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev5/tableau_helpers/cli/__init__.py
+-rw-rw-rw-   0        0        0     3152 2023-07-12 14:12:59.000000 tableau-helpers-2.0.5.dev5/tableau_helpers/cli/csv_to_hyper.py
+-rw-rw-rw-   0        0        0      609 2023-07-12 14:12:59.000000 tableau-helpers-2.0.5.dev5/tableau_helpers/cli/logs.py
+-rw-rw-rw-   0        0        0     1686 2023-07-12 14:12:59.000000 tableau-helpers-2.0.5.dev5/tableau_helpers/cli/upload_hyper.py
+-rw-rw-rw-   0        0        0     8307 2023-07-12 13:16:21.000000 tableau-helpers-2.0.5.dev5/tableau_helpers/hyper.py
+-rw-rw-rw-   0        0        0     8052 2023-07-12 14:12:59.000000 tableau-helpers-2.0.5.dev5/tableau_helpers/server.py
+-rw-rw-rw-   0        0        0     1142 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev5/tableau_helpers/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:17:11.127905 tableau-helpers-2.0.5.dev5/tableau_helpers.egg-info/
+-rw-rw-rw-   0        0        0     1914 2023-07-12 14:17:10.000000 tableau-helpers-2.0.5.dev5/tableau_helpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1081 2023-07-12 14:17:10.000000 tableau-helpers-2.0.5.dev5/tableau_helpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 14:17:10.000000 tableau-helpers-2.0.5.dev5/tableau_helpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-07-12 14:17:10.000000 tableau-helpers-2.0.5.dev5/tableau_helpers.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      183 2023-07-12 14:17:10.000000 tableau-helpers-2.0.5.dev5/tableau_helpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-12 14:17:10.000000 tableau-helpers-2.0.5.dev5/tableau_helpers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 14:17:11.206268 tableau-helpers-2.0.5.dev5/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:17:11.237531 tableau-helpers-2.0.5.dev5/tests/cli/
+-rw-rw-rw-   0        0        0        0 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev5/tests/cli/__init__.py
+-rw-rw-rw-   0        0        0      881 2023-07-05 18:07:23.000000 tableau-helpers-2.0.5.dev5/tests/cli/test_csv_to_hyper.py
+-rw-rw-rw-   0        0        0      696 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev5/tests/cli/test_upload_hyper.py
+-rw-rw-rw-   0        0        0     2055 2023-07-05 16:59:14.000000 tableau-helpers-2.0.5.dev5/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:17:11.346904 tableau-helpers-2.0.5.dev5/tests/resources/
+-rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev5/tests/resources/good_default_format.csv
+-rw-rw-rw-   0        0        0    65536 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev5/tests/resources/good_default_format.hyper
+-rw-rw-rw-   0        0        0       34 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev5/tests/resources/good_default_format.tab
+-rw-rw-rw-   0        0        0       32 2022-11-10 13:11:46.000000 tableau-helpers-2.0.5.dev5/tests/resources/good_default_format2.csv
+-rw-rw-rw-   0        0        0      334 2023-07-05 18:42:13.000000 tableau-helpers-2.0.5.dev5/tests/resources/good_default_format_table_def.json
+-rw-rw-rw-   0        0        0      364 2023-07-05 17:20:54.000000 tableau-helpers-2.0.5.dev5/tests/resources/good_join_left_def.json
+-rw-rw-rw-   0        0        0      459 2023-07-05 17:20:43.000000 tableau-helpers-2.0.5.dev5/tests/resources/good_join_right_def.json
+-rw-rw-rw-   0        0        0       52 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev5/tests/resources/good_left.csv
+-rw-rw-rw-   0        0        0       56 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev5/tests/resources/good_right.csv
+-rw-rw-rw-   0        0        0    65536 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev5/tests/resources/joined.hyper
+-rw-rw-rw-   0        0        0     6019 2023-07-12 13:16:21.000000 tableau-helpers-2.0.5.dev5/tests/test_hyper.py
+-rw-rw-rw-   0        0        0     1128 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev5/tests/test_server.py
+-rw-rw-rw-   0        0        0      564 2023-06-27 13:37:39.000000 tableau-helpers-2.0.5.dev5/tox.ini
```

### Comparing `tableau-helpers-2.0.5.dev4/LICENSE` & `tableau-helpers-2.0.5.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev4/PKG-INFO` & `tableau-helpers-2.0.5.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau-helpers
-Version: 2.0.5.dev4
+Version: 2.0.5.dev5
 Summary: A collection of helpers to reduce boilerplate with Tableau APIs.
 License: MIT License
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `tableau-helpers-2.0.5.dev4/README.md` & `tableau-helpers-2.0.5.dev5/README.md`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev4/pyproject.toml` & `tableau-helpers-2.0.5.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev4/tableau_helpers/cli/upload_hyper.py` & `tableau-helpers-2.0.5.dev5/tableau_helpers/cli/upload_hyper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import argparse
+import logging
 from pathlib import Path
-import sys
 
 from tableau_helpers import server
+from tableau_helpers.cli import logs
+
+log = logging.getLogger(__name__)
 
 
 def _parse_args(args) -> argparse.Namespace:
     description = "Upload or overwrite a hyperfile on tableau-server"
     parser = argparse.ArgumentParser(description=description)
+    levels = ("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL")
+    parser.add_argument("--log-level", default="INFO", choices=levels)
+    parser.add_argument("--log-level-stdout", default=None, choices=levels)
+    parser.add_argument("--log-level-stderr", default="WARNING", choices=levels)
     parser.add_argument(
         "--hyperfile",
         type=Path,
         required=True,
         help="The path to the hyperfile to be uploaded.",
     )
     parser.add_argument(
@@ -27,18 +34,22 @@
         default=None,
         help="A name for the datasource (if desired different from hyperfile)",
     )
     return parser.parse_args(args)
 
 
 def main(args):
-    args = _parse_args(args)
-    server.create_or_replace_hyper_file(
-        project=args.dest, hyperfile_path=args.hyperfile, name=args.new_name
-    )
+    try:
+        args = _parse_args(args)
+        logs.config_logs(args.log_level, args.log_level_stdout, args.log_level_stderr)
+        server.create_or_replace_hyper_file(
+            project=args.dest, hyperfile_path=args.hyperfile, name=args.new_name
+        )
+    except Exception as e:
+        log.critical("Uncaught exception", exc_info=e)
 
 
 def entry_point():
     main(sys.argv[1:])
 
 
 if __name__ == "__main__":
```

### Comparing `tableau-helpers-2.0.5.dev4/tableau_helpers/hyper.py` & `tableau-helpers-2.0.5.dev5/tableau_helpers/hyper.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,43 @@
     TypeTag,
     escape_string_literal,
 )
 
 logger = logging.getLogger(__name__)
 
 
+def hyperprocess_env_kws() -> dict:
+    telemetry_enabled = os.getenv("TABLEAU_HYPERAPI_TELEMETRY", False)
+    telemetry = Telemetry.DO_NOT_SEND_USAGE_DATA_TO_TABLEAU
+    if telemetry_enabled:
+        telemetry = Telemetry.SEND_USAGE_DATA_TO_TABLEAU
+
+    user_agent = os.getenv("TABLEAU_HYPERAPI_USER_AGENT", "")
+    hyper_bin = os.getenv("TABLEAU_HYPERAPI_HYPER_BINARY", None)
+
+    parameters = {}
+    log_disable = os.getenv("TABLEAU_HYPERAPI_LOG_DISABLE", None)
+    if log_disable is not None:
+        parameters["log_config"] = ""  # empty string disables log
+    log_dir = os.getenv("TABLEAU_HYPERAPI_LOG_DIR", None)
+    if log_dir is not None:
+        parameters["log_dir"] = log_dir
+    log_file_max_count = os.getenv("TABLEAU_HYPERAPI_LOG_FILE_MAX_COUNT", "7")
+    parameters["log_file_max_count"] = log_file_max_count
+    log_file_size_limit = os.getenv("TABLEAU_HYPERAPI_LOG_FILE_SIZE_LIMIT", "100M")
+    parameters["log_file_size_limit"] = log_file_size_limit
+
+    return {
+        "telemetry": telemetry,
+        "user_agent": user_agent,
+        "hyper_path": hyper_bin,
+        "parameters": parameters,
+    }
+
+
 def _gen_sql_for_with_csv(
     delimiter: str = ",",
     null: str = "",
     encoding: str = "utf-8",
     on_cast_failure: str = "error",
     header: bool = False,
     quote: str = '"',
@@ -34,30 +63,30 @@
     sql_with: str = "WITH ("
     sql_with += "FORMAT csv"
     sql_with += f", NULL {escape_string_literal(null)}"
     sql_with += f", DELIMITER {escape_string_literal(delimiter)}"
     sql_with += f", ENCODING {escape_string_literal(encoding)}"
     sql_with += f", ON_CAST_FAILURE {escape_string_literal(on_cast_failure)}"
     if header:
-        sql_with += f", HEADER"
+        sql_with += ", HEADER"
     sql_with += f", QUOTE {escape_string_literal(quote)}"
     if escape is not None:
         sql_with += f", ESCAPE {escape_string_literal(escape)}"
     if force_not_null is not None:
         sql_with += f", FORCE_NOT_NULL ({','.join(force_not_null)})"
     if force_null is not None:
         sql_with += f", FORCE_NULL ({','.join(force_null)})"
     sql_with += ")"
     return sql_with
 
 
-def load_table_defs(table_conf_file: Path) -> list[TableDefinition]:
+def load_table_def(table_conf_file: Path) -> TableDefinition:
     with open(table_conf_file) as file:
-        table_confs = json.load(file)
-    return [parse_table_definition(table_conf) for table_conf in table_confs]
+        table_conf = json.load(file)
+    return parse_table_definition(table_conf)
 
 
 def parse_columns(columns: dict) -> Iterable[TableDefinition.Column]:
     for col in columns:
         name = col.get("name", None)
         if not name:
             raise ValueError("No name was provided for a column.")
@@ -94,24 +123,25 @@
         ]
     return table_def
 
 
 def copy_csv_to_hyper(
     save_path: Path,
     csv: Union[Path, list[Path]],
-    schema: Union[TableDefinition, list[TableDefinition]],
+    schema: TableDefinition,
     delimiter: str = ",",
     null: str = "",
     encoding: str = "utf-8",
     on_cast_failure: str = "error",
     header: bool = False,
     quote: str = '"',
     escape: Optional[str] = None,
     force_not_null: Optional[list[str]] = None,
     force_null: Optional[list[str]] = None,
+    create_mode: CreateMode = CreateMode.CREATE_AND_REPLACE,
 ) -> Optional[int]:
     """
     :param save_path: where to save the resulting hyperfile
     :param csv: the csv or list of csv paths to be imported
     :param schema: the TableDefinition for the destination hyperfile
     :param delimiter: the separator character for the input csv
     :param null: the string which represents a null in the csv
@@ -132,30 +162,29 @@
         values will be read as zero-length strings rather than
         nulls, even when they are not quoted.
     :param force_null: Match the specified columns' values
         against the null string, even if it has been quoted,
         and if a match is found set the value to NULL.
         In the default case where the null string is empty,
         this converts a quoted empty string into NULL.
+    :param hyper_process
     :return: the count of rows written to the hyper file,
         otherwise None
     """  # noqa
     sql_commands: list[str] = []
     alterations: list[str] = []
 
     if isinstance(csv, str):
         raise TypeError("str instead of Path object passed as csv")
     if isinstance(csv, Path):
         csv = [csv]
-    if isinstance(schema, TableDefinition):
-        schema = [schema]
-    for c, s in zip(csv, schema):
+    for c in csv:
         if not c.exists():
             raise FileNotFoundError(str(c))
-        sql_from = f"COPY {s.table_name} "
+        sql_from = f"COPY {schema.table_name} "
         sql_from += f"FROM {escape_string_literal(str(c))}"
 
         sql_with = _gen_sql_for_with_csv(
             delimiter=delimiter,
             null=null,
             encoding=encoding,
             on_cast_failure=on_cast_failure,
@@ -163,38 +192,29 @@
             quote=quote,
             escape=escape,
             force_not_null=force_not_null,
             force_null=force_null,
         )
         sql_commands.append(f"{sql_from} {sql_with}")
         try:
-            if s.th_alterations is not None:
-                [alterations.append(x) for x in s.th_alterations]
+            if schema.th_alterations is not None:
+                [alterations.append(x) for x in schema.th_alterations]
         except AttributeError:
             # alterations are optional
             pass
 
-    process_parameters = {}
-    log_file_max_count = os.getenv("TABLEAU_HYPERAPI_LOG_FILE_MAX_COUNT", "3")
-    process_parameters["log_file_max_count"] = log_file_max_count
-    log_file_size_limit = os.getenv("TABLEAU_HYPERAPI_LOG_FILE_SIZE_LIMIT", "100M")
-    process_parameters["log_file_size_limit"] = log_file_size_limit
-    log_dir = os.getenv("TABLEAU_HYPERAPI_LOG_DIR", None)
-    if log_dir is not None:
-        process_parameters["log_dir"] = log_dir
-
-    with HyperProcess(
-        telemetry=Telemetry.DO_NOT_SEND_USAGE_DATA_TO_TABLEAU,
-        parameters=process_parameters,
-    ) as hyper_process:
-        with Connection(
+    with (
+        HyperProcess(**hyperprocess_env_kws()) as hyper_process,
+        Connection(
             endpoint=hyper_process.endpoint,
             database=save_path,
-            create_mode=CreateMode.CREATE_AND_REPLACE,
-        ) as connection:
-            rowcount = 0
-            for s, command in zip(schema, sql_commands):
-                connection.catalog.create_table(table_definition=s)
-                rowcount += connection.execute_command(command)
-            for command in alterations:
-                connection.execute_command(command)
-            return rowcount
+            create_mode=create_mode,
+        ) as connection,
+    ):
+        rowcount = 0
+        for command in sql_commands:
+            connection.catalog.create_table_if_not_exists(table_definition=schema)
+            rowcount += connection.execute_command(command)
+        for command in alterations:
+            connection.execute_command(command)
+
+    return rowcount
```

### Comparing `tableau-helpers-2.0.5.dev4/tableau_helpers/server.py` & `tableau-helpers-2.0.5.dev5/tableau_helpers/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import logging
 import os
 from pathlib import Path
 from typing import Optional, Union
 
 import tableauserverclient as TSC
 
+log = logging.getLogger(__name__)
+
 
 class MultipleProjectsShareNameException(Exception):
     def __init__(self, name_shared, projects: Optional[list[TSC.ProjectItem]] = None):
         messages: list[str] = [
             f'Multiple projects share the name "{name_shared}",',
             "try providing a project name including parent projects separated by '/'",
             "or try referencing using the id of the project instead:",
@@ -74,15 +77,15 @@
             server.use_server_version()
         else:
             server.version = tableau_api_version
 
         auth = TSC.PersonalAccessTokenAuth(
             token_name=token_name,
             personal_access_token=personal_access_token,
-            site_id=os.getenv("TABLEAU_SITE", "")
+            site_id=os.getenv("TABLEAU_SITE", ""),
         )
         server.auth.sign_in_with_personal_access_token(auth)
         return server
 
     def get_project_id(
         self,
         project_name: str,
```

### Comparing `tableau-helpers-2.0.5.dev4/tableau_helpers/utils.py` & `tableau-helpers-2.0.5.dev5/tableau_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/PKG-INFO` & `tableau-helpers-2.0.5.dev5/tableau_helpers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau-helpers
-Version: 2.0.5.dev4
+Version: 2.0.5.dev5
 Summary: A collection of helpers to reduce boilerplate with Tableau APIs.
 License: MIT License
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `tableau-helpers-2.0.5.dev4/tableau_helpers.egg-info/SOURCES.txt` & `tableau-helpers-2.0.5.dev5/tableau_helpers.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,26 @@
 tableau_helpers.egg-info/SOURCES.txt
 tableau_helpers.egg-info/dependency_links.txt
 tableau_helpers.egg-info/entry_points.txt
 tableau_helpers.egg-info/requires.txt
 tableau_helpers.egg-info/top_level.txt
 tableau_helpers/cli/__init__.py
 tableau_helpers/cli/csv_to_hyper.py
+tableau_helpers/cli/logs.py
 tableau_helpers/cli/upload_hyper.py
 tests/__init__.py
 tests/conftest.py
 tests/test_hyper.py
 tests/test_server.py
 tests/cli/__init__.py
 tests/cli/test_csv_to_hyper.py
 tests/cli/test_upload_hyper.py
 tests/resources/good_default_format.csv
 tests/resources/good_default_format.hyper
 tests/resources/good_default_format.tab
 tests/resources/good_default_format2.csv
 tests/resources/good_default_format_table_def.json
-tests/resources/good_join_table_def.json
+tests/resources/good_join_left_def.json
+tests/resources/good_join_right_def.json
 tests/resources/good_left.csv
 tests/resources/good_right.csv
 tests/resources/joined.hyper
```

### Comparing `tableau-helpers-2.0.5.dev4/tests/cli/test_csv_to_hyper.py` & `tableau-helpers-2.0.5.dev5/tests/cli/test_csv_to_hyper.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev4/tests/cli/test_upload_hyper.py` & `tableau-helpers-2.0.5.dev5/tests/cli/test_upload_hyper.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev4/tests/conftest.py` & `tableau-helpers-2.0.5.dev5/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 def good_left_path():
     return os.path.abspath("tests/resources/good_left.csv")
 
 
 def good_right_path():
-    return os.path.abspath("tests/resources/good_left.csv")
+    return os.path.abspath("tests/resources/good_right.csv")
 
 
 def good_tab_path():
     return os.path.abspath("tests/resources/good_default_format.tab")
 
 
 def doesnt_exist_path():
@@ -60,13 +60,21 @@
     return os.path.abspath("tests/resources/good_default_format_table_def.json")
 
 
 def good_join_table_def_path():
     return os.path.abspath("tests/resources/good_join_table_def.json")
 
 
+def good_join_right_def_path():
+    return os.path.abspath("tests/resources/good_join_right_def.json")
+
+
+def good_join_left_def_path():
+    return os.path.abspath("tests/resources/good_join_left_def.json")
+
+
 def good_hyper_path():
     return os.path.abspath("tests/resources/good_default_format.hyper")
 
 
 def joined_hyper_path():
     return os.path.abspath("tests/resources/joined.hyper")
```

### Comparing `tableau-helpers-2.0.5.dev4/tests/resources/good_default_format.hyper` & `tableau-helpers-2.0.5.dev5/tests/resources/good_default_format.hyper`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev4/tests/resources/joined.hyper` & `tableau-helpers-2.0.5.dev5/tests/resources/joined.hyper`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev4/tests/test_server.py` & `tableau-helpers-2.0.5.dev5/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `tableau-helpers-2.0.5.dev4/tox.ini` & `tableau-helpers-2.0.5.dev5/tox.ini`

 * *Files identical despite different names*


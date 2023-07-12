# Comparing `tmp/target-duckdb-0.5.0.tar.gz` & `tmp/target-duckdb-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target-duckdb-0.5.0.tar", last modified: Wed May 17 17:27:47 2023, max compression
+gzip compressed data, was "target-duckdb-0.6.0.tar", last modified: Wed Jul 12 20:40:17 2023, max compression
```

## Comparing `target-duckdb-0.5.0.tar` & `target-duckdb-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-17 17:27:47.177855 target-duckdb-0.5.0/
--rw-r--r--   0 jwills     (501) staff       (20)    10409 2022-12-17 04:32:30.000000 target-duckdb-0.5.0/LICENSE
--rw-r--r--   0 jwills     (501) staff       (20)     5627 2023-05-17 17:27:47.177740 target-duckdb-0.5.0/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)     5240 2022-12-17 04:32:30.000000 target-duckdb-0.5.0/README.md
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-05-17 17:27:47.177891 target-duckdb-0.5.0/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)     1010 2023-05-17 17:27:43.000000 target-duckdb-0.5.0/setup.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-17 17:27:47.176787 target-duckdb-0.5.0/target_duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)    15202 2023-05-17 16:08:02.000000 target-duckdb-0.5.0/target_duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)    22568 2023-05-17 17:27:43.000000 target-duckdb-0.5.0/target_duckdb/db_sync.py
--rw-r--r--   0 jwills     (501) staff       (20)      685 2023-01-24 22:42:31.000000 target-duckdb-0.5.0/target_duckdb/logger.py
--rw-r--r--   0 jwills     (501) staff       (20)      370 2022-12-17 04:32:30.000000 target-duckdb-0.5.0/target_duckdb/logging.conf
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-17 17:27:47.177583 target-duckdb-0.5.0/target_duckdb.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)     5627 2023-05-17 17:27:47.000000 target-duckdb-0.5.0/target_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)      352 2023-05-17 17:27:47.000000 target-duckdb-0.5.0/target_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-05-17 17:27:47.000000 target-duckdb-0.5.0/target_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       53 2023-05-17 17:27:47.000000 target-duckdb-0.5.0/target_duckdb.egg-info/entry_points.txt
--rw-r--r--   0 jwills     (501) staff       (20)       65 2023-05-17 17:27:47.000000 target-duckdb-0.5.0/target_duckdb.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)       14 2023-05-17 17:27:47.000000 target-duckdb-0.5.0/target_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-07-12 20:40:17.973100 target-duckdb-0.6.0/
+-rw-r--r--   0 jwills     (501) staff       (20)    10409 2022-12-17 04:32:30.000000 target-duckdb-0.6.0/LICENSE
+-rw-r--r--   0 jwills     (501) staff       (20)     6313 2023-07-12 20:40:17.972989 target-duckdb-0.6.0/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)     5928 2023-07-12 14:08:00.000000 target-duckdb-0.6.0/README.md
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-07-12 20:40:17.973132 target-duckdb-0.6.0/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)     1008 2023-07-11 20:26:39.000000 target-duckdb-0.6.0/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-07-12 20:40:17.972137 target-duckdb-0.6.0/target_duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)    15373 2023-07-12 14:08:05.000000 target-duckdb-0.6.0/target_duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)    23362 2023-07-12 14:08:05.000000 target-duckdb-0.6.0/target_duckdb/db_sync.py
+-rw-r--r--   0 jwills     (501) staff       (20)      685 2023-01-24 22:42:31.000000 target-duckdb-0.6.0/target_duckdb/logger.py
+-rw-r--r--   0 jwills     (501) staff       (20)      370 2022-12-17 04:32:30.000000 target-duckdb-0.6.0/target_duckdb/logging.conf
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-07-12 20:40:17.972842 target-duckdb-0.6.0/target_duckdb.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)     6313 2023-07-12 20:40:17.000000 target-duckdb-0.6.0/target_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)      352 2023-07-12 20:40:17.000000 target-duckdb-0.6.0/target_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-07-12 20:40:17.000000 target-duckdb-0.6.0/target_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       53 2023-07-12 20:40:17.000000 target-duckdb-0.6.0/target_duckdb.egg-info/entry_points.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       65 2023-07-12 20:40:17.000000 target-duckdb-0.6.0/target_duckdb.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       14 2023-07-12 20:40:17.000000 target-duckdb-0.6.0/target_duckdb.egg-info/top_level.txt
```

### Comparing `target-duckdb-0.5.0/LICENSE` & `target-duckdb-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `target-duckdb-0.5.0/PKG-INFO` & `target-duckdb-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: target-duckdb
-Version: 0.5.0
-Summary: Singer.io target for loading data into DuckDB
-Home-page: https://github.com/jwills/target-duckdb
-Author: TransferWise
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 :: Only
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # target-duckdb
 
 [![License: Apache2](https://img.shields.io/badge/License-Apache2-yellow.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [Singer](https://www.singer.io/) target that loads data into DuckDB following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
 
 ### Install
@@ -41,24 +29,28 @@
 
 ### Configuration settings
 
 Running the target connector requires a `config.json` file. An example with the minimal settings:
 
 ```json
 {
-    "filepath": "/path/to/local/duckdb.file",
+    "path": "/path/to/local/file.duckdb",
     "default_target_schema": "main"
 }
 ```
 
 Additional options in `config.json`:
 
 | Property                            | Type    | Required?  | Description                                                   |
 |-------------------------------------|---------|------------|---------------------------------------------------------------|
-| filepath                            | String  | Yes        | The path to the DuckDB file that you want to write on the local filesystem. |	
+| path (alias: filepath)              | String  | Yes        | The path to use for the `duckdb.connect` call; either a local file or a MotherDuck connection uri. |
+| dbname (alias: database)            | String  |            | The database name to write to; this will be inferred from the path property if it is not specified. |
+| token                               | String  |            | For MotherDuck connections, the auth token to use (this may also be set directly via the MOTHERDUCK_TOKEN environment variable. |
+| delimiter                           | String  |            | (Default: ',') The delimiter to use for the CSV files that are used for record imports. |
+| quotechar                           | String  |            | (Default: '"') The quote character to use for the CSV files that are used for record imports. |
 | batch_size_rows                     | Integer |            | (Default: 100000) Maximum number of rows in each batch. At the end of each batch, the rows in the batch are loaded into DuckDB. |
 | flush_all_streams                   | Boolean |            | (Default: False) Flush and load every stream into DuckDB when one batch is full. Warning: This may trigger the COPY command to use files with low number of records. |
 | default_target_schema               | String  |            | Name of the schema where the tables will be created. If `schema_mapping` is not defined then every stream sent by the tap is loaded into this schema.    |
 | schema_mapping                      | Object  |            | Useful if you want to load multiple streams from one tap to multiple DuckDB schemas.<br><br>If the tap sends the `stream_id` in `<schema_name>-<table_name>` format then this option overwrites the `default_target_schema` value. |
 | add_metadata_columns                | Boolean |            | (Default: False) Metadata columns add extra row level information about data ingestions, (i.e. when was the row read in source, when was inserted or deleted in postgres etc.) Metadata columns are creating automatically by adding extra columns to the tables with a column prefix `_SDC_`. The column names are following the stitch naming conventions documented at https://www.stitchdata.com/docs/data-structure/integration-schemas#sdc-columns. Enabling metadata columns will flag the deleted rows by setting the `_SDC_DELETED_AT` metadata column. Without the `add_metadata_columns` option the deleted rows from singer taps will not be recognisable in DuckDB. |
 | hard_delete                         | Boolean |            | (Default: False) When `hard_delete` option is true then DELETE SQL commands will be performed in DuckDB to delete rows in tables. It's achieved by continuously checking the  `_SDC_DELETED_AT` metadata column sent by the singer tap. Due to deleting rows requires metadata columns, `hard_delete` option automatically enables the `add_metadata_columns` option as well. |
 | data_flattening_max_level           | Integer |            | (Default: 0) Object type RECORD items from taps can be transformed to flattened columns by creating columns automatically.<br><br>When value is 0 (default) then flattening functionality is turned off. |
```

### Comparing `target-duckdb-0.5.0/README.md` & `target-duckdb-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: target-duckdb
+Version: 0.6.0
+Summary: Singer.io target for loading data into DuckDB
+Home-page: https://github.com/jwills/target-duckdb
+Author: Josh Wills
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3 :: Only
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # target-duckdb
 
 [![License: Apache2](https://img.shields.io/badge/License-Apache2-yellow.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [Singer](https://www.singer.io/) target that loads data into DuckDB following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
 
 ### Install
@@ -29,24 +41,28 @@
 
 ### Configuration settings
 
 Running the target connector requires a `config.json` file. An example with the minimal settings:
 
 ```json
 {
-    "filepath": "/path/to/local/duckdb.file",
+    "path": "/path/to/local/file.duckdb",
     "default_target_schema": "main"
 }
 ```
 
 Additional options in `config.json`:
 
 | Property                            | Type    | Required?  | Description                                                   |
 |-------------------------------------|---------|------------|---------------------------------------------------------------|
-| filepath                            | String  | Yes        | The path to the DuckDB file that you want to write on the local filesystem. |	
+| path (alias: filepath)              | String  | Yes        | The path to use for the `duckdb.connect` call; either a local file or a MotherDuck connection uri. |
+| dbname (alias: database)            | String  |            | The database name to write to; this will be inferred from the path property if it is not specified. |
+| token                               | String  |            | For MotherDuck connections, the auth token to use (this may also be set directly via the MOTHERDUCK_TOKEN environment variable. |
+| delimiter                           | String  |            | (Default: ',') The delimiter to use for the CSV files that are used for record imports. |
+| quotechar                           | String  |            | (Default: '"') The quote character to use for the CSV files that are used for record imports. |
 | batch_size_rows                     | Integer |            | (Default: 100000) Maximum number of rows in each batch. At the end of each batch, the rows in the batch are loaded into DuckDB. |
 | flush_all_streams                   | Boolean |            | (Default: False) Flush and load every stream into DuckDB when one batch is full. Warning: This may trigger the COPY command to use files with low number of records. |
 | default_target_schema               | String  |            | Name of the schema where the tables will be created. If `schema_mapping` is not defined then every stream sent by the tap is loaded into this schema.    |
 | schema_mapping                      | Object  |            | Useful if you want to load multiple streams from one tap to multiple DuckDB schemas.<br><br>If the tap sends the `stream_id` in `<schema_name>-<table_name>` format then this option overwrites the `default_target_schema` value. |
 | add_metadata_columns                | Boolean |            | (Default: False) Metadata columns add extra row level information about data ingestions, (i.e. when was the row read in source, when was inserted or deleted in postgres etc.) Metadata columns are creating automatically by adding extra columns to the tables with a column prefix `_SDC_`. The column names are following the stitch naming conventions documented at https://www.stitchdata.com/docs/data-structure/integration-schemas#sdc-columns. Enabling metadata columns will flag the deleted rows by setting the `_SDC_DELETED_AT` metadata column. Without the `add_metadata_columns` option the deleted rows from singer taps will not be recognisable in DuckDB. |
 | hard_delete                         | Boolean |            | (Default: False) When `hard_delete` option is true then DELETE SQL commands will be performed in DuckDB to delete rows in tables. It's achieved by continuously checking the  `_SDC_DELETED_AT` metadata column sent by the singer tap. Due to deleting rows requires metadata columns, `hard_delete` option automatically enables the `add_metadata_columns` option as well. |
 | data_flattening_max_level           | Integer |            | (Default: 0) Object type RECORD items from taps can be transformed to flattened columns by creating columns automatically.<br><br>When value is 0 (default) then flattening functionality is turned off. |
```

### Comparing `target-duckdb-0.5.0/setup.py` & `target-duckdb-0.6.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="target-duckdb",
-    version="0.5.0",
+    version="0.6.0",
     description="Singer.io target for loading data into DuckDB",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author="TransferWise",
+    author="Josh Wills",
     url="https://github.com/jwills/target-duckdb",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3 :: Only",
     ],
     py_modules=["target_duckdb"],
     install_requires=[
         "jsonschema>=3.2.0",
-        "duckdb>=0.3.3",
+        "duckdb>=0.7.0",
     ],
     extras_require={
         "test": [
             "pytest",
             "pylint",
             "pytest-cov",
         ]
```

### Comparing `target-duckdb-0.5.0/target_duckdb/__init__.py` & `target-duckdb-0.6.0/target_duckdb/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #!/usr/bin/env python3
 
 import argparse
+import copy
 import io
 import json
-import os
 import sys
-import copy
+import tempfile
 from datetime import datetime
 from decimal import Decimal
-from tempfile import mkstemp
 
 import duckdb
 from jsonschema import Draft7Validator, FormatChecker
 
 from target_duckdb.db_sync import DbSync
 from target_duckdb.logger import get_logger
 
@@ -86,22 +85,18 @@
         sys.stdout.write("{}\n".format(line))
         sys.stdout.flush()
 
 
 # pylint: disable=missing-function-docstring,missing-class-docstring
 def validate_config(config):
     errors = []
-    required_config_keys = [
-        "filepath",
-    ]
-
-    # Check if mandatory keys exist
-    for k in required_config_keys:
-        if not config.get(k, None):
-            errors.append("Required key is missing from config: [{}]".format(k))
+
+    # Check that either 'path' or 'filepath' is defined in the config
+    if not config.get("path", config.get("filepath")):
+        errors.append("Either 'path' or 'filepath' must be defined in config.")
 
     # Check target schema config
     config_default_target_schema = config.get("default_target_schema", None)
     config_schema_mapping = config.get("schema_mapping", None)
     if not config_default_target_schema and not config_schema_mapping:
         errors.append(
             "Neither 'default_target_schema' (string) nor 'schema_mapping' (object) keys set in config."
@@ -115,16 +110,23 @@
     config_errors = validate_config(config)
 
     # Exit if config has errors
     if len(config_errors) > 0:
         LOGGER.error("Invalid configuration:\n   * %s", "\n   * ".join(config_errors))
         sys.exit(1)
 
-    # TODO(jwills): make this richer-- threads, pre-load extensions, etc.
-    return duckdb.connect(config["filepath"])
+    path = config.get("path", config.get("filepath"))
+    token = config.get("token", None)
+    if token:
+        path = f"{path}?token={token}"
+    db = duckdb.connect(path)
+    settings = config.get("settings", {})
+    for setting, value in settings.items():
+        db.execute(f"SET {setting} = '{value}'")
+    return db
 
 
 # pylint: disable=too-many-locals,too-many-branches,too-many-statements,invalid-name,consider-iterating-dictionary
 def persist_lines(connection, config, lines) -> None:
     """Read singer messages and process them line by line"""
     state = None
     flushed_state = None
@@ -348,15 +350,15 @@
     for stream in streams_to_flush:
         load_stream_batch(
             stream=stream,
             records_to_load=streams[stream],
             row_count=row_count,
             db_sync=stream_to_sync[stream],
             delete_rows=config.get("hard_delete"),
-            temp_dir=config.get("temp_dir"),
+            temp_dir=config.get("temp_dir", tempfile.gettempdir()),
         )
 
     # reset flushed stream records to empty to avoid flushing same records
     for stream in streams_to_flush:
         streams[stream] = {}
 
         # Update flushed streams
@@ -398,17 +400,17 @@
         db_sync.delete_rows(stream)
 
     # reset row count for the current stream
     row_count[stream] = 0
 
 
 # pylint: disable=unused-argument
-def flush_records(stream, records_to_load, row_count, db_sync, temp_dir=None):
+def flush_records(stream, records_to_load, row_count, db_sync, temp_dir):
     """Take a list of records and load into database"""
-    db_sync.load_rows(records_to_load.values(), row_count)
+    db_sync.load_rows(records_to_load.values(), row_count, temp_dir)
 
 
 def main():
     """Main entry point"""
     arg_parser = argparse.ArgumentParser()
     arg_parser.add_argument("-c", "--config", help="Config file")
     args = arg_parser.parse_args()
```

### Comparing `target-duckdb-0.5.0/target_duckdb/db_sync.py` & `target-duckdb-0.6.0/target_duckdb/db_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import collections.abc
+import csv
 import itertools
 import json
 import os
 import re
 import time
 import uuid
-
-import duckdb
+from urllib.parse import urlparse
 
 from target_duckdb.logger import get_logger
 
 
 # copied from inflection.camelize to eliminate a dependency
 def camelize(string: str, uppercase_first_letter: bool = True) -> str:
     if uppercase_first_letter:
@@ -187,14 +187,24 @@
     return {
         "catalog_name": catalog_name,
         "schema_name": schema_name,
         "table_name": table_name,
     }
 
 
+def get_catalog_name(connection_config):
+    raw_path = connection_config.get("path", connection_config.get("filepath"))
+    parsed = urlparse(raw_path)
+    base_file = os.path.basename(parsed.path)
+    path_db = os.path.splitext(base_file)[0]
+    if parsed.scheme in {"md", "motherduck"} and path_db == "":
+        path_db = "my_db"
+    return path_db
+
+
 # pylint: disable=too-many-public-methods,too-many-instance-attributes
 class DbSync:
     def __init__(self, connection, connection_config, stream_schema_message=None):
         """
         connection:  DuckDB connection
         connection_config: Connection config information
         stream_schema_message:  An instance of the DbSync class is typically used to load
@@ -216,22 +226,20 @@
         self.connection_config = connection_config
         self.stream_schema_message = stream_schema_message
 
         # logger to be used across the class's methods
         self.logger = get_logger("target_duckdb")
 
         # setup a catalog name
-        if duckdb.__version__ >= "0.7.0":
-            if self.connection_config.get("dbname"):
-                self.catalog_name = self.connection_config.get("dbname")
-            else:
-                filepath = self.connection_config.get("filepath")
-                self.catalog_name = os.path.splitext(os.path.basename(filepath))[0]
+        if self.connection_config.get("database"):
+            self.catalog_name = self.connection_config.get("database")
+        elif self.connection_config.get("dbname"):
+            self.catalog_name = self.connection_config.get("dbname")
         else:
-            self.catalog_name = None
+            self.catalog_name = get_catalog_name(self.connection_config)
         self.schema_name = None
 
         # Init stream schema
         if stream_schema_message is not None:
             # Define initial list of indices to created
             self.hard_delete = self.connection_config.get("hard_delete")
             if self.hard_delete:
@@ -286,14 +294,18 @@
                 "data_flattening_max_level", 0
             )
             self.flatten_schema = flatten_schema(
                 stream_schema_message["schema"],
                 max_level=self.data_flattening_max_level,
             )
 
+            # Delimiters/quotechars for CSV temp files
+            self.delimiter = self.connection_config.get("delimiter", ",")
+            self.quotechar = self.connection_config.get("quotechar", '"')
+
     def query(self, query, params=None):
         self.logger.debug("Running query: %s", query)
         cur = self.conn
         if params:
             cur.execute(query, params)
         else:
             cur.execute(query)
@@ -346,37 +358,43 @@
         return [
             flatten[name]
             if name in flatten and (flatten[name] == 0 or flatten[name])
             else None
             for name in self.flatten_schema
         ]
 
-    def load_rows(self, records, count):
+    def load_rows(self, records, count, temp_dir):
         stream_schema_message = self.stream_schema_message
         stream = stream_schema_message["stream"]
         self.logger.info(
             "Loading %d rows into '%s'", count, self.table_name(stream, False)
         )
 
         cur = self.conn
         temp_table = self.table_name(stream_schema_message["stream"], is_temporary=True)
+        temp_file_csv = os.path.join(temp_dir, f"{temp_table}.csv")
         cur.execute(self.create_table_query(table_name=temp_table, is_temporary=True))
 
-        insert_sql = "INSERT INTO {} ({}) VALUES ({})".format(
-            temp_table,
-            ", ".join(self.column_names()),
-            ", ".join(["?" for x in self.column_names()]),
-        )
-        self.logger.debug(insert_sql)
-        for record in records:
-            cur.execute(insert_sql, self.record_to_flattened(record))
+        # batch the records into a CSV file and do a copy operation
+        with open(temp_file_csv, "w") as f:
+            csvwriter = csv.writer(
+                f,
+                delimiter=self.delimiter,
+                quotechar=self.quotechar,
+                quoting=csv.QUOTE_MINIMAL,
+            )
+            for record in records:
+                csvwriter.writerow(self.record_to_flattened(record))
+        cur.execute("COPY {} FROM '{}'".format(temp_table, temp_file_csv))
 
         if len(self.stream_schema_message["key_properties"]) > 0:
             cur.execute(self.update_from_temp_table(temp_table))
         cur.execute(self.insert_from_temp_table(temp_table))
+        cur.execute(f"DROP TABLE {temp_table}")
+        os.unlink(temp_file_csv)
 
     # pylint: disable=duplicate-string-formatting-argument
     def insert_from_temp_table(self, temp_table):
         stream_schema_message = self.stream_schema_message
         columns = self.column_names()
         table = self.table_name(stream_schema_message["stream"])
 
@@ -400,21 +418,21 @@
 
     def update_from_temp_table(self, temp_table):
         stream_schema_message = self.stream_schema_message
         primary_key_columns = set(primary_column_names(self.stream_schema_message))
         columns = [x for x in self.column_names() if x not in primary_key_columns]
         table = self.table_name(stream_schema_message["stream"])
 
-        return """UPDATE {} SET {} FROM {} s
+        return """UPDATE {} as s SET {} FROM {} t
         WHERE {}
         """.format(
             table,
-            ", ".join(["{}=s.{}".format(c, c) for c in columns]),
+            ", ".join(["{}=t.{}".format(c, c) for c in columns]),
             temp_table,
-            self.primary_key_condition(table),
+            self.primary_key_condition("t"),
         )
 
     def primary_key_condition(self, right_table):
         stream_schema_message = self.stream_schema_message
         names = primary_column_names(stream_schema_message)
         return " AND ".join(["s.{} = {}.{}".format(c, right_table, c) for c in names])
 
@@ -446,16 +464,15 @@
             primary_key = []
 
         if not table_name:
             gen_table_name = self.table_name(
                 stream_schema_message["stream"], is_temporary=is_temporary
             )
 
-        return "CREATE {}TABLE IF NOT EXISTS {} ({})".format(
-            "TEMP " if is_temporary else "",
+        return "CREATE TABLE IF NOT EXISTS {} ({})".format(
             table_name if table_name else gen_table_name,
             ", ".join(columns + primary_key),
         )
 
     def create_index(self, stream, column):
         table = self.table_name(stream)
         table_without_schema = self.table_name(stream, without_schema=True)
```

### Comparing `target-duckdb-0.5.0/target_duckdb/logger.py` & `target-duckdb-0.6.0/target_duckdb/logger.py`

 * *Files identical despite different names*

### Comparing `target-duckdb-0.5.0/target_duckdb.egg-info/PKG-INFO` & `target-duckdb-0.6.0/target_duckdb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: target-duckdb
-Version: 0.5.0
+Version: 0.6.0
 Summary: Singer.io target for loading data into DuckDB
 Home-page: https://github.com/jwills/target-duckdb
-Author: TransferWise
+Author: Josh Wills
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # target-duckdb
@@ -41,24 +41,28 @@
 
 ### Configuration settings
 
 Running the target connector requires a `config.json` file. An example with the minimal settings:
 
 ```json
 {
-    "filepath": "/path/to/local/duckdb.file",
+    "path": "/path/to/local/file.duckdb",
     "default_target_schema": "main"
 }
 ```
 
 Additional options in `config.json`:
 
 | Property                            | Type    | Required?  | Description                                                   |
 |-------------------------------------|---------|------------|---------------------------------------------------------------|
-| filepath                            | String  | Yes        | The path to the DuckDB file that you want to write on the local filesystem. |	
+| path (alias: filepath)              | String  | Yes        | The path to use for the `duckdb.connect` call; either a local file or a MotherDuck connection uri. |
+| dbname (alias: database)            | String  |            | The database name to write to; this will be inferred from the path property if it is not specified. |
+| token                               | String  |            | For MotherDuck connections, the auth token to use (this may also be set directly via the MOTHERDUCK_TOKEN environment variable. |
+| delimiter                           | String  |            | (Default: ',') The delimiter to use for the CSV files that are used for record imports. |
+| quotechar                           | String  |            | (Default: '"') The quote character to use for the CSV files that are used for record imports. |
 | batch_size_rows                     | Integer |            | (Default: 100000) Maximum number of rows in each batch. At the end of each batch, the rows in the batch are loaded into DuckDB. |
 | flush_all_streams                   | Boolean |            | (Default: False) Flush and load every stream into DuckDB when one batch is full. Warning: This may trigger the COPY command to use files with low number of records. |
 | default_target_schema               | String  |            | Name of the schema where the tables will be created. If `schema_mapping` is not defined then every stream sent by the tap is loaded into this schema.    |
 | schema_mapping                      | Object  |            | Useful if you want to load multiple streams from one tap to multiple DuckDB schemas.<br><br>If the tap sends the `stream_id` in `<schema_name>-<table_name>` format then this option overwrites the `default_target_schema` value. |
 | add_metadata_columns                | Boolean |            | (Default: False) Metadata columns add extra row level information about data ingestions, (i.e. when was the row read in source, when was inserted or deleted in postgres etc.) Metadata columns are creating automatically by adding extra columns to the tables with a column prefix `_SDC_`. The column names are following the stitch naming conventions documented at https://www.stitchdata.com/docs/data-structure/integration-schemas#sdc-columns. Enabling metadata columns will flag the deleted rows by setting the `_SDC_DELETED_AT` metadata column. Without the `add_metadata_columns` option the deleted rows from singer taps will not be recognisable in DuckDB. |
 | hard_delete                         | Boolean |            | (Default: False) When `hard_delete` option is true then DELETE SQL commands will be performed in DuckDB to delete rows in tables. It's achieved by continuously checking the  `_SDC_DELETED_AT` metadata column sent by the singer tap. Due to deleting rows requires metadata columns, `hard_delete` option automatically enables the `add_metadata_columns` option as well. |
 | data_flattening_max_level           | Integer |            | (Default: 0) Object type RECORD items from taps can be transformed to flattened columns by creating columns automatically.<br><br>When value is 0 (default) then flattening functionality is turned off. |
```


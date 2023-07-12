# Comparing `tmp/recap-core-0.5.2.tar.gz` & `tmp/recap-core-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recap-core-0.5.2.tar", last modified: Mon Feb 27 18:13:12 2023, max compression
+gzip compressed data, was "recap-core-0.6.0.tar", last modified: Wed Jul 12 17:33:09 2023, max compression
```

## Comparing `recap-core-0.5.2.tar` & `recap-core-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0     1064 2022-12-27 00:12:51.238947 recap-core-0.5.2/LICENSE
--rw-r--r--   0        0        0     3143 2023-02-27 17:55:54.033672 recap-core-0.5.2/README.md
--rw-r--r--   0        0        0     1915 2023-02-27 18:12:13.607886 recap-core-0.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-12 19:37:02.802831 recap-core-0.5.2/recap/__init__.py
--rw-r--r--   0        0        0    14611 2023-02-27 17:55:54.044422 recap-core-0.5.2/recap/catalog.py
--rw-r--r--   0        0        0     4987 2023-02-27 17:55:54.045297 recap-core-0.5.2/recap/cli.py
--rw-r--r--   0        0        0      999 2023-02-27 17:55:54.046284 recap-core-0.5.2/recap/config.py
--rw-r--r--   0        0        0     3351 2023-02-27 17:55:54.047148 recap-core-0.5.2/recap/crawler.py
--rw-r--r--   0        0        0      226 2023-02-27 18:06:58.422507 recap-core-0.5.2/recap/integrations/__init__.py
--rw-r--r--   0        0        0     8626 2023-02-27 17:55:54.048402 recap-core-0.5.2/recap/integrations/bigquery.py
--rw-r--r--   0        0        0     2818 2023-02-27 17:55:54.048977 recap-core-0.5.2/recap/integrations/fsspec.py
--rw-r--r--   0        0        0     3024 2023-02-27 17:55:54.049592 recap-core-0.5.2/recap/integrations/sqlalchemy.py
--rw-r--r--   0        0        0     1637 2023-02-27 18:09:39.798963 recap-core-0.5.2/recap/logging.py
--rw-r--r--   0        0        0      965 2023-02-27 17:55:54.051096 recap-core-0.5.2/recap/metadata.py
--rw-r--r--   0        0        0     4778 2023-02-27 17:55:54.051607 recap-core-0.5.2/recap/registry.py
--rw-r--r--   0        0        0     4676 2023-02-27 17:55:54.051989 recap-core-0.5.2/recap/repl.py
--rw-r--r--   0        0        0     2150 2023-02-27 17:55:54.052469 recap-core-0.5.2/recap/server.py
--rw-r--r--   0        0        0      548 2023-02-27 17:55:54.052956 recap-core-0.5.2/recap/storage/__init__.py
--rw-r--r--   0        0        0     2789 2023-02-27 17:55:54.053411 recap-core-0.5.2/recap/storage/abstract.py
--rw-r--r--   0        0        0     7807 2023-02-27 17:55:54.053828 recap-core-0.5.2/recap/storage/db.py
--rw-r--r--   0        0        0     3491 2023-02-27 17:55:54.054232 recap-core-0.5.2/recap/storage/remote.py
--rw-r--r--   0        0        0     3185 2023-02-27 17:55:54.054837 recap-core-0.5.2/tests/storage/test_db.py
--rw-r--r--   0        0        0     3683 1970-01-01 00:00:00.000000 recap-core-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-27 15:48:10.562535 recap-core-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2342 2023-07-12 17:33:01.552447 recap-core-0.6.0/README.md
+-rw-r--r--   0        0        0     1689 2023-07-12 17:31:37.807135 recap-core-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 18:01:48.247590 recap-core-0.6.0/recap/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 17:59:03.920427 recap-core-0.6.0/recap/converters/__init__.py
+-rw-r--r--   0        0        0    16690 2023-07-10 19:39:47.783465 recap-core-0.6.0/recap/converters/avro.py
+-rw-r--r--   0        0        0     2739 2023-07-03 15:46:50.002671 recap-core-0.6.0/recap/converters/json_schema.py
+-rw-r--r--   0        0        0    10037 2023-07-12 02:14:49.971563 recap-core-0.6.0/recap/converters/protobuf.py
+-rw-r--r--   0        0        0        0 2023-06-01 17:59:03.922807 recap-core-0.6.0/recap/readers/__init__.py
+-rw-r--r--   0        0        0     1208 2023-07-03 15:46:50.003079 recap-core-0.6.0/recap/readers/confluent_registry.py
+-rw-r--r--   0        0        0     3038 2023-07-03 15:46:50.003258 recap-core-0.6.0/recap/readers/dbapi.py
+-rw-r--r--   0        0        0    11579 2023-07-12 17:31:28.689536 recap-core-0.6.0/recap/readers/hive_metastore.py
+-rw-r--r--   0        0        0     2586 2023-06-29 17:21:46.545044 recap-core-0.6.0/recap/readers/postgresql.py
+-rw-r--r--   0        0        0     2968 2023-06-29 16:46:51.946949 recap-core-0.6.0/recap/readers/snowflake.py
+-rw-r--r--   0        0        0    22251 2023-07-12 17:15:08.209961 recap-core-0.6.0/recap/types.py
+-rw-r--r--   0        0        0     3587 2023-07-03 15:46:50.003654 recap-core-0.6.0/tests/integration/readers/test_confluent_registry.py
+-rw-r--r--   0        0        0    13742 2023-07-03 15:46:50.003860 recap-core-0.6.0/tests/integration/readers/test_hive_metastore.py
+-rw-r--r--   0        0        0     5163 2023-07-03 15:46:50.004149 recap-core-0.6.0/tests/integration/readers/test_postgresql.py
+-rw-r--r--   0        0        0    24290 2023-07-10 19:45:25.750661 recap-core-0.6.0/tests/unit/converters/test_avro.py
+-rw-r--r--   0        0        0     7435 2023-07-03 15:46:50.004540 recap-core-0.6.0/tests/unit/converters/test_json_schema.py
+-rw-r--r--   0        0        0    20941 2023-07-12 02:14:49.971854 recap-core-0.6.0/tests/unit/converters/test_protobuf.py
+-rw-r--r--   0        0        0     3913 2023-07-03 15:46:50.004960 recap-core-0.6.0/tests/unit/readers/test_confluent_registry.py
+-rw-r--r--   0        0        0    17010 2023-07-10 22:27:09.612147 recap-core-0.6.0/tests/unit/readers/test_hive_metastore.py
+-rw-r--r--   0        0        0    11056 2023-07-03 15:46:50.005364 recap-core-0.6.0/tests/unit/readers/test_snowflake.py
+-rw-r--r--   0        0        0    32574 2023-07-12 17:15:08.210414 recap-core-0.6.0/tests/unit/test_types.py
+-rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 recap-core-0.6.0/PKG-INFO
```

### Comparing `recap-core-0.5.2/LICENSE` & `recap-core-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recap-core-0.5.2/pyproject.toml` & `recap-core-0.6.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,86 @@
 [project]
 name = "recap-core"
-version = "0.5.2"
-description = "A metadata toolkit written in Python"
+version = "0.6.0"
+description = "Read schemas from web service, databases, and schema registries in a standard format"
 authors = [
     { name = "Chris Riccomini", email = "criccomini@apache.org" },
 ]
-dependencies = [
-    "fastapi>=0.88.0",
-    "uvicorn[standard]>=0.20.0",
-    "httpx>=0.23.1",
-    "typer>=0.7.0",
-    "sqlalchemy>=1.4.45",
-    "rich>=12.6.0",
-    "setuptools>=65.6.3",
-    "starlette>=0.22.0",
-    "pydantic[dotenv]>=1.10.5",
-    "pandas>=1.5.3",
-    "fsspec>=2023.1.0",
-    "frictionless[json,parquet]>=5.6.3",
-    "tomli>=2.0.1",
-]
-requires-python = ">=3.10, <3.11"
+dependencies = []
+requires-python = ">=3.10, <=3.11"
 readme = "README.md"
 keywords = [
-    "metadata",
+    "avro",
     "data",
     "data catalog",
+    "data discovery",
     "data engineering",
+    "data governance",
     "data infrastructure",
-    "infrastructure",
-    "devtools",
+    "data integration",
+    "data pipelines",
+    "data quality",
     "devops",
+    "devtools",
+    "etl",
+    "infrastructure",
+    "json schema",
+    "metadata",
+    "protobuf",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
-documentation = "https://docs.recap.cloud"
-homepage = "https://github.com/recap-cloud/recap"
+documentation = "https://recap.build"
+homepage = "https://recap.build"
 repository = "https://github.com/recap-cloud/recap"
 
-[project.scripts]
-recap = "recap.cli:app"
-
 [project.optional-dependencies]
-gcp = [
-    "gcsfs>=2023.1.0",
-    "sqlalchemy-bigquery>=1.5.0",
+kafka = [
+    "confluent-kafka[schema-registry]>=2.1.1",
+]
+proto = [
+    "proto-schema-parser>=0.2.0",
+]
+hive = [
+    "pymetastore>=0.2.0",
 ]
 
 [build-system]
 requires = [
     "pdm-pep517>=1.0.0",
 ]
 build-backend = "pdm.pep517.api"
 
 [tool.pdm.dev-dependencies]
-docs = [
-    "mkdocs-material>=8.5.11",
-    "mkdocs-git-revision-date-plugin>=0.3.2",
-    "mike>=1.1.2",
-    "mkdocstrings[python]>=0.20.0",
-    "mkdocs-typer>=0.0.2",
-]
-dbs = [
-    "psycopg2>=2.9.5",
-    "snowflake-sqlalchemy>=1.4.4",
-    "sqlalchemy-bigquery>=1.5.0",
-    "google-cloud-bigquery>=3.6.0",
-]
-fss = [
-    "s3fs>=2023.1.0",
-    "gcsfs>=2023.1.0",
-]
 tests = [
     "pytest>=7.2.1",
+    "snowflake-connector-python>=3.0.4",
+    "fakesnow>=0.1.0",
+    "psycopg2-binary>=2.9.6",
 ]
 style = [
     "black>=23.1.0",
     "isort>=5.12.0",
     "pylint>=2.16.1",
     "pyright>=1.1.293",
 ]
 
+[tool.pdm.scripts]
+black = "black recap/ tests/"
+isort = "isort recap/ tests/"
+
+[tool.pdm.scripts.style]
+composite = [
+    "black",
+    "isort",
+]
+
 [tool.isort]
 profile = "black"
 case_sensitive = true
 
 [tool.pylint.messages_control]
 max-line-length = 110
```


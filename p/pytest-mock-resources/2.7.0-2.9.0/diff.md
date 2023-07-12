# Comparing `tmp/pytest_mock_resources-2.7.0.tar.gz` & `tmp/pytest_mock_resources-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_mock_resources-2.7.0.tar", max compression
+gzip compressed data, was "pytest_mock_resources-2.9.0.tar", max compression
```

## Comparing `pytest_mock_resources-2.7.0.tar` & `pytest_mock_resources-2.9.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    15317 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1053 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/LICENSE
--rw-r--r--   0        0        0     5549 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/README.md
--rw-r--r--   0        0        0     3597 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     1846 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/__init__.py
--rw-r--r--   0        0        0     1305 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/action.py
--rw-r--r--   0        0        0     2173 2023-06-09 13:02:20.155211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/cli.py
--rw-r--r--   0        0        0     1867 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/compat/__init__.py
--rw-r--r--   0        0        0      822 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/compat/import_.py
--rw-r--r--   0        0        0      923 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/compat/sqlalchemy.py
--rw-r--r--   0        0        0     3013 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/config.py
--rw-r--r--   0        0        0      622 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/__init__.py
--rw-r--r--   0        0        0     6429 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/base.py
--rw-r--r--   0        0        0     1702 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/mongo.py
--rw-r--r--   0        0        0     1399 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/moto.py
--rw-r--r--   0        0        0     2792 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/mysql.py
--rw-r--r--   0        0        0     3713 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/postgres.py
--rw-r--r--   0        0        0     1369 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/redis.py
--rw-r--r--   0        0        0     1569 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/redshift.py
--rw-r--r--   0        0        0     3070 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/credentials.py
--rw-r--r--   0        0        0     1490 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/__init__.py
--rw-r--r--   0        0        0      750 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/base.py
--rw-r--r--   0        0        0     2364 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/mongo.py
--rw-r--r--   0        0        0      406 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/moto/__init__.py
--rw-r--r--   0        0        0     1960 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/moto/action.py
--rw-r--r--   0        0        0     4438 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/moto/base.py
--rw-r--r--   0        0        0     3417 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/mysql.py
--rw-r--r--   0        0        0    11154 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/postgresql.py
--rw-r--r--   0        0        0     2714 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/redis.py
--rw-r--r--   0        0        0     4658 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/redshift/__init__.py
--rw-r--r--   0        0        0     4939 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/redshift/udf.py
--rw-r--r--   0        0        0     9051 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/sqlite.py
--rw-r--r--   0        0        0     3813 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/hooks.py
--rw-r--r--   0        0        0        0 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/__init__.py
--rw-r--r--   0        0        0     7054 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/mock_s3_copy.py
--rw-r--r--   0        0        0     7286 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/mock_s3_unload.py
--rw-r--r--   0        0        0     2486 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/psycopg2.py
--rw-r--r--   0        0        0     2905 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/py.typed
--rw-r--r--   0        0        0    10187 2023-06-09 13:02:20.159211 pytest_mock_resources-2.7.0/src/pytest_mock_resources/sqlalchemy.py
--rw-r--r--   0        0        0     7906 1970-01-01 00:00:00.000000 pytest_mock_resources-2.7.0/setup.py
--rw-r--r--   0        0        0     7788 1970-01-01 00:00:00.000000 pytest_mock_resources-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0    15315 2023-07-12 20:13:38.614969 pytest_mock_resources-2.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1053 2023-07-12 20:13:38.614969 pytest_mock_resources-2.9.0/LICENSE
+-rw-r--r--   0        0        0     5549 2023-07-12 20:13:38.614969 pytest_mock_resources-2.9.0/README.md
+-rw-r--r--   0        0        0     3848 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1792 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/__init__.py
+-rw-r--r--   0        0        0     1305 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/action.py
+-rw-r--r--   0        0        0     2174 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/cli.py
+-rw-r--r--   0        0        0     1867 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/compat/__init__.py
+-rw-r--r--   0        0        0      822 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/compat/import_.py
+-rw-r--r--   0        0        0      923 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/compat/sqlalchemy.py
+-rw-r--r--   0        0        0     3013 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/config.py
+-rw-r--r--   0        0        0      622 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/__init__.py
+-rw-r--r--   0        0        0     6429 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/base.py
+-rw-r--r--   0        0        0     1702 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/mongo.py
+-rw-r--r--   0        0        0     1399 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/moto.py
+-rw-r--r--   0        0        0     2792 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/mysql.py
+-rw-r--r--   0        0        0     3713 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/postgres.py
+-rw-r--r--   0        0        0     1369 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/redis.py
+-rw-r--r--   0        0        0     1569 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/redshift.py
+-rw-r--r--   0        0        0     3070 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/credentials.py
+-rw-r--r--   0        0        0     1436 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/__init__.py
+-rw-r--r--   0        0        0      951 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/base.py
+-rw-r--r--   0        0        0     2364 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/mongo.py
+-rw-r--r--   0        0        0      416 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/moto/__init__.py
+-rw-r--r--   0        0        0     1960 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/moto/action.py
+-rw-r--r--   0        0        0     5013 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/moto/base.py
+-rw-r--r--   0        0        0     3417 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/mysql.py
+-rw-r--r--   0        0        0    11153 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/postgresql.py
+-rw-r--r--   0        0        0     2713 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/redis.py
+-rw-r--r--   0        0        0     4659 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/redshift/__init__.py
+-rw-r--r--   0        0        0     4939 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/redshift/udf.py
+-rw-r--r--   0        0        0     9051 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/sqlite.py
+-rw-r--r--   0        0        0     3813 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/hooks.py
+-rw-r--r--   0        0        0        0 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/__init__.py
+-rw-r--r--   0        0        0     7056 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/mock_s3_copy.py
+-rw-r--r--   0        0        0     7290 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/mock_s3_unload.py
+-rw-r--r--   0        0        0     2486 2023-07-12 20:13:38.618969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/psycopg2.py
+-rw-r--r--   0        0        0     2905 2023-07-12 20:13:38.622969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-07-12 20:13:38.622969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/py.typed
+-rw-r--r--   0        0        0    10215 2023-07-12 20:13:38.622969 pytest_mock_resources-2.9.0/src/pytest_mock_resources/sqlalchemy.py
+-rw-r--r--   0        0        0     7928 1970-01-01 00:00:00.000000 pytest_mock_resources-2.9.0/setup.py
+-rw-r--r--   0        0        0     7821 1970-01-01 00:00:00.000000 pytest_mock_resources-2.9.0/PKG-INFO
```

### Comparing `pytest_mock_resources-2.7.0/CHANGELOG.md` & `pytest_mock_resources-2.9.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Changelog
 
-## [Unreleased](https://github.com/schireson/pytest-mock-resources/compare/v2.6.13...HEAD) (2023-05-31)
+## [v2.7.0](https://github.com/schireson/pytest-mock-resources/compare/v2.6.13...v2.7.0) (2023-06-06)
 
 ### Features
 
 * Implement moto "ordered actions" for declaring a specific bucket state.
-  ([e7efece](https://github.com/schireson/pytest-mock-resources/commit/e7efece534178a70d1f1b4bcd11985a88003b92a))
+  ([5d6665e](https://github.com/schireson/pytest-mock-resources/commit/5d6665e340a48c7f3ce7cda4a09793986fd4c318))
 
 ### [v2.6.13](https://github.com/schireson/pytest-mock-resources/compare/v2.6.12...v2.6.13) (2023-05-23)
 
 #### Fixes
 
 * Increase time to wait for mysql to spin up. (#190)
   ([5d94aea](https://github.com/schireson/pytest-mock-resources/commit/5d94aeaf93576d2009f0da3568e0a84e0183f7bc))
```

### Comparing `pytest_mock_resources-2.7.0/LICENSE` & `pytest_mock_resources-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/README.md` & `pytest_mock_resources-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/pyproject.toml` & `pytest_mock_resources-2.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-mock-resources"
-version = "2.7.0"
+version = "2.9.0"
 description = "A pytest plugin for easily instantiating reproducible mock resources."
 authors = [
     "Omar Khan <oakhan3@gmail.com>",
     "Dan Cardin <ddcardin@gmail.com>",
     "Gabriel Michael <gabriel.j.michael@gmail.com>",
     "Prateek Pisat <pisatprateek12@gmail.com>",
 ]
@@ -23,14 +23,16 @@
 
 [tool.poetry.dependencies]
 python = ">=3.7, <4"
 
 pytest = {version = ">=1.0"}
 sqlalchemy = {version = ">1.0, !=1.4.0, !=1.4.1, !=1.4.2, !=1.4.3, !=1.4.4, !=1.4.5, !=1.4.6, !=1.4.7, !=1.4.8, !=1.4.9, !=1.4.10, !=1.4.11, !=1.4.12, !=1.4.13, !=1.4.14, !=1.4.15, !=1.4.16, !=1.4.17, !=1.4.18, !=1.4.19, !=1.4.20, !=1.4.21, !=1.4.22, !=1.4.23"}
 
+typing_extensions = "*"
+
 # extra [postgres]
 psycopg2 = {version = "*", optional = true}
 psycopg2-binary = {version = "*", optional = true}
 asyncpg = {version = "*", optional = true}
 
 # extra [redshift]
 moto = {version = "*", optional = true}
@@ -48,29 +50,32 @@
 
 # extra [docker]
 filelock = {version = "*", optional = true}
 python-on-whales = {version = ">=0.22.0", optional = true}
 
 [tool.poetry.dev-dependencies]
 black = "22.3.0"
+botocore = ">=1.10.84"
 coverage = "*"
 flake8 = "*"
 isort = ">=5.0"
+moto = ">=2.3.2"
 mypy = {version = "0.982"}
 pydocstyle = {version = "*"}
-sqlalchemy-stubs = {version = "*"}
-pytest-xdist = "*"
 pytest-asyncio = "*"
-types-six = "^1.16.0"
-types-PyMySQL = "^1.0.2"
-types-redis = "^3.5.6"
+pytest-xdist = "*"
+responses = ">=0.23.0"
+sqlalchemy-stubs = {version = "*"}
 sqlalchemy2-stubs = "^0.0.2-alpha.19"
-types-filelock = "^3.2.7"
+types-PyMySQL = "^1.0.2"
 types-dataclasses = "^0.6.5"
+types-filelock = "^3.2.7"
+types-redis = "^3.5.6"
 types-requests = "*"
+types-six = "^1.16.0"
 
 [tool.poetry.extras]
 docker = ['python-on-whales', 'filelock']
 postgres = ['psycopg2', 'python-on-whales', 'filelock']
 postgres-binary = ['psycopg2-binary', 'python-on-whales', 'filelock']
 postgres-async = ['asyncpg', 'python-on-whales', 'filelock']
 redshift = ['boto3', 'moto', 'sqlparse', 'python-on-whales', 'filelock']
@@ -116,12 +121,14 @@
     "mongo",
     "redis",
     "mysql",
 ]
 filterwarnings = [
   "error",
   "ignore:There is no current event loop:DeprecationWarning",
+  "ignore:stream argument is deprecated. Use stream parameter in request directly:DeprecationWarning",
+  "ignore:Boto3 will no longer support Python 3.7.*::boto3"
 ]
 
 [build-system]
 requires = ["poetry_core==1.0.8"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/__init__.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     create_redis_fixture,
     create_redshift_fixture,
     create_sqlite_fixture,
     pmr_mongo_config,
     pmr_mongo_container,
     pmr_moto_config,
     pmr_moto_container,
-    pmr_moto_credentials,
     pmr_mysql_config,
     pmr_mysql_container,
     pmr_postgres_config,
     pmr_postgres_container,
     pmr_redis_config,
     pmr_redis_container,
     pmr_redshift_config,
@@ -61,15 +60,14 @@
     "create_redshift_fixture",
     "create_sqlite_fixture",
     "get_container",
     "pmr_mongo_config",
     "pmr_mongo_container",
     "pmr_moto_config",
     "pmr_moto_container",
-    "pmr_moto_credentials",
     "pmr_mysql_config",
     "pmr_mysql_container",
     "pmr_postgres_config",
     "pmr_postgres_container",
     "pmr_redis_config",
     "pmr_redis_container",
     "pmr_redshift_config",
```

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/action.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/action.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/cli.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             )
 
         execute(fixture, pytestconfig, start=start, stop=stop)
 
 
 def create_parser():
     parser = argparse.ArgumentParser(
-        description="Premptively run docker containers to speed up initial startup of PMR Fixtures."
+        description="Preemptively run docker containers to speed up initial startup of PMR Fixtures."
     )
     parser.add_argument(
         "fixtures",
         metavar="Fixture",
         type=str,
         nargs="+",
         help="Available Fixtures: {}".format(", ".join(DockerContainerConfig.subclasses)),
```

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/compat/__init__.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/compat/import_.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/compat/import_.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/compat/sqlalchemy.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/compat/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/config.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/config.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/__init__.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/base.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/base.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/mongo.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/mongo.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/moto.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/moto.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/mysql.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/postgres.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/postgres.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/redis.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/redis.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/container/redshift.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/container/redshift.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/credentials.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/credentials.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/__init__.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
     pmr_mongo_config,
     pmr_mongo_container,
 )
 from pytest_mock_resources.fixture.moto import (
     create_moto_fixture,
     pmr_moto_config,
     pmr_moto_container,
-    pmr_moto_credentials,
     S3Bucket,
     S3Object,
 )
 from pytest_mock_resources.fixture.mysql import (
     create_mysql_fixture,
     pmr_mysql_config,
     pmr_mysql_container,
@@ -43,15 +42,14 @@
     "create_redis_fixture",
     "create_redshift_fixture",
     "create_sqlite_fixture",
     "pmr_mongo_config",
     "pmr_mongo_container",
     "pmr_moto_config",
     "pmr_moto_container",
-    "pmr_moto_credentials",
     "pmr_mysql_config",
     "pmr_mysql_container",
     "pmr_postgres_config",
     "pmr_postgres_container",
     "pmr_redis_config",
     "pmr_redis_container",
     "pmr_redshift_config",
```

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/mongo.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/mongo.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/moto/action.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/moto/action.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/moto/base.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/moto/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import pytest
 
 from pytest_mock_resources.action import validate_actions
 from pytest_mock_resources.compat import boto3
 from pytest_mock_resources.container.base import get_container
 from pytest_mock_resources.container.moto import endpoint_url, MotoConfig
+from pytest_mock_resources.fixture.base import Scope
 from pytest_mock_resources.fixture.moto.action import apply_ordered_actions, MotoAction
 
 
 @pytest.fixture(scope="session")
 def pmr_moto_config():
     """Override this fixture with a :class:`MotoConfig` instance to specify different defaults.
 
@@ -25,90 +26,101 @@
 
 
 @pytest.fixture(scope="session")
 def pmr_moto_container(pytestconfig, pmr_moto_config):
     yield from get_container(pytestconfig, pmr_moto_config)
 
 
-def create_moto_fixture(*ordered_actions: MotoAction, scope="function"):
+def create_moto_fixture(
+    *ordered_actions: MotoAction,
+    region_name: str = "us-east-1",
+    scope: Scope = "function",
+):
     """Produce a Moto fixture.
 
     Any number of fixture functions can be created. Under the hood they will all share the same
     moto server.
 
     .. note::
 
        Each test executes using a different (fake) AWS account through moto. If you create
        boto3 ``client``/``resource`` objects outside of the one handed to the test (for example,
        in the code under test), they should be sure to use the ``aws_access_key_id``,
        ``aws_secret_access_key``, ``aws_session_token``, and ``endpoint_url`` given by the
-       ``pmr_moto_credentials`` fixture.
+       ``<fixturename>.pmr_credentials`` attribute.
 
     .. note::
 
        A moto dashboard should be available for debugging while the container is running.
        By default it would be available at ``http://localhost:5555/moto-api/#`` (but
        the exact URL may be different depending on your host/port config.
 
     Args:
         ordered_actions: Any number of ordered actions to be run on test setup.
+        region_name (str): The name of the AWS region to use, defaults to "us-east-1".
         scope (str): The scope of the fixture can be specified by the user, defaults to "function".
     """
     validate_actions(ordered_actions, fixture="moto")
 
     @pytest.fixture(scope=scope)
-    def _fixture(pmr_moto_credentials) -> Session:
+    def _fixture(pmr_moto_container, pmr_moto_config) -> Session:
+        url = endpoint_url(pmr_moto_config)
+        credentials = Credentials.from_endpoint_url(url, region_name=region_name)
+
         session = Session(
             boto3.Session(
-                aws_access_key_id=pmr_moto_credentials.aws_access_key_id,
-                aws_secret_access_key=pmr_moto_credentials.aws_secret_access_key,
-                aws_session_token=pmr_moto_credentials.aws_session_token,
+                aws_access_key_id=credentials.aws_access_key_id,
+                aws_secret_access_key=credentials.aws_secret_access_key,
+                aws_session_token=credentials.aws_session_token,
+                region_name=region_name,
             ),
-            endpoint_url=pmr_moto_credentials.endpoint_url,
+            endpoint_url=credentials.endpoint_url,
+            pmr_credentials=credentials,
         )
         apply_ordered_actions(session, ordered_actions)
         return session
 
     return _fixture
 
 
-@pytest.fixture()
-def pmr_moto_credentials(pmr_moto_container, pmr_moto_config) -> Credentials:
-    # Attempt at a cross-process way of generating unique 12-character integers.
-    account_id = str(time.time_ns())[:12]
-
-    url = endpoint_url(pmr_moto_config)
-
-    sts = boto3.client(
-        "sts",
-        endpoint_url=url,
-        aws_access_key_id="test",
-        aws_secret_access_key="test",
-    )
-    response = sts.assume_role(
-        RoleArn=f"arn:aws:iam::{account_id}:role/my-role",
-        RoleSessionName="test-session-name",
-        ExternalId="test-external-id",
-    )
-
-    return Credentials(
-        aws_access_key_id=response["Credentials"]["AccessKeyId"],
-        aws_secret_access_key=response["Credentials"]["SecretAccessKey"],
-        aws_session_token=response["Credentials"]["SessionToken"],
-        endpoint_url=url,
-    )
-
-
 @dataclass
 class Credentials:
     aws_access_key_id: str
     aws_secret_access_key: str
     aws_session_token: str
     endpoint_url: str
-    region_name = "us-east-1"
+    region_name: str = "us-east-1"
+
+    @classmethod
+    def from_endpoint_url(
+        cls, url: str, account_id: str | None = None, region_name: str = "us-east-1"
+    ):
+        if account_id is None:
+            # Attempt at a cross-process way of generating unique 12-character integers.
+            account_id = str(time.time_ns())[:12]
+
+        sts = boto3.client(
+            "sts",
+            endpoint_url=url,
+            aws_access_key_id="test",
+            aws_secret_access_key="test",
+        )
+        response = sts.assume_role(
+            RoleArn=f"arn:aws:iam::{account_id}:role/my-role",
+            RoleSessionName="test-session-name",
+            ExternalId="test-external-id",
+        )
+
+        return cls(
+            aws_access_key_id=response["Credentials"]["AccessKeyId"],
+            aws_secret_access_key=response["Credentials"]["SecretAccessKey"],
+            aws_session_token=response["Credentials"]["SessionToken"],
+            endpoint_url=url,
+            region_name=region_name,
+        )
 
     def as_kwargs(self):
         return {
             "aws_access_key_id": self.aws_access_key_id,
             "aws_secret_access_key": self.aws_secret_access_key,
             "aws_session_token": self.aws_session_token,
             "endpoint_url": self.endpoint_url,
@@ -118,13 +130,14 @@
 
 @dataclass
 class Session:
     """Wrap the vanilla boto3 Session object, automatically inserting the endpoint_url field."""
 
     session: boto3.Session
     endpoint_url: str
+    pmr_credentials: Credentials
 
     def client(self, service_name, **kwargs):
         return self.session.client(service_name, endpoint_url=self.endpoint_url, **kwargs)
 
     def resource(self, service_name, **kwargs):
         return self.session.resource(service_name, endpoint_url=self.endpoint_url, **kwargs)
```

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/mysql.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/postgresql.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/postgresql.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 log = logging.getLogger(__name__)
 
 
 class DatabaseExistsError(RuntimeError):
     """Raise when the database being created already exists.
 
     This exception commonly occurs during multiprocess test execution, as a
-    sentinel for gracefully continueing among test workers which attempt to create
+    sentinel for gracefully continuing among test workers which attempt to create
     the same database.
     """
 
 
 @pytest.fixture(scope="session")
 def pmr_postgres_config():
     """Override this fixture with a :class:`PostgresConfig` instance to specify different defaults.
```

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/redis.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     Any number of fixture functions can be created. Under the hood they will all share the same
     database server.
 
     .. note::
 
        If running tests in parallel, the implementation fans out to different redis "database"s,
-       up to a 16 (which is the default container fixed limite). This means you can only run
+       up to a 16 (which is the default container fixed limit). This means you can only run
        up to 16 simultaneous tests.
 
        Additionally, any calls to `flushall` or any other cross-database calls **will** still
        represent cross-test state.
 
        Finally, the above notes are purely describing the current implementation, and should not
        be assumed. In the future, the current database selection mechanism may change, or
```

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/redshift/__init__.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/redshift/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 ):
     """Produce a Redshift fixture.
 
     Any number of fixture functions can be created. Under the hood they will all share the same
     database server.
 
     Note that, by default, redshift uses a postgres container as the database server
-    and attempts to reintroduce appoximations of Redshift features, such as
+    and attempts to reintroduce approximations of Redshift features, such as
     S3 COPY/UNLOAD, redshift-specific functions, and other specific behaviors.
 
     Arguments:
         ordered_actions: Any number of ordered actions to be run on test setup.
         scope: Passthrough pytest's fixture scope.
         tables: Subsets the tables created by `ordered_actions`. This is generally
             most useful when a model-base was specified in `ordered_actions`.
```

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/redshift/udf.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/redshift/udf.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/fixture/sqlite.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/fixture/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Adapt SQLite to act more in line with typical postgresql usage.
 
-SQLite is a desireable test database target because it introduces much less latency across
+SQLite is a desirable test database target because it introduces much less latency across
 tests, is parallelizable, and has a lower minimum fixed test-startup cost.
 
 Unfortunately, SQLite and postgresql do not behave identically in all cases. However, in
 many (typically CRUD) API type database designs, there is no need for postgresql-specific
 features, and SQLite can act as an appropriate stand in.
 
 Where possible though, this module changes the default SQLite behavior to more closely
@@ -111,15 +111,15 @@
         @compiles(JSON, "pmrsqlite")
         @compiles(JSONB, "pmrsqlite")
         @compiles(sqltypes.JSON, "pmrsqlite")
         def compile_json(type_, compiler, **kwargs):
             return "BLOB"
 
     class PostgresLikeDialect(SQLiteDialect_pysqlite):
-        """Define the dialect that collects all postgres-like adapations."""
+        """Define the dialect that collects all postgres-like adaptations."""
 
         name = "pmrsqlite"
 
         supports_statement_cache = True
         ddl_compiler = PMRSQLiteDDLCompiler
         type_compiler = PostgresLikeTypeCompiler
         colspecs = {
```

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/hooks.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/hooks.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/mock_s3_copy.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/mock_s3_copy.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     # Fetching s3_uri
     if tokens.pop(0).lower() != "from":
         raise ValueError(
             (
                 "Possibly malformed S3 URI Format. "
                 "Statement = {statement}"
-                "Redshift fixture only supports S3 Copy statments with the following syntax: "
+                "Redshift fixture only supports S3 Copy statements with the following syntax: "
                 "COPY <table_name> FROM [(column 1, [column2, [..]])] '<file path on S3 bucket>' "
                 "credentials 'aws_access_key_id=<aws_access_key_id>;"
                 "aws_secret_access_key=<aws_secret_access_key>'"
             ).format(statement=statement)
         )
     params["s3_uri"] = strip(tokens.pop(0))
     empty_as_null = False
@@ -91,15 +91,15 @@
                 elif "aws_secret_access_key" in credentials:
                     params["aws_secret_access_key"] = credentials.split("=")[-1]
                 else:
                     raise ValueError(
                         (
                             "Possibly malformed AWS Credentials Format. "
                             "Statement = {statement}"
-                            "Redshift fixture only supports S3 Copy statments with the following "
+                            "Redshift fixture only supports S3 Copy statements with the following "
                             "syntax: COPY <table_name> FROM [(column 1, [column2, [..]])] '"
                             "<file path on S3 bucket>' "
                             "credentials 'aws_access_key_id=<aws_access_key_id>;"
                             "aws_secret_access_key=<aws_secret_access_key>' "
                             "Supportred AWS credentials format: "
                             "[with ]credentials[ AS] 'aws_secret_access_key=y; aws_access_key_id=x'"
                             " No Support for additional credential formats, eg IAM roles, etc, yet."
```

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/mock_s3_unload.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/mock_s3_unload.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,29 +38,29 @@
         select_statement += " " + token
     params["select_statement"] = select_statement
     if error_flag:
         raise ValueError(
             (
                 "Possibly malformed SELECT Statement. "
                 "Statement = {statement}"
-                "Redshift fixture only supports S3 Unload statments with the following syntax: "
+                "Redshift fixture only supports S3 Unload statements with the following syntax: "
                 "UNLOAD ('select-statement') TO 's3://object-path/name-prefix'"
                 "authorization 'aws_access_key_id=<aws_access_key_id>;"
                 "aws_secret_access_key=<aws_secret_access_key>'"
                 "[GZIP] [DELIMITER [ AS ] 'delimiter-char']"
             ).format(statement=statement)
         )
 
     # Fetching s3_uri
     if tokens.pop(0).lower() != "to":
         raise ValueError(
             (
                 "Possibly malformed S3 URI Format. "
                 "Statement = {statement}"
-                "Redshift fixture only supports S3 Unload statments with the following syntax: "
+                "Redshift fixture only supports S3 Unload statements with the following syntax: "
                 "UNLOAD ('select-statement') TO 's3://object-path/name-prefix'"
                 "authorization 'aws_access_key_id=<aws_access_key_id>;"
                 "aws_secret_access_key=<aws_secret_access_key>'"
                 "[GZIP] [DELIMITER [ AS ] 'delimiter-char']"
             ).format(statement=statement)
         )
     params["s3_uri"] = strip(tokens.pop(0))
@@ -86,15 +86,15 @@
                 elif "aws_secret_access_key" in credentials:
                     params["aws_secret_access_key"] = credentials.split("=")[-1]
                 else:
                     raise ValueError(
                         (
                             "Possibly malformed AWS Credentials Format. "
                             "Statement = {statement}"
-                            "Redshift fixture only supports S3 Copy statments with the following "
+                            "Redshift fixture only supports S3 Copy statements with the following "
                             "syntax: COPY <table_name> FROM [(column 1, [column2, [..]])] '"
                             "<file path on S3 bucket>' "
                             "credentials 'aws_access_key_id=<aws_access_key_id>;"
                             "aws_secret_access_key=<aws_secret_access_key>' "
                             "Supportred AWS credentials format: "
                             "[with ]credentials[ AS] 'aws_secret_access_key=y; aws_access_key_id=x'"
                             " No Support for additional credential formats, eg IAM roles, etc, yet."
@@ -116,15 +116,15 @@
                 else:
                     params["delimiter"] = strip(tokens[index + 2])
             except IndexError:
                 raise ValueError(
                     (
                         "Possibly malformed Delimiter Format. "
                         "Statement = {statement}"
-                        "Redshift fixture only supports S3 Unload statments with the following"
+                        "Redshift fixture only supports S3 Unload statements with the following"
                         "syntax: UNLOAD ('select-statement') TO 's3://object-path/name-prefix'"
                         "authorization 'aws_access_key_id=<aws_access_key_id>;"
                         "aws_secret_access_key=<aws_secret_access_key>'"
                         "[GZIP] [DELIMITER [ AS ] 'delimiter-char']"
                     ).format(statement=statement)
                 )
     return params
```

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/psycopg2.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/psycopg2.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/patch/redshift/sqlalchemy.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/patch/redshift/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `pytest_mock_resources-2.7.0/src/pytest_mock_resources/sqlalchemy.py` & `pytest_mock_resources-2.9.0/src/pytest_mock_resources/sqlalchemy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import fnmatch
 import logging
+from collections.abc import Callable
 from dataclasses import dataclass, field
-from typing import Callable, Dict, Iterable, List, Optional, Set, TypeVar, Union
+from typing import Dict, Iterable, List, Optional, Set, TypeVar, Union
 
 import sqlalchemy
 from sqlalchemy import MetaData, text
 from sqlalchemy.orm import scoped_session, Session, sessionmaker
 from sqlalchemy.sql.ddl import CreateSchema
 from sqlalchemy.sql.schema import Table
 
@@ -312,9 +313,9 @@
 def commit(conn):
     try:
         if isinstance(conn, Session):
             return conn.commit()
 
         return conn.execute(text("COMMIT"))
     except sqlalchemy.exc.InvalidRequestError:
-        # In autocommit mode, we wont be able to commit.
+        # In autocommit mode, we won't be able to commit.
         pass
```

### Comparing `pytest_mock_resources-2.7.0/setup.py` & `pytest_mock_resources-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
  'pytest_mock_resources.patch.redshift']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pytest>=1.0',
- 'sqlalchemy>1.0,!=1.4.0,!=1.4.1,!=1.4.2,!=1.4.3,!=1.4.4,!=1.4.5,!=1.4.6,!=1.4.7,!=1.4.8,!=1.4.9,!=1.4.10,!=1.4.11,!=1.4.12,!=1.4.13,!=1.4.14,!=1.4.15,!=1.4.16,!=1.4.17,!=1.4.18,!=1.4.19,!=1.4.20,!=1.4.21,!=1.4.22,!=1.4.23']
+ 'sqlalchemy>1.0,!=1.4.0,!=1.4.1,!=1.4.2,!=1.4.3,!=1.4.4,!=1.4.5,!=1.4.6,!=1.4.7,!=1.4.8,!=1.4.9,!=1.4.10,!=1.4.11,!=1.4.12,!=1.4.13,!=1.4.14,!=1.4.15,!=1.4.16,!=1.4.17,!=1.4.18,!=1.4.19,!=1.4.20,!=1.4.21,!=1.4.22,!=1.4.23',
+ 'typing_extensions']
 
 extras_require = \
 {'docker': ['filelock', 'python-on-whales>=0.22.0'],
  'mongo': ['pymongo', 'filelock', 'python-on-whales>=0.22.0'],
  'moto': ['boto3', 'filelock', 'python-on-whales>=0.22.0'],
  'mysql': ['pymysql>=1.0', 'filelock', 'python-on-whales>=0.22.0'],
  'postgres': ['psycopg2', 'filelock', 'python-on-whales>=0.22.0'],
@@ -38,15 +39,15 @@
 
 entry_points = \
 {'console_scripts': ['pmr = pytest_mock_resources.cli:main'],
  'pytest11': ['pytest_mock_resources = pytest_mock_resources']}
 
 setup_kwargs = {
     'name': 'pytest-mock-resources',
-    'version': '2.7.0',
+    'version': '2.9.0',
     'description': 'A pytest plugin for easily instantiating reproducible mock resources.',
     'long_description': '![CircleCI](https://img.shields.io/circleci/build/gh/schireson/pytest-mock-resources/master)\n[![codecov](https://codecov.io/gh/schireson/pytest-mock-resources/branch/master/graph/badge.svg)](https://codecov.io/gh/schireson/pytest-mock-resources)\n[![Documentation\nStatus](https://readthedocs.org/projects/pytest-mock-resources/badge/?version=latest)](https://pytest-mock-resources.readthedocs.io/en/latest/?badge=latest)\n\n## Introduction\n\nCode which depends on external resources such a databases (postgres, redshift, etc) can be difficult\nto write automated tests for. Conventional wisdom might be to mock or stub out the actual database\ncalls and assert that the code works correctly before/after the calls.\n\nHowever take the following, _simple_ example:\n\n```python\ndef serialize(users):\n    return [\n        {\n            \'user\': user.serialize(),\n            \'address\': user.address.serialize(),\n            \'purchases\': [p.serialize() for p in user.purchases],\n        }\n        for user in users\n    ]\n\ndef view_function(session):\n    users = session.query(User).join(Address).options(selectinload(User.purchases)).all()\n    return serialize(users)\n```\n\nSure, you can test `serialize`, but whether the actual **query** did the correct thing _truly_\nrequires that you execute the query.\n\n## The Pitch\n\nHaving tests depend upon a **real** postgres instance running somewhere is a pain, very fragile, and\nprone to issues across machines and test failures.\n\nTherefore `pytest-mock-resources` (primarily) works by managing the lifecycle of docker containers\nand providing access to them inside your tests.\n\nAs such, this package makes 2 primary assumptions:\n\n- You\'re using `pytest` (hopefully that\'s appropriate, given the package name)\n- For many resources, `docker` is required to be available and running (or accessible through remote\n  docker).\n\nIf you aren\'t familiar with Pytest Fixtures, you can read up on them in the [Pytest\ndocumentation](https://docs.pytest.org/en/latest/fixture.html).\n\nIn the above example, your test file could look something like\n\n```python\nfrom pytest_mock_resources import create_postgres_fixture\nfrom models import ModelBase\n\npg = create_postgres_fixture(ModelBase, session=True)\n\ndef test_view_function_empty_db(pg):\n  response = view_function(pg)\n  assert response == ...\n\ndef test_view_function_user_without_purchases(pg):\n  pg.add(User(...))\n  pg.flush()\n\n  response = view_function(pg)\n  assert response == ...\n\ndef test_view_function_user_with_purchases(pg):\n  pg.add(User(..., purchases=[Purchase(...)]))\n  pg.flush()\n\n  response = view_function(pg)\n  assert response == ...\n```\n\n## Existing Resources (many more possible)\n\n- SQLite\n\n  ```python\n  from pytest_mock_resources import create_sqlite_fixture\n  ```\n\n- Postgres\n\n  ```python\n  from pytest_mock_resources import create_postgres_fixture\n  ```\n\n- Redshift\n\n  **note** Uses postgres under the hood, but the fixture tries to support as much redshift\n  functionality as possible (including redshift\'s `COPY`/`UNLOAD` commands).\n\n  ```python\n  from pytest_mock_resources import create_redshift_fixture\n  ```\n\n- Mongo\n\n  ```python\n  from pytest_mock_resources import create_mongo_fixture\n  ```\n\n- Redis\n\n  ```python\n  from pytest_mock_resources import create_redis_fixture\n  ```\n\n- MySQL\n\n  ```python\n  from pytest_mock_resources import create_mysql_fixture\n  ```\n\n- Moto\n\n  ```python\n  from pytest_mock_resources import create_moto_fixture\n  ```\n\n## Features\n\nGeneral features include:\n\n- Support for "actions" which pre-populate the resource you\'re mocking before the test\n- [Async fixtures](https://pytest-mock-resources.readthedocs.io/en/latest/async.html)\n- Custom configuration for container/resource startup\n\n## Installation\n\n```bash\n# Basic fixture support i.e. SQLite\npip install "pytest-mock-resources"\n\n# General, docker-based fixture support\npip install "pytest-mock-resources[docker]"\n\n# Mongo fixture support, installs `pymongo`\npip install "pytest-mock-resources[mongo]"\n\n# Moto fixture support, installs non-driver extras specific to moto support\npip install "pytest-mock-resources[moto]"\n\n# Redis fixture support, Installs `redis` client\npip install "pytest-mock-resources[redis]"\n\n# Redshift fixture support, installs non-driver extras specific to redshift support\npip install "pytest-mock-resources[redshift]"\n```\n\nAdditionally there are number of **convenience** extras currently provided\nfor installing drivers/clients of specific features. However in most cases,\nyou **should** already be installing the driver/client used for that fixture\nas as first-party dependency of your project.\n\nAs such, we recommend against using these extras, and instead explcitly depending\non the package in question in your own project\'s 1st party dependencies.\n\n```bash\n# Installs psycopg2/psycopg2-binary driver\npip install "pytest-mock-resources[postgres-binary]"\npip install "pytest-mock-resources[postgres]"\n\n# Installs asyncpg driver\npip install "pytest-mock-resources[postgres-async]"\n\n# Installs pymysql driver\npip install "pytest-mock-resources[mysql]"\n```\n\n## Possible Future Resources\n\n- Rabbit Broker\n- AWS Presto\n\nFeel free to file an [issue](https://github.com/schireson/pytest-mock-resources/issues) if you find\nany bugs or want to start a conversation around a mock resource you want implemented!\n\n## Python 2\n\nReleases in the 1.x series were supportive of python 2. However starting from 2.0.0, support for\npython 2 was dropped. We may accept bugfix PRs for the 1.x series, however new development and\nfeatures will not be backported.\n',
     'author': 'Omar Khan',
     'author_email': 'oakhan3@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/schireson/pytest-mock-resources',
```

### Comparing `pytest_mock_resources-2.7.0/PKG-INFO` & `pytest_mock_resources-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mock-resources
-Version: 2.7.0
+Version: 2.9.0
 Summary: A pytest plugin for easily instantiating reproducible mock resources.
 Home-page: https://github.com/schireson/pytest-mock-resources
 License: MIT
 Keywords: pytest,sqlalchemy,docker,fixture,mock
 Author: Omar Khan
 Author-email: oakhan3@gmail.com
 Requires-Python: >=3.7,<4
@@ -34,14 +34,15 @@
 Requires-Dist: pymongo; extra == "mongo"
 Requires-Dist: pymysql (>=1.0); extra == "mysql"
 Requires-Dist: pytest (>=1.0)
 Requires-Dist: python-on-whales (>=0.22.0); extra == "docker" or extra == "postgres" or extra == "postgres-binary" or extra == "postgres-async" or extra == "redshift" or extra == "mongo" or extra == "moto" or extra == "redis" or extra == "mysql"
 Requires-Dist: redis; extra == "redis"
 Requires-Dist: sqlalchemy (>1.0,!=1.4.0,!=1.4.1,!=1.4.2,!=1.4.3,!=1.4.4,!=1.4.5,!=1.4.6,!=1.4.7,!=1.4.8,!=1.4.9,!=1.4.10,!=1.4.11,!=1.4.12,!=1.4.13,!=1.4.14,!=1.4.15,!=1.4.16,!=1.4.17,!=1.4.18,!=1.4.19,!=1.4.20,!=1.4.21,!=1.4.22,!=1.4.23)
 Requires-Dist: sqlparse; extra == "redshift"
+Requires-Dist: typing_extensions
 Project-URL: Repository, https://github.com/schireson/pytest-mock-resources
 Description-Content-Type: text/markdown
 
 ![CircleCI](https://img.shields.io/circleci/build/gh/schireson/pytest-mock-resources/master)
 [![codecov](https://codecov.io/gh/schireson/pytest-mock-resources/branch/master/graph/badge.svg)](https://codecov.io/gh/schireson/pytest-mock-resources)
 [![Documentation
 Status](https://readthedocs.org/projects/pytest-mock-resources/badge/?version=latest)](https://pytest-mock-resources.readthedocs.io/en/latest/?badge=latest)
```


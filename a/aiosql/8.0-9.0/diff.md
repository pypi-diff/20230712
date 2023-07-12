# Comparing `tmp/aiosql-8.0.tar.gz` & `tmp/aiosql-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosql-8.0.tar", last modified: Sat Mar 18 08:21:06 2023, max compression
+gzip compressed data, was "aiosql-9.0.tar", last modified: Wed Jul 12 06:03:48 2023, max compression
```

## Comparing `aiosql-8.0.tar` & `aiosql-9.0.tar`

### file list

```diff
@@ -1,30 +1,124 @@
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-03-18 08:21:06.652553 aiosql-8.0/
--rw-------   0 fabien    (1001) fabien    (1001)     1552 2020-08-14 21:58:38.000000 aiosql-8.0/LICENSE
--rw-------   0 fabien    (1001) fabien    (1001)      778 2023-03-18 08:21:06.652553 aiosql-8.0/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)     8356 2023-03-18 08:20:06.000000 aiosql-8.0/README.rst
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-03-18 08:21:06.652553 aiosql-8.0/aiosql/
--rw-------   0 fabien    (1001) fabien    (1001)      404 2022-10-07 11:14:43.000000 aiosql-8.0/aiosql/__init__.py
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-03-18 08:21:06.652553 aiosql-8.0/aiosql/adapters/
--rw-------   0 fabien    (1001) fabien    (1001)      370 2022-07-31 08:07:34.000000 aiosql-8.0/aiosql/adapters/__init__.py
--rw-------   0 fabien    (1001) fabien    (1001)     2438 2023-03-18 08:20:06.000000 aiosql-8.0/aiosql/adapters/aiosqlite.py
--rw-------   0 fabien    (1001) fabien    (1001)     5120 2023-03-18 08:20:06.000000 aiosql-8.0/aiosql/adapters/asyncpg.py
--rw-------   0 fabien    (1001) fabien    (1001)     3075 2023-03-18 08:20:06.000000 aiosql-8.0/aiosql/adapters/generic.py
--rw-------   0 fabien    (1001) fabien    (1001)     1033 2022-10-27 17:00:40.000000 aiosql-8.0/aiosql/adapters/mysql.py
--rw-------   0 fabien    (1001) fabien    (1001)      182 2022-07-18 12:48:02.000000 aiosql-8.0/aiosql/adapters/pg8000.py
--rw-------   0 fabien    (1001) fabien    (1001)      497 2023-03-18 08:20:06.000000 aiosql-8.0/aiosql/adapters/pyformat.py
--rw-------   0 fabien    (1001) fabien    (1001)      502 2022-07-18 12:48:02.000000 aiosql-8.0/aiosql/adapters/sqlite3.py
--rw-------   0 fabien    (1001) fabien    (1001)     6151 2023-03-18 08:20:06.000000 aiosql-8.0/aiosql/aiosql.py
--rw-------   0 fabien    (1001) fabien    (1001)        0 2021-12-29 16:44:12.000000 aiosql-8.0/aiosql/py.typed
--rw-------   0 fabien    (1001) fabien    (1001)     7198 2022-11-21 20:51:11.000000 aiosql-8.0/aiosql/queries.py
--rw-------   0 fabien    (1001) fabien    (1001)     6812 2023-03-18 08:20:06.000000 aiosql-8.0/aiosql/query_loader.py
--rw-------   0 fabien    (1001) fabien    (1001)     4746 2022-11-21 20:50:44.000000 aiosql-8.0/aiosql/types.py
--rw-------   0 fabien    (1001) fabien    (1001)      673 2023-03-18 08:20:06.000000 aiosql-8.0/aiosql/utils.py
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-03-18 08:21:06.652553 aiosql-8.0/aiosql.egg-info/
--rw-------   0 fabien    (1001) fabien    (1001)      778 2023-03-18 08:21:06.000000 aiosql-8.0/aiosql.egg-info/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)      543 2023-03-18 08:21:06.000000 aiosql-8.0/aiosql.egg-info/SOURCES.txt
--rw-------   0 fabien    (1001) fabien    (1001)        1 2023-03-18 08:21:06.000000 aiosql-8.0/aiosql.egg-info/dependency_links.txt
--rw-------   0 fabien    (1001) fabien    (1001)       11 2023-03-18 08:21:06.000000 aiosql-8.0/aiosql.egg-info/requires.txt
--rw-------   0 fabien    (1001) fabien    (1001)        7 2023-03-18 08:21:06.000000 aiosql-8.0/aiosql.egg-info/top_level.txt
--rw-------   0 fabien    (1001) fabien    (1001)     1247 2023-03-18 08:20:06.000000 aiosql-8.0/pyproject.toml
--rw-------   0 fabien    (1001) fabien    (1001)      914 2023-03-18 08:21:06.652553 aiosql-8.0/setup.cfg
--rw-------   0 fabien    (1001) fabien    (1001)       38 2021-12-29 16:44:12.000000 aiosql-8.0/setup.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.245507 aiosql-9.0/
+-rw-------   0 fabien    (1001) fabien    (1001)     1502 2023-05-29 10:11:04.000000 aiosql-9.0/.dockerignore
+-rw-------   0 fabien    (1001) fabien    (1001)      417 2023-05-14 12:34:57.000000 aiosql-9.0/.editorconfig
+-rw-------   0 fabien    (1001) fabien    (1001)      176 2023-05-14 12:34:57.000000 aiosql-9.0/.flake8
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.241507 aiosql-9.0/.github/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.241507 aiosql-9.0/.github/scripts/
+-rwx------   0 fabien    (1001) fabien    (1001)      577 2023-07-12 04:41:21.000000 aiosql-9.0/.github/scripts/docs.sh
+-rwx------   0 fabien    (1001) fabien    (1001)       87 2023-05-14 12:34:57.000000 aiosql-9.0/.github/scripts/package-build.sh
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.241507 aiosql-9.0/.github/workflows/
+-rw-------   0 fabien    (1001) fabien    (1001)     1540 2023-05-27 17:26:40.000000 aiosql-9.0/.github/workflows/aiosql-package.yml
+-rw-------   0 fabien    (1001) fabien    (1001)      742 2023-05-14 12:34:57.000000 aiosql-9.0/.github/workflows/deploy-pages.yml
+-rw-------   0 fabien    (1001) fabien    (1001)     1502 2023-05-29 10:11:04.000000 aiosql-9.0/.gitignore
+-rw-------   0 fabien    (1001) fabien    (1001)     1552 2023-05-14 12:34:57.000000 aiosql-9.0/LICENSE
+-rw-------   0 fabien    (1001) fabien    (1001)       25 2023-05-29 10:11:04.000000 aiosql-9.0/MANIFEST.in
+-rw-------   0 fabien    (1001) fabien    (1001)    10073 2023-07-12 04:42:41.000000 aiosql-9.0/Makefile
+-rw-------   0 fabien    (1001) fabien    (1001)     9128 2023-07-12 06:03:48.245507 aiosql-9.0/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)     8295 2023-07-12 04:40:21.000000 aiosql-9.0/README.rst
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.241507 aiosql-9.0/aiosql/
+-rw-------   0 fabien    (1001) fabien    (1001)      283 2023-05-27 17:26:40.000000 aiosql-9.0/aiosql/__init__.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.241507 aiosql-9.0/aiosql/adapters/
+-rw-------   0 fabien    (1001) fabien    (1001)      370 2023-05-14 12:34:57.000000 aiosql-9.0/aiosql/adapters/__init__.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2436 2023-05-29 10:11:04.000000 aiosql-9.0/aiosql/adapters/aiosqlite.py
+-rw-------   0 fabien    (1001) fabien    (1001)     5120 2023-05-14 12:34:57.000000 aiosql-9.0/aiosql/adapters/asyncpg.py
+-rw-------   0 fabien    (1001) fabien    (1001)     3156 2023-05-27 17:26:40.000000 aiosql-9.0/aiosql/adapters/duckdb.py
+-rw-------   0 fabien    (1001) fabien    (1001)     3075 2023-05-20 08:35:49.000000 aiosql-9.0/aiosql/adapters/generic.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1033 2023-05-14 12:34:57.000000 aiosql-9.0/aiosql/adapters/mysql.py
+-rw-------   0 fabien    (1001) fabien    (1001)      182 2023-05-14 12:34:57.000000 aiosql-9.0/aiosql/adapters/pg8000.py
+-rw-------   0 fabien    (1001) fabien    (1001)      497 2023-05-14 12:34:57.000000 aiosql-9.0/aiosql/adapters/pyformat.py
+-rw-------   0 fabien    (1001) fabien    (1001)      502 2023-05-14 12:34:57.000000 aiosql-9.0/aiosql/adapters/sqlite3.py
+-rw-------   0 fabien    (1001) fabien    (1001)     6416 2023-05-29 10:11:04.000000 aiosql-9.0/aiosql/aiosql.py
+-rw-------   0 fabien    (1001) fabien    (1001)        0 2023-05-14 12:34:57.000000 aiosql-9.0/aiosql/py.typed
+-rw-------   0 fabien    (1001) fabien    (1001)     7176 2023-05-29 10:11:04.000000 aiosql-9.0/aiosql/queries.py
+-rw-------   0 fabien    (1001) fabien    (1001)     7005 2023-05-27 17:26:40.000000 aiosql-9.0/aiosql/query_loader.py
+-rw-------   0 fabien    (1001) fabien    (1001)     4746 2023-05-14 12:34:57.000000 aiosql-9.0/aiosql/types.py
+-rw-------   0 fabien    (1001) fabien    (1001)      703 2023-05-27 17:26:40.000000 aiosql-9.0/aiosql/utils.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.241507 aiosql-9.0/aiosql.egg-info/
+-rw-------   0 fabien    (1001) fabien    (1001)     9128 2023-07-12 06:03:48.000000 aiosql-9.0/aiosql.egg-info/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)     2490 2023-07-12 06:03:48.000000 aiosql-9.0/aiosql.egg-info/SOURCES.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        1 2023-07-12 06:03:48.000000 aiosql-9.0/aiosql.egg-info/dependency_links.txt
+-rw-------   0 fabien    (1001) fabien    (1001)      427 2023-07-12 06:03:48.000000 aiosql-9.0/aiosql.egg-info/requires.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        7 2023-07-12 06:03:48.000000 aiosql-9.0/aiosql.egg-info/top_level.txt
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.241507 aiosql-9.0/docker/
+-rw-------   0 fabien    (1001) fabien    (1001)       17 2023-05-14 12:34:57.000000 aiosql-9.0/docker/.gitignore
+-rwx------   0 fabien    (1001) fabien    (1001)     1458 2023-05-14 12:34:57.000000 aiosql-9.0/docker/Makefile
+-rw-------   0 fabien    (1001) fabien    (1001)     1052 2023-07-06 06:28:03.000000 aiosql-9.0/docker/README.md
+-rw-------   0 fabien    (1001) fabien    (1001)     1346 2023-05-27 17:26:40.000000 aiosql-9.0/docker/docker-compose.yml
+-rw-------   0 fabien    (1001) fabien    (1001)      791 2023-07-06 06:26:19.000000 aiosql-9.0/docker/dockerfile.python-mariadb
+-rw-------   0 fabien    (1001) fabien    (1001)      505 2023-07-06 06:26:19.000000 aiosql-9.0/docker/dockerfile.python-mysql
+-rw-------   0 fabien    (1001) fabien    (1001)      492 2023-07-06 06:26:19.000000 aiosql-9.0/docker/dockerfile.python-postgres
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.241507 aiosql-9.0/docs/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.241507 aiosql-9.0/docs/source/
+-rw-------   0 fabien    (1001) fabien    (1001)     7898 2023-05-28 06:48:04.000000 aiosql-9.0/docs/source/advanced-topics.rst
+-rw-------   0 fabien    (1001) fabien    (1001)     2493 2023-06-26 06:53:04.000000 aiosql-9.0/docs/source/conf.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2447 2023-05-28 06:48:04.000000 aiosql-9.0/docs/source/contributing.rst
+-rw-------   0 fabien    (1001) fabien    (1001)     4738 2023-05-28 06:48:04.000000 aiosql-9.0/docs/source/database-driver-adapters.rst
+-rw-------   0 fabien    (1001) fabien    (1001)     8311 2023-05-29 10:11:04.000000 aiosql-9.0/docs/source/defining-sql-queries.rst
+-rw-------   0 fabien    (1001) fabien    (1001)     9793 2023-05-29 10:11:04.000000 aiosql-9.0/docs/source/getting-started.rst
+-rw-------   0 fabien    (1001) fabien    (1001)     8295 2023-07-12 04:40:21.000000 aiosql-9.0/docs/source/index.rst
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.245507 aiosql-9.0/docs/source/pydoc/
+-rw-------   0 fabien    (1001) fabien    (1001)     1452 2023-05-28 06:58:31.000000 aiosql-9.0/docs/source/pydoc/aiosql.adapters.rst
+-rw-------   0 fabien    (1001) fabien    (1001)      896 2023-05-28 06:58:31.000000 aiosql-9.0/docs/source/pydoc/aiosql.rst
+-rw-------   0 fabien    (1001) fabien    (1001)       55 2023-05-28 06:58:31.000000 aiosql-9.0/docs/source/pydoc/modules.rst
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.245507 aiosql-9.0/example/
+-rw-------   0 fabien    (1001) fabien    (1001)     2640 2023-05-14 12:34:57.000000 aiosql-9.0/example/example.py
+-rw-------   0 fabien    (1001) fabien    (1001)      299 2023-05-14 12:34:57.000000 aiosql-9.0/example/greetings.py
+-rwx------   0 fabien    (1001) fabien    (1001)      303 2023-05-14 12:34:57.000000 aiosql-9.0/example/greetings.sh
+-rw-------   0 fabien    (1001) fabien    (1001)      289 2023-05-14 12:34:57.000000 aiosql-9.0/example/greetings.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      485 2023-05-14 12:34:57.000000 aiosql-9.0/example/greetings_async.py
+-rw-------   0 fabien    (1001) fabien    (1001)      509 2023-05-14 12:34:57.000000 aiosql-9.0/example/greetings_create.sql
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.245507 aiosql-9.0/example/sql/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.245507 aiosql-9.0/example/sql/blogs/
+-rw-------   0 fabien    (1001) fabien    (1001)      671 2023-05-14 12:34:57.000000 aiosql-9.0/example/sql/blogs/blogs.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      422 2023-05-14 12:34:57.000000 aiosql-9.0/example/sql/create_schema.sql
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.245507 aiosql-9.0/example/sql/users/
+-rw-------   0 fabien    (1001) fabien    (1001)      189 2023-05-14 12:34:57.000000 aiosql-9.0/example/sql/users/users.sql
+-rw-------   0 fabien    (1001) fabien    (1001)     1625 2023-06-26 06:52:51.000000 aiosql-9.0/pyproject.toml
+-rw-------   0 fabien    (1001) fabien    (1001)       38 2023-07-12 06:03:48.245507 aiosql-9.0/setup.cfg
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.245507 aiosql-9.0/tests/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.241507 aiosql-9.0/tests/blogdb/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.245507 aiosql-9.0/tests/blogdb/data/
+-rw-------   0 fabien    (1001) fabien    (1001)      199 2023-05-14 12:34:57.000000 aiosql-9.0/tests/blogdb/data/blogs_data.csv
+-rw-------   0 fabien    (1001) fabien    (1001)       53 2023-05-14 12:34:57.000000 aiosql-9.0/tests/blogdb/data/users_data.csv
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.241507 aiosql-9.0/tests/blogdb/sql/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.245507 aiosql-9.0/tests/blogdb/sql/blogs/
+-rw-------   0 fabien    (1001) fabien    (1001)       29 2023-05-14 12:34:57.000000 aiosql-9.0/tests/blogdb/sql/blogs/blogs.oops
+-rw-------   0 fabien    (1001) fabien    (1001)      935 2023-05-27 17:26:40.000000 aiosql-9.0/tests/blogdb/sql/blogs/blogs.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      700 2023-05-27 17:26:40.000000 aiosql-9.0/tests/blogdb/sql/blogs/blogs_duckdb.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      486 2023-05-14 12:34:57.000000 aiosql-9.0/tests/blogdb/sql/blogs/blogs_mysql.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      975 2023-05-27 17:26:40.000000 aiosql-9.0/tests/blogdb/sql/blogs/blogs_pg.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      588 2023-05-27 17:26:40.000000 aiosql-9.0/tests/blogdb/sql/blogs/blogs_sqlite.sql
+-rw-------   0 fabien    (1001) fabien    (1001)        0 2023-05-14 12:34:57.000000 aiosql-9.0/tests/blogdb/sql/blogs/empty.sql
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.245507 aiosql-9.0/tests/blogdb/sql/comments/
+-rw-------   0 fabien    (1001) fabien    (1001)      271 2023-05-27 17:26:40.000000 aiosql-9.0/tests/blogdb/sql/comments/comments_duckdb.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      218 2023-05-14 12:34:57.000000 aiosql-9.0/tests/blogdb/sql/comments/comments_pg.sql
+-rw-------   0 fabien    (1001) fabien    (1001)      241 2023-05-14 12:34:57.000000 aiosql-9.0/tests/blogdb/sql/comments/comments_sqlite.sql
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.245507 aiosql-9.0/tests/blogdb/sql/misc/
+-rw-------   0 fabien    (1001) fabien    (1001)      735 2023-05-27 17:26:40.000000 aiosql-9.0/tests/blogdb/sql/misc/misc.sql
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-12 06:03:48.245507 aiosql-9.0/tests/blogdb/sql/users/
+-rw-------   0 fabien    (1001) fabien    (1001)     1122 2023-05-14 12:34:57.000000 aiosql-9.0/tests/blogdb/sql/users/users.sql
+-rw-------   0 fabien    (1001) fabien    (1001)     1436 2023-05-29 10:11:04.000000 aiosql-9.0/tests/conf_duckdb.py
+-rw-------   0 fabien    (1001) fabien    (1001)     3288 2023-05-14 12:34:57.000000 aiosql-9.0/tests/conf_mysql.py
+-rw-------   0 fabien    (1001) fabien    (1001)     3656 2023-05-29 10:11:04.000000 aiosql-9.0/tests/conf_pgsql.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2216 2023-05-27 17:26:40.000000 aiosql-9.0/tests/conf_schema.py
+-rw-------   0 fabien    (1001) fabien    (1001)      494 2023-05-29 10:11:04.000000 aiosql-9.0/tests/conf_sqlite.py
+-rw-------   0 fabien    (1001) fabien    (1001)      830 2023-05-27 17:26:40.000000 aiosql-9.0/tests/conftest.py
+-rw-------   0 fabien    (1001) fabien    (1001)      256 2023-05-27 17:26:40.000000 aiosql-9.0/tests/pytest.ini
+-rw-------   0 fabien    (1001) fabien    (1001)    14739 2023-05-27 17:26:40.000000 aiosql-9.0/tests/run_tests.py
+-rw-------   0 fabien    (1001) fabien    (1001)     3305 2023-05-29 10:11:04.000000 aiosql-9.0/tests/test_aiosqlite.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2757 2023-05-29 10:11:04.000000 aiosql-9.0/tests/test_apsw.py
+-rw-------   0 fabien    (1001) fabien    (1001)     5363 2023-05-29 10:11:04.000000 aiosql-9.0/tests/test_asyncpg.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2250 2023-05-29 10:11:04.000000 aiosql-9.0/tests/test_duckdb.py
+-rw-------   0 fabien    (1001) fabien    (1001)     6090 2023-05-14 12:34:57.000000 aiosql-9.0/tests/test_loading.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2346 2023-05-29 10:11:04.000000 aiosql-9.0/tests/test_mariadb.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2386 2023-05-29 10:11:04.000000 aiosql-9.0/tests/test_myco.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2637 2023-05-29 10:11:04.000000 aiosql-9.0/tests/test_mysqldb.py
+-rw-------   0 fabien    (1001) fabien    (1001)     3439 2023-05-14 12:34:57.000000 aiosql-9.0/tests/test_patterns.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2303 2023-05-29 10:11:04.000000 aiosql-9.0/tests/test_pg8000.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2129 2023-05-29 10:11:04.000000 aiosql-9.0/tests/test_psycopg2.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2101 2023-05-29 10:11:04.000000 aiosql-9.0/tests/test_psycopg3.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2424 2023-05-29 10:11:04.000000 aiosql-9.0/tests/test_pygresql.py
+-rw-------   0 fabien    (1001) fabien    (1001)     2323 2023-05-29 10:11:04.000000 aiosql-9.0/tests/test_pymysql.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1933 2023-05-29 10:11:04.000000 aiosql-9.0/tests/test_sqlite3.py
+-rw-------   0 fabien    (1001) fabien    (1001)      948 2023-05-14 12:34:57.000000 aiosql-9.0/tests/utils.py
+-rwx------   0 fabien    (1001) fabien    (1001)      149 2023-05-14 12:34:57.000000 aiosql-9.0/tests/wait.py
```

### Comparing `aiosql-8.0/LICENSE` & `aiosql-9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosql-8.0/README.rst` & `aiosql-9.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -28,17 +28,19 @@
 `psycopg2 <https://www.psycopg.org/docs/>`__,
 `pg8000 <https://pypi.org/project/pg8000/>`__,
 `pygresql <http://www.pygresql.org/>`__,
 `asyncpg <https://magicstack.github.io/asyncpg/current/>`__),
 `MySQL <https://www.mysql.com/>`__
 (`PyMySQL <https://github.com/PyMySQL/PyMySQL/>`__,
 `mysqlclient <https://pypi.org/project/mysqlclient/>`__,
-`mysql-connector <https://dev.mysql.com/doc/connector-python/en/>`__) and
+`mysql-connector <https://dev.mysql.com/doc/connector-python/en/>`__),
 `MariaDB <https://mariadb.org/>`__
-(`mariadb <https://pypi.org/project/mariadb/>`__)
+(`mariadb <https://pypi.org/project/mariadb/>`__) and
+`DuckDB <https://www.duckdb.org/>`__
+(`duckdb <https://duckdb.org/docs/api/python/dbapi>`__),
 out of the box.
 Note that some detailed feature support may vary depending on the underlying driver
 and database engine actual capabilities.
 
 This module is an implementation of
 `Kris Jenkins' yesql <https://github.com/krisajenkins/yesql>`__
 `Clojure <https://clojure.org/>`__ library to the
@@ -62,15 +64,15 @@
 ..
    hardcoded coverage and tests, 100% and 162/15 if docker run is ok
 
 .. image:: https://img.shields.io/badge/coverage-100%25-success
    :alt: Code Coverage
    :target: https://github.com/nackjicholson/aiosql/actions/
 
-.. image:: https://img.shields.io/badge/tests-167%20✓-success
+.. image:: https://img.shields.io/badge/tests-189%20✓-success
    :alt: Tests
    :target: https://github.com/nackjicholson/aiosql/actions/
 
 .. image:: https://img.shields.io/github/issues/nackjicholson/aiosql?style=flat
    :alt: Issues
    :target: https://github.com/nackjicholson/aiosql/issues/
 
@@ -86,19 +88,23 @@
    :alt: Stars
    :target: https://github.com/nackjicholson/aiosql/stargazers
 
 .. image:: https://img.shields.io/pypi/v/aiosql
    :alt: Version
    :target: https://pypi.org/project/aiosql/
 
-.. image:: https://img.shields.io/badge/databases-4-informational
+.. image:: https://img.shields.io/github/languages/code-size/nackjicholson/aiosql?style=flat
+   :alt: Code Size
+   :target: https://github.com/nackjicholson/aiosql/
+
+.. image:: https://img.shields.io/badge/databases-5-informational
    :alt: Databases
    :target: https://github.com/nackjicholson/aiosql/
 
-.. image:: https://img.shields.io/badge/drivers-12-informational
+.. image:: https://img.shields.io/badge/drivers-13-informational
    :alt: Drivers
    :target: https://github.com/nackjicholson/aiosql/
 
 .. image:: https://img.shields.io/github/languages/count/nackjicholson/aiosql?style=flat
    :alt: Language Count
    :target: https://en.wikipedia.org/wiki/Programming_language
 
@@ -109,15 +115,15 @@
 .. image:: https://img.shields.io/pypi/pyversions/aiosql?style=flat
    :alt: Python Versions
    :target: https://www.python.org/
 
 ..
    some non-sense badge about badges:-)
 
-.. image:: https://img.shields.io/badge/badges-15-informational
+.. image:: https://img.shields.io/badge/badges-16-informational
    :alt: Badges
    :target: https://shields.io/
 
 .. image:: https://img.shields.io/pypi/l/aiosql?style=flat
    :alt: BSD 2-Clause License
    :target: https://opensource.org/licenses/BSD-2-Clause
 
@@ -207,35 +213,20 @@
 Why you might want to use this
 ------------------------------
 
 * You think SQL is pretty good, and writing SQL is an important part of your applications.
 * You don't want to write your SQL in strings intermixed with your python code.
 * You're not using an ORM like `SQLAlchemy <https://www.sqlalchemy.org/>`__ or
   `Django <https://www.djangoproject.com/>`__ ,
-  with large (100k lines) code imprints vs under 800 for `aiosql`,
+  with large (100k lines) code imprints vs about 800 for `aiosql`,
   and you don't need to.
 * You want to be able to reuse your SQL in other contexts.
   Loading it into `psql` or other database tools.
 
 
 Why you might NOT want to use this
 ----------------------------------
 
 * You're looking for an `ORM <https://en.wikipedia.org/wiki/Object-relational_mapping>`__.
 * You aren't comfortable writing SQL code.
 * You don't have anything in your application that requires complicated SQL beyond basic CRUD operations.
 * Dynamically loaded objects built at runtime really bother you.
-
-
-Table of Contents
------------------
-
-.. toctree::
-   :maxdepth: 2
-   :caption: Contents:
-
-   Getting Started <getting-started>
-   Defining SQL Queries <defining-sql-queries>
-   Advanced Topics <advanced-topics>
-   Database Driver Adapters <database-driver-adapters>
-   Contributing <contributing>
-   API <pydoc/modules>
```

### Comparing `aiosql-8.0/aiosql/adapters/aiosqlite.py` & `aiosql-9.0/aiosql/adapters/aiosqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 
 class AioSQLiteAdapter:
     is_aio_driver = True
 
     def process_sql(self, _query_name, _op_type, sql):
         """Pass through function because the ``aiosqlite`` driver can already handle the
-        :var_name format used by aiosql and doesn't need any additional processing.
+        ``:var_name`` format used by aiosql and doesn't need any additional processing.
 
         Args:
-            _query_name (str): The name of the sql query.
-            _op_type (SQLOperationType): The type of SQL operation performed by the query.
-            sql (str): The sql as written before processing.
+
+        - _query_name (str): The name of the sql query.
+        - _op_type (SQLOperationType): The type of SQL operation performed by the query.
+        - sql (str): The sql as written before processing.
 
         Returns:
-            str: Original SQL text unchanged.
+
+        - str: Original SQL text unchanged.
         """
         return sql
 
     async def select(self, conn, _query_name, sql, parameters, record_class=None):
         async with conn.execute(sql, parameters) as cur:
             results = await cur.fetchall()
             if record_class is not None:
```

### Comparing `aiosql-8.0/aiosql/adapters/asyncpg.py` & `aiosql-9.0/aiosql/adapters/asyncpg.py`

 * *Files identical despite different names*

### Comparing `aiosql-8.0/aiosql/adapters/generic.py` & `aiosql-9.0/aiosql/adapters/generic.py`

 * *Files identical despite different names*

### Comparing `aiosql-8.0/aiosql/adapters/mysql.py` & `aiosql-9.0/aiosql/adapters/mysql.py`

 * *Files identical despite different names*

### Comparing `aiosql-8.0/aiosql/aiosql.py` & `aiosql-9.0/aiosql/aiosql.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .adapters.aiosqlite import AioSQLiteAdapter
 from .adapters.asyncpg import AsyncPGAdapter
 from .adapters.pyformat import PyFormatAdapter
 from .adapters.mysql import BrokenMySQLAdapter
 from .adapters.generic import GenericAdapter
 from .adapters.sqlite3 import SQLite3Adapter
 from .adapters.pg8000 import Pg8000Adapter
+from .adapters.duckdb import DuckDBAdapter
 from .utils import SQLLoadException, log
 from .queries import Queries
 from .query_loader import QueryLoader
 from .types import DriverAdapterProtocol
 
 _ADAPTERS: Dict[str, Callable[..., DriverAdapterProtocol]] = {
     "aiosqlite": AioSQLiteAdapter,  # type: ignore
@@ -22,14 +23,15 @@
     "mysql-connector": PyFormatAdapter,
     "pg8000": Pg8000Adapter,
     "psycopg": PyFormatAdapter,
     "psycopg2": PyFormatAdapter,
     "pygresql": PyFormatAdapter,
     "pymysql": BrokenMySQLAdapter,
     "sqlite3": SQLite3Adapter,
+    "duckdb": DuckDBAdapter,
 }
 
 
 def register_adapter(name: str, adapter: Callable[..., DriverAdapterProtocol]):
     """Register or override an adapter."""
     if name.lower() in _ADAPTERS:
         log.warning(f"overriding aiosql adapter {name}")
@@ -69,48 +71,49 @@
     loader_cls: Type[QueryLoader] = QueryLoader,
     queries_cls: Type[Queries] = Queries,
 ):
     """Load queries from a SQL string.
 
     **Parameters:**
 
-    * **sql** - A string containing SQL statements and aiosql name.
-    * **driver_adapter** - Either a string to designate one of the aiosql built-in database driver
-    adapters. One of many available for SQLite, Postgres and MySQL. If you have defined your
-    own adapter class, you can pass it's constructor.
-    * **record_classes** - *(optional)* **DEPRECATED** Mapping of strings used in "record_class"
-    declarations to the python classes which aiosql should use when marshaling SQL results.
-    * **loader_cls** - *(optional)* Custom constructor for QueryLoader extensions.
-    * **queries_cls** - *(optional)* Custom constructor for Queries extensions.
+    - **sql** - A string containing SQL statements and aiosql name.
+    - **driver_adapter** - Either a string to designate one of the aiosql built-in database driver
+      adapters. One of many available for SQLite, Postgres and MySQL. If you have defined your
+      own adapter class, you can pass it's constructor.
+    - **record_classes** - *(optional)* **DEPRECATED** Mapping of strings used in "record_class"
+      declarations to the python classes which aiosql should use when marshaling SQL results.
+    - **loader_cls** - *(optional)* Custom constructor for QueryLoader extensions.
+    - **queries_cls** - *(optional)* Custom constructor for Queries extensions.
 
-    **Returns:** `Queries`
+    **Returns:** ``Queries``
 
     Usage:
 
     Loading queries from a SQL string.
 
-    ```python
-    import sqlite3
-    import aiosql
-
-    sql_text = \"""
-    -- name: get-all-greetings
-    -- Get all the greetings in the database
-    select * from greetings;
-
-    -- name: get-user-by-username^
-    -- Get all the users from the database,
-    -- and return it as a dict
-    select * from users where username = :username;
-    \"""
-
-    queries = aiosql.from_str(sql_text, "sqlite3")
-    queries.get_all_greetings(conn)
-    queries.get_user_by_username(conn, username="willvaughn")
-    ```
+    .. code-block:: python
+
+      import sqlite3
+      import aiosql
+
+      sql_text = \"""
+      -- name: get-all-greetings
+      -- Get all the greetings in the database
+      select * from greetings;
+
+      -- name: get-user-by-username^
+      -- Get all the users from the database,
+      -- and return it as a dict
+      select * from users where username = :username;
+      \"""
+
+      queries = aiosql.from_str(sql_text, "sqlite3")
+      queries.get_all_greetings(conn)
+      queries.get_user_by_username(conn, username="willvaughn")
+
     """
     adapter = _make_driver_adapter(driver_adapter)
     query_loader = loader_cls(adapter, record_classes)
     query_data = query_loader.load_query_data_from_sql(sql)
     return queries_cls(adapter).load_from_list(query_data)
 
 
@@ -118,47 +121,51 @@
     sql_path: Union[str, Path],
     driver_adapter: Union[str, Callable[..., DriverAdapterProtocol]],
     record_classes: Optional[Dict] = None,
     *,
     loader_cls: Type[QueryLoader] = QueryLoader,
     queries_cls: Type[Queries] = Queries,
     ext: Tuple[str] = (".sql",),
+    encoding=None,
 ):
     """Load queries from a `.sql` file, or directory of `.sql` files.
 
     **Parameters:**
 
-    * **sql_path** - Path to a `.sql` file or directory containing `.sql` files.
-    * **driver_adapter** - Either a string to designate one of the aiosql built-in database driver
-    adapters. One of many available for SQLite, Postgres and MySQL. If you have defined your own
-    adapter class, you may pass its constructor.
-    * **record_classes** - *(optional)* **DEPRECATED** Mapping of strings used in "record_class"
-    declarations to the python classes which aiosql should use when marshaling SQL results.
-    * **loader_cls** - *(optional)* Custom constructor for `QueryLoader` extensions.
-    * **queries_cls** - *(optional)* Custom constructor for `Queries` extensions.
-    * **ext** - *(optional)* allowed file extensions for query files, default is `(".sql",)`
+    - **sql_path** - Path to a `.sql` file or directory containing `.sql` files.
+    - **driver_adapter** - Either a string to designate one of the aiosql built-in database driver
+      adapters. One of many available for SQLite, Postgres and MySQL. If you have defined your own
+      adapter class, you may pass its constructor.
+    - **record_classes** - *(optional)* **DEPRECATED** Mapping of strings used in "record_class"
+      declarations to the python classes which aiosql should use when marshaling SQL results.
+    - **loader_cls** - *(optional)* Custom constructor for `QueryLoader` extensions.
+    - **queries_cls** - *(optional)* Custom constructor for `Queries` extensions.
+    - **ext** - *(optional)* allowed file extensions for query files, default is `(".sql",)`.
+    - **encoding** - *(optional)* encoding for reading files.
 
     **Returns:** `Queries`
 
     Usage:
 
-    ```python
-    >>> queries = aiosql.from_path("./sql", "psycopg2")
-    >>> queries = aiosql.from_path("./sql", MyDBAdapter)
-    ```
+    .. code-block:: python
+
+      queries = aiosql.from_path("./sql", "psycopg2")
+      queries = aiosql.from_path("./sql", MyDBAdapter)
     """
     path = Path(sql_path)
 
     if not path.exists():
         raise SQLLoadException(f"File does not exist: {path}")
 
     adapter = _make_driver_adapter(driver_adapter)
     query_loader = loader_cls(adapter, record_classes)
 
     if path.is_file():
-        query_data = query_loader.load_query_data_from_file(path)
+        query_data = query_loader.load_query_data_from_file(path, encoding=encoding)
         return queries_cls(adapter).load_from_list(query_data)
     elif path.is_dir():
-        query_data_tree = query_loader.load_query_data_from_dir_path(path, ext=ext)
+        query_data_tree = query_loader.load_query_data_from_dir_path(
+            path, ext=ext, encoding=encoding
+        )
         return queries_cls(adapter).load_from_tree(query_data_tree)
     else:  # pragma: no cover
         raise SQLLoadException(f"The sql_path must be a directory or file, got {sql_path}")
```

### Comparing `aiosql-8.0/aiosql/queries.py` & `aiosql-9.0/aiosql/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,47 +122,47 @@
     else:
         return [fn]
 
 
 class Queries:
     """Container object with dynamic methods built from SQL queries.
 
-    The `-- name` definition comments in the content of the SQL determine what the dynamic
+    The ``-- name`` definition comments in the content of the SQL determine what the dynamic
     methods of this class will be named.
 
     **Parameters:**
 
-    * **driver_adapter** - Either a string to designate one of the aiosql built-in database driver
-    adapters. One of "sqlite3", "psycopg2", "aiosqlite", or "asyncpg". If you have defined your
-    own adapter class, you can pass it's constructor.
+    - **driver_adapter** - Either a string to designate one of the aiosql built-in database driver
+      adapters (e.g. "sqlite3", "psycopg").
+      If you have defined your own adapter class, you can pass its constructor.
     """
 
     def __init__(self, driver_adapter: DriverAdapterProtocol):
         self.driver_adapter: DriverAdapterProtocol = driver_adapter
         self.is_aio: bool = getattr(driver_adapter, "is_aio_driver", False)
         self._available_queries: Set[str] = set()
 
     @property
     def available_queries(self) -> List[str]:
         """Returns listing of all the available query methods loaded in this class.
 
-        **Returns:** `List[str]` List of dot-separated method accessor names.
+        **Returns:** ``list[str]`` List of dot-separated method accessor names.
         """
         return sorted(self._available_queries)
 
     def __repr__(self):
         return "Queries(" + self.available_queries.__repr__() + ")"
 
     def add_query(self, query_name: str, fn: Callable):
         """Adds a new dynamic method to this class.
 
         **Parameters:**
 
-        * **query_name** - The method name as found in the SQL content.
-        * **fn** - The loaded query function.
+        - **query_name** - The method name as found in the SQL content.
+        - **fn** - The loaded query function.
         """
         setattr(self, query_name, fn)
         self._available_queries.add(query_name)
 
     def add_queries(self, queries: List[QueryFn]):
         """Add query methods to `Queries` instance."""
         for fn in queries:
@@ -170,16 +170,16 @@
             self.add_query(query_name, MethodType(fn, self))
 
     def add_child_queries(self, child_name: str, child_queries: "Queries"):
         """Adds a Queries object as a property.
 
         **Parameters:**
 
-        * **child_name** - The property name to group the child queries under.
-        * **child_queries** - Queries instance to add as sub-queries.
+        - **child_name** - The property name to group the child queries under.
+        - **child_queries** - Queries instance to add as sub-queries.
         """
         setattr(self, child_name, child_queries)
         for child_query_name in child_queries.available_queries:
             self._available_queries.add(f"{child_name}.{child_query_name}")
 
     def load_from_list(self, query_data: List[QueryDatum]):
         """Load Queries from a list of `QuaryDatum`"""
```

### Comparing `aiosql-8.0/aiosql/query_loader.py` & `aiosql-9.0/aiosql/query_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,32 +143,38 @@
         data = []
         # first item is anything before the first query definition, drop it!
         for qdef in qdefs[1:]:
             data.append(self._make_query_datum(qdef, ns_parts, (fname, lineno) if fname else None))
             lineno += qdef.count("\n")
         return data
 
-    def load_query_data_from_file(self, path: Path, ns_parts: List[str] = []) -> List[QueryDatum]:
-        return self.load_query_data_from_sql(path.read_text(), ns_parts, path)
+    def load_query_data_from_file(
+        self, path: Path, ns_parts: List[str] = [], encoding=None
+    ) -> List[QueryDatum]:
+        return self.load_query_data_from_sql(path.read_text(encoding=encoding), ns_parts, path)
 
-    def load_query_data_from_dir_path(self, dir_path, ext=(".sql",)) -> QueryDataTree:
+    def load_query_data_from_dir_path(
+        self, dir_path, ext=(".sql",), encoding=None
+    ) -> QueryDataTree:
         if not dir_path.is_dir():
             raise ValueError(f"The path {dir_path} must be a directory")
 
-        def _recurse_load_query_data_tree(path, ns_parts=[], ext=(".sql",)):
+        def _recurse_load_query_data_tree(path, ns_parts=[], ext=(".sql",), encoding=None):
             query_data_tree = {}
             for p in path.iterdir():
                 if p.is_file():
                     if p.suffix not in ext:
                         continue
-                    for query_datum in self.load_query_data_from_file(p, ns_parts):
+                    for query_datum in self.load_query_data_from_file(
+                        p, ns_parts, encoding=encoding
+                    ):
                         query_data_tree[query_datum.query_name] = query_datum
                 elif p.is_dir():
                     query_data_tree[p.name] = _recurse_load_query_data_tree(
-                        p, ns_parts + [p.name], ext=ext
+                        p, ns_parts + [p.name], ext=ext, encoding=encoding
                     )
                 else:  # pragma: no cover
                     # This should be practically unreachable.
                     raise SQLLoadException(f"The path must be a directory or file, got {p}")
             return query_data_tree
 
-        return _recurse_load_query_data_tree(dir_path, ext=ext)
+        return _recurse_load_query_data_tree(dir_path, ext=ext, encoding=encoding)
```

### Comparing `aiosql-8.0/aiosql/types.py` & `aiosql-9.0/aiosql/types.py`

 * *Files identical despite different names*

### Comparing `aiosql-8.0/aiosql/utils.py` & `aiosql-9.0/aiosql/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     r"(?P<squote>\'(\'\'|[^\'])*\')|"
     # NOTE beware of overlapping re
     r"(?P<lead>[^:]):(?P<var_name>[\w-]+)(?=[^:]?)"
 )
 """Pattern to identifies colon-variables in SQL code"""
 
 log = logging.getLogger("aiosql")
+# log.setLevel(logging.DEBUG)
 
 
 class SQLLoadException(Exception):
     """Raised when there is a problem loading SQL content from a file or directory"""
 
     pass
```


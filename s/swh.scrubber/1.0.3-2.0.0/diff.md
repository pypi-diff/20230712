# Comparing `tmp/swh.scrubber-1.0.3.tar.gz` & `tmp/swh.scrubber-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.scrubber-1.0.3.tar", last modified: Tue Apr 18 15:50:00 2023, max compression
+gzip compressed data, was "swh.scrubber-2.0.0.tar", last modified: Wed Jul 12 09:53:36 2023, max compression
```

## Comparing `swh.scrubber-1.0.3.tar` & `swh.scrubber-2.0.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/
--rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)     1039 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      149 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     2329 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1408 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/README.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1408 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)      156 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      246 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      413 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      222 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       57 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      252 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2454 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh/scrubber/
--rw-r--r--   0 jenkins    (115) docker     (999)      727 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8189 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18626 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/db.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7601 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/fixer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2764 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/journal_checker.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3052 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/origin_locator.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/py.typed
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh/scrubber/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)      201 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/20-enums.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5048 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2911 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/60-indexes.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/
--rw-r--r--   0 jenkins    (115) docker     (999)      942 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/2.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2338 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/3.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      989 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/4.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1567 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/5.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    16545 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/storage_checker.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh/scrubber/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      901 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)    14324 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/storage_checker_tests.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5345 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2693 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_db.py
--rw-r--r--   0 jenkins    (115) docker     (999)    11471 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_fixer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1053 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3913 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_journal_kafka.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5408 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_origin_locator.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1035 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_storage_cassandra.py
--rw-r--r--   0 jenkins    (115) docker     (999)      780 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_storage_postgresql.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1671 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     2329 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1499 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       50 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      192 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1514 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:36.374925 swh.scrubber-2.0.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)     1039 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      149 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     3822 2023-07-12 09:53:36.378924 swh.scrubber-2.0.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     2901 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/README.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:36.370925 swh.scrubber-2.0.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2901 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:36.370925 swh.scrubber-2.0.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:36.370925 swh.scrubber-2.0.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)      156 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      246 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      413 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      222 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       75 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      261 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-07-12 09:53:36.378924 swh.scrubber-2.0.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2454 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:36.370925 swh.scrubber-2.0.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:36.374925 swh.scrubber-2.0.0/swh/scrubber/
+-rw-r--r--   0 jenkins    (115) docker     (999)      727 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12162 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    27791 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/db.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7601 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/fixer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2764 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/journal_checker.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3052 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/origin_locator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/py.typed
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:36.374925 swh.scrubber-2.0.0/swh/scrubber/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)      201 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/sql/20-enums.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5735 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3081 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/sql/60-indexes.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:36.374925 swh.scrubber-2.0.0/swh/scrubber/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) docker     (999)      942 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/sql/upgrades/2.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2338 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/sql/upgrades/3.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      989 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/sql/upgrades/4.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1567 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/sql/upgrades/5.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2524 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/sql/upgrades/6.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    16136 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/storage_checker.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:36.374925 swh.scrubber-2.0.0/swh/scrubber/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1329 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    14835 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/tests/storage_checker_tests.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    15336 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8262 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/tests/test_db.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    11471 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/tests/test_fixer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1053 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3913 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/tests/test_journal_kafka.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5408 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/tests/test_origin_locator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1035 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/tests/test_storage_cassandra.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      780 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/tests/test_storage_postgresql.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1671 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/swh/scrubber/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-12 09:53:36.370925 swh.scrubber-2.0.0/swh.scrubber.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3822 2023-07-12 09:53:36.000000 swh.scrubber-2.0.0/swh.scrubber.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1531 2023-07-12 09:53:36.000000 swh.scrubber-2.0.0/swh.scrubber.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-07-12 09:53:36.000000 swh.scrubber-2.0.0/swh.scrubber.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       50 2023-07-12 09:53:36.000000 swh.scrubber-2.0.0/swh.scrubber.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      219 2023-07-12 09:53:36.000000 swh.scrubber-2.0.0/swh.scrubber.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-07-12 09:53:36.000000 swh.scrubber-2.0.0/swh.scrubber.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1550 2023-07-12 09:53:30.000000 swh.scrubber-2.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `swh.scrubber-1.0.3/.pre-commit-config.yaml` & `swh.scrubber-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/CODE_OF_CONDUCT.md` & `swh.scrubber-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/LICENSE` & `swh.scrubber-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/setup.py` & `swh.scrubber-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/__init__.py` & `swh.scrubber-2.0.0/swh/scrubber/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/cli.py` & `swh.scrubber-2.0.0/swh/scrubber/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # Copyright (C) 2022  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import os
 from typing import Optional
+import warnings
 
 import click
 
 from swh.core.cli import CONTEXT_SETTINGS
 from swh.core.cli import swh as swh_cli_group
+from swh.model.swhids import ObjectType
 
 
 @swh_cli_group.group(name="scrubber", context_settings=CONTEXT_SETTINGS)
 @click.option(
     "--config-file",
     "-C",
     default=None,
@@ -25,16 +27,16 @@
 )
 @click.pass_context
 def scrubber_cli_group(ctx, config_file: Optional[str]) -> None:
     """main command group of the datastore scrubber
 
     Expected config format::
 
-        scrubber_db:
-            cls: local
+        scrubber:
+            cls: postgresql
             db: "service=..."    # libpq DSN
 
         # for storage checkers + origin locator only:
         storage:
             cls: postgresql     # cannot be remote for checkers, as they need direct
                                 # access to the pg DB
             db": "service=..."  # libpq DSN
@@ -71,30 +73,40 @@
     if config_file:
         if not os.path.exists(config_file):
             raise ValueError("%s does not exist" % config_file)
         conf = config.read(config_file)
     else:
         conf = {}
 
-    if "scrubber_db" not in conf:
-        ctx.fail("You must have a scrubber_db configured in your config file.")
-
     ctx.ensure_object(dict)
     ctx.obj["config"] = conf
-    ctx.obj["db"] = get_scrubber_db(**conf["scrubber_db"])
+    if "scrubber_db" in conf:
+        warnings.warn(
+            "the 'scrubber_db' configuration section has been renamed to 'scrubber'; "
+            f"please update your configuration file {config_file}",
+            DeprecationWarning,
+        )
+        conf["scrubber"] = conf.pop("scrubber_db")
+
+    if "scrubber" not in conf:
+        click.echo(
+            "WARNING: You must have a scrubber configured in your config file.\n"
+        )
+    else:
+        ctx.obj["db"] = get_scrubber_db(**conf["scrubber"])
 
 
 @scrubber_cli_group.group(name="check")
 @click.pass_context
 def scrubber_check_cli_group(ctx):
     """group of commands which read from data stores and report errors."""
     pass
 
 
-@scrubber_check_cli_group.command(name="storage")
+@scrubber_check_cli_group.command(name="init")
 @click.option(
     "--object-type",
     type=click.Choice(
         # use a hardcoded list to prevent having to load the
         # replay module at cli loading time
         [
             "snapshot",
@@ -103,66 +115,216 @@
             "directory",
             # TODO:
             # "raw_extrinsic_metadata",
             # "extid",
         ]
     ),
 )
-@click.option("--start-partition-id", default=0, type=int)
-@click.option("--end-partition-id", default=4096, type=int)
 @click.option("--nb-partitions", default=4096, type=int)
+@click.option("--name", default=None, type=str)
 @click.pass_context
-def scrubber_check_storage(
+def scrubber_check_init(
     ctx,
     object_type: str,
-    start_partition_id: int,
-    end_partition_id: int,
     nb_partitions: int,
+    name: Optional[str],
+):
+    """Initialise a scrubber check configuration for the datastore defined in the
+    configuration file and given object_type.
+
+    A checker configuration configuration consists simply in a set of:
+
+    - object type: the type of object being checked,
+    - number of partitions: the number of partitions the hash space is divided
+      in; must be a power of 2,
+    - name: an unique name for easier reference,
+
+    linked to the storage provided in the configuration file.
+
+    """
+    if not object_type or not name:
+        raise click.ClickException(
+            "Invalid parameters: you must provide the object type and configuration name"
+        )
+
+    conf = ctx.obj["config"]
+    if "storage" not in conf:
+        raise click.ClickException(
+            "You must have a storage configured in your config file."
+        )
+
+    db = ctx.obj["db"]
+    from swh.storage import get_storage
+
+    from .storage_checker import get_datastore
+
+    datastore = get_datastore(storage=get_storage(**conf["storage"]))
+    db.datastore_get_or_add(datastore)
+
+    if db.config_get_by_name(name):
+        raise click.ClickException(f"Configuration {name} already exists")
+
+    config_id = db.config_add(
+        name, datastore, getattr(ObjectType, object_type.upper()), nb_partitions
+    )
+    click.echo(
+        f"Created configuration {name} [{config_id}] for checking {object_type} "
+        f"in {datastore.cls} {datastore.package}"
+    )
+
+
+@scrubber_check_cli_group.command(name="list")
+@click.pass_context
+def scrubber_check_list(
+    ctx,
+):
+    """List the know configurations"""
+    conf = ctx.obj["config"]
+    if "storage" not in conf:
+        ctx.fail("You must have a storage configured in your config file.")
+
+    db = ctx.obj["db"]
+
+    for id_, cfg in db.config_iter():
+        ds = db.datastore_get(cfg.datastore_id)
+        if not ds:
+            click.echo(
+                f"[{id_}] {cfg.name}: Invalid configuration entry; datastore not found"
+            )
+        else:
+            click.echo(
+                f"[{id_}] {cfg.name}: {cfg.object_type}, {cfg.nb_partitions}, "
+                f"{ds.package}:{ds.cls} ({ds.instance})"
+            )
+
+
+@scrubber_check_cli_group.command(name="stalled")
+@click.argument(
+    "name",
+    type=str,
+    default=None,
+    required=False,  # can be given by config_id instead
+)
+@click.option(
+    "--config-id",
+    type=int,
+)
+@click.option(
+    "--for",
+    "delay",
+    type=str,
+    default="auto",
+    help="Delay for a partition to be considered as stuck; in seconds or 'auto'",
+)
+@click.option(
+    "--reset",
+    is_flag=True,
+    default=False,
+    help="Reset the stalled partition so it can be grabbed by a scrubber worker",
+)
+@click.pass_context
+def scrubber_check_stalled(
+    ctx, name: str, config_id: int, delay: Optional[str], reset: bool
+):
+    """List the stuck partitions for a given config"""
+    import datetime
+
+    from humanize import naturaldate, naturaldelta
+
+    db = ctx.obj["db"]
+    if name and config_id is None:
+        config_id = db.config_get_by_name(name)
+
+    if config_id is None:
+        raise click.ClickException("A valid configuration name/id must be set")
+
+    cfg = db.config_get(config_id)
+    delay_td: Optional[datetime.timedelta]
+    if delay == "auto":
+        delay_td = None
+    elif delay:
+        delay_td = datetime.timedelta(seconds=int(delay))
+    in_flight = list(db.checked_partition_get_stuck(config_id, delay_td))
+    if in_flight:
+        click.echo(
+            f"Stuck partitions for {cfg.name} [id={config_id}, type={cfg.object_type}]:"
+        )
+        now = datetime.datetime.now(tz=datetime.timezone.utc)
+        for partition, stuck_since in in_flight:
+            click.echo(
+                f"{partition}:\tstuck since {naturaldate(stuck_since)} "
+                f"({naturaldelta(now-stuck_since)})"
+            )
+            if reset:
+                if db.checked_partition_reset(config_id, partition):
+                    click.echo("\tpartition reset")
+                else:
+                    click.echo("\tpartition NOT reset")
+
+    else:
+        click.echo(
+            f"No stuck partition found for {cfg.name} [id={config_id}, type={cfg.object_type}]"
+        )
+
+
+@scrubber_check_cli_group.command(name="storage")
+@click.argument(
+    "name",
+    type=str,
+    default=None,
+    required=False,  # can be given by config_id instead
+)
+@click.option(
+    "--config-id",
+    type=int,
+)
+@click.option("--limit", default=0, type=int)
+@click.pass_context
+def scrubber_check_storage(
+    ctx,
+    name: str,
+    config_id: int,
+    limit: int,
 ):
     """Reads a swh-storage instance, and reports corrupt objects to the scrubber DB.
 
     This runs a single thread; parallelism is achieved by running this command multiple
-    times, on disjoint ranges.
+    times.
+
+    This command references an existing scrubbing configuration (either by name
+    or by id); the configuration holds the object type, number of partitions
+    and the storage configuration this scrubbing session will check on.
 
     All objects of type ``object_type`` are ordered, and split into the given number
-    of partitions. When running in parallel, the number of partitions should be the
-    same for all workers or they may work on overlapping or non-exhaustive ranges.
+    of partitions.
+
+    Then, this process will check all partitions. The status of the ongoing
+    check session is stored in the database, so the number of concurrent
+    workers can be dynamically adjusted.
 
-    Then, this process will check all partitions in the given
-    ``[start_partition_id, end_partition_id)`` range. When running in parallel, these
-    ranges should be set so that processes over the whole ``[0, nb_partitions)`` range.
-
-    For example in order to have 8 threads checking revisions in parallel and with 64k
-    checkpoints (to recover on crashes), the CLI should be ran 8 times with these
-    parameters::
-
-        --object-type revision --nb-partitions 65536 --start-partition-id 0 --end-partition-id 8192
-        --object-type revision --nb-partitions 65536 --start-partition-id 8192 --end-partition-id 16384
-        --object-type revision --nb-partitions 65536 --start-partition-id 16384 --end-partition-id 24576
-        --object-type revision --nb-partitions 65536 --start-partition-id 24576 --end-partition-id 32768
-        --object-type revision --nb-partitions 65536 --start-partition-id 32768 --end-partition-id 40960
-        --object-type revision --nb-partitions 65536 --start-partition-id 40960 --end-partition-id 49152
-        --object-type revision --nb-partitions 65536 --start-partition-id 49152 --end-partition-id 57344
-        --object-type revision --nb-partitions 65536 --start-partition-id 57344 --end-partition-id 65536
     """  # noqa
     conf = ctx.obj["config"]
     if "storage" not in conf:
         ctx.fail("You must have a storage configured in your config file.")
+    db = ctx.obj["db"]
 
     from swh.storage import get_storage
 
     from .storage_checker import StorageChecker
 
+    if name and config_id is None:
+        config_id = db.config_get_by_name(name)
+
+    if config_id is None:
+        raise click.ClickExceptino("A valid configuration name/id must be set")
     checker = StorageChecker(
         db=ctx.obj["db"],
         storage=get_storage(**conf["storage"]),
-        object_type=object_type,
-        start_partition_id=start_partition_id,
-        end_partition_id=end_partition_id,
-        nb_partitions=nb_partitions,
+        config_id=config_id,
+        limit=limit,
     )
 
     checker.run()
 
 
 @scrubber_check_cli_group.command(name="journal")
 @click.pass_context
```

### Comparing `swh.scrubber-1.0.3/swh/scrubber/db.py` & `swh.scrubber-2.0.0/swh/scrubber/storage_checker.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,540 +1,416 @@
-# Copyright (C) 2022  The Software Heritage developers
+# Copyright (C) 2021-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+"""Reads all objects in a swh-storage instance and recomputes their checksums."""
 
-import dataclasses
-import datetime
-import functools
-from typing import Iterable, Iterator, List, Optional, Tuple
+import collections
+import contextlib
+from itertools import count, islice
+import json
+import logging
+from typing import Iterable, Optional, Tuple, Union
 
 import psycopg2
+import tenacity
 
-from swh.core.db import BaseDb
-from swh.model.swhids import CoreSWHID, ObjectType
-
-
-@dataclasses.dataclass(frozen=True)
-class Datastore:
-    """Represents a datastore being scrubbed; eg. swh-storage or swh-journal."""
-
-    package: str
-    """'storage', 'journal', or 'objstorage'."""
-    cls: str
-    """'postgresql'/'cassandra' for storage, 'kafka' for journal,
-    'pathslicer'/'winery'/... for objstorage."""
-    instance: str
-    """Human readable string."""
-
-
-@dataclasses.dataclass(frozen=True)
-class CorruptObject:
-    id: CoreSWHID
-    datastore: Datastore
-    first_occurrence: datetime.datetime
-    object_: bytes
-
-
-@dataclasses.dataclass(frozen=True)
-class MissingObject:
-    id: CoreSWHID
-    datastore: Datastore
-    first_occurrence: datetime.datetime
-
-
-@dataclasses.dataclass(frozen=True)
-class MissingObjectReference:
-    missing_id: CoreSWHID
-    reference_id: CoreSWHID
-    datastore: Datastore
-    first_occurrence: datetime.datetime
-
-
-@dataclasses.dataclass(frozen=True)
-class FixedObject:
-    id: CoreSWHID
-    object_: bytes
-    method: str
-    recovery_date: Optional[datetime.datetime] = None
-
-
-class ScrubberDb(BaseDb):
-    current_version = 5
-
-    ####################################
-    # Shared tables
-    ####################################
-
-    @functools.lru_cache(1000)
-    def datastore_get_or_add(self, datastore: Datastore) -> int:
-        """Creates a datastore if it does not exist, and returns its id."""
-        with self.transaction() as cur:
-            cur.execute(
-                """
-                WITH inserted AS (
-                    INSERT INTO datastore (package, class, instance)
-                    VALUES (%(package)s, %(cls)s, %(instance)s)
-                    ON CONFLICT DO NOTHING
-                    RETURNING id
-                )
-                SELECT id
-                FROM inserted
-                UNION (
-                    -- If the datastore already exists, we need to fetch its id
-                    SELECT id
-                    FROM datastore
-                    WHERE
-                        package=%(package)s
-                        AND class=%(cls)s
-                        AND instance=%(instance)s
-                )
-                LIMIT 1
-                """,
-                (dataclasses.asdict(datastore)),
-            )
-            res = cur.fetchone()
-            assert res is not None
-            (id_,) = res
-            return id_
-
-    ####################################
-    # Checkpointing/progress tracking
-    ####################################
-
-    def checked_partition_upsert(
-        self,
-        datastore: Datastore,
-        object_type: ObjectType,
-        partition_id: int,
-        nb_partitions: int,
-        date: datetime.datetime,
-    ) -> None:
-        """
-        Records in the database the given partition was last checked at the given date.
-        """
-        datastore_id = self.datastore_get_or_add(datastore)
-        with self.transaction() as cur:
-            cur.execute(
-                """
-                INSERT INTO checked_partition(
-                    datastore, object_type, partition_id, nb_partitions, last_date
-                )
-                VALUES (%s, %s, %s, %s, %s)
-                ON CONFLICT (datastore, object_type, partition_id, nb_partitions)
-                    DO UPDATE
-                    SET last_date = GREATEST(
-                        checked_partition.last_date, EXCLUDED.last_date
-                    )
-                """,
-                (
-                    datastore_id,
-                    object_type.name.lower(),
-                    partition_id,
-                    nb_partitions,
-                    date,
-                ),
-            )
-
-    def checked_partition_get_last_date(
-        self,
-        datastore: Datastore,
-        object_type: ObjectType,
-        partition_id: int,
-        nb_partitions: int,
-    ) -> Optional[datetime.datetime]:
-        """
-        Returns the last date the given partition was checked in the given datastore,
-        or :const:`None` if it was never checked.
-
-        Currently, this matches partition id and number exactly, with no regard for
-        partitions that contain or are contained by it.
+from swh.core.statsd import Statsd
+from swh.journal.serializers import value_to_kafka
+from swh.model import swhids
+from swh.model.model import (
+    Content,
+    Directory,
+    ObjectType,
+    Release,
+    Revision,
+    Snapshot,
+    TargetType,
+)
+from swh.storage.algos.directory import (
+    directory_get_many_with_possibly_duplicated_entries,
+)
+from swh.storage.algos.snapshot import snapshot_get_all_branches
+from swh.storage.cassandra.storage import CassandraStorage
+from swh.storage.interface import StorageInterface
+from swh.storage.postgresql.storage import Storage as PostgresqlStorage
+
+from .db import ConfigEntry, Datastore, ScrubberDb
+
+logger = logging.getLogger(__name__)
+
+ScrubbableObject = Union[Revision, Release, Snapshot, Directory, Content]
+
+
+@contextlib.contextmanager
+def postgresql_storage_db(storage):
+    db = storage.get_db()
+    try:
+        yield db
+    finally:
+        storage.put_db(db)
+
+
+def _get_inclusive_range_swhids(
+    inclusive_range_start: Optional[bytes],
+    exclusive_range_end: Optional[bytes],
+    object_type: swhids.ObjectType,
+) -> Tuple[swhids.CoreSWHID, swhids.CoreSWHID]:
+    r"""
+    Given a ``[range_start, range_end)`` right-open interval of id prefixes
+    and an object type (as returned by :const:`swh.storage.backfill.RANGE_GENERATORS`),
+    returns a ``[range_start_swhid, range_end_swhid]`` closed interval of SWHIDs
+    suitable for the scrubber database.
+
+    >>> _get_inclusive_range_swhids(b"\x42", None, swhids.ObjectType.SNAPSHOT)
+    (CoreSWHID.from_string('swh:1:snp:4200000000000000000000000000000000000000'), CoreSWHID.from_string('swh:1:snp:ffffffffffffffffffffffffffffffffffffffff'))
+
+    >>> _get_inclusive_range_swhids(b"\x00", b"\x12\x34", swhids.ObjectType.REVISION)
+    (CoreSWHID.from_string('swh:1:rev:0000000000000000000000000000000000000000'), CoreSWHID.from_string('swh:1:rev:1233ffffffffffffffffffffffffffffffffffff'))
+
+    """  # noqa
+    range_start_swhid = swhids.CoreSWHID(
+        object_type=object_type,
+        object_id=(inclusive_range_start or b"").ljust(20, b"\00"),
+    )
+    if exclusive_range_end is None:
+        inclusive_range_end = b"\xff" * 20
+    else:
+        # convert "1230000000..." to "122fffffff..."
+        inclusive_range_end = (
+            int.from_bytes(exclusive_range_end.ljust(20, b"\x00"), "big") - 1
+        ).to_bytes(20, "big")
+    range_end_swhid = swhids.CoreSWHID(
+        object_type=object_type,
+        object_id=inclusive_range_end,
+    )
+
+    return (range_start_swhid, range_end_swhid)
+
+
+def get_datastore(storage) -> Datastore:
+    if isinstance(storage, PostgresqlStorage):
+        with postgresql_storage_db(storage) as db:
+            datastore = Datastore(
+                package="storage",
+                cls="postgresql",
+                instance=db.conn.dsn,
+            )
+    elif isinstance(storage, CassandraStorage):
+        datastore = Datastore(
+            package="storage",
+            cls="cassandra",
+            instance=json.dumps(
+                {
+                    "keyspace": storage.keyspace,
+                    "hosts": storage.hosts,
+                    "port": storage.port,
+                }
+            ),
+        )
+    else:
+        raise NotImplementedError(f"StorageChecker(storage={storage!r}).datastore()")
+    return datastore
+
+
+class StorageChecker:
+    """Reads a chunk of a swh-storage database, recomputes checksums, and
+    reports errors in a separate database."""
+
+    def __init__(
+        self, db: ScrubberDb, config_id: int, storage: StorageInterface, limit: int = 0
+    ):
+        self.db = db
+        self.storage = storage
+        self.config_id = config_id
+        self.limit = limit
+
+        self._config: Optional[ConfigEntry] = None
+        self._datastore: Optional[Datastore] = None
+        self._statsd: Optional[Statsd] = None
+
+    @property
+    def config(self) -> ConfigEntry:
+        if self._config is None:
+            self._config = self.db.config_get(self.config_id)
+
+        assert self._config is not None
+        return self._config
+
+    @property
+    def nb_partitions(self) -> int:
+        return self.config.nb_partitions
+
+    @property
+    def object_type(self) -> str:
+        return self.config.object_type
+
+    @property
+    def datastore(self) -> Datastore:
+        """Returns a :class:`Datastore` instance representing the swh-storage instance
+        being checked."""
+        if self._datastore is None:
+            self._datastore = get_datastore(self.storage)
+            datastore_id = self.db.datastore_get_or_add(self._datastore)
+            assert self.config.datastore_id == datastore_id
+        return self._datastore
+
+    @property
+    def statsd(self) -> Statsd:
+        if self._statsd is None:
+            self._statsd = Statsd(
+                namespace="swh_scrubber",
+                constant_tags={
+                    "object_type": self.object_type,
+                    "nb_partitions": self.nb_partitions,
+                    "datastore_package": self.datastore.package,
+                    "datastore_cls": self.datastore.cls,
+                },
+            )
+        return self._statsd
+
+    def run(self) -> None:
+        """Runs on all objects of ``object_type`` in a partition between
+        ``start_partition_id`` (inclusive) and ``end_partition_id`` (exclusive)
         """
-        datastore_id = self.datastore_get_or_add(datastore)
-        with self.transaction() as cur:
-            cur.execute(
-                """
-                SELECT last_date
-                FROM checked_partition
-                WHERE datastore=%s AND object_type=%s AND partition_id=%s AND nb_partitions=%s
-                """,
-                (datastore_id, object_type.name.lower(), partition_id, nb_partitions),
-            )
-
-            res = cur.fetchone()
-            if res is None:
-                return None
-            else:
-                (date,) = res
-                return date
-
-    def checked_partition_iter(
-        self, datastore: Datastore
-    ) -> Iterator[Tuple[ObjectType, int, int, datetime.datetime]]:
-        """Yields tuples of ``(partition_id, nb_partitions, last_date)``"""
-        datastore_id = self.datastore_get_or_add(datastore)
-        with self.transaction() as cur:
-            cur.execute(
-                """
-                SELECT object_type, partition_id, nb_partitions, last_date
-                FROM checked_partition
-                WHERE datastore=%s
-                """,
-                (datastore_id,),
-            )
-
-            for (object_type, *rest) in cur:
-                yield (getattr(ObjectType, object_type.upper()), *rest)  # type: ignore[misc]
-
-    ####################################
-    # Inventory of objects with issues
-    ####################################
-
-    def corrupt_object_add(
-        self,
-        id: CoreSWHID,
-        datastore: Datastore,
-        serialized_object: bytes,
+        object_type = getattr(swhids.ObjectType, self.object_type.upper())
+        counter: Iterable[int] = count()
+        if self.limit:
+            counter = islice(counter, 0, self.limit)
+        for i, partition_id in zip(
+            counter, self.db.checked_partition_iter_next(self.config_id)
+        ):
+            logger.debug(
+                "Processing %s partition %d/%d",
+                self.object_type,
+                partition_id,
+                self.nb_partitions,
+            )
+
+            self._check_partition(object_type, partition_id)
+
+            self.db.checked_partition_upsert(
+                self.config_id,
+                partition_id,
+            )
+
+    @tenacity.retry(
+        retry=tenacity.retry_if_exception_type(psycopg2.OperationalError),
+        wait=tenacity.wait_random_exponential(min=10, max=180),
+    )
+    def _check_partition(
+        self, object_type: swhids.ObjectType, partition_id: int
     ) -> None:
-        datastore_id = self.datastore_get_or_add(datastore)
-        with self.transaction() as cur:
-            cur.execute(
-                """
-                INSERT INTO corrupt_object (id, datastore, object)
-                VALUES (%s, %s, %s)
-                ON CONFLICT DO NOTHING
-                """,
-                (str(id), datastore_id, serialized_object),
-            )
-
-    def corrupt_object_iter(self) -> Iterator[CorruptObject]:
-        """Yields all records in the 'corrupt_object' table."""
-        with self.transaction() as cur:
-            cur.execute(
-                """
-                SELECT
-                    co.id, co.first_occurrence, co.object,
-                    ds.package, ds.class, ds.instance
-                FROM corrupt_object AS co
-                INNER JOIN datastore AS ds ON (ds.id=co.datastore)
-                """
-            )
-
-            for row in cur:
-                (id, first_occurrence, object_, ds_package, ds_class, ds_instance) = row
-                yield CorruptObject(
-                    id=CoreSWHID.from_string(id),
-                    first_occurrence=first_occurrence,
-                    object_=object_,
-                    datastore=Datastore(
-                        package=ds_package, cls=ds_class, instance=ds_instance
-                    ),
+        page_token = None
+        while True:
+            if object_type in (swhids.ObjectType.RELEASE, swhids.ObjectType.REVISION):
+                method = getattr(self.storage, f"{self.object_type}_get_partition")
+                page = method(partition_id, self.nb_partitions, page_token=page_token)
+                objects = page.results
+            elif object_type == swhids.ObjectType.DIRECTORY:
+                page = self.storage.directory_get_id_partition(
+                    partition_id, self.nb_partitions, page_token=page_token
                 )
-
-    def _corrupt_object_list_from_cursor(
-        self, cur: psycopg2.extensions.cursor
-    ) -> List[CorruptObject]:
-        results = []
-        for row in cur:
-            (id, first_occurrence, object_, ds_package, ds_class, ds_instance) = row
-            results.append(
-                CorruptObject(
-                    id=CoreSWHID.from_string(id),
-                    first_occurrence=first_occurrence,
-                    object_=object_,
-                    datastore=Datastore(
-                        package=ds_package, cls=ds_class, instance=ds_instance
+                directory_ids = page.results
+                objects = []
+                for (dir_id, item) in zip(
+                    directory_ids,
+                    directory_get_many_with_possibly_duplicated_entries(
+                        self.storage, directory_ids
                     ),
+                ):
+                    assert item is not None, f"Directory {dir_id.hex()} disappeared"
+                    (has_duplicate_entries, object_) = item
+                    if has_duplicate_entries:
+                        self.statsd.increment("duplicate_directory_entries_total")
+                        self.db.corrupt_object_add(
+                            object_.swhid(),
+                            self.datastore,
+                            value_to_kafka(object_.to_dict()),
+                        )
+                    objects.append(object_)
+            elif object_type == swhids.ObjectType.SNAPSHOT:
+                page = self.storage.snapshot_get_id_partition(
+                    partition_id, self.nb_partitions, page_token=page_token
                 )
-            )
-
-        return results
-
-    def corrupt_object_get(
-        self,
-        start_id: CoreSWHID,
-        end_id: CoreSWHID,
-        limit: int = 100,
-    ) -> List[CorruptObject]:
-        """Yields a page of records in the 'corrupt_object' table, ordered by id.
-
-        Arguments:
-            start_id: Only return objects after this id
-            end_id: Only return objects before this id
-            in_origin: An origin URL. If provided, only returns objects that may be
-                found in the given origin
-        """
-        with self.transaction() as cur:
-            cur.execute(
-                """
-                SELECT
-                    co.id, co.first_occurrence, co.object,
-                    ds.package, ds.class, ds.instance
-                FROM corrupt_object AS co
-                INNER JOIN datastore AS ds ON (ds.id=co.datastore)
-                WHERE
-                    co.id >= %s
-                    AND co.id <= %s
-                ORDER BY co.id
-                LIMIT %s
-                """,
-                (str(start_id), str(end_id), limit),
-            )
-            return self._corrupt_object_list_from_cursor(cur)
-
-    def corrupt_object_grab_by_id(
-        self,
-        cur: psycopg2.extensions.cursor,
-        start_id: CoreSWHID,
-        end_id: CoreSWHID,
-        limit: int = 100,
-    ) -> List[CorruptObject]:
-        """Returns a page of records in the 'corrupt_object' table for a fixer,
-        ordered by id
-
-        These records are not already fixed (ie. do not have a corresponding entry
-        in the 'fixed_object' table), and they are selected with an exclusive update
-        lock.
-
-        Arguments:
-            start_id: Only return objects after this id
-            end_id: Only return objects before this id
-        """
-        cur.execute(
-            """
-            SELECT
-                co.id, co.first_occurrence, co.object,
-                ds.package, ds.class, ds.instance
-            FROM corrupt_object AS co
-            INNER JOIN datastore AS ds ON (ds.id=co.datastore)
-            WHERE
-                co.id >= %(start_id)s
-                AND co.id <= %(end_id)s
-                AND NOT EXISTS (SELECT 1 FROM fixed_object WHERE fixed_object.id=co.id)
-            ORDER BY co.id
-            LIMIT %(limit)s
-            FOR UPDATE SKIP LOCKED
-            """,
-            dict(
-                start_id=str(start_id),
-                end_id=str(end_id),
-                limit=limit,
-            ),
-        )
-        return self._corrupt_object_list_from_cursor(cur)
-
-    def corrupt_object_grab_by_origin(
-        self,
-        cur: psycopg2.extensions.cursor,
-        origin_url: str,
-        start_id: Optional[CoreSWHID] = None,
-        end_id: Optional[CoreSWHID] = None,
-        limit: int = 100,
-    ) -> List[CorruptObject]:
-        """Returns a page of records in the 'corrupt_object' table for a fixer,
-        ordered by id
-
-        These records are not already fixed (ie. do not have a corresponding entry
-        in the 'fixed_object' table), and they are selected with an exclusive update
-        lock.
-
-        Arguments:
-            origin_url: only returns objects that may be found in the given origin
-        """
-        cur.execute(
-            """
-            SELECT
-                co.id, co.first_occurrence, co.object,
-                ds.package, ds.class, ds.instance
-            FROM corrupt_object AS co
-            INNER JOIN datastore AS ds ON (ds.id=co.datastore)
-            INNER JOIN object_origin AS oo ON (oo.object_id=co.id)
-            WHERE
-                (co.id >= %(start_id)s OR %(start_id)s IS NULL)
-                AND (co.id <= %(end_id)s OR %(end_id)s IS NULL)
-                AND NOT EXISTS (SELECT 1 FROM fixed_object WHERE fixed_object.id=co.id)
-                AND oo.origin_url=%(origin_url)s
-            ORDER BY co.id
-            LIMIT %(limit)s
-            FOR UPDATE SKIP LOCKED
-            """,
-            dict(
-                start_id=None if start_id is None else str(start_id),
-                end_id=None if end_id is None else str(end_id),
-                origin_url=origin_url,
-                limit=limit,
-            ),
-        )
-        return self._corrupt_object_list_from_cursor(cur)
-
-    def missing_object_add(
-        self,
-        id: CoreSWHID,
-        reference_ids: Iterable[CoreSWHID],
-        datastore: Datastore,
-    ) -> None:
-        """
-        Adds a "hole" to the inventory, ie. an object missing from a datastore
-        that is referenced by an other object of the same datastore.
+                snapshot_ids = page.results
+                objects = [
+                    snapshot_get_all_branches(self.storage, snapshot_id)
+                    for snapshot_id in snapshot_ids
+                ]
+            else:
+                assert False, f"Unexpected object type: {object_type}"
 
-        If the missing object is already known to be missing by the scrubber database,
-        this only records the reference (which can be useful to locate an origin
-        to recover the object from).
-        If that reference is already known too, this is a noop.
-
-        Args:
-            id: SWHID of the missing object (the hole)
-            reference_id: SWHID of the object referencing the missing object
-            datastore: representation of the swh-storage/swh-journal/... instance
-              containing this hole
-        """
-        if not reference_ids:
-            raise ValueError("reference_ids is empty")
-        datastore_id = self.datastore_get_or_add(datastore)
-        with self.transaction() as cur:
-            cur.execute(
-                """
-                INSERT INTO missing_object (id, datastore)
-                VALUES (%s, %s)
-                ON CONFLICT DO NOTHING
-                """,
-                (str(id), datastore_id),
-            )
-            psycopg2.extras.execute_batch(
-                cur,
-                """
-                INSERT INTO missing_object_reference (missing_id, reference_id, datastore)
-                VALUES (%s, %s, %s)
-                ON CONFLICT DO NOTHING
-                """,
-                [
-                    (str(id), str(reference_id), datastore_id)
-                    for reference_id in reference_ids
-                ],
-            )
-
-    def missing_object_iter(self) -> Iterator[MissingObject]:
-        """Yields all records in the 'missing_object' table."""
-        with self.transaction() as cur:
-            cur.execute(
-                """
-                SELECT
-                    mo.id, mo.first_occurrence,
-                    ds.package, ds.class, ds.instance
-                FROM missing_object AS mo
-                INNER JOIN datastore AS ds ON (ds.id=mo.datastore)
-                """
-            )
-
-            for row in cur:
-                (id, first_occurrence, ds_package, ds_class, ds_instance) = row
-                yield MissingObject(
-                    id=CoreSWHID.from_string(id),
-                    first_occurrence=first_occurrence,
-                    datastore=Datastore(
-                        package=ds_package, cls=ds_class, instance=ds_instance
-                    ),
+            with self.statsd.timed(
+                "batch_duration_seconds", tags={"operation": "check_hashes"}
+            ):
+                logger.debug("Checking %s %s object hashes", len(objects), object_type)
+                self.check_object_hashes(objects)
+            with self.statsd.timed(
+                "batch_duration_seconds", tags={"operation": "check_references"}
+            ):
+                logger.debug(
+                    "Checking %s %s object references", len(objects), object_type
                 )
+                self.check_object_references(objects)
 
-    def missing_object_reference_iter(
-        self, missing_id: CoreSWHID
-    ) -> Iterator[MissingObjectReference]:
-        """Yields all records in the 'missing_object_reference' table."""
-        with self.transaction() as cur:
-            cur.execute(
-                """
-                SELECT
-                    mor.reference_id, mor.first_occurrence,
-                    ds.package, ds.class, ds.instance
-                FROM missing_object_reference AS mor
-                INNER JOIN datastore AS ds ON (ds.id=mor.datastore)
-                WHERE mor.missing_id=%s
-                """,
-                (str(missing_id),),
-            )
-
-            for row in cur:
-                (
-                    reference_id,
-                    first_occurrence,
-                    ds_package,
-                    ds_class,
-                    ds_instance,
-                ) = row
-                yield MissingObjectReference(
-                    missing_id=missing_id,
-                    reference_id=CoreSWHID.from_string(reference_id),
-                    first_occurrence=first_occurrence,
-                    datastore=Datastore(
-                        package=ds_package, cls=ds_class, instance=ds_instance
-                    ),
+            page_token = page.next_page_token
+            if page_token is None:
+                break
+
+    def check_object_hashes(self, objects: Iterable[ScrubbableObject]):
+        """Recomputes hashes, and reports mismatches."""
+        count = 0
+        for object_ in objects:
+            if isinstance(object_, Content):
+                # TODO
+                continue
+            real_id = object_.compute_hash()
+            count += 1
+            if object_.id != real_id:
+                self.statsd.increment("hash_mismatch_total")
+                self.db.corrupt_object_add(
+                    object_.swhid(),
+                    self.datastore,
+                    value_to_kafka(object_.to_dict()),
                 )
+        if count:
+            self.statsd.increment("objects_hashed_total", count)
 
-    ####################################
-    # Issue resolution
-    ####################################
+    def check_object_references(self, objects: Iterable[ScrubbableObject]):
+        """Check all objects references by these objects exist."""
+        cnt_references = collections.defaultdict(set)
+        dir_references = collections.defaultdict(set)
+        rev_references = collections.defaultdict(set)
+        rel_references = collections.defaultdict(set)
+        snp_references = collections.defaultdict(set)
+
+        for object_ in objects:
+            swhid = object_.swhid()
+
+            if isinstance(object_, Content):
+                pass
+            elif isinstance(object_, Directory):
+                for entry in object_.entries:
+                    if entry.type == "file":
+                        cnt_references[entry.target].add(swhid)
+                    elif entry.type == "dir":
+                        dir_references[entry.target].add(swhid)
+                    elif entry.type == "rev":
+                        # dir->rev holes are not considered a problem because they
+                        # happen whenever git submodules point to repositories that
+                        # were not loaded yet; ignore them
+                        pass
+                    else:
+                        assert False, entry
+            elif isinstance(object_, Revision):
+                dir_references[object_.directory].add(swhid)
+                for parent in object_.parents:
+                    rev_references[parent].add(swhid)
+            elif isinstance(object_, Release):
+                if object_.target is None:
+                    pass
+                elif object_.target_type == ObjectType.CONTENT:
+                    cnt_references[object_.target].add(swhid)
+                elif object_.target_type == ObjectType.DIRECTORY:
+                    dir_references[object_.target].add(swhid)
+                elif object_.target_type == ObjectType.REVISION:
+                    rev_references[object_.target].add(swhid)
+                elif object_.target_type == ObjectType.RELEASE:
+                    rel_references[object_.target].add(swhid)
+                else:
+                    assert False, object_
+            elif isinstance(object_, Snapshot):
+                for branch in object_.branches.values():
+                    if branch is None:
+                        pass
+                    elif branch.target_type == TargetType.ALIAS:
+                        pass
+                    elif branch.target_type == TargetType.CONTENT:
+                        cnt_references[branch.target].add(swhid)
+                    elif branch.target_type == TargetType.DIRECTORY:
+                        dir_references[branch.target].add(swhid)
+                    elif branch.target_type == TargetType.REVISION:
+                        rev_references[branch.target].add(swhid)
+                    elif branch.target_type == TargetType.RELEASE:
+                        rel_references[branch.target].add(swhid)
+                    elif branch.target_type == TargetType.SNAPSHOT:
+                        snp_references[branch.target].add(swhid)
+                    else:
+                        assert False, (str(object_.swhid()), branch)
+            else:
+                assert False, object_.swhid()
 
-    def object_origin_add(
-        self, cur: psycopg2.extensions.cursor, swhid: CoreSWHID, origins: List[str]
-    ) -> None:
-        psycopg2.extras.execute_values(
-            cur,
-            """
-            INSERT INTO object_origin (object_id, origin_url)
-            VALUES %s
-            ON CONFLICT DO NOTHING
-            """,
-            [(str(swhid), origin_url) for origin_url in origins],
+        missing_cnts = set(
+            self.storage.content_missing_per_sha1_git(list(cnt_references))
+        )
+        missing_dirs = set(self.storage.directory_missing(list(dir_references)))
+        missing_revs = set(self.storage.revision_missing(list(rev_references)))
+        missing_rels = set(self.storage.release_missing(list(rel_references)))
+        missing_snps = set(self.storage.snapshot_missing(list(snp_references)))
+
+        self.statsd.increment(
+            "missing_object_total",
+            len(missing_cnts),
+            tags={"target_object_type": "content"},
+        )
+        self.statsd.increment(
+            "missing_object_total",
+            len(missing_dirs),
+            tags={"target_object_type": "directory"},
+        )
+        self.statsd.increment(
+            "missing_object_total",
+            len(missing_revs),
+            tags={"target_object_type": "revision"},
+        )
+        self.statsd.increment(
+            "missing_object_total",
+            len(missing_rels),
+            tags={"target_object_type": "release"},
+        )
+        self.statsd.increment(
+            "missing_object_total",
+            len(missing_snps),
+            tags={"target_object_type": "snapshot"},
         )
 
-    def object_origin_get(self, after: str = "", limit: int = 1000) -> List[str]:
-        """Returns origins with non-fixed corrupt objects, ordered by URL.
+        for missing_id in missing_cnts:
+            missing_swhid = swhids.CoreSWHID(
+                object_type=swhids.ObjectType.CONTENT, object_id=missing_id
+            )
+            self.db.missing_object_add(
+                missing_swhid, cnt_references[missing_id], self.datastore
+            )
 
-        Arguments:
-            after: if given, only returns origins with an URL after this value
-        """
-        with self.transaction() as cur:
-            cur.execute(
-                """
-                SELECT DISTINCT origin_url
-                FROM object_origin
-                WHERE
-                    origin_url > %(after)s
-                    AND object_id IN (
-                        (SELECT id FROM corrupt_object)
-                        EXCEPT (SELECT id FROM fixed_object)
-                    )
-                ORDER BY origin_url
-                LIMIT %(limit)s
-                """,
-                dict(after=after, limit=limit),
+        for missing_id in missing_dirs:
+            missing_swhid = swhids.CoreSWHID(
+                object_type=swhids.ObjectType.DIRECTORY, object_id=missing_id
+            )
+            self.db.missing_object_add(
+                missing_swhid, dir_references[missing_id], self.datastore
             )
 
-            return [origin_url for (origin_url,) in cur]
+        for missing_id in missing_revs:
+            missing_swhid = swhids.CoreSWHID(
+                object_type=swhids.ObjectType.REVISION, object_id=missing_id
+            )
+            self.db.missing_object_add(
+                missing_swhid, rev_references[missing_id], self.datastore
+            )
 
-    def fixed_object_add(
-        self, cur: psycopg2.extensions.cursor, fixed_objects: List[FixedObject]
-    ) -> None:
-        psycopg2.extras.execute_values(
-            cur,
-            """
-            INSERT INTO fixed_object (id, object, method)
-            VALUES %s
-            ON CONFLICT DO NOTHING
-            """,
-            [
-                (str(fixed_object.id), fixed_object.object_, fixed_object.method)
-                for fixed_object in fixed_objects
-            ],
-        )
+        for missing_id in missing_rels:
+            missing_swhid = swhids.CoreSWHID(
+                object_type=swhids.ObjectType.RELEASE, object_id=missing_id
+            )
+            self.db.missing_object_add(
+                missing_swhid, rel_references[missing_id], self.datastore
+            )
 
-    def fixed_object_iter(self) -> Iterator[FixedObject]:
-        with self.transaction() as cur:
-            cur.execute("SELECT id, object, method, recovery_date FROM fixed_object")
-            for (id, object_, method, recovery_date) in cur:
-                yield FixedObject(
-                    id=CoreSWHID.from_string(id),
-                    object_=object_,
-                    method=method,
-                    recovery_date=recovery_date,
-                )
+        for missing_id in missing_snps:
+            missing_swhid = swhids.CoreSWHID(
+                object_type=swhids.ObjectType.SNAPSHOT, object_id=missing_id
+            )
+            self.db.missing_object_add(
+                missing_swhid, snp_references[missing_id], self.datastore
+            )
```

### Comparing `swh.scrubber-1.0.3/swh/scrubber/fixer.py` & `swh.scrubber-2.0.0/swh/scrubber/fixer.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/journal_checker.py` & `swh.scrubber-2.0.0/swh/scrubber/journal_checker.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/origin_locator.py` & `swh.scrubber-2.0.0/swh/scrubber/origin_locator.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/sql/30-schema.sql` & `swh.scrubber-2.0.0/swh/scrubber/sql/30-schema.sql`

 * *Files 17% similar despite different names*

```diff
@@ -2,45 +2,63 @@
 -- Shared definitions
 -------------------------------------
 
 create domain swhid as text check (value ~ '^swh:[0-9]+:.*');
 
 create table datastore
 (
-  id                bigserial not null,
+  id                serial not null,
   package           datastore_type not null,
   class             text,
   instance          text
 );
 
 comment on table datastore is 'Each row identifies a data store being scrubbed';
 comment on column datastore.id is 'Internal identifier of the datastore';
 comment on column datastore.package is 'Name of the component using this datastore (storage/journal/objstorage)';
 comment on column datastore.class is 'For datastores with multiple backends, name of the backend (postgresql/cassandra for storage, kafka for journal, pathslicer/azure/winery/... for objstorage)';
 comment on column datastore.instance is 'Human-readable way to uniquely identify the datastore; eg. its URL or DSN.';
 
 
 -------------------------------------
--- Checkpointing/progress tracking
+-- Checker configuration
 -------------------------------------
 
-create table checked_partition
+create table check_config
 (
+  id					serial not null,
   datastore             int not null,
   object_type           object_type not null,
-  partition_id          bigint not null,
   nb_partitions         bigint not null,
-  last_date             timestamptz not null
+  name                  text,
+  comment               text
+);
+
+comment on table check_config is 'Configuration of a checker for a given object type from a given datastore.';
+comment on column check_config.datastore is 'The datastore this checker config is about.';
+comment on column check_config.object_type is 'The type of checked objects.';
+comment on column check_config.nb_partitions is 'Number of partitions the set of objects is split into.';
+
+-------------------------------------
+-- Checkpointing/progress tracking
+-------------------------------------
+
+create table checked_partition
+(
+  config_id             int not null,
+  partition_id          bigint not null,
+  start_date            timestamptz,
+  end_date              timestamptz
 );
 
-comment on table checked_partition is 'Each row represents a range of objects in a datastore that were fetched, checksummed, and checked at some point in the past. The whole set of objects of the given type is split into nb_partitions and partition_id is a value from 0 to nb_partitions-1.';
-comment on column checked_partition.object_type is 'The type of tested objects.';
+comment on table checked_partition is 'Each row represents a range of objects in a datastore that were fetched, checksummed, and checked at some point in the past. The whole set of objects of the given type is split into config.nb_partitions and partition_id is a value from 0 to config.nb_partitions-1.';
+comment on column checked_partition.config_id is 'The check configuration this partition concerns.';
 comment on column checked_partition.partition_id is 'Index of the partition to fetch';
-comment on column checked_partition.nb_partitions is 'Number of partitions the set of objects is split into.';
-comment on column checked_partition.last_date is 'Date the last scrub of this partition *started*.';
+comment on column checked_partition.start_date is 'Date the last scrub started for this partition.';
+comment on column checked_partition.end_date is 'Date the last scrub ended of this partition.';
 
 -------------------------------------
 -- Inventory of objects with issues
 -------------------------------------
 
 create table corrupt_object
 (
```

### Comparing `swh.scrubber-1.0.3/swh/scrubber/sql/60-indexes.sql` & `swh.scrubber-2.0.0/swh/scrubber/sql/60-indexes.sql`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,73 @@
 -------------------------------------
 -- Shared tables
 -------------------------------------
 
 -- datastore
 
-create unique index concurrently datastore_pkey on datastore(id);
+create unique index datastore_pkey on datastore(id);
 alter table datastore add primary key using index datastore_pkey;
 
-create unique index concurrently datastore_package_class_instance on datastore(package, class, instance);
+create unique index datastore_package_class_instance on datastore(package, class, instance);
+
+-------------------------------------
+-- Checker config
+-------------------------------------
+
+create unique index check_config_pkey on check_config(id);
+create unique index check_config_unicity_idx on check_config(datastore, object_type, nb_partitions);
+alter table check_config add primary key using index check_config_pkey;
 
 -------------------------------------
 -- Checkpointing/progress tracking
 -------------------------------------
 
-create unique index concurrently checked_partition_pkey on checked_partition(datastore, object_type, nb_partitions, partition_id);
+create unique index checked_partition_pkey on checked_partition(config_id, partition_id);
 alter table checked_partition add primary key using index checked_partition_pkey;
 
 -------------------------------------
 -- Inventory of objects with issues
 -------------------------------------
 
 -- corrupt_object
 
 alter table corrupt_object add constraint corrupt_object_datastore_fkey foreign key (datastore) references datastore(id) not valid;
 alter table corrupt_object validate constraint corrupt_object_datastore_fkey;
 
-create unique index concurrently corrupt_object_pkey on corrupt_object(id, datastore);
+create unique index corrupt_object_pkey on corrupt_object(id, datastore);
 alter table corrupt_object add primary key using index corrupt_object_pkey;
 
 
 -- missing_object
 
 alter table missing_object add constraint missing_object_datastore_fkey foreign key (datastore) references datastore(id) not valid;
 alter table missing_object validate constraint missing_object_datastore_fkey;
 
-create unique index concurrently missing_object_pkey on missing_object(id, datastore);
+create unique index missing_object_pkey on missing_object(id, datastore);
 alter table missing_object add primary key using index missing_object_pkey;
 
 
 -- missing_object_reference
 
 alter table missing_object_reference add constraint missing_object_reference_datastore_fkey foreign key (datastore) references datastore(id) not valid;
 alter table missing_object_reference validate constraint missing_object_reference_datastore_fkey;
 
-create unique index concurrently missing_object_reference_missing_id_reference_id_datastore on missing_object_reference(missing_id, reference_id, datastore);
-create unique index concurrently missing_object_reference_reference_id_missing_id_datastore on missing_object_reference(reference_id, missing_id, datastore);
+create unique index missing_object_reference_missing_id_reference_id_datastore on missing_object_reference(missing_id, reference_id, datastore);
+create unique index missing_object_reference_reference_id_missing_id_datastore on missing_object_reference(reference_id, missing_id, datastore);
 
 -------------------------------------
 -- Issue resolution
 -------------------------------------
 
 -- object_origin
 
-create unique index concurrently object_origin_pkey on object_origin (object_id, origin_url);
-create index concurrently object_origin_by_origin on object_origin (origin_url, object_id);
+create unique index object_origin_pkey on object_origin (object_id, origin_url);
+create index object_origin_by_origin on object_origin (origin_url, object_id);
 
 -- FIXME: not valid, because corrupt_object(id) is not unique
 -- alter table object_origin add constraint object_origin_object_fkey foreign key (object_id) references corrupt_object(id) not valid;
 -- alter table object_origin validate constraint object_origin_object_fkey;
 
 -- fixed_object
 
-create unique index concurrently fixed_object_pkey on fixed_object(id);
+create unique index fixed_object_pkey on fixed_object(id);
 alter table fixed_object add primary key using index fixed_object_pkey;
```

### Comparing `swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/2.sql` & `swh.scrubber-2.0.0/swh/scrubber/sql/upgrades/2.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/3.sql` & `swh.scrubber-2.0.0/swh/scrubber/sql/upgrades/3.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/4.sql` & `swh.scrubber-2.0.0/swh/scrubber/sql/upgrades/4.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/5.sql` & `swh.scrubber-2.0.0/swh/scrubber/sql/upgrades/5.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/tests/storage_checker_tests.py` & `swh.scrubber-2.0.0/swh/scrubber/tests/storage_checker_tests.py`

 * *Files 21% similar despite different names*

```diff
@@ -60,74 +60,91 @@
 EXPECTED_PARTITIONS = {
     (swhids.ObjectType.SNAPSHOT, 0, 1),
     (swhids.ObjectType.DIRECTORY, 0, 1),
     (swhids.ObjectType.REVISION, 0, 1),
     (swhids.ObjectType.RELEASE, 0, 1),
 }
 
+OBJECT_TYPES = (
+    swhids.ObjectType.SNAPSHOT,
+    swhids.ObjectType.DIRECTORY,
+    swhids.ObjectType.REVISION,
+    swhids.ObjectType.RELEASE,
+)
+
 
 def assert_checked_ranges(
-    scrubber_db, datastore, expected_ranges, before_date=None, after_date=None
+    scrubber_db, config, expected_ranges, before_date=None, after_date=None
 ):
-    if before_date is not None:
-        assert all(
-            before_date < date < after_date
-            for (_, _, _, date) in scrubber_db.checked_partition_iter(datastore)
-        )
+    checked_ranges = set()
+    for object_type, config_id in config:
+        if before_date is not None:
+            assert all(
+                before_date < date < after_date
+                for (_, _, date, _) in scrubber_db.checked_partition_iter(config_id)
+            )
 
-    checked_ranges = {
-        (object_type, start, end)
-        for (object_type, start, end, date) in scrubber_db.checked_partition_iter(
-            datastore
+        checked_ranges.update(
+            {
+                (object_type, partition, nb_partitions)
+                for (
+                    partition,
+                    nb_partitions,
+                    start_date,
+                    end_date,
+                ) in scrubber_db.checked_partition_iter(config_id)
+            }
         )
-    }
-
     assert checked_ranges == expected_ranges
 
 
 def test_no_corruption(scrubber_db, datastore, swh_storage):
     swh_storage.directory_add(swh_model_data.DIRECTORIES)
     swh_storage.revision_add(swh_model_data.REVISIONS)
     swh_storage.release_add(swh_model_data.RELEASES)
     swh_storage.snapshot_add(swh_model_data.SNAPSHOTS)
 
     before_date = datetime.datetime.now(tz=datetime.timezone.utc)
-    for object_type in ("snapshot", "release", "revision", "directory"):
+    config = []
+    for object_type in OBJECT_TYPES:
+        config_id = scrubber_db.config_add(
+            f"cfg_{object_type.name}", datastore, object_type, 1
+        )
+        config.append((object_type, config_id))
         StorageChecker(
             db=scrubber_db,
             storage=swh_storage,
-            object_type=object_type,
-            start_partition_id=0,
-            end_partition_id=1,
-            nb_partitions=1,
+            config_id=config_id,
         ).run()
     after_date = datetime.datetime.now(tz=datetime.timezone.utc)
 
     assert list(scrubber_db.corrupt_object_iter()) == []
 
     assert_checked_ranges(
-        scrubber_db, datastore, EXPECTED_PARTITIONS, before_date, after_date
+        scrubber_db, config, EXPECTED_PARTITIONS, before_date, after_date
     )
 
 
 @pytest.mark.parametrize("corrupt_idx", range(len(swh_model_data.SNAPSHOTS)))
 def test_corrupt_snapshot(scrubber_db, datastore, swh_storage, corrupt_idx):
     snapshots = list(swh_model_data.SNAPSHOTS)
     snapshots[corrupt_idx] = attr.evolve(snapshots[corrupt_idx], id=b"\x00" * 20)
     swh_storage.snapshot_add(snapshots)
 
     before_date = datetime.datetime.now(tz=datetime.timezone.utc)
-    for object_type in ("snapshot", "release", "revision", "directory"):
+    config = []
+    for object_type in OBJECT_TYPES:
+        config_id = scrubber_db.config_add(
+            f"cfg_{object_type.name}", datastore, object_type, 1
+        )
+        config.append((object_type, config_id))
         StorageChecker(
             db=scrubber_db,
             storage=swh_storage,
-            object_type=object_type,
-            start_partition_id=0,
-            end_partition_id=1,
-            nb_partitions=1,
+            config_id=config_id,
         ).run()
     after_date = datetime.datetime.now(tz=datetime.timezone.utc)
 
     corrupt_objects = list(scrubber_db.corrupt_object_iter())
     assert len(corrupt_objects) == 1
     assert corrupt_objects[0].id == swhids.CoreSWHID.from_string(
         "swh:1:snp:0000000000000000000000000000000000000000"
@@ -139,92 +156,92 @@
         <= after_date + datetime.timedelta(seconds=5)
     )
     assert (
         kafka_to_value(corrupt_objects[0].object_) == snapshots[corrupt_idx].to_dict()
     )
 
     assert_checked_ranges(
-        scrubber_db, datastore, EXPECTED_PARTITIONS, before_date, after_date
+        scrubber_db, config, EXPECTED_PARTITIONS, before_date, after_date
     )
 
 
 def test_corrupt_snapshots_same_batch(scrubber_db, datastore, swh_storage):
     snapshots = list(swh_model_data.SNAPSHOTS)
     for i in (0, 1):
         snapshots[i] = attr.evolve(snapshots[i], id=bytes([i]) * 20)
     swh_storage.snapshot_add(snapshots)
 
+    config_id = scrubber_db.config_add("cfg1", datastore, swhids.ObjectType.SNAPSHOT, 1)
     StorageChecker(
         db=scrubber_db,
         storage=swh_storage,
-        object_type="snapshot",
-        start_partition_id=0,
-        end_partition_id=1,
-        nb_partitions=1,
+        config_id=config_id,
     ).run()
 
     corrupt_objects = list(scrubber_db.corrupt_object_iter())
     assert len(corrupt_objects) == 2
     assert {co.id for co in corrupt_objects} == {
         swhids.CoreSWHID.from_string(swhid)
         for swhid in [
             "swh:1:snp:0000000000000000000000000000000000000000",
             "swh:1:snp:0101010101010101010101010101010101010101",
         ]
     }
 
-    assert_checked_ranges(scrubber_db, datastore, {(swhids.ObjectType.SNAPSHOT, 0, 1)})
+    assert_checked_ranges(
+        scrubber_db,
+        [(swhids.ObjectType.SNAPSHOT, config_id)],
+        {(swhids.ObjectType.SNAPSHOT, 0, 1)},
+    )
 
 
 def test_corrupt_snapshots_different_batches(scrubber_db, datastore, swh_storage):
-    # FIXME: this is brittle, because it relies on both objects being on different
+    # FIXME: this is brittle, because it relies on objects being on different
     # partitions. In particular on Cassandra, it will break if the hashing scheme
     # or hash algorithm changes.
     snapshots = list(swh_model_data.SNAPSHOTS)
-    snapshots.extend([attr.evolve(snapshots[0], id=bytes([i]) * 20) for i in (0, 255)])
+    snapshots.extend(
+        [attr.evolve(snapshots[0], id=bytes([17 * i]) * 20) for i in range(16)]
+    )
     swh_storage.snapshot_add(snapshots)
 
+    config_id = scrubber_db.config_add(
+        "cfg1", datastore, swhids.ObjectType.SNAPSHOT, 16
+    )
     StorageChecker(
         db=scrubber_db,
         storage=swh_storage,
-        object_type="snapshot",
-        start_partition_id=0,
-        end_partition_id=1,
-        nb_partitions=2,
+        config_id=config_id,
+        limit=8,
     ).run()
 
     corrupt_objects = list(scrubber_db.corrupt_object_iter())
-    assert len(corrupt_objects) == 1
+    assert len(corrupt_objects) == 8
 
-    # Simulates resuming from a different process, with an empty lru_cache
+    # Simulates resuming from a different process
     scrubber_db.datastore_get_or_add.cache_clear()
 
     StorageChecker(
         db=scrubber_db,
         storage=swh_storage,
-        object_type="snapshot",
-        start_partition_id=1,
-        end_partition_id=2,
-        nb_partitions=2,
+        config_id=config_id,
+        limit=8,
     ).run()
 
     corrupt_objects = list(scrubber_db.corrupt_object_iter())
-    assert len(corrupt_objects) == 2
+    assert len(corrupt_objects) == 16
     assert {co.id for co in corrupt_objects} == {
         swhids.CoreSWHID.from_string(swhid)
-        for swhid in [
-            "swh:1:snp:0000000000000000000000000000000000000000",
-            "swh:1:snp:ffffffffffffffffffffffffffffffffffffffff",
-        ]
+        for swhid in ["swh:1:snp:" + f"{i:x}" * 40 for i in range(16)]
     }
 
     assert_checked_ranges(
         scrubber_db,
-        datastore,
-        {(swhids.ObjectType.SNAPSHOT, 0, 2), (swhids.ObjectType.SNAPSHOT, 1, 2)},
+        [(swhids.ObjectType.SNAPSHOT, config_id)],
+        {(swhids.ObjectType.SNAPSHOT, i, 16) for i in range(16)},
     )
 
 
 def test_directory_duplicate_entries(scrubber_db, datastore, swh_storage):
     run_validators = attr.get_run_validators()
     attr.set_run_validators(False)
     try:
@@ -256,22 +273,22 @@
             + b"0 foo\x00" + b"\x00" * 20
             + b"1 foo\x00" + b"\x01" * 20
             # fmt: on
         ),
     )
 
     before_date = datetime.datetime.now(tz=datetime.timezone.utc)
-    for object_type in ("snapshot", "release", "revision", "directory"):
+    config = []
+    for object_type in OBJECT_TYPES:
+        config_id = scrubber_db.config_add("cfg2", datastore, object_type, 1)
+        config.append((object_type, config_id))
         StorageChecker(
             db=scrubber_db,
             storage=swh_storage,
-            object_type=object_type,
-            start_partition_id=0,
-            end_partition_id=1,
-            nb_partitions=1,
+            config_id=config_id,
         ).run()
     after_date = datetime.datetime.now(tz=datetime.timezone.utc)
 
     corrupt_objects = list(scrubber_db.corrupt_object_iter())
     assert len(corrupt_objects) == 1
     assert corrupt_objects[0].id == invalid_directory.swhid()
     assert corrupt_objects[0].datastore == datastore
@@ -281,76 +298,75 @@
         <= after_date + datetime.timedelta(seconds=5)
     )
     assert kafka_to_value(corrupt_objects[0].object_) == msgpack.loads(
         msgpack.dumps(deduplicated_directory.to_dict())  # turn entry list into tuple
     )
 
     assert_checked_ranges(
-        scrubber_db, datastore, EXPECTED_PARTITIONS, before_date, after_date
+        scrubber_db, config, EXPECTED_PARTITIONS, before_date, after_date
     )
 
 
 def test_no_recheck(scrubber_db, datastore, swh_storage):
     """
     Tests that objects that were already checked are not checked again on
     the next run.
     """
-    # Corrupt two snapshots
+    # check the whole (empty) storage with a given config
+    config_id = scrubber_db.config_add("cfg2", datastore, swhids.ObjectType.SNAPSHOT, 1)
+    StorageChecker(
+        db=scrubber_db,
+        storage=swh_storage,
+        config_id=config_id,
+    ).run()
+
+    # Corrupt two snapshots and add them to the storage
     snapshots = list(swh_model_data.SNAPSHOTS)
     for i in (0, 1):
         snapshots[i] = attr.evolve(snapshots[i], id=bytes([i]) * 20)
     swh_storage.snapshot_add(snapshots)
 
-    # Mark ranges as already checked
-    now = datetime.datetime.now(tz=datetime.timezone.utc)
-    for (object_type, range_start, range_end) in EXPECTED_PARTITIONS:
-        scrubber_db.checked_partition_upsert(
-            datastore, object_type, range_start, range_end, now
-        )
-
-    previous_partitions = set(scrubber_db.checked_partition_iter(datastore))
+    previous_partitions = set(scrubber_db.checked_partition_iter(config_id))
 
+    # rerun a checker for the same config, it should be a noop
     StorageChecker(
         db=scrubber_db,
         storage=swh_storage,
-        object_type="snapshot",
-        start_partition_id=0,
-        end_partition_id=1,
-        nb_partitions=1,
+        config_id=config_id,
     ).run()
 
     corrupt_objects = list(scrubber_db.corrupt_object_iter())
     assert (
         corrupt_objects == []
     ), "Detected corrupt objects in ranges that should have been skipped."
 
     # Make sure the DB was not changed (in particular, that timestamps were not bumped)
-    assert set(scrubber_db.checked_partition_iter(datastore)) == previous_partitions
+    assert set(scrubber_db.checked_partition_iter(config_id)) == previous_partitions
 
 
 def test_no_hole(scrubber_db, datastore, swh_storage):
     swh_storage.content_add([CONTENT1])
     swh_storage.directory_add([DIRECTORY1, DIRECTORY2])
     swh_storage.revision_add([REVISION1])
     swh_storage.release_add([RELEASE1])
     swh_storage.snapshot_add([SNAPSHOT1])
 
-    for object_type in ("snapshot", "release", "revision", "directory"):
+    config = []
+    for object_type in OBJECT_TYPES:
+        config_id = scrubber_db.config_add("cfg2", datastore, object_type, 1)
+        config.append((object_type, config_id))
         StorageChecker(
             db=scrubber_db,
             storage=swh_storage,
-            object_type=object_type,
-            start_partition_id=0,
-            end_partition_id=1,
-            nb_partitions=1,
+            config_id=config_id,
         ).run()
 
     assert list(scrubber_db.missing_object_iter()) == []
 
-    assert_checked_ranges(scrubber_db, datastore, EXPECTED_PARTITIONS)
+    assert_checked_ranges(scrubber_db, config, EXPECTED_PARTITIONS)
 
 
 @pytest.mark.parametrize(
     "missing_object",
     ["content1", "directory1", "directory2", "revision1", "release1"],
 )
 def test_one_hole(scrubber_db, datastore, swh_storage, missing_object):
@@ -382,47 +398,51 @@
         missing_swhid = RELEASE1.swhid()
         reference_swhids = [SNAPSHOT1.swhid()]
     else:
         swh_storage.release_add([RELEASE1])
 
     swh_storage.snapshot_add([SNAPSHOT1])
 
-    for object_type in ("snapshot", "release", "revision", "directory"):
+    config = []
+    for object_type in OBJECT_TYPES:
+        config_id = scrubber_db.config_add(
+            f"cfg_{object_type.name}", datastore, object_type, 1
+        )
+        config.append((object_type, config_id))
         StorageChecker(
             db=scrubber_db,
             storage=swh_storage,
-            object_type=object_type,
-            start_partition_id=0,
-            end_partition_id=1,
-            nb_partitions=1,
+            config_id=config_id,
         ).run()
 
     assert [mo.id for mo in scrubber_db.missing_object_iter()] == [missing_swhid]
     assert {
         (mor.missing_id, mor.reference_id)
         for mor in scrubber_db.missing_object_reference_iter(missing_swhid)
     } == {(missing_swhid, reference_swhid) for reference_swhid in reference_swhids}
 
-    assert_checked_ranges(scrubber_db, datastore, EXPECTED_PARTITIONS)
+    assert_checked_ranges(scrubber_db, config, EXPECTED_PARTITIONS)
 
 
 def test_two_holes(scrubber_db, datastore, swh_storage):
     # missing content and revision
     swh_storage.directory_add([DIRECTORY1, DIRECTORY2])
     swh_storage.release_add([RELEASE1])
     swh_storage.snapshot_add([SNAPSHOT1])
 
-    for object_type in ("snapshot", "release", "revision", "directory"):
+    config = []
+    for object_type in OBJECT_TYPES:
+        config_id = scrubber_db.config_add(
+            f"cfg_{object_type.name}", datastore, object_type, 1
+        )
+        config.append((object_type, config_id))
         StorageChecker(
             db=scrubber_db,
             storage=swh_storage,
-            object_type=object_type,
-            start_partition_id=0,
-            end_partition_id=1,
-            nb_partitions=1,
+            config_id=config_id,
         ).run()
 
     assert {mo.id for mo in scrubber_db.missing_object_iter()} == {
         CONTENT1.swhid(),
         REVISION1.swhid(),
     }
     assert {
@@ -430,8 +450,8 @@
         for mor in scrubber_db.missing_object_reference_iter(CONTENT1.swhid())
     } == {DIRECTORY1.swhid(), DIRECTORY2.swhid()}
     assert {
         mor.reference_id
         for mor in scrubber_db.missing_object_reference_iter(REVISION1.swhid())
     } == {RELEASE1.swhid()}
 
-    assert_checked_ranges(scrubber_db, datastore, EXPECTED_PARTITIONS)
+    assert_checked_ranges(scrubber_db, config, EXPECTED_PARTITIONS)
```

### Comparing `swh.scrubber-1.0.3/swh/scrubber/tests/test_fixer.py` & `swh.scrubber-2.0.0/swh/scrubber/tests/test_fixer.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/tests/test_init.py` & `swh.scrubber-2.0.0/swh/scrubber/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/tests/test_journal_kafka.py` & `swh.scrubber-2.0.0/swh/scrubber/tests/test_journal_kafka.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/tests/test_origin_locator.py` & `swh.scrubber-2.0.0/swh/scrubber/tests/test_origin_locator.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/tests/test_storage_cassandra.py` & `swh.scrubber-2.0.0/swh/scrubber/tests/test_storage_cassandra.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/tests/test_storage_postgresql.py` & `swh.scrubber-2.0.0/swh/scrubber/tests/test_storage_postgresql.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh/scrubber/utils.py` & `swh.scrubber-2.0.0/swh/scrubber/utils.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.3/swh.scrubber.egg-info/SOURCES.txt` & `swh.scrubber-2.0.0/swh.scrubber.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 swh/scrubber/sql/20-enums.sql
 swh/scrubber/sql/30-schema.sql
 swh/scrubber/sql/60-indexes.sql
 swh/scrubber/sql/upgrades/2.sql
 swh/scrubber/sql/upgrades/3.sql
 swh/scrubber/sql/upgrades/4.sql
 swh/scrubber/sql/upgrades/5.sql
+swh/scrubber/sql/upgrades/6.sql
 swh/scrubber/tests/__init__.py
 swh/scrubber/tests/conftest.py
 swh/scrubber/tests/storage_checker_tests.py
 swh/scrubber/tests/test_cli.py
 swh/scrubber/tests/test_db.py
 swh/scrubber/tests/test_fixer.py
 swh/scrubber/tests/test_init.py
```

### Comparing `swh.scrubber-1.0.3/tox.ini` & `swh.scrubber-2.0.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [tox]
-requires =
-  tox>4
+minversion=4
 envlist=black,flake8,mypy,py3
 
 [testenv]
+passenv =
+  JAVA_HOME
+  SWH_CASSANDRA_LOG
 extras =
   testing
 deps =
   pytest-cov
 commands =
   pytest --doctest-modules \
          {envsitepackagesdir}/swh/scrubber \
```


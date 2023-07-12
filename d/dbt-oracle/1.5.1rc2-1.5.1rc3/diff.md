# Comparing `tmp/dbt-oracle-1.5.1rc2.tar.gz` & `tmp/dbt-oracle-1.5.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-oracle-1.5.1rc2.tar", last modified: Thu Jul  6 23:24:55 2023, max compression
+gzip compressed data, was "dbt-oracle-1.5.1rc3.tar", last modified: Wed Jul 12 18:06:48 2023, max compression
```

## Comparing `dbt-oracle-1.5.1rc2.tar` & `dbt-oracle-1.5.1rc3.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.924222 dbt-oracle-1.5.1rc2/
--rw-r--r--   0 abhisoms   (501) staff       (20)      398 2022-05-04 01:22:16.000000 dbt-oracle-1.5.1rc2/HISTORY.md
--rw-r--r--   0 abhisoms   (501) staff       (20)    11364 2022-03-16 18:13:02.000000 dbt-oracle-1.5.1rc2/LICENSE.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)      259 2021-11-24 19:19:59.000000 dbt-oracle-1.5.1rc2/MANIFEST.in
--rw-r--r--   0 abhisoms   (501) staff       (20)      129 2022-04-26 13:32:00.000000 dbt-oracle-1.5.1rc2/NOTICE.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-07-06 23:24:55.924393 dbt-oracle-1.5.1rc2/PKG-INFO
--rw-r--r--   0 abhisoms   (501) staff       (20)     2015 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc2/README.md
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.679486 dbt-oracle-1.5.1rc2/bin/
--rw-r--r--   0 abhisoms   (501) staff       (20)     2582 2022-07-07 19:56:20.000000 dbt-oracle-1.5.1rc2/bin/create-pem-from-p12
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.681639 dbt-oracle-1.5.1rc2/dbt/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:47.000000 dbt-oracle-1.5.1rc2/dbt/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.684117 dbt-oracle-1.5.1rc2/dbt/adapters/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:04:45.000000 dbt-oracle-1.5.1rc2/dbt/adapters/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.700775 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1040 2022-03-30 23:04:11.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      654 2023-07-03 19:36:07.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/__version__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2237 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/column.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4707 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/connection_helper.py
--rw-r--r--   0 abhisoms   (501) staff       (20)    11633 2023-07-05 22:26:22.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/connections.py
--rw-r--r--   0 abhisoms   (501) staff       (20)    14634 2023-07-06 17:14:57.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/impl.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6054 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/keyword_catalog.py
--rw-r--r--   0 abhisoms   (501) staff       (20)    10054 2023-07-06 22:57:39.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/python_submissions.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1354 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc2/dbt/adapters/oracle/relation.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.702580 dbt-oracle-1.5.1rc2/dbt/include/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:43.000000 dbt-oracle-1.5.1rc2/dbt/include/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.712661 dbt-oracle-1.5.1rc2/dbt/include/oracle/
--rw-r--r--   0 abhisoms   (501) staff       (20)      687 2022-03-30 23:08:38.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      138 2021-11-08 19:31:21.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/dbt_project.yml
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.728603 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/
--rw-r--r--   0 abhisoms   (501) staff       (20)    14870 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/adapters.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1332 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/apply_grants.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     5447 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/catalog.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     2177 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/columns.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.665531 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.740613 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/incremental/
--rw-r--r--   0 abhisoms   (501) staff       (20)     4373 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     6918 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/incremental/strategies.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.752296 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/python_model/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3412 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/python_model/python.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.756227 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/seed/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1907 2022-03-30 23:05:21.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.768434 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/
--rw-r--r--   0 abhisoms   (501) staff       (20)     9649 2022-11-15 22:09:50.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1444 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     4922 2022-12-16 19:27:06.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.774998 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/table/
--rw-r--r--   0 abhisoms   (501) staff       (20)     5486 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/table/table.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.782236 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/tests/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1191 2022-03-30 23:06:10.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/tests/helpers.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.788842 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/view/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3468 2023-06-13 04:33:00.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/view/view.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1906 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/schema_tests.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.861091 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/
--rw-r--r--   0 abhisoms   (501) staff       (20)      792 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      881 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/data_types.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1457 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/dateadd.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     2378 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/datediff.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1037 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/datetrunc.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      691 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/except.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      807 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/hash.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      842 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/last_day.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      761 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/position.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      939 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/right.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      916 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/timestamps.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      729 2022-05-24 00:59:25.000000 dbt-oracle-1.5.1rc2/dbt/include/oracle/profile_template.yml
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.867016 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-07-06 23:24:55.000000 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/PKG-INFO
--rw-r--r--   0 abhisoms   (501) staff       (20)     4219 2023-07-06 23:24:55.000000 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)        1 2023-07-06 23:24:55.000000 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)        1 2022-04-11 10:34:24.000000 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/not-zip-safe
--rw-r--r--   0 abhisoms   (501) staff       (20)       49 2023-07-06 23:24:55.000000 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/requires.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)       10 2023-07-06 23:24:55.000000 dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/top_level.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)      100 2021-12-16 21:41:11.000000 dbt-oracle-1.5.1rc2/pyproject.toml
--rw-r--r--   0 abhisoms   (501) staff       (20)     1449 2023-07-06 23:24:55.926019 dbt-oracle-1.5.1rc2/setup.cfg
--rw-r--r--   0 abhisoms   (501) staff       (20)     2973 2023-07-06 23:24:15.000000 dbt-oracle-1.5.1rc2/setup.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.873521 dbt-oracle-1.5.1rc2/tests/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3339 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/tests/README.md
--rw-r--r--   0 abhisoms   (501) staff       (20)      636 2022-08-08 20:50:48.000000 dbt-oracle-1.5.1rc2/tests/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1507 2022-06-27 15:21:32.000000 dbt-oracle-1.5.1rc2/tests/conftest.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.666638 dbt-oracle-1.5.1rc2/tests/functional/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.892958 dbt-oracle-1.5.1rc2/tests/functional/adapter/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.897876 dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/
--rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5635 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/fixtures.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6658 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/test_constraints.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.903565 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.909258 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4919 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4558 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4765 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.912328 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/sync_schema/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/sync_schema/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5473 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2456 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4652 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4882 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5907 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_unique_id.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.914778 dbt-oracle-1.5.1rc2/tests/functional/adapter/macros/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-06-27 15:21:18.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/macros/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2441 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/macros/test_alter_column_type.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.919222 dbt-oracle-1.5.1rc2/tests/functional/adapter/simple_seed/
--rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/simple_seed/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1103 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/simple_seed/test_simple_seed.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.921130 dbt-oracle-1.5.1rc2/tests/functional/adapter/snapshots/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-08-03 17:58:52.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/snapshots/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     3883 2022-08-03 17:58:52.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/snapshots/test_invalidate_deletes.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4629 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_basic.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     3038 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_caching.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      783 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_concurrency.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4307 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_config.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2979 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_data_types.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5413 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_docs_generate.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6587 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_docs_genreferences.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1201 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_ephemeral.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1993 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_generictests_where.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2910 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_grants.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4711 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/test_quoted_relations.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-06 23:24:55.923588 dbt-oracle-1.5.1rc2/tests/functional/adapter/utils/
--rw-r--r--   0 abhisoms   (501) staff       (20)     5777 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/utils/test_common_utils.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6830 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc2/tests/functional/adapter/utils/test_dateutils.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.942989 dbt-oracle-1.5.1rc3/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      398 2022-05-04 01:22:16.000000 dbt-oracle-1.5.1rc3/HISTORY.md
+-rw-r--r--   0 abhisoms   (501) staff       (20)    11364 2022-03-16 18:13:02.000000 dbt-oracle-1.5.1rc3/LICENSE.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)      259 2021-11-24 19:19:59.000000 dbt-oracle-1.5.1rc3/MANIFEST.in
+-rw-r--r--   0 abhisoms   (501) staff       (20)      129 2022-04-26 13:32:00.000000 dbt-oracle-1.5.1rc3/NOTICE.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-07-12 18:06:48.943433 dbt-oracle-1.5.1rc3/PKG-INFO
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2015 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc3/README.md
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.664013 dbt-oracle-1.5.1rc3/bin/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2582 2022-07-07 19:56:20.000000 dbt-oracle-1.5.1rc3/bin/create-pem-from-p12
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.666761 dbt-oracle-1.5.1rc3/dbt/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:47.000000 dbt-oracle-1.5.1rc3/dbt/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.669620 dbt-oracle-1.5.1rc3/dbt/adapters/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:04:45.000000 dbt-oracle-1.5.1rc3/dbt/adapters/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.691001 dbt-oracle-1.5.1rc3/dbt/adapters/oracle/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1040 2022-03-30 23:04:11.000000 dbt-oracle-1.5.1rc3/dbt/adapters/oracle/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      654 2023-07-12 16:52:57.000000 dbt-oracle-1.5.1rc3/dbt/adapters/oracle/__version__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2237 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc3/dbt/adapters/oracle/column.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4707 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc3/dbt/adapters/oracle/connection_helper.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)    11633 2023-07-12 16:52:57.000000 dbt-oracle-1.5.1rc3/dbt/adapters/oracle/connections.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)    14634 2023-07-12 16:52:57.000000 dbt-oracle-1.5.1rc3/dbt/adapters/oracle/impl.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6054 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/dbt/adapters/oracle/keyword_catalog.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)    10054 2023-07-12 16:52:57.000000 dbt-oracle-1.5.1rc3/dbt/adapters/oracle/python_submissions.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1354 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc3/dbt/adapters/oracle/relation.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.692643 dbt-oracle-1.5.1rc3/dbt/include/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:43.000000 dbt-oracle-1.5.1rc3/dbt/include/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.697841 dbt-oracle-1.5.1rc3/dbt/include/oracle/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      687 2022-03-30 23:08:38.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      138 2021-11-08 19:31:21.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/dbt_project.yml
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.713415 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/
+-rw-r--r--   0 abhisoms   (501) staff       (20)    14894 2023-07-12 16:52:57.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/adapters.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1332 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/apply_grants.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5447 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/catalog.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2177 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/columns.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.650550 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.719545 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/incremental/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4373 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6918 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/incremental/strategies.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.725304 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/python_model/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3412 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/python_model/python.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.731209 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/seed/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1907 2022-03-30 23:05:21.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.745112 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/snapshot/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     9649 2022-11-15 22:09:50.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1444 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4922 2022-12-16 19:27:06.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.751776 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/table/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5486 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/table/table.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.755290 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/tests/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1191 2022-03-30 23:06:10.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/tests/helpers.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.757576 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/view/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3468 2023-06-13 04:33:00.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/view/view.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1906 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/schema_tests.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.859866 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      792 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      881 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/data_types.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1457 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/dateadd.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2378 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/datediff.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1037 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/datetrunc.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      691 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/except.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      807 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/hash.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      842 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/last_day.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      761 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/position.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      939 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/right.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      916 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/timestamps.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      729 2022-05-24 00:59:25.000000 dbt-oracle-1.5.1rc3/dbt/include/oracle/profile_template.yml
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.869467 dbt-oracle-1.5.1rc3/dbt_oracle.egg-info/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-07-12 18:06:48.000000 dbt-oracle-1.5.1rc3/dbt_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4219 2023-07-12 18:06:48.000000 dbt-oracle-1.5.1rc3/dbt_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)        1 2023-07-12 18:06:48.000000 dbt-oracle-1.5.1rc3/dbt_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)        1 2022-04-11 10:34:24.000000 dbt-oracle-1.5.1rc3/dbt_oracle.egg-info/not-zip-safe
+-rw-r--r--   0 abhisoms   (501) staff       (20)       49 2023-07-12 18:06:48.000000 dbt-oracle-1.5.1rc3/dbt_oracle.egg-info/requires.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)       10 2023-07-12 18:06:48.000000 dbt-oracle-1.5.1rc3/dbt_oracle.egg-info/top_level.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)      100 2021-12-16 21:41:11.000000 dbt-oracle-1.5.1rc3/pyproject.toml
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1449 2023-07-12 18:06:48.948544 dbt-oracle-1.5.1rc3/setup.cfg
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2973 2023-07-12 16:53:25.000000 dbt-oracle-1.5.1rc3/setup.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.872371 dbt-oracle-1.5.1rc3/tests/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3339 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc3/tests/README.md
+-rw-r--r--   0 abhisoms   (501) staff       (20)      636 2022-08-08 20:50:48.000000 dbt-oracle-1.5.1rc3/tests/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1507 2022-06-27 15:21:32.000000 dbt-oracle-1.5.1rc3/tests/conftest.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.651684 dbt-oracle-1.5.1rc3/tests/functional/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.886771 dbt-oracle-1.5.1rc3/tests/functional/adapter/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.889598 dbt-oracle-1.5.1rc3/tests/functional/adapter/constraints/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/constraints/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5631 2023-07-12 16:52:57.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/constraints/fixtures.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6658 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/constraints/test_constraints.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.896920 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.902972 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/quotes/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/quotes/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4919 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4558 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4765 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.904850 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/sync_schema/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/sync_schema/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5473 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2456 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4652 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4882 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5907 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/test_unique_id.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.906540 dbt-oracle-1.5.1rc3/tests/functional/adapter/macros/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-06-27 15:21:18.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/macros/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2441 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/macros/test_alter_column_type.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.913264 dbt-oracle-1.5.1rc3/tests/functional/adapter/simple_seed/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/simple_seed/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1103 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/simple_seed/test_simple_seed.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.927564 dbt-oracle-1.5.1rc3/tests/functional/adapter/snapshots/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-08-03 17:58:52.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/snapshots/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3883 2022-08-03 17:58:52.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/snapshots/test_invalidate_deletes.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4629 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/test_basic.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3038 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/test_caching.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      783 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/test_concurrency.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4307 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/test_config.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2979 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/test_data_types.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5413 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/test_docs_generate.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6587 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/test_docs_genreferences.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1201 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/test_ephemeral.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1993 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/test_generictests_where.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2910 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/test_grants.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4711 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/test_quoted_relations.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-07-12 18:06:48.941412 dbt-oracle-1.5.1rc3/tests/functional/adapter/utils/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5777 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/utils/test_common_utils.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6830 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc3/tests/functional/adapter/utils/test_dateutils.py
```

### Comparing `dbt-oracle-1.5.1rc2/LICENSE.txt` & `dbt-oracle-1.5.1rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/PKG-INFO` & `dbt-oracle-1.5.1rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-oracle
-Version: 1.5.1rc2
+Version: 1.5.1rc3
 Summary: dbt (data build tool) adapter for the Oracle database
 Home-page: https://github.com/oracle/dbt-oracle
 Author: Oracle
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile
 Project-URL: Source, https://github.com/oracle/dbt-oracle
 Project-URL: Bug Tracker, https://github.com/oracle/dbt-oracle/issues
```

### Comparing `dbt-oracle-1.5.1rc2/README.md` & `dbt-oracle-1.5.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/bin/create-pem-from-p12` & `dbt-oracle-1.5.1rc3/bin/create-pem-from-p12`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/__init__.py` & `dbt-oracle-1.5.1rc3/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/adapters/__init__.py` & `dbt-oracle-1.5.1rc3/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/__init__.py` & `dbt-oracle-1.5.1rc3/dbt/adapters/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/__version__.py` & `dbt-oracle-1.5.1rc3/dbt/adapters/oracle/__version__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/column.py` & `dbt-oracle-1.5.1rc3/dbt/adapters/oracle/column.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/connection_helper.py` & `dbt-oracle-1.5.1rc3/dbt/adapters/oracle/connection_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/connections.py` & `dbt-oracle-1.5.1rc3/dbt/adapters/oracle/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/impl.py` & `dbt-oracle-1.5.1rc3/dbt/adapters/oracle/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/keyword_catalog.py` & `dbt-oracle-1.5.1rc3/dbt/adapters/oracle/keyword_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/python_submissions.py` & `dbt-oracle-1.5.1rc3/dbt/adapters/oracle/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/adapters/oracle/relation.py` & `dbt-oracle-1.5.1rc3/dbt/adapters/oracle/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/__init__.py` & `dbt-oracle-1.5.1rc3/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/__init__.py` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/adapters.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/adapters.sql`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         ) dbt_sbq_tmp
         where 1 = 0 and rownum < 1
     {% endcall %}
 
     {{ return(load_result('get_columns_in_query').table.columns | map(attribute='name') | list) }}
 {% endmacro %}
 
-{% macro oracle__get_empty_subquery_sql(select_sql) %}
+{% macro oracle__get_empty_subquery_sql(select_sql, select_sql_header=none) %}
     select * from (
         {{ select_sql }}
     ) dbt_sbq_tmp
     where 1 = 0 and rownum < 1
 {% endmacro %}
 
 {% macro oracle__get_empty_schema_sql(columns) %}
```

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/apply_grants.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/catalog.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/columns.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/incremental/incremental.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/incremental/strategies.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/python_model/python.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/seed/seed.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/snapshot/strategies.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/table/table.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/tests/helpers.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/materializations/view/view.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/materializations/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/schema_tests.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/schema_tests.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/cast_bool_to_text.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/cast_bool_to_text.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/data_types.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/dateadd.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/datediff.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/datetrunc.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/datetrunc.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/except.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/except.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/hash.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/hash.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/last_day.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/last_day.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/position.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/position.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/right.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/right.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/macros/utils/timestamps.sql` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt/include/oracle/profile_template.yml` & `dbt-oracle-1.5.1rc3/dbt/include/oracle/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/PKG-INFO` & `dbt-oracle-1.5.1rc3/dbt_oracle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-oracle
-Version: 1.5.1rc2
+Version: 1.5.1rc3
 Summary: dbt (data build tool) adapter for the Oracle database
 Home-page: https://github.com/oracle/dbt-oracle
 Author: Oracle
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile
 Project-URL: Source, https://github.com/oracle/dbt-oracle
 Project-URL: Bug Tracker, https://github.com/oracle/dbt-oracle/issues
```

### Comparing `dbt-oracle-1.5.1rc2/dbt_oracle.egg-info/SOURCES.txt` & `dbt-oracle-1.5.1rc3/dbt_oracle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/setup.cfg` & `dbt-oracle-1.5.1rc3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dbt-oracle
-version = 1.5.1rc2
+version = 1.5.1rc3
 description = dbt (data build tool) adapter for the Oracle database
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = Oracle dbt
 author = Oracle
 license = Apache Software License 2.0
 classifiers =
```

### Comparing `dbt-oracle-1.5.1rc2/setup.py` & `dbt-oracle-1.5.1rc3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     'Bug Tracker': 'https://github.com/oracle/dbt-oracle/issues',
     'CI': 'https://github.com/oracle/dbt-oracle/actions',
     "Release Notes": "https://github.com/oracle/dbt-oracle/releases"
 }
 
 url = 'https://github.com/oracle/dbt-oracle'
 
-VERSION = '1.5.1rc2'
+VERSION = '1.5.1rc3'
 setup(
     author="Oracle",
     python_requires='>=3.7.2',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `dbt-oracle-1.5.1rc2/tests/README.md` & `dbt-oracle-1.5.1rc3/tests/README.md`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/__init__.py` & `dbt-oracle-1.5.1rc3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/conftest.py` & `dbt-oracle-1.5.1rc3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/__init__.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/fixtures.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/constraints/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         quote: true
         data_type: integer
         description: hello
         constraints:
           - type: not_null
           - type: primary_key
           - type: check
-            expression: (id > 0)
+            expression: id > 0
         tests:
           - unique
       - name: color
         data_type: char
       - name: date_day
         data_type: date
   - name: my_model_error
@@ -265,15 +265,15 @@
 models:
   - name: my_model
     config:
       contract:
         enforced: true
     constraints:
       - type: check
-        expression: (id > 0)
+        expression: id > 0
       - type: primary_key
         columns: [ id ]
       - type: unique
         columns: [ color, date_day ]
         name: strange_uniqueness_requirement
     columns:
       - name: id
```

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/constraints/test_constraints.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/constraints/test_constraints.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/incremental_materialization/test_unique_id.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/incremental_materialization/test_unique_id.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/macros/test_alter_column_type.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/macros/test_alter_column_type.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/simple_seed/__init__.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/simple_seed/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/simple_seed/test_simple_seed.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/simple_seed/test_simple_seed.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/snapshots/test_invalidate_deletes.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/snapshots/test_invalidate_deletes.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_basic.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_caching.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/test_caching.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_concurrency.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_config.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/test_config.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_data_types.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/test_data_types.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_docs_generate.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_docs_genreferences.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/test_docs_genreferences.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_ephemeral.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_generictests_where.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/test_generictests_where.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_grants.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/test_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/test_quoted_relations.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/test_quoted_relations.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/utils/test_common_utils.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/utils/test_common_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.1rc2/tests/functional/adapter/utils/test_dateutils.py` & `dbt-oracle-1.5.1rc3/tests/functional/adapter/utils/test_dateutils.py`

 * *Files identical despite different names*


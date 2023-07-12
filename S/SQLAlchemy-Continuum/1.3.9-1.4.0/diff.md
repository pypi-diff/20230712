# Comparing `tmp/SQLAlchemy-Continuum-1.3.9.tar.gz` & `tmp/SQLAlchemy-Continuum-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SQLAlchemy-Continuum-1.3.9.tar", last modified: Tue Mar 19 13:32:22 2019, max compression
+gzip compressed data, was "SQLAlchemy-Continuum-1.4.0.tar", last modified: Wed Jul 12 17:13:17 2023, max compression
```

## Comparing `SQLAlchemy-Continuum-1.3.9.tar` & `SQLAlchemy-Continuum-1.4.0.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/
--rw-r--r--   0 konsta     (501) staff       (20)    16466 2019-03-19 13:10:38.000000 SQLAlchemy-Continuum-1.3.9/CHANGES.rst
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/docs/
--rw-r--r--   0 konsta     (501) staff       (20)    12292 2014-09-02 12:34:50.000000 SQLAlchemy-Continuum-1.3.9/docs/.DS_Store
--rw-r--r--   0 konsta     (501) staff       (20)      544 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/docs/alembic.rst
--rw-r--r--   0 konsta     (501) staff       (20)      757 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/docs/api.rst
--rw-r--r--   0 konsta     (501) staff       (20)     8420 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/docs/conf.py
--rw-r--r--   0 konsta     (501) staff       (20)     5375 2014-12-09 15:05:34.000000 SQLAlchemy-Continuum-1.3.9/docs/configuration.rst
--rw-r--r--   0 konsta     (501) staff       (20)      297 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.9/docs/index.rst
--rw-r--r--   0 konsta     (501) staff       (20)     3377 2018-03-07 18:18:00.000000 SQLAlchemy-Continuum-1.3.9/docs/intro.rst
--rw-r--r--   0 konsta     (501) staff       (20)       41 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/docs/license.rst
--rw-r--r--   0 konsta     (501) staff       (20)     6729 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/docs/make.bat
--rw-r--r--   0 konsta     (501) staff       (20)     6818 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/docs/Makefile
--rw-r--r--   0 konsta     (501) staff       (20)     1068 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.9/docs/native_versioning.rst
--rw-r--r--   0 konsta     (501) staff       (20)      801 2019-01-13 14:08:39.000000 SQLAlchemy-Continuum-1.3.9/docs/plugins.rst
--rw-r--r--   0 konsta     (501) staff       (20)     1714 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/docs/queries.rst
--rw-r--r--   0 konsta     (501) staff       (20)     2209 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/docs/revert.rst
--rw-r--r--   0 konsta     (501) staff       (20)     1898 2014-04-24 08:21:06.000000 SQLAlchemy-Continuum-1.3.9/docs/schema.rst
--rw-r--r--   0 konsta     (501) staff       (20)     1877 2017-06-28 12:35:40.000000 SQLAlchemy-Continuum-1.3.9/docs/transactions.rst
--rw-r--r--   0 konsta     (501) staff       (20)      892 2014-08-27 09:58:16.000000 SQLAlchemy-Continuum-1.3.9/docs/utilities.rst
--rw-r--r--   0 konsta     (501) staff       (20)     6020 2014-04-24 09:58:30.000000 SQLAlchemy-Continuum-1.3.9/docs/version_objects.rst
--rw-r--r--   0 konsta     (501) staff       (20)     1437 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/LICENSE
--rw-r--r--   0 konsta     (501) staff       (20)      193 2014-01-07 19:05:59.000000 SQLAlchemy-Continuum-1.3.9/MANIFEST.in
--rw-r--r--   0 konsta     (501) staff       (20)     1079 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/PKG-INFO
--rw-r--r--   0 konsta     (501) staff       (20)     2977 2019-01-13 14:08:39.000000 SQLAlchemy-Continuum-1.3.9/README.rst
--rw-r--r--   0 konsta     (501) staff       (20)       38 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/setup.cfg
--rw-r--r--   0 konsta     (501) staff       (20)     2413 2018-03-07 18:18:00.000000 SQLAlchemy-Continuum-1.3.9/setup.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/
--rw-r--r--   0 konsta     (501) staff       (20)     3258 2019-03-19 12:18:33.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     6758 2017-06-28 12:35:40.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/builder.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/dialects/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-08-14 14:08:11.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/dialects/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)    15324 2014-12-06 10:19:14.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/dialects/postgresql.py
--rw-r--r--   0 konsta     (501) staff       (20)      152 2014-04-29 12:36:20.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/exc.py
--rw-r--r--   0 konsta     (501) staff       (20)      975 2015-07-24 06:47:20.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/expression_reflector.py
--rw-r--r--   0 konsta     (501) staff       (20)      407 2014-09-04 12:34:32.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/factory.py
--rw-r--r--   0 konsta     (501) staff       (20)     5799 2014-07-10 11:45:57.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/fetcher.py
--rw-r--r--   0 konsta     (501) staff       (20)    18570 2018-07-30 12:47:07.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/manager.py
--rw-r--r--   0 konsta     (501) staff       (20)     9348 2016-01-21 08:13:38.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/model_builder.py
--rw-r--r--   0 konsta     (501) staff       (20)     2840 2014-07-16 13:16:55.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/operation.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/
--rw-r--r--   0 konsta     (501) staff       (20)      322 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)    10395 2017-01-30 16:29:17.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/activity.py
--rw-r--r--   0 konsta     (501) staff       (20)     1866 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/base.py
--rw-r--r--   0 konsta     (501) staff       (20)     2188 2017-01-30 16:29:17.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/flask.py
--rw-r--r--   0 konsta     (501) staff       (20)      987 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/null_delete.py
--rw-r--r--   0 konsta     (501) staff       (20)     2487 2014-08-19 08:18:11.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/property_mod_tracker.py
--rw-r--r--   0 konsta     (501) staff       (20)     3193 2014-12-30 15:57:18.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/transaction_changes.py
--rw-r--r--   0 konsta     (501) staff       (20)     3172 2014-10-01 06:46:34.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/transaction_meta.py
--rw-r--r--   0 konsta     (501) staff       (20)    12507 2019-03-19 12:18:33.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/relationship_builder.py
--rw-r--r--   0 konsta     (501) staff       (20)     4464 2015-09-27 08:54:29.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/reverter.py
--rw-r--r--   0 konsta     (501) staff       (20)     5593 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/schema.py
--rw-r--r--   0 konsta     (501) staff       (20)     4752 2017-10-12 10:54:04.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/table_builder.py
--rw-r--r--   0 konsta     (501) staff       (20)     5497 2019-03-19 13:08:16.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/transaction.py
--rw-r--r--   0 konsta     (501) staff       (20)    11266 2015-07-24 07:20:58.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/unit_of_work.py
--rw-r--r--   0 konsta     (501) staff       (20)    12240 2019-02-27 15:07:50.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/utils.py
--rw-r--r--   0 konsta     (501) staff       (20)     2095 2017-11-05 16:02:23.000000 SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/version.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/
--rw-r--r--   0 konsta     (501) staff       (20)        1 2019-03-19 13:32:21.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/dependency_links.txt
--rw-r--r--   0 konsta     (501) staff       (20)        1 2014-02-10 07:59:41.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/not-zip-safe
--rw-r--r--   0 konsta     (501) staff       (20)     1079 2019-03-19 13:32:21.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/PKG-INFO
--rw-r--r--   0 konsta     (501) staff       (20)      411 2019-03-19 13:32:21.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/requires.txt
--rw-r--r--   0 konsta     (501) staff       (20)     4049 2019-03-19 13:32:21.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/SOURCES.txt
--rw-r--r--   0 konsta     (501) staff       (20)       21 2019-03-19 13:32:21.000000 SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/top_level.txt
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/
--rw-r--r--   0 konsta     (501) staff       (20)     6588 2019-02-27 15:22:36.000000 SQLAlchemy-Continuum-1.3.9/tests/__init__.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/builders/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/builders/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)      259 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/builders/test_model_builder.py
--rw-r--r--   0 konsta     (501) staff       (20)     1146 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/builders/test_relationship_builder.py
--rw-r--r--   0 konsta     (501) staff       (20)     3550 2017-10-12 10:54:04.000000 SQLAlchemy-Continuum-1.3.9/tests/builders/test_table_builder.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/dialects/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.9/tests/dialects/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     2045 2014-10-13 19:41:57.000000 SQLAlchemy-Continuum-1.3.9/tests/dialects/test_triggers.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)      940 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_common_base_class.py
--rw-r--r--   0 konsta     (501) staff       (20)     3272 2014-06-16 09:20:44.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_concrete_inheritance.py
--rw-r--r--   0 konsta     (501) staff       (20)     7059 2015-09-27 08:36:34.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_join_table_inheritance.py
--rw-r--r--   0 konsta     (501) staff       (20)     1646 2017-06-28 12:35:40.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_multi_level_inheritance.py
--rw-r--r--   0 konsta     (501) staff       (20)     2980 2014-08-18 13:30:03.000000 SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_single_table_inheritance.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     5680 2014-08-14 13:56:49.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_activity.py
--rw-r--r--   0 konsta     (501) staff       (20)     8766 2017-01-30 16:29:17.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_flask.py
--rw-r--r--   0 konsta     (501) staff       (20)     1000 2014-08-14 13:56:49.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_null_delete.py
--rw-r--r--   0 konsta     (501) staff       (20)     1070 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_plugin_collection.py
--rw-r--r--   0 konsta     (501) staff       (20)     5881 2014-08-26 11:51:22.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_property_mod_tracker.py
--rw-r--r--   0 konsta     (501) staff       (20)     2473 2014-12-30 16:00:18.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_transaction_changes.py
--rw-r--r--   0 konsta     (501) staff       (20)     1253 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/plugins/test_transaction_meta.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     2048 2018-06-03 11:24:04.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_association_table_relations.py
--rw-r--r--   0 konsta     (501) staff       (20)     2035 2015-07-24 07:48:10.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_custom_condition_relations.py
--rw-r--r--   0 konsta     (501) staff       (20)     3029 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_dynamic_relationships.py
--rw-r--r--   0 konsta     (501) staff       (20)    14534 2017-10-12 10:54:04.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_many_to_many_relations.py
--rw-r--r--   0 konsta     (501) staff       (20)     3291 2016-01-21 08:13:38.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_non_versioned_classes.py
--rw-r--r--   0 konsta     (501) staff       (20)     9110 2014-12-28 13:06:15.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_one_to_many_relations.py
--rw-r--r--   0 konsta     (501) staff       (20)     2882 2014-07-10 11:45:57.000000 SQLAlchemy-Continuum-1.3.9/tests/relationships/test_one_to_one_relations.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/revert/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/revert/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     2112 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/revert/test_deep_relationships.py
--rw-r--r--   0 konsta     (501) staff       (20)     2806 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/revert/test_many_to_many_relationships.py
--rw-r--r--   0 konsta     (501) staff       (20)     1817 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/revert/test_one_to_one_relationship.py
--rw-r--r--   0 konsta     (501) staff       (20)     2127 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/revert/test_one_to_one_with_secondary_table.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/schema/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/schema/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)     2129 2014-10-01 13:34:49.000000 SQLAlchemy-Continuum-1.3.9/tests/schema/test_update_end_transaction_id.py
--rw-r--r--   0 konsta     (501) staff       (20)     2946 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/schema/test_update_property_mod_flags.py
--rw-r--r--   0 konsta     (501) staff       (20)     8343 2014-10-01 06:46:34.000000 SQLAlchemy-Continuum-1.3.9/tests/test_accessors.py
--rw-r--r--   0 konsta     (501) staff       (20)     3470 2017-11-05 16:02:23.000000 SQLAlchemy-Continuum-1.3.9/tests/test_changeset.py
--rw-r--r--   0 konsta     (501) staff       (20)     1935 2014-04-21 09:09:53.000000 SQLAlchemy-Continuum-1.3.9/tests/test_column_aliases.py
--rw-r--r--   0 konsta     (501) staff       (20)     3661 2018-03-07 18:18:00.000000 SQLAlchemy-Continuum-1.3.9/tests/test_column_inclusion_and_exclusion.py
--rw-r--r--   0 konsta     (501) staff       (20)     2456 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/test_composite_primary_key.py
--rw-r--r--   0 konsta     (501) staff       (20)     3713 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.9/tests/test_configuration.py
--rw-r--r--   0 konsta     (501) staff       (20)     2057 2014-10-01 09:31:26.000000 SQLAlchemy-Continuum-1.3.9/tests/test_custom_schema.py
--rw-r--r--   0 konsta     (501) staff       (20)     1114 2014-04-09 07:07:56.000000 SQLAlchemy-Continuum-1.3.9/tests/test_custom_version_base_class.py
--rw-r--r--   0 konsta     (501) staff       (20)     1356 2014-09-25 09:34:37.000000 SQLAlchemy-Continuum-1.3.9/tests/test_delete.py
--rw-r--r--   0 konsta     (501) staff       (20)     1068 2014-07-16 13:11:49.000000 SQLAlchemy-Continuum-1.3.9/tests/test_exotic_listener_chaining.py
--rw-r--r--   0 konsta     (501) staff       (20)     2509 2015-07-24 07:16:05.000000 SQLAlchemy-Continuum-1.3.9/tests/test_exotic_operation_combos.py
--rw-r--r--   0 konsta     (501) staff       (20)     2602 2017-01-30 17:14:23.000000 SQLAlchemy-Continuum-1.3.9/tests/test_i18n.py
--rw-r--r--   0 konsta     (501) staff       (20)     2647 2015-07-24 10:14:05.000000 SQLAlchemy-Continuum-1.3.9/tests/test_insert.py
--rw-r--r--   0 konsta     (501) staff       (20)     2336 2014-04-22 15:07:31.000000 SQLAlchemy-Continuum-1.3.9/tests/test_mapper_args.py
--rw-r--r--   0 konsta     (501) staff       (20)      976 2014-10-01 13:34:49.000000 SQLAlchemy-Continuum-1.3.9/tests/test_raw_sql.py
--rw-r--r--   0 konsta     (501) staff       (20)     6000 2015-09-27 08:54:29.000000 SQLAlchemy-Continuum-1.3.9/tests/test_revert.py
--rw-r--r--   0 konsta     (501) staff       (20)     1540 2014-09-02 06:42:43.000000 SQLAlchemy-Continuum-1.3.9/tests/test_savepoints.py
--rw-r--r--   0 konsta     (501) staff       (20)     2170 2018-07-30 12:47:07.000000 SQLAlchemy-Continuum-1.3.9/tests/test_sessions.py
--rw-r--r--   0 konsta     (501) staff       (20)     2654 2017-10-12 10:54:04.000000 SQLAlchemy-Continuum-1.3.9/tests/test_transaction.py
--rw-r--r--   0 konsta     (501) staff       (20)     3414 2015-07-24 06:49:15.000000 SQLAlchemy-Continuum-1.3.9/tests/test_update.py
--rw-r--r--   0 konsta     (501) staff       (20)     1707 2014-10-01 06:46:34.000000 SQLAlchemy-Continuum-1.3.9/tests/test_vacuum.py
--rw-r--r--   0 konsta     (501) staff       (20)     3640 2014-09-02 06:44:39.000000 SQLAlchemy-Continuum-1.3.9/tests/test_validity_strategy.py
--rw-r--r--   0 konsta     (501) staff       (20)      669 2014-04-09 15:04:22.000000 SQLAlchemy-Continuum-1.3.9/tests/test_versions.py
-drwxr-xr-x   0 konsta     (501) staff       (20)        0 2019-03-19 13:32:22.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/
--rw-r--r--   0 konsta     (501) staff       (20)        0 2014-04-25 11:06:55.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/__init__.py
--rw-r--r--   0 konsta     (501) staff       (20)      869 2014-04-25 11:08:20.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_changeset.py
--rw-r--r--   0 konsta     (501) staff       (20)     1079 2014-08-27 09:54:26.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_count_versions.py
--rw-r--r--   0 konsta     (501) staff       (20)      877 2014-12-06 08:57:22.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_is_modified.py
--rw-r--r--   0 konsta     (501) staff       (20)      440 2014-04-25 11:12:06.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_parent_class.py
--rw-r--r--   0 konsta     (501) staff       (20)      477 2014-04-25 11:22:10.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_transaction_class.py
--rw-r--r--   0 konsta     (501) staff       (20)      824 2014-04-25 11:21:06.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_tx_column_name.py
--rw-r--r--   0 konsta     (501) staff       (20)      887 2016-01-21 08:13:38.000000 SQLAlchemy-Continuum-1.3.9/tests/utils/test_version_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.627967 SQLAlchemy-Continuum-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)    17882 2023-07-12 17:01:02.000000 SQLAlchemy-Continuum-1.4.0/CHANGES.rst
+-rw-r--r--   0 root         (0) root         (0)     1480 2022-01-26 18:31:39.000000 SQLAlchemy-Continuum-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      193 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-12 17:13:17.627967 SQLAlchemy-Continuum-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.597967 SQLAlchemy-Continuum-1.4.0/SQLAlchemy_Continuum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-12 17:13:17.000000 SQLAlchemy-Continuum-1.4.0/SQLAlchemy_Continuum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4080 2023-07-12 17:13:17.000000 SQLAlchemy-Continuum-1.4.0/SQLAlchemy_Continuum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 17:13:17.000000 SQLAlchemy-Continuum-1.4.0/SQLAlchemy_Continuum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 17:13:17.000000 SQLAlchemy-Continuum-1.4.0/SQLAlchemy_Continuum.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      315 2023-07-12 17:13:17.000000 SQLAlchemy-Continuum-1.4.0/SQLAlchemy_Continuum.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-12 17:13:17.000000 SQLAlchemy-Continuum-1.4.0/SQLAlchemy_Continuum.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.597967 SQLAlchemy-Continuum-1.4.0/docs/
+-rw-r--r--   0 root         (0) root         (0)     6818 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      830 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/docs/alembic.rst
+-rw-r--r--   0 root         (0) root         (0)      757 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/docs/api.rst
+-rw-r--r--   0 root         (0) root         (0)     8420 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     5375 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/docs/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)      297 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     3468 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/docs/intro.rst
+-rw-r--r--   0 root         (0) root         (0)       41 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/docs/license.rst
+-rw-r--r--   0 root         (0) root         (0)     6729 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     1223 2022-08-28 14:29:19.000000 SQLAlchemy-Continuum-1.4.0/docs/native_versioning.rst
+-rw-r--r--   0 root         (0) root         (0)      801 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/docs/plugins.rst
+-rw-r--r--   0 root         (0) root         (0)     1714 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/docs/queries.rst
+-rw-r--r--   0 root         (0) root         (0)     2209 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/docs/revert.rst
+-rw-r--r--   0 root         (0) root         (0)     1898 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/docs/schema.rst
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-06-05 00:09:48.000000 SQLAlchemy-Continuum-1.4.0/docs/transactions.rst
+-rw-r--r--   0 root         (0) root         (0)      892 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/docs/utilities.rst
+-rw-r--r--   0 root         (0) root         (0)     6020 2023-06-09 21:50:46.000000 SQLAlchemy-Continuum-1.4.0/docs/version_objects.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 17:13:17.627967 SQLAlchemy-Continuum-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2306 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.607967 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/
+-rw-r--r--   0 root         (0) root         (0)     3244 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8541 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.607967 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/dialects/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/dialects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15473 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/dialects/postgresql.py
+-rw-r--r--   0 root         (0) root         (0)      152 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/exc.py
+-rw-r--r--   0 root         (0) root         (0)      975 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/expression_reflector.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/factory.py
+-rw-r--r--   0 root         (0) root         (0)     5839 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/fetcher.py
+-rw-r--r--   0 root         (0) root         (0)    15939 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/manager.py
+-rw-r--r--   0 root         (0) root         (0)     9815 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/model_builder.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/operation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.607967 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/
+-rw-r--r--   0 root         (0) root         (0)      322 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10607 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/activity.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/base.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2023-06-09 21:50:46.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/flask.py
+-rw-r--r--   0 root         (0) root         (0)      987 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/null_delete.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/property_mod_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     3239 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/transaction_changes.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-06-05 00:10:49.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/transaction_meta.py
+-rw-r--r--   0 root         (0) root         (0)    12703 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/relationship_builder.py
+-rw-r--r--   0 root         (0) root         (0)     4464 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/reverter.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/schema.py
+-rw-r--r--   0 root         (0) root         (0)     4672 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/table_builder.py
+-rw-r--r--   0 root         (0) root         (0)     5800 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/transaction.py
+-rw-r--r--   0 root         (0) root         (0)    10939 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/unit_of_work.py
+-rw-r--r--   0 root         (0) root         (0)    12249 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.617967 SQLAlchemy-Continuum-1.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     7955 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.617967 SQLAlchemy-Continuum-1.4.0/tests/builders/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/tests/builders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      259 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/tests/builders/test_model_builder.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/builders/test_relationship_builder.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/builders/test_table_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.617967 SQLAlchemy-Continuum-1.4.0/tests/dialects/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/tests/dialects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/dialects/test_triggers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.617967 SQLAlchemy-Continuum-1.4.0/tests/inheritance/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/tests/inheritance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      940 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/inheritance/test_common_base_class.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/inheritance/test_concrete_inheritance.py
+-rw-r--r--   0 root         (0) root         (0)     7122 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/inheritance/test_join_table_inheritance.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/inheritance/test_multi_level_inheritance.py
+-rw-r--r--   0 root         (0) root         (0)     3308 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/inheritance/test_single_table_inheritance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.617967 SQLAlchemy-Continuum-1.4.0/tests/plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:10:37.000000 SQLAlchemy-Continuum-1.4.0/tests/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6895 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/plugins/test_activity.py
+-rw-r--r--   0 root         (0) root         (0)     8227 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/plugins/test_flask.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2023-06-05 00:10:37.000000 SQLAlchemy-Continuum-1.4.0/tests/plugins/test_null_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-06-05 00:10:37.000000 SQLAlchemy-Continuum-1.4.0/tests/plugins/test_plugin_collection.py
+-rw-r--r--   0 root         (0) root         (0)     5947 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/plugins/test_property_mod_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2023-06-05 00:10:37.000000 SQLAlchemy-Continuum-1.4.0/tests/plugins/test_transaction_changes.py
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/plugins/test_transaction_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.627967 SQLAlchemy-Continuum-1.4.0/tests/relationships/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/tests/relationships/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2336 2022-09-02 22:30:07.000000 SQLAlchemy-Continuum-1.4.0/tests/relationships/test_association_table_relations.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2022-09-02 22:30:07.000000 SQLAlchemy-Continuum-1.4.0/tests/relationships/test_custom_condition_relations.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/relationships/test_dynamic_relationships.py
+-rw-r--r--   0 root         (0) root         (0)    14738 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/relationships/test_many_to_many_relations.py
+-rw-r--r--   0 root         (0) root         (0)     3291 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/relationships/test_non_versioned_classes.py
+-rw-r--r--   0 root         (0) root         (0)     9182 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/relationships/test_one_to_many_relations.py
+-rw-r--r--   0 root         (0) root         (0)     2882 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/relationships/test_one_to_one_relations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.627967 SQLAlchemy-Continuum-1.4.0/tests/revert/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/tests/revert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/revert/test_deep_relationships.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/revert/test_many_to_many_relationships.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/revert/test_one_to_one_relationship.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/revert/test_one_to_one_with_secondary_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.627967 SQLAlchemy-Continuum-1.4.0/tests/schema/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/tests/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/schema/test_update_end_transaction_id.py
+-rw-r--r--   0 root         (0) root         (0)     2955 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/schema/test_update_property_mod_flags.py
+-rw-r--r--   0 root         (0) root         (0)     8343 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/test_accessors.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/test_changeset.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.0/tests/test_column_aliases.py
+-rw-r--r--   0 root         (0) root         (0)     3661 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.0/tests/test_column_inclusion_and_exclusion.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.0/tests/test_composite_primary_key.py
+-rw-r--r--   0 root         (0) root         (0)     3660 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/test_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/test_custom_schema.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.0/tests/test_custom_version_base_class.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.0/tests/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.0/tests/test_exotic_listener_chaining.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.0/tests/test_exotic_operation_combos.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/test_i18n.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/test_insert.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.0/tests/test_mapper_args.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/test_raw_sql.py
+-rw-r--r--   0 root         (0) root         (0)     6000 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.0/tests/test_revert.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/test_savepoints.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/test_sessions.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/test_transaction.py
+-rw-r--r--   0 root         (0) root         (0)     3420 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/test_update.py
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.0/tests/test_vacuum.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/test_validity_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2023-07-12 17:09:37.000000 SQLAlchemy-Continuum-1.4.0/tests/test_validity_strategy_multithreaded.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-05 00:10:31.000000 SQLAlchemy-Continuum-1.4.0/tests/test_versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 17:13:17.627967 SQLAlchemy-Continuum-1.4.0/tests/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/tests/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      869 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/utils/test_changeset.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/utils/test_count_versions.py
+-rw-r--r--   0 root         (0) root         (0)      877 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/utils/test_is_modified.py
+-rw-r--r--   0 root         (0) root         (0)      440 2022-01-01 15:24:43.000000 SQLAlchemy-Continuum-1.4.0/tests/utils/test_parent_class.py
+-rw-r--r--   0 root         (0) root         (0)      477 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/utils/test_transaction_class.py
+-rw-r--r--   0 root         (0) root         (0)      824 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/utils/test_tx_column_name.py
+-rw-r--r--   0 root         (0) root         (0)      887 2022-08-28 14:42:37.000000 SQLAlchemy-Continuum-1.4.0/tests/utils/test_version_class.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `SQLAlchemy-Continuum-1.3.9/CHANGES.rst` & `SQLAlchemy-Continuum-1.4.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,52 @@
 Changelog
 ---------
 
 Here you can see the full list of changes between each SQLAlchemy-Continuum release.
 
+1.4.0 (2023-07-12)
+- Add support for SQLAlchemy 2.0 and remove for < 1.4
+- Using before_execute for association tracking might break stuff
+- create_trigger's signature has changed to accept session
+- change to validity logic to avoid deadlock
+- removed Operation.iteritems
+
+1.3.14 (2023-01-04)
+^^^^^^^^^^^^^^^^^^^
+
+- Undo unneeded change to Flask-Login that breaks alternative IDs (#325, thanks to anthraxx)
+
+
+1.3.13 (2022-09-07)
+^^^^^^^^^^^^^^^^^^^
+
+- Fixes for Flask 2.2 and Flask-Login 0.6.2 (#288, thanks to AbdealiJK)
+- Allow changed_entities to work without TransactionChanges plugin (#268, thanks to TomGoBravo)
+- Fix Activity plugin for non-composite primary keys not named id (#210, thanks to dryobates)
+- Allow sync_trigger to pass arguments through to create_trigger (#273, thanks to nanvel)
+- Fix association tables on Oracle (#291, thanks to AbdealiJK)
+- Fix some deprecation warnings in SA 1.4 (#269, #277, #279, #300, #302, thanks to TomGoBravo, edhaz, and indiVar0508)
+
+1.3.12 (2022-01-18)
+^^^^^^^^^^^^^^^^^^^
+
+- Support SA 1.4
+
+1.3.11 (2020-05-24)
+^^^^^^^^^^^^^^^^^^^
+
+- Made ModelBuilder create column aliases in version models (#246, courtesy of killthekitten)
+
+
+1.3.10 (2020-05-10)
+^^^^^^^^^^^^^^^^^^^
+
+- Added explicit "pseudo-backref" relationships for version/parent (#240, courtesy of lgedgar)
+- Fixed m2m Bug when an unrelated change is made to a model (#242, courtesy of Andrew-Dickinson)
+
 
 1.3.9 (2019-03-19)
 ^^^^^^^^^^^^^^^^^^
 
 - Added SA 1.3 support
 - Reverted trigger creation from 1.3.7
```

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/api.rst` & `SQLAlchemy-Continuum-1.4.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/conf.py` & `SQLAlchemy-Continuum-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/configuration.rst` & `SQLAlchemy-Continuum-1.4.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/intro.rst` & `SQLAlchemy-Continuum-1.4.0/docs/intro.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Introduction
 ------------
 
 
 Why?
 ^^^^
 
-SQLAlchemy already has a versioning extension. This extension however is very limited. It does not support versioning entire transactions.
+SQLAlchemy `already has a versioning extension <https://docs.sqlalchemy.org/en/13/orm/examples.html#module-examples.versioned_history>`_. This extension however is very limited. It does not support versioning entire transactions.
 
 Hibernate for Java has Envers, which had nice features but lacks a nice API. Ruby on Rails has papertrail_, which has very nice API but lacks the efficiency and feature set of Envers.
 
 As a Python/SQLAlchemy enthusiast I wanted to create a database versioning tool for Python with all the features of Envers and with as intuitive API as papertrail. Also I wanted to make it _fast_ keeping things as close to the database as possible.
 
 .. _papertrail:  https://github.com/airblade/paper_trail
```

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/make.bat` & `SQLAlchemy-Continuum-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/Makefile` & `SQLAlchemy-Continuum-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/native_versioning.rst` & `SQLAlchemy-Continuum-1.4.0/docs/native_versioning.rst`

 * *Files 8% similar despite different names*

```diff
@@ -26,7 +26,13 @@
 
 ::
 
     from sqlalchemy_continuum.dialects.postgresql import sync_trigger
 
 
     sync_trigger(conn, 'article_version')
+
+If you don't use `PropertyModTrackerPlugin`, then you have to disable it:
+
+::
+
+    sync_trigger(conn, 'article_version', use_property_mod_tracking=False)
```

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/plugins.rst` & `SQLAlchemy-Continuum-1.4.0/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/queries.rst` & `SQLAlchemy-Continuum-1.4.0/docs/queries.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/revert.rst` & `SQLAlchemy-Continuum-1.4.0/docs/revert.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/schema.rst` & `SQLAlchemy-Continuum-1.4.0/docs/schema.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/transactions.rst` & `SQLAlchemy-Continuum-1.4.0/docs/transactions.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/utilities.rst` & `SQLAlchemy-Continuum-1.4.0/docs/utilities.rst`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/docs/version_objects.rst` & `SQLAlchemy-Continuum-1.4.0/docs/version_objects.rst`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     version = article.versions[1]
     version.changeset
     # {
     #   'name': [u'New article', u'Updated article'],
     # }
 
     session.delete(article)
-    version = article.versions[1]
+    version = article.versions[2]
     version.changeset
     # {
     #   'id': [1, None]
     #   'name': [u'Updated article', None],
     #   'content': [u'Some content', None]
     # }
 
@@ -98,15 +98,15 @@
 
 
     from sqlalchemy_continuum import changeset
 
 
     article = Article(name=u'Some article')
     changeset(article)
-    # {'name': [u'Some article', None]}
+    # {'name': [None, u'Some article']}
 
 
 Version relationships
 ---------------------
 
 Each version object reflects all parent object relationships. You can think version object relations as 'relations of parent object in given point in time'.
```

### Comparing `SQLAlchemy-Continuum-1.3.9/LICENSE` & `SQLAlchemy-Continuum-1.4.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
 
 * Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.
 
-* The names of the contributors may not be used to endorse or promote products
-  derived from this software without specific prior written permission.
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
 ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER BE LIABLE FOR ANY DIRECT,
 INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
 BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
```

### Comparing `SQLAlchemy-Continuum-1.3.9/PKG-INFO` & `SQLAlchemy-Continuum-1.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: SQLAlchemy-Continuum
-Version: 1.3.9
+Version: 1.4.0
 Summary: Versioning and auditing extension for SQLAlchemy.
 Home-page: https://github.com/kvesteri/sqlalchemy-continuum
 Author: Konsta Vesterinen
 Author-email: konsta@fastmonkeys.com
 License: BSD
-Description: 
-        SQLAlchemy-Continuum
-        --------------------
-        
-        Versioning and auditing extension for SQLAlchemy.
-        
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: test
+Provides-Extra: flask
+Provides-Extra: flask-login
+Provides-Extra: flask-sqlalchemy
+Provides-Extra: i18n
+License-File: LICENSE
+
+
+SQLAlchemy-Continuum
+--------------------
+
+Versioning and auditing extension for SQLAlchemy.
```

### Comparing `SQLAlchemy-Continuum-1.3.9/README.rst` & `SQLAlchemy-Continuum-1.4.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -70,28 +70,60 @@
 
     # lets revert back to first version
     article.versions[0].revert()
 
     article.name
     # 'Some article'
 
+For completeness, below is a working example.
+
+.. code-block:: python
+
+    from sqlalchemy_continuum import make_versioned
+    from sqlalchemy import Column, Integer, Unicode, UnicodeText, create_engine
+    from sqlalchemy.orm import create_session, configure_mappers, declarative_base
+
+    make_versioned(user_cls=None)
+
+    Base = declarative_base()
+    class Article(Base):
+        __versioned__ = {}
+        __tablename__ = 'article'
+        id = Column(Integer, primary_key=True, autoincrement=True)
+        name = Column(Unicode(255))
+        content = Column(UnicodeText)
+
+    configure_mappers()
+    engine = create_engine('sqlite://')
+    Base.metadata.create_all(engine)
+    session = create_session(bind=engine, autocommit=False)
+
+    article = Article(name=u'Some article', content=u'Some content')
+    session.add(article)
+    session.commit()
+    article.versions[0].name
+    article.name = u'Updated name'
+    session.commit()
+    article.versions[1].name
+    article.versions[0].revert()
+    article.name
 
 Resources
 ---------
 
 - `Documentation <https://sqlalchemy-continuum.readthedocs.io/>`_
 - `Issue Tracker <http://github.com/kvesteri/sqlalchemy-continuum/issues>`_
 - `Code <http://github.com/kvesteri/sqlalchemy-continuum/>`_
 
 
 .. image:: http://i.imgur.com/UFaRx.gif
 
 
-.. |Build Status| image:: https://travis-ci.org/kvesteri/sqlalchemy-continuum.png?branch=master
-   :target: https://travis-ci.org/kvesteri/sqlalchemy-continuum
+.. |Build Status| image:: https://github.com/kvesteri/sqlalchemy-continuum/workflows/Test/badge.svg
+   :target: https://github.com/kvesteri/sqlalchemy-continuum/actions?query=workflow%3ATest
 .. |Version Status| image:: https://img.shields.io/pypi/v/SQLAlchemy-Continuum.png
    :target: https://pypi.python.org/pypi/SQLAlchemy-Continuum/
 .. |Downloads| image:: https://img.shields.io/pypi/dm/SQLAlchemy-Continuum.png
    :target: https://pypi.python.org/pypi/SQLAlchemy-Continuum/
 
 
 More information
```

### Comparing `SQLAlchemy-Continuum-1.3.9/setup.py` & `SQLAlchemy-Continuum-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,21 @@
     pattern = r"^__version__ = '(.*?)'$"
     return re.search(pattern, contents, re.MULTILINE).group(1)
 
 
 extras_require = {
     'test': [
         'pytest>=2.3.5',
-        'flexmock>=0.9.7',
         'psycopg2>=2.4.6',
-        'PyMySQL==0.6.1',
-        'six>=1.4.0'
+        'PyMySQL>=0.8.0',
     ],
-    'anyjson': ['anyjson>=0.3.3'],
     'flask': ['Flask>=0.9'],
     'flask-login': ['Flask-Login>=0.2.9'],
     'flask-sqlalchemy': ['Flask-SQLAlchemy>=1.0'],
-    'flexmock': ['flexmock>=0.9.7'],
-    'i18n': ['SQLAlchemy-i18n>=0.8.4'],
+    'i18n': ['SQLAlchemy-i18n>=0.8.4,!=1.1.0'],
 }
 
 
 # Add all optional dependencies to testing requirements.
 for name, requirements in extras_require.items():
     if name != 'test':
         extras_require['test'] += requirements
@@ -60,27 +56,27 @@
         'sqlalchemy_continuum.plugins',
         'sqlalchemy_continuum.dialects'
     ],
     zip_safe=False,
     include_package_data=True,
     platforms='any',
     install_requires=[
-        'SQLAlchemy>=1.0.8',
-        'SQLAlchemy-Utils>=0.30.12'
+        'SQLAlchemy>=1.4.0',
+        'SQLAlchemy-Utils>=0.30.12',
     ],
     extras_require=extras_require,
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ]
 )
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/__init__.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,22 +14,22 @@
     transaction_class,
     tx_column_name,
     vacuum,
     version_class,
 )
 
 
-__version__ = '1.3.9'
+__version__ = '1.4.0'
 
 
 versioning_manager = VersioningManager()
 
 
 def make_versioned(
-    mapper=sa.orm.mapper,
+    mapper=sa.orm.Mapper,
     session=sa.orm.session.Session,
     manager=versioning_manager,
     plugins=None,
     options=None,
     user_cls='User'
 ):
     """
@@ -62,15 +62,15 @@
     manager.user_cls = user_cls
     manager.apply_class_configuration_listeners(mapper)
     manager.track_operations(mapper)
     manager.track_session(session)
 
     sa.event.listen(
         sa.engine.Engine,
-        'before_cursor_execute',
+        'before_execute',
         manager.track_association_operations
     )
 
     sa.event.listen(
         sa.engine.Engine,
         'rollback',
         manager.clear_connection
@@ -80,15 +80,15 @@
         sa.engine.Engine,
         'set_connection_execution_options',
         manager.track_cloned_connections
     )
 
 
 def remove_versioning(
-    mapper=sa.orm.mapper,
+    mapper=sa.orm.Mapper,
     session=sa.orm.session.Session,
     manager=versioning_manager
 ):
     """
     Remove the versioning from given mapper / session and manager.
 
     :param mapper:
@@ -101,15 +101,15 @@
     """
     manager.reset()
     manager.remove_class_configuration_listeners(mapper)
     manager.remove_operations_tracking(mapper)
     manager.remove_session_tracking(session)
     sa.event.remove(
         sa.engine.Engine,
-        'before_cursor_execute',
+        'before_execute',
         manager.track_association_operations
     )
 
     sa.event.remove(
         sa.engine.Engine,
         'rollback',
         manager.clear_connection
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/dialects/postgresql.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/dialects/postgresql.py`

 * *Files 7% similar despite different names*

```diff
@@ -452,52 +452,52 @@
         sa.schema.DDL(
             'DROP FUNCTION IF EXISTS %s()' %
             '%s_audit' % cls.__table__.name,
         )
     )
 
 
-def sync_trigger(conn, table_name):
+def sync_trigger(session, table_name, **kwargs):
     """
-    Synchronizes versioning trigger for given table with given connection.
+    Synchronizes versioning trigger for given table with given session.
 
     ::
 
 
-        sync_trigger(conn, 'my_table')
+        sync_trigger(session, 'my_table')
+        session.commit()
 
 
-    :param conn: SQLAlchemy connection object
+    :param session: SQLAlchemy session object
     :param table_name: Name of the table to synchronize versioning trigger for
+    :params **kwargs: kwargs to pass to create_trigger
 
     .. versionadded: 1.1.0
     """
     meta = sa.MetaData()
     version_table = sa.Table(
         table_name,
         meta,
-        autoload=True,
-        autoload_with=conn
+        autoload_with=session.connection()
     )
     parent_table = sa.Table(
         table_name[0:-len('_version')],
         meta,
-        autoload=True,
-        autoload_with=conn
+        autoload_with=session.connection()
     )
     excluded_columns = (
         set(c.name for c in parent_table.c) -
         set(c.name for c in version_table.c if not c.name.endswith('_mod'))
     )
-    drop_trigger(conn, parent_table.name)
-    create_trigger(conn, table=parent_table, excluded_columns=excluded_columns)
+    drop_trigger(session, parent_table.name)
+    create_trigger(session, table=parent_table, excluded_columns=excluded_columns, **kwargs)
 
 
 def create_trigger(
-    conn,
+    session,
     table,
     transaction_column_name='transaction_id',
     operation_type_column_name='operation_type',
     version_table_name_format='%s_version',
     excluded_columns=None,
     use_property_mod_tracking=True,
     end_transaction_column_name=None,
@@ -508,19 +508,19 @@
         transaction_column_name=transaction_column_name,
         operation_type_column_name=operation_type_column_name,
         version_table_name_format=version_table_name_format,
         excluded_columns=excluded_columns,
         use_property_mod_tracking=use_property_mod_tracking,
         end_transaction_column_name=end_transaction_column_name,
     )
-    conn.execute(str(CreateTriggerFunctionSQL(**params)))
-    conn.execute(str(CreateTriggerSQL(**params)))
+    session.execute(sa.text(str(CreateTriggerFunctionSQL(**params))))
+    session.execute(sa.text(str(CreateTriggerSQL(**params))))
 
 
-def drop_trigger(conn, table_name):
-    conn.execute(
+def drop_trigger(session, table_name):
+    session.execute(sa.text(
         'DROP TRIGGER IF EXISTS %s_trigger ON "%s"' % (
             table_name,
             table_name
         )
-    )
-    conn.execute('DROP FUNCTION IF EXISTS %s_audit()' % table_name)
+    ))
+    session.execute(sa.text('DROP FUNCTION IF EXISTS %s_audit()' % table_name))
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/expression_reflector.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/expression_reflector.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/fetcher.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/fetcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,30 +55,30 @@
             op = operator.gt
             func = sa.func.min
         else:
             op = operator.lt
             func = sa.func.max
 
         if alias is None:
-            alias = sa.orm.aliased(obj)
+            alias = sa.orm.aliased(obj.__class__)
             table = alias.__table__
             if hasattr(alias, 'c'):
                 attrs = alias.c
             else:
                 attrs = alias
         else:
             table = alias.original
             attrs = alias.c
         query = (
             sa.select(
-                [func(
+                func(
                     getattr(attrs, tx_column_name(obj))
-                )],
-                from_obj=[table]
+                )
             )
+            .select_from(table)
             .where(
                 sa.and_(
                     op(
                         getattr(attrs, tx_column_name(obj)),
                         getattr(obj, tx_column_name(obj))
                     ),
                     *[
@@ -86,55 +86,56 @@
                         for pk in get_primary_keys(obj.__class__)
                         if pk != tx_column_name(obj)
                     ]
                 )
             )
             .correlate(table)
         )
-        return query
+        return query.scalar_subquery()
 
     def _next_prev_query(self, obj, next_or_prev='next'):
         session = sa.orm.object_session(obj)
 
+        subquery = self._transaction_id_subquery(
+            obj, next_or_prev=next_or_prev
+        )
+        subquery = subquery.scalar_subquery()
+
         return (
             session.query(obj.__class__)
             .filter(
                 sa.and_(
                     getattr(
                         obj.__class__,
                         tx_column_name(obj)
-                    )
-                    ==
-                    self._transaction_id_subquery(
-                        obj, next_or_prev=next_or_prev
-                    ),
+                    ) == subquery,
                     *parent_criteria(obj)
                 )
             )
         )
 
     def _index_query(self, obj):
         """
         Returns the query needed for fetching the index of this record relative
         to version history.
         """
-        alias = sa.orm.aliased(obj)
+        alias = sa.orm.aliased(obj.__class__)
 
         subquery = (
-            sa.select([sa.func.count('1')], from_obj=[alias.__table__])
+            sa.select(sa.func.count()).select_from(alias.__table__)
             .where(
                 getattr(alias, tx_column_name(obj))
                 <
                 getattr(obj, tx_column_name(obj))
             )
             .correlate(alias.__table__)
             .label('position')
         )
         query = (
-            sa.select([subquery], from_obj=[obj.__table__])
+            sa.select(subquery).select_from(obj.__table__)
             .where(
                 sa.and_(*eqmap(identity, (obj.__class__, obj)))
             )
             .order_by(
                 getattr(obj.__class__, tx_column_name(obj))
             )
         )
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/manager.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,36 +7,24 @@
 
 from .builder import Builder
 from .fetcher import SubqueryFetcher, ValidityFetcher
 from .operation import Operation
 from .plugins import PluginCollection
 from .transaction import TransactionFactory
 from .unit_of_work import UnitOfWork
-from .utils import is_modified, is_versioned
+from .utils import is_modified, is_versioned, version_table
 
 
 def tracked_operation(func):
     @wraps(func)
     def wrapper(self, mapper, connection, target):
         if not is_versioned(target):
             return
         session = object_session(target)
-        conn = session.connection()
-        try:
-            uow = self.units_of_work[conn]
-        except KeyError:
-            try:
-                uow = self.units_of_work[conn.engine]
-            except KeyError:
-                for connection in self.units_of_work.keys():
-                    if not connection.closed and connection.connection is conn.connection:
-                        uow = self.unit_of_work(session)
-                        break  # The ConnectionFairy is the same, this connection is a clone
-                else:
-                    raise
+        uow = self._uow_from_conn(session.connection())
         return func(self, uow, target)
     return wrapper
 
 
 class VersioningManager(object):
     """
     VersioningManager delegates versioning configuration operations to builder
@@ -321,14 +309,30 @@
         if conn in self.units_of_work:
             return self.units_of_work[conn]
         else:
             uow = self.uow_class(self)
             self.units_of_work[conn] = uow
             return uow
 
+    def _uow_from_conn(self, conn):
+        try:
+            uow = self.units_of_work[conn]
+        except KeyError:
+            try:
+                uow = self.units_of_work[conn.engine]
+            except KeyError:
+                for connection in self.units_of_work.keys():
+                    if not connection.closed and connection.connection is conn.connection:
+                        uow = self.unit_of_work(session)
+                        break  # The ConnectionFairy is the same, this connection is a clone
+                else:
+                    raise
+
+        return uow
+
     def before_flush(self, session, flush_context, instances):
         """
         Before flush listener for SQLAlchemy sessions. If this manager has
         versioning enabled this listener invokes the process before flush of
         associated UnitOfWork object.
 
         :param session: SQLAlchemy session
@@ -358,15 +362,15 @@
         Simple SQLAlchemy listener that is being invoked after successful
         transaction commit or when transaction rollback occurs. The purpose of
         this listener is to reset this UnitOfWork back to its initialization
         state.
 
         :param session: SQLAlchemy session object
         """
-        if session.transaction.nested:
+        if session.in_nested_transaction():
             return
         conn = self.session_connection_map.pop(session, None)
         if conn is None:
             return
 
         if conn in self.units_of_work:
             uow = self.units_of_work[conn]
@@ -398,115 +402,54 @@
                 del self.units_of_work[connection]
 
 
     def append_association_operation(self, conn, table_name, params, op):
         """
         Append history association operation to pending_statements list.
         """
-        params['operation_type'] = op
         stmt = (
             self.metadata.tables[self.options['table_name'] % table_name]
             .insert()
-            .values(params)
+            .values({**params, 'operation_type': op})
         )
-        try:
-            uow = self.units_of_work[conn]
-        except KeyError:
-            try:
-                uow = self.units_of_work[conn.engine]
-            except KeyError:
-                for connection in self.units_of_work.keys():
-                    if not connection.closed and connection.connection is conn.connection:
-                        uow = self.unit_of_work(conn.session)
-                        break  # The ConnectionFairy is the same, this connection is a clone
-                else:
-                    raise
+        uow = self.uow_from_conn(conn)
         uow.pending_statements.append(stmt)
 
     def track_cloned_connections(self, c, opt):
         """
         Track cloned connections from association tables.
         """
         if c not in self.units_of_work.keys():
             for connection, uow in dict(self.units_of_work).items():
                 if not connection.closed and connection.connection is c.connection:  # ConnectionFairy is the same - this is a clone
                     self.units_of_work[c] = uow
 
     def track_association_operations(
-        self, conn, cursor, statement, parameters, context, executemany
+        self, conn, clauseelement, multiparams, params, execution_options,
     ):
-        """
-        Track association operations and adds the generated history
-        association operations to pending_statements list.
-        """
+
         if (
             not self.options['versioning'] and
             not self.options['native_versioning']
         ):
             return
 
-        op = None
-        if context.isinsert:
+        if clauseelement.is_insert:
             op = Operation.INSERT
-        elif context.isdelete:
+        elif clauseelement.is_delete:
             op = Operation.DELETE
+        else:
+            op = None
+
+        if op is not None and clauseelement.table in self.association_tables:
+            if not multiparams:
+                multiparams = [params]
+
+            uow = self._uow_from_conn(conn)
+
+            for params in multiparams:
+                stmt = version_table(clauseelement.table).insert().values({
+                    **params,
+                    'operation_type': op,
+                })
+                uow.pending_statements.append(stmt)
 
-        if op is not None:
-            table_name = statement.split(' ')[2]
-            table_names = [
-                table.name if not table.schema else table.schema + '.' + table.name
-                for table in self.association_tables
-            ]
-            if table_name in table_names:
-                if executemany:
-                    # SQLAlchemy does not support function based values for
-                    # multi-inserts, hence we need to convert the orignal
-                    # multi-insert into batch of normal inserts
-                    for params in parameters:
-                        self.append_association_operation(
-                            conn,
-                            table_name,
-                            self.positional_args_to_dict(
-                                op, statement, params
-                            ),
-                            op
-                        )
-                else:
-                    self.append_association_operation(
-                        conn,
-                        table_name,
-                        self.positional_args_to_dict(
-                            op,
-                            statement,
-                            parameters
-                        ),
-                        op
-                    )
-
-    def positional_args_to_dict(self, op, statement, params):
-        """
-        On some drivers (eg sqlite) generated INSERT statements use positional
-        args instead of key value dictionary. This method converts positional
-        args to key value dict.
-
-        :param statement: SQL statement string
-        :param params: tuple or dict of statement parameters
-        """
-        if isinstance(params, tuple):
-            parameters = {}
-            if op == Operation.DELETE:
-                regexp = '^DELETE FROM (.+?) WHERE'
-                match = re.match(regexp, statement)
-                tablename = match.groups()[0].strip('"').strip("'").strip('`')
-                table = self.metadata.tables[tablename]
-                columns = table.primary_key.columns.values()
-                for index, column in enumerate(columns):
-                    parameters[column.name] = params[index]
-            else:
-                columns = [
-                    column.strip() for column in
-                    statement.split('(')[1].split(')')[0].split(',')
-                ]
-                for index, column in enumerate(columns):
-                    parameters[column] = params[index]
-            return parameters
-        return params
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/model_builder.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/model_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from copy import copy
-import six
 import sqlalchemy as sa
 from sqlalchemy.ext.declarative import declared_attr
 from sqlalchemy.orm import column_property
 from sqlalchemy_utils.functions import get_declarative_base
 
 from .utils import adapt_columns, option
 from .version import VersionClassBase
@@ -67,20 +66,20 @@
                     model.__mapper_args__[arg]
                 )
 
         if 'order_by' in model.__mapper_args__:
             arg = model.__mapper_args__['order_by']
             # Only allow string based order_by reflection to version
             # classes.
-            if isinstance(arg, six.string_types):
+            if isinstance(arg, str):
                 args['order_by'] = arg
 
         if 'polymorphic_on' in model.__mapper_args__:
             column = model.__mapper_args__['polymorphic_on']
-            if isinstance(column, six.string_types):
+            if isinstance(column, str):
                 args['polymorphic_on'] = column
             else:
                 args['polymorphic_on'] = column.key
     return args
 
 
 class ModelBuilder(object):
@@ -103,42 +102,53 @@
         """
         Builds a relationship between currently built version class and
         parent class (the model whose history the currently build version
         class represents).
         """
         conditions = []
         foreign_keys = []
+        model_keys = []
         for key, column in sa.inspect(self.model).columns.items():
             if column.primary_key:
                 conditions.append(
                     getattr(self.model, key)
                     ==
                     getattr(self.version_class, key)
                 )
                 foreign_keys.append(
                     getattr(self.version_class, key)
                 )
+                model_keys.append(
+                    getattr(self.model, key)
+                )
 
         # We need to check if versions relation was already set for parent
         # class.
         if not hasattr(self.model, 'versions'):
             self.model.versions = sa.orm.relationship(
                 self.version_class,
                 primaryjoin=sa.and_(*conditions),
                 foreign_keys=foreign_keys,
                 order_by=lambda: getattr(
                     self.version_class,
                     option(self.model, 'transaction_column_name')
                 ),
                 lazy='dynamic',
-                backref=sa.orm.backref(
-                    'version_parent'
-                ),
                 viewonly=True
             )
+            # We must explicitly declare this relationship, instead of
+            # specifying as a backref to the one above, since they are
+            # viewonly=True and SQLAlchemy will warn if using backref.
+            self.version_class.version_parent = sa.orm.relationship(
+                self.model,
+                primaryjoin=sa.and_(*conditions),
+                foreign_keys=model_keys,
+                viewonly=True,
+                uselist=False,
+            )
 
     def build_transaction_relationship(self, tx_class):
         """
         Builds a relationship between currently built version class and
         Transaction class.
 
         :param tx_class: Transaction class
@@ -257,14 +267,15 @@
                 self.model.__module__.title().replace('.', ''),
                 self.model.__name__
             )
         else:
             name = '%sVersion' % (self.model.__name__,)
         return type(name, self.base_classes(), args)
 
+
     def __call__(self, table, tx_class):
         """
         Build history model and relationships to parent model, transaction
         log model.
         """
         # versioned attributes need to be copied for each child class,
         # otherwise each child class would share the same __versioned__
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/operation.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/operation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 from copy import copy
-try:
-    from collections import OrderedDict
-except ImportError:
-    from ordereddict import OrderedDict
+from collections import OrderedDict
 
-import six
 import sqlalchemy as sa
 from sqlalchemy_utils import identity
 
 
 class Operation(object):
     INSERT = 0
     UPDATE = 1
@@ -65,18 +61,15 @@
     @property
     def entities(self):
         """
         Return a set of changed versioned entities for given session.
 
         :param session: SQLAlchemy session object
         """
-        return set(key[0] for key, _ in self.iteritems())
-
-    def iteritems(self):
-        return six.iteritems(self.objects)
+        return set(k[0] for k in self.objects)
 
     def items(self):
         return self.objects.items()
 
     def add(self, operation):
         self[self.format_key(operation.target)] = operation
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/activity.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,15 @@
     http://www.activitystrea.ms
 .. _generic relationships:
     https://sqlalchemy-utils.readthedocs.io/en/latest/generic_relationship.html
 """
 
 import sqlalchemy as sa
 from sqlalchemy.ext.hybrid import hybrid_property
+from sqlalchemy.inspection import inspect
 from sqlalchemy_utils import JSONType, generic_relationship
 
 from .base import Plugin
 from ..factory import ModelFactory
 from ..utils import version_class, version_obj
 
 
@@ -250,19 +251,21 @@
             def _calculate_tx_id(self, obj):
                 session = sa.orm.object_session(self)
                 if obj:
                     object_version = version_obj(session, obj)
                     if object_version:
                         return object_version.transaction_id
 
-                    version_cls = version_class(obj.__class__)
+                    model = obj.__class__
+                    version_cls = version_class(model)
+                    primary_key = inspect(model).primary_key[0].name
                     return session.query(
                         sa.func.max(version_cls.transaction_id)
                     ).filter(
-                        version_cls.id == obj.id
+                        getattr(version_cls, primary_key) == getattr(obj, primary_key)
                     ).scalar()
 
             def calculate_object_tx_id(self):
                 self.object_tx_id = self._calculate_tx_id(self.object)
 
             def calculate_target_tx_id(self):
                 self.target_tx_id = self._calculate_tx_id(self.target)
@@ -310,14 +313,16 @@
             ),
             foreign_keys=[Activity.transaction_id]
         )
         return Activity
 
 
 class ActivityPlugin(Plugin):
+    activity_cls = None
+    
     def after_build_models(self, manager):
         self.activity_cls = ActivityFactory()(manager)
         manager.activity_cls = self.activity_cls
 
     def is_session_modified(self, session):
         """
         Return that the session has been modified if the session contains an
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/base.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/base.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/flask.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/flask.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/null_delete.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/null_delete.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/property_mod_tracker.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/property_mod_tracker.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/transaction_changes.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/transaction_changes.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 ================    =================
 transaction_id          entity_name
 ----------------    -----------------
 233678                  User
 233678                  Article
 ================    =================
 """
-import six
 import sqlalchemy as sa
 
 from .base import Plugin
 from ..factory import ModelFactory
 from ..utils import option
 
 
@@ -71,20 +70,22 @@
         self.model_class = TransactionChangesFactory()(manager)
 
     def after_build_models(self, manager):
         self.model_class = TransactionChangesFactory()(manager)
 
     def before_create_version_objects(self, uow, session):
         for entity in uow.operations.entities:
-            params = uow.current_transaction.id, six.text_type(entity.__name__)
+            if not hasattr(entity, '__name__'):
+                breakpoint()
+            params = uow.current_transaction.id, str(entity.__name__)
             changes = session.query(self.model_class).get(params)
             if not changes:
                 changes = self.model_class(
                     transaction_id=uow.current_transaction.id,
-                    entity_name=six.text_type(entity.__name__)
+                    entity_name=str(entity.__name__)
                 )
                 session.add(changes)
 
     def clear(self):
         self.objects = None
 
     def after_rollback(self, uow, session):
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/plugins/transaction_meta.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/plugins/transaction_meta.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/relationship_builder.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/relationship_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,15 @@
         primary_keys = [
             getattr(remote_alias, column.name) for column
             in sa.inspect(remote_alias).mapper.columns
             if column.primary_key and column.name != tx_column
         ]
 
         return sa.exists(
-            sa.select(
-                [1]
-            ).where(
+            sa.select(1).where(
                 sa.and_(
                     getattr(remote_alias, tx_column) <=
                     getattr(obj, tx_column),
                     *[
                         getattr(remote_alias, pk.name) ==
                         getattr(self.remote_cls, pk.name)
                         for pk in primary_keys
@@ -43,26 +41,26 @@
                 getattr(self.remote_cls, tx_column)
             ).correlate(self.local_cls, self.remote_cls)
         )
 
     def many_to_one_subquery(self, obj):
         tx_column = option(obj, 'transaction_column_name')
         reflector = VersionExpressionReflector(obj, self.property)
-
-        return getattr(self.remote_cls, tx_column) == (
-            sa.select(
-                [sa.func.max(getattr(self.remote_cls, tx_column))]
-            ).where(
-                sa.and_(
-                    getattr(self.remote_cls, tx_column) <=
-                    getattr(obj, tx_column),
-                    reflector(self.property.primaryjoin)
-                )
+        subquery = sa.select(
+            sa.func.max(getattr(self.remote_cls, tx_column))
+        ).where(
+            sa.and_(
+                getattr(self.remote_cls, tx_column) <=
+                getattr(obj, tx_column),
+                reflector(self.property.primaryjoin)
             )
         )
+        subquery = subquery.scalar_subquery()
+
+        return getattr(self.remote_cls, tx_column) == subquery
 
     def query(self, obj):
         session = sa.orm.object_session(obj)
         return (
             session.query(self.remote_cls)
             .filter(
                 self.criteria(obj)
@@ -245,57 +243,57 @@
             AND tag_id = tags_version.id
             AND operation_type != 2
             AND EXISTS (
                 SELECT 1
                 FROM article_tag_version as article_tag_version2
                 WHERE article_tag_version2.tag_id = article_tag_version.tag_id
                 AND article_tag_version2.tx_id <=5
+                AND article_tag_version2.article_id = 3
                 GROUP BY article_tag_version2.tag_id
                 HAVING
                     MAX(article_tag_version2.tx_id) =
                     article_tag_version.tx_id
             )
         )
 
         :param obj: SQLAlchemy declarative object
         """
 
         tx_column = option(obj, 'transaction_column_name')
+        join_column = self.property.primaryjoin.right.name
+        object_join_column = self.property.primaryjoin.left.name
         reflector = VersionExpressionReflector(obj, self.property)
 
         association_table_alias = self.association_version_table.alias()
         association_cols = [
             association_table_alias.c[association_col.name]
             for _, association_col
             in self.remote_to_association_column_pairs
         ]
 
         association_exists = sa.exists(
-            sa.select(
-                [1]
-            ).where(
+            sa.select(1).where(
                 sa.and_(
                     association_table_alias.c[tx_column] <=
                     getattr(obj, tx_column),
+                    association_table_alias.c[join_column] == getattr(obj, object_join_column),
                     *[association_col ==
                       self.association_version_table.c[association_col.name]
                       for association_col
                       in association_cols]
                 )
             ).group_by(
                 *association_cols
             ).having(
                 sa.func.max(association_table_alias.c[tx_column]) ==
                 self.association_version_table.c[tx_column]
             ).correlate(self.association_version_table)
         )
         return sa.exists(
-            sa.select(
-                [1]
-            ).where(
+            sa.select(1).where(
                 sa.and_(
                     reflector(self.property.primaryjoin),
                     association_exists,
                     self.association_version_table.c.operation_type !=
                     Operation.DELETE,
                     adapt_columns(self.property.secondaryjoin),
                 )
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/reverter.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/reverter.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/schema.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,33 +10,35 @@
     v1 = sa.alias(table, name='v')
     v2 = sa.alias(table, name='v2')
     v3 = sa.alias(table, name='v3')
 
     primary_keys = [c.name for c in table.c if c.primary_key]
 
     tx_criterion = sa.select(
-        [sa.func.min(getattr(v3.c, tx_column_name))]
+        sa.func.min(getattr(v3.c, tx_column_name))
     ).where(
         sa.and_(
             getattr(v3.c, tx_column_name) > getattr(v1.c, tx_column_name),
             *[
                 getattr(v3.c, pk) == getattr(v1.c, pk)
                 for pk in primary_keys
                 if pk != tx_column_name
             ]
         )
     )
-    return sa.select(
-        columns=[
-            getattr(v1.c, column)
-            for column in primary_keys
-        ] + [
-            getattr(v2.c, tx_column_name).label(end_tx_column_name)
-        ],
-        from_obj=v1.outerjoin(
+    tx_criterion = tx_criterion.scalar_subquery()
+
+    columns = [
+        getattr(v1.c, column)
+        for column in primary_keys
+    ]
+    columns += [getattr(v2.c, tx_column_name).label(end_tx_column_name)]
+
+    return sa.select(*columns).select_from(
+        v1.outerjoin(
             v2,
             sa.and_(
                 getattr(v2.c, tx_column_name) ==
                 tx_criterion
             )
         )
     ).order_by(getattr(v1.c, tx_column_name))
@@ -70,27 +72,27 @@
         conn = op.get_bind()
 
     query = get_end_tx_column_query(
         table,
         end_tx_column_name=end_tx_column_name,
         tx_column_name=tx_column_name
     )
-    stmt = conn.execute(query)
+    result = conn.execute(query)
     primary_keys = [c.name for c in table.c if c.primary_key]
-    for row in stmt:
-        if row[end_tx_column_name]:
+    for row in result:
+        if getattr(row, end_tx_column_name):
             criteria = [
-                getattr(table.c, pk) == row[pk]
+                getattr(table.c, pk) == getattr(row, pk)
                 for pk in primary_keys
             ]
 
             update_stmt = (
                 table.update()
                 .where(sa.and_(*criteria))
-                .values({end_tx_column_name: row[end_tx_column_name]})
+                .values({end_tx_column_name: getattr(row, end_tx_column_name)})
             )
             conn.execute(update_stmt)
 
 
 def get_property_mod_flags_query(
     table,
     tracked_columns,
@@ -98,26 +100,27 @@
     end_tx_column_name='end_transaction_id',
     tx_column_name='transaction_id',
 ):
     v1 = sa.alias(table, name='v')
     v2 = sa.alias(table, name='v2')
     primary_keys = [c.name for c in table.c if c.primary_key]
 
-    return sa.select(
-        columns=[
-            getattr(v1.c, column)
-            for column in primary_keys
-        ] + [
-            (sa.or_(
-                getattr(v1.c, column) != getattr(v2.c, column),
-                getattr(v2.c, tx_column_name).is_(None)
-            )).label(column + mod_suffix)
-            for column in tracked_columns
-        ],
-        from_obj=v1.outerjoin(
+    columns = [
+        getattr(v1.c, column)
+        for column in primary_keys
+    ]
+    columns += [
+        (sa.or_(
+            getattr(v1.c, column) != getattr(v2.c, column),
+            getattr(v2.c, tx_column_name).is_(None)
+        )).label(column + mod_suffix)
+        for column in tracked_columns
+    ]
+    return sa.select(*columns).select_from(
+        v1.outerjoin(
             v2,
             sa.and_(
                 getattr(v2.c, end_tx_column_name) ==
                 getattr(v1.c, tx_column_name),
                 *[
                     getattr(v2.c, pk) == getattr(v1.c, pk)
                     for pk in primary_keys
@@ -161,22 +164,22 @@
     query = get_property_mod_flags_query(
         table,
         tracked_columns,
         mod_suffix=mod_suffix,
         end_tx_column_name=end_tx_column_name,
         tx_column_name=tx_column_name,
     )
-    stmt = conn.execute(query)
+    result = conn.execute(query)
 
     primary_keys = [c.name for c in table.c if c.primary_key]
-    for row in stmt:
+    for row in result:
         values = dict([
-            (column + mod_suffix, row[column + mod_suffix])
+            (column + mod_suffix, getattr(row, column + mod_suffix))
             for column in tracked_columns
-            if row[column + mod_suffix]
+            if getattr(row, column + mod_suffix)
         ])
         if values:
             criteria = [
-                getattr(table.c, pk) == row[pk] for pk in primary_keys
+                getattr(table.c, pk) == getattr(row, pk) for pk in primary_keys
             ]
             query = table.update().where(sa.and_(*criteria)).values(values)
             conn.execute(query)
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/table_builder.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/table_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,17 @@
 
     def reflect_column(self, column):
         """
         Make a copy of parent table column and some alterations to it.
 
         :param column: SQLAlchemy Column object of parent table
         """
-        # Make a copy of the column so that it does not point to wrong
-        # table.
-        column_copy = column.copy()
-        # Remove unique constraints
+        # Make a copy of the column so that it does not point to wrong table.
+        column_copy = column._copy()
         column_copy.unique = False
-        # Remove onupdate triggers
         column_copy.onupdate = None
         if column_copy.autoincrement:
             column_copy.autoincrement = False
         if column_copy.name == self.option('transaction_column_name'):
             column_copy.nullable = False
 
         if not column_copy.primary_key:
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/transaction.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/transaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from datetime import datetime
 from functools import partial
 
-try:
-    from collections import OrderedDict
-except ImportError:
-    from ordereddict import OrderedDict
-import six
+from collections import OrderedDict
 import sqlalchemy as sa
 from sqlalchemy.ext.compiler import compiles
 
 from .dialects.postgresql import (
     CreateTemporaryTransactionTableSQL,
     InsertTemporaryTransactionSQL,
     TransactionTriggerSQL
@@ -19,23 +15,32 @@
 
 
 @compiles(sa.types.BigInteger, 'sqlite')
 def compile_big_integer(element, compiler, **kw):
     return 'INTEGER'
 
 
+class NoChangesAttribute(Exception):
+    pass
+
+
 class TransactionBase(object):
     issued_at = sa.Column(sa.DateTime, default=datetime.utcnow)
 
     @property
     def entity_names(self):
         """
         Return a list of entity names that changed during this transaction.
+        Raises a NoChangesAttribute exception if the 'changes' column does
+        not exist, most likely because TransactionChangesPlugin is not enabled.
         """
-        return [changes.entity_name for changes in self.changes]
+        if hasattr(self, 'changes'):
+          return [changes.entity_name for changes in self.changes]
+        else:
+          raise NoChangesAttribute()
 
     @property
     def changed_entities(self):
         """
         Return all changed entities for this transaction log entry.
 
         Entities are returned as a dict where keys are entity classes and
@@ -44,16 +49,19 @@
         manager = self.__versioning_manager__
         tuples = set(manager.version_class_map.items())
         entities = {}
 
         session = sa.orm.object_session(self)
 
         for class_, version_class in tuples:
-            if class_.__name__ not in self.entity_names:
-                continue
+            try:
+                if class_.__name__ not in self.entity_names:
+                    continue
+            except NoChangesAttribute:
+                pass
 
             tx_column = manager.option(class_, 'transaction_column_name')
 
             entities[version_class] = (
                 session
                 .query(version_class)
                 .filter(getattr(version_class, tx_column) == self.id)
@@ -128,17 +136,18 @@
             )
 
             if self.remote_addr:
                 remote_addr = sa.Column(sa.String(50))
 
             if manager.user_cls:
                 user_cls = manager.user_cls
-                registry = manager.declarative_base._decl_class_registry
+                Base = manager.declarative_base
+                registry = Base.registry._class_registry
 
-                if isinstance(user_cls, six.string_types):
+                if isinstance(user_cls, str):
                     try:
                         user_cls = registry[user_cls]
                     except KeyError:
                         raise ImproperlyConfigured(
                             'Could not build relationship between Transaction'
                             ' and %s. %s was not found in declarative class '
                             'registry. Either configure VersioningManager to '
@@ -160,15 +169,15 @@
                     (field, getattr(self, field))
                     for field in fields
                     if hasattr(self, field)
                 )
                 return '<Transaction %s>' % ', '.join(
                     (
                         '%s=%r' % (field, value)
-                        if not isinstance(value, six.integer_types)
+                        if not isinstance(value, int)
                         # We want the following line to ensure that longs get
                         # shown without the ugly L suffix on python 2.x
                         # versions
                         else '%s=%d' % (field, value)
                         for field, value in field_values.items()
                     )
                 )
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/unit_of_work.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/unit_of_work.py`

 * *Files 3% similar despite different names*

```diff
@@ -218,21 +218,14 @@
         session = sa.orm.object_session(version_obj)
 
         subquery = fetcher._transaction_id_subquery(
             version_obj,
             next_or_prev='prev',
             alias=alias
         )
-        if session.connection().engine.dialect.name == 'mysql':
-            return sa.select(
-                [sa.text('max_1')],
-                from_obj=[
-                    sa.sql.expression.alias(subquery, name='subquery')
-                ]
-            )
         return subquery
 
     def update_version_validity(self, parent, version_obj):
         """
         Updates previous version object end_transaction_id based on given
         parent object and newly created version object.
 
@@ -249,38 +242,35 @@
             if class_ in self.manager.parent_class_map:
 
                 subquery = self.version_validity_subquery(
                     parent,
                     version_obj,
                     alias=sa.orm.aliased(class_.__table__)
                 )
+                subquery = subquery.scalar_subquery()
+
+                vobj_tx_col = getattr(class_, tx_column_name(version_obj))
                 query = (
-                    session.query(class_.__table__)
-                    .filter(
-                        sa.and_(
-                            getattr(
-                                class_,
-                                tx_column_name(version_obj)
-                            ) == subquery,
-                            *[
-                                getattr(version_obj, pk) ==
-                                getattr(class_.__table__.c, pk)
-                                for pk in get_primary_keys(class_)
-                                if pk != tx_column_name(class_)
-                            ]
-                        )
+                    sa.select(class_)
+                    .where(
+                        vobj_tx_col == subquery,
+                        *[
+                            getattr(version_obj, pk) ==
+                            getattr(class_.__table__.c, pk)
+                            for pk in get_primary_keys(class_)
+                            if pk != tx_column_name(class_)
+                        ]
                     )
+                    .execution_options(synchronize_session=False)
                 )
-                query.update(
-                    {
-                        end_tx_column_name(version_obj):
-                        self.current_transaction.id
-                    },
-                    synchronize_session=False
-                )
+
+                old_versions = session.scalars(query).all()
+                for old_version in old_versions:
+                    setattr(old_version, end_tx_column_name(version_obj), self.current_transaction.id)
+
 
     def create_association_versions(self, session):
         """
         Creates association table version records for given session.
 
         :param session: SQLAlchemy session object
         """
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/utils.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,18 +388,18 @@
         return 0
     manager = get_versioning_manager(obj)
     table_name = manager.option(obj, 'table_name') % obj.__table__.name
     criteria = [
         '%s = %r' % (pk, getattr(obj, pk))
         for pk in get_primary_keys(obj)
     ]
-    query = 'SELECT COUNT(1) FROM %s WHERE %s' % (
+    query = sa.text('SELECT COUNT(1) FROM %s WHERE %s' % (
         table_name,
         ' AND '.join(criteria)
-    )
+    ))
     return session.execute(query).scalar()
 
 
 def changeset(obj):
     """
     Return a humanized changeset for given SQLAlchemy declarative object. With
     this function you can easily check the changeset of given object in current
```

### Comparing `SQLAlchemy-Continuum-1.3.9/sqlalchemy_continuum/version.py` & `SQLAlchemy-Continuum-1.4.0/sqlalchemy_continuum/version.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/PKG-INFO` & `SQLAlchemy-Continuum-1.4.0/SQLAlchemy_Continuum.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: SQLAlchemy-Continuum
-Version: 1.3.9
+Version: 1.4.0
 Summary: Versioning and auditing extension for SQLAlchemy.
 Home-page: https://github.com/kvesteri/sqlalchemy-continuum
 Author: Konsta Vesterinen
 Author-email: konsta@fastmonkeys.com
 License: BSD
-Description: 
-        SQLAlchemy-Continuum
-        --------------------
-        
-        Versioning and auditing extension for SQLAlchemy.
-        
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: test
+Provides-Extra: flask
+Provides-Extra: flask-login
+Provides-Extra: flask-sqlalchemy
+Provides-Extra: i18n
+License-File: LICENSE
+
+
+SQLAlchemy-Continuum
+--------------------
+
+Versioning and auditing extension for SQLAlchemy.
```

### Comparing `SQLAlchemy-Continuum-1.3.9/SQLAlchemy_Continuum.egg-info/SOURCES.txt` & `SQLAlchemy-Continuum-1.4.0/SQLAlchemy_Continuum.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 setup.py
 SQLAlchemy_Continuum.egg-info/PKG-INFO
 SQLAlchemy_Continuum.egg-info/SOURCES.txt
 SQLAlchemy_Continuum.egg-info/dependency_links.txt
 SQLAlchemy_Continuum.egg-info/not-zip-safe
 SQLAlchemy_Continuum.egg-info/requires.txt
 SQLAlchemy_Continuum.egg-info/top_level.txt
-docs/.DS_Store
 docs/Makefile
 docs/alembic.rst
 docs/api.rst
 docs/conf.py
 docs/configuration.rst
 docs/index.rst
 docs/intro.rst
@@ -73,14 +72,15 @@
 tests/test_revert.py
 tests/test_savepoints.py
 tests/test_sessions.py
 tests/test_transaction.py
 tests/test_update.py
 tests/test_vacuum.py
 tests/test_validity_strategy.py
+tests/test_validity_strategy_multithreaded.py
 tests/test_versions.py
 tests/builders/__init__.py
 tests/builders/test_model_builder.py
 tests/builders/test_relationship_builder.py
 tests/builders/test_table_builder.py
 tests/dialects/__init__.py
 tests/dialects/test_triggers.py
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/__init__.py` & `SQLAlchemy-Continuum-1.4.0/tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from copy import copy
 import inspect
 import itertools as it
 import os
 import warnings
 import sqlalchemy as sa
 from sqlalchemy import create_engine
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import sessionmaker, column_property
+from sqlalchemy.orm import sessionmaker, column_property, close_all_sessions, declarative_base
 from sqlalchemy_continuum import (
     ClassNotVersioned,
     version_class,
     make_versioned,
     versioning_manager,
     remove_versioning
 )
@@ -36,19 +35,24 @@
     parameters,
     context,
     executemany
 ):
     QueryPool.queries.append(statement)
 
 
-def get_dns_from_driver(driver):
+def get_url_from_driver(driver):
+    url = os.environ.get('DATABASE_URL')
+    if url:
+        return url
+
     if driver == 'postgres':
-        return 'postgres://postgres@localhost/sqlalchemy_continuum_test'
+        return 'postgresql://postgres:postgres@localhost/main'
     elif driver == 'mysql':
-        return 'mysql+pymysql://travis@localhost/sqlalchemy_continuum_test'
+        # NB username is also in create_schema
+        return 'mysql+pymysql://root@localhost/main'
     elif driver == 'sqlite':
         return 'sqlite:///:memory:'
     else:
         raise Exception('Unknown driver given: %r' % driver)
 
 
 def get_driver_name(driver):
@@ -86,59 +90,69 @@
 
         driver = os.environ.get('DB', 'sqlite')
         self.driver = get_driver_name(driver)
         versioning_manager.plugins = self.plugins
         versioning_manager.transaction_cls = self.transaction_cls
         versioning_manager.user_cls = self.user_cls
 
-        self.engine = create_engine(get_dns_from_driver(self.driver))
+        self.engine = create_engine(get_url_from_driver(self.driver), echo=True)
         # self.engine.echo = True
         self.create_models()
 
         sa.orm.configure_mappers()
 
-        self.connection = self.engine.connect()
-
         if hasattr(self, 'Article'):
             try:
                 self.ArticleVersion = version_class(self.Article)
             except ClassNotVersioned:
                 pass
         if hasattr(self, 'Tag'):
             try:
                 self.TagVersion = version_class(self.Tag)
             except ClassNotVersioned:
                 pass
-        self.create_tables()
 
+        self.connection = self.engine.connect()
         Session = sessionmaker(bind=self.connection)
         self.session = Session(autoflush=False)
+
         if driver == 'postgres-native':
-            self.session.execute('CREATE EXTENSION IF NOT EXISTS hstore')
+            self.session.execute(sa.text('CREATE EXTENSION IF NOT EXISTS hstore'))
 
-    def create_tables(self):
-        self.Model.metadata.create_all(self.connection)
+        # Run any other custom SQL in here
+        self.create_schema('other')
+        self.session.commit()
+
+        # Using an engine here instead of connection will call commit for us,
+        # which lets us use the same syntax for 1.4 and 2.0
+        self.Model.metadata.create_all(self.engine)
 
-    def drop_tables(self):
-        self.Model.metadata.drop_all(self.connection)
 
     def teardown_method(self, method):
         self.session.rollback()
         uow_leaks = versioning_manager.units_of_work
         session_map_leaks = versioning_manager.session_connection_map
 
         remove_versioning()
         QueryPool.queries = []
         versioning_manager.reset()
 
-        self.session.close_all()
+        try:
+            close_all_sessions()
+        except Exception:
+            pass
         self.session.expunge_all()
-        self.drop_tables()
-        self.engine.dispose()
+
+        self.Model.metadata.drop_all(self.engine)
+
+        self.drop_schema('other')
+        self.session.commit()
+
         self.connection.close()
+        self.engine.dispose()
 
         assert not uow_leaks
         assert not session_map_leaks
 
     def create_models(self):
         class Article(self.Model):
             __tablename__ = 'article'
@@ -160,14 +174,42 @@
             name = sa.Column(sa.Unicode(255))
             article_id = sa.Column(sa.Integer, sa.ForeignKey(Article.id))
             article = sa.orm.relationship(Article, backref='tags')
 
         self.Article = Article
         self.Tag = Tag
 
+    def create_schema(self, schema):
+        if self.driver == 'postgres':
+            self.session.execute(sa.text(f'CREATE SCHEMA {schema}'))
+
+        elif self.driver == 'mysql':
+            self.session.execute(sa.text(f'CREATE DATABASE {schema}'))
+            # This user must match the value in get_url_from_driver
+            self.session.execute(sa.text(f'GRANT ALL PRIVILEGES ON {schema}.* TO root'))
+
+        elif self.driver == 'sqlite':
+            self.session.execute(sa.text(f"ATTACH DATABASE ':memory:' AS {schema}"))
+
+        else:
+            raise NotImplementedError
+
+
+    def drop_schema(self, schema):
+        if self.driver == 'postgres':
+            self.session.execute(sa.text(f'DROP SCHEMA IF EXISTS {schema} CASCADE'))
+
+        elif self.driver == 'mysql':
+            self.session.execute(sa.text(f'DROP DATABASE IF EXISTS {schema}'))
+
+        elif self.driver == 'sqlite':
+            self.session.execute(sa.text(f'DETACH DATABASE {schema}'))
+
+        else:
+            raise NotImplementedError
 
 setting_variants = {
     'versioning_strategy': [
         'subquery',
         'validity',
     ],
     'transaction_column_name': [
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/builders/test_relationship_builder.py` & `SQLAlchemy-Continuum-1.4.0/tests/builders/test_relationship_builder.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/builders/test_table_builder.py` & `SQLAlchemy-Continuum-1.4.0/tests/builders/test_table_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,14 @@
             )
         self.Article = Article
 
     def test_takes_out_onupdate_triggers(self):
         table = version_class(self.Article).__table__
         assert table.c.last_update.onupdate is None
 
-@mark.skipif("os.environ.get('DB') == 'sqlite'")
 class TestTableBuilderInOtherSchema(TestCase):
     def create_models(self):
         class Article(self.Model):
             __tablename__ = 'article'
             __versioned__ = copy(self.options)
             __table_args__ = {'schema': 'other'}
 
@@ -84,17 +83,12 @@
                 sa.DateTime,
                 default=datetime.utcnow,
                 onupdate=datetime.utcnow,
                 nullable=False
             )
         self.Article = Article
 
-    def create_tables(self):
-        self.connection.execute('DROP SCHEMA IF EXISTS other')
-        self.connection.execute('CREATE SCHEMA other')
-        TestCase.create_tables(self)
-
     def test_created_tables_retain_schema(self):
         table = version_class(self.Article).__table__
         assert table.schema is not None
         assert table.schema == self.Article.__table__.schema
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/dialects/test_triggers.py` & `SQLAlchemy-Continuum-1.4.0/tests/relationships/test_dynamic_relationships.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,100 @@
-import os
-
-import pytest
+from copy import copy
+from tests import TestCase
 import sqlalchemy as sa
 
-from sqlalchemy_continuum.dialects.postgresql import (
-    drop_trigger,
-    sync_trigger
-)
-from tests import (
-    get_dns_from_driver,
-    get_driver_name,
-    QueryPool,
-    uses_native_versioning
-)
-
-
-@pytest.mark.skipif('not uses_native_versioning()')
-class TestTriggerSyncing(object):
-    def setup_method(self, method):
-        driver = os.environ.get('DB', 'sqlite')
-        self.driver = get_driver_name(driver)
-        self.engine = sa.create_engine(get_dns_from_driver(self.driver))
-        self.connection = self.engine.connect()
-        if driver == 'postgres-native':
-            self.connection.execute('CREATE EXTENSION IF NOT EXISTS hstore')
-
-        self.connection.execute(
-            'CREATE TABLE article '
-            '(id INT PRIMARY KEY, name VARCHAR(200), content TEXT)'
-        )
-        self.connection.execute(
-            'CREATE TABLE article_version '
-            '(id INT, transaction_id INT, name VARCHAR(200), '
-            'name_mod BOOLEAN, PRIMARY KEY (id, transaction_id))'
-        )
 
-    def teardown_method(self, method):
-        self.connection.execute('DROP TABLE IF EXISTS article')
-        self.connection.execute('DROP TABLE IF EXISTS article_version')
-        self.engine.dispose()
-        self.connection.close()
-
-    def test_sync_triggers(self):
-        sync_trigger(self.connection, 'article_version')
-        assert (
-            'DROP TRIGGER IF EXISTS article_trigger ON "article"'
-            in QueryPool.queries[-4]
+class TestDynamicOneToManyRelationships(TestCase):
+    def create_models(self):
+        class Article(self.Model):
+            __tablename__ = 'article'
+            __versioned__ = copy(self.options)
+
+            id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
+            name = sa.Column(sa.Unicode(255), nullable=False)
+            content = sa.Column(sa.UnicodeText)
+            description = sa.Column(sa.UnicodeText)
+
+        class Tag(self.Model):
+            __tablename__ = 'tag'
+            __versioned__ = copy(self.options)
+
+            id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
+            name = sa.Column(sa.Unicode(255))
+            article_id = sa.Column(sa.Integer, sa.ForeignKey(Article.id))
+            article = sa.orm.relationship(
+                Article,
+                backref=sa.orm.backref(
+                    'tags',
+                    lazy='dynamic'
+                )
+            )
+
+        self.Article = Article
+        self.Tag = Tag
+
+    def test_reflects_dynamic_relationships_as_dynamic(self):
+        article = self.Article()
+        article.name = u'Some article'
+        article.content = u'Some content'
+        self.session.add(article)
+        self.session.commit()
+
+        assert article.versions[0].tags
+
+
+class TestDynamicManyToManyRelationships(TestCase):
+    def create_models(self):
+        class Article(self.Model):
+            __tablename__ = 'article'
+            __versioned__ = {
+                'base_classes': (self.Model, )
+            }
+
+            id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
+            name = sa.Column(sa.Unicode(255))
+
+        article_tag = sa.Table(
+            'article_tag',
+            self.Model.metadata,
+            sa.Column(
+                'article_id',
+                sa.Integer,
+                sa.ForeignKey('article.id', ondelete='CASCADE'),
+                primary_key=True,
+            ),
+            sa.Column(
+                'tag_id',
+                sa.Integer,
+                sa.ForeignKey('tag.id', ondelete='CASCADE'),
+                primary_key=True
+            )
         )
-        assert 'DROP FUNCTION ' in QueryPool.queries[-3]
-        assert 'CREATE OR REPLACE FUNCTION ' in QueryPool.queries[-2]
-        assert 'CREATE TRIGGER ' in QueryPool.queries[-1]
-        sync_trigger(self.connection, 'article_version')
-
-    def test_drop_triggers(self):
-        drop_trigger(self.connection, 'article')
-        assert (
-            'DROP TRIGGER IF EXISTS article_trigger ON "article"'
-            in QueryPool.queries[-2]
+
+        class Tag(self.Model):
+            __tablename__ = 'tag'
+            __versioned__ = {
+                'base_classes': (self.Model, )
+            }
+
+            id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
+            name = sa.Column(sa.Unicode(255))
+
+        Tag.articles = sa.orm.relationship(
+            Article,
+            secondary=article_tag,
+            backref=sa.orm.backref(
+                'tags',
+                lazy='dynamic'
+            )
         )
-        assert 'DROP FUNCTION ' in QueryPool.queries[-1]
+
+        self.Article = Article
+        self.Tag = Tag
+
+    def test_version_relations(self):
+        article = self.Article()
+        article.name = u'Some article'
+        article.content = u'Some content'
+        self.session.add(article)
+        self.session.commit()
+        assert article.versions[0].tags
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_common_base_class.py` & `SQLAlchemy-Continuum-1.4.0/tests/inheritance/test_common_base_class.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_concrete_inheritance.py` & `SQLAlchemy-Continuum-1.4.0/tests/inheritance/test_concrete_inheritance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pytest import mark
 import sqlalchemy as sa
 from sqlalchemy_continuum import versioning_manager, version_class
 from tests import TestCase
 
 
-class TestConreteTableInheritance(TestCase):
+class TestConcreteTableInheritance(TestCase):
     def create_models(self):
         class TextItem(self.Model):
             __tablename__ = 'text_item'
             __versioned__ = {
                 'base_classes': (self.Model, )
             }
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_join_table_inheritance.py` & `SQLAlchemy-Continuum-1.4.0/tests/inheritance/test_join_table_inheritance.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,20 +97,20 @@
         self.session.commit()
 
     def test_assign_transaction_id_to_both_parent_and_child_tables(self):
         tx_column = self.options['transaction_column_name']
         article = self.Article()
         self.session.add(article)
         self.session.commit()
-        assert self.session.execute(
+        assert self.session.execute(sa.text(
             'SELECT %s FROM article_version' % tx_column
-        ).fetchone()[0]
-        assert self.session.execute(
+        )).fetchone()[0]
+        assert self.session.execute(sa.text(
             'SELECT %s FROM text_item_version' % tx_column
-        ).fetchone()[0]
+        )).fetchone()[0]
 
     def test_primary_keys(self):
         tx_column = self.options['transaction_column_name']
         table = self.TextItemVersion.__table__
         assert len(table.primary_key.columns)
         assert 'id' in table.primary_key.columns
         assert tx_column in table.primary_key.columns
@@ -129,22 +129,22 @@
         article = self.Article()
         self.session.add(article)
         self.session.commit()
         article.name = u'Updated article'
         self.session.commit()
         assert article.versions.count() == 2
 
-        assert self.session.execute(
+        assert self.session.execute(sa.text(
             'SELECT %s FROM text_item_version '
             'ORDER BY %s LIMIT 1' % (end_tx_column, tx_column)
-        ).scalar()
-        assert self.session.execute(
+        )).scalar()
+        assert self.session.execute(sa.text(
             'SELECT %s FROM article_version '
             'ORDER BY %s LIMIT 1' % (end_tx_column, tx_column)
-        ).scalar()
+        )).scalar()
 
 
 create_test_cases(JoinTableInheritanceTestCase)
 
 
 class TestDeepJoinedTableInheritance(TestCase):
     def create_models(self):
@@ -190,16 +190,16 @@
         self.Content = Content
         self.Document = Document
 
     def test_insert(self):
         document = self.Document()
         self.session.add(document)
         self.session.commit()
-        assert self.session.execute(
+        assert self.session.execute(sa.text(
             'SELECT COUNT(1) FROM document_version'
-        ).scalar() == 1
-        assert self.session.execute(
+        )).scalar() == 1
+        assert self.session.execute(sa.text(
             'SELECT COUNT(1) FROM content_version'
-        ).scalar() == 1
-        assert self.session.execute(
+        )).scalar() == 1
+        assert self.session.execute(sa.text(
             'SELECT COUNT(1) FROM node_version'
-        ).scalar() == 1
+        )).scalar() == 1
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_multi_level_inheritance.py` & `SQLAlchemy-Continuum-1.4.0/tests/inheritance/test_multi_level_inheritance.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/inheritance/test_single_table_inheritance.py` & `SQLAlchemy-Continuum-1.4.0/tests/inheritance/test_single_table_inheritance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sqlalchemy as sa
+from sqlalchemy.ext.declarative import declared_attr
 from sqlalchemy_continuum import versioning_manager, version_class
 from tests import TestCase, create_test_cases
 
 
 class SingleTableInheritanceTestCase(TestCase):
     def create_models(self):
         class TextItem(self.Model):
@@ -14,21 +15,26 @@
 
             discriminator = sa.Column(
                 sa.Unicode(100)
             )
 
             __mapper_args__ = {
                 'polymorphic_on': discriminator,
+                'polymorphic_identity': u'base',
                 'with_polymorphic': '*'
             }
 
         class Article(TextItem):
             __mapper_args__ = {'polymorphic_identity': u'article'}
             name = sa.Column(sa.Unicode(255))
 
+            @sa.ext.declarative.declared_attr
+            def status(cls):
+                return sa.Column("_status", sa.Unicode(255))
+
         class BlogPost(TextItem):
             __mapper_args__ = {'polymorphic_identity': u'blog_post'}
             title = sa.Column(sa.Unicode(255))
 
         self.TextItem = TextItem
         self.Article = Article
         self.BlogPost = BlogPost
@@ -75,9 +81,12 @@
         transaction = (
             self.session.query(Transaction)
             .order_by(sa.sql.expression.desc(Transaction.issued_at))
         ).first()
         assert transaction.entity_names == [u'Article']
         assert transaction.changed_entities
 
+    def test_declared_attr_inheritance(self):
+        assert self.ArticleVersion.status
+
 
 create_test_cases(SingleTableInheritanceTestCase)
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_activity.py` & `SQLAlchemy-Continuum-1.4.0/tests/plugins/test_activity.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,28 +32,56 @@
             target=target,
             verb=u'create',
         )
         self.session.add(activity)
         return activity
 
 
+class TestActivityNotId(ActivityTestCase):
+
+    def create_models(self):
+        TestCase.create_models(self)
+
+        class NotIdModel(self.Model):
+            __tablename__ = 'not_id'
+            __versioned__ = {
+                'base_classes': (self.Model, )
+            }
+
+            pk = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
+            name = sa.Column(sa.Unicode(255), nullable=False)
+        self.NotIdModel = NotIdModel
+
+    def test_create_activity_with_pk(self):
+        not_id_model = self.NotIdModel(name=u'Some model without id PK')
+        self.session.add(not_id_model)
+        self.session.commit()
+        self.create_activity(not_id_model)
+        self.session.commit()
+        activity = self.session.query(versioning_manager.activity_cls).first()
+        assert activity
+        assert activity.transaction_id
+        assert activity.object == not_id_model
+        assert activity.object_version == list(not_id_model.versions)[-1]
+
+
 class TestActivity(ActivityTestCase):
     def test_creates_activity_class(self):
         assert versioning_manager.activity_cls.__name__ == 'Activity'
 
     def test_create_activity(self):
         article = self.create_article()
         self.session.flush()
         self.create_activity(article)
         self.session.commit()
         activity = self.session.query(versioning_manager.activity_cls).first()
         assert activity
         assert activity.transaction_id
         assert activity.object == article
-        assert activity.object_version == article.versions[-1]
+        assert activity.object_version == list(article.versions)[-1]
 
     def test_delete_activity(self):
         article = self.create_article()
         self.create_activity(article)
         self.session.commit()
         self.session.delete(article)
         activity = versioning_manager.activity_cls(
@@ -66,15 +94,15 @@
             self.session.query(self.ArticleVersion)
             .order_by(sa.desc(self.ArticleVersion.transaction_id))
             .all()
         )
         assert activity
         assert activity.transaction_id
         assert activity.object is None
-        assert activity.object_version == versions[-1]
+        assert activity.object_version == list(versions)[-1]
 
     def test_activity_queries(self):
         article = self.create_article()
         self.session.flush()
         self.create_activity(article)
         self.session.commit()
         tag = self.Tag(name=u'some tag', article=article)
@@ -103,50 +131,54 @@
     @pytest.mark.skipif('uses_native_versioning()')
     def test_does_not_query_db_if_version_obj_in_session(self):
         article = self.create_article()
         self.session.flush()
         self.create_activity(object=article)
         query_count = len(QueryPool.queries)
         self.session.commit()
+        if QueryPool.queries[-2] == 'select nextval(activity_id_seq)':
+            query_count += 1
         assert query_count + 1 == len(QueryPool.queries)
 
     def test_create_activity_with_multiple_existing_objects(self):
         article = self.create_article()
         self.session.commit()
         self.create_article()
         self.session.commit()
         activity = self.create_activity(article)
         self.session.commit()
         assert activity
         assert activity.transaction_id
         assert activity.object == article
-        assert activity.object_version == article.versions[-1]
+        assert activity.object_version == list(article.versions)[-1]
 
 
 class TestTargetTxIdGeneration(ActivityTestCase):
     @pytest.mark.skipif('uses_native_versioning()')
     def test_does_not_query_db_if_version_obj_in_session(self):
         article = self.create_article()
         self.session.flush()
         self.create_activity(target=article)
         query_count = len(QueryPool.queries)
         self.session.commit()
+        if QueryPool.queries[-2] == 'select nextval(activity_id_seq)':
+            query_count += 1
         assert query_count + 1 == len(QueryPool.queries)
 
     def test_with_multiple_existing_targets(self):
         article = self.create_article()
         self.session.commit()
         self.create_article()
         self.session.commit()
         activity = self.create_activity(target=article)
         self.session.commit()
         assert activity
         assert activity.transaction_id
         assert activity.target == article
-        assert activity.target_version == article.versions[-1]
+        assert activity.target_version == list(article.versions)[-1]
 
     def test_activity_target(self):
         article = self.create_article()
         self.create_activity(article)
         self.session.commit()
         tag = self.Tag(name=u'some tag', article=article)
         self.session.add(tag)
@@ -160,10 +192,10 @@
         self.session.commit()
         activity = self.session.query(
             versioning_manager.activity_cls
         ).filter_by(id=activity.id).one()
         assert activity
         assert activity.transaction_id
         assert activity.object == tag
-        assert activity.object_version == tag.versions[-1]
+        assert activity.object_version == list(tag.versions)[-1]
         assert activity.target == article
-        assert activity.target_version == article.versions[-1]
+        assert activity.target_version == list(article.versions)[-1]
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_flask.py` & `SQLAlchemy-Continuum-1.4.0/tests/plugins/test_flask.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 
 from flask import Flask, url_for
-from flask_login import LoginManager
-from flask_sqlalchemy import SQLAlchemy, _SessionSignalEvents
-from flexmock import flexmock
+from flask_login import LoginManager, UserMixin, login_user
+from flask_sqlalchemy import SQLAlchemy
 
 import sqlalchemy as sa
+from sqlalchemy.orm import close_all_sessions
 from sqlalchemy_continuum import (
     make_versioned, remove_versioning, versioning_manager
 )
 from sqlalchemy_continuum.plugins import FlaskPlugin
 from sqlalchemy_continuum.transaction import TransactionFactory
 from tests import (
     TestCase,
     get_driver_name,
-    get_dns_from_driver,
+    get_url_from_driver,
     uses_native_versioning
 )
 
 
 class TestFlaskPluginConfiguration(object):
     def test_set_factories(self):
         some_func = lambda: None
@@ -55,32 +55,18 @@
     def teardown_method(self, method):
         TestCase.teardown_method(self, method)
         self.context.pop()
         self.context = None
         self.client = None
         self.app = None
 
-    def login(self, user):
-        """
-        Log in the user returned by :meth:`create_user`.
-
-        :returns: the logged in user
-        """
-        with self.client.session_transaction() as s:
-            s['user_id'] = user.id
-        return user
-
-    def logout(self, user=None):
-        with self.client.session_transaction() as s:
-            s['user_id'] = None
-
     def create_models(self):
         TestCase.create_models(self)
 
-        class User(self.Model):
+        class User(self.Model, UserMixin):
             __tablename__ = 'user'
             __versioned__ = {
                 'base_classes': (self.Model, )
             }
 
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
             name = sa.Column(sa.Unicode(255), nullable=False)
@@ -93,43 +79,43 @@
             article.name = u'Some article'
             self.session.add(article)
             self.session.commit()
             return ''
 
         @self.app.route('/raw-sql-and-flush')
         def test_raw_sql_and_flush():
-            self.session.execute(
+            self.session.execute(sa.text(
                 "INSERT INTO article (name) VALUES ('some article')"
-            )
+            ))
             article = self.Article()
             article.name = u'Some article'
             self.session.add(article)
             self.session.flush()
-            self.session.execute(
+            self.session.execute(sa.text(
                 "INSERT INTO article (name) VALUES ('some article')"
-            )
+            ))
             self.session.commit()
             return ''
 
     def test_versioning_inside_request(self):
         user = self.User(name=u'Rambo')
         self.session.add(user)
         self.session.commit()
-        self.login(user)
+        login_user(user)
         self.client.get(url_for('.test_simple_flush'))
 
         article = self.session.query(self.Article).first()
-        tx = article.versions[-1].transaction
+        tx = list(article.versions)[-1].transaction
         assert tx.user.id == user.id
 
     def test_raw_sql_and_flush(self):
         user = self.User(name=u'Rambo')
         self.session.add(user)
         self.session.commit()
-        self.login(user)
+        login_user(user)
         self.client.get(url_for('.test_raw_sql_and_flush'))
         assert (
             self.session.query(versioning_manager.transaction_cls).count() == 2
         )
 
 
 class TestFlaskPluginWithoutRequestContext(TestCase):
@@ -210,49 +196,46 @@
         )
 
         self.User = User
         self.Article = Article
         self.Tag = Tag
 
     def setup_method(self, method):
-        # Mock the event registering of Flask-SQLAlchemy. Currently there is no
-        # way of unregistering Flask-SQLAlchemy event listeners, hence the
-        # event listeners would affect other tests.
-        flexmock(_SessionSignalEvents).should_receive('register')
-
         self.db = SQLAlchemy()
         make_versioned()
 
         versioning_manager.transaction_cls = TransactionFactory()
         versioning_manager.options['native_versioning'] = (
             uses_native_versioning()
         )
 
         self.create_models()
 
         sa.orm.configure_mappers()
 
         self.app = Flask(__name__)
         # self.app.config['SQLALCHEMY_ECHO'] = True
-        self.app.config['SQLALCHEMY_DATABASE_URI'] = get_dns_from_driver(
+        self.app.config['SQLALCHEMY_DATABASE_URI'] = get_url_from_driver(
             get_driver_name(os.environ.get('DB', 'sqlite'))
         )
         self.db.init_app(self.app)
         self.app.secret_key = 'secret'
         self.app.debug = True
         self.client = self.app.test_client()
         self.context = self.app.test_request_context()
         self.context.push()
         self.db.create_all()
+        self.db.session.commit()
 
     def teardown_method(self, method):
         remove_versioning()
         self.db.session.remove()
         self.db.drop_all()
-        self.db.session.close_all()
+        self.db.session.commit()
+        close_all_sessions()
         self.db.engine.dispose()
         self.context.pop()
         self.context = None
         self.client = None
         self.app = None
 
     def test_version_relations(self):
@@ -277,9 +260,7 @@
         article = self.Article()
         article.name = u'Some article'
         article.content = u'Some content'
         self.db.session.add(article)
         uow = versioning_manager.unit_of_work(self.db.session)
         transaction = uow.create_transaction(self.db.session)
         assert transaction.id
-
-
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_null_delete.py` & `SQLAlchemy-Continuum-1.4.0/tests/plugins/test_null_delete.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_plugin_collection.py` & `SQLAlchemy-Continuum-1.4.0/tests/plugins/test_plugin_collection.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_property_mod_tracker.py` & `SQLAlchemy-Continuum-1.4.0/tests/plugins/test_property_mod_tracker.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,24 +33,24 @@
         assert 'id_mod' not in UserVersion.__table__.c
 
     def test_mod_properties_with_insert(self):
         user = self.User(name=u'John')
         self.session.add(user)
         self.session.commit()
 
-        assert user.versions[-1].name_mod
+        assert list(user.versions)[-1].name_mod
 
     def test_mod_properties_with_update(self):
         user = self.User(name=u'John')
         self.session.add(user)
         self.session.commit()
         user.age = 14
         self.session.commit()
-        assert user.versions[-1].age_mod
-        assert not user.versions[-1].name_mod
+        assert list(user.versions)[-1].age_mod
+        assert not list(user.versions)[-1].name_mod
 
     def test_mod_properties_with_delete(self):
         user = self.User(name=u'John')
         self.session.add(user)
         self.session.commit()
         self.session.delete(user)
         self.session.commit()
@@ -65,39 +65,39 @@
 
     def test_consequtive_insert_and_update(self):
         user = self.User(name=u'John')
         self.session.add(user)
         self.session.flush()
         user.age = 15
         self.session.commit()
-        assert user.versions[-1].age_mod
-        assert user.versions[-1].name_mod
+        assert list(user.versions)[-1].age_mod
+        assert list(user.versions)[-1].name_mod
 
     def test_consequtive_update_and_update(self):
         user = self.User(name=u'John')
         self.session.add(user)
         self.session.commit()
         user.name = u'Jack'
         self.session.flush()
         user.age = 15
         self.session.commit()
-        assert user.versions[-1].age_mod
-        assert user.versions[-1].name_mod
+        assert list(user.versions)[-1].age_mod
+        assert list(user.versions)[-1].name_mod
 
 
 class TestChangeSetWithPropertyModPlugin(TestCase):
     plugins = [PropertyModTrackerPlugin()]
 
     def test_changeset_for_insert(self):
         article = self.Article()
         article.name = u'Some article'
         article.content = u'Some content'
         self.session.add(article)
         self.session.commit()
-        assert article.versions[0].changeset == {
+        assert list(article.versions)[0].changeset == {
             'content': [None, u'Some content'],
             'name': [None, u'Some article'],
             'id': [None, 1]
         }
 
     def test_changeset_for_update(self):
         article = self.Article()
@@ -106,15 +106,15 @@
         self.session.add(article)
         self.session.commit()
 
         article.name = u'Updated name'
         article.content = u'Updated content'
         self.session.commit()
 
-        assert article.versions[1].changeset == {
+        assert list(article.versions)[1].changeset == {
             'content': [u'Some content', u'Updated content'],
             'name': [u'Some article', u'Updated name']
         }
 
 
 class TestWithAssociationTables(TestCase):
     plugins = [PropertyModTrackerPlugin()]
@@ -175,17 +175,17 @@
 class TestModTrackingWithRelationships(TestCase):
     plugins = [PropertyModTrackerPlugin()]
 
     def test_with_insert(self):
         tag = self.Tag(article=self.Article(name=u'Some article'))
         self.session.add(tag)
         self.session.commit()
-        assert tag.versions[-1]
+        assert list(tag.versions)[-1]
 
     def test_with_update(self):
         tag = self.Tag(article=self.Article(name=u'Some article'))
         self.session.add(tag)
         self.session.commit()
         tag.article = None
         self.session.commit()
 
-        assert tag.versions[-1].article_id_mod
+        assert list(tag.versions)[-1].article_id_mod
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_transaction_changes.py` & `SQLAlchemy-Continuum-1.4.0/tests/plugins/test_transaction_changes.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/plugins/test_transaction_meta.py` & `SQLAlchemy-Continuum-1.4.0/tests/plugins/test_transaction_meta.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,9 +28,9 @@
         self.article.name = u'Some update article'
         meta = {u'some_key': u'some_value'}
         uow = versioning_manager.unit_of_work(self.session)
         tx = uow.create_transaction(self.session)
         tx.meta = meta
         self.session.commit()
 
-        tx = self.article.versions[-1].transaction
+        tx = list(self.article.versions)[-1].transaction
         assert tx.meta[u'some_key'] == u'some_value'
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_association_table_relations.py` & `SQLAlchemy-Continuum-1.4.0/tests/relationships/test_association_table_relations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import sqlalchemy as sa
 from sqlalchemy import PrimaryKeyConstraint
 from sqlalchemy.orm import relationship
 from tests import TestCase, create_test_cases
+from packaging import version as py_pkg_version
 
 
 class AssociationTableRelationshipsTestCase(TestCase):
     def create_models(self):
         super(AssociationTableRelationshipsTestCase, self).create_models()
 
         class PublishedArticle(self.Model):
             __tablename__ = 'published_article'
             __table_args__ = (
                 PrimaryKeyConstraint("article_id", "author_id"),
-                {'useexisting': True}
+                {'keep_existing': True}
             )
 
             article_id = sa.Column(sa.Integer, sa.ForeignKey('article.id'))
             author_id = sa.Column(sa.Integer, sa.ForeignKey('author.id'))
-            author = relationship('Author')
-            article = relationship('Article')
+            relationship_kwargs = {}
+            if py_pkg_version.parse(sa.__version__) >= py_pkg_version.parse('1.4.0'):
+                relationship_kwargs.update({'overlaps': 'articles'})
+            author = relationship('Author', **relationship_kwargs)
+            article = relationship('Article', **relationship_kwargs)
 
         self.PublishedArticle = PublishedArticle
 
         published_articles_table = sa.Table(PublishedArticle.__tablename__,
                                             PublishedArticle.metadata,
                                             extend_existing=True)
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_custom_condition_relations.py` & `SQLAlchemy-Continuum-1.4.0/tests/relationships/test_custom_condition_relations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sqlalchemy as sa
 from tests import TestCase, create_test_cases
-
+from packaging import version as py_pkg_version
 
 class CustomConditionRelationsTestCase(TestCase):
     def create_models(self):
         class Article(self.Model):
             __tablename__ = 'article'
             __versioned__ = {
                 'base_classes': (self.Model, )
@@ -22,28 +22,36 @@
             }
 
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
             name = sa.Column(sa.Unicode(255))
             article_id = sa.Column(sa.Integer, sa.ForeignKey(Article.id))
             category = sa.Column(sa.Unicode(20))
 
+        if py_pkg_version.parse(sa.__version__) < py_pkg_version.parse('1.4.0'):
+            primary_key_overlaps = {}
+            secondary_key_overlaps = {}
+        else:
+            primary_key_overlaps = {'overlaps': 'secondary_tags, Article'}
+            secondary_key_overlaps = {'overlaps': 'primary_tags, Article'}
         Article.primary_tags = sa.orm.relationship(
             Tag,
             primaryjoin=sa.and_(
                 Tag.article_id == Article.id,
                 Tag.category == u'primary'
             ),
+            **primary_key_overlaps
         )
 
         Article.secondary_tags = sa.orm.relationship(
             Tag,
             primaryjoin=sa.and_(
                 Tag.article_id == Article.id,
                 Tag.category == u'secondary'
             ),
+            **secondary_key_overlaps
         )
 
         self.Article = Article
         self.Tag = Tag
 
     def test_relationship_condition_reflection(self):
         article = self.Article()
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_dynamic_relationships.py` & `SQLAlchemy-Continuum-1.4.0/tests/relationships/test_non_versioned_classes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 from copy import copy
 from tests import TestCase
 import sqlalchemy as sa
 
 
-class TestDynamicOneToManyRelationships(TestCase):
+class TestRelationshipToNonVersionedClass(TestCase):
     def create_models(self):
+        class User(self.Model):
+            __tablename__ = 'user'
+
+            id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
+            name = sa.Column(sa.Unicode(255))
+
         class Article(self.Model):
             __tablename__ = 'article'
             __versioned__ = copy(self.options)
 
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
             name = sa.Column(sa.Unicode(255), nullable=False)
             content = sa.Column(sa.UnicodeText)
             description = sa.Column(sa.UnicodeText)
+            author_id = sa.Column(sa.Integer, sa.ForeignKey(User.id))
+            author = sa.orm.relationship(User)
 
-        class Tag(self.Model):
-            __tablename__ = 'tag'
-            __versioned__ = copy(self.options)
+        self.Article = Article
+        self.User = User
 
-            id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
-            name = sa.Column(sa.Unicode(255))
-            article_id = sa.Column(sa.Integer, sa.ForeignKey(Article.id))
-            article = sa.orm.relationship(
-                Article,
-                backref=sa.orm.backref(
-                    'tags',
-                    lazy='dynamic'
-                )
-            )
+    def test_single_insert(self):
+        article = self.Article()
+        article.name = u'Some article'
+        article.content = u'Some content'
+        user = self.User(name=u'Some user')
+        article.author = user
+        self.session.add(article)
+        self.session.commit()
 
-        self.Article = Article
-        self.Tag = Tag
+        assert isinstance(article.versions[0].author, self.User)
 
-    def test_reflects_dynamic_relationships_as_dynamic(self):
+    def test_change_relationship(self):
         article = self.Article()
         article.name = u'Some article'
         article.content = u'Some content'
+        user = self.User(name=u'Some user')
         self.session.add(article)
+        self.session.add(user)
         self.session.commit()
 
-        assert article.versions[0].tags
+        assert article.versions.count() == 1
+        article.author = user
+        self.session.commit()
+        assert article.versions.count() == 2
 
 
-class TestDynamicManyToManyRelationships(TestCase):
+class TestManyToManyRelationshipToNonVersionedClass(TestCase):
     def create_models(self):
         class Article(self.Model):
             __tablename__ = 'article'
             __versioned__ = {
                 'base_classes': (self.Model, )
             }
 
@@ -55,46 +64,43 @@
 
         article_tag = sa.Table(
             'article_tag',
             self.Model.metadata,
             sa.Column(
                 'article_id',
                 sa.Integer,
-                sa.ForeignKey('article.id', ondelete='CASCADE'),
+                sa.ForeignKey('article.id'),
                 primary_key=True,
             ),
             sa.Column(
                 'tag_id',
                 sa.Integer,
-                sa.ForeignKey('tag.id', ondelete='CASCADE'),
+                sa.ForeignKey('tag.id'),
                 primary_key=True
             )
         )
 
         class Tag(self.Model):
             __tablename__ = 'tag'
-            __versioned__ = {
-                'base_classes': (self.Model, )
-            }
 
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
             name = sa.Column(sa.Unicode(255))
 
         Tag.articles = sa.orm.relationship(
             Article,
             secondary=article_tag,
-            backref=sa.orm.backref(
-                'tags',
-                lazy='dynamic'
-            )
+            backref='tags'
         )
 
         self.Article = Article
         self.Tag = Tag
 
-    def test_version_relations(self):
+    def test_single_insert(self):
         article = self.Article()
         article.name = u'Some article'
         article.content = u'Some content'
+        tag = self.Tag(name=u'some tag')
+        article.tags.append(tag)
         self.session.add(article)
         self.session.commit()
-        assert article.versions[0].tags
+        assert len(article.versions[0].tags) == 1
+        assert isinstance(article.versions[0].tags[0], self.Tag)
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_many_to_many_relations.py` & `SQLAlchemy-Continuum-1.4.0/tests/relationships/test_many_to_many_relations.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,41 @@
         article.content = u'Some content'
         tag = self.Tag(name=u'some tag')
         article.tags.append(tag)
         self.session.add(article)
         self.session.commit()
         assert len(article.versions[0].tags) == 1
 
+    def test_unrelated_change(self):
+        tag1 = self.Tag(name=u'some tag')
+        tag2 = self.Tag(name=u'some tag2')
+
+        self.session.add(tag1)
+        self.session.add(tag2)
+        self.session.commit()
+
+        article1 = self.Article(name="Some article", )
+        article1.name = u'Some article'
+        article1.tags.append(tag1)
+
+        self.session.add(article1)
+        self.session.commit()
+
+        article2 = self.Article()
+        article2.name = u'Some article2'
+        article2.tags.append(tag1)
+
+        self.session.add(article2)
+        self.session.commit()
+
+        article1.name = u'Some other name'
+        self.session.commit()
+
+        assert len(article1.versions[1].tags) == 1
+
     def test_multi_insert(self):
         article = self.Article()
         article.name = u'Some article'
         article.content = u'Some content'
         tag = self.Tag(name=u'some tag')
         article.tags.append(tag)
         article.tags.append(self.Tag(name=u'another tag'))
@@ -339,15 +366,14 @@
         assert reference1.versions[2] in article.versions[2].references
         assert reference2.versions[0] in article.versions[2].references
 
         assert len(reference1.versions[2].cited_by) == 1
         assert article.versions[2] in reference1.versions[2].cited_by
 
 
-@mark.skipif("os.environ.get('DB') == 'sqlite'")
 class TestManyToManySelfReferentialInOtherSchema(TestManyToManySelfReferential):
     def create_models(self):
         class Article(self.Model):
             __tablename__ = 'article'
             __versioned__ = {}
             __table_args__ = {'schema': 'other'}
 
@@ -379,21 +405,15 @@
             secondaryjoin=Article.id == article_references.c.referred_id,
             backref='cited_by'
         )
 
         self.Article = Article
         self.referenced_articles_table = article_references
 
-    def create_tables(self):
-        self.connection.execute('DROP SCHEMA IF EXISTS other')
-        self.connection.execute('CREATE SCHEMA other')
-        TestManyToManySelfReferential.create_tables(self)
 
-
-@mark.skipif("os.environ.get('DB') == 'sqlite'")
 class ManyToManyRelationshipsInOtherSchemaTestCase(ManyToManyRelationshipsTestCase):
     def create_models(self):
         class Article(self.Model):
             __tablename__ = 'article'
             __versioned__ = {
                 'base_classes': (self.Model, )
             }
@@ -436,14 +456,9 @@
             backref='tags'
         )
 
         self.Article = Article
         self.Tag = Tag
 
 
-    def create_tables(self):
-        self.connection.execute('DROP SCHEMA IF EXISTS other')
-        self.connection.execute('CREATE SCHEMA other')
-        ManyToManyRelationshipsTestCase.create_tables(self)
-
 create_test_cases(ManyToManyRelationshipsInOtherSchemaTestCase)
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_non_versioned_classes.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_configuration.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,106 +1,116 @@
-from copy import copy
-from tests import TestCase
+from pytest import raises, skip
 import sqlalchemy as sa
+from sqlalchemy.orm import declarative_base
+from sqlalchemy_continuum import (
+    versioning_manager, ImproperlyConfigured, TransactionFactory
+)
+
+from tests import TestCase
 
 
-class TestRelationshipToNonVersionedClass(TestCase):
+class TestVersionedModelWithoutVersioning(TestCase):
     def create_models(self):
-        class User(self.Model):
-            __tablename__ = 'user'
+        class TextItem(self.Model):
+            __tablename__ = 'text_item'
+            __versioned__ = {
+                'versioning': False
+            }
 
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
-            name = sa.Column(sa.Unicode(255))
 
+        self.TextItem = TextItem
+
+    def test_does_not_create_history_class(self):
+        assert 'class' not in self.TextItem.__versioned__
+
+    def test_does_not_create_history_table(self):
+        assert 'text_item_history' not in self.Model.metadata.tables
+
+    def test_does_add_objects_to_unit_of_work(self):
+        self.session.add(self.TextItem())
+        self.session.commit()
+
+
+class TestWithUnknownUserClass(object):
+    def test_raises_improperly_configured_error(self):
+        self.Model = declarative_base()
+
+        class TextItem(self.Model):
+            __tablename__ = 'text_item'
+            __versioned__ = {}
+
+            id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
+
+        self.TextItem = TextItem
+
+        versioning_manager.user_cls = 'User'
+        versioning_manager.declarative_base = self.Model
+
+        factory = TransactionFactory()
+        with raises(ImproperlyConfigured):
+            factory(versioning_manager)
+
+
+class TestWithCreateModelsAsFalse(TestCase):
+    should_create_models = False
+
+    def create_models(self):
         class Article(self.Model):
             __tablename__ = 'article'
-            __versioned__ = copy(self.options)
+            __versioned__ = {}
 
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
             name = sa.Column(sa.Unicode(255), nullable=False)
             content = sa.Column(sa.UnicodeText)
             description = sa.Column(sa.UnicodeText)
-            author_id = sa.Column(sa.Integer, sa.ForeignKey(User.id))
-            author = sa.orm.relationship(User)
 
-        self.Article = Article
-        self.User = User
+        class Category(self.Model):
+            __tablename__ = 'category'
+            __versioned__ = {}
 
-    def test_single_insert(self):
-        article = self.Article()
-        article.name = u'Some article'
-        article.content = u'Some content'
-        user = self.User(name=u'Some user')
-        article.author = user
-        self.session.add(article)
-        self.session.commit()
+            id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
+            name = sa.Column(sa.Unicode(255))
+            article_id = sa.Column(sa.Integer, sa.ForeignKey(Article.id))
+            article = sa.orm.relationship(
+                Article,
+                backref=sa.orm.backref(
+                    'category',
+                    uselist=False
+                )
+            )
 
-        assert isinstance(article.versions[0].author, self.User)
+        self.Article = Article
+        self.Category = Category
 
-    def test_change_relationship(self):
-        article = self.Article()
-        article.name = u'Some article'
-        article.content = u'Some content'
-        user = self.User(name=u'Some user')
+    def test_does_not_create_models(self):
+        assert 'class' not in self.Article.__versioned__
+
+    def test_insert(self):
+        if self.options['native_versioning'] is False:
+            skip()
+        article = self.Article(name=u'Some article')
         self.session.add(article)
-        self.session.add(user)
         self.session.commit()
 
-        assert article.versions.count() == 1
-        article.author = user
-        self.session.commit()
-        assert article.versions.count() == 2
+        version = self.session.execute(sa.text('SELECT * FROM article_version')).fetchone()
+        assert version.transaction_id > 0
+        assert version.id == article.id
+        assert version.name == u'Some article'
 
 
-class TestManyToManyRelationshipToNonVersionedClass(TestCase):
+class TestWithoutAnyVersionedModels(TestCase):
     def create_models(self):
         class Article(self.Model):
             __tablename__ = 'article'
-            __versioned__ = {
-                'base_classes': (self.Model, )
-            }
 
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
-            name = sa.Column(sa.Unicode(255))
-
-        article_tag = sa.Table(
-            'article_tag',
-            self.Model.metadata,
-            sa.Column(
-                'article_id',
-                sa.Integer,
-                sa.ForeignKey('article.id'),
-                primary_key=True,
-            ),
-            sa.Column(
-                'tag_id',
-                sa.Integer,
-                sa.ForeignKey('tag.id'),
-                primary_key=True
-            )
-        )
-
-        class Tag(self.Model):
-            __tablename__ = 'tag'
-
-            id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
-            name = sa.Column(sa.Unicode(255))
-
-        Tag.articles = sa.orm.relationship(
-            Article,
-            secondary=article_tag,
-            backref='tags'
-        )
+            name = sa.Column(sa.Unicode(255), nullable=False)
+            content = sa.Column(sa.UnicodeText)
+            description = sa.Column(sa.UnicodeText)
 
         self.Article = Article
-        self.Tag = Tag
 
-    def test_single_insert(self):
-        article = self.Article()
-        article.name = u'Some article'
-        article.content = u'Some content'
-        tag = self.Tag(name=u'some tag')
-        article.tags.append(tag)
+    def test_insert(self):
+        article = self.Article(name=u'Some article')
         self.session.add(article)
         self.session.commit()
-        assert len(article.versions[0].tags) == 1
-        assert isinstance(article.versions[0].tags[0], self.Tag)
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_one_to_many_relations.py` & `SQLAlchemy-Continuum-1.4.0/tests/relationships/test_one_to_many_relations.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     def test_relationships_for_history_objects(self):
         article = self.Article()
         article.name = u'Some article'
         article.content = u'Some content'
         article.tags.append(self.Tag(name=u'some tag'))
         self.session.add(article)
         self.session.commit()
-        version = article.versions.all()[0]
+        version = list(article.versions)[0]
         assert version.name == u'Some article'
         assert version.content == u'Some content'
-        version = article.tags[0].versions.all()[0]
+        version = list(article.tags[0].versions)[0]
         assert version.name == u'some tag'
 
     def test_consecutive_inserts_and_removes(self):
         article = self.Article()
         article.name = u'Some article'
         article.content = u'Some content'
         tag = self.Tag(name=u'some tag')
@@ -88,14 +88,15 @@
         self.session.commit()
 
         # update the article and the tag, and add a 2nd tag
         article.name = u'Updated article'
         tag.name = u'updated tag'
         tag2 = self.Tag(name=u'other tag',
                         article=article)
+        self.session.add(tag2)
         self.session.commit()
 
         # update the article and the tag again
         article.name = u'Updated again article'
         tag.name = u'updated again tag'
         self.session.commit()
 
@@ -216,14 +217,15 @@
         self.session.commit()
 
         # update articles, add a 2nd child
         parent_article.name = u'Updated article'
         child_article1.name = u'Updated child article1'
         child_article2 = self.Article(name=u'Child article2',
                                       parent_article=parent_article)
+        self.session.add(child_article2)
         self.session.commit()
         # update the parent and 1st child
         parent_article.name = u'Updated article x2'
         child_article1.name = u'Updated child article1 x2'
         self.session.commit()
 
         assert len(parent_article.versions[1].child_articles) == 2
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/relationships/test_one_to_one_relations.py` & `SQLAlchemy-Continuum-1.4.0/tests/relationships/test_one_to_one_relations.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/revert/test_deep_relationships.py` & `SQLAlchemy-Continuum-1.4.0/tests/revert/test_deep_relationships.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/revert/test_many_to_many_relationships.py` & `SQLAlchemy-Continuum-1.4.0/tests/revert/test_many_to_many_relationships.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/revert/test_one_to_one_relationship.py` & `SQLAlchemy-Continuum-1.4.0/tests/revert/test_one_to_one_relationship.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/revert/test_one_to_one_with_secondary_table.py` & `SQLAlchemy-Continuum-1.4.0/tests/revert/test_one_to_one_with_secondary_table.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/schema/test_update_end_transaction_id.py` & `SQLAlchemy-Continuum-1.4.0/tests/schema/test_update_end_transaction_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sqlalchemy as sa
 from sqlalchemy_continuum import version_class
 from sqlalchemy_continuum.schema import update_end_tx_column
 from tests import TestCase
 
 
 class TestSchemaTools(TestCase):
     versioning_strategy = 'validity'
@@ -51,17 +52,17 @@
                 'transaction_id': 5,
                 'name': u'Article 2 updated',
                 'operation_type': 2,
             }
         )
 
         update_end_tx_column(table, conn=self.session)
-        rows = self.session.execute(
+        rows = self.session.execute(sa.text(
             'SELECT * FROM article_version ORDER BY transaction_id'
-        ).fetchall()
+        )).fetchall()
         assert rows[0].transaction_id == 1
         assert rows[0].end_transaction_id == 2
         assert rows[1].transaction_id == 2
         assert rows[1].end_transaction_id == 4
         assert rows[2].transaction_id == 3
         assert rows[2].end_transaction_id == 5
         assert rows[3].transaction_id == 4
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/schema/test_update_property_mod_flags.py` & `SQLAlchemy-Continuum-1.4.0/tests/schema/test_update_property_mod_flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,17 +80,17 @@
         )
 
         update_property_mod_flags(
             table,
             ['name'],
             conn=self.session
         )
-        rows = self.session.execute(
+        rows = self.session.execute(sa.text(
             'SELECT * FROM article_version ORDER BY transaction_id'
-        ).fetchall()
+        )).fetchall()
         assert rows[0].transaction_id == 1
         assert rows[0].name_mod
         assert rows[1].transaction_id == 2
         assert not rows[1].name_mod
         assert rows[2].transaction_id == 3
         assert rows[2].name_mod
         assert rows[3].transaction_id == 4
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_accessors.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_accessors.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         self.session.add(article)
         self.session.commit()
         article.name = u'Updated article'
         self.session.commit()
         article.content = u'Updated content'
         self.session.commit()
 
-        versions = article.versions.all()
+        versions = list(article.versions)
         version = versions[0]
         assert version.next == versions[1]
         assert version.next.next == versions[2]
 
     def test_index_for_deleted_parent(self):
         article = self.Article()
         article.name = u'Some article'
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_changeset.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_changeset.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,21 +43,21 @@
         self.session.add(tx_log)
         self.session.commit()
 
         # Needed when using native versioning
         self.session.expunge_all()
         tx_log = self.session.query(tx_log_class).first()
 
-        self.session.execute(
+        self.session.execute(sa.text(
             '''INSERT INTO article_version
             (id, %s, name, content, operation_type)
             VALUES
             (1, %d, 'something', 'some content', 1)
             ''' % (self.transaction_column_name, tx_log.id)
-        )
+        ))
 
         assert self.session.query(self.ArticleVersion).first().changeset == {
             'content': [None, 'some content'],
             'id': [None, 1],
             'name': [None, 'something']
         }
 
@@ -89,16 +89,16 @@
                 'base_classes': (self.Model,)
             }
 
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
             name = sa.Column(sa.Unicode(255))
             article_id = sa.Column(sa.Integer, sa.ForeignKey(Article.id))
             article = sa.orm.relationship(Article, backref='tags')
-
-        Article.tag_count = sa.orm.column_property(
-            sa.select([sa.func.count(Tag.id)])
-            .where(Tag.article_id == Article.id)
-            .correlate_except(Tag)
-        )
+        
+        subquery = (sa.select(sa.func.count(Tag.id))
+        .where(Tag.article_id == Article.id)
+        .correlate_except(Tag))
+        subquery = subquery.scalar_subquery()
+        Article.tag_count = sa.orm.column_property(subquery)
 
         self.Article = Article
         self.Tag = Tag
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_column_aliases.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_column_aliases.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_column_inclusion_and_exclusion.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_column_inclusion_and_exclusion.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_composite_primary_key.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_composite_primary_key.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_configuration.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_insert.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,119 +1,82 @@
-from pytest import raises, skip
 import sqlalchemy as sa
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy_continuum import (
-    versioning_manager, ImproperlyConfigured, TransactionFactory
-)
+from sqlalchemy_continuum import count_versions, versioning_manager
 
 from tests import TestCase
 
 
-class TestVersionedModelWithoutVersioning(TestCase):
-    def create_models(self):
-        class TextItem(self.Model):
-            __tablename__ = 'text_item'
-            __versioned__ = {
-                'versioning': False
-            }
-
-            id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
-
-        self.TextItem = TextItem
-
-    def test_does_not_create_history_class(self):
-        assert 'class' not in self.TextItem.__versioned__
-
-    def test_does_not_create_history_table(self):
-        assert 'text_item_history' not in self.Model.metadata.tables
-
-    def test_does_add_objects_to_unit_of_work(self):
-        self.session.add(self.TextItem())
+class TestInsert(TestCase):
+    def _insert(self):
+        article = self.Article()
+        article.name = u'Some article'
+        article.content = u'Some content'
+        self.session.add(article)
         self.session.commit()
+        return article
 
+    def test_insert_creates_version(self):
+        article = self._insert()
+        version = list(article.versions)[-1]
+        assert version.name == u'Some article'
+        assert version.content == u'Some content'
+        assert version.transaction.id == version.transaction_id
+
+    def test_stores_operation_type(self):
+        article = self._insert()
+        assert article.versions[0].operation_type == 0
+
+    def test_multiple_consecutive_flushes(self):
+        article = self.Article()
+        article.name = u'Some article'
+        article.content = u'Some content'
+        self.session.add(article)
+        self.session.flush()
+        article2 = self.Article()
+        article2.name = u'Some article'
+        article2.content = u'Some content'
+        self.session.add(article2)
+        self.session.flush()
+        self.session.commit()
+        assert article.versions.count() == 1
+        assert article2.versions.count() == 1
 
-class TestWithUnknownUserClass(object):
-    def test_raises_improperly_configured_error(self):
-        self.Model = declarative_base()
 
+class TestInsertWithDeferredColumn(TestCase):
+    def create_models(self):
         class TextItem(self.Model):
             __tablename__ = 'text_item'
             __versioned__ = {}
-
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
+            name = sa.orm.deferred(sa.Column(sa.Unicode(255)))
 
         self.TextItem = TextItem
 
-        versioning_manager.user_cls = 'User'
-        versioning_manager.declarative_base = self.Model
-
-        factory = TransactionFactory()
-        with raises(ImproperlyConfigured):
-            factory(versioning_manager)
-
+    def test_insert(self):
+        item = self.TextItem()
+        self.session.add(item)
+        self.session.commit()
+        assert count_versions(item) == 1
 
-class TestWithCreateModelsAsFalse(TestCase):
-    should_create_models = False
 
+class TestInsertNonVersionedObject(TestCase):
     def create_models(self):
-        class Article(self.Model):
-            __tablename__ = 'article'
-            __versioned__ = {}
-
+        class TextItem(self.Model):
+            __tablename__ = 'text_item'
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
-            name = sa.Column(sa.Unicode(255), nullable=False)
-            content = sa.Column(sa.UnicodeText)
-            description = sa.Column(sa.UnicodeText)
+            name = sa.orm.deferred(sa.Column(sa.Unicode(255)))
 
-        class Category(self.Model):
-            __tablename__ = 'category'
+        class Tag(self.Model):
+            __tablename__ = 'tag'
             __versioned__ = {}
-
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
-            name = sa.Column(sa.Unicode(255))
-            article_id = sa.Column(sa.Integer, sa.ForeignKey(Article.id))
-            article = sa.orm.relationship(
-                Article,
-                backref=sa.orm.backref(
-                    'category',
-                    uselist=False
-                )
-            )
+            name = sa.orm.deferred(sa.Column(sa.Unicode(255)))
 
-        self.Article = Article
-        self.Category = Category
-
-    def test_does_not_create_models(self):
-        assert 'class' not in self.Article.__versioned__
+        self.TextItem = TextItem
 
-    def test_insert(self):
-        if self.options['native_versioning'] is False:
-            skip()
-        article = self.Article(name=u'Some article')
-        self.session.add(article)
+    def test_does_not_create_transaction(self):
+        item = self.TextItem()
+        self.session.add(item)
         self.session.commit()
 
-        version = dict(
-            self.session.execute('SELECT * FROM article_version')
-            .fetchone()
-        )
-        assert version['transaction_id'] > 0
-        assert version['id'] == article.id
-        assert version['name'] == u'Some article'
-
-
-class TestWithoutAnyVersionedModels(TestCase):
-    def create_models(self):
-        class Article(self.Model):
-            __tablename__ = 'article'
-
-            id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
-            name = sa.Column(sa.Unicode(255), nullable=False)
-            content = sa.Column(sa.UnicodeText)
-            description = sa.Column(sa.UnicodeText)
-
-        self.Article = Article
-
-    def test_insert(self):
-        article = self.Article(name=u'Some article')
-        self.session.add(article)
-        self.session.commit()
+        assert self.session.query(
+            versioning_manager.transaction_cls
+        ).count() == 0
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_custom_schema.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_custom_schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import os
 import sqlalchemy as sa
-from six import PY3
 from pytest import mark
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import declarative_base
 from tests import TestCase
 
 
-@mark.skipif("os.environ.get('DB') == 'sqlite'")
 class TestCustomSchema(TestCase):
     def create_models(self):
-        self.Model = declarative_base(metadata=sa.MetaData(schema='continuum'))
+        self.Model = declarative_base(metadata=sa.MetaData(schema='other'))
 
         class Article(self.Model):
             __tablename__ = 'article'
             __versioned__ = {
                 'base_classes': (self.Model, )
             }
 
@@ -51,19 +49,14 @@
             secondary=article_tag,
             backref='tags'
         )
 
         self.Article = Article
         self.Tag = Tag
 
-    def create_tables(self):
-        self.connection.execute('DROP SCHEMA IF EXISTS continuum')
-        self.connection.execute('CREATE SCHEMA continuum')
-        TestCase.create_tables(self)
-
     def test_version_relations(self):
         article = self.Article()
         article.name = u'Some article'
         article.content = u'Some content'
         self.session.add(article)
         self.session.commit()
         assert article.versions[0].tags == []
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_custom_version_base_class.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_custom_version_base_class.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_delete.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_exotic_listener_chaining.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_exotic_listener_chaining.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_exotic_operation_combos.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_exotic_operation_combos.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_i18n.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_i18n.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import sqlalchemy as sa
 from sqlalchemy_continuum import versioning_manager
 from sqlalchemy_i18n import Translatable, make_translatable, translation_base
 from sqlalchemy_utils import i18n
 from . import TestCase
 
+# sqlalchemy-i18n doesn't fully support 1.4 yet
+# See https://github.com/kvesteri/sqlalchemy-i18n/issues/34
+import pytest
+pytest.skip(allow_module_level=True)
+
 
 i18n.get_locale = lambda: 'en'
 make_translatable()
 
 
 class TestVersioningWithI18nExtension(TestCase):
     def create_models(self):
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_insert.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_mapper_args.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,85 @@
-import sqlalchemy as sa
-from sqlalchemy_continuum import count_versions, versioning_manager
+from pytest import mark
+from packaging import version
 
+import sqlalchemy as sa
+from sqlalchemy_continuum import version_class
 from tests import TestCase
 
 
-class TestInsert(TestCase):
-    def _insert(self):
-        article = self.Article()
-        article.name = u'Some article'
-        article.content = u'Some content'
-        self.session.add(article)
-        self.session.commit()
-        return article
-
-    def test_insert_creates_version(self):
-        article = self._insert()
-        version = article.versions.all()[-1]
-        assert version.name == u'Some article'
-        assert version.content == u'Some content'
-        assert version.transaction.id == version.transaction_id
-
-    def test_stores_operation_type(self):
-        article = self._insert()
-        assert article.versions[0].operation_type == 0
-
-    def test_multiple_consecutive_flushes(self):
-        article = self.Article()
-        article.name = u'Some article'
-        article.content = u'Some content'
-        self.session.add(article)
-        self.session.flush()
-        article2 = self.Article()
-        article2.name = u'Some article'
-        article2.content = u'Some content'
-        self.session.add(article2)
-        self.session.flush()
-        self.session.commit()
-        assert article.versions.count() == 1
-        assert article2.versions.count() == 1
+class TestColumnPrefix(TestCase):
+    def create_models(self):
+        class TextItem(self.Model):
+            __tablename__ = 'text_item'
+            __versioned__ = {
+                'base_classes': (self.Model, )
+            }
+            id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
+
+            name = sa.Column(sa.Unicode(255))
+
+            __mapper_args__ = {
+                'column_prefix': '_'
+            }
+
+        self.TextItem = TextItem
+
+    def setup_method(self, method):
+        TestCase.setup_method(self, method)
+        self.TextItemVersion = version_class(self.TextItem)
+
+    def test_supports_column_prefix(self):
+        assert self.TextItemVersion._id
+        assert self.TextItem._id
 
 
-class TestInsertWithDeferredColumn(TestCase):
+@mark.skipif("version.parse(sa.__version__) >= version.parse('1.4')")
+class TestOrderByWithStringArg(TestCase):
     def create_models(self):
         class TextItem(self.Model):
             __tablename__ = 'text_item'
-            __versioned__ = {}
+            __versioned__ = {
+                'base_classes': (self.Model, )
+            }
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
-            name = sa.orm.deferred(sa.Column(sa.Unicode(255)))
+
+            name = sa.Column(sa.Unicode(255))
+
+            __mapper_args__ = {
+                'order_by': 'id',
+                'column_prefix': '_'
+            }
 
         self.TextItem = TextItem
 
-    def test_insert(self):
-        item = self.TextItem()
-        self.session.add(item)
-        self.session.commit()
-        assert count_versions(item) == 1
+    def setup_method(self, method):
+        TestCase.setup_method(self, method)
+        self.TextItemVersion = version_class(self.TextItem)
 
+    def test_reflects_order_by(self):
+        assert self.TextItemVersion.__mapper_args__['order_by'] == 'id'
 
-class TestInsertNonVersionedObject(TestCase):
+
+@mark.skipif("version.parse(sa.__version__) >= version.parse('1.4')")
+class TestOrderByWithInstrumentedAttribute(TestCase):
     def create_models(self):
         class TextItem(self.Model):
             __tablename__ = 'text_item'
+            __versioned__ = {
+                'base_classes': (self.Model, )
+            }
             id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
-            name = sa.orm.deferred(sa.Column(sa.Unicode(255)))
 
-        class Tag(self.Model):
-            __tablename__ = 'tag'
-            __versioned__ = {}
-            id = sa.Column(sa.Integer, autoincrement=True, primary_key=True)
-            name = sa.orm.deferred(sa.Column(sa.Unicode(255)))
+            name = sa.Column(sa.Unicode(255))
+
+            __mapper_args__ = {
+                'order_by': id
+            }
 
         self.TextItem = TextItem
 
-    def test_does_not_create_transaction(self):
-        item = self.TextItem()
-        self.session.add(item)
-        self.session.commit()
-
-        assert self.session.query(
-            versioning_manager.transaction_cls
-        ).count() == 0
+    def setup_method(self, method):
+        TestCase.setup_method(self, method)
+        self.TextItemVersion = version_class(self.TextItem)
+
+    def test_reflects_order_by(self):
+        assert 'order_by' not in self.TextItemVersion.__mapper_args__
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_raw_sql.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_raw_sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import pytest
+import sqlalchemy as sa
 from sqlalchemy_continuum import versioning_manager
 
 from tests import TestCase, uses_native_versioning
 
 
 @pytest.mark.skipif('not uses_native_versioning()')
 class TestRawSQL(TestCase):
     def assert_has_single_transaction(self):
         assert (
             self.session.query(versioning_manager.transaction_cls)
             .count() == 1
         )
 
     def test_flush_after_raw_insert(self):
-        self.session.execute(
+        self.session.execute(sa.text(
             "INSERT INTO article (name) VALUES ('some article')"
-        )
+        ))
         self.session.add(self.Article(name=u'some other article'))
         self.session.commit()
         self.assert_has_single_transaction()
 
     def test_raw_insert_after_flush(self):
         self.session.add(self.Article(name=u'some other article'))
         self.session.flush()
-        self.session.execute(
+        self.session.execute(sa.text(
             "INSERT INTO article (name) VALUES ('some article')"
-        )
+        ))
         self.session.commit()
         self.assert_has_single_transaction()
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_revert.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_revert.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_sessions.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_sessions.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,50 +3,50 @@
 from sqlalchemy_continuum import versioning_manager, UnitOfWork
 from tests import TestCase
 
 
 class TestSessions(TestCase):
     plugins = []
 
+    def test_new_session(self):
+        self.session2 = Session(bind=self.engine)
+        article = self.Article(name=u'Session2 article')
+        self.session2.add(article)
+        self.session2.commit()
+        assert list(article.versions)[-1].transaction_id
+
     def test_multiple_connections(self):
         self.session2 = Session(bind=self.engine.connect())
         article = self.Article(name=u'Session1 article')
         article2 = self.Article(name=u'Session2 article')
         self.session.add(article)
         self.session2.add(article2)
         self.session.flush()
         self.session2.flush()
 
         self.session.commit()
         self.session2.commit()
-        assert article.versions[-1].transaction_id
+        assert list(article.versions)[-1].transaction_id
         assert (
-            article2.versions[-1].transaction_id >
-            article.versions[-1].transaction_id
+            list(article2.versions)[-1].transaction_id >
+            list(article.versions)[-1].transaction_id
         )
 
-    def test_connection_binded_to_engine(self):
-        self.session2 = Session(bind=self.engine)
-        article = self.Article(name=u'Session1 article')
-        self.session2.add(article)
-        self.session2.commit()
-        assert article.versions[-1].transaction_id
-
     def test_manual_transaction_creation(self):
         uow = versioning_manager.unit_of_work(self.session)
         transaction = uow.create_transaction(self.session)
         self.session.flush()
         assert transaction.id
         article = self.Article(name=u'Session1 article')
         self.session.add(article)
         self.session.flush()
         assert uow.current_transaction.id
 
         self.session.commit()
-        assert article.versions[-1].transaction_id
+        assert list(article.versions)[-1].transaction_id
 
     def test_commit_without_objects(self):
         self.session.commit()
 
 
 class TestUnitOfWork(TestCase):
     def test_with_session_arg(self):
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_transaction.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_transaction.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import sqlalchemy as sa
 from sqlalchemy_continuum import versioning_manager
 from tests import TestCase
 from pytest import mark
+from sqlalchemy_continuum.plugins import TransactionMetaPlugin
+
 
 
 class TestTransaction(TestCase):
     def setup_method(self, method):
         TestCase.setup_method(self, method)
         self.article = self.Article()
         self.article.name = u'Some article'
@@ -34,14 +36,27 @@
             '<Transaction id=%d, issued_at=%r>' % (
                 transaction.id,
                 transaction.issued_at
             ) ==
             repr(transaction)
         )
 
+    def test_changed_entities(self):
+        article_v0 = self.article.versions[0]
+        transaction = article_v0.transaction
+        assert transaction.changed_entities == {
+            self.ArticleVersion: [article_v0],
+            self.TagVersion: [self.article.tags[0].versions[0]],
+        }
+
+
+# Check that the tests pass without TransactionChangesPlugin
+class TestTransactionWithoutChangesPlugin(TestTransaction):
+    plugins = [TransactionMetaPlugin()]
+
 
 class TestAssigningUserClass(TestCase):
     user_cls = 'User'
 
     def create_models(self):
         class User(self.Model):
             __tablename__ = 'user'
@@ -55,15 +70,14 @@
         self.User = User
 
     def test_copies_primary_key_type_from_user_class(self):
         attr = versioning_manager.transaction_cls.user_id
         assert isinstance(attr.property.columns[0].type, sa.Unicode)
 
 
-@mark.skipif("os.environ.get('DB') == 'sqlite'")
 class TestAssigningUserClassInOtherSchema(TestCase):
     user_cls = 'User'
 
     def create_models(self):
         class User(self.Model):
             __tablename__ = 'user'
             __versioned__ = {
@@ -72,16 +86,11 @@
             __table_args__ = {'schema': 'other'}
 
             id = sa.Column(sa.Unicode(255), primary_key=True)
             name = sa.Column(sa.Unicode(255), nullable=False)
 
         self.User = User
 
-    def create_tables(self):
-        self.connection.execute('DROP SCHEMA IF EXISTS other')
-        self.connection.execute('CREATE SCHEMA other')
-        TestCase.create_tables(self)
-
     def test_can_build_transaction_model(self):
         # If create_models didn't crash this should be good
         pass
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_update.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self.session.commit()
 
         article.name = u'Updated name'
         article.content = u'Updated content'
 
         self.session.commit()
         self.session.refresh(article)
-        version = article.versions.all()[-1]
+        version = list(article.versions)[-1]
         assert version.name == u'Updated name'
         assert version.content == u'Updated content'
         assert version.transaction.id == version.transaction_id
 
     def test_partial_update(self):
         article = self.Article()
         article.name = u'Some article'
@@ -27,15 +27,15 @@
         self.session.add(article)
         self.session.commit()
 
         article.content = u'Updated content'
 
         self.session.commit()
         self.session.refresh(article)
-        version = article.versions.all()[-1]
+        version = list(article.versions)[-1]
         assert version.name == u'Some article'
         assert version.content == u'Updated content'
         assert version.transaction.id == version.transaction_id
 
     def test_update_with_same_values(self):
         article = self.Article()
         article.name = u'Some article'
@@ -54,29 +54,29 @@
         article.content = u'Some content'
         self.session.add(article)
         self.session.commit()
 
         article.name = u'Some other article'
 
         self.session.commit()
-        assert article.versions[-1].operation_type == 1
+        assert list(article.versions)[-1].operation_type == 1
 
     def test_multiple_updates_within_same_transaction(self):
         article = self.Article()
         article.name = u'Some article'
         article.content = u'Some content'
         self.session.add(article)
         self.session.commit()
 
         article.content = u'Updated content'
         self.session.flush()
         article.content = u'Updated content 2'
         self.session.commit()
         assert article.versions.count() == 2
-        version = article.versions.all()[-1]
+        version = list(article.versions)[-1]
         assert version.name == u'Some article'
         assert version.content == u'Updated content 2'
 
 
 class TestUpdateWithDefaultValues(TestCase):
     def create_models(self):
         class Article(self.Model):
@@ -97,9 +97,9 @@
         article.name = u'Some article'
         article.is_editable = False
         self.session.add(article)
         self.session.commit()
 
         article.is_editable = True
         self.session.commit()
-        article = article.versions.all()[-1]
+        article = list(article.versions)[-1]
         assert article.name == u'Some article'
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_vacuum.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_vacuum.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_validity_strategy.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_validity_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         assert table.c.end_transaction_id.nullable
         assert not table.c.end_transaction_id.primary_key
 
     def test_end_transaction_id_none_for_newly_inserted_record(self):
         article = self.Article(name=u'Something')
         self.session.add(article)
         self.session.commit()
-        assert article.versions[-1].end_transaction_id is None
+        assert list(article.versions)[-1].end_transaction_id is None
 
     def test_updated_end_transaction_id_of_previous_version(self):
         article = self.Article(name=u'Something')
         self.session.add(article)
         self.session.commit()
 
         article.name = u'Some other thing'
         self.session.commit()
         assert (
-            article.versions[-2].end_transaction_id ==
-            article.versions[-1].transaction_id
+            list(article.versions)[-2].end_transaction_id ==
+            list(article.versions)[-1].transaction_id
         )
 
 
 class TestJoinTableInheritanceWithValidityVersioning(TestCase):
     def create_models(self):
         class TextItem(self.Model):
             __tablename__ = 'text_item'
```

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/test_versions.py` & `SQLAlchemy-Continuum-1.4.0/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/utils/test_changeset.py` & `SQLAlchemy-Continuum-1.4.0/tests/utils/test_changeset.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/utils/test_count_versions.py` & `SQLAlchemy-Continuum-1.4.0/tests/utils/test_count_versions.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/utils/test_is_modified.py` & `SQLAlchemy-Continuum-1.4.0/tests/utils/test_is_modified.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/utils/test_tx_column_name.py` & `SQLAlchemy-Continuum-1.4.0/tests/utils/test_tx_column_name.py`

 * *Files identical despite different names*

### Comparing `SQLAlchemy-Continuum-1.3.9/tests/utils/test_version_class.py` & `SQLAlchemy-Continuum-1.4.0/tests/utils/test_version_class.py`

 * *Files identical despite different names*


# Comparing `tmp/signac-2.0.0.tar.gz` & `tmp/signac-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signac-2.0.0.tar", last modified: Thu Mar 30 19:22:31 2023, max compression
+gzip compressed data, was "signac-2.1.0.tar", last modified: Wed Jul 12 16:55:40 2023, max compression
```

## Comparing `signac-2.0.0.tar` & `signac-2.1.0.tar`

### file list

```diff
@@ -1,83 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:22:31.008231 signac-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-30 19:21:57.000000 signac-2.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-30 19:21:57.000000 signac-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-03-30 19:22:31.008231 signac-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-03-30 19:21:57.000000 signac-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-03-30 19:21:57.000000 signac-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 19:22:31.008231 signac-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:22:31.000231 signac-2.0.0/signac/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-30 19:21:57.000000 signac-2.0.0/signac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52808 2023-03-30 19:21:57.000000 signac-2.0.0/signac/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_dict_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_search_indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:22:31.000231 signac-2.0.0/signac/_synced_collections/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/_caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:22:31.000231 signac-2.0.0/signac/_synced_collections/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21341 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/backends/collection_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/backends/collection_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/backends/collection_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/backends/collection_zarr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:22:31.004231 signac-2.0.0/signac/_synced_collections/buffers/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/buffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/buffers/buffered_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/buffers/file_buffered_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/buffers/memory_buffered_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/buffers/serialized_file_buffered_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:22:31.004231 signac-2.0.0/signac/_synced_collections/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/data_types/attr_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/data_types/synced_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/data_types/synced_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/data_types/synced_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_synced_collections/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:22:31.004231 signac-2.0.0/signac/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:22:31.004231 signac-2.0.0/signac/_vendor/configobj/
--rw-r--r--   0 runner    (1001) docker     (123)    88462 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_vendor/configobj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_vendor/configobj/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    47125 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_vendor/configobj/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:22:31.004231 signac-2.0.0/signac/_vendor/deprecation/
--rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-03-30 19:21:57.000000 signac-2.0.0/signac/_vendor/deprecation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-03-30 19:21:57.000000 signac-2.0.0/signac/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-03-30 19:21:57.000000 signac-2.0.0/signac/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-03-30 19:21:57.000000 signac-2.0.0/signac/filterparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16545 2023-03-30 19:21:57.000000 signac-2.0.0/signac/h5store.py
--rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-03-30 19:21:57.000000 signac-2.0.0/signac/import_export.py
--rw-r--r--   0 runner    (1001) docker     (123)    32653 2023-03-30 19:21:57.000000 signac-2.0.0/signac/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-03-30 19:21:57.000000 signac-2.0.0/signac/linked_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:22:31.004231 signac-2.0.0/signac/migration/
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-03-30 19:21:57.000000 signac-2.0.0/signac/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-30 19:21:57.000000 signac-2.0.0/signac/migration/v0_to_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-03-30 19:21:57.000000 signac-2.0.0/signac/migration/v1_to_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    74343 2023-03-30 19:21:57.000000 signac-2.0.0/signac/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-03-30 19:21:57.000000 signac-2.0.0/signac/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    31433 2023-03-30 19:21:57.000000 signac-2.0.0/signac/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-30 19:21:57.000000 signac-2.0.0/signac/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:22:31.000231 signac-2.0.0/signac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-03-30 19:22:30.000000 signac-2.0.0/signac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-30 19:22:30.000000 signac-2.0.0/signac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 19:22:30.000000 signac-2.0.0/signac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-30 19:22:30.000000 signac-2.0.0/signac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-30 19:22:30.000000 signac-2.0.0/signac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-30 19:22:30.000000 signac-2.0.0/signac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 19:22:31.008231 signac-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-03-30 19:21:57.000000 signac-2.0.0/tests/test_buffered_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-30 19:21:57.000000 signac-2.0.0/tests/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-03-30 19:21:57.000000 signac-2.0.0/tests/test_find_command_line_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    30835 2023-03-30 19:21:57.000000 signac-2.0.0/tests/test_h5store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-03-30 19:21:57.000000 signac-2.0.0/tests/test_h5store_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    64505 2023-03-30 19:21:57.000000 signac-2.0.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-03-30 19:21:57.000000 signac-2.0.0/tests/test_numpy_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-03-30 19:21:57.000000 signac-2.0.0/tests/test_pandas_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)   102205 2023-03-30 19:21:57.000000 signac-2.0.0/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-03-30 19:21:57.000000 signac-2.0.0/tests/test_searchindexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-03-30 19:21:57.000000 signac-2.0.0/tests/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    25568 2023-03-30 19:21:57.000000 signac-2.0.0/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-30 19:21:57.000000 signac-2.0.0/tests/test_temporary_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:55:40.536379 signac-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-12 16:55:05.000000 signac-2.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 16:55:05.000000 signac-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-12 16:55:40.532379 signac-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-12 16:55:05.000000 signac-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-12 16:55:05.000000 signac-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 16:55:40.536379 signac-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:55:40.528379 signac-2.1.0/signac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-12 16:55:05.000000 signac-2.1.0/signac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52808 2023-07-12 16:55:05.000000 signac-2.1.0/signac/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-12 16:55:05.000000 signac-2.1.0/signac/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-12 16:55:05.000000 signac-2.1.0/signac/_dict_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-07-12 16:55:05.000000 signac-2.1.0/signac/_search_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-12 16:55:05.000000 signac-2.1.0/signac/_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:55:40.528379 signac-2.1.0/signac/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-12 16:55:05.000000 signac-2.1.0/signac/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:55:40.528379 signac-2.1.0/signac/_vendor/configobj/
+-rw-r--r--   0 runner    (1001) docker     (123)    88462 2023-07-12 16:55:05.000000 signac-2.1.0/signac/_vendor/configobj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 16:55:05.000000 signac-2.1.0/signac/_vendor/configobj/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47125 2023-07-12 16:55:05.000000 signac-2.1.0/signac/_vendor/configobj/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:55:40.532379 signac-2.1.0/signac/_vendor/deprecation/
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-07-12 16:55:05.000000 signac-2.1.0/signac/_vendor/deprecation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-12 16:55:05.000000 signac-2.1.0/signac/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-12 16:55:05.000000 signac-2.1.0/signac/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-12 16:55:05.000000 signac-2.1.0/signac/filterparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16545 2023-07-12 16:55:05.000000 signac-2.1.0/signac/h5store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-07-12 16:55:05.000000 signac-2.1.0/signac/import_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32640 2023-07-12 16:55:05.000000 signac-2.1.0/signac/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-12 16:55:05.000000 signac-2.1.0/signac/linked_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:55:40.532379 signac-2.1.0/signac/migration/
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-12 16:55:05.000000 signac-2.1.0/signac/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-12 16:55:05.000000 signac-2.1.0/signac/migration/v0_to_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-12 16:55:05.000000 signac-2.1.0/signac/migration/v1_to_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74472 2023-07-12 16:55:05.000000 signac-2.1.0/signac/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-07-12 16:55:05.000000 signac-2.1.0/signac/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31433 2023-07-12 16:55:05.000000 signac-2.1.0/signac/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-12 16:55:05.000000 signac-2.1.0/signac/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:55:40.528379 signac-2.1.0/signac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-12 16:55:40.000000 signac-2.1.0/signac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-12 16:55:40.000000 signac-2.1.0/signac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:55:40.000000 signac-2.1.0/signac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 16:55:40.000000 signac-2.1.0/signac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-12 16:55:40.000000 signac-2.1.0/signac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 16:55:40.000000 signac-2.1.0/signac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:55:40.532379 signac-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-07-12 16:55:05.000000 signac-2.1.0/tests/test_buffered_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-12 16:55:05.000000 signac-2.1.0/tests/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-12 16:55:05.000000 signac-2.1.0/tests/test_find_command_line_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30835 2023-07-12 16:55:05.000000 signac-2.1.0/tests/test_h5store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-12 16:55:05.000000 signac-2.1.0/tests/test_h5store_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64505 2023-07-12 16:55:05.000000 signac-2.1.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-12 16:55:05.000000 signac-2.1.0/tests/test_numpy_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-12 16:55:05.000000 signac-2.1.0/tests/test_pandas_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102205 2023-07-12 16:55:05.000000 signac-2.1.0/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16849 2023-07-12 16:55:05.000000 signac-2.1.0/tests/test_searchindexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-07-12 16:55:05.000000 signac-2.1.0/tests/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25568 2023-07-12 16:55:05.000000 signac-2.1.0/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-12 16:55:05.000000 signac-2.1.0/tests/test_temporary_project.py
```

### Comparing `signac-2.0.0/LICENSE.txt` & `signac-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/PKG-INFO` & `signac-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signac
-Version: 2.0.0
+Version: 2.1.0
 Summary: Manage large and heterogeneous data spaces on the file system.
 Author-email: "Carl Simon Adorf et al." <csadorf@umich.edu>
 Maintainer-email: signac Developers <signac-support@umich.edu>
 License: BSD 3-Clause License for the software signac.
         
         Copyright (c) 2016, The Regents of the University of Michigan
         All rights reserved.
@@ -108,15 +108,15 @@
 
 The framework facilitates a project-based workflow.
 Set up a new project:
 
 ```bash
 $ mkdir my_project
 $ cd my_project
-$ signac init MyProject
+$ signac init
 ```
 
 and access the project handle:
 
 ```python
 >>> project = signac.get_project()
 ```
```

### Comparing `signac-2.0.0/README.md` & `signac-2.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 The framework facilitates a project-based workflow.
 Set up a new project:
 
 ```bash
 $ mkdir my_project
 $ cd my_project
-$ signac init MyProject
+$ signac init
 ```
 
 and access the project handle:
 
 ```python
 >>> project = signac.get_project()
 ```
```

### Comparing `signac-2.0.0/pyproject.toml` & `signac-2.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This software is licensed under the BSD 3-Clause License.
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=64.0.0"]
 
 [project]
 name = "signac"
-version = "2.0.0"
+version = "2.1.0"
 description = "Manage large and heterogeneous data spaces on the file system."
 readme = "README.md"
 # Supported versions are determined according to NEP 29.
 # https://numpy.org/neps/nep-0029-deprecation_policy.html
 requires-python = ">=3.8"
 license = { file = "LICENSE.txt" }
 maintainers = [{ name = "signac Developers", email = "signac-support@umich.edu" }]
@@ -31,14 +31,16 @@
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     # Platform-independent file locking
     "filelock>=3.0",
     # Used for version parsing and comparison
     "packaging>=15.0",
+    # Synced collections for signac's backend
+    "synced_collections>=1.0.0",
     # Progress bars
     "tqdm>=4.10.0",
 ]
 
 [project.optional-dependencies]
 h5 = ["h5py"]
```

### Comparing `signac-2.0.0/signac/__init__.py` & `signac-2.1.0/signac/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 
 It provides a simple and robust data model to create a well-defined, indexable
 storage layout for data and metadata. This makes it easier to operate on large
 data spaces, streamlines post-processing and analysis, and makes data
 collectively accessible.
 """
 
+from synced_collections.backends.collection_json import BufferedJSONAttrDict as JSONDict
+
 from . import errors, sync
-from ._synced_collections.backends.collection_json import (
-    BufferedJSONAttrDict as JSONDict,
-)
 from .diff import diff_jobs
 from .h5store import H5Store, H5StoreManager
 from .project import Project, TemporaryProject, get_job, get_project, init_project
 from .version import __version__
 
 # Alias some properties related to buffering into the signac namespace.
 buffered = JSONDict.buffer_backend
```

### Comparing `signac-2.0.0/signac/__main__.py` & `signac-2.1.0/signac/__main__.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/_config.py` & `signac-2.1.0/signac/_config.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/_dict_manager.py` & `signac-2.1.0/signac/_dict_manager.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/_search_indexer.py` & `signac-2.1.0/signac/_search_indexer.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/_utility.py` & `signac-2.1.0/signac/_utility.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/_vendor/configobj/__init__.py` & `signac-2.1.0/signac/_vendor/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/_vendor/configobj/validate.py` & `signac-2.1.0/signac/_vendor/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/_vendor/deprecation/__init__.py` & `signac-2.1.0/signac/_vendor/deprecation/__init__.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/diff.py` & `signac-2.1.0/signac/diff.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/errors.py` & `signac-2.1.0/signac/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) 2017 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 """Errors raised by signac."""
 
-from ._synced_collections.errors import InvalidKeyError, KeyTypeError
+from synced_collections.errors import InvalidKeyError, KeyTypeError
 
 
 class Error(Exception):
     """Base class used for signac Errors."""
 
     pass
```

### Comparing `signac-2.0.0/signac/filterparse.py` & `signac-2.1.0/signac/filterparse.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/h5store.py` & `signac-2.1.0/signac/h5store.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/import_export.py` & `signac-2.1.0/signac/import_export.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/job.py` & `signac-2.1.0/signac/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 import logging
 import os
 import shutil
 from copy import deepcopy
 from threading import RLock
 from typing import FrozenSet
 
-from ._synced_collections.backends.collection_json import (
+from synced_collections.backends.collection_json import (
     BufferedJSONAttrDict,
     JSONAttrDict,
     json_attr_dict_validator,
 )
-from ._synced_collections.errors import KeyTypeError
-from ._synced_collections.utils import SyncedCollectionJSONEncoder
+from synced_collections.errors import KeyTypeError
+from synced_collections.utils import SyncedCollectionJSONEncoder
+
 from ._utility import _mkdir_p
 from .errors import DestinationExistsError, JobsCorruptedError
 from .h5store import H5StoreManager
 from .sync import sync_jobs
 
 logger = logging.getLogger(__name__)
 
@@ -420,15 +421,15 @@
             The state point object behaves like a dictionary in most cases,
             but because it persists changes to the filesystem, making a copy
             requires explicitly converting it to a dict. If you need a
             modifiable copy that will not modify the underlying JSON file,
             you can access a dict copy of the state point by calling it, e.g.
             ``sp_dict = job.statepoint()`` instead of ``sp = job.statepoint``.
             For more information, see
-            :class:`~signac._synced_collections.backends.collection_json.JSONAttrDict`.
+            :class:`~synced_collections.backends.collection_json.JSONAttrDict`.
 
         See :ref:`signac statepoint <signac-cli-statepoint>` for the command line equivalent.
 
         .. danger::
 
             Use this function with caution! Resetting a job's state point
             may sometimes be necessary, but can possibly lead to incoherent
```

### Comparing `signac-2.0.0/signac/linked_view.py` & `signac-2.1.0/signac/linked_view.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/migration/__init__.py` & `signac-2.1.0/signac/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/migration/v0_to_v1.py` & `signac-2.1.0/signac/migration/v0_to_v1.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/migration/v1_to_v2.py` & `signac-2.1.0/signac/migration/v1_to_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,17 @@
       solely by their directories.
     - Removing the workspace_dir key from the config. The workspace directory
       is no longer configurable.
 """
 
 import os
 
+from synced_collections.backends.collection_json import BufferedJSONAttrDict
+
 from .._config import _get_project_config_fn
-from .._synced_collections.backends.collection_json import BufferedJSONAttrDict
 from .._vendor import configobj
 from ..project import Project
 from .v0_to_v1 import _load_config_v1
 
 # A minimal v2 config.
 _CFG = """
 schema_version = string(default='0')
```

### Comparing `signac-2.0.0/signac/project.py` & `signac-2.1.0/signac/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 from contextlib import contextmanager
 from datetime import timedelta
 from itertools import groupby
 from multiprocessing.pool import ThreadPool
 from tempfile import TemporaryDirectory
 from threading import RLock
 
+from synced_collections.backends.collection_json import BufferedJSONAttrDict
+
 from ._config import (
     _Config,
     _get_project_config_fn,
     _load_config,
     _locate_config_dir,
     _raise_if_older_schema,
     _read_config_file,
 )
 from ._search_indexer import _SearchIndexer
-from ._synced_collections.backends.collection_json import BufferedJSONAttrDict
 from ._utility import _mkdir_p, _nested_dicts_to_dotted_keys
 from .errors import (
     DestinationExistsError,
     IncompatibleSchemaVersion,
     JobsCorruptedError,
     WorkspaceError,
 )
@@ -512,17 +513,19 @@
         KeyError
             If the attempt to open the job by id fails.
         LookupError
             If the attempt to open the job by an abbreviated id returns more
             than one match.
 
         """
-        if (statepoint is None) == (id is None):
+        if statepoint is None and id is None:
+            raise ValueError("Must provide statepoint or id.")
+        elif statepoint is not None and id is not None:
             raise ValueError("Either statepoint or id must be provided, but not both.")
-        if id is None:
+        elif statepoint is not None:
             # Second best case (Job will update self._sp_cache on init)
             return Job(project=self, statepoint=statepoint)
         try:
             # Optimal case (id is in the state point cache)
             return Job(project=self, statepoint=self._sp_cache[id], id_=id)
         except KeyError:
             # Worst case: no state point was provided and the state point cache
```

### Comparing `signac-2.0.0/signac/schema.py` & `signac-2.1.0/signac/schema.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac/sync.py` & `signac-2.1.0/signac/sync.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/signac.egg-info/PKG-INFO` & `signac-2.1.0/signac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signac
-Version: 2.0.0
+Version: 2.1.0
 Summary: Manage large and heterogeneous data spaces on the file system.
 Author-email: "Carl Simon Adorf et al." <csadorf@umich.edu>
 Maintainer-email: signac Developers <signac-support@umich.edu>
 License: BSD 3-Clause License for the software signac.
         
         Copyright (c) 2016, The Regents of the University of Michigan
         All rights reserved.
@@ -108,15 +108,15 @@
 
 The framework facilitates a project-based workflow.
 Set up a new project:
 
 ```bash
 $ mkdir my_project
 $ cd my_project
-$ signac init MyProject
+$ signac init
 ```
 
 and access the project handle:
 
 ```python
 >>> project = signac.get_project()
 ```
```

### Comparing `signac-2.0.0/tests/test_buffered_mode.py` & `signac-2.1.0/tests/test_buffered_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import os
 import platform
 from stat import S_IREAD
 from tempfile import TemporaryDirectory
 from time import sleep
 
 import pytest
+from synced_collections.errors import BufferedError
 from test_project import TestProjectBase
 
 import signac
-from signac._synced_collections.errors import BufferedError
 
 PYPY = "PyPy" in platform.python_implementation()
 
 
 # Determine if we can run permission error tests
 with TemporaryDirectory() as tmp_dir:
     path = os.path.join(tmp_dir, "subdir")
```

### Comparing `signac-2.0.0/tests/test_diff.py` & `signac-2.1.0/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/tests/test_find_command_line_interface.py` & `signac-2.1.0/tests/test_find_command_line_interface.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/tests/test_h5store.py` & `signac-2.1.0/tests/test_h5store.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/tests/test_h5store_manager.py` & `signac-2.1.0/tests/test_h5store_manager.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/tests/test_job.py` & `signac-2.1.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/tests/test_numpy_integration.py` & `signac-2.1.0/tests/test_numpy_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (c) 2018 The Regents of the University of Michigan
 # All rights reserved.
 # This software is licensed under the BSD 3-Clause License.
 import pytest
+from synced_collections.numpy_utils import NumpyConversionWarning
 from test_project import TestProjectBase
 
-from signac._synced_collections.numpy_utils import NumpyConversionWarning
-
 try:
     import numpy  # noqa
     import numpy.testing
 
     NUMPY = True
 except ImportError:
     NUMPY = False
```

### Comparing `signac-2.0.0/tests/test_pandas_integration.py` & `signac-2.1.0/tests/test_pandas_integration.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/tests/test_project.py` & `signac-2.1.0/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/tests/test_searchindexer.py` & `signac-2.1.0/tests/test_searchindexer.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/tests/test_shell.py` & `signac-2.1.0/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/tests/test_sync.py` & `signac-2.1.0/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `signac-2.0.0/tests/test_temporary_project.py` & `signac-2.1.0/tests/test_temporary_project.py`

 * *Files identical despite different names*


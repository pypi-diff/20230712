# Comparing `tmp/pulp-ostree-2.1.0.tar.gz` & `tmp/pulp-ostree-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-ostree-2.1.0.tar", last modified: Sun May 28 21:25:08 2023, max compression
+gzip compressed data, was "pulp-ostree-2.1.1.tar", last modified: Wed Jul 12 13:18:26 2023, max compression
```

## Comparing `pulp-ostree-2.1.0.tar` & `pulp-ostree-2.1.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.679677 pulp-ostree-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-28 21:25:05.000000 pulp-ostree-2.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/COMMITMENT
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/functest_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/
--rwxr-xr-x   0 runner    (1001) docker     (123)       65 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/app/
--rwxr-xr-x   0 runner    (1001) docker     (123)      262 2023-05-28 21:25:07.000000 pulp-ostree-2.1.0/pulp_ostree/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/0002_add_relative_path_uniqueness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/0003_create_many_to_many_objs_commits.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/0004_add_include_exclude_refs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/0005_add_static_delta_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/0006_alter_pointers_to_related_models_globally.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/migrations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4963 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7109 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/app/tasks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      174 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/tasks/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/tasks/modifying.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/tasks/stages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11608 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/tasks/synchronizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/tasks/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9455 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/app/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/functional/
--rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/
--rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_modify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6565 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1118 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3196 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/functional/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/performance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/performance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/unit/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/unit/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/upgrade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/upgrade/post/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/upgrade/post/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree/tests/upgrade/pre/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pulp_ostree/tests/upgrade/pre/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:25:08.675676 pulp-ostree-2.1.0/pulp_ostree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-28 21:25:08.000000 pulp-ostree-2.1.0/pulp_ostree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-28 21:25:08.000000 pulp-ostree-2.1.0/pulp_ostree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:25:08.000000 pulp-ostree-2.1.0/pulp_ostree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-28 21:25:08.000000 pulp-ostree-2.1.0/pulp_ostree.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 21:25:08.000000 pulp-ostree-2.1.0/pulp_ostree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-28 21:25:08.000000 pulp-ostree-2.1.0/pulp_ostree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:25:08.679677 pulp-ostree-2.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-05-28 21:25:07.000000 pulp-ostree-2.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-28 21:24:53.000000 pulp-ostree-2.1.0/unittest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.586586 pulp-ostree-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-12 13:18:25.000000 pulp-ostree-2.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-12 13:18:26.586586 pulp-ostree-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.578586 pulp-ostree-2.1.1/pulp_ostree/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       65 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.582586 pulp-ostree-2.1.1/pulp_ostree/app/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      262 2023-07-12 13:18:25.000000 pulp-ostree-2.1.1/pulp_ostree/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.582586 pulp-ostree-2.1.1/pulp_ostree/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/migrations/0002_add_relative_path_uniqueness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/migrations/0003_create_many_to_many_objs_commits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/migrations/0004_add_include_exclude_refs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/migrations/0005_add_static_delta_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/migrations/0006_alter_pointers_to_related_models_globally.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/migrations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4963 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7109 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.582586 pulp-ostree-2.1.1/pulp_ostree/app/tasks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      174 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/tasks/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/tasks/modifying.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/tasks/stages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11608 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/tasks/synchronizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/tasks/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9455 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/app/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.582586 pulp-ostree-2.1.1/pulp_ostree/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.582586 pulp-ostree-2.1.1/pulp_ostree/tests/functional/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       31 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.586586 pulp-ostree-2.1.1/pulp_ostree/tests/functional/api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/functional/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/functional/api/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/functional/api/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/functional/api/test_modify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6565 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/functional/api/test_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1118 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/functional/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3196 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.586586 pulp-ostree-2.1.1/pulp_ostree/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/performance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.586586 pulp-ostree-2.1.1/pulp_ostree/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/unit/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/unit/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.586586 pulp-ostree-2.1.1/pulp_ostree/tests/upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/upgrade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.586586 pulp-ostree-2.1.1/pulp_ostree/tests/upgrade/post/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/upgrade/post/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.586586 pulp-ostree-2.1.1/pulp_ostree/tests/upgrade/pre/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pulp_ostree/tests/upgrade/pre/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:18:26.578586 pulp-ostree-2.1.1/pulp_ostree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-12 13:18:26.000000 pulp-ostree-2.1.1/pulp_ostree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-12 13:18:26.000000 pulp-ostree-2.1.1/pulp_ostree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:18:26.000000 pulp-ostree-2.1.1/pulp_ostree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-12 13:18:26.000000 pulp-ostree-2.1.1/pulp_ostree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 13:18:26.000000 pulp-ostree-2.1.1/pulp_ostree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 13:18:26.000000 pulp-ostree-2.1.1/pulp_ostree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:18:26.586586 pulp-ostree-2.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-07-12 13:18:25.000000 pulp-ostree-2.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 13:18:15.000000 pulp-ostree-2.1.1/unittest_requirements.txt
```

### Comparing `pulp-ostree-2.1.0/CHANGES.rst` & `pulp-ostree-2.1.1/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,27 @@
     file is managed by towncrier. You *may* edit previous change logs to
     fix problems like typo corrections or such.
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+2.1.1 (2023-07-12)
+==================
+
+Bugfixes
+--------
+
+- Started re-generating summary files and publishing them during the import.
+  `#269 <https://github.com/pulp/pulp_ostree/issues/269>`_
+
+
+----
+
+
 2.1.0 (2023-05-28)
 ==================
 
 Features
 --------
 
 - Made the plugin compatible with Django 4.2 and pulpcore 3.25.
```

### Comparing `pulp-ostree-2.1.0/COMMITMENT` & `pulp-ostree-2.1.1/COMMITMENT`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/COPYRIGHT` & `pulp-ostree-2.1.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/LICENSE` & `pulp-ostree-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/PKG-INFO` & `pulp-ostree-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-ostree
-Version: 2.1.0
+Version: 2.1.1
 Summary: OSTree plugin for the Pulp Project
 Home-page: http://www.pulpproject.org
 Author: Pulp Project Developers
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Description: ![Nightly CI/CD](https://github.com/pulp/pulp_ostree/actions/workflows/nightly.yml/badge.svg?branch=main)
```

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/migrations/0001_initial.py` & `pulp-ostree-2.1.1/pulp_ostree/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/migrations/0002_add_relative_path_uniqueness.py` & `pulp-ostree-2.1.1/pulp_ostree/app/migrations/0002_add_relative_path_uniqueness.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/migrations/0003_create_many_to_many_objs_commits.py` & `pulp-ostree-2.1.1/pulp_ostree/app/migrations/0003_create_many_to_many_objs_commits.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/migrations/0004_add_include_exclude_refs.py` & `pulp-ostree-2.1.1/pulp_ostree/app/migrations/0004_add_include_exclude_refs.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/migrations/0005_add_static_delta_support.py` & `pulp-ostree-2.1.1/pulp_ostree/app/migrations/0005_add_static_delta_support.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/migrations/0006_alter_pointers_to_related_models_globally.py` & `pulp-ostree-2.1.1/pulp_ostree/app/migrations/0006_alter_pointers_to_related_models_globally.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/models.py` & `pulp-ostree-2.1.1/pulp_ostree/app/models.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/serializers.py` & `pulp-ostree-2.1.1/pulp_ostree/app/serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/tasks/importing.py` & `pulp-ostree-2.1.1/pulp_ostree/app/tasks/importing.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Stage,
 )
 
 from pulp_ostree.app.models import (
     OstreeCommit,
     OstreeConfig,
     OstreeObjectType,
+    OstreeSummary,
 )
 from pulp_ostree.app.tasks.utils import copy_to_local_storage, get_checksum_filepath
 from pulp_ostree.app.tasks.stages import OstreeAssociateContent, DeclarativeContentCreatorMixin
 
 import gi
 
 gi.require_version("OSTree", "1.0")
@@ -263,14 +264,17 @@
                             ref_commit_checksum, ref_parent_commit_checksum
                         )
 
                 await pb.aincrement()
 
             await self.submit_ref_objects()
 
+            self.repo.regenerate_summary()
+            await self.submit_metafile_object("summary", OstreeSummary())
+
 
 class OstreeImportAllRefsFirstStage(
     DeclarativeContentCreatorMixin, OstreeSingleRefParserMixin, OstreeImportStage
 ):
     """A first stage of the OSTree importing pipeline that handles creation of content units."""
 
     def __init__(self, tarball_artifact, repo_name, compute_delta):
@@ -318,14 +322,17 @@
                                 ref_commit_checksum, ref_parent_commit_checksum
                             )
 
                 await pb.aincrement()
 
             await self.submit_ref_objects()
 
+            self.repo.regenerate_summary()
+            await self.submit_metafile_object("summary", OstreeSummary())
+
 
 class OstreeImportDeclarativeVersion(DeclarativeVersion):
     """A customized DeclarativeVersion class that creates a pipeline for the OSTree import."""
 
     def pipeline_stages(self, new_version):
         """Build a list of stages."""
         pipeline = [
```

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/tasks/modifying.py` & `pulp-ostree-2.1.1/pulp_ostree/app/tasks/modifying.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/tasks/stages.py` & `pulp-ostree-2.1.1/pulp_ostree/app/tasks/stages.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
-import uuid
+import shutil
+import tempfile
 
 from asgiref.sync import sync_to_async
 
 from pulpcore.plugin.models import Artifact
 from pulpcore.plugin.stages import (
     DeclarativeArtifact,
     DeclarativeContent,
@@ -86,21 +87,21 @@
 
         return DeclarativeContent(content=content, d_artifacts=[da])
 
     def init_artifact(self, relative_file_path):
         """Initialize a new artifact from the passed filepath."""
         filepath = os.path.join(self.repo_path, relative_file_path)
 
-        # this is a hack that prevents the pipeline to remove a temporary file which can be
-        # referenced by multiple content units at the same time; in particular, this means that
-        # one OSTree object (e.g., dirmeta, filez) is referenced by two different commits
-        filepath_copy = filepath + str(uuid.uuid4())
-        os.link(filepath, filepath_copy)
+        # we still need to keep the file in the local repository for further processing
+        with tempfile.NamedTemporaryFile("wb", dir=".", delete=False) as new_file:
+            with open(filepath, mode="rb") as f:
+                shutil.copyfileobj(f, new_file)
+                new_file.flush()
 
-        return Artifact.init_and_validate(filepath_copy)
+        return Artifact.init_and_validate(new_file.name)
 
     async def compute_static_delta(self, ref_commit_checksum, parent_checksum=None):
         if not self.commit_dcs:
             return
 
         if parent_checksum:
             from_ = parent_checksum
```

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/tasks/synchronizing.py` & `pulp-ostree-2.1.1/pulp_ostree/app/tasks/synchronizing.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/tasks/utils.py` & `pulp-ostree-2.1.1/pulp_ostree/app/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/app/viewsets.py` & `pulp-ostree-2.1.1/pulp_ostree/app/viewsets.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_filter.py` & `pulp-ostree-2.1.1/pulp_ostree/tests/functional/api/test_filter.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_import.py` & `pulp-ostree-2.1.1/pulp_ostree/tests/functional/api/test_import.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_modify.py` & `pulp-ostree-2.1.1/pulp_ostree/tests/functional/api/test_modify.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/tests/functional/api/test_sync.py` & `pulp-ostree-2.1.1/pulp_ostree/tests/functional/api/test_sync.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/tests/functional/constants.py` & `pulp-ostree-2.1.1/pulp_ostree/tests/functional/constants.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree/tests/functional/utils.py` & `pulp-ostree-2.1.1/pulp_ostree/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pulp_ostree.egg-info/PKG-INFO` & `pulp-ostree-2.1.1/pulp_ostree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-ostree
-Version: 2.1.0
+Version: 2.1.1
 Summary: OSTree plugin for the Pulp Project
 Home-page: http://www.pulpproject.org
 Author: Pulp Project Developers
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Description: ![Nightly CI/CD](https://github.com/pulp/pulp_ostree/actions/workflows/nightly.yml/badge.svg?branch=main)
```

### Comparing `pulp-ostree-2.1.0/pulp_ostree.egg-info/SOURCES.txt` & `pulp-ostree-2.1.1/pulp_ostree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/pyproject.toml` & `pulp-ostree-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-ostree-2.1.0/setup.py` & `pulp-ostree-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = requirements.readlines()
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="pulp-ostree",
-    version="2.1.0",
+    version="2.1.1",
     description="OSTree plugin for the Pulp Project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPLv2+",
     author="Pulp Project Developers",
     author_email="pulp-list@redhat.com",
     url="http://www.pulpproject.org",
```


# Comparing `tmp/ocdsextensionregistry-0.3.5.tar.gz` & `tmp/ocdsextensionregistry-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocdsextensionregistry-0.3.5.tar", last modified: Wed Jul 12 04:33:58 2023, max compression
+gzip compressed data, was "ocdsextensionregistry-0.3.6.tar", last modified: Wed Jul 12 05:01:00 2023, max compression
```

## Comparing `ocdsextensionregistry-0.3.5.tar` & `ocdsextensionregistry-0.3.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.006075 ocdsextensionregistry-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-12 04:33:58.006075 ocdsextensionregistry-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:57.998076 ocdsextensionregistry-0.3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:57.998076 ocdsextensionregistry-0.3.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/codelist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/codelist_code.rst
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/extension_registry.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/extension_version.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/profile_builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18630 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/translation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.002076 ocdsextensionregistry-0.3.5/ocdsextensionregistry/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/codelist_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.002076 ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16489 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.002076 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-12 04:33:57.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-12 04:33:57.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 04:33:57.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 04:33:57.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-12 04:33:57.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 04:33:57.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-12 04:33:58.010075 ocdsextensionregistry-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.006075 ocdsextensionregistry-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.006075 ocdsextensionregistry-0.3.5/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/commands/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/commands/test_generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/commands/test_generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/commands/test_none.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.006075 ocdsextensionregistry-0.3.5/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/fixtures/location-v1.1.4.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.006075 ocdsextensionregistry-0.3.5/tests/fixtures/ocds_coveredBy_extension/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/fixtures/ocds_coveredBy_extension/release-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_codelist_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:01:00.388605 ocdsextensionregistry-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-12 05:01:00.388605 ocdsextensionregistry-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:01:00.380604 ocdsextensionregistry-0.3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:01:00.380604 ocdsextensionregistry-0.3.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/api/codelist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/api/codelist_code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/api/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/api/extension_registry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/api/extension_version.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/api/profile_builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18973 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/docs/translation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:01:00.384605 ocdsextensionregistry-0.3.6/ocdsextensionregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/codelist_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:01:00.384605 ocdsextensionregistry-0.3.6/ocdsextensionregistry/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/commands/generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/commands/generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15777 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16489 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:01:00.384605 ocdsextensionregistry-0.3.6/ocdsextensionregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-12 05:01:00.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-12 05:01:00.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 05:01:00.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 05:01:00.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-12 05:01:00.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 05:01:00.000000 ocdsextensionregistry-0.3.6/ocdsextensionregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-12 05:01:00.388605 ocdsextensionregistry-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:01:00.384605 ocdsextensionregistry-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:01:00.388605 ocdsextensionregistry-0.3.6/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/commands/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/commands/test_generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/commands/test_generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/commands/test_none.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:01:00.388605 ocdsextensionregistry-0.3.6/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/fixtures/location-v1.1.4.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:01:00.388605 ocdsextensionregistry-0.3.6/tests/fixtures/ocds_coveredBy_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/fixtures/ocds_coveredBy_extension/release-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/test_codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/test_codelist_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/test_extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/test_extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/test_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-12 05:00:48.000000 ocdsextensionregistry-0.3.6/tox.ini
```

### Comparing `ocdsextensionregistry-0.3.5/LICENSE` & `ocdsextensionregistry-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/PKG-INFO` & `ocdsextensionregistry-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.3.5
+Version: 0.3.6
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.3.5/README.rst` & `ocdsextensionregistry-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/docs/Makefile` & `ocdsextensionregistry-0.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/docs/changelog.rst` & `ocdsextensionregistry-0.3.6/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+0.3.6 (2023-07-12)
+------------------
+
+-  fix: Make :meth:`ocdsextensionregistry.extension_version.ExtensionVersion.files`, `~ocdsextensionregistry.extension_version.ExtensionVersion.files`, `~ocdsextensionregistry.extension_version.ExtensionVersion.schemas`, `~ocdsextensionregistry.extension_version.ExtensionVersion.codelists` thread-safe.
+
 0.3.5 (2023-07-12)
 ------------------
 
 -  fix: Make :meth:`ocdsextensionregistry.profile_builder.ProfileBuilder.get_standard_file_contents` thread-safe.
 
 0.3.4 (2023-07-08)
 ------------------
@@ -217,15 +222,15 @@
 -  Add a ``standard_base_url`` argument to :meth:`ocdsextensionregistry.api.build_profile` to modify the standard base URL.
 
 0.0.20 (2020-06-08)
 -------------------
 
 -  Add Windows support for:
 
-   -  :meth:`~ocdsextensionregistry.extension_version.ExtensionVersion.files`
+   -  :meth:`ocdsextensionregistry.extension_version.ExtensionVersion.files`
    -  :meth:`ocdsextensionregistry.profile_builder.ProfileBuilder.get_standard_file_contents`
    -  :meth:`ocdsextensionregistry.profile_builder.ProfileBuilder.standard_codelists`
 
 0.0.19 (2020-04-07)
 -------------------
 
 -  The ``generate-data-file`` command warns if an MO file is missing.
```

### Comparing `ocdsextensionregistry-0.3.5/docs/cli.rst` & `ocdsextensionregistry-0.3.6/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/docs/conf.py` & `ocdsextensionregistry-0.3.6/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OCDS Extension Registry Python Package"
 copyright = "2018, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.3.5"
+version = "0.3.6"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `ocdsextensionregistry-0.3.5/docs/index.rst` & `ocdsextensionregistry-0.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/docs/translation.rst` & `ocdsextensionregistry-0.3.6/docs/translation.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/__init__.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/__main__.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/__main__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/api.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/codelist.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/codelist_code.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/base.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/commands/base.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/download.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/commands/download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/generate_data_file.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/commands/generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/generate_pot_files.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/commands/generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/exceptions.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/extension.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/extension_registry.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/extension_version.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/extension_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,28 +122,30 @@
 
         If the extension has a download URL, caches all the files' contents. Otherwise, returns an empty dict. Raises
         an HTTPError if the download fails.
 
         :raises zipfile.BadZipFile: if the download URL is not a ZIP file
         """
         if self._files is None:
-            self._files = {}
+            files = {}
 
             if self.download_url:
                 with closing(self.zipfile()) as zipfile:
                     names = zipfile.namelist()
                     start = len(names[0])
 
                     for name in names[1:]:
                         filename = name[start:]
                         if filename[-1] != '/' and not filename.startswith('.'):
                             content = zipfile.read(name)
                             if os.path.splitext(name)[1] in ('.csv', '.json', '.md'):
                                 content = content.decode('utf-8')
-                            self._files[filename] = content
+                            files[filename] = content
+
+            self._files = files
 
         return self._files
 
     def zipfile(self):
         """
         If the extension has a download URL, downloads and returns the ZIP archive.
 
@@ -180,63 +182,67 @@
 
     @property
     def schemas(self):
         """
         Retrieves and returns the parsed contents of the extension's schemas files.
         """
         if self._schemas is None:
-            self._schemas = {}
+            schemas = {}
 
             if 'schemas' in self.metadata:
                 names = self.metadata['schemas']
             elif self.download_url:
                 names = [name for name in self.files if name in SCHEMAS]
             else:
                 names = SCHEMAS
 
             for name in names:
                 try:
-                    self._schemas[name] = json.loads(self.remote(name))
+                    schemas[name] = json.loads(self.remote(name))
                 except requests.exceptions.HTTPError:
                     if 'schemas' in self.metadata:  # avoid raising if using SCHEMAS
                         raise
 
+            self._schemas = schemas
+
         return self._schemas
 
     @property
     def codelists(self):
         """
         Retrieves and returns the parsed contents of the extension's codelists files.
 
         If the extension has no download URL, and if no codelists are listed in extension.json, returns an empty dict.
         """
         if self._codelists is None:
-            self._codelists = {}
+            codelists = {}
 
             if 'codelists' in self.metadata:
                 names = self.metadata['codelists']
             elif self.download_url:
                 names = [name[10:] for name in self.files if name.startswith('codelists/')]
             else:
                 names = []
 
             for name in names:
                 try:
-                    self._codelists[name] = Codelist(name)
+                    codelists[name] = Codelist(name)
                     # Use universal newlines mode, to avoid parsing errors.
                     io = StringIO(self.remote('codelists/' + name), newline='')
-                    self._codelists[name].extend(csv.DictReader(io))
+                    codelists[name].extend(csv.DictReader(io))
                 except (
                     UnicodeDecodeError,
                     requests.RequestException,
                     zipfile.BadZipFile,
                 ) as e:
                     warnings.warn(ExtensionCodelistWarning(self, name, e))
                     continue
 
+            self._codelists = codelists
+
         return self._codelists
 
     @property
     def repository_full_name(self):
         """
         Returns the full name of the extension's repository, which should be a unique identifier on the hosting
         service, e.g. open-contracting-extensions/ocds_bid_extension
```

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/profile_builder.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/profile_builder.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry/util.py` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry/util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/PKG-INFO` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.3.5
+Version: 0.3.6
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/SOURCES.txt` & `ocdsextensionregistry-0.3.6/ocdsextensionregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/setup.cfg` & `ocdsextensionregistry-0.3.6/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ocdsextensionregistry
-version = 0.3.5
+version = 0.3.6
 author = Open Contracting Partnership
 author_email = data@open-contracting.org
 license = BSD
 description = Eases access to information from the extension registry of the Open Contracting Data Standard
 url = https://github.com/open-contracting/extension_registry.py
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `ocdsextensionregistry-0.3.5/tests/commands/test_download.py` & `ocdsextensionregistry-0.3.6/tests/commands/test_download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/tests/commands/test_generate_data_file.py` & `ocdsextensionregistry-0.3.6/tests/commands/test_generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/tests/commands/test_generate_pot_files.py` & `ocdsextensionregistry-0.3.6/tests/commands/test_generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/tests/fixtures/location-v1.1.4.json` & `ocdsextensionregistry-0.3.6/tests/fixtures/location-v1.1.4.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/tests/fixtures/ocds_coveredBy_extension/release-schema.json` & `ocdsextensionregistry-0.3.6/tests/fixtures/ocds_coveredBy_extension/release-schema.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/tests/test_api.py` & `ocdsextensionregistry-0.3.6/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/tests/test_codelist.py` & `ocdsextensionregistry-0.3.6/tests/test_codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/tests/test_codelist_code.py` & `ocdsextensionregistry-0.3.6/tests/test_codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/tests/test_extension.py` & `ocdsextensionregistry-0.3.6/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/tests/test_extension_registry.py` & `ocdsextensionregistry-0.3.6/tests/test_extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/tests/test_extension_version.py` & `ocdsextensionregistry-0.3.6/tests/test_extension_version.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/tests/test_profile_builder.py` & `ocdsextensionregistry-0.3.6/tests/test_profile_builder.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/tests/test_util.py` & `ocdsextensionregistry-0.3.6/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.5/tox.ini` & `ocdsextensionregistry-0.3.6/tox.ini`

 * *Files identical despite different names*


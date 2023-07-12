# Comparing `tmp/ocdsextensionregistry-0.3.4.tar.gz` & `tmp/ocdsextensionregistry-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocdsextensionregistry-0.3.4.tar", last modified: Sat Jul  8 04:27:30 2023, max compression
+gzip compressed data, was "ocdsextensionregistry-0.3.5.tar", last modified: Wed Jul 12 04:33:58 2023, max compression
```

## Comparing `ocdsextensionregistry-0.3.4.tar` & `ocdsextensionregistry-0.3.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:30.320250 ocdsextensionregistry-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-08 04:27:30.320250 ocdsextensionregistry-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:30.312250 ocdsextensionregistry-0.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:30.316250 ocdsextensionregistry-0.3.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/api/codelist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/api/codelist_code.rst
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/api/extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/api/extension_registry.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/api/extension_version.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/api/profile_builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18476 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/docs/translation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:30.316250 ocdsextensionregistry-0.3.4/ocdsextensionregistry/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/codelist_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:30.316250 ocdsextensionregistry-0.3.4/ocdsextensionregistry/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/commands/generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/commands/generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:30.316250 ocdsextensionregistry-0.3.4/ocdsextensionregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-08 04:27:30.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-08 04:27:30.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 04:27:30.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-08 04:27:30.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-08 04:27:30.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 04:27:30.000000 ocdsextensionregistry-0.3.4/ocdsextensionregistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-08 04:27:30.320250 ocdsextensionregistry-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:30.320250 ocdsextensionregistry-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:30.320250 ocdsextensionregistry-0.3.4/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/commands/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/commands/test_generate_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/commands/test_generate_pot_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/commands/test_none.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:30.320250 ocdsextensionregistry-0.3.4/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/fixtures/location-v1.1.4.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 04:27:30.320250 ocdsextensionregistry-0.3.4/tests/fixtures/ocds_coveredBy_extension/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/fixtures/ocds_coveredBy_extension/release-schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/test_codelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/test_codelist_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/test_extension_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/test_extension_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/test_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-08 04:27:21.000000 ocdsextensionregistry-0.3.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.006075 ocdsextensionregistry-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-12 04:33:58.006075 ocdsextensionregistry-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:57.998076 ocdsextensionregistry-0.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:57.998076 ocdsextensionregistry-0.3.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/codelist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/codelist_code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/extension_registry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/extension_version.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/profile_builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18630 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/docs/translation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.002076 ocdsextensionregistry-0.3.5/ocdsextensionregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/codelist_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.002076 ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16489 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.002076 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-12 04:33:57.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-12 04:33:57.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 04:33:57.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 04:33:57.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-12 04:33:57.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 04:33:57.000000 ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-12 04:33:58.010075 ocdsextensionregistry-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.006075 ocdsextensionregistry-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.006075 ocdsextensionregistry-0.3.5/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/commands/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/commands/test_generate_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/commands/test_generate_pot_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/commands/test_none.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.006075 ocdsextensionregistry-0.3.5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/fixtures/location-v1.1.4.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 04:33:58.006075 ocdsextensionregistry-0.3.5/tests/fixtures/ocds_coveredBy_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/fixtures/ocds_coveredBy_extension/release-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_codelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_codelist_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_extension_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_extension_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15543 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-12 04:33:44.000000 ocdsextensionregistry-0.3.5/tox.ini
```

### Comparing `ocdsextensionregistry-0.3.4/LICENSE` & `ocdsextensionregistry-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/PKG-INFO` & `ocdsextensionregistry-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.3.4
+Version: 0.3.5
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.3.4/README.rst` & `ocdsextensionregistry-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/docs/Makefile` & `ocdsextensionregistry-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/docs/changelog.rst` & `ocdsextensionregistry-0.3.5/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+0.3.5 (2023-07-12)
+------------------
+
+-  fix: Make :meth:`ocdsextensionregistry.profile_builder.ProfileBuilder.get_standard_file_contents` thread-safe.
+
 0.3.4 (2023-07-08)
 ------------------
 
 -  feat: :class:`ocdsextensionregistry.profile_builder.ProfileBuilder` accepts ``standard_base_url`` as a ZIP file, in addition to a directory.
 
 0.3.3 (2023-07-07)
 ------------------
```

### Comparing `ocdsextensionregistry-0.3.4/docs/cli.rst` & `ocdsextensionregistry-0.3.5/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/docs/conf.py` & `ocdsextensionregistry-0.3.5/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OCDS Extension Registry Python Package"
 copyright = "2018, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.3.4"
+version = "0.3.5"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `ocdsextensionregistry-0.3.4/docs/index.rst` & `ocdsextensionregistry-0.3.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/docs/translation.rst` & `ocdsextensionregistry-0.3.5/docs/translation.rst`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/__init__.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/__main__.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/__main__.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/api.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/codelist.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/codelist.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         return [row['Code'] for row in self.rows]
 
     @property
     def fieldnames(self):
         """
         Returns all fieldnames used in any rows.
         """
-        fieldnames = {}
+        fieldnames = {}  # sets are unordered
         for row in self.rows:
             for field in row:
                 fieldnames[field] = True
         return list(fieldnames.keys())
 
     @property
     def basename(self):
```

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/codelist_code.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/commands/base.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/base.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/commands/download.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/commands/generate_data_file.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/commands/generate_pot_files.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/commands/generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/exceptions.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/extension.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/extension_registry.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/extension_version.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/extension_version.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/profile_builder.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/profile_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,17 +335,21 @@
             path = names[0]
             if self.standard_tag < '1__1__5':
                 path += 'standard/schema/'
             else:
                 path += 'schema/'
             start = len(path)
 
+            cache = {}
             for name in names[1:]:
                 if path in name:
-                    self._file_cache[name[start:]] = zipfile.read(name).decode('utf-8')
+                    cache[name[start:]] = zipfile.read(name).decode('utf-8')
+
+            # Set _file_cache at once, e.g. if threaded.
+            self._file_cache = cache
 
         return self._file_cache[basename]
 
 
 def _add_extension_field(schema, extension_name, field_name, pointer=None):
     if pointer is None:
         pointer = ()
```

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry/util.py` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry/util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry.egg-info/PKG-INFO` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocdsextensionregistry
-Version: 0.3.4
+Version: 0.3.5
 Summary: Eases access to information from the extension registry of the Open Contracting Data Standard
 Home-page: https://github.com/open-contracting/extension_registry.py
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `ocdsextensionregistry-0.3.4/ocdsextensionregistry.egg-info/SOURCES.txt` & `ocdsextensionregistry-0.3.5/ocdsextensionregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/setup.cfg` & `ocdsextensionregistry-0.3.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ocdsextensionregistry
-version = 0.3.4
+version = 0.3.5
 author = Open Contracting Partnership
 author_email = data@open-contracting.org
 license = BSD
 description = Eases access to information from the extension registry of the Open Contracting Data Standard
 url = https://github.com/open-contracting/extension_registry.py
 long_description = file: README.rst
 long_description_content_type = text/x-rst
@@ -20,15 +20,15 @@
 
 [options]
 packages = find:
 install_requires = 
 	json-merge-patch
 	jsonref>=1
 	requests
-	requests-cache
+	requests-cache>=1
 	cattrs!=22.1.0;platform_python_implementation=="PyPy"
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
```

### Comparing `ocdsextensionregistry-0.3.4/tests/commands/test_download.py` & `ocdsextensionregistry-0.3.5/tests/commands/test_download.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/tests/commands/test_generate_data_file.py` & `ocdsextensionregistry-0.3.5/tests/commands/test_generate_data_file.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/tests/commands/test_generate_pot_files.py` & `ocdsextensionregistry-0.3.5/tests/commands/test_generate_pot_files.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/tests/fixtures/location-v1.1.4.json` & `ocdsextensionregistry-0.3.5/tests/fixtures/location-v1.1.4.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/tests/fixtures/ocds_coveredBy_extension/release-schema.json` & `ocdsextensionregistry-0.3.5/tests/fixtures/ocds_coveredBy_extension/release-schema.json`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/tests/test_api.py` & `ocdsextensionregistry-0.3.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/tests/test_codelist.py` & `ocdsextensionregistry-0.3.5/tests/test_codelist.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/tests/test_codelist_code.py` & `ocdsextensionregistry-0.3.5/tests/test_codelist_code.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/tests/test_extension.py` & `ocdsextensionregistry-0.3.5/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/tests/test_extension_registry.py` & `ocdsextensionregistry-0.3.5/tests/test_extension_registry.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/tests/test_extension_version.py` & `ocdsextensionregistry-0.3.5/tests/test_extension_version.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/tests/test_profile_builder.py` & `ocdsextensionregistry-0.3.5/tests/test_profile_builder.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/tests/test_util.py` & `ocdsextensionregistry-0.3.5/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `ocdsextensionregistry-0.3.4/tox.ini` & `ocdsextensionregistry-0.3.5/tox.ini`

 * *Files identical despite different names*


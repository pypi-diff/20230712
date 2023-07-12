# Comparing `tmp/grokcore.catalog-3.0.1.tar.gz` & `tmp/grokcore.catalog-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grokcore.catalog-3.0.1.tar", last modified: Fri Jan 12 12:48:43 2018, max compression
+gzip compressed data, was "grokcore.catalog-4.0.tar", last modified: Wed Jul 12 07:30:30 2023, max compression
```

## Comparing `grokcore.catalog-3.0.1.tar` & `grokcore.catalog-4.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/
--rw-r--r--   0 jw         (501) staff       (20)      357 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/.travis.yml
--rw-r--r--   0 jw         (501) staff       (20)     6158 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/bootstrap.py
--rw-r--r--   0 jw         (501) staff       (20)      492 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/buildout.cfg
--rw-r--r--   0 jw         (501) staff       (20)     1288 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/CHANGES.txt
--rw-r--r--   0 jw         (501) staff       (20)       32 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/COPYRIGHT.txt
--rw-r--r--   0 jw         (501) staff       (20)     2105 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/CREDITS.txt
--rw-r--r--   0 jw         (501) staff       (20)     2070 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/LICENSE.txt
--rw-r--r--   0 jw         (501) staff       (20)      124 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/MANIFEST.in
--rw-r--r--   0 jw         (501) staff       (20)     4535 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/PKG-INFO
--rw-r--r--   0 jw         (501) staff       (20)     1409 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/README.txt
--rw-r--r--   0 jw         (501) staff       (20)       38 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/setup.cfg
--rw-r--r--   0 jw         (501) staff       (20)     2199 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/setup.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore/
--rw-r--r--   0 jw         (501) staff       (20)      200 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/__init__.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/
--rw-r--r--   0 jw         (501) staff       (20)      371 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)     3126 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/components.py
--rw-r--r--   0 jw         (501) staff       (20)      493 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/configure.zcml
--rw-r--r--   0 jw         (501) staff       (20)      376 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftesting.zcml
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/
--rw-r--r--   0 jw         (501) staff       (20)       20 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/__init__.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/
--rw-r--r--   0 jw         (501) staff       (20)       32 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)     1670 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/catalog.py
--rw-r--r--   0 jw         (501) staff       (20)     2802 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes.py
--rw-r--r--   0 jw         (501) staff       (20)     2317 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_app_interface.py
--rw-r--r--   0 jw         (501) staff       (20)     1887 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_attribute.py
--rw-r--r--   0 jw         (501) staff       (20)     2318 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_class.py
--rw-r--r--   0 jw         (501) staff       (20)     3131 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_datetimeindex.py
--rw-r--r--   0 jw         (501) staff       (20)     1994 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_install_on.py
--rw-r--r--   0 jw         (501) staff       (20)     2154 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_multiple.py
--rw-r--r--   0 jw         (501) staff       (20)     1739 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_multiple_conflict.py
--rw-r--r--   0 jw         (501) staff       (20)     1713 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_name.py
--rw-r--r--   0 jw         (501) staff       (20)     1894 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_nonexistent.py
--rw-r--r--   0 jw         (501) staff       (20)     2154 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_set.py
--rw-r--r--   0 jw         (501) staff       (20)     1563 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_site.py
--rw-r--r--   0 jw         (501) staff       (20)     2172 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_valueindex.py
--rw-r--r--   0 jw         (501) staff       (20)     1770 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/setuporder.py
--rw-r--r--   0 jw         (501) staff       (20)     1302 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/test_grok_functional.py
--rw-r--r--   0 jw         (501) staff       (20)     9409 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/index.py
--rw-r--r--   0 jw         (501) staff       (20)     1906 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/interfaces.py
--rw-r--r--   0 jw         (501) staff       (20)     5249 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/meta.py
--rw-r--r--   0 jw         (501) staff       (20)      241 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/meta.zcml
--rw-r--r--   0 jw         (501) staff       (20)     1038 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/testing.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/tests/
--rw-r--r--   0 jw         (501) staff       (20)       32 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/tests/__init__.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/tests/catalog/
--rw-r--r--   0 jw         (501) staff       (20)       20 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/tests/catalog/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)     1012 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/tests/catalog/indexes_module.py
--rw-r--r--   0 jw         (501) staff       (20)     1133 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/tests/catalog/indexes_no_app.py
--rw-r--r--   0 jw         (501) staff       (20)     1330 2018-01-12 12:48:42.000000 grokcore.catalog-3.0.1/src/grokcore/catalog/tests/test_grok.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore.catalog.egg-info/
--rw-r--r--   0 jw         (501) staff       (20)        1 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore.catalog.egg-info/dependency_links.txt
--rw-r--r--   0 jw         (501) staff       (20)        9 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore.catalog.egg-info/namespace_packages.txt
--rw-r--r--   0 jw         (501) staff       (20)        1 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore.catalog.egg-info/not-zip-safe
--rw-r--r--   0 jw         (501) staff       (20)     4535 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore.catalog.egg-info/PKG-INFO
--rw-r--r--   0 jw         (501) staff       (20)      366 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore.catalog.egg-info/requires.txt
--rw-r--r--   0 jw         (501) staff       (20)     1954 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore.catalog.egg-info/SOURCES.txt
--rw-r--r--   0 jw         (501) staff       (20)        9 2018-01-12 12:48:43.000000 grokcore.catalog-3.0.1/src/grokcore.catalog.egg-info/top_level.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 07:30:30.536334 grokcore.catalog-4.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1485 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2105 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/CREDITS.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      225 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3881 2023-07-12 07:30:30.536405 grokcore.catalog-4.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1377 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      483 2023-07-12 07:30:30.536645 grokcore.catalog-4.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2170 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 07:30:30.526154 grokcore.catalog-4.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 07:30:30.528752 grokcore.catalog-4.0/src/grokcore/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 07:30:30.531418 grokcore.catalog-4.0/src/grokcore/catalog/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      615 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3120 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/components.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      493 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)      386 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/ftesting.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     9397 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/index.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1930 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5241 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/meta.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      241 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1038 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/testing.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 07:30:30.531864 grokcore.catalog-4.0/src/grokcore/catalog/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 07:30:30.532022 grokcore.catalog-4.0/src/grokcore/catalog/tests/base/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/base/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 07:30:30.532498 grokcore.catalog-4.0/src/grokcore/catalog/tests/base/catalog/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       20 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/base/catalog/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      957 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/base/catalog/indexes_module.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1045 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/base/catalog/indexes_no_app.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 07:30:30.532660 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       20 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 07:30:30.535979 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1703 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/catalog.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2888 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2375 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_app_interface.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1973 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_attribute.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2352 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_class.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3223 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_datetimeindex.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2089 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_install_on.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2186 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_multiple.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1771 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_multiple_conflict.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1747 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_name.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1863 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_nonexistent.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2240 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_set.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1595 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_site.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2258 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_valueindex.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1828 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/setuporder.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1177 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/test_base.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1345 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore/catalog/tests/test_functional.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 07:30:30.530054 grokcore.catalog-4.0/src/grokcore.catalog.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3881 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore.catalog.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2173 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore.catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore.catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore.catalog.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore.catalog.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      357 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore.catalog.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/src/grokcore.catalog.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1474 2023-07-12 07:30:30.000000 grokcore.catalog-4.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grokcore.catalog-3.0.1/CHANGES.txt` & `grokcore.catalog-4.0/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 CHANGES
 *******
 
+4.0 (2023-07-12)
+================
+
+- Add support for Python 3.7, 3.8, 3.9, 3.10, 3.11.
+
+- Drop support for Python 2.7, 3.4, 3.5, 3.6.
+
+- Fix tests to be able to run with ``zope.component >= 5``.
+
+
 3.0.1 (2018-01-12)
 ==================
 
 - Rearrange tests such that Travis CI can pick up all functional tests too.
 
 3.0.0 (2018-01-05)
 ==================
```

### Comparing `grokcore.catalog-3.0.1/CREDITS.txt` & `grokcore.catalog-4.0/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `grokcore.catalog-3.0.1/LICENSE.txt` & `grokcore.catalog-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grokcore.catalog-3.0.1/README.txt` & `grokcore.catalog-4.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -27,22 +27,22 @@
 
 "ME GROK SMASH ZCML!"
 
 Getting grok
 ============
 
 The easiest way to get started with grok is to install the
-`grokproject <http://cheeseshop.python.org/pypi/grokproject>`_ package
-(e.g. via ``easy_install grokproject``) and then create a new project
+`grokproject <https://pypi.org/project/grokproject/>`_ package
+(e.g. via ``pip install grokproject``) and then create a new project
 area by calling the ``grokproject`` script like so::
 
   $ grokproject MyProject
   ... many lines of output here
 
 This will create a project area in ``MyProject`` as well as download
 and install grok.
 
-You can also get grok from the subversion repository::
+You can also get grok from GitHub::
 
-  svn co svn://svn.zope.org/repos/main/grok/trunk grok
+  git clone git@github.com:zopefoundation/grok.git
 
 Then follow the instructions of ``INSTALL.txt``.
```

### Comparing `grokcore.catalog-3.0.1/setup.py` & `grokcore.catalog-4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 # -*- coding: utf-8 -*-
 
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
-    return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
+    with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
+        return f.read()
 
 
 long_description = (
-    read('README.txt') + '\n' + read('CHANGES.txt'))
+    read('README.rst') + '\n' + read('CHANGES.rst'))
 
 
 tests_require = [
     'grokcore.content',
     'zope.app.appsetup',
     'zope.component',
     'zope.configuration',
     'zope.location',
     'zope.testing',
     'zope.app.wsgi',
-    ]
+]
 
 
 setup(
     name='grokcore.catalog',
-    version='3.0.1',
+    version='4.0',
     author='Grok Team',
-    author_email='grok-dev@zope.org',
-    url='http://grok.zope.org',
-    download_url='http://pypi.python.org/pypi/grokcore.catalog',
+    author_email='zope-dev@zope.dev',
+    url='https://github.com/zopefoundation/grokcore.catalog',
     description='Grok-like configuration for catalog and indexes',
     long_description=long_description,
-    license='ZPL',
+    license='ZPL 2.1',
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
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
         'Programming Language :: Python :: Implementation',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
-        'Framework :: Zope3',
-        ],
+        'Framework :: Zope :: 3',
+    ],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['grokcore'],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        'grokcore.component >= 2.5dev',
+        'grokcore.component >= 2.5',
         'grokcore.site >= 1.7',
         'martian >= 0.13',
         'setuptools',
         'zc.catalog',
         'zope.annotation',
         'zope.catalog',
         'zope.component',
@@ -67,11 +69,10 @@
         'zope.event',
         'zope.exceptions',
         'zope.interface',
         'zope.intid',
         'zope.lifecycleevent',
         'zope.keyreference',
         'zope.site',
-        ],
-    tests_require=tests_require,
+    ],
     extras_require={'test': tests_require},
 )
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/components.py` & `grokcore.catalog-4.0/src/grokcore/catalog/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
 import martian.util
+
 from grokcore.catalog.interfaces import IIndexDefinition
 
 
-class IndexesClass(object):
+class IndexesClass:
     """Base class for index collections in a Grok application.
 
     A `grokcore.catalog.Indexes` utility provides one or more Zope Database
     content indexes for use in a :class:`grokcore.site.Site` or
     :class:`grok.Application`.  The site or application that the
     indexes are intended for should be named with the :func:`grok.site()`
     directive, and the kind of object to index should be named with a
@@ -67,8 +68,9 @@
                 continue
             indexes[name] = value
         self.__grok_indexes__ = indexes
         # __grok_module__ is needed to make defined_locally() return True for
         # inline templates
         self.__grok_module__ = martian.util.caller_module()
 
+
 Indexes = IndexesClass('Indexes')
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/catalog.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Let's setup a site in which we manage a couple of objects:
 
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
-  >>> from zope.site.hooks import setSite
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
 
 Now we add some indexable objects to the site:
 
   >>> herd['manfred'] = Mammoth('Manfred')
   >>> herd['ellie'] = Mammoth('Ellie')
 
@@ -30,21 +30,22 @@
   >>> intids = component.getUtility(IIntIds)
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
 
 """
 
 import grokcore.site
+from grokcore.content import Container
+from grokcore.content import Model
 from zope import interface
-from zope.intid import IntIds
-from zope.intid.interfaces import IIntIds
 from zope.catalog.catalog import Catalog
-from zope.catalog.interfaces import ICatalog
 from zope.catalog.field import FieldIndex
-from grokcore.content import Model, Container
+from zope.catalog.interfaces import ICatalog
+from zope.intid import IntIds
+from zope.intid.interfaces import IIntIds
 
 
 def setup_catalog(catalog):
     catalog['name'] = FieldIndex('name', IMammoth)
 
 
 class IMammoth(interface.Interface):
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Grok allows you to set up catalog indexes in your application with a
 special indexes declaration.
 
 Let's set up a site in which we manage a couple of objects::
 
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
-  >>> from zope.site.hooks import setSite
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
 
 Now we add some indexable objects to the site::
 
   >>> herd['alpha'] = Mammoth('Alpha', 13, 'Hello world!')
   >>> herd['beta'] = Mammoth('Beta', 14, 'Bye World!')
 
@@ -58,18 +58,22 @@
   >>> intids = component.getUtility(IIntIds)
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
 
 Unfortunately ftests don't have good isolation from each other yet.
 """
 
-import grokcore.catalog
 import grokcore.site
-from grokcore.content import Container, Model
-from zope.interface import Interface, Attribute, implementer
+from grokcore.content import Container
+from grokcore.content import Model
+from zope.interface import Attribute
+from zope.interface import Interface
+from zope.interface import implementer
+
+import grokcore.catalog
 
 
 class Herd(Container, grokcore.site.Application):
     pass
 
 
 class Herd2(Container, grokcore.site.Application):
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_app_interface.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_app_interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 special indexes declaration. Here we see how we can register indexes for
 an interface instead of an application directly.
 
 Let's set up a site in which we manage a couple of objects::
 
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
-  >>> from zope.site.hooks import setSite
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
 
 We are able to find the catalog::
 
   >>> from zope.catalog.interfaces import ICatalog
   >>> from zope.component import getUtility
   >>> catalog = getUtility(ICatalog)
@@ -52,17 +52,20 @@
   True
   >>> intids = component.getUtility(IIntIds)
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
 """
 
 import grokcore.site
-import grokcore.catalog
 from grokcore.content import Container
-from zope.interface import Attribute, Interface, implementer
+from zope.interface import Attribute
+from zope.interface import Interface
+from zope.interface import implementer
+
+import grokcore.catalog
 
 
 class IHerd(Interface):
     pass
 
 
 @implementer(IHerd)
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_attribute.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_attribute.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from the attribute, you can do so, by passing an explicit `attribute`
 keyword argument to the field.
 
 Let's set up a site in which we manage a couple of objects::
 
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
-  >>> from zope.site.hooks import setSite
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
 
 Now we add some indexable objects to the site::
 
   >>> herd['alpha'] = Mammoth('Alpha', 13)
   >>> herd['beta'] = Mammoth('Beta', 14)
 
@@ -37,17 +37,21 @@
   >>> from zope import component
   >>> intids = component.getUtility(IIntIds)
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
 """
 
 import grokcore.site
+from grokcore.content import Container
+from grokcore.content import Model
+from zope.interface import Attribute
+from zope.interface import Interface
+from zope.interface import implementer
+
 import grokcore.catalog
-from grokcore.content import Container, Model
-from zope.interface import implementer, Attribute, Interface
 
 
 class Herd(Container, grokcore.site.Application):
     pass
 
 
 class IMammoth(Interface):
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_class.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 special indexes declaration. This can also be done without explicit interface.
 The context of the indexes applies to a class in this case.
 
 Let's set up a site in which we manage a couple of objects::
 
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
-  >>> from zope.site.hooks import setSite
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
 
 Now we add some indexable objects to the site::
 
   >>> herd['alpha'] = Mammoth('Alpha', 13, 'Hello world!')
   >>> herd['beta'] = Mammoth('Beta', 14, 'Bye World!')
 
@@ -50,16 +50,18 @@
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
 
 Unfortunately ftests don't have good isolation from each other yet.
 """
 
 import grokcore.site
+from grokcore.content import Container
+from grokcore.content import Model
+
 import grokcore.catalog
-from grokcore.content import Container, Model
 
 
 class Herd(Container, grokcore.site.Application):
     pass
 
 
 class Mammoth(Model):
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_datetimeindex.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_datetimeindex.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 We now demonstrate the use of a ValueIndex with Grok::
 
 Let's set up a site in which we manage a couple of objects::
 
+  >>> import datetime
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
-  >>> from zope.site.hooks import setSite
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
 
 Now we add some indexable objects to the site::
 
   >>> herd['alpha'] = Opossum('Alpha', datetime.datetime(2001, 6, 7))
   >>> herd['beta'] = Opossum('Beta', datetime.datetime(2001, 7, 8))
   >>> herd['gamma'] = Opossum('Gamma', datetime.datetime(2001, 7, 9))
@@ -63,19 +64,22 @@
   >>> intids = component.getUtility(IIntIds)
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
 
 Unfortunately ftests don't have good isolation from each other yet.
 """
 
-import datetime
 import grokcore.site
+from grokcore.content import Container
+from grokcore.content import Model
+from zope.interface import Attribute
+from zope.interface import Interface
+from zope.interface import implementer
+
 import grokcore.catalog
-from grokcore.content import Container, Model
-from zope.interface import implementer, Interface, Attribute
 
 
 class Herd(Container, grokcore.site.Application):
     pass
 
 
 class IOpossum(Interface):
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_install_on.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_site.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,23 @@
 """
 Grok allows you to set up catalog indexes in your application with a
 special indexes declaration. In fact, these indexes can be set up for
 any site::
 
 Let's set up a site in which we manage a couple of objects::
 
-  >>> from zope.site.hooks import setSite
-
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
 
-The catalog is not yet in the site::
+The catalog is there in the site::
 
   >>> from zope.catalog.interfaces import ICatalog
-  >>> from zope.component import queryUtility
-
-  >>> catalog = queryUtility(ICatalog, default=None)
-  >>> catalog is None
-  True
-
-After a mud party it gets there though:
-
-  >>> from zope.event import notify
-
-  >>> notify(MudPartyEvent(herd))
+  >>> from zope.component import getUtility, queryUtility
   >>> catalog = queryUtility(ICatalog, default=None)
   >>> catalog is not None
   True
 
 Nuke the catalog and intids in the end, so as not to confuse
 other tests::
 
@@ -37,47 +26,37 @@
   >>> sm.unregisterUtility(catalog, provided=ICatalog)
   True
   >>> from zope.intid.interfaces import IIntIds
   >>> from zope import component
   >>> intids = component.getUtility(IIntIds)
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
-
 """
 
 import grokcore.site
-import grokcore.catalog
 from grokcore.content import Container
-from zope.interface import Interface, Attribute, implementer
-from zope.component.interfaces import ObjectEvent, IObjectEvent
-
+from zope.interface import Attribute
+from zope.interface import Interface
 
-class Herd(Container, grokcore.site.Site):
-    pass
-
-
-class IMudPartyEvent(IObjectEvent):
-    pass
+import grokcore.catalog
 
 
-@implementer(IMudPartyEvent)
-class MudPartyEvent(ObjectEvent):
+class Herd(Container, grokcore.site.Site):
     pass
 
 
 class IMammoth(Interface):
     name = Attribute('Name')
     age = Attribute('Age')
 
     def message():
         """Message the mammoth has for the world.
         """
 
 
 class MammothIndexes(grokcore.catalog.Indexes):
-    grokcore.catalog.context(IMammoth)
     grokcore.site.site(Herd)
-    grokcore.site.install_on(IMudPartyEvent)
+    grokcore.catalog.context(IMammoth)
 
     name = grokcore.catalog.Field()
     age = grokcore.catalog.Field()
     message = grokcore.catalog.Text()
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_multiple.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_multiple.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 special indexes declaration. In fact, we have multiple grok.Indexes
 setting up more than one set of indexes in the same catalog.
 
 Let's set up a site in which we manage a couple of objects::
 
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
-  >>> from zope.site.hooks import setSite
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
 
 We are able to query the catalog::
 
   >>> from zope.catalog.interfaces import ICatalog
   >>> from zope.component import getUtility, queryUtility
   >>> catalog = getUtility(ICatalog)
@@ -31,18 +31,20 @@
   >>> intids = component.getUtility(IIntIds)
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
 
 Unfortunately ftests don't have good isolation from each other yet.
 """
 
-import grokcore.catalog
 import grokcore.site
 from grokcore.content import Container
-from zope.interface import Interface, Attribute
+from zope.interface import Attribute
+from zope.interface import Interface
+
+import grokcore.catalog
 
 
 class Herd(Container, grokcore.site.Application):
     pass
 
 
 class IMammoth(Interface):
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_multiple_conflict.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_multiple_conflict.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
   Traceback (most recent call last):
     ...
   KeyError:...
 
-  >>> from zope.site.hooks import setSite
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
   >>> from zope.catalog.interfaces import ICatalog
   >>> from zope.component import getUtility, queryUtility
   >>> catalog = getUtility(ICatalog)
 
 Nuke the catalog and intids in the end, so as not to confuse
 other tests::
@@ -31,17 +31,19 @@
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
 
 Unfortunately ftests don't have good isolation from each other yet.
 """
 
 import grokcore.site
-import grokcore.catalog
 from grokcore.content import Container
-from zope.interface import Interface, Attribute
+from zope.interface import Attribute
+from zope.interface import Interface
+
+import grokcore.catalog
 
 
 class Herd(Container, grokcore.site.Application):
     pass
 
 
 class IMammoth(Interface):
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_name.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 special indexes declaration. We can specify the catalog name using
 grok.name.
 
 Let's set up a site in which we manage a couple of objects::
 
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
-  >>> from zope.site.hooks import setSite
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
 
   >>> from zope.catalog.interfaces import ICatalog
   >>> from zope.component import getUtility
 
 We have to look up the catalog by name now::
 
@@ -31,16 +31,18 @@
   >>> intids = component.getUtility(IIntIds)
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
 
 Unfortunately ftests don't have good isolation from each other yet.
 """
 import grokcore.site
+from grokcore.content import Container
+from grokcore.content import Model
+
 import grokcore.catalog
-from grokcore.content import Container, Model
 
 
 class Herd(Container, grokcore.site.Application):
     pass
 
 
 class Mammoth(Model):
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_nonexistent.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_nonexistent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 """
 Grok allows you to set up catalog indexes in your application with a
 special indexes declaration. Here we show what happens if you try
 to set up an index for an attribute that does not exist on the interface.
 
 Let's set up a site in which we manage a couple of objects::
 
-(Note how the test output needs to be on one line to please to
-IGNORE_EXCEPTION_MODULE_IN_PYTHON2 normalizer)
-
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
   Traceback (most recent call last):
     ...
-  martian.error.GrokError: grokcore.catalog.Indexes in <module 'grokcore.catalog.ftests.catalog.indexes_nonexistent' from ...> refers to an attribute or method 'foo' on interface <InterfaceClass grokcore.catalog.ftests.catalog.indexes_nonexistent.IMammoth>, but this does not exist.
+  martian.error.GrokError: grokcore.catalog.Indexes in <module 'grokcore.catalog.tests.functional.catalog.indexes_nonexistent' from ...> refers to an attribute or method 'foo' on interface <InterfaceClass grokcore.catalog.tests.functional.catalog.indexes_nonexistent.IMammoth>, but this does not exist.
 
 Nuke the catalog and intids in the end, so as not to confuse
 other tests::
 
-  >>> from zope.site.hooks import setSite
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
   >>> from zope.catalog.interfaces import ICatalog
   >>> from zope.component import getUtility
   >>> catalog = getUtility(ICatalog)
 
   >>> sm = herd.getSiteManager()
   >>> from zope.catalog.interfaces import ICatalog
   >>> sm.unregisterUtility(catalog, provided=ICatalog)
   True
   >>> from zope.intid.interfaces import IIntIds
   >>> from zope import component
   >>> intids = component.getUtility(IIntIds)
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
-"""
+"""  # noqa: E501 line too long
 
 import grokcore.site
-import grokcore.catalog
-from zope.interface import Interface, Attribute
 from grokcore.content import Container
+from zope.interface import Attribute
+from zope.interface import Interface
+
+import grokcore.catalog
 
 
 class Herd(Container, grokcore.site.Application):
     pass
 
 
 class IMammoth(Interface):
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_set.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 We now demonstrate the use of a SetIndex with Grok::
 
 Let's set up a site in which we manage a couple of objects::
 
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
-  >>> from zope.site.hooks import setSite
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
 
 Now we add some indexable objects to the site::
 
   >>> herd['alpha'] = Mammoth('Alpha', ['big', 'brown'])
   >>> herd['beta'] = Mammoth('Beta', ['big', 'black', 'friendly'])
   >>> herd['gamma'] = Mammoth('Gamma', ['brown', 'friendly', 'gorgeous'])
@@ -43,17 +43,21 @@
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
 
 Unfortunately ftests don't have good isolation from each other yet.
 """
 
 import grokcore.site
+from grokcore.content import Container
+from grokcore.content import Model
+from zope.interface import Attribute
+from zope.interface import Interface
+from zope.interface import implementer
+
 import grokcore.catalog
-from grokcore.content import Container, Model
-from zope.interface import implementer, Interface, Attribute
 
 
 class Herd(Container, grokcore.site.Application):
     pass
 
 
 class IMammoth(Interface):
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_site.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/setuporder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,71 @@
 """
-Grok allows you to set up catalog indexes in your application with a
-special indexes declaration. In fact, these indexes can be set up for
-any site::
+This is similar to catalog.py, except that the site uses a base class
+which also defines a local utility.
 
-Let's set up a site in which we manage a couple of objects::
+Let's setup a site in which we manage a couple of objects:
 
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
-  >>> from zope.site.hooks import setSite
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
 
-The catalog is there in the site::
+Now we add some indexable objects to the site:
+
+  >>> herd['manfred'] = Mammoth('Manfred')
+  >>> herd['ellie'] = Mammoth('Ellie')
+
+Then we are able to query the catalog:
 
   >>> from zope.catalog.interfaces import ICatalog
-  >>> from zope.component import getUtility, queryUtility
-  >>> catalog = queryUtility(ICatalog, default=None)
-  >>> catalog is not None
-  True
+  >>> from zope.component import getUtility
+  >>> catalog = getUtility(ICatalog)
+  >>> for obj in catalog.searchResults(name=('Ellie', 'Ellie')):
+  ...     print(obj.name)
+  Ellie
 
 Nuke the catalog and intids in the end, so as not to confuse
 other tests::
 
+  >>> from zope import component
   >>> sm = herd.getSiteManager()
-  >>> from zope.catalog.interfaces import ICatalog
   >>> sm.unregisterUtility(catalog, provided=ICatalog)
   True
-  >>> from zope.intid.interfaces import IIntIds
-  >>> from zope import component
   >>> intids = component.getUtility(IIntIds)
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
+
 """
 
-import grokcore.site
-import grokcore.catalog
 from grokcore.content import Container
-from zope.interface import Interface, Attribute
+from grokcore.content import Model
+from grokcore.site import Site
+from grokcore.site import local_utility
+from zope import interface
+from zope.catalog.catalog import Catalog
+from zope.catalog.field import FieldIndex
+from zope.catalog.interfaces import ICatalog
+from zope.intid import IntIds
+from zope.intid.interfaces import IIntIds
+
+
+def setup_catalog(catalog):
+    catalog['name'] = FieldIndex('name', IMammoth)
+
 
+class IMammoth(interface.Interface):
+    name = interface.Attribute('Name')
 
-class Herd(Container, grokcore.site.Site):
-    pass
 
+@interface.implementer(IMammoth)
+class Mammoth(Model):
 
-class IMammoth(Interface):
-    name = Attribute('Name')
-    age = Attribute('Age')
+    def __init__(self, name):
+        self.name = name
 
-    def message():
-        """Message the mammoth has for the world.
-        """
 
+class BaseHerd(Container, Site):
+    local_utility(IntIds, provides=IIntIds)
 
-class MammothIndexes(grokcore.catalog.Indexes):
-    grokcore.site.site(Herd)
-    grokcore.catalog.context(IMammoth)
 
-    name = grokcore.catalog.Field()
-    age = grokcore.catalog.Field()
-    message = grokcore.catalog.Text()
+class Herd(BaseHerd):
+    local_utility(Catalog, provides=ICatalog, setup=setup_catalog)
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/catalog/indexes_valueindex.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/functional/catalog/indexes_valueindex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 We now demonstrate the use of a ValueIndex with Grok::
 
 Let's set up a site in which we manage a couple of objects::
 
   >>> herd = Herd()
   >>> getRootFolder()['herd'] = herd
-  >>> from zope.site.hooks import setSite
+  >>> from zope.component.hooks import setSite
   >>> setSite(herd)
 
 Now we add some indexable objects to the site::
 
   >>> herd['alpha'] = SabreTooth('Alpha', 'tolerant')
   >>> herd['beta'] = SabreTooth('Beta', 'narrowminded')
   >>> herd['gamma'] = SabreTooth('Gamma', 'friendly')
@@ -45,17 +45,21 @@
   >>> sm.unregisterUtility(intids, provided=IIntIds)
   True
 
 Unfortunately ftests don't have good isolation from each other yet.
 """
 
 import grokcore.site
+from grokcore.content import Container
+from grokcore.content import Model
+from zope.interface import Attribute
+from zope.interface import Interface
+from zope.interface import implementer
+
 import grokcore.catalog
-from grokcore.content import Container, Model
-from zope.interface import implementer, Interface, Attribute
 
 
 class Herd(Container, grokcore.site.Application):
     pass
 
 
 class ISabreTooth(Interface):
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/ftests/test_grok_functional.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/test_functional.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 import doctest
 import unittest
+
 from pkg_resources import resource_listdir
 
 from zope.app.appsetup.testlayer import ZODBLayer
-from zope.testing import renormalizing
+from zope.component.hooks import setSite
 
 import grokcore.catalog
 
 
-FunctionalLayer = ZODBLayer(grokcore.catalog)
+class CatalogZODBLayer(ZODBLayer):
+    """Custom ZODBLayer which also cleans up the site."""
+
+    def testTearDown(self):
+        setSite(None)
+        super().testTearDown()
 
 
-checker = renormalizing.RENormalizing()
+FunctionalLayer = CatalogZODBLayer(grokcore.catalog)
 
 
 def suiteFromPackage(name):
-    files = resource_listdir(__name__, name)
+    layer_dir = 'functional'
+    files = resource_listdir(__name__, f'{layer_dir}/{name}')
     suite = unittest.TestSuite()
     for filename in files:
         if not filename.endswith('.py'):
             continue
         if filename == '__init__.py':
             continue
 
-        dottedname = 'grokcore.catalog.ftests.%s.%s' % (name, filename[:-3])
+        dottedname = 'grokcore.catalog.tests.{}.{}.{}'.format(
+            layer_dir, name, filename[:-3])
         test = doctest.DocTestSuite(
             dottedname,
-            checker=checker,
             extraglobs=dict(getRootFolder=FunctionalLayer.getRootFolder),
             optionflags=(doctest.ELLIPSIS +
                          doctest.NORMALIZE_WHITESPACE +
-                         doctest.REPORT_NDIFF +
-                         renormalizing.IGNORE_EXCEPTION_MODULE_IN_PYTHON2))
+                         doctest.REPORT_NDIFF))
         test.layer = FunctionalLayer
 
         suite.addTest(test)
     return suite
 
 
 def test_suite():
     suite = unittest.TestSuite()
     for name in ["catalog"]:
         suite.addTest(suiteFromPackage(name))
     return suite
-
-
-if __name__ == '__main__':
-    unittest.main(defaultTest='test_suite')
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/index.py` & `grokcore.catalog-4.0/src/grokcore/catalog/index.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,38 +9,42 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """grokcore.catalog index definitions
 """
-import sys
 import calendar
+import sys
+
 import BTrees.Length
+import zc.catalog.index
+import zope.catalog.attribute
+import zope.catalog.interfaces
 import zope.component
 import zope.container.contained
-import zope.catalog.interfaces
-import zope.catalog.attribute
-import zc.catalog.index
-
-from zope.interface import implementer
-from zope.interface.interfaces import IMethod, IInterface
-from zope.catalog.interfaces import IAttributeIndex
+from martian.error import GrokError
+from martian.error import GrokImportError
+from martian.util import frame_is_class
+from zc.catalog.catalogindex import SetIndex
+from zc.catalog.catalogindex import ValueIndex
 from zope.catalog.field import FieldIndex
+from zope.catalog.interfaces import IAttributeIndex
 from zope.catalog.text import TextIndex
+from zope.interface import implementer
+from zope.interface.interfaces import IInterface
+from zope.interface.interfaces import IMethod
 from zope.intid.interfaces import IIntIds
-from zc.catalog.catalogindex import SetIndex, ValueIndex
-from martian.error import GrokError, GrokImportError
-from martian.util import frame_is_class
-from grokcore.catalog.interfaces import IIndexDefinition
+
 from grokcore.catalog.interfaces import IAttributeIndexDefinition
+from grokcore.catalog.interfaces import IIndexDefinition
 
 
 @implementer(IIndexDefinition)
-class IndexDefinition(object):
+class IndexDefinition:
     """The definition of a particular index in a
     :data:`grokcore.catalog.Indexes` class.
 
     Note that, since index creation (and thus a call to our :meth:`setup()`
     method) currently occurs only during the creation of a new Grok
     `Application` object in the Zope Database, the presence of this
     declaration in Grok application code is nearly always a no-op.
@@ -61,15 +65,15 @@
         # For indexes that do not implement IAttributeIndex, we
         # cannot do magic things. In these cases, just initialize
         # the index with the given attributes.
         catalog[name] = self.index_class(*self._args, **self._kw)
 
 
 @implementer(IAttributeIndexDefinition)
-class AttributeIndexDefinition(object):
+class AttributeIndexDefinition:
     """The definition of a particular index in a
     :data:`grokcore.catalog.Indexes` class.
 
     This base class defines the actual behavior of
     :class:`grokcore.catalog.index.Field` and the other kinds of attribute
     index that Grok supports. Upon our instantiation, we save every parameter
     that we were passed; later, if an index actually needs to be created
@@ -179,35 +183,35 @@
         self.documentCount = BTrees.Length.Length(0)
         self.wordCount = BTrees.Length.Length(0)
 
     def index_doc(self, doc_id, value):
         if value is None:
             return
         value = to_timestamp(value)
-        super(_DatetimeIndex, self).index_doc(doc_id, value)
+        super().index_doc(doc_id, value)
 
     def apply(self, query):
         if 'any_of' in query:
             # The "value" of the dict is a sequence of datetime objects.
             # Convert it into a timestamps.
             query['any_of'] = [to_timestamp(v) for v in query['any_of']]
         elif 'between' in query:
             # The "value" of the dict is a sequence of arguments to pass on to
             # the underlying btree. Convert the first two parameters that are
             # datetime objects (or None) into timestamps.
             query['between'] = parameters = list(query['between'])
             parameters[0] = to_timestamp(parameters[0])
             parameters[1] = to_timestamp(parameters[1])
-        return super(_DatetimeIndex, self).apply(query)
+        return super().apply(query)
 
     def values(self, min=None, max=None, excludemin=False, excludemax=False,
                doc_id=None):
         min = to_timestamp(min) if min is not None else None
         max = to_timestamp(max) if max is not None else None
-        return super(_DatetimeIndex, self).values(
+        return super().values(
             min, max, excludemin, excludemax, doc_id)
 
 
 class DatetimeIndex(
         zope.catalog.attribute.AttributeIndex,
         _DatetimeIndex,
         zope.container.contained.Contained):
@@ -226,20 +230,20 @@
             return None
         if isinstance(value, int):
             return value
         intids = zope.component.getUtility(IIntIds)
         return intids.getId(value)
 
     def index_doc(self, docid, value):
-        return super(_IntIdIndex, self).index_doc(
+        return super().index_doc(
             docid, self._get_value_id(value))
 
     def apply(self, query):
         value = self._get_value_id(query)
-        return super(_IntIdIndex, self).apply((value, value))
+        return super().apply((value, value))
 
 
 class IntIdIndex(
         zope.catalog.attribute.AttributeIndex,
         _IntIdIndex,
         zope.container.contained.Contained):
     pass
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/interfaces.py` & `grokcore.catalog-4.0/src/grokcore/catalog/interfaces.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """grokcore.catalog interfaces
 """
-from zope.interface import Interface, Attribute
+from zope.interface import Attribute
+from zope.interface import Interface
+
 
 class IIndexDefinition(Interface):
-    """Define an index for grok.Indexes.
-    """
+    """Define an index for grok.Indexes."""
 
     def __init__(self, *args, **kw):
         """Arguments and keyword arguments passed to the index class.
 
         All parameters are simply passed along to the index class we create,
         which interprets them as configuration details of its own.
         """
@@ -29,23 +30,25 @@
     def setup(catalog, name, context):
         """Set up index called name in given catalog.
 
         Use name for index name and attribute to index. Set up
         index for interface or class context.
         """
 
+
 class IAttributeIndexDefinition(IIndexDefinition):
     """Define an index for grok.Indexes providing IAttributeIndex.
     """
 
     def __init__(self, attribute=None, *args, **kw):
         """Attribute to index.
 
         Attribute (optionally) defines the attribute we should index. All
         other parameters are simply passed along to the index class we
         create, which interprets them as configuration details of its own.
 
         Arguments and keyword arguments passed to the index class.
         """
 
+
 class IBaseClasses(Interface):
     Indexes = Attribute("Base class for a catalog indexes component.")
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/meta.py` & `grokcore.catalog-4.0/src/grokcore/catalog/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """grokcore.catalog meta
 """
-import martian
-import zope.component
 import grokcore.component
 import grokcore.site
 import grokcore.site.interfaces
-
-from grokcore.catalog.components import IndexesClass
+import martian
+import zope.component
 from martian.error import GrokError
 from zope.catalog.catalog import Catalog
 from zope.catalog.interfaces import ICatalog
 from zope.exceptions.interfaces import DuplicationError
 from zope.intid import IntIds
 from zope.intid.interfaces import IIntIds
 from zope.lifecycleevent.interfaces import IObjectAddedEvent
 
+from grokcore.catalog.components import IndexesClass
+
 
 class IndexesGrokker(martian.InstanceGrokker):
     """Grokker for index bundles."""
     martian.component(IndexesClass)
 
     def grok(self, name, factory, module_info, config, **kw):
         site = grokcore.site.site.bind().get(factory)
@@ -59,15 +59,15 @@
         config.action(
             discriminator=None,
             callable=grokcore.component.provideHandler,
             args=(subscriber, subscribed))
         return True
 
 
-class IndexesSetupSubscriber(object):
+class IndexesSetupSubscriber:
     """Helper that sets up indexes when their Grok site is created.
 
     Each `grokcore.catalog.Indexes` class serves as an assertion that,
     whenever an instance of its `grokcore.site.site()` is created,
     the given list of indexes should be generated as well.
 
     But a long period of time could elapse between when the application
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/testing.py` & `grokcore.catalog-4.0/src/grokcore/catalog/testing.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Grok test helpers
 """
-from zope.configuration.config import ConfigurationMachine
 from grokcore.component import zcml
+from zope.configuration.config import ConfigurationMachine
 
 
 def grok(module_name):
     config = ConfigurationMachine()
     zcml.do_grok('grokcore.component.meta', config)
     zcml.do_grok('grokcore.site.meta', config)
     zcml.do_grok('grokcore.catalog.meta', config)
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/tests/catalog/indexes_no_app.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/base/catalog/indexes_no_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """
 Grok allows you to set up catalog indexes in your application with a
 special indexes declaration.  We do need to specify a site (such as
 the application) for the Indexes however, otherwise we get a GrokError:
 
-(Note how the test output needs to be on one line to please to
-IGNORE_EXCEPTION_MODULE_IN_PYTHON2 normalizer)
-
   >>> from grokcore.catalog import testing
   >>> testing.grok(__name__)
   Traceback (most recent call last):
     ...
-  martian.error.GrokError: No site specified for grokcore.catalog.Indexes subclass in module <module 'grokcore.catalog.tests.catalog.indexes_no_app' from ...>. Use grokcore.site.site() to specify.
+  martian.error.GrokError: No site specified for grokcore.catalog.Indexes subclass in module <module 'grokcore.catalog.tests.base.catalog.indexes_no_app' from ...>. Use grokcore.site.site() to specify.
 
-"""
-import grokcore.site
-import grokcore.catalog
+"""  # noqa: E501 line too long
 import grokcore.component
+import grokcore.site
+from grokcore.content import Container
+from grokcore.content import Model
 
-from grokcore.site import Application
-from grokcore.content import Model, Container
+import grokcore.catalog
 
 
 class Herd(Container, grokcore.site.Application):
     pass
 
 
 class Mammoth(Model):
```

### Comparing `grokcore.catalog-3.0.1/src/grokcore/catalog/tests/test_grok.py` & `grokcore.catalog-4.0/src/grokcore/catalog/tests/test_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,51 @@
 import doctest
 import unittest
+
 from pkg_resources import resource_listdir
 
-from zope.testing import cleanup, renormalizing
 import zope.component.eventtesting
+from zope.testing import cleanup
 
 
 def setUpZope(test):
     zope.component.eventtesting.setUp(test)
 
 
 def cleanUpZope(test):
     cleanup.cleanUp()
 
 
-checker = renormalizing.RENormalizing()
-
-
 def suiteFromPackage(name):
-    files = resource_listdir(__name__, name)
+    layer_dir = 'base'
+    files = resource_listdir(__name__, f'{layer_dir}/{name}')
     suite = unittest.TestSuite()
     for filename in files:
         if not filename.endswith('.py'):
             continue
         if filename.endswith('_fixture.py'):
             continue
         if filename == '__init__.py':
             continue
 
         print(filename)
 
-        dottedname = 'grokcore.catalog.tests.%s.%s' % (name, filename[:-3])
+        dottedname = 'grokcore.catalog.tests.{}.{}.{}'.format(
+            layer_dir, name, filename[:-3])
         test = doctest.DocTestSuite(
             dottedname,
             setUp=setUpZope,
             tearDown=cleanUpZope,
-            checker=checker,
             optionflags=(
                 doctest.ELLIPSIS +
-                doctest.NORMALIZE_WHITESPACE +
-                renormalizing.IGNORE_EXCEPTION_MODULE_IN_PYTHON2))
+                doctest.NORMALIZE_WHITESPACE))
 
         suite.addTest(test)
 
     return suite
 
 
 def test_suite():
     suite = unittest.TestSuite()
     for name in ['catalog']:
         suite.addTest(suiteFromPackage(name))
     return suite
-
-if __name__ == '__main__':
-    unittest.main(defaultTest='test_suite')
```


# Comparing `tmp/spotfire-2.0.1.tar.gz` & `tmp/spotfire-2.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotfire-2.0.1.tar", last modified: Wed May 24 20:58:19 2023, max compression
+gzip compressed data, was "spotfire-2.0.1.post1.tar", last modified: Tue Jul 11 21:52:38 2023, max compression
```

## Comparing `spotfire-2.0.1.tar` & `spotfire-2.0.1.post1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:19.826495 spotfire-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-24 20:58:12.000000 spotfire-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-24 20:58:12.000000 spotfire-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-24 20:58:19.826495 spotfire-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-24 20:58:12.000000 spotfire-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-24 20:58:12.000000 spotfire-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 20:58:12.000000 spotfire-2.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 20:58:19.826495 spotfire-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-24 20:58:12.000000 spotfire-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:19.822495 spotfire-2.0.1/spotfire/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-24 20:58:12.000000 spotfire-2.0.1/spotfire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-24 20:58:12.000000 spotfire-2.0.1/spotfire/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-05-24 20:58:12.000000 spotfire-2.0.1/spotfire/cabfile.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-24 20:58:12.000000 spotfire-2.0.1/spotfire/cabfile_helpers.c
--rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-05-24 20:58:12.000000 spotfire-2.0.1/spotfire/codesign.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    18848 2023-05-24 20:58:12.000000 spotfire-2.0.1/spotfire/data_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-24 20:58:12.000000 spotfire-2.0.1/spotfire/public.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-24 20:58:12.000000 spotfire-2.0.1/spotfire/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    84617 2023-05-24 20:58:12.000000 spotfire-2.0.1/spotfire/sbdf.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-24 20:58:12.000000 spotfire-2.0.1/spotfire/sbdf_helpers.c
--rw-r--r--   0 runner    (1001) docker     (123)    44229 2023-05-24 20:58:12.000000 spotfire-2.0.1/spotfire/spk.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-24 20:58:12.000000 spotfire-2.0.1/spotfire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:19.822495 spotfire-2.0.1/spotfire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-24 20:58:19.000000 spotfire-2.0.1/spotfire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-24 20:58:19.000000 spotfire-2.0.1/spotfire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 20:58:19.000000 spotfire-2.0.1/spotfire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-24 20:58:19.000000 spotfire-2.0.1/spotfire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 20:58:19.000000 spotfire-2.0.1/spotfire.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:19.822495 spotfire-2.0.1/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:12.000000 spotfire-2.0.1/vendor/__init__.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:19.818495 spotfire-2.0.1/vendor/sbdf-c/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:19.822495 spotfire-2.0.1/vendor/sbdf-c/include/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/all.h
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/all_io.h
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/bytearray.h
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/columnmetadata.h
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/columnslice.h
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/columnslice_io.h
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/config.h
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/errors.h
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/fileheader.h
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/metadata.h
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/object.h
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/object_io.h
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/sbdfstring.h
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/sectiontypeid.h
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/sectiontypeid_io.h
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/tablemetadata.h
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/tablemetadata_io.h
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/tableslice.h
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/tableslice_io.h
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/valuearray.h
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/valuearray_io.h
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/valuetype.h
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/valuetype_io.h
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/include/valuetypeid.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:19.826495 spotfire-2.0.1/vendor/sbdf-c/src/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/bswap.c
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/bswap.h
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/bytearray.c
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/columnmetadata.c
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/columnslice.c
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/errors.c
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/fileheader.c
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/internals.c
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/metadata.c
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/object.c
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/sbdfstring.c
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/tablemetadata.c
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/tableslice.c
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/valuearray.c
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/src/valuetype.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:19.826495 spotfire-2.0.1/vendor/sbdf-c/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/tests/api_scenario.c
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/tests/cppsupp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/tests/test.h
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-24 20:58:13.000000 spotfire-2.0.1/vendor/sbdf-c/tests/test_c.h
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-24 20:58:12.000000 spotfire-2.0.1/vendor/sbdf_c.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 20:58:19.826495 spotfire-2.0.1/vendor/windows/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-24 20:58:12.000000 spotfire-2.0.1/vendor/windows/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-24 20:58:12.000000 spotfire-2.0.1/vendor/windows/fci.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-24 20:58:12.000000 spotfire-2.0.1/vendor/windows/mssign32.h
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-24 20:58:12.000000 spotfire-2.0.1/vendor/windows/mssign32.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-24 20:58:12.000000 spotfire-2.0.1/vendor/windows/wincrypt.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:52:38.834288 spotfire-2.0.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-11 21:52:38.834288 spotfire-2.0.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:52:38.834288 spotfire-2.0.1.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:52:38.822287 spotfire-2.0.1.post1/spotfire/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/spotfire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/spotfire/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/spotfire/cabfile.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/spotfire/cabfile_helpers.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/spotfire/codesign.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    18848 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/spotfire/data_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/spotfire/public.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/spotfire/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    84617 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/spotfire/sbdf.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/spotfire/sbdf_helpers.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44232 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/spotfire/spk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/spotfire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:52:38.826287 spotfire-2.0.1.post1/spotfire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-11 21:52:38.000000 spotfire-2.0.1.post1/spotfire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-11 21:52:38.000000 spotfire-2.0.1.post1/spotfire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:52:38.000000 spotfire-2.0.1.post1/spotfire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 21:52:38.000000 spotfire-2.0.1.post1/spotfire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 21:52:38.000000 spotfire-2.0.1.post1/spotfire.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:52:38.826287 spotfire-2.0.1.post1/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/vendor/__init__.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:52:38.822287 spotfire-2.0.1.post1/vendor/sbdf-c/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:52:38.830287 spotfire-2.0.1.post1/vendor/sbdf-c/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/all.h
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/all_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/bytearray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/columnmetadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/columnslice.h
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/columnslice_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/errors.h
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/fileheader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/metadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/object.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/object_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/sbdfstring.h
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/sectiontypeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/sectiontypeid_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/tablemetadata.h
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/tablemetadata_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/tableslice.h
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/tableslice_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/valuearray.h
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/valuearray_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/valuetype.h
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/valuetype_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/include/valuetypeid.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:52:38.830287 spotfire-2.0.1.post1/vendor/sbdf-c/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/bswap.c
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/bswap.h
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/bytearray.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/columnmetadata.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/columnslice.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/errors.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/fileheader.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/internals.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/metadata.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/object.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/sbdfstring.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/tablemetadata.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/tableslice.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/valuearray.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/src/valuetype.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:52:38.830287 spotfire-2.0.1.post1/vendor/sbdf-c/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/tests/api_scenario.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/tests/cppsupp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/tests/test.h
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 21:52:29.000000 spotfire-2.0.1.post1/vendor/sbdf-c/tests/test_c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/vendor/sbdf_c.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:52:38.834288 spotfire-2.0.1.post1/vendor/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/vendor/windows/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/vendor/windows/fci.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/vendor/windows/mssign32.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/vendor/windows/mssign32.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-11 21:52:28.000000 spotfire-2.0.1.post1/vendor/windows/wincrypt.pxd
```

### Comparing `spotfire-2.0.1/LICENSE` & `spotfire-2.0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/PKG-INFO` & `spotfire-2.0.1.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: spotfire
-Version: 2.0.1
-Summary: Package for Building Python Extensions to TIBCO Spotfire
+Version: 2.0.1.post1
+Summary: Package for Building Python Extensions to Spotfire
 Home-page: https://github.com/TIBCOSoftware/spotfire-python
 Author: Cloud Software Group, Inc.
 Maintainer: Spotfire Python Package Support
 Maintainer-email: spotfirepython@tibco.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Package for Building Python Extensions to TIBCO Spotfire® 
+# Package for Building Python Extensions to Spotfire® 
 
 This package provides functions used for integrating Python with Spotfire, including: 
 * reading and writing files in Spotfire Binary Data Format (SBDF)
 * building Spotfire Packages (SPKs) for distributing Python interpreters and custom packages with Spotfire
 * internal handler code for executing Data Functions from Spotfire
 
 ### Installation
```

### Comparing `spotfire-2.0.1/README.md` & `spotfire-2.0.1.post1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Package for Building Python Extensions to TIBCO Spotfire® 
+# Package for Building Python Extensions to Spotfire® 
 
 This package provides functions used for integrating Python with Spotfire, including: 
 * reading and writing files in Spotfire Binary Data Format (SBDF)
 * building Spotfire Packages (SPKs) for distributing Python interpreters and custom packages with Spotfire
 * internal handler code for executing Data Functions from Spotfire
 
 ### Installation
```

### Comparing `spotfire-2.0.1/setup.py` & `spotfire-2.0.1.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
               cython_c_in_temp=True
               ),
 ]
 
 setup(
     name='spotfire',
     version=version['__version__'],
-    description='Package for Building Python Extensions to TIBCO Spotfire',
+    description='Package for Building Python Extensions to Spotfire',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Cloud Software Group, Inc.',
     maintainer='Spotfire Python Package Support',
     maintainer_email='spotfirepython@tibco.com',
     url='https://github.com/TIBCOSoftware/spotfire-python',
     license='BSD 3-Clause License',
```

### Comparing `spotfire-2.0.1/spotfire/_utils.py` & `spotfire-2.0.1.post1/spotfire/_utils.py`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/spotfire/cabfile.pyx` & `spotfire-2.0.1.post1/spotfire/cabfile.pyx`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/spotfire/cabfile_helpers.c` & `spotfire-2.0.1.post1/spotfire/cabfile_helpers.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/spotfire/codesign.pyx` & `spotfire-2.0.1.post1/spotfire/codesign.pyx`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/spotfire/data_function.py` & `spotfire-2.0.1.post1/spotfire/data_function.py`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/spotfire/public.py` & `spotfire-2.0.1.post1/spotfire/public.py`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/spotfire/sbdf.pyx` & `spotfire-2.0.1.post1/spotfire/sbdf.pyx`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/spotfire/sbdf_helpers.c` & `spotfire-2.0.1.post1/spotfire/sbdf_helpers.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/spotfire/spk.py` & `spotfire-2.0.1.post1/spotfire/spk.py`

 * *Files 0% similar despite different names*

```diff
@@ -699,15 +699,15 @@
 
     # Verify the version component
     version_identifier = getattr(args, "version")
     if version_identifier < 0:
         print("Error: '--version' cannot be less than 0.")
         sys.exit(1)
     if version_identifier < 1000:
-        print("Warning: '--version' should not be less than 1000 in order to avoid conflicts with TIBCO-provided "
+        print("Warning: '--version' should not be less than 1000 in order to avoid conflicts with Spotfire-provided "
               "packages.")
 
     # Set up the package builder
     analyst = getattr(args, "analyst")
     if analyst:
         package_builder = _CabPackageBuilder()
         package_builder.excludes = getattr(args, "exclude")
```

### Comparing `spotfire-2.0.1/spotfire.egg-info/PKG-INFO` & `spotfire-2.0.1.post1/spotfire.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: spotfire
-Version: 2.0.1
-Summary: Package for Building Python Extensions to TIBCO Spotfire
+Version: 2.0.1.post1
+Summary: Package for Building Python Extensions to Spotfire
 Home-page: https://github.com/TIBCOSoftware/spotfire-python
 Author: Cloud Software Group, Inc.
 Maintainer: Spotfire Python Package Support
 Maintainer-email: spotfirepython@tibco.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Package for Building Python Extensions to TIBCO Spotfire® 
+# Package for Building Python Extensions to Spotfire® 
 
 This package provides functions used for integrating Python with Spotfire, including: 
 * reading and writing files in Spotfire Binary Data Format (SBDF)
 * building Spotfire Packages (SPKs) for distributing Python interpreters and custom packages with Spotfire
 * internal handler code for executing Data Functions from Spotfire
 
 ### Installation
```

### Comparing `spotfire-2.0.1/spotfire.egg-info/SOURCES.txt` & `spotfire-2.0.1.post1/spotfire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/all.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/all.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/all_io.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/all_io.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/bytearray.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/bytearray.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/columnmetadata.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/columnmetadata.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/columnslice.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/columnslice.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/columnslice_io.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/columnslice_io.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/errors.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/errors.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/fileheader.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/fileheader.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/metadata.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/metadata.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/object.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/object.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/object_io.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/object_io.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/sbdfstring.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/sbdfstring.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/sectiontypeid.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/sectiontypeid.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/sectiontypeid_io.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/sectiontypeid_io.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/tablemetadata.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/tablemetadata.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/tablemetadata_io.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/tablemetadata_io.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/tableslice.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/tableslice.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/tableslice_io.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/tableslice_io.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/valuearray.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/valuearray.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/valuearray_io.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/valuearray_io.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/valuetype.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/valuetype.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/valuetype_io.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/valuetype_io.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/include/valuetypeid.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/include/valuetypeid.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/bswap.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/bswap.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/bytearray.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/bytearray.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/columnmetadata.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/columnmetadata.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/columnslice.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/columnslice.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/errors.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/errors.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/fileheader.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/fileheader.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/internals.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/internals.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/internals.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/internals.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/metadata.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/metadata.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/object.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/object.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/sbdfstring.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/sbdfstring.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/tablemetadata.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/tablemetadata.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/tableslice.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/tableslice.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/valuearray.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/valuearray.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/src/valuetype.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/src/valuetype.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/tests/api_scenario.c` & `spotfire-2.0.1.post1/vendor/sbdf-c/tests/api_scenario.c`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/tests/cppsupp.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/tests/cppsupp.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/tests/test.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/tests/test.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf-c/tests/test_c.h` & `spotfire-2.0.1.post1/vendor/sbdf-c/tests/test_c.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/sbdf_c.pxd` & `spotfire-2.0.1.post1/vendor/sbdf_c.pxd`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/windows/__init__.pxd` & `spotfire-2.0.1.post1/vendor/windows/__init__.pxd`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/windows/fci.pxd` & `spotfire-2.0.1.post1/vendor/windows/fci.pxd`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/windows/mssign32.h` & `spotfire-2.0.1.post1/vendor/windows/mssign32.h`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/windows/mssign32.pxd` & `spotfire-2.0.1.post1/vendor/windows/mssign32.pxd`

 * *Files identical despite different names*

### Comparing `spotfire-2.0.1/vendor/windows/wincrypt.pxd` & `spotfire-2.0.1.post1/vendor/windows/wincrypt.pxd`

 * *Files identical despite different names*


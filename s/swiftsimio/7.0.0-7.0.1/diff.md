# Comparing `tmp/swiftsimio-7.0.0.tar.gz` & `tmp/swiftsimio-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftsimio-7.0.0.tar", last modified: Thu Jul  6 15:44:02 2023, max compression
+gzip compressed data, was "swiftsimio-7.0.1.tar", last modified: Wed Jul 12 15:53:47 2023, max compression
```

## Comparing `swiftsimio-7.0.0.tar` & `swiftsimio-7.0.1.tar`

### file list

```diff
@@ -1,47 +1,89 @@
-drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-06 15:44:02.098849 swiftsimio-7.0.0/
--rw-r--r--   0 jborrow    (501) staff       (20)    35147 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/COPYING
--rw-r--r--   0 jborrow    (501) staff       (20)     7651 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/COPYING.LESSER
--rw-r--r--   0 jborrow    (501) staff       (20)     4080 2023-07-06 15:44:02.098689 swiftsimio-7.0.0/PKG-INFO
--rw-r--r--   0 jborrow    (501) staff       (20)     3244 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/README.md
--rw-r--r--   0 jborrow    (501) staff       (20)     1049 2023-07-06 15:43:53.000000 swiftsimio-7.0.0/pyproject.toml
--rw-r--r--   0 jborrow    (501) staff       (20)       38 2023-07-06 15:44:02.098894 swiftsimio-7.0.0/setup.cfg
-drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-06 15:44:02.094030 swiftsimio-7.0.0/swiftsimio/
--rw-r--r--   0 jborrow    (501) staff       (20)      378 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/swiftsimio/__cite__.py
--rw-r--r--   0 jborrow    (501) staff       (20)     2864 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/__init__.py
--rw-r--r--   0 jborrow    (501) staff       (20)       22 2023-07-06 15:43:30.000000 swiftsimio-7.0.0/swiftsimio/__version__.py
--rw-r--r--   0 jborrow    (501) staff       (20)    15983 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/accelerated.py
--rw-r--r--   0 jborrow    (501) staff       (20)     4713 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/conversions.py
--rw-r--r--   0 jborrow    (501) staff       (20)    13993 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/masks.py
--rw-r--r--   0 jborrow    (501) staff       (20)    35791 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/objects.py
--rw-r--r--   0 jborrow    (501) staff       (20)     1708 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/optional_packages.py
--rw-r--r--   0 jborrow    (501) staff       (20)    51005 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/reader.py
--rw-r--r--   0 jborrow    (501) staff       (20)     3590 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/swiftsimio/statistics.py
--rw-r--r--   0 jborrow    (501) staff       (20)    10236 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/subset_writer.py
--rwxr-xr-x   0 jborrow    (501) staff       (20)     5779 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/swiftsnap.py
--rw-r--r--   0 jborrow    (501) staff       (20)      800 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/swiftsimio/units.py
--rw-r--r--   0 jborrow    (501) staff       (20)    22898 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/swiftsimio/writer.py
-drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-06 15:44:02.095209 swiftsimio-7.0.0/swiftsimio.egg-info/
--rw-r--r--   0 jborrow    (501) staff       (20)     4080 2023-07-06 15:44:02.000000 swiftsimio-7.0.0/swiftsimio.egg-info/PKG-INFO
--rw-r--r--   0 jborrow    (501) staff       (20)     1049 2023-07-06 15:44:02.000000 swiftsimio-7.0.0/swiftsimio.egg-info/SOURCES.txt
--rw-r--r--   0 jborrow    (501) staff       (20)        1 2023-07-06 15:44:02.000000 swiftsimio-7.0.0/swiftsimio.egg-info/dependency_links.txt
--rw-r--r--   0 jborrow    (501) staff       (20)       61 2023-07-06 15:44:02.000000 swiftsimio-7.0.0/swiftsimio.egg-info/entry_points.txt
--rw-r--r--   0 jborrow    (501) staff       (20)       37 2023-07-06 15:44:02.000000 swiftsimio-7.0.0/swiftsimio.egg-info/requires.txt
--rw-r--r--   0 jborrow    (501) staff       (20)       11 2023-07-06 15:44:02.000000 swiftsimio-7.0.0/swiftsimio.egg-info/top_level.txt
-drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-06 15:44:02.098271 swiftsimio-7.0.0/tests/
--rw-r--r--   0 jborrow    (501) staff       (20)     2878 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_accelerated.py
--rw-r--r--   0 jborrow    (501) staff       (20)     1414 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_chunked_read_ranges.py
--rw-r--r--   0 jborrow    (501) staff       (20)     1028 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_conversions.py
--rw-r--r--   0 jborrow    (501) staff       (20)     1487 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_cosmo_array.py
--rw-r--r--   0 jborrow    (501) staff       (20)    23634 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_cosmo_array_attrs.py
--rw-r--r--   0 jborrow    (501) staff       (20)    11412 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_data.py
--rw-r--r--   0 jborrow    (501) staff       (20)     4502 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_extraparts.py
--rw-r--r--   0 jborrow    (501) staff       (20)      259 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_helper.py
--rw-r--r--   0 jborrow    (501) staff       (20)     2640 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_mask.py
--rw-r--r--   0 jborrow    (501) staff       (20)      897 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_metadata.py
--rw-r--r--   0 jborrow    (501) staff       (20)      436 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_physical_conversion.py
--rw-r--r--   0 jborrow    (501) staff       (20)     2022 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_read_ic.py
--rw-r--r--   0 jborrow    (501) staff       (20)     3737 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_rotate_visualisations.py
--rw-r--r--   0 jborrow    (501) staff       (20)      890 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_rotation.py
--rw-r--r--   0 jborrow    (501) staff       (20)     2046 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_smoothing_length_generation.py
--rw-r--r--   0 jborrow    (501) staff       (20)     1158 2021-10-21 12:24:47.000000 swiftsimio-7.0.0/tests/test_vistools.py
--rw-r--r--   0 jborrow    (501) staff       (20)    14136 2023-07-06 15:41:16.000000 swiftsimio-7.0.0/tests/test_visualisation.py
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.220269 swiftsimio-7.0.1/
+-rw-r--r--   0 jborrow    (501) staff       (20)    35147 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/COPYING
+-rw-r--r--   0 jborrow    (501) staff       (20)     7651 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/COPYING.LESSER
+-rw-r--r--   0 jborrow    (501) staff       (20)     4080 2023-07-12 15:53:47.220135 swiftsimio-7.0.1/PKG-INFO
+-rw-r--r--   0 jborrow    (501) staff       (20)     3244 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/README.md
+-rw-r--r--   0 jborrow    (501) staff       (20)     1370 2023-07-12 15:53:40.000000 swiftsimio-7.0.1/pyproject.toml
+-rw-r--r--   0 jborrow    (501) staff       (20)       38 2023-07-12 15:53:47.220311 swiftsimio-7.0.1/setup.cfg
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.211902 swiftsimio-7.0.1/swiftsimio/
+-rw-r--r--   0 jborrow    (501) staff       (20)      378 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/__cite__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     2864 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/__init__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)       22 2023-07-06 15:43:30.000000 swiftsimio-7.0.1/swiftsimio/__version__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    15983 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/accelerated.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     4713 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/conversions.py
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.213019 swiftsimio-7.0.1/swiftsimio/initial_conditions/
+-rw-r--r--   0 jborrow    (501) staff       (20)       39 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/initial_conditions/__init__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)       39 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/initial_conditions/generate_particles.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    13993 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/masks.py
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.213160 swiftsimio-7.0.1/swiftsimio/metadata/
+-rw-r--r--   0 jborrow    (501) staff       (20)      378 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/metadata/__init__.py
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.213433 swiftsimio-7.0.1/swiftsimio/metadata/cosmology/
+-rw-r--r--   0 jborrow    (501) staff       (20)       32 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/metadata/cosmology/__init__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     2802 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/metadata/cosmology/cosmology_fields.py
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.213723 swiftsimio-7.0.1/swiftsimio/metadata/metadata/
+-rw-r--r--   0 jborrow    (501) staff       (20)       31 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/metadata/metadata/__init__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     2124 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/metadata/metadata/metadata_fields.py
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.214176 swiftsimio-7.0.1/swiftsimio/metadata/particle/
+-rw-r--r--   0 jborrow    (501) staff       (20)       61 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/metadata/particle/__init__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     1814 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/metadata/particle/particle_fields.py
+-rw-r--r--   0 jborrow    (501) staff       (20)      559 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/metadata/particle/particle_types.py
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.214583 swiftsimio-7.0.1/swiftsimio/metadata/unit/
+-rw-r--r--   0 jborrow    (501) staff       (20)       53 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/metadata/unit/__init__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     3281 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/metadata/unit/unit_fields.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     1859 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/metadata/unit/unit_types.py
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.214852 swiftsimio-7.0.1/swiftsimio/metadata/writer/
+-rw-r--r--   0 jborrow    (501) staff       (20)       31 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/metadata/writer/__init__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)      521 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/metadata/writer/required_fields.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    35791 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/objects.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     1708 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/optional_packages.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    51005 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/reader.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     3590 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/statistics.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    10236 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/subset_writer.py
+-rwxr-xr-x   0 jborrow    (501) staff       (20)     5779 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/swiftsnap.py
+-rw-r--r--   0 jborrow    (501) staff       (20)      800 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/units.py
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.215884 swiftsimio-7.0.1/swiftsimio/visualisation/
+-rw-r--r--   0 jborrow    (501) staff       (20)      280 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/visualisation/__init__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    16895 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/visualisation/projection.py
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.217148 swiftsimio-7.0.1/swiftsimio/visualisation/projection_backends/
+-rw-r--r--   0 jborrow    (501) staff       (20)     2151 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/visualisation/projection_backends/__init__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     8843 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/visualisation/projection_backends/fast.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     8728 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/visualisation/projection_backends/gpu.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     6157 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/visualisation/projection_backends/histogram.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     2522 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/visualisation/projection_backends/kernels.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     8536 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/visualisation/projection_backends/reference.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    10777 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/visualisation/projection_backends/renormalised.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    15432 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/visualisation/projection_backends/subsampled.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    15589 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/visualisation/projection_backends/subsampled_extreme.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     2393 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/visualisation/rotation.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    20777 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/visualisation/slice.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     4138 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/visualisation/smoothing_length_generation.py
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.217379 swiftsimio-7.0.1/swiftsimio/visualisation/tools/
+-rw-r--r--   0 jborrow    (501) staff       (20)        0 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/visualisation/tools/__init__.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    12056 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/swiftsimio/visualisation/tools/cmaps.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    20354 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/visualisation/volume_render.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    22898 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/swiftsimio/writer.py
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.212756 swiftsimio-7.0.1/swiftsimio.egg-info/
+-rw-r--r--   0 jborrow    (501) staff       (20)     4080 2023-07-12 15:53:47.000000 swiftsimio-7.0.1/swiftsimio.egg-info/PKG-INFO
+-rw-r--r--   0 jborrow    (501) staff       (20)     2542 2023-07-12 15:53:47.000000 swiftsimio-7.0.1/swiftsimio.egg-info/SOURCES.txt
+-rw-r--r--   0 jborrow    (501) staff       (20)        1 2023-07-12 15:53:47.000000 swiftsimio-7.0.1/swiftsimio.egg-info/dependency_links.txt
+-rw-r--r--   0 jborrow    (501) staff       (20)       61 2023-07-12 15:53:47.000000 swiftsimio-7.0.1/swiftsimio.egg-info/entry_points.txt
+-rw-r--r--   0 jborrow    (501) staff       (20)       37 2023-07-12 15:53:47.000000 swiftsimio-7.0.1/swiftsimio.egg-info/requires.txt
+-rw-r--r--   0 jborrow    (501) staff       (20)       11 2023-07-12 15:53:47.000000 swiftsimio-7.0.1/swiftsimio.egg-info/top_level.txt
+drwxr-xr-x   0 jborrow    (501) staff       (20)        0 2023-07-12 15:53:47.219851 swiftsimio-7.0.1/tests/
+-rw-r--r--   0 jborrow    (501) staff       (20)     2878 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/tests/test_accelerated.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     1414 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/tests/test_chunked_read_ranges.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     1028 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/tests/test_conversions.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     1487 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/tests/test_cosmo_array.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    23634 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/tests/test_cosmo_array_attrs.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    11412 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/tests/test_data.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     4502 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/tests/test_extraparts.py
+-rw-r--r--   0 jborrow    (501) staff       (20)      259 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/tests/test_helper.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     2640 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/tests/test_mask.py
+-rw-r--r--   0 jborrow    (501) staff       (20)      897 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/tests/test_metadata.py
+-rw-r--r--   0 jborrow    (501) staff       (20)      436 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/tests/test_physical_conversion.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     2022 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/tests/test_read_ic.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     3737 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/tests/test_rotate_visualisations.py
+-rw-r--r--   0 jborrow    (501) staff       (20)      890 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/tests/test_rotation.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     2046 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/tests/test_smoothing_length_generation.py
+-rw-r--r--   0 jborrow    (501) staff       (20)     1158 2021-10-21 12:24:47.000000 swiftsimio-7.0.1/tests/test_vistools.py
+-rw-r--r--   0 jborrow    (501) staff       (20)    14136 2023-07-06 15:41:16.000000 swiftsimio-7.0.1/tests/test_visualisation.py
```

### Comparing `swiftsimio-7.0.0/COPYING` & `swiftsimio-7.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/COPYING.LESSER` & `swiftsimio-7.0.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/PKG-INFO` & `swiftsimio-7.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftsimio
-Version: 7.0.0
+Version: 7.0.1
 Summary: SWIFTsim (swift.dur.ac.uk) i/o routines for python.
 Author-email: Josh Borrow <joshua.borrow@durham.ac.uk>
 Project-URL: Homepage, https://github.com/SWIFTSIM/swiftsimio
 Project-URL: Bug Tracker, https://github.com/SWIFTSIM/swiftsimio/issues
 Project-URL: Documentation, https://swiftsimio.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swiftsimio-7.0.0/README.md` & `swiftsimio-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/swiftsimio/__init__.py` & `swiftsimio-7.0.1/swiftsimio/__init__.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/swiftsimio/accelerated.py` & `swiftsimio-7.0.1/swiftsimio/accelerated.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/swiftsimio/conversions.py` & `swiftsimio-7.0.1/swiftsimio/conversions.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/swiftsimio/masks.py` & `swiftsimio-7.0.1/swiftsimio/masks.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/swiftsimio/objects.py` & `swiftsimio-7.0.1/swiftsimio/objects.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/swiftsimio/optional_packages.py` & `swiftsimio-7.0.1/swiftsimio/optional_packages.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/swiftsimio/reader.py` & `swiftsimio-7.0.1/swiftsimio/reader.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/swiftsimio/statistics.py` & `swiftsimio-7.0.1/swiftsimio/statistics.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/swiftsimio/subset_writer.py` & `swiftsimio-7.0.1/swiftsimio/subset_writer.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/swiftsimio/swiftsnap.py` & `swiftsimio-7.0.1/swiftsimio/swiftsnap.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/swiftsimio/units.py` & `swiftsimio-7.0.1/swiftsimio/units.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/swiftsimio/writer.py` & `swiftsimio-7.0.1/swiftsimio/writer.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/swiftsimio.egg-info/PKG-INFO` & `swiftsimio-7.0.1/swiftsimio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftsimio
-Version: 7.0.0
+Version: 7.0.1
 Summary: SWIFTsim (swift.dur.ac.uk) i/o routines for python.
 Author-email: Josh Borrow <joshua.borrow@durham.ac.uk>
 Project-URL: Homepage, https://github.com/SWIFTSIM/swiftsimio
 Project-URL: Bug Tracker, https://github.com/SWIFTSIM/swiftsimio/issues
 Project-URL: Documentation, https://swiftsimio.readthedocs.io/en/latest
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swiftsimio-7.0.0/tests/test_accelerated.py` & `swiftsimio-7.0.1/tests/test_accelerated.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_chunked_read_ranges.py` & `swiftsimio-7.0.1/tests/test_chunked_read_ranges.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_conversions.py` & `swiftsimio-7.0.1/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_cosmo_array.py` & `swiftsimio-7.0.1/tests/test_cosmo_array.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_cosmo_array_attrs.py` & `swiftsimio-7.0.1/tests/test_cosmo_array_attrs.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_data.py` & `swiftsimio-7.0.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_extraparts.py` & `swiftsimio-7.0.1/tests/test_extraparts.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_mask.py` & `swiftsimio-7.0.1/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_metadata.py` & `swiftsimio-7.0.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_read_ic.py` & `swiftsimio-7.0.1/tests/test_read_ic.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_rotate_visualisations.py` & `swiftsimio-7.0.1/tests/test_rotate_visualisations.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_rotation.py` & `swiftsimio-7.0.1/tests/test_rotation.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_smoothing_length_generation.py` & `swiftsimio-7.0.1/tests/test_smoothing_length_generation.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_vistools.py` & `swiftsimio-7.0.1/tests/test_vistools.py`

 * *Files identical despite different names*

### Comparing `swiftsimio-7.0.0/tests/test_visualisation.py` & `swiftsimio-7.0.1/tests/test_visualisation.py`

 * *Files identical despite different names*


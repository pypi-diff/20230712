# Comparing `tmp/pystac-1.8.1.tar.gz` & `tmp/pystac-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystac-1.8.1.tar", last modified: Fri Jun 30 16:52:37 2023, max compression
+gzip compressed data, was "pystac-1.8.2.tar", last modified: Wed Jul 12 20:22:47 2023, max compression
```

## Comparing `pystac-1.8.1.tar` & `pystac-1.8.2.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.025838 pystac-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-30 16:52:21.000000 pystac-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-30 16:52:21.000000 pystac-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-30 16:52:37.025838 pystac-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-30 16:52:21.000000 pystac-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-30 16:52:21.000000 pystac-1.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.013837 pystac-1.8.1/pystac/
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    46127 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    27635 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/common_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21024 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    22597 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/datacube.py
--rw-r--r--   0 runner    (1001) docker     (123)    24359 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/eo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/item_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    28917 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/mgrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    25804 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/raster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/sat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/scientific.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/extensions/xarray_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/html/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/html/JSON.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/html/Macros.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/html/jinja_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/item_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22077 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/link.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/media_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/rel_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/serialization/common_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/serialization/identify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/serialization/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16039 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/stac_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/stac_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/summaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/validation/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.021838 pystac-1.8.1/pystac/validation/jsonschemas/geojson/
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/geojson/Feature.json
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/geojson/Geometry.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.009837 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.025838 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/basics.json
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/catalog.json
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/collection.json
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/datetime.json
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/instrument.json
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/item.json
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/licensing.json
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/provider.json
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/local_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/schema_uri_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/validation/stac_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-30 16:52:21.000000 pystac-1.8.1/pystac/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:52:37.013837 pystac-1.8.1/pystac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-30 16:52:37.000000 pystac-1.8.1/pystac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-30 16:52:37.000000 pystac-1.8.1/pystac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:52:37.000000 pystac-1.8.1/pystac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-30 16:52:37.000000 pystac-1.8.1/pystac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 16:52:37.000000 pystac-1.8.1/pystac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:52:37.025838 pystac-1.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:47.440110 pystac-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-12 20:22:26.000000 pystac-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-12 20:22:26.000000 pystac-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-12 20:22:47.440110 pystac-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-12 20:22:26.000000 pystac-1.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-12 20:22:26.000000 pystac-1.8.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:47.412109 pystac-1.8.2/pystac/
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46127 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27635 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/common_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:47.428109 pystac-1.8.2/pystac/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21024 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22597 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/datacube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24359 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/eo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/item_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28917 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/mgrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25804 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/sat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/scientific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/extensions/xarray_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:47.428109 pystac-1.8.2/pystac/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/html/JSON.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/html/Macros.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/html/jinja_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/item_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22077 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/rel_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:47.432109 pystac-1.8.2/pystac/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/serialization/common_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/serialization/identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/serialization/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16039 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/stac_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/stac_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:47.432109 pystac-1.8.2/pystac/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24229 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/static/fields-normalized.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/summaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:47.432109 pystac-1.8.2/pystac/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:47.432109 pystac-1.8.2/pystac/validation/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:47.436109 pystac-1.8.2/pystac/validation/jsonschemas/geojson/
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/jsonschemas/geojson/Feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/jsonschemas/geojson/Geometry.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:47.404109 pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:47.440110 pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/basics.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/catalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/datetime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/instrument.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/item.json
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/licensing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/provider.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/local_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/schema_uri_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/validation/stac_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-12 20:22:26.000000 pystac-1.8.2/pystac/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:22:47.416109 pystac-1.8.2/pystac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-12 20:22:47.000000 pystac-1.8.2/pystac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-12 20:22:47.000000 pystac-1.8.2/pystac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:22:47.000000 pystac-1.8.2/pystac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-12 20:22:47.000000 pystac-1.8.2/pystac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 20:22:47.000000 pystac-1.8.2/pystac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 20:22:47.440110 pystac-1.8.2/setup.cfg
```

### Comparing `pystac-1.8.1/LICENSE` & `pystac-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/PKG-INFO` & `pystac-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac
-Version: 1.8.1
+Version: 1.8.2
 Summary: Python library for working with the SpatioTemporal Asset Catalog (STAC) specification
 Author-email: Rob Emanuele <rdemanuele@gmail.com>, Jon Duckworth <duckontheweb@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac
 Project-URL: documentation, https://pystac.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac.git
```

### Comparing `pystac-1.8.1/README.md` & `pystac-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pyproject.toml` & `pystac-1.8.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -60,25 +60,26 @@
     "mypy~=1.2",
     "orjson~=3.8",
     "pre-commit~=3.2",
     "pytest-cov~=4.0",
     "pytest-mock~=3.10",
     "pytest-recording~=0.12",
     "pytest~=7.3",
-    "ruff==0.0.275",
+    "ruff==0.0.277",
     "types-html5lib~=1.1",
     "types-orjson~=3.6",
     "types-python-dateutil~=2.8",
     "types-urllib3~=1.26",
     # pytest-recording breakage with v5.0.0, need release of
     # https://github.com/kiwicom/pytest-recording/pull/110 to remove this ceil
     "vcrpy<5",
 ]
 urllib3 = ["urllib3>=1.26"]
-validation = ["jsonschema>=4.0.1"]
+# jsonschema v4.18.2 breaks validation, and it feels safer to set a ceiling rather than just skip this version. The ceiling should be removed when the v4.18 lineage has settled down and feels safer.
+validation = ["jsonschema>=4.0.1,<4.18"]
 
 [project.urls]
 homepage = "https://github.com/stac-utils/pystac"
 documentation = "https://pystac.readthedocs.io"
 repository = "https://github.com/stac-utils/pystac.git"
 changelog = "https://github.com/stac-utils/pystac/blob/main/CHANGELOG.md"
 discussions = "https://github.com/radiantearth/stac-spec/discussions/categories/stac-software"
@@ -93,12 +94,15 @@
 [tool.ruff]
 line-length = 88
 select = ["E", "F", "I"]
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "error",
+    # Allows jsonschema's RefResolver deprecation warning through until we're
+    # updated to support jsonschema v4.18
+    "default::DeprecationWarning:pystac.validation.*"
 ]
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `pystac-1.8.1/pystac/__init__.py` & `pystac-1.8.2/pystac/__init__.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/asset.py` & `pystac-1.8.2/pystac/asset.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/cache.py` & `pystac-1.8.2/pystac/cache.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/catalog.py` & `pystac-1.8.2/pystac/catalog.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/collection.py` & `pystac-1.8.2/pystac/collection.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/common_metadata.py` & `pystac-1.8.2/pystac/common_metadata.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/errors.py` & `pystac-1.8.2/pystac/errors.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/base.py` & `pystac-1.8.2/pystac/extensions/base.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/classification.py` & `pystac-1.8.2/pystac/extensions/classification.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/datacube.py` & `pystac-1.8.2/pystac/extensions/datacube.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/eo.py` & `pystac-1.8.2/pystac/extensions/eo.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/file.py` & `pystac-1.8.2/pystac/extensions/file.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/grid.py` & `pystac-1.8.2/pystac/extensions/grid.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/hooks.py` & `pystac-1.8.2/pystac/extensions/hooks.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/item_assets.py` & `pystac-1.8.2/pystac/extensions/item_assets.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/label.py` & `pystac-1.8.2/pystac/extensions/label.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/mgrs.py` & `pystac-1.8.2/pystac/extensions/mgrs.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/pointcloud.py` & `pystac-1.8.2/pystac/extensions/pointcloud.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/projection.py` & `pystac-1.8.2/pystac/extensions/projection.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/raster.py` & `pystac-1.8.2/pystac/extensions/raster.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/sar.py` & `pystac-1.8.2/pystac/extensions/sar.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/sat.py` & `pystac-1.8.2/pystac/extensions/sat.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/scientific.py` & `pystac-1.8.2/pystac/extensions/scientific.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/storage.py` & `pystac-1.8.2/pystac/extensions/storage.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/table.py` & `pystac-1.8.2/pystac/extensions/table.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/timestamps.py` & `pystac-1.8.2/pystac/extensions/timestamps.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/version.py` & `pystac-1.8.2/pystac/extensions/version.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/view.py` & `pystac-1.8.2/pystac/extensions/view.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/extensions/xarray_assets.py` & `pystac-1.8.2/pystac/extensions/xarray_assets.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/html/JSON.jinja2` & `pystac-1.8.2/pystac/html/JSON.jinja2`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/html/Macros.jinja2` & `pystac-1.8.2/pystac/html/Macros.jinja2`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/item.py` & `pystac-1.8.2/pystac/item.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/item_collection.py` & `pystac-1.8.2/pystac/item_collection.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/layout.py` & `pystac-1.8.2/pystac/layout.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/link.py` & `pystac-1.8.2/pystac/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from copy import copy
 from html import escape
 from typing import TYPE_CHECKING, Any, Dict, Optional, Type, TypeVar, Union
 
 import pystac
 from pystac.html.jinja_env import get_jinja_env
 from pystac.utils import (
-    HREF,
+    HREF as HREF,
+)
+from pystac.utils import (
     is_absolute_href,
     make_absolute_href,
     make_posix_style,
     make_relative_href,
 )
 
 if TYPE_CHECKING:
```

### Comparing `pystac-1.8.1/pystac/media_type.py` & `pystac-1.8.2/pystac/media_type.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/provider.py` & `pystac-1.8.2/pystac/provider.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/rel_type.py` & `pystac-1.8.2/pystac/rel_type.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/serialization/common_properties.py` & `pystac-1.8.2/pystac/serialization/common_properties.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/serialization/identify.py` & `pystac-1.8.2/pystac/serialization/identify.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/serialization/migrate.py` & `pystac-1.8.2/pystac/serialization/migrate.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/stac_io.py` & `pystac-1.8.2/pystac/stac_io.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/stac_object.py` & `pystac-1.8.2/pystac/stac_object.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/summaries.py` & `pystac-1.8.2/pystac/summaries.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/utils.py` & `pystac-1.8.2/pystac/utils.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/validation/__init__.py` & `pystac-1.8.2/pystac/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/validation/jsonschemas/geojson/Feature.json` & `pystac-1.8.2/pystac/validation/jsonschemas/geojson/Feature.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/validation/jsonschemas/geojson/Geometry.json` & `pystac-1.8.2/pystac/validation/jsonschemas/geojson/Geometry.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/basics.json` & `pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/basics.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/catalog.json` & `pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/catalog.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/collection.json` & `pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/collection.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/datetime.json` & `pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/datetime.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/instrument.json` & `pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/instrument.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/item.json` & `pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/item.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/validation/jsonschemas/stac-spec/v1.0.0/provider.json` & `pystac-1.8.2/pystac/validation/jsonschemas/stac-spec/v1.0.0/provider.json`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/validation/local_validator.py` & `pystac-1.8.2/pystac/validation/local_validator.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/validation/schema_uri_map.py` & `pystac-1.8.2/pystac/validation/schema_uri_map.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/validation/stac_validator.py` & `pystac-1.8.2/pystac/validation/stac_validator.py`

 * *Files identical despite different names*

### Comparing `pystac-1.8.1/pystac/version.py` & `pystac-1.8.2/pystac/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from typing import Optional
 
-__version__ = "1.8.1"
+__version__ = "1.8.2"
 """Library version"""
 
 
 class STACVersion:
     DEFAULT_STAC_VERSION = "1.0.0"
     """Latest STAC version supported by PySTAC"""
```

### Comparing `pystac-1.8.1/pystac.egg-info/PKG-INFO` & `pystac-1.8.2/pystac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac
-Version: 1.8.1
+Version: 1.8.2
 Summary: Python library for working with the SpatioTemporal Asset Catalog (STAC) specification
 Author-email: Rob Emanuele <rdemanuele@gmail.com>, Jon Duckworth <duckontheweb@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac
 Project-URL: documentation, https://pystac.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac.git
```

### Comparing `pystac-1.8.1/pystac.egg-info/SOURCES.txt` & `pystac-1.8.2/pystac.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 pystac/html/__init__.py
 pystac/html/jinja_env.py
 pystac/serialization/__init__.py
 pystac/serialization/common_properties.py
 pystac/serialization/identify.py
 pystac/serialization/migrate.py
 pystac/static/__init__.py
+pystac/static/fields-normalized.json
 pystac/validation/__init__.py
 pystac/validation/local_validator.py
 pystac/validation/schema_uri_map.py
 pystac/validation/stac_validator.py
 pystac/validation/jsonschemas/__init__.py
 pystac/validation/jsonschemas/geojson/Feature.json
 pystac/validation/jsonschemas/geojson/Geometry.json
```

### Comparing `pystac-1.8.1/pystac.egg-info/requires.txt` & `pystac-1.8.2/pystac.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 mypy~=1.2
 orjson~=3.8
 pre-commit~=3.2
 pytest-cov~=4.0
 pytest-mock~=3.10
 pytest-recording~=0.12
 pytest~=7.3
-ruff==0.0.275
+ruff==0.0.277
 types-html5lib~=1.1
 types-orjson~=3.6
 types-python-dateutil~=2.8
 types-urllib3~=1.26
 vcrpy<5
 
 [urllib3]
 urllib3>=1.26
 
 [validation]
-jsonschema>=4.0.1
+jsonschema<4.18,>=4.0.1
```


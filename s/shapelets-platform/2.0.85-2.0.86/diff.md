# Comparing `tmp/shapelets-platform-2.0.85.tar.gz` & `tmp/shapelets-platform-2.0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapelets-platform-2.0.85.tar", last modified: Thu Jun  8 11:01:24 2023, max compression
+gzip compressed data, was "shapelets-platform-2.0.86.tar", last modified: Wed Jul 12 16:17:26 2023, max compression
```

## Comparing `shapelets-platform-2.0.85.tar` & `shapelets-platform-2.0.86.tar`

### file list

```diff
@@ -1,295 +1,295 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.116513 shapelets-platform-2.0.85/
--rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/COPYING.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-06-08 11:01:24.116513 shapelets-platform-2.0.85/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/noxfile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)     3068 2023-06-08 11:01:24.116513 shapelets-platform-2.0.85/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     4030 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.020513 shapelets-platform-2.0.85/src/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.028513 shapelets-platform-2.0.85/src/shapelets/
--rw-r--r--   0 vsts      (1001) docker     (123)      891 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8472 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19249 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/_cli.py
--rw-r--r--   0 vsts      (1001) docker     (123)    51403 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/_relations.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/_uom.py
--rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-06-08 11:01:20.000000 shapelets-platform-2.0.85/src/shapelets/_version.py
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/_version.pyi
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.028513 shapelets-platform-2.0.85/src/shapelets/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    68076 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/data_app.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/data_app_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.032513 shapelets-platform-2.0.85/src/shapelets/apps/widgets/
--rw-r--r--   0 vsts      (1001) docker     (123)      752 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3123 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/attribute_names.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.036513 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/
--rw-r--r--   0 vsts      (1001) docker     (123)      744 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3273 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/altair_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/bar_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2602 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/folium_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2500 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/heatmap.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1705 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/histogram.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19053 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/line_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/pie_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/plotly_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2039 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/polar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/radar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4186 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/scatter_plot.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.036513 shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/
--rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/filtering_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1106 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/metadata_field.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/metadata_filter.py
--rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/temporal_context.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.044513 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/
--rw-r--r--   0 vsts      (1001) docker     (123)     1357 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1996 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/button.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4503 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/checkbox.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2151 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/collection_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7465 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8050 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/datetime_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4164 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/gauge.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8263 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/image.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5978 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/metric.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2022 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11087 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/number_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7391 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/progress.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9880 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/radio_group.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.044513 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/resources/
--rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
--rw-r--r--   0 vsts      (1001) docker     (123)     4678 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/ring.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10639 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1818 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/sequence_list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1843 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14796 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/slider.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8253 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/text.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9070 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/text_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/timer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/datetime_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.048513 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/
--rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/grid_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6057 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/horizontal_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/panel.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/tabs_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5683 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/vertical_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2756 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    24284 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/widget.py
--rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/iris.csv
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.052513 shapelets-platform-2.0.85/src/shapelets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)     1463 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1084 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/altair.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1523 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/capsule.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4487 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/collection.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4297 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/dataframe.py
--rw-r--r--   0 vsts      (1001) docker     (123)      260 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3472 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/function_description.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2625 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/function_parameter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1252 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/group.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2214 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/image.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4992 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/metadata_item.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2749 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2666 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/ndarray.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2360 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/permissions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/replicated_param.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5553 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/sequence.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2292 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/sequence_axis.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1869 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/user.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4446 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/view_match.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.052513 shapelets-platform-2.0.85/src/shapelets/svr/
--rw-r--r--   0 vsts      (1001) docker     (123)    10262 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/app.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.056513 shapelets-platform-2.0.85/src/shapelets/svr/authn/
--rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8820 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/authhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9843 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/authrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9665 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/authservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/gc_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2162 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/iauthrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8976 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/iauthservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.056513 shapelets-platform-2.0.85/src/shapelets/svr/data/
--rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.060513 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/
--rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/access_token_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/azure_gen1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/azure_gen2.py
--rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/driver.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/dynamic_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_vfs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/ftp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/local.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/protocols.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/smb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/vfs_sample_config.toml
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.064513 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/
--rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3116 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataapps_ws.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9309 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataappshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    25604 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2439 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataappsservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1781 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/idataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1507 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/idataappsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.068513 shapelets-platform-2.0.85/src/shapelets/svr/db/
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.068513 shapelets-platform-2.0.85/src/shapelets/svr/db/native/
--rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/native/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/native/database.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/native/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/schema_builder.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3449 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v3.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5579 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v4.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2021 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/setup.py
--rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/docs.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.068513 shapelets-platform-2.0.85/src/shapelets/svr/execution/
--rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1710 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/executionhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/executionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1854 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/executionservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/iexecutionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/iexecutionservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.072513 shapelets-platform-2.0.85/src/shapelets/svr/groups/
--rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1596 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/groupservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4374 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/groupshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4754 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/groupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1968 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/igroupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2626 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/igroupsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.072513 shapelets-platform-2.0.85/src/shapelets/svr/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      369 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      826 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/model/dataapps.py
--rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/model/function.py
--rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/model/groups.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/model/principals.py
--rw-r--r--   0 vsts      (1001) docker     (123)      867 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/model/users.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.080513 shapelets-platform-2.0.85/src/shapelets/svr/mustang/
--rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/asttranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/conversions.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12907 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/core.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/decompiling.py
--rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/hashdict.py
--rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/identifier.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/ormtypes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.080513 shapelets-platform-2.0.85/src/shapelets/svr/mustang/prototypes/
--rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/prototypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/python_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/serialization.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/sqlbuilding.py
--rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/sqltranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4102 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/server.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.084513 shapelets-platform-2.0.85/src/shapelets/svr/settings/
--rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/defaults.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/http.py
--rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/reload.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/server.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/settings.toml
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/ssl.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/telemetry.py
--rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.084513 shapelets-platform-2.0.85/src/shapelets/svr/telemetry/
--rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/telemetry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/telemetry/itelemetryservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/telemetry/sysinfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/telemetry/telemetryservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.088513 shapelets-platform-2.0.85/src/shapelets/svr/users/
--rw-r--r--   0 vsts      (1001) docker     (123)      685 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/iusersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2653 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/iusersservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5587 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/usershttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13629 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/usersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3582 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/usersservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.092513 shapelets-platform-2.0.85/src/shapelets/svr/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/utils/crypto.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/utils/flexbytes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.092513 shapelets-platform-2.0.85/src/shapelets/svr/www/
--rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/altair.json
--rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/asset-manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/dataapp.json
--rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/favicon.ico
--rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/index.html
--rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/robots.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.020513 shapelets-platform-2.0.85/src/shapelets/svr/www/static/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.096513 shapelets-platform-2.0.85/src/shapelets/svr/www/static/css/
--rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
--rw-r--r--   0 vsts      (1001) docker     (123)    79553 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/css/main.8349d999.chunk.css
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.104513 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/
--rw-r--r--   0 vsts      (1001) docker     (123)  6284390 2023-06-08 11:01:19.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   173518 2023-06-08 11:01:19.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/4.77242983.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/4.77242983.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   813635 2023-06-08 11:01:19.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/main.83b9aa07.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/runtime-main.fd20aea3.js
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.112513 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/
--rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/audit.cb539a06.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/bin.7e762965.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/clear.27b15301.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/download-image.87310709.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/filter.cec803b8.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
--rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
--rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logout.57c593a5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/share.bc9a8370.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
--rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
--rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/systemd_template.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.116513 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-06-08 11:01:20.000000 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)    11406 2023-06-08 11:01:23.000000 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-08 11:01:20.000000 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-06-08 11:01:20.000000 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)     1305 2023-06-08 11:01:20.000000 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-06-08 11:01:20.000000 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.444218 shapelets-platform-2.0.86/
+-rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/COPYING.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-07-12 16:17:26.444218 shapelets-platform-2.0.86/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/noxfile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)     3069 2023-07-12 16:17:26.444218 shapelets-platform-2.0.86/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     4030 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.332217 shapelets-platform-2.0.86/src/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.340217 shapelets-platform-2.0.86/src/shapelets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      924 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8739 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19249 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    51403 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/_relations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/_uom.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-07-12 16:17:22.000000 shapelets-platform-2.0.86/src/shapelets/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/_version.pyi
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.340217 shapelets-platform-2.0.86/src/shapelets/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    68871 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/data_app.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/data_app_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.344217 shapelets-platform-2.0.86/src/shapelets/apps/widgets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      752 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3150 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/attribute_names.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.348217 shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      744 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3273 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/altair_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/bar_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2602 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/folium_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2500 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/heatmap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1705 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/histogram.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19053 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/line_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/pie_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/plotly_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2039 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/polar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/radar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4186 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/scatter_plot.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.348217 shapelets-platform-2.0.86/src/shapelets/apps/widgets/contexts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/contexts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/contexts/filtering_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1106 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/contexts/metadata_field.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/contexts/metadata_filter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/contexts/temporal_context.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.360217 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1357 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1996 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/button.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4503 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/checkbox.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2151 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/collection_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7578 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8196 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/datetime_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4164 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/gauge.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8263 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/image.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5978 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/metric.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2022 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11087 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/number_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7391 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9880 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/radio_group.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.360217 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/resources/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
+-rw-r--r--   0 vsts      (1001) docker     (123)     4678 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/ring.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10639 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1818 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/sequence_list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1843 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14789 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/slider.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9255 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/text.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9070 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/text_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/timer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/datetime_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.360217 shapelets-platform-2.0.86/src/shapelets/apps/widgets/layouts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/layouts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/layouts/grid_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6057 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/layouts/horizontal_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/layouts/panel.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/layouts/tabs_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5683 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/layouts/vertical_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2756 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    26073 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/apps/widgets/widget.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/iris.csv
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.368217 shapelets-platform-2.0.86/src/shapelets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1463 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1084 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/altair.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1523 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/capsule.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4487 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4297 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/dataframe.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      260 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3472 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/function_description.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2625 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/function_parameter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1252 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/group.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2214 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/image.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4992 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/metadata_item.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2749 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2666 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/ndarray.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2360 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/permissions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/replicated_param.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5553 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/sequence.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2292 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/sequence_axis.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1869 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/user.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4446 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/model/view_match.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.372217 shapelets-platform-2.0.86/src/shapelets/svr/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10262 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/app.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.376217 shapelets-platform-2.0.86/src/shapelets/svr/authn/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/authn/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8820 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/authn/authhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10269 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/authn/authrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9665 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/authn/authservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/authn/gc_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2162 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/authn/iauthrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8976 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/authn/iauthservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.376217 shapelets-platform-2.0.86/src/shapelets/svr/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.380217 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/access_token_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/azure_gen1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/azure_gen2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/driver.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/dynamic_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/fsspec_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/fsspec_vfs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/ftp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/local.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/smb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/vfs_sample_config.toml
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.384217 shapelets-platform-2.0.86/src/shapelets/svr/dataapps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/dataapps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3116 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/dataapps/dataapps_ws.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9536 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/dataapps/dataappshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    25885 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/dataapps/dataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2407 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/dataapps/dataappsservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/dataapps/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1781 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/dataapps/idataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1507 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/dataapps/idataappsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.384217 shapelets-platform-2.0.86/src/shapelets/svr/db/
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.388218 shapelets-platform-2.0.86/src/shapelets/svr/db/native/
+-rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/db/native/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/db/native/database.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/db/native/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/db/schema_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3449 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/db/schema_v1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/db/schema_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/db/schema_v3.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5579 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/db/schema_v4.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2021 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/db/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/docs.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.388218 shapelets-platform-2.0.86/src/shapelets/svr/execution/
+-rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/execution/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1710 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/execution/executionhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/execution/executionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2088 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/execution/executionservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/execution/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/execution/iexecutionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/execution/iexecutionservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.392217 shapelets-platform-2.0.86/src/shapelets/svr/groups/
+-rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/groups/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1603 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/groups/groupservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4392 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/groups/groupshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4951 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/groups/groupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/groups/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/groups/igroupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2633 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/groups/igroupsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.396218 shapelets-platform-2.0.86/src/shapelets/svr/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      369 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      826 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/model/dataapps.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/model/function.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/model/groups.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/model/principals.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      867 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/model/users.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.408218 shapelets-platform-2.0.86/src/shapelets/svr/mustang/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/asttranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12907 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/core.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/decompiling.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/hashdict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/identifier.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/ormtypes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.408218 shapelets-platform-2.0.86/src/shapelets/svr/mustang/prototypes/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/prototypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/python_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/sqlbuilding.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/mustang/sqltranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4102 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/server.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.412218 shapelets-platform-2.0.86/src/shapelets/svr/settings/
+-rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/settings/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/settings/client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/settings/defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/settings/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/settings/http.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/settings/reload.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/settings/server.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/settings/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/settings/settings.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/settings/ssl.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/settings/telemetry.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/settings/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.416218 shapelets-platform-2.0.86/src/shapelets/svr/telemetry/
+-rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/telemetry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/telemetry/itelemetryservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/telemetry/sysinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/telemetry/telemetryservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.416218 shapelets-platform-2.0.86/src/shapelets/svr/users/
+-rw-r--r--   0 vsts      (1001) docker     (123)      685 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/users/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/users/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/users/iusersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2653 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/users/iusersservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5587 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/users/usershttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13629 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/users/usersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3582 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/users/usersservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.420218 shapelets-platform-2.0.86/src/shapelets/svr/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/utils/crypto.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/svr/utils/flexbytes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.420218 shapelets-platform-2.0.86/src/shapelets/svr/www/
+-rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/altair.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/asset-manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/dataapp.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/favicon.ico
+-rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/index.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/robots.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.332217 shapelets-platform-2.0.86/src/shapelets/svr/www/static/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.420218 shapelets-platform-2.0.86/src/shapelets/svr/www/static/css/
+-rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
+-rw-r--r--   0 vsts      (1001) docker     (123)    79553 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/css/main.8349d999.chunk.css
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.432218 shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/
+-rw-r--r--   0 vsts      (1001) docker     (123)  6284390 2023-07-12 16:17:22.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   173518 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/4.77242983.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/4.77242983.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   813635 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/main.83b9aa07.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/runtime-main.fd20aea3.js
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.440218 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/
+-rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/audit.cb539a06.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/bin.7e762965.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/clear.27b15301.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/download-image.87310709.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/filter.cec803b8.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/logout.57c593a5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/share.bc9a8370.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-07-12 16:17:21.000000 shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
+-rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-07-12 16:00:01.000000 shapelets-platform-2.0.86/src/shapelets/systemd_template.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-12 16:17:26.444218 shapelets-platform-2.0.86/src/shapelets_platform.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-07-12 16:17:23.000000 shapelets-platform-2.0.86/src/shapelets_platform.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)    11406 2023-07-12 16:17:26.000000 shapelets-platform-2.0.86/src/shapelets_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-12 16:17:23.000000 shapelets-platform-2.0.86/src/shapelets_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-07-12 16:17:23.000000 shapelets-platform-2.0.86/src/shapelets_platform.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     1306 2023-07-12 16:17:23.000000 shapelets-platform-2.0.86/src/shapelets_platform.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-07-12 16:17:23.000000 shapelets-platform-2.0.86/src/shapelets_platform.egg-info/top_level.txt
```

### Comparing `shapelets-platform-2.0.85/LICENSE.md` & `shapelets-platform-2.0.86/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/PKG-INFO` & `shapelets-platform-2.0.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.85
+Version: 2.0.86
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
```

### Comparing `shapelets-platform-2.0.85/README.md` & `shapelets-platform-2.0.86/README.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/noxfile.py` & `shapelets-platform-2.0.86/noxfile.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/pyproject.toml` & `shapelets-platform-2.0.86/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/setup.cfg` & `shapelets-platform-2.0.86/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -51,20 +51,20 @@
 	matplotlib >= 3.5.3
 	mypy ~= 0.990
 	numpy >=1.21.6
 	pandas >=1.3.5
 	psutil >= 5.9.2
 	pyarrow >=12.0.0
 	py-cpuinfo>=9.0.0
-	pydantic >= 1.10.2
+	pydantic == 1.10.11
 	pygeohash >= 1.2.0
 	PyNaCl >= 1.5.0
 	requests >= 2.28.1
 	setuptools-scm >= 7.1.0
-	shapelets_native == 2.0.85
+	shapelets_native == 2.0.86
 	tabulate>=0.8.10
 	tomlkit >= 0.11.4
 	tqdm >= 4.64.1
 	typing_extensions >= 4.6.2
 	uvicorn >= 0.18.3
 	vega-datasets >= 0.9
 	websocket-client >= 1.5.2
```

### Comparing `shapelets-platform-2.0.85/setup.py` & `shapelets-platform-2.0.86/setup.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 from ._relations import DataSet, CSVCompression, SandBox, sandbox, ParquetCodec
 from ._cli import cli
 from ._api import (
     add_user_to_group,
     create_group,
+    delete_group,
     forget_me,
     list_current_groups,
     list_current_users,
     login,
     register,
     remove_user_from_group,
     unregister
@@ -20,10 +21,10 @@
 from . import _uom
 
 svr.get_service(svr.ITelemetryService).library_loaded()
 
 __all__ = ["__version__", "svr", "apps"]
 __all__ += ["cli"]
 __all__ += ['DataSet', 'CSVCompression', 'SandBox', 'sandbox', 'ParquetCodec', 'functions']
-__all__ += ['add_user_to_group', 'create_group', 'forget_me', 'list_current_groups', 'list_current_users',
+__all__ += ['add_user_to_group', 'create_group', 'delete_group' 'forget_me', 'list_current_groups', 'list_current_users',
             'login', 'register', 'remove_user_from_group', 'unregister']
 __all__ += _uom.__all__
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/_api.py` & `shapelets-platform-2.0.86/src/shapelets/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,27 @@
     description: str, optional
         Group description.
     """
     groups_svc = get_service(IGroupsService)
     return groups_svc.create(group_name, description)
 
 
+def delete_group(group_name: str) -> str:
+    """
+    Delete a group from Shapelets
+
+    Parameters
+    ----------
+    group_name: str, required
+        Group name.
+    """
+    groups_svc = get_service(IGroupsService)
+    return groups_svc.delete_group(group_name)
+
+
 def add_user_to_group(user_name: str, groups: Union[List[str], str], write: bool = False):
     """
     Add a Shapelets user to an existed group
 
     Parameters
     ----------
     user_name: str, required
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/_cli.py` & `shapelets-platform-2.0.86/src/shapelets/_cli.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/_relations.py` & `shapelets-platform-2.0.86/src/shapelets/_relations.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/_uom.py` & `shapelets-platform-2.0.86/src/shapelets/_uom.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/data_app.py` & `shapelets-platform-2.0.86/src/shapelets/apps/data_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,25 @@
         self.title = name
         self.temporal_contexts = []
         self.filtering_contexts = []
         self.functions = {}
         self.groups = None
         self._data = []
 
+    def _update_data(self, data: List[str]):
+        from ..svr.dataapps.dataappsrepo import _add_data, _load_dataapp_by_name_and_version
+        from ..svr.db import transaction
+        """
+        Update data info belonging to the dataApp to keep track of what files belong to each dataApp. This allows us
+        to do a correct cleaning once the dataApp is deleted.
+        """
+        with transaction() as conn:
+           uid = _load_dataapp_by_name_and_version(self.name, self.version[0], self.version[1], conn).uid
+           _add_data(uid, data, conn)
+
     def register(self, groups: Optional[Union[List[str], str]] = None):
         """
         Registers the DataApp.
 
         Parameters
         ----------
         groups : List[str], str, optional
@@ -1699,14 +1710,15 @@
                               parent_data_app=self, **additional)
 
     def table(self,
               data: Union[pd.DataFrame, DataSet] = None,
               rows_per_page: Optional[int] = None,
               tools_visible: Optional[bool] = None,
               conditional_formats: Optional[List[Union[Condition, dict]]] = None,
+              date_format: Optional[str] = None,
               **additional):
         """
         Displays rows of data.
 
         Parameters
         ----------
         data : Dataset or pd.Dataframe, optional
@@ -1739,14 +1751,16 @@
               "conditions": [
                 { "value": "Peligro", "backcolor": "#ff0000", "color": "#ffffff" },
                 { "value": "Precaución", "backcolor": "#000077", "color": "#ffffff" },
                 { "value": "OK", "backcolor": "#00aa00", "color": "#ffffff" }
               ]
             }
 
+        date_format: str, Optional
+            If a column has a type timestamp, a format could be provided to trasnform the date.
 
         Returns
         -------
         Table
 
         Examples
         --------
@@ -1775,15 +1789,16 @@
             * Shapelets Dataset
             * Pandas DataFrame
             * list
             * :func:`~shapelets.apps.DataApp.table`
 
         """
         return TableWidget(data=data, rows_per_page=rows_per_page, tools_visible=tools_visible,
-                           conditional_formats=conditional_formats, parent_data_app=self, **additional)
+                           conditional_formats=conditional_formats, parent_data_app=self, date_format=date_format,
+                           **additional)
 
     def gauge(self,
               title: Optional[str] = None,
               value: Optional[Union[int, float]] = None,
               **additional) -> GaugeWidget:
         """
         Creates a Gauge.
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/data_app_utils.py` & `shapelets-platform-2.0.86/src/shapelets/apps/data_app_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/attribute_names.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/attribute_names.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     CAPTION = "caption"
     CATEGORIES = "categories"
     CHECKED = "checked"
     COLLECTION_ID = "collectionId"
     COLLECTION_LABEL = "collectionLabel"
     COLUMN = "column"
     COLS = "cols"
+    COL_TYPES = "colTypes"
     COL_OFFSET = "colOffset"
     COL_SPAN = "colSpan"
     COLOR = "color"
     CONDITION = "condition"
     CONDITIONAL_FORMATS = "conditionalFormats"
     CUMULATIVE = "cumulative"
     DATA = "data"
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/altair_chart.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/altair_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/bar_chart.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/folium_chart.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/folium_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/heatmap.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/heatmap.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/histogram.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/histogram.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/line_chart.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/pie_chart.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/plotly_chart.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/polar_area.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/polar_area.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/radar_area.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/radar_area.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/scatter_plot.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/charts/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/filtering_context.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/contexts/filtering_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/metadata_field.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/contexts/metadata_field.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/metadata_filter.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/contexts/metadata_filter.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/temporal_context.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/contexts/temporal_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/button.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/button.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/checkbox.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/checkbox.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/collection_selector.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/collection_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/datetime_range_selector.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/datetime_range_selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,14 +140,19 @@
                 AttributeNames.START_DATE.value: self._start_datetime_str
             })
 
         if self.end_datetime is not None:
             date_dict[AttributeNames.PROPERTIES.value].update({
                 AttributeNames.END_DATE.value: self._end_datetime_str
             })
+        # Add props.value too as list to set the initial state value in the UI
+        if self.start_datetime is not None and self.end_datetime is not None:
+            date_dict[AttributeNames.PROPERTIES.value].update({
+                AttributeNames.VALUE.value: [self._start_datetime_str, self._end_datetime_str]
+            })
 
         if self._format is not None:
             date_dict[AttributeNames.PROPERTIES.value].update({
                 AttributeNames.FORMAT.value: self._format
             })
 
         if self.min_datetime is not None:
@@ -166,29 +171,26 @@
         return date_dict
 
 
 class DatetimeRangeSelectorWidget(DateRangeSelector, Widget):
 
     def __init__(self,
                  title: Optional[str] = None,
-                 start_datetime: Optional[Union[float, int, str, datetime, date, time]] = None,
-                 end_datetime: Optional[Union[float, int, str, datetime, date, time]] = None,
-                 min_datetime: Optional[Union[float, int, str, date, time]] = None,
-                 max_datetime: Optional[Union[float, int, str, date, time]] = None,
+                 start_datetime: Optional[Union[int, str, datetime, date, time]] = None,
+                 end_datetime: Optional[Union[int, str, datetime, date, time]] = None,
+                 min_datetime: Optional[Union[int, str, date, time]] = None,
+                 max_datetime: Optional[Union[int, str, date, time]] = None,
                  **additional):
         Widget.__init__(self,
                         DateRangeSelector.__name__,
                         compatibility=tuple(
                             [
                                 DateRangeSelector.__name__,
-                                float.__name__,
-                                str.__name__,
-                                datetime.__name__,
-                                date.__name__,
-                                time.__name__
+                                tuple.__name__
+
                             ]
                         ),
                         **additional)
         DateRangeSelector.__init__(self,
                                    title=title,
                                    start_datetime=start_datetime,
                                    end_datetime=end_datetime,
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/datetime_selector.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/datetime_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,18 @@
         self.date_time = dt
         return self
 
     def from_time(self, dt: time) -> DateSelector:
         self.date_time = dt
         return self
 
+    def from_string(self, dt: str) -> DateSelector:
+        self._date_time_str, self._format = _transform_date_time_value(dt)
+        return dt
+
     def to_string(self) -> str:
         if isinstance(self.date_time, str):
             return self.date_time
 
         if isinstance(self.date_time, datetime):
             date_str = self.date_time.strftime("%Y-%m-%d, %H:%M:%S")
             return date_str
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/gauge.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/gauge.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/image.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/image.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/list.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/list.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/metric.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/metric.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/number_input.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/number_input.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/progress.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/progress.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/radio_group.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/radio_group.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/ring.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/ring.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/selector.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/sequence_list.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/sequence_list.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/sequence_selector.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/sequence_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/slider.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/slider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import uuid
 
 from dataclasses import dataclass
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Union
 
 from ..widget import AttributeNames, StateControl, Widget
 
 
 @dataclass
 class Slider(StateControl):
     """
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/table.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,26 +29,29 @@
 
 @dataclass
 class Table(StateControl):
     data: Optional[Union[pd.DataFrame, sh.DataSet]] = None
     rows_per_page: Optional[int] = None
     tools_visible: Optional[bool] = None
     conditional_formats: Optional[List[Union[Condition, dict]]] = None
+    date_format: Optional[str] = None
 
     def __post_init__(self):
         if not hasattr(self, "widget_id"):
             self.widget_id = str(uuid.uuid1())
 
     def replace_widget(self, new_widget: Table):
         """
         Replace the current values of the widget for the values of a similar widget type.
         """
         self.data = new_widget.data
         self.rows_per_page = new_widget.rows_per_page
         self.tools_visible = new_widget.tools_visible
+        self.conditional_formats = new_widget.conditional_formats
+        self.date_format = new_widget.date_format
 
     def get_current_value(self):
         """
         Return the current value of the widget. Return None is the widget value is not set.
         """
         if self.data is not None:
             return self.data
@@ -155,14 +158,22 @@
                                     col_dict["conditionalType"] = condition.type
                                     col_dict["conditions"] = condition.conditions
                         cols.append(col_dict)
 
                     table_dict[AttributeNames.PROPERTIES.value].update({
                         AttributeNames.COLS.value: cols
                     })
+                if isinstance(self.data, pd.DataFrame):
+                    table_dict[AttributeNames.PROPERTIES.value].update({
+                        AttributeNames.COL_TYPES.value: [str(x) for x in self.data.dtypes]
+                    })
+                elif isinstance(self.data, sh.DataSet):
+                    table_dict[AttributeNames.PROPERTIES.value].update({
+                        AttributeNames.COL_TYPES.value: [str(x) for x in self.data.describe().column_type]
+                    })
 
             else:
                 raise ValueError("Data type not supported")
 
         if self.rows_per_page is not None:
             if isinstance(self.rows_per_page, int):
                 table_dict[AttributeNames.PROPERTIES.value].update({
@@ -171,34 +182,42 @@
 
         if self.tools_visible is not None:
             if isinstance(self.tools_visible, int):
                 table_dict[AttributeNames.PROPERTIES.value].update({
                     AttributeNames.TOOLS_VISIBLE.value: self.tools_visible
                 })
 
+        if self.date_format is not None:
+            if isinstance(self.date_format, str):
+                table_dict[AttributeNames.PROPERTIES.value].update({
+                    AttributeNames.FORMAT.value: self.date_format
+                })
+
         return table_dict
 
 
 class TableWidget(Table, Widget):
 
     def __init__(self,
                  data: Optional[Union[pd.DataFrame, sh.DataSet]] = None,
                  rows_per_page: Optional[int] = None,
                  tools_visible: Optional[bool] = None,
                  conditional_formats: Optional[List[Union[Condition, dict]]] = None,
+                 date_format: Optional[str] = None,
                  **additional):
         Widget.__init__(self, Table.__name__,
                         compatibility=tuple(
                             [pd.DataFrame.__name__, np.ndarray.__name__, list.__name__, Table.__name__]),
                         **additional)
         Table.__init__(self,
                        data=data,
                        rows_per_page=rows_per_page,
                        tools_visible=tools_visible,
-                       conditional_formats=conditional_formats)
+                       conditional_formats=conditional_formats,
+                       date_format=date_format)
         self._parent_class = Table.__name__
         self._compatibility: Tuple = (pd.DataFrame.__name__,
                                       np.ndarray.__name__,
                                       list.__name__,
                                       Table.__name__,
                                       sh.DataSet.__name__)
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/text.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/text.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/text_input.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/text_input.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/timer.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/controllers/timer.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/datetime_utils.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/grid_layout.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/layouts/grid_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/horizontal_layout.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/layouts/horizontal_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/panel.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/layouts/panel.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/tabs_layout.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/layouts/tabs_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/vertical_layout.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/layouts/vertical_layout.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/util.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/util.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/apps/widgets/widget.py` & `shapelets-platform-2.0.86/src/shapelets/apps/widgets/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 from typing_extensions import get_args
 
 from .attribute_names import AttributeNames
 
 import __main__
 import sys
 
+import os
+
+SH_DIR = os.path.expanduser('~/.shapelets')
+DATA_DIR = os.path.join(SH_DIR, 'data')
+
 
 class Widget:
     """
     Units defined in Layout
     """
 
     def __init__(self,
@@ -232,22 +237,24 @@
                             "mute") else on_changes_widgets.append(arguments.widget_id)
 
                     references.append(
                         {
                             "ref": arguments.widget_id,
                             "name": entry_arguments[i]["name"],
                             "type": entry_arguments[i]["type"],
+                            "default": entry_arguments[i]["default"],
                         }
                     )
                 else:
                     references.append(
                         {
                             "value": str(base64.b64encode(dill.dumps(arguments, recurse=True)), encoding='utf-8'),
                             "name": entry_arguments[i]["name"],
                             "type": entry_arguments[i]["type"],
+                            "default": entry_arguments[i]["default"],
                             "pickled": True
                         }
                     )
 
             # Get widgets from Triggers
             triggers = self._find_triggers(kwargs)
             on_changes_widgets.extend(triggers)
@@ -255,35 +262,54 @@
             wrong_widgets = self._intersection(mute_widgets, on_changes_widgets)
             # Get only well defined triggers
             on_changes_widgets = [trigger for trigger in on_changes_widgets if trigger not in wrong_widgets]
 
             # We need to check if there is another function already in the bind attribute in order to avoid looping with triggers
             if on_changes_widgets and len(self._bind) > 0:
                 self._check_triggers(on_changes_widgets)
-            # Add to Widget Structure
-            self._add_bind_to_widget(fn_name=fn_original_name, parameters=references, triggers=on_changes_widgets)
             # Adjust entry arguments
             fn = self._adjust_arguments(fn, entry_arguments)
 
             body = fn
             if return_type != self._parent_class:
+                # If the return type is not a widget, we need to adjust the return type.
                 body = self._adjust_return(fn, return_type)
+
+            # Function are saved  with a unique id, so the function won't be replaced when it is used multiple times.
+            # This is because when a basic type is returned like str or int, the return value will only change the
+            # value of the widget, but we want to keep the other widget attributes like the title.
+            # If we don't use unique functions for each widget, we won't be able to keep the other attributes.
+            fn_uid = str(uuid.uuid1())
+            # Add to Widget Structure
+            self._add_bind_to_widget(fn=fn_uid, result=self._parent_class, parameters=references, triggers=on_changes_widgets)
+            # Serialize function and save it to file.
+            ser_body = base64.b64encode(zlib.compress(dill.dumps(body, recurse=True))).decode('utf-8')
+            with open(os.path.join(DATA_DIR, fn_uid), 'wt') as f:
+                f.write(ser_body)
             result = {
-                "body": base64.b64encode(zlib.compress(dill.dumps(body, recurse=True))).decode('utf-8'),
+                "body": fn_uid,
                 "parameters": entry_arguments,
                 "result": self._parent_class
             }
-
-            # Add to DataApp Structure
-            self.parent_data_app.functions[fn_original_name] = result
+            # Add to DataApp Structure with function uid
+            self.parent_data_app.functions[fn_uid] = result
+            # Append fn uid to dataApp data to keep track of what files belong to each dataApp.
+            try:
+                # If this bind ins happening inside a custom function, there is no access to the dataApp, therefore
+                # insert the information into the database.
+                self.parent_data_app._update_data([fn_uid])
+            except Exception:
+                # If the previous call fails, It means the dataApp is not yet created, and therefor we add the information
+                # to the _data attribute, which will be added to the database once the dataApp is registered.
+                self.parent_data_app._data.append(fn_uid)
 
             if kwargs.get("on_init"):
                 try:
                     self._prepare_execution_on_registration(args, body)
-                except Exception:
+                except Exception as e:
                     # Continue with the dataApp registration although on_init execution could not be completed.
                     pass
 
         else:
             raise ValueError("Return type does not match")
 
     def _prepare_execution_on_registration(self, input_args: Tuple, fn_body: Callable):
@@ -340,27 +366,30 @@
         return List of all the triggers.
         """
         triggers = []
         if kwargs.get("triggers"):
             triggers = [y.widget_id for y in kwargs.get("triggers")]
         return triggers
 
-    def _add_bind_to_widget(self, fn_name: str = None,
+    def _add_bind_to_widget(self,
+                            fn: str = None,
+                            result: str = None,
                             props: str = None,
                             parameters: List = None,
                             triggers: List = None):
         """
         Find if there are triggers to bind in the kwargs. In bind function, triggers are defined in the triggers parameter.
-        param fn_name: Name of the function to add.
+        param fn_name: Name of the function or uid to add.
         param props: Properties to change.
         param parameters: Parameters use in the function.
         param triggers: Widgets that trigger the bind.
         """
         self._bind.append({
-            "fn": fn_name,
+            "fn": fn,
+            "result": result,
             "props": props,
             "parameters": parameters,
             "triggers": triggers
         })
 
     def _adjust_return(self, fn: Callable, return_type) -> Callable:
         """
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/functions.py` & `shapelets-platform-2.0.86/src/shapelets/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/iris.csv` & `shapelets-platform-2.0.86/src/shapelets/iris.csv`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/model/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/altair.py` & `shapelets-platform-2.0.86/src/shapelets/model/altair.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/capsule.py` & `shapelets-platform-2.0.86/src/shapelets/model/capsule.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/collection.py` & `shapelets-platform-2.0.86/src/shapelets/model/collection.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/dataframe.py` & `shapelets-platform-2.0.86/src/shapelets/model/dataframe.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/function_description.py` & `shapelets-platform-2.0.86/src/shapelets/model/function_description.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/function_parameter.py` & `shapelets-platform-2.0.86/src/shapelets/model/function_parameter.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/group.py` & `shapelets-platform-2.0.86/src/shapelets/model/group.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/image.py` & `shapelets-platform-2.0.86/src/shapelets/model/image.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/metadata_item.py` & `shapelets-platform-2.0.86/src/shapelets/model/metadata_item.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/model.py` & `shapelets-platform-2.0.86/src/shapelets/model/model.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/ndarray.py` & `shapelets-platform-2.0.86/src/shapelets/model/ndarray.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/permissions.py` & `shapelets-platform-2.0.86/src/shapelets/model/permissions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/replicated_param.py` & `shapelets-platform-2.0.86/src/shapelets/model/replicated_param.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/sequence.py` & `shapelets-platform-2.0.86/src/shapelets/model/sequence.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/sequence_axis.py` & `shapelets-platform-2.0.86/src/shapelets/model/sequence_axis.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/user.py` & `shapelets-platform-2.0.86/src/shapelets/model/user.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/model/view_match.py` & `shapelets-platform-2.0.86/src/shapelets/model/view_match.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/svr/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/app.py` & `shapelets-platform-2.0.86/src/shapelets/svr/app.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/authn/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/svr/authn/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/authn/authhttp.py` & `shapelets-platform-2.0.86/src/shapelets/svr/authn/authhttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/authn/authrepo.py` & `shapelets-platform-2.0.86/src/shapelets/svr/authn/authrepo.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     FROM groups 
     LEFT JOIN users_groups on users_groups.groupId = groups.uid where users_groups.userId = ?
     """, [new_user_id])
     new_user_groups = conn.fetch_all()
     if new_user_groups:
         group_names = [group[0] for group in new_user_groups]
     else:
-        raise ValueError("Transfer user does not belong to any group")
+        raise ValueError("Transfer user does not belong to any group or does not have write permissions over the group.")
     # Try transferring dataApps with group
     dataapp_with_group = _user_group_dataapp_list(old_user_id, conn)
     for app in dataapp_with_group:
         if any(x in app.groups for x in group_names):
             conn.execute(""" 
                 UPDATE dataapps 
                 SET userId = ?
@@ -178,14 +178,20 @@
                 return False
 
             if transfer is not None:
                 transfer_user_id = _principals_find_userId(scope, transfer, conn)
                 if transfer_user_id is None:
                     return False
                 _transfer_data_apps(uid, transfer_user_id, conn)
+            else:
+                dataapp = _user_group_dataapp_list(uid, conn)
+                if dataapp:
+                    message = f"User {userName} cannot be deleted because this user owns dataApp/s belonging to a group. "
+                    message += "Please, use transfer to change the owner before removing user."
+                    raise RuntimeError(message)
 
             _principals_delete_by_userId(uid, scope, conn)
             _unp_users_delete(userName, conn)
             _users_delete(uid, conn)
             return True
 
     def get_salt(self, userName: str) -> Optional[bytes]:
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/authn/authservice.py` & `shapelets-platform-2.0.86/src/shapelets/svr/authn/authservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/authn/gc_client.py` & `shapelets-platform-2.0.86/src/shapelets/svr/authn/gc_client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/authn/iauthrepo.py` & `shapelets-platform-2.0.86/src/shapelets/svr/authn/iauthrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/authn/iauthservice.py` & `shapelets-platform-2.0.86/src/shapelets/svr/authn/iauthservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/access_token_credentials.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/access_token_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/azure_gen1.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/azure_gen1.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/azure_gen2.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/azure_gen2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/driver.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/driver.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/dynamic_credentials.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/dynamic_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_config.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/fsspec_config.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_vfs.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/fsspec_vfs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_vfs_file.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/fsspec_vfs_file.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/ftp.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/ftp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/local.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/local.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/protocols.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/protocols.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/smb.py` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/smb.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/vfs_sample_config.toml` & `shapelets-platform-2.0.86/src/shapelets/svr/data/vfs/vfs_sample_config.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/svr/dataapps/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataapps_ws.py` & `shapelets-platform-2.0.86/src/shapelets/svr/dataapps/dataapps_ws.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataappshttp.py` & `shapelets-platform-2.0.86/src/shapelets/svr/dataapps/dataappshttp.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     async def get_dataapp_spec(self, specId: str) -> file:
         shapelets_dir = os.path.expanduser('~/.shapelets')
         data_apps_store = os.path.join(shapelets_dir, 'dataAppsStore')
         spec_path = os.path.join(data_apps_store, f"{specId}.json")
         return file(spec_path, "multipart/form-data")
 
     @get("/{id}/{major}/{minor}")
-    async def get_dataapp_by_version(self, dataAppName: str, major: int, minor: int) -> DataAppAttributes:
+    async def get_dataapp_by_version(self, dataAppName: str, major: int, minor: int) -> DataAppProfile:
         return self._svr.get_dataapp_by_version(dataAppName, major, minor)
 
     @get("/{id}/lastVersion")
     async def get_dataapp_last_version(self, dataAppName: str) -> float:
         return self._svr.get_dataapp_last_version(dataAppName)
 
     @get("/{id}/tags")
@@ -176,15 +176,15 @@
                                     minor=dataapp.version[1] if dataapp.version else None,
                                     description=dataapp.description,
                                     specId=dataapp.to_json(),
                                     tags=dataapp.tags,
                                     groups=dataapp.groups)
         params = None
         if dataapp._data:
-            params=[("data", dataapp._data)]
+            params = [("data", dataapp._data)]
         response = self.session.post('/api/dataapps/', json=json.loads(payload.json()), params=params)
         if response.status_code != 200:
             raise RuntimeError(response.content)
         return response
 
     def get_dataapp(self, dataAppName: str) -> DataAppAttributes:
         return self.session.get('/api/dataapps/', params=[("dataAppName", dataAppName)])
@@ -199,17 +199,20 @@
     def get_dataapp_privileges(self, dataAppName: str) -> List[DataAppAttributes]:
         pass
 
     def get_dataapp_versions(self, dataAppName: str) -> List[float]:
         return self.session.get('/api/{id}/versions', params=[("dataAppName", dataAppName)])
 
     def get_dataapp_by_id(self, uid: int) -> DataAppProfile:
-        return self.session.get('/api/{id}', params=[("uid", uid), ("uid", uid)])
+        return self.session.get('/api/{id}', params=[("uid", uid)])
 
-    def get_dataapp_by_version(self, dataAppName: str, version: float) -> List[float]:
-        return self.session.get('/api/{id}/{version}', params=[("dataAppName", dataAppName), ("version", version)])
+    def get_dataapp_by_version(self, dataAppName: str, major: int, minor: int) -> DataAppProfile:
+        response = self.session.get(f'/api/dataapps/{id}/{major}/{minor}', params=[("dataAppName", dataAppName),
+                                                                                   ("major", major),
+                                                                                   ("minor", minor)])
+        return response.json()
 
     def get_dataapp_last_version(self, dataAppName: str) -> float:
         return self.session.get('/api/{id}/lastVersion', params=[("dataAppName", dataAppName)])
 
     def get_dataapp_tags(self, dataAppName: str) -> List[str]:
         return self.session.get('/api/{id}/tags', params=[("dataAppName", dataAppName)])
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataappsrepo.py` & `shapelets-platform-2.0.86/src/shapelets/svr/dataapps/dataappsrepo.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
     conn.execute(base_query)
 
     result = []
     for record in conn.fetch_all():
         dataapp = _load_dataapp_by_id(record[0], conn)
         conn.execute(""" 
-            SELECT groups.name
+            SELECT distinct(groups.name)
             FROM groups
             INNER JOIN dataapp_group ON dataapp_group.groupId = groups.uid
             WHERE dataapp_group.dataappId = ?;
         """, [dataapp.uid])
         groups = conn.fetch_all()
         if groups is not None:
             dataapp.groups = [group[0] for group in groups]
@@ -452,14 +452,22 @@
             INSERT INTO dataapp_group 
             (dataappId, groupId)
             VALUES (?, ?);
         """, [uid, group_id])
 
 
 def _add_data(uid: int, data: List[str], conn: Connection):
+    for widget_id in data:
+        conn.execute("""
+                INSERT INTO dataapp_data 
+                (dataappId, dataInfo)
+                VALUES (?, ?);
+            """, [uid, widget_id])
+
+def _overwrite_data(uid: int, data: List[str], conn: Connection):
     # First remove the data from the given dataApp, as it's going to be updated.
     remove_data(uid, conn)
     for widget_id in data:
         conn.execute("""
                 INSERT INTO dataapp_data 
                 (dataappId, dataInfo)
                 VALUES (?, ?);
@@ -524,15 +532,15 @@
                         raise WritePermission(user_name=user_name, group_name=group)
                 details.groups = group_ids
                 dataapp = self._create_for_group(details, conn)
             else:
                 # DataApp is going to user space
                 dataapp = self._create_for_user(details, conn)
             if data:
-                _add_data(dataapp.uid, data, conn)
+                _overwrite_data(dataapp.uid, data, conn)
             return dataapp
 
     def load_by_name(self, dataapp_name: str) -> Optional[DataAppProfile]:
         with connect() as conn:
             return _load_dataapp_by_name(dataapp_name, conn)
 
     def load_by_id(self, uid: int) -> Optional[DataAppProfile]:
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataappsservice.py` & `shapelets-platform-2.0.86/src/shapelets/svr/dataapps/dataappsservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,15 @@
     def user_local_dataapp_list(self, user_id: int) -> List[DataAppProfile]:
         return self._dataapp_repo.user_local_dataapp_list(user_id)
 
     def user_group_dataapp_list(self, user_id: int) -> List[DataAppProfile]:
         return self._dataapp_repo.user_group_dataapp_list(user_id)
 
     def create(self, attributes: DataAppAttributes, data: List[str] = None) -> DataAppProfile:
-        with transaction():
-            return self._dataapp_repo.create(attributes, data)
+        return self._dataapp_repo.create(attributes, data)
 
     def get_dataapp(self, dataapp_name: str):
         return self._dataapp_repo.load_by_name(dataapp_name)
 
     def get_dataapp_by_id(self, uid: int) -> DataAppProfile:
         return self._dataapp_repo.load_by_id(uid)
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/http_docs.py` & `shapelets-platform-2.0.86/src/shapelets/svr/dataapps/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/idataappsrepo.py` & `shapelets-platform-2.0.86/src/shapelets/svr/dataapps/idataappsrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/idataappsservice.py` & `shapelets-platform-2.0.86/src/shapelets/svr/dataapps/idataappsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/db/native/database.py` & `shapelets-platform-2.0.86/src/shapelets/svr/db/native/database.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/db/native/settings.py` & `shapelets-platform-2.0.86/src/shapelets/svr/db/native/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/db/schema_builder.py` & `shapelets-platform-2.0.86/src/shapelets/svr/db/schema_builder.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v1.py` & `shapelets-platform-2.0.86/src/shapelets/svr/db/schema_v1.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v2.py` & `shapelets-platform-2.0.86/src/shapelets/svr/db/schema_v2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v3.py` & `shapelets-platform-2.0.86/src/shapelets/svr/db/schema_v3.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v4.py` & `shapelets-platform-2.0.86/src/shapelets/svr/db/schema_v4.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/db/setup.py` & `shapelets-platform-2.0.86/src/shapelets/svr/db/setup.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/execution/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/svr/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/execution/executionhttp.py` & `shapelets-platform-2.0.86/src/shapelets/svr/execution/executionhttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/execution/executionservice.py` & `shapelets-platform-2.0.86/src/shapelets/svr/execution/executionservice.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,24 +26,29 @@
 def _serialize_table(table: pa.Table):
     sink = pa.BufferOutputStream()
     with pa.ipc.RecordBatchFileWriter(sink, table.schema) as writer:
         writer.write(table)
     buffer = sink.getvalue()
     return base64.b64encode(buffer).decode("utf-8")
 
+SH_DIR = os.path.expanduser('~/.shapelets')
+DATA_DIR = os.path.join(SH_DIR, 'data')
 
 class ExecutionService(IExecutionService):
     __slots__ = ('_execution_repo',)
 
     def __init__(self, execution_repo: IExecutionRepo) -> None:
         self._execution_repo = execution_repo
 
     def execute_function(self, fn: FunctionProfile) -> Any:
-        # fn body is serialize and compressed with zlib
-        bytes_from_str = base64.decodebytes(bytes(fn.body, encoding="utf-8"))
+        # Function is saved in .shapelets/data
+        with open(os.path.join(DATA_DIR, fn.body), 'r') as f:
+            lines = f.read()
+        # In addition, fn body is serialized and compressed with zlib
+        bytes_from_str = base64.decodebytes(bytes(lines, encoding="utf-8"))
         decompress = zlib.decompress(bytes_from_str)
         callable_fn = dill.loads(decompress)
         arg_values = []
         for arg in fn.parameters:
             if arg.get('pickled'):
                 arg_values.append(dill.loads(base64.decodebytes(bytes(arg.get('value'), encoding="utf-8"))))
             else:
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/execution/http_docs.py` & `shapelets-platform-2.0.86/src/shapelets/svr/execution/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/groups/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/svr/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/groups/groupservice.py` & `shapelets-platform-2.0.86/src/shapelets/svr/groups/groupservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     def get_details(self, group_name: str) -> GroupProfile:
         return self._groups_repo.get_details(group_name)
 
     def group_name_exists(self, group_name: str) -> bool:
         return self._groups_repo.group_name_exists(group_name)
 
-    def delete_group(self, group_name: str):
+    def delete_group(self, group_name: str) -> str:
         return self._groups_repo.delete_by_name(group_name)
 
     def delete_all(self):
         self._groups_repo.delete_all()
 
     def all_users_in_group(self, group_name: str) -> List[UserProfile]:
         self._groups_repo.all_users_in_group(group_name)
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/groups/groupshttp.py` & `shapelets-platform-2.0.86/src/shapelets/svr/groups/groupshttp.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,17 +56,17 @@
     async def group_name_exists(self, groupName: str) -> bool:
         try:
             return self.json(self._svr.group_name_exists(groupName))
         except Exception as e:
             return self.status_code(500, str(e))
 
     @get('/unp/remove')
-    async def delete_group(self, groupName: str):
+    async def delete_group(self, groupName: str) -> str:
         try:
-            return self.json(self._svr.delete_by_name(groupName))
+            return self.json(self._svr.delete_group(groupName))
         except InvalidGroupName as e:
             return self.bad_request(str(e))
         except Exception as e:
             return self.status_code(500, str(e))
 
     @get('/unp/removeAll')
     async def delete_all(self):
@@ -77,15 +77,16 @@
 
 
 class GroupsHttpProxy(IGroupsService):
     def __init__(self, session: Session) -> None:
         self.session = session
 
     def create(self, group_name: str, group_description: str) -> Optional[GroupProfile]:
-        response = self.session.post('/api/groups/', params=[("groupName", group_name), ("groupDescription", group_description)])
+        response = self.session.post(
+            '/api/groups/', params=[("groupName", group_name), ("groupDescription", group_description)])
         if response.status_code == 400 or response.status_code == 500:
             raise Exception(response.content)
         return response.json()
 
     def get_all(self) -> List[GroupProfile]:
         response = self.session.get('/api/groups/unp/all')
         return response.json()
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/groups/groupsrepo.py` & `shapelets-platform-2.0.86/src/shapelets/svr/groups/groupsrepo.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,19 +75,19 @@
     record = conn.fetch_one()
     if record is None:
         return None
     return GroupProfile(uid=record[0], name=record[1], description=record[2])
 
 
 def _delete_group_by_id(uid: int, conn: Connection):
-    conn.execute("DELETE FROM groups WHERE uid = ?;", [uid]);
+    conn.execute("DELETE FROM groups WHERE uid = ?;", [uid])
 
 
 def _delete_group_by_name(group_name: str, conn: Connection):
-    conn.execute("DELETE FROM groups WHERE name = ?;", [group_name]);
+    conn.execute("DELETE FROM groups WHERE name = ?;", [group_name])
 
 
 def _clear_all_groups(conn: Connection):
     conn.execute("DELETE FROM groups;")
 
 
 def _load_users_in_group(group_name: str, conn: Connection) -> Optional[UserProfile]:
@@ -132,17 +132,22 @@
         with connect() as conn:
             return group_has_group_name(group_name, conn)
 
     def delete_by_id(self, uid: int):
         with connect() as conn:
             _delete_group_by_id(uid, conn)
 
-    def delete_by_name(self, group_name: str):
-        with connect() as conn:
-            _delete_group_by_name(group_name, conn)
+    def delete_by_name(self, group_name: str) -> str:
+
+        if self.group_name_exists(group_name):
+            with connect() as conn:
+                _delete_group_by_name(group_name, conn)
+                return 'Group %s has been deleted' % group_name
+        else:
+            return 'Group %s does not exist' % group_name
 
     def delete_all(self):
         with connect() as conn:
             _clear_all_groups(conn)
 
     def get_all(self,
                 sort_by: Optional[List[Tuple[GroupField, bool]]] = None,
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/groups/igroupsrepo.py` & `shapelets-platform-2.0.86/src/shapelets/svr/groups/igroupsrepo.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         """
         Delete group providing its id.
         param uid
         """
         pass
 
     @abstractmethod
-    def delete_by_name(self, group_name: str):
+    def delete_by_name(self, group_name: str) -> str:
         """
         Delete group providing its name.
         param group_name
         """
         pass
 
     @abstractmethod
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/groups/igroupsservice.py` & `shapelets-platform-2.0.86/src/shapelets/svr/groups/igroupsservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         Returns
         -------
         A boolean flag; when True, the group name exists.  False otherwise.
         """
         pass
 
     @abstractmethod
-    def delete_group(self, group_name: str):
+    def delete_group(self, group_name: str) -> str:
         """
         Delete group from the system
 
         Parameters
         ----------
         group_name
         """
```

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/model/dataapps.py` & `shapelets-platform-2.0.86/src/shapelets/svr/model/dataapps.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/model/principals.py` & `shapelets-platform-2.0.86/src/shapelets/svr/model/principals.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/model/users.py` & `shapelets-platform-2.0.86/src/shapelets/svr/model/users.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/mustang/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/svr/mustang/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/mustang/asttranslation.py` & `shapelets-platform-2.0.86/src/shapelets/svr/mustang/asttranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/mustang/conversions.py` & `shapelets-platform-2.0.86/src/shapelets/svr/mustang/conversions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/mustang/core.py` & `shapelets-platform-2.0.86/src/shapelets/svr/mustang/core.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/mustang/decompiling.py` & `shapelets-platform-2.0.86/src/shapelets/svr/mustang/decompiling.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/mustang/exceptions.py` & `shapelets-platform-2.0.86/src/shapelets/svr/mustang/exceptions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/mustang/hashdict.py` & `shapelets-platform-2.0.86/src/shapelets/svr/mustang/hashdict.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/mustang/ormtypes.py` & `shapelets-platform-2.0.86/src/shapelets/svr/mustang/ormtypes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/mustang/prototypes/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/svr/mustang/prototypes/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/mustang/serialization.py` & `shapelets-platform-2.0.86/src/shapelets/svr/mustang/serialization.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/mustang/sqlbuilding.py` & `shapelets-platform-2.0.86/src/shapelets/svr/mustang/sqlbuilding.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/mustang/sqltranslation.py` & `shapelets-platform-2.0.86/src/shapelets/svr/mustang/sqltranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/server.py` & `shapelets-platform-2.0.86/src/shapelets/svr/server.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/settings/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/svr/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/settings/client.py` & `shapelets-platform-2.0.86/src/shapelets/svr/settings/client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/settings/defaults.py` & `shapelets-platform-2.0.86/src/shapelets/svr/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/settings/functions.py` & `shapelets-platform-2.0.86/src/shapelets/svr/settings/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/settings/http.py` & `shapelets-platform-2.0.86/src/shapelets/svr/settings/http.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/settings/reload.py` & `shapelets-platform-2.0.86/src/shapelets/svr/settings/reload.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/settings/server.py` & `shapelets-platform-2.0.86/src/shapelets/svr/settings/server.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/settings/settings.py` & `shapelets-platform-2.0.86/src/shapelets/svr/settings/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/settings/settings.toml` & `shapelets-platform-2.0.86/src/shapelets/svr/settings/settings.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/settings/ssl.py` & `shapelets-platform-2.0.86/src/shapelets/svr/settings/ssl.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/settings/telemetry.py` & `shapelets-platform-2.0.86/src/shapelets/svr/settings/telemetry.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/settings/websocket.py` & `shapelets-platform-2.0.86/src/shapelets/svr/settings/websocket.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/telemetry/sysinfo.py` & `shapelets-platform-2.0.86/src/shapelets/svr/telemetry/sysinfo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/telemetry/telemetryservice.py` & `shapelets-platform-2.0.86/src/shapelets/svr/telemetry/telemetryservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/users/__init__.py` & `shapelets-platform-2.0.86/src/shapelets/svr/users/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/users/http_docs.py` & `shapelets-platform-2.0.86/src/shapelets/svr/users/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/users/iusersrepo.py` & `shapelets-platform-2.0.86/src/shapelets/svr/users/iusersrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/users/iusersservice.py` & `shapelets-platform-2.0.86/src/shapelets/svr/users/iusersservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/users/usershttp.py` & `shapelets-platform-2.0.86/src/shapelets/svr/users/usershttp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/users/usersrepo.py` & `shapelets-platform-2.0.86/src/shapelets/svr/users/usersrepo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/users/usersservice.py` & `shapelets-platform-2.0.86/src/shapelets/svr/users/usersservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/utils/crypto.py` & `shapelets-platform-2.0.86/src/shapelets/svr/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/utils/flexbytes.py` & `shapelets-platform-2.0.86/src/shapelets/svr/utils/flexbytes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/altair.json` & `shapelets-platform-2.0.86/src/shapelets/svr/www/altair.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/asset-manifest.json` & `shapelets-platform-2.0.86/src/shapelets/svr/www/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/dataapp.json` & `shapelets-platform-2.0.86/src/shapelets/svr/www/dataapp.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/favicon.ico` & `shapelets-platform-2.0.86/src/shapelets/svr/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/index.html` & `shapelets-platform-2.0.86/src/shapelets/svr/www/index.html`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/css/main.8349d999.chunk.css` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/css/main.8349d999.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/4.77242983.chunk.js` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/4.77242983.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/main.83b9aa07.chunk.js` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/main.83b9aa07.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/runtime-main.fd20aea3.js` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/js/runtime-main.fd20aea3.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/audit.cb539a06.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/audit.cb539a06.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/bin.7e762965.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/bin.7e762965.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/clear.27b15301.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/clear.27b15301.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/collections.06fdf54a.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/collections.06fdf54a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/date-time.a1e86419.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/date-time.a1e86419.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/download-image.87310709.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/download-image.87310709.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/filter.cec803b8.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/filter.cec803b8.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logout.57c593a5.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/logout.57c593a5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/pdf.5d189efa.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/pdf.5d189efa.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/share.bc9a8370.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/share.bc9a8370.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/single-plot.864a583b.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/single-plot.864a583b.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/wave-top.6d51781b.png` & `shapelets-platform-2.0.86/src/shapelets/svr/www/static/media/wave-top.6d51781b.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets_platform.egg-info/PKG-INFO` & `shapelets-platform-2.0.86/src/shapelets_platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.85
+Version: 2.0.86
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
```

### Comparing `shapelets-platform-2.0.85/src/shapelets_platform.egg-info/SOURCES.txt` & `shapelets-platform-2.0.86/src/shapelets_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.85/src/shapelets_platform.egg-info/requires.txt` & `shapelets-platform-2.0.86/src/shapelets_platform.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 matplotlib>=3.5.3
 mypy~=0.990
 numpy>=1.21.6
 pandas>=1.3.5
 psutil>=5.9.2
 pyarrow>=12.0.0
 py-cpuinfo>=9.0.0
-pydantic>=1.10.2
+pydantic==1.10.11
 pygeohash>=1.2.0
 PyNaCl>=1.5.0
 requests>=2.28.1
 setuptools-scm>=7.1.0
-shapelets_native==2.0.85
+shapelets_native==2.0.86
 tabulate>=0.8.10
 tomlkit>=0.11.4
 tqdm>=4.64.1
 typing_extensions>=4.6.2
 uvicorn>=0.18.3
 vega-datasets>=0.9
 websocket-client>=1.5.2
```


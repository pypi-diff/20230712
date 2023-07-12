# Comparing `tmp/quality-result-gui-2.0.0.tar.gz` & `tmp/quality-result-gui-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quality-result-gui-2.0.0.tar", last modified: Tue Jul 11 10:47:36 2023, max compression
+gzip compressed data, was "quality-result-gui-2.0.1.tar", last modified: Wed Jul 12 09:41:37 2023, max compression
```

## Comparing `quality-result-gui-2.0.0.tar` & `quality-result-gui-2.0.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.278218 quality-result-gui-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.282218 quality-result-gui-2.0.0/src/quality_result_gui/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/api/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/api/quality_api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/api/types/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/api/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/api/types/quality_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/layer_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_data_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_error_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_error_manager_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_error_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_errors_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_errors_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/quality_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_error_fatal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_error_info.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_error_warning.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_result_gui.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/style/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/style/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/style/default_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/style/quality_layer_error_symbol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_error_tree_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_errors_dock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_errors_dock.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_errors_tree_filter_menu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/utils/layer_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui/utils/styling_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.286219 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-11 10:47:36.000000 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-11 10:47:36.000000 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:47:36.000000 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-11 10:47:36.000000 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 10:47:36.000000 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 10:47:36.000000 quality-result-gui-2.0.0/src/quality_result_gui.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/example_quality_errors/
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/example_quality_errors/quality_errors.json
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/mock_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/metadata.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/i18n/fi.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:47:36.290219 quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-07-11 10:47:25.000000 quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/icons/quality_result_gui.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.463596 quality-result-gui-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-12 09:41:37.463596 quality-result-gui-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-12 09:41:37.463596 quality-result-gui-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.455595 quality-result-gui-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.459596 quality-result-gui-2.0.1/src/quality_result_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.459596 quality-result-gui-2.0.1/src/quality_result_gui/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/api/quality_api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.459596 quality-result-gui-2.0.1/src/quality_result_gui/api/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/api/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/api/types/quality_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.459596 quality-result-gui-2.0.1/src/quality_result_gui/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/layer_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/quality_data_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/quality_error_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/quality_error_manager_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/quality_error_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14796 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/quality_errors_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/quality_errors_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/quality_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.459596 quality-result-gui-2.0.1/src/quality_result_gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.459596 quality-result-gui-2.0.1/src/quality_result_gui/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/resources/icons/quality_error_fatal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/resources/icons/quality_error_info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/resources/icons/quality_error_warning.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/resources/icons/quality_result_gui.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.459596 quality-result-gui-2.0.1/src/quality_result_gui/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/style/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/style/default_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/style/quality_layer_error_symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.459596 quality-result-gui-2.0.1/src/quality_result_gui/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/ui/quality_error_tree_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/ui/quality_errors_dock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/ui/quality_errors_dock.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/ui/quality_errors_tree_filter_menu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.463596 quality-result-gui-2.0.1/src/quality_result_gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/utils/layer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui/utils/styling_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.459596 quality-result-gui-2.0.1/src/quality_result_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-12 09:41:37.000000 quality-result-gui-2.0.1/src/quality_result_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-12 09:41:37.000000 quality-result-gui-2.0.1/src/quality_result_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:41:37.000000 quality-result-gui-2.0.1/src/quality_result_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 09:41:37.000000 quality-result-gui-2.0.1/src/quality_result_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 09:41:37.000000 quality-result-gui-2.0.1/src/quality_result_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 09:41:37.000000 quality-result-gui-2.0.1/src/quality_result_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.463596 quality-result-gui-2.0.1/src/quality_result_gui_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.463596 quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.463596 quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/example_quality_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/example_quality_errors/quality_errors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/mock_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/metadata.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.463596 quality-result-gui-2.0.1/src/quality_result_gui_plugin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.463596 quality-result-gui-2.0.1/src/quality_result_gui_plugin/resources/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/resources/i18n/fi.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:41:37.463596 quality-result-gui-2.0.1/src/quality_result_gui_plugin/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-07-12 09:41:27.000000 quality-result-gui-2.0.1/src/quality_result_gui_plugin/resources/icons/quality_result_gui.svg
```

### Comparing `quality-result-gui-2.0.0/CHANGELOG.md` & `quality-result-gui-2.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # CHANGELOG
 
+## [2.0.1] - 2023-07-12
+
+- Feat: Add Finnish translations
+
 ## [2.0.0] - 2023-07-11
 
-- Refactor!: replace hierachical representation of quality errors with a flat quality error list
+- Refactor!: replace hierarchical representation of quality errors with a flat quality error list
 
 ## [1.1.6] - 2023-05-23
 
 - Feat: Add functionality to display quality error feature type and attribute names from layer aliases.
 
 ## [1.1.5] - 2023-03-29
 
@@ -73,7 +77,8 @@
 [1.1.1]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.1
 [1.1.2]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.2
 [1.1.3]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.3
 [1.1.4]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.4
 [1.1.5]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.5
 [1.1.6]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.6
 [2.0.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v2.0.0
+[2.0.1]: https://github.com/nlsfi/quality-result-gui/releases/tag/v2.0.1
```

### Comparing `quality-result-gui-2.0.0/LICENSE` & `quality-result-gui-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/PKG-INFO` & `quality-result-gui-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quality-result-gui
-Version: 2.0.0
+Version: 2.0.1
 Summary: QGIS plugin for visualizing quality check results.
 Home-page: https://github.com/nlsfi/quality-result-gui
 Author: National Land Survey of Finland
 Author-email: eero.hietanen@maanmittauslaitos.fi
 License: GNU GPL v3.0
 Project-URL: Changelog, https://github.com/nlsfi/quality-result-gui/blob/main/CHANGELOG.md
 Keywords: qgis
@@ -95,17 +95,21 @@
 Copyright (C) 2022 [National Land Survey of Finland].
 
 [National Land Survey of Finland]: https://www.maanmittauslaitos.fi/en
 [qgis-plugin-dev-tools]: https://github.com/nlsfi/qgis-plugin-dev-tools
 
 # CHANGELOG
 
+## [2.0.1] - 2023-07-12
+
+- Feat: Add Finnish translations
+
 ## [2.0.0] - 2023-07-11
 
-- Refactor!: replace hierachical representation of quality errors with a flat quality error list
+- Refactor!: replace hierarchical representation of quality errors with a flat quality error list
 
 ## [1.1.6] - 2023-05-23
 
 - Feat: Add functionality to display quality error feature type and attribute names from layer aliases.
 
 ## [1.1.5] - 2023-03-29
 
@@ -172,7 +176,8 @@
 [1.1.1]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.1
 [1.1.2]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.2
 [1.1.3]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.3
 [1.1.4]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.4
 [1.1.5]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.5
 [1.1.6]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.6
 [2.0.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v2.0.0
+[2.0.1]: https://github.com/nlsfi/quality-result-gui/releases/tag/v2.0.1
```

### Comparing `quality-result-gui-2.0.0/README.md` & `quality-result-gui-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/setup.cfg` & `quality-result-gui-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/__init__.py` & `quality-result-gui-2.0.1/src/quality_result_gui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #  of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with quality-result-gui. If not, see <https://www.gnu.org/licenses/>.
 
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 
 from enum import Enum, auto
 
 
 class SelectionType(Enum):
     LeftClick = auto()
```

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/api/__init__.py` & `quality-result-gui-2.0.1/src/quality_result_gui/api/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/api/quality_api_client.py` & `quality-result-gui-2.0.1/src/quality_result_gui/api/quality_api_client.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/api/types/__init__.py` & `quality-result-gui-2.0.1/src/quality_result_gui/api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/api/types/quality_error.py` & `quality-result-gui-2.0.1/src/quality_result_gui/api/types/quality_error.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/configuration/__init__.py` & `quality-result-gui-2.0.1/src/quality_result_gui/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/layer_mapping.py` & `quality-result-gui-2.0.1/src/quality_result_gui/layer_mapping.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/quality_data_fetcher.py` & `quality-result-gui-2.0.1/src/quality_result_gui/quality_data_fetcher.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/quality_error_manager.py` & `quality-result-gui-2.0.1/src/quality_result_gui/quality_error_manager.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/quality_error_manager_settings.py` & `quality-result-gui-2.0.1/src/quality_result_gui/quality_error_manager_settings.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/quality_error_visualizer.py` & `quality-result-gui-2.0.1/src/quality_result_gui/quality_error_visualizer.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/quality_errors_filters.py` & `quality-result-gui-2.0.1/src/quality_result_gui/quality_errors_filters.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/quality_errors_tree_model.py` & `quality-result-gui-2.0.1/src/quality_result_gui/quality_errors_tree_model.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/quality_layer.py` & `quality-result-gui-2.0.1/src/quality_result_gui/quality_layer.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/resources/__init__.py` & `quality-result-gui-2.0.1/src/quality_result_gui/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_error_fatal.svg` & `quality-result-gui-2.0.1/src/quality_result_gui/resources/icons/quality_error_fatal.svg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_error_info.svg` & `quality-result-gui-2.0.1/src/quality_result_gui/resources/icons/quality_error_info.svg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_error_warning.svg` & `quality-result-gui-2.0.1/src/quality_result_gui/resources/icons/quality_error_warning.svg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/resources/icons/quality_result_gui.svg` & `quality-result-gui-2.0.1/src/quality_result_gui/resources/icons/quality_result_gui.svg`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/style/__init__.py` & `quality-result-gui-2.0.1/src/quality_result_gui/style/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/style/default_style.py` & `quality-result-gui-2.0.1/src/quality_result_gui/style/default_style.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/style/quality_layer_error_symbol.py` & `quality-result-gui-2.0.1/src/quality_result_gui/style/quality_layer_error_symbol.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_error_tree_view.py` & `quality-result-gui-2.0.1/src/quality_result_gui/ui/quality_error_tree_view.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_errors_dock.py` & `quality-result-gui-2.0.1/src/quality_result_gui/ui/quality_errors_dock.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_errors_dock.ui` & `quality-result-gui-2.0.1/src/quality_result_gui/ui/quality_errors_dock.ui`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/ui/quality_errors_tree_filter_menu.py` & `quality-result-gui-2.0.1/src/quality_result_gui/ui/quality_errors_tree_filter_menu.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/utils/__init__.py` & `quality-result-gui-2.0.1/src/quality_result_gui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/utils/layer_utils.py` & `quality-result-gui-2.0.1/src/quality_result_gui/utils/layer_utils.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui/utils/styling_utils.py` & `quality-result-gui-2.0.1/src/quality_result_gui/utils/styling_utils.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui.egg-info/PKG-INFO` & `quality-result-gui-2.0.1/src/quality_result_gui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quality-result-gui
-Version: 2.0.0
+Version: 2.0.1
 Summary: QGIS plugin for visualizing quality check results.
 Home-page: https://github.com/nlsfi/quality-result-gui
 Author: National Land Survey of Finland
 Author-email: eero.hietanen@maanmittauslaitos.fi
 License: GNU GPL v3.0
 Project-URL: Changelog, https://github.com/nlsfi/quality-result-gui/blob/main/CHANGELOG.md
 Keywords: qgis
@@ -95,17 +95,21 @@
 Copyright (C) 2022 [National Land Survey of Finland].
 
 [National Land Survey of Finland]: https://www.maanmittauslaitos.fi/en
 [qgis-plugin-dev-tools]: https://github.com/nlsfi/qgis-plugin-dev-tools
 
 # CHANGELOG
 
+## [2.0.1] - 2023-07-12
+
+- Feat: Add Finnish translations
+
 ## [2.0.0] - 2023-07-11
 
-- Refactor!: replace hierachical representation of quality errors with a flat quality error list
+- Refactor!: replace hierarchical representation of quality errors with a flat quality error list
 
 ## [1.1.6] - 2023-05-23
 
 - Feat: Add functionality to display quality error feature type and attribute names from layer aliases.
 
 ## [1.1.5] - 2023-03-29
 
@@ -172,7 +176,8 @@
 [1.1.1]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.1
 [1.1.2]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.2
 [1.1.3]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.3
 [1.1.4]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.4
 [1.1.5]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.5
 [1.1.6]: https://github.com/nlsfi/quality-result-gui/releases/tag/v1.1.6
 [2.0.0]: https://github.com/nlsfi/quality-result-gui/releases/tag/v2.0.0
+[2.0.1]: https://github.com/nlsfi/quality-result-gui/releases/tag/v2.0.1
```

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui.egg-info/SOURCES.txt` & `quality-result-gui-2.0.1/src/quality_result_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/__init__.py` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/__init__.py` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.py` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.ui` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/dev_tools_dialog.ui`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/example_quality_errors/quality_errors.json` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/example_quality_errors/quality_errors.json`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/mock_api_client.py` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/mock_api_client.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/dev_tools/response_parser.py` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/dev_tools/response_parser.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/env.py` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/env.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/metadata.txt` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/metadata.txt`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/plugin.py` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/__init__.py` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/i18n/fi.ts` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/resources/i18n/fi.ts`

 * *Files 16% similar despite different names*

#### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/i18n/fi.ts` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/resources/i18n/fi.ts`

```diff
@@ -1,127 +1,127 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
-<TS version="2.1">
+<TS version="2.1" language="fi_FI">
   <context>
     <name>@default</name>
     <message>
       <location filename="src/quality_result_gui/api/types/quality_error.py" line="36"/>
       <source>Attribute error</source>
-      <translation type="unfinished"/>
+      <translation>Attribuuttivirhe</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/api/types/quality_error.py" line="37"/>
       <source>Geometry error</source>
-      <translation type="unfinished"/>
+      <translation>Geometriavirhe</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/api/types/quality_error.py" line="38"/>
       <source>Topology error</source>
-      <translation type="unfinished"/>
+      <translation>Topologiavirhe</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/api/types/quality_error.py" line="39"/>
       <source>Continuity error</source>
-      <translation type="unfinished"/>
+      <translation>Jatkuvuusvirhe</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/api/types/quality_error.py" line="50"/>
       <source>Fatal</source>
-      <translation type="unfinished"/>
+      <translation>Hylkäävä</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/api/types/quality_error.py" line="51"/>
       <source>Warning</source>
-      <translation type="unfinished"/>
+      <translation>Vakava huomautus</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/api/types/quality_error.py" line="52"/>
       <source>Info</source>
-      <translation type="unfinished"/>
+      <translation>Info</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/quality_data_fetcher.py" line="49"/>
       <source>Checking for quality result updates</source>
-      <translation type="unfinished"/>
+      <translation>Päivitetään laatuajon tuloksia</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/quality_data_fetcher.py" line="50"/>
       <source>Quality check is in progress</source>
-      <translation type="unfinished"/>
+      <translation>Laatuajo on käynnissä</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/quality_data_fetcher.py" line="51"/>
       <source>Quality result update failed</source>
-      <translation type="unfinished"/>
+      <translation>Laatuajon tulosten päivittäminen epäonnistui</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/quality_data_fetcher.py" line="52"/>
       <source>Quality results are up to date</source>
-      <translation type="unfinished"/>
+      <translation>Laatuajon tulokset ovat päivitetty</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/quality_errors_filters.py" line="42"/>
       <source>Feature type</source>
-      <translation type="unfinished"/>
+      <translation>Kohdeluokan mukaan</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/quality_errors_filters.py" line="43"/>
       <source>Error type</source>
-      <translation type="unfinished"/>
+      <translation>Virhetyypin mukaan</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/quality_errors_filters.py" line="44"/>
       <source>Attribute Filter</source>
-      <translation type="unfinished"/>
+      <translation>Ominaisuustiedon mukaan</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/quality_errors_filters.py" line="114"/>
       <source>Select all</source>
-      <translation type="unfinished"/>
+      <translation>Valitse kaikki</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/quality_errors_filters.py" line="117"/>
       <source>Deselect all</source>
-      <translation type="unfinished"/>
+      <translation>Poista valinnat</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/quality_errors_tree_model.py" line="82"/>
       <source>Errors</source>
-      <translation type="unfinished"/>
+      <translation>Virheet</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/quality_errors_tree_model.py" line="83"/>
       <source>Error description</source>
-      <translation type="unfinished"/>
+      <translation>Virheen kuvaus</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/quality_error_manager.py" line="160"/>
       <source>Status of fetching quality result unknown</source>
-      <translation type="unfinished"/>
+      <translation>Laatuajon status ei tiedossa</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/quality_layer.py" line="95"/>
       <source>Quality errors</source>
-      <translation type="unfinished"/>
+      <translation>Laatuvirheet</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/ui/quality_errors_dock.py" line="76"/>
       <source>Toggle show errors on map filter</source>
-      <translation type="unfinished"/>
+      <translation>Näytä virheet kartalla</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui/ui/quality_errors_tree_filter_menu.py" line="44"/>
       <source>Reset filters</source>
-      <translation type="unfinished"/>
+      <translation>Palauta oletussuodatukset</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui_plugin/plugin.py" line="68"/>
       <source>Quality result GUI</source>
-      <translation type="unfinished"/>
+      <translation>Laatudialogi</translation>
     </message>
     <message>
       <location filename="src/quality_result_gui_plugin/plugin.py" line="76"/>
       <source>Development tools</source>
-      <translation type="unfinished"/>
+      <translation>Kehitystyökalut</translation>
     </message>
   </context>
 </TS>
```

### Comparing `quality-result-gui-2.0.0/src/quality_result_gui_plugin/resources/icons/quality_result_gui.svg` & `quality-result-gui-2.0.1/src/quality_result_gui_plugin/resources/icons/quality_result_gui.svg`

 * *Files identical despite different names*


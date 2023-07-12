# Comparing `tmp/ms-mint-app-0.2.3.2.tar.gz` & `tmp/ms-mint-app-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms-mint-app-0.2.3.2.tar", last modified: Thu Apr 27 18:52:19 2023, max compression
+gzip compressed data, was "ms-mint-app-0.3.0.tar", last modified: Wed Jul 12 16:39:53 2023, max compression
```

## Comparing `ms-mint-app-0.2.3.2.tar` & `ms-mint-app-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:52:19.319421 ms-mint-app-0.2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-27 18:52:19.319421 ms-mint-app-0.2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:52:19.323421 ms-mint-app-0.2.3.2/ms_mint_app/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-27 18:52:19.323421 ms-mint-app-0.2.3.2/ms_mint_app/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/add_metab.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/hierachical_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/ms_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/peak_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/quality_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:52:19.319421 ms-mint-app-0.2.3.2/ms_mint_app/static/
--rw-r--r--   0 runner    (1001) docker     (123)  9253590 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/static/ChEBI-Chem.parquet
--rw-r--r--   0 runner    (1001) docker     (123)  1058677 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/static/ChEBI-Groups.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/static/Standard_Peaklist.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:52:05.000000 ms-mint-app-0.2.3.2/ms_mint_app/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-27 18:52:06.000000 ms-mint-app-0.2.3.2/ms_mint_app/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)    22141 2023-04-27 18:52:06.000000 ms-mint-app-0.2.3.2/ms_mint_app/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-04-27 18:52:06.000000 ms-mint-app-0.2.3.2/ms_mint_app/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:52:19.311421 ms-mint-app-0.2.3.2/ms_mint_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-27 18:52:19.000000 ms-mint-app-0.2.3.2/ms_mint_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-27 18:52:19.000000 ms-mint-app-0.2.3.2/ms_mint_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:52:19.000000 ms-mint-app-0.2.3.2/ms_mint_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 18:52:19.000000 ms-mint-app-0.2.3.2/ms_mint_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 18:52:19.000000 ms-mint-app-0.2.3.2/ms_mint_app.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:52:19.319421 ms-mint-app-0.2.3.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-27 18:52:06.000000 ms-mint-app-0.2.3.2/scripts/Mint.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 18:52:19.323421 ms-mint-app-0.2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-27 18:52:06.000000 ms-mint-app-0.2.3.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-04-27 18:52:06.000000 ms-mint-app-0.2.3.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.311085 ms-mint-app-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-12 16:39:53.311085 ms-mint-app-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.311085 ms-mint-app-0.3.0/ms_mint_app/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-12 16:39:53.311085 ms-mint-app-0.3.0/ms_mint_app/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugin_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.299085 ms-mint-app-0.3.0/ms_mint_app/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/add_metabolites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.299085 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/hierachical_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/ms_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/target_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/plugins/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.307085 ms-mint-app-0.3.0/ms_mint_app/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  9253590 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/static/ChEBI-Chem.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)  1058677 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/static/ChEBI-Groups.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/static/Standard_Peaklist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:37.000000 ms-mint-app-0.3.0/ms_mint_app/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22254 2023-07-12 16:39:38.000000 ms-mint-app-0.3.0/ms_mint_app/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.295085 ms-mint-app-0.3.0/ms_mint_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-12 16:39:53.000000 ms-mint-app-0.3.0/ms_mint_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-12 16:39:53.000000 ms-mint-app-0.3.0/ms_mint_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:39:53.000000 ms-mint-app-0.3.0/ms_mint_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-12 16:39:53.000000 ms-mint-app-0.3.0/ms_mint_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 16:39:53.000000 ms-mint-app-0.3.0/ms_mint_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:39:53.307085 ms-mint-app-0.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-07-12 16:39:38.000000 ms-mint-app-0.3.0/scripts/Mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-12 16:39:53.311085 ms-mint-app-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-12 16:39:38.000000 ms-mint-app-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-07-12 16:39:38.000000 ms-mint-app-0.3.0/versioneer.py
```

### Comparing `ms-mint-app-0.2.3.2/LICENSE` & `ms-mint-app-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.2/PKG-INFO` & `ms-mint-app-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint-app
-Version: 0.2.3.2
+Version: 0.3.0
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint-app
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,14 +38,18 @@
 - describe accepted file types in ms_files tab
 - target-list add columns database_ref, formula, polarity
 - add descriptions to the optimization tab
 - total ion chromatogram (TIC)
 - full extracted ion chromatogram (EIC or XIC)
 - feature to convert intensities to concentrations
 
+### 0.2.3
+- update to pandas 2.0
+- faster processing of mzML and mzXML files
+
 ### 0.2.2
 - version strings in GUI
 - fixed issues with QC figures
 
 ### 0.2.1
 - uses ms-mint 0.2.1 with new implementation of `peak_area_top3`
 - new quality control tab
```

### Comparing `ms-mint-app-0.2.3.2/README.md` & `ms-mint-app-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 - describe accepted file types in ms_files tab
 - target-list add columns database_ref, formula, polarity
 - add descriptions to the optimization tab
 - total ion chromatogram (TIC)
 - full extracted ion chromatogram (EIC or XIC)
 - feature to convert intensities to concentrations
 
+### 0.2.3
+- update to pandas 2.0
+- faster processing of mzML and mzXML files
+
 ### 0.2.2
 - version strings in GUI
 - fixed issues with QC figures
 
 ### 0.2.1
 - uses ms-mint 0.2.1 with new implementation of `peak_area_top3`
 - new quality control tab
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/add_metab.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/add_metabolites.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,41 @@
 import os
 import pandas as pd
 
 from dash import html, dcc
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 from dash_tabulator import DashTabulator
+from pkg_resources import resource_filename
 
 import dash_bootstrap_components as dbc
 
 from ms_mint.standards import M_PROTON
-from . import tools as T
 
-from pkg_resources import resource_filename
+
+from .. import tools as T
+from ..plugin_interface import PluginInterface
+
+
+
+class AddMetabolitesPlugin(PluginInterface):
+    def __init__(self):
+        self._label = _label
+        self._order = 5
+
+    def layout(self):
+        return _layout
+
+    def callbacks(self, app, fsc, cache):
+        callbacks(app, fsc, cache)
+    
+    def outputs(self):
+        return _outputs
+
+
 
 CHEBI_CHEM_FN = os.path.abspath(
     resource_filename("ms_mint_app.static", "ChEBI-Chem.parquet")
 )
 CHEBI_GROUPS_FN = os.path.abspath(
     resource_filename("ms_mint_app.static", "ChEBI-Groups.parquet")
 )
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/analysis.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/analysis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,55 @@
 from dash import html, dcc
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 import dash_bootstrap_components as dbc
 
-from . import heatmap
-from . import pca
-from . import distributions
-from . import hierachical_clustering
-from . import plotting
-from . import tools as T
+from .analysis_tools import heatmap
+from .analysis_tools import pca
+from .analysis_tools import distributions
+from .analysis_tools import hierachical_clustering
+from .analysis_tools import plotting
+
+
+from .. import tools as T
+from ..plugin_interface import PluginInterface
+
+
+
+class AnalysisPlugin(PluginInterface):
+    def __init__(self):
+        self._label = _label
+        self._order = 9
+
+    def layout(self):
+        return _layout
+
+    def callbacks(self, app, fsc, cache):
+        callbacks(app, fsc, cache)
+    
+    def outputs(self):
+        return _outputs
+    
 
 
 _modules = [heatmap, distributions, pca, hierachical_clustering, plotting]
 
 modules = {module._label: module for module in _modules}
 
 groupby_options = [
-    {"label": "Batch", "value": "Batch"},
-    {"label": "Label", "value": "Label"},
-    {"label": "Type", "value": "Type"},
-    {"label": "Color", "value": "Color"},
+    {"label": "plate", "value": "plate"},
+    {"label": "label", "value": "label"},
+    {"label": "sample_type", "value": "sample_type"},
+    {"label": "color", "value": "color"},
 ]
 
 ana_normalization_cols = [
-    {"label": "Batch", "value": "Batch"},
+    {"label": "plate", "value": "plate"},
     {"label": "peak_label", "value": "peak_label"},
-    {"label": "ms_file", "value": "ms_file"},
+    {"label": "ms_file_id", "value": "ms_file_id"},
 ]
 
 _layout = html.Div(
     [
         dcc.Tabs(
             id="ana-secondary-tab",
             value=_modules[0]._label,
@@ -124,31 +144,31 @@
     )
     def file_types(tab, wdir):
         if tab != _label:
             raise PreventUpdate
         meta = T.get_metadata(wdir)
         if meta is None:
             raise PreventUpdate
-        file_types = meta["Type"].drop_duplicates().sort_values()
+        file_types = meta["sample_type"].drop_duplicates().sort_values()
         options = [{"value": str(i), "label": str(i)} for i in file_types]
         print(file_types, options)
         return options, file_types
 
     @app.callback(
         Output("ana-ms-order", "options"),
         Output("ana-groupby", "options"),
         Input("ana-secondary-tab", "value"),
         State("wdir", "children"),
     )
     def ms_order_options(tab, wdir):
         cols = T.get_metadata(wdir).dropna(how="all", axis=1).columns.to_list()
         if "index" in cols:
             cols.remove("index")
-        if "PeakOpt" in cols:
-            cols.remove("PeakOpt")
+        if "use_for_optimization" in cols:
+            cols.remove("use_for_optimization")
         options = [{"value": i, "label": i} for i in cols]
         return options, options
 
     @app.callback(
         Output("ana-peak-labels-include", "options"),
         Output("ana-peak-labels-exclude", "options"),
         Input("tab", "value"),
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/app.py` & `ms-mint-app-0.3.0/ms_mint_app/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import tempfile
 import logging
+import importlib
 
 import pandas as pd
 
 from pathlib import Path as P
 
 import matplotlib
 
@@ -16,35 +17,26 @@
 
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 from dash.dcc import Download
 from dash_extensions.enrich import FileSystemCache
 from dash.long_callback import DiskcacheLongCallbackManager
 
-
+from .plugin_manager import PluginManager
+from .plugin_interface import PluginInterface
 
 import dash_bootstrap_components as dbc
 
 from flask_caching import Cache
 from flask_login import current_user
 
 import ms_mint
 import ms_mint_app
 
 from . import tools as T
-
-from . import workspaces
-from . import ms_files
-from . import metadata
-from . import targets
-from . import peak_optimization
-from . import processing
-from . import add_metab
-from . import quality_control
-from . import analysis
 from . import messages
 
 import dash_uploader as du
 
 
 def make_dirs():
     tmpdir = tempfile.gettempdir()
@@ -75,35 +67,46 @@
 cache = diskcache.Cache(CACHEDIR)
 long_callback_manager = DiskcacheLongCallbackManager(
     cache, cache_by=[lambda: launch_uid], expire=60,
 )
 
 pd.options.display.max_colwidth = 1000
 
-_modules = [
-    workspaces,
-    ms_files,
-    metadata,
-    targets,
-    add_metab,
-    peak_optimization,
-    processing,
-    quality_control,
-    analysis,
-]
 
-modules = {module._label: module for module in _modules}
+def load_plugins(plugin_dir, package_name):
+    logging.info('Loading plugins')
+    plugins = {}
+
+    for file in os.listdir(plugin_dir):
+        if file.endswith(".py") and not file.startswith("__"):
+            module_name = file[:-3]
+            module_path = f"{package_name}.{module_name}"
+            module = importlib.import_module(module_path)
+
+            for name, cls in module.__dict__.items():
+                if isinstance(cls, type) and issubclass(cls, PluginInterface) and cls is not PluginInterface:
+                    plugin_instance = cls()
+                    plugins[plugin_instance.label] = plugin_instance
+
+    return plugins
+
+# Assuming 'plugins' is a subdirectory in the same directory as this script
+plugin_manager = PluginManager()
+plugins = plugin_manager.get_plugins()
+
+logging.info(f'Plugins: {plugins.keys()}')
 
 # Collect outputs:
 _outputs = html.Div(
     id="outputs",
-    children=[module._outputs for module in _modules if module._outputs is not None],
+    children=[plugin.outputs() for plugin in plugins.values() if plugin.outputs is not None],
     style={"visibility": "hidden"},
 )
 
+#logging.info(f'Outputs: {_outputs}')
 
 logout_button = (
     dbc.Button(
         "Logout",
         id="logout-button",
         style={"marginRight": "10px", "visibility": "hidden"},
     ),
@@ -156,27 +159,28 @@
             dbc.Col(
                 dbc.Alert(
                     [
                         html.H6(id="wdir", style={"display": "inline"}),
                     ]
                 , color='info', style={'text-align': 'center'}),
             ),
-        ], style={'margin-top': '5px', "margin-bottom": "30px"}),
+        ], style={'marginTop': '5px', "marginBottom": "30px"}),
 
         html.Div(id="pko-creating-chromatograms"),
+
         dcc.Tabs(
             id="tab",
-            value=_modules[0]._label,
+            value=list(plugins.keys())[0],
             children=[
                 dcc.Tab(
-                    id=modules[key]._label,
-                    value=key,
-                    label=modules[key]._label,
+                    id=plugin_id,
+                    value=plugin_id,
+                    label=plugin_instance.label,
                 )
-                for key in modules.keys()
+                for plugin_id, plugin_instance in plugins.items()
             ],
         ),
 
         messages.layout(),
 
         html.Div(id="pko-image-store", style={"visibility": "hidden", "height": "0px"}),
         html.Div(id="tab-content"),
@@ -195,19 +199,19 @@
     upload_root = os.getenv("MINT_DATA_DIR", tempfile.gettempdir())
     upload_dir = str(P(upload_root) / "MINT-Uploads")
     UPLOAD_FOLDER_ROOT = upload_dir
     du.configure_upload(app, UPLOAD_FOLDER_ROOT)
 
     messages.callbacks(app=app, fsc=fsc, cache=cache)
 
-    for module in _modules:
-        func = module.callbacks
-        if func is not None:
-            func(app=app, fsc=fsc, cache=cache)
+    for label, plugin in plugins.items():
+        logging.info(f"Loading callbacks of plugin {label}")
+        plugin.callbacks(app=app, fsc=fsc, cache=cache)
 
+    logging.info(f"Define clientside callbacks")
     # Updates the current viewport
     app.clientside_callback(
         """
         function(href) {
             var w = window.innerWidth;
             var h = window.innerHeight;
             return `${w},${h}` ;
@@ -219,15 +223,15 @@
 
     @app.callback(
         Output("tab-content", "children"),
         Input("tab", "value"),
         State("wdir", "children"),
     )
     def render_content(tab, wdir):
-        func = modules[tab].layout
+        func = plugins[tab].layout
         if tab != "Workspaces" and wdir == "":
             return dbc.Alert(
                 "Please, create and activate a workspace.", color="warning"
             )
         elif (
             tab in ["Metadata", "Peak Optimization", "Processing"]
             and len(T.get_ms_fns(wdir)) == 0
@@ -249,19 +253,21 @@
     )
     def upate_tmpdir(x):
         if hasattr(app.server, "login_manager"):
             username = current_user.username
             tmpdir = str(TMPDIR / "User" / username)
             return tmpdir, {"visibility": "visible"}
         return str(TMPDIR / "Local"), {"visibility": "hidden"}
+    logging.info("Done registering callbacks")
 
 
 def create_app(**kwargs):
-
-    logging.warning(f'ms-mint: {ms_mint.__version__}, ({ms_mint.__file__})')
+    logging.info('Create application')
+    logging.info(f'ms-mint: {ms_mint.__version__}, ({ms_mint.__file__})')
+    logging.info(f'ms-mint-app: {ms_mint_app.__version__}, ({ms_mint.__file__})')
 
     app = dash.Dash(
         __name__,
         long_callback_manager=long_callback_manager,
         external_stylesheets=[
             dbc.themes.MINTY,
             "https://codepen.io/chriddyp/pen/bWLwgP.css",
@@ -272,25 +278,16 @@
     app.layout = _layout
     app.title = "MINT"
     app.config["suppress_callback_exceptions"] = True
 
     upload_root = os.getenv("MINT_DATA_DIR", tempfile.gettempdir())
     CACHE_DIR = str(P(upload_root) / "MINT-Cache")
 
+    logging.info('Defining filesystem cache')
     cache = Cache(
         app.server, config={"CACHE_TYPE": "filesystem", "CACHE_DIR": CACHE_DIR}
     )
 
     fsc = FileSystemCache(str(CACHEDIR))
-
+    logging.info('Done creating app')
     return app, cache, fsc
 
-
-if __name__ == "__main__":
-    app, cache = create_app()
-    register_callbacks(app, cache)
-    app.run_server(
-        debug=True,
-        threaded=True,
-        dev_tools_hot_reload_interval=5000,
-        dev_tools_hot_reload_max_retry=30,
-    )
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/auth.py` & `ms-mint-app-0.3.0/ms_mint_app/auth.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/database.py` & `ms-mint-app-0.3.0/ms_mint_app/database.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/distributions.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/distributions.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import seaborn as sns
 
 from dash import html, dcc
 import dash_bootstrap_components as dbc
 from dash.exceptions import PreventUpdate
 from dash.dependencies import Input, Output, State
 
-from . import tools as T
+from ... import tools as T
 
 graph_options = [
     {"label": "Histograms", "value": "hist"},
     {"label": "Boxplots", "value": "boxplot"},
     {"label": "Probability Density", "value": "density"},
 ]
 
@@ -106,15 +106,15 @@
                 return dbc.Alert(
                     'For boxplots at least two groups have to be defined in selected "Group-by" column in metadata sheet.',
                     color="info",
                 )
 
         sns.set_context("paper")
 
-        sort_by_col = "Batch"
+        sort_by_col = "plate"
         quant_col = "log(peak_max+1)"
 
         if sort_by_col is not None:
             df = df.sort_values(["peak_label", sort_by_col])
 
         if options is None:
             options = []
@@ -133,58 +133,67 @@
 
             # Sorting to ensure similar legends
             if sort_by_col is not None:
                 grp = grp.sort_values(sort_by_col).reset_index(drop=True)
 
             # if len(grp) < 1:
             #    continue
-
             if "hist" in kinds:
-                sns.displot(data=grp, x=quant_col, height=3, hue=groupby, aspect=1)
-                plt.title(peak_label)
+                # define your figure and axis
+                fig, ax = plt.subplots(figsize=(3, 3))
+                
+                sns.histplot(data=grp, x=quant_col, hue=groupby, ax=ax)
+                ax.set_title(peak_label)
                 fig_label = f"by-{groupby}__{quant_col}__{peak_label}"
-                T.savefig(kind="hist", wdir=wdir, label=fig_label)
-                src = T.fig_to_src(dpi=150)
+                #T.savefig(fig, kind="hist", wdir=wdir, label=fig_label)
+                src = T.fig_to_src(fig, dpi=150)
                 figures.append(html.Img(src=src, style={"width": "300px"}))
 
             if "density" in kinds:
-                sns.displot(
-                    data=grp,
-                    x=quant_col,
-                    hue=groupby,
-                    kind="kde",
-                    common_norm=False,
-                    height=3,
-                    aspect=1,
-                )
-                plt.title(peak_label)
+                # define your figure and axis
+                fig, ax = plt.subplots(figsize=(3, 3))
+
+                for label, group_df in grp.groupby(groupby):
+                    sns.kdeplot(
+                        data=group_df,
+                        x=quant_col,
+                        ax=ax,
+                        label=label,
+                        common_norm=False,
+                    )
+                ax.set_title(peak_label)
+                ax.legend()
                 fig_label = f"by-{groupby}__{quant_col}__{peak_label}"
-                T.savefig(kind="density", wdir=wdir, label=fig_label)
-                src = T.fig_to_src(dpi=150)
+                #T.savefig(fig, kind="density", wdir=wdir, label=fig_label)
+                src = T.fig_to_src(fig, dpi=150)
                 figures.append(html.Img(src=src, style={"width": "300px"}))
 
             if "boxplot" in kinds:
                 n_groups = len(grp[groupby].drop_duplicates())
                 aspect = max(1, n_groups / 10)
-                sns.catplot(
+                
+                # define your figure and axis
+                fig, ax = plt.subplots(figsize=(aspect*3, 3))
+
+                sns.boxplot(
                     data=grp,
                     y=quant_col,
                     x=groupby,
-                    height=3,
-                    kind="box",
-                    aspect=aspect,
                     color="w",
+                    ax=ax
                 )
+
                 if quant_col in ["peak_max", "peak_area"]:
-                    plt.gca().ticklabel_format(axis="y", style="sci", scilimits=(0, 0))
-                plt.title(peak_label)
+                    ax.ticklabel_format(axis="y", style="sci", scilimits=(0, 0))
+
+                ax.set_title(peak_label)
                 plt.xticks(rotation=90)
                 fig_label = f"by-{groupby}__{quant_col}__{peak_label}"
-                T.savefig(kind="boxplot", wdir=wdir, label=fig_label)
-                src = T.fig_to_src(dpi=150)
+                #T.savefig(fig, kind="boxplot", wdir=wdir, label=fig_label)
+                src = T.fig_to_src(fig, dpi=150)
                 figures.append(html.Img(src=src, style={"width": "300px"}))
 
             if not "Dense" in options:
                 figures.append(dcc.Markdown("---"))
 
             # if i == 3: break
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/filelock.py` & `ms-mint-app-0.3.0/ms_mint_app/filelock.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/heatmap.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/heatmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 import dash_bootstrap_components as dbc
 
 from ms_mint.Mint import Mint
 from ms_mint.plotly_tools import plotly_heatmap
 
-from . import tools as T
+from ... import tools as T
 
 _label = "Heatmap"
 
 
 heatmap_options = [
     {"label": "Normalized by biomarker", "value": "normed_by_cols"},
     {"label": "Cluster", "value": "clustered"},
@@ -91,22 +91,23 @@
             file_types=file_types,
         )
 
         if len(df) == 0:
             return "No results yet. First run MINT."
 
         mint.results = df
-
+        mint.load_metadata(T.get_metadata_fn(wdir))
+        
         var_name = "peak_max"
         data = mint.crosstab(var_name)
         data.index = [T.Basename(i) for i in data.index]
 
         if ms_order is not None and len(ms_order) > 0:
             df = df.sort_values(ms_order)
-            ms_files = df["MS-file"].drop_duplicates()
+            ms_files = df["ms_file_id"].drop_duplicates()
             data = data.loc[ms_files]
 
         data.fillna(0, inplace=True)
 
         name = var_name
         if "log1p" in options:
             data = data.apply(np.log1p)
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/hierachical_clustering.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/hierachical_clustering.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,60 @@
 from dash import html, dcc
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 import dash_bootstrap_components as dbc
 
 from ms_mint.notebook import Mint
 
-from . import tools as T
+from ... import tools as T
 
 
 _label = "Hierachical Clustering"
 
 _options = ["Transposed"]
 
 options = [{"value": x, "label": x} for x in _options]
 
+metrics_options = [{"value": x, "label": x.capitalize()} for x in [
+    'braycurtis', 'canberra', 'chebyshev', 'cityblock', 'correlation', 'cosine',
+    'dice', 'euclidean', 'hamming', 'jaccard', 'jensenshannon', 'kulsinski',
+    'mahalanobis', 'matching', 'minkowski', 'rogerstanimoto', 'russellrao',
+    'seuclidean', 'sokalmichener', 'sokalsneath', 'sqeuclidean', 'yule']
+]
+
+
+
 _layout = html.Div(
     [
         html.H3(_label),
-        dcc.Input(
-            id="hc-figsize-x", placeholder="Figure size x", value=8, type="number"
-        ),
-        dcc.Input(
-            id="hc-figsize-y", placeholder="Figure size x", value=8, type="number"
-        ),
-        dcc.Dropdown(id="hc-options", options=options, value=[]),
+        dbc.Row([
+            dbc.Col([
+                dbc.Row([
+                    dbc.Label('Figure width'),
+                    dcc.Input(
+                        id="hc-figsize-x", placeholder="Figure size x", value=8, type="number"
+                    ),
+                    dbc.Label('Figure height'),
+                    dcc.Input(
+                        id="hc-figsize-y", placeholder="Figure size x", value=8, type="number"
+                    ),
+                    dbc.Label('Options'), 
+                    dcc.Dropdown(id="hc-options", options=options, value=[]),
+                ]),
+
+            ]),      
+            
+            dbc.Col([
+                dbc.Row([dbc.Label('Metric X'), dcc.Dropdown(id='hc-metric-x', options=metrics_options, value='cosine')]),
+                dbc.Row([dbc.Label('Metric Y'), dcc.Dropdown(id='hc-metric-y', options=metrics_options, value='cosine')]),
+            ]),            
+        ]),
+
         dbc.Button("Update", id="hc-update"),
+
         dcc.Loading(
             html.Div(
                 id="hc-figures",
                 style={
                     "margin": "auto",
                     "text-align": "center",
                     "maxWidth": "100%",
@@ -46,25 +72,29 @@
     return _layout
 
 
 def callbacks(app, fsc, cache):
     @app.callback(
         Output("hc-figures", "children"),
         Input("hc-update", "n_clicks"),
+        State("hc-metric-x", "value"),
+        State("hc-metric-y", "value"),        
         State("hc-figsize-x", "value"),
         State("hc-figsize-y", "value"),
         State("hc-options", "value"),
         State("ana-file-types", "value"),
         State("ana-peak-labels-include", "value"),
         State("ana-peak-labels-exclude", "value"),
         State("ana-ms-order", "value"),
         State("wdir", "children"),
     )
     def create_figure(
         n_clicks,
+        metrix_x,
+        metrix_y,
         fig_size_x,
         fig_size_y,
         options,
         file_types,
         include_labels,
         exclude_labels,
         ms_order,
@@ -73,16 +103,14 @@
 
         if n_clicks is None:
             raise PreventUpdate
 
         if options is None: 
             options = []
         
-        print(options)
-
         mint = Mint()
 
         if fig_size_x is None:
             fig_size_x = 8
         if fig_size_y is None:
             fig_size_y = 8
 
@@ -91,18 +119,19 @@
 
         df = T.get_complete_results(
             wdir,
             include_labels=include_labels,
             exclude_labels=exclude_labels,
             file_types=file_types,
         )
-
-        df["ms_file"] = df["MS-file"]
+    
+        df["ms_file"] = df["ms_file_label"]
         mint.results = df
+        mint.load_metadata(T.get_metadata_fn(wdir))
 
-        mint.plot.hierarchical_clustering(
-            figsize=(fig_size_x, fig_size_y), transposed="Transposed" in options
+        fig = mint.plot.hierarchical_clustering(
+            figsize=(fig_size_x, fig_size_y), transposed="Transposed" in options, metric=(metrix_x, metrix_y)
         )
 
-        src = T.fig_to_src()
+        src = T.fig_to_src(fig.figure)
 
         return html.Img(src=src, style={"maxWidth": "80%"})
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/messages.py` & `ms-mint-app-0.3.0/ms_mint_app/messages.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/metadata.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,32 @@
 import dash_bootstrap_components as dbc
 from dash_extensions.javascript import Namespace
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 
 from dash_tabulator import DashTabulator
 
-from . import tools as T
+from .. import tools as T
+from ..plugin_interface import PluginInterface
 
 
+class MetadataPlugin(PluginInterface):
+    def __init__(self):
+        self._label = _label
+        self._order = 3
+
+    def layout(self):
+        return _layout
+
+    def callbacks(self, app, fsc, cache):
+        callbacks(app, fsc, cache)
+    
+    def outputs(self):
+        return _outputs
+
 ns = Namespace("myNamespace", "tabulator")
 
 tabulator_options = {
     "groupBy": "Label",
     "selectable": True,
     "headerFilterLiveFilterDelay": 3000,
     "layout": "fitDataFill",
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/ms_files.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/ms_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,31 @@
 
 from ms_mint.io import convert_ms_file_to_feather
 
 from dash_tabulator import DashTabulator
 
 import dash_uploader as du
 
-from . import tools as T
+from .. import tools as T
+from ..plugin_interface import PluginInterface
+
+
+class MsFilesPlugin(PluginInterface):
+    def __init__(self):
+        self._label = _label
+        self._order = 2
+
+    def layout(self):
+        return _layout
+
+    def callbacks(self, app, fsc, cache):
+        callbacks(app, fsc, cache)
+    
+    def outputs(self):
+        return _outputs
 
 
 upload_root = os.getenv("MINT_DATA_DIR", tempfile.gettempdir())
 upload_dir = str(P(upload_root) / "MINT-Uploads")
 UPLOAD_FOLDER_ROOT = upload_dir
 
 
@@ -48,25 +64,25 @@
         },
         "hozAlign": "center",
         "headerSort": False,
         "width": "1px",
         "frozen": True,
     },
     {
-        "title": "MS-file",
-        "field": "MS-file",
+        "title": "ms_file",
+        "field": "ms_file",
         "headerFilter": True,
         "headerSort": True,
         "editor": None,
         "width": "80%",
         "sorter": "string",
         "frozen": True,
     },
     {
-        "title": "Size [MB]",
+        "title": "ms_file_size_mb",
         "field": "file_size",
         "headerFilter": True,
         "headerSort": True,
         "editor": None,
         "width": "20%",
         "sorter": "string",
         "frozen": True,
@@ -112,24 +128,25 @@
                 cancel_button=True,
                 text="Upload mzXML/mzML files.",
             ),
             style={
                 "textAlign": "center",
                 "width": "100%",
                 "padding": "0px",
-                "margin-bottom": "20px",
+                "marginBottom": "20px",
                 "display": "inline-block",
             },
         ),
         dcc.Markdown("##### Actions"),
         dbc.Row(
             [
                 dbc.Col(
                     [
                         dbc.Button("Convert selected files to Feather", id="ms-convert"),
+                        dbc.Button("Convert selected files to Parquet", id="ms-convert-parquet"),
                     ]
                 ),
                 dbc.Col(
                     [
                         dbc.Button("Delete selected files", id="ms-delete", color='danger')
                     ]
                 , style={"text-align": 'right'}),
@@ -168,18 +185,19 @@
         Input({"index": "ms-delete-output", "type": "output"}, "children"),
         Input({"index": "ms-convert-output", "type": "output"}, "children"),
         State("active-workspace", "children"),
     )
     def ms_table(value, wdir, files_deleted, files_converted, workspace):
 
         ms_files = T.get_ms_fns(wdir)
-
+        logging.info(f'# Files in {wdir} {workspace} {len(ms_files)}')
+        
         data = pd.DataFrame(
             {
-                "MS-file": [os.path.basename(fn) for fn in ms_files],
+                "ms_file": [os.path.basename(fn) for fn in ms_files],
                 "file_size": [
                     np.round(os.path.getsize(fn) / 1024 / 1024, 2) for fn in ms_files
                 ],
             }
         )
 
         downloadButtonType = {
@@ -197,15 +215,15 @@
         State("ms-table", "multiRowsClicked"),
         State("wdir", "children"),
     )
     def ms_convert(n_clicks, rows, wdir):
         target_dir = os.path.join(wdir, "ms_files")
         if n_clicks is None:
             raise PreventUpdate
-        fns = [row["MS-file"] for row in rows]
+        fns = [row["ms_file"] for row in rows]
         fns = [fn for fn in fns if not fn.endswith(".feather")]
         fns = [os.path.join(target_dir, fn) for fn in fns]
         n_total = len(fns)
         for i, fn in enumerate(fns):
             fsc.set("progress", int(100 * (i + 1) / n_total))
             new_fn = convert_ms_file_to_feather(fn)
             if os.path.isfile(new_fn):
@@ -219,15 +237,15 @@
         State("wdir", "children"),
     )
     def ms_delete(n_clicks, rows, wdir):
         if n_clicks is None:
             raise PreventUpdate
         target_dir = os.path.join(wdir, "ms_files")
         for row in rows:
-            fn = row["MS-file"]
+            fn = row["ms_file"]
             fn = P(target_dir) / fn
             os.remove(fn)
         return dbc.Alert(f"{len(rows)} files deleted", color="info")
 
 
     @du.callback(
         output=Output('ms-uploader-fns', 'children'),
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/pca.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/pca.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,93 +6,90 @@
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 
 import dash_bootstrap_components as dbc
 
 from ms_mint import Mint
 
-from . import tools as T
+from ... import tools as T
 
 options = [{"value": i, "label": i} for i in ["Standard scaling", "Corner"]]
 
 _layout = html.Div(
     [
         html.H3("Principal Components Analysis"),
         dbc.Button("Run PCA", id="pca-update"),
         dcc.Dropdown(
             id="pca-options",
             options=options,
             value=["Standard scaling"],
             multi=True,
             placeholder="Scaling used before PCA",
         ),
+
         html.Label("Number of PCA components"),
         dcc.Slider(
             id="pca-nvars",
             value=3,
             min=2,
             max=10,
             step=1,
             marks={i: f"{i}" for i in range(2, 11)},
         ),
-        html.Label("Height of facets"),
-        dcc.Slider(
-            id="pca-facent-height",
-            value=2.5,
-            min=1,
-            max=5,
-            step=0.1,
-            marks={i: f"{i}" for i in np.arange(1, 5.5, 0.5)},
-        ),
-        html.H4("Cumulative explained variance"),
-        dcc.Loading(
-            html.Div(
-                id="pca-figure-explained-variance",
-                style={"margin": "auto", "text-align": "center"},
-            )
-        ),
+
         html.H4("Scatter plot of principal components"),
-        dcc.Loading(
-            html.Div(
-                id="pca-figure-pairplot",
-                style={"margin": "auto", "text-align": "center"},
-            )
-        ),
-        html.H4("Principal components compositions"),
-        dcc.Loading(dcc.Graph(id="pca-figure-contrib")),
+        html.Center([
+            dcc.Loading(
+                dcc.Graph(
+                    id="pca-figure-pairplot",
+                )
+            ),
+        ]),
+
+        html.H4("Cumulative explained variance"),
+        html.Center([
+            dcc.Loading(
+                dcc.Graph(
+                    id="pca-figure-explained-variance",
+                )
+            ),
+        ]),
+    
+        html.H4("PCA-Loadings"),
+        html.Center([
+            dcc.Loading(dcc.Graph(id="pca-figure-contrib")),
+        ]),
     ]
 )
 
 _label = "PCA"
 
 
 def layout():
     return _layout
 
 
 def callbacks(app, fsc, cache):
     @app.callback(
-        Output("pca-figure-explained-variance", "children"),
-        Output("pca-figure-pairplot", "children"),
+        Output("pca-figure-pairplot", "figure"),
+        Output("pca-figure-explained-variance", "figure"),
         Output("pca-figure-contrib", "figure"),
         Input("pca-update", "n_clicks"),
         State("pca-nvars", "value"),
-        State("pca-facent-height", "value"),
         State("ana-groupby", "value"),
         State("ana-peak-labels-include", "value"),
         State("ana-peak-labels-exclude", "value"),
         State("ana-normalization-cols", "value"),
         State("ana-file-types", "value"),
         State("pca-options", "value"),
         State("wdir", "children"),
     )
     def create_pca(
         n_clicks,
         n_components,
-        facet_height,
         groupby,
         include_labels,
         exclude_labels,
         norm_cols,
         file_types,
         options,
         wdir,
@@ -106,19 +103,19 @@
             wdir,
             include_labels=include_labels,
             exclude_labels=exclude_labels,
             file_types=file_types,
         )
 
         if file_types is not None and len(file_types) > 0:
-            df = df[df["Type"].isin(file_types)]
+            df = df[df["sample_type"].isin(file_types)]
 
         if groupby is not None and len(groupby) > 0:
             labels = (
-                df[["ms_file", groupby]].drop_duplicates().set_index("ms_file")
+                df[["ms_file_label", groupby]].drop_duplicates().set_index("ms_file_label")
             )
         else:
             labels = None
             groupby = None
 
         if len(norm_cols) != 0:
             if ("peak_label" in norm_cols) and ("ms_file" in norm_cols):
@@ -139,44 +136,33 @@
                 )
                 / df[cols + norm_cols].groupby(norm_cols).transform("std")[cols].values
             ).reset_index()
 
         figures = []
         mint = Mint()
         mint.results = df
-        mint.pca.run(n_components=n_components)
-
-        ndx = mint.pca.results["df_projected"].index.to_list()
-        mint.pca.plot.cumulative_variance()
+        mint.load_metadata(T.get_metadata_fn(wdir))
 
-        src = T.fig_to_src()
-
-        figures.append(html.Img(src=src))
-
-        if labels is not None:
-            labels = labels.loc[ndx].values
+        mint.pca.run(n_components=n_components)
 
-        with sns.plotting_context("paper"):
-            mint.pca.plot.pairplot(
+        fig_scattermatrix = mint.pca.plot.pairplot(
                 n_components=n_components,
-                labels=labels,
-                height=facet_height,
-                corner="Corner" in options,
+                hue=groupby,
+                interactive=True,
+                height=n_components*200+100,
+                width=n_components*200+100,
+                title='Principal components scatter plot',
+                diag='box'
             )
 
-        src = T.fig_to_src()
-        figures.append(html.Img(src=src))
+        fig_cumvar = mint.pca.plot.cumulative_variance(interactive=True, width=n_components*20+500)
 
-        contrib = mint.pca.results["feature_contributions"]
-
-        fig_contrib = px.bar(
-            data_frame=contrib,
-            x="peak_label",
-            y="Coefficient",
-            facet_col="PC",
-            facet_col_wrap=1,
-            height=200 * n_components + 200,
-        )
+        fig_contrib = mint.pca.plot.loadings(interactive=True, 
+                                             height=n_components*200+100, 
+                                             width=len(mint.targets)*20+500,
+                                             title='Principal component loadings')
 
+        fig_scattermatrix.update_layout(autosize=True)
+        fig_cumvar.update_layout(autosize=True)        
         fig_contrib.update_layout(autosize=True)
 
-        return figures[0], figures[1], fig_contrib
+        return fig_scattermatrix, fig_cumvar, fig_contrib
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/peak_optimization.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/target_optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,31 @@
 
 import dash_bootstrap_components as dbc
 
 import plotly.graph_objects as go
 
 from ms_mint import Mint
 
-from . import tools as T
+from .. import tools as T
+from ..plugin_interface import PluginInterface
+
+
+class TargetOptimizationPlugin(PluginInterface):
+    def __init__(self):
+        self._label = _label
+        self._order = 6
+
+    def layout(self):
+        return _layout
+
+    def callbacks(self, app, fsc, cache):
+        callbacks(app, fsc, cache)
+    
+    def outputs(self):
+        return _outputs
 
 
 info_txt = """
 Creating chromatograms from mzXML/mzML files can last 
 a long time the first time. Try converting your files to 
 _feather_ format first.'
 """
@@ -39,15 +55,15 @@
         html.H3("Target Optimization"),
         dcc.Markdown("---"),
         html.H4("File selection"),
         dcc.Dropdown(
             id="pko-ms-selection",
             options=[
                 {
-                    "label": "Use selected files from metadata table (PeakOpt)",
+                    "label": "Use selected files from metadata table (use_for_optimization)",
                     "value": "peakopt",
                 },
                 {"label": "Use all files (may take a long time)", "value": "all"},
             ],
             value="peakopt",
             clearable=False,
             style={'max-width': '400px'}
@@ -77,15 +93,15 @@
             style={"marginBottom": "20px", "width": "100%"},
         ),
 
         dbc.Row([
             dbc.Col(dbc.Button("Set RT to current view", id="pko-set-rt", style={"width": "100%"})),
             dbc.Col(dbc.Button("Detect rt_min,rt_max", id="pko-detect-rtmin-rtmax", style={"width": "100%"})),
             dbc.Col(dbc.Button("Confirm retention time", id="pko-confirm-rt", style={"width": "100%"})),
-            dbc.Col(dbc.Button("Remove Peak", id="pko-delete", style={"width": "100%"}, color='danger')),
+            dbc.Col(dbc.Button("Remove target", id="pko-delete", style={"width": "100%"}, color='danger')),
         ]),
 
         dcc.Loading(dcc.Graph("pko-figure")),
         dcc.Checklist(
             id="pko-figure-options",
             options=[{"value": "log", "label": "Logarithmic y-scale"}],
             value=[],
@@ -103,15 +119,15 @@
 )
 
 
 pko_layout_no_data = html.Div(
     [
         dcc.Markdown(
             """### No targets found.
-    You did not generate a targets yet.
+    You did not genefrate a targets yet.
     """
         )
     ]
 )
 
 
 _outputs = html.Div(
@@ -268,17 +284,17 @@
         if ms_selection == "peakopt":
             ms_files = T.get_ms_fns_for_peakopt(wdir)
 
         elif ms_selection == "all":
             ms_files = T.get_ms_fns(wdir)
 
         mint = Mint()
-        mint.targets = targets.reset_index()
+        mint.targets = targets
         mint.ms_files = ms_files
-        mint.opt.rt_min_max(sigma=1000)       
+        mint.opt.rt_min_max(rel_height=0.8)       
         new_targets = mint.targets
 
         T.write_targets(new_targets, wdir)
 
         return dbc.Alert("Rt detection finished.", color="success")
 
     @app.callback(
@@ -380,15 +396,15 @@
         Output("pko-peak-preview-images", "children"),
         Input("pko-peak-preview", "n_clicks"),
         Input("pko-peak-preview-from-scratch", "n_clicks"),
         State("pko-ms-selection", "value"),
         State("wdir", "children"),
     )
     def peak_preview(n_clicks, from_scratch, ms_selection, wdir):  # peak_opt, #set_rt,
-        logging.warning(f'Create peak previews {wdir}')
+        logging.info(f'Create peak previews {wdir}')
         if n_clicks is None:
             raise PreventUpdate
         # reset updating after 5 attempts
         n_attempts = fsc.get(f"{wdir}-update-attempt")
         if n_attempts is None:
             n_attempts = 1
         elif n_attempts % 5:
@@ -414,15 +430,15 @@
         elif ms_selection == "all":
             ms_files = T.get_ms_fns(wdir)
         else:
             assert False, ms_selection
 
         if len(ms_files) == 0:
             return dbc.Alert(
-                'No files selected for peak optimization in Metadata tab. Please, select some files in column "PeakOpt".',
+                'No files selected for peak optimization in Metadata tab. Please, select some files in column "use_for_optimization".',
                 color="warning",
             )
         else:
             logging.info(
                 f"Using {len(ms_files)} files for peak preview. ({ms_selection})"
             )
 
@@ -539,46 +555,49 @@
             ms_files = T.get_ms_fns(wdir)
 
         peak_label = targets.at[peak_label_ndx, 'peak_label']
         
         mint = Mint()
         mint.targets = targets
         mint.ms_files = ms_files
-        mint.opt.rt_min_max(peak_labels=[peak_label])
+        mint.opt.rt_min_max(peak_labels=[peak_label], rel_height=0.8)
         new_targets = mint.targets
-        new_targets.to_csv(T.get_targets_fn(wdir), index=False)
+        T.write_targets(new_targets, wdir)
 
         return dbc.Alert(
             f"Done optimize rt_min rt_max for {peak_label}", color="info"
         )
         
 
 def create_preview_peakshape(
     ms_files, mz_mean, mz_width, rt, rt_min, rt_max, image_label, wdir, peak_label, colors
 ):
     """Create peak shape previews."""
-    plt.figure(figsize=(2, 1), dpi=30)
+    logging.info(f'Create_preview_peakshape {peak_label}')
+    fig, ax = plt.subplots(figsize=(2, 1), dpi=30)
     y_max = 0
     for fn in ms_files:
         color = colors[T.filename_to_label(fn)]
         if color is None or color == "":
             color = "grey"
         fn_chro = T.get_chromatogram(fn, mz_mean, mz_width, wdir)
         fn_chro = fn_chro[
             (rt_min < fn_chro["scan_time"]) & (fn_chro["scan_time"] < rt_max)
         ]
-        plt.plot(fn_chro["scan_time"], fn_chro["intensity"], lw=1, color=color)
+        ax.plot(fn_chro["scan_time"], fn_chro["intensity"], lw=1, color=color)
         y_max = max(y_max, fn_chro["intensity"].max())
     if (not np.isnan(rt)) and not (np.isnan(rt_max)) and not (np.isnan(rt_min)):
         x = max(min(rt, rt_max), rt_min)
         rt_mean = np.mean([rt_min, rt_max])
         color_value = np.abs(rt_mean - rt) / 10
         color = T.float_to_color(color_value, vmin=0, vmax=1, cmap="coolwarm")
-        plt.vlines(x, 0, y_max, lw=3, color=color)
+        ax.vlines(x, 0, y_max, lw=3, color=color)
     title = f'{peak_label[:30]}\nm/z={mz_mean:.2f}'
-    plt.gca().set_title(title, y=1.0, pad=15)
-    plt.gca().ticklabel_format(axis="y", style="sci", scilimits=(0, 0))
-    plt.xlabel("Scan Time [s]")
-    plt.ylabel("Intensity")
-    filename = T.savefig(kind="peak-preview", wdir=wdir, label=image_label)
-    plt.close()
+    ax.set_title(title, y=1.0, pad=15)
+    ax.ticklabel_format(axis="y", style="sci", scilimits=(0, 0))
+    ax.set_xlabel("Scan Time [s]")
+    ax.set_ylabel("Intensity")
+    filename = T.savefig(fig, kind="peak-preview", wdir=wdir, label=image_label)
+    plt.close(fig)
+    logging.info(f'Create_preview_peakshape {peak_label} done.')
     return filename
+
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/plotting.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/analysis_tools/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from matplotlib import pyplot as plt
 
 import seaborn as sns
 
 plt.rcParams["figure.autolayout"] = False
 
 
-from . import tools as T
+from ... import tools as T
 
 
 _label = "Plotting"
 
 _kinds = [
     "bar",
     "violin",
@@ -284,15 +284,15 @@
                     "minHeight": "300px",
                 },
             )
         ),
     ]
 )
 
-_ouptuts = html.Div([])
+_outputs = html.Div([])
 
 
 def layout():
     return _layout
 
 
 def callbacks(app, fsc, cache, cpu=None):
@@ -312,15 +312,15 @@
             raise PreventUpdate
         results = T.get_complete_results(wdir)
         results = results.dropna(axis=1, how="all")
         cols = results.columns
         options = [{"value": x, "label": x} for x in cols]
         return [options] * 7
 
-    @app.long_callback(
+    @app.callback(
         Output("plot-figures", "children"),
         Input("plot-update", "n_clicks"),
         State("plot-kind", "value"),
         State("plot-fig-height", "value"),
         State("plot-fig-aspect", "value"),
         State("plot-x", "value"),
         State("plot-y", "value"),
@@ -486,10 +486,10 @@
             g.set_xticklabels(rotation=90)
 
         if title is not None:
             g.fig.suptitle(title, y=1.01)
 
         g.tight_layout(w_pad=0)
 
-        src = T.fig_to_src(dpi=300 if "HQ" in options else None)
+        src = T.fig_to_src(g.fig, dpi=300 if "HQ" in options else None)
 
         return html.Img(src=src, style={"maxWidth": "80%"})
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/processing.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/processing.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,33 @@
 from dash.exceptions import PreventUpdate
 from dash.dcc import send_file, send_bytes
 
 from dash.dependencies import Input, Output, State
 
 from ms_mint.Mint import Mint
 
-from . import tools as T
+from .. import tools as T
+from ..plugin_interface import PluginInterface
+
+
+
+class ProcessingPlugin(PluginInterface):
+    def __init__(self):
+        self._label = _label
+        self._order = 7
+
+    def layout(self):
+        return _layout
+
+    def callbacks(self, app, fsc, cache):
+        callbacks(app, fsc, cache)
+    
+    def outputs(self):
+        return _outputs
+    
 
 _label = "Processing"
 
 
 _layout = html.Div(
     [
         html.H3("Run MINT"),
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/quality_control.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/quality_control.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,32 @@
 import numpy as np
 import seaborn as sns
 import matplotlib.pyplot as plt 
 import contextlib
 
 from ms_mint import Mint
 
-from . import tools as T
+from .. import tools as T
+from ..plugin_interface import PluginInterface
+
+
+class QualityControlPlugin(PluginInterface):
+    def __init__(self):
+        self._label = _label
+        self._order = 8
+
+    def layout(self):
+        return _layout
+
+    def callbacks(self, app, fsc, cache):
+        callbacks(app, fsc, cache)
+    
+    def outputs(self):
+        return _outputs
+    
 
 _label = "Quality Control"
 
 _layout = html.Div([
     html.H1('Quality Control'),
     html.H2('m/z drift'),
     html.H3('Overall'),
@@ -96,15 +113,15 @@
         if tab != "Quality Control":
             raise PreventUpdate
         
         df = T.get_complete_results(
             wdir
         )
 
-        return px.violin(data_frame=df, y='peak_mass_diff_50pc', color='Type')
+        return px.violin(data_frame=df, y='peak_mass_diff_50pc', color='sample_type')
         
     
     @app.callback(
         Output("qc-fig-mz-drift-by-target", "figure"),
         Input("tab", "value"),
         State("wdir", "children"),
     )
@@ -118,15 +135,15 @@
         df = T.get_complete_results(
             wdir
         )
 
         fig = px.scatter(data_frame=df, 
                          y='peak_mass_diff_50pc', 
                          x='peak_label',
-                         color='Type', 
+                         color='sample_type', 
                          hover_data=['ms_file'],
                          #facet_col_wrap=10, 
                          height=750
                 )
         fig.update_xaxes(automargin = True)
         return fig
 
@@ -140,28 +157,22 @@
         tab,
         wdir,
     ):
 
         if tab != "Quality Control":
             raise PreventUpdate
 
-        meta = T.get_metadata(wdir).set_index('MS-file')
-
         mint = Mint()
         mint.load(T.get_results_fn(wdir))
-        mint.pca.run(4)
-
-        ndx = mint.pca.results["df_projected"].index.to_list()
-        ndx = [P(e).with_suffix('').name for e in ndx]
-
-        labels = list(meta.loc[ndx].Type)
+        mint.load_metadata(T.get_metadata_fn(wdir))
 
+        mint.pca.run(4)
 
         fig = mint.pca.plot.pairplot(interactive=True, 
-                                     labels=labels,
+                                     hue='sample_type',
                                      height=1000, 
                                      width=1000, 
                                      diag='box')
         return fig
 
 
     @app.callback(
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/static/ChEBI-Chem.parquet` & `ms-mint-app-0.3.0/ms_mint_app/static/ChEBI-Chem.parquet`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/static/ChEBI-Groups.parquet` & `ms-mint-app-0.3.0/ms_mint_app/static/ChEBI-Groups.parquet`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/targets.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/targets.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,32 @@
 import dash
 from dash import html, dcc
 from dash.dependencies import Input, Output, State
 from dash_tabulator import DashTabulator
 
 import dash_bootstrap_components as dbc
 
-from . import tools as T
+from .. import tools as T
+from ..plugin_interface import PluginInterface
+
+
+class TargetsPlugin(PluginInterface):
+    def __init__(self):
+        self._label = _label
+        self._order = 4
+
+    def layout(self):
+        return _layout
+
+    def callbacks(self, app, fsc, cache):
+        callbacks(app, fsc, cache)
+    
+    def outputs(self):
+        return _outputs
+    
 
 from ms_mint.standards import TARGETS_COLUMNS
 
 INFO = dcc.Markdown(
 """
 ---
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/tools.py` & `ms-mint-app-0.3.0/ms_mint_app/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -216,31 +216,25 @@
         for ndx, row in targets.iterrows():
             mz_mean, mz_width = row[["mz_mean", "mz_width"]]
             fn_chro = get_chromatogram_fn(fn, mz_mean, mz_width, wdir)
             if not os.path.isfile(fn_chro):
                 create_chromatogram(fn, mz_mean, mz_width, fn_chro)
 
 
-def create_chromatogram(ms_file, mz_mean, mz_width, fn_out, verbose=False):
-    if verbose:
-        print("Creating chromatogram")
+def create_chromatogram(ms_file, mz_mean, mz_width, fn_out):
     df = ms_file_to_df(ms_file)
-    if verbose:
-        print("...file read")
     dirname = os.path.dirname(fn_out)
     if not os.path.isdir(dirname):
         os.makedirs(dirname)
     dmz = mz_mean * 1e-6 * mz_width
     chrom = df[(df["mz"] - mz_mean).abs() <= dmz]
     chrom["scan_time"] = chrom["scan_time"].round(3)
     chrom = chrom.groupby("scan_time").max().reset_index()
     with lock(fn_out):
         chrom[["scan_time", "intensity"]].to_feather(fn_out)
-    if verbose:
-        print("...done creating chromatogram.")
     return chrom
 
 
 def get_chromatogram(ms_file, mz_mean, mz_width, wdir):
     fn = get_chromatogram_fn(ms_file, mz_mean, mz_width, wdir)
     if not os.path.isfile(fn):
         chrom = create_chromatogram(ms_file, mz_mean, mz_width, fn)
@@ -315,96 +309,96 @@
 def get_results_fn(wdir):
     return os.path.join(wdir, "results", "results.csv")
 
 
 def get_results(wdir):
     fn = get_results_fn(wdir)
     df = pd.read_csv(fn)
-    df["MS-file"] = [filename_to_label(fn) for fn in df["ms_file"]]
+    df["ms_file_label"] = [filename_to_label(fn) for fn in df["ms_file"]]
     return df
 
 
 def get_metadata(wdir):
     fn = get_metadata_fn(wdir)
     fn_path = os.path.dirname(fn)
     ms_files = get_ms_fns(wdir, abs_path=False)
     ms_files = [filename_to_label(fn) for fn in ms_files]
     df = None
     if not os.path.isdir(fn_path):
         os.makedirs(fn_path)
     if os.path.isfile(fn):
         df = pd.read_csv(fn)
-        if "MS-file" not in df.columns:
+        if "ms_file_label" not in df.columns:
             df = None
 
     if df is None or len(df) == 0:
         df = init_metadata(ms_files)
 
     for col in [
-        "Color",
-        "Column",
-        "Row",
-        "Batch",
-        "Label",
-        "InAnalysis",
-        "PeakOpt",
-        "MS-file",
+        "color",
+        "plate_column",
+        "plate_row",
+        "plate",
+        "label",
+        "in_analysis",
+        "use_for_optimization",
+        "ms_file_label",
+        "ms_column",
+        "ionization_mode",
     ]:
         if col not in df.columns:
             df[col] = None
 
-    df = df[df["MS-file"] != ""]
+    df = df[df["ms_file_label"] != ""]
 
-    new_files = [e for e in ms_files if e not in df['MS-file'].values]
+    new_files = [e for e in ms_files if e not in df['ms_file_label'].values]
 
-    df = df.groupby("MS-file").first().reindex(ms_files, ).reset_index()
+    df = df.groupby("ms_file_label").first().reindex(ms_files, ).reset_index()
     
-    print('NEW FILES:', new_files)
     if new_files :
-        # Default for PeakOpt for new files should be False
-        ndx = df[df['MS-file'].isin(new_files)].index
-        print('INDEX:', ndx)
-        df.loc[ndx, 'PeakOpt'] = False
+        # Default for use_for_optimization for new files should be False
+        ndx = df[df['ms_file_label'].isin(new_files)].index
+        df.loc[ndx, 'use_for_optimization'] = False
 
-    if "PeakOpt" not in df.columns:
-        df["PeakOpt"] = False
+    if "use_for_optimization" not in df.columns:
+        df["use_for_optimization"] = False
 
     else:
-        df["PeakOpt"] = df["PeakOpt"].astype(bool)
+        df["use_for_optimization"] = df["use_for_optimization"].astype(bool)
 
-    if "InAnalysis" not in df.columns:
-        df["InAnalysis"] = True
+    if "in_analysis" not in df.columns:
+        df["in_analysis"] = True
     else:
-        df["InAnalysis"] = df["InAnalysis"].astype(bool)
+        df["in_analysis"] = df["in_analysis"].astype(bool)
 
     if "index" in df.columns:
         del df["index"]
 
-    df["Column"] = df["Column"].apply(format_columns)
+    df["plate_column"] = df["plate_column"].apply(format_columns)
 
-    df["Type"] = df["Type"].fillna("Not set")
+    df["sample_type"] = df["sample_type"].fillna("Not set")
 
     df.reset_index(inplace=True)
 
     return df
 
 
 def init_metadata(ms_files):
     ms_files = list(ms_files)
     ms_files = [filename_to_label(fn) for fn in ms_files]
-    df = pd.DataFrame({"MS-file": ms_files})
-    df["InAnalysis"] = True
-    df["Label"] = ""
-    df["Color"] = None
-    df["Type"] = "Unknown"
-    df["RunOrder"] = ""
-    df["Batch"] = ""
-    df["Row"] = ""
-    df["Column"] = ""
-    df["PeakOpt"] = ""
+    df = pd.DataFrame({"ms_file_label": ms_files})
+    df["in_analysis"] = True
+    df["label"] = ""
+    df["color"] = None
+    df["sample_type"] = "Unknown"
+    df["run_order"] = ""
+    df["plate"] = ""
+    df["plate_row"] = ""
+    df["plate_column"] = ""
+    df["use_for_optimization"] = ""
     return df
 
 
 def write_metadata(meta, wdir):
     fn = get_metadata_fn(wdir)
     with lock(fn):
         meta.to_csv(fn, index=False)
@@ -452,15 +446,14 @@
             else:
                 return x
         elif x is None:
             return None
         elif np.isnan(x):
             return None
     except:
-        print(type(x), x)
         assert False
     return f"{int(x):02.0f}"
 
 
 def get_complete_results(
     wdir,
     include_labels=None,
@@ -468,22 +461,22 @@
     file_types=None,
     include_excluded=False,
 ):
     meta = get_metadata(wdir)
     resu = get_results(wdir)
 
     if not include_excluded:
-        meta = meta[meta["InAnalysis"]]
-    df = pd.merge(meta, resu, on=["MS-file"])
+        meta = meta[meta["in_analysis"]]
+    df = pd.merge(meta, resu, on=["ms_file_label"])
     if include_labels is not None and len(include_labels) > 0:
         df = df[df.peak_label.isin(include_labels)]
     if exclude_labels is not None and len(exclude_labels) > 0:
         df = df[~df.peak_label.isin(exclude_labels)]
     if file_types is not None and file_types != []:
-        df = df[df.Type.isin(file_types)]
+        df = df[df.sample_type.isin(file_types)]
     df["log(peak_max+1)"] = df.peak_max.apply(np.log1p)
     if "index" in df.columns:
         df = df.drop("index", axis=1)
     return df
 
 
 def gen_tabulator_columns(
@@ -497,19 +490,19 @@
 ):
 
     if col_names is None:
         col_names = []
     col_names = list(col_names)
 
     standard_columns = [
-        "MS-file",
-        "InAnalysis",
-        "Color",
+        "ms_file_label",
+        "in_analysis",
+        "color",
         "index",
-        "PeakOpt",
+        "use_for_optimization",
     ]
 
     for col in standard_columns:
         if col in col_names:
             col_names.remove(col)
 
     columns = [
@@ -525,56 +518,56 @@
             "frozen": True,
         }
     ]
 
     if add_ms_file_col:
         columns.append(
             {
-                "title": "MS-file",
-                "field": "MS-file",
+                "title": "ms_file_label",
+                "field": "ms_file_label",
                 "headerFilter": True,
                 "headerSort": True,
                 "editor": "input",
                 "sorter": "string",
                 "frozen": True,
             }
         )
 
     if add_color_col:
         columns.append(
             {
-                "title": "Color",
-                "field": "Color",
+                "title": "color",
+                "field": "color",
                 "headerFilter": False,
                 "editor": "input",
                 "formatter": "color",
                 "width": "3px",
                 "headerSort": False,
             }
         )
 
     if add_peakopt_col:
         columns.append(
             {
-                "title": "PeakOpt",
-                "field": "PeakOpt",
+                "title": "use_for_optimization",
+                "field": "use_for_optimization",
                 "headerFilter": False,
                 "formatter": "tickCross",
                 "width": "6px",
                 "headerSort": True,
                 "hozAlign": "center",
                 "editor": True,
             }
         )
 
     if add_ms_file_active_col:
         columns.append(
             {
-                "title": "InAnalysis",
-                "field": "InAnalysis",
+                "title": "in_analysis",
+                "field": "in_analysis",
                 "headerFilter": True,
                 "formatter": "tickCross",
                 "width": "6px",
                 "headerSort": True,
                 "hozAlign": "center",
                 "editor": True,
             }
@@ -599,26 +592,24 @@
     if filename.lower().endswith(".csv"):
         df = pd.read_csv(io.StringIO(decoded.decode("utf-8")))
     elif filename.lower().endswith(".xlsx"):
         df = pd.read_excel(io.BytesIO(decoded))
     return df
 
 
-def fig_to_src(dpi=100):
+def fig_to_src(fig, dpi=100):
     out_img = io.BytesIO()
-
-    plt.savefig(out_img, format="jpeg", bbox_inches="tight", dpi=dpi)
-
-    plt.close("all")
+    fig.savefig(out_img, format="jpeg", bbox_inches="tight", dpi=dpi)
+    plt.close(fig)
     out_img.seek(0)  # rewind file
     encoded = base64.b64encode(out_img.read()).decode("ascii").replace("\n", "")
     return "data:image/png;base64,{}".format(encoded)
 
 
-def merge_metadata(old: pd.DataFrame, new: pd.DataFrame, index_col='MS-file') -> pd.DataFrame:
+def merge_metadata(old: pd.DataFrame, new: pd.DataFrame, index_col='ms_file_label') -> pd.DataFrame:
     """
     This function updates one existing dataframe 
     with information from a second dataframe.
     If a column of the new dataframe does not 
     exist it will be created.
 
     Parameters:
@@ -647,15 +638,15 @@
 
     return old.reset_index()
 
 
 def file_colors(wdir):
     meta = get_metadata(wdir)
     colors = {}
-    for ndx, (fn, co) in meta[["MS-file", "Color"]].iterrows():
+    for ndx, (fn, co) in meta[["ms_file_label", "color"]].iterrows():
         if not (isinstance(co, str)):
             co = None
         colors[fn] = co
     return colors
 
 
 def get_figure_fn(kind, wdir, label, format):
@@ -668,22 +659,22 @@
 
 def clean_string(fn: str):
     for x in ['"', "'", "(", ")", "[", "]", " ", "\\", "/", "{", "}"]:
         fn = fn.replace(x, "_")
     return fn
 
 
-def savefig(kind=None, wdir=None, label=None, format="png", dpi=150):
+def savefig(fig, kind=None, wdir=None, label=None, format="png", dpi=150):
     path, fn = get_figure_fn(kind=kind, wdir=wdir, label=label, format=format)
     maybe_create(path)
     try:
         with lock(fn):
-            plt.savefig(fn, dpi=dpi, bbox_inches="tight")
+            fig.savefig(fn, dpi=dpi, bbox_inches="tight")
     except:
-        print(f"Could not save figure {fn}, maybe no figure was created: {label}")
+        logging.error(f"Could not save figure {fn}, maybe no figure was created: {label}")
     return fn
 
 
 def maybe_create(dir_name):
     if not os.path.isdir(dir_name):
         os.makedirs(dir_name)
 
@@ -693,15 +684,15 @@
     return "data:image/png;base64,{}".format(encoded_image.decode())
 
 
 def get_ms_fns_for_peakopt(wdir):
     """Extract the filenames for peak optimization from
     the metadata table and recreate the complete filename."""
     df = get_metadata(wdir)
-    fns = df[df.PeakOpt.astype(bool) == True]["MS-file"]
+    fns = df[df.use_for_optimization.astype(bool) == True]["ms_file_label"]
     ms_files = get_ms_fns(wdir)
     mapping = {filename_to_label(fn): fn for fn in ms_files}
     fns = [mapping[fn] for fn in fns]
     return fns
 
 
 def float_to_color(x, vmin=0, vmax=2, cmap=None):
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app/workspaces.py` & `ms-mint-app-0.3.0/ms_mint_app/plugins/workspaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,35 @@
 
 import dash
 from dash import html, dcc, dash_table
 from dash.exceptions import PreventUpdate
 from dash.dependencies import Input, Output, State
 import dash_bootstrap_components as dbc
 
+from .. import tools as T
+from ..plugin_interface import PluginInterface
 
-from . import tools as T
 
 
+class WorkspacesPlugin(PluginInterface):
+    def __init__(self):
+        self._label = _label
+        self._order = 0
+
+    def layout(self):
+        return _layout
+
+    def callbacks(self, app, fsc, cache):
+        callbacks(app, fsc, cache)
+    
+    def outputs(self):
+        return _outputs
+        
+_label = "Workspaces"
+
 ws_table = html.Div(
     id="ws-table-container",
     style={"minHeight": 100, "margin": "5%"},
     children=[
         dash_table.DataTable(
             id="ws-table",
             columns=[{"name": i, "id": i, "selectable": True} for i in ["Workspace"]],
@@ -80,32 +97,26 @@
                         ]
                     )
                 ),
             ],
             id="ws-delete-popup",
         ),
     ]
-)
+)    
 
 
 _outputs = html.Div(
     id="ws-outputs",
     children=[
         html.Div(id={"index": "ws-created-output", "type": "output"}),
         html.Div(id={"index": "ws-activate-output", "type": "output"}),
         html.Div(id={"index": "ws-delete-output", "type": "output"}),
     ],
 )
 
-_label = "Workspaces"
-
-
-def layout():
-    return _layout
-
 
 def callbacks(app, fsc, cache):
     @app.callback(
         Output("ws-table", "data"),
         Input({"index": "ws-created-output", "type": "output"}, "children"),
         Input("tab", "value"),
         Input({"index": "ws-delete-output", "type": "output"}, "children"),
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app.egg-info/PKG-INFO` & `ms-mint-app-0.3.0/ms_mint_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint-app
-Version: 0.2.3.2
+Version: 0.3.0
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint-app
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,14 +38,18 @@
 - describe accepted file types in ms_files tab
 - target-list add columns database_ref, formula, polarity
 - add descriptions to the optimization tab
 - total ion chromatogram (TIC)
 - full extracted ion chromatogram (EIC or XIC)
 - feature to convert intensities to concentrations
 
+### 0.2.3
+- update to pandas 2.0
+- faster processing of mzML and mzXML files
+
 ### 0.2.2
 - version strings in GUI
 - fixed issues with QC figures
 
 ### 0.2.1
 - uses ms-mint 0.2.1 with new implementation of `peak_area_top3`
 - new quality control tab
```

### Comparing `ms-mint-app-0.2.3.2/ms_mint_app.egg-info/SOURCES.txt` & `ms-mint-app-0.3.0/ms_mint_app.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -2,37 +2,41 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 ms_mint_app/__init__.py
 ms_mint_app/_version.py
-ms_mint_app/add_metab.py
-ms_mint_app/analysis.py
 ms_mint_app/app.py
 ms_mint_app/auth.py
 ms_mint_app/database.py
-ms_mint_app/distributions.py
 ms_mint_app/filelock.py
-ms_mint_app/heatmap.py
-ms_mint_app/hierachical_clustering.py
 ms_mint_app/messages.py
-ms_mint_app/metadata.py
-ms_mint_app/ms_files.py
-ms_mint_app/pca.py
-ms_mint_app/peak_optimization.py
-ms_mint_app/plotting.py
-ms_mint_app/processing.py
-ms_mint_app/quality_control.py
-ms_mint_app/targets.py
+ms_mint_app/plugin_interface.py
+ms_mint_app/plugin_manager.py
 ms_mint_app/tools.py
-ms_mint_app/workspaces.py
 ms_mint_app.egg-info/PKG-INFO
 ms_mint_app.egg-info/SOURCES.txt
 ms_mint_app.egg-info/dependency_links.txt
 ms_mint_app.egg-info/requires.txt
 ms_mint_app.egg-info/top_level.txt
+ms_mint_app/plugins/__init__.py
+ms_mint_app/plugins/add_metabolites.py
+ms_mint_app/plugins/analysis.py
+ms_mint_app/plugins/metadata.py
+ms_mint_app/plugins/ms_files.py
+ms_mint_app/plugins/processing.py
+ms_mint_app/plugins/quality_control.py
+ms_mint_app/plugins/target_optimization.py
+ms_mint_app/plugins/targets.py
+ms_mint_app/plugins/workspaces.py
+ms_mint_app/plugins/analysis_tools/__init__.py
+ms_mint_app/plugins/analysis_tools/distributions.py
+ms_mint_app/plugins/analysis_tools/heatmap.py
+ms_mint_app/plugins/analysis_tools/hierachical_clustering.py
+ms_mint_app/plugins/analysis_tools/pca.py
+ms_mint_app/plugins/analysis_tools/plotting.py
 ms_mint_app/static/ChEBI-Chem.parquet
 ms_mint_app/static/ChEBI-Groups.parquet
 ms_mint_app/static/Standard_Peaklist.csv
 ms_mint_app/static/__init__.py
 scripts/Mint.py
```

### Comparing `ms-mint-app-0.2.3.2/scripts/Mint.py` & `ms-mint-app-0.3.0/scripts/Mint.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sys
 import subprocess
 import multiprocessing
 import argparse
 import pkg_resources
 import xlsxwriter
 import bs4
+import logging
 
 from waitress import serve
 from os.path import expanduser
 from pathlib import Path as P
 from collections import namedtuple
 from multiprocessing import freeze_support
 
@@ -130,14 +131,17 @@
         os.environ["MINT_DATA_DIR"] = args.data_dir
 
     if args.serve_path is not None:
         os.environ["MINT_SERVE_PATH"] = args.serve_path
 
     print(welcome)
 
+    root_logger = logging.getLogger()
+    root_logger.setLevel(logging.INFO)
+
     print("Loading app...")
 
     from ms_mint_app.app import create_app, register_callbacks
 
     app, cache, fsc = create_app()
     register_callbacks(app, cache, fsc)
```

### Comparing `ms-mint-app-0.2.3.2/setup.py` & `ms-mint-app-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.2.3.2/versioneer.py` & `ms-mint-app-0.3.0/versioneer.py`

 * *Files identical despite different names*


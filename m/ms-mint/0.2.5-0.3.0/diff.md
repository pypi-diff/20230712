# Comparing `tmp/ms-mint-0.2.5.tar.gz` & `tmp/ms-mint-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms-mint-0.2.5.tar", last modified: Tue Jul 11 19:38:41 2023, max compression
+gzip compressed data, was "ms-mint-0.3.0.tar", last modified: Wed Jul 12 16:23:58 2023, max compression
```

## Comparing `ms-mint-0.2.5.tar` & `ms-mint-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:38:41.310567 ms-mint-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-07-11 19:38:29.000000 ms-mint-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-11 19:38:29.000000 ms-mint-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-11 19:38:41.310567 ms-mint-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-07-11 19:38:29.000000 ms-mint-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:38:41.314567 ms-mint-0.2.5/ms_mint/
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/Chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    18035 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/Mint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/MintPlotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/TargetOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 19:38:41.314567 ms-mint-0.2.5/ms_mint/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/matplotlib_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/plotly_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-11 19:38:29.000000 ms-mint-0.2.5/ms_mint/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:38:41.310567 ms-mint-0.2.5/ms_mint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-11 19:38:41.000000 ms-mint-0.2.5/ms_mint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-11 19:38:41.000000 ms-mint-0.2.5/ms_mint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:38:41.000000 ms-mint-0.2.5/ms_mint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-11 19:38:41.000000 ms-mint-0.2.5/ms_mint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 19:38:41.000000 ms-mint-0.2.5/ms_mint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:38:41.310567 ms-mint-0.2.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-11 19:38:29.000000 ms-mint-0.2.5/scripts/ms-mint-convert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-07-11 19:38:41.314567 ms-mint-0.2.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-07-11 19:38:29.000000 ms-mint-0.2.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68780 2023-07-11 19:38:30.000000 ms-mint-0.2.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:23:58.521733 ms-mint-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-07-12 16:23:41.000000 ms-mint-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-12 16:23:41.000000 ms-mint-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-12 16:23:58.521733 ms-mint-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-07-12 16:23:41.000000 ms-mint-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:23:58.525733 ms-mint-0.3.0/ms_mint/
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/Chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/Mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/MintPlotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/TargetOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-12 16:23:58.525733 ms-mint-0.3.0/ms_mint/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/matplotlib_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/plotly_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-12 16:23:41.000000 ms-mint-0.3.0/ms_mint/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:23:58.521733 ms-mint-0.3.0/ms_mint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-12 16:23:58.000000 ms-mint-0.3.0/ms_mint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-12 16:23:58.000000 ms-mint-0.3.0/ms_mint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:23:58.000000 ms-mint-0.3.0/ms_mint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-12 16:23:58.000000 ms-mint-0.3.0/ms_mint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 16:23:58.000000 ms-mint-0.3.0/ms_mint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:23:58.521733 ms-mint-0.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-12 16:23:41.000000 ms-mint-0.3.0/scripts/ms-mint-convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-07-12 16:23:58.521733 ms-mint-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-07-12 16:23:41.000000 ms-mint-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68780 2023-07-12 16:23:42.000000 ms-mint-0.3.0/versioneer.py
```

### Comparing `ms-mint-0.2.5/LICENSE` & `ms-mint-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/PKG-INFO` & `ms-mint-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint
-Version: 0.2.5
+Version: 0.3.0
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ms-mint-0.2.5/README.md` & `ms-mint-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/ms_mint/Chromatogram.py` & `ms-mint-0.3.0/ms_mint/Chromatogram.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/ms_mint/Mint.py` & `ms-mint-0.3.0/ms_mint/Mint.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,15 +388,15 @@
         The values in the cells are determined by *col_name*.
 
         :param col_name: Name of the column from *mint.results* table that is used for the cell values.
         :type col_name: str
 
         cells of the returned table.
         """
-
+        
         df_meta = pd.merge(self.meta, self.results, left_index=True, right_on='ms_file_label')
 
         if index is None:
             index = 'ms_file_label'
         if column is None:
             column = 'peak_label'
         if values is None:
@@ -548,14 +548,16 @@
     def load_metadata(self, fn=None):
         if fn is None:
             fn = self.wdir/METADATA_DEFAUT_FN
         if str(fn).endswith('.csv'):
             self.meta = pd.read_csv(fn, index_col=0)
         elif str(fn).endswith('.parquet'):
             self.meta = pd.read_parquet(fn)
+        if 'ms_file_label' in self.meta.columns:
+            self.meta = self.meta.set_index('ms_file_label')
         return self
 
     def save_metadata(self, fn=None):
         if fn is None:
             fn = self.wdir/METADATA_DEFAUT_FN
         if str(fn).endswith('.csv'):
             self.meta.to_csv(fn, na_filter=False)
```

### Comparing `ms-mint-0.2.5/ms_mint/MintPlotter.py` & `ms-mint-0.3.0/ms_mint/MintPlotter.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/ms_mint/TargetOptimizer.py` & `ms-mint-0.3.0/ms_mint/TargetOptimizer.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/ms_mint/filelock.py` & `ms-mint-0.3.0/ms_mint/filelock.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/ms_mint/filters.py` & `ms-mint-0.3.0/ms_mint/filters.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/ms_mint/io.py` & `ms-mint-0.3.0/ms_mint/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,20 +71,15 @@
                 "retentionTime": "scan_time",
                 "intensity array": "intensity",
                 "m/z array": "mz",
             }
         )
         # Set datatypes
         set_dtypes(df)
-
-    # assert df.scan_id.dtype in [np.int32, np.int64], df.scan_id.dtype
-    # assert df.intensity.dtype == np.int64, df.intensity.dtype
-    # assert df.mz.dtype == np.float64, df.mz.dtype
-    # assert df.scan_time.dtype == np.float64, df.scan_time.dtype
-
+    print(df.columns)
     return df
 
 
 def mzxml_to_df(
     fn: Union[str, pathlib.Path],
     read_only: bool = False,
     time_unit_in_file: str = "min",
```

### Comparing `ms-mint-0.2.5/ms_mint/matplotlib_tools.py` & `ms-mint-0.3.0/ms_mint/matplotlib_tools.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/ms_mint/notebook.py` & `ms-mint-0.3.0/ms_mint/notebook.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/ms_mint/pca.py` & `ms-mint-0.3.0/ms_mint/pca.py`

 * *Files 17% similar despite different names*

```diff
@@ -96,36 +96,72 @@
         Class for plotting Mint PCA results.
 
         :param pca: PrincipalComponentsAnalyser instance
         :type pca: ms_mint.pca.PrincipalComponentsAnalyser
         """
         self.pca = pca
 
-    def cumulative_variance(self, height=4, aspect=2):
+        
+    def cumulative_variance(self, interactive=False, **kwargs):
+        if interactive:
+            return self.cumulative_variance_px(**kwargs)
+        else:
+            return self.cumulative_variance_sns(**kwargs) 
+        
+        
+    def cumulative_variance_px(self, **kwargs):
+        """
+        After running mint.pca() this function can be used to plot the cumulative variance of the
+        principal components.
+
+        :return: Returns a plotly express figure.
+        :rtype: plotly.graph_objs._figure.Figure
+        """
+        n_components = self.pca.results["n_components"]
+        cum_expl_var = self.pca.results["cum_expl_var"]
+        df = pd.DataFrame({'Principal Component': np.arange(n_components) + 1, 'Explained variance [%]': cum_expl_var})
+        fig = px.bar(df, x='Principal Component', y='Explained variance [%]', 
+                     title="Cumulative explained variance",
+                     labels={'Principal Component':'Principal Component', 'Explained variance [%]':'Explained variance [%]'},
+                     **kwargs)
+        fig.update_layout(autosize=True, showlegend=False)
+        return fig
+
+    def cumulative_variance_sns(self, **kwargs):
         """
         After running mint.pca() this function can be used to plot the cumulative variance of the
         principal components.
 
         :return: Returns a matplotlib figure.
         :rtype: matplotlib.figure.Figure
         """
+        # Set default values for aspect and height
+        aspect = kwargs.get('aspect', 1)
+        height = kwargs.get('height', 5)
+
         n_components = self.pca.results["n_components"]
-        fig = plt.figure(figsize=(height * aspect, height))
         cum_expl_var = self.pca.results["cum_expl_var"]
-        plt.bar(
+
+        # Calculate width based on aspect ratio and number of components
+        width = height * aspect
+
+        fig, ax = plt.subplots(figsize=(width, height))
+        ax.bar(
             np.arange(n_components) + 1,
             cum_expl_var,
             facecolor="grey",
             edgecolor="none",
         )
-        plt.xlabel("Principal Component")
-        plt.ylabel("Explained variance [%]")
-        plt.title("Cumulative explained variance")
-        plt.grid()
-        plt.xticks(range(1, len(cum_expl_var) + 1))
+        ax.set_xlabel("Principal Component")
+        ax.set_ylabel("Explained variance [%]")
+        ax.set_title("Cumulative explained variance")
+        #ax.grid()
+        ax.spines['top'].set_visible(False)
+        ax.spines['right'].set_visible(False)        
+        ax.set_xticks(range(1, len(cum_expl_var) + 1))
         return fig
 
     def _prepare_data(self, n_components=3, hue=None):
         df = self.pca.results["df_projected"].copy()
         cols = df.columns.to_list()[:n_components]
         df = df[cols]
 
@@ -151,15 +187,15 @@
         :return: Returns a matplotlib figure.
         :rtype: seaborn.axisgrid.PairGrid
         """
 
         df = self._prepare_data(n_components=n_components, hue=hue)
 
         if isinstance(hue, list):
-            hue = 'Label'
+            hue = 'label'
 
         if interactive:
             return self.pairplot_plotly(df, color_col=hue, **kwargs)
         else:
             return self.pairplot_sns(df, fig_kws=fig_kws, hue=hue, **kwargs)
 
     def pairplot_sns(self, df, fig_kws=None, **kwargs):
```

### Comparing `ms-mint-0.2.5/ms_mint/plotly_tools.py` & `ms-mint-0.3.0/ms_mint/plotly_tools.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/ms_mint/processing.py` & `ms-mint-0.3.0/ms_mint/processing.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/ms_mint/standards.py` & `ms-mint-0.3.0/ms_mint/standards.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/ms_mint/targets.py` & `ms-mint-0.3.0/ms_mint/targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     :type ms_mode: str, optional
     :return: DataFrame in formated target-list format
     :rtype: pandas.DataFrame
     """
     targets = targets.rename(columns=DEPRECATED_LABELS)
     if targets.index.name == "peak_label":
         targets = targets.reset_index()
+
     assert pd.value_counts(targets.columns).max() == 1, pd.value_counts(targets.columns)
     cols = targets.columns
     if "formula" in targets.columns and not "mz_mean" in targets.columns:
         targets["mz_mean"] = formula_to_mass(targets["formula"], ms_mode)
     if "intensity_threshold" not in cols:
         targets["intensity_threshold"] = 0
     if "mz_width" not in cols:
@@ -81,16 +82,19 @@
     targets["rt_unit"] = targets["rt_unit"].replace("seconds", "s")
 
     for c in ["rt", "rt_min", "rt_max"]:
         if c not in cols:
             targets[c] = None
             targets[c] = targets[c].astype(float)
     del c
+    
     if "peak_label" not in cols:
+        logging.warning(f'"peak_label" not in cols, assigning new labels:\n{targets}')
         targets["peak_label"] = [f"C_{i}" for i in range(len(targets))]
+        
     targets["intensity_threshold"] = targets["intensity_threshold"].fillna(0)
     targets["peak_label"] = targets["peak_label"].astype(str)
 
     targets.index = range(len(targets))
     targets = targets[targets.mz_mean.notna()]
     targets = targets.replace(np.NaN, None)
     fill_missing_rt_values(targets)
```

### Comparing `ms-mint-0.2.5/ms_mint/tools.py` & `ms-mint-0.3.0/ms_mint/tools.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/ms_mint.egg-info/PKG-INFO` & `ms-mint-0.3.0/ms_mint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint
-Version: 0.2.5
+Version: 0.3.0
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ms-mint-0.2.5/ms_mint.egg-info/SOURCES.txt` & `ms-mint-0.3.0/ms_mint.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 ms_mint/filelock.py
 ms_mint/filters.py
 ms_mint/io.py
 ms_mint/matplotlib_tools.py
 ms_mint/notebook.py
 ms_mint/pca.py
 ms_mint/plotly_tools.py
-ms_mint/plotting.py
 ms_mint/processing.py
 ms_mint/standards.py
 ms_mint/targets.py
 ms_mint/tools.py
 ms_mint.egg-info/PKG-INFO
 ms_mint.egg-info/SOURCES.txt
 ms_mint.egg-info/dependency_links.txt
```

### Comparing `ms-mint-0.2.5/scripts/ms-mint-convert.py` & `ms-mint-0.3.0/scripts/ms-mint-convert.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/setup.py` & `ms-mint-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.5/versioneer.py` & `ms-mint-0.3.0/versioneer.py`

 * *Files identical despite different names*


# Comparing `tmp/mlbi_at_dku_lib-0.2.6.tar.gz` & `tmp/mlbi_at_dku_lib-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.2.6.tar", last modified: Tue Jul 11 14:22:57 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.2.7.tar", last modified: Wed Jul 12 11:02:28 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.2.6.tar` & `mlbi_at_dku_lib-0.2.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 14:22:57.203400 mlbi_at_dku_lib-0.2.6/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.6/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      102 2023-07-02 06:59:42.000000 mlbi_at_dku_lib-0.2.6/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-11 14:22:57.203400 mlbi_at_dku_lib-0.2.6/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.6/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      827 2023-07-11 14:21:48.000000 mlbi_at_dku_lib-0.2.6/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-11 14:22:57.203400 mlbi_at_dku_lib-0.2.6/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-02 05:17:52.000000 mlbi_at_dku_lib-0.2.6/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 14:22:57.139402 mlbi_at_dku_lib-0.2.6/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 14:22:57.139402 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 14:22:57.187401 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/GTmap_hg19.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/GTmap_hg38.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/GTmap_mm10.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    14644 2023-07-11 14:20:18.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-11 04:52:53.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    36550 2023-07-11 10:36:34.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30776 2023-07-11 14:11:49.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-11 14:22:57.139402 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-11 14:22:57.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      633 2023-07-11 14:22:57.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-11 14:22:57.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-11 14:22:57.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-11 14:22:57.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       16 2023-07-11 14:22:57.000000 mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:02:28.153323 mlbi_at_dku_lib-0.2.7/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.7/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      102 2023-07-02 06:59:42.000000 mlbi_at_dku_lib-0.2.7/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-12 11:02:28.153323 mlbi_at_dku_lib-0.2.7/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.7/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      827 2023-07-12 11:01:22.000000 mlbi_at_dku_lib-0.2.7/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-12 11:02:28.153323 mlbi_at_dku_lib-0.2.7/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-02 05:17:52.000000 mlbi_at_dku_lib-0.2.7/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:02:27.409337 mlbi_at_dku_lib-0.2.7/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:02:27.429336 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21347 2023-07-12 10:58:09.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:02:27.985326 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/data/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/data/GTmap_hg19.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/data/GTmap_hg38.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/data/GTmap_mm10.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    14644 2023-07-11 14:20:18.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-11 04:52:53.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    36550 2023-07-11 10:36:34.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30776 2023-07-11 14:11:49.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:02:27.433336 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-12 11:02:27.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      633 2023-07-12 11:02:27.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-12 11:02:27.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-12 11:02:27.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-12 11:02:27.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       16 2023-07-12 11:02:27.000000 mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib.egg-info/top_level.txt
```

### Comparing `mlbi_at_dku_lib-0.2.6/LICENSE` & `mlbi_at_dku_lib-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.6/PKG-INFO` & `mlbi_at_dku_lib-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.2.6
+Version: 0.2.7
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mlbi_at_dku_lib-0.2.6/pyproject.toml` & `mlbi_at_dku_lib-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlbi_at_dku_lib"
-version = "0.2.6"
+version = "0.2.7"
 description = "Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/cpdb.py`

 * *Files 11% similar despite different names*

```diff
@@ -174,14 +174,122 @@
             rend[idx] = idx_new
 
     if len(rend.keys()) > 0:
         dfv.rename(index = rend, inplace = True)
     '''        
     return df_pval_info, df_pval_pairs, df_mean_pairs, dfv
 
+###################################
+### CellPhoneDB 4.1.0 #############
+
+try:
+    from cellphonedb.src.core.methods import cpdb_degs_analysis_method
+    from cellphonedb.src.core.methods import cpdb_statistical_analysis_method
+except ImportError:
+    print('WARNING: CellPhoneDB seems not be installed. ')
+
+
+def cpdb4_run( adata, cell_types, db, out_dir,
+               gene_id_type = 'gene_name', 
+               n_iter = None, pval_th = None, threshold = None):
+    
+    if isinstance(adata, pd.DataFrame):
+        X = adata.astype(int).copy(deep = True)
+        cols = list(X.columns.values)
+        rows = list(X.index.values)
+        file_cpm = '%s/cnt_tmp.tsv' % out_dir
+    elif isinstance(adata, anndata.AnnData):         
+        cols = list(adata.var.index.values)
+        rows = list(adata.obs.index.values)
+        file_cpm = '%s/adata_tmp.h5ad' % out_dir
+    else:
+        print('ERROR: input data must be either DataFrame or AnnData.')
+        return None
+    
+    start = time.time()
+    print('Running CellPhoneDB .. ')    
+    
+    if out_dir[-1] == '/':
+        out_dir = out_dir[:-1]
+    
+    if not os.path.isdir(out_dir):
+        os.mkdir(out_dir)
+            
+    cols2 = [s.upper() for s in cols]
+    rend = dict(zip(cols, cols2))
+    
+    if isinstance(adata, pd.DataFrame):
+        X.rename(columns = rend, inplace = True)
+        X.transpose().to_csv(file_cpm, sep = '\t')
+        
+    elif isinstance(adata, anndata.AnnData):         
+        adata.var.rename(index = rend, inplace = True)    
+        adata.write(file_cpm)
+        
+    file_meta = '%s/meta_tmp.tsv' % out_dir
+    df_celltype = pd.DataFrame({'cell_type': cell_types}, 
+                               index = rows)    
+    df_celltype.to_csv(file_meta, sep = '\t')
+    
+    deconv, means, pvals, signif_means = cpdb_statistical_analysis_method.call(
+            cpdb_file_path = db,
+            meta_file_path = file_meta,
+            counts_file_path = file_cpm,
+            counts_data = gene_id_type,
+            output_path = out_dir)
+    
+    ## if gene_a or gene_b is None, set it with partner's name
+    b = means['gene_a'].isnull()
+    if np.sum(b) > 0:
+        means.loc[b, 'gene_a'] = means.loc[b, 'partner_a']
+
+    b = means['gene_b'].isnull()
+    if np.sum(b) > 0:
+        means.loc[b, 'gene_b'] = means.loc[b, 'partner_b']
+
+    b = pvals['gene_a'].isnull()
+    if np.sum(b) > 0:
+        pvals.loc[b, 'gene_a'] = pvals.loc[b, 'partner_a']
+
+    b = pvals['gene_b'].isnull()
+    if np.sum(b) > 0:
+        pvals.loc[b, 'gene_b'] = pvals.loc[b, 'partner_b']
+
+    elapsed = time.time() - start
+    print('Running CellPhoneDB .. done. %i' % elapsed )    
+    
+    if os.path.exists(file_cpm):
+        os.remove(file_cpm)
+    if os.path.exists(file_meta):
+        os.remove(file_meta)
+    
+    return  means, pvals
+
+
+def cpdb4_get_results( df_pval, df_mean, pval_max = 0.05, mean_min = 0.01 ):
+    
+    # df_mean_info, df_mean_pairs, df_pval_info, df_pval_pairs = \
+    #       cpdb_get_res( out_dir )
+    
+    cols = list(df_pval.columns.values)
+    df_pval_info = df_pval[cols[:11]]
+    df_pval_pairs = df_pval[cols[11:]]
+    
+    cols = list(df_mean.columns.values)
+    df_mean_info = df_mean[cols[:11]]
+    df_mean_pairs = df_mean[cols[11:]]
+    
+    dfv = cpdb_get_vec( df_pval_info, df_mean_pairs, df_pval_pairs, 
+                        pval_max = pval_max, mean_min = mean_min )
+    
+    return df_pval_info, df_pval_pairs, df_mean_pairs, dfv
+
+
+###################################
+### Plot functions for CellPhoneDB
 
 def cpdb_plot( dfp, mkr_sz = 6, tick_sz = 6, 
                              legend_fs = 11, title_fs = 14,
                              dpi = 120, title = None, swap_ax = False ):
     if swap_ax == False:
         a = 'gene_pair'
         b = 'cell_pair'
```

### Comparing `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/GTmap_hg19.csv` & `mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/data/GTmap_hg19.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/GTmap_hg38.csv` & `mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/data/GTmap_hg38.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/data/GTmap_mm10.csv` & `mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/data/GTmap_mm10.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/deg.py` & `mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/deg.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/deiso.py` & `mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/deiso.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/icnv.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib/misc.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.2.6
+Version: 0.2.7
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mlbi_at_dku_lib-0.2.6/src/mlbi_at_dku_lib.egg-info/SOURCES.txt` & `mlbi_at_dku_lib-0.2.7/src/mlbi_at_dku_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/mlbi_at_dku_lib-0.2.8.tar.gz` & `tmp/mlbi_at_dku_lib-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.2.8.tar", last modified: Wed Jul 12 11:37:45 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.2.9.tar", last modified: Wed Jul 12 11:54:52 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.2.8.tar` & `mlbi_at_dku_lib-0.2.9.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:37:45.357799 mlbi_at_dku_lib-0.2.8/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.8/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      102 2023-07-02 06:59:42.000000 mlbi_at_dku_lib-0.2.8/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-12 11:37:45.357799 mlbi_at_dku_lib-0.2.8/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.8/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      827 2023-07-12 11:37:30.000000 mlbi_at_dku_lib-0.2.8/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-12 11:37:45.357799 mlbi_at_dku_lib-0.2.8/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-02 05:17:52.000000 mlbi_at_dku_lib-0.2.8/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:37:45.289802 mlbi_at_dku_lib-0.2.8/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:37:45.289802 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21356 2023-07-12 11:37:11.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:37:45.341800 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/data/
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/data/GTmap_hg19.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/data/GTmap_hg38.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/data/GTmap_mm10.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    14644 2023-07-11 14:20:18.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-11 04:52:53.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    36550 2023-07-11 10:36:34.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30776 2023-07-11 14:11:49.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:37:45.289802 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-12 11:37:45.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      633 2023-07-12 11:37:45.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-12 11:37:45.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-12 11:37:45.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-12 11:37:45.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       16 2023-07-12 11:37:45.000000 mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:54:52.523246 mlbi_at_dku_lib-0.2.9/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.9/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      102 2023-07-02 06:59:42.000000 mlbi_at_dku_lib-0.2.9/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-12 11:54:52.523246 mlbi_at_dku_lib-0.2.9/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.9/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      827 2023-07-12 11:49:16.000000 mlbi_at_dku_lib-0.2.9/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-12 11:54:52.523246 mlbi_at_dku_lib-0.2.9/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-02 05:17:52.000000 mlbi_at_dku_lib-0.2.9/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:54:52.459248 mlbi_at_dku_lib-0.2.9/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:54:52.459248 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-12 11:45:27.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:54:52.511247 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/data/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/data/GTmap_hg19.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/data/GTmap_hg38.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-02 05:45:36.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/data/GTmap_mm10.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    14644 2023-07-11 14:20:18.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-11 04:52:53.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157732 2023-07-12 11:53:08.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    36606 2023-07-12 11:49:13.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30776 2023-07-11 14:11:49.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-12 11:54:52.459248 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41231 2023-07-12 11:54:52.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      662 2023-07-12 11:54:52.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-12 11:54:52.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-12 11:54:52.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-12 11:54:52.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       16 2023-07-12 11:54:52.000000 mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib.egg-info/top_level.txt
```

### Comparing `mlbi_at_dku_lib-0.2.8/LICENSE` & `mlbi_at_dku_lib-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.8/PKG-INFO` & `mlbi_at_dku_lib-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.2.8
+Version: 0.2.9
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mlbi_at_dku_lib-0.2.8/pyproject.toml` & `mlbi_at_dku_lib-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlbi_at_dku_lib"
-version = "0.2.8"
+version = "0.2.9"
 description = "Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/cpdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     from cellphonedb.src.core.methods import cpdb_degs_analysis_method
     from cellphonedb.src.core.methods import cpdb_statistical_analysis_method
 except ImportError:
     print('WARNING: CellPhoneDB seems not be installed. ')
 
 
 def cpdb4_run( adata, cell_types, db, out_dir,
-               gene_id_type = 'gene_name', 
+               gene_id_type = 'gene_name', n_cores = 4,
                n_iter = None, pval_th = None, threshold = None):
     
     if isinstance(adata, pd.DataFrame):
         X = adata.astype(int).copy(deep = True)
         cols = list(X.columns.values)
         rows = list(X.index.values)
         file_cpm = '%s/cnt_tmp.tsv' % out_dir
@@ -231,15 +231,15 @@
     df_celltype.to_csv(file_meta, sep = '\t')
     
     deconv, means, pvals, signif_means = cpdb_statistical_analysis_method.call(
             cpdb_file_path = db,
             meta_file_path = file_meta,
             counts_file_path = file_cpm,
             counts_data = gene_id_type,
-            output_path = out_dir)
+            output_path = out_dir, threads = n_cores )
     
     ## if gene_a or gene_b is None, set it with partner's name
     b = means['gene_a'].isnull()
     if np.sum(b) > 0:
         means.loc[b, 'gene_a'] = means.loc[b, 'partner_a']
 
     b = means['gene_b'].isnull()
```

### Comparing `mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/data/GTmap_hg19.csv` & `mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/data/GTmap_hg19.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/data/GTmap_hg38.csv` & `mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/data/GTmap_hg38.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/data/GTmap_mm10.csv` & `mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/data/GTmap_mm10.csv`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/deg.py` & `mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/deg.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/deiso.py` & `mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/deiso.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/icnv.py`

 * *Files 1% similar despite different names*

```diff
@@ -902,28 +902,29 @@
     return adata.obs[[cluster_key, score_key, 'tumor_dec'+suffix, 
                       'tumor_prob'+suffix, 'tumor_cluster'+ suffix]], params
 
 
 import warnings
 
 def run_icnv(adata, ref_key, ref_types, gtf_file, cluster_key = 'cnv_leiden', 
-             resolution = 2, N_pca = 15, n_neighbors = 10, pca_umap = True ):
+             resolution = 2, N_pca = 15, n_neighbors = 10, pca_umap = True, n_cores = 4 ):
     
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
     
         ## Normalize and log-transform
         sc.pp.normalize_total(adata, target_sum=1e4)
         sc.pp.log1p(adata)
 
         sc.pp.highly_variable_genes(adata, n_top_genes = 2000) # , flavor = 'seurat_v3')
         # sc.tl.score_genes_cell_cycle(adata, cell_cycle_genes_s, cell_cycle_genes_g2m)
 
         cnv.io.genomic_position_from_gtf(gtf_file, adata, gtf_gene_id='gene_name', adata_gene_id=None, inplace=True)
-        cnv.tl.infercnv(adata, reference_key = ref_key, reference_cat=ref_types, window_size=100)
+        cnv.tl.infercnv(adata, reference_key = ref_key, reference_cat=ref_types, 
+                        window_size=100, n_jobs = n_cores)
 
         if pca_umap:
             print('PCA .. ', end = '')
             cnv.tl.pca(adata, svd_solver='arpack', n_comps = N_pca) 
             print('Finding neighbors .. ', end = '')
             cnv.pp.neighbors(adata, key_added = 'cnv_neighbors', n_neighbors=n_neighbors, n_pcs=N_pca)
             print('Clustering .. ', end = '')
```

### Comparing `mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib/misc.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.2.8
+Version: 0.2.9
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `mlbi_at_dku_lib-0.2.8/src/mlbi_at_dku_lib.egg-info/SOURCES.txt` & `mlbi_at_dku_lib-0.2.9/src/mlbi_at_dku_lib.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.py
 src/mlbi_at_dku_lib/__init__.py
 src/mlbi_at_dku_lib/cpdb.py
 src/mlbi_at_dku_lib/deg.py
 src/mlbi_at_dku_lib/deiso.py
 src/mlbi_at_dku_lib/gsea.py
+src/mlbi_at_dku_lib/hicat.py
 src/mlbi_at_dku_lib/icnv.py
 src/mlbi_at_dku_lib/misc.py
 src/mlbi_at_dku_lib.egg-info/PKG-INFO
 src/mlbi_at_dku_lib.egg-info/SOURCES.txt
 src/mlbi_at_dku_lib.egg-info/dependency_links.txt
 src/mlbi_at_dku_lib.egg-info/entry_points.txt
 src/mlbi_at_dku_lib.egg-info/requires.txt
```


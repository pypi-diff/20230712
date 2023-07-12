# Comparing `tmp/hta-0.0.2.tar.gz` & `tmp/hta-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/levy.alona/Google Drive/phd/hta/dist/tmpylz4im5t/hta-0.0.2.tar", last modified: Fri Jul 30 12:52:31 2021, max compression
+gzip compressed data, was "/Users/levy.alona/Google Drive/phd/hta/dist/.tmp-8h1u4flu/hta-0.1.0.tar", last modified: Wed Jul 12 19:37:42 2023, max compression
```

## Comparing `hta-0.0.2.tar` & `hta-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 levy.alona   (501) staff       (20)        0 2021-07-30 12:52:31.867667 hta-0.0.2/
--rw-r--r--   0 levy.alona   (501) staff       (20)     1066 2020-12-06 15:30:22.000000 hta-0.0.2/LICENSE
--rw-r--r--   0 levy.alona   (501) staff       (20)     8565 2021-07-30 12:52:31.860796 hta-0.0.2/PKG-INFO
--rw-r--r--   0 levy.alona   (501) staff       (20)     7974 2021-07-30 12:44:00.000000 hta-0.0.2/README.md
-drwxr-xr-x   0 levy.alona   (501) staff       (20)        0 2021-07-30 12:52:31.811151 hta-0.0.2/hta_stats/
-drwxr-xr-x   0 levy.alona   (501) staff       (20)        0 2021-07-30 12:52:31.836093 hta-0.0.2/hta_stats/hta/
--rw-r--r--   0 levy.alona   (501) staff       (20)        0 2020-12-06 14:57:54.000000 hta-0.0.2/hta_stats/hta/__init__.py
--rw-r--r--   0 levy.alona   (501) staff       (20)    27457 2021-07-30 11:52:08.000000 hta-0.0.2/hta_stats/hta/stats.py
--rw-r--r--   0 levy.alona   (501) staff       (20)    13548 2021-07-30 12:44:00.000000 hta-0.0.2/hta_stats/hta/utils.py
-drwxr-xr-x   0 levy.alona   (501) staff       (20)        0 2021-07-30 12:52:31.858306 hta-0.0.2/hta_stats/hta.egg-info/
--rw-r--r--   0 levy.alona   (501) staff       (20)     8565 2021-07-30 12:52:31.000000 hta-0.0.2/hta_stats/hta.egg-info/PKG-INFO
--rw-r--r--   0 levy.alona   (501) staff       (20)      297 2021-07-30 12:52:31.000000 hta-0.0.2/hta_stats/hta.egg-info/SOURCES.txt
--rw-r--r--   0 levy.alona   (501) staff       (20)        1 2021-07-30 12:52:31.000000 hta-0.0.2/hta_stats/hta.egg-info/dependency_links.txt
--rw-r--r--   0 levy.alona   (501) staff       (20)       30 2021-07-30 12:52:31.000000 hta-0.0.2/hta_stats/hta.egg-info/requires.txt
--rw-r--r--   0 levy.alona   (501) staff       (20)        4 2021-07-30 12:52:31.000000 hta-0.0.2/hta_stats/hta.egg-info/top_level.txt
--rw-r--r--   0 levy.alona   (501) staff       (20)      103 2021-07-30 07:18:37.000000 hta-0.0.2/pyproject.toml
--rw-r--r--   0 levy.alona   (501) staff       (20)       38 2021-07-30 12:52:31.867782 hta-0.0.2/setup.cfg
--rw-r--r--   0 levy.alona   (501) staff       (20)      967 2021-07-30 12:52:04.000000 hta-0.0.2/setup.py
+drwxr-xr-x   0 levy.alona   (501) staff       (20)        0 2023-07-12 19:37:42.882162 hta-0.1.0/
+-rw-r--r--   0 levy.alona   (501) staff       (20)     1066 2020-12-06 15:30:22.000000 hta-0.1.0/LICENSE
+-rw-r--r--   0 levy.alona   (501) staff       (20)     9226 2023-07-12 19:37:42.876294 hta-0.1.0/PKG-INFO
+-rw-r--r--   0 levy.alona   (501) staff       (20)     8671 2021-10-23 11:50:11.000000 hta-0.1.0/README.md
+drwxr-xr-x   0 levy.alona   (501) staff       (20)        0 2023-07-12 19:37:42.803157 hta-0.1.0/hta_stats/
+drwxr-xr-x   0 levy.alona   (501) staff       (20)        0 2023-07-12 19:37:42.842735 hta-0.1.0/hta_stats/hta/
+-rw-r--r--   0 levy.alona   (501) staff       (20)        0 2020-12-06 14:57:54.000000 hta-0.1.0/hta_stats/hta/__init__.py
+-rw-r--r--   0 levy.alona   (501) staff       (20)    27457 2021-07-30 11:52:08.000000 hta-0.1.0/hta_stats/hta/stats.py
+-rw-r--r--   0 levy.alona   (501) staff       (20)    15067 2023-07-12 19:22:56.000000 hta-0.1.0/hta_stats/hta/utils.py
+drwxr-xr-x   0 levy.alona   (501) staff       (20)        0 2023-07-12 19:37:42.867741 hta-0.1.0/hta_stats/hta.egg-info/
+-rw-r--r--   0 levy.alona   (501) staff       (20)     9226 2023-07-12 19:37:42.000000 hta-0.1.0/hta_stats/hta.egg-info/PKG-INFO
+-rw-r--r--   0 levy.alona   (501) staff       (20)      312 2023-07-12 19:37:42.000000 hta-0.1.0/hta_stats/hta.egg-info/SOURCES.txt
+-rw-r--r--   0 levy.alona   (501) staff       (20)        1 2023-07-12 19:37:42.000000 hta-0.1.0/hta_stats/hta.egg-info/dependency_links.txt
+-rw-r--r--   0 levy.alona   (501) staff       (20)       30 2023-07-12 19:37:42.000000 hta-0.1.0/hta_stats/hta.egg-info/requires.txt
+-rw-r--r--   0 levy.alona   (501) staff       (20)        4 2023-07-12 19:37:42.000000 hta-0.1.0/hta_stats/hta.egg-info/top_level.txt
+-rw-r--r--   0 levy.alona   (501) staff       (20)      103 2021-07-30 07:18:37.000000 hta-0.1.0/pyproject.toml
+-rw-r--r--   0 levy.alona   (501) staff       (20)       38 2023-07-12 19:37:42.882301 hta-0.1.0/setup.cfg
+-rw-r--r--   0 levy.alona   (501) staff       (20)      967 2023-07-12 19:33:13.000000 hta-0.1.0/setup.py
+drwxr-xr-x   0 levy.alona   (501) staff       (20)        0 2023-07-12 19:37:42.869863 hta-0.1.0/tests/
+-rw-r--r--   0 levy.alona   (501) staff       (20)    12067 2023-07-12 19:24:31.000000 hta-0.1.0/tests/tests.py
```

### Comparing `hta-0.0.2/LICENSE` & `hta-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hta-0.0.2/PKG-INFO` & `hta-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: hta
-Version: 0.0.2
+Version: 0.1.0
 Summary: Statistically assess the level of both spatial and global heterogeneity within a spatial sample.
 Home-page: https://github.com/alonalj/hta
 Author: Alona Levy-Jurgenson
 Author-email: levyalona@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/alonalj/hta/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
 # Welcome to the HTA package!
 
 The HTA package can statistically assess the level of both spatial, and global, heterogeneity within a spatial sample. HTA was specifically designed to handle multivariate spatial transcriptomics data, such as Visium samples (10x Genomics), but can be used in other domains (see our paper [1] for further details).
 
-## Prerequisites
-Python 3.8 or above.
+If you use hta in your research, pleas cite: [Levy-Jurgenson et al. (Bioinformatics, 2021) [1].](https://doi.org/10.1093/bioinformatics/btab569)
+
+## Installation
+You will need Python 3.8 or above.
+
+To install the package and follow along with our examples below use the following command:
+
+    pip install hta
 
 ## Support and bug reports
-If you encounter any issues, please contact levyalona at gmail.
+If you encounter any issues, please contact levy alona (as one word) through gmail.
 
 # Example 1 - Synthetic Data
 
 ### Input format:
 
 Since generating a trait-combination matrix may be complicated, HTA generates it for you from a simpler form of input: a stacked set of matrices where each matrix represents one trait, and each entry indicates if the trait manifests or not (0/1) at the corresponding spatial position. 
 
@@ -78,34 +83,33 @@
     rr = hta.region_report(trait_names)
     rr.to_csv('region_report.csv')
 
 # Example 2 - Visium data
 
 If you are analysing Visium spatial gene expression data (e.g. any of those listed [here](https://support.10xgenomics.com/spatial-gene-expression/datasets), or [this one](https://support.10xgenomics.com/spatial-gene-expression/datasets/1.1.0/V1_Breast_Cancer_Block_A_Section_1) used in our examples below) you can use our `Visium` built-in class to generate the input format for HTA (i.e., the `t` as in Example 1). 
 
-Make sure you have the following folders from your Visium data:
+Make sure you have obtained the following files for your Visium data:
 
 > filtered_feature_bc_matrix
+>
 > spatial
 
 and place them in a folder hierarchy as shown below (all shown files are required, and all file/folder names must be identical to those shown below, except for the data folder name):
  ```
 YOUR_DATA_FOLDER
 └───filtered_feature_bc_matrix
 │   │   barcodes.tsv.gz
 │   │   features.tsv.gz
 │   │   matrix.mtx.gz
 └───spatial
 	│   tissue_positions_list.csv
 	│   ...
 ```
 
-additionally, your project should have an 'out' folder. 
-
-You are now ready to load your Visium data and use HTA:
+You are now ready to load your Visium data and use HTA. The following code loads the data (note that this may take around 30s), prepares it for HTA analysis, and computes the HTA p-value:
 
     from hta.stats import HTA  
     from hta.utils import Visium    
     
     path = "/PATH_TO/YOUR_DATA_FOLDER" # TODO: insert path to 'YOUR_DATA_FOLDER' (no '/' on end)
     trait_names = ['ERBB2', 'CD8A']   # names of features to use in features.tsv.gz  
       
@@ -114,19 +118,21 @@
     visium.load()  
     t, t_mask = visium.prep(trait_names)  
       
     # compute HTA and HTA p-val  
     region_size = 15   # modify region_size as needed
     hta = HTA(t, region_size=region_size, tissue_mask=t_mask) 
     hta_stat, hta_pval = hta.calc()
+    print("HTA p-value: ", hta_pval)
 
 >What is `t_mask`? It identifies, using barcodes.tsv.gz, which barcodes are under
 > the tissue, and is used to discard barcodeds that are not.
 
-Now we can proceed to produce the heterogeneity map and region report (we've left the p-val title formatting in the example below for your convenience, but you can replace it with your own title format):
+Now we can proceed to produce the heterogeneity map and region report. The code below uses the results from the previous block of code
+ to generate the heterogeneity map and region report. We've left the p-val title formatting code for your convenience so that you can easily replace it with your own title format:
 
   
     import math
     
     # generate heterogeneity map and legend
     hm = hta.plot_heterogeneity_map(trait_names, dot_size=8)  
     hm.legend(loc='upper center', bbox_to_anchor=(0.5, -0.15), ncol=4, fontsize=9)  
@@ -140,37 +146,39 @@
         title = 'HTA {:.2f} (p-val: 10^{:.0f}), region size: {}'.format(hta_stat, hta_pval, region_size)  
     else:  
         title = 'HTA {:.2f} (p-val: {:.2f}), region size: {}'.format(hta_stat, hta_pval, region_size)  
     
     # save heterogeneity map 
     font_dict = {'family': 'normal', 'size': 9}  
     hm.title(title, fontdict=font_dict)  
-    hm.savefig('../out/{}_hetero_map.jpeg'.format('_'.join(trait_names)), dpi=350)  
+    hm.savefig('{}_hetero_map.jpeg'.format('_'.join(trait_names)), dpi=350)  
     hm.close()  
       
     # save region report  
     rr = hta.region_report(trait_names)  
-    rr.to_csv('../out/{}_region_report.csv'.format('_'.join(trait_names)))
+    rr.to_csv('{}_region_report.csv'.format('_'.join(trait_names)))
 
 
 
 
 # Example 3 - Visium with cluster id per barcode
 
+(*) This is slightly more advanced. We recommend going through the previous Visium example before attempting this one.
+
 You can also use HTA with cluster IDs generated per barcode. The best example is using the cluster IDs provided in Visium's analysis folder, but you can use your own cluster IDs, provided they have the same format. 
 
-As an example, you can place Visium's 'analysis' folder (see links above) under your 'data_folder'. The 'analysis' folder contains many k-means clustering results where each barcode has a cluster ID.  
+As an example, you can place Visium's 'analysis' folder (see links above) under your 'YOUR_DATA_FOLDER'. The 'analysis' folder contains many k-means clustering results where each barcode has a cluster ID.  
 
 The main differences in the code below compared to Example 2 above are in the lines of code marked with (***):
 
 
     from hta.utils import Visium  
     from hta.stats import HTA  
       
-    path = "../res/data_folder"  
+    path = "/PATH_TO/YOUR_DATA_FOLDER" # TODO: insert path to 'YOUR_DATA_FOLDER' (no '/' on end)
     k = 10
     clusters_path = '{}/analysis/clustering/kmeans_{}_clusters/clusters.csv'.format(path, k)
     trait_names = [str(i+1) for i in range(k)]  
       
     visium = Visium(path)  
     visium.load()  
     t, t_mask = visium.prep_clusters(clusters_path)  # (***)
@@ -192,8 +200,7 @@
     hm.close()  
       
     # save region report  
     rr = hta.region_report(trait_names)  
     rr.to_csv('../out/{}_region_report.csv'.format('_'.join(trait_names)))
 
 [1] Assessing heterogeneity in spatial data using the HTA index with applications to spatial transcriptomics and imaging. *Levy-Jurgenson et al.* 
-
```

### Comparing `hta-0.0.2/README.md` & `hta-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,23 @@
+
 # Welcome to the HTA package!
 
 The HTA package can statistically assess the level of both spatial, and global, heterogeneity within a spatial sample. HTA was specifically designed to handle multivariate spatial transcriptomics data, such as Visium samples (10x Genomics), but can be used in other domains (see our paper [1] for further details).
 
-## Prerequisites
-Python 3.8 or above.
+If you use hta in your research, pleas cite: [Levy-Jurgenson et al. (Bioinformatics, 2021) [1].](https://doi.org/10.1093/bioinformatics/btab569)
+
+## Installation
+You will need Python 3.8 or above.
+
+To install the package and follow along with our examples below use the following command:
+
+    pip install hta
 
 ## Support and bug reports
-If you encounter any issues, please contact levyalona at gmail.
+If you encounter any issues, please contact levy alona (as one word) through gmail.
 
 # Example 1 - Synthetic Data
 
 ### Input format:
 
 Since generating a trait-combination matrix may be complicated, HTA generates it for you from a simpler form of input: a stacked set of matrices where each matrix represents one trait, and each entry indicates if the trait manifests or not (0/1) at the corresponding spatial position. 
 
@@ -61,34 +68,33 @@
     rr = hta.region_report(trait_names)
     rr.to_csv('region_report.csv')
 
 # Example 2 - Visium data
 
 If you are analysing Visium spatial gene expression data (e.g. any of those listed [here](https://support.10xgenomics.com/spatial-gene-expression/datasets), or [this one](https://support.10xgenomics.com/spatial-gene-expression/datasets/1.1.0/V1_Breast_Cancer_Block_A_Section_1) used in our examples below) you can use our `Visium` built-in class to generate the input format for HTA (i.e., the `t` as in Example 1). 
 
-Make sure you have the following folders from your Visium data:
+Make sure you have obtained the following files for your Visium data:
 
 > filtered_feature_bc_matrix
+>
 > spatial
 
 and place them in a folder hierarchy as shown below (all shown files are required, and all file/folder names must be identical to those shown below, except for the data folder name):
  ```
 YOUR_DATA_FOLDER
 └───filtered_feature_bc_matrix
 │   │   barcodes.tsv.gz
 │   │   features.tsv.gz
 │   │   matrix.mtx.gz
 └───spatial
 	│   tissue_positions_list.csv
 	│   ...
 ```
 
-additionally, your project should have an 'out' folder. 
-
-You are now ready to load your Visium data and use HTA:
+You are now ready to load your Visium data and use HTA. The following code loads the data (note that this may take around 30s), prepares it for HTA analysis, and computes the HTA p-value:
 
     from hta.stats import HTA  
     from hta.utils import Visium    
     
     path = "/PATH_TO/YOUR_DATA_FOLDER" # TODO: insert path to 'YOUR_DATA_FOLDER' (no '/' on end)
     trait_names = ['ERBB2', 'CD8A']   # names of features to use in features.tsv.gz  
       
@@ -97,19 +103,21 @@
     visium.load()  
     t, t_mask = visium.prep(trait_names)  
       
     # compute HTA and HTA p-val  
     region_size = 15   # modify region_size as needed
     hta = HTA(t, region_size=region_size, tissue_mask=t_mask) 
     hta_stat, hta_pval = hta.calc()
+    print("HTA p-value: ", hta_pval)
 
 >What is `t_mask`? It identifies, using barcodes.tsv.gz, which barcodes are under
 > the tissue, and is used to discard barcodeds that are not.
 
-Now we can proceed to produce the heterogeneity map and region report (we've left the p-val title formatting in the example below for your convenience, but you can replace it with your own title format):
+Now we can proceed to produce the heterogeneity map and region report. The code below uses the results from the previous block of code
+ to generate the heterogeneity map and region report. We've left the p-val title formatting code for your convenience so that you can easily replace it with your own title format:
 
   
     import math
     
     # generate heterogeneity map and legend
     hm = hta.plot_heterogeneity_map(trait_names, dot_size=8)  
     hm.legend(loc='upper center', bbox_to_anchor=(0.5, -0.15), ncol=4, fontsize=9)  
@@ -123,37 +131,39 @@
         title = 'HTA {:.2f} (p-val: 10^{:.0f}), region size: {}'.format(hta_stat, hta_pval, region_size)  
     else:  
         title = 'HTA {:.2f} (p-val: {:.2f}), region size: {}'.format(hta_stat, hta_pval, region_size)  
     
     # save heterogeneity map 
     font_dict = {'family': 'normal', 'size': 9}  
     hm.title(title, fontdict=font_dict)  
-    hm.savefig('../out/{}_hetero_map.jpeg'.format('_'.join(trait_names)), dpi=350)  
+    hm.savefig('{}_hetero_map.jpeg'.format('_'.join(trait_names)), dpi=350)  
     hm.close()  
       
     # save region report  
     rr = hta.region_report(trait_names)  
-    rr.to_csv('../out/{}_region_report.csv'.format('_'.join(trait_names)))
+    rr.to_csv('{}_region_report.csv'.format('_'.join(trait_names)))
 
 
 
 
 # Example 3 - Visium with cluster id per barcode
 
+(*) This is slightly more advanced. We recommend going through the previous Visium example before attempting this one.
+
 You can also use HTA with cluster IDs generated per barcode. The best example is using the cluster IDs provided in Visium's analysis folder, but you can use your own cluster IDs, provided they have the same format. 
 
-As an example, you can place Visium's 'analysis' folder (see links above) under your 'data_folder'. The 'analysis' folder contains many k-means clustering results where each barcode has a cluster ID.  
+As an example, you can place Visium's 'analysis' folder (see links above) under your 'YOUR_DATA_FOLDER'. The 'analysis' folder contains many k-means clustering results where each barcode has a cluster ID.  
 
 The main differences in the code below compared to Example 2 above are in the lines of code marked with (***):
 
 
     from hta.utils import Visium  
     from hta.stats import HTA  
       
-    path = "../res/data_folder"  
+    path = "/PATH_TO/YOUR_DATA_FOLDER" # TODO: insert path to 'YOUR_DATA_FOLDER' (no '/' on end)
     k = 10
     clusters_path = '{}/analysis/clustering/kmeans_{}_clusters/clusters.csv'.format(path, k)
     trait_names = [str(i+1) for i in range(k)]  
       
     visium = Visium(path)  
     visium.load()  
     t, t_mask = visium.prep_clusters(clusters_path)  # (***)
```

### Comparing `hta-0.0.2/hta_stats/hta/stats.py` & `hta-0.1.0/hta_stats/hta/stats.py`

 * *Files identical despite different names*

### Comparing `hta-0.0.2/hta_stats/hta/utils.py` & `hta-0.1.0/hta_stats/hta/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -269,8 +269,48 @@
         return self.trait_tensor, self.tissue_mask
 
     def prep_curated_traits(self, df, threshold_fn=np.median):
         self._set_shape_where_tissue()
         self._make_tissue_mask()
         self._make_curated_tensor(df, threshold_fn)
         self._preprocess_tensor_and_tissue_mask()
-        return self.trait_tensor, self.tissue_mask
+        return self.trait_tensor, self.tissue_mask
+
+
+class Images():
+    def __init__(self, path, trait_names, slice_names, img_format):
+        self._path = path
+        self._traits = trait_names
+        self._slices = slice_names
+        self._img_format = img_format
+        self.trait_tensor = None
+
+    def prep(self):
+        import PIL
+
+        def is_hot(a):
+            ''' If the image is grayscale, it checks if it's above the middle threshold (more white)'''
+            in_upper_hot_quadrant = (128 < a[:,:,0])
+            return in_upper_hot_quadrant
+
+        t_3d_for_trait_all = []
+        for slice_name in self._slices:
+            trait_images_per_slice = []
+            for trait in self._traits:
+                path_trait = self._path + '/{}'.format(trait)
+                path_slice = path_trait + '/{}.{}'.format(slice_name, self._img_format)
+                im = PIL.Image.open(path_slice)
+
+                im = im.convert('RGB')
+                im_arr = np.asarray(im)
+                im_arr = is_hot(im_arr) * 1
+
+                plot_heatmap(im_arr, 'images_bin_intensity_{}_{}'.format(trait,path_slice.split('/')[-1]))
+                im_arr = np.expand_dims(im_arr, -1)
+                im_arr = np.expand_dims(im_arr, -1)
+                trait_images_per_slice.append(im_arr)
+                im.close()
+            t_3d_for_trait = np.concatenate(trait_images_per_slice, axis=-1)
+            t_3d_for_trait_all.append(t_3d_for_trait)
+        self.trait_tensor = np.concatenate(t_3d_for_trait_all, axis=2)
+
+        return self.trait_tensor
```

### Comparing `hta-0.0.2/hta_stats/hta.egg-info/PKG-INFO` & `hta-0.1.0/hta_stats/hta.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: hta
-Version: 0.0.2
+Version: 0.1.0
 Summary: Statistically assess the level of both spatial and global heterogeneity within a spatial sample.
 Home-page: https://github.com/alonalj/hta
 Author: Alona Levy-Jurgenson
 Author-email: levyalona@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/alonalj/hta/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
 # Welcome to the HTA package!
 
 The HTA package can statistically assess the level of both spatial, and global, heterogeneity within a spatial sample. HTA was specifically designed to handle multivariate spatial transcriptomics data, such as Visium samples (10x Genomics), but can be used in other domains (see our paper [1] for further details).
 
-## Prerequisites
-Python 3.8 or above.
+If you use hta in your research, pleas cite: [Levy-Jurgenson et al. (Bioinformatics, 2021) [1].](https://doi.org/10.1093/bioinformatics/btab569)
+
+## Installation
+You will need Python 3.8 or above.
+
+To install the package and follow along with our examples below use the following command:
+
+    pip install hta
 
 ## Support and bug reports
-If you encounter any issues, please contact levyalona at gmail.
+If you encounter any issues, please contact levy alona (as one word) through gmail.
 
 # Example 1 - Synthetic Data
 
 ### Input format:
 
 Since generating a trait-combination matrix may be complicated, HTA generates it for you from a simpler form of input: a stacked set of matrices where each matrix represents one trait, and each entry indicates if the trait manifests or not (0/1) at the corresponding spatial position. 
 
@@ -78,34 +83,33 @@
     rr = hta.region_report(trait_names)
     rr.to_csv('region_report.csv')
 
 # Example 2 - Visium data
 
 If you are analysing Visium spatial gene expression data (e.g. any of those listed [here](https://support.10xgenomics.com/spatial-gene-expression/datasets), or [this one](https://support.10xgenomics.com/spatial-gene-expression/datasets/1.1.0/V1_Breast_Cancer_Block_A_Section_1) used in our examples below) you can use our `Visium` built-in class to generate the input format for HTA (i.e., the `t` as in Example 1). 
 
-Make sure you have the following folders from your Visium data:
+Make sure you have obtained the following files for your Visium data:
 
 > filtered_feature_bc_matrix
+>
 > spatial
 
 and place them in a folder hierarchy as shown below (all shown files are required, and all file/folder names must be identical to those shown below, except for the data folder name):
  ```
 YOUR_DATA_FOLDER
 └───filtered_feature_bc_matrix
 │   │   barcodes.tsv.gz
 │   │   features.tsv.gz
 │   │   matrix.mtx.gz
 └───spatial
 	│   tissue_positions_list.csv
 	│   ...
 ```
 
-additionally, your project should have an 'out' folder. 
-
-You are now ready to load your Visium data and use HTA:
+You are now ready to load your Visium data and use HTA. The following code loads the data (note that this may take around 30s), prepares it for HTA analysis, and computes the HTA p-value:
 
     from hta.stats import HTA  
     from hta.utils import Visium    
     
     path = "/PATH_TO/YOUR_DATA_FOLDER" # TODO: insert path to 'YOUR_DATA_FOLDER' (no '/' on end)
     trait_names = ['ERBB2', 'CD8A']   # names of features to use in features.tsv.gz  
       
@@ -114,19 +118,21 @@
     visium.load()  
     t, t_mask = visium.prep(trait_names)  
       
     # compute HTA and HTA p-val  
     region_size = 15   # modify region_size as needed
     hta = HTA(t, region_size=region_size, tissue_mask=t_mask) 
     hta_stat, hta_pval = hta.calc()
+    print("HTA p-value: ", hta_pval)
 
 >What is `t_mask`? It identifies, using barcodes.tsv.gz, which barcodes are under
 > the tissue, and is used to discard barcodeds that are not.
 
-Now we can proceed to produce the heterogeneity map and region report (we've left the p-val title formatting in the example below for your convenience, but you can replace it with your own title format):
+Now we can proceed to produce the heterogeneity map and region report. The code below uses the results from the previous block of code
+ to generate the heterogeneity map and region report. We've left the p-val title formatting code for your convenience so that you can easily replace it with your own title format:
 
   
     import math
     
     # generate heterogeneity map and legend
     hm = hta.plot_heterogeneity_map(trait_names, dot_size=8)  
     hm.legend(loc='upper center', bbox_to_anchor=(0.5, -0.15), ncol=4, fontsize=9)  
@@ -140,37 +146,39 @@
         title = 'HTA {:.2f} (p-val: 10^{:.0f}), region size: {}'.format(hta_stat, hta_pval, region_size)  
     else:  
         title = 'HTA {:.2f} (p-val: {:.2f}), region size: {}'.format(hta_stat, hta_pval, region_size)  
     
     # save heterogeneity map 
     font_dict = {'family': 'normal', 'size': 9}  
     hm.title(title, fontdict=font_dict)  
-    hm.savefig('../out/{}_hetero_map.jpeg'.format('_'.join(trait_names)), dpi=350)  
+    hm.savefig('{}_hetero_map.jpeg'.format('_'.join(trait_names)), dpi=350)  
     hm.close()  
       
     # save region report  
     rr = hta.region_report(trait_names)  
-    rr.to_csv('../out/{}_region_report.csv'.format('_'.join(trait_names)))
+    rr.to_csv('{}_region_report.csv'.format('_'.join(trait_names)))
 
 
 
 
 # Example 3 - Visium with cluster id per barcode
 
+(*) This is slightly more advanced. We recommend going through the previous Visium example before attempting this one.
+
 You can also use HTA with cluster IDs generated per barcode. The best example is using the cluster IDs provided in Visium's analysis folder, but you can use your own cluster IDs, provided they have the same format. 
 
-As an example, you can place Visium's 'analysis' folder (see links above) under your 'data_folder'. The 'analysis' folder contains many k-means clustering results where each barcode has a cluster ID.  
+As an example, you can place Visium's 'analysis' folder (see links above) under your 'YOUR_DATA_FOLDER'. The 'analysis' folder contains many k-means clustering results where each barcode has a cluster ID.  
 
 The main differences in the code below compared to Example 2 above are in the lines of code marked with (***):
 
 
     from hta.utils import Visium  
     from hta.stats import HTA  
       
-    path = "../res/data_folder"  
+    path = "/PATH_TO/YOUR_DATA_FOLDER" # TODO: insert path to 'YOUR_DATA_FOLDER' (no '/' on end)
     k = 10
     clusters_path = '{}/analysis/clustering/kmeans_{}_clusters/clusters.csv'.format(path, k)
     trait_names = [str(i+1) for i in range(k)]  
       
     visium = Visium(path)  
     visium.load()  
     t, t_mask = visium.prep_clusters(clusters_path)  # (***)
@@ -192,8 +200,7 @@
     hm.close()  
       
     # save region report  
     rr = hta.region_report(trait_names)  
     rr.to_csv('../out/{}_region_report.csv'.format('_'.join(trait_names)))
 
 [1] Assessing heterogeneity in spatial data using the HTA index with applications to spatial transcriptomics and imaging. *Levy-Jurgenson et al.* 
-
```

### Comparing `hta-0.0.2/setup.py` & `hta-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hta",
-    version="0.0.2",
+    version="0.1.0",
     author="Alona Levy-Jurgenson",
     author_email="levyalona@gmail.com",
     description="Statistically assess the level of both spatial and global heterogeneity within a spatial sample.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alonalj/hta",
     project_urls={
```


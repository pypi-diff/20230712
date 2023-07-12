# Comparing `tmp/bbknn-1.5.1.tar.gz` & `tmp/bbknn-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/krzysztofpolanski/Documents/bbknn/dist/tmpabj2z9d7/bbknn-1.5.1.tar", last modified: Wed Jun  2 18:58:34 2021, max compression
+gzip compressed data, was "bbknn-1.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bbknn-1.5.1.tar` & `bbknn-1.6.0.tar`

### file list

```diff
@@ -1,16 +1,32 @@
-drwxr-xr-x   0 krzysztofpolanski   (501) staff       (20)        0 2021-06-02 18:58:34.000000 bbknn-1.5.1/
--rw-r--r--   0 krzysztofpolanski   (501) staff       (20)     1073 2021-05-24 11:13:50.000000 bbknn-1.5.1/LICENSE
--rw-r--r--   0 krzysztofpolanski   (501) staff       (20)       16 2021-05-24 11:13:50.000000 bbknn-1.5.1/MANIFEST.in
--rw-r--r--   0 krzysztofpolanski   (501) staff       (20)      279 2021-06-02 18:58:34.000000 bbknn-1.5.1/PKG-INFO
--rw-r--r--   0 krzysztofpolanski   (501) staff       (20)     7529 2021-06-02 17:37:35.000000 bbknn-1.5.1/README.md
-drwxr-xr-x   0 krzysztofpolanski   (501) staff       (20)        0 2021-06-02 18:58:34.000000 bbknn-1.5.1/bbknn/
--rw-r--r--   0 krzysztofpolanski   (501) staff       (20)    12685 2021-06-02 18:56:40.000000 bbknn-1.5.1/bbknn/__init__.py
--rw-r--r--   0 krzysztofpolanski   (501) staff       (20)    13642 2021-06-02 18:34:55.000000 bbknn-1.5.1/bbknn/matrix.py
-drwxr-xr-x   0 krzysztofpolanski   (501) staff       (20)        0 2021-06-02 18:58:34.000000 bbknn-1.5.1/bbknn.egg-info/
--rw-r--r--   0 krzysztofpolanski   (501) staff       (20)      279 2021-06-02 18:58:33.000000 bbknn-1.5.1/bbknn.egg-info/PKG-INFO
--rw-r--r--   0 krzysztofpolanski   (501) staff       (20)      216 2021-06-02 18:58:34.000000 bbknn-1.5.1/bbknn.egg-info/SOURCES.txt
--rw-r--r--   0 krzysztofpolanski   (501) staff       (20)        1 2021-06-02 18:58:33.000000 bbknn-1.5.1/bbknn.egg-info/dependency_links.txt
--rw-r--r--   0 krzysztofpolanski   (501) staff       (20)       86 2021-06-02 18:58:33.000000 bbknn-1.5.1/bbknn.egg-info/requires.txt
--rw-r--r--   0 krzysztofpolanski   (501) staff       (20)        6 2021-06-02 18:58:33.000000 bbknn-1.5.1/bbknn.egg-info/top_level.txt
--rw-r--r--   0 krzysztofpolanski   (501) staff       (20)       38 2021-06-02 18:58:34.000000 bbknn-1.5.1/setup.cfg
--rw-r--r--   0 krzysztofpolanski   (501) staff       (20)      474 2021-06-02 18:41:30.000000 bbknn-1.5.1/setup.py
+-rw-r--r--   0        0        0      136 2023-07-12 16:34:25.000000 bbknn-1.6.0/.gitignore
+-rw-r--r--   0        0        0      470 2023-07-12 16:34:25.000000 bbknn-1.6.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     3100 2023-07-12 16:34:25.000000 bbknn-1.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1073 2023-07-12 16:34:25.000000 bbknn-1.6.0/LICENSE
+-rw-r--r--   0        0        0       16 2023-07-12 16:34:25.000000 bbknn-1.6.0/MANIFEST.in
+-rw-r--r--   0        0        0     7586 2023-07-12 16:34:25.000000 bbknn-1.6.0/README.md
+-rw-r--r--   0        0        0    11545 2023-07-12 16:34:25.000000 bbknn-1.6.0/bbknn/__init__.py
+-rw-r--r--   0        0        0    15457 2023-07-12 16:34:25.000000 bbknn-1.6.0/bbknn/matrix.py
+-rw-r--r--   0        0        0      603 2023-07-12 16:34:25.000000 bbknn-1.6.0/docs/Makefile
+-rw-r--r--   0        0        0     4926 2023-07-12 16:34:25.000000 bbknn-1.6.0/docs/conf.py
+-rw-r--r--   0        0        0      582 2023-07-12 16:34:25.000000 bbknn-1.6.0/docs/index.rst
+-rw-r--r--   0        0        0      120 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/README.md
+-rw-r--r--   0        0        0      156 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/benchmark-times/annoy.txt
+-rw-r--r--   0        0        0      154 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/benchmark-times/bbknn.txt
+-rw-r--r--   0        0        0       85 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/benchmark-times/cca.txt
+-rw-r--r--   0        0        0       85 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/benchmark-times/conos.txt
+-rw-r--r--   0        0        0      170 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/benchmark-times/faiss.txt
+-rw-r--r--   0        0        0      151 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/benchmark-times/harmony.txt
+-rw-r--r--   0        0        0       85 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/benchmark-times/mnn.txt
+-rw-r--r--   0        0        0       84 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/benchmark-times/scanorama.txt
+-rw-r--r--   0        0        0       85 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/benchmark-times/seurat3.txt
+-rw-r--r--   0        0        0    28089 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/benchmark.ipynb
+-rw-r--r--   0        0        0   142188 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/benchmark2.ipynb
+-rw-r--r--   0        0        0    12354 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/benchmark3-new-R-methods.ipynb
+-rw-r--r--   0        0        0  2194925 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/demo.ipynb
+-rw-r--r--   0        0        0   694695 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/mouse-harmony.ipynb
+-rw-r--r--   0        0        0  8187007 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/mouse.ipynb
+-rw-r--r--   0        0        0   546660 2023-07-12 16:34:26.000000 bbknn-1.6.0/examples/simulation.ipynb
+-rw-r--r--   0        0        0   320537 2023-07-12 16:34:26.000000 bbknn-1.6.0/figures/batch1.png
+-rw-r--r--   0        0        0   329696 2023-07-12 16:34:26.000000 bbknn-1.6.0/figures/batch2.png
+-rw-r--r--   0        0        0      726 2023-07-12 16:34:26.000000 bbknn-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8170 1970-01-01 00:00:00.000000 bbknn-1.6.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bbknn-1.5.1/LICENSE` & `bbknn-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbknn-1.5.1/README.md` & `bbknn-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,65 +20,80 @@
 	  year={2019}
 	}
 
 ## Installation
 
 BBKNN depends on Cython, numpy, scipy, annoy, pynndescent, umap-learn and scikit-learn. The package is available on pip and conda, and can be easily installed as follows:
 
-	pip3 install bbknn
+```bash
+pip3 install bbknn
+```
 
 or
 
-	conda install -c bioconda bbknn
+```bash
+conda install -c bioconda bbknn
+```
 
 BBKNN can also make use of faiss. Consult the [official installation instructions](https://github.com/facebookresearch/faiss/blob/master/INSTALL.md), the easiest way to get it is via conda.
 
 ## Usage and Documentation
 
 BBKNN has the option to immediately slot into the spot occupied by `scanpy.neighbors()` in the [Seurat-inspired scanpy workflow](https://nbviewer.jupyter.org/github/theislab/scanpy_usage/blob/master/170505_seurat/seurat.ipynb). It computes a batch aligned variant of the neighbourhood graph, with its uses within scanpy including clustering, diffusion map pseudotime inference and UMAP visualisation. The basic syntax to run BBKNN on scanpy's AnnData object (with PCA computed via `scanpy.tl.pca()`) is as follows:
 
-	import bbknn
-	bbknn.bbknn(adata)
+```python3
+import bbknn
+
+bbknn.bbknn(adata)
+```
 
 You can provide which `adata.obs` column to use for batch discrimination via the `batch_key` parameter. This defaults to `'batch'`, which is created by scanpy when you merge multiple AnnData objects (e.g. if you were to import multiple samples separately and then concatenate them).
 
 Integration can be improved by using ridge regression on both a technical effect and a biological grouping prior to BBKNN, following a workflow from [Park _et al._, 2020](https://science.sciencemag.org/content/367/6480/eaay3224.abstract). In the event of not having a biological grouping at hand, a coarse clustering obtained from a BBKNN-corrected graph can be used in its place. This creates the following basic workflow syntax:
 
-	import bbknn
-	import scanpy
-	bbknn.bbknn(adata)
-	scanpy.tl.leiden(adata)
-	bbknn.ridge_regression(adata, batch_key=['batch'], confounder_key=['leiden'])
-	scanpy.tl.pca(adata)
-	bbknn.bbknn(adata)
+```python3
+import bbknn
+import scanpy
+
+bbknn.bbknn(adata)
+scanpy.tl.leiden(adata)
+bbknn.ridge_regression(adata, batch_key=['batch'], confounder_key=['leiden'])
+scanpy.tl.pca(adata)
+bbknn.bbknn(adata)
+```
 
 Alternately, you can just provide a PCA matrix with cells as rows and a matching vector of batch assignments for each of the cells and call BBKNN as follows (with `connectivities` being the primary graph output of interest):
 
-	import bbknn.matrix
-	distances, connectivities, parameters = bbknn.matrix.bbknn(pca_matrix, batch_list)
+```python3
+import bbknn.matrix
+
+distances, connectivities, parameters = bbknn.matrix.bbknn(pca_matrix, batch_list)
+```
 
 An HTML render of the BBKNN function docstring, detailing all the parameters, can be accessed at [ReadTheDocs](https://bbknn.readthedocs.io/en/latest/). BBKNN use, along with using ridge regression to improve the integration, is shown in a [demonstration notebook](https://nbviewer.jupyter.org/github/Teichlab/bbknn/blob/master/examples/demo.ipynb).
 
 ## BBKNN in R
 
 At this point, there is no plan to create a BBKNN R package. However, it can be ran quite easily via reticulate. Using the base functions is the same as in python. If you're in possession of a PCA matrix and a batch assignment vector and want to get UMAP coordinates out of it, you can use the following code snippet to do so. The weird PCA computation part and replacing it with your original values is unfortunately necessary due to how AnnData innards operate from a reticulate level. Provide your python path in `use_python()`
 
-	library(reticulate)
-	use_python("/usr/bin/python3")
-
-	anndata = import("anndata",convert=FALSE)
-	bbknn = import("bbknn", convert=FALSE)
-	sc = import("scanpy",convert=FALSE)
-
-	adata = anndata$AnnData(X=pca, obs=batch)
-	sc$tl$pca(adata)
-	adata$obsm$X_pca = pca
-	bbknn$bbknn(adata,batch_key=0)
-	sc$tl$umap(adata)
-	umap = py_to_r(adata$obsm[["X_umap"]])
+```R
+library(reticulate)
+use_python("/usr/bin/python3")
+
+anndata = import("anndata",convert=FALSE)
+bbknn = import("bbknn", convert=FALSE)
+sc = import("scanpy",convert=FALSE)
+
+adata = anndata$AnnData(X=pca, obs=batch)
+sc$tl$pca(adata)
+adata$obsm$X_pca = pca
+bbknn$bbknn(adata,batch_key=0)
+sc$tl$umap(adata)
+umap = py_to_r(adata$obsm[["X_umap"]])
+```
 
 If you wish to change any integer arguments (such as `neighbors_within_batch`), you'll have to `as.integer()` the value so python understands it as an integer.
 
 When testing locally, faiss refused to work when BBKNN was reticulated. As such, provide `use_faiss=FALSE` to the BBKNN call if you run into this problem.
 
 ## Example Notebooks
```

### Comparing `bbknn-1.5.1/bbknn/__init__.py` & `bbknn-1.6.0/bbknn/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,35 @@
+"""Batch balanced KNN"""
+__version__ = "1.6.0"
+
 import pandas as pd
 import numpy as np
 import scipy
 import sys
-from bbknn.matrix import bbknn as bbknn_matrix
-from bbknn.matrix import check_knn_metric
-from packaging import version
 from sklearn.linear_model import Ridge
 try:
 	from scanpy import logging as logg
 except ImportError:
 	pass
-try:
-	import anndata
-except ImportError:
-	pass
 
+from . import matrix
 
-def bbknn(adata, batch_key='batch', use_rep='X_pca', approx=True, use_annoy=True, 
-		  metric='euclidean', copy=False, **kwargs):
+def bbknn(adata, batch_key='batch', use_rep='X_pca', key_added=None, copy=False, **kwargs):
 	'''
 	Batch balanced KNN, altering the KNN procedure to identify each cell's top neighbours in
 	each batch separately instead of the entire cell pool with no accounting for batch. 
 	The nearest neighbours for each batch are then merged to create a final list of 
 	neighbours for the cell.
 	Aligns batches in a quick and lightweight manner.
 	For use in the scanpy workflow as an alternative to ``scanpy.pp.neighbors()``.
 
 	Input
 	-----
 	adata : ``AnnData``
-		Needs the PCA computed and stored in ``adata.obsm["X_pca"]``.
+		Needs your dimensionality reduction of choice computed and stored in ``.obsm``.
 	batch_key : ``str``, optional (default: "batch")
 		``adata.obs`` column name discriminating between your batches.
 	neighbors_within_batch : ``int``, optional (default: 3)
 		How many top neighbours to report for each batch; total number of neighbours in 
 		the initial k-nearest-neighbours computation will be this number times the number 
 		of batches. This then serves as the basis for the construction of a symmetrical 
 		matrix of connectivities.
@@ -43,36 +39,29 @@
 		How many dimensions (in case of PCA, principal components) to use in the analysis.
 	trim : ``int`` or ``None``, optional (default: ``None``)
 		Trim the neighbours of each cell to these many top connectivities. May help with
 		population independence and improve the tidiness of clustering. The lower the value the
 		more independent the individual populations, at the cost of more conserved batch effect.
 		If ``None``, sets the parameter value automatically to 10 times ``neighbors_within_batch`` 
 		times the number of batches. Set to 0 to skip.
-	approx : ``bool``, optional (default: ``True``)
-		If ``True``, use approximate neighbour finding - annoy or pyNNDescent. This results 
-		in a quicker run time for large datasets while also potentially increasing the degree of 
-		batch correction.
-	use_annoy : ``bool``, optional (default: ``True``)
-		Only used when ``approx=True``. If ``True``, will use annoy for neighbour finding. If
-		``False``, will use pyNNDescent instead.
+	computation : ``str``, optional (default: "annoy")
+		Which KNN algorithm to use. BBKNN supports the approximate neighbour search of "annoy" 
+		and "pynndescent", and the exact neighbour search of "faiss", "cKDTree" and "KDTree". 
+		Available metric choices depend on the package used here.
 	annoy_n_trees : ``int``, optional (default: 10)
 		Only used with annoy neighbour identification. The number of trees to construct in the 
 		annoy forest. More trees give higher precision when querying, at the cost of increased 
 		run time and resource intensity.
 	pynndescent_n_neighbors : ``int``, optional (default: 30)
 		Only used with pyNNDescent neighbour identification. The number of neighbours to include
 		in the approximate neighbour graph. More neighbours give higher precision when querying, 
 		at the cost of increased run time and resource intensity.
 	pynndescent_random_state : ``int``, optional (default: 0)
 		Only used with pyNNDescent neighbour identification. The RNG seed to use when creating 
 		the graph.
-	use_faiss : ``bool``, optional (default: ``True``)
-		If ``approx=False`` and the metric is "euclidean", use the faiss package to compute
-		nearest neighbours if installed. This improves performance at a minor cost to numerical
-		precision as faiss operates on float32.
 	metric : ``str`` or ``sklearn.neighbors.DistanceMetric`` or ``types.FunctionType``, optional (default: "euclidean")
 		What distance metric to use. The options depend on the choice of neighbour algorithm.
 		
 		"euclidean", the default, is always available.
 		
 		Annoy supports "angular", "manhattan" and "hamming".
 		
@@ -82,20 +71,20 @@
 		>>> pynndescent.distances.named_distances.keys()
 		dict_keys(['euclidean', 'l2', 'sqeuclidean', 'manhattan', 'taxicab', 'l1', 'chebyshev', 'linfinity', 
 		'linfty', 'linf', 'minkowski', 'seuclidean', 'standardised_euclidean', 'wminkowski', 'weighted_minkowski', 
 		'mahalanobis', 'canberra', 'cosine', 'dot', 'correlation', 'hellinger', 'haversine', 'braycurtis', 'spearmanr', 
 		'kantorovich', 'wasserstein', 'tsss', 'true_angular', 'hamming', 'jaccard', 'dice', 'matching', 'kulsinski', 
 		'rogerstanimoto', 'russellrao', 'sokalsneath', 'sokalmichener', 'yule'])
 		
-		KDTree supports members of the ``sklearn.neighbors.KDTree.valid_metrics`` list, or parameterised
-		``sklearn.neighbors.DistanceMetric`` `objects
-		<https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.DistanceMetric.html>`_:
+		KDTree supports members of the ``sklearn.neighbors.KDTree.valid_metrics()`` list, or parameterised
+		``sklearn.metrics.DistanceMetric`` `objects
+		<https://scikit-learn.org/stable/modules/generated/sklearn.metrics.DistanceMetric.html>`_:
 
-		>>> sklearn.neighbors.KDTree.valid_metrics
-		['p', 'chebyshev', 'cityblock', 'minkowski', 'infinity', 'l2', 'euclidean', 'manhattan', 'l1']
+		>>> sklearn.neighbors.KDTree.valid_metrics()
+		['euclidean', 'l2', 'minkowski', 'p', 'manhattan', 'cityblock', 'l1', 'chebyshev', 'infinity']
 	set_op_mix_ratio : ``float``, optional (default: 1)
 		UMAP connectivity computation parameter, float between 0 and 1, controlling the
 		blend between a connectivity matrix formed exclusively from mutual nearest neighbour
 		pairs (0) and a union of all observed neighbour relationships with the mutual pairs
 		emphasised (1)
 	local_connectivity : ``int``, optional (default: 1)
 		UMAP connectivity computation parameter, how many nearest neighbors of each cell
@@ -108,47 +97,41 @@
 	#basic sanity checks to begin
 	#is our batch key actually present in the object?
 	if batch_key not in adata.obs:
 		raise ValueError("Batch key '"+batch_key+"' not present in `adata.obs`.")
 	#do we have a computed PCA?
 	if use_rep not in adata.obsm.keys():
 		raise ValueError("Did not find "+use_rep+" in `.obsm.keys()`. You need to compute it first.")
-	#metric sanity checks, using the bbknn.matrix function
-	#set up a fake params with the arguments that impact the metric correction outcome
-	params = {'approx':approx, 'use_annoy':use_annoy, 'metric':metric, 'use_faiss':False}
-	params = check_knn_metric(params, adata.obs[batch_key].value_counts(), True)
-	#this fake params has the corrected metric, and appropriate logging was made
 	#prepare bbknn.matrix.bbknn input
 	pca = adata.obsm[use_rep]
 	batch_list = adata.obs[batch_key].values
-	#call BBKNN proper
-	bbknn_out = bbknn_matrix(pca=pca, batch_list=batch_list, approx=approx,
-							 use_annoy=use_annoy, metric=params['metric'], **kwargs)
-	#store the parameters in .uns['neighbors']['params'], add use_rep and batch_key
-	adata.uns['neighbors'] = {}
-	adata.uns['neighbors']['params'] = bbknn_out[2]
-	adata.uns['neighbors']['params']['use_rep'] = use_rep
-	adata.uns['neighbors']['params']['bbknn']['batch_key'] = batch_key
-	#store the graphs in .uns['neighbors'] or .obsp, conditional on anndata version
-	if version.parse(str(anndata.__version__)) < version.parse('0.7.0'):
-		adata.uns['neighbors']['distances'] = bbknn_out[0]
-		adata.uns['neighbors']['connectivities'] = bbknn_out[1]
-		logg.info('	finished', time=start,
-			deep=('added to `.uns[\'neighbors\']`\n'
-			'	\'distances\', distances for each pair of neighbors\n'
-			'	\'connectivities\', weighted adjacency matrix'))
+	#call BBKNN proper, telling it to use scanpy logging for its internal things
+	bbknn_out = matrix.bbknn(pca=pca, batch_list=batch_list, scanpy_logging=True, **kwargs)
+	#store the parameters, add use_rep and batch_key
+	#mirror scanpy neighbour key_added logic
+	if key_added is None:
+		key_added = 'neighbors'
+		conns_key = 'connectivities'
+		dists_key = 'distances'
 	else:
-		adata.obsp['distances'] = bbknn_out[0]
-		adata.obsp['connectivities'] = bbknn_out[1]
-		adata.uns['neighbors']['distances_key'] = 'distances'
-		adata.uns['neighbors']['connectivities_key'] = 'connectivities'
-		logg.info('	finished', time=start,
-			deep=('added to `.uns[\'neighbors\']`\n'
-			'	`.obsp[\'distances\']`, distances for each pair of neighbors\n'
-			'	`.obsp[\'connectivities\']`, weighted adjacency matrix'))
+		conns_key = key_added + '_connectivities'
+		dists_key = key_added + '_distances'
+	adata.uns[key_added] = {}
+	adata.uns[key_added]['params'] = bbknn_out[2]
+	adata.uns[key_added]['params']['use_rep'] = use_rep
+	adata.uns[key_added]['params']['bbknn']['batch_key'] = batch_key
+	#store the graphs in an anndata 0.7.0+ compliant manner
+	adata.obsp[dists_key] = bbknn_out[0]
+	adata.obsp[conns_key] = bbknn_out[1]
+	adata.uns[key_added]['distances_key'] = dists_key
+	adata.uns[key_added]['connectivities_key'] = conns_key
+	logg.info('	finished', time=start,
+		deep=(f'added to `.uns[{key_added!r}]`\n'
+		f'    `.obsp[{dists_key!r}]`, distances for each pair of neighbors\n'
+		f'    `.obsp[{conns_key!r}]`, weighted adjacency matrix'))
 	return adata if copy else None
 
 def ridge_regression(adata, batch_key, confounder_key=[], chunksize=1e8, copy=False, **kwargs):
 	'''
 	Perform ridge regression on scaled expression data, accepting both technical and 
 	biological categorical variables. The effect of the technical variables is removed 
 	while the effect of the biological variables is retained. This is a preprocessing 
@@ -201,15 +184,15 @@
 	#(as the data is centered). create holders for results
 	LR = Ridge(fit_intercept=False, **kwargs)
 	X_explained = []
 	X_remain = []
 	#loop over the gene space in chunkcount-sized chunks
 	for ind in np.arange(0,adata.shape[1],chunkcount):
 		#extract the expression and turn to dense if need be
-		X_exp = adata.X[:,np.int(ind):np.int(ind+chunkcount)] # scaled data
+		X_exp = adata.X[:,int(ind):int(ind+chunkcount)] # scaled data
 		if scipy.sparse.issparse(X_exp):
 			X_exp = X_exp.todense()
 		#fit the ridge regression model, compute the expression explained by the technical 
 		#effect, and the remaining residual
 		LR.fit(dummy,X_exp)	
 		X_explained.append(dm.dot(LR.coef_[:,batch_index].T))
 		X_remain.append(X_exp - X_explained[-1])
```

### Comparing `bbknn-1.5.1/bbknn/matrix.py` & `bbknn-1.6.0/bbknn/matrix.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+import warnings
 import pandas as pd
 import numpy as np
 import scipy
 import types
 import sys
 from annoy import AnnoyIndex
 import pynndescent
-from packaging import version
 from scipy.spatial import cKDTree
 from scipy.sparse import coo_matrix
 from umap.umap_ import fuzzy_simplicial_set
+from sklearn.metrics import DistanceMetric
 from sklearn.neighbors import KDTree
-from sklearn.neighbors import DistanceMetric
 try:
 	from scanpy import logging as logg
 except ImportError:
 	pass
 try:
 	import faiss
 except ImportError:
@@ -133,15 +133,15 @@
 	elif params['computation'] == 'faiss':
 		D, I = ckd.search(data, params['neighbors_within_batch'])
 		#sometimes this turns up marginally negative values, just set those to zero
 		D[D<0] = 0
 		#the distance returned by faiss needs to be square rooted to be actual euclidean
 		ckdout = (np.sqrt(D), I)
 	elif params['computation'] == 'cKDTree':
-		ckdout = ckd.query(x=data, k=params['neighbors_within_batch'], n_jobs=-1)
+		ckdout = ckd.query(x=data, k=params['neighbors_within_batch'], workers=-1)
 	elif params['computation'] == 'KDTree':
 		ckdout = ckd.query(data, k=params['neighbors_within_batch'])
 	return ckdout
 
 def get_graph(pca, batch_list, params):
 	'''
 	Identify the KNN structure to be used in graph construction. All input as in ``bbknn.bbknn()``
@@ -169,87 +169,127 @@
 		#create a boolean mask identifying the cells within this batch
 		#and then get the corresponding row numbers for later use
 		batch_to = batches[to_ind]
 		mask_to = batch_list == batch_to
 		ind_to = np.arange(len(batch_list))[mask_to]
 		#create the faiss/cKDTree/KDTree/annoy, depending on approx/metric
 		ckd = create_tree(data=pca[mask_to,:params['n_pcs']], params=params)
-		for from_ind in range(len(batches)):
-			#this is the batch that will have its neighbours identified
-			#repeat the mask/row number getting
-			batch_from = batches[from_ind]
-			mask_from = batch_list == batch_from
-			ind_from = np.arange(len(batch_list))[mask_from]
-			#fish the neighbours out, getting a (distances, indices) tuple back
-			ckdout = query_tree(data=pca[mask_from,:params['n_pcs']], ckd=ckd, params=params)
-			#the identified indices are relative to the subsetted PCA matrix
-			#so we need to convert it back to the original row numbers
-			for i in range(ckdout[1].shape[0]):
-				for j in range(ckdout[1].shape[1]):
-					ckdout[1][i,j] = ind_to[ckdout[1][i,j]]
-			#save the results within the appropriate rows and columns of the structures
-			col_range = np.arange(to_ind*params['neighbors_within_batch'], (to_ind+1)*params['neighbors_within_batch'])
-			knn_indices[ind_from[:,None],col_range[None,:]] = ckdout[1]
-			knn_distances[ind_from[:,None],col_range[None,:]] = ckdout[0]
+		#fish the neighbours out, getting a (distances, indices) tuple back
+		ckdout = query_tree(data=pca[:,:params['n_pcs']], ckd=ckd, params=params)
+		#save the results within the appropriate columns of the structures
+		#this batch gets the to_ind'th interval neighbors_within_batch wide
+		col_range = np.arange(to_ind*params['neighbors_within_batch'], (to_ind+1)*params['neighbors_within_batch'])
+		#the identified indices are relative to the subsetted PCA matrix
+		#so we need to convert it back to the original row numbers
+		knn_indices[:,col_range] = ind_to[ckdout[1]]
+		knn_distances[:,col_range] = ckdout[0]
 	return knn_distances, knn_indices
 
-def check_knn_metric(params, counts, scanpy_logging=False):
+def print_warning(message, scanpy_logging):
+	'''
+	Print a specified warning to the screen, using either warnings or scanpy.
+	
+	Input
+	-----
+	message : ``str``
+		The warning message to print
+	scanpy_logging : ``bool``
+		Whether to use scanpy logging to print updates rather than ``warnings.warn()``
+	'''
+	if scanpy_logging:
+		logg.warning(message)
+	else:
+		warnings.warn(message)
+
+def legacy_computation_selection(params, scanpy_logging):
+	'''
+	Do pre-1.6.0 computation algorithm selection based on possible legacy arguments. Looks 
+	at the following (default None) parameters: approx, use_annoy, use_faiss
+	
+	Input
+	-----
+	params : ``dict``
+		A dictionary of arguments used to call ``bbknn.matrix.bbknn()``
+	scanpy_logging : ``bool``
+		Whether to use scanpy logging to print updates rather than ``warnings.warn()``
+	'''
+	#if these are not None then they were set at the time of the call
+	if any([params[i] is not None for i in ['approx','use_annoy','use_faiss']]):
+		#encourage upgrading the call
+		print_warning('consider updating your call to make use of `computation`', scanpy_logging)
+		#fill in any missing defaults
+		if params['approx'] is None:
+			params['approx'] = True
+		if params['use_annoy'] is None:
+			params['use_annoy'] = True
+		if params['use_faiss'] is None:
+			params['use_faiss'] = True
+		#now that we have all the old defaults restored, use them to pick a computation
+		if params['approx']:
+			#pick between these two packages based on another param
+			if params['use_annoy']:
+				params['computation'] = 'annoy'
+			else:
+				params['computation'] = 'pynndescent'
+		else:
+			#if the metric is euclidean, then pick between these two packages
+			if params['metric'] == 'euclidean':
+				if params['use_faiss'] and 'faiss' in sys.modules:
+					params['computation'] = 'faiss'
+				else:
+					params['computation'] = 'cKDTree'
+			else:
+				params['computation'] = 'KDTree'
+	return params
+
+def check_knn_metric(params, counts, scanpy_logging):
 	'''
 	Checks if the provided metric can be used with the implied KNN algorithm. Returns parameters
-	with the metric altered and the KNN algorithm stated outright in params['computation'].
+	with the metric validated.
 	
 	Input
 	-----
 	params : ``dict``
 		A dictionary of arguments used to call ``bbknn.matrix.bbknn()``
 	counts : ``np.array``
 		The number of cells in each batch
-	scanpy_logging : ``bool``, optional (default: ``False``)
-		Whether to use scanpy logging to print updates rather than a ``print()``
+	scanpy_logging : ``bool``
+		Whether to use scanpy logging to print updates rather than ``warnings.warn()``
 	'''
 	#take note if we end up going back to Euclidean
 	swapped = False
-	if params['approx']:
-		#we're approximate
-		if params['use_annoy']:
-			params['computation'] = 'annoy'
-			if params['metric'] not in ['angular', 'euclidean', 'manhattan', 'hamming']:
-				swapped = True
-				params['metric'] = 'euclidean'
-		else:
-			params['computation'] = 'pynndescent'
-			#pynndescent wants at least 11 cells per batch, from testing
-			if np.min(counts) < 11:
-				raise ValueError("Not all batches have at least 11 cells in them - required by pynndescent.")
-			#metric needs to be a function or in the named list
-			if not (params['metric'] in pynndescent.distances.named_distances or
-					isinstance(params['metric'], types.FunctionType)):
-				swapped = True
-				params['metric'] = 'euclidean'
-	else:
-		#we're not approximate
-		#metric needs to either be a DistanceMetric object or fall in the KDTree name list
-		if not (params['metric']=='euclidean' or 
-				isinstance(params['metric'], DistanceMetric) or 
+	if params['computation'] == 'annoy':
+		if params['metric'] not in ['angular', 'euclidean', 'manhattan', 'hamming']:
+			swapped = True
+	elif params['computation'] == 'pynndescent':
+		if np.min(counts) < 11:
+			raise ValueError("Not all batches have at least 11 cells in them - required by pynndescent.")
+		#metric needs to be a function or in the named list
+		if not (params['metric'] in pynndescent.distances.named_distances or
+				isinstance(params['metric'], types.FunctionType)):
+			swapped = True
+	elif params['computation'] == 'faiss':
+		if params['metric'] != 'euclidean':
+			swapped = True
+	elif params['computation'] == 'cKDTree':
+		if params['metric'] != 'euclidean':
+			swapped = True
+	elif params['computation'] == 'KDTree':
+		if not (isinstance(params['metric'], DistanceMetric) or 
 				params['metric'] in KDTree.valid_metrics):
 			swapped = True
-			params['metric'] = 'euclidean'
-		if params['metric']=='euclidean':
-			if 'faiss' in sys.modules and params['use_faiss']:
-				params['computation']='faiss'
-			else:
-				params['computation']='cKDTree'
-		else:
-			params['computation']='KDTree'
+			#and now for a next level swap - this can be done more efficiently via cKDTree
+			params['computation'] = 'cKDTree'
+	else:
+		raise ValueError("Incorrect value of `computation`.")
 	if swapped:
+		#go back to euclidean
+		params['metric'] = 'euclidean'
 		#need to let the user know we swapped the metric
-		if scanpy_logging:
-			logg.warning('unrecognised metric for type of neighbor calculation, switching to euclidean')
-		else:
-			print('unrecognised metric for type of neighbor calculation, switching to euclidean')
+		print_warning('unrecognised metric for type of neighbor calculation, switching to euclidean', scanpy_logging)
 	return params
 
 def trimming(cnts,trim):
 	'''
 	Trims the graph to the top connectivities for each cell. All undescribed input as in
 	``bbknn.bbknn()``.
 
@@ -274,61 +314,71 @@
 			#apply cutoff
 			row_array[row_array<vals[i]] = 0
 		cnts.eliminate_zeros()
 		cnts = cnts.T.tocsr()
 	return cnts
 
 def bbknn(pca, batch_list, neighbors_within_batch=3, n_pcs=50, trim=None,
-		  approx=True, annoy_n_trees=10, pynndescent_n_neighbors=30, 
-		  pynndescent_random_state=0, use_annoy=True, use_faiss=True, 
-		  metric='euclidean', set_op_mix_ratio=1, local_connectivity=1):
+		  computation='annoy', annoy_n_trees=10, pynndescent_n_neighbors=30, 
+		  pynndescent_random_state=0, metric='euclidean', set_op_mix_ratio=1, 
+		  local_connectivity=1, approx=None, use_annoy=None, use_faiss=None,
+		  scanpy_logging=False):
 	'''
 	Scanpy-independent BBKNN variant that runs on a PCA matrix and list of per-cell batch assignments instead of
 	an AnnData object. Non-data-entry arguments behave the same way as ``bbknn.bbknn()``.
 	Returns a ``(distances, connectivities, parameters)`` tuple, like what would have been stored in the AnnData object.
 	The connectivities are the actual neighbourhood graph.
 
 	Input
 	-----
 	pca : ``numpy.array``
 		PCA (or other dimensionality reduction) coordinates for each cell, with cells as rows.
 	batch_list : ``numpy.array`` or ``list``
 		A list of batch assignments for each cell.
+	scanpy_logging : ``bool``, optional (default: ``False``)
+		Whether to use scanpy logging to print updates rather than ``warnings.warn()``
 	'''
 	#catch all arguments for easy passing to subsequent functions
 	params = locals()
 	del params['pca']
 	del params['batch_list']
 	#more basic sanity checks/processing
 	#do we have the same number of cells in pca and batch_list?
 	if pca.shape[0] != len(batch_list):
 		raise ValueError("Different cell counts indicated by `pca.shape[0]` and `len(batch_list)`.")
+	#make sure n_pcs is not larger than the actual dimensions of the data
+	#as that can introduce some uninformative knock-on errors in UMAP
+	params['n_pcs'] = np.min([params['n_pcs'], pca.shape[1]])
 	#convert batch_list to np.array of strings for ease of mask making later
 	batch_list = np.asarray([str(i) for i in batch_list])
 	#assert that all batches have at least neighbors_within_batch cells in there
 	unique, counts = np.unique(batch_list, return_counts=True)
 	if np.min(counts) < params['neighbors_within_batch']:
 		raise ValueError("Not all batches have at least `neighbors_within_batch` cells in them.")
-	#so what knn algorithm will be using? sanity check the metrics while at it
-	params = check_knn_metric(params, counts)
+	#if any of the old legacy computation selection arguments are detected
+	#use them to select the knn computation algorithm
+	params = legacy_computation_selection(params, scanpy_logging)
+	#sanity check the metric
+	params = check_knn_metric(params, counts, scanpy_logging)
 	#obtain the batch balanced KNN graph
 	knn_distances, knn_indices = get_graph(pca=pca,batch_list=batch_list,params=params)
 	#sort the neighbours so that they're actually in order from closest to furthest
 	newidx = np.argsort(knn_distances,axis=1)
 	knn_indices = knn_indices[np.arange(np.shape(knn_indices)[0])[:,np.newaxis],newidx]
 	knn_distances = knn_distances[np.arange(np.shape(knn_distances)[0])[:,np.newaxis],newidx]
 	#this part of the processing is akin to scanpy.api.neighbors()
 	dist, cnts = compute_connectivities_umap(knn_indices, knn_distances, knn_indices.shape[0],
 											 knn_indices.shape[1], set_op_mix_ratio=set_op_mix_ratio,
 											 local_connectivity=local_connectivity)
 	#trimming. compute default range if absent
+	#both this and the parameter dictionary need a neighbour total for each cell
+	#easiest retrieved from the shape of the knn variables
 	if params['trim'] is None:
-		trim = 10 * knn_distances.shape[1]
+		params['trim'] = 10 * knn_distances.shape[1]
 	#skip trimming if set to 0, otherwise trim
-	if trim > 0:
-		cnts = trimming(cnts=cnts,trim=trim)
-	#create a collated parameters dictionary
-	#we'll have a zero distance for our cell of origin, and nonzero for every other neighbour computed
-	params = {'n_neighbors': len(dist[0,:].data)+1, 'method': 'umap', 
+	if params['trim'] > 0:
+		cnts = trimming(cnts=cnts,trim=params['trim'])
+	#create a collated parameters dictionary, formatted like scanpy's neighbours one
+	p_dict = {'n_neighbors': knn_distances.shape[1], 'method': 'umap', 
 			  'metric': params['metric'], 'n_pcs': params['n_pcs'], 
 			  'bbknn': {'trim': params['trim'], 'computation': params['computation']}}
-	return (dist, cnts, params)
+	return (dist, cnts, p_dict)
```


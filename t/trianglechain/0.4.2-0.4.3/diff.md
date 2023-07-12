# Comparing `tmp/trianglechain-0.4.2.tar.gz` & `tmp/trianglechain-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trianglechain-0.4.2.tar", last modified: Mon Jun 19 13:43:18 2023, max compression
+gzip compressed data, was "trianglechain-0.4.3.tar", last modified: Wed Jul 12 12:14:31 2023, max compression
```

## Comparing `trianglechain-0.4.2.tar` & `trianglechain-0.4.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-19 13:43:18.043530 trianglechain-0.4.2/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-05-04 11:29:54.000000 trianglechain-0.4.2/AUTHORS.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2023-05-04 11:29:54.000000 trianglechain-0.4.2/CONTRIBUTING.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1752 2023-06-19 13:42:54.000000 trianglechain-0.4.2/HISTORY.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-05-04 11:29:54.000000 trianglechain-0.4.2/LICENSE
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-05-04 11:29:54.000000 trianglechain-0.4.2/MANIFEST.in
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-06-19 13:43:18.043597 trianglechain-0.4.2/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-05-04 11:29:54.000000 trianglechain-0.4.2/README.md
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-05-04 11:29:54.000000 trianglechain-0.4.2/pyproject.toml
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1385 2023-06-19 13:43:18.043939 trianglechain-0.4.2/setup.cfg
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-19 13:43:18.038831 trianglechain-0.4.2/src/
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-19 13:43:18.041632 trianglechain-0.4.2/src/trianglechain/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     8714 2023-05-04 11:29:54.000000 trianglechain-0.4.2/src/trianglechain/BaseChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13478 2023-05-04 11:29:54.000000 trianglechain-0.4.2/src/trianglechain/LineChain.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    28041 2023-06-19 13:40:12.000000 trianglechain-0.4.2/src/trianglechain/TriangleChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      319 2023-06-19 13:42:58.000000 trianglechain-0.4.2/src/trianglechain/__init__.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13417 2023-05-04 11:29:54.000000 trianglechain-0.4.2/src/trianglechain/bestfit.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     9932 2023-06-05 12:25:46.000000 trianglechain-0.4.2/src/trianglechain/density_estimation.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7853 2023-05-04 11:29:54.000000 trianglechain-0.4.2/src/trianglechain/limits.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    16854 2023-06-09 15:08:20.000000 trianglechain-0.4.2/src/trianglechain/make_subplots.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4349 2023-05-04 11:29:54.000000 trianglechain-0.4.2/src/trianglechain/params.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3024 2023-05-04 11:29:54.000000 trianglechain-0.4.2/src/trianglechain/utils_pj_hpd.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    19680 2023-06-05 12:25:46.000000 trianglechain-0.4.2/src/trianglechain/utils_plots.py
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-19 13:43:18.042646 trianglechain-0.4.2/src/trianglechain.egg-info/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-06-19 13:43:17.000000 trianglechain-0.4.2/src/trianglechain.egg-info/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      809 2023-06-19 13:43:18.000000 trianglechain-0.4.2/src/trianglechain.egg-info/SOURCES.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-06-19 13:43:17.000000 trianglechain-0.4.2/src/trianglechain.egg-info/dependency_links.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-05-11 08:24:36.000000 trianglechain-0.4.2/src/trianglechain.egg-info/not-zip-safe
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      308 2023-06-19 13:43:17.000000 trianglechain-0.4.2/src/trianglechain.egg-info/requires.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-06-19 13:43:17.000000 trianglechain-0.4.2/src/trianglechain.egg-info/top_level.txt
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-06-19 13:43:18.043415 trianglechain-0.4.2/tests/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      674 2023-05-04 11:29:54.000000 trianglechain-0.4.2/tests/test_bestfit.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2013 2023-05-04 11:29:54.000000 trianglechain-0.4.2/tests/test_limits.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      748 2023-05-04 11:29:54.000000 trianglechain-0.4.2/tests/test_linechain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2897 2023-05-04 11:29:54.000000 trianglechain-0.4.2/tests/test_params.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     4006 2023-05-04 11:29:54.000000 trianglechain-0.4.2/tests/test_trianglechain.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-07-12 12:14:31.481029 trianglechain-0.4.3/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-06-19 14:00:45.000000 trianglechain-0.4.3/AUTHORS.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2023-06-19 14:00:45.000000 trianglechain-0.4.3/CONTRIBUTING.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2034 2023-07-12 12:13:09.000000 trianglechain-0.4.3/HISTORY.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-06-19 14:00:45.000000 trianglechain-0.4.3/LICENSE
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-06-19 14:00:45.000000 trianglechain-0.4.3/MANIFEST.in
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-07-12 12:14:31.481109 trianglechain-0.4.3/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-06-19 14:00:45.000000 trianglechain-0.4.3/README.md
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-06-19 14:00:45.000000 trianglechain-0.4.3/pyproject.toml
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1387 2023-07-12 12:14:31.481487 trianglechain-0.4.3/setup.cfg
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-07-12 12:14:31.472698 trianglechain-0.4.3/src/
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-07-12 12:14:31.477847 trianglechain-0.4.3/src/trianglechain/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     8714 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/BaseChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13478 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/LineChain.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    28284 2023-07-12 12:05:01.000000 trianglechain-0.4.3/src/trianglechain/TriangleChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      319 2023-07-12 12:13:52.000000 trianglechain-0.4.3/src/trianglechain/__init__.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13417 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     9932 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/density_estimation.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7853 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    16854 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/make_subplots.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4386 2023-07-12 12:05:01.000000 trianglechain-0.4.3/src/trianglechain/params.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3024 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/utils_pj_hpd.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    19766 2023-07-12 12:05:01.000000 trianglechain-0.4.3/src/trianglechain/utils_plots.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-07-12 12:14:31.479443 trianglechain-0.4.3/src/trianglechain.egg-info/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-07-12 12:14:31.000000 trianglechain-0.4.3/src/trianglechain.egg-info/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      809 2023-07-12 12:14:31.000000 trianglechain-0.4.3/src/trianglechain.egg-info/SOURCES.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-07-12 12:14:31.000000 trianglechain-0.4.3/src/trianglechain.egg-info/dependency_links.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-06-19 14:01:00.000000 trianglechain-0.4.3/src/trianglechain.egg-info/not-zip-safe
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      310 2023-07-12 12:14:31.000000 trianglechain-0.4.3/src/trianglechain.egg-info/requires.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-07-12 12:14:31.000000 trianglechain-0.4.3/src/trianglechain.egg-info/top_level.txt
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-07-12 12:14:31.480821 trianglechain-0.4.3/tests/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      674 2023-06-19 14:00:45.000000 trianglechain-0.4.3/tests/test_bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2013 2023-06-19 14:00:45.000000 trianglechain-0.4.3/tests/test_limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      748 2023-06-19 14:00:45.000000 trianglechain-0.4.3/tests/test_linechain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2897 2023-06-19 14:00:45.000000 trianglechain-0.4.3/tests/test_params.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     4006 2023-06-19 14:00:45.000000 trianglechain-0.4.3/tests/test_trianglechain.py
```

### Comparing `trianglechain-0.4.2/CONTRIBUTING.rst` & `trianglechain-0.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/HISTORY.rst` & `trianglechain-0.4.3/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 .. :changelog:
 
 History
 -------
 
+0.4.3 (2023-07-01)
+++++++++++++++++++
+
+* FIX: grid is also plotted in the upper triangle if the plotting order is lower upper lower (and vice versa)
+* FIX: ranges of empty plots are correctly displayed
+* added warning for people like Arne that use the parameter names incorrectly.
+
 0.4.2 (2023-06-19)
 ++++++++++++++++++
 
 * FIX: scatter_kwargs for scatter_density
 
 0.4.1 (2023-06-09)
 ++++++++++++++++++
```

### Comparing `trianglechain-0.4.2/LICENSE` & `trianglechain-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/PKG-INFO` & `trianglechain-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.4.2
+Version: 0.4.3
 Summary: Code to plot multidimensional distributions
 Author: Silvan Fischbacher, Tomasz Kacprzak
 Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `trianglechain-0.4.2/README.md` & `trianglechain-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/pyproject.toml` & `trianglechain-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/setup.cfg` & `trianglechain-0.4.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 	flake8
 	black @ git+https://github.com/psf/black   # binary wheels are broken on some machines
 	isort
 	sphinx
 	sphinx-pynpoint-theme
 	myst-parser
 docs = 
-	sphinx
+	sphinx<7
 	sphinx-pynpoint-theme
 	myst-parser
 	nbsphinx
 	sphinx-copybutton
 	recommonmark
 
 [egg_info]
```

### Comparing `trianglechain-0.4.2/src/trianglechain/BaseChain.py` & `trianglechain-0.4.3/src/trianglechain/BaseChain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/src/trianglechain/LineChain.py` & `trianglechain-0.4.3/src/trianglechain/LineChain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/src/trianglechain/TriangleChain.py` & `trianglechain-0.4.3/src/trianglechain/TriangleChain.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,14 +309,20 @@
         if the 1D probability should be normalized, default: True
     :param normalize_prob2D: bool
         if the 2D probability should be normalized, default: True
     :param progress_bar: bool
         if a progress bar should be shown, default: True
     """
 
+    if (names is not None) and (not isinstance(data, np.ndarray)):
+        LOGGER.warning(
+            "The names argument is only used if data is a numpy array. "
+            "Probably you want to use the params argument instead."
+        )
+
     ###############################
     # prepare data and setup plot #
     ###############################
     data = ensure_rec(data, names=names)
     data, columns, empty_columns = prepare_columns(
         data,
         params=params,
```

### Comparing `trianglechain-0.4.2/src/trianglechain/bestfit.py` & `trianglechain-0.4.3/src/trianglechain/bestfit.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/src/trianglechain/density_estimation.py` & `trianglechain-0.4.3/src/trianglechain/density_estimation.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/src/trianglechain/limits.py` & `trianglechain-0.4.3/src/trianglechain/limits.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/src/trianglechain/make_subplots.py` & `trianglechain-0.4.3/src/trianglechain/make_subplots.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/src/trianglechain/params.py` & `trianglechain-0.4.3/src/trianglechain/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         >>> rec_df = ensure_rec(df)
         >>> print(rec_df)
         [(1, 3) (2, 4)]
     """
     if isinstance(data, pd.DataFrame):
         data = data.to_records(index=False)
 
-    if names is not None:
+    if (names is not None) and (isinstance(data, np.ndarray)):
         assert (
             len(names) == data.shape[1]
         ), "number of names does not match the number of parameters"
         data = at.arr2rec(data, names)
 
     if isinstance(data, dict):
         return at.dict2rec(data)
```

### Comparing `trianglechain-0.4.2/src/trianglechain/utils_pj_hpd.py` & `trianglechain-0.4.3/src/trianglechain/utils_pj_hpd.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/src/trianglechain/utils_plots.py` & `trianglechain-0.4.3/src/trianglechain/utils_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,17 +192,19 @@
 
 
 def check_orientation(ax):
     """
     Check the orientation of the axes of an previously created figure.
 
     :param ax: The axes.
-    :return: The orientation of the axes.
+    :return: The orientation of the axes, either "upper", "lower" or "both".
     """
     if ax[-1, 0].axison:
+        if ax[0, -1].axison:
+            return "both"
         return "lower"
     else:
         return "upper"
 
 
 def update_current_ranges(current_ranges, ranges, columns, data):
     """
@@ -539,15 +541,15 @@
     except Exception:
         xlims = current_ranges[col2]
     try:
         ylims = ranges[col1]
     except Exception:
         ylims = current_ranges[col1]
 
-        axc.set_xlim(xlims)
+    axc.set_xlim(xlims)
     if np.isfinite(ylims[0]):
         axc.set_ylim(ylims)
     axc.get_yaxis().set_major_formatter(FormatStrFormatter("%.3e"))
     axc.get_xaxis().set_major_formatter(FormatStrFormatter("%.3e"))
 
 
 def pixel_coords(x, ranges, n_pix_img):
```

### Comparing `trianglechain-0.4.2/src/trianglechain.egg-info/PKG-INFO` & `trianglechain-0.4.3/src/trianglechain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.4.2
+Version: 0.4.3
 Summary: Code to plot multidimensional distributions
 Author: Silvan Fischbacher, Tomasz Kacprzak
 Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `trianglechain-0.4.2/src/trianglechain.egg-info/SOURCES.txt` & `trianglechain-0.4.3/src/trianglechain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/tests/test_bestfit.py` & `trianglechain-0.4.3/tests/test_bestfit.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/tests/test_limits.py` & `trianglechain-0.4.3/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/tests/test_linechain.py` & `trianglechain-0.4.3/tests/test_linechain.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/tests/test_params.py` & `trianglechain-0.4.3/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.2/tests/test_trianglechain.py` & `trianglechain-0.4.3/tests/test_trianglechain.py`

 * *Files identical despite different names*


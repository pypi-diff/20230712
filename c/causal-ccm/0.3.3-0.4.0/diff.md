# Comparing `tmp/causal_ccm-0.3.3.tar.gz` & `tmp/causal_ccm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/causal_ccm-0.3.3.tar", last modified: Tue Jun  8 15:41:20 2021, max compression
+gzip compressed data, was "causal_ccm-0.4.0.tar", last modified: Wed Jul 12 07:56:47 2023, max compression
```

## Comparing `causal_ccm-0.3.3.tar` & `causal_ccm-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 prince.javier (1520356659) 1452017807        0 2021-06-08 15:41:20.000000 causal_ccm-0.3.3/
--rw-r--r--   0 prince.javier (1520356659) 1452017807     2561 2021-06-08 15:41:20.000000 causal_ccm-0.3.3/PKG-INFO
--rw-r--r--   0 prince.javier (1520356659) 1452017807     1401 2021-01-16 13:58:54.000000 causal_ccm-0.3.3/README.md
-drwxr-xr-x   0 prince.javier (1520356659) 1452017807        0 2021-06-08 15:41:20.000000 causal_ccm-0.3.3/causal_ccm/
--rw-r--r--   0 prince.javier (1520356659) 1452017807       38 2021-01-16 11:48:12.000000 causal_ccm-0.3.3/causal_ccm/__init__.py
--rw-r--r--   0 prince.javier (1520356659) 1452017807     9316 2021-06-05 15:20:45.000000 causal_ccm-0.3.3/causal_ccm/causal_ccm.py
-drwxr-xr-x   0 prince.javier (1520356659) 1452017807        0 2021-06-08 15:41:20.000000 causal_ccm-0.3.3/causal_ccm.egg-info/
--rw-r--r--   0 prince.javier (1520356659) 1452017807     2561 2021-06-08 15:41:20.000000 causal_ccm-0.3.3/causal_ccm.egg-info/PKG-INFO
--rw-r--r--   0 prince.javier (1520356659) 1452017807      245 2021-06-08 15:41:20.000000 causal_ccm-0.3.3/causal_ccm.egg-info/SOURCES.txt
--rw-r--r--   0 prince.javier (1520356659) 1452017807        1 2021-06-08 15:41:20.000000 causal_ccm-0.3.3/causal_ccm.egg-info/dependency_links.txt
--rw-r--r--   0 prince.javier (1520356659) 1452017807       38 2021-06-08 15:41:20.000000 causal_ccm-0.3.3/causal_ccm.egg-info/requires.txt
--rw-r--r--   0 prince.javier (1520356659) 1452017807       11 2021-06-08 15:41:20.000000 causal_ccm-0.3.3/causal_ccm.egg-info/top_level.txt
--rw-r--r--   0 prince.javier (1520356659) 1452017807       79 2021-06-08 15:41:20.000000 causal_ccm-0.3.3/setup.cfg
--rw-r--r--   0 prince.javier (1520356659) 1452017807     1919 2021-06-08 15:41:17.000000 causal_ccm-0.3.3/setup.py
+drwxr-xr-x   0 princejavier   (501) staff       (20)        0 2023-07-12 07:56:47.316302 causal_ccm-0.4.0/
+-rw-r--r--   0 princejavier   (501) staff       (20)     1063 2023-07-12 07:24:49.000000 causal_ccm-0.4.0/LICENSE
+-rw-r--r--   0 princejavier   (501) staff       (20)     2918 2023-07-12 07:56:47.316350 causal_ccm-0.4.0/PKG-INFO
+-rw-r--r--   0 princejavier   (501) staff       (20)     2063 2023-07-12 07:24:49.000000 causal_ccm-0.4.0/README.md
+drwxr-xr-x   0 princejavier   (501) staff       (20)        0 2023-07-12 07:56:47.315491 causal_ccm-0.4.0/causal_ccm/
+-rw-r--r--   0 princejavier   (501) staff       (20)       69 2023-07-12 07:24:49.000000 causal_ccm-0.4.0/causal_ccm/__init__.py
+-rw-r--r--   0 princejavier   (501) staff       (20)     9329 2023-07-12 07:24:49.000000 causal_ccm-0.4.0/causal_ccm/causal_ccm.py
+-rw-r--r--   0 princejavier   (501) staff       (20)     7240 2023-07-12 07:24:49.000000 causal_ccm-0.4.0/causal_ccm/pai.py
+drwxr-xr-x   0 princejavier   (501) staff       (20)        0 2023-07-12 07:56:47.316186 causal_ccm-0.4.0/causal_ccm.egg-info/
+-rw-r--r--   0 princejavier   (501) staff       (20)     2918 2023-07-12 07:56:47.000000 causal_ccm-0.4.0/causal_ccm.egg-info/PKG-INFO
+-rw-r--r--   0 princejavier   (501) staff       (20)      271 2023-07-12 07:56:47.000000 causal_ccm-0.4.0/causal_ccm.egg-info/SOURCES.txt
+-rw-r--r--   0 princejavier   (501) staff       (20)        1 2023-07-12 07:56:47.000000 causal_ccm-0.4.0/causal_ccm.egg-info/dependency_links.txt
+-rw-r--r--   0 princejavier   (501) staff       (20)       51 2023-07-12 07:56:47.000000 causal_ccm-0.4.0/causal_ccm.egg-info/requires.txt
+-rw-r--r--   0 princejavier   (501) staff       (20)       11 2023-07-12 07:56:47.000000 causal_ccm-0.4.0/causal_ccm.egg-info/top_level.txt
+-rw-r--r--   0 princejavier   (501) staff       (20)       79 2023-07-12 07:56:47.316518 causal_ccm-0.4.0/setup.cfg
+-rw-r--r--   0 princejavier   (501) staff       (20)     1894 2023-07-12 07:56:14.000000 causal_ccm-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `causal_ccm-0.3.3/PKG-INFO` & `causal_ccm-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,70 @@
 Metadata-Version: 2.1
 Name: causal_ccm
-Version: 0.3.3
+Version: 0.4.0
 Summary: implementation of convergent cross mapping by Sugihara et al (2012)
 Home-page: https://github.com/PrinceJavier/causal_ccm
+Download-URL: https://github.com/PrinceJavier/causal_ccm/archive/refs/tags/v_040.tar.gz
 Author: Prince Javier
 Author-email: othepjavier@gmail.com
 License: MIT
-Download-URL: https://github.com/PrinceJavier/causal_ccm/archive/refs/tags/v_033.tar.gz
-Description: # causal_ccm
-        Package implementing Convergent Cross Mapping for causality inference in dynamical systems as defined by [Sugihara et al (2012)](https://science.sciencemag.org/content/338/6106/496)
-        
-        ### Example usage
-        For an example how to use, see: https://github.com/PrinceJavier/causal_ccm/blob/main/usage_sample.ipynb 
-        <br>Source code: https://github.com/PrinceJavier/causal_ccm
-        
-        ### To install
-        `pip install causal-ccm`
-        
-        ### To use
-        Say we want to check if X drives Y. We first define `ccm` using:
-        * `X` and `Y` - time series data
-        * `tau` - time lag (if `tau=1` we get `[t, t-1, t-2...]` as our shadow manifold embedding
-        * `E` - embedding dimension (default=2) for the shadow manifold
-        * `L` - time horizon to consider, defaults at length of time series X
-        
-        We import the package
-        <br>`from causal_ccm.causal_ccm import ccm`
-        
-        We define `ccm`:
-        <br>`ccm1 = ccm(X, Y, tau, E, L) # define ccm with X, Y time series `
-        
-        We check the strength of causality measured as correlation in prediction vs true (see Sugihara (2012))
-        <br>`ccm1.causality()`
-        
-        We can visualize cross mapping between manifolds of X and Y
-        <br>`ccm1.visualize_cross_mapping()`
-        
-        We visualize correlation of X->Y
-        <br>We stronger correlation = stronger causal relationship
-        <br>`ccm1.plot_ccm_correls()`
-        
-        Finally, we can check convergence in predictions (correlations) by computing `ccm1.causality()` for `ccm1` defined with different L values.
-        
-        
-        
-        
 Keywords: causality,dynamical systems,complex systems
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# causal_ccm
+Package implementing Convergent Cross Mapping for causality inference in dynamical systems as defined by [Sugihara et al (2012)](https://science.sciencemag.org/content/338/6106/496)
+
+### Example usage
+For an example how to use, see: https://github.com/PrinceJavier/causal_ccm/blob/main/usage_sample.ipynb 
+<br>Source code: https://github.com/PrinceJavier/causal_ccm
+
+### To install
+`pip install causal-ccm`
+
+### To use
+Say we want to check if X drives Y. We first define `ccm` using:
+* `X` and `Y` - time series data
+* `tau` - time lag (if `tau=1` we get `[t, t-1, t-2...]` as our shadow manifold embedding
+* `E` - embedding dimension (default=2) for the shadow manifold
+* `L` - time horizon to consider, defaults at length of time series X
+
+We import the package
+<br>`from causal_ccm.causal_ccm import ccm`
+
+We define `ccm`:
+<br>`ccm1 = ccm(X, Y, tau, E, L) # define ccm with X, Y time series `
+
+We check the strength of causality measured as correlation in prediction vs true (see Sugihara (2012))
+<br>`ccm1.causality()`
+
+We can visualize cross mapping between manifolds of X and Y
+<br>`ccm1.visualize_cross_mapping()`
+
+We visualize correlation of X->Y
+<br>We stronger correlation = stronger causal relationship
+<br>`ccm1.plot_ccm_correls()`
+
+Finally, we can check convergence in predictions (correlations) by computing `ccm1.causality()` for `ccm1` defined with different L values.
+
+### Additional Feature (PAI)
+
+The pai class implements the Pairwise Asymmetric Inference (see McCracken (2014)). The major difference of pai to ccm is the shadow manifold used to predict `X`. To create the manifold, use the `manifold_pattern` and `tau` parameters. For example, `manifold_pattern=[[0, -1, -2],[0]], tau=2` is the same as the shadow manifold `(X_t, X_{t-1*2}, X_{t-2*2}, Y_t)`.
+
+If this package helped you in your work, pls. cite:
+```
+@software{Javier_causal-ccm_a_Python_2021,
+author = {Javier, Prince Joseph Erneszer},
+month = {6},
+title = {{causal-ccm a Python implementation of Convergent Cross Mapping}},
+version = {0.3.3},
+year = {2021}
+}
+```
```

### Comparing `causal_ccm-0.3.3/README.md` & `causal_ccm-0.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -29,9 +29,21 @@
 
 We visualize correlation of X->Y
 <br>We stronger correlation = stronger causal relationship
 <br>`ccm1.plot_ccm_correls()`
 
 Finally, we can check convergence in predictions (correlations) by computing `ccm1.causality()` for `ccm1` defined with different L values.
 
+### Additional Feature (PAI)
 
+The pai class implements the Pairwise Asymmetric Inference (see McCracken (2014)). The major difference of pai to ccm is the shadow manifold used to predict `X`. To create the manifold, use the `manifold_pattern` and `tau` parameters. For example, `manifold_pattern=[[0, -1, -2],[0]], tau=2` is the same as the shadow manifold `(X_t, X_{t-1*2}, X_{t-2*2}, Y_t)`.
 
+If this package helped you in your work, pls. cite:
+```
+@software{Javier_causal-ccm_a_Python_2021,
+author = {Javier, Prince Joseph Erneszer},
+month = {6},
+title = {{causal-ccm a Python implementation of Convergent Cross Mapping}},
+version = {0.3.3},
+year = {2021}
+}
+```
```

### Comparing `causal_ccm-0.3.3/causal_ccm/causal_ccm.py` & `causal_ccm-0.4.0/causal_ccm/causal_ccm.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
             tau: time lag
             E: shadow manifold embedding dimension
             L: time duration
         Returns
             None. Just correlation plots between predicted X|M_y and true X
         """
         X_My_true, X_My_pred = [], []
-        for t in range(self.tau, self.L):
+        for t in range((self.E-1) * self.tau, self.L):
             true, pred = self.predict(t)
             X_My_true.append(true)
             X_My_pred.append(pred)
 
         # predicting X from My
         r, p = np.round(pearsonr(X_My_true, X_My_pred), 4)
```

### Comparing `causal_ccm-0.3.3/causal_ccm.egg-info/PKG-INFO` & `causal_ccm-0.4.0/causal_ccm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,70 @@
 Metadata-Version: 2.1
 Name: causal-ccm
-Version: 0.3.3
+Version: 0.4.0
 Summary: implementation of convergent cross mapping by Sugihara et al (2012)
 Home-page: https://github.com/PrinceJavier/causal_ccm
+Download-URL: https://github.com/PrinceJavier/causal_ccm/archive/refs/tags/v_040.tar.gz
 Author: Prince Javier
 Author-email: othepjavier@gmail.com
 License: MIT
-Download-URL: https://github.com/PrinceJavier/causal_ccm/archive/refs/tags/v_033.tar.gz
-Description: # causal_ccm
-        Package implementing Convergent Cross Mapping for causality inference in dynamical systems as defined by [Sugihara et al (2012)](https://science.sciencemag.org/content/338/6106/496)
-        
-        ### Example usage
-        For an example how to use, see: https://github.com/PrinceJavier/causal_ccm/blob/main/usage_sample.ipynb 
-        <br>Source code: https://github.com/PrinceJavier/causal_ccm
-        
-        ### To install
-        `pip install causal-ccm`
-        
-        ### To use
-        Say we want to check if X drives Y. We first define `ccm` using:
-        * `X` and `Y` - time series data
-        * `tau` - time lag (if `tau=1` we get `[t, t-1, t-2...]` as our shadow manifold embedding
-        * `E` - embedding dimension (default=2) for the shadow manifold
-        * `L` - time horizon to consider, defaults at length of time series X
-        
-        We import the package
-        <br>`from causal_ccm.causal_ccm import ccm`
-        
-        We define `ccm`:
-        <br>`ccm1 = ccm(X, Y, tau, E, L) # define ccm with X, Y time series `
-        
-        We check the strength of causality measured as correlation in prediction vs true (see Sugihara (2012))
-        <br>`ccm1.causality()`
-        
-        We can visualize cross mapping between manifolds of X and Y
-        <br>`ccm1.visualize_cross_mapping()`
-        
-        We visualize correlation of X->Y
-        <br>We stronger correlation = stronger causal relationship
-        <br>`ccm1.plot_ccm_correls()`
-        
-        Finally, we can check convergence in predictions (correlations) by computing `ccm1.causality()` for `ccm1` defined with different L values.
-        
-        
-        
-        
 Keywords: causality,dynamical systems,complex systems
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# causal_ccm
+Package implementing Convergent Cross Mapping for causality inference in dynamical systems as defined by [Sugihara et al (2012)](https://science.sciencemag.org/content/338/6106/496)
+
+### Example usage
+For an example how to use, see: https://github.com/PrinceJavier/causal_ccm/blob/main/usage_sample.ipynb 
+<br>Source code: https://github.com/PrinceJavier/causal_ccm
+
+### To install
+`pip install causal-ccm`
+
+### To use
+Say we want to check if X drives Y. We first define `ccm` using:
+* `X` and `Y` - time series data
+* `tau` - time lag (if `tau=1` we get `[t, t-1, t-2...]` as our shadow manifold embedding
+* `E` - embedding dimension (default=2) for the shadow manifold
+* `L` - time horizon to consider, defaults at length of time series X
+
+We import the package
+<br>`from causal_ccm.causal_ccm import ccm`
+
+We define `ccm`:
+<br>`ccm1 = ccm(X, Y, tau, E, L) # define ccm with X, Y time series `
+
+We check the strength of causality measured as correlation in prediction vs true (see Sugihara (2012))
+<br>`ccm1.causality()`
+
+We can visualize cross mapping between manifolds of X and Y
+<br>`ccm1.visualize_cross_mapping()`
+
+We visualize correlation of X->Y
+<br>We stronger correlation = stronger causal relationship
+<br>`ccm1.plot_ccm_correls()`
+
+Finally, we can check convergence in predictions (correlations) by computing `ccm1.causality()` for `ccm1` defined with different L values.
+
+### Additional Feature (PAI)
+
+The pai class implements the Pairwise Asymmetric Inference (see McCracken (2014)). The major difference of pai to ccm is the shadow manifold used to predict `X`. To create the manifold, use the `manifold_pattern` and `tau` parameters. For example, `manifold_pattern=[[0, -1, -2],[0]], tau=2` is the same as the shadow manifold `(X_t, X_{t-1*2}, X_{t-2*2}, Y_t)`.
+
+If this package helped you in your work, pls. cite:
+```
+@software{Javier_causal-ccm_a_Python_2021,
+author = {Javier, Prince Joseph Erneszer},
+month = {6},
+title = {{causal-ccm a Python implementation of Convergent Cross Mapping}},
+version = {0.3.3},
+year = {2021}
+}
+```
```

### Comparing `causal_ccm-0.3.3/setup.py` & `causal_ccm-0.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,30 +4,31 @@
     long_description = f.read()
     
 print(long_description)
     
 setup(
   name = 'causal_ccm',         # How you named your package folder (MyLib)
   packages = ['causal_ccm'],   # Chose the same as "name"
-  version = '0.3.3',      # updated the docstrings where X and Y were switched
+  version = '0.4.0',      # add new feature: PAI method
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'implementation of convergent cross mapping by Sugihara et al (2012)',
   long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Prince Javier',                   # Type in your name
   author_email = 'othepjavier@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/PrinceJavier/causal_ccm',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/PrinceJavier/causal_ccm/archive/refs/tags/v_033.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/PrinceJavier/causal_ccm/archive/refs/tags/v_040.tar.gz',
   keywords = ['causality', 'dynamical systems', 'complex systems'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'pandas',
           'matplotlib',
           'seaborn',
-          'scipy'
+          'scipy',
+          'scikit-learn',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
```


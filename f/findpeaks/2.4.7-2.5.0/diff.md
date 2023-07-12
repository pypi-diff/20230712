# Comparing `tmp/findpeaks-2.4.7.tar.gz` & `tmp/findpeaks-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findpeaks-2.4.7.tar", last modified: Sat May 20 18:40:20 2023, max compression
+gzip compressed data, was "findpeaks-2.5.0.tar", last modified: Wed Jul 12 20:07:10 2023, max compression
```

## Comparing `findpeaks-2.4.7.tar` & `findpeaks-2.5.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 18:40:20.099969 findpeaks-2.4.7/
--rw-rw-rw-   0        0        0     1122 2021-01-28 13:20:53.000000 findpeaks-2.4.7/LICENSE
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0     8724 2023-05-20 18:40:20.082904 findpeaks-2.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     8149 2023-02-18 16:10:18.000000 findpeaks-2.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 18:40:19.946205 findpeaks-2.4.7/findpeaks/
--rw-rw-rw-   0        0        0     2199 2023-05-20 18:24:20.000000 findpeaks-2.4.7/findpeaks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 18:40:20.007900 findpeaks-2.4.7/findpeaks/data/
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.4.7/findpeaks/data/__init__.py
--rw-rw-rw-   0        0        0    18962 2023-05-20 18:02:04.000000 findpeaks-2.4.7/findpeaks/examples.py
-drwxrwxrwx   0        0        0        0 2023-05-20 18:40:20.062249 findpeaks-2.4.7/findpeaks/filters/
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.4.7/findpeaks/filters/__init__.py
--rw-rw-rw-   0        0        0     5665 2021-12-05 14:23:41.000000 findpeaks-2.4.7/findpeaks/filters/frost.py
--rw-rw-rw-   0        0        0     4133 2021-12-05 14:23:35.000000 findpeaks-2.4.7/findpeaks/filters/kuan.py
--rw-rw-rw-   0        0        0     6429 2021-12-05 14:24:04.000000 findpeaks-2.4.7/findpeaks/filters/lee.py
--rw-rw-rw-   0        0        0     5248 2021-12-05 14:25:22.000000 findpeaks-2.4.7/findpeaks/filters/lee_enhanced.py
--rw-rw-rw-   0        0        0     3921 2021-12-05 14:27:45.000000 findpeaks-2.4.7/findpeaks/filters/mean.py
--rw-rw-rw-   0        0        0     3180 2021-12-05 14:30:08.000000 findpeaks-2.4.7/findpeaks/filters/median.py
--rw-rw-rw-   0        0        0    52243 2023-05-20 18:08:01.000000 findpeaks-2.4.7/findpeaks/findpeaks.py
--rw-rw-rw-   0        0        0     5995 2021-12-05 12:54:20.000000 findpeaks-2.4.7/findpeaks/interpolate.py
--rw-rw-rw-   0        0        0    23022 2023-02-24 22:51:49.000000 findpeaks-2.4.7/findpeaks/stats.py
-drwxrwxrwx   0        0        0        0 2023-05-20 18:40:20.081913 findpeaks-2.4.7/findpeaks/tests/
--rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.4.7/findpeaks/tests/__init__.py
--rw-rw-rw-   0        0        0     9124 2023-05-20 18:26:50.000000 findpeaks-2.4.7/findpeaks/tests/test_findpeaks.py
--rw-rw-rw-   0        0        0     2469 2021-01-28 13:20:53.000000 findpeaks-2.4.7/findpeaks/union_find.py
-drwxrwxrwx   0        0        0        0 2023-05-20 18:40:19.989403 findpeaks-2.4.7/findpeaks.egg-info/
--rw-rw-rw-   0        0        0     8724 2023-05-20 18:40:19.000000 findpeaks-2.4.7/findpeaks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-05-20 18:40:19.000000 findpeaks-2.4.7/findpeaks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 18:40:19.000000 findpeaks-2.4.7/findpeaks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-05-20 18:40:19.000000 findpeaks-2.4.7/findpeaks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-20 18:40:19.000000 findpeaks-2.4.7/findpeaks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 18:40:20.100972 findpeaks-2.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1467 2023-05-20 18:39:58.000000 findpeaks-2.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 20:07:10.346871 findpeaks-2.5.0/
+-rw-rw-rw-   0        0        0     1122 2021-01-28 13:20:53.000000 findpeaks-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8724 2023-07-12 20:07:10.344886 findpeaks-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8149 2023-02-18 16:10:18.000000 findpeaks-2.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 20:07:10.259363 findpeaks-2.5.0/findpeaks/
+-rw-rw-rw-   0        0        0     2232 2023-07-12 20:00:25.000000 findpeaks-2.5.0/findpeaks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 20:07:10.315778 findpeaks-2.5.0/findpeaks/data/
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.5.0/findpeaks/data/__init__.py
+-rw-rw-rw-   0        0        0    20069 2023-07-12 18:43:54.000000 findpeaks-2.5.0/findpeaks/examples.py
+drwxrwxrwx   0        0        0        0 2023-07-12 20:07:10.335315 findpeaks-2.5.0/findpeaks/filters/
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.5.0/findpeaks/filters/__init__.py
+-rw-rw-rw-   0        0        0     5665 2021-12-05 14:23:41.000000 findpeaks-2.5.0/findpeaks/filters/frost.py
+-rw-rw-rw-   0        0        0     4133 2021-12-05 14:23:35.000000 findpeaks-2.5.0/findpeaks/filters/kuan.py
+-rw-rw-rw-   0        0        0     6429 2021-12-05 14:24:04.000000 findpeaks-2.5.0/findpeaks/filters/lee.py
+-rw-rw-rw-   0        0        0     5248 2021-12-05 14:25:22.000000 findpeaks-2.5.0/findpeaks/filters/lee_enhanced.py
+-rw-rw-rw-   0        0        0    12835 2023-07-12 18:57:51.000000 findpeaks-2.5.0/findpeaks/filters/lee_sigma.py
+-rw-rw-rw-   0        0        0     3921 2021-12-05 14:27:45.000000 findpeaks-2.5.0/findpeaks/filters/mean.py
+-rw-rw-rw-   0        0        0     3180 2021-12-05 14:30:08.000000 findpeaks-2.5.0/findpeaks/filters/median.py
+-rw-rw-rw-   0        0        0    54480 2023-07-12 19:49:33.000000 findpeaks-2.5.0/findpeaks/findpeaks.py
+-rw-rw-rw-   0        0        0     5995 2021-12-05 12:54:20.000000 findpeaks-2.5.0/findpeaks/interpolate.py
+-rw-rw-rw-   0        0        0    23627 2023-07-12 18:58:17.000000 findpeaks-2.5.0/findpeaks/stats.py
+drwxrwxrwx   0        0        0        0 2023-07-12 20:07:10.342878 findpeaks-2.5.0/findpeaks/tests/
+-rw-rw-rw-   0        0        0        0 2021-01-28 13:20:53.000000 findpeaks-2.5.0/findpeaks/tests/__init__.py
+-rw-rw-rw-   0        0        0     9288 2023-07-12 18:44:51.000000 findpeaks-2.5.0/findpeaks/tests/test_findpeaks.py
+-rw-rw-rw-   0        0        0     2469 2021-01-28 13:20:53.000000 findpeaks-2.5.0/findpeaks/union_find.py
+drwxrwxrwx   0        0        0        0 2023-07-12 20:07:10.314142 findpeaks-2.5.0/findpeaks.egg-info/
+-rw-rw-rw-   0        0        0     8724 2023-07-12 20:07:10.000000 findpeaks-2.5.0/findpeaks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2023-07-12 20:07:10.000000 findpeaks-2.5.0/findpeaks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 20:07:10.000000 findpeaks-2.5.0/findpeaks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-07-12 20:07:10.000000 findpeaks-2.5.0/findpeaks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 20:07:10.000000 findpeaks-2.5.0/findpeaks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 20:07:10.346987 findpeaks-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1676 2023-07-12 15:59:47.000000 findpeaks-2.5.0/setup.py
```

### Comparing `findpeaks-2.4.7/LICENSE` & `findpeaks-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.7/PKG-INFO` & `findpeaks-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: findpeaks
-Version: 2.4.7
+Version: 2.5.0
 Summary: findpeaks is for the detection of peaks and valleys in a 1D vector and 2D array (image).
 Home-page: https://erdogant.github.io/findpeaks
-Download-URL: https://github.com/erdogant/findpeaks/archive/2.4.7.tar.gz
+Download-URL: https://github.com/erdogant/findpeaks/archive/2.5.0.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: findpeaks Version: 2.4.7 Summary: findpeaks is for
+Metadata-Version: 2.1 Name: findpeaks Version: 2.5.0 Summary: findpeaks is for
 the detection of peaks and valleys in a 1D vector and 2D array (image). Home-
 page: https://erdogant.github.io/findpeaks Download-URL: https://github.com/
-erdogant/findpeaks/archive/2.4.7.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant/findpeaks/archive/2.5.0.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE # findpeaks [![Python](https://img.shields.io/pypi/
 pyversions/findpeaks)](https://img.shields.io/pypi/pyversions/findpeaks) [!
 [Pypi](https://img.shields.io/pypi/v/findpeaks)](https://pypi.org/project/
 findpeaks/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
```

### Comparing `findpeaks-2.4.7/README.md` & `findpeaks-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.7/findpeaks/__init__.py` & `findpeaks-2.5.0/findpeaks/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,32 +5,31 @@
     stats,
     interpolate,
     )
 
 # Import the denosing filters
 from findpeaks.filters.lee import lee_filter
 from findpeaks.filters.lee_enhanced import lee_enhanced_filter
+from findpeaks.filters.lee_sigma import lee_sigma_filter
 from findpeaks.filters.kuan import kuan_filter
 from findpeaks.filters.frost import frost_filter
 from findpeaks.filters.median import median_filter
 from findpeaks.filters.mean import mean_filter
 
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.4.7'
+__version__ = '2.5.0'
 
 # module level doc-string
 __doc__ = """
 findpeaks
 =====================================================================
 
-Description
------------
 findpeaks is for the detection and vizualization of peaks and valleys in a 1D-vector and 2D-array.
 In case of 2D-array, the image can be pre-processed by resizing, scaling, and denoising.
 Peaks are detected using the masking and the topology method.
 The results can be plotted for the preprocessing steps, the persistence of peaks, the final masking plot and a 3d-mesh plot.
 
 Examples
 --------
@@ -45,15 +44,15 @@
 >>> fp = findpeaks(method='topology')
 >>> X = fp.import_example('2dpeaks')
 >>> results = fp.fit(X)
 >>> fp.plot()
 >>>
 >>> # Image example
 >>> from findpeaks import findpeaks
->>> fp = findpeaks(method='topology', denoise='fastnl', window=30, imsize=(300,300))
+>>> fp = findpeaks(method='topology', denoise='fastnl', window=30, imsize=(300, 300))
 >>> X = fp.import_example('2dpeaks_image')
 >>> results = fp.fit(X)
 >>> fp.plot()
 >>>
 >>> # Plot each seperately
 >>> fp.plot_preprocessing()
 >>> fp.plot_persistence()
```

### Comparing `findpeaks-2.4.7/findpeaks/examples.py` & `findpeaks-2.5.0/findpeaks/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,47 @@
 # print(dir(findpeaks))
 # print(findpeaks.__version__)
 
 # pip install opencv-python
 # import matplotlib.pyplot as plt
 # from findpeaks import findpeaks
 
+# %% New functionality:
+import findpeaks
+import matplotlib.pyplot as plt
+img = findpeaks.import_example('2dpeaks_image')
+# Resize
+img = findpeaks.stats.resize(img, size=(300,300))
+# Make grey image
+img = findpeaks.stats.togray(img)
+# Scale between [0-255]
+img = findpeaks.stats.scale(img)
+# Filter
+img_filtered = findpeaks.stats.lee_sigma_filter(img.copy(), win_size=7)
+
+plt.figure()
+fig, axs = plt.subplots(1,2)
+axs[0].imshow(img, cmap='gray'); axs[0].set_title('Input')
+axs[1].imshow(img_filtered, cmap='gray'); axs[1].set_title('Lee sigma filter')
+
+
+import findpeaks
+img = findpeaks.import_example('2dpeaks_image')
+
+from findpeaks import findpeaks
+fp = findpeaks(method='topology', scale=True, denoise='lee_sigma', togray=True, params={'window': 31})
+results = fp.fit(img)
+fp.plot_persistence()
+fp.plot()
+
+
 # %% Issue 18:
 from findpeaks import findpeaks
 
-fp = findpeaks(method='topology', scale=False, denoise=None, togray=False, imsize=False, window=15)
+fp = findpeaks(method='topology', scale=False, denoise=None, togray=False, imsize=False, params={'window': 15})
 X = fp.import_example('2dpeaks')
 fp.fit(X)
 # fp.plot_mesh(wireframe=False, title='Test', cmap='RdBu', view=(70,5))
 fp.plot_mesh()
 fp.plot_mesh(xlim=[10, 30], ylim=[4, 10])
 fp.plot_mesh(xlim=[10, None], ylim=[4, 10])
 fp.plot_mesh(xlim=[10, None], ylim=[4, None])
@@ -24,16 +53,16 @@
 fp.plot_mesh(xlim=[10, 30], ylim=[4, 10], zlim=[0, None])
 fp.plot_mesh(xlim=[10, 30], ylim=[4, 10], zlim=[None, 6])
 fp.plot_mesh(xlim=[10, 30], ylim=[4, 10], zlim=[2, 6])
 
 # %%
 from findpeaks import findpeaks
 path = r'https://user-images.githubusercontent.com/44827483/221152897-133839bb-7364-492a-921b-c9077ab9930b.png'
-fp = findpeaks(method='topology', denoise='lee_enhanced', window=5, whitelist='peak')
-
+fp = findpeaks(method='topology', denoise='lee_enhanced', params={'window':5}, whitelist='peak')
+fp = findpeaks(method='topology', denoise='lee_sigma', params={'window':5}, whitelist='peak')
 X = fp.imread(path)
 results = fp.fit(X)
 fp.plot_persistence()
 fp.plot()
 # fp.plot_mesh()
 
 fp.results['persistence'].iloc[0:10,:]
@@ -100,22 +129,23 @@
 
 # %% issue #12
 # https://github.com/erdogant/findpeaks/issues/12
 import numpy as np
 
 X = np.sin(np.linspace(0, 1, 100))
 from findpeaks import findpeaks
-fp = findpeaks(method='caerus', params_caerus={'minperc': 5, 'window': 50})
+# fp = findpeaks(method='caerus', params_caerus={'minperc': 5, 'window': 50})
+fp = findpeaks(method='caerus', params={'minperc': 5, 'window': 50})
 results = fp.fit(X)
 
 
 # %% Issue 13
 # https://github.com/erdogant/findpeaks/issues/13
 from findpeaks import findpeaks
-fp = findpeaks(method="mask", denoise=None, window=3, limit=None, verbose=0)
+fp = findpeaks(method="mask", denoise=None, params={'window': 3}, limit=None, verbose=0)
 X = fp.import_example("2dpeaks_image")
 results = fp.fit(X)
 fp.plot()
 
 
 # %%
 # Load library
@@ -210,15 +240,15 @@
 fp.plot_persistence(fontsize_ax1=4)
 
 fp = findpeaks(method="peakdetect", lookahead=15, verbose=verbose)
 # Make fit
 results = fp.fit(X)
 fp.plot()
 
-fp = findpeaks(method="caerus", params_caerus={'minperc':100}, interpolate=None, verbose=verbose)
+fp = findpeaks(method="caerus", params={'minperc':100}, interpolate=None, verbose=verbose)
 # Make fit
 results = fp.fit(X)
 ax = fp.plot()
 
 
 # %%
 from findpeaks import findpeaks
@@ -254,36 +284,36 @@
 
 # %%
 # Import library
 from findpeaks import findpeaks
 # Import image example
 img = fp.import_example('2dpeaks_image')
 # Initializatie
-fp = findpeaks(scale=True, denoise='fastnl', window=31, togray=True, imsize=(300,300), whitelist=['peak', 'valley'], verbose=3)
+fp = findpeaks(scale=True, denoise='fastnl', params={'window': 31}, togray=True, imsize=(300,300), whitelist=['peak', 'valley'], verbose=3)
 # Fit
 fp.fit(img)
 fp.plot()
 fp.results["persistence"]
 
 # Take the minimum score for the top peaks off the diagonal.
 limit = fp.results['persistence'][0:5]['score'].min()
-fp = findpeaks(scale=True, denoise='fastnl', window=31, togray=True, imsize=(300,300), limit=254, whitelist=['peak', 'valley'], verbose=3)
+fp = findpeaks(scale=True, denoise='fastnl', params={'window': 31}, togray=True, imsize=(300,300), limit=254, whitelist=['peak', 'valley'], verbose=3)
 fp.fit(img)
 
 fp.results["persistence"]
 fp.plot(text=True)
 
 # Plot
 fp.plot_mesh()
 # Rotate to make a top view
 fp.plot_mesh(view=(90,0))
 
 # %%
 from findpeaks import findpeaks
-fp = findpeaks(method="topology", denoise=None, window=3, limit=None, verbose=0)
+fp = findpeaks(method="topology", denoise=None, params={'window': 3}, limit=None, verbose=0)
 X = fp.import_example("2dpeaks_image")
 # X = fp.import_example("2dpeaks")
 results = fp.fit(X)
 
 fp.plot_persistence()
 
 results["persistence"]
@@ -337,25 +367,25 @@
 filters = ['fastnl','bilateral','frost','median','mean', None]
 windows = [3, 9, 15, 31, 63]
 cus = [0.25, 0.5, 0.75]
 verbose=3
 
 for getfilter in filters:
     for window in windows:
-            fp = findpeaks(method='topology', scale=True, denoise=getfilter, window=window, togray=True, imsize=(300,300), verbose=verbose)
+            fp = findpeaks(method='topology', scale=True, denoise=getfilter, params={'window': window}, togray=True, imsize=(300,300), verbose=verbose)
             img = fp.import_example('2dpeaks_image')
             results = fp.fit(img)
             title = 'Method=' + str(getfilter) + ', window='+str(window)
             _, ax1 = fp.plot_mesh(wireframe=False, title=title, savepath=savepath+title+'.png')
 
 filters = ['lee','lee_enhanced','kuan']
 for getfilter in filters:
     for window in windows:
         for cu in cus:
-            fp = findpeaks(method='topology', scale=True, denoise=getfilter, window=window, cu=cu, togray=True, imsize=(300,300), verbose=verbose)
+            fp = findpeaks(method='topology', scale=True, denoise=getfilter, params={'window': window, 'cu': cu}, togray=True, imsize=(300,300), verbose=verbose)
             img = fp.import_example('2dpeaks_image')
             results = fp.fit(img)
             title = 'Method=' + str(getfilter) + ', window='+str(window) + ', cu='+str(cu)
             _, ax1 = fp.plot_mesh(wireframe=False, title=title, savepath=savepath+title+'.png')
 
 
 #%% Plot each seperately
@@ -416,15 +446,15 @@
 fp = findpeaks(method='mask', verbose=3)
 img = fp.import_example()
 fp.fit(img)
 fp.plot()
 
 
 # 2dpeaks example with other settings
-fp = findpeaks(method='topology', scale=True, denoise='fastnl', window=31, togray=True, imsize=(300,300), verbose=3)
+fp = findpeaks(method='topology', scale=True, denoise='fastnl', params={'window': 31}, togray=True, imsize=(300,300), verbose=3)
 img = fp.import_example('2dpeaks')
 fp.fit(img)
 fp.plot()
 
 # %%
 from findpeaks import findpeaks
 fp = findpeaks(method='topology')
```

### Comparing `findpeaks-2.4.7/findpeaks/filters/frost.py` & `findpeaks-2.5.0/findpeaks/filters/frost.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.7/findpeaks/filters/kuan.py` & `findpeaks-2.5.0/findpeaks/filters/kuan.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.7/findpeaks/filters/lee.py` & `findpeaks-2.5.0/findpeaks/filters/lee.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.7/findpeaks/filters/lee_enhanced.py` & `findpeaks-2.5.0/findpeaks/filters/lee_enhanced.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.7/findpeaks/filters/mean.py` & `findpeaks-2.5.0/findpeaks/filters/mean.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.7/findpeaks/filters/median.py` & `findpeaks-2.5.0/findpeaks/filters/median.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.7/findpeaks/findpeaks.py` & `findpeaks-2.5.0/findpeaks/findpeaks.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     >>> from findpeaks import findpeaks
     >>> X = fp.import_example('2dpeaks')
     >>> results = fp.fit(X)
     >>> fp.plot()
     >>>
     >>> # Image example
     >>> from findpeaks import findpeaks
-    >>> fp = findpeaks(method='topology', denoise='fastnl', window=30, imsize=(300,300))
+    >>> fp = findpeaks(method='topology', denoise='fastnl', params={'window': 30}, imsize=(300,300))
     >>> X = fp.import_example('2dpeaks_image')
     >>> results = fp.fit(X)
     >>> fp.plot()
     >>>
     >>> # Plot each seperately
     >>> fp.plot_preprocessing()
     >>> fp.plot_persistence()
@@ -67,15 +67,30 @@
 
     References
     ----------
         * https://erdogant.github.io/findpeaks/
 
     """
 
-    def __init__(self, method=None, whitelist=['peak', 'valley'], lookahead=200, interpolate=None, limit=None, imsize=None, scale=True, togray=True, denoise='fastnl', window=3, cu=0.25, params_caerus={'window': 50, 'minperc': 3, 'nlargest': 10, 'threshold': 0.25}, figsize=(15, 8), verbose=3):
+    def __init__(self,
+                 method=None,
+                 whitelist=['peak', 'valley'],
+                 lookahead=200,
+                 interpolate=None,
+                 limit=None,
+                 imsize=None,
+                 scale=True,
+                 togray=True,
+                 denoise='fastnl',
+                 window=None,  # DEPRECATED IN LATER VERSIONS: specify in params
+                 cu=None,  # DEPRECATED IN LATER VERSIONS: specify in params
+                 params_caerus={},  # DEPRECATED IN LATER VERSIONS: use params instead
+                 params={'window': 3, 'cu': 0.25},
+                 figsize=(15, 8),
+                 verbose=3):
         """Initialize findpeaks parameters.
 
         Parameters
         ----------
         X : array-like (1d-vector or 2d-image)
             Input image data.
         method : String, (default : None).
@@ -95,45 +110,48 @@
         lookahead : int, (default : 200)
             Looking ahead for peaks. For very small 1d arrays (such as up to 50 datapoints), use low numbers such as 1 or 2.
         interpolate : int, (default : None)
             Interpolation factor. The higher the number, the less sharp the edges will be.
         limit : float, (default : None)
             In case method='topology'
             Values > limit are active search areas to detect regions of interest (ROI).
+        imsize : tuple, (default : None)
+            resize to (width,length).
         scale : bool, (default : False)
             Scaling in range [0-255] by img*(255/max(img))
         denoise : string, (default : 'fastnl', None to disable)
             Filtering method to remove noise:
                 * None
                 * 'fastnl'
                 * 'bilateral'
                 * 'lee'
                 * 'lee_enhanced'
+                * 'lee_sigma'
                 * 'kuan'
                 * 'frost'
                 * 'median'
                 * 'mean'
-        window : int, (default : 3)
-            Denoising window. Increasing the window size may removes noise better but may also removes details of image in certain denoising methods.
-        cu : float, (default: 0.25)
-            The noise variation coefficient, applies for methods: ['kuan','lee','lee_enhanced']
-        params : dict() (Default: None)
-            caerus parameters can be defined in this dict. If None defined, then all default caerus parameters are used:
-            {'window': 50, 'minperc': 3, 'nlargest': 10, 'threshold': 0.25}
+        params : dict():
+            Denoising parameters for the methods. If None are defined, the default will be used:
+            caerus (default): {'window': 50, 'minperc': 3, 'nlargest': 10, 'threshold': 0.25}
+            lee_sigma (default): {'window': 7, 'sigma': 0.9, 'num_looks': 1, 'tk': 5}
+                * 'sigma': float, (default: 0.9): Speckle noise standard deviation, applies for methods: ['lee_sigma']
+                * 'num_looks': int, (default: 1): Number of looks of the SAR img, applies for methods: ['lee_sigma']
+                * 'tk': int, (default: 5): Threshold of neighbouring pixels outside of the 98th percentile, applies for methods: ['lee_sigma']
+                * cu : float, (default: 0.25): The noise variation coefficient, applies for methods: ['kuan','lee','lee_enhanced']
+                * window : int, (default : 3): Denoising window. Increasing the window size may removes noise better but may also removes details of image in certain denoising methods.
         togray : bool, (default : False)
             Conversion to gray scale.
-        imsize : tuple, (default : None)
-            size to desired (width,length).
         verbose : int (default : 3)
             Print to screen. 0: None, 1: Error, 2: Warning, 3: Info, 4: Debug, 5: Trace.
 
         Returns
         -------
         dict()
-            * See 1dpeaks and 2dpeaks for more details.
+            See 1dpeaks and 2dpeaks for more details.
 
         Examples
         --------
         >>> from findpeaks import findpeaks
         >>> X = [9,60,377,985,1153,672,501,1068,1110,574,135,23,3,47,252,812,1182,741,263,33]
         >>> fp = findpeaks(method='peakdetect', interpolate=10, lookahead=1)
         >>> results = fp.fit(X)
@@ -143,51 +161,63 @@
         >>> from findpeaks import findpeaks
         >>> X = fp.import_example('2dpeaks')
         >>> results = fp.fit(X)
         >>> fp.plot()
         >>>
         >>> # Image example
         >>> from findpeaks import findpeaks
-        >>> fp = findpeaks(method='topology', denoise='fastnl', window=30, imsize=(300,300))
+        >>> fp = findpeaks(method='topology', denoise='fastnl', params={'window': 30}, imsize=(300,300))
         >>> X = fp.import_example('2dpeaks_image')
         >>> results = fp.fit(X)
         >>> fp.plot()
         >>>
         >>> # Plot each seperately
         >>> fp.plot_preprocessing()
         >>> fp.plot_persistence()
         >>> fp.plot_mesh()
 
         References
         ----------
             * https://erdogant.github.io/findpeaks/
         """
+        if window is not None: print('The input parameter "window" will be deprecated in future releases. Please use "params={"window": 5}" instead.')
+        if cu is not None: print('The input parameter "cu" will be deprecated in future releases. Please use "params={"cu": 3}" instead.')
+
         # Store in object
         if isinstance(whitelist, str): whitelist=[whitelist]
         if lookahead is None: lookahead=1
         lookahead = np.maximum(1, lookahead)
         # if method is None: raise Exception('[findpeaks] >Specify the desired method="topology", "peakdetect", or "mask".')
         self.method = method
         self.whitelist = whitelist
         self.lookahead = lookahead
         self.interpolate = interpolate
         self.limit = limit
         self.imsize = imsize
         self.scale = scale
         self.togray = togray
         self.denoise = denoise
-        self.window = window
-        self.cu = cu
         self.figsize = figsize
         self.verbose = verbose
 
         # Store parameters for caerus
-        caerus_defaults = {'window': 50, 'minperc': 3, 'nlargest': 10, 'threshold': 0.25}
-        params_caerus = {**caerus_defaults, **params_caerus}
-        self.params_caerus = params_caerus
+        defaults={}
+        if method=='caerus':
+            if len(params_caerus)>0:
+                print('The input parameter "params_caerus" will be deprecated in future releases. Please use "params" instead.')
+                params = params_caerus
+            defaults = {'window': 50, 'minperc': 3, 'nlargest': 10, 'threshold': 0.25}
+        elif method=='lee_sigma':
+            defaults = {'window': 7, 'sigma': 0.9, 'num_looks': 1, 'tk': 5}
+        defaults = {**{'window': 3, 'cu': 3}, **defaults}
+
+        params = {**defaults, **params}
+        self.window = params['window']
+        self.cu = params['cu']
+        self.params = params
 
     def fit(self, X, x=None):
         """Detect peaks and valleys in a 1D vector or 2D-array (image).
 
         Description
         -----------
         * Fit the method on your data for the detection of peaks.
@@ -296,15 +326,15 @@
             result['peakdetect'] = stats._post_processing(X, Xraw, min_peaks, max_peaks, self.interpolate, self.lookahead)
         elif method=='topology':
             # Compute persistence using toplogy method
             result = stats.topology(np.c_[X, X], limit=self.limit, verbose=self.verbose)
             # Post processing for the topology method
             result['topology'] = stats._post_processing(X, Xraw, result['valley'], result['peak'], self.interpolate, 1)
         elif method=='caerus':
-            cs = caerus(**self.params_caerus)
+            cs = caerus(**self.params)
             result = cs.fit(X, return_as_dict=True, verbose=self.verbose)
             # Post processing for the caerus method
             result['caerus'] = stats._post_processing(X, Xraw, np.c_[result['loc_start_best'], result['loc_start_best']], np.c_[result['loc_stop_best'], result['loc_stop_best']], self.interpolate, 1, labxRaw=result['df']['labx'].values)
             result['caerus']['model'] = cs
         else:
             if self.verbose>=2: print('[findpeaks] >WARNING: [method="%s"] is not supported in 1d-vector data. <return>' %(self.method))
             return None
@@ -415,15 +445,15 @@
             results['df'] = dfint
 
         if self.method=='caerus':
             results['model'] = result['caerus']['model']
         # Arguments
         args = {}
         args['method'] = self.method
-        args['params_caerus'] = self.params_caerus
+        args['params'] = self.params
         args['lookahead'] = self.lookahead
         args['interpolate'] = self.interpolate
         args['figsize'] = self.figsize
         args['type'] = self.type
         # Return
         return results, args
 
@@ -439,14 +469,15 @@
             * scale : Scaling data in range [0-255] by img*(255/max(img))
             * denoise : Remove noise using method:
                 * None
                 * 'fastnl'
                 * 'bilateral'
                 * 'lee'
                 * 'lee_enhanced'
+                * 'lee_sigma'
                 * 'kuan'
                 * 'frost'
                 * 'median'
                 * 'mean'
             * window : Denoising window.
             * cu : noise variation coefficient
             * togray : Conversion to gray scale.
@@ -478,15 +509,15 @@
         >>> X = fp.import_example('2dpeaks')
         >>> results = fp.fit(X)
         >>> fp.plot()
         >>>
         >>> # Image example
         >>> from findpeaks import findpeaks
         >>> X = fp.import_example('2dpeaks_image')
-        >>> fp = findpeaks(denoise='fastnl', window=30, imsize=(300,300))
+        >>> fp = findpeaks(denoise='fastnl', params={'window': 30}, imsize=(300,300))
         >>> results = fp.fit(X)
         >>> fp.plot()
         >>>
         >>> # Plot each seperately
         >>> fp.plot_preprocessing()
         >>> fp.plot_persistence()
         >>> fp.plot_mesh()
@@ -550,16 +581,14 @@
         # Return
         return results, args
 
     # Pre-processing
     def preprocessing(self, X, showfig=False):
         """Preprocessing steps of the 2D array (image).
 
-        Description
-        -----------
         The pre-processing has 4 (optional) steps.
             1. Resizing (to reduce computation time).
             2. Scaling color pixels between [0-255]
             3. Conversion to gray-scale. This is required for some analysis.
             4. Denoising of the image.
 
         Parameters
@@ -582,15 +611,15 @@
             iax = 0
 
             # Plot RAW input image
             ax[iax].imshow(X, cmap=('gray_r' if self.togray else None))
             ax[iax].grid(False)
             ax[iax].set_title('Input\nRange: [%.3g,%.3g]' %(X.min(), X.max()))
             iax = iax + 1
-            plt.show()
+            # plt.show()
 
         # Resize
         if self.imsize:
             X = stats.resize(X, size=self.imsize, verbose=self.verbose)
             if showfig:
                 # plt.figure(figsize=self.figsize)
                 ax[iax].imshow(X, cmap=('gray_r' if self.togray else None))
@@ -915,14 +944,33 @@
             [None, 5]: Limit between range unlimited and 5.
         figsize : (int, int), (default: None)
             (width, height) in inches.
         savepath : bool (default : None)
             Path with filename to save the figure, eg: './tmp/my_image.png'
         verbose : int (default : 3)
             Print to screen. 0: None, 1: Error, 2: Warning, 3: Info, 4: Debug, 5: Trace.
+        
+        Example
+        -------
+        >>> # Import library
+        >>> from findpeaks import findpeaks
+        >>> #
+        >>> # Initialize
+        >>> fp = findpeaks(method='topology', scale=False, denoise=None, togray=False, imsize=False, params={'window': 15})
+        >>> #
+        >>> # Load example data set
+        >>> X = fp.import_example('2dpeaks')
+        >>> #
+        >>> # Fit model
+        >>> fp.fit(X)
+        >>> #
+        >>> # Create mesh plot
+        >>> fp.plot_mesh()
+        >>> # Create mesh plot with limit on x-axis and y-axis
+        >>> fp.plot_mesh(xlim=[10, 30], ylim=[4, 10], zlim=[None, 8])
 
         Returns
         -------
         fig_axis : tuple containing axis for each figure.
 
         """
         if not hasattr(self, 'results'):
```

### Comparing `findpeaks-2.4.7/findpeaks/interpolate.py` & `findpeaks-2.5.0/findpeaks/interpolate.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.7/findpeaks/stats.py` & `findpeaks-2.5.0/findpeaks/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 # github: https://github.com/erdogant/findpeaks
 # Licence: MIT
 # ----------------------------------------------------
 
 import findpeaks.union_find as union_find
 from findpeaks.filters.lee import lee_filter
 from findpeaks.filters.lee_enhanced import lee_enhanced_filter
+from findpeaks.filters.lee_sigma import lee_sigma_filter
 from findpeaks.filters.kuan import kuan_filter
 from findpeaks.filters.frost import frost_filter
 from findpeaks.filters.median import median_filter
 from findpeaks.filters.mean import mean_filter
 
 # #### DEBUG ONLY ####
 # import union_find as union_find
 # from filters.lee import lee_filter
 # from filters.lee_enhanced import lee_enhanced_filter
+# from filters.lee_sigma import lee_sigma_filter
 # from filters.kuan import kuan_filter
 # from filters.frost import frost_filter
 # from filters.median import median_filter
 # from filters.mean import mean_filter
 # ######################
 
 from scipy.ndimage.morphology import generate_binary_structure, binary_erosion
@@ -159,22 +161,29 @@
     method: string, (default: 'fastnl', None to disable)
         Filtering method to remove noise
             * None
             * 'fastnl'
             * 'bilateral'
             * 'lee'
             * 'lee_enhanced'
+            * 'lee_sigma'
             * 'kuan'
             * 'frost'
             * 'median'
             * 'mean'
     window: int, (default: 3)
         Denoising window. Increasing the window size may removes noise better but may also removes details of image in certain denoising methods.
     cu: float, (default: 0.25)
         The noise variation coefficient, applies for methods: ['kuan','lee','lee_enhanced']
+    sigma: float, (default: 0.9)
+        Speckle noise standard deviation, applies for methods: ['lee_sigma']
+    num_looks : int, (default: 1)
+        Number of looks of the SAR img, applies for methods: ['lee_sigma']
+    tk: int, (default: 5)
+        Threshold of neighbouring pixels outside of the 98th percentile, applies for methods: ['lee_sigma']
     verbose: int (default: 3)
         Print to screen. 0: None, 1: Error, 2: Warning, 3: Info, 4: Debug, 5: Trace.
 
     Returns
     -------
     X: array-like
         Denoised data.
@@ -200,14 +209,16 @@
             X = cv2.fastNlMeansDenoisingColored(X, h=window)
     elif method=='bilateral':
         X = cv2.bilateralFilter(X, window, 75, 75)
     elif method=='lee':
         X = lee_filter(X, win_size=window, cu=cu)
     elif method=='lee_enhanced':
         X = lee_enhanced_filter(X, win_size=window, cu=cu, k=1, cmax=1.73)
+    elif method=='lee_sigma':
+        X = lee_sigma_filter(X, sigma=0.9, win_size=window, num_looks=1, tk=5)
     elif method=='kuan':
         X = kuan_filter(X, win_size=window, cu=cu)
     elif method=='frost':
         X = frost_filter(X, win_size=window, damping_factor=2)
     elif method=='median':
         X = median_filter(X, win_size=window)
     elif method=='mean':
```

### Comparing `findpeaks-2.4.7/findpeaks/tests/test_findpeaks.py` & `findpeaks-2.5.0/findpeaks/tests/test_findpeaks.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     
         # CHECK OUTPUT METHOD TOPOLOGY
         fp = findpeaks(method="topology")
         X = fp.import_example('1dpeaks')
         results = fp.fit(X)
         assert fp.type=='peaks1d'
         assert [*results.keys()]==['persistence', 'Xdetect', 'Xranked', 'groups0', 'df']
-        assert [*fp.args]==['method', 'params_caerus', 'lookahead', 'interpolate', 'figsize', 'type']
+        assert [*fp.args]==['method', 'params', 'lookahead', 'interpolate', 'figsize', 'type']
         assert len(X)==len(results['Xdetect'])
         assert len(X)==len(results['Xranked'])
         assert len(X)==results['df'].shape[0]
         assert np.all(np.isin(results['df'].columns, ['x', 'y', 'labx', 'rank', 'score', 'valley', 'peak']))
         assert np.all(np.isin(results['persistence'].columns, ['x', 'y', 'birth_level', 'death_level', 'score']))
         
         # CHECK RESULTS METHOD TOPOLOGY
@@ -107,15 +107,15 @@
         
         # CHECK OUTPUT METHOD PEAKDETECT
         fp = findpeaks(method="peakdetect", lookahead=1, verbose=3)
         X = fp.import_example('1dpeaks')
         results = fp.fit(X)
         assert fp.type=='peaks1d'
         assert [*results.keys()]==['df']
-        assert [*fp.args]==['method', 'params_caerus', 'lookahead', 'interpolate', 'figsize', 'type']
+        assert [*fp.args]==['method', 'params', 'lookahead', 'interpolate', 'figsize', 'type']
         assert len(X)==results['df'].shape[0]
         assert np.all(np.isin(results['df'].columns, ['x', 'y', 'labx', 'valley', 'peak', 'rank', 'score']))
         
         # CHECK RESULTS METHOD TOPOLOGY
         assert results['df']['peak'].sum()==2
         assert results['df']['valley'].sum()==4
     
@@ -127,14 +127,16 @@
         for method in methods:
             for interpolate in interpolates:
                 for lookahead in lookaheads:
                     fp = findpeaks(lookahead=lookahead, interpolate=interpolate, method=method, verbose=0)
                     assert fp.fit(X)
     
     
+    def test_denoising(self):
+
         # DENOISING METHODS TEST
         from findpeaks import findpeaks
         fp = findpeaks()
         img = fp.import_example('2dpeaks_image')
         import findpeaks
         
         # filters parameters
@@ -168,32 +170,34 @@
         image_frost = findpeaks.stats.frost_filter(img.copy(), damping_factor=k_value1, win_size=winsize)
         # kuan filter
         image_kuan = findpeaks.kuan_filter(img.copy(), win_size=winsize, cu=cu_value)
         # lee filter
         image_lee = findpeaks.stats.lee_filter(img.copy(), win_size=winsize, cu=cu_value)
         # lee enhanced filter
         image_lee_enhanced = findpeaks.stats.lee_enhanced_filter(img.copy(), win_size=winsize, k=k_value2, cu=cu_lee_enhanced, cmax=cmax_value)
+        # lee sigma filter
+        image_lee_sigma = findpeaks.stats.lee_sigma_filter(img.copy(), win_size=winsize)
         # mean filter
         image_mean = findpeaks.stats.mean_filter(img.copy(), win_size=winsize)
         # median filter
         image_median = findpeaks.stats.median_filter(img.copy(), win_size=winsize)
     
         
         # Loop throughout many combinations of parameter settings
         from findpeaks import findpeaks
         methods = ['caerus', 'mask','topology', None]
-        filters = ['lee','lee_enhanced','kuan','fastnl','bilateral','frost','median','mean', None]
+        filters = ['lee','lee_enhanced','lee_sigma','kuan','fastnl','bilateral','frost','median','mean', None]
         windows = [None, 3, 63]
         cus = [None, 0, 0.75]
         img = fp.import_example('2dpeaks')
     
         for getfilter in filters:
             for window in windows:
                 for cu in cus:
-                    fp = findpeaks(method='topology', scale=True, denoise=getfilter, window=window, cu=cu, togray=True, imsize=None, verbose=3)
+                    fp = findpeaks(method='topology', scale=True, denoise=getfilter, params={'window': window, 'cu': cu}, togray=True, imsize=None, verbose=3)
                     assert fp.fit(img)
                     # assert fp.plot_mesh(wireframe=False)
                     # plt.close('all')
                     # assert fp.plot_persistence()
                     # plt.close('all')
                     # assert fp.plot()
                     # plt.close('all')
```

### Comparing `findpeaks-2.4.7/findpeaks/union_find.py` & `findpeaks-2.5.0/findpeaks/union_find.py`

 * *Files identical despite different names*

### Comparing `findpeaks-2.4.7/findpeaks.egg-info/PKG-INFO` & `findpeaks-2.5.0/findpeaks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: findpeaks
-Version: 2.4.7
+Version: 2.5.0
 Summary: findpeaks is for the detection of peaks and valleys in a 1D vector and 2D array (image).
 Home-page: https://erdogant.github.io/findpeaks
-Download-URL: https://github.com/erdogant/findpeaks/archive/2.4.7.tar.gz
+Download-URL: https://github.com/erdogant/findpeaks/archive/2.5.0.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: findpeaks Version: 2.4.7 Summary: findpeaks is for
+Metadata-Version: 2.1 Name: findpeaks Version: 2.5.0 Summary: findpeaks is for
 the detection of peaks and valleys in a 1D vector and 2D array (image). Home-
 page: https://erdogant.github.io/findpeaks Download-URL: https://github.com/
-erdogant/findpeaks/archive/2.4.7.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant/findpeaks/archive/2.5.0.tar.gz Author: Erdogan Taskesen Author-email:
 erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE # findpeaks [![Python](https://img.shields.io/pypi/
 pyversions/findpeaks)](https://img.shields.io/pypi/pyversions/findpeaks) [!
 [Pypi](https://img.shields.io/pypi/v/findpeaks)](https://pypi.org/project/
 findpeaks/) [![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
```

### Comparing `findpeaks-2.4.7/findpeaks.egg-info/SOURCES.txt` & `findpeaks-2.5.0/findpeaks.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 findpeaks.egg-info/top_level.txt
 findpeaks/data/__init__.py
 findpeaks/filters/__init__.py
 findpeaks/filters/frost.py
 findpeaks/filters/kuan.py
 findpeaks/filters/lee.py
 findpeaks/filters/lee_enhanced.py
+findpeaks/filters/lee_sigma.py
 findpeaks/filters/mean.py
 findpeaks/filters/median.py
 findpeaks/tests/__init__.py
 findpeaks/tests/test_findpeaks.py
```

### Comparing `findpeaks-2.4.7/setup.py` & `findpeaks-2.5.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,23 @@
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-     install_requires=['scipy','matplotlib','numpy','pandas','tqdm','peakdetect==1.1','requests','caerus>=0.1.9'],
+     install_requires=['scipy',
+                       'matplotlib',
+                       'numpy',
+                       'pandas',
+                       'tqdm',
+                       'peakdetect==1.1',
+                       'requests',
+                       'caerus>=0.1.9',
+                       'xarray'],
      python_requires='>=3',
      name='findpeaks',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="findpeaks is for the detection of peaks and valleys in a 1D vector and 2D array (image).",
      long_description=long_description,
```


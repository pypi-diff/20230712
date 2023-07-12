# Comparing `tmp/scientific_plots-1.6.0.tar.gz` & `tmp/scientific_plots-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scientific_plots-1.6.0.tar", last modified: Fri Jul  7 14:48:26 2023, max compression
+gzip compressed data, was "scientific_plots-1.7.0.tar", last modified: Wed Jul 12 15:55:48 2023, max compression
```

## Comparing `scientific_plots-1.6.0.tar` & `scientific_plots-1.7.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.476354 scientific_plots-1.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-25 08:00:18.000000 scientific_plots-1.6.0/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)    11607 2023-07-07 14:48:26.476354 scientific_plots-1.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-25 08:15:40.000000 scientific_plots-1.6.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.6.0/readme.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 14:48:26.476354 scientific_plots-1.6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/cycler-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/cycler-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/hurst-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/hurst-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/matplotlib-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-30 21:18:04.000000 scientific_plots-1.6.0/src/matplotlib-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/matplotlib-stubs/animation.pyi
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.6.0/src/matplotlib-stubs/cm.pyi
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/matplotlib-stubs/colors.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1354 2023-07-07 14:38:21.000000 scientific_plots-1.6.0/src/matplotlib-stubs/figure.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/matplotlib-stubs/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     8959 2023-07-07 14:38:21.000000 scientific_plots-1.6.0/src/matplotlib-stubs/pyplot/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/matplotlib-stubs/pyplot/style.pyi
--rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.6.0/src/matplotlib-stubs/ticker.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/mpl_toolkits-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.6.0/src/mpl_toolkits-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.6.0/src/mpl_toolkits-stubs/mplot.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/numba-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/numba-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.468354 scientific_plots-1.6.0/src/python_translator-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/python_translator-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.472354 scientific_plots-1.6.0/src/scientific_plots/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-07-07 14:38:21.000000 scientific_plots-1.6.0/src/scientific_plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scientific_plots/data_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18907 2023-06-25 08:00:18.000000 scientific_plots-1.6.0/src/scientific_plots/default_plots.py
--rw-rw-rw-   0 root         (0) root         (0)    17756 2023-06-25 08:00:18.000000 scientific_plots-1.6.0/src/scientific_plots/plot_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 14:48:00.000000 scientific_plots-1.6.0/src/scientific_plots/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scientific_plots/two_d_plot.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scientific_plots/types_.py
--rw-rw-rw-   0 root         (0) root         (0)     8954 2023-06-25 09:05:46.000000 scientific_plots-1.6.0/src/scientific_plots/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.472354 scientific_plots-1.6.0/src/scientific_plots.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11607 2023-07-07 14:48:26.000000 scientific_plots-1.6.0/src/scientific_plots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1363 2023-07-07 14:48:26.000000 scientific_plots-1.6.0/src/scientific_plots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 14:48:26.000000 scientific_plots-1.6.0/src/scientific_plots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-07 14:48:26.000000 scientific_plots-1.6.0/src/scientific_plots.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      126 2023-07-07 14:48:26.000000 scientific_plots-1.6.0/src/scientific_plots.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.472354 scientific_plots-1.6.0/src/scipy-stubs/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/fft.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1134 2023-07-07 14:38:21.000000 scientific_plots-1.6.0/src/scipy-stubs/integrate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3032 2023-07-07 14:38:21.000000 scientific_plots-1.6.0/src/scipy-stubs/interpolate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/optimize.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.472354 scientific_plots-1.6.0/src/scipy-stubs/signal/
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/signal/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/signal/windows.pyi
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/special.pyi
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/src/scipy-stubs/stats.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 14:48:26.476354 scientific_plots-1.6.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.6.0/tests/test_plot_manual.py
--rw-rw-rw-   0 root         (0) root         (0)     3672 2023-06-25 09:13:03.000000 scientific_plots-1.6.0/tests/test_plots.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.6.0/tests/test_utilties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-25 08:00:18.000000 scientific_plots-1.7.0/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)    11607 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-25 08:15:40.000000 scientific_plots-1.7.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.7.0/readme.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.611552 scientific_plots-1.7.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.611552 scientific_plots-1.7.0/src/cycler-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/cycler-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.611552 scientific_plots-1.7.0/src/hurst-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/hurst-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.615552 scientific_plots-1.7.0/src/matplotlib-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-30 21:18:04.000000 scientific_plots-1.7.0/src/matplotlib-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/matplotlib-stubs/animation.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.7.0/src/matplotlib-stubs/cm.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/matplotlib-stubs/colors.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1464 2023-07-12 15:45:02.000000 scientific_plots-1.7.0/src/matplotlib-stubs/figure.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.615552 scientific_plots-1.7.0/src/matplotlib-stubs/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     8988 2023-07-12 15:45:02.000000 scientific_plots-1.7.0/src/matplotlib-stubs/pyplot/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/matplotlib-stubs/pyplot/style.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-06-24 21:33:21.000000 scientific_plots-1.7.0/src/matplotlib-stubs/ticker.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.615552 scientific_plots-1.7.0/src/mpl_toolkits-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.7.0/src/mpl_toolkits-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.7.0/src/mpl_toolkits-stubs/mplot.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.615552 scientific_plots-1.7.0/src/numba-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/numba-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.615552 scientific_plots-1.7.0/src/python_translator-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/python_translator-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.615552 scientific_plots-1.7.0/src/scientific_plots/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-07-11 17:08:49.000000 scientific_plots-1.7.0/src/scientific_plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scientific_plots/data_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18907 2023-06-25 08:00:18.000000 scientific_plots-1.7.0/src/scientific_plots/default_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    19709 2023-07-12 15:45:02.000000 scientific_plots-1.7.0/src/scientific_plots/plot_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-12 15:55:22.000000 scientific_plots-1.7.0/src/scientific_plots/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scientific_plots/two_d_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scientific_plots/types_.py
+-rw-rw-rw-   0 root         (0) root         (0)     8954 2023-06-25 09:05:46.000000 scientific_plots-1.7.0/src/scientific_plots/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/src/scientific_plots.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11607 2023-07-12 15:55:48.000000 scientific_plots-1.7.0/src/scientific_plots.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-07-12 15:55:48.000000 scientific_plots-1.7.0/src/scientific_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 15:55:48.000000 scientific_plots-1.7.0/src/scientific_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-12 15:55:48.000000 scientific_plots-1.7.0/src/scientific_plots.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-07-12 15:55:48.000000 scientific_plots-1.7.0/src/scientific_plots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/src/scipy-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/fft.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2023-07-07 14:38:21.000000 scientific_plots-1.7.0/src/scipy-stubs/integrate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3032 2023-07-07 14:38:21.000000 scientific_plots-1.7.0/src/scipy-stubs/interpolate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/optimize.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/src/scipy-stubs/signal/
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/signal/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/signal/windows.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/special.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/src/scipy-stubs/stats.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 15:55:48.619552 scientific_plots-1.7.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.7.0/tests/test_plot_manual.py
+-rw-rw-rw-   0 root         (0) root         (0)     3783 2023-07-12 15:45:02.000000 scientific_plots-1.7.0/tests/test_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.7.0/tests/test_utilties.py
```

### Comparing `scientific_plots-1.6.0/COPYING.LESSER` & `scientific_plots-1.7.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/PKG-INFO` & `scientific_plots-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific_plots
-Version: 1.6.0
+Version: 1.7.0
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scientific_plots-1.6.0/pyproject.toml` & `scientific_plots-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/readme.md` & `scientific_plots-1.7.0/readme.md`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/cycler-stubs/__init__.pyi` & `scientific_plots-1.7.0/src/cycler-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/matplotlib-stubs/__init__.pyi` & `scientific_plots-1.7.0/src/matplotlib-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/matplotlib-stubs/colors.pyi` & `scientific_plots-1.7.0/src/matplotlib-stubs/colors.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/matplotlib-stubs/figure.pyi` & `scientific_plots-1.7.0/src/matplotlib-stubs/figure.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 """This is the stub for the figure-type in matplot-lib."""
 from __future__ import annotations
 
+from pathlib import Path
 from typing import Optional, Tuple, Iterable, Any, Union
 
 from .pyplot import Axes
 
 
 class Canvas:
     """Canvas, which contains the figure."""
@@ -40,11 +41,14 @@
     def set_label(self, label: str) -> None: ...
 
     def text(self, x: float, y: float, s: str) -> None: ...
 
     def legend(self, *args: Any, **kwargs: Any) -> None: ...
 
     def savefig(
-        self, fname: str, *, dpi: Union[str, float] = "figure",
-        bbox_inches: Optional[tuple[float, float]] = None,
+        self, fname: Union[str, Path], *,
+        dpi: Union[str, float, int, None] = "figure",
+        bbox_inches: Optional[Union[tuple[float, float], str]] = None,
         pad_inches: float = 0.1, backend: Optional[str] = None
         ) -> None: ...
+
+    def tight_layout(self) -> None: ...
```

### Comparing `scientific_plots-1.6.0/src/matplotlib-stubs/pyplot/__init__.pyi` & `scientific_plots-1.7.0/src/matplotlib-stubs/pyplot/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,18 @@
 
 
 def set_cmap(color: Union[colors.ListedColormap,
                           str,
                           colors.LinearSegmentedColormap]) -> None: ...
 
 
-def savefig(filename: Union[Path, str],
-            dpi: Optional[int] = None, bbox_inches: Optional[str] = None)\
+def savefig(
+    filename: Union[Path, str],
+    dpi: Optional[int] = None,
+    bbox_inches: Optional[Union[tuple[float, float], str]] = None)\
         -> None: ...
 
 
 def tight_layout() -> None: ...
 
 
 class Label:
```

### Comparing `scientific_plots-1.6.0/src/matplotlib-stubs/ticker.pyi` & `scientific_plots-1.7.0/src/matplotlib-stubs/ticker.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/numba-stubs/__init__.pyi` & `scientific_plots-1.7.0/src/numba-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/scientific_plots/data_analysis.py` & `scientific_plots-1.7.0/src/scientific_plots/data_analysis.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/scientific_plots/default_plots.py` & `scientific_plots-1.7.0/src/scientific_plots/default_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/scientific_plots/plot_settings.py` & `scientific_plots-1.7.0/src/scientific_plots/plot_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 the hard drive
 """
 from __future__ import annotations
 
 import csv
 import locale
 from contextlib import contextmanager
-from math import sqrt
-from copy import copy
+from copy import copy, deepcopy
 from functools import wraps
 from typing import (
     Generator, Optional, Union, Callable, Any, overload)
 from pathlib import Path
-from warnings import warn
+from warnings import warn, catch_warnings, simplefilter
 from textwrap import dedent
 
 import mpl_toolkits
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.pyplot import Axes
 from matplotlib import colors
@@ -30,15 +29,16 @@
 from .utilities import translate
 from .types_ import Vector
 
 mpl.use("Agg")
 plt.rcParams["axes.unicode_minus"] = False
 
 SPINE_COLOR = "black"
-FIGSIZE = (4.0, 4.0 * (sqrt(5) - 1.0) / 2.0)
+FIGSIZE = (4.4, 3.0)
+FIGSIZE_SMALL = (2.2, 2.1)
 _savefig = copy(plt.savefig)  # backup the old save-function
 
 
 def linestyles() -> Generator[str, None, None]:
     """get the line-stiles as an iterator"""
     yield "-"
     yield "dotted"
@@ -265,38 +265,66 @@
 
 
 old_save = plt.savefig
 
 
 def try_save(filename: Path,
              dpi: Optional[int] = None,
-             bbox_inches: Optional[str] = None) -> None:
+             bbox_inches: Optional[Union[str, tuple[float, float]]] = None, *,
+             small: bool = False) -> None:
     """Try to save the current figure to the given path, if it is not possible,
-    try to save it under a different name."""
+    try to save it under a different name.
+    If small is set to true, also create
+    a smaller version of the given plot."""
     try:
         old_save(filename, dpi=dpi, bbox_inches=bbox_inches)
     except PermissionError:
         old_save(filename.parent / (filename.stem + "_" + filename.suffix),
                  dpi=dpi, bbox_inches=bbox_inches)
 
+    if small:
+        fig = deepcopy(plt.gcf())
+        fig.set_size_inches(*FIGSIZE_SMALL)
+        with catch_warnings(record=True) as warning:
+            simplefilter("always")
+            fig.tight_layout()
+            if warning:
+                if issubclass(warning[-1].category, UserWarning):
+                    plt.close(fig)
+                    return
+        folder = filename.parent / "small"
+        folder.mkdir(exist_ok=True)
+        try:
+            fig.savefig(
+                folder
+                / filename.name, dpi=dpi, bbox_inches=bbox_inches)
+        except PermissionError:
+            fig.savefig(
+                folder
+                / (filename.stem + "_" + filename.suffix),
+                dpi=dpi, bbox_inches=bbox_inches)
+        plt.close(fig)
+
 
-def new_save_simple(subfolder: str = "", suffix: str = "",
-                    german: bool = False)\
+def new_save_simple(subfolder: Union[str, Path] = "", suffix: str = "", *,
+                    german: bool = False, png: bool = True,
+                    pdf: bool = True, small: bool = False)\
         -> Callable[..., None]:
     """
     Return a new save function, which saves the file to a new given name in pdf
     format, and also creates a png version.
     If the argument "german" is set to true, also create German language
     version of the plots.
     """
 
     @wraps(old_save)
     def savefig_(filename: Union[Path, str],
                  dpi: Optional[int] = None,
-                 bbox_inches: Optional[str] = None) -> None:
+                 bbox_inches: Optional[
+                     Union[tuple[float, float], str]] = None) -> None:
         """Save the plot to this location as pdf and png."""
         if isinstance(filename, str):
             filename = Path(filename)
         if filename.parent == Path("."):
             warn(
                 f"The filename {filename} in 'savefig' does "
                 f"not contain a subfolder (i.e. 'subfolder/{filename})! "
@@ -322,26 +350,32 @@
             data_plot(data_path)
 
         try:
             plt.tight_layout()
         except IndexError:
             pass
         # save the figure
-        try_save(new_path_pdf, bbox_inches=bbox_inches)
-        try_save(new_path_png, bbox_inches=bbox_inches,
-                 dpi=dpi)
+        if pdf:
+            try_save(new_path_pdf, bbox_inches=bbox_inches, small=small)
+        if png:
+            try_save(new_path_png, bbox_inches=bbox_inches,
+                     dpi=dpi, small=small)
 
         if german:
             with germanify(plt.gca()):
-                try_save(
-                    new_path_pdf.parent / (new_path_pdf.stem + "_german.pdf"),
-                    bbox_inches=bbox_inches)
-                try_save(
-                    new_path_png.parent / (new_path_png.stem + "_german.png"),
-                    bbox_inches=bbox_inches, dpi=dpi)
+                if pdf:
+                    try_save(
+                        new_path_pdf.parent
+                        / (new_path_pdf.stem + "_german.pdf"),
+                        bbox_inches=bbox_inches, small=small)
+                if png:
+                    try_save(
+                        new_path_png.parent
+                        / (new_path_png.stem + "_german.png"),
+                        bbox_inches=bbox_inches, dpi=dpi, small=small)
 
     return savefig_
 
 
 def presentation_settings() -> None:
     """Change the settings of rcParams for presentations."""
     # increase size
@@ -425,105 +459,131 @@
                  three_d: bool = False)\
         -> Union[Callable[[PlotFunction], PlotFunction], PlotFunction]:
     """Apply the newly defined styles to a function, which creates a plot."""
     # pylint: disable=too-many-statements
 
     def _decorator(_plot_function: PlotFunction) -> PlotFunction:
         """This is the  actual decorator. Thus, the outer function
-        'apply_styles' is acutally a decorator-factory."""
+        'apply_styles' is actually a decorator-factory."""
 
         @wraps(_plot_function)
         def new_plot_function(*args: Any, **kwargs: Any) -> None:
             """
             New plotting function, with applied styles.
             """
             # default plot
             plt.set_cmap("rwth_list")
             plt.savefig = new_save_simple()
             _plot_function(*args, **kwargs)
 
             errors = (OSError, FileNotFoundError, ThreeDPlotException)
 
+            def journal() -> None:
+                """Create a plot for journals."""
+                set_rwth_colors(three_d)
+                set_serif()
+                plt.savefig = new_save_simple("journal", png=False,
+                                              small=not three_d)
+                _plot_function(*args, **kwargs)
+
+            def sans_serif() -> None:
+                """
+                Create a plot for journals with sans-serif-fonts.
+                """
+                set_rwth_colors(three_d)
+                set_sans_serif()
+                plt.savefig = new_save_simple("sans_serif", german=True,
+                                              small=not three_d)
+                _plot_function(*args, **kwargs)
+
+            def grayscale() -> None:
+                """
+                Create a plot in grayscales for disserations.
+                """
+                mpl.rcParams["text.usetex"] = False
+                set_serif()
+                if three_d:
+                    plt.set_cmap("Greys")
+                    new_kwargs = copy(kwargs)
+                    new_kwargs["colorscheme"] = "Greys"
+                else:
+                    new_kwargs = kwargs
+                plt.savefig = new_save_simple("grayscale", png=False,
+                                              small=not three_d)
+                _plot_function(*args, **new_kwargs)
+
+            def presentation() -> None:
+                """
+                Create a plot for presentations.
+                """
+                if three_d:
+                    new_kwargs = copy(kwargs)
+                    new_kwargs["figsize"] = (9, 7)
+                    new_kwargs["labelpad"] = 20
+                    new_kwargs["nbins"] = 5
+                else:
+                    new_kwargs = kwargs
+                set_rwth_colors(three_d)
+                presentation_settings()
+                set_sans_serif()
+                plt.savefig = new_save_simple("presentation",
+                                              german=True, pdf=False)
+                _plot_function(*args, **new_kwargs)
+
             try:
                 check_3d(three_d)
+
+                # test if this context is available
+                plt.close("all")
+
                 # journal
                 with plt.style.context(["science", "ieee"]):
-                    set_rwth_colors()
-                    set_serif()
-                    plt.savefig = new_save_simple("journal")
-                    _plot_function(*args, **kwargs)
+                    journal()
 
                 # sans-serif
                 with plt.style.context(["science", "ieee", "nature"]):
-                    set_rwth_colors()
-                    set_sans_serif()
-                    plt.savefig = new_save_simple("sans_serif", german=True)
-                    _plot_function(*args, **kwargs)
+                    sans_serif()
 
                 # grayscale
                 with plt.style.context(["science", "ieee", "grayscale"]):
-                    mpl.rcParams["text.usetex"] = False
-                    set_serif()
-                    plt.savefig = new_save_simple("grayscale")
-                    _plot_function(*args, **kwargs)
+                    grayscale()
 
                 # presentation
                 with plt.style.context(["science", "ieee"]):
-                    set_rwth_colors()
-                    presentation_settings()
-                    set_sans_serif()
-                    plt.savefig = new_save_simple("presentation", german=True)
-                    _plot_function(*args, **kwargs)
+                    presentation()
 
             except errors:
                 if not three_d:
                     warn(dedent(""""Could not found style 'science'.
                                 The package was probably installed incorrectly.
                                 Using a fallback-style."""), ImportWarning)
                 # journal
                 with plt.style.context("fast"):
-                    set_rwth_colors(three_d)
-                    set_serif()
-                    plt.savefig = new_save_simple("journal")
-                    _plot_function(*args, **kwargs)
+                    if not three_d:
+                        mpl.rcParams["figure.figsize"] = FIGSIZE
+                        mpl.rcParams["font.size"] = 10
+                    journal()
 
                 # sans-serif
                 with plt.style.context("fast"):
-                    set_rwth_colors(three_d)
-                    set_sans_serif()
-                    plt.savefig = new_save_simple("sans_serif")
-                    _plot_function(*args, **kwargs)
+                    if not three_d:
+                        mpl.rcParams["figure.figsize"] = FIGSIZE
+                        mpl.rcParams["font.size"] = 10
+                    sans_serif()
 
                 # grayscale
                 with plt.style.context("grayscale"):
-                    if three_d:
-                        plt.set_cmap("Greys")
-                        new_kwargs = copy(kwargs)
-                        new_kwargs["colorscheme"] = "Greys"
-                    else:
-                        new_kwargs = kwargs
-                    mpl.rcParams["text.usetex"] = False
-                    set_serif()
-                    plt.savefig = new_save_simple("grayscale")
-                    _plot_function(*args, **new_kwargs)
+                    if not three_d:
+                        mpl.rcParams["figure.figsize"] = FIGSIZE
+                        mpl.rcParams["font.size"] = 10
+                    grayscale()
 
                 # presentation
                 with plt.style.context("fast"):
-                    if three_d:
-                        new_kwargs = copy(kwargs)
-                        new_kwargs["figsize"] = (9, 7)
-                        new_kwargs["labelpad"] = 20
-                        new_kwargs["nbins"] = 5
-                    else:
-                        new_kwargs = kwargs
-                    set_rwth_colors(three_d)
-                    presentation_settings()
-                    set_sans_serif()
-                    plt.savefig = new_save_simple("presentation", german=True)
-                    _plot_function(*args, **new_kwargs)
+                    presentation()
 
             plt.savefig = old_save
 
         return new_plot_function
 
     if plot_function is not None:
         return _decorator(plot_function)
```

### Comparing `scientific_plots-1.6.0/src/scientific_plots/two_d_plot.py` & `scientific_plots-1.7.0/src/scientific_plots/two_d_plot.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/scientific_plots/types_.py` & `scientific_plots-1.7.0/src/scientific_plots/types_.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/scientific_plots/utilities.py` & `scientific_plots-1.7.0/src/scientific_plots/utilities.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/scientific_plots.egg-info/PKG-INFO` & `scientific_plots-1.7.0/src/scientific_plots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific-plots
-Version: 1.6.0
+Version: 1.7.0
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scientific_plots-1.6.0/src/scientific_plots.egg-info/SOURCES.txt` & `scientific_plots-1.7.0/src/scientific_plots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/scipy-stubs/fft.pyi` & `scientific_plots-1.7.0/src/scipy-stubs/fft.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/scipy-stubs/integrate.pyi` & `scientific_plots-1.7.0/src/scipy-stubs/integrate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/scipy-stubs/interpolate.pyi` & `scientific_plots-1.7.0/src/scipy-stubs/interpolate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/scipy-stubs/optimize.pyi` & `scientific_plots-1.7.0/src/scipy-stubs/optimize.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/src/scipy-stubs/signal/__init__.pyi` & `scientific_plots-1.7.0/src/scipy-stubs/signal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/tests/test_plot_manual.py` & `scientific_plots-1.7.0/tests/test_plot_manual.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/tests/test_plots.py` & `scientific_plots-1.7.0/tests/test_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     """
     x_test: Vector = linspace(1., 100., 100)
     y_test: Vector = x_test**2
 
     x_label = "x-values"
     y_label = "y-values"
     filename = Path(".test_plot.tmp.pdf")
+    filename2 = Path(".test_plot.tmp.png")
     plot(x_test, y_test, x_label, y_label, tmp_path / filename)
     assert exists(tmp_path / filename)
 
     # test data-plot creation
     assert exists(tmp_path / (filename.stem + ".csv"))
     data = read_data_plot(tmp_path / (filename.stem + ".csv"))
     assert data
@@ -40,15 +41,17 @@
     remove(tmp_path / filename)
 
     # logarithmic plot
     plot(x_test, y_test, x_label, y_label, tmp_path / filename, logscale=True)
     assert exists(tmp_path / filename)
     subfolder = ["sans_serif", "grayscale", "journal", "presentation"]
     for folder in subfolder:
-        assert exists(tmp_path / folder / filename)
+        assert (
+            exists(tmp_path / folder / filename)
+            or exists(tmp_path / folder / filename2))
 
 
 @mark.use_style
 def test_default_plot_nan(tmp_path: Path) -> None:
     """
     Test the default plot creation by 'plot', if there are data points with
     nan.
```

### Comparing `scientific_plots-1.6.0/tests/test_types.py` & `scientific_plots-1.7.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.6.0/tests/test_utilties.py` & `scientific_plots-1.7.0/tests/test_utilties.py`

 * *Files identical despite different names*


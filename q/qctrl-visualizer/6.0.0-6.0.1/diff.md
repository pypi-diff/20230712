# Comparing `tmp/qctrl_visualizer-6.0.0.tar.gz` & `tmp/qctrl_visualizer-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_visualizer-6.0.0.tar", max compression
+gzip compressed data, was "qctrl_visualizer-6.0.1.tar", max compression
```

## Comparing `qctrl_visualizer-6.0.0.tar` & `qctrl_visualizer-6.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    36653 2023-06-26 23:47:58.155482 qctrl_visualizer-6.0.0/LICENSE
--rw-r--r--   0        0        0      755 2023-06-26 23:47:58.155482 qctrl_visualizer-6.0.0/README.md
--rw-r--r--   0        0        0     2495 2023-06-26 23:48:20.368034 qctrl_visualizer-6.0.0/pyproject.toml
--rw-r--r--   0        0        0     2106 2023-06-26 23:48:20.380034 qctrl_visualizer-6.0.0/qctrlvisualizer/__init__.py
--rw-r--r--   0        0        0    23319 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/bloch.py
--rw-r--r--   0        0        0    13992 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/confidence_ellipses.py
--rw-r--r--   0        0        0    17782 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/controls.py
--rw-r--r--   0        0        0     4555 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/cost_histories.py
--rw-r--r--   0        0        0     7355 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/density_matrix.py
--rw-r--r--   0        0        0     8486 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/filter_functions.py
--rw-r--r--   0        0        0     6553 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/histogram.py
--rw-r--r--   0        0        0    12487 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/populations.py
--rw-r--r--   0        0        0     4195 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/style.py
--rw-r--r--   0        0        0     5525 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/utils.py
--rw-r--r--   0        0        0     5858 2023-06-26 23:47:58.159482 qctrl_visualizer-6.0.0/qctrlvisualizer/wigner_function.py
--rw-r--r--   0        0        0     2902 1970-01-01 00:00:00.000000 qctrl_visualizer-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0    36653 2023-07-12 05:33:34.051236 qctrl_visualizer-6.0.1/LICENSE
+-rw-r--r--   0        0        0      754 2023-07-12 05:33:34.051236 qctrl_visualizer-6.0.1/README.md
+-rw-r--r--   0        0        0     2495 2023-07-12 05:33:54.543112 qctrl_visualizer-6.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2106 2023-07-12 05:33:54.551112 qctrl_visualizer-6.0.1/qctrlvisualizer/__init__.py
+-rw-r--r--   0        0        0    23319 2023-07-12 05:33:34.055236 qctrl_visualizer-6.0.1/qctrlvisualizer/bloch.py
+-rw-r--r--   0        0        0    13992 2023-07-12 05:33:34.055236 qctrl_visualizer-6.0.1/qctrlvisualizer/confidence_ellipses.py
+-rw-r--r--   0        0        0    17782 2023-07-12 05:33:34.055236 qctrl_visualizer-6.0.1/qctrlvisualizer/controls.py
+-rw-r--r--   0        0        0     4555 2023-07-12 05:33:34.055236 qctrl_visualizer-6.0.1/qctrlvisualizer/cost_histories.py
+-rw-r--r--   0        0        0     7355 2023-07-12 05:33:34.055236 qctrl_visualizer-6.0.1/qctrlvisualizer/density_matrix.py
+-rw-r--r--   0        0        0     8486 2023-07-12 05:33:34.055236 qctrl_visualizer-6.0.1/qctrlvisualizer/filter_functions.py
+-rw-r--r--   0        0        0     6553 2023-07-12 05:33:34.055236 qctrl_visualizer-6.0.1/qctrlvisualizer/histogram.py
+-rw-r--r--   0        0        0    12487 2023-07-12 05:33:34.055236 qctrl_visualizer-6.0.1/qctrlvisualizer/populations.py
+-rw-r--r--   0        0        0     4195 2023-07-12 05:33:34.055236 qctrl_visualizer-6.0.1/qctrlvisualizer/style.py
+-rw-r--r--   0        0        0     5525 2023-07-12 05:33:34.055236 qctrl_visualizer-6.0.1/qctrlvisualizer/utils.py
+-rw-r--r--   0        0        0     5858 2023-07-12 05:33:34.059236 qctrl_visualizer-6.0.1/qctrlvisualizer/wigner_function.py
+-rw-r--r--   0        0        0     2901 1970-01-01 00:00:00.000000 qctrl_visualizer-6.0.1/PKG-INFO
```

### Comparing `qctrl_visualizer-6.0.0/LICENSE` & `qctrl_visualizer-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-6.0.0/README.md` & `qctrl_visualizer-6.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,5 @@
 # Q-CTRL Visualizer
 
-The Q-CTRL Visualizer offers broad functionality to visually engage with
-quantum dynamics and quantum controls.  These tools can help you develop
-understanding and intuition, and ultimately support the implementation of your
-quantum controls. See the topic [Visualizing your data using the Q-CTRL
-Visualizer](https://docs.q-ctrl.com/boulder-opal/topics/visualizing-your-data-using-the-q-ctrl-visualizer)
-in the Q-CTRL documentation for more information.
+The Q-CTRL Visualizer offers broad functionality to visually engage with quantum dynamics and quantum controls. These tools can help you develop understanding and intuition, and ultimately support the implementation of your quantum controls. See the topic [Visualizing your data using the Q-CTRL Visualizer](https://docs.q-ctrl.com/boulder-opal/topics/visualizing-your-data-using-the-q-ctrl-visualizer) in the Q-CTRL documentation for more information.
 
-The Q-CTRL Visualizer is meant to be used with the Q-CTRL products Boulder
-Opal, Fire Opal, and Open Controls. See how you can get started with [Boulder
-Opal](https://docs.q-ctrl.com/boulder-opal/get-started) and [Fire
-Opal](https://docs.q-ctrl.com/fire-opal/get-started) today.
+The Q-CTRL Visualizer is meant to be used with the Q-CTRL products Boulder Opal, Fire Opal, and Open Controls. See how you can get started with [Boulder Opal](https://docs.q-ctrl.com/boulder-opal/get-started) and [Fire Opal](https://docs.q-ctrl.com/fire-opal/get-started) today.
```

### Comparing `qctrl_visualizer-6.0.0/pyproject.toml` & `qctrl_visualizer-6.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-visualizer"
-version = "6.0.0"
+version = "6.0.1"
 description = "Q-CTRL Visualizer"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 repository = ""
@@ -61,15 +61,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 matplotlib = ">=3.6.3"
 numpy = "^1.23.5"
 scipy = ">=1.9.3"
-qctrl-commons = "^18.1.1"
+qctrl-commons = "^19.1.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 pytest = "^7.3.2"
 pylint = "^2.17.4"
```

### Comparing `qctrl_visualizer-6.0.0/qctrlvisualizer/__init__.py` & `qctrl_visualizer-6.0.1/qctrlvisualizer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,8 +61,8 @@
     "plot_population_dynamics",
     "plot_population_distributions",
     "plot_bitstring_probabilities_histogram",
     "plot_sequences",
     "plot_wigner_function",
 ]
 
-__version__ = "6.0.0"
+__version__ = "6.0.1"
```

### Comparing `qctrl_visualizer-6.0.0/qctrlvisualizer/bloch.py` & `qctrl_visualizer-6.0.1/qctrlvisualizer/bloch.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-6.0.0/qctrlvisualizer/confidence_ellipses.py` & `qctrl_visualizer-6.0.1/qctrlvisualizer/confidence_ellipses.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-6.0.0/qctrlvisualizer/controls.py` & `qctrl_visualizer-6.0.1/qctrlvisualizer/controls.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-6.0.0/qctrlvisualizer/cost_histories.py` & `qctrl_visualizer-6.0.1/qctrlvisualizer/cost_histories.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-6.0.0/qctrlvisualizer/density_matrix.py` & `qctrl_visualizer-6.0.1/qctrlvisualizer/density_matrix.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-6.0.0/qctrlvisualizer/filter_functions.py` & `qctrl_visualizer-6.0.1/qctrlvisualizer/filter_functions.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-6.0.0/qctrlvisualizer/histogram.py` & `qctrl_visualizer-6.0.1/qctrlvisualizer/histogram.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-6.0.0/qctrlvisualizer/populations.py` & `qctrl_visualizer-6.0.1/qctrlvisualizer/populations.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-6.0.0/qctrlvisualizer/style.py` & `qctrl_visualizer-6.0.1/qctrlvisualizer/style.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-6.0.0/qctrlvisualizer/utils.py` & `qctrl_visualizer-6.0.1/qctrlvisualizer/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-6.0.0/qctrlvisualizer/wigner_function.py` & `qctrl_visualizer-6.0.1/qctrlvisualizer/wigner_function.py`

 * *Files identical despite different names*

### Comparing `qctrl_visualizer-6.0.0/PKG-INFO` & `qctrl_visualizer-6.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-visualizer
-Version: 6.0.0
+Version: 6.0.1
 Summary: Q-CTRL Visualizer
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -30,28 +30,20 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: matplotlib (>=3.6.3)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: qctrl-commons (>=18.1.1,<19.0.0)
+Requires-Dist: qctrl-commons (>=19.1.0,<20.0.0)
 Requires-Dist: scipy (>=1.9.3)
 Project-URL: Documentation, https://docs.q-ctrl.com/boulder-opal/references/qctrl-visualizer/
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Description-Content-Type: text/markdown
 
 # Q-CTRL Visualizer
 
-The Q-CTRL Visualizer offers broad functionality to visually engage with
-quantum dynamics and quantum controls.  These tools can help you develop
-understanding and intuition, and ultimately support the implementation of your
-quantum controls. See the topic [Visualizing your data using the Q-CTRL
-Visualizer](https://docs.q-ctrl.com/boulder-opal/topics/visualizing-your-data-using-the-q-ctrl-visualizer)
-in the Q-CTRL documentation for more information.
+The Q-CTRL Visualizer offers broad functionality to visually engage with quantum dynamics and quantum controls. These tools can help you develop understanding and intuition, and ultimately support the implementation of your quantum controls. See the topic [Visualizing your data using the Q-CTRL Visualizer](https://docs.q-ctrl.com/boulder-opal/topics/visualizing-your-data-using-the-q-ctrl-visualizer) in the Q-CTRL documentation for more information.
 
-The Q-CTRL Visualizer is meant to be used with the Q-CTRL products Boulder
-Opal, Fire Opal, and Open Controls. See how you can get started with [Boulder
-Opal](https://docs.q-ctrl.com/boulder-opal/get-started) and [Fire
-Opal](https://docs.q-ctrl.com/fire-opal/get-started) today.
+The Q-CTRL Visualizer is meant to be used with the Q-CTRL products Boulder Opal, Fire Opal, and Open Controls. See how you can get started with [Boulder Opal](https://docs.q-ctrl.com/boulder-opal/get-started) and [Fire Opal](https://docs.q-ctrl.com/fire-opal/get-started) today.
```


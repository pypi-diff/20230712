# Comparing `tmp/sierras-0.2.3.tar.gz` & `tmp/sierras-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sierras-0.2.3.tar", last modified: Tue Jun  6 21:18:00 2023, max compression
+gzip compressed data, was "sierras-0.2.4.tar", last modified: Wed Jul 12 18:50:05 2023, max compression
```

## Comparing `sierras-0.2.3.tar` & `sierras-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:18:00.397035 sierras-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-06 21:17:45.000000 sierras-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-06 21:17:45.000000 sierras-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-06 21:18:00.397035 sierras-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-06 21:17:45.000000 sierras-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-06 21:17:45.000000 sierras-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 21:18:00.397035 sierras-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:18:00.397035 sierras-0.2.3/sierras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-06 21:18:00.000000 sierras-0.2.3/sierras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-06 21:18:00.000000 sierras-0.2.3/sierras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:18:00.000000 sierras-0.2.3/sierras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 21:18:00.000000 sierras-0.2.3/sierras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 21:18:00.000000 sierras-0.2.3/sierras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-06-06 21:17:45.000000 sierras-0.2.3/sierras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:50:05.949802 sierras-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-12 18:49:45.000000 sierras-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-12 18:49:45.000000 sierras-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-07-12 18:50:05.949802 sierras-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-12 18:49:45.000000 sierras-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-12 18:49:45.000000 sierras-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:50:05.949802 sierras-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:50:05.945802 sierras-0.2.4/sierras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-07-12 18:50:05.000000 sierras-0.2.4/sierras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-12 18:50:05.000000 sierras-0.2.4/sierras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:50:05.000000 sierras-0.2.4/sierras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-12 18:50:05.000000 sierras-0.2.4/sierras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 18:50:05.000000 sierras-0.2.4/sierras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-12 18:49:45.000000 sierras-0.2.4/sierras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-07-12 18:49:45.000000 sierras-0.2.4/test_sierras.py
```

### Comparing `sierras-0.2.3/LICENSE` & `sierras-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sierras-0.2.3/PKG-INFO` & `sierras-0.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sierras
-Version: 0.2.3
+Version: 0.2.4
 Summary: A tool for empirical Arrhenius equation fitting for thermally-induced physicochemical processes.
 Author-email: Francisco Fernandez <ffernandev@gmail.com>
 License: MIT License
         
         Copyright (c) 2021-2023 Francisco Fernandez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -72,16 +72,15 @@
 ## Usage
 
 A simple example of use:
 
 ```python
 import sierras
 
-k_boltzmann = 8.617333262e-5  # eV / K
-areg = sierras.ArrheniusRegressor(k_boltzmann)
+areg = sierras.ArrheniusRegressor()
 
 areg.fit(Temperatures, target_process)
 
 areg.activation_energy_  # in this case in eV
 areg.extrapolated_process_  # extrapolated process at room temperature
 
 areg.plot.arrhenius(Temperatures, target_process)  # plot the fitting
```

### Comparing `sierras-0.2.3/README.md` & `sierras-0.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 ## Usage
 
 A simple example of use:
 
 ```python
 import sierras
 
-k_boltzmann = 8.617333262e-5  # eV / K
-areg = sierras.ArrheniusRegressor(k_boltzmann)
+areg = sierras.ArrheniusRegressor()
 
 areg.fit(Temperatures, target_process)
 
 areg.activation_energy_  # in this case in eV
 areg.extrapolated_process_  # extrapolated process at room temperature
 
 areg.plot.arrhenius(Temperatures, target_process)  # plot the fitting
```

### Comparing `sierras-0.2.3/pyproject.toml` & `sierras-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sierras"
-version = "0.2.3"
+version = "0.2.4"
 authors = [{name = "Francisco Fernandez", email = "ffernandev@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 description = "A tool for empirical Arrhenius equation fitting for thermally-induced physicochemical processes."
 keywords = [
     "arrhenius-process",
     "arrhenius-equation",
```

### Comparing `sierras-0.2.3/sierras.egg-info/PKG-INFO` & `sierras-0.2.4/sierras.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sierras
-Version: 0.2.3
+Version: 0.2.4
 Summary: A tool for empirical Arrhenius equation fitting for thermally-induced physicochemical processes.
 Author-email: Francisco Fernandez <ffernandev@gmail.com>
 License: MIT License
         
         Copyright (c) 2021-2023 Francisco Fernandez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -72,16 +72,15 @@
 ## Usage
 
 A simple example of use:
 
 ```python
 import sierras
 
-k_boltzmann = 8.617333262e-5  # eV / K
-areg = sierras.ArrheniusRegressor(k_boltzmann)
+areg = sierras.ArrheniusRegressor()
 
 areg.fit(Temperatures, target_process)
 
 areg.activation_energy_  # in this case in eV
 areg.extrapolated_process_  # extrapolated process at room temperature
 
 areg.plot.arrhenius(Temperatures, target_process)  # plot the fitting
```

### Comparing `sierras-0.2.3/sierras.py` & `sierras-0.2.4/sierras.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,16 +64,15 @@
 import sklearn.linear_model
 from sklearn.base import BaseEstimator, RegressorMixin
 
 # =============================================================================
 # CONSTANTS
 # =============================================================================
 
-__all__ = ["ArrheniusRegressor", "ArrheniusPlotter"]
-
+__all__ = ["ArrheniusRegressor"]
 
 NAME = "sierras"
 
 DOC = __doc__
 
 VERSION = importlib_metadata.version(NAME)
 
@@ -87,21 +86,17 @@
 
 
 class ArrheniusRegressor(BaseEstimator, RegressorMixin):
     r"""Arrhenius equation fitting.
 
     Parameters
     ----------
-    constant : float
+    constant : float, default=8.617333262e-5
         Either the universal gas constant, :math:`R`, or the Boltzmann
-        constant, :math:`k_B`.
-
-    **kwargs
-        Keyword arguments that are passed and are documented in
-        ``sklearn.linear_model.LinearRegression``.
+        constant, :math:`k_B`, default value is the later in eV/K units.
 
     Attributes
     ----------
     activation_energy_ : float
         Activation energy of the process, this is the same as
         ``-self.constant * self.reg_.coef_[0]``.
 
@@ -110,32 +105,37 @@
         process, note that this is the same that
         ``self.predict(np.array([[300.0]]))[0]``.
 
     reg_ : sklearn.linear_model.LinearRegressor
         The linear regressor for :math:`\ln k` versus :math:`\frac{1}{T}`.
     """
 
-    def __init__(self, constant, **kwargs):
+    def __init__(self, constant=8.617333262e-5):
         self.constant = constant
-        self.reg_ = sklearn.linear_model.LinearRegression(**kwargs)
 
-    def fit(self, X, y, sample_weight=None):
+    def fit(self, X, y, sample_weight=None, **kwargs):
         """Fit the Arrhenius empirical equation.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, 1)
             Temperature data.
 
         y : array-like of shape (n_samples,)
             Target values of the thermally-induced process.
 
         sample_weight : array-like of shape (n_samples,), defualt=None
             Individual weight of each thermally-induced value.
+
+        **kwargs
+            Keyword arguments that are passed and are documented in
+            ``sklearn.linear_model.LinearRegression``.
         """
+        self.reg_ = sklearn.linear_model.LinearRegression(**kwargs)
+
         self._X = 1 / X
         self._y = np.log(y)
         self._sample_weight = (
             sample_weight / y if sample_weight is not None else None
         )
 
         self.reg_.fit(self._X, self._y, self._sample_weight)
@@ -183,34 +183,16 @@
         )
 
         if sample_weight is not None:
             df["weights"] = sample_weight
 
         return df
 
-    @property
-    def plot(self):
-        """Arrhenius plot accessor."""
-        return ArrheniusPlotter(self)
-
-
-class ArrheniusPlotter:
-    """Arrhenius plot.
-
-    Parameters
-    ----------
-    areg : sierras.ArrheniusRegressor
-        An ArrheniusRegressor already fitted.
-    """
-
-    def __init__(self, areg):
-        self.areg = areg
-
-    def arrhenius(self, X, y, ax=None, data_kws=None, pred_kws=None):
-        """Arrhenius plot function.
+    def plot(self, ax=None, data_kws=None, pred_kws=None):
+        """Arrhenius plotter.
 
         Parameters
         ----------
         ax : matplotlib.axes.Axes, default=None
             The current axes.
 
         data_kws : dict, default=None
@@ -232,16 +214,11 @@
         pred_kws = {} if pred_kws is None else pred_kws
 
         for key, value in zip(("marker", "ls", "label"), ("o", "", "data")):
             data_kws.setdefault(key, value)
 
         pred_kws.setdefault("label", "fit")
 
-        ax.errorbar(
-            self.areg._X,
-            self.areg._y,
-            yerr=self.areg._sample_weight,
-            **data_kws,
-        )
-        ax.plot(self.areg._X, self.areg.reg_.predict(self.areg._X), **pred_kws)
+        ax.errorbar(self._X, self._y, yerr=self._sample_weight, **data_kws)
+        ax.plot(self._X, self.reg_.predict(self._X), **pred_kws)
 
         return ax
```


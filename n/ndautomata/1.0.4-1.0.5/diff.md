# Comparing `tmp/ndautomata-1.0.4.tar.gz` & `tmp/ndautomata-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndautomata-1.0.4.tar", last modified: Tue Jan 24 14:55:14 2023, max compression
+gzip compressed data, was "ndautomata-1.0.5.tar", last modified: Wed Jul 12 08:47:38 2023, max compression
```

## Comparing `ndautomata-1.0.4.tar` & `ndautomata-1.0.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:55:14.635943 ndautomata-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:55:14.635943 ndautomata-1.0.4/.devcontainer/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-01-24 14:54:47.000000 ndautomata-1.0.4/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:55:14.631943 ndautomata-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:55:14.635943 ndautomata-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-24 14:54:47.000000 ndautomata-1.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-01-24 14:54:47.000000 ndautomata-1.0.4/.github/workflows/qc-sec.yml
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-01-24 14:54:47.000000 ndautomata-1.0.4/.github/workflows/qc-sty.yml
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-01-24 14:54:47.000000 ndautomata-1.0.4/.github/workflows/qc-uni.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-01-24 14:54:47.000000 ndautomata-1.0.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:55:14.635943 ndautomata-1.0.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-01-24 14:54:47.000000 ndautomata-1.0.4/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-01-24 14:54:47.000000 ndautomata-1.0.4/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-01-24 14:54:47.000000 ndautomata-1.0.4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-24 14:54:47.000000 ndautomata-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-01-24 14:55:14.635943 ndautomata-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17539 2023-01-24 14:54:47.000000 ndautomata-1.0.4/README.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-01-24 14:54:47.000000 ndautomata-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:55:14.635943 ndautomata-1.0.4/README_files/
--rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-01-24 14:54:47.000000 ndautomata-1.0.4/README_files/README_10_0.png
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-01-24 14:54:47.000000 ndautomata-1.0.4/README_files/README_13_0.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     8019 2023-01-24 14:54:47.000000 ndautomata-1.0.4/README_files/ndautomata-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:55:14.635943 ndautomata-1.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    22252 2023-01-24 14:54:47.000000 ndautomata-1.0.4/examples/elementary.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    34745 2023-01-24 14:54:47.000000 ndautomata-1.0.4/examples/gameoflife.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20546 2023-01-24 14:54:47.000000 ndautomata-1.0.4/examples/hexagonal.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19798 2023-01-24 14:54:47.000000 ndautomata-1.0.4/examples/orthogonal.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23248 2023-01-24 14:54:47.000000 ndautomata-1.0.4/examples/ternary.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    26936 2023-01-24 14:54:47.000000 ndautomata-1.0.4/examples/tridimensional.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-01-24 14:54:47.000000 ndautomata-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-24 14:54:47.000000 ndautomata-1.0.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-24 14:54:47.000000 ndautomata-1.0.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-24 14:54:47.000000 ndautomata-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 14:55:14.635943 ndautomata-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:55:14.631943 ndautomata-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:55:14.635943 ndautomata-1.0.4/src/ndautomata/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-24 14:54:47.000000 ndautomata-1.0.4/src/ndautomata/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-01-24 14:54:47.000000 ndautomata-1.0.4/src/ndautomata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-01-24 14:54:47.000000 ndautomata-1.0.4/src/ndautomata/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-01-24 14:54:47.000000 ndautomata-1.0.4/src/ndautomata/neighbours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:55:14.635943 ndautomata-1.0.4/src/ndautomata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-01-24 14:55:14.000000 ndautomata-1.0.4/src/ndautomata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-24 14:55:14.000000 ndautomata-1.0.4/src/ndautomata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 14:55:14.000000 ndautomata-1.0.4/src/ndautomata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-24 14:55:14.000000 ndautomata-1.0.4/src/ndautomata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-24 14:55:14.000000 ndautomata-1.0.4/src/ndautomata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:55:14.635943 ndautomata-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 14:54:47.000000 ndautomata-1.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-01-24 14:54:47.000000 ndautomata-1.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:55:14.635943 ndautomata-1.0.4/tests/test_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-01-24 14:54:47.000000 ndautomata-1.0.4/tests/test_requirements/test_automaton.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-01-24 14:54:47.000000 ndautomata-1.0.4/tests/test_requirements/test_neighbours.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-01-24 14:54:47.000000 ndautomata-1.0.4/tests/test_requirements/test_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 14:55:14.635943 ndautomata-1.0.4/tests/test_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-01-24 14:54:47.000000 ndautomata-1.0.4/tests/test_utilities/test_neighborhoods.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-01-24 14:54:47.000000 ndautomata-1.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:38.959084 ndautomata-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:38.955084 ndautomata-1.0.5/.devcontainer/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-07-12 08:47:27.000000 ndautomata-1.0.5/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:38.951084 ndautomata-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:38.955084 ndautomata-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-12 08:47:27.000000 ndautomata-1.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-12 08:47:27.000000 ndautomata-1.0.5/.github/workflows/qc-sec.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-12 08:47:27.000000 ndautomata-1.0.5/.github/workflows/qc-sty.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-12 08:47:27.000000 ndautomata-1.0.5/.github/workflows/qc-uni.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-12 08:47:27.000000 ndautomata-1.0.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:38.955084 ndautomata-1.0.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-12 08:47:27.000000 ndautomata-1.0.5/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-12 08:47:27.000000 ndautomata-1.0.5/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-12 08:47:27.000000 ndautomata-1.0.5/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 08:47:27.000000 ndautomata-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-12 08:47:38.959084 ndautomata-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17539 2023-07-12 08:47:27.000000 ndautomata-1.0.5/README.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-12 08:47:27.000000 ndautomata-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:38.955084 ndautomata-1.0.5/README_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    13271 2023-07-12 08:47:27.000000 ndautomata-1.0.5/README_files/README_10_0.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-12 08:47:27.000000 ndautomata-1.0.5/README_files/README_13_0.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8019 2023-07-12 08:47:27.000000 ndautomata-1.0.5/README_files/ndautomata-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:38.955084 ndautomata-1.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    22252 2023-07-12 08:47:27.000000 ndautomata-1.0.5/examples/elementary.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    34745 2023-07-12 08:47:27.000000 ndautomata-1.0.5/examples/gameoflife.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20546 2023-07-12 08:47:27.000000 ndautomata-1.0.5/examples/hexagonal.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19798 2023-07-12 08:47:27.000000 ndautomata-1.0.5/examples/orthogonal.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23248 2023-07-12 08:47:27.000000 ndautomata-1.0.5/examples/ternary.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    26936 2023-07-12 08:47:27.000000 ndautomata-1.0.5/examples/tridimensional.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-12 08:47:27.000000 ndautomata-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 08:47:27.000000 ndautomata-1.0.5/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-12 08:47:27.000000 ndautomata-1.0.5/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 08:47:27.000000 ndautomata-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 08:47:38.959084 ndautomata-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:38.951084 ndautomata-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:38.955084 ndautomata-1.0.5/src/ndautomata/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 08:47:27.000000 ndautomata-1.0.5/src/ndautomata/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-12 08:47:27.000000 ndautomata-1.0.5/src/ndautomata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-12 08:47:27.000000 ndautomata-1.0.5/src/ndautomata/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-12 08:47:27.000000 ndautomata-1.0.5/src/ndautomata/neighbours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:38.955084 ndautomata-1.0.5/src/ndautomata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-12 08:47:38.000000 ndautomata-1.0.5/src/ndautomata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-12 08:47:38.000000 ndautomata-1.0.5/src/ndautomata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:47:38.000000 ndautomata-1.0.5/src/ndautomata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 08:47:38.000000 ndautomata-1.0.5/src/ndautomata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 08:47:38.000000 ndautomata-1.0.5/src/ndautomata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:38.959084 ndautomata-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:27.000000 ndautomata-1.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-12 08:47:27.000000 ndautomata-1.0.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:38.959084 ndautomata-1.0.5/tests/test_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-12 08:47:27.000000 ndautomata-1.0.5/tests/test_requirements/test_automaton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-12 08:47:27.000000 ndautomata-1.0.5/tests/test_requirements/test_neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-12 08:47:27.000000 ndautomata-1.0.5/tests/test_requirements/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:47:38.959084 ndautomata-1.0.5/tests/test_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-12 08:47:27.000000 ndautomata-1.0.5/tests/test_utilities/test_neighborhoods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-12 08:47:27.000000 ndautomata-1.0.5/tox.ini
```

### Comparing `ndautomata-1.0.4/.devcontainer/devcontainer.json` & `ndautomata-1.0.5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/.github/workflows/python-publish.yml` & `ndautomata-1.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/.github/workflows/qc-sec.yml` & `ndautomata-1.0.5/.github/workflows/qc-sec.yml`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/.github/workflows/qc-sty.yml` & `ndautomata-1.0.5/.github/workflows/qc-sty.yml`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/.github/workflows/qc-uni.yml` & `ndautomata-1.0.5/.github/workflows/qc-uni.yml`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/.gitignore` & `ndautomata-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/.vscode/launch.json` & `ndautomata-1.0.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/.vscode/settings.json` & `ndautomata-1.0.5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/LICENSE` & `ndautomata-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/PKG-INFO` & `ndautomata-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndautomata
-Version: 1.0.4
+Version: 1.0.5
 Summary: Multidimensional cellular automata in Python.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/BorjaEst/ndautomata/
 Project-URL: Bug Tracker, https://github.com/BorjaEst/ndautomata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `ndautomata-1.0.4/README.ipynb` & `ndautomata-1.0.5/README.ipynb`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/README.md` & `ndautomata-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/README_files/README_10_0.png` & `ndautomata-1.0.5/README_files/README_10_0.png`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/README_files/README_13_0.png` & `ndautomata-1.0.5/README_files/README_13_0.png`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/README_files/ndautomata-logo.png` & `ndautomata-1.0.5/README_files/ndautomata-logo.png`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/examples/elementary.ipynb` & `ndautomata-1.0.5/examples/elementary.ipynb`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/examples/gameoflife.ipynb` & `ndautomata-1.0.5/examples/gameoflife.ipynb`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/examples/hexagonal.ipynb` & `ndautomata-1.0.5/examples/hexagonal.ipynb`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/examples/orthogonal.ipynb` & `ndautomata-1.0.5/examples/orthogonal.ipynb`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/examples/ternary.ipynb` & `ndautomata-1.0.5/examples/ternary.ipynb`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/examples/tridimensional.ipynb` & `ndautomata-1.0.5/examples/tridimensional.ipynb`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/pyproject.toml` & `ndautomata-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/src/ndautomata/__init__.py` & `ndautomata-1.0.5/src/ndautomata/__init__.py`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/src/ndautomata/initializers.py` & `ndautomata-1.0.5/src/ndautomata/initializers.py`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/src/ndautomata/neighbours.py` & `ndautomata-1.0.5/src/ndautomata/neighbours.py`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/src/ndautomata.egg-info/PKG-INFO` & `ndautomata-1.0.5/src/ndautomata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndautomata
-Version: 1.0.4
+Version: 1.0.5
 Summary: Multidimensional cellular automata in Python.
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/BorjaEst/ndautomata/
 Project-URL: Bug Tracker, https://github.com/BorjaEst/ndautomata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `ndautomata-1.0.4/src/ndautomata.egg-info/SOURCES.txt` & `ndautomata-1.0.5/src/ndautomata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/tests/conftest.py` & `ndautomata-1.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/tests/test_requirements/test_automaton.py` & `ndautomata-1.0.5/tests/test_requirements/test_automaton.py`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/tests/test_requirements/test_neighbours.py` & `ndautomata-1.0.5/tests/test_requirements/test_neighbours.py`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/tests/test_requirements/test_values.py` & `ndautomata-1.0.5/tests/test_requirements/test_values.py`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/tests/test_utilities/test_neighborhoods.py` & `ndautomata-1.0.5/tests/test_utilities/test_neighborhoods.py`

 * *Files identical despite different names*

### Comparing `ndautomata-1.0.4/tox.ini` & `ndautomata-1.0.5/tox.ini`

 * *Files identical despite different names*


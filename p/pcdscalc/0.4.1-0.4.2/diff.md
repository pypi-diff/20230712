# Comparing `tmp/pcdscalc-0.4.1.tar.gz` & `tmp/pcdscalc-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcdscalc-0.4.1.tar", last modified: Tue Apr  4 19:25:56 2023, max compression
+gzip compressed data, was "pcdscalc-0.4.2.tar", last modified: Tue Jul 11 22:49:23 2023, max compression
```

## Comparing `pcdscalc-0.4.1.tar` & `pcdscalc-0.4.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)      976 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.github/workflows/standard.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3005 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/conda-recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      796 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     2376 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs/source/be_lens_calcs.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5592 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs/source/pmps.rst
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/pcdscalc/
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-04 19:25:56.000000 pcdscalc-0.4.1/pcdscalc/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    37830 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/be_lens_calcs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2683 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     9458 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     3504 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/diffraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    10268 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/pmps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/pcdscalc/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    19199 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/test_be_lens_calcs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/test_diffraction.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/pcdscalc/tests/test_lens_sets/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/test_lens_sets/lens_set
--rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/tests/test_pmps.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pcdscalc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/pcdscalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-04-04 19:25:56.000000 pcdscalc-0.4.1/pcdscalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1021 2023-04-04 19:25:56.000000 pcdscalc-0.4.1/pcdscalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 19:25:56.000000 pcdscalc-0.4.1/pcdscalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-04-04 19:25:56.000000 pcdscalc-0.4.1/pcdscalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-04 19:25:56.000000 pcdscalc-0.4.1/pcdscalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-04 19:25:41.000000 pcdscalc-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-04 19:25:56.825311 pcdscalc-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 22:49:23.686626 pcdscalc-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      976 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 22:49:23.682626 pcdscalc-0.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 22:49:23.682626 pcdscalc-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3005 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-07-11 22:49:23.686626 pcdscalc-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 22:49:23.682626 pcdscalc-0.4.2/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 22:49:23.682626 pcdscalc-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      796 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 22:49:23.682626 pcdscalc-0.4.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     2376 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/docs/source/be_lens_calcs.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5592 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/docs/source/pmps.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 22:49:23.682626 pcdscalc-0.4.2/pcdscalc/
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-07-11 22:49:23.000000 pcdscalc-0.4.2/pcdscalc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37830 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/be_lens_calcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2683 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9458 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3504 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/diffraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10268 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/pmps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 22:49:23.682626 pcdscalc-0.4.2/pcdscalc/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19199 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/tests/test_be_lens_calcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/tests/test_diffraction.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 22:49:23.682626 pcdscalc-0.4.2/pcdscalc/tests/test_lens_sets/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/tests/test_lens_sets/lens_set
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/tests/test_pmps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pcdscalc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 22:49:23.682626 pcdscalc-0.4.2/pcdscalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-07-11 22:49:23.000000 pcdscalc-0.4.2/pcdscalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1021 2023-07-11 22:49:23.000000 pcdscalc-0.4.2/pcdscalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 22:49:23.000000 pcdscalc-0.4.2/pcdscalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-07-11 22:49:23.000000 pcdscalc-0.4.2/pcdscalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-11 22:49:23.000000 pcdscalc-0.4.2/pcdscalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-11 22:49:06.000000 pcdscalc-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 22:49:23.686626 pcdscalc-0.4.2/setup.cfg
```

### Comparing `pcdscalc-0.4.1/.flake8` & `pcdscalc-0.4.2/.flake8`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/.github/ISSUE_TEMPLATE.md` & `pcdscalc-0.4.2/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/.github/PULL_REQUEST_TEMPLATE.md` & `pcdscalc-0.4.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/.github/workflows/standard.yml` & `pcdscalc-0.4.2/.github/workflows/standard.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
   release:
     types:
       - published
 
 jobs:
   standard:
     uses: pcdshub/pcds-ci-helpers/.github/workflows/python-standard.yml@master
+    secrets: inherit
     with:
       # The workflow needs to know the package name.  This can be determined
       # automatically if the repository name is the same as the import name.
       package-name: "pcdscalc"
       # Extras that will be installed for both conda/pip:
       testing-extras: ""
       # Extras to be installed only for conda-based testing:
```

### Comparing `pcdscalc-0.4.1/.gitignore` & `pcdscalc-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/.pre-commit-config.yaml` & `pcdscalc-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/CONTRIBUTING.rst` & `pcdscalc-0.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/LICENSE` & `pcdscalc-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/PKG-INFO` & `pcdscalc-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdscalc
-Version: 0.4.1
+Version: 0.4.2
 Summary: PCDS Calculation Routines
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -45,15 +45,15 @@
         
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: test
-Provides-Extra: docs
+Provides-Extra: doc
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===============================
 pcdscalc
 ===============================
```

### Comparing `pcdscalc-0.4.1/README.rst` & `pcdscalc-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/conda-recipe/meta.yaml` & `pcdscalc-0.4.2/conda-recipe/meta.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -19,16 +19,15 @@
   - python >=3.9
   - setuptools_scm
   - pip
   run:
   - python >=3.9
   - numpy
   - scipy
-  - sqlalchemy <2.0
-  - xraydb <4.5.0
+  - xraydb
 
 test:
   imports:
   - pcdscalc
   requires:
   - pytest
```

### Comparing `pcdscalc-0.4.1/docs/Makefile` & `pcdscalc-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/docs/make.bat` & `pcdscalc-0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/docs/source/be_lens_calcs.rst` & `pcdscalc-0.4.2/docs/source/be_lens_calcs.rst`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/docs/source/conf.py` & `pcdscalc-0.4.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/docs/source/index.rst` & `pcdscalc-0.4.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/pcdscalc/be_lens_calcs.py` & `pcdscalc-0.4.2/pcdscalc/be_lens_calcs.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/pcdscalc/common.py` & `pcdscalc-0.4.2/pcdscalc/common.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/pcdscalc/constants.py` & `pcdscalc-0.4.2/pcdscalc/constants.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/pcdscalc/diffraction.py` & `pcdscalc-0.4.2/pcdscalc/diffraction.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/pcdscalc/pmps.py` & `pcdscalc-0.4.2/pcdscalc/pmps.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/pcdscalc/tests/test_be_lens_calcs.py` & `pcdscalc-0.4.2/pcdscalc/tests/test_be_lens_calcs.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/pcdscalc/tests/test_common.py` & `pcdscalc-0.4.2/pcdscalc/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/pcdscalc/tests/test_diffraction.py` & `pcdscalc-0.4.2/pcdscalc/tests/test_diffraction.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/pcdscalc/tests/test_pmps.py` & `pcdscalc-0.4.2/pcdscalc/tests/test_pmps.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/pcdscalc/version.py` & `pcdscalc-0.4.2/pcdscalc/version.py`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/pcdscalc.egg-info/PKG-INFO` & `pcdscalc-0.4.2/pcdscalc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcdscalc
-Version: 0.4.1
+Version: 0.4.2
 Summary: PCDS Calculation Routines
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -45,15 +45,15 @@
         
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: test
-Provides-Extra: docs
+Provides-Extra: doc
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===============================
 pcdscalc
 ===============================
```

### Comparing `pcdscalc-0.4.1/pcdscalc.egg-info/SOURCES.txt` & `pcdscalc-0.4.2/pcdscalc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcdscalc-0.4.1/pyproject.toml` & `pcdscalc-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,9 +32,9 @@
 
 [tool.setuptools.dynamic.dependencies]
 file = [ "requirements.txt",]
 
 [tool.setuptools.dynamic.optional-dependencies.test]
 file = "dev-requirements.txt"
 
-[tool.setuptools.dynamic.optional-dependencies.docs]
+[tool.setuptools.dynamic.optional-dependencies.doc]
 file = "docs-requirements.txt"
```


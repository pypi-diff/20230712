# Comparing `tmp/seaduck-0.1.2.tar.gz` & `tmp/seaduck-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaduck-0.1.2.tar", last modified: Wed May 24 18:15:12 2023, max compression
+gzip compressed data, was "seaduck-0.1.3.tar", last modified: Wed Jul 12 03:28:50 2023, max compression
```

## Comparing `seaduck-0.1.2.tar` & `seaduck-0.1.3.tar`

### file list

```diff
@@ -1,80 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.265813 seaduck-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.257813 seaduck-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-24 18:14:57.000000 seaduck-0.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.257813 seaduck-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-24 18:14:57.000000 seaduck-0.1.2/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-24 18:14:57.000000 seaduck-0.1.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-24 18:14:57.000000 seaduck-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-24 18:14:57.000000 seaduck-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-24 18:14:57.000000 seaduck-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-24 18:14:57.000000 seaduck-0.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-24 18:15:12.265813 seaduck-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-24 18:14:57.000000 seaduck-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.257813 seaduck-0.1.2/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-24 18:14:57.000000 seaduck-0.1.2/ci/environment-ci.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.257813 seaduck-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/AVISO.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/Global_ECCO.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/all_in_one.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.257813 seaduck-0.1.2/docs/api_reference/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_OceData.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_OceInterp.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_eulerian.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_getmasks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_kernelNweight.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_lagrangian.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_smartread.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_topology.rst
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/api_reference/apiref_utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.261813 seaduck-0.1.2/docs/contribute/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/contribute/contr_cod.md
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/contribute/contr_doc.md
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/contribute/prep_env.md
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/contribute/tidyNpr.md
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/contribute/use_git.md
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/how_to_install.md
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)   577233 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/network_of_object.md
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/notebooks.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/reference.md
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.261813 seaduck-0.1.2/docs/sciserver_notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-24 18:14:57.000000 seaduck-0.1.2/docs/sciserver_notebooks/IGP.md
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-24 18:14:57.000000 seaduck-0.1.2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-24 18:14:57.000000 seaduck-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.261813 seaduck-0.1.2/seaduck/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48174 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/eulerian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/get_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    28319 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/kernel_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)    37779 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/lagrangian.py
--rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/ocedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/oceinterp.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/runtime_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/smart_read.py
--rw-r--r--   0 runner    (1001) docker     (123)    23085 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/topology.py
--rw-r--r--   0 runner    (1001) docker     (123)    21854 2023-05-24 18:14:57.000000 seaduck-0.1.2/seaduck/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 18:15:12.000000 seaduck-0.1.2/seaduck/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.261813 seaduck-0.1.2/seaduck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-24 18:15:12.000000 seaduck-0.1.2/seaduck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-24 18:15:12.000000 seaduck-0.1.2/seaduck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:15:12.000000 seaduck-0.1.2/seaduck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 18:15:12.000000 seaduck-0.1.2/seaduck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 18:15:12.000000 seaduck-0.1.2/seaduck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 18:15:12.265813 seaduck-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:15:12.265813 seaduck-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_eulerian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_get_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_lagrangian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_ocedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_oceinterp.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_smart_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_topology.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-24 18:14:57.000000 seaduck-0.1.2/tests/test_weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:50.518759 seaduck-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:50.510759 seaduck-0.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-12 03:28:35.000000 seaduck-0.1.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:50.510759 seaduck-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-12 03:28:35.000000 seaduck-0.1.3/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-12 03:28:35.000000 seaduck-0.1.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-12 03:28:35.000000 seaduck-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-12 03:28:35.000000 seaduck-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-12 03:28:35.000000 seaduck-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-12 03:28:35.000000 seaduck-0.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    15038 2023-07-12 03:28:50.518759 seaduck-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-12 03:28:35.000000 seaduck-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:50.510759 seaduck-0.1.3/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-12 03:28:35.000000 seaduck-0.1.3/ci/environment-ci.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:50.510759 seaduck-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:50.510759 seaduck-0.1.3/docs/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/api_reference/apiref_OceData.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/api_reference/apiref_OceInterp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/api_reference/apiref_RelCoord.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/api_reference/apiref_eulerian.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/api_reference/apiref_getmasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/api_reference/apiref_kernelNweight.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/api_reference/apiref_lagrangian.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/api_reference/apiref_smartread.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/api_reference/apiref_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/api_reference/apiref_utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/api_reference.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:50.514759 seaduck-0.1.3/docs/contribute/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/contribute/contr_cod.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/contribute/contr_doc.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/contribute/prep_env.md
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/contribute/tidyNpr.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/contribute/use_git.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/get_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/guide_for_developer.md
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/how_to_install.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/ideal_test.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:50.514759 seaduck-0.1.3/docs/idealize_test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10787 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/idealize_test/hor_stream.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/idealize_test/tilted_stream.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/idealize_test/ver_stream.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)   577233 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/network_of_object.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:50.514759 seaduck-0.1.3/docs/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)    18389 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/notebook/AVISO.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/notebook/global_ECCO.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/notebook/topology_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/ocean_example.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/one_min_guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/sciserver_example.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:50.514759 seaduck-0.1.3/docs/sciserver_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/sciserver_notebooks/ECCO_plot_stations.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/sciserver_notebooks/IGPwinter.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/sciserver_notebooks/KangerFjord.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-12 03:28:35.000000 seaduck-0.1.3/docs/sciserver_notebooks/LLC4320.md
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-12 03:28:35.000000 seaduck-0.1.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-12 03:28:35.000000 seaduck-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:50.514759 seaduck-0.1.3/seaduck/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-12 03:28:35.000000 seaduck-0.1.3/seaduck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47934 2023-07-12 03:28:35.000000 seaduck-0.1.3/seaduck/eulerian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-12 03:28:35.000000 seaduck-0.1.3/seaduck/get_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28583 2023-07-12 03:28:35.000000 seaduck-0.1.3/seaduck/kernel_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36159 2023-07-12 03:28:35.000000 seaduck-0.1.3/seaduck/lagrangian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15868 2023-07-12 03:28:35.000000 seaduck-0.1.3/seaduck/ocedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-12 03:28:35.000000 seaduck-0.1.3/seaduck/oceinterp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-12 03:28:35.000000 seaduck-0.1.3/seaduck/runtime_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-12 03:28:35.000000 seaduck-0.1.3/seaduck/smart_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24423 2023-07-12 03:28:35.000000 seaduck-0.1.3/seaduck/topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-07-12 03:28:35.000000 seaduck-0.1.3/seaduck/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 03:28:50.000000 seaduck-0.1.3/seaduck/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:50.514759 seaduck-0.1.3/seaduck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15038 2023-07-12 03:28:50.000000 seaduck-0.1.3/seaduck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-12 03:28:50.000000 seaduck-0.1.3/seaduck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:28:50.000000 seaduck-0.1.3/seaduck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 03:28:50.000000 seaduck-0.1.3/seaduck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 03:28:50.000000 seaduck-0.1.3/seaduck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 03:28:50.518759 seaduck-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:50.518759 seaduck-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 03:28:35.000000 seaduck-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-12 03:28:35.000000 seaduck-0.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-07-12 03:28:35.000000 seaduck-0.1.3/tests/test_eulerian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-12 03:28:35.000000 seaduck-0.1.3/tests/test_get_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-07-12 03:28:35.000000 seaduck-0.1.3/tests/test_lagrangian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-12 03:28:35.000000 seaduck-0.1.3/tests/test_ocedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-12 03:28:35.000000 seaduck-0.1.3/tests/test_oceinterp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-07-12 03:28:35.000000 seaduck-0.1.3/tests/test_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-12 03:28:35.000000 seaduck-0.1.3/tests/test_smart_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-12 03:28:35.000000 seaduck-0.1.3/tests/test_streamfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-07-12 03:28:35.000000 seaduck-0.1.3/tests/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-12 03:28:35.000000 seaduck-0.1.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-12 03:28:35.000000 seaduck-0.1.3/tests/test_weight.py
```

### Comparing `seaduck-0.1.2/.github/workflows/on-push.yml` & `seaduck-0.1.3/.github/workflows/on-push.yml`

 * *Files 6% similar despite different names*

```diff
@@ -15,23 +15,14 @@
   cancel-in-progress: true
 
 defaults:
   run:
     shell: bash -l {0}
 
 jobs:
-  pre-commit:
-    runs-on: ubuntu-latest
-    steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
-      with:
-        python-version: 3.x
-    - uses: pre-commit/action@v3.0.0
-
   combine-environments:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
     - name: Install conda-merge
       run: |
@@ -47,58 +38,60 @@
 
   unit-tests:
     name: unit-tests
     needs: combine-environments
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ["3.9", "3.11"]
+        optional-dependencies: ["", "numba"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Download combined environments
       uses: actions/download-artifact@v3
       with:
         name: combined-environments
         path: ci
     - name: Install Conda environment with Micromamba
-      uses: mamba-org/provision-with-micromamba@v15
+      uses: mamba-org/setup-micromamba@v1
       with:
         environment-file: ci/combined-environment-ci.yml
         environment-name: DEVELOP
-        channels: conda-forge
-        cache-env: true
-        extra-specs: |
+        cache-environment: true
+        create-args: >-
           python=${{ matrix.python-version }}
+          ${{ matrix.optional-dependencies }}
     - name: Install package
       run: |
         python -m pip install --no-deps -e .
     - name: Run tests
       run: |
         make unit-tests COV_REPORT=xml
+    - name: Upload coverage reports to Codecov
+      uses: codecov/codecov-action@v3
 
   type-check:
     needs: [combine-environments, unit-tests]
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
     - name: Download combined environments
       uses: actions/download-artifact@v3
       with:
         name: combined-environments
         path: ci
     - name: Install Conda environment with Micromamba
-      uses: mamba-org/provision-with-micromamba@v15
+      uses: mamba-org/setup-micromamba@v1
       with:
         environment-file: ci/combined-environment-ci.yml
         environment-name: DEVELOP
-        channels: conda-forge
-        cache-env: true
-        extra-specs: |
+        cache-environment: true
+        create-args: >-
           python=3.11
     - name: Install package
       run: |
         python -m pip install --no-deps -e .
     - name: Run code quality checks
       run: |
         make type-check
@@ -111,21 +104,20 @@
     - uses: actions/checkout@v3
     - name: Download combined environments
       uses: actions/download-artifact@v3
       with:
         name: combined-environments
         path: ci
     - name: Install Conda environment with Micromamba
-      uses: mamba-org/provision-with-micromamba@v15
+      uses: mamba-org/setup-micromamba@v1
       with:
         environment-file: ci/combined-environment-ci.yml
         environment-name: DEVELOP
-        channels: conda-forge
-        cache-env: true
-        extra-specs: |
+        cache-environment: true
+        create-args: >-
           python=3.11
     - name: Install package
       run: |
         python -m pip install --no-deps -e .
     - name: Build documentation
       run: |
         make docs-build
```

### Comparing `seaduck-0.1.2/.github/workflows/pypi.yml` & `seaduck-0.1.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `seaduck-0.1.2/.gitignore` & `seaduck-0.1.3/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -342,14 +342,15 @@
 .ionide
 
 # Ignore code-workspaces
 *.code-workspace
 
 # User Defined
 test*.ipynb
+PleaseIgnore*
 *.npy
 *.jpg
 .vscode/
 tests/Data
 tests/testDat*
 assets/
 *.pyc
```

### Comparing `seaduck-0.1.2/LICENSE` & `seaduck-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seaduck-0.1.2/PKG-INFO` & `seaduck-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaduck
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package that interpolates data from ocean dataset from both Eulerian and Lagrangian perspective. 
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -220,25 +220,30 @@
 # seaduck
 
 A python package that interpolates data from ocean dataset from both Eulerian and Lagrangian perspective.
 
 ## Quick Start
 
 ```python
->>> import seaduck
+>>> import seaduck as sd
 
 ```
 
+## Documentation
+
+Checkout this half-way-through documentation:
+https://macekuailv.github.io/seaduck/
+
 ## Workflow for developers/contributors
 
-For best experience create a new conda environment (e.g. seaduck):
+For best experience create a new conda environment (e.g. bubblebath):
 
 ```
-conda create -n seaduck
-conda activate seaduck
+conda create -n bubblebath
+conda activate bubblebath
 ```
 
 Before pushing to GitHub, run the following commands:
 
 1. Update conda environment: `make conda-env-update`
 1. Install this package: `pip install -e .`
 1. Run quality assurance checks: `make qa`
```

### Comparing `seaduck-0.1.2/README.md` & `seaduck-0.1.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # seaduck
 
 A python package that interpolates data from ocean dataset from both Eulerian and Lagrangian perspective.
 
 ## Quick Start
 
 ```python
->>> import seaduck
+>>> import seaduck as sd
 
 ```
 
+## Documentation
+
+Checkout this half-way-through documentation:
+https://macekuailv.github.io/seaduck/
+
 ## Workflow for developers/contributors
 
-For best experience create a new conda environment (e.g. seaduck):
+For best experience create a new conda environment (e.g. bubblebath):
 
 ```
-conda create -n seaduck
-conda activate seaduck
+conda create -n bubblebath
+conda activate bubblebath
 ```
 
 Before pushing to GitHub, run the following commands:
 
 1. Update conda environment: `make conda-env-update`
 1. Install this package: `pip install -e .`
 1. Run quality assurance checks: `make qa`
```

### Comparing `seaduck-0.1.2/docs/AVISO.ipynb` & `seaduck-0.1.3/docs/idealize_test/hor_stream.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7672554399637732%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Horizontal stream function conservation\\n'), (2, "*

 * *            "'author, Wenrui Jiang 06/06/2022\\n'), (4, 'This package currently only supports "*

 * *            'velocity fields that are piecewise stationary in time. For a stable velocity field, '*

 * *            "the streaklines will match the streamlines of the field.\\n'), (5, '\\n'), (6, 'For "*

 * *            "2D cases, this means conservation of stream function.')], delete: [4, 2, 0]}, "*

 * *            "'attachments':  […]*

```diff
@@ -1,411 +1,430 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "c6c93715",
             "metadata": {},
             "source": [
-                "# Lagrangian particle demonstration in a periodic domain.\n",
+                "# Horizontal stream function conservation\n",
                 "\n",
-                "**Particles are simulated in the Southern Ocean AVISO altimetrey velocity field.**\n",
+                "author, Wenrui Jiang 06/06/2022\n",
                 "\n",
-                "Author: Wenrui Jiang, Tom Haine Feb '23"
+                "This package currently only supports velocity fields that are piecewise stationary in time. For a stable velocity field, the streaklines will match the streamlines of the field.\n",
+                "\n",
+                "For 2D cases, this means conservation of stream function."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "c63f1559",
+            "attachments": {},
+            "cell_type": "markdown",
             "metadata": {
-                "tags": []
+                "tags": [
+                    "mdformat-skip"
+                ]
             },
-            "outputs": [],
             "source": [
-                "import cartopy.crs as ccrs\n",
-                "import matplotlib.pyplot as plt\n",
-                "import numpy as np\n",
-                "\n",
-                "import seaduck as sd"
+                "$$\n",
+                "\\frac{d \\Psi}{dt} = 0\n",
+                "$$"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "256affe3",
             "metadata": {},
             "source": [
-                "### Loading data\n",
-                "\n",
-                "The AVISO velocity field dataset is a lat-lon grid with staggered velocity. It's a snapshot from a single time (see below). `seaduck.utils` provides a few datasets for testing and demonstration purposes. The corresponding dataset are called when the corresponding functions are called."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "906f5971",
-            "metadata": {},
-            "source": [
-                "<div class=\"alert alert-block alert-warning\">\n",
-                "<b>Download:</b> If you are running this notebook for the first time, The dataset needs to be downloaded and cached, which can be a little slow.\n",
-                "</div>"
+                "A strong test can be constructed as follows: **simulate the particles under an arbitrary stream function and compare the stream function before-and-after**. If the code is correct, the stream function defined at the starting position of a particle should match that defined at the final position."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c670efe2",
             "metadata": {
-                "tags": []
+                "tags": [
+                    "hide-input"
+                ]
             },
             "outputs": [],
             "source": [
-                "ds = sd.utils.get_dataset(\"aviso\")\n",
-                "ds"
+                "import warnings\n",
+                "\n",
+                "import matplotlib as mpl\n",
+                "import matplotlib.pyplot as plt\n",
+                "import numpy as np\n",
+                "import pooch\n",
+                "import xarray as xr\n",
+                "from matplotlib import cm, colors\n",
+                "\n",
+                "import seaduck as sd\n",
+                "\n",
+                "mpl.rcParams[\"figure.dpi\"] = 300\n",
+                "\n",
+                "warnings.filterwarnings(\"ignore\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "e2300abc",
             "metadata": {},
             "source": [
-                "Now, create the `OceData` object which provides methods to translate between lat-lon and grid-oriented coords. The model coords frequently needed are also cached. "
+                "## Loading data\n",
+                "\n",
+                "For this test example, the stream function we are going to use is an award-winning eddy in the arbitrary/cute department. Let's load it."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "528f9f42",
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "bathtub = sd.OceData(ds)"
+                "file_path = pooch.retrieve(\n",
+                "    url=\"https://github.com/MaceKuailv/seaduck_sciserver_notebook/raw/master/diffused_duck.npy\",\n",
+                "    known_hash=\"8968fc89a57a492879dff6b458ffa1e03bb533e82bd76ca5db8496182fa2c32f\",\n",
+                ")\n",
+                "\n",
+                "strmf = np.load(file_path)[::-1]\n",
+                "M, N = strmf.shape\n",
+                "M -= 1\n",
+                "N -= 1\n",
+                "x = np.linspace(-1, 1, N + 1)\n",
+                "y = np.linspace(-1, 1, M + 1)\n",
+                "xg, yg = np.meshgrid(x, y)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "c1f84484",
             "metadata": {},
             "source": [
-                "The object also contains a `tp` (topology) object. It looks at the shape of the coordinate data. In this case, based on longitude range, it thinks the type is `x_periodic`, which is correct for the Southern Ocean."
+                "To show that I am not volkswagening you, I will plot the stream function."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "08e23745",
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "bathtub.tp.typ"
+                "plt.pcolormesh(xg, yg, strmf, cmap=\"Oranges\")\n",
+                "plt.gca().set_aspect(\"equal\")\n",
+                "plt.xlabel(\"X\")\n",
+                "plt.ylabel(\"Y\")\n",
+                "plt.title(\"Stream function of a very arbitrary eddy\")\n",
+                "plt.show()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "fd56bcf1",
             "metadata": {},
             "source": [
-                "We've prepared the bathtub that the ducks are going to swim (passively drift) in. Now decide where and when to drop them. \n",
-                "\n",
-                "We are going to use a short-hand defined in `seaduck.utils` to define the initial position for simplicity. The returns are normal than four 1D `numpy` array of `lon, lat, dep`, and `time`. It is as simple as that."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "4c4a6f6a",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "# Define the extend of the box\n",
-                "west = -180.0\n",
-                "east = 180.0\n",
-                "south = -75.0\n",
-                "north = -40.0\n",
-                "shallow = -10.0\n",
-                "deep = -10.0\n",
-                "\n",
-                "time = \"1970-01-01\"\n",
-                "\n",
-                "Nlon = 300  # How many along longitudinal direction?\n",
-                "Nlat = 30  # How many along latitudinal direction?\n",
-                "Ndep = 1  # How many along vertical direction?\n",
-                "\n",
-                "x, y, z, t = sd.utils.easy_3d_cube(\n",
-                "    (west, east, Nlon),\n",
-                "    (south, north, Nlat),\n",
-                "    (shallow, deep, Ndep),\n",
-                "    time,\n",
-                "    print_total_number=True,\n",
-                ")"
+                "**Fig.1** A stream function that is not particular in any senses."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "cd57d0a6",
             "metadata": {},
             "source": [
-                "**Here is where the particles start on the map:**"
+                "Now we prepare create the grids needed and therefore the xarray dataset for the simulation."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5c150e21",
             "metadata": {
-                "tags": []
+                "tags": [
+                    "hide-input"
+                ]
             },
             "outputs": [],
             "source": [
-                "plt.figure(figsize=(15, 6))\n",
-                "ax = plt.axes(projection=ccrs.PlateCarree(central_longitude=170.0))\n",
-                "ax.plot(x, y, \"r+\", markersize=1, transform=ccrs.PlateCarree())\n",
-                "ax.coastlines()\n",
-                "plt.show()"
+                "xv = 0.5 * (xg[:, 1:] + xg[:, :-1])\n",
+                "yv = 0.5 * (yg[:, 1:] + yg[:, :-1])\n",
+                "xu = 0.5 * (xg[1:] + xg[:-1])\n",
+                "yu = 0.5 * (yg[1:] + yg[:-1])\n",
+                "\n",
+                "xc = 0.5 * (xv[1:] + xv[:-1])\n",
+                "yc = 0.5 * (yv[1:] + yv[:-1])"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "604c2561",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "The AVISO velocity data only has the horizontal velocity component. Or in other words, all the particles are assume to be at the same (implicit) level, which is the surface for this example. `seaduck` takes care of that by just setting:"
+                "u = np.diff(strmf, axis=0)\n",
+                "v = -np.diff(strmf, axis=1)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c64e79be",
             "metadata": {
-                "tags": []
+                "tags": [
+                    "hide-input"
+                ]
             },
             "outputs": [],
             "source": [
-                "z = None"
+                "ds = xr.Dataset(\n",
+                "    coords=dict(\n",
+                "        XC=([\"Y\", \"X\"], xc),\n",
+                "        YC=([\"Y\", \"X\"], yc),\n",
+                "        XG=([\"Yp1\", \"Xp1\"], xg),\n",
+                "        YG=([\"Yp1\", \"Xp1\"], yg),\n",
+                "        rA=([\"Y\", \"X\"], np.ones_like(xc, float)),\n",
+                "    ),\n",
+                "    data_vars=dict(\n",
+                "        UVELMASS=([\"Y\", \"Xp1\"], u),\n",
+                "        VVELMASS=([\"Yp1\", \"X\"], v),\n",
+                "        streamfunc=([\"Yp1\", \"Xp1\"], strmf),\n",
+                "    ),\n",
+                ")\n",
+                "ds"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "1cbcc5c9",
             "metadata": {},
             "source": [
-                "The AVISO velocity field is a snapshot and does not have a time dimension. Therefore, the time is only valid in a relative sense, i.e. how long has the simulation gone in \"real\" time.\n",
+                "## Prepare for the test\n",
                 "\n",
-                "The standard format for time in `seaduck` is seconds since `1970-01-01 00:00` and could be negative. Remember what time is set as the initial time?"
+                "First, we create the `seaduck.OceData` object"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "73e5e169",
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "all(t == 0)"
+                "tub = sd.OceData(ds)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "c164519e",
             "metadata": {},
             "source": [
-                "Let's now define the duration of the simulation (end before start means integrate backwards in time). We can again use a short hand from `seaduck.utils`."
+                "Then, initialize the particle position."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8421fbba",
             "metadata": {},
             "outputs": [],
             "source": [
-                "tf = sd.utils.convert_time(\"1970-02-01\")"
+                "num_particle = 8000\n",
+                "np.random.seed(99)\n",
+                "x = np.random.random(num_particle) * 1.6 - 0.8\n",
+                "y = np.random.random(num_particle) * 1.8 - 0.9"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "9658dc2a",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "This is equivalent to:"
-            ]
-        },
-        {
-            "cell_type": "raw",
-            "id": "9b874e11",
-            "metadata": {
-                "tags": []
-            },
-            "source": [
-                "tf = (np.datetime64(\"1970-02-01\") - np.datetime64(\"1970-01-01\")) / np.timedelta64(\n",
-                "    1, \"s\"\n",
+                "pt = sd.Particle(\n",
+                "    x=x, y=y, z=None, t=np.zeros_like(x), data=tub, wname=None, transport=True\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "72f67743",
             "metadata": {},
             "source": [
-                "We are only interested when the particle is still in the domain, we can disregard the ones left from the northern boundary by defining:"
+                "Finally, we need a proper kernel for interpolating stream function. The natural definition for this case is to interpolate using the four closest corner points."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "60649e82",
             "metadata": {},
             "outputs": [],
             "source": [
-                "def interested_in(p):\n",
-                "    return np.logical_and(-74.5 < p.lat, p.lat < -45.5)"
+                "kkk = np.array([[0, 0], [0, 1], [1, 0], [1, 1]])\n",
+                "\n",
+                "gknw = sd.KnW(kkk, vkernel=\"nearest\", tkernel=\"nearest\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "907e4756",
             "metadata": {},
             "source": [
-                "### Now create the `OceInterp.lagrangian.particle` object.\n",
+                "## The actual test\n",
                 "\n",
-                "We have all the information we need. The final step of preparation is to create the `seaduck.lagrangian.particle` object. We need to tell the `seaduck` where, when, which bathtub, as well as the name of the velocity components, because they are not great at guessing."
+                "First we interpolate the streamfunction at the starting position."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "124718ad",
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "p = sd.particle(\n",
-                "    x=x,\n",
-                "    y=y,\n",
-                "    z=z,\n",
-                "    t=t,\n",
-                "    data=bathtub,\n",
-                "    uname=\"u\",\n",
-                "    vname=\"v\",\n",
-                "    wname=None,\n",
-                "    callback=interested_in,\n",
-                ")\n",
-                "p"
+                "before = pt.interpolate(\"streamfunc\", gknw)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "974b3cda",
             "metadata": {},
             "source": [
-                "### Perform the particle trajectory simulation.\n",
-                "\n",
-                "Notice how we define when to dump output (`normal_stops`) and when to update the velocity field (`update_stops`). By default, the `stops` returned by the integration is the combination (union) of `normal_stops` and `update_stops`. `raw` is a list of `OceInterp.eulerian.position` objects with the same length as `stops`."
+                "Now, simulate the particles forward for a decent amount of time."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6d8ee9cc",
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "normal_stops = np.linspace(t[0], tf, 10)\n",
-                "stops, raw = p.to_list_of_time(normal_stops=normal_stops, update_stops=[])"
+                "steps = 15\n",
+                "stops, ps = pt.to_list_of_time(\n",
+                "    normal_stops=np.linspace(0, 2 * steps * N, steps), update_stops=[]\n",
+                ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "e3866e40",
             "metadata": {},
             "source": [
-                "### Extract the information from the position objects."
+                "Now that, the particles are at a different position. Let's look at the stream functions again and compare."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "after = ps[-1].interpolate(\"streamfunc\", gknw)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "25f862a7",
             "metadata": {
-                "tags": []
+                "tags": [
+                    "hide-input"
+                ]
             },
             "outputs": [],
             "source": [
-                "lons = np.array([pt.lon for pt in raw]).T\n",
-                "lats = np.array([pt.lat for pt in raw]).T"
+                "is_it_close = np.allclose(after, before, atol=1e-7)\n",
+                "max_difference = np.max(np.abs(after - before))\n",
+                "print(f\"Is the stream function conserved? {is_it_close}\")\n",
+                "print(f\"The maximum difference is {max_difference }\")"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "To put that in perspective: The stream function ranges from 0 to around 0.6. So this is a small difference!"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "0e8b0f78",
             "metadata": {},
             "source": [
-                "Some particles passed through the dateline (periodic boundary). Here is some pre-processing to handle the plot."
+                "## If you're not convinced\n",
+                "\n",
+                "\"Hey, you just used your own function to test another function. I didn't see anything under the hood. \"\n",
+                "\"Also, the stream function should be conserved along the **entire trajectory**. Not only the start and the end\"\n",
+                "\n",
+                "Well, here is a more visual way of proving my points.\n",
+                "\n",
+                "I am going to plot the trajectory of all the particles, and color them using the **initial** stream function.\n",
+                "\n",
+                "If the stream function is not conserved at any point, the color of the lines drawn (initial value of stream function) will not match that we plotted earlier (the actual value defined at that point)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0e0fc0c8",
             "metadata": {
-                "tags": []
+                "tags": [
+                    "hide-input"
+                ]
             },
             "outputs": [],
             "source": [
-                "for i in range(len(lons)):\n",
-                "    diff = np.diff(lons[i])\n",
-                "\n",
-                "    if max(abs(diff)) > 330:\n",
-                "        for j in np.where(abs(diff) > 300)[0]:\n",
-                "            j = int(j)\n",
-                "            lons[i, j + 1 :] -= np.sign(diff[j]) * 360"
+                "lons = []\n",
+                "lats = []\n",
+                "for ppp in ps:\n",
+                "    lons.append(ppp.lon)\n",
+                "    lats.append(ppp.lat)\n",
+                "lons = np.array(lons)\n",
+                "lats = np.array(lats)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "c7046590",
             "metadata": {},
             "source": [
-                "## Here are the trajectories:"
+                "Using the same color scheme as the previous plot"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5338b2f2",
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "plt.figure(figsize=(24, 6))\n",
-                "ax = plt.axes(projection=ccrs.PlateCarree(central_longitude=170.0))\n",
-                "ax.plot(lons.T, lats.T, \"darkblue\", lw=0.3, transform=ccrs.PlateCarree())\n",
-                "ax.coastlines()"
+                "norm = colors.Normalize(vmin=0.0, vmax=0.6, clip=True)\n",
+                "mapper = cm.ScalarMappable(norm=norm, cmap=cm.Oranges)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f5516722",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-input"
+                ]
+            },
             "outputs": [],
-            "source": []
+            "source": [
+                "for i in range(len(x)):\n",
+                "    plt.plot(lons.T[i], lats.T[i], c=mapper.to_rgba(before[i]), lw=0.55)\n",
+                "plt.gca().set_aspect(\"equal\")\n",
+                "plt.xlim([-1, 1])\n",
+                "plt.ylim([-1, 1])\n",
+                "plt.xlabel(\"X\")\n",
+                "plt.ylabel(\"Y\")\n",
+                "plt.title(\"Streamline of particles advected by the very arbitrary eddy\")\n",
+                "plt.show()"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "**Fig.1** The trajectories of particles advected by the very arbitrary eddy. The color denotes the initial value of stream function."
+            ]
         }
     ],
     "metadata": {
+        "celltoolbar": "Tags",
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
@@ -413,13 +432,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.11.4"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 4
 }
```

### Comparing `seaduck-0.1.2/docs/Global_ECCO.ipynb` & `seaduck-0.1.3/docs/notebook/global_ECCO.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9294047509062753%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Use `seaduck.OceInterp` with ECCO\\n'), (2, "*

 * *            "'`seaduck` Lagrangian particle demonstration. This version uses a reduced version of "*

 * *            "the ECCO MITgcm velocity field data.\\n')], delete: [2, 0]}}, 1: {'metadata': "*

 * *            "{replace: OrderedDict([('tags', ['hide-input'])])}, 'source': {insert: [(1, 'import "*

 * *            "matplotlib as mpl\\n'), (5, 'import seaduck as sd\\n'), (6, '\\n'), (7, "*

 * *            '\'mpl.rcParams["figure.dpi"]  […]*

```diff
@@ -1,204 +1,169 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Lagrangian and Eulerian demonstration on ECCO\n",
+                "# Use `seaduck.OceInterp` with ECCO\n",
                 "\n",
-                "`seaduck` Lagrangian particle demonstration. This version uses the ECCO MITgcm velocity field data available on SciServer.\n",
+                "`seaduck` Lagrangian particle demonstration. This version uses a reduced version of the ECCO MITgcm velocity field data.\n",
                 "\n",
                 "authors: Wenrui Jiang, Tom Haine Feb '23"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-input"
+                ]
+            },
             "outputs": [],
             "source": [
                 "import cartopy.crs as ccrs\n",
+                "import matplotlib as mpl\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "\n",
-                "import seaduck as sd"
+                "import seaduck as sd\n",
+                "\n",
+                "mpl.rcParams[\"figure.dpi\"] = 300"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### The ECCO MITgcm run is a low-resolution global state estimate, available on SciServer. The simulation is opened using the OceanSpy package.\n",
+                "## Loading Dataset\n",
                 "\n",
-                "Choose between the monthly-mean data ('ECCO') or the daily-mean data ('daily_ecco').\n",
+                "The ECCO MITgcm run is a low-resolution global state estimate. An artifact of note is that this dataset has complex grid topology, which means there is a `face` (also called tile) dimension in the dataset.\n",
                 "\n",
-                "### See: https://dev-poseidon-ocean.pantheonsite.io/products/datasets/."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "# ecco = ospy.open_oceandataset.from_catalog(\"ECCO\")\n",
-                "# ecco = ospy.open_oceandataset.from_catalog('daily_ecco')\n",
-                "ecco = sd.utils.get_dataset(\"ecco\")\n",
-                "ecco = sd.utils.process_ecco(ecco)"
+                "A built-in function in `seaduck.utils` can help access the snippet of ECCO that this example is based on. The grid of this dataset is the same as the original dataset, while all other variables are synthetic."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "ecco = sd.utils.get_dataset(\"ecco\")\n",
                 "ecco"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Initialize seaduck package. Then set the debug level."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "sd.rcParam[\n",
-                "    \"debug_level\"\n",
-                "] = \"very_high\"  # Options are: 'high','very_high','not that high'"
+                "```{admonition} Access full ECCO dataset\n",
+                "The ECCO dataset is publicly available on [SciServer](https://sciserver.org/). The simulation output can be opened using the [OceanSpy](https://github.com/hainegroup/oceanspy) package with the [`from_catalog`](https://oceanspy.readthedocs.io/en/latest/generated/oceanspy.open_oceandataset.from_catalog.html#oceanspy.open_oceandataset.from_catalog) method (Oceanspy is already available in the Oceanography container environment on SciServer).\n",
+                "\n",
+                "Choose between the monthly-mean data ('ECCO')\n",
+                "\n",
+                "`ecco = ospy.open_oceandataset.from_catalog(\"ECCO\")._ds`\n",
+                "\n",
+                "or the daily-mean data ('daily_ecco').\n",
+                "\n",
+                "`ecco = ospy.open_oceandataset.from_catalog('daily_ecco')._ds`\n",
+                "\n",
+                "Click [here](https://dev-poseidon-ocean.pantheonsite.io/products/datasets/) for a full list of the datasets hosted on SciServer.\n",
+                "```"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Specify the parameters for the particles (number, positions, start time)."
+                "## Experiment setup\n",
+                "\n",
+                "Specify the parameters for the particles (number, positions, start time)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Define the extend of the box\n",
-                "west = -19.0\n",
-                "east = -9.0\n",
-                "south = 57.0\n",
-                "north = 63.0\n",
+                "# Define the extent of the box\n",
+                "west = -90.0\n",
+                "east = 0.0\n",
+                "south = 23.0\n",
+                "north = 67.0\n",
                 "shallow = -10.0\n",
                 "deep = -10.0\n",
                 "\n",
                 "time = \"1992-02-15\"\n",
                 "\n",
-                "Nlon = 20  # How many along longitudinal direction?\n",
-                "Nlat = 20  # How many along latitudinal direction?\n",
+                "Nlon = 80  # How many along longitudinal direction?\n",
+                "Nlat = 80  # How many along latitudinal direction?\n",
                 "Ndep = 1  # How many along vertical direction?\n",
                 "\n",
                 "x, y, z, t = sd.utils.easy_3d_cube(\n",
                 "    (east, west, Nlon),\n",
                 "    (south, north, Nlat),\n",
                 "    (shallow, deep, Ndep),\n",
                 "    time,\n",
                 "    print_total_number=True,\n",
                 ")"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# x,y,z,t =\n",
-                "# # Change the number of particles here\n",
-                "# N = int(1e2)\n",
-                "\n",
-                "# # Change the vertical depth of the particles here\n",
-                "# levels = np.array([-5])\n",
-                "# sqrtN = int(np.sqrt(N))\n",
-                "\n",
-                "# # Change the longitude and latitude positions of the particles here\n",
-                "# xx = np.linspace(-19, -9, sqrtN)\n",
-                "# yy = np.linspace(63, 57, sqrtN)\n",
-                "\n",
-                "# # Compute intermediate grid variables\n",
-                "# xxx, yyy = np.meshgrid(xx, yy)\n",
-                "# x = xxx.ravel()\n",
-                "# y = yyy.ravel()\n",
-                "# x, z = np.meshgrid(x, levels)\n",
-                "# y, z = np.meshgrid(y, levels)\n",
-                "# x = x.ravel()\n",
-                "# y = y.ravel()\n",
-                "# z = z.ravel()\n",
-                "\n",
-                "# # Change the times here\n",
-                "# start_time = \"1998-12-15\"\n",
-                "# t = (\n",
-                "#     np.array([np.datetime64(start_time) for i in x]) - np.datetime64(\"1970-01-01\")\n",
-                "# ) / np.timedelta64(1, \"s\")"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Plot the particle positions"
+                "Plot the particle positions"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "tags": []
+                "tags": [
+                    "hide-input"
+                ]
             },
             "outputs": [],
             "source": [
                 "ax = plt.axes(projection=ccrs.PlateCarree())\n",
-                "ax.plot(x, y, \"r+\")\n",
+                "ax.plot(x, y, \"ro\", markersize=0.5)\n",
                 "ax.coastlines()\n",
-                "ax.set_xlim([-25, 0])\n",
-                "ax.set_ylim([50, 70])\n",
+                "ax.set_title(\"Interpolation position\")\n",
                 "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Let's explore the interpolation function in `seaduck`:"
+                "## Let's explore `seaduck.OceInterp`\n",
+                "\n",
+                "This is the most high-level function of the package. Yes, it's very easy to use."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "tags": []
+                "tags": [
+                    "hide-output"
+                ]
             },
             "outputs": [],
             "source": [
                 "help(sd.OceInterp)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Interpolate these ECCO fields onto the particle positions."
+                "### Interpolate these ECCO fields at Eulerian positions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
@@ -208,111 +173,100 @@
                 "[s, (u, v), eta, mask] = sd.OceInterp(\n",
                 "    ecco, [\"SALT\", (\"UVELMASS\", \"VVELMASS\"), \"ETAN\", \"maskC\"], x, y, z, t\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Plot the interpolated salinity field."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
+            "metadata": {
+                "tags": [
+                    "mdformat-skip"
+                ]
+            },
             "source": [
-                "ax = plt.axes(projection=ccrs.PlateCarree())\n",
-                "c = ax.scatter(x, y, c=s)\n",
-                "ax.coastlines()\n",
-                "ax.set_xlim([-25, 0])\n",
-                "ax.set_ylim([50, 70])\n",
-                "plt.colorbar(c)\n",
-                "plt.title(\"Salinity (psu)\")"
+                "Plot the interpolated salinity, $u$, $\\eta$ field."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Plot the interpolated $u$ field."
+                "```{warning}\n",
+                "In case you haven't notice, SALT, ETAN are purely synthetic. \n",
+                "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-input"
+                ]
+            },
             "outputs": [],
             "source": [
-                "ax = plt.axes(projection=ccrs.PlateCarree())\n",
-                "c = ax.scatter(x, y, c=u)\n",
-                "ax.coastlines()\n",
-                "ax.set_xlim([-25, 0])\n",
-                "ax.set_ylim([50, 70])\n",
-                "plt.colorbar(c)\n",
-                "plt.title(\"Zonal Velocity (m/s)\")"
+                "unit = [\"psu\", \"m/s\", \"m\"]\n",
+                "name = [\"Salinity\", \"Zonal Velocity\", \"Sea Surface Height\"]\n",
+                "for i, var in enumerate([s, u, eta]):\n",
+                "    ax = plt.subplot(1, 3, 1 + i, projection=ccrs.PlateCarree())\n",
+                "    c = ax.scatter(x, y, c=var, s=0.5)\n",
+                "    ax.coastlines()\n",
+                "    ax.set_xlim([west, east])\n",
+                "    ax.set_ylim([south, north])\n",
+                "    plt.colorbar(c, location=\"bottom\", label=unit[i], pad=0.03)\n",
+                "    ax.set_title(name[i])\n",
+                "plt.tight_layout()\n",
+                "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Plot the interpolated $\\\\eta$ field."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ax = plt.axes(projection=ccrs.PlateCarree())\n",
-                "c = ax.scatter(x, y, c=eta)\n",
-                "ax.coastlines()\n",
-                "ax.set_xlim([-25, 0])\n",
-                "ax.set_ylim([50, 70])\n",
-                "plt.colorbar(c)\n",
-                "plt.title(\"Sea Surface Height (m)\")"
+                "The salinity and the sea surface height variable here are not model output but randomly generated noise and there are values on land as well. However, the package respects the mask provided by the model, so even though there are apparently values on land, NaNs are returned.\n",
+                "\n",
+                "This is not the case for velocity. The mask for the staggered velocity field is not provided by the model, so the actual value (zero here) is returned."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Now compute Lagrangian trajectories for these particles.\n",
                 "\n",
-                "#### Define the `start_time` and `end_time`. Here the particles are integrated backwards in time."
+                "First, define the `start_time` and `end_time`. Here the particles are integrated backwards in time."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "start_time = \"1992-01-17\"\n",
                 "end_time = \"1992-03-12\"\n",
                 "\n",
                 "t_bnds = np.array(\n",
                 "    [\n",
-                "        np.datetime64(start_time) - np.datetime64(\"1970-01-01\"),\n",
-                "        np.datetime64(end_time) - np.datetime64(\"1970-01-01\"),\n",
+                "        sd.utils.convert_time(start_time),\n",
+                "        sd.utils.convert_time(end_time),\n",
                 "    ]\n",
-                ") / np.timedelta64(1, \"s\")"
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Perform the particle trajectory simulation.\n",
                 "\n",
-                "#### Record the salinity along the particle trajectories as well as their (lat,lon) positions."
+                "To switch between Lagrangian and Eulerian modes, you only need to change the `lagrangian` keyword argument.\n",
+                "\n",
+                "The following code block simulates the trajectory and records the salinity along the particle trajectories, as well as their (lat,lon) positions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -322,39 +276,38 @@
                 "    [\"SALT\", \"__particle.raw\", \"__particle.lat\", \"__particle.lon\"],\n",
                 "    x,\n",
                 "    y,\n",
                 "    z,\n",
                 "    t_bnds,\n",
                 "    lagrangian=True,\n",
                 "    return_pt_time=True,\n",
-                "    lagrange_kwarg={\"save_raw\": True},\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### There are 4 output times. See also the diagnostic output from running the integration."
+                "There are 3 output times. See also the diagnostic output from running the integration."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "stops"
+                "len(stops)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### The `raw` output is a vector of `OceInterp` objects with position information"
+                "The `raw` output is a list of `seaduck.Position` objects which stores, of course, the position of the particle at specific times."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -368,86 +321,93 @@
             "source": [
                 "### Plot the interpolated salinity field on the final particle positions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-input"
+                ]
+            },
             "outputs": [],
             "source": [
                 "ax = plt.axes(projection=ccrs.PlateCarree())\n",
-                "ax.scatter(lon[-1], lat[-1], c=s[-1], s=1)\n",
+                "ax.scatter(lon[-1], lat[-1], c=s[-1], s=6)\n",
                 "ax.coastlines()\n",
                 "ax.set_xlim([-70, 0])\n",
                 "ax.set_ylim([30, 70])\n",
-                "plt.title(\"salinity map\")"
+                "plt.title(\"salinity map\")\n",
+                "plt.show()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### There are some other `OceInterp` classes:\n",
+                "## Calculate derivatives\n",
                 "\n",
-                "#### 1. Kernel object"
+                "### Kernel object\n",
+                "\n",
+                "The `kernel` object defines which neighboring points are used for the interpolation, and also what kind of operation is conducted. The default is interpolation. However, you can also use this class to calculate derivatives."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-output"
+                ]
+            },
             "outputs": [],
             "source": [
-                "KnW = sd.kernel_weight.KnW"
+                "KnW = sd.kernel_weight.KnW\n",
+                "help(KnW)"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "mdformat-skip"
+                ]
+            },
             "source": [
-                "#### Define derivative kernels for\n",
-                "\n",
-                "$\\\\partial / \\\\partial z$, $\\\\partial^2 / \\\\partial x^2$, and $\\\\partial / \\\\partial t$."
+                "Let's define derivative kernels for $\\partial / \\partial z$, $\\partial^2 / \\partial x^2$, $\\partial^2 / \\partial y^2$, and $\\partial / \\partial t$ as examples:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "default = KnW()\n",
                 "dz_kernel = KnW(vkernel=\"dz\")\n",
-                "dx2_kernel = KnW(\n",
-                "    hkernel=\"dx\", h_order=2, inheritance=[[0, 1, 2, 3, 4, 5, 6, 7, 8]], tkernel=\"linear\"\n",
-                ")\n",
+                "dx2_kernel = KnW(hkernel=\"dx\", h_order=2, inheritance=None)\n",
+                "dy2_kernel = KnW(hkernel=\"dy\", h_order=2, inheritance=None)\n",
                 "dt_kernel = KnW(tkernel=\"dt\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "#### Apply the kernels to the ECCO fields:"
+                "Apply the kernels to the ECCO fields:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "[dsdz, (d2udx2, dvdt)] = sd.OceInterp(\n",
-                "    ecco,\n",
-                "    {\"SALT\": dz_kernel, (\"UVELMASS\", \"VVELMASS\"): (dx2_kernel, dt_kernel)},\n",
-                "    x,\n",
-                "    y,\n",
-                "    z,\n",
-                "    t,\n",
+                "d2edx2, d2edy2 = sd.OceInterp(\n",
+                "    ecco, [\"ETAN\", \"ETAN\"], x, y, z, t, kernel_list=[dx2_kernel, dy2_kernel]\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -456,32 +416,38 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ax = plt.axes(projection=ccrs.PlateCarree())\n",
-                "c = ax.scatter(x, y, c=d2udx2)\n",
-                "ax.coastlines()\n",
-                "ax.set_xlim([-25, 0])\n",
-                "ax.set_ylim([50, 70])\n",
-                "plt.colorbar(c)\n",
-                "plt.title(\"Second Derivative of the Zonal Velocity (m/s per grid scale squared)\")"
+                "laplacian = d2edx2 + d2edy2"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": [
+                    "hide-input"
+                ]
+            },
             "outputs": [],
-            "source": []
+            "source": [
+                "ax = plt.axes(projection=ccrs.PlateCarree())\n",
+                "c = ax.scatter(x, y, c=laplacian, s=5)\n",
+                "ax.coastlines()\n",
+                "plt.colorbar(c, location=\"bottom\", label=\"m/s per grid scale squared\")\n",
+                "plt.title(\"Laplacian of sea surface height\")\n",
+                "plt.show()"
+            ]
         }
     ],
     "metadata": {
+        "celltoolbar": "Tags",
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
```

### Comparing `seaduck-0.1.2/docs/_config.yml` & `seaduck-0.1.3/docs/_config.yml`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 title: My sample book
 author: The Jupyter Book Community
 logo: logo.png
 
 # Force re-execution of notebooks on each build.
 # See https://jupyterbook.org/content/execute.html
 execute:
+  timeout: 300
   execute_notebooks: 'auto'
   stderr_output: "remove"
   exclude_patterns:
   - '*.md'
 
 # Define the name of the latex output file for PDF builds
 latex:
   latex_documents:
     targetname: book.tex
 
 # Add sphinx autodoc to generate api reference from code files
 sphinx:
   extra_extensions:
   - 'sphinx.ext.autodoc'
+  - 'sphinx.ext.napoleon'
   config:
     html_theme: sphinx_book_theme
     autodoc_member_order: groupwise
     # html_theme_options: {
     #     "relbarbgcolor": 'Orange',
     #     "codebgcolor": 'Coral'
     # }
```

### Comparing `seaduck-0.1.2/docs/_toc.yml` & `seaduck-0.1.3/docs/_toc.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 format: jb-book
 root: intro
 parts:
 - caption: Tutorial
   chapters:
   - file: how_to_install
-  - file: notebooks
+  - file: get_started
     sections:
+    - file: one_min_guide
     - file: network_of_object
-  - file: reference
+  - file: api_reference
     sections:
     - file: api_reference/apiref_OceData.rst
     - file: api_reference/apiref_topology.rst
     - file: api_reference/apiref_eulerian.rst
     - file: api_reference/apiref_lagrangian.rst
     - file: api_reference/apiref_OceInterp.rst
     - file: api_reference/apiref_kernelNweight.rst
     - file: api_reference/apiref_smartread.rst
     - file: api_reference/apiref_getmasks.rst
     - file: api_reference/apiref_utils.rst
-    - file: all_in_one
+    - file: api_reference/apiref_RelCoord.rst
 - caption: Examples
   chapters:
-  - file: Global_ECCO
-  - file: AVISO
-  - file: sciserver_notebooks/IGP
+  - file: ideal_test
+    sections:
+    - file: idealize_test/hor_stream
+    - file: idealize_test/ver_stream
+    - file: idealize_test/tilted_stream
+  - file: ocean_example
+    sections:
+    - file: notebook/global_ECCO
+    - file: notebook/AVISO
+    - file: notebook/topology_tutorial
+  - file: sciserver_example
+    sections:
+    - file: sciserver_notebooks/IGPwinter
+    - file: sciserver_notebooks/KangerFjord
+    - file: sciserver_notebooks/LLC4320
+    - file: sciserver_notebooks/ECCO_plot_stations
 - caption: Contributing
   chapters:
-  - file: contribute/use_git
-  - file: contribute/prep_env
-  - file: contribute/contr_cod
-  - file: contribute/contr_doc
-  - file: contribute/tidyNpr
+  - file: guide_for_developer
+    sections:
+    - file: contribute/use_git
+    - file: contribute/prep_env
+    - file: contribute/contr_cod
+    - file: contribute/contr_doc
+    - file: contribute/tidyNpr
```

### Comparing `seaduck-0.1.2/docs/contribute/contr_doc.md` & `seaduck-0.1.3/docs/contribute/contr_doc.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Contributing to documentaion🦆
+# Contributing to documentation🦆
 
 We are using [Jupyter Book](https://jupyterbook.org/en/stable/intro.html#)📙 to build the documentation. The online documentaion is hosted by [github pages](https://pages.github.com/).
 
 ## Add/Modify
 
 [Jupyter Book](https://jupyterbook.org/en/stable/intro.html#)📗 support several different kinds of files as input, including [.md files](https://jupyterbook.org/en/stable/reference/cheatsheet.html#tags)⬇️ [.rst files](https://docutils.sourceforge.io/docs/user/rst/cheatsheet.html)📜, [.ipynb files](https://www.ibm.com/docs/en/watson-studio-local/1.2.3?topic=notebooks-markdown-jupyter-cheatsheet)🐍, etc. Executable ones generally requires a slightly different procedures to the narrative files. Here are some instruction on how to work with each of them.
 
@@ -23,21 +23,21 @@
 ```
 
 6. Go to `seaduck/docs/_build/html`, you can either open `index.html` or the html file with the same name to the one that you have made changes to. See if it looks right to you. If not, iterate a little. Send me a message if you need help.
 1. When you are happy with the result, you can [tidy things up and make a pull request](tidyNpr.md). After approval, your changes will be {ref}`deployed <deploy_doc>`.
 
 ## Notebooks that could be run any where
 
-As a package that works with oceanographical datasets, almost all the demonstrations requires some supporting data. `seaduck` provides several datasets available to be downloaded everywhere. It can be accessed simply by
+As a package that works with oceanographic datasets, almost all the demonstrations requires some supporting data. `seaduck` provides several datasets available to be downloaded everywhere. It can be accessed simply by
 
 ```python
 ds = seaduck.utils.get_dataset(name)
 ```
 
-Another option is to generate the dataset using mathematical expressions out of thin air. Since this kind of notebook is executed whenever the github action is triggered, it is prefered that these notebooks being very fast to run. For example, do not perform heavy calculations in those notebooks and please do not install packages within them.
+Another option is to generate the dataset using mathematical expressions out of thin air. Since this kind of notebook is executed whenever the github action is triggered, it is preferrable that these notebooks run very fast. For example, do not perform heavy calculations in those notebooks and please do not install packages within them.
 
 The procedure is slightly different from that of [non-executable files](text_file).
 
 1. Follow step 1 to 6 in the [previous](text_file) section.
 1. Run
 
 ```none
@@ -45,26 +45,35 @@
 ```
 
 This step will "style" all the files and crucially strip the output of the notebooks. The first time running it is almost certainly going to fail. Don't worry, `pre-commit`, the thing under the hood, will automatically fix most of the problems.
 
 Now, run it again. If this time it still has an error, look at the error message and see what you can do.
 3\. Now, you can [tidy things up and make a pull request](tidyNpr.md)
 
-## Cooler(Sciserver) notebooks
+## Cooler (Sciserver) notebooks
 
 Cool stuff are not always portable. The ocean 🌊 is an example of that.
 Say you have something really cool you want to demonstrate, but the dataset it is based on is to large to distribute or it simply takes too long to run. Wouldn't it be nice if we could have a cloud platform that host a bunch of ocean dataset that is free for everyone to use? It would be even better if the packages I need as an oceanographer is readily installed and I don't have to worry about a thing.
 You can use [Sciserver](https://sciserver.org/)! (Am I too dramatic?). Sciserver is also the home base of [oceanspy](https://oceanspy.readthedocs.io/en/latest/), a package that will make your life so much easier as a oceanographer. After registering on sciserver (you can follow this youtube tutorial here(Tom, if you are reading this, can you send me the link?)), you can simply call this oceanspy function
 
 ```python
 import ocenspy as ospy
 od = ospy.open_oceandataset.from_catalog('NameOfDataset')
 ds = od._ds
 ```
 
+Note that since you are using an `Oceanography` image, most packages are already downloaded. We still need two dependencies just to convert the notebooks.
+
+```
+pip install -U jupyter-book
+pip install jupytext
+```
+
+And that's it, you don't have to follow the steps of preparing environment.
+
 Now, follow these steps:
 
 1. [Fork and clone](use_git.md) this repo adjacent to the seaduck directory
 
 ```shell
 git clone https://github.com/YourGithubNickname/seaduck_sciserver_notebook.git
 ```
```

### Comparing `seaduck-0.1.2/docs/contribute/tidyNpr.md` & `seaduck-0.1.3/docs/contribute/tidyNpr.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 # Tidy it up and make Pull Request
 
-Every time you make some change, run
+When you are in the `seaduck` directory and feel like you are finished with your changes, just before you submit everything, simply run
 
 ```shell
-git add .
-git commit -m "A description of the good stuff you have done"
+make
 ```
 
-When you are in the `seaduck` directory and feel like you are finished with your changes, just before you submit everything, simply run
+This will do the style check and run [pytest](https://docs.pytest.org). If you followed the steps in ["prepare the environment"](prep_env.md), everything here should pass.
+
+Make sure before you push everything is committed.
 
 ```shell
-make
+git add .
+git commit -m "A description of the good stuff you have done"
+```
+
+```{tip} Sometimes the style check will make changes to the file, make sure you commit after that.
+Alternatively, you could ask `pre-commit` to run every time you commit by running `pre-commit install`.
 ```
 
-This will do the style check, run pytest. If you followed the steps in ["prepare the environment"](prep_env.md), everything here should pass. If this is the case, then
+If everything passed then
 
 ```shell
-git push
+git push -u origin name_of_your_branch
 ```
 
 Now open your forked directory, you should be able to "start a pull request" by clicking around.
 
-Now, wait Mr. Duckmaster to merge your branch into the main branch.
+Now, wait for Mr. Duckmaster to merge your branch into the main branch.
```

### Comparing `seaduck-0.1.2/docs/logo.png` & `seaduck-0.1.3/docs/logo.png`

 * *Files identical despite different names*

### Comparing `seaduck-0.1.2/docs/reference.md` & `seaduck-0.1.3/docs/api_reference.md`

 * *Files 17% similar despite different names*

```diff
@@ -19,9 +19,7 @@
 [Kernal_and_Weight](api_reference/apiref_kernelNweight.rst)
 
 ## Utils
 
 [smart_read](api_reference/apiref_smartread.rst)
 [get_masks](api_reference/apiref_getmasks.rst)
 [utils](api_reference/apiref_utils.rst)
-
-### [All in one page](all_in_one)
```

### Comparing `seaduck-0.1.2/pyproject.toml` & `seaduck-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering"
 ]
 dependencies = [
   "numpy",
   "pandas",
   "scipy",
+  "dask[array]",
   "xarray"
 ]
 description = "A python package that interpolates data from ocean dataset from both Eulerian and Lagrangian perspective. "
 dynamic = ["version"]
 license = {file = "LICENSE"}
 name = "seaduck"
 readme = "README.md"
@@ -34,15 +35,16 @@
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = [
   "matplotlib.*",
   "numba",
   "pooch",
-  "scipy"
+  "scipy",
+  "scipy.interpolate"
 ]
 
 [tool.ruff]
 ignore = [
   # pydocstyle: Missing Docstrings
   "D1",
   # pydocstyle: numpy convention
```

### Comparing `seaduck-0.1.2/seaduck/__init__.py` & `seaduck-0.1.3/seaduck/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,25 +16,25 @@
     # NOTE: the `version.py` file must not be present in the git repository
     #   as it is generated by setuptools at install time
     from seaduck.version import __version__
 except ImportError:  # pragma: no cover
     # Local copy or not installed with setuptools
     __version__ = "999"
 
-from seaduck.eulerian import position
+from seaduck.eulerian import Position
 from seaduck.kernel_weight import KnW
-from seaduck.lagrangian import particle
+from seaduck.lagrangian import Particle
 from seaduck.ocedata import OceData
 from seaduck.oceinterp import OceInterp
 from seaduck.runtime_conf import rcParam
-from seaduck.topology import topology
+from seaduck.topology import Topology
 
 __all__ = [
     "__version__",
-    "position",
+    "Position",
     "KnW",
-    "particle",
+    "Particle",
     "OceData",
     "OceInterp",
     "rcParam",
-    "topology",
+    "Topology",
 ]
```

### Comparing `seaduck-0.1.2/seaduck/eulerian.py` & `seaduck-0.1.3/seaduck/eulerian.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 import copy
+import logging
 
 import numpy as np
 
 from seaduck.get_masks import get_masked
 from seaduck.kernel_weight import KnW, _translate_to_tendency, find_pk_4d
-from seaduck.ocedata import OceData
+from seaduck.ocedata import HRel, OceData, RelCoord, TRel, VlRel, VRel
 
 # from OceInterp.kernel_and_weight import _translate_to_tendency,find_pk_4d
-from seaduck.smart_read import smart_read as sread
+from seaduck.smart_read import smart_read
 from seaduck.utils import (
     _general_len,
     find_px_py,
     get_key_by_value,
     local_to_latlon,
+    to_180,
     weight_f_node,
 )
 
 
 def _ind_broadcast(x, ind):
     """Perform a "cartesian product" on two fattened dimensions.
 
-    **Parameters:**
-
-    + x: numpy.ndarray
+    Parameters
+    ----------
+    x: numpy.ndarray
         A new dimension
-    + ind: tuple
+    ind: tuple
         Existing indexes
     """
     n = x.shape[0]
     if len(x.shape) == 1:
         x = x.reshape((n, 1))
     xsp = x.shape
     ysp = ind[0].shape
     final_shape = [n] + list(ysp[1:]) + list(xsp[1:])
 
-    R = [np.zeros(final_shape, int) for i in range(len(ind) + 1)]
+    to_return = [np.zeros(final_shape, int) for i in range(len(ind) + 1)]
 
     dims = len(final_shape)
     ydim = len(ysp) - 1
     trsp = list(range(1, 1 + ydim)) + [0] + list(range(1 + ydim, dims))
     inv = np.argsort(trsp)
-    R[0] = R[0].transpose(trsp)
-    R[0][:] = x
-    R[0] = R[0].transpose(inv)
+    to_return[0] = to_return[0].transpose(trsp)
+    to_return[0][:] = x
+    to_return[0] = to_return[0].transpose(inv)
 
     for i in range(1, len(ind) + 1):
-        R[i] = R[i].T
-        R[i][:] = ind[i - 1].T
-        R[i] = R[i].T
-    return R
+        to_return[i] = to_return[i].T
+        to_return[i][:] = ind[i - 1].T
+        to_return[i] = to_return[i].T
+    return to_return
 
 
 def _partial_flatten(ind):
     """Convert a high dimensional index set to a 2D one."""
     if isinstance(ind, tuple):
         shape = ind[0].shape
 
         # num_neighbor = 1
         # for i in range(1,len(shape)):
         #     num_neighbor*=shape[i]
-        R = []
+        to_return = []
         for i in range(len(ind)):
-            R.append(ind[i].reshape(shape[0], -1))
-        return tuple(R)
+            to_return.append(ind[i].reshape(shape[0], -1))
+        return tuple(to_return)
     elif isinstance(ind, np.ndarray):
         shape = ind.shape
         num_neighbor = 1
         for i in range(1, len(shape)):
             num_neighbor *= shape[i]
         return ind.reshape(shape[0], num_neighbor)
+    else:
+        raise NotImplementedError("ind type not supported")
 
 
 def _in_required(name, required):
     """See if a name is in required."""
     if required == "all":
         return True
     else:
@@ -88,228 +92,233 @@
     """
     ind_for_mask = [ind[i] for i in range(len(ind)) if dims[i] not in ["time"]]
     if "Z" not in dims and "Zl" not in dims:
         ind_for_mask.insert(0, np.zeros_like(ind[0]))
     return tuple(ind_for_mask)
 
 
-def _subtract_i_min(ind, i_min):
+def _subtract_prefetch_prefix(ind, prefetch_prefix):
     """Subtract the index prefix from the actual index.
 
     This is used when one is reading from a prefetched subset of the data.
     """
     temp_ind = []
-    for i in range(len(i_min)):
-        temp_ind.append(ind[i] - i_min[i])
+    for i in range(len(prefetch_prefix)):
+        temp_ind.append(ind[i] - prefetch_prefix[i])
     return tuple(temp_ind)
 
 
-class position:
-    """The position object that performs the interpolation.
+class Position:
+    """The Position object that performs the interpolation.
 
     Create a empty one by default.
     To actually do interpolation, use from_latlon method to tell the ducks where they are.
     """
 
-    #     self.ind_h_dict = {}
+    def __new__(cls, *arg, **kwarg):
+        new_position = object.__new__(cls)
+        new_position.rel = RelCoord()
+        return new_position
+
+    def __getattr__(self, attr):
+        if attr == "rel":
+            object.__getattribute__(self, attr)
+        elif attr in self.rel.keys():
+            return getattr(self.rel, attr)
+        else:
+            object.__getattribute__(self, attr)
+
+    def __setattr__(self, attr, value):
+        if attr == "rel":
+            object.__setattr__(self, attr, value)
+        elif attr in self.rel.keys():
+            setattr(self.rel, attr, value)
+        else:
+            object.__setattr__(self, attr, value)
+
     def from_latlon(self, x=None, y=None, z=None, t=None, data=None):
         """Fill in the coord info using lat-lon-dep-time dims.
 
         Use the methods from the ocedata to transform
         from lat-lon-dep-time coords to rel-coords
-        store the output in the position object.
+        store the output in the Position object.
 
-        **Parameters:**
-
-        + x,y,z,t: numpy.ndarray
+        Parameters
+        ----------
+        x,y,z,t: numpy.ndarray, float or None, default None
             1D array of the lat-lon-dep-time coords
-        + data: OceData object
-            The field where the positions are defined on.
+        data: OceData object
+            The field where the Positions are defined on.
         """
         if data is None:
             try:
                 self.ocedata
-            except AttributeError:
-                raise ValueError("data not provided")
+            except AttributeError as exc:
+                raise ValueError("data not provided") from exc
         else:
             if isinstance(data, OceData):
                 self.ocedata = data
             else:
                 raise ValueError("Input data must be OceData")
         self.tp = self.ocedata.tp
         length = [_general_len(i) for i in [x, y, z, t]]
         self.N = max(length)
-        if any([i != self.N for i in length if i > 1]):
+        if any(i != self.N for i in length if i > 1):
             raise ValueError("Shapes of input coordinates are not compatible")
 
-        if isinstance(x, float):
-            x = np.array([1.0]) * x
-        if isinstance(y, float):
-            y = np.array([1.0]) * y
-        if isinstance(z, float):
-            z = np.array([1.0]) * z
-        if isinstance(t, float):
-            t = np.array([1.0]) * t
+        if isinstance(x, (int, float, np.floating)):
+            x = np.ones(self.N, float) * x
+        if isinstance(y, (int, float, np.floating)):
+            y = np.ones(self.N, float) * y
+        if isinstance(z, (int, float, np.floating)):
+            z = np.ones(self.N, float) * z
+        if isinstance(t, (int, float, np.floating)):
+            t = np.ones(self.N, float) * t
 
         for thing in [x, y, z, t]:
-            if len(x.shape) > 1:
+            if thing is None:
+                continue
+            if len(thing.shape) > 1:
                 raise ValueError("Input need to be 1D numpy arrays")
         if (x is not None) and (y is not None):
-            self.lon = x
-            self.lat = y
-            (
-                self.face,
-                self.iy,
-                self.ix,
-                self.rx,
-                self.ry,
-                self.cs,
-                self.sn,
-                self.dx,
-                self.dy,
-                self.bx,
-                self.by,
-            ) = self.ocedata.find_rel_h(x, y)
+            self.lon = copy.deepcopy(x)
+            self.lat = copy.deepcopy(y)
+            self.rel.update(self.ocedata.find_rel_h(self.lon, self.lat))
         else:
+            self.rel.update(HRel._make([None for i in range(11)]))
             self.lon = None
             self.lat = None
-            self.face = None
-            self.iy = None
-            self.ix = None
-            self.rx = None
-            self.ry = None
-            self.cs = None
-            self.sn = None
-            self.dx = None
-            self.dy = None
-            self.bx = None
-            self.by = None
         if z is not None:
-            self.dep = z
+            self.dep = copy.deepcopy(z)
             if self.ocedata.readiness["Z"]:
-                (self.iz, self.rz, self.dz, self.bz) = self.ocedata.find_rel_v(z)
+                self.rel.update(self.ocedata.find_rel_v(z))
             else:
-                (
-                    self.iz,
-                    self.rz,
-                    self.dz,
-                    self.bz,
-                ) = (None for i in range(4))
+                self.rel.update(VRel._make(None for i in range(4)))
             if self.ocedata.readiness["Zl"]:
-                (self.izl, self.rzl, self.dzl, self.bzl) = self.ocedata.find_rel_vl(z)
+                self.rel.update(self.ocedata.find_rel_vl(z))
             else:
-                (
-                    self.izl,
-                    self.rzl,
-                    self.dzl,
-                    self.bzl,
-                ) = (None for i in range(4))
+                self.rel.update(VlRel._make(None for i in range(4)))
         else:
-            (
-                self.iz,
-                self.rz,
-                self.dz,
-                self.bz,
-                self.izl,
-                self.rzl,
-                self.dzl,
-                self.bzl,
-                self.dep,
-            ) = (None for i in range(9))
+            self.rel.update(VRel._make(None for i in range(4)))
+            self.rel.update(VlRel._make(None for i in range(4)))
+            self.dep = None
 
         if t is not None:
-            self.t = t
+            self.t = copy.deepcopy(t)
             if self.ocedata.readiness["time"]:
-                (self.it, self.rt, self.dt, self.bt) = self.ocedata.find_rel_t(t)
+                self.rel.update(self.ocedata.find_rel_t(t))
             else:
-                (
-                    self.it,
-                    self.rt,
-                    self.dt,
-                    self.bt,
-                ) = (None for i in range(4))
+                self.rel.update(TRel._make(None for i in range(4)))
         else:
-            (self.it, self.rt, self.dt, self.bt, self.t) = (None for i in range(5))
+            self.rel.update(TRel._make(None for i in range(4)))
+            self.t = None
+            # (self.it, self.rt, self.dt, self.bt, self.t) = (None for i in range(5))
         return self
 
     def subset(self, which):
-        """Create a subset of the position object.
+        """Create a subset of the Position object.
 
-        **Parameters:**
-
-        + which: numpy.ndarray
+        Parameters
+        ----------
+        which: numpy.ndarray, optional
             Define which points survive the subset operation.
             It be an array of either boolean or int.
             The selection is similar to that of selecting from a 1D numpy array.
 
-        **Returns:**
-
-        + the_subset: position object
-            The selected positions.
+        Returns
+        -------
+        the_subset: Position object
+            The selected Positions.
         """
-        p = position()
-        keys = self.__dict__.keys()
-        for i in keys:
-            item = self.__dict__[i]
+        p = object.__new__(type(self))
+        vardict = vars(self)
+        keys = vardict.keys()
+        for key in keys:
+            item = vardict[key]
             if isinstance(item, np.ndarray):
                 if len(item.shape) == 1:
-                    p.__dict__[i] = item[which]
-                    p.N = len(p.__dict__[i])
+                    setattr(p, key, item[which])
+                    p.N = len(getattr(p, key))
+                elif key in ["px", "py"]:
+                    setattr(p, key, item[:, which])
                 else:
-                    p.__dict__[i] = item
+                    setattr(p, key, item)
+            elif isinstance(item, RelCoord):
+                setattr(p, key, item.subset(which))
             else:
-                p.__dict__[i] = item
-        # p.N = max([_general_len(i) for i in p.__dict__.values()])
+                setattr(p, key, item)
         return p
 
+    def update_from_subset(self, sub, which):
+        vardict = vars(sub)
+        keys = vardict.keys()
+        for key in keys:
+            item = vardict[key]
+            if not hasattr(self, key):
+                logging.warning(
+                    f"A new attribute {key} defined" "after updating from subset"
+                )
+                setattr(self, key, item)
+            if getattr(self, key) is None:
+                continue
+            if isinstance(item, np.ndarray):
+                if len(item.shape) == 1:
+                    getattr(self, key)[which] = item
+                elif key in ["px", "py"]:
+                    getattr(self, key)[:, which] = item
+            elif isinstance(item, RelCoord):
+                self.rel.update_from_subset(item, which)
+            elif isinstance(item, list):
+                setattr(self, key, item)
+
     def fatten_h(self, knw, ind_moves_kwarg={}):
         """Fatten horizontal indices.
 
         Fatten means to find the neighboring points of the points of interest based on the kernel.
         faces,iys,ixs are 1d arrays of size n.
         We are applying a kernel of size m.
         This is going to return a n * m array of indexes.
         A very slim vector is now a matrix, and hence the name.
         each row represen all the node needed for interpolation of a single point.
         "h" represent we are only doing it on the horizontal plane.
 
-        **Parameters:**
-
-        + knw: KnW object
+        Parameters
+        ----------
+        knw: KnW object
             The kernel used to find neighboring points.
-        + ind_moves_kward: dict
-            Key word argument to put into ind_moves method of the topology object.
-            Read topology.ind_moves for more detail.
+        ind_moves_kward: dict, optional
+            Key word argument to put into ind_moves method of the Topology object.
+            Read Topology.ind_moves for more detail.
         """
         #         self.ind_h_dict
-        kernel = knw.kernel
+        kernel = knw.kernel.astype(int)
         kernel_tends = [_translate_to_tendency(k) for k in kernel]
         m = len(kernel_tends)
         n = len(self.iy)
         tp = self.ocedata.tp
 
         # the arrays we are going to return
         if self.face is not None:
-            n_faces = np.zeros((n, m))
+            n_faces = np.zeros((n, m), int)
             n_faces.T[:] = self.face
-        n_iys = np.zeros((n, m))
-        n_ixs = np.zeros((n, m))
+        n_iys = np.zeros((n, m), int)
+        n_ixs = np.zeros((n, m), int)
 
         # first try to fatten it naively(fast and vectorized)
         for i, node in enumerate(kernel):
             x_disp, y_disp = node
             n_iys[:, i] = self.iy + y_disp
             n_ixs[:, i] = self.ix + x_disp
         if self.face is not None:
             illegal = tp.check_illegal((n_faces, n_iys, n_ixs))
         else:
             illegal = tp.check_illegal((n_iys, n_ixs))
 
         redo = np.array(np.where(illegal)).T
-        for num, loc in enumerate(redo):
+        for loc in redo:
             j, i = loc
             if self.face is not None:
                 ind = (self.face[j], self.iy[j], self.ix[j])
             else:
                 ind = (self.iy[j], self.ix[j])
             # everyone start from the [0,0] node
             moves = kernel_tends[i]
@@ -317,120 +326,105 @@
             # [2,2] means move to the left and then move to the left again.
             n_ind = tp.ind_moves(ind, moves, **ind_moves_kwarg)
             if self.face is not None:
                 n_faces[j, i], n_iys[j, i], n_ixs[j, i] = n_ind
             else:
                 n_iys[j, i], n_ixs[j, i] = n_ind
         if self.face is not None:
-            return n_faces.astype("int"), n_iys.astype("int"), n_ixs.astype("int")
+            return n_faces, n_iys, n_ixs
         else:
-            return None, n_iys.astype("int"), n_ixs.astype("int")
+            return None, n_iys, n_ixs
 
     def fatten_v(self, knw):
         """Fatten in vertical center coord.
 
         Find the neighboring center grid points in the vertical direction.
 
-        **Parameters:**
-
-        + knw: KnW object
+        Parameters
+        ----------
+        knw: KnW object
             The kernel used to find neighboring points.
         """
         if self.iz is None:
             return None
         if knw.vkernel == "nearest":
-            return copy.deepcopy(self.iz.astype(int))
+            return copy.deepcopy(self.iz)
         elif knw.vkernel in ["dz", "linear"]:
             try:
                 self.iz_lin
             except AttributeError:
-                (
-                    self.iz_lin,
-                    self.rz_lin,
-                    self.dz_bin,
-                    self.bz_lin,
-                ) = self.ocedata.find_rel_v_lin(self.dep)
-            return np.vstack([self.iz_lin.astype(int), self.iz_lin.astype(int) - 1]).T
+                self.rel.update(self.ocedata.find_rel_v_lin(self.dep))
+            return np.vstack([self.iz_lin, self.iz_lin - 1]).T
         else:
             raise ValueError("vkernel not supported")
 
     def fatten_vl(self, knw):
         """Fatten in vertical staggered coord.
 
         Finding the neighboring staggered grid points in the vertical direction.
 
-        **Parameters:**
-
-        + knw: KnW object
+        Parameters
+        ----------
+        knw: KnW object
             The kernel used to find neighboring points.
         """
         if self.izl is None:
             return None
         if knw.vkernel == "nearest":
-            return copy.deepcopy(self.izl.astype(int))
+            return copy.deepcopy(self.izl)
         elif knw.vkernel in ["dz", "linear"]:
             try:
                 self.izl_lin
             except AttributeError:
-                (
-                    self.izl_lin,
-                    self.rzl_lin,
-                    self.dzl_bin,
-                    self.bzl_lin,
-                ) = self.ocedata.find_rel_vl_lin(self.dep)
-            return np.vstack([self.izl_lin.astype(int), self.izl_lin.astype(int) - 1]).T
+                self.rel.update(self.ocedata.find_rel_vl_lin(self.dep))
+            return np.vstack([self.izl_lin, self.izl_lin - 1]).T
         else:
             raise ValueError("vkernel not supported")
 
     def fatten_t(self, knw):
         """Fatten in the temporal coord.
 
         Finding the neighboring center grid points in the temporal dimension.
 
-        **Parameters:**
-
-        + knw: KnW object
+        Parameters
+        ----------
+        knw: KnW object
             The kernel used to find neighboring points.
         """
         if self.it is None:
             return None
         if knw.tkernel == "nearest":
-            return copy.deepcopy(self.it.astype(int))
+            return copy.deepcopy(self.it)
         elif knw.tkernel in ["dt", "linear"]:
             try:
                 self.izl_lin
             except AttributeError:
-                (
-                    self.it_lin,
-                    self.rt_lin,
-                    self.dt_bin,
-                    self.bt_lin,
-                ) = self.ocedata.find_rel_t_lin(self.t)
-            return np.vstack([self.it_lin.astype(int), self.it_lin.astype(int) + 1]).T
+                self.rel.update(self.ocedata.find_rel_t_lin(self.t))
+            return np.vstack([self.it_lin, self.it_lin + 1]).T
         else:
             raise ValueError("tkernel not supported")
 
-    def fatten(self, knw, fourD=False, required="all", ind_moves_kwarg={}):
+    def fatten(self, knw, four_d=False, required="all", ind_moves_kwarg={}):
         """Fatten in all the required dimensions.
 
         Finding the neighboring center grid points in all 4 dimensions.
 
-        **Parameters:**
-
-        + knw: KnW object
+        Parameters
+        ----------
+        knw: KnW object
             The kernel used to find neighboring points.
-        + fourD: Boolean
+        four_d: Boolean, default False
             When we are doing nearest neighbor interpolation on some of the dimensions,
-            with fourD = True, this will create dimensions with length 1, and will squeeze
-            the dimension if fourD = False
-        + required: str, iterable of str
+            with four_d = True, this will create dimensions with length 1, and will squeeze
+            the dimension if four_d = False
+        required: str, iterable of str, default "all"
             Which dims is needed in the process
-        + ind_moves_kward: dict
-            Key word argument to put into ind_moves method of the topology object.
-            Read topology.ind_moves for more detail.
+        ind_moves_kward: dict, optional
+            Key word argument to put into ind_moves method of the Topology object.
+            Read Topology.ind_moves for more detail.
         """
         if required != "all" and isinstance(required, str):
             required = tuple([required])
         if required == "all" or isinstance(required, tuple):
             pass
         else:
             required = tuple(required)
@@ -439,265 +433,231 @@
         if (
             _in_required("X", required)
             or _in_required("Y", required)
             or _in_required("face", required)
         ):
             ffc, fiy, fix = self.fatten_h(knw, ind_moves_kwarg=ind_moves_kwarg)
             if ffc is not None:
-                R = (ffc, fiy, fix)
+                to_return = (ffc, fiy, fix)
                 keys = ["face", "Y", "X"]
             else:
-                R = (fiy, fix)
+                to_return = (fiy, fix)
                 keys = ["Y", "X"]
         else:
-            R = tuple([np.zeros(self.N)])
+            to_return = tuple([np.zeros(self.N)])
             keys = ["place_holder"]
 
         if _in_required("Z", required):
             fiz = self.fatten_v(knw)
             if fiz is not None:
-                R = _ind_broadcast(fiz, R)
+                to_return = _ind_broadcast(fiz, to_return)
                 keys.insert(0, "Z")
         elif _in_required("Zl", required):
             fizl = self.fatten_vl(knw)
             if fizl is not None:
-                R = _ind_broadcast(fizl, R)
+                to_return = _ind_broadcast(fizl, to_return)
                 keys.insert(0, "Zl")
-        elif fourD:
-            R = [np.expand_dims(R[i], axis=-1) for i in range(len(R))]
+        elif four_d:
+            to_return = [
+                np.expand_dims(to_return[i], axis=-1) for i in range(len(to_return))
+            ]
 
         if _in_required("time", required):
             fit = self.fatten_t(knw)
             if fit is not None:
-                R = _ind_broadcast(fit, R)
+                to_return = _ind_broadcast(fit, to_return)
                 keys.insert(0, "time")
-        elif fourD:
-            R = [np.expand_dims(R[i], axis=-1) for i in range(len(R))]
-        R = dict(zip(keys, R))
+        elif four_d:
+            to_return = [
+                np.expand_dims(to_return[i], axis=-1) for i in range(len(to_return))
+            ]
+        to_return = dict(zip(keys, to_return))
         if required == "all":
             required = [i for i in keys if i != "place_holder"]
-        return tuple([R[i] for i in required])
+        return tuple(to_return[i] for i in required)
 
     def get_px_py(self):
         """Get the nearest 4 corner points of the given point.
 
         Used for oceanparcel style horizontal interpolation.
         """
         if self.face is not None:
-            return find_px_py(
-                self.ocedata.XG,
-                self.ocedata.YG,
-                self.ocedata.tp,
+            ind = (
                 self.face,
                 self.iy,
                 self.ix,
             )
         else:
-            return find_px_py(
-                self.ocedata.XG, self.ocedata.YG, self.ocedata.tp, self.iy, self.ix
-            )
+            ind = (self.iy, self.ix)
+        px, py = find_px_py(
+            self.ocedata.XG,
+            self.ocedata.YG,
+            self.ocedata.tp,
+            ind,
+        )
+        px = self.lon + to_180(px - self.lon)
+        return px, py
 
     def get_f_node_weight(self):
         """Find weight for the corner points interpolation."""
         return weight_f_node(self.rx, self.ry)
 
-    def _get_lon_lat(self):  # pragma: no cover
-        """Return the lat-lon value based on relative coordinate.
-
-        This method only work if the dataset has readiness['h'] == 'oceanparcel'.
-        """
-        px, py = self.get_px_py()
-        w = self.get_f_node_weight()
-        lon = np.einsum("nj,nj->n", w, px.T)
-        lat = np.einsum("nj,nj->n", w, py.T)
-        return lon, lat
-
-    def _get_needed(
-        self, varName, knw, required=None, prefetched=None, **kwarg
-    ):  # pragma: no cover
-        if required is None:
-            required = self.ocedata._ds[varName].dims
-        ind = self.fatten(knw, required=required, **kwarg)
-        if len(ind) != len(self.ocedata._ds[varName].dims):
-            raise Exception(
-                """dimension mismatch.
-                            Please check if the position objects have all the dimensions needed"""
-            )
-        if prefetched is None:
-            return sread(self.ocedata[varName], ind)
-        else:
-            return prefetched[ind]
-
-    def _get_masked(self, knw, gridtype="C", **kwarg):  # pragma: no cover
-        ind = self.fatten(knw, fourD=True, **kwarg)
-        if self.it is not None:
-            ind = ind[1:]
-        if len(ind) != len(self.ocedata._ds["maskC"].dims):
-            raise Exception(
-                """dimension mismatch.
-                            Please check if the position objects have all the dimensions needed"""
-            )
-        return get_masked(self.ocedata, ind, gridtype=gridtype)
-
-    def _find_pk4d(self, knw, gridtype="C"):  # pragma: no cover
-        masked = self._get_masked(knw, gridtype=gridtype)
-        pk4d = find_pk_4d(masked, russian_doll=knw.inheritance)
-        return pk4d
-
-    def _register_interpolation_input(self, varName, knw, prefetched=None, i_min=None):
+    def _register_interpolation_input(
+        self, var_name, knw, prefetched=None, prefetch_prefix=None
+    ):
         """Register the input of interpolation function.
 
         Part of the interpolation function.
         Register the input of the interpolation function.
         For the input format, go to interpolation for more details.
 
-        **Returns:**
-
-        + output_format: dict
-            Record information about the original varName input.
+        Returns
+        -------
+        output_format: dict
+            Record information about the original var_name input.
             Provide the formatting information for output,
             such that it matches the input in a direct fashion.
-        + main_keys: list
+        main_keys: list
             A list that defines each interpolation to be performed.
             The combination of variable name and kernel uniquely define such an operation.
-        + prefetch_dict: dict
+        prefetch_dict: dict
             Lookup the prefetched the data and its index prefix using main_key
-        + main_dict: dict
+        main_dict: dict
             Lookup the raw information using main_key
-        + hash_index: dict
+        hash_index: dict
             Lookup the token that uniquely define its indexing operation using main_key.
             Different main_key could share the same token.
-        + hash_mask: dict
+        hash_mask: dict
             Lookup the token that uniquely define its masking operation using main_key.
             Different main_key could share the same token.
-        + hash_read: dict
+        hash_read: dict
             Lookup the token that uniquely define its reading of the data using main_key.
             Different main_key could share the same token.
-        + hash_weight: dict
+        hash_weight: dict
             Lookup the token that uniquely define its computation of the weight using main_key.
             Different main_key could share the same token.
         """
-        # prefetch_dict = {var:(prefetched,i_min)}
+        # prefetch_dict = {var:(prefetched,prefetch_prefix)}
         # main_dict = {var:(var,kernel)}
-        # hash_index = {var:hash(cuvg,kernel_size)}
+        # hash_index = {var:hash(cuvwg,kernel_size)}
         # hash_read  = {var:hash(var,kernel_size)}
-        # hash_weight= {var:hash(kernel,cuvg)}
+        # hash_weight= {var:hash(kernel,cuvwg)}
         output_format = {}
-        if isinstance(varName, str) or isinstance(varName, tuple):
-            varName = [varName]
+        if isinstance(var_name, (str, tuple)):
+            var_name = [var_name]
             output_format["single"] = True
-        elif isinstance(varName, list):
+        elif isinstance(var_name, list):
             output_format["single"] = False
         else:
             raise ValueError(
-                "varName needs to be string, tuple, or a list of the above."
+                "var_name needs to be string, tuple, or a list of the above."
             )
-        Nvar = len(varName)
+        num_var = len(var_name)
 
         if isinstance(knw, KnW):
-            knw = [knw for i in range(Nvar)]
+            knw = [knw for i in range(num_var)]
         if isinstance(knw, tuple):
             if len(knw) != 2:
                 raise ValueError(
                     "When knw is a tuple, we assume it to be kernels for a horizontal vector,"
                     "thus, it has to have 2 elements"
                 )
-            knw = [knw for i in range(Nvar)]
+            knw = [knw for i in range(num_var)]
         elif isinstance(knw, list):
-            if len(knw) != Nvar:
+            if len(knw) != num_var:
                 raise ValueError("Mismatch between the number of kernels and variables")
         elif isinstance(knw, dict):
             temp = []
-            for var in varName:
+            for var in var_name:
                 a_knw = knw.get(var)
-                if (a_knw is None) or not (isinstance(a_knw, (tuple, KnW))):
+                if a_knw is None or not isinstance(a_knw, (tuple, KnW)):
                     raise ValueError(
                         f"Variable {var} does not have a proper corresponding kernel"
                     )
                 else:
                     temp.append(a_knw)
             knw = temp
         else:
             raise ValueError(
                 "knw needs to be a KnW object, or list/dictionaries containing that "
             )
 
         if isinstance(prefetched, np.ndarray):
-            prefetched = [prefetched for i in range(Nvar)]
+            prefetched = [prefetched for i in range(num_var)]
         elif isinstance(prefetched, tuple):
-            prefetched = [prefetched for i in range(Nvar)]
+            prefetched = [prefetched for i in range(num_var)]
         elif prefetched is None:
-            prefetched = [prefetched for i in range(Nvar)]
+            prefetched = [prefetched for i in range(num_var)]
         elif isinstance(prefetched, list):
-            if len(prefetched) != Nvar:
+            if len(prefetched) != num_var:
                 raise ValueError(
                     "Mismatch between the number of prefetched arrays and variables"
                 )
         elif isinstance(prefetched, dict):
-            prefetched = [prefetched.get(var) for var in varName]
+            prefetched = [prefetched.get(var) for var in var_name]
         else:
             raise ValueError(
                 "prefetched needs to be a numpy array/tuple pair of numpy array,"
                 " or list/dictionaries containing that"
             )
 
-        if isinstance(i_min, tuple):
-            i_min = [i_min for i in range(Nvar)]
-        elif i_min is None:
-            i_min = [None for i in range(Nvar)]
-        elif isinstance(i_min, list):
-            if len(i_min) != Nvar:
+        if isinstance(prefetch_prefix, tuple):
+            prefetch_prefix = [prefetch_prefix for i in range(num_var)]
+        elif prefetch_prefix is None:
+            prefetch_prefix = [None for i in range(num_var)]
+        elif isinstance(prefetch_prefix, list):
+            if len(prefetch_prefix) != num_var:
                 raise ValueError(
-                    "Mismatch between the number of prefetched arrays prefix i_min and variables"
+                    "Mismatch between the number of prefetched arrays prefix prefetch_prefix and variables"
                 )
-        elif isinstance(i_min, dict):
-            i_min = [i_min.get(var) for var in varName]
+        elif isinstance(prefetch_prefix, dict):
+            prefetch_prefix = [prefetch_prefix.get(var) for var in var_name]
         else:
             raise ValueError(
-                "prefetched prefix i_min needs to be a tuple, or list/dictionaries containing that "
+                "prefetched prefix prefetch_prefix needs to be a tuple, or list/dictionaries containing that "
             )
 
-        output_format["ori_list"] = copy.deepcopy(list(zip(varName, knw)))
-        new_varName = []
+        output_format["ori_list"] = copy.deepcopy(list(zip(var_name, knw)))
+        new_var_name = []
         new_prefetched = []
         new_knw = []
-        new_i_min = []
-        for i, var in enumerate(varName):
+        new_prefetch_prefix = []
+        for i, var in enumerate(var_name):
             if isinstance(var, str):
-                new_varName.append(var)
+                new_var_name.append(var)
                 new_prefetched.append(prefetched[i])
                 new_knw.append(knw[i])
-                new_i_min.append(i_min[i])
+                new_prefetch_prefix.append(prefetch_prefix[i])
             elif isinstance(var, tuple):
                 if self.face is None:
                     for j in range(len(var)):
-                        new_varName.append(var[j])
+                        new_var_name.append(var[j])
                         if prefetched[i] is not None:
                             new_prefetched.append(prefetched[i][j])
                         else:
                             new_prefetched.append(None)
                         new_knw.append(knw[i][j])
-                        new_i_min.append(i_min[i])
+                        new_prefetch_prefix.append(prefetch_prefix[i])
                 else:
-                    new_varName.append(var)
+                    new_var_name.append(var)
                     new_prefetched.append(prefetched[i])
                     new_knw.append(knw[i])
-                    new_i_min.append(i_min[i])
+                    new_prefetch_prefix.append(prefetch_prefix[i])
             elif var is None:
                 pass
             else:
                 raise ValueError(
-                    "varName needs to be string, tuple, or a list of the above."
+                    "var_name needs to be string, tuple, or a list of the above."
                 )
 
         prefetched = new_prefetched
         knw = new_knw
-        i_min = new_i_min
-        varName = new_varName
-        output_format["final_varName"] = list(zip(varName, knw))
+        prefetch_prefix = new_prefetch_prefix
+        var_name = new_var_name
+        output_format["final_var_name"] = list(zip(var_name, knw))
 
         kernel_size_hash = []
         kernel_hash = []
         mask_ignore = []
         for kkk in knw:
             if isinstance(kkk, KnW):
                 kernel_size_hash.append(kkk.size_hash())
@@ -706,43 +666,38 @@
             elif isinstance(kkk, tuple):
                 if len(kkk) != 2:
                     raise ValueError(
                         "When knw is a tuple, we assume it to be kernels for a horizontal vector,"
                         "thus, it has to have 2 elements"
                     )
                 uknw, vknw = kkk
-                # if not uknw.same_size(vknw):
-                #     raise Exception('u,v kernel needs to have same size'
-                #                     'to navigate the complex grid orientation.'
-                #                     'use a kernel that include both of the uv kernels'
-                #                    )
                 kernel_size_hash.append(uknw.size_hash())
                 kernel_hash.append(hash((uknw, vknw)))
                 mask_ignore.append(uknw.ignore_mask or vknw.ignore_mask)
         dims = []
-        for var in varName:
+        for var in var_name:
             if isinstance(var, str):
                 dims.append(self.ocedata[var].dims)
             elif isinstance(var, tuple):
                 temp = []
                 for vvv in var:
                     temp.append(self.ocedata[vvv].dims)
                 dims.append(tuple(temp))
 
-        main_keys = list(zip(varName, kernel_hash))
-        prefetch_dict = dict(zip(main_keys, zip(prefetched, i_min)))
-        main_dict = dict(zip(main_keys, zip(varName, dims, knw)))
+        main_keys = list(zip(var_name, kernel_hash))
+        prefetch_dict = dict(zip(main_keys, zip(prefetched, prefetch_prefix)))
+        main_dict = dict(zip(main_keys, zip(var_name, dims, knw)))
         hash_index = dict(
             zip(main_keys, [hash(i) for i in zip(dims, kernel_size_hash)])
         )
         hash_mask = dict(
             zip(main_keys, [hash(i) for i in zip(dims, mask_ignore, kernel_size_hash)])
         )
         hash_read = dict(
-            zip(main_keys, [hash(i) for i in zip(varName, kernel_size_hash)])
+            zip(main_keys, [hash(i) for i in zip(var_name, kernel_size_hash)])
         )
         hash_weight = dict(zip(main_keys, [hash(i) for i in zip(dims, kernel_hash)]))
         return (
             output_format,
             main_keys,
             prefetch_dict,
             main_dict,
@@ -753,94 +708,100 @@
         )
 
     def _fatten_required_index_and_register(self, hash_index, main_dict):
         """Fatten for the interpolation process.
 
         Perform the fatten process for each unique token. Register the result as a dict.
 
-        **Parameters:**
-
-        + hash_index: dict
+        Parameters
+        ----------
+        hash_index: dict
             See _register_interpolation_input
-        + main_dict: dict
+        main_dict: dict
             See _register_interpolation_input
 
-        **Returns:**
-
+        Returns
+        -------
         + index_lookup: dict
             A dictionary to lookup fatten results.
             The keys are the token in hash_index.
             The values are corresponding results.
         """
         hsh = np.unique(list(hash_index.values()))
         index_lookup = {}
         for hs in hsh:
             main_key = get_key_by_value(hash_index, hs)
-            varName, dims, knw = main_dict[main_key]
-            if isinstance(varName, str):
+            var_name, dims, knw = main_dict[main_key]
+            if isinstance(var_name, str):
                 old_dims = dims
-            elif isinstance(varName, tuple):
+            elif isinstance(var_name, tuple):
                 old_dims = dims[0]
             dims = []
             for i in old_dims:
                 if i in ["Xp1", "Yp1"]:
                     dims.append(i[:1])
                 else:
                     dims.append(i)
             dims = tuple(dims)
-            if isinstance(varName, str):
-                ind = self.fatten(knw, required=dims, fourD=True)
+            if isinstance(var_name, str):
+                if "Xp1" in old_dims and "Yp1" in old_dims:
+                    cuvwg = "G"
+                else:
+                    cuvwg = "C"
+                ind = self.fatten(
+                    knw, required=dims, four_d=True, ind_moves_kwarg={"cuvwg": cuvwg}
+                )
                 index_lookup[hs] = ind
-            elif isinstance(varName, tuple):
+            elif isinstance(var_name, tuple):
                 uknw, vknw = knw
                 uind = self.fatten(
-                    uknw, required=dims, fourD=True, ind_moves_kwarg={"cuvg": "U"}
+                    uknw, required=dims, four_d=True, ind_moves_kwarg={"cuvwg": "U"}
                 )
                 vind = self.fatten(
-                    vknw, required=dims, fourD=True, ind_moves_kwarg={"cuvg": "V"}
+                    vknw, required=dims, four_d=True, ind_moves_kwarg={"cuvwg": "V"}
                 )
                 index_lookup[hs] = (uind, vind)
 
         return index_lookup
 
     def _transform_vector_and_register(self, index_lookup, hash_index, main_dict):
         """Transform vectors for interpolation.
 
         Perform the vector transformation.
         This is to say that sometimes u velocity becomes v velocity for datasets with face topology.
           Register the result as a dict.
 
-        **Parameters:**
-
-        + index_lookup: dict
+        Parameters
+        ----------
+        index_lookup: dict
             See _fatten_required_index_and_register
-        + hash_index: dict
+        hash_index: dict
             See _register_interpolation_input
-        + main_dict: dict
+        main_dict: dict
             See _register_interpolation_input
 
-        **Returns:**
-
+        Returns
+        -------
         + transform_lookup: dict
             A dictionary to lookup transformation results.
             The keys are the token in hash_index.
             The values are corresponding results.
         """
         hsh = np.unique(list(hash_index.values()))
         transform_lookup = {}
         if self.face is None:
             for hs in hsh:
                 transform_lookup[hs] = None
             return transform_lookup
         for hs in hsh:
             main_key = get_key_by_value(hash_index, hs)
-            varName, dims, knw = main_dict[main_key]
-            if isinstance(varName, str):
+            var_name, dims, knw = main_dict[main_key]
+            if isinstance(var_name, str):
                 transform_lookup[hs] = None
-            elif isinstance(varName, tuple):
+            elif isinstance(var_name, tuple):
                 uind, vind = index_lookup[hs]
                 uind_dic = dict(zip(dims[0], uind))
                 vind_dic = dict(zip(dims[1], vind))
                 # This only matters when dim == 'face', no need to think about 'Xp1'
                 (UfromUvel, UfromVvel, _, _) = self.ocedata.tp.four_matrix_for_uv(
                     uind_dic["face"][:, :, 0, 0]
                 )
@@ -855,18 +816,18 @@
                 VfromVvel = np.round(VfromVvel)
 
                 bool_ufromu = np.abs(UfromUvel).astype(bool)
                 bool_ufromv = np.abs(UfromVvel).astype(bool)
                 bool_vfromu = np.abs(VfromUvel).astype(bool)
                 bool_vfromv = np.abs(VfromVvel).astype(bool)
 
-                indufromu = tuple([idid[bool_ufromu] for idid in uind])
-                indufromv = tuple([idid[bool_ufromv] for idid in uind])
-                indvfromu = tuple([idid[bool_vfromu] for idid in vind])
-                indvfromv = tuple([idid[bool_vfromv] for idid in vind])
+                indufromu = tuple(idid[bool_ufromu] for idid in uind)
+                indufromv = tuple(idid[bool_ufromv] for idid in uind)
+                indvfromu = tuple(idid[bool_vfromu] for idid in vind)
+                indvfromv = tuple(idid[bool_vfromv] for idid in vind)
 
                 transform_lookup[hs] = (
                     (UfromUvel, UfromVvel, VfromUvel, VfromVvel),
                     (bool_ufromu, bool_ufromv, bool_vfromu, bool_vfromv),
                     (indufromu, indufromv, indvfromu, indvfromv),
                 )
             else:
@@ -877,49 +838,49 @@
     def _mask_value_and_register(
         self, index_lookup, transform_lookup, hash_mask, hash_index, main_dict
     ):
         """Create masks for interpolation.
 
         Perform the masking process and register in a dictionary.
 
-        **Parameters:**
-
-        + index_lookup: dict
+        Parameters
+        ----------
+        index_lookup: dict
             See _fatten_required_index_and_register
-        + transform_lookup: dict
+        transform_lookup: dict
             See _transform_vector_and_lookup
-        + hash_mask: dict
+        hash_mask: dict
             See _register_interpolation_input
-        + hash_index: dict
+        hash_index: dict
             See _register_interpolation_input
-        + main_dict: dict
+        main_dict: dict
             See _register_interpolation_input
 
-        **Returns:**
-
+        Returns
+        -------
         + mask_lookup: dict
             A dictionary to lookup masking results.
             The keys are the token in hash_mask.
             The values are corresponding results.
         """
         hsh = np.unique(list(hash_mask.values()))
         mask_lookup = {}
         for hs in hsh:
             main_key = get_key_by_value(hash_mask, hs)
-            varName, dims, knw = main_dict[main_key]
+            var_name, dims, knw = main_dict[main_key]
             hsind = hash_index[main_key]
             longDims = "".join([str(a_thing) for a_thing in dims])
             if isinstance(knw, KnW):
                 ignore_mask = knw.ignore_mask
             elif isinstance(knw, tuple):
                 ignore_mask = (knw[0].ignore_mask) or (knw[1].ignore_mask)
 
             if ignore_mask or ("X" not in longDims) or ("Y" not in longDims):
                 mask_lookup[hs] = None
-            elif isinstance(varName, str):
+            elif isinstance(var_name, str):
                 ind = index_lookup[hsind]
                 ind_for_mask = _ind_for_mask(ind, dims)
                 if "Zl" in dims:
                     cuvw = "Wvel"
                 elif "Z" in dims:
                     if "Xp1" in dims and "Yp1" in dims:
                         raise NotImplementedError(
@@ -931,44 +892,44 @@
                         cuvw = "U"
                     elif "Yp1" in dims:
                         cuvw = "V"
                     else:
                         cuvw = "C"
                 else:
                     cuvw = "C"
-                masked = get_masked(self.ocedata, ind_for_mask, gridtype=cuvw)
+                masked = get_masked(self.ocedata, ind_for_mask, cuvwg=cuvw)
                 mask_lookup[hs] = masked
-            elif isinstance(varName, tuple):
+            elif isinstance(var_name, tuple):
                 to_unzip = transform_lookup[hsind]
                 uind, vind = index_lookup[hsind]
                 if to_unzip is None:
                     uind_for_mask = _ind_for_mask(uind, dims[0])
                     vind_for_mask = _ind_for_mask(vind, dims[1])
-                    umask = get_masked(self.ocedata, uind_for_mask, gridtype="U")
-                    vmask = get_masked(self.ocedata, vind_for_mask, gridtype="V")
+                    umask = get_masked(self.ocedata, uind_for_mask, cuvwg="U")
+                    vmask = get_masked(self.ocedata, vind_for_mask, cuvwg="V")
                 else:
                     (
                         _,
                         (bool_ufromu, bool_ufromv, bool_vfromu, bool_vfromv),
                         (indufromu, indufromv, indvfromu, indvfromv),
                     ) = to_unzip
                     umask = np.full(uind[0].shape, np.nan)
                     vmask = np.full(vind[0].shape, np.nan)
 
                     umask[bool_ufromu] = get_masked(
-                        self.ocedata, _ind_for_mask(indufromu, dims[0]), gridtype="U"
+                        self.ocedata, _ind_for_mask(indufromu, dims[0]), cuvwg="U"
                     )
                     umask[bool_ufromv] = get_masked(
-                        self.ocedata, _ind_for_mask(indufromv, dims[1]), gridtype="V"
+                        self.ocedata, _ind_for_mask(indufromv, dims[1]), cuvwg="V"
                     )
                     vmask[bool_vfromu] = get_masked(
-                        self.ocedata, _ind_for_mask(indvfromu, dims[0]), gridtype="U"
+                        self.ocedata, _ind_for_mask(indvfromu, dims[0]), cuvwg="U"
                     )
                     vmask[bool_vfromv] = get_masked(
-                        self.ocedata, _ind_for_mask(indvfromv, dims[1]), gridtype="V"
+                        self.ocedata, _ind_for_mask(indvfromv, dims[1]), cuvwg="V"
                     )
                 mask_lookup[hs] = (umask, vmask)
         return mask_lookup
 
     def _read_data_and_register(
         self,
         index_lookup,
@@ -976,87 +937,89 @@
         hash_read,
         hash_index,
         main_dict,
         prefetch_dict,
     ):
         """Read the data and register them as dict.
 
-        **Parameters:**
-
-        + index_lookup: dict
+        Parameters
+        ----------
+        index_lookup: dict
             See _fatten_required_index_and_register
-        + transform_lookup: dict
+        transform_lookup: dict
             See _transform_vector_and_lookup
-        + hash_read: dict
+        hash_read: dict
             See _register_interpolation_input
-        + hash_index: dict
+        hash_index: dict
             See _register_interpolation_input
-        + main_dict: dict
+        main_dict: dict
             See _register_interpolation_input
-        + prefetch_dict: dict
+        prefetch_dict: dict
             See _register_interpolation_input
 
-        **Returns:**
-
+        Returns
+        -------
         + read_lookup: dict
             A dictionary to lookup data reading results.
             The keys are the token in hash_read.
             The values are corresponding results.
         """
         hsh = np.unique(list(hash_read.values()))
         data_lookup = {}
         for hs in hsh:
             main_key = get_key_by_value(hash_read, hs)
             hsind = hash_index[main_key]
-            varName, dims, knw = main_dict[main_key]
-            prefetched, i_min = prefetch_dict[main_key]
-            if isinstance(varName, str):
+            var_name, dims, knw = main_dict[main_key]
+            prefetched, prefetch_prefix = prefetch_dict[main_key]
+            if isinstance(var_name, str):
                 ind = index_lookup[hsind]
                 if prefetched is not None:
-                    if i_min is None:
+                    if prefetch_prefix is None:
                         raise ValueError(
                             "please pass value of the prefix of prefetched dataset, "
                             "even if the prefix is zero"
                         )
-                    temp_ind = _subtract_i_min(ind, i_min)
+                    temp_ind = _subtract_prefetch_prefix(ind, prefetch_prefix)
                     needed = np.nan_to_num(prefetched[temp_ind])
                 else:
-                    needed = np.nan_to_num(sread(self.ocedata[varName], ind))
+                    needed = np.nan_to_num(smart_read(self.ocedata[var_name], ind))
                 data_lookup[hs] = needed
-            elif isinstance(varName, tuple):
-                uname, vname = varName
+            elif isinstance(var_name, tuple):
+                uname, vname = var_name
                 uind, vind = index_lookup[hsind]
                 (
                     (UfromUvel, UfromVvel, VfromUvel, VfromVvel),
                     (bool_ufromu, bool_ufromv, bool_vfromu, bool_vfromv),
                     (indufromu, indufromv, indvfromu, indvfromv),
                 ) = transform_lookup[hsind]
                 temp_n_u = np.full(uind[0].shape, np.nan)
                 temp_n_v = np.full(vind[0].shape, np.nan)
                 if prefetched is not None:
                     upre, vpre = prefetched
-                    ufromu = np.nan_to_num(upre[_subtract_i_min(indufromu, i_min)])
-                    ufromv = np.nan_to_num(vpre[_subtract_i_min(indufromv, i_min)])
-                    vfromu = np.nan_to_num(upre[_subtract_i_min(indvfromu, i_min)])
-                    vfromv = np.nan_to_num(vpre[_subtract_i_min(indvfromv, i_min)])
+                    ufromu = np.nan_to_num(
+                        upre[_subtract_prefetch_prefix(indufromu, prefetch_prefix)]
+                    )
+                    ufromv = np.nan_to_num(
+                        vpre[_subtract_prefetch_prefix(indufromv, prefetch_prefix)]
+                    )
+                    vfromu = np.nan_to_num(
+                        upre[_subtract_prefetch_prefix(indvfromu, prefetch_prefix)]
+                    )
+                    vfromv = np.nan_to_num(
+                        vpre[_subtract_prefetch_prefix(indvfromv, prefetch_prefix)]
+                    )
                 else:
-                    ufromu = np.nan_to_num(sread(self.ocedata[uname], indufromu))
-                    ufromv = np.nan_to_num(sread(self.ocedata[vname], indufromv))
-                    vfromu = np.nan_to_num(sread(self.ocedata[uname], indvfromu))
-                    vfromv = np.nan_to_num(sread(self.ocedata[vname], indvfromv))
+                    ufromu = np.nan_to_num(smart_read(self.ocedata[uname], indufromu))
+                    ufromv = np.nan_to_num(smart_read(self.ocedata[vname], indufromv))
+                    vfromu = np.nan_to_num(smart_read(self.ocedata[uname], indvfromu))
+                    vfromv = np.nan_to_num(smart_read(self.ocedata[vname], indvfromv))
                 temp_n_u[bool_ufromu] = ufromu  # 0#
                 temp_n_u[bool_ufromv] = ufromv  # 1#
                 temp_n_v[bool_vfromu] = vfromu  # 0#
                 temp_n_v[bool_vfromv] = vfromv  # 1#
-                # dont_break = np.isclose(temp_n_v,2).any()
-                # if not dont_break:
-                #     print(bool_vfromu)
-                #     raise Exception('what is going on')
-                # else:
-                #     print('somehow it passed')
 
                 n_u = np.einsum("nijk,ni->nijk", temp_n_u, UfromUvel) + np.einsum(
                     "nijk,ni->nijk", temp_n_u, UfromVvel
                 )
                 n_v = np.einsum("nijk,ni->nijk", temp_n_v, VfromUvel) + np.einsum(
                     "nijk,ni->nijk", temp_n_v, VfromVvel
                 )
@@ -1065,40 +1028,40 @@
         return data_lookup
 
     def _compute_weight_and_register(
         self, mask_lookup, hash_weight, hash_mask, main_dict
     ):
         """Compute the weights and register them as dict.
 
-        **Parameters:**
-
-        + mask_lookup: dict
+        Parameters
+        ----------
+        mask_lookup: dict
             See _mask_value_and_register
-        + hash_weight: dict
+        hash_weight: dict
             See _register_interpolation_input
-        + hash_mask: dict
+        hash_mask: dict
             See _register_interpolation_input
-        + main_dict: dict
+        main_dict: dict
             See _register_interpolation_input
 
-        **Returns:**
-
+        Returns
+        -------
         + weight_lookup: dict
             A dictionary to lookup the weights computed.
             The keys are the token in hash_weight.
             The values are corresponding results.
         """
         hsh = np.unique(list(hash_weight.values()))
         weight_lookup = {}
         for hs in hsh:
             main_key = get_key_by_value(hash_weight, hs)
             hsmsk = hash_mask[main_key]
-            varName, dims, knw = main_dict[main_key]
+            var_name, dims, knw = main_dict[main_key]
             masked = mask_lookup[hsmsk]
-            if isinstance(varName, tuple):
+            if isinstance(var_name, tuple):
                 ori_dims = dims
                 dims = ori_dims[0]
                 ori_knw = knw
                 knw = ori_knw[0]
                 # Assuming the two kernels have the same
                 # vertical dimensions, which is reasonable.
 
@@ -1127,106 +1090,106 @@
                 if knw.tkernel == "nearest":
                     rt = self.rt
                 else:
                     rt = self.rt_lin
             else:
                 rt = 0
 
-            if isinstance(varName, str):
+            if isinstance(var_name, str):
                 if "Xp1" in dims:
                     rx = self.rx + 0.5
                 else:
                     rx = self.rx
                 if "Yp1" in dims:
                     ry = self.ry + 0.5
                 else:
                     ry = self.ry
                 if masked is None:
                     pk4d = None
                 else:
-                    pk4d = find_pk_4d(masked, russian_doll=knw.inheritance)
+                    pk4d = find_pk_4d(masked, inheritance=knw.inheritance)
                 weight = knw.get_weight(
                     rx=rx,
                     ry=ry,
                     rz=rz,
                     rt=rt,
                     pk4d=pk4d,
                     bottom_scheme=this_bottom_scheme,
                 )
                 weight_lookup[hs] = weight
-            elif isinstance(varName, tuple):
+            elif isinstance(var_name, tuple):
                 uknw, vknw = ori_knw
                 if masked is None:
                     upk4d = None
                     vpk4d = None
                 else:
                     umask, vmask = masked
-                    upk4d = find_pk_4d(umask, russian_doll=uknw.inheritance)
-                    vpk4d = find_pk_4d(vmask, russian_doll=vknw.inheritance)
+                    upk4d = find_pk_4d(umask, inheritance=uknw.inheritance)
+                    vpk4d = find_pk_4d(vmask, inheritance=vknw.inheritance)
                 uweight = uknw.get_weight(
                     self.rx + 1 / 2, self.ry, rz=rz, rt=rt, pk4d=upk4d
                 )
                 vweight = vknw.get_weight(
                     self.rx, self.ry + 1 / 2, rz=rz, rt=rt, pk4d=vpk4d
                 )
                 weight_lookup[hs] = (uweight, vweight)
         return weight_lookup
 
     def interpolate(
-        self, varName, knw, vec_transform=True, prefetched=None, i_min=None
+        self, var_name, knw, vec_transform=True, prefetched=None, prefetch_prefix=None
     ):
         """Do interpolation.
 
         This is the method that does the actual interpolation/derivative.
         It is a combination of the following methods:
         _register_interpolation_input,
         _fatten_required_index_and_register,
         _transform_vector_and_register,
         _read_data_and_register,
         _mask_value_and_register,
         _compute_weight_and_registe,.
 
-        **Parameters:**
-
-        + varName: list, str, tuple
+        Parameters
+        ----------
+        var_name: list, str, tuple
             The variables to interpolate. Tuples are used for horizontal vectors.
             Put str and list in a list if you have multiple things to interpolate.
             This input also defines the format of the output.
-        + knw: KnW object, tuple, list, dict
+        knw: KnW object, tuple, list, dict
             The kernel object used for the operation.
-            Put them in the same order as varName.
+            Put them in the same order as var_name.
             Some level of automatic broadcasting is also supported.
-        + vec_transform: Boolean
+        vec_transform: Boolean
             Whether to project the vector field to the local zonal/meridional direction.
-        + prefetched: numpy.ndarray, tuple, list, dict, None
-            The prefetched array for the data, this will effectively overwrite varName.
-            Put them in the same order as varName.
+        prefetched: numpy.ndarray, tuple, list, dict, None, default None
+            The prefetched array for the data, this will effectively overwrite var_name.
+            Put them in the same order as var_name.
             Some level of automatic broadcasting is also supported.
-        + i_min: tuple, list, dict, None
+        prefetch_prefix: tuple, list, dict, None, default None
             The prefix of the prefetched array.
-            Put them in the same order as varName.
+            Put them in the same order as var_name.
             Some level of automatic broadcasting is also supported.
 
-        **Returns:**
-
-        + R: list, numpy.array, tuple
-            The interpolation/derivative output in the same format as varName.
+        Returns
+        -------
+        to_return: list, numpy.array, tuple
+            The interpolation/derivative output in the same format as var_name.
         """
-        R = []
+        to_return = []
         (
             output_format,
             main_keys,
             prefetch_dict,
             main_dict,
             hash_index,
             hash_mask,
             hash_read,
             hash_weight,
         ) = self._register_interpolation_input(
-            varName, knw, prefetched=prefetched, i_min=i_min
+            var_name, knw, prefetched=prefetched, prefetch_prefix=prefetch_prefix
         )
         index_lookup = self._fatten_required_index_and_register(hash_index, main_dict)
         transform_lookup = self._transform_vector_and_register(
             index_lookup, hash_index, main_dict
         )
         data_lookup = self._read_data_and_register(
             index_lookup,
@@ -1240,42 +1203,42 @@
             index_lookup, transform_lookup, hash_mask, hash_index, main_dict
         )
         weight_lookup = self._compute_weight_and_register(
             mask_lookup, hash_weight, hash_mask, main_dict
         )
         # index_list = []
         for key in main_keys:
-            varName, dims, knw = main_dict[key]
-            if isinstance(varName, str):
+            var_name, dims, knw = main_dict[key]
+            if isinstance(var_name, str):
                 needed = data_lookup[hash_read[key]]
                 weight = weight_lookup[hash_weight[key]]
                 needed = _partial_flatten(needed)
                 weight = _partial_flatten(weight)
-                R.append(np.einsum("nj,nj->n", needed, weight))
+                to_return.append(np.einsum("nj,nj->n", needed, weight))
                 # index_list.append((index_lookup[hash_index[key]],
                 #                    transform_lookup[hash_index[key]],
                 #                    data_lookup[hash_read[key]]))
-            elif isinstance(varName, tuple):
+            elif isinstance(var_name, tuple):
                 n_u, n_v = data_lookup[hash_read[key]]
                 uweight, vweight = weight_lookup[hash_weight[key]]
                 u = np.einsum("nijk,nijk->n", n_u, uweight)
                 v = np.einsum("nijk,nijk->n", n_v, vweight)
                 if vec_transform:
                     u, v = local_to_latlon(u, v, self.cs, self.sn)
-                R.append((u, v))
+                to_return.append((u, v))
                 # index_list.append((index_lookup[hash_index[key]],
                 #                    transform_lookup[hash_index[key]],
                 #                    data_lookup[hash_read[key]]))
             else:
-                raise ValueError(f"unexpected varName: {varName}")
+                raise ValueError(f"unexpected var_name: {var_name}")
 
-        final_dict = dict(zip(output_format["final_varName"], R))
+        final_dict = dict(zip(output_format["final_var_name"], to_return))
         ori_list = output_format["ori_list"]
         output = []
-        # print(ori_list,R,final_dict.keys())
+        # print(ori_list,to_return,final_dict.keys())
         for key in ori_list:
             var, knw = key
 
             if var is None:
                 output.append(None)
             elif isinstance(var, tuple):
                 if self.face is None:
```

### Comparing `seaduck-0.1.2/seaduck/get_masks.py` & `seaduck-0.1.3/seaduck/get_masks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,81 @@
 import copy
 import logging
 import warnings
 
 import numpy as np
 import xarray as xr
 
+from seaduck.ocedata import RelCoord
 from seaduck.smart_read import smart_read
 
-# from seaduck.topology import topology
-
 
 def mask_u_node(maskC, tp):
     """Mask out U-points.
 
     for MITgcm indexing, U is defined on the left of the cell,
     When the C grid is dry, U are either:
     a. dry;
     b. on the interface, where the cell to the left is wet.
     if b is the case, we need to unmask the udata, because it makes some physical sense.
 
-    **Parameters:**
-
-    + maskC: numpy.ndarray
+    Parameters
+    ----------
+    maskC: numpy.ndarray
         numpy array with the same shape as the model spacial coordinates.
         1 for wet cells (center points), 0 for dry ones.
-    + tp: topology object
-        The topology object for the dataset.
+    tp: Topology object
+        The Topology object for the dataset.
 
-    **Returns:**
-
-    + maskU: numpy.ndarray
+    Returns
+    -------
+    maskU: numpy.ndarray
         numpy array with the same shape as the model spacial coordinates.
         1 for wet U-walls (including interface between wet and dry), 0 for dry ones.
     """
     maskU = copy.deepcopy(maskC)
     indexes = np.array(np.where(maskC == 0)).T
     # find out which points are masked will make the search faster.
-    nind = tp.ind_tend_vec(indexes.T[1:], np.ones_like(indexes.T[0], int) * 2)
-    nind = np.vstack([indexes.T[0], nind])
-    switch = indexes[np.where(maskC[tuple(nind)])]
+    new_ind = tp.ind_tend_vec(indexes.T[1:], np.ones_like(indexes.T[0], int) * 2)
+    new_ind = np.vstack([indexes.T[0], new_ind])
+    switch = indexes[np.where(maskC[tuple(new_ind)])]
     maskU[tuple(switch.T)] = 1
 
     return maskU
 
 
 def mask_v_node(maskC, tp):
     """Mask out v-points.
 
     for MITgcm indexing, V is defined on the "south" side of the cell,
     When the C grid is dry, V are either:
     a. dry;
     b. on the interface, where the cell to the downside is wet.
     if b is the case, we need to unmask the vdata.
 
-    **Parameters:**
-
-    + maskC: numpy.ndarray
+    Parameters
+    ----------
+    maskC: numpy.ndarray
         numpy array with the same shape as the model spacial coordinates.
         1 for wet cells (center points), 0 for dry ones.
-    + tp: topology object
-        The topology object for the dataset.
-
-    **Returns:**
+    tp: Topology object
+        The Topology object for the dataset.
 
+    Returns
+    -------
     + maskV: numpy.ndarray
         numpy array with the same shape as the model spacial coordinates.
         1 for wet W-walls (including interface between wet and dry), 0 for dry ones.
     """
     maskV = copy.deepcopy(maskC)
     indexes = np.array(np.where(maskC == 0)).T
     # find out which points are masked will make the search faster.
-    nind = tp.ind_tend_vec(indexes.T[1:], np.ones_like(indexes.T[0], int) * 1)
-    nind = np.vstack([indexes.T[0], nind])
-    switch = indexes[np.where(maskC[tuple(nind)])]
+    new_ind = tp.ind_tend_vec(indexes.T[1:], np.ones_like(indexes.T[0], int) * 1)
+    new_ind = np.vstack([indexes.T[0], new_ind])
+    switch = indexes[np.where(maskC[tuple(new_ind)])]
     maskV[tuple(switch.T)] = 1
     return maskV
 
 
 def mask_w_node(maskC, tp=None):
     # this one does not need tp object
     # if you pass something into it by mistake, it will be ignored.
@@ -84,58 +83,57 @@
 
     for MITgcm indexing, W is defined on the top of the cell,
     When the C grid is dry, W are either:
     a. dry;
     b. on the interface, where the cell above is wet.
     if b is the case, we need to unmask the wdata.
 
-    **Parameters:**
-
-    + maskC: numpy.ndarray
+    Parameters
+    ----------
+    maskC: numpy.ndarray
         numpy array with the same shape as the model spacial coordinates.
         1 for wet cells (center points), 0 for dry ones.
-    + tp: topology object
-        The topology object for the dataset.
-
-    **Returns:**
+    tp: Topology object
+        The Topology object for the dataset.
 
+    Returns
+    -------
     + maskWvel: numpy.ndarray
         numpy array with the same shape as the model spacial coordinates.
         1 for wet W-walls (including interface between wet and dry), 0 for dry ones.
     """
-    temp = np.zeros_like(maskC)
-    temp[1:] = maskC[:-1]
-    maskW = np.logical_or(temp, maskC).astype(int)
+    maskW = np.zeros_like(maskC)
+    maskW[1:] = maskC[:-1]
+    maskW = np.logical_or(maskW, maskC).astype(int)
     return maskW
 
 
-def get_masks(od, tp):
+def get_mask_arrays(od):
     """Mask all staggered valocity points.
 
     A wrapper around mask_u_node, mask_v_node, mask_w_node.
     If there is no maskC in the dataset, just return nothing is masked.
 
-    **Parameters:**
-
-    + od: OceData object
+    Parameters
+    ----------
+    od: OceData object
         The dataset to compute masks on.
-    + tp: topology object
-        The topology of the datset
+    tp: Topology object
+        The Topology of the datset
 
-    **Returns:**
-
-    + maskC,maskU,maskV,maskW: numpy.ndarray
+    Returns
+    -------
+    maskC,maskU,maskV,maskW: numpy.ndarray
         masks at center points, U-walls, V-walls, W-walls respectively.
     """
-    # tp = topology(od)
+    tp = od.tp
     keys = od._ds.keys()
     if "maskC" not in keys:
         warnings.warn("no maskC in the dataset, assuming nothing is masked.")
         logging.warning("no maskC in the dataset, assuming nothing is masked.")
-        # od._ds.C_GRID_VARIABLE.to_masked_array().mask
         maskC = np.ones_like(od._ds.XC + od._ds.Z)
         # it is inappropriate to fill in the dataset,
         # expecially given that there is no performance boost.
         return maskC, maskC, maskC, maskC
     maskC = np.array(od._ds["maskC"])
     if "Z" not in od._ds["maskC"].dims:
         raise NotImplementedError(
@@ -164,53 +162,87 @@
         od._ds["maskWvel"] = od._ds["Z"] + od._ds["YC"]
         od._ds["maskWvel"].values = maskW
     else:
         maskW = np.array(od._ds["maskWvel"])
     return maskC, maskU, maskV, maskW
 
 
-def get_masked(od, ind, gridtype="C"):
+def get_masked(od, ind, cuvwg="C"):
     """Return whether points are masked.
 
     Return whether the indexes of intersts are masked or not.
 
-    **Parameters:**
-
-    + od: OceData object
+    Parameters
+    ----------
+    od: OceData object
         Dataset to find mask values from.
-    + ind: tuple of numpy.ndarray
+    ind: tuple of numpy.ndarray
         Indexes of grid points.
-    + gridtype: str
+    cuvwg: str
         Whether the indexes is for points at center points or on the walls.
         Options are: ['C','U','V','Wvel'].
     """
-    if gridtype not in ["C", "U", "V", "Wvel"]:
-        raise NotImplementedError("gridtype for mask not supported")
+    if cuvwg not in ["C", "U", "V", "Wvel"]:
+        raise NotImplementedError(
+            "cuvwg(the kind of grid point) for mask not supported"
+        )
     keys = od._ds.keys()
     if "maskC" not in keys:
         warnings.warn("no maskC in the dataset, assuming nothing is masked.")
         return np.ones_like(ind[0])
-    elif gridtype == "C":
+    elif cuvwg == "C":
         return smart_read(od._ds.maskC, ind)
 
-    name = "mask" + gridtype
+    name = "mask" + cuvwg
     tp = od.tp
     maskC = np.array(od._ds["maskC"])
     func_dic = {"U": mask_u_node, "V": mask_v_node, "Wvel": mask_w_node}
     rename_dic = {
         "U": lambda x: x if x != "X" else "Xp1",
         "V": lambda x: x if x != "Y" else "Xp1",
         "Wvel": lambda x: x if x != "Z" else "Zl",
     }
     if name not in keys:
-        small_mask = func_dic[gridtype](maskC, tp)
-        dims = tuple(map(rename_dic[gridtype], od._ds.maskC.dims))
-        sizes = tuple([len(od._ds[dim]) for dim in dims])
+        small_mask = func_dic[cuvwg](maskC, tp)
+        dims = tuple(map(rename_dic[cuvwg], od._ds.maskC.dims))
+        sizes = tuple(len(od._ds[dim]) for dim in dims)
         mask = np.zeros(sizes)
         # indexing sensitive
         old_size = small_mask.shape
-        slices = tuple([slice(0, i) for i in old_size])
+        slices = tuple(slice(0, i) for i in old_size)
         mask[slices] = small_mask
         od._ds[name] = xr.DataArray(mask, dims=dims)
         return mask[ind]
     else:
         return smart_read(od._ds[name], ind)
+
+
+def which_not_stuck(p):
+    """Investigate which points are in land mask."""
+    ind = []
+    if p.izl_lin is not None:
+        ind.append(p.izl_lin - 1)
+    if p.face is not None:
+        ind.append(p.face)
+    ind += [p.iy, p.ix]
+    ind = tuple(ind)
+    return get_masked(p.ocedata, ind).astype(bool)
+
+
+def abandon_stuck(p):
+    """Abandon those stucked in mud."""
+    which = which_not_stuck(p)
+    vardict = vars(p)
+    keys = vardict.keys()
+    for i in keys:
+        item = vardict[i]
+        if isinstance(item, np.ndarray):
+            if len(item.shape) == 1:
+                setattr(p, i, item[which])
+                p.N = len(getattr(p, i))
+            else:
+                setattr(p, i, item)
+        elif isinstance(item, RelCoord):
+            setattr(p, i, item.subset(which))
+        else:
+            setattr(p, i, item)
+    return p
```

### Comparing `seaduck-0.1.2/seaduck/kernel_weight.py` & `seaduck-0.1.3/seaduck/kernel_weight.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 import copy
 import logging
+from functools import cache
+from itertools import combinations
 
 import numpy as np
 
 from seaduck.runtime_conf import compileable
-from seaduck.utils import get_combination
 
 # default kernel for interpolation.
-default_kernel = np.array(
+DEFAULT_KERNEL = np.array(
     [[0, 0], [0, 1], [0, 2], [0, -1], [0, -2], [-1, 0], [-2, 0], [1, 0], [2, 0]]
 )
-default_inheritance = [
+DEFAULT_INHERITANCE = [
     [0, 1, 2, 3, 4, 5, 6, 7, 8],
     [0, 1, 2, 3, 5, 7, 8],
     [0, 1, 3, 5, 7],
     [0],
 ]
-weight_func: dict[int, str] = {}
 
-default_kernels = [
-    np.array([default_kernel[i] for i in doll]) for doll in default_inheritance
+DEFAULT_KERNELS = [
+    np.array([DEFAULT_KERNEL[i] for i in doll]) for doll in DEFAULT_INHERITANCE
 ]
 
 
 # It just tell you what the kernels look like
-def show_kernels(kernels=default_kernels):
+def show_kernels(kernels=DEFAULT_KERNELS):
     """Plot a small scatter plot of the shape of a list of kernel.
 
-    **Parameters:**
-
-    + kernels: list of numpy.ndarray
+    Parameters
+    ----------
+    kernels: list of numpy.ndarray
         Each of the element is a (n,2) shaped array,
         where n is the number of element in the kernel.
     """
     try:
         import matplotlib.pyplot as plt
-    except ImportError:
-        raise ImportError("maptlotlib.pyplot is needed to use this function.")
+    except ImportError as exc:
+        raise ImportError("maptlotlib.pyplot is needed to use this function.") from exc
 
     for i, k in enumerate(kernels):
         x, y = k.T
         plt.plot(x + 0.1 * i, y + 0.1 * i, "+")
 
 
-def _translate_to_tendency(k):
+def _translate_to_tendency(kernel):
     """Translate a movement to directions.
 
     A kernel looks like
     np.array([
     [x1,y1],
     [x2,y2],....
     ])
     where [xn,yn] represent a coordinate relative to [0,0]
     which is just the nearest neighbor.
     this function return how you could move from [0,0] to k = [x,y]
     If you need to go to [0,2], you need to move up twice.
     it will return [0,0] or more explicitly ['up','up']
     [0,0] will produce a empty array.
 
-    **Parameters:**
-
-    + k: numpy.ndarray
+    Parameters
+    ----------
+    k: numpy.ndarray
         A (n,2)-shaped array, where n is the number of
         element in the kernel.
     """
     tend = []
-    x, y = k
+    x, y = kernel
     if y > 0:
         for j in range(y):
             tend.append(0)  # up
     else:
         for j in range(-y):
             tend.append(1)  # down
     if x < 0:
@@ -77,88 +77,83 @@
             tend.append(2)  # left
     else:
         for j in range(x):
             tend.append(3)  # right
     return tend
 
 
-def kernel_weight_x(kernel, ktype="interp", order=0):
-    """Return the function that calculate the interpolation/derivative weight.
+def kernel_weight_x(kernel, kernel_type="interp", order=0):
+    r"""Return the function that calculate the interpolation/derivative weight.
 
     input needs to be a cross-shaped (that's where x is coming from) Lagrangian kernel.
 
-    **Parameters:**
+    If you don't want to know what is going on under the hood.
+    it's totally fine.
 
-    + kernel: np.ndarray
+    all of the following is a bit hard to understand.
+    The k th (k>=0) derivative of the lagrangian polynomial is
+    $$
+    w_j= \frac{\Sigma_{i\neq j} Pi_{i<m-1-k} (x-x_i)}{\Pi_{i\neq j} (x_j - x_i)}
+    $$
+    for example: if the points are [-1,0,1] for point 0
+    k = 0: w = (x-1)(x+1)/(0-1)(0+1)
+    k = 1: w = [(x+1)+(x-1)]/(0-1)(0+1)
+
+    for a cross shape kernel:
+    f(rx,ry) = f_x(rx) + f_y(ry) - f(0,0)
+
+    Parameters
+    ----------
+    kernel: np.ndarray
         2D array with shape (n,2), where n is the number of nodes.
         It has to be shaped like a cross
-    + ktype: str
+    kernel_type: str
         "interp" (default): Use both x y direction for interpolation,
         implies that order = 0
         "x": Use only x direction for interpolation/derivative
         "y": Use only y direction for interpolation/derivative
-    + order: int
+    order: int
         The order of derivatives. Zero for interpolation.
 
-    **Returns:**
-
-    + func(rx,ry): compilable function
+    Returns
+    -------
+    func(rx,ry): compilable function
         function to calculate the hotizontal interpolation/derivative
         weight
     """
-    xs = np.array(list(set(kernel.T[0]))).astype(float)
-    ys = np.array(list(set(kernel.T[1]))).astype(float)
+    xs = np.array(list(set(kernel.T[0])), dtype=float)
+    ys = np.array(list(set(kernel.T[1])), dtype=float)
 
     # if you the kernel is a line rather than a cross
     if len(xs) == 1:
-        ktype = "y"
+        kernel_type = "y"
     elif len(ys) == 1:
-        ktype = "x"
-
-    """
-    If you don't want to know what is going on under the hood.
-    it's totally fine.
-
-    all of the following is a bit hard to understand.
-    The k th (k>=0) derivative of the lagrangian polynomial is
-          Sigma_{i\neq j} Pi_{i<m-1-k} (x-x_i)
-    w_j= ----------------------------------------
-          Pi_{i\neq j} (x_j - x_i)
-
-    for example: if the points are [-1,0,1] for point 0
-    k = 0: w = (x-1)(x+1)/(0-1)(0+1)
-    k = 1: w = [(x+1)+(x-1)]/(0-1)(0+1)
-
-    for a cross shape kernel:
-    f(rx,ry) = f_x(rx) + f_y(ry) - f(0,0)
-
-    The following equation is just that.
-    """
+        kernel_type = "x"
 
     x_poly = []
     y_poly = []
-    if ktype == "interp":
+    if kernel_type == "interp":
         for ax in xs:
-            x_poly.append(get_combination([i for i in xs if i != ax], len(xs) - 1))
+            x_poly.append(list(combinations([i for i in xs if i != ax], len(xs) - 1)))
         for ay in ys:
-            y_poly.append(get_combination([i for i in ys if i != ay], len(ys) - 1))
-    if ktype == "x":
+            y_poly.append(list(combinations([i for i in ys if i != ay], len(ys) - 1)))
+    if kernel_type == "x":
         for ax in xs:
             x_poly.append(
-                get_combination([i for i in xs if i != ax], len(xs) - 1 - order)
+                list(combinations([i for i in xs if i != ax], len(xs) - 1 - order))
             )
         y_poly = [[[]]]
-    if ktype == "y":
+    if kernel_type == "y":
         x_poly = [[[]]]
         for ay in ys:
             y_poly.append(
-                get_combination([i for i in ys if i != ay], len(ys) - 1 - order)
+                list(combinations([i for i in ys if i != ay], len(ys) - 1 - order))
             )
-    x_poly = np.array(x_poly).astype(float)
-    y_poly = np.array(y_poly).astype(float)
+    x_poly = np.array(x_poly, dtype=float)
+    y_poly = np.array(y_poly, dtype=float)
 
     @compileable
     def the_interp_func(rx, ry):
         nonlocal kernel, xs, ys, x_poly, y_poly
         n = len(rx)
         m = len(kernel)
         weight = np.ones((n, m)) * 0.0
@@ -286,99 +281,103 @@
                 for other in ys:
                     if other != y:
                         weight[:, i] /= y - other
             else:
                 weight[:, i] = 0.0
         return weight
 
-    if ktype == "interp":
+    if kernel_type == "interp":
         return the_interp_func
-    if ktype == "x":
+    if kernel_type == "x":
         max_order = len(xs) - 1
         if order < max_order:
             return the_x_func
         elif order == max_order:
             return the_x_maxorder_func
         else:
-            raise Exception("Kernel is too small for this derivative")
-    if ktype == "y":
+            raise ValueError("Kernel is too small for this derivative")
+    if kernel_type == "y":
         max_order = len(ys) - 1
         if order < max_order:
             return the_y_func
         elif order == max_order:
             return the_y_maxorder_func
         else:
-            raise Exception("Kernel is too small for this derivative")
+            raise ValueError("Kernel is too small for this derivative")
 
 
 # we can define the default interpolation functions here,
 # so if we are using it over and over, we don't have to compile it.
 # and it really takes a lot of time to compile.
 
 
 def kernel_weight_s(kernel, xorder=0, yorder=0):
     """Return the function that calculate the interpolation/derivative weight.
 
     input needs to be a rectangle-shaped (that's where x is coming from)
     Lagrangian kernel.
 
-    **Parameters:**
-
-    + kernel: np.ndarray
+    Parameters
+    ----------
+    kernel: np.ndarray
         2D array with shape (n,2), where n is the number of nodes.
         It has to be shaped like a rectangle
-    + xorder: int
+    xorder: int
         The order of derivatives in the x direction.
         Zero for interpolation.
-    + yorder: int
+    yorder: int
         The order of derivatives in the y direction.
         Zero for interpolation.
 
-    **Returns:**
-
-    + func(rx,ry): compilable function
+    Returns
+    -------
+    func(rx,ry): compilable function
         function to calculate the hotizontal interpolation/derivative
         weight
     """
-    xs = np.array(list(set(kernel.T[0]))).astype(float)
-    ys = np.array(list(set(kernel.T[1]))).astype(float)
+    xs = np.array(list(set(kernel.T[0])), dtype=float)
+    ys = np.array(list(set(kernel.T[1])), dtype=float)
     xmaxorder = False
     ymaxorder = False
     if xorder < len(xs) - 1:
         pass
     elif xorder == len(xs) - 1:
         xmaxorder = True
     else:
-        raise Exception("Kernel is too small for this derivative")
+        raise ValueError("Kernel is too small for this derivative")
 
     if yorder < len(ys) - 1:
         pass
     elif yorder == len(ys) - 1:
         ymaxorder = True
     else:
-        raise Exception("Kernel is too small for this derivative")
+        raise ValueError("Kernel is too small for this derivative")
 
     x_poly = []
     y_poly = []
     for ax in xs:
-        x_poly.append(get_combination([i for i in xs if i != ax], len(xs) - 1 - xorder))
+        x_poly.append(
+            list(combinations([i for i in xs if i != ax], len(xs) - 1 - xorder))
+        )
     for ay in ys:
-        y_poly.append(get_combination([i for i in ys if i != ay], len(ys) - 1 - yorder))
-    x_poly = np.array(x_poly).astype(float)
-    y_poly = np.array(y_poly).astype(float)
+        y_poly.append(
+            list(combinations([i for i in ys if i != ay], len(ys) - 1 - yorder))
+        )
+    x_poly = np.array(x_poly, dtype=float)
+    y_poly = np.array(y_poly, dtype=float)
 
     @compileable
     def the_square_func(rx, ry):
         nonlocal kernel, xs, ys, y_poly, x_poly, xorder, yorder, xmaxorder, ymaxorder
         n = len(rx)
-        mx = len(xs)
-        my = len(ys)
+        num_node_x = len(xs)
+        num_node_y = len(ys)
         m = len(kernel)
-        yweight = np.ones((n, my))
-        xweight = np.ones((n, mx))
+        yweight = np.ones((n, num_node_y))
+        xweight = np.ones((n, num_node_x))
         weight = np.ones((n, m)) * 0.0
 
         if ymaxorder:
             common = 1
             for i in range(1, yorder):
                 common *= i
             yweight *= float(common)
@@ -425,69 +424,74 @@
             weight[:, i] = yweight[:, iy] * xweight[:, ix]
 
         return weight
 
     return the_square_func
 
 
-def kernel_weight(kernel, ktype="interp", order=0):
+def kernel_weight(kernel, kernel_type="interp", order=0):
     """Return a function that compute weights.
 
     A wrapper around kernel_weight_x and kernel_weight_s.
     Return the function that calculate the interpolation/derivative weight
     of a  Lagrangian kernel.
 
-    **Parameters:**
-
-    + kernel: np.ndarray
+    Parameters
+    ----------
+    kernel: np.ndarray
         2D array with shape (n,2), where n is the number of nodes.
         It need to either shape like a rectangle or a cross
-    + ktype: str
+    kernel_type: str
         "interp" (default): Use both x y direction for interpolation,
         implies that order = 0
         "dx": Use only x direction for interpolation/derivative
         "dy": Use only y direction for interpolation/derivative
-    + order: int
+    order: int
         The order of derivatives. Zero for interpolation.
 
-    **Returns:**
-
-    + func(rx,ry): compilable function
+    Returns
+    -------
+    func(rx,ry): compilable function
         function to calculate the hotizontal interpolation/derivative
         weight
     """
-    mx = len(set(kernel[:, 0]))
-    my = len(set(kernel[:, 1]))
-    if len(kernel) == mx + my - 1:
-        if "d" in ktype:
-            ktype = ktype[1:]
-        return kernel_weight_x(kernel, ktype=ktype, order=order)
-    elif len(kernel) == mx * my:
-        # mx*my == mx+my-1 only when mx==1 or my ==1
-        if ktype == "interp":
+    num_node_x = len(set(kernel[:, 0]))
+    num_node_y = len(set(kernel[:, 1]))
+    if len(kernel) == num_node_x + num_node_y - 1:
+        if "d" in kernel_type:
+            kernel_type = kernel_type[1:]
+        return kernel_weight_x(kernel, kernel_type=kernel_type, order=order)
+    elif len(kernel) == num_node_x * num_node_y:
+        # num_node_x*num_node_y == num_node_x+num_node_y-1
+        # only when num_node_x==1 or num_node_y ==1
+        if kernel_type == "interp":
             return kernel_weight_s(kernel, xorder=0, yorder=0)
-        elif ktype == "dx":
+        elif kernel_type == "dx":
             return kernel_weight_s(kernel, xorder=order, yorder=0)
-        elif ktype == "dy":
+        elif kernel_type == "dy":
             return kernel_weight_s(kernel, xorder=0, yorder=order)
+        else:
+            raise ValueError(f"kernel_type = {kernel_type} not supported")
+    else:
+        raise NotImplementedError("The shape of the kernel is neither cross or square")
 
 
-default_interp_funcs = [kernel_weight_x(a_kernel) for a_kernel in default_kernels]
+default_interp_funcs = [kernel_weight_x(a_kernel) for a_kernel in DEFAULT_KERNELS]
 
 
-def find_which_points_for_each_kernel(masked, russian_doll="default"):
+def find_which_points_for_each_kernel(masked, inheritance="default"):
     """Find which kernel to use at each point.
 
     masked is going to be a n*m array,
     where n is the number of points of interest.
     m is the size of the largest kernel.
 
-    russian_doll defines the shape of smaller kernels.
+    inheritance defines the shape of smaller kernels.
     say
-    russian_doll = [
+    inheritance = [
     [0,1,2,3,4],
     [0,1],
     [0]
     ]
     it means that the largest kernel have all 5 nodes
     the second kernel only contain the first and second node,
     and the last one only have the nearest neighbor.
@@ -500,134 +504,130 @@
     although it fits both 2nd and 3rd kernel, 2nd has priority,
     so the index will be in the 2nd element of the return pk.
 
     if a row looks like [0,0,0,0,0],
     none of the kernel can fit it, so the index will not be in the
     return
     """
-    if russian_doll == "default":
-        russian_doll = default_inheritance
+    if inheritance == "default":
+        inheritance = DEFAULT_INHERITANCE
     already_wet = []
-    for i, doll in enumerate(russian_doll):
+    for i, doll in enumerate(inheritance):
         wet_1d = masked[:, np.array(doll)].all(axis=1)
         already_wet.append(np.where(wet_1d)[0])
     point_for_each_kernel = [list(already_wet[0])]
-    for i in range(1, len(russian_doll)):
+    for i in range(1, len(inheritance)):
         point_for_each_kernel.append(
             list(np.setdiff1d(already_wet[i], already_wet[i - 1]))
         )
     return point_for_each_kernel
 
 
 def get_weight_cascade(
     rx,
     ry,
     pk,
-    kernel_large=default_kernel,
-    russian_doll=default_inheritance,
+    kernel_large=DEFAULT_KERNEL,
+    inheritance=DEFAULT_INHERITANCE,
     funcs=default_interp_funcs,
 ):
-    weight = np.zeros((len(rx), len(kernel_large)))
-    weight[:, 0] = np.nan
-    """Compute the weight
+    """Compute the weight.
 
     apply the corresponding functions that was figured out in
     find_which_points_for_each_kernel
 
-    **Parameters:**
-
-    + rx,ry: numpy.ndarray
+    Parameters
+    ----------
+    rx,ry: numpy.ndarray
         1D array with length N of non-dimensional relative horizontal
         position to the nearest node
-    + kernel_large: numpy.ndarray
+    kernel_large: numpy.ndarray
         A numpy kernel of shape (M,2) that contains all the kernels needed.
-    + russian_doll: list of list(s)
+    inheritance: list of list(s)
         The inheritance sequence when some of the node is masked.
-    + funcs: list of compileable functions
+    funcs: list of compileable functions
         The weight function of each kernel in the inheritance sequence.
 
-    **Returns:**
-
+    Returns
+    -------
     + weight: numpy.ndarray
         The horizontal weight of interpolation/derivative for the points
         with shape (N,M)
 
     """
+    weight = np.zeros((len(rx), len(kernel_large)))
+    weight[:, 0] = np.nan
     for i in range(len(pk)):
         if len(pk[i]) == 0:
             continue
         sub_rx = rx[pk[i]]
         sub_ry = ry[pk[i]]
         #     slim_weight = interp_func[i](sub_rx,sub_ry)
         sub_weight = np.zeros((len(pk[i]), len(kernel_large)))
-        sub_weight[:, np.array(russian_doll[i])] = funcs[i](sub_rx, sub_ry)
+        sub_weight[:, np.array(inheritance[i])] = funcs[i](sub_rx, sub_ry)
         weight[pk[i]] = sub_weight
     return weight
 
 
-def find_pk_4d(masked, russian_doll=default_inheritance):
-    """Find the masking condition for 4D space time."""
+def find_pk_4d(masked, inheritance=DEFAULT_INHERITANCE):
+    """Find the masking condition for 4D space time.
+
+    See find_which_points_for_each_kernel
+    """
     maskedT = masked.T
     ind_shape = maskedT.shape
-    tz = []
+    pk4d = []
     for i in range(ind_shape[0]):
         z = []
         for j in range(ind_shape[1]):
-            z.append(find_which_points_for_each_kernel(maskedT[i, j].T, russian_doll))
-        tz.append(z)
-    return tz
+            z.append(find_which_points_for_each_kernel(maskedT[i, j].T, inheritance))
+        pk4d.append(z)
+    return pk4d
 
 
 def kash(kernel):  # hash kernel
     """Hash a horizontal kernel.
 
     Return the hash value.
 
-    **Parameters:**
-
+    Parameters
+    ----------
     + kernel: numpy.ndarray
         A horizontal kernel
     """
-    temp_lst = [(i, j) for (i, j) in kernel]
-    return hash(tuple(temp_lst))
+    return hash(tuple((i, j) for (i, j) in kernel))
+
+
+@cache
+def _get_func_from_hashable(
+    kernel_tuple, kernel_shape, hkernel="interp", h_order=0, **kwargs
+):
+    kernel = np.array(kernel_tuple).reshape(kernel_shape)
+    return kernel_weight(kernel, kernel_type=hkernel, order=h_order)
 
 
-def get_func(kernel, hkernel="interp", h_order=0):
+def get_func(kernel, **kwargs):
     """Return functions that compute weights.
 
     Similar to the kernel_weight function,
     the only difference is that this function can
-    read existing functions from a global dictionary,
-    and can register to the dictionary when new ones are created.
-    """
-    global weight_func
-    ker_ind = kash(kernel)
-    layer_1 = weight_func.get(ker_ind)
-    if layer_1 is None:
-        weight_func[ker_ind] = dict()
-    layer_1 = weight_func[ker_ind]
-
-    layer_2 = layer_1.get(hkernel)
-    if layer_2 is None:
-        layer_1[hkernel] = dict()
-    layer_2 = layer_1[hkernel]
-
-    layer_3 = layer_2.get(h_order)
-    if layer_3 is None:
-        logging.info("Creating new weight function, the first time is going to be slow")
-        layer_2[h_order] = kernel_weight(kernel, ktype=hkernel, order=h_order)
-    layer_3 = layer_2[h_order]
+    read existing functions that is cached.
+    See _get_func_from_hashable
 
-    return layer_3
+    See Also
+    --------
+    kernel_weight: the un-hashed version of this function.
+    """
+    return _get_func_from_hashable(tuple(kernel.ravel()), kernel.shape, **kwargs)
 
 
-def auto_doll(kernel, hkernel="interp"):
+def auto_inheritance(kernel, hkernel="interp"):
     """Find a natural inheritance pattern given one horizontal kernel."""
     if hkernel == "interp":
-        doll = [[i for i in range(len(kernel))]]
+        doll = [list(range(len(kernel)))]
     elif hkernel == "dx":
         doll = [[i for i in range(len(kernel)) if kernel[i][1] == 0]]
     elif hkernel == "dy":
         doll = [[i for i in range(len(kernel)) if kernel[i][0] == 0]]
     doll[0] = sorted(
         doll[0], key=lambda i: max(abs(kernel[i] + np.array([0.01, 0.00618])))
     )
@@ -644,70 +644,70 @@
 
 class KnW:
     """Kernel object.
 
     A class that describes anything about the
     interpolation/derivative kernel to be used.
 
-    **Parameters:**
-
-    + kernel: numpy.ndarray
+    Parameters
+    ----------
+    kernel: numpy.ndarray
         The largest horizontal kernel to be used
-    + inheritance: list
+    inheritance: list
         The inheritance sequence of the kernels
-    + hkernel: str
+    hkernel: str
         What to do in the horizontal direction
         'interp', 'dx', or 'dy'?
-    + tkernel: str
+    tkernel: str
         What kind of operation to do in the temporal dimension:
         'linear', 'nearest' interpolation, or 'dt'
-    + zkernel: str
+    vkernel: str
         What kind of operation to do in the vertical:
         'linear', 'nearest' interpolation, or 'dz'
-    + h_order: int
+    h_order: int
         How many derivative to take in the horizontal direction.
         Zero for pure interpolation
-    + ignore_mask: bool
+    ignore_mask: bool
         Whether to diregard the masking of the dataset.
         You can select True if there is no
         inheritance, or if performance is a big concern.
     """
 
     def __init__(
         self,
-        kernel=default_kernel,
+        kernel=DEFAULT_KERNEL,
         inheritance="auto",  # None, or list of lists
         hkernel="interp",  # dx,dy
         vkernel="nearest",  # linear,dz
         tkernel="nearest",  # linear,dt
         h_order=0,  # depend on hkernel type
         ignore_mask=False,
     ):
-        ksort = np.abs(kernel + np.array([0.01, 0.00618])).sum(axis=1).argsort()
+        kernel_sort = np.abs(kernel + np.array([0.01, 0.00618])).sum(axis=1).argsort()
         # Avoid points having same distance
-        ksort_inv = ksort.argsort()
+        kernel_sort_inv = kernel_sort.argsort()
 
         if (inheritance is not None) and (ignore_mask):
             logging.info(
                 "Overwriting the inheritance object to None,"
                 " because we ignore masking"
             )
 
         if inheritance == "auto":
-            inheritance = auto_doll(kernel, hkernel=hkernel)
+            inheritance = auto_inheritance(kernel, hkernel=hkernel)
         elif inheritance is None:  # does not apply cascade
-            inheritance = [[i for i in range(len(kernel))]]
+            inheritance = [list(range(len(kernel)))]
         elif isinstance(inheritance, list):
             pass
         else:
             raise ValueError("Unknown type of inherirance")
 
-        self.kernel = kernel[ksort]
+        self.kernel = kernel[kernel_sort]
         self.inheritance = [
-            sorted([ksort_inv[i] for i in heir]) for heir in inheritance
+            sorted([kernel_sort_inv[i] for i in heir]) for heir in inheritance
         ]
         self.hkernel = hkernel
         self.vkernel = vkernel
         self.tkernel = tkernel
         self.h_order = h_order
         self.ignore_mask = ignore_mask
 
@@ -721,33 +721,31 @@
 
     def same_hsize(self, other):
         """Return True if 2 KnW object has the same horizontal size."""
         type_same = isinstance(other, type(self))
         if not type_same:
             raise TypeError("the argument is not a KnW object")
         try:
-            return (self.kernel == other.kernel).all()
-        except AttributeError:
+            return np.allclose(self.kernel, other.kernel)
+        except (ValueError, AttributeError):
             return False
 
     def same_size(self, other):
         """Return True if 2 KnW object has the same 4D size."""
         only_size = {"dz": 2, "linear": 2, "dt": 2, "nearest": 1}
         hsize_same = self.same_hsize(other)
         vsize_same = only_size[self.vkernel] == only_size[other.vkernel]
         tsize_same = only_size[self.tkernel] == only_size[other.tkernel]
         return hsize_same and vsize_same and tsize_same
 
     def __eq__(self, other):
         type_same = isinstance(other, type(self))
         if not type_same:
             return False
-        shpe_same = (
-            self.kernel == other.kernel
-        ).all() and self.inheritance == other.inheritance
+        shpe_same = self.same_hsize(other) and self.inheritance == other.inheritance
         diff_same = (
             (self.hkernel == other.hkernel)
             and (self.vkernel == other.vkernel)
             and (self.tkernel == other.tkernel)
         )
         return type_same and shpe_same and diff_same
 
@@ -778,28 +776,28 @@
         rz=0,
         rt=0,
         pk4d=None,  # All using the largest
         bottom_scheme="no flux",  # None
     ):
         """Return the weight of values given particle rel-coords.
 
-        **Parameters:**
-
-        + rx,ry,rz,rt: numpy.ndarray
+        Parameters
+        ----------
+        rx,ry,rz,rt: numpy.ndarray
             1D array of non-dimensional particle positions
-        + pk4d: list
+        pk4d: list
             A mapping on which points should use which kernel.
-        + bottom_scheme: str
+        bottom_scheme: str
             Whether to assume there is a ghost point with same value at
             the bottom boundary.
             Choose None for vertical flux, 'no flux' for most other cases.
 
-        **Returns:**
-
-        + weight: numpy.ndarray
+        Returns
+        -------
+        weight: numpy.ndarray
             The weight of interpolation/derivative for the points
             with shape (N,M),
             M is the num of node in the largest kernel.
         """
         if self.vkernel in ["linear", "dz"]:
             nz = 2
         else:
@@ -851,15 +849,15 @@
             for jt in range(nt):
                 for jz in range(nz):
                     weight[:, :, jz, jt] = get_weight_cascade(
                         rx,
                         ry,
                         pk4d[jt][jz],
                         kernel_large=self.kernel,
-                        russian_doll=self.inheritance,
+                        inheritance=self.inheritance,
                         funcs=self.hfuncs,
                     )
         for jt in range(nt):
             if (self.vkernel == "linear") and (bottom_scheme == "no flux"):
                 # whereever the bottom layer is masked,
                 # replace it with a ghost point above it
                 secondlayermasked = np.isnan(weight[:, :, 0, jt]).any(axis=1)
```

### Comparing `seaduck-0.1.2/seaduck/ocedata.py` & `seaduck-0.1.3/seaduck/ocedata.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,175 @@
 import logging
 
 import numpy as np
 
 try:  # pragma: no cover
-    import pandas as _pd
+    import pandas as pd
 except ImportError:  # pragma: no cover
     pass
 import xarray as xr
 
-from seaduck.topology import topology
+from seaduck.topology import Topology
 from seaduck.utils import (
     _general_len,
     create_tree,
-    find_cs_sn,
     find_rel_h_naive,
     find_rel_h_oceanparcel,
     find_rel_h_rectilinear,
     find_rel_nearest,
     find_rel_time,
     find_rel_z,
+    missing_cs_sn,
 )
 
-no_alias = {
-    "XC": "XC",
-    "YC": "YC",
-    "Z": "Z",
-    "Zl": "Zl",
-    "time": "time",
+NO_ALIAS = {
     "dXC": "dxC",
     "dYC": "dyC",
     "dZ": "drC",
-    "XG": "XG",
-    "YG": "YG",
     "dXG": "dxG",
     "dYG": "dyG",
     "dZl": "drF",
-    "CS": "CS",
-    "SN": "SN",
 }
 
 
+class RelCoord(dict):
+    """
+    NamedTuple that also has update method.
+
+    This class is used to store the relative coordinates.
+    Attributes starts with "i" are indexes of the nearest grid point.
+    Attributes starts with "b" are value (time/dep/lat/lon) of the nearest grid point.
+    Attributes starts with "d" are distance between the nearest grid point and its
+    neighboring point in meters or seconds.
+    Attributes starts with "r" are the distance from the point of interest to the nearest
+    non-dimensionalized by the "d" variable.
+    "cs", "sn" are the cosine and sine of the grid orientation relative to meridian.
+    "face" is the face/tile the point is on, if the dataset has such a dimension.
+
+    All of those attributes should be None or 1D numpy array.
+
+    Methods
+    -------
+    update(other)
+        Inheritated from dictionary.
+    """
+
+    def __getattr__(self, attr):
+        try:
+            return self[attr]
+        except KeyError as exc:
+            raise AttributeError(
+                f"'RelCoord' object has no attribute '{attr}'"
+            ) from exc
+
+    def __setattr__(self, attr, value):
+        self[attr] = value
+
+    def subset(self, which):
+        """Create a subset of all the non-None items."""
+        new = RelCoord()
+        for var in self.keys():
+            if self[var] is not None:
+                new[var] = self[var][which]
+            else:
+                new[var] = None
+        return new
+
+    def update_from_subset(self, sub, which):
+        for var in sub.keys():
+            if var in self.keys():
+                if self[var] is not None:
+                    self[var][which] = sub[var]
+            else:
+                raise KeyError(
+                    f"Key {var} is in subset, " "but not in the one to update."
+                )
+
+    @classmethod
+    def create_class(cls, class_name, fields):
+        """Create a subclass with predetermined keys."""
+
+        class NewClass(cls):
+            __slots__ = ()
+            _fields = fields
+
+            def __init__(self, *args):
+                if len(args) > len(fields):
+                    raise TypeError(
+                        f"{class_name} takes {len(fields)} positional arguments"
+                        f" but {len(args)} were given"
+                    )
+                for name, value in zip(fields, args):
+                    setattr(self, name, value)
+
+            @classmethod
+            def _make(cls, iterable):
+                """Make a instance of this class similar to that of collections.namedtuple."""
+                return cls(*iterable)
+
+            def __repr__(self):
+                field_values = ", ".join(
+                    f"{name}={getattr(self, name)!r}" for name in self._fields
+                )
+                return f"{class_name}({field_values})"
+
+        NewClass.__name__ = class_name
+        return NewClass
+
+
+HRel = RelCoord.create_class(
+    "HRel", ["face", "iy", "ix", "rx", "ry", "cs", "sn", "dx", "dy", "bx", "by"]
+)
+HRel.__doc__ = "Wrap around the horizontal rel-coords. See also RelCoord."
+VRel = RelCoord.create_class("VRel", ["iz", "rz", "dz", "bz"])
+VRel.__doc__ = (
+    "Wrap around the vertical centered nearest rel-coords. See also RelCoord."
+)
+VLinRel = RelCoord.create_class("VLRel", ["iz_lin", "rz_lin", "dz_lin", "bz_lin"])
+VLinRel.__doc__ = (
+    "Wrap around the vertical centered linear rel-coords. See also RelCoord."
+)
+VlRel = RelCoord.create_class("VlRel", ["izl", "rzl", "dzl", "bzl"])
+VlRel.__doc__ = (
+    "Wrap around the vertical staggered nearest rel-coords. See also RelCoord."
+)
+VlLinRel = RelCoord.create_class(
+    "VlLinRel", ["izl_lin", "rzl_lin", "dzl_lin", "bzl_lin"]
+)
+VlLinRel.__doc__ = (
+    "Wrap around the vertical staggered linear rel-coords. See also RelCoord."
+)
+TRel = RelCoord.create_class("TRel", ["it", "rt", "dt", "bt"])
+TRel.__doc__ = "Wrap around the temporal nearest rel-coords."
+TLinRel = RelCoord.create_class("TLinRel", ["it_lin", "rt_lin", "dt_lin", "bt_lin"])
+TRel.__doc__ = "Wrap around the temporal linear rel-coords. See also RelCoord."
+
+
 class OceData:
     """Ocean dataset.
 
     Class that enables variable aliasing, topology extraction, and 4-D translation
     between latitude-longitude-depth-time grid and relative description.
 
-    **Parameters**
-
-    + data: xarray.Dataset
-        The dataset to extract grid information, create cKD tree, and topology object on.
-    + alias: dict, None, or 'auto'
+    Parameters
+    ----------
+    data: xarray.Dataset
+        The dataset to extract grid information, create cKD tree, and Topology object on.
+    alias: dict, None, or 'auto'
         1. dict: Map the variable used by this package (key) to
            that used by the dataset (value).
         2. None (default): Do not apply alias.
         3. 'auto' (Not implemented): Automatically generate a list for the alias.
     """
 
     def __init__(self, data, alias=None, memory_limit=1e7):
         self._ds = data
-        self.tp = topology(data)
+        self.tp = Topology(data)
         if alias is None:
-            self.alias = no_alias
+            self.alias = NO_ALIAS
         elif alias == "auto":
             raise NotImplementedError("auto alias not yet implemented")
         elif isinstance(alias, dict):
             self.alias = alias
 
         try:
             self.too_large = self._ds["XC"].nbytes > memory_limit
@@ -86,51 +190,52 @@
     def __setitem__(self, key, item):
         if isinstance(item, xr.DataArray):
             if key in self.alias.keys():
                 self._ds[self.alias[key]] = item
             else:
                 self._ds[key] = item
         else:
-            self.__dict__[key] = item
+            object.__setattr__(self, key, item)
 
     def __getitem__(self, key):
-        if key in self.__dict__.keys():
-            return self.__dict__[key]
+        varsdict = vars(self)
+        if key in varsdict.keys():
+            return object.__getattribute__(self, key)
         else:
             if key in self.alias.keys():
                 return self._ds[self.alias[key]]
             else:
                 return self._ds[key]
 
     def check_readiness(self):
         """Return readiness.
 
         Function that checks what kind of interpolation is supported.
 
-        **Returns:**
-
-        + readiness: dict
+        Returns
+        -------
+        readiness: dict
             'h': The scheme of horizontal interpolation to be used,
                  including 'oceanparcel', 'local_cartesian', and 'rectilinear'.
             'Z': Whether the dataset has a vertical dimension at the center points.
             'Zl': Whether the dataset has a vertical dimension at staggered points
                  (vertical velocity).
             'time': Whether the dataset has a temporal dimension.
         """
         # TODO: make the check more detailed
         varnames = list(self._ds.data_vars) + list(self._ds.coords)
         readiness = {}
         missing = []
-        if all([i in varnames for i in ["XC", "YC", "XG", "YG"]]):
+        if all(i in varnames for i in ["XC", "YC", "XG", "YG"]):
             readiness["h"] = "oceanparcel"
             # could be a curvilinear grid that can use oceanparcel style
-        elif all([i in varnames for i in ["XC", "YC", "dxG", "dyG", "CS", "SN"]]):
+        elif all(i in varnames for i in ["XC", "YC", "dxG", "dyG", "CS", "SN"]):
             readiness["h"] = "local_cartesian"
             # could be a curvilinear grid that can use local cartesian style
-        elif all([i in varnames for i in ["lon", "lat"]]):
+        elif all(i in varnames for i in ["lon", "lat"]):
             ratio = 6371e3 * np.pi / 180
             self.dlon = np.gradient(self["lon"]) * ratio
             self.dlat = np.gradient(self["lat"]) * ratio
             readiness["h"] = "rectilinear"
             # corresponding to a rectilinear dataset
         else:
             readiness["h"] = False
@@ -150,101 +255,101 @@
 
     def _add_missing_grid(self):
         # TODO:
         pass
 
     def show_alias(self):
         """Print out the alias in a nice pd.DataFrame format."""
-        try:
-            return _pd.DataFrame.from_dict(
-                self.alias, orient="index", columns=["original name"]
-            )
-        except NameError:
-            raise NameError("pandas is needed to perform this function.")
+        return pd.DataFrame.from_dict(
+            self.alias, orient="index", columns=["original name"]
+        )
 
     def _add_missing_cs_sn(self):
         try:
-            assert (self["SN"] is not None) and (self["CS"] is not None)
+            assert self["SN"] is not None
+            assert self["CS"] is not None
         except (AttributeError, AssertionError):
-            xc = np.deg2rad(np.array(self["XC"]))
-            yc = np.deg2rad(np.array(self["YC"]))
-            cs = np.zeros_like(xc)
-            sn = np.zeros_like(xc)
-            cs[0], sn[0] = find_cs_sn(yc[0], xc[0], yc[1], xc[1])
-            cs[-1], sn[-1] = find_cs_sn(yc[-2], xc[-2], yc[-1], xc[-1])
-            cs[1:-1], sn[1:-1] = find_cs_sn(yc[:-2], xc[:-2], yc[2:], xc[2:])
-            # it makes no sense to turn it into DataArray again when you already have in memory
-            # and you know where this data is defined.
+            cs, sn = missing_cs_sn(self)
             self["CS"] = cs
             self["SN"] = sn
 
     def hgrid2array(self):
         """Extract the horizontal grid data into numpy arrays.
 
         This is done based on the readiness['h'] of the OceData object.
         """
-        way = self.readiness["h"]
         if self.too_large:  # pragma: no cover
             logging.warning(
                 "Loading grid into memory, it's a large dataset please be patient"
             )
 
-        if way == "oceanparcel":
+        if self.readiness["h"] == "oceanparcel":
             for var in ["XC", "YC", "XG", "YG"]:
-                self[var] = np.array(self[var]).astype("float32")
+                self[var] = np.array(self[var], dtype="float32")
             for var in ["rA", "CS", "SN"]:
                 try:
-                    self[var] = np.array(self[var]).astype("float32")
+                    self[var] = np.array(self[var], dtype="float32")
                 except KeyError:
-                    logging.info(f"no {var} in dataset, skip")
+                    logging.info("no %s in dataset, skip", var)
                     self[var] = None
             try:
-                self.dX = np.array(self["dXG"]).astype("float32")
-                self.dY = np.array(self["dYG"]).astype("float32")
+                self.dX = np.array(self["dXG"], dtype="float32")
+                self.dY = np.array(self["dYG"], dtype="float32")
             except KeyError:
                 self.dX = None
                 self.dY = None
             if self.too_large:  # pragma: no cover
                 logging.info("numpy arrays of grid loaded into memory")
             self.tree = create_tree(self.XC, self.YC)
             if self.too_large:  # pragma: no cover
                 logging.info("cKD created")
 
-        if way == "local_cartesian":
+        if self.readiness["h"] == "local_cartesian":
             for var in ["XC", "YC", "CS", "SN"]:
-                self[var] = np.array(self[var]).astype("float32")
-            self.dX = np.array(self["dXG"]).astype("float32")
-            self.dY = np.array(self["dYG"]).astype("float32")
+                self[var] = np.array(self[var], dtype="float32")
+            self.dX = np.array(self["dXG"], dtype="float32")
+            self.dY = np.array(self["dYG"], dtype="float32")
 
             if not self.too_large:  # pragma: no cover
                 for var in ["XG", "YG", "dXC", "dYC", "rA"]:
                     try:
-                        self[var] = np.array(self[var]).astype("float32")
+                        self[var] = np.array(self[var], dtype="float32")
                     except KeyError:
-                        logging.info(f"no {var} in dataset, skip")
+                        logging.info("no %s in dataset, skip", var)
                         self[var] = None
             if self.too_large:  # pragma: no cover
                 logging.info("numpy arrays of grid loaded into memory")
             self.tree = create_tree(self.XC, self.YC)
             if self.too_large:  # pragma: no cover
                 logging.info("cKD created")
 
-        if way == "rectilinear":
-            self.lon = np.array(self["lon"]).astype("float32")
-            self.lat = np.array(self["lat"]).astype("float32")
+        if self.readiness["h"] == "rectilinear":
+            self.lon = np.array(self["lon"], dtype="float32")
+            self.lat = np.array(self["lat"], dtype="float32")
 
     def vgrid2array(self):
         """Extract the vertical center point grid data into numpy arrays."""
-        self.Z = np.array(self["Z"]).astype("float32")
-        self.dZ = np.array(self["dZ"]).astype("float32")
+        self.Z = np.array(self["Z"], dtype="float32")
+        try:
+            self.dZ = np.array(self["dZ"], dtype="float32")
+        except KeyError:
+            self.dZ = np.diff(self.Z)
+            self.dZ = np.append(self.dZ, self.dZ[-1])
 
     def vlgrid2array(self):
         """Extract the vertical staggered point grid data into numpy arrays."""
-        self.Zl = np.array(self["Zl"]).astype("float32")
-        self.dZl = np.array(self["dZl"]).astype("float32")
+        self.Zl = np.array(self["Zl"], dtype="float32")
+        try:
+            self.dZl = np.array(self["dZl"], dtype="float32")
+        except KeyError:
+            if "Zp1" in self._ds.variables:
+                self.dZl = np.diff(np.array(self["Zp1"]))
+            else:
+                self.dZl = np.diff(self.Zl)
+                self.dZl = np.append(self.dZl, self.dZl[-1])
 
         # special treatment for dZl
         # self.dZl = np.roll(self.dZl,1)
         # self.dZl[0] = 1e-10
 
     def tgrid2array(self):
         """Extract the temporal grid data into numpy arrays."""
@@ -269,144 +374,69 @@
             self.tgrid2array()
 
     def find_rel_h(self, x, y):
         """Find the horizontal rel-coordinate.
 
         Find the horizontal rel-coordinate of the given 4-D position based on readiness['h'].
 
-        **Parameters:**
-
-        + x, y: np.ndarray
+        Parameters
+        ----------
+        x, y: np.ndarray
             1D array of longitude and latitude.
 
-        **Returns:**
-
-        + faces, iys, ixs: np.ndarray or None
-            Indexes of the nearest horizontal point.
-        + rx, ry: np.ndarray
-            Non-dimensional distance to the nearest point.
-        + cs, sn: np.ndarray or None
-            The cosine and sine of the grid orientation compared to local meridian.
-        + dx, dy:
-            The size of the horizontal cell used for the Non-dimensionalization.
-        + bx, by:
-            The longitude and latitude for the nearest grid point.
+        Returns
+        -------
+        hrel: seaduck.ocedata.HRel object
+            A dictionary that defines the horizontal rel-coords
         """
         if self.readiness["h"] == "oceanparcel":
-            faces, iys, ixs, rx, ry, cs, sn, dx, dy, bx, by = find_rel_h_oceanparcel(
+            h_rel_tuple = find_rel_h_oceanparcel(
                 x,
                 y,
                 self.XC,
                 self.YC,
                 self.dX,
                 self.dY,
                 self.CS,
                 self.SN,
                 self.XG,
                 self.YG,
                 self.tree,
                 self.tp,
             )
         elif self.readiness["h"] == "local_cartesian":
-            faces, iys, ixs, rx, ry, cs, sn, dx, dy, bx, by = find_rel_h_naive(
+            h_rel_tuple = find_rel_h_naive(
                 x, y, self.XC, self.YC, self.dX, self.dY, self.CS, self.SN, self.tree
             )
         elif self.readiness["h"] == "rectilinear":
-            faces, iys, ixs, rx, ry, cs, sn, dx, dy, bx, by = find_rel_h_rectilinear(
-                x, y, self.lon, self.lat
-            )
-        return faces, iys, ixs, rx, ry, cs, sn, dx, dy, bx, by
+            h_rel_tuple = find_rel_h_rectilinear(x, y, self.lon, self.lat)
+        return HRel._make(h_rel_tuple)
+
+    def find_rel_v(self, z):
+        """Find the rel-coord based on vertical center grid using the nearest neighbor scheme."""
+        iz, rz, dz, bz = find_rel_nearest(z, self.Z)
+        return VRel(iz, rz, dz, bz)
+
+    def find_rel_v_lin(self, z):
+        """Find the rel-coord based on vertical center grid using the 2-point linear scheme."""
+        iz, rz, dz, bz = find_rel_z(z, self.Z, self.dZ)
+        return VLinRel(iz, rz, dz, bz)
 
     def find_rel_vl(self, z):
         """Find the rel-coord based on vertical staggered grid using the nearest neighbor scheme."""
         iz, rz, dz, bz = find_rel_nearest(z, self.Zl)
-        return iz.astype(int), rz, dz, bz
+        return VlRel(iz, rz, dz, bz)
 
     def find_rel_vl_lin(self, z):
         """Find the rel-coord based on vertical staggered grid using the 2-point linear scheme."""
         iz, rz, dz, bz = find_rel_z(z, self.Zl, self.dZl, dz_above_z=False)
-        return iz.astype(int), rz, dz, bz
-
-    def find_rel_v(self, z):
-        """Find the rel-coord based on vertical center grid using the nearest neighbor scheme."""
-        iz, rz, dz, bz = find_rel_z(z, self.Zl, self.dZl)
-        return (iz - 1).astype(int), rz - 0.5, dz, bz
-
-    def find_rel_v_lin(self, z):
-        """Find the rel-coord based on vertical center grid using the 2-point linear scheme."""
-        iz, rz, dz, bz = find_rel_z(z, self.Z, self.dZ)
-        return iz.astype(int), rz, dz, bz
+        return VlLinRel(iz, rz, dz, bz)
 
     def find_rel_t(self, t):
-        """Find the rel-coord based along the temporal direction using the nearest neighbor scheme."""
+        """Find the rel-coord based on the temporal direction using the nearest neighbor scheme."""
         it, rt, dt, bt = find_rel_nearest(t, self.ts)
-        return it.astype(int), rt, dt, bt
+        return TRel(it, rt, dt, bt)
 
     def find_rel_t_lin(self, t):
-        """Find the rel-coord based along the temporal direction using the 2-point linear scheme."""
+        """Find the rel-coord based on the temporal direction using the 2-point linear scheme."""
         it, rt, dt, bt = find_rel_time(t, self.ts)
-        return it.astype(int), rt, dt, bt
-
-    def _find_rel_3d(self, x, y, z):  # pragma: no cover
-        # for internal test
-        faces, iys, ixs, rx, ry, cs, sn, dx, dy, bx, by = self.find_rel_h(
-            x, y, self.XC, self.YC, self.dX, self.dY, self.CS, self.SN, self.tree
-        )
-        iz, rz, dz, bz = find_rel_z(z, self.Zl, self.dZl)
-        iz = iz.astype(int)
-        return (
-            iz.astype(int),
-            faces,
-            iys,
-            ixs,
-            rx,
-            ry,
-            rz,
-            cs,
-            sn,
-            dx,
-            dy,
-            dz,
-            bx,
-            by,
-            bz,
-        )
-
-    def _find_rel_4d(self, x, y, z, t):  # pragma: no cover
-        # for internal tests
-        faces, iys, ixs, rx, ry, cs, sn, dx, dy, bx, by = self.find_rel_h(
-            x, y, self.XC, self.YC, self.dX, self.dY, self.CS, self.SN, self.tree
-        )
-        iz, rz, dz, bz = find_rel_z(z, self.Zl, self.dZl)
-        iz = iz.astype(int)
-        it, rt, dt, bt = find_rel_time(t, self.ts)
-        it = it.astype(int)
-        return (
-            it.astype(int),
-            iz.astype(int),
-            faces,
-            iys,
-            ixs,
-            rx,
-            ry,
-            rz,
-            rt,
-            cs,
-            sn,
-            dx,
-            dy,
-            dz,
-            dt,
-            bx,
-            by,
-            bz,
-            bt,
-        )
-
-    def _find_rel(self, *arg):  # pragma: no cover
-        # Internal testing
-        if len(arg) == 2:
-            return self.find_rel_2d(*arg)
-        if len(arg) == 3:
-            return self.find_rel_3d(*arg)
-        if len(arg) == 4:
-            return self.find_rel_4d(*arg)
+        return TLinRel(it, rt, dt, bt)
```

### Comparing `seaduck-0.1.2/seaduck/oceinterp.py` & `seaduck-0.1.3/seaduck/oceinterp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,137 +1,146 @@
 import warnings
 
 import numpy as np
 
-from seaduck.eulerian import position
+from seaduck.eulerian import Position
 from seaduck.kernel_weight import KnW
-from seaduck.lagrangian import particle, uknw, vknw
+from seaduck.lagrangian import Particle, uknw, vknw
 from seaduck.ocedata import OceData
+from seaduck.utils import convert_time
 
 lagrange_token = "__particle."
 
 
 def OceInterp(
     od,
-    varList,
+    var_list,
     x,
     y,
     z,
     t,
-    kernelList=None,
+    kernel_list=None,
     lagrangian=False,
     lagrange_kwarg={},
     update_stops="default",
     return_in_between=True,
     return_pt_time=True,
     kernel_kwarg={},
 ):
     """Interp for people who just want to take a quick look.
 
     **This is the centerpiece function of the package, through which
     you can access almost all of its functionality.**.
 
-    **Parameters:**
-
-    + od: OceInterp.OceData object or xarray.Dataset (limited support for netCDF Dataset)
+    Parameters
+    ----------
+    od: OceInterp.OceData object or xarray.Dataset (limited support for netCDF Dataset)
         The dataset to work on.
-    + varList: str or list
+    var_list: str or list
         A list of variable or pair of variables.
-    + kernelList: OceInterp.KnW or list of OceInterp.KnW objects
+    kernel_list: OceInterp.KnW or list of OceInterp.KnW objects, optional
         Indicates which kernel to use for each interpolation.
-    + x, y, z: numpy.ndarray
+    x, y, z: numpy.ndarray, float
         The location of the particles, where x and y are in degrees,
         and z is in meters (deeper locations are represented by more negative values).
-    + t: numpy.ndarray
+    t: numpy.ndarray, float, string/numpy.datetime64
         In the Eulerian scheme, this represents the time of interpolation.
         In the Lagrangian scheme, it represents the time needed for output.
-    + lagrangian: bool
+    lagrangian: bool, default False
         Specifies whether the interpolation is done in the Eulerian or Lagrangian scheme.
-    + lagrange_kwarg: dict
-        Keyword arguments passed into the OceInterp.lagrangian.particle object.
-    + update_stops: None, 'default', or iterable of float
+    lagrange_kwarg: dict, optional
+        Keyword arguments passed into the OceInterp.lagrangian.Particle object.
+    update_stops: None, 'default', or iterable of float
         Specifies the time to update the prefetch velocity.
-    + return_in_between: bool
+    return_in_between: bool, default True
         In Lagrangian mode, this returns the interpolation not only at time t,
         but also at every point in time when the speed is updated.
-    + return_pt_time: bool
+    return_pt_time: bool, default True
         Specifies whether to return the time of all the steps.
-    + kernel_kwarg: dict
+    kernel_kwarg: dict, optional
         keyword arguments to pass into seaduck.KnW object.
     """
     if not isinstance(od, OceData):
         od = OceData(od)
 
-    if isinstance(varList, dict):
-        kernelList = list(varList.values())
-        varList = list(varList.keys())
-        print(f"result will be in the order of {varList}")
-    elif isinstance(varList, str):
-        varList = [varList]
-    elif isinstance(varList, tuple):
-        varList = [varList]
-    elif isinstance(varList, list):
+    if isinstance(var_list, dict):
+        kernel_list = list(var_list.values())
+        var_list = list(var_list.keys())
+    elif isinstance(var_list, str):
+        var_list = [var_list]
+    elif isinstance(var_list, tuple):
+        var_list = [var_list]
+    elif isinstance(var_list, list):
         pass
     else:
-        raise ValueError("varList type not recognized.")
-    if isinstance(kernelList, list):
+        raise ValueError("var_list type not recognized.")
+    if isinstance(kernel_list, list):
         pass
-    elif kernelList is None:
-        kernelList = []
+    elif kernel_list is None:
+        kernel_list = []
         the_kernel = KnW(**kernel_kwarg)
-        for i in varList:
+        for i in var_list:
             if isinstance(i, str):
-                kernelList.append(the_kernel)
+                kernel_list.append(the_kernel)
             elif isinstance(i, tuple):
-                if kernel_kwarg != dict():
-                    kernelList.append((the_kernel, the_kernel))
+                if kernel_kwarg != {}:
+                    kernel_list.append((the_kernel, the_kernel))
                 else:
-                    kernelList.append((uknw, vknw))
+                    kernel_list.append((uknw, vknw))
             else:
-                raise ValueError("varList need to be made up of string or tuples")
+                raise ValueError(
+                    "members of var_list need to be made up of string or tuples"
+                )
+    if isinstance(t, np.ndarray):
+        if np.issubdtype(t.dtype, np.datetime64) or np.issubdtype(t.dtype, str):
+            t = np.array([convert_time(some_t) for some_t in t])
+    elif isinstance(t, (np.datetime64, str)):
+        t = convert_time(t)
+    else:
+        raise ValueError("time format not supported")
     if not lagrangian:
-        pt = position()
+        pt = Position()
         pt.from_latlon(x=x, y=y, z=z, t=t, data=od)
-        for i, var in enumerate(varList):
+        for i, var in enumerate(var_list):
             if lagrange_token in var:
                 raise AttributeError(
-                    "__particle variables is only available for Lagrangian particles"
+                    "__particle variables is only available for Lagrangian Particles"
                 )
-        R = pt.interpolate(varList, kernelList)
-        return R
+        to_return = pt.interpolate(var_list, kernel_list)
+        return to_return
 
     else:
         try:
             assert len(t) > 1
-        except AssertionError:
+        except AssertionError as exc:
             raise ValueError(
-                "There needs to be at least two time steps to run the lagrangian particle"
-            )
+                "There needs to be at least two time steps to run the lagrangian Particle"
+            ) from exc
         t_start = t[0]
         t_nec = t[1:]
-        pt = particle(
+        pt = Particle(
             x=x, y=y, z=z, t=np.ones_like(x) * t_start, data=od, **lagrange_kwarg
         )
         stops, raw = pt.to_list_of_time(
             t_nec, update_stops=update_stops, return_in_between=return_in_between
         )
-        R = []
-        for i, var in enumerate(varList):
+        to_return = []
+        for i, var in enumerate(var_list):
             if var == lagrange_token + "raw":
-                R.append(raw)
+                to_return.append(raw)
             elif lagrange_token in var:
                 sublist = []
                 for snap in raw:
-                    sublist.append(snap.__dict__[var[len(lagrange_token) :]])
-                R.append(sublist)
+                    sublist.append(getattr(snap, var[len(lagrange_token) :]))
+                to_return.append(sublist)
             else:
                 sublist = []
                 for snap in raw:
-                    sublist.append(snap.interpolate(var, kernelList[i]))
-                R.append(sublist)
+                    sublist.append(snap.interpolate(var, kernel_list[i]))
+                to_return.append(sublist)
 
         if return_pt_time:
-            return stops, R
+            return stops, to_return
         else:
             if return_in_between:
                 warnings.warn("Some of the returns is not on the times you specified.")
-            return R
+            return to_return
```

### Comparing `seaduck-0.1.2/seaduck/topology.py` & `seaduck-0.1.3/seaduck/topology.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import copy
 import logging
 
 import numpy as np
 
 from seaduck.runtime_conf import compileable
 
-# If you have encountered a NotImplementedError and come to this file,
-# I suggest you read the ***class topology*** near the bottom of this file.
+# legal_tends = [0, 1, 2, 3]  # up,down,left,right #list(LLC_FACE_CONNECT.columns)
 
-tends = [0, 1, 2, 3]  # up,down,left,right #list(llc_face_connect.columns)
-
-llc_face_connect = np.array(
+LLC_FACE_CONNECT = np.array(
     [
         [1, 42, 12, 3],
         [2, 0, 11, 4],
         [6, 1, 10, 5],
         [4, 42, 0, 9],
         [5, 3, 1, 8],
         [6, 4, 2, 7],
@@ -24,86 +21,88 @@
         [12, 3, 8, 42],
         [2, 7, 6, 11],
         [1, 8, 10, 12],
         [0, 9, 11, 42],
     ]
 )
 
-directions = np.array([np.pi / 2, -np.pi / 2, np.pi, 0])
+DIRECTIONS = np.array([np.pi / 2, -np.pi / 2, np.pi, 0])
 
 
 @compileable
-def llc_mutual_direction(face, nface, transitive=False):
+def llc_mutual_direction(face, neighbor_face, transitive=False):
     """Find the relative orientation of two faces.
 
     The compileable version of mutual direction for llc grid.
-    See topology.mutual direction for more detail.
+    See Topology.mutual direction for more detail.
     """
-    edge_n = np.where(llc_face_connect[face] == nface)
-    nedge_n = np.where(llc_face_connect[nface] == face)
-    try:
-        found = edge_n[0][0] in [0, 1, 2, 3] and nedge_n[0][0] in [0, 1, 2, 3]
-    except Exception:  # It has to be a index error, but numba does not support that
+    connected_to_face = np.where(LLC_FACE_CONNECT[face] == neighbor_face)
+    connected_to_neigh = np.where(LLC_FACE_CONNECT[neighbor_face] == face)
+    if len(connected_to_face[0]) == 0:
         found = False
+    else:
+        found = connected_to_face[0][0] in [0, 1, 2, 3] and connected_to_neigh[0][
+            0
+        ] in [0, 1, 2, 3]
     if found:
-        return edge_n[0][0], nedge_n[0][0]
+        return connected_to_face[0][0], connected_to_neigh[0][0]
     elif transitive:
         common = -1
-        for i in llc_face_connect[face]:
-            if i in llc_face_connect[nface]:
+        for i in LLC_FACE_CONNECT[face]:
+            if i in LLC_FACE_CONNECT[neighbor_face]:
                 common = i
                 break
         if common < 0:
             raise ValueError(
                 "The two faces does not share common face, transitive did not help"
             )
         else:
-            edge_1 = np.where(llc_face_connect[face] == common)[0][0]
-            nedge_1 = np.where(llc_face_connect[common] == face)[0][0]
-            edge_2 = np.where(llc_face_connect[common] == nface)[0][0]
-            nedge_2 = np.where(llc_face_connect[nface] == common)[0][0]
-            if (edge_1 in [0, 1] and nedge_1 in [0, 1]) or (
-                edge_1 in [2, 3] and nedge_1 in [2, 3]
+            edge_1 = np.where(LLC_FACE_CONNECT[face] == common)[0][0]
+            new_edge_1 = np.where(LLC_FACE_CONNECT[common] == face)[0][0]
+            edge_2 = np.where(LLC_FACE_CONNECT[common] == neighbor_face)[0][0]
+            new_edge_2 = np.where(LLC_FACE_CONNECT[neighbor_face] == common)[0][0]
+            if (edge_1 in [0, 1] and new_edge_1 in [0, 1]) or (
+                edge_1 in [2, 3] and new_edge_1 in [2, 3]
             ):
-                return edge_2, nedge_2
-            elif (edge_2 in [0, 1] and nedge_2 in [0, 1]) or (
-                edge_2 in [2, 3] and nedge_2 in [2, 3]
+                return edge_2, new_edge_2
+            elif (edge_2 in [0, 1] and new_edge_2 in [0, 1]) or (
+                edge_2 in [2, 3] and new_edge_2 in [2, 3]
             ):
-                return edge_1, nedge_1
+                return edge_1, new_edge_1
             else:
                 raise NotImplementedError(
                     "the common face is not parallel to either of the face"
                 )
     else:
         raise ValueError("The two faces are not connected (transitive = False)")
 
 
 @compileable
 def llc_get_the_other_edge(face, edge):
     """See what is adjacent to the face by this edge.
 
     The compileable version of get_the_other_edge for llc grid.
-    See topology.get_the_other_edge for more detail.
+    See Topology.get_the_other_edge for more detail.
     """
-    face_connect = llc_face_connect
-    nface = face_connect[face, edge]
-    if nface == 42:
+    face_connect = LLC_FACE_CONNECT
+    neighbor_face = face_connect[face, edge]
+    if neighbor_face == 42:
         raise IndexError(
             "Reaching the edge where the face is not connected to any other face"
         )
-    nedge_n = np.where(face_connect[nface] == face)
-    return nface, nedge_n[0][0]
+    connected_to_neigh = np.where(face_connect[neighbor_face] == face)
+    return neighbor_face, connected_to_neigh[0][0]
 
 
 @compileable
 def box_ind_tend(ind, tend, iymax, ixmax):
     """Move an index in a direction.
 
     The compileable version of ind_tend for regional (box) grid.
-    See topology.ind_tend for more detail.
+    See Topology.ind_tend for more detail.
     """
     iy, ix = ind
     if tend == 0:
         iy += 1
     elif tend == 1:
         iy -= 1
     elif tend == 2:
@@ -119,15 +118,15 @@
 
 
 @compileable
 def x_per_ind_tend(ind, tend, iymax, ixmax):
     """Move an index in a direction.
 
     The compileable version of ind_tend for zonally periodic (x-per) grid.
-    See topology.ind_tend for more detail.
+    See Topology.ind_tend for more detail.
     """
     iy, ix = ind
     if tend == 0:
         iy += 1
     elif tend == 1:
         iy -= 1
     elif tend == 2:
@@ -144,80 +143,80 @@
 
 
 @compileable
 def llc_ind_tend(ind, tendency, iymax, ixmax):
     """Move an index in a direction.
 
     The compileable version of ind_tend for llc grid.
-    See topology.ind_tend for more detail.
+    See Topology.ind_tend for more detail.
     """
     #     iymax = 89
     #     ixmax = 89
     face, iy, ix = ind
     if tendency == 3:
         if ix != ixmax:
             ix += 1
         else:
-            nface, nedge = llc_get_the_other_edge(face, 3)
-            if nedge == 1:
-                face, iy, ix = [nface, 0, ixmax - iy]
-            elif nedge == 0:
-                face, iy, ix = [nface, iymax, iy]
-            elif nedge == 2:
-                face, iy, ix = [nface, iy, 0]
-            elif nedge == 3:
-                face, iy, ix = [nface, iymax - iy, ixmax]
+            neighbor_face, new_edge = llc_get_the_other_edge(face, 3)
+            if new_edge == 1:
+                face, iy, ix = [neighbor_face, 0, ixmax - iy]
+            elif new_edge == 0:
+                face, iy, ix = [neighbor_face, iymax, iy]
+            elif new_edge == 2:
+                face, iy, ix = [neighbor_face, iy, 0]
+            elif new_edge == 3:
+                face, iy, ix = [neighbor_face, iymax - iy, ixmax]
     if tendency == 2:
         if ix != 0:
             ix -= 1
         else:
-            nface, nedge = llc_get_the_other_edge(face, 2)
-            if nedge == 1:
-                face, iy, ix = [nface, 0, iy]
-            elif nedge == 0:
-                face, iy, ix = [nface, iymax, ixmax - iy]
-            elif nedge == 2:
-                face, iy, ix = [nface, iymax - iy, 0]
-            elif nedge == 3:
-                face, iy, ix = [nface, iy, ixmax]
+            neighbor_face, new_edge = llc_get_the_other_edge(face, 2)
+            if new_edge == 1:
+                face, iy, ix = [neighbor_face, 0, iy]
+            elif new_edge == 0:
+                face, iy, ix = [neighbor_face, iymax, ixmax - iy]
+            elif new_edge == 2:
+                face, iy, ix = [neighbor_face, iymax - iy, 0]
+            elif new_edge == 3:
+                face, iy, ix = [neighbor_face, iy, ixmax]
     if tendency == 0:
         if iy != iymax:
             iy += 1
         else:
-            nface, nedge = llc_get_the_other_edge(face, 0)
-            if nedge == 1:
-                face, iy, ix = [nface, 0, ix]
-            elif nedge == 0:
-                face, iy, ix = [nface, iymax, ixmax - ix]
-            elif nedge == 2:
-                face, iy, ix = [nface, iymax - ix, 0]
-            elif nedge == 3:
-                face, iy, ix = [nface, ix, ixmax]
+            neighbor_face, new_edge = llc_get_the_other_edge(face, 0)
+            if new_edge == 1:
+                face, iy, ix = [neighbor_face, 0, ix]
+            elif new_edge == 0:
+                face, iy, ix = [neighbor_face, iymax, ixmax - ix]
+            elif new_edge == 2:
+                face, iy, ix = [neighbor_face, iymax - ix, 0]
+            elif new_edge == 3:
+                face, iy, ix = [neighbor_face, ix, ixmax]
     if tendency == 1:
         if iy != 0:
             iy -= 1
         else:
-            nface, nedge = llc_get_the_other_edge(face, 1)
-            if nedge == 1:
-                face, iy, ix = [nface, 0, ixmax - ix]
-            elif nedge == 0:
-                face, iy, ix = [nface, iymax, ix]
-            elif nedge == 2:
-                face, iy, ix = [nface, ix, 0]
-            elif nedge == 3:
-                face, iy, ix = [nface, iymax - ix, ixmax]
+            neighbor_face, new_edge = llc_get_the_other_edge(face, 1)
+            if new_edge == 1:
+                face, iy, ix = [neighbor_face, 0, ixmax - ix]
+            elif new_edge == 0:
+                face, iy, ix = [neighbor_face, iymax, ix]
+            elif new_edge == 2:
+                face, iy, ix = [neighbor_face, ix, 0]
+            elif new_edge == 3:
+                face, iy, ix = [neighbor_face, iymax - ix, ixmax]
     return (face, iy, ix)
 
 
 @compileable
 def llc_get_uv_mask_from_face(faces):
     """Get the masking of UV points.
 
     The compileable version of get_uv_mask_from_face for llc grid.
-    See topology.get_uv_mask_from_face for more detail.
+    See Topology.get_uv_mask_from_face for more detail.
     """
     # we are considering a row from the fatten_face
     # faces is essentially which face each node of the kernel is on.
     n = len(faces)  # it should have been m to be more consistent with other code
     UfromUvel = np.ones(n)
     UfromVvel = np.zeros(n)
     VfromUvel = np.zeros(n)
@@ -228,37 +227,39 @@
     else:
         for i in range(1, n):
             if faces[i] == faces[0]:
                 continue
             # if the face is not the same, we need to do something
             else:
                 # get how much the new face is rotated from the old face
-                edge, nedge = llc_mutual_direction(faces[0], faces[i], transitive=True)
-                rot = np.pi - directions[edge] + directions[nedge]
+                edge, new_edge = llc_mutual_direction(
+                    faces[0], faces[i], transitive=True
+                )
+                rot = np.pi - DIRECTIONS[edge] + DIRECTIONS[new_edge]
                 # you can think of this as a rotation matrix
                 UfromUvel[i] = np.cos(rot)
                 UfromVvel[i] = np.sin(rot)
                 VfromUvel[i] = -np.sin(rot)
                 VfromVvel[i] = np.cos(rot)
         return UfromUvel, UfromVvel, VfromUvel, VfromVvel
 
 
-class topology:
+class Topology:
     """Topology object.
 
     A light weight object that remembers the structure of the grid,
     what is connected, what is not. The core method is simply move the index to a direction.
     In the movie kill Bill, the bride sat in a car and said "wiggle your big toe".
     After the toe moved, "the hard part is over". You get the idea.
 
-    **Parameters:**
-
-    + od: xarray.Dataset, OceData object
+    Parameters
+    ----------
+    od: xarray.Dataset
         The dataset to record topological info from.
-    + typ: None, or str
+    typ: None, or str
         Type of the grid.
         Currently we support
         'box' for regional dataset,
         'x-periodic' for zonally periodic ones,
         'llc' for lat-lon-cap dataset.
         We recommend that users put None here,
         so that the type is figured out automatically.
@@ -266,19 +267,23 @@
 
     def __init__(self, od, typ=None):
         try:
             h_shape = od["XC"].shape
         except KeyError:
             try:
                 h_shape = (int(od["lat"].shape[0]), int(od["lon"].shape[0]))
-            except KeyError:
+            except KeyError as exc:
                 raise KeyError(
-                    "Either XC or lat/lon is needed to create the topology object"
-                )
+                    "Either XC or lat/lon is needed to create the Topology object"
+                ) from exc
         self.h_shape = h_shape
+        if "XG" in od.variables:
+            self.g_shape = od["XG"].shape
+        else:
+            self.g_shape = None
         try:
             self.itmax = len(od["time"]) - 1
         except (KeyError, TypeError):
             self.itmax = 0
         try:
             self.izmax = len(od["Z"]) - 1
         except (KeyError, TypeError):
@@ -317,204 +322,209 @@
                 else:
                     self.typ = "box"
 
     def get_the_other_edge(self, face, edge):
         """See what is adjacent to the face by this edge.
 
         The (edge) side of the (face) is connected to
-        the (nedge) side of the (nface).
+        the (new_edge) side of the (new_face).
         0,1,2,3 stands for up, down, left, right.
 
-        **Parameters:**
-
-        + face: int
+        Parameters
+        ----------
+        face: int
             The face of interst
-        + edge: 0,1,2,3
+        edge: 0,1,2,3
             which direction of the face we are looking for
 
-        **Returns:**
-
-        + nface: int
+        Returns
+        -------
+        new_face: int
             The face adjacent to face in the edge direction.
-        + nedge: 0,1,2,3
-            The face is connected to nface in which direction.
+        new_edge: 0,1,2,3
+            The face is connected to new_face in which direction.
         """
         if self.typ == "LLC":
             return llc_get_the_other_edge(face, edge)
         elif self.typ in ["x_periodic", "box"]:
-            raise Exception(
+            raise ValueError(
                 "It makes no sense to tinker with face_connection when there is only one face"
             )
         else:
             raise NotImplementedError
 
-    def mutual_direction(self, face, nface, **kwarg):
+    def mutual_direction(self, face, new_face, **kwarg):
         """Find the relative orientation of two faces.
 
         0,1,2,3 stands for up, down, left, right
         given 2 faces, the returns are
         1. the 2nd face is to which direction of the 1st face
         2. the 1st face is to which direction of the 2nd face.
         """
         if self.typ == "LLC":
-            return llc_mutual_direction(face, nface, **kwarg)
+            return llc_mutual_direction(face, new_face, **kwarg)
         elif self.typ in ["x_periodic", "box"]:
-            raise Exception(
+            raise ValueError(
                 "It makes no sense to tinker with face_connection when there is only one face"
             )
         else:
             raise NotImplementedError
 
-    def ind_tend(self, ind, tend, cuvg="C", **kwarg):
+    def ind_tend(self, ind, tend, cuvwg="C", **kwarg):
         """Move an index in a direction.
 
         ind is a tuple that is face,iy,ix,
         tendency again is up, down, left, right represented by 0,1,2,3
         return the next cell.
 
-        **Parameters:**
-
-        + ind: tuple
+        Parameters
+        ----------
+        ind: tuple
             The index to find the neighbor of
-        + tend: int
+        tend: int
             Which direction to move from the original index.
-        + cuvg:
+        cuvwg: str, default "C"
             Whether we are moving from C grid, U grid, V grid, or G grid.
-        + kwarg:dict
+        kwarg:dict, optional
             Keyword argument that currently only apply for the llc case.
-            Use gridoffset keyword when you are dealing with different grid-indexing,
-            -1 for MITgcm (default), 1 for NEMO.
         """
         if -1 in ind:
             # meaning invalid point
-            return tuple([-1 for i in ind])
-        #         if tend not in [0,1,2,3]:
-        #             raise Exception('Illegal move. Must be 0,1,2,3')
+            return tuple(-1 for i in ind)
         if self.typ == "LLC":
-            if cuvg == "C":
-                return llc_ind_tend(ind, tend, self.iymax, self.ixmax, **kwarg)
-            elif cuvg == "U":
-                UorV, R = self._ind_tend_U(ind, tend)
-                return R
-            elif cuvg == "V":
-                UorV, R = self._ind_tend_V(ind, tend)
-                return R
-            elif cuvg == "G":
-                raise NotImplementedError("G grid is not yet supported")
+            if cuvwg == "C":
+                to_return = llc_ind_tend(ind, tend, self.iymax, self.ixmax, **kwarg)
+            elif cuvwg == "U":
+                _, to_return = self._ind_tend_U(ind, tend)
+            elif cuvwg == "V":
+                _, to_return = self._ind_tend_V(ind, tend)
+            elif cuvwg == "G":
+                to_return = self._ind_tend_G(ind, tend)
             else:
                 raise ValueError("The type of grid point should be among C,U,V,G")
         elif self.typ == "x_periodic":
-            return x_per_ind_tend(ind, tend, self.iymax, self.ixmax, **kwarg)
+            to_return = x_per_ind_tend(ind, tend, self.iymax, self.ixmax, **kwarg)
         elif self.typ == "box":
-            return box_ind_tend(ind, tend, self.iymax, self.ixmax, **kwarg)
+            to_return = box_ind_tend(ind, tend, self.iymax, self.ixmax, **kwarg)
         else:
             raise NotImplementedError
+        return tuple(int(i) for i in to_return)
 
     def ind_moves(self, ind, moves, **kwarg):
         """Move an index in a serie of directions.
 
         moves being a list of directions (0,1,2,3),
         ind being the starting index,
         return the index after moving in the directions in the list.
 
-        **Parameters:**
-
-        + ind: tuple
+        Parameters
+        ----------
+        ind: tuple
             Index of the starting position
-        + moves: iterable
+        moves: iterable
             A sequence of steps to "walk" from the original position.
-        + kwarg: dict
+        kwarg: dict, optional
             Keyword arguments that pass into ind_tend.
         """
         if self.check_illegal(ind):
-            return tuple([-1 for i in ind])  # the origin is invalid
+            return tuple(-1 for i in ind)  # the origin is invalid
         if not set(moves).issubset({0, 1, 2, 3}):
             raise ValueError("Illegal move. Must be 0,1,2,3")
         if self.typ in ["LLC", "cubed_sphere"]:
             face, iy, ix = ind
             for k in range(len(moves)):
                 move = moves[k]
                 ind = self.ind_tend(ind, move, **kwarg)
                 if ind[0] != face:  # if the face has changed
-                    """
-                    there are times where the the kernel lies between
-                    2 faces that define 'left' differently. That's why
-                    when that happens we need to correct the direction
-                    you want to move the indexes.
-                    """
-                    edge, nedge = self.mutual_direction(face, ind[0], transitive=True)
-                    rot = (np.pi - directions[edge] + directions[nedge]) % (np.pi * 2)
+                    # there are times where the the kernel lies between
+                    # 2 faces that define 'left' differently. That's why
+                    # when that happens we need to correct the direction
+                    # you want to move the indexes.
+                    edge, new_edge = self.mutual_direction(
+                        face, ind[0], transitive=True
+                    )
+                    rot = (np.pi - DIRECTIONS[edge] + DIRECTIONS[new_edge]) % (
+                        np.pi * 2
+                    )
                     if np.isclose(rot, 0):
                         pass
                     elif np.isclose(rot, np.pi / 2):
                         moves[k + 1 :] = [[2, 3, 1, 0][move] for move in moves[k + 1 :]]
                     elif np.isclose(rot, 3 * np.pi / 2):
                         moves[k + 1 :] = [[3, 2, 0, 1][move] for move in moves[k + 1 :]]
                     face = ind[0]
                     # if the old face is on the left of the new face,
                     # the particle should be heading right
         elif self.typ in ["x_periodic", "box"]:
             for move in moves:
                 ind = self.ind_tend(ind, move)
-        return ind
+        return tuple(int(i) for i in ind)
 
-    def check_illegal(self, ind):
+    def check_illegal(self, ind, cuvwg="C"):
         """Check if the index is legal.
 
         A vectorized check to see whether the index is legal,
         index can be a tuple of numpy ndarrays.
         no negative index is permitted for sanity reason.
 
-        **Parameters:**
-
-        + ind: tuple
+        Parameters
+        ----------
+        ind: tuple
             Each element of the tuple is iterable of one dimension of the indexes.
+        cuvwg: 'C' or 'G'
+            Whether use the center grid or the corner grid.
         """
+        if cuvwg == "C":
+            the_shape = self.h_shape
+        else:
+            the_shape = self.g_shape
+
         if isinstance(ind[0], int):  # for single item
             result = False
             for i, z in enumerate(ind):
-                max_pos = self.h_shape[i]
-                if not (0 <= z <= max_pos - 1):
+                max_pos = the_shape[i]
+                if not 0 <= z <= max_pos - 1:
                     result = True
             return result
         else:  # for numpy ndarray
             result = np.zeros_like(ind[0])
             result = False  # make it cleaner
             for i, z in enumerate(ind):
-                max_pos = self.h_shape[i]
+                max_pos = the_shape[i]
                 result = np.logical_or(
                     np.logical_or((0 > z), (z > max_pos - 1)), result
                 )
             return result
 
     def ind_tend_vec(self, inds, tend, **kwarg):
         """Move many indices in a list of directions.
 
         Vectorized version for ind_tend method.
 
-        **Parameters:**
-
-        + inds: tuple or numpy.array
+        Parameters
+        ----------
+        inds: tuple of numpy.array or numpy.array
             Each element of the tuple is iterable of one dimension of the indexes.
-        + tend: iterable
+        tend: iterable
             Which direction should each index take.
-        + kwarg: dict
+        kwarg: dict,optional
             Keyword argument that feeds into ind_tend.
         """
         inds = np.array(inds)
         old_inds = copy.deepcopy(inds)
         move_dic = {
             0: np.array([1, 0]),  # delta_y,delta_x
             1: np.array([-1, 0]),
             2: np.array([0, -1]),
             3: np.array([0, 1]),
         }
-        naive_move = np.array([move_dic[i] for i in tend]).T.astype(int)
+        naive_move = np.array([move_dic[i] for i in tend], dtype=int).T
         inds[-2:] += naive_move
-        illegal = self.check_illegal(inds)
+        cuvwg = kwarg.get("cuvwg", "C")
+        illegal = self.check_illegal(inds, cuvwg=cuvwg)
         redo = np.array(np.where(illegal)).T
         particle_on_edge = False
         for num, loc in enumerate(redo):
             j = loc[0]
             ind = tuple(old_inds[:, j])
             try:
                 n_ind = self.ind_tend(ind, int(tend[j]), **kwarg)
@@ -530,52 +540,54 @@
 
     def _find_wall_between(self, ind1, ind2):
         """Return the wall between two adjacent cells.
 
         if the input is not adjacent, error may not be raised
         This scheme is only valid if there is face in the dimensions.
         """
-        (fc1, iy1, ix1) = ind1
-        (fc2, iy2, ix2) = ind2
-        Non_normal_connection = ValueError(
+        (fc1, _, _) = ind1
+        (fc2, _, _) = ind2
+        non_normal_connection = ValueError(
             f"The two face connecting the indexes {ind1},{ind2}"
             " are not connected in a normal way"
         )
         if fc1 == fc2:
-            R = tuple(np.ceil((np.array(ind1) + np.array(ind2)) / 2).astype(int))
-            other = ind1 if ind2 == R else ind2
-            (fcr, iyr, ixr) = R
-            (fco, iyo, ixo) = other
+            to_return = tuple(
+                np.ceil((np.array(ind1) + np.array(ind2)) / 2).astype(int)
+            )
+            other = ind1 if ind2 == to_return else ind2
+            (_, iyr, ixr) = to_return
+            (_, iyo, ixo) = other
             if ixr > ixo:
-                return "U", R
+                return "U", to_return
             elif iyr > iyo:
-                return "V", R
+                return "V", to_return
             else:
                 raise IndexError("there is no wall between a cell and itself")
                 # This error can be raised when there is three instead of four points in a corner
         else:
             d1to2, d2to1 = self.mutual_direction(fc1, fc2)
             if d1to2 in [0, 3]:
-                R = ind2
+                to_return = ind2
                 if d2to1 == 1:
-                    return "V", R
+                    return "V", to_return
                 elif d2to1 == 2:
-                    return "U", R
+                    return "U", to_return
                 else:
-                    raise Non_normal_connection
+                    raise non_normal_connection
             elif d2to1 in [0, 3]:
-                R = ind1
+                to_return = ind1
                 if d1to2 == 1:
-                    return "V", R
+                    return "V", to_return
                 elif d1to2 == 2:
-                    return "U", R
+                    return "U", to_return
                 else:
-                    raise Non_normal_connection
+                    raise non_normal_connection
             else:
-                raise Non_normal_connection
+                raise non_normal_connection
 
     def _ind_tend_U(self, ind, tend):
         """Move an U-index in a direction.
 
         A subset of ind_tend that deal with special issues
         that comes from staggered grid. Read ind_tend for more info.
         """
@@ -588,15 +600,15 @@
                 return "U", first
             else:
                 alter = self.ind_moves(ind, [2, tend])
                 # TODO: Add the case of alter == first for three-way join of faces.Low priority
                 return self._find_wall_between(first, alter)
 
     def _ind_tend_V(self, ind, tend):
-        """Move an V-index in a direction.
+        """Move a V-index in a direction.
 
         A subset of ind_tend that deal with special issues
         that comes from staggered grid. Read ind_tend for more info.
         """
         # TODO: implement different grid offset case
         if tend in [0, 1]:
             return "V", self.ind_tend(ind, tend)
@@ -604,33 +616,49 @@
             first = self.ind_tend(ind, tend)
             if first[0] == ind[0]:
                 return "V", first
             else:
                 alter = self.ind_moves(ind, [1, tend])
                 return self._find_wall_between(first, alter)
 
+    def _ind_tend_G(self, ind, tend):
+        """Move a G-index(corner point) in a direction.
+
+        If there is a index for the corner point at all,
+        it needs to be connected to the two edges with the same index.
+        Therefore, this will always work, regardless of the grid.
+        """
+        if tend in [0, 1]:
+            _, nind = self._ind_tend_U(ind, tend)
+            return nind
+        elif tend in [2, 3]:
+            _, nind = self._ind_tend_V(ind, tend)
+            return nind
+        else:
+            raise ValueError(f"tend {tend} not supported")
+
     def get_uv_mask_from_face(self, faces):
         """Get the masking of UV points.
 
         The background is as following:
         For a dataset with face connection,
         when one is finding the neighboring cells for vector interpolation,
         the fact that faces can be rotated against each other can create
         local inconsistency in vector definition near face connections.
         This method corrects that.
 
-        **Parameters:**
-
-        + faces: iterable
+        Parameters
+        ----------
+        faces: iterable
             1D iterable of faces, the first one is assumed to be the reference.
         """
         if self.typ == "LLC":
             return llc_get_uv_mask_from_face(faces)
         elif self.typ in ["x_periodic", "box"]:
-            raise Exception(
+            raise ValueError(
                 "It makes no sense to tinker with face_connection when there is only one face"
             )
         else:
             raise NotImplementedError
 
     def four_matrix_for_uv(self, fface):
         """Expand get_uv_mask_from_face to 2D array of faces."""
```

### Comparing `seaduck-0.1.2/seaduck/utils.py` & `seaduck-0.1.3/seaduck/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,80 +14,109 @@
 except ImportError:
     pass
 
 
 @functools.cache
 def pooch_prepare():
     """Prepare for loading datasets using pooch."""
-    POOCH = pooch.create(
+    pooch_testdata = pooch.create(
         path=pooch.os_cache("seaduck"),
         base_url="doi:10.5281/zenodo.7949168",
         registry=None,
     )
-    POOCH.load_registry_from_doi()  # Automatically populate the registry
-    POOCH_FETCH_KWARGS = {"progressbar": True}
-    return POOCH, POOCH_FETCH_KWARGS
+    pooch_testdata.load_registry_from_doi()  # Automatically populate the registry
+    pooch_fetch_kwargs = {"progressbar": True}
+    return pooch_testdata, pooch_fetch_kwargs
+
+
+def _flower_func(x, y, pedals=8, sin=True, vmin=0, vmax=1):
+    theta = np.arctan2(x, y)
+    r = np.hypot(x, y)
+    center = np.exp(-(r**2) * 8)
+    if sin:
+        pedal = np.abs(np.sin(pedals / 2 * theta)) / (1 + r)
+    else:
+        pedal = np.abs(np.cos(pedals / 2 * theta)) / (1 + r)
+    return (vmax - vmin) * np.maximum(pedal, center) + vmin
 
 
 def process_ecco(ds):
     """Add more meat to ECCO dataset after the skeleton is downloaded."""
+    np.random.seed(90)
     rand1 = np.random.random((50, 13, 90, 90))
     rand2 = np.random.random((50, 13, 90, 90))
-    rand3 = np.random.random((50, 13, 90, 90))
+    flower_x, flower_y = tuple(np.linspace(-1, 1, 90) for i in range(2))
+    flower_x, flower_y = np.meshgrid(flower_x, flower_y)
+    salt_flower = _flower_func(flower_x, flower_y, vmin=33, vmax=36)
+    etan_flower = _flower_func(flower_x, flower_y, vmin=-0.1, vmax=0.1, sin=False)
+    salt_4d = np.zeros((50, 13, 90, 90))
+    salt_4d[:] = salt_flower
+    etan_3d = np.zeros((13, 90, 90))
+    etan_3d[:] = etan_flower
+
     ds["UVELMASS"] = xr.DataArray(
-        np.stack([rand1, rand2, rand3], axis=0), dims=("time", "Z", "face", "Y", "Xp1")
+        np.stack([rand1, rand2, rand2], axis=0), dims=("time", "Z", "face", "Y", "Xp1")
     )
     ds["UVELMASS"][0] = ds.UVELMASS1
     ds["UVELMASS"][1] = ds.UVELMASS1 * rand1
     ds["UVELMASS"][2] = ds.UVELMASS1 * rand2
 
     ds["WVELMASS"] = xr.DataArray(
-        np.stack([rand1, rand2, rand3], axis=0), dims=("time", "Zl", "face", "Y", "X")
+        np.stack([rand1, rand2, rand2], axis=0), dims=("time", "Zl", "face", "Y", "X")
     )
     ds["WVELMASS"][0] = ds.WVELMASS1
     ds["WVELMASS"][1] = ds.WVELMASS1 * rand1
     ds["WVELMASS"][2] = ds.WVELMASS1 * rand2
 
     ds["VVELMASS"] = xr.DataArray(
-        np.stack([rand1, rand2, rand3], axis=0), dims=("time", "Z", "face", "Yp1", "X")
+        np.stack([rand1, rand2, rand2], axis=0), dims=("time", "Z", "face", "Yp1", "X")
     )
     ds["VVELMASS"][0] = ds.VVELMASS1
     ds["VVELMASS"][1] = ds.VVELMASS1 * rand1
     ds["VVELMASS"][2] = ds.VVELMASS1 * rand2
 
     ds["SALT"] = xr.DataArray(
-        np.stack([rand1, rand2, rand3], axis=0), dims=("time", "Z", "face", "Y", "X")
+        np.stack([salt_4d, salt_4d * 2 - 34.5, salt_4d], axis=0),
+        dims=("time", "Z", "face", "Y", "X"),
     )
     ds["SALT_snap"] = xr.DataArray(
-        np.stack([rand3, rand1], axis=0), dims=("time_midp", "Z", "face", "Y", "X")
+        np.stack([salt_4d * 2 - 34.5, salt_4d * 2.5], axis=0),
+        dims=("time_midp", "Z", "face", "Y", "X"),
+    )
+    ds["ETAN"] = xr.DataArray(
+        np.stack([etan_3d, etan_3d * 2, etan_3d * 3], axis=0),
+        dims=("time", "face", "Y", "X"),
+    )
+    ds["ETAN_snap"] = xr.DataArray(
+        np.stack([etan_3d * 1.5, etan_3d * 2.5], axis=0),
+        dims=("time_midp", "face", "Y", "X"),
     )
-    ds["ETAN"] = xr.DataArray(rand1[:3], dims=("time", "face", "Y", "X"))
-    ds["ETAN_snap"] = xr.DataArray(rand3[:2], dims=("time_midp", "face", "Y", "X"))
     return ds
 
 
 @functools.cache
 def get_dataset(name):
     """Use pooch to download datasets from cloud.
 
-    This is just for testing purposes.
-    **Parameters:**
+        This is just for testing purposes.
 
-    + name: string
+    Parameters
+    ----------
+    name: string
         The name of dataset, now support "ecco", "aviso", "curv", "rect"
     """
-    POOCH, POOCH_FETCH_KWARGS = pooch_prepare()
-    fnames = POOCH.fetch(f"{name}.tar.gz", pooch.Untar(), **POOCH_FETCH_KWARGS)
+    pooch_testdata, pooch_fetch_kwargs = pooch_prepare()
+    fnames = pooch_testdata.fetch(f"{name}.tar.gz", pooch.Untar(), **pooch_fetch_kwargs)
     ds = xr.open_zarr(os.path.commonpath(fnames))
     if name == "ecco":
         return process_ecco(ds)
     return ds
 
 
-def rel_lon(x, ref_lon):
+def chg_ref_lon(x, ref_lon):
     """Change the definition of 0 longitude.
 
     Return how much east one need to go from ref_lon to x
     This function aims to address
     the confusion caused by the discontinuity in longitude.
     """
     return (x - ref_lon) % 360
@@ -102,143 +131,120 @@
 
 
 def get_key_by_value(d, value):
     """Find one of the keys in a dictionary.
 
     the key that correspond to the given value.
 
-    **Parameters:**
-
-    + d: dictionaty
+    Parameters
+    ----------
+    d: dictionaty
         dictionary to lookup key from
-    + value: object
+    value: object
         A object that has __eq__ method.
     """
     for k, v in d.items():
         if v == value:
             return k
     return None
 
 
 @compileable
-def spherical2cartesian(Y, X, R=6371.0):
+def spherical2cartesian(lat, lon, R=6371.0):
     """Convert spherical coordinates to cartesian.
 
-    **Parameters:**
-
-    + Y: np.array
+    Parameters
+    ----------
+    lat: np.array
         Spherical Y coordinate (latitude)
-    + X: np.array
+    lon: np.array
         Spherical X coordinate (longitude)
-    + R: scalar
+    R: scalar
         Earth radius in km
         If None, use geopy default
 
-    **Returns:**
-
-    + x: np.array
+    Returns
+    -------
+    x: np.array
         Cartesian x coordinate
-    + y: np.array
+    y: np.array
         Cartesian y coordinate
-    + z: np.array
+    z: np.array
         Cartesian z coordinate
     """
     # Convert
-    Y_rad = np.deg2rad(Y)
-    X_rad = np.deg2rad(X)
-    x = R * np.cos(Y_rad) * np.cos(X_rad)
-    y = R * np.cos(Y_rad) * np.sin(X_rad)
-    z = R * np.sin(Y_rad)
+    y_rad = np.deg2rad(lat)
+    x_rad = np.deg2rad(lon)
+    x = R * np.cos(y_rad) * np.cos(x_rad)
+    y = R * np.cos(y_rad) * np.sin(x_rad)
+    z = R * np.sin(y_rad)
 
     return x, y, z
 
 
 @compileable
-def to_180(x):
+def to_180(x, peri=360):
     """Convert any longitude scale to [-180,180)."""
-    x = x % 360
-    return x + (-1) * (x // 180) * 360
+    x = x % peri % peri
+    # underflow resistant
+    return x + (-1) * (x // (peri / 2)) * peri
 
 
 def local_to_latlon(u, v, cs, sn):
     """Convert local vector to north-east."""
     uu = u * cs - v * sn
     vv = u * sn + v * cs
     return uu, vv
 
 
 @compileable
-def rel2latlon(rx, ry, rzl, cs, sn, dx, dy, dzl, dt, bx, by, bzl):
+def rel2latlon(rx, ry, cs, sn, dx, dy, bx, by):
     """Translate the spatial rel-coords into lat-lon-dep coords."""
     temp_x = rx * dx / deg2m
     temp_y = ry * dy / deg2m
     dlon = (temp_x * cs - temp_y * sn) / np.cos(by * np.pi / 180)
     dlat = temp_x * sn + temp_y * cs
     lon = dlon + bx
     lat = dlat + by
-    dep = bzl + dzl * rzl
-    return lon, lat, dep
+    return lon, lat
 
 
-def get_combination(lst, select):
-    """Get the combinations of the list.
-
-    Iteratively find all the combination that
-    has (select) amount of elements
-    and every element belongs to lst
-    This is almost the same as the one in itertools.
-    """
-    if select == 1:
-        return [[num] for num in lst]
-    else:
-        the_lst = []
-        for i, num in enumerate(lst):
-            sub_lst = get_combination(lst[i + 1 :], select - 1)
-            for com in sub_lst:
-                com.append(num)
-            #             print(sub_lst)
-            the_lst += sub_lst
-        return the_lst
-
-
-def create_tree(X, Y, R=6371, leafsize=16):
+def create_tree(x, y, R=6371.0, leafsize=16):
     """Create a cKD tree object.
 
-    **Parameters:**
-
-    + X,Y: np.ndarray
+    Parameters
+    ----------
+    x,y: np.ndarray
         longitude and latitude of the grid location
-    + R: float
+    R: float
         The radius in kilometers of the planet.
-    + leafsize: int
+    leafsize: int
         When to switch to brute force search.
     """
     if R:
-        x, y, z = spherical2cartesian(Y=Y, X=X, R=R)
+        x, y, z = spherical2cartesian(lat=y, lon=x, R=R)
     else:
-        x = X
-        y = Y
-        z = xr.zeros_like(Y)
+        z = xr.zeros_like(y)
 
     # Stack
-    rid_value = 777777
+    ridiculous_value = 777777
     if isinstance(x, xr.DataArray):
-        x = x.stack(points=x.dims).fillna(rid_value).data
-        y = y.stack(points=y.dims).fillna(rid_value).data
-        z = z.stack(points=z.dims).fillna(rid_value).data
+        x = x.fillna(ridiculous_value).data.ravel()
+        y = y.fillna(ridiculous_value).data.ravel()
+        z = z.fillna(ridiculous_value).data.ravel()
     elif isinstance(x, np.ndarray):
         x = x.ravel()
-        np.nan_to_num(x.ravel(), nan=rid_value, copy=False)
+        np.nan_to_num(x.ravel(), nan=ridiculous_value, copy=False)
         y = y.ravel()
-        np.nan_to_num(y.ravel(), nan=rid_value, copy=False)
+        np.nan_to_num(y.ravel(), nan=ridiculous_value, copy=False)
         z = z.ravel()
-        np.nan_to_num(z.ravel(), nan=rid_value, copy=False)
+        np.nan_to_num(z.ravel(), nan=ridiculous_value, copy=False)
 
     # Construct KD-tree
-    tree = spatial.cKDTree(np.column_stack((x, y, z)), leafsize=leafsize)
+    tree = spatial.cKDTree(np.vstack((x, y, z)).T, leafsize=leafsize)
 
     return tree
 
 
 def NoneIn(lst):
     """See if there is a None in the iterable object. Return a Boolean."""
     ans = False
@@ -246,369 +252,245 @@
         if i is None:
             ans = True
             break
     return ans
 
 
 @compileable
-def find_ind_z(array, value):
-    """Find the index of the nearest level that is lower."""
-    array = np.asarray(array)
-    idx = np.argmin(np.abs(array - value))
-    if array[idx] > value:
-        # z is special because it does not make
-        # much sense to interpolate beyond the two layers
-        idx += 1
-    idx = int(idx)
-    return idx, array[idx]
-
-
-@compileable
-def find_ind_t(array, value):
-    """Find the index of the latest time that is before the time."""
-    array = np.asarray(array)
-    idx = np.argmin(np.abs(array - value))
-    if array[idx] > value and idx != 0:
-        idx -= 1
-    idx = int(idx)
-    return idx, array[idx]
-
-
-@compileable
-def find_ind_nearest(array, value):
-    """Find the index of the nearest value to the given value."""
-    array = np.asarray(array)
-    idx = np.argmin(np.abs(array - value))
-    idx = int(idx)
-    return idx, array[idx]
-
-
-@compileable
-def find_ind_periodic(array, value, peri):
+def find_ind(array, value, peri=None, ascending=1, above=True):
     """Find the index of the nearest value to the given value.
 
-    Here the values are assumed to be periodic.
+    Parameters
+    ----------
+    array: numpy.ndarray
+        1D numpy array to search index from
+    value: number
+        The value to find nearest neighbor with
+    peri: number, optional
+        The periodicity of the array.
+        For example, 360 for longitude.
+    ascending: int, default 1
+        Whether the array is in ascending order.
+        1 for ascending order, -1 for descending order.
+    above: boolean, default True
+        If True, return the index of the largest item in
+        array smaller than value.
+        Otherwise, return the closest value.
     """
     array = np.asarray(array)
-    idx = np.argmin(np.abs((array - value) % peri))
-    idx = int(idx)
-    return idx, array[idx]
+    if peri is None:
+        index = np.argmin(np.abs(array - value))
+    else:
+        index = np.argmin(np.abs(to_180((array - value), peri=peri)))
+    if above and array[index] > value and peri is None:
+        index -= ascending * 1
+    if index < 0 or index >= len(array):
+        raise ValueError("Value out of bound.")
+    index = int(index)
+    return index, array[index]
 
 
 deg2m = 6271e3 * np.pi / 180
 
 
-def find_ind_h(Xs, Ys, tree, h_shape):
+def find_ind_h(lons, lats, tree, h_shape):
     """Use ckd tree to find the horizontal indexes,."""
-    x, y, z = spherical2cartesian(Ys, Xs)
+    x, y, z = spherical2cartesian(lats, lons)
     _, index1d = tree.query(np.array([x, y, z]).T)
     if len(h_shape) == 3:
-        faces, iys, ixs = np.unravel_index((index1d), h_shape)
+        face, iy, ix = np.unravel_index((index1d), h_shape)
     elif len(h_shape) == 2:
-        faces = None
-        iys, ixs = np.unravel_index((index1d), h_shape)
-    return faces, iys, ixs
+        face = None
+        iy, ix = np.unravel_index((index1d), h_shape)
+    return face, iy, ix
 
 
 @compileable
+def find_rel(
+    value, array, darray=None, ascending=1, above=True, peri=None, dx_right=True
+):
+    """Find the rel-coords of the 1D coords.
+
+    The backend for all find_rel functions
+
+    Parameters
+    ----------
+    value: numpy.ndarray
+        1D array for the value to find rel-coords.
+    array: numpy.ndarray
+        The array of potential reference levels.
+    darray: numpy.ndarray, optional
+        The distances between reference levels.
+    peri: number, optional
+        The periodicity of the array.
+        For example, 360 for longitude.
+    ascending: int, default 1
+        Whether the array is in ascending order.
+        1 for ascending order, -1 for descending order.
+    above: boolean, default True
+        If True, return the index of the largest item in
+        array smaller than value.
+        Otherwise, return the closest value.
+    dx_right: boolean, default True
+        If True, darray[i] = abs(array[i+1] - array[i])
+
+    Returns
+    -------
+    ix: numpy.ndarray
+        Indexes of the reference level
+    rx: numpy.ndarray
+        Non-dimensional distance to the reference level
+    dx: numpy.ndarray
+        distance between the reference t level and the next one.
+    bx: numpy.ndarray
+        Value of the reference level
+    """
+    if darray is None:
+        darray = np.abs(array[1:] - array[:-1])
+        darray = np.append(darray, darray[-1])
+        dx_right = True
+    ix_arr = np.zeros(len(value), dtype="int")
+    rx_arr = np.ones_like(value) * 0.0
+    dx_arr = np.ones_like(value) * 0.0
+    bx_arr = np.ones_like(value) * 0.0
+
+    dx_offset = int(not dx_right) + int(ascending > 0) - 1
+    for i, x in enumerate(value):
+        ix, bx = find_ind(array, x, ascending=ascending, above=above, peri=peri)
+        if peri is None:
+            dx = x - bx
+        else:
+            dx = to_180(x - bx, peri=peri)
+
+        if not above or peri is not None:
+            # peri not None will effectively overwrite above
+            dx_offset = int(not dx_right) + int(ascending * dx > 0) - 1
+        index = ix + dx_offset
+
+        ix_arr[i] = ix
+        rx_arr[i] = dx / darray[index]
+        dx_arr[i] = darray[index]
+        bx_arr[i] = bx
+    return ix_arr, rx_arr, dx_arr, bx_arr
+
+
+# Here are a few partial functions for find_rel
+@compileable
 def find_rel_nearest(value, ts):
     """Find the rel-coords based on the find_ind_nearest method."""
-    its = np.zeros_like(value)
-    rts = np.ones_like(value) * 0.0
-    # the way to create zeros with float32 type
-    dts = np.ones_like(value) * 0.0
-    bts = np.ones_like(value) * 0.0
-
-    DT = np.zeros(len(ts) + 1)
-    DT[1:-1] = ts[1:] - ts[:-1]
-    DT[0] = DT[1]
-    DT[-1] = DT[-2]
-    for i in range(len(value)):
-        t = value[i]
-        it, bt = find_ind_nearest(ts, t)
-        delta_t = t - bt
-        if delta_t * DT[it] > 0:
-            Delta_t = DT[it + 1]
-        else:
-            Delta_t = DT[it]
-        rt = delta_t / abs(Delta_t)
-        its[i] = it
-        rts[i] = rt
-        dts[i] = abs(Delta_t)
-        bts[i] = bt
-    return its, rts, dts, bts
+    return find_rel(value, ts, above=False)
 
 
 @compileable
 def find_rel_periodic(value, ts, peri):
     """Find the rel-coords based on the find_ind_periodic method."""
-    its = np.zeros_like(value)
-    rts = np.ones_like(value) * 0.0
-    # the way to create zeros with float32 type
-    dts = np.ones_like(value) * 0.0
-    bts = np.ones_like(value) * 0.0
-
-    DT = np.zeros(len(ts) + 1)
-    DT[1:-1] = ts[1:] - ts[:-1]
-    DT[0] = DT[1]
-    DT[-1] = DT[-2]
-    for i in range(len(value)):
-        t = value[i]
-        it, bt = find_ind_periodic(ts, t, peri)
-        delta_t = (t - bt) % peri
-        if delta_t * DT[i] > 0:
-            Delta_t = DT[it + 1]
-        else:
-            Delta_t = DT[it]
-        rt = delta_t / abs(Delta_t)
-        its[i] = it
-        rts[i] = rt
-        dts[i] = abs(Delta_t)
-        bts[i] = bt
-    return its, rts, dts, bts
+    return find_rel(value, ts, peri=peri)
 
 
 @compileable
-def find_rel_z(depth, some_z, some_dz, dz_above_z=True):
+def find_rel_z(depth, some_z, some_dz=None, dz_above_z=True):
     """Find the rel-coords of the vertical coords.
 
-    **Paramters:**
-
-    + depth: numpy.ndarray
+    Parameters
+    ----------
+    depth: numpy.ndarray
         1D array for the depth of interest in meters.
         More negative means deeper.
-    + some_z: numpy.ndarray
+    some_z: numpy.ndarray
         The depth of reference depth.
-    + some_dz: numpy.ndarray
+    some_dz: numpy.ndarray or None
         dz_i = abs(z_{i+1}- z_i)
-    + dz_above_z: Boolean
+    dz_above_z: Boolean
         Whether the dz as the distance between the depth level and
         a shallower one(True) or a deeper one(False)
 
-    **Returns:**
-
-    + iz: numpy.ndarray
+    Returns
+    -------
+    iz: numpy.ndarray
         Indexes of the reference z level
-    + rz: numpy.ndarray
+    rz: numpy.ndarray
         Non-dimensional distance to the reference z level
-    + dz: numpy.ndarray
+    dz: numpy.ndarray
         distance between the reference z level and the next one.
     """
-    izs = np.zeros_like(depth)
-    rzs = np.ones_like(depth) * 0.0
-    # the way to create zeros with float32 type
-    dzs = np.ones_like(depth) * 0.0
-    bzs = np.ones_like(depth) * 0.0
-    for i, d in enumerate(depth):
-        iz, bz = find_ind_z(some_z, d)
-        izs[i] = iz
-        bzs[i] = bz
-        #         try:
-        delta_z = d - bz
-        #         except IndexError:
-        #             raise IndexError('the point is too deep')
-        if dz_above_z:
-            Delta_z = some_dz[iz]
-        else:
-            Delta_z = some_dz[iz - 1]
-        dzs[i] = Delta_z
-        rzs[i] = delta_z / Delta_z
-    return izs, rzs, dzs, bzs
+    return find_rel(
+        depth, some_z, darray=some_dz, ascending=-1, dx_right=(not dz_above_z)
+    )
 
 
 @compileable
 def find_rel_time(time, ts):
     """Find the rel-coords of the temporal coords.
 
-    **Paramters:**
-
-    + time: numpy.ndarray
+    Parameters
+    ----------
+    time: numpy.ndarray
         1D array for the time since 1970-01-01 in seconds.
-    + ts: numpy.ndarray
+    ts: numpy.ndarray
         The time of model time steps also in seconds.
 
-    **Returns:**
-
-    + it: numpy.ndarray
+    Returns
+    -------
+    it: numpy.ndarray
         Indexes of the reference t level
-    + rt: numpy.ndarray
+    rt: numpy.ndarray
         Non-dimensional distance to the reference t level
-    + dt: numpy.ndarray
+    dt: numpy.ndarray
         distance between the reference t level and the next one.
     """
-    its = np.zeros(time.shape)
-    rts = np.ones(time.shape) * 0.0
-    dts = np.ones(time.shape) * 0.0
-    bts = np.ones(time.shape) * 0.0
-
-    for i, t in enumerate(time):
-        it, bt = find_ind_t(ts, t)
-        delta_t = t - bt
-        if it < len(ts) - 1:
-            Delta_t = ts[it + 1] - ts[it]
-        else:
-            Delta_t = ts[it] - ts[it - 1]
-        rt = delta_t / Delta_t
-        its[i] = it
-        rts[i] = rt
-        dts[i] = Delta_t
-        bts[i] = bt
-    return its, rts, dts, bts
+    return find_rel(time, ts)
 
 
-@compileable
-def _read_h_with_face(some_x, some_y, some_dx, some_dy, CS, SN, faces, iys, ixs):
-    """Read the grid coords when there is a face dimension to it."""
-    n = len(ixs)
-
-    bx = np.ones_like(ixs) * 0.0
-    by = np.ones_like(ixs) * 0.0
-    for i in range(n):
-        bx[i] = some_x[faces[i], iys[i], ixs[i]]
-        by[i] = some_y[faces[i], iys[i], ixs[i]]
+def _read_h(some_x, some_y, some_dx, some_dy, CS, SN, ind):
+    """Read the grid coords at given index.
 
-    if CS is not None and SN is not None:
-        cs = np.ones_like(ixs) * 0.0
-        sn = np.ones_like(ixs) * 0.0
-        for i in range(n):
-            cs[i] = CS[faces[i], iys[i], ixs[i]]
-            sn[i] = SN[faces[i], iys[i], ixs[i]]
-    else:
-        cs = None
-        sn = None
-
-    if some_dx is not None and some_dy is not None:
-        dx = np.ones_like(ixs) * 0.0
-        dy = np.ones_like(ixs) * 0.0
-        for i in range(n):
-            dx[i] = some_dx[faces[i], iys[i], ixs[i]]
-            dy[i] = some_dy[faces[i], iys[i], ixs[i]]
-    else:
-        dx = None
-        dy = None
-
-    return cs, sn, dx, dy, bx, by
-
-
-@compileable
-def _read_h_without_face(some_x, some_y, some_dx, some_dy, CS, SN, iys, ixs):
-    """Read _read_h_with_face for more info."""
-    # TODO ADD test if those are Nones.
-    n = len(ixs)
+    Parameters
+    ----------
+    some_x: numpy.ndarray
+        array of longitude, could be XC or XG
+    some_y: numpy.ndarray
+        array of latitude, could be YC or YG
+    some_dx: numpy.ndarray or None
+        array of distances between grid in the longitudinal direction.
+    some_dy: numpy.ndarray or None
+        array of distances between grid in the latitudinal direction.
+    CS: numpy.ndarray or None
+        array of the cosine of the angle between grid and meridian.
+    SN: numpy.ndarray or None
+        array of the sine of the angle between grid and meridian.
+    ind: tuple
+        indexes to read the grid data from.
+    """
+    bx = some_x[ind]
+    by = some_y[ind]
     if some_dx is not None and some_dy is not None:
-        dx = np.ones_like(ixs) * 0.0
-        dy = np.ones_like(ixs) * 0.0
-        for i in range(n):
-            dx[i] = some_dx[iys[i], ixs[i]]
-            dy[i] = some_dy[iys[i], ixs[i]]
+        dx = some_dx[ind]
+        dy = some_dy[ind]
     else:
         dx = None
         dy = None
 
     if CS is not None and SN is not None:
-        cs = np.ones_like(ixs) * 0.0
-        sn = np.ones_like(ixs) * 0.0
-        for i in range(n):
-            cs[i] = CS[iys[i], ixs[i]]
-            sn[i] = SN[iys[i], ixs[i]]
+        cs = CS[ind]
+        sn = SN[ind]
     else:
         cs = None
         sn = None
-
-    bx = np.ones_like(ixs) * 0.0
-    by = np.ones_like(ixs) * 0.0
-    for i in range(n):
-        bx[i] = some_x[iys[i], ixs[i]]
-        by[i] = some_y[iys[i], ixs[i]]
-
     return cs, sn, dx, dy, bx, by
 
 
-@compileable
-def find_rx_ry_naive(x, y, bx, by, cs, sn, dx, dy):
-    """Find the non-dimensional coords using the local cartesian scheme."""
-    dlon = to_180(x - bx)
-    dlat = to_180(y - by)
-    rx = (dlon * np.cos(by * np.pi / 180) * cs + dlat * sn) * deg2m / dx
-    ry = (dlat * cs - dlon * sn * np.cos(by * np.pi / 180)) * deg2m / dy
-    return rx, ry
-
-
-def find_rel_h_naive(Xs, Ys, some_x, some_y, some_dx, some_dy, CS, SN, tree):
-    """Find the rel-coords in the horizontal.
-
-    very similar to find_rel_time/v
-    rx,ry,dx,dy are defined the same way
-    for example
-    rx = "how much to the right of the node"/"size of the cell in left-right direction"
-    dx = "size of the cell in left-right direction".
-
-    cs,sn is just the cos and sin of the grid orientation.
-    It will come in handy when we transfer vectors.
-    """
-    if NoneIn([Xs, Ys, some_x, some_y, some_dx, some_dy, CS, SN, tree]):
-        raise ValueError("Some of the required variables are missing")
-    h_shape = some_x.shape
-    faces, iys, ixs = find_ind_h(Xs, Ys, tree, h_shape)
-    if faces is not None:
-        cs, sn, dx, dy, bx, by = _read_h_with_face(
-            some_x, some_y, some_dx, some_dy, CS, SN, faces, iys, ixs
-        )
-    else:
-        cs, sn, dx, dy, bx, by = _read_h_without_face(
-            some_x, some_y, some_dx, some_dy, CS, SN, iys, ixs
-        )
-    rx, ry = find_rx_ry_naive(Xs, Ys, bx, by, cs, sn, dx, dy)
-    return faces, iys, ixs, rx, ry, cs, sn, dx, dy, bx, by
-
-
-def find_rel_h_rectilinear(x, y, lon, lat):
-    """Find the rel-coords using the rectilinear scheme."""
-    ratio = 6371e3 * np.pi / 180
-    ix, rx, dx, bx = find_rel_periodic(x, lon, 360.0)
-    iy, ry, dy, by = find_rel_periodic(y, lat, 360.0)
-    dx = np.cos(y * np.pi / 180) * ratio * dx
-    dy = ratio * dy
-    face = None
-    cs = np.ones_like(x)
-    sn = np.zeros_like(x)
-    return face, iy, ix, rx, ry, cs, sn, dx, dy, bx, by
-
-
-def find_rel_h_oceanparcel(
-    x, y, some_x, some_y, some_dx, some_dy, CS, SN, XG, YG, tree, tp
-):
-    """Find the rel-coords using the rectilinear scheme."""
-    if NoneIn([x, y, some_x, some_y, XG, YG, tree]):
-        raise ValueError("Some of the required variables are missing")
-    h_shape = some_x.shape
-    faces, iys, ixs = find_ind_h(x, y, tree, h_shape)
-    if faces is not None:
-        cs, sn, dx, dy, bx, by = _read_h_with_face(
-            some_x, some_y, some_dx, some_dy, CS, SN, faces, iys, ixs
-        )
-        px, py = find_px_py(XG, YG, tp, faces, iys, ixs)
-    else:
-        cs, sn, dx, dy, bx, by = _read_h_without_face(
-            some_x, some_y, some_dx, some_dy, CS, SN, iys, ixs
-        )
-        px, py = find_px_py(XG, YG, tp, iys, ixs)
-    rx, ry = find_rx_ry_oceanparcel(x, y, px, py)
-    return faces, iys, ixs, rx, ry, cs, sn, dx, dy, bx, by
-
-
-def find_px_py(XG, YG, tp, *ind, gridoffset=-1):
+def find_px_py(XG, YG, tp, ind, cuvwg="G"):
     """Find the nearest 4 corner points.
 
     This is used in oceanparcel interpolation scheme.
     """
     N = len(ind[0])
-    ind1 = tuple(i for i in tp.ind_tend_vec(ind, np.ones(N) * 3, gridoffset=gridoffset))
-    ind2 = tuple(i for i in tp.ind_tend_vec(ind1, np.zeros(N), gridoffset=gridoffset))
-    ind3 = tuple(i for i in tp.ind_tend_vec(ind, np.zeros(N), gridoffset=gridoffset))
+    ind1 = tuple(i for i in tp.ind_tend_vec(ind, np.ones(N) * 3, cuvwg=cuvwg))
+    ind2 = tuple(i for i in tp.ind_tend_vec(ind1, np.zeros(N), cuvwg=cuvwg))
+    ind3 = tuple(i for i in tp.ind_tend_vec(ind, np.zeros(N), cuvwg=cuvwg))
 
     x0 = XG[ind]
     x1 = XG[ind1]
     x2 = XG[ind2]
     x3 = XG[ind3]
 
     y0 = YG[ind]
@@ -619,14 +501,24 @@
     px = np.vstack([x0, x1, x2, x3]).astype("float64")
     py = np.vstack([y0, y1, y2, y3]).astype("float64")
 
     return px, py
 
 
 @compileable
+def find_rx_ry_naive(x, y, bx, by, cs, sn, dx, dy):
+    """Find the non-dimensional coords using the local cartesian scheme."""
+    dlon = to_180(x - bx)
+    dlat = to_180(y - by)
+    rx = (dlon * np.cos(by * np.pi / 180) * cs + dlat * sn) * deg2m / dx
+    ry = (dlat * cs - dlon * sn * np.cos(by * np.pi / 180)) * deg2m / dy
+    return rx, ry
+
+
+@compileable
 def find_rx_ry_oceanparcel(x, y, px, py):
     """Find the non-dimensional horizontal distance.
 
     This is done using the oceanparcel scheme.
     """
     rx = np.ones_like(x) * 0.0
     ry = np.ones_like(y) * 0.0
@@ -650,32 +542,83 @@
     bb = a[3] * b[0] - a[0] * b[3] + a[1] * b[2] - a[2] * b[1] + x * b[3] - y * a[3]
     cc = a[1] * b[0] - a[0] * b[1] + x * b[1] - y * a[1]
 
     det2 = bb * bb - 4 * aa * cc
 
     order1 = np.abs(aa) < 1e-12
     order2 = np.logical_and(~order1, det2 >= 0)
-    #     nans   = np.logical_and(~order1,det2< 0)
-
-    #     ry[order1] = -(cc/bb)[order1]
     ry = -(cc / bb)  # if it is supposed to be nan, just try linear solve.
     ry[order2] = ((-bb + np.sqrt(det2)) / (2 * aa))[order2]
-    #     ry[nans  ] = np.nan
 
     rot_rectilinear = np.abs(a[1] + a[3] * ry) < 1e-12
     rx[rot_rectilinear] = (
         (y - py[0]) / (py[1] - py[0]) + (y - py[3]) / (py[2] - py[3])
     )[rot_rectilinear] * 0.5
     rx[~rot_rectilinear] = ((x - a[0] - a[2] * ry) / (a[1] + a[3] * ry))[
         ~rot_rectilinear
     ]
 
     return rx - 1 / 2, ry - 1 / 2
 
 
+def find_rel_h_naive(lon, lat, some_x, some_y, some_dx, some_dy, CS, SN, tree):
+    """Find the rel-coords in the horizontal.
+
+    very similar to find_rel_time/v
+    rx,ry,dx,dy are defined the same way
+    for example
+    rx = "how much to the right of the node"/"size of the cell in left-right direction"
+    dx = "size of the cell in left-right direction".
+
+    cs,sn is just the cos and sin of the grid orientation.
+    It will come in handy when we transfer vectors.
+    """
+    if NoneIn([lon, lat, some_x, some_y, some_dx, some_dy, CS, SN, tree]):
+        raise ValueError("Some of the required variables are missing")
+    h_shape = some_x.shape
+    face, iy, ix = find_ind_h(lon, lat, tree, h_shape)
+    if face is not None:
+        ind = (face, iy, ix)
+    else:
+        ind = (iy, ix)
+    cs, sn, dx, dy, bx, by = _read_h(some_x, some_y, some_dx, some_dy, CS, SN, ind)
+    rx, ry = find_rx_ry_naive(lon, lat, bx, by, cs, sn, dx, dy)
+    return face, iy, ix, rx, ry, cs, sn, dx, dy, bx, by
+
+
+def find_rel_h_rectilinear(x, y, lon, lat):
+    """Find the rel-coords using the rectilinear scheme."""
+    ix, rx, dx, bx = find_rel_periodic(x, lon, 360.0)
+    iy, ry, dy, by = find_rel_periodic(y, lat, 360.0)
+    dx = np.cos(by * np.pi / 180) * deg2m * dx
+    dy = deg2m * dy
+    face = None
+    cs = np.ones_like(x)
+    sn = np.zeros_like(x)
+    return face, iy, ix, rx, ry, cs, sn, dx, dy, bx, by
+
+
+def find_rel_h_oceanparcel(
+    x, y, some_x, some_y, some_dx, some_dy, CS, SN, XG, YG, tree, tp
+):
+    """Find the rel-coords using the rectilinear scheme."""
+    if NoneIn([x, y, some_x, some_y, XG, YG, tree]):
+        raise ValueError("Some of the required variables are missing")
+    h_shape = some_x.shape
+    face, iy, ix = find_ind_h(x, y, tree, h_shape)
+    if face is not None:
+        ind = (face, iy, ix)
+    else:
+        ind = (iy, ix)
+    cs, sn, dx, dy, bx, by = _read_h(some_x, some_y, some_dx, some_dy, CS, SN, ind)
+    px, py = find_px_py(XG, YG, tp, ind)
+    rx, ry = find_rx_ry_oceanparcel(x, y, px, py)
+    return face, iy, ix, rx, ry, cs, sn, dx, dy, bx, by
+
+
 def weight_f_node(rx, ry):
     """Assign weights to four corners.
 
     assign weight based on the non-dimensional
     coords to the four corner points.
     """
     return np.vstack(
@@ -706,46 +649,53 @@
     sin_AB = np.sqrt(1 - cos_AB**2)
     # spherical law of sine on triangle AOB
     SN = np.sin(BO) * np.sin(dphi) / sin_AB
     CS = np.sign(thetaB - thetaA) * np.sqrt(1 - SN**2)
     return CS, SN
 
 
-def missing_cs_sn(ds):
+def missing_cs_sn(ds, return_xr=False):
     """Fill in the CS,SN of a dataset."""
     xc = np.deg2rad(np.array(ds.XC))
     yc = np.deg2rad(np.array(ds.YC))
     cs = np.zeros_like(xc)
     sn = np.zeros_like(xc)
     cs[0], sn[0] = find_cs_sn(yc[0], xc[0], yc[1], xc[1])
     cs[-1], sn[-1] = find_cs_sn(yc[-2], xc[-2], yc[-1], xc[-1])
     cs[1:-1], sn[1:-1] = find_cs_sn(yc[:-2], xc[:-2], yc[2:], xc[2:])
-    ds["CS"] = ds["XC"]
-    ds["CS"].values = cs
+    if return_xr:
+        ds["CS"] = ds["XC"]
+        ds["CS"].values = cs
 
-    ds["SN"] = ds["XC"]
-    ds["SN"].values = sn
+        ds["SN"] = ds["XC"]
+        ds["SN"].values = sn
+
+        return ds
+    else:
+        return cs, sn
 
 
 def convert_time(time):
     """Convert time into seconds after 1970-01-01.
 
     time needs to be a string or a np.datetime64 object.
     """
     t0 = np.datetime64("1970-01-01")
     one_sec = np.timedelta64(1, "s")
     if isinstance(time, str):
         dt = np.datetime64(time) - t0
         return dt / one_sec
     elif isinstance(time, np.datetime64):
         return (time - t0) / one_sec
+    else:
+        raise ValueError(f"Unsupported time format {type(time)}")
 
 
 def easy_3d_cube(lon, lat, dep, tim, print_total_number=False):
-    """Create 4D coords for initializing position/particle."""
+    """Create 4D coords for initializing Position/Particle."""
     east, west, Nlon = lon
     south, north, Nlat = lat
     shallow, deep, Ndep = dep
     t_in_sec = convert_time(tim)
 
     x = np.linspace(east, west, Nlon)
     y = np.linspace(south, north, Nlat)
@@ -757,9 +707,9 @@
     y, z = np.meshgrid(y, levels)
     x = x.ravel()
     y = y.ravel()
     z = z.ravel()
 
     t = np.ones_like(x) * t_in_sec
     if print_total_number:
-        print(f"A total {len(x)} positions defined.")
+        print(f"A total of {len(x)} positions are defined.")
     return x, y, z, t
```

### Comparing `seaduck-0.1.2/seaduck.egg-info/PKG-INFO` & `seaduck-0.1.3/seaduck.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaduck
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package that interpolates data from ocean dataset from both Eulerian and Lagrangian perspective. 
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -220,25 +220,30 @@
 # seaduck
 
 A python package that interpolates data from ocean dataset from both Eulerian and Lagrangian perspective.
 
 ## Quick Start
 
 ```python
->>> import seaduck
+>>> import seaduck as sd
 
 ```
 
+## Documentation
+
+Checkout this half-way-through documentation:
+https://macekuailv.github.io/seaduck/
+
 ## Workflow for developers/contributors
 
-For best experience create a new conda environment (e.g. seaduck):
+For best experience create a new conda environment (e.g. bubblebath):
 
 ```
-conda create -n seaduck
-conda activate seaduck
+conda create -n bubblebath
+conda activate bubblebath
 ```
 
 Before pushing to GitHub, run the following commands:
 
 1. Update conda environment: `make conda-env-update`
 1. Install this package: `pip install -e .`
 1. Run quality assurance checks: `make qa`
```

### Comparing `seaduck-0.1.2/tests/test_get_masks.py` & `seaduck-0.1.3/tests/test_get_masks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numpy as np
 import pytest
+import xarray as xr
 
 import seaduck as sd
 import seaduck.get_masks as gm
-import seaduck.topology as topology
 from seaduck import utils
 
 
 # TODO: have a dataset that actually has maskC and is also not ECCO in the test datasets
 @pytest.fixture
 def masks():
     ds = utils.get_dataset("ecco")
-    return gm.get_masks(sd.OceData(ds), topology(ds))
+    return gm.get_mask_arrays(sd.OceData(ds))
 
 
 def test_maskC_contains_others(masks):
     # if one of the u,v,w is not defined, this cell must be a solid
     # or in other words, the maskC land is contained in other lands.
     maskC, maskU, maskV, maskW = masks
     assert np.logical_or(np.logical_not(maskC), maskU).all()
@@ -26,19 +26,29 @@
 def test_not_the_same(masks):
     maskC, maskU, maskV, maskW = masks
     assert not np.allclose(maskC, maskU)
     assert not np.allclose(maskC, maskV)
     assert not np.allclose(maskC, maskW)
 
 
+@pytest.mark.parametrize("od", ["ecco"], indirect=True)
+def test_repeated_get_mask_array(od):
+    a_mask = gm.get_masked(od, (1, 1, 1), cuvwg="U")
+    assert a_mask[0] == 1
+    od._ds = od._ds.drop_vars(["maskU"])
+    _ = gm.get_mask_arrays(od)
+    assert "maskV" in od._ds.keys()
+    assert isinstance(od["maskU"], xr.DataArray)
+
+
 @pytest.mark.parametrize("od", ["rect", "curv"], indirect=True)
 def test_without_maskC(od):
-    with pytest.warns(Warning):
-        _, maskU, *_ = gm.get_masks(od, od.tp)
+    with pytest.warns(UserWarning):
+        _, maskU, *_ = gm.get_mask_arrays(od)
     assert maskU.all()
 
 
 @pytest.mark.parametrize("od", ["rect", "curv"], indirect=True)
 def test_get_masked_without_maskC(od):
-    with pytest.warns(Warning):
+    with pytest.warns(UserWarning):
         hello = gm.get_masked(od, (1, 1))
     assert hello == 1
```

### Comparing `seaduck-0.1.2/tests/test_topology.py` & `seaduck-0.1.3/tests/test_topology.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 import numpy as np
 import pytest
 
-from seaduck.topology import llc_get_uv_mask_from_face, llc_mutual_direction, topology
+from seaduck.topology import Topology, llc_get_uv_mask_from_face, llc_mutual_direction
+
+try:
+    import numba
+
+    print(numba)
+    # just to avoid the line got deleted by pre-commit
+    HAS_NUMBA = True
+except ImportError:
+    HAS_NUMBA = False
 
 
 @pytest.mark.parametrize("face", [1, 2, 4, 5, 6, 7, 8, 10, 11])
 @pytest.mark.parametrize("edge", [0, 1, 2, 3])
 @pytest.mark.parametrize("tp", ["ecco"], indirect=True)
 def test_get_the_neighbor_face(tp, face, edge):
     nf, ne = tp.get_the_other_edge(face, edge)
@@ -27,15 +36,15 @@
     [
         ("get_the_other_edge", (0, 0)),
         ("mutual_direction", (0, 1)),
     ],
 )
 @pytest.mark.parametrize("ds", ["ecco"], indirect=True)
 def test_not_applicable(ds, typ, func, args, error):
-    tpp = topology(ds, typ)
+    tpp = Topology(ds, typ)
     with pytest.raises(error):
         getattr(tpp, func)(*args)
 
 
 @pytest.mark.parametrize("face,edge", [(0, 1), (3, 1), (9, 3), (12, 3)])
 @pytest.mark.parametrize("tp", ["ecco"], indirect=True)
 def test_antarctica_error(tp, face, edge):
@@ -67,15 +76,16 @@
     res = tp.ind_tend(ind, tend)
     assert res == result
 
 
 @pytest.mark.parametrize("tend", [0, 1, 2, 3])
 @pytest.mark.parametrize("tp", ["aviso", "rect"], indirect=True)
 def test_boxish_ind_tend(tp, tend):
-    tp.ind_tend((0, 0), tend)
+    ind = tp.ind_tend((0, 0), tend)
+    assert len(ind) == 2
 
 
 @pytest.mark.parametrize("tend", [0, 3])
 @pytest.mark.parametrize("tp", ["aviso", "rect"], indirect=True)
 def test_boundary_case(tp, tend):
     out = tp.ind_tend((tp.ixmax, tp.iymax), tend)
     if tp.typ == "box" or tend == 0:
@@ -106,70 +116,71 @@
         assert not np.allclose(ans, mundane)
 
 
 @pytest.mark.parametrize("ds", ["rect"], indirect=True)
 def test_unable_to_cereate(ds):
     temp = ds.drop_vars("XC")
     with pytest.raises(KeyError):
-        topology(temp)
+        Topology(temp)
 
 
 @pytest.mark.parametrize("ds", ["aviso"], indirect=True)
 def test_create_without_time(ds):
     temp = ds.drop_vars("time")
-    topology(temp)
+    tp = Topology(temp)
+    assert tp.itmax == 0
 
 
 @pytest.mark.parametrize(
     "func,args,kwargs,error",
     [
-        ("ind_tend", ((1, 45, 45), 0), {"cuvg": "G"}, NotImplementedError),
-        ("ind_tend", ((1, 45, 45), 0), {"cuvg": "other"}, ValueError),
+        ("ind_tend", ((1, 45, 45), 0), {"cuvwg": "other"}, ValueError),
         ("ind_moves", ((1, 45, 45), ["left", "left"]), {}, ValueError),
     ],
 )
 @pytest.mark.parametrize("tp", ["ecco"], indirect=True)
 def test_other_errors(tp, func, args, kwargs, error):
     with pytest.raises(error):
         getattr(tp, func)(*args, **kwargs)
 
 
 @pytest.mark.parametrize("tp", ["ecco"], indirect=True)
 def test_ind_moves_with1illegal(tp):
-    tp.ind_moves((1, -1, 89), [0, 0])
+    res = tp.ind_moves((1, -1, 89), [0, 0])
+    assert res == (-1, -1, -1)
 
 
 @pytest.mark.parametrize(
     "ind,tend,ans",
     [
         ((1, 45, 45), 0, (1, 46, 45)),
         ((1, 45, 45), 2, (1, 45, 44)),
         ((1, 0, 0), 2, (12, 89, 0)),
         ((1, 0, 0), 1, (0, 89, 0)),
         ((4, 45, 89), 3, (8, 0, 45)),
     ],
 )
 @pytest.mark.parametrize("tp", ["ecco"], indirect=True)
 def test_ind_tend_v(tp, ind, tend, ans):
-    res = tp.ind_tend(ind, tend, cuvg="V")
+    res = tp.ind_tend(ind, tend, cuvwg="V")
     assert res == ans
 
 
 @pytest.mark.parametrize(
     "ans,tend,ind",
     [
         ((1, 45, 45), 1, (1, 46, 45)),
         ((1, 45, 44), 2, (1, 45, 45)),
         ((1, 0, 0), 0, (12, 89, 0)),
         ((4, 45, 89), 1, (8, 0, 45)),
     ],
 )
 @pytest.mark.parametrize("tp", ["ecco"], indirect=True)
 def test_ind_tend_u(tp, ind, tend, ans):
-    res = tp.ind_tend(ind, tend, cuvg="U")
+    res = tp.ind_tend(ind, tend, cuvwg="U")
     assert res == ans
 
 
 @pytest.mark.parametrize("tp", ["ecco"], indirect=True)
 def test_wall_between(tp):
     # it is a bit hard to think about an example
     # that uses this case from higher level.
@@ -195,78 +206,33 @@
 )
 def test_transitive_mututal_direction(face, nface, rot):
     e1, e2 = llc_mutual_direction(face, nface, transitive=True)
     isrot = (e1 // 2 + e2 // 2) % 2
     assert isrot == rot
 
 
+@pytest.mark.skipif(
+    HAS_NUMBA, reason="Weird numba behavior that needs to be revisited."
+)
 @pytest.mark.parametrize("transitive,face, nface", [(True, 0, 7), (False, 4, 9)])
 def test_mutual_face_error(transitive, face, nface):
     with pytest.raises(ValueError):
         llc_mutual_direction(face, nface, transitive=transitive)
 
 
 def test_uv_mask():
     faces = np.array([1, 1, 1, 1, 4])
-    llc_get_uv_mask_from_face(faces)
+    uu, uv, vu, vv = llc_get_uv_mask_from_face(faces)
+    assert (uu == 1).all()
 
 
 @pytest.mark.parametrize("tp", ["rect"], indirect=True)
 def test_uv_mask_error(tp):
     faces = np.array([1, 1, 1, 1, 4])
     with pytest.raises(Exception):
         tp.get_uv_mask_from_face(faces)
 
 
 @pytest.mark.parametrize("tp", ["ecco"], indirect=True)
 def test_wall_between_itself(tp):
     with pytest.raises(IndexError):
         tp._find_wall_between((1, 14, 14), (1, 14, 14))
-
-
-# def test_fatten_ind_h_ecco():
-#     faces = np.array([0, 0])
-#     iys = np.array([45, 46])
-#     ixs = np.array([45, 46])
-#     tp = topology(ecco)
-#     nface, niy, nix = kw.fatten_ind_h(faces, iys, ixs, tp)
-#     assert nface.dtype == "int"
-#     assert nface.shape == (2, 9)
-
-
-# @pytest.mark.parametrize("od", [rect, curv])
-# def test_fatten_ind_h_other(od):
-#     faces = None
-#     iys = np.array([5, 46])
-#     ixs = np.array([5, 6])
-#     tp = topology(od)
-#     nface, niy, nix = kw.fatten_ind_h(faces, iys, ixs, tp)
-#     assert nface is None
-#     assert nix.dtype == "int"
-#     assert niy.shape == (2, 9)
-
-
-# def test_fatten_ind_3d_ecco():
-#     izs = np.array([9, 10])
-#     faces = np.array([0, 0])
-#     iys = np.array([45, 46])
-#     ixs = np.array([45, 46])
-#     tp = topology(ecco)
-#     niz, nface, niy, nix = kw.fatten_ind_3d(izs, faces, iys, ixs, tp)
-#     assert niz.dtype == "int"
-#     assert niz.shape == (2, 18)
-
-
-# @pytest.mark.parametrize("od", [rect, curv])
-# def test_fatten_ind_3d_other(od):
-#     izs = np.array([9, 10])
-#     faces = None
-#     iys = np.array([5, 46])
-#     ixs = np.array([5, 46])
-#     tp = topology(od)
-#     niz, nface, niy, nix = kw.fatten_ind_3d(izs, faces, iys, ixs, tp)
-#     assert niz.dtype == "int"
-#     assert niz.shape == (2, 18)
-
-
-# if __name__ == '__main__':
-#     test_fatten_ind_3d()
```

### Comparing `seaduck-0.1.2/tests/test_weight.py` & `seaduck-0.1.3/tests/test_weight.py`

 * *Files 21% similar despite different names*

```diff
@@ -86,25 +86,40 @@
 def test_interp_func(kernel, rx, ry):
     func = kw.get_func(kernel)
     weight = func(rx, ry)
     assert weight.shape == (1, len(kernel))
     np.testing.assert_allclose(np.sum(weight), 1)
 
 
-@pytest.mark.parametrize("ktype", ["dx", "dy"])
+@pytest.mark.parametrize(
+    "rx,ry",
+    [
+        (np.array([0]), np.array([0])),
+        (np.array([0.5]), np.array([0.08])),
+    ],
+)
+@pytest.mark.parametrize("kernel_type", ["dx", "dy"])
 @pytest.mark.parametrize("horder", [0, 1])
-def test_create_different_square(ktype, horder):
+def test_create_different_square(kernel_type, horder, rx, ry):
     k = np.array([[0, 0], [0, 1], [1, 0], [1, 1]])
-    kw.get_func(k, hkernel=ktype, h_order=horder)
+    func = kw.get_func(k, hkernel=kernel_type, h_order=horder)
+    weight = func(rx, ry)
+    assert weight.shape == (1, len(k))
+    if horder == 0:
+        np.testing.assert_allclose(np.sum(weight), 1)
+    else:
+        np.testing.assert_allclose(np.sum(weight), 0, atol=1e-14)
 
 
 @pytest.mark.parametrize("hkernel", ["dx", "dy"])
-def test_auto_doll(hkernel):
+def test_auto_inheritance(hkernel):
     k = np.array([[0, 0], [0, 1], [1, 0], [1, 1]])
-    kw.auto_doll(k, hkernel=hkernel)
+    inheritance = kw.auto_inheritance(k, hkernel=hkernel)
+    assert len(inheritance) > 1
+    assert isinstance(inheritance[0], list)
 
 
 @pytest.mark.parametrize(
     "rx,ry", [(np.array([0]), np.array([0])), (np.array([0.5]), np.array([0.08]))]
 )
 @pytest.mark.parametrize(
     "kernel",
@@ -118,15 +133,15 @@
     ],
 )
 @pytest.mark.parametrize("order", [1, 2])
 def test_dx(kernel, rx, ry, order):
     func = kw.get_func(kernel, hkernel="dx", h_order=order)
     weight = func(rx, ry)
     assert weight.shape == (1, len(kernel))
-    assert np.allclose(0, np.sum(weight))
+    assert np.allclose(0, np.sum(weight), atol=1e-14)
 
 
 @pytest.mark.parametrize(
     "rx,ry", [(np.array([0]), np.array([0])), (np.array([0.5]), np.array([0.08]))]
 )
 @pytest.mark.parametrize(
     "kernel",
@@ -139,18 +154,18 @@
     ],
 )
 @pytest.mark.parametrize("order", [1, 2])
 def test_dy(kernel, rx, ry, order):
     func = kw.get_func(kernel, hkernel="dy", h_order=order)
     weight = func(rx, ry)
     assert weight.shape == (1, len(kernel))
-    assert np.allclose(0, np.sum(weight))
+    assert np.allclose(0, np.sum(weight), atol=1e-14)
 
 
-@pytest.mark.parametrize("ktype", ["dx", "dy"])
+@pytest.mark.parametrize("kernel_type", ["dx", "dy"])
 @pytest.mark.parametrize(
     "kernel,order",
     [
         (
             np.array(
                 [
                     [0, 0],
@@ -170,34 +185,39 @@
             np.array([[0, 0], [0, 1], [0, -1], [-1, 0], [1, 0]]),
             3,
         ),
         (np.array([[0, 0]]), 1),
         (np.array([[0, 0], [0, 1], [1, 0], [1, 1]]), 2),
     ],
 )
-def test_order_too_high_error(kernel, order, ktype):
+def test_order_too_high_error(kernel, order, kernel_type):
     with pytest.raises(Exception):
-        kw.kernel_weight(kernel, ktype=ktype, order=order)
+        kw.kernel_weight(kernel, kernel_type=kernel_type, order=order)
 
 
 def test_plot_kernel():
     pytest.importorskip("matplotlib.pyplot")
     kw.show_kernels()
+    # no way to assert here
 
 
 def test_dt_and_bottom_scheme(aknw):
-    aknw.get_weight(np.array([0.618]), np.array([0.0618]))
+    weight = aknw.get_weight(np.array([0.618]), np.array([0.0618]))
+    assert weight.shape[0] == 1
+    assert np.allclose(0, np.sum(weight))
 
 
 @pytest.mark.parametrize("which", ["dx", "dy"])
 def test_maxorder_dxdy_square(which):
     kkk = np.array(
         [[0, 0], [0, 1], [1, 0], [1, 1], [1, 2], [0, 2], [2, 2], [2, 0], [2, 1]]
     )
     xorder = 0
     yorder = 0
     if which == "dx":
         xorder = 2
     else:
         yorder = 2
     func = kw.kernel_weight_s(kkk, xorder, yorder)
-    func(np.array([0.0]), np.array([0.0]))
+    weight = func(np.array([0.0]), np.array([0.0]))
+    assert weight.shape == (1, len(kkk))
+    assert np.allclose(0, np.sum(weight), atol=1e-14)
```


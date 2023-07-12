# Comparing `tmp/hickleable-0.2.2.tar.gz` & `tmp/hickleable-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hickleable-0.2.2.tar", last modified: Fri Jul  7 23:37:21 2023, max compression
+gzip compressed data, was "hickleable-0.2.3.tar", last modified: Wed Jul 12 06:03:59 2023, max compression
```

## Comparing `hickleable-0.2.2.tar` & `hickleable-0.2.3.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.887752 hickleable-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 23:37:12.000000 hickleable-0.2.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-07 23:37:12.000000 hickleable-0.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.879752 hickleable-0.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/labels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.879752 hickleable-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/workflows/auto-merge-deps.yml
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/workflows/check-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/workflows/deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/workflows/release-draft.yml
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-07 23:37:12.000000 hickleable-0.2.2/.github/workflows/testsuite.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-07 23:37:12.000000 hickleable-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-07 23:37:12.000000 hickleable-0.2.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-07 23:37:12.000000 hickleable-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-07 23:37:12.000000 hickleable-0.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 23:37:12.000000 hickleable-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-07 23:37:21.887752 hickleable-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-07 23:37:12.000000 hickleable-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.883751 hickleable-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.883751 hickleable-0.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.883751 hickleable-0.2.2/docs/faqs/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/faqs/misc.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.883751 hickleable-0.2.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.883751 hickleable-0.2.2/docs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-07 23:37:12.000000 hickleable-0.2.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 23:37:12.000000 hickleable-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-07 23:37:21.887752 hickleable-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 23:37:12.000000 hickleable-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.871751 hickleable-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.883751 hickleable-0.2.2/src/hickleable/
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-07-07 23:37:12.000000 hickleable-0.2.2/src/hickleable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.887752 hickleable-0.2.2/src/hickleable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-07 23:37:21.000000 hickleable-0.2.2/src/hickleable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-07 23:37:21.000000 hickleable-0.2.2/src/hickleable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:37:21.000000 hickleable-0.2.2/src/hickleable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:37:21.000000 hickleable-0.2.2/src/hickleable.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-07 23:37:21.000000 hickleable-0.2.2/src/hickleable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-07 23:37:21.000000 hickleable-0.2.2/src/hickleable.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:37:21.887752 hickleable-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-07 23:37:12.000000 hickleable-0.2.2/tests/test_hickleable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 06:03:47.000000 hickleable-0.2.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-12 06:03:47.000000 hickleable-0.2.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.252550 hickleable-0.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.252550 hickleable-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/workflows/auto-merge-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/workflows/check-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/workflows/release-draft.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-12 06:03:47.000000 hickleable-0.2.3/.github/workflows/testsuite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-12 06:03:47.000000 hickleable-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-12 06:03:47.000000 hickleable-0.2.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-12 06:03:47.000000 hickleable-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-12 06:03:47.000000 hickleable-0.2.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 06:03:47.000000 hickleable-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-12 06:03:59.260550 hickleable-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-12 06:03:47.000000 hickleable-0.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/docs/faqs/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/faqs/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 06:03:47.000000 hickleable-0.2.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-12 06:03:47.000000 hickleable-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-12 06:03:59.260550 hickleable-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 06:03:47.000000 hickleable-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.252550 hickleable-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/src/hickleable/
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-12 06:03:47.000000 hickleable-0.2.3/src/hickleable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/src/hickleable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-12 06:03:59.000000 hickleable-0.2.3/src/hickleable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-12 06:03:59.000000 hickleable-0.2.3/src/hickleable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 06:03:59.000000 hickleable-0.2.3/src/hickleable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 06:03:59.000000 hickleable-0.2.3/src/hickleable.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-12 06:03:59.000000 hickleable-0.2.3/src/hickleable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 06:03:59.000000 hickleable-0.2.3/src/hickleable.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 06:03:59.256549 hickleable-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-12 06:03:47.000000 hickleable-0.2.3/tests/test_hickleable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-12 06:03:47.000000 hickleable-0.2.3/tests/test_yaml.py
```

### Comparing `hickleable-0.2.2/.github/labels.yml` & `hickleable-0.2.3/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/.github/release-drafter.yml` & `hickleable-0.2.3/.github/release-drafter.yml`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,14 @@
     title:
       - '/fix/i'
   - label: 'enhancement'
     branch:
       - '/feature.*|add-.+/'
     title:
       - '/feat:.+|feature:.+/i'
-    body:
-      - '/JIRA-[0-9]{1,4}/'
   - label: "removal"
     title:
       - "/remove .*/i"
   - label: "performance"
     title:
       - "/.* performance .*/i"
   - label: "ci"
```

### Comparing `hickleable-0.2.2/.github/workflows/check-build.yml` & `hickleable-0.2.3/.github/workflows/check-build.yml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/.github/workflows/deploy.yaml` & `hickleable-0.2.3/.github/workflows/deploy.yaml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/.github/workflows/testsuite.yaml` & `hickleable-0.2.3/.github/workflows/testsuite.yaml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/.gitignore` & `hickleable-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/.pre-commit-config.yaml` & `hickleable-0.2.3/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -50,11 +50,11 @@
 
 - repo: https://github.com/pre-commit/pygrep-hooks
   rev: v1.10.0
   hooks:
     - id: rst-backticks
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.8.0
+  rev: v3.9.0
   hooks:
   -   id: pyupgrade
       args: [--py38-plus]
```

### Comparing `hickleable-0.2.2/.readthedocs.yml` & `hickleable-0.2.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/LICENSE` & `hickleable-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/PKG-INFO` & `hickleable-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hickleable
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple decorator to make your classes hickle-able
 Home-page: https://github.com/steven-murray/hickleable
 Author: Steven Murray
 License: mit
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `hickleable-0.2.2/README.rst` & `hickleable-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/docs/Makefile` & `hickleable-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/docs/conf.py` & `hickleable-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/docs/index.rst` & `hickleable-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/docs/templates/class.rst` & `hickleable-0.2.3/docs/templates/class.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/docs/templates/module.rst` & `hickleable-0.2.3/docs/templates/module.rst`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/setup.cfg` & `hickleable-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `hickleable-0.2.2/src/hickleable/__init__.py` & `hickleable-0.2.3/src/hickleable/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,16 +165,24 @@
                         if isinstance(value, cached_property)
                     ]
                     for cp in all_cached_properties:
                         getattr(py_obj, cp)
 
                 if hasattr(py_obj, "__gethstate__"):
                     state = py_obj.__gethstate__()
+                    if not isinstance(state, dict):
+                        raise TypeError(
+                            f"__gethstate__ must return a dictionary. Got {state} with type {type(state)} from {type(py_obj)}."
+                        )
                 elif hasattr(py_obj, "__getstate__"):
                     state = py_obj.__getstate__()
+                    if not isinstance(state, dict):
+                        raise TypeError(
+                            f"__getstate__ must return a dictionary. Got {state} with type {type(state)} from {type(py_obj)}."
+                        )
                 elif py_obj.__dict__ is not None:
                     state = py_obj.__dict__
                 elif attrs is not None and attrs.has(py_obj):
                     state = attrs.asdict(py_obj)
                 else:
                     state = {}
 
@@ -232,12 +240,12 @@
     b"PosixPath",
     dump_function=_path_dump_function,
     load_function=_load_path,
 )
 
 if yaml is not None:
     # Register a YAML loader for hickle-dumped files.
-    def _hickle_yaml_loader(path):
-        return hickle.load(path)
+    def _hickle_yaml_loader(loader: yaml.SafeLoader, node):
+        return hickle.load(node.value)
 
     yaml.add_constructor("!hickle", _hickle_yaml_loader, Loader=yaml.FullLoader)
     yaml.add_constructor("!hickle", _hickle_yaml_loader, Loader=yaml.Loader)
```

### Comparing `hickleable-0.2.2/src/hickleable.egg-info/PKG-INFO` & `hickleable-0.2.3/src/hickleable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hickleable
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple decorator to make your classes hickle-able
 Home-page: https://github.com/steven-murray/hickleable
 Author: Steven Murray
 License: mit
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `hickleable-0.2.2/src/hickleable.egg-info/SOURCES.txt` & `hickleable-0.2.3/src/hickleable.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -36,8 +36,9 @@
 src/hickleable/__init__.py
 src/hickleable.egg-info/PKG-INFO
 src/hickleable.egg-info/SOURCES.txt
 src/hickleable.egg-info/dependency_links.txt
 src/hickleable.egg-info/not-zip-safe
 src/hickleable.egg-info/requires.txt
 src/hickleable.egg-info/top_level.txt
-tests/test_hickleable.py
+tests/test_hickleable.py
+tests/test_yaml.py
```

### Comparing `hickleable-0.2.2/tests/test_hickleable.py` & `hickleable-0.2.3/tests/test_hickleable.py`

 * *Files 21% similar despite different names*

```diff
@@ -175,7 +175,33 @@
 
     a = FrozenWithCachedProperty("warnme")
 
     hickle.dump(a, fl)
 
     with pytest.warns(UserWarning, match="warning you!"):
         hickle.load(fl)
+
+
+@hickleable()
+class ClassWithBadGetState:
+    def __getstate__(self):
+        return 1
+
+
+def test_bad_getstate(tmpdir):
+    a = ClassWithBadGetState()
+
+    with pytest.raises(TypeError, match="__getstate__ must return a dictionary"):
+        hickle.dump(a, tmpdir / "test.h5")
+
+
+@hickleable()
+class ClassWithBadGetHState:
+    def __gethstate__(self):
+        return 1
+
+
+def test_bad_gethstate(tmpdir):
+    a = ClassWithBadGetHState()
+
+    with pytest.raises(TypeError, match="__gethstate__ must return a dictionary"):
+        hickle.dump(a, tmpdir / "test.h5")
```


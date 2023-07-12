# Comparing `tmp/jaraco.itertools-6.2.1.tar.gz` & `tmp/jaraco.itertools-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.itertools-6.2.1.tar", last modified: Mon Feb 21 03:01:47 2022, max compression
+gzip compressed data, was "jaraco.itertools-6.4.0.tar", last modified: Wed Jul 12 20:04:11 2023, max compression
```

## Comparing `jaraco.itertools-6.2.1.tar` & `jaraco.itertools-6.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 03:01:47.201205 jaraco.itertools-6.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 03:01:47.197204 jaraco.itertools-6.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 03:01:47.197204 jaraco.itertools-6.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3497 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-02-21 03:01:47.201205 jaraco.itertools-6.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 03:01:47.197204 jaraco.itertools-6.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 03:01:47.197204 jaraco.itertools-6.2.1/jaraco/
--rw-r--r--   0 runner    (1001) docker     (121)    31353 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/jaraco/itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-21 03:01:47.201205 jaraco.itertools-6.2.1/jaraco.itertools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-02-21 03:01:46.000000 jaraco.itertools-6.2.1/jaraco.itertools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-02-21 03:01:47.000000 jaraco.itertools-6.2.1/jaraco.itertools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-21 03:01:46.000000 jaraco.itertools-6.2.1/jaraco.itertools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-02-21 03:01:47.000000 jaraco.itertools-6.2.1/jaraco.itertools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-21 03:01:47.000000 jaraco.itertools-6.2.1/jaraco.itertools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-02-21 03:01:47.201205 jaraco.itertools-6.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-02-21 03:01:24.000000 jaraco.itertools-6.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:04:11.266453 jaraco.itertools-6.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:04:11.262453 jaraco.itertools-6.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:04:11.262453 jaraco.itertools-6.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-12 20:04:11.266453 jaraco.itertools-6.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:04:11.262453 jaraco.itertools-6.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:04:11.262453 jaraco.itertools-6.4.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (123)    32645 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/jaraco/itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:04:11.266453 jaraco.itertools-6.4.0/jaraco.itertools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-12 20:04:11.000000 jaraco.itertools-6.4.0/jaraco.itertools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-12 20:04:11.000000 jaraco.itertools-6.4.0/jaraco.itertools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:04:11.000000 jaraco.itertools-6.4.0/jaraco.itertools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-12 20:04:11.000000 jaraco.itertools-6.4.0/jaraco.itertools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 20:04:11.000000 jaraco.itertools-6.4.0/jaraco.itertools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-12 20:04:11.266453 jaraco.itertools-6.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/tox.ini
```

### Comparing `jaraco.itertools-6.2.1/CHANGES.rst` & `jaraco.itertools-6.4.0/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v6.4.0
+======
+
+Features
+--------
+
+- Added ``summarize``.
+- Require Python 3.8 or later.
+
+
+v6.3.0
+======
+
+Added ``find_subseq``.
+
 v6.2.1
 ======
 
 #15: Fixed broken test in ``ensure_unique``.
 
 v6.2.0
 ======
```

### Comparing `jaraco.itertools-6.2.1/LICENSE` & `jaraco.itertools-6.4.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.itertools-6.2.1/PKG-INFO` & `jaraco.itertools-6.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: jaraco.itertools
-Version: 6.2.1
+Version: 6.4.0
 Summary: jaraco.itertools
 Home-page: https://github.com/jaraco/jaraco.itertools
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.itertools.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.itertools
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.itertools.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.itertools
 
 .. image:: https://github.com/jaraco/jaraco.itertools/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.itertools/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracoitertools/badge/?version=latest
    :target: https://jaracoitertools.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
-
-
```

### Comparing `jaraco.itertools-6.2.1/README.rst` & `jaraco.itertools-6.4.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 .. image:: https://img.shields.io/pypi/v/jaraco.itertools.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.itertools
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.itertools.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.itertools
 
 .. image:: https://github.com/jaraco/jaraco.itertools/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.itertools/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracoitertools/badge/?version=latest
    :target: https://jaracoitertools.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
```

### Comparing `jaraco.itertools-6.2.1/docs/conf.py` & `jaraco.itertools-6.4.0/docs/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,46 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
                 pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
                 with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
-                url='https://www.python.org/dev/peps/pep-{pep_number:0>4}/',
+                url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
             dict(
                 pattern=r"more_itertools (?P<more_itertools_ver>[0-9.]+)",
                 url="https://more-itertools.readthedocs.io/en/latest/versions.html",  # noqa: E501
             ),
         ],
     )
 }
 
-# Be strict about any broken references:
+# Be strict about any broken references
 nitpicky = True
 
 # Include Python intersphinx mapping to prevent failures
 # jaraco/skeleton#51
 extensions += ['sphinx.ext.intersphinx']
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
 }
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
```

### Comparing `jaraco.itertools-6.2.1/jaraco/itertools.py` & `jaraco.itertools-6.4.0/jaraco/itertools.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import collections
 import math
 import warnings
 import functools
 import heapq
 import collections.abc
 import queue
+from typing import Iterable, Any
 
 import inflect
 import more_itertools
 
 
 def make_rows(num_columns, seq):
     """
@@ -1209,7 +1210,49 @@
         value = next(items_)
     except StopIteration:
         return
     yield value
     for item in items_:
         value += item
         yield value
+
+
+def find_subseq(seq: Iterable[Any], cand: Iterable[Any]):
+    """Find cand in seq.
+
+    Args:
+        seq: iterable of items to be searched
+        cand: iterable of items that must match
+
+    Returns:
+        The index where cand can be found in seq or None.
+
+    >>> find_subseq([-1, 0, 1, 2], [1, 2])
+    2
+    >>> find_subseq([-1, 0, 1, 2], [0, 2])
+    >>> find_subseq([-1, 0, 1, 2], [2, 1])
+    >>> find_subseq([-1, 0, 1, 2], [])
+    Traceback (most recent call last):
+    ...
+    ValueError: window size must be at least 1
+    """
+    cand = tuple(cand)
+
+    def check(*window):
+        return window == cand
+
+    match_indexes = more_itertools.locate(seq, check, window_size=len(cand))
+    return next(match_indexes, None)
+
+
+def summarize(items: Iterable, **bin_checks):
+    """
+    >>> is_str = lambda item: isinstance(item, str)
+    >>> is_int = lambda item: isinstance(item, int)
+    >>> summarize(['a', 'b', 20], strings=is_str, ints=is_int)
+    {'strings': 2, 'ints': 1}
+    """
+    counters = {name: itertools.count() for name in bin_checks}
+    for item, check in itertools.product(items, bin_checks):
+        if bin_checks[check](item):
+            next(counters[check])
+    return {name: next(counter) for name, counter in counters.items()}
```

### Comparing `jaraco.itertools-6.2.1/jaraco.itertools.egg-info/PKG-INFO` & `jaraco.itertools-6.4.0/jaraco.itertools.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 Metadata-Version: 2.1
 Name: jaraco.itertools
-Version: 6.2.1
+Version: 6.4.0
 Summary: jaraco.itertools
 Home-page: https://github.com/jaraco/jaraco.itertools
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.itertools.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/jaraco.itertools
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.itertools.svg
-   :target: `PyPI link`_
-
-.. _PyPI link: https://pypi.org/project/jaraco.itertools
 
 .. image:: https://github.com/jaraco/jaraco.itertools/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.itertools/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracoitertools/badge/?version=latest
    :target: https://jaracoitertools.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2022-informational
+.. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
-
-
```

### Comparing `jaraco.itertools-6.2.1/setup.cfg` & `jaraco.itertools-6.4.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	more_itertools>=4.0.0
 	inflect
 
 [options.packages.find]
 exclude = 
 	build*
@@ -27,25 +27,27 @@
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.0.1
+	pytest-enabler >= 2.2
+	pytest-ruff
 docs = 
-	sphinx
-	jaraco.packaging >= 9
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```


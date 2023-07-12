# Comparing `tmp/jaraco.itertools-6.4.0.tar.gz` & `tmp/jaraco.itertools-6.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.itertools-6.4.0.tar", last modified: Wed Jul 12 20:04:11 2023, max compression
+gzip compressed data, was "jaraco.itertools-6.4.1.tar", last modified: Wed Jul 12 20:21:58 2023, max compression
```

## Comparing `jaraco.itertools-6.4.0.tar` & `jaraco.itertools-6.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:04:11.266453 jaraco.itertools-6.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:04:11.262453 jaraco.itertools-6.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:04:11.262453 jaraco.itertools-6.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-12 20:04:11.266453 jaraco.itertools-6.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:04:11.262453 jaraco.itertools-6.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:04:11.262453 jaraco.itertools-6.4.0/jaraco/
--rw-r--r--   0 runner    (1001) docker     (123)    32645 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/jaraco/itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:04:11.266453 jaraco.itertools-6.4.0/jaraco.itertools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-12 20:04:11.000000 jaraco.itertools-6.4.0/jaraco.itertools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-12 20:04:11.000000 jaraco.itertools-6.4.0/jaraco.itertools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:04:11.000000 jaraco.itertools-6.4.0/jaraco.itertools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-12 20:04:11.000000 jaraco.itertools-6.4.0/jaraco.itertools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 20:04:11.000000 jaraco.itertools-6.4.0/jaraco.itertools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-12 20:04:11.266453 jaraco.itertools-6.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-12 20:03:43.000000 jaraco.itertools-6.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:21:58.404817 jaraco.itertools-6.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:21:58.396818 jaraco.itertools-6.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:21:58.400817 jaraco.itertools-6.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-12 20:21:58.404817 jaraco.itertools-6.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:21:58.400817 jaraco.itertools-6.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:21:58.400817 jaraco.itertools-6.4.1/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (123)    32512 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/jaraco/itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:21:58.404817 jaraco.itertools-6.4.1/jaraco.itertools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-12 20:21:58.000000 jaraco.itertools-6.4.1/jaraco.itertools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-12 20:21:58.000000 jaraco.itertools-6.4.1/jaraco.itertools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:21:58.000000 jaraco.itertools-6.4.1/jaraco.itertools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-12 20:21:58.000000 jaraco.itertools-6.4.1/jaraco.itertools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 20:21:58.000000 jaraco.itertools-6.4.1/jaraco.itertools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-12 20:21:58.404817 jaraco.itertools-6.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-12 20:21:30.000000 jaraco.itertools-6.4.1/tox.ini
```

### Comparing `jaraco.itertools-6.4.0/.github/workflows/main.yml` & `jaraco.itertools-6.4.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco.itertools-6.4.0/LICENSE` & `jaraco.itertools-6.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.itertools-6.4.0/NEWS.rst` & `jaraco.itertools-6.4.1/NEWS.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v6.4.1
+======
+
+Bugfixes
+--------
+
+- Remove use of ``OrderedDict`` in ``partition_dict``. (#17)
+
+
 v6.4.0
 ======
 
 Features
 --------
 
 - Added ``summarize``.
```

### Comparing `jaraco.itertools-6.4.0/PKG-INFO` & `jaraco.itertools-6.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.itertools
-Version: 6.4.0
+Version: 6.4.1
 Summary: jaraco.itertools
 Home-page: https://github.com/jaraco/jaraco.itertools
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.itertools-6.4.0/README.rst` & `jaraco.itertools-6.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.itertools-6.4.0/docs/conf.py` & `jaraco.itertools-6.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.itertools-6.4.0/jaraco/itertools.py` & `jaraco.itertools-6.4.1/jaraco/itertools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1124,47 +1124,47 @@
     """
     before, item, after = partition_result
     return (before, item, after) if item else (after, item, before)
 
 
 def partition_dict(items, key):
     """
-    Given an ordered dictionary of items and a key in that dict,
-    return an ordered dict of items before, the keyed item, and
-    an ordered dict of items after.
+    Given a dictionary of items and a key in that dict,
+    return another dict of items before, the keyed item, and
+    the dict of items after.
 
-    >>> od = collections.OrderedDict(zip(range(5), 'abcde'))
+    >>> od = dict(zip(range(5), 'abcde'))
     >>> before, item, after = partition_dict(od, 3)
     >>> before
-    OrderedDict([(0, 'a'), (1, 'b'), (2, 'c')])
+    {0: 'a', 1: 'b', 2: 'c'}
     >>> item
     'd'
     >>> after
-    OrderedDict([(4, 'e')])
+    {4: 'e'}
 
     Like string.partition, if the key is not found in the items,
     the before will contain all items, item will be None, and
     after will be an empty iterable.
 
     >>> before, item, after = partition_dict(od, -1)
     >>> before
-    OrderedDict([(0, 'a'), ..., (4, 'e')])
+    {0: 'a', ..., 4: 'e'}
     >>> item
-    >>> list(after)
-    []
+    >>> after
+    {}
     """
 
     def unmatched(pair):
         test_key, item = pair
         return test_key != key
 
     items_iter = iter(items.items())
     item = items.get(key)
-    left = collections.OrderedDict(itertools.takewhile(unmatched, items_iter))
-    right = collections.OrderedDict(items_iter)
+    left = dict(itertools.takewhile(unmatched, items_iter))
+    right = dict(items_iter)
     return left, item, right
 
 
 def ensure_unique(iterable, key=lambda x: x):
     """
     Wrap an iterable to raise a ValueError if non-unique values are encountered.
```

### Comparing `jaraco.itertools-6.4.0/jaraco.itertools.egg-info/PKG-INFO` & `jaraco.itertools-6.4.1/jaraco.itertools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.itertools
-Version: 6.4.0
+Version: 6.4.1
 Summary: jaraco.itertools
 Home-page: https://github.com/jaraco/jaraco.itertools
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.itertools-6.4.0/pytest.ini` & `jaraco.itertools-6.4.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.itertools-6.4.0/setup.cfg` & `jaraco.itertools-6.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaraco.itertools-6.4.0/tox.ini` & `jaraco.itertools-6.4.1/tox.ini`

 * *Files identical despite different names*


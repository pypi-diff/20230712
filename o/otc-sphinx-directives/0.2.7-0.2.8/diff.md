# Comparing `tmp/otc_sphinx_directives-0.2.7.tar.gz` & `tmp/otc_sphinx_directives-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otc_sphinx_directives-0.2.7.tar", last modified: Fri Jul  7 10:56:17 2023, max compression
+gzip compressed data, was "otc_sphinx_directives-0.2.8.tar", last modified: Wed Jul 12 13:33:18 2023, max compression
```

## Comparing `otc_sphinx_directives-0.2.7.tar` & `otc_sphinx_directives-0.2.8.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.576236 otc_sphinx_directives-0.2.7/
--rw-r--r--   0 root         (0) root         (0)       50 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/.stestr.conf
--rw-r--r--   0 root         (0) root         (0)      229 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     2065 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      744 2023-07-07 10:56:17.576236 otc_sphinx_directives-0.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.574236 otc_sphinx_directives-0.2.7/doc/
--rw-r--r--   0 root         (0) root         (0)      329 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.574236 otc_sphinx_directives-0.2.7/doc/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.574236 otc_sphinx_directives-0.2.7/doc/source/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/_static/.placeholder
--rw-r--r--   0 root         (0) root         (0)      311 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.574236 otc_sphinx_directives-0.2.7/doc/source/examples/
--rw-r--r--   0 root         (0) root         (0)      221 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/examples/directives_docsportal.rst
--rw-r--r--   0 root         (0) root         (0)      966 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/examples/directives_ecs.rst
--rw-r--r--   0 root         (0) root         (0)     1386 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/examples/directives_obs.rst
--rw-r--r--   0 root         (0) root         (0)      423 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/examples/directives_obs_clean.rst
--rw-r--r--   0 root         (0) root         (0)      146 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/examples/index.rst
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/doc/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.575236 otc_sphinx_directives-0.2.7/otc_sphinx_directives/
--rw-r--r--   0 root         (0) root         (0)      108 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2589 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/container_item.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/directive_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/document_navigator.py
--rw-r--r--   0 root         (0) root         (0)     2993 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/navigator.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/otc_sphinx_directives_setup.py
--rw-r--r--   0 root         (0) root         (0)     3582 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/service_card.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/service_group.py
--rw-r--r--   0 root         (0) root         (0)     2960 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/service_navigator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.576236 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.573236 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.576236 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/directive_wrapper/
--rw-r--r--   0 root         (0) root         (0)      791 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py
--rw-r--r--   0 root         (0) root         (0)      250 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/directive_wrapper/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.576236 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/service_card/
--rw-r--r--   0 root         (0) root         (0)      791 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/service_card/conf.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/service_card/index.rst
--rw-r--r--   0 root         (0) root         (0)     2330 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/test_directive_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/test_service_card.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 10:56:17.576236 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1523 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-07 10:56:17.000000 otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      586 2023-07-07 10:56:17.577236 otc_sphinx_directives-0.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      651 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/setup.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1366 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/tox.ini
--rw-r--r--   0 root         (0) root         (0)      245 2023-07-07 10:54:56.000000 otc_sphinx_directives-0.2.7/zuul.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:33:18.294905 otc_sphinx_directives-0.2.8/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/.stestr.conf
+-rw-r--r--   0 root         (0) root         (0)      229 2023-07-12 13:33:18.000000 otc_sphinx_directives-0.2.8/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     2126 2023-07-12 13:33:18.000000 otc_sphinx_directives-0.2.8/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-12 13:33:18.294905 otc_sphinx_directives-0.2.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:33:18.291905 otc_sphinx_directives-0.2.8/doc/
+-rw-r--r--   0 root         (0) root         (0)      394 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/doc/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:33:18.291905 otc_sphinx_directives-0.2.8/doc/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:33:18.291905 otc_sphinx_directives-0.2.8/doc/source/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/doc/source/_static/.placeholder
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/doc/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:33:18.292905 otc_sphinx_directives-0.2.8/doc/source/examples/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/doc/source/examples/directives_docsportal.rst
+-rw-r--r--   0 root         (0) root         (0)      966 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/doc/source/examples/directives_ecs.rst
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/doc/source/examples/directives_ecs_internal.rst
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/doc/source/examples/directives_obs.rst
+-rw-r--r--   0 root         (0) root         (0)      423 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/doc/source/examples/directives_obs_clean.rst
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/doc/source/examples/index.rst
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/doc/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:33:18.293905 otc_sphinx_directives-0.2.8/otc_sphinx_directives/
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/container_item.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/directive_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/document_navigator.py
+-rw-r--r--   0 root         (0) root         (0)     2993 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/navigator.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/otc_sphinx_directives_setup.py
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/service_card.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/service_group.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/service_navigator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:33:18.293905 otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:33:18.290905 otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:33:18.294905 otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/templates/directive_wrapper/
+-rw-r--r--   0 root         (0) root         (0)      791 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py
+-rw-r--r--   0 root         (0) root         (0)      250 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/templates/directive_wrapper/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:33:18.294905 otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/templates/service_card/
+-rw-r--r--   0 root         (0) root         (0)      791 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/templates/service_card/conf.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/templates/service_card/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/test_directive_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/test_service_card.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 13:33:18.293905 otc_sphinx_directives-0.2.8/otc_sphinx_directives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-12 13:33:18.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-07-12 13:33:18.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-07-12 13:33:18.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 13:33:18.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-07-12 13:33:18.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-12 13:33:18.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 13:33:18.000000 otc_sphinx_directives-0.2.8/otc_sphinx_directives.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      586 2023-07-12 13:33:18.294905 otc_sphinx_directives-0.2.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      651 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/setup.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/tox.ini
+-rw-r--r--   0 root         (0) root         (0)      245 2023-07-12 13:31:59.000000 otc_sphinx_directives-0.2.8/zuul.yaml
```

### Comparing `otc_sphinx_directives-0.2.7/ChangeLog` & `otc_sphinx_directives-0.2.8/ChangeLog`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+0.2.8
+-----
+
+* Added flag for internal or hidden docs (#24)
+
 0.2.7
 -----
 
 * fix doc type typo (#23)
 
 0.2.6
 -----
```

### Comparing `otc_sphinx_directives-0.2.7/LICENSE` & `otc_sphinx_directives-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/PKG-INFO` & `otc_sphinx_directives-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otc_sphinx_directives
-Version: 0.2.7
+Version: 0.2.8
 Summary: Open Telekom Cloud Sphinx Directives
 Home-page: UNKNOWN
 Author: Open Telekom Cloud Ecosystem Squad
 License: UNKNOWN
 Keywords: Sphinx, Sphinx Directives, Open Telekom Cloud
 Platform: UNKNOWN
 Classifier: Framework :: Sphinx
```

### Comparing `otc_sphinx_directives-0.2.7/doc/source/examples/directives_ecs.rst` & `otc_sphinx_directives-0.2.8/doc/source/examples/directives_ecs.rst`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/doc/source/examples/directives_obs.rst` & `otc_sphinx_directives-0.2.8/doc/source/examples/directives_obs.rst`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives/container_item.py` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives/container_item.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives/directive_wrapper.py` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives/directive_wrapper.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives/document_navigator.py` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives/document_navigator.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives/navigator.py` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives/navigator.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives/otc_sphinx_directives_setup.py` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives/otc_sphinx_directives_setup.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives/service_card.py` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives/service_card.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,40 +66,46 @@
         'parallel-file-system': directives.unchanged,
         'permissions-configuration-guide': directives.unchanged,
         'permissions': directives.unchanged,
         'swiftapi': directives.unchanged,
         's3api': directives.unchanged,
         'umn': directives.unchanged,
         'best-practice': directives.unchanged,
+        'environment': directives.unchanged
     }
 
     has_content = True
 
     def run(self):
         node = self.node_class()
         for k in self.option_spec:
             if self.options.get(k):
                 node[k] = self.options.get(k)
+            elif k == 'environment':
+                node[k] = 'public'
             else:
                 node[k] = ''
 
         return [node]
 
 
 def service_card_html(self, node):
     # This method renders containers per each service of the category with all
     # links as individual list items
-    # This method renders containers per each service of the category with all
-    # links as individual list items
 
     data = ''
     service = METADATA.get_service_with_docs_by_service_type(node['service_type'])
     docs = sort_docs(service['documents'])
 
     for doc in docs:
+        environment = doc.get('environment')
+        if environment == "hidden":
+            continue
+        if environment == "internal" and node['environment'] != "internal":
+            continue
         link = ""
         if service["service"]["service_uri"] in doc["link"]:
             link = doc['link'].split("/")[2] + '/'
         else:
             link = doc['link']
 
         data = '<div class="card item-sbv">'
```

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives/service_group.py` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives/service_group.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives/service_navigator.py` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives/service_navigator.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/base.py` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/base.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/templates/service_card/conf.py` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/templates/service_card/conf.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/test_directive_wrapper.py` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/test_directive_wrapper.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives/tests/test_service_card.py` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives/tests/test_service_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,14 @@
     '<div class="card-body">'
     '<h4>User Guide</h4><p></p></div></a></div>'
     '<div class="card item-sbv">'
     '<a href="api-ref/">'
     '<div class="card-body">'
     '<h4>API Reference</h4><p></p></div></a></div>'
     '<div class="card item-sbv">'
-    '<a href="best-practice/">'
-    '<div class="card-body">'
-    '<h4>Best Practice</h4><p></p></div></a></div>'
-    '<div class="card item-sbv">'
     '<a href="dev-guide/">'
     '<div class="card-body">'
     '<h4>Developer Guide</h4><p></p></div></a></div></div>'
 )
 
 
 class TestServiceCardHTML(base.TestCase):
```

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/PKG-INFO` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otc-sphinx-directives
-Version: 0.2.7
+Version: 0.2.8
 Summary: Open Telekom Cloud Sphinx Directives
 Home-page: UNKNOWN
 Author: Open Telekom Cloud Ecosystem Squad
 License: UNKNOWN
 Keywords: Sphinx, Sphinx Directives, Open Telekom Cloud
 Platform: UNKNOWN
 Classifier: Framework :: Sphinx
```

### Comparing `otc_sphinx_directives-0.2.7/otc_sphinx_directives.egg-info/SOURCES.txt` & `otc_sphinx_directives-0.2.8/otc_sphinx_directives.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 zuul.yaml
 doc/requirements.txt
 doc/source/conf.py
 doc/source/index.rst
 doc/source/_static/.placeholder
 doc/source/examples/directives_docsportal.rst
 doc/source/examples/directives_ecs.rst
+doc/source/examples/directives_ecs_internal.rst
 doc/source/examples/directives_obs.rst
 doc/source/examples/directives_obs_clean.rst
 doc/source/examples/index.rst
 otc_sphinx_directives/__init__.py
 otc_sphinx_directives/container_item.py
 otc_sphinx_directives/directive_wrapper.py
 otc_sphinx_directives/document_navigator.py
```

### Comparing `otc_sphinx_directives-0.2.7/setup.cfg` & `otc_sphinx_directives-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/setup.py` & `otc_sphinx_directives-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.7/tox.ini` & `otc_sphinx_directives-0.2.8/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 deps =
     -r{toxinidir}/requirements.txt
 commands = {posargs}
 
 [testenv:docs]
 deps =
     -r{toxinidir}/doc/requirements.txt
+    -e .
 allowlist_externals =
     sphinx-build
 commands =
     sphinx-build -W --keep-going -b html doc/source/ doc/build/html
 
 [flake8]
 # The following are ignored on purpose. It's not super worth it to fix them.
@@ -41,8 +42,8 @@
 #      breaks should occur before the binary operator for readability.
 ignore = H306,H4,W503, E501
 show-source = True
 exclude=.venv,.git,.tox,dist,doc,*lib/python*,*egg,build
 
 [doc8]
 ignore = D001
-extensions = .rst, .yaml
+extensions = .rst, .yaml
```


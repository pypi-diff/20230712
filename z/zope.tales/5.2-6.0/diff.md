# Comparing `tmp/zope.tales-5.2.tar.gz` & `tmp/zope.tales-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.tales-5.2.tar", last modified: Wed Aug 24 06:12:33 2022, max compression
+gzip compressed data, was "zope.tales-6.0.tar", last modified: Wed Jul 12 06:36:34 2023, max compression
```

## Comparing `zope.tales-5.2.tar` & `zope.tales-6.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-24 06:12:33.685027 zope.tales-5.2/
--rw-r--r--   0 mac        (513) staff       (20)     3224 2022-08-24 06:12:31.000000 zope.tales-5.2/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-08-24 06:12:31.000000 zope.tales-5.2/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-08-24 06:12:31.000000 zope.tales-5.2/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-08-24 06:12:31.000000 zope.tales-5.2/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      315 2022-08-24 06:12:31.000000 zope.tales-5.2/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     6376 2022-08-24 06:12:33.685154 zope.tales-5.2/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1400 2022-08-24 06:12:31.000000 zope.tales-5.2/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      119 2022-08-24 06:12:31.000000 zope.tales-5.2/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)        8 2022-08-24 06:12:31.000000 zope.tales-5.2/doc-requirements.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-24 06:12:33.677647 zope.tales-5.2/docs/
--rw-r--r--   0 mac        (513) staff       (20)       28 2022-08-24 06:12:31.000000 zope.tales-5.2/docs/changelog.rst
--rw-r--r--   0 mac        (513) staff       (20)      308 2022-08-24 06:12:31.000000 zope.tales-5.2/docs/compiler.rst
--rw-r--r--   0 mac        (513) staff       (20)     8958 2022-08-24 06:12:31.000000 zope.tales-5.2/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)      294 2022-08-24 06:12:31.000000 zope.tales-5.2/docs/engine.rst
--rw-r--r--   0 mac        (513) staff       (20)      175 2022-08-24 06:12:31.000000 zope.tales-5.2/docs/expressions.rst
--rw-r--r--   0 mac        (513) staff       (20)      276 2022-08-24 06:12:31.000000 zope.tales-5.2/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)       77 2022-08-24 06:12:31.000000 zope.tales-5.2/docs/interfaces.rst
--rw-r--r--   0 mac        (513) staff       (20)       89 2022-08-24 06:12:31.000000 zope.tales-5.2/docs/other.rst
--rw-r--r--   0 mac        (513) staff       (20)      174 2022-08-24 06:12:33.685724 zope.tales-5.2/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3566 2022-08-24 06:12:31.000000 zope.tales-5.2/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-24 06:12:33.670282 zope.tales-5.2/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-24 06:12:33.677986 zope.tales-5.2/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-08-24 06:12:31.000000 zope.tales-5.2/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-24 06:12:33.682704 zope.tales-5.2/src/zope/tales/
--rw-r--r--   0 mac        (513) staff       (20)      697 2022-08-24 06:12:31.000000 zope.tales-5.2/src/zope/tales/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     2164 2022-08-24 06:12:31.000000 zope.tales-5.2/src/zope/tales/engine.py
--rw-r--r--   0 mac        (513) staff       (20)    13193 2022-08-24 06:12:31.000000 zope.tales-5.2/src/zope/tales/expressions.py
--rw-r--r--   0 mac        (513) staff       (20)     3532 2022-08-24 06:12:31.000000 zope.tales-5.2/src/zope/tales/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     3336 2022-08-24 06:12:31.000000 zope.tales-5.2/src/zope/tales/pythonexpr.py
--rw-r--r--   0 mac        (513) staff       (20)    23184 2022-08-24 06:12:31.000000 zope.tales-5.2/src/zope/tales/tales.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-24 06:12:33.684800 zope.tales-5.2/src/zope/tales/tests/
--rw-r--r--   0 mac        (513) staff       (20)      365 2022-08-24 06:12:31.000000 zope.tales-5.2/src/zope/tales/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1027 2022-08-24 06:12:31.000000 zope.tales-5.2/src/zope/tales/tests/simpleexpr.py
--rw-r--r--   0 mac        (513) staff       (20)    19945 2022-08-24 06:12:31.000000 zope.tales-5.2/src/zope/tales/tests/test_expressions.py
--rw-r--r--   0 mac        (513) staff       (20)     2651 2022-08-24 06:12:31.000000 zope.tales-5.2/src/zope/tales/tests/test_pythonexpr.py
--rw-r--r--   0 mac        (513) staff       (20)    11527 2022-08-24 06:12:31.000000 zope.tales-5.2/src/zope/tales/tests/test_tales.py
--rw-r--r--   0 mac        (513) staff       (20)     4468 2022-08-24 06:12:31.000000 zope.tales-5.2/src/zope/tales/tests/test_traverser.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-08-24 06:12:33.680514 zope.tales-5.2/src/zope.tales.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     6376 2022-08-24 06:12:33.000000 zope.tales-5.2/src/zope.tales.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      955 2022-08-24 06:12:33.000000 zope.tales-5.2/src/zope.tales.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-08-24 06:12:33.000000 zope.tales-5.2/src/zope.tales.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-08-24 06:12:33.000000 zope.tales-5.2/src/zope.tales.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-08-24 06:12:33.000000 zope.tales-5.2/src/zope.tales.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      135 2022-08-24 06:12:33.000000 zope.tales-5.2/src/zope.tales.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-08-24 06:12:33.000000 zope.tales-5.2/src/zope.tales.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1381 2022-08-24 06:12:31.000000 zope.tales-5.2/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:36:34.883843 zope.tales-6.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3334 2023-07-12 06:36:34.000000 zope.tales-6.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-12 06:36:34.000000 zope.tales-6.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-12 06:36:34.000000 zope.tales-6.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-12 06:36:34.000000 zope.tales-6.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      315 2023-07-12 06:36:34.000000 zope.tales-6.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6244 2023-07-12 06:36:34.883900 zope.tales-6.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1400 2023-07-12 06:36:34.000000 zope.tales-6.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      119 2023-07-12 06:36:34.000000 zope.tales-6.0/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)        8 2023-07-12 06:36:34.000000 zope.tales-6.0/doc-requirements.txt
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:36:34.880889 zope.tales-6.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       28 2023-07-12 06:36:34.000000 zope.tales-6.0/docs/changelog.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      308 2023-07-12 06:36:34.000000 zope.tales-6.0/docs/compiler.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8958 2023-07-12 06:36:34.000000 zope.tales-6.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      294 2023-07-12 06:36:34.000000 zope.tales-6.0/docs/engine.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      175 2023-07-12 06:36:34.000000 zope.tales-6.0/docs/expressions.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      276 2023-07-12 06:36:34.000000 zope.tales-6.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       77 2023-07-12 06:36:34.000000 zope.tales-6.0/docs/interfaces.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       89 2023-07-12 06:36:34.000000 zope.tales-6.0/docs/other.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      447 2023-07-12 06:36:34.884117 zope.tales-6.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3326 2023-07-12 06:36:34.000000 zope.tales-6.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:36:34.878176 zope.tales-6.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:36:34.881036 zope.tales-6.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:36:34.882854 zope.tales-6.0/src/zope/tales/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      697 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope/tales/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2164 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope/tales/engine.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12996 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope/tales/expressions.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3533 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope/tales/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3307 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope/tales/pythonexpr.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    22950 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope/tales/tales.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:36:34.883707 zope.tales-6.0/src/zope/tales/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope/tales/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1023 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope/tales/tests/simpleexpr.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    19602 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope/tales/tests/test_expressions.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2495 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope/tales/tests/test_pythonexpr.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    11019 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope/tales/tests/test_tales.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4453 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope/tales/tests/test_traverser.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:36:34.882007 zope.tales-6.0/src/zope.tales.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6244 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope.tales.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      955 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope.tales.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope.tales.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope.tales.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope.tales.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      131 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope.tales.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-07-12 06:36:34.000000 zope.tales-6.0/src/zope.tales.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1610 2023-07-12 06:36:34.000000 zope.tales-6.0/tox.ini
```

### Comparing `zope.tales-5.2/CHANGES.rst` & `zope.tales-6.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
  Changes
 =========
 
+6.0 (2023-07-12)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 5.2 (2022-08-24)
 ================
 
 - Add support for Python 3.9, 3.10.
 
 - Fix error message raised if the first element of a path expression is not
   a valid name.
```

### Comparing `zope.tales-5.2/CONTRIBUTING.md` & `zope.tales-6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.tales-5.2/LICENSE.txt` & `zope.tales-6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.tales-5.2/PKG-INFO` & `zope.tales-6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 Metadata-Version: 2.1
 Name: zope.tales
-Version: 5.2
+Version: 6.0
 Summary: Zope Template Application Language Expression Syntax (TALES)
 Home-page: https://github.com/zopefoundation/zope.tales
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Documentation, https://zopetales.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.tales/issues
 Project-URL: Sources, https://github.com/zopefoundation/zope.tales
 Keywords: zope template xml tales
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
-Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: tal
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 ============
  zope.tales
@@ -75,14 +70,22 @@
 https://zopetales.readthedocs.io/
 
 
 =========
  Changes
 =========
 
+6.0 (2023-07-12)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 5.2 (2022-08-24)
 ================
 
 - Add support for Python 3.9, 3.10.
 
 - Fix error message raised if the first element of a path expression is not
   a valid name.
@@ -230,9 +233,7 @@
 
 
 3.0.0 (2004-11-07)
 ==================
 
 - Corresponds to the verison of the zope.tales package shipped as part of
   the Zope X3.0.0 release.
-
-
```

### Comparing `zope.tales-5.2/README.rst` & `zope.tales-6.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.tales-5.2/docs/conf.py` & `zope.tales-6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.tales-5.2/setup.py` & `zope.tales-6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 # This package is developed by the Zope Toolkit project, documented here:
-# http://docs.zope.org/zopetoolkit
+# https://zopetoolkit.readthedocs.io/
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.tales package
 """
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
@@ -31,73 +33,67 @@
     'zope.testing',
     'zope.testrunner',
 ]
 
 
 setup(
     name='zope.tales',
-    version='5.2',
+    version='6.0',
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     description='Zope Template Application Language Expression Syntax '
                 '(TALES)',
     long_description=(
         read('README.rst')
         + '\n\n' +
         read('CHANGES.rst')
     ),
     keywords="zope template xml tales",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Topic :: Internet :: WWW/HTTP',
         'Framework :: Zope :: 3',
-        'Framework :: Zope :: 4',
         'Framework :: Zope :: 5',
     ],
     url='https://github.com/zopefoundation/zope.tales',
     project_urls={
         'Documentation': 'https://zopetales.readthedocs.io/',
         'Issue Tracker': 'https://github.com/zopefoundation/zope.tales/issues',
         'Sources': 'https://github.com/zopefoundation/zope.tales',
     },
     license='ZPL 2.1',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['zope'],
-    python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*',
+    python_requires='>=3.7',
     extras_require={
         'test': TESTS_REQUIRE,
         'tal': [
             'zope.tal',
         ],
         'docs': [
             'Sphinx',
             'repoze.sphinx.autointerface',
             'zope.tal',
         ],
     },
     install_requires=[
         'setuptools',
         'zope.interface',
-        'six',
     ],
-    tests_require=TESTS_REQUIRE,
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `zope.tales-5.2/src/zope/tales/__init__.py` & `zope.tales-6.0/src/zope/tales/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.tales-5.2/src/zope/tales/engine.py` & `zope.tales-6.0/src/zope/tales/engine.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Expression engine configuration and registration.
 
 Each expression engine can have its own expression types and base names.
 """
-from zope.tales.tales import ExpressionEngine
-from zope.tales.expressions import PathExpr
-from zope.tales.expressions import StringExpr
-from zope.tales.expressions import NotExpr
 from zope.tales.expressions import DeferExpr
 from zope.tales.expressions import LazyExpr
+from zope.tales.expressions import NotExpr
+from zope.tales.expressions import PathExpr
 from zope.tales.expressions import SimpleModuleImporter
+from zope.tales.expressions import StringExpr
 from zope.tales.pythonexpr import PythonExpr
+from zope.tales.tales import ExpressionEngine
 
 
 def DefaultEngine():
     """
     Create and return an instance of :class:`~.ExpressionEngine` (an
     implementation of
     :class:`zope.tal.interfaces.ITALExpressionCompiler`) with the
```

### Comparing `zope.tales-5.2/src/zope/tales/expressions.py` & `zope.tales-6.0/src/zope/tales/expressions.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 (they must have previously been registered with
 :func:`~zope.tales.tales.ExpressionEngine.registerType`).  The expression
 object itself is a callable object taking one argument, *econtext*, which is
 the local expression namespace.
 
 """
 import re
-import sys
-import types
-
-import six
 
 from zope.interface import implementer
-from zope.tales.tales import _valid_name, _parse_expr, NAME_RE, Undefined
-from zope.tales.interfaces import ITALESExpression, ITALESFunctionNamespace
+
+from zope.tales.interfaces import ITALESExpression
+from zope.tales.interfaces import ITALESFunctionNamespace
+from zope.tales.tales import NAME_RE
+from zope.tales.tales import Undefined
+from zope.tales.tales import _parse_expr
+from zope.tales.tales import _valid_name
+
 
 Undefs = (Undefined, AttributeError, LookupError, TypeError)
 
 _marker = object()
 namespace_re = re.compile(r'(\w+):(.+)')
 
-PY2 = sys.version_info[0] == 2
-
 
 def simpleTraverse(object, path_items, econtext):
     """Traverses a sequence of names, first trying attributes then items.
     """
 
     for name in path_items:
         next = getattr(object, name, _marker)
@@ -51,15 +51,15 @@
             object = object[name]
         else:
             # Allow AttributeError to propagate
             object = getattr(object, name)
     return object
 
 
-class SubPathExpr(object):
+class SubPathExpr:
     """
     Implementation of a single path expression.
     """
 
     ALLOWED_BUILTINS = {}
 
     def __init__(self, path, traverser, engine):
@@ -112,15 +112,15 @@
 
         first = compiledpath[0]
 
         if callable(first):
             # check for initial function
             raise engine.getCompilerError()(
                 'Namespace function specified in first subpath element')
-        elif isinstance(first, six.string_types):
+        elif isinstance(first, str):
             # check for initial ?
             raise engine.getCompilerError()(
                 'Dynamic name specified in first subpath element')
 
         base = first[0]
         if base and not _valid_name(base):
             raise engine.getCompilerError()(
@@ -147,33 +147,33 @@
                     raise
         if isinstance(ob, DeferWrapper):
             ob = ob()
 
         for element in compiled_path:
             if isinstance(element, tuple):
                 ob = self._traverser(ob, element, econtext)
-            elif isinstance(element, six.string_types):
+            elif isinstance(element, str):
                 val = vars[element]
                 # If the value isn't a string, assume it's a sequence
                 # of path names.
-                if isinstance(val, six.string_types):
+                if isinstance(val, str):
                     val = (val,)
                 ob = self._traverser(ob, val, econtext)
             elif callable(element):
                 ob = element(ob)
                 # TODO: Once we have n-ary adapters, use them.
                 if ITALESFunctionNamespace.providedBy(ob):
                     ob.setEngine(econtext)
             else:
                 raise ValueError(repr(element))
         return ob
 
 
 @implementer(ITALESExpression)
-class PathExpr(object):
+class PathExpr:
     """
     One or more :class:`subpath expressions <SubPathExpr>`, separated
     by ``|``.
     """
 
     # _default_type_names contains the expression type names this
     # class is usually registered for.
@@ -233,40 +233,38 @@
             return ob
 
         # Call the object if it is callable.  Note that checking for
         # callable() isn't safe because the object might be security
         # proxied (and security proxies report themselves callable, no
         # matter what the underlying object is).  We therefore check
         # for the __call__ attribute, but not with hasattr as that
-        # eats babies, err, exceptions.  In addition to that, we
-        # support calling old style classes which don't have a
-        # __call__.
+        # eats babies, err, exceptions.
         if getattr(ob, '__call__', _marker) is not _marker:
             return ob()
-        return ob() if PY2 and isinstance(ob, types.ClassType) else ob
+        return ob
 
     def __call__(self, econtext):
         if self._name == 'exists':
             return self._exists(econtext)
         return self._eval(econtext)
 
     def __str__(self):
-        return '%s expression (%s)' % (self._name, repr(self._s))
+        return '{} expression ({})'.format(self._name, repr(self._s))
 
     def __repr__(self):
-        return '<PathExpr %s:%s>' % (self._name, repr(self._s))
+        return '<PathExpr {}:{}>'.format(self._name, repr(self._s))
 
 
 _interp = re.compile(
     r'\$(%(n)s)|\${(%(n)s(?:/[^}|]*)*(?:\|\s*%(n)s(?:/[^}|]*)*)*)}'
     % {'n': NAME_RE})
 
 
 @implementer(ITALESExpression)
-class StringExpr(object):
+class StringExpr:
     """
     An expression that produces a string.
 
     Sub-sequences of the string that begin with ``$`` are
     interpreted as path expressions to evaluate.
     """
 
@@ -308,15 +306,15 @@
         return 'string expression (%s)' % repr(self._s)
 
     def __repr__(self):
         return '<StringExpr %s>' % repr(self._s)
 
 
 @implementer(ITALESExpression)
-class NotExpr(object):
+class NotExpr:
     """
     An expression that negates the boolean value
     of its sub-expression.
     """
 
     def __init__(self, name, expr, engine):
         self._s = expr = expr.lstrip()
@@ -325,28 +323,28 @@
     def __call__(self, econtext):
         return int(not econtext.evaluateBoolean(self._c))
 
     def __repr__(self):
         return '<NotExpr %s>' % repr(self._s)
 
 
-class DeferWrapper(object):
+class DeferWrapper:
     def __init__(self, expr, econtext):
         self._expr = expr
         self._econtext = econtext
 
     def __str__(self):
         return str(self())
 
     def __call__(self):
         return self._expr(self._econtext)
 
 
 @implementer(ITALESExpression)
-class DeferExpr(object):
+class DeferExpr:
     """
     An expression that will defer evaluation of the sub-expression
     until necessary, preserving the execution context it was created
     with.
 
     This is useful in ``tal:define`` expressions::
 
@@ -394,15 +392,15 @@
     def __call__(self, econtext):
         return LazyWrapper(self._c, econtext)
 
     def __repr__(self):
         return 'lazy:%s' % repr(self._s)
 
 
-class SimpleModuleImporter(object):
+class SimpleModuleImporter:
     """Minimal module importer with no security."""
 
     def __getitem__(self, module):
         mod = self._get_toplevel_module(module)
         path = module.split('.')
         for name in path[1:]:
             mod = getattr(mod, name)
```

### Comparing `zope.tales-5.2/src/zope/tales/interfaces.py` & `zope.tales-6.0/src/zope/tales/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #
 ##############################################################################
 """
 Interface that describes the TALES implementation.
 """
 from zope.interface import Interface
 
+
 try:
     from zope.tal.interfaces import ITALIterator
 except ImportError:
     class ITALIterator(Interface):
         """Stub: See zope.tal.interfaces.ITALIterator"""
 
         def next():
```

### Comparing `zope.tales-5.2/src/zope/tales/pythonexpr.py` & `zope.tales-6.0/src/zope/tales/pythonexpr.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 ##############################################################################
 """Generic Python Expression Handler
 """
 import types
 
 
-class PythonExpr(object):
+class PythonExpr:
     """
     Evaluates a python expression by calling :func:`eval` after
     compiling it with :func:`compile`.
     """
     def __init__(self, name, expr, engine):
         """
         :param str expr: The Python expression.
@@ -32,15 +32,15 @@
         self.text = text
         try:
             code = self._compile(text, '<string>')
         except SyntaxError as e:
             raise engine.getCompilerError()(str(e))
         self._code = code
         self._varnames = code.co_names
-        # In Python 3, variables used inside list comprehensions are not
+        # Variables used inside list comprehensions are not
         # directly available via co_names.
         for const in code.co_consts:
             if isinstance(const, types.CodeType):
                 self._varnames += const.co_names
 
     def _compile(self, text, filename):
         return compile(text, filename, 'eval')
@@ -75,15 +75,15 @@
     def __str__(self):
         return 'Python expression "%s"' % self.text
 
     def __repr__(self):
         return '<PythonExpr %s>' % self.text
 
 
-class ExprTypeProxy(object):
+class ExprTypeProxy:
     '''Class that proxies access to an expression type handler'''
     def __init__(self, name, handler, econtext):
         self._name = name
         self._handler = handler
         self._econtext = econtext
 
     def __call__(self, text):
```

### Comparing `zope.tales-5.2/src/zope/tales/tales.py` & `zope.tales-6.0/src/zope/tales/tales.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,23 +12,18 @@
 #
 ##############################################################################
 """TALES
 
 An implementation of a TAL expression engine
 """
 import re
+from html import escape
 
-try:
-    from html import escape
-except ImportError:  # pragma: PY2
-    from cgi import escape
-
-from zope.interface import implementer
 from zope.interface import Interface
-import six
+from zope.interface import implementer
 
 from zope.tales.interfaces import ITALESIterator
 
 
 class ITALExpressionEngine(Interface):
     pass
 
@@ -39,17 +34,17 @@
 
 class ITALExpressionErrorInfo(Interface):
     pass
 
 
 try:
     # Override with real, if present
-    from zope.tal.interfaces import (ITALExpressionEngine,  # noqa: F811
-                                     ITALExpressionCompiler,
-                                     ITALExpressionErrorInfo)
+    from zope.tal.interfaces import ITALExpressionCompiler  # noqa: F811
+    from zope.tal.interfaces import ITALExpressionEngine  # noqa: F811
+    from zope.tal.interfaces import ITALExpressionErrorInfo  # noqa: F811
 except ImportError:
     pass
 
 
 NAME_RE = r"[a-zA-Z][a-zA-Z0-9_]*"
 _parse_expr = re.compile(r"(%s):" % NAME_RE).match
 _valid_name = re.compile('%s$' % NAME_RE).match
@@ -71,15 +66,15 @@
     """Expression type or base name registration Error."""
 
 
 _default = object()
 
 
 @implementer(ITALESIterator)
-class Iterator(object):
+class Iterator:
     """
     TALES Iterator.
 
     Default implementation of :class:`zope.tales.interfaces.ITALESIterator`.
 
     """
 
@@ -100,25 +95,25 @@
         We can create an iterator on an empty sequence:
 
         >>> it = Iterator('foo', (), context)
 
         An iterator works as well:
 
         >>> it = Iterator('foo', {"apple":1, "pear":1, "orange":1}, context)
-        >>> it.next()
+        >>> next(it)
         True
 
         >>> it = Iterator('foo', {}, context)
-        >>> it.next()
+        >>> next(it)
         False
 
         >>> it = Iterator('foo', iter((1, 2, 3)), context)
-        >>> it.next()
+        >>> next(it)
         True
-        >>> it.next()
+        >>> next(it)
         True
 
         """
 
         self._seq = seq
         self._iter = i = iter(seq)
         self._nextIndex = 0
@@ -136,45 +131,45 @@
             self._done = False
 
     def __next__(self):
         """Advance the iterator, if possible.
 
         >>> context = Context(ExpressionEngine(), {})
         >>> it = Iterator('foo', ("apple", "pear", "orange"), context)
-        >>> bool(it.next())
+        >>> bool(next(it))
         True
         >>> context.vars['foo']
         'apple'
-        >>> bool(it.next())
+        >>> bool(next(it))
         True
         >>> context.vars['foo']
         'pear'
-        >>> bool(it.next())
+        >>> bool(next(it))
         True
         >>> context.vars['foo']
         'orange'
-        >>> bool(it.next())
+        >>> bool(next(it))
         False
 
         >>> it = Iterator('foo', {"apple":1, "pear":1, "orange":1}, context)
-        >>> bool(it.next())
+        >>> bool(next(it))
         True
-        >>> bool(it.next())
+        >>> bool(next(it))
         True
-        >>> bool(it.next())
+        >>> bool(next(it))
         True
-        >>> bool(it.next())
+        >>> bool(next(it))
         False
 
         >>> it = Iterator('foo', (), context)
-        >>> bool(it.next())
+        >>> bool(next(it))
         False
 
         >>> it = Iterator('foo', {}, context)
-        >>> bool(it.next())
+        >>> bool(next(it))
         False
 
 
         If we can advance, set a local variable to the new value.
         """
         # Note that these are *NOT* Python iterators!
         if self._done:
@@ -186,117 +181,115 @@
             self._done = True
             self._last = True
 
         self._nextIndex += 1
         self._setLocal(self._name, v)
         return True
 
-    next = __next__  # Python 2 compatibility
-
     def index(self):
         """Get the iterator index
 
         >>> context = Context(ExpressionEngine(), {})
         >>> it = Iterator('foo', ("apple", "pear", "orange"), context)
         >>> it.index()
         Traceback (most recent call last):
         ...
         TypeError: No iteration position
-        >>> int(bool(it.next()))
+        >>> int(bool(next(it)))
         1
         >>> it.index()
         0
-        >>> int(bool(it.next()))
+        >>> int(bool(next(it)))
         1
         >>> it.index()
         1
-        >>> int(bool(it.next()))
+        >>> int(bool(next(it)))
         1
         >>> it.index()
         2
         """
         index = self._nextIndex - 1
         if index < 0:
             raise TypeError("No iteration position")
         return index
 
     def number(self):
         """Get the iterator position
 
         >>> context = Context(ExpressionEngine(), {})
         >>> it = Iterator('foo', ("apple", "pear", "orange"), context)
-        >>> int(bool(it.next()))
+        >>> int(bool(next(it)))
         1
         >>> it.number()
         1
-        >>> int(bool(it.next()))
+        >>> int(bool(next(it)))
         1
         >>> it.number()
         2
-        >>> int(bool(it.next()))
+        >>> int(bool(next(it)))
         1
         >>> it.number()
         3
         """
         return self._nextIndex
 
     def even(self):
         """Test whether the position is even
 
         >>> context = Context(ExpressionEngine(), {})
         >>> it = Iterator('foo', ("apple", "pear", "orange"), context)
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.even()
         True
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.even()
         False
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.even()
         True
         """
         return not ((self._nextIndex - 1) % 2)
 
     def odd(self):
         """Test whether the position is odd
 
         >>> context = Context(ExpressionEngine(), {})
         >>> it = Iterator('foo', ("apple", "pear", "orange"), context)
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.odd()
         False
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.odd()
         True
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.odd()
         False
         """
         return bool((self._nextIndex - 1) % 2)
 
     def parity(self):
         """Return 'odd' or 'even' depending on the position's parity
 
         >>> context = Context(ExpressionEngine(), {})
         >>> it = Iterator('foo', ("apple", "pear", "orange"), context)
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.parity()
         'odd'
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.parity()
         'even'
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.parity()
         'odd'
         """
         if self._nextIndex % 2:
             return 'odd'
         return 'even'
@@ -306,23 +299,23 @@
 
         >>> context = Context(ExpressionEngine(), {})
         >>> it = Iterator('foo', ("apple", "pear", "orange"), context)
         >>> it.letter()
         Traceback (most recent call last):
         ...
         TypeError: No iteration position
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.letter()
         'a'
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.letter()
         'b'
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.letter()
         'c'
         """
         index = self._nextIndex - 1
         if index < 0:
             raise TypeError("No iteration position")
@@ -334,46 +327,46 @@
                 return s
 
     def Letter(self):
         """Get the iterator position as an upper-case letter
 
         >>> context = Context(ExpressionEngine(), {})
         >>> it = Iterator('foo', ("apple", "pear", "orange"), context)
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.Letter()
         'A'
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.Letter()
         'B'
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.Letter()
         'C'
         """
         return self.letter(base=ord('A'))
 
     def Roman(self, rnvalues=(
             (1000, 'M'), (900, 'CM'), (500, 'D'), (400, 'CD'),
             (100, 'C'), (90, 'XC'), (50, 'L'), (40, 'XL'),
             (10, 'X'), (9, 'IX'), (5, 'V'), (4, 'IV'), (1, 'I'))):
         """Get the iterator position as an upper-case roman numeral
 
         >>> context = Context(ExpressionEngine(), {})
         >>> it = Iterator('foo', ("apple", "pear", "orange"), context)
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.Roman()
         'I'
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.Roman()
         'II'
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.Roman()
         'III'
         """
         n = self._nextIndex
         s = ''
         for v, r in rnvalues:
@@ -382,79 +375,79 @@
         return s
 
     def roman(self):
         """Get the iterator position as a lower-case roman numeral
 
         >>> context = Context(ExpressionEngine(), {})
         >>> it = Iterator('foo', ("apple", "pear", "orange"), context)
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.roman()
         'i'
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.roman()
         'ii'
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.roman()
         'iii'
         """
         return self.Roman().lower()
 
     def start(self):
         """Test whether the position is the first position
 
         >>> context = Context(ExpressionEngine(), {})
         >>> it = Iterator('foo', ("apple", "pear", "orange"), context)
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.start()
         True
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.start()
         False
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.start()
         False
 
         >>> it = Iterator('foo', {}, context)
         >>> it.start()
         False
-        >>> it.next()
+        >>> next(it)
         False
         >>> it.start()
         False
         """
         return self._nextIndex == 1
 
     def end(self):
         """Test whether the position is the last position
 
         >>> context = Context(ExpressionEngine(), {})
         >>> it = Iterator('foo', ("apple", "pear", "orange"), context)
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.end()
         False
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.end()
         False
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.end()
         True
 
         >>> it = Iterator('foo', {}, context)
         >>> it.end()
         False
-        >>> it.next()
+        >>> next(it)
         False
         >>> it.end()
         False
         """
         return self._last
 
     def item(self):
@@ -462,29 +455,29 @@
 
         >>> context = Context(ExpressionEngine(), {})
         >>> it = Iterator('foo', ("apple", "pear", "orange"), context)
         >>> it.item()
         Traceback (most recent call last):
         ...
         TypeError: No iteration position
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.item()
         'apple'
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.item()
         'pear'
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.item()
         'orange'
 
         >>> it = Iterator('foo', {1:2}, context)
-        >>> it.next()
+        >>> next(it)
         True
         >>> it.item()
         1
 
         """
         if self._nextIndex == 0:
             raise TypeError("No iteration position")
@@ -523,15 +516,15 @@
         ... else:
         ...     print('Expected TypeError')
         """
         return len(self._seq)
 
 
 @implementer(ITALExpressionErrorInfo)
-class ErrorInfo(object):
+class ErrorInfo:
     """Information about an exception passed to an on-error handler."""
 
     # XXX: This is a duplicate of zope.tal.taldefs.ErrorInfo
     value = None
 
     def __init__(self, err, position=(None, None)):
         self.type = err
@@ -540,15 +533,15 @@
             self.value = err
 
         self.lineno = position[0]
         self.offset = position[1]
 
 
 @implementer(ITALExpressionCompiler)
-class ExpressionEngine(object):
+class ExpressionEngine:
     """
     Expression compiler, an implementation of
     :class:`zope.tal.interfaces.ITALExpressionCompiler`.
 
     An instance of this class keeps :meth:`a mutable collection of
     expression type handlers
     <zope.tales.tales.ExpressionEngine.registerType>`.  It can compile
@@ -672,15 +665,15 @@
         return Context(self, kwcontexts)
 
     def getCompilerError(self):
         return CompilerError
 
 
 @implementer(ITALExpressionEngine)
-class Context(object):
+class Context:
     """
     Expression engine, an implementation of
     :class:`zope.tal.interfaces.ITALExpressionEngine`.
 
     This class is called ``Context`` because an instance of this class
     holds context information (namespaces) that it uses when evaluating
     compiled expressions.
@@ -785,18 +778,18 @@
         # reassigned.
         return not not self.evaluate(expr)
 
     def evaluateText(self, expr):
         text = self.evaluate(expr)
         if text is self.getDefault() or text is None:
             return text
-        if isinstance(text, six.string_types):
+        if isinstance(text, str):
             # text could already be something text-ish, e.g. a Message object
             return text
-        return six.text_type(text)
+        return str(text)
 
     evaluateStructure = evaluate
 
     # TODO: Should return None or a macro definition
     evaluateMacro = evaluate
 
     def createErrorInfo(self, err, position):
@@ -810,18 +803,18 @@
 
     def setPosition(self, position):
         self.position = position
 
     def translate(self, msgid, domain=None, mapping=None, default=None):
         # custom Context implementations are supposed to customize
         # this to call whichever translation routine they want to use
-        return six.text_type(msgid)
+        return str(msgid)
 
 
-class TALESTracebackSupplement(object):
+class TALESTracebackSupplement:
     """Implementation of zope.exceptions.ITracebackSupplement"""
 
     def __init__(self, context, expression):
         self.context = context
         self.source_url = context.source_file
         self.line = context.position[0]
         self.column = context.position[1]
```

### Comparing `zope.tales-5.2/src/zope/tales/tests/simpleexpr.py` & `zope.tales-6.0/src/zope/tales/tests/simpleexpr.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Simple TALES Expression
 """
 
 
-class SimpleExpr(object):
+class SimpleExpr:
     """Simple example of an expression type handler for testing."""
 
     def __init__(self, name, expr, engine):
         self._name = name
         self._expr = expr
 
     def __call__(self, econtext):
         return self._name, self._expr
 
     def __repr__(self):
-        return '<SimpleExpr %s %s>' % (self._name, repr(self._expr))
+        return '<SimpleExpr {} {}>'.format(self._name, repr(self._expr))
```

### Comparing `zope.tales-5.2/src/zope/tales/tests/test_expressions.py` & `zope.tales-6.0/src/zope/tales/tests/test_expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ##############################################################################
 #
 # Copyright (c) 2001, 2002 Zope Foundation and Contributors.
 # All Rights Reserved.
 #
 # This software is subject to the provisions of the Zope Public License,
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
@@ -10,27 +9,27 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Default TALES expression implementations tests.
 """
-import six
 import unittest
 
+from zope.interface import implementer
+
 from zope.tales.engine import Engine
 from zope.tales.interfaces import ITALESFunctionNamespace
 from zope.tales.tales import Undefined
-from zope.interface import implementer
-import zope.tales.tests
+
 
 text_type = str if str is not bytes else unicode  # noqa PY2
 
 
-class Data(object):
+class Data:
 
     def __init__(self, **kw):
         self.__dict__.update(kw)
 
     def __getattr__(self, name):
         # Let linters (like pylint) know this is a dynamic class and they
         # shouldn't emit "Data has no attribute" errors
@@ -38,36 +37,36 @@
 
     def __repr__(self):
         return self.name
 
     __str__ = __repr__
 
 
-class ErrorGenerator(object):
+class ErrorGenerator:
 
     def __getitem__(self, name):
-        from six.moves import builtins
+        import builtins
         if name == 'Undefined':
             e = Undefined
         else:
             e = getattr(builtins, name, None) or SystemError
         raise e('mess')
 
 
-class Callable(object):
+class Callable:
 
     def __call__(self):
         return 42
 
 
 class OldStyleCallable:  # NOT object
     pass
 
 
-class ExpressionTestBase(zope.tales.tests.TestCase):
+class ExpressionTestBase(unittest.TestCase):
 
     def setUp(self):
         # Test expression compilation
         d = Data(
             name='xander',
             y=Data(
                 name='yikes',
@@ -82,24 +81,23 @@
             vars=dict(
                 x=d,
                 y=Data(z=3),
                 b='boot',
                 B=2,
                 adapterTest=at,
                 dynamic='z',
-                eightBits=u'déjà vu'.encode('utf-8'),
+                eightBits='déjà vu'.encode(),
                 ErrorGenerator=ErrorGenerator(),
                 callable=Callable(),
                 old_callable_class=OldStyleCallable,
             )
         )
 
         self.engine = Engine
-
-        self.py3BrokenEightBits = "a b'd\\xc3\\xa9j\\xc3\\xa0 vu'"
+        self.brokenEightBits = "a b'd\\xc3\\xa9j\\xc3\\xa0 vu'"
 
     def _compiled_expr(self, expr):
         return self.engine.compile(expr) if isinstance(expr, str) else expr
 
     def _check_evals_to(self, expr, result):
         expr = self._compiled_expr(expr)
         self.assertEqual(expr(self.context), result)
@@ -169,15 +167,15 @@
             expr = self.engine.compile(
                 'path:ErrorGenerator/%s | b | c/d/e' % e)
             self._check_evals_to(expr, 'boot')
 
     def testNonAsciiPath(self):
         error = self.engine.getCompilerError()
         with self.assertRaises(error):
-            self.engine.compile(u'path: ä')
+            self.engine.compile('path: ä')
 
     def test_path_CONTEXTS(self):
         self.context.contexts = 42
         self._check_evals_to('CONTEXTS', 42)
 
     def testDynamic(self):
         expr = self.engine.compile('x/y/?dynamic')
@@ -239,39 +237,34 @@
         # See https://bugs.launchpad.net/zope.tales/+bug/1002242
         CompilerError = self.engine.getCompilerError()
         self.assertRaises(CompilerError,
                           self.engine.compile,
                           'string:${nothig/nothing|python:1}')
 
     def testString8Bits(self):
-        # Simple eight bit string interpolation should just work.
-        # Except on Py3, where we really mess it up.
+        # Simple eight bit string interpolation is a real mess.
         expr = self.engine.compile('string:a ${eightBits}')
-        expected = ('a ' + self.context.vars['eightBits']
-                    if not six.PY3 else self.py3BrokenEightBits)
-        self._check_evals_to(expr, expected)
+        self._check_evals_to(expr, self.brokenEightBits)
 
     def testStringUnicode(self):
         # Unicode string expressions should return unicode strings
-        expr = self.engine.compile(u'string:Fred')
+        expr = self.engine.compile('string:Fred')
         context = self.context
         result = expr(context)
-        self.assertEqual(result, u'Fred')
+        self.assertEqual(result, 'Fred')
         self.assertIsInstance(result, text_type)
 
     def testStringFailureWhenMixed(self):
         # Mixed Unicode and 8bit string interpolation fails with a
         # UnicodeDecodeError, assuming there is no default encoding
-        expr = self.engine.compile(u'string:a ${eightBits}')
+        expr = self.engine.compile('string:a ${eightBits}')
         with self.assertRaises(UnicodeDecodeError):
             result = expr(self.context)
-            # If we get here, we're on Python 3, which handles this
-            # poorly.
-            self.assertTrue(six.PY3)
-            self.assertEqual(result, self.py3BrokenEightBits)
+            # Python which handles this poorly.
+            self.assertEqual(result, self.brokenEightBits)
             # raise UnicodeDecodeError
             self.context.vars['eightBits'].decode('ascii')
 
     def test_string_escape_percent(self):
         self._check_evals_to('string:%', '%')
 
     def testPython(self):
@@ -337,16 +330,16 @@
         check('string:foo${ab/cd | c//d | e/f}bar')
         check('string:foo${ab/cd | c/d/ | e/f}bar')
         check('string:foo${ab/cd | c/d | /e/f}bar')
         check('string:foo${ab/cd | c/d | e//f}bar')
         check('string:foo${ab/cd | c/d | e/f/}bar')
 
     def test_defer_expression_returns_wrapper(self):
-        from zope.tales.expressions import DeferWrapper
         from zope.tales.expressions import DeferExpr
+        from zope.tales.expressions import DeferWrapper
         expr = self.engine.compile('defer: B')
         self.assertIsInstance(expr, DeferExpr)
         self.assertEqual(str(expr), "<DeferExpr 'B'>")
         self._check_evals_to_instance(expr, DeferWrapper)
 
         wrapper = expr(self.context)
         # It evaluates to what its underlying expression evaluates to
@@ -357,16 +350,16 @@
 
     def test_eval_defer_wrapper(self):
         expr = self.engine.compile('defer: b')
         self.context.vars['deferred'] = expr(self.context)
         self._check_evals_to('deferred', self.context.vars['b'])
 
     def test_lazy_expression_returns_wrapper(self):
-        from zope.tales.expressions import LazyWrapper
         from zope.tales.expressions import LazyExpr
+        from zope.tales.expressions import LazyWrapper
         expr = self.engine.compile('lazy: b')
         self.assertIsInstance(expr, LazyExpr)
         self.assertEqual(repr(expr), "lazy:'b'")
         lazy = expr(self.context)
         self.assertIsInstance(lazy, LazyWrapper)
 
         first_result = lazy()
@@ -389,16 +382,17 @@
     def test_bad_initial_name_subexpr(self):
         self._check_subexpr_raises_compiler_error(
             '123',
             "Invalid variable name"
         )
 
     def test_builtins_in_path(self):
+        from ..expressions import PathExpr
+        from ..expressions import SubPathExpr
         from ..tales import ExpressionEngine
-        from ..expressions import PathExpr, SubPathExpr
 
         class MySubPathExpr(SubPathExpr):
             ALLOWED_BUILTINS = {'True': True, 'False': False, 'x': None}
 
         class MyPathExpr(PathExpr):
             SUBEXPR_FACTORY = MySubPathExpr
 
@@ -419,15 +413,15 @@
 class FunctionTests(ExpressionTestBase):
 
     def setUp(self):
         ExpressionTestBase.setUp(self)
 
         # a test namespace
         @implementer(ITALESFunctionNamespace)
-        class TestNameSpace(object):
+        class TestNameSpace:
 
             def __init__(self, context):
                 self.context = context
 
             def setEngine(self, engine):
                 self._engine = engine
```

### Comparing `zope.tales-5.2/src/zope/tales/tests/test_pythonexpr.py` & `zope.tales-6.0/src/zope/tales/tests/test_pythonexpr.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,41 +8,35 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
-import six
 import unittest
 
 from zope.tales.engine import Engine
-from zope.tales.tales import Context
-
-from zope.tales.pythonexpr import PythonExpr
 from zope.tales.pythonexpr import ExprTypeProxy
+from zope.tales.pythonexpr import PythonExpr
+from zope.tales.tales import Context
 
 
 class TestPythonExpr(unittest.TestCase):
 
     def setUp(self):
         self.context = Context(Engine, {})
         self.engine = Engine
 
     def test_init(self):
         expr = PythonExpr(None, 'a', None)
         self.assertEqual(expr._varnames, ('a',))
 
     def test_init_listcomp(self):
         expr = PythonExpr(None, '[f for f in foo if exists(f)]', None)
-        if six.PY2:
-            self.assertEqual(
-                expr._varnames, ('foo', 'f', 'exists'))  # pragma: no cover
-        else:
-            self.assertEqual(expr._varnames, ('foo', 'exists'))
+        self.assertEqual(expr._varnames, ('foo', 'exists'))
 
     def test_repr_str(self):
         expr = PythonExpr(None, 'a', None)
         self.assertEqual('Python expression "(a)"', str(expr))
         self.assertEqual('<PythonExpr (a)>', repr(expr))
 
     def test_bind_not_dict(self):
```

### Comparing `zope.tales-5.2/src/zope/tales/tests/test_tales.py` & `zope.tales-6.0/src/zope/tales/tests/test_tales.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,20 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """TALES Tests
 """
-from doctest import DocTestSuite
-import unittest
-import re
 import sys
+import unittest
+from doctest import DocTestSuite
 
-import six
 from zope.tales import tales
 from zope.tales.tests.simpleexpr import SimpleExpr
-from zope.testing import renormalizing
-import zope.tales.tests
 
 
 class TestIterator(unittest.TestCase):
 
     def testIterator0(self):
         # Test sample Iterator class
         context = Harness(self)
@@ -108,15 +104,15 @@
         se = self.getContext().evaluate('simple:x')
         self.assertEqual(se, ('simple', 'x'), (
             'Improperly evaluated expression %s.' % repr(se)))
 
     def testContext_evaluateText(self):
         # Test use of Context
         se = self.getContext().evaluateText('simple:x')
-        self.assertTrue(isinstance(se, six.text_type))
+        self.assertTrue(isinstance(se, str))
         self.assertEqual(se, "('simple', 'x')")
 
     def test_context_createErrorInfo(self):
         ei = self.getContext().createErrorInfo(self, (0, 0))
         self.assertEqual(ei.type, self)
         self.assertEqual(ei.value, None)
 
@@ -149,15 +145,15 @@
         c = ctxt.vars
         self.assertEqual(c['v1'], 1, "Uncovered local")
         self.assertEqual(c['g'], 1, "Global from inner scope")
 
         ctxt.endScope()
 
 
-class TestExpressionEngine(zope.tales.tests.TestCase):
+class TestExpressionEngine(unittest.TestCase):
 
     def setUp(self):
         self.engine = tales.ExpressionEngine()
 
     def test_register_invalid_name(self):
         with self.assertRaisesRegex(tales.RegistrationError,
                                     "Invalid base name"):
@@ -221,40 +217,37 @@
         self.context.beginScope()
         self.context.vars['it'] = 2
         self.assertEqual(self.context.getValue('it'), 1)
 
     def test_evaluate_boolean(self):
         # Make sure it always returns a regular bool, no matter
         # what the class returns
-        class WithCustomBool(object):
+        class WithCustomBool:
 
             def __init__(self, value):
                 self.value = value
 
             def __bool__(self):
                 return self.value
 
-            __nonzero__ = __bool__
-
-        # On Python 2, you can return only bool or int from __nonzero__
-        # Python 3 requires just a bool from __bool__. This is true whether
+        # Python requires just a bool from __bool__. This is true whether
         # you pass it to the bool builtin on the not operator
-        # On both 2 and 3, you cannot subclass bool()
-        bool_value = 1 if str is bytes else True
+        # You cannot subclass bool()
+        bool_value = True
         self.context.vars['it'] = WithCustomBool(bool_value)
         self.assertEqual(bool_value, self.context.evaluate('it').__bool__())
         self.assertIs(True, self.context.evaluateBoolean('it'))
 
     def test_evaluateText_none(self):
         self.context.vars['it'] = None
         self.assertIsNone(self.context.evaluateText('it'))
 
     def test_evaluateText_text(self):
-        self.context.vars['it'] = u'text'
-        self.assertEqual(u'text', self.context.evaluateText("it"))
+        self.context.vars['it'] = 'text'
+        self.assertEqual('text', self.context.evaluateText("it"))
 
     def test_traceback_supplement(self):
         def raises(self):
             raise Exception()
 
         self.context.contexts['modules'] = 1
         self.context.setSourceFile("source")
@@ -285,19 +278,18 @@
         html_info = supp.getInfo(as_html=True)
         self.assertIn('<b>Names', html_info)
 
         # And we didn't change the data in the context
         self.assertIn('modules', self.context.contexts)
 
     def test_translate(self):
-        import six
-        self.assertIsInstance(self.context.translate(b'abc'), six.text_type)
+        self.assertIsInstance(self.context.translate(b'abc'), str)
 
 
-class Harness(object):
+class Harness:
     def __init__(self, testcase):
         self._callstack = []
         self._testcase = testcase
 
     def _assert_(self, name, *args, **kwargs):
         self._callstack.append((name, args, kwargs))
 
@@ -305,15 +297,15 @@
         self._testcase.assertEqual(len(self._callstack), 0,
                                    "Harness methods called")
 
     def __getattr__(self, name):
         return HarnessMethod(self, name)
 
 
-class HarnessMethod(object):
+class HarnessMethod:
 
     def __init__(self, harness, name):
         self._harness = harness
         self._name = name
 
     def __call__(self, *args, **kwargs):
         name = self._name
@@ -333,15 +325,10 @@
         name, aargs, akwargs = self._callstack.pop(0)
         self._testcase.assertEqual(aargs, args, "Harness method arguments")
         self._testcase.assertEqual(akwargs, kwargs,
                                    "Harness method keyword args")
 
 
 def test_suite():
-    checker = renormalizing.RENormalizing([
-        (re.compile(r"object of type 'MyIter' has no len\(\)"),
-         r"len() of unsized object"),
-    ])
     suite = unittest.defaultTestLoader.loadTestsFromName(__name__)
-    suite.addTest(DocTestSuite("zope.tales.tales",
-                               checker=checker))
+    suite.addTest(DocTestSuite("zope.tales.tales"))
     return suite
```

### Comparing `zope.tales-5.2/src/zope/tales/tests/test_traverser.py` & `zope.tales-6.0/src/zope/tales/tests/test_traverser.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """ Tests for zope.tales.expressions.simpleTraverse
 """
 from unittest import TestCase
+
 from zope.tales.expressions import simpleTraverse
 
 
-class AttrTraversable(object):
+class AttrTraversable:
     """Traversable by attribute access"""
     attr = 'foo'
 
 
-class ItemTraversable(object):
+class ItemTraversable:
     """Traversable by item access"""
 
     def __getitem__(self, name):
         if name == 'attr':
             return 'foo'
         raise KeyError(name)
```

### Comparing `zope.tales-5.2/src/zope.tales.egg-info/PKG-INFO` & `zope.tales-6.0/src/zope.tales.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 Metadata-Version: 2.1
 Name: zope.tales
-Version: 5.2
+Version: 6.0
 Summary: Zope Template Application Language Expression Syntax (TALES)
 Home-page: https://github.com/zopefoundation/zope.tales
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Documentation, https://zopetales.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/zopefoundation/zope.tales/issues
 Project-URL: Sources, https://github.com/zopefoundation/zope.tales
 Keywords: zope template xml tales
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Zope :: 3
-Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 Provides-Extra: test
 Provides-Extra: tal
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 ============
  zope.tales
@@ -75,14 +70,22 @@
 https://zopetales.readthedocs.io/
 
 
 =========
  Changes
 =========
 
+6.0 (2023-07-12)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Add support for Python 3.11.
+
+
 5.2 (2022-08-24)
 ================
 
 - Add support for Python 3.9, 3.10.
 
 - Fix error message raised if the first element of a path expression is not
   a valid name.
@@ -230,9 +233,7 @@
 
 
 3.0.0 (2004-11-07)
 ==================
 
 - Corresponds to the verison of the zope.tales package shipped as part of
   the Zope X3.0.0 release.
-
-
```

### Comparing `zope.tales-5.2/src/zope.tales.egg-info/SOURCES.txt` & `zope.tales-6.0/src/zope.tales.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.tales-5.2/tox.ini` & `zope.tales-6.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
-    pypy
+    py311
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
+package = wheel
+wheel_build_env = .pkg
 deps =
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
     test
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+commands =
+    isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
+    flake8 src setup.py
+    check-manifest
+    check-python-versions
 deps =
-    flake8
     check-manifest
     check-python-versions >= 0.19.1
     wheel
+    flake8
+    isort
+
+[testenv:isort-apply]
+basepython = python3
+skip_install = true
+commands_pre =
+deps =
+    isort
 commands =
-    flake8 src setup.py
-    check-manifest
-    check-python-versions
+    isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:docs]
 basepython = python3
 skip_install = false
 extras =
     docs
 commands_pre =
@@ -48,24 +58,22 @@
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
-    coverage html
-    coverage report -m --fail-under=99
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=99
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.tales
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```


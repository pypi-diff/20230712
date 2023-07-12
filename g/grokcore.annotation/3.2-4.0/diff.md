# Comparing `tmp/grokcore.annotation-3.2.tar.gz` & `tmp/grokcore.annotation-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grokcore.annotation-3.2.tar", last modified: Tue Aug 31 14:21:01 2021, max compression
+gzip compressed data, was "grokcore.annotation-4.0.tar", last modified: Wed Jul 12 06:41:17 2023, max compression
```

## Comparing `grokcore.annotation-3.2.tar` & `grokcore.annotation-4.0.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2021-08-31 14:21:01.254725 grokcore.annotation-3.2/
--rw-r--r--   0 jw         (501) staff       (20)     2296 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/CHANGES.rst
--rw-r--r--   0 jw         (501) staff       (20)       32 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/COPYRIGHT.txt
--rw-r--r--   0 jw         (501) staff       (20)     2070 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/LICENSE.txt
--rw-r--r--   0 jw         (501) staff       (20)      212 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/MANIFEST.in
--rw-r--r--   0 jw         (501) staff       (20)     7376 2021-08-31 14:21:01.254885 grokcore.annotation-3.2/PKG-INFO
--rw-r--r--   0 jw         (501) staff       (20)     2529 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/README.rst
--rw-r--r--   0 jw         (501) staff       (20)      412 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/buildout.cfg
--rw-r--r--   0 jw         (501) staff       (20)      124 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/requirements.txt
--rw-r--r--   0 jw         (501) staff       (20)      213 2021-08-31 14:21:01.255367 grokcore.annotation-3.2/setup.cfg
--rw-r--r--   0 jw         (501) staff       (20)     2196 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/setup.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2021-08-31 14:21:01.243223 grokcore.annotation-3.2/src/
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2021-08-31 14:21:01.246850 grokcore.annotation-3.2/src/grokcore/
--rw-r--r--   0 jw         (501) staff       (20)      200 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/__init__.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2021-08-31 14:21:01.251653 grokcore.annotation-3.2/src/grokcore/annotation/
--rw-r--r--   0 jw         (501) staff       (20)     1386 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)     2861 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/components.py
--rw-r--r--   0 jw         (501) staff       (20)      172 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/configure.zcml
--rw-r--r--   0 jw         (501) staff       (20)     1859 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/interfaces.py
--rw-r--r--   0 jw         (501) staff       (20)     4181 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/lazy.py
--rw-r--r--   0 jw         (501) staff       (20)     3073 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/meta.py
--rw-r--r--   0 jw         (501) staff       (20)      291 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/meta.zcml
--rw-r--r--   0 jw         (501) staff       (20)     1071 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/testing.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2021-08-31 14:21:01.252181 grokcore.annotation-3.2/src/grokcore/annotation/tests/
--rw-r--r--   0 jw         (501) staff       (20)       32 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/tests/__init__.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2021-08-31 14:21:01.254381 grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/
--rw-r--r--   0 jw         (501) staff       (20)       20 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/__init__.py
--rw-r--r--   0 jw         (501) staff       (20)     2314 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/annotation.py
--rw-r--r--   0 jw         (501) staff       (20)      815 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/implementsmany.py
--rw-r--r--   0 jw         (501) staff       (20)      561 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/implementsnone.py
--rw-r--r--   0 jw         (501) staff       (20)     5534 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/lazy.py
--rw-r--r--   0 jw         (501) staff       (20)     1600 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/name.py
--rw-r--r--   0 jw         (501) staff       (20)     1055 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/provides.py
--rw-r--r--   0 jw         (501) staff       (20)     1567 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/src/grokcore/annotation/tests/test_grok.py
-drwxr-xr-x   0 jw         (501) staff       (20)        0 2021-08-31 14:21:01.249040 grokcore.annotation-3.2/src/grokcore.annotation.egg-info/
--rw-r--r--   0 jw         (501) staff       (20)     7376 2021-08-31 14:21:01.000000 grokcore.annotation-3.2/src/grokcore.annotation.egg-info/PKG-INFO
--rw-r--r--   0 jw         (501) staff       (20)     1224 2021-08-31 14:21:01.000000 grokcore.annotation-3.2/src/grokcore.annotation.egg-info/SOURCES.txt
--rw-r--r--   0 jw         (501) staff       (20)        1 2021-08-31 14:21:01.000000 grokcore.annotation-3.2/src/grokcore.annotation.egg-info/dependency_links.txt
--rw-r--r--   0 jw         (501) staff       (20)        9 2021-08-31 14:21:01.000000 grokcore.annotation-3.2/src/grokcore.annotation.egg-info/namespace_packages.txt
--rw-r--r--   0 jw         (501) staff       (20)        1 2021-08-31 14:21:01.000000 grokcore.annotation-3.2/src/grokcore.annotation.egg-info/not-zip-safe
--rw-r--r--   0 jw         (501) staff       (20)      238 2021-08-31 14:21:01.000000 grokcore.annotation-3.2/src/grokcore.annotation.egg-info/requires.txt
--rw-r--r--   0 jw         (501) staff       (20)        9 2021-08-31 14:21:01.000000 grokcore.annotation-3.2/src/grokcore.annotation.egg-info/top_level.txt
--rw-r--r--   0 jw         (501) staff       (20)     1220 2021-08-31 14:21:00.000000 grokcore.annotation-3.2/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:41:17.665022 grokcore.annotation-4.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2469 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      225 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5982 2023-07-12 06:41:17.665091 grokcore.annotation-4.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2529 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      486 2023-07-12 06:41:17.665349 grokcore.annotation-4.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1890 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:41:17.659317 grokcore.annotation-4.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:41:17.660963 grokcore.annotation-4.0/src/grokcore/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:41:17.663311 grokcore.annotation-4.0/src/grokcore/annotation/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1463 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2854 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/components.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      172 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/configure.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1859 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4203 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/lazy.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3074 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/meta.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      291 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/meta.zcml
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1036 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/testing.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:41:17.663642 grokcore.annotation-4.0/src/grokcore/annotation/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/tests/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:41:17.664866 grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       20 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2315 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/annotation.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      816 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/implementsmany.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      561 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/implementsnone.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5521 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/lazy.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1601 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/name.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1056 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/provides.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1114 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore/annotation/tests/test_grok.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-12 06:41:17.662041 grokcore.annotation-4.0/src/grokcore.annotation.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5982 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore.annotation.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1210 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore.annotation.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore.annotation.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore.annotation.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore.annotation.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      235 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore.annotation.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/src/grokcore.annotation.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1400 2023-07-12 06:41:17.000000 grokcore.annotation-4.0/tox.ini
```

### Comparing `grokcore.annotation-3.2/CHANGES.rst` & `grokcore.annotation-4.0/CHANGES.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changes
 =======
 
+4.0 (2023-07-12)
+----------------
+
+- Add support for Python 3.10, 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+- Drop support for deprecated ``python setup.py test``.
+
+
 3.2 (2021-08-31)
 ----------------
 
 - ``grokcore.annotation.testing.warn`` was removed as it was not used
   internally. If you still need it, a copy is in ``grokcore.view.testing``.
 
 - Add ``_p_changed`` property to the LazyAnnotation object, proxying it to
```

### Comparing `grokcore.annotation-3.2/LICENSE.txt` & `grokcore.annotation-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grokcore.annotation-3.2/README.rst` & `grokcore.annotation-4.0/README.rst`

 * *Files identical despite different names*

### Comparing `grokcore.annotation-3.2/setup.py` & `grokcore.annotation-4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(name):
     """Read a file."""
     with open(name) as f:
         return f.read()
 
@@ -19,54 +20,50 @@
     'zope.testing > 4.6',
     'zope.testrunner',
 ]
 
 
 setup(
     name='grokcore.annotation',
-    version='3.2',
+    version='4.0',
     author='Grok Team',
-    author_email='grok-dev@zope.org',
-    url='http://grok.zope.org',
-    download_url='http://pypi.python.org/pypi/grokcore.annotation',
+    author_email='zope-dev@zope.dev',
+    url='https://github.com/zopefoundation/grokcore.annotation',
     description='Grok-like configuration for Zope annotations',
     long_description=long_description,
-    license='ZPL',
-    classifiers=['Environment :: Web Environment',
-                 'Intended Audience :: Developers',
-                 'License :: OSI Approved :: Zope Public License',
-                 'Programming Language :: Python',
-                 'Programming Language :: Python :: 2',
-                 'Programming Language :: Python :: 2.7',
-                 'Programming Language :: Python :: 3',
-                 'Programming Language :: Python :: 3.5',
-                 'Programming Language :: Python :: 3.6',
-                 'Programming Language :: Python :: 3.7',
-                 'Programming Language :: Python :: 3.8',
-                 'Programming Language :: Python :: 3.9',
-                 'Programming Language :: Python :: Implementation :: CPython',
-                 'Programming Language :: Python :: Implementation :: PyPy',
-                 'Framework :: Zope :: 3',
-                 ],
-
+    license='ZPL 2.1',
+    classifiers=[
+        'Environment :: Web Environment',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: Zope Public License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy',
+        'Framework :: Zope :: 3',
+    ],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['grokcore'],
     include_package_data=True,
     zip_safe=False,
+    python_requires='>=3.7',
     install_requires=[
-        'grokcore.component >= 2.5dev',
+        'grokcore.component >= 2.5',
         'martian',
         'setuptools',
         'zope.annotation',
         'zope.cachedescriptors',
         'zope.component',
         'zope.container',
         'zope.event',
         'zope.interface',
         'zope.location',
         'zope.schema',
     ],
-    tests_require=tests_require,
-    test_suite='grokcore.annotation.tests.test_grok.test_suite',
     extras_require={'test': tests_require},
 )
```

### Comparing `grokcore.annotation-3.2/src/grokcore/annotation/__init__.py` & `grokcore.annotation-4.0/src/grokcore/annotation/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Grokcore.annotation
 """
 
 from grokcore.component import *
+from zope.interface import moduleProvides
 
-from grokcore.annotation.components import Annotation, Model
-from grokcore.annotation.components import queryAnnotation
+from grokcore.annotation.components import Annotation
+from grokcore.annotation.components import Model
 from grokcore.annotation.components import deleteAnnotation
-
-from grokcore.annotation.lazy import LazyAnnotation, LazyAnnotationProperty
-
+from grokcore.annotation.components import queryAnnotation
+# Our __init__ provides the grok API directly so using 'import grok' is enough.
+from grokcore.annotation.interfaces import IGrokcoreAnnotationAPI
+from grokcore.annotation.lazy import LazyAnnotation
+from grokcore.annotation.lazy import LazyAnnotationProperty
 # BBB These two functions are meant for test fixtures and should be
 # imported from grok.testing, not from grok.
 from grokcore.annotation.testing import grok
 
-# Our __init__ provides the grok API directly so using 'import grok' is enough.
-from grokcore.annotation.interfaces import IGrokcoreAnnotationAPI
-from zope.interface import moduleProvides
+
 moduleProvides(IGrokcoreAnnotationAPI)
 __all__ = list(IGrokcoreAnnotationAPI)
```

### Comparing `grokcore.annotation-3.2/src/grokcore/annotation/components.py` & `grokcore.annotation-4.0/src/grokcore/annotation/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Base classes for Grok application components.
 
 """
 
-from zope.annotation.interfaces import IAttributeAnnotatable
+import grokcore.component
+import persistent
 from zope.annotation.interfaces import IAnnotations
+from zope.annotation.interfaces import IAttributeAnnotatable
+from zope.component import getSiteManager
 from zope.container import contained
 from zope.interface import providedBy
-from zope.component import getSiteManager
+
 from grokcore.annotation.interfaces import IAnnotationFactory
-import persistent
-import grokcore.component
 
 
 @grokcore.component.implementer(IAttributeAnnotatable)
 class Model(grokcore.component.Context):
     """Base class for an object which is able to handle annotations
     """
 
@@ -35,15 +36,15 @@
     """The base class for annotation classes in Grok applications.
 
     Inherits from the :class:`persistent.Persistent` class.
     """
 
 
 @grokcore.component.implementer(IAnnotationFactory)
-class AnnotationFactory(object):
+class AnnotationFactory:
 
     def __init__(self, factory, name):
         self.factory = factory
         self.name = name
 
     def query(self, context):
         """Return None if the annotation doesn't exists.
```

### Comparing `grokcore.annotation-3.2/src/grokcore/annotation/interfaces.py` & `grokcore.annotation-4.0/src/grokcore/annotation/interfaces.py`

 * *Files identical despite different names*

### Comparing `grokcore.annotation-3.2/src/grokcore/annotation/lazy.py` & `grokcore.annotation-4.0/src/grokcore/annotation/lazy.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 #
 ##############################################################################
 """Base classes for Grok application components.
 
 """
 
 import persistent
-from zope import event
 import zope.annotation.interfaces
 import zope.cachedescriptors.property
-
+from zope import event
+from zope.annotation.interfaces import IAnnotations
 from zope.interface import implementer
 from zope.location import Location
-from zope.schema.fieldproperty import FieldUpdatedEvent, NO_VALUE
-from zope.annotation.interfaces import IAnnotations
+from zope.schema.fieldproperty import NO_VALUE
+from zope.schema.fieldproperty import FieldUpdatedEvent
+
 from grokcore.annotation.interfaces import IAnnotationFactory
 
+
 _marker = object()
 
 
-class LazyAnnotationProperty(object):
+class LazyAnnotationProperty:
 
     def __init__(self, field, name=None):
         if name is None:
             name = field.__name__
 
         self.__field = field
         self.__name = name
@@ -110,15 +112,15 @@
     def _p_changed(self, value):
         storage = self.storage
         if storage is not None:
             storage._p_changed = value
 
 
 @implementer(IAnnotationFactory)
-class LazyAnnotationFactory(object):
+class LazyAnnotationFactory:
 
     def __init__(self, factory, name):
         self.factory = factory
         self.name = name
 
     def query(self, context):
         annotations = IAnnotations(context)
```

### Comparing `grokcore.annotation-3.2/src/grokcore/annotation/meta.py` & `grokcore.annotation-4.0/src/grokcore/annotation/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Grokkers for Grokcore Annotation component.
 """
+import martian
 from martian import util
-from grokcore.annotation.components import AnnotationFactory
-from grokcore.annotation.lazy import LazyAnnotationFactory
 from zope.interface import implementedBy
+
 import grokcore.annotation
-import martian
+from grokcore.annotation.components import AnnotationFactory
+from grokcore.annotation.lazy import LazyAnnotationFactory
 
 
 def default_annotation_provides(factory, module, **data):
     base_interfaces = implementedBy(grokcore.annotation.Annotation)
     factory_interfaces = implementedBy(factory)
     real_interfaces = list(factory_interfaces - base_interfaces)
     util.check_implements_one_from_list(real_interfaces, factory)
```

### Comparing `grokcore.annotation-3.2/src/grokcore/annotation/testing.py` & `grokcore.annotation-4.0/src/grokcore/annotation/testing.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Grok test helpers
 """
-from __future__ import print_function
-from zope.configuration.config import ConfigurationMachine
+
 from grokcore.component import zcml
+from zope.configuration.config import ConfigurationMachine
+
+
 # Provide this import here for BBB reasons:
 
 
 def grok(module_name):
     config = ConfigurationMachine()
     zcml.do_grok('grokcore.component.meta', config)
     zcml.do_grok('grokcore.annotation.meta', config)
```

### Comparing `grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/annotation.py` & `grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,18 @@
 
   >>> grok.deleteAnnotation(manfred, None)
   False
 
 
 """
 
-import grokcore.annotation as grok
-from zope import interface
 from BTrees.OOBTree import OOTreeSet
+from zope import interface
+
+import grokcore.annotation as grok
 
 
 class Mammoth(grok.Model):
     pass
 
 
 class IBranding(interface.Interface):
```

### Comparing `grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/implementsmany.py` & `grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/implementsmany.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
   >>> grok.testing.grok(__name__)
   Traceback (most recent call last):
   ...
   martian.error.GrokError: <class 'grokcore.annotation.tests.annotation.implementsmany.MammothAnnotations'> is implementing more than one interface (use grok.provides to specify which one to use).
 """  # noqa: E501 line too long
 
-import grokcore.annotation as grok
 from zope import interface
 
+import grokcore.annotation as grok
+
 
 class Mammoth(grok.Model):
     pass
 
 
 class IOneInterface(interface.Interface):
     pass
```

### Comparing `grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/implementsnone.py` & `grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/implementsnone.py`

 * *Files identical despite different names*

### Comparing `grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/lazy.py` & `grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/lazy.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,33 +146,33 @@
   >>> event_log[0].inst is lazyannotation
   True
   >>> event_log[0].field.__name__
   'lazy_attribute'
 
 """
 
-import grokcore.annotation as grok
-
 from zope import interface
 from zope import schema
 
+import grokcore.annotation as grok
+
 
 class Mammoth(grok.Model):
     pass
 
 
 class ILazy(interface.Interface):
 
     lazy_attribute = schema.TextLine(
-        title=u'So, so lazy',
-        default=u'lazily waiting for a value.')
+        title='So, so lazy',
+        default='lazily waiting for a value.')
 
     lazy_readonly_attribute = schema.TextLine(
-        title=u'So, so lazy, but readonly',
-        default=u'no writing here',
+        title='So, so lazy, but readonly',
+        default='no writing here',
         readonly=True)
 
 
 @grok.implementer(ILazy)
 class Lazy(grok.LazyAnnotation):
     grok.name('lazy.annotation.custom.name')
     grok.provides(ILazy)
@@ -182,15 +182,15 @@
 
     lazy_readonly_attribute = grok.LazyAnnotationProperty(
         ILazy['lazy_readonly_attribute'])
 
 
 # Fixtures for tests for internal details
 
-class _FauxField(object):
+class _FauxField:
 
     def bind(self, other):
         return self
 
 
 class _IFauxLazy(interface.Interface):
     pass
@@ -201,15 +201,15 @@
     grok.provides(_IFauxLazy)
 
     testing = grok.LazyAnnotationProperty(_FauxField(), 'testing')
 
 
 class IIncorrect(interface.Interface):
 
-    testing = schema.TextLine(title=u'testing')
+    testing = schema.TextLine(title='testing')
 
 
 @grok.implementer(IIncorrect)
 class IncorrectAnnotation(grok.Annotation):
     grok.provides(IIncorrect)
 
     testing = grok.LazyAnnotationProperty(IIncorrect['testing'])
```

### Comparing `grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/name.py` & `grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/name.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,17 +31,18 @@
 And the name is stored in __name__:
 
   >>> ann.__name__
   'mammoth.branding'
 
 """  # noqa: E501 line too long
 
-import grokcore.annotation as grok
 from zope import interface
 
+import grokcore.annotation as grok
+
 
 class Mammoth(grok.Model):
     pass
 
 
 class IExplicitName(interface.Interface):
     pass
```

### Comparing `grokcore.annotation-3.2/src/grokcore/annotation/tests/annotation/provides.py` & `grokcore.annotation-4.0/src/grokcore/annotation/tests/annotation/provides.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 
   >>> IAnotherOne(manfred)
   Traceback (most recent call last):
   TypeError: ('Could not adapt', <grokcore.annotation.tests.annotation.provides.Mammoth object at ...>, <InterfaceClass grokcore.annotation.tests.annotation.provides.IAnotherOne>)
 
 """  # noqa: E501 line too long
 
-import grokcore.annotation as grok
 from zope import interface
 
+import grokcore.annotation as grok
+
 
 class Mammoth(grok.Model):
     pass
 
 
 class IOneInterface(interface.Interface):
     pass
```

### Comparing `grokcore.annotation-3.2/src/grokcore.annotation.egg-info/SOURCES.txt` & `grokcore.annotation-4.0/src/grokcore.annotation.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
-buildout.cfg
-requirements.txt
 setup.cfg
 setup.py
 tox.ini
 src/grokcore/__init__.py
 src/grokcore.annotation.egg-info/PKG-INFO
 src/grokcore.annotation.egg-info/SOURCES.txt
 src/grokcore.annotation.egg-info/dependency_links.txt
```

### Comparing `grokcore.annotation-3.2/tox.ini` & `grokcore.annotation-4.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,67 @@
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
-    pypy
+    py310
+    py311
     pypy3
     coverage
 
 [testenv]
 usedevelop = true
 deps =
-    zope.testrunner
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
     test
 
 [testenv:lint]
 basepython = python3
 skip_install = true
-deps =
-    flake8
-    check-manifest
-    check-python-versions
 commands =
+    isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
     flake8 src setup.py
     check-manifest
     check-python-versions
+deps =
+    check-manifest
+    check-python-versions >= 0.19.1
+    wheel
+    flake8
+    isort
+
+[testenv:isort-apply]
+basepython = python3
+skip_install = true
+commands_pre =
+deps =
+    isort
+commands =
+    isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
-    zope.testrunner
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
-    coverage html
-    coverage report -m --fail-under=94.5
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=94.5
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = grokcore.annotation
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```


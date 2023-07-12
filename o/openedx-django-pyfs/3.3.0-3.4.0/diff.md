# Comparing `tmp/openedx-django-pyfs-3.3.0.tar.gz` & `tmp/openedx-django-pyfs-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-django-pyfs-3.3.0.tar", last modified: Sat Jun  3 12:11:10 2023, max compression
+gzip compressed data, was "openedx-django-pyfs-3.4.0.tar", last modified: Wed Jul 12 10:20:57 2023, max compression
```

## Comparing `openedx-django-pyfs-3.3.0.tar` & `openedx-django-pyfs-3.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.096089 openedx-django-pyfs-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4186 2023-06-03 12:11:10.096089 openedx-django-pyfs-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3476 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.092089 openedx-django-pyfs-3.3.0/djpyfs/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/djpyfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6183 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/djpyfs/djpyfs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/djpyfs/models.py
--rw-r--r--   0 runner    (1001) docker     (122)    13272 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/djpyfs/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.092089 openedx-django-pyfs-3.3.0/example/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.092089 openedx-django-pyfs-3.3.0/example/example/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5481 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/example/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/example/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.096089 openedx-django-pyfs-3.3.0/example/sample/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/sample/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/sample/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/example/sample/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.096089 openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4186 2023-06-03 12:11:10.000000 openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-06-03 12:11:10.000000 openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-03 12:11:10.000000 openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-03 12:11:10.000000 openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-03 12:11:10.000000 openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-03 12:11:10.096089 openedx-django-pyfs-3.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-03 12:11:10.096089 openedx-django-pyfs-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4964 2023-06-03 12:11:05.000000 openedx-django-pyfs-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 10:20:57.562913 openedx-django-pyfs-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4225 2023-07-12 10:20:57.562913 openedx-django-pyfs-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3476 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 10:20:57.558912 openedx-django-pyfs-3.4.0/djpyfs/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/djpyfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6183 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/djpyfs/djpyfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/djpyfs/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13272 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/djpyfs/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 10:20:57.558912 openedx-django-pyfs-3.4.0/example/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 10:20:57.558912 openedx-django-pyfs-3.4.0/example/example/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5481 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/example/example/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/example/example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/example/example/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (122)      250 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/example/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 10:20:57.562913 openedx-django-pyfs-3.4.0/example/sample/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/example/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/example/sample/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/example/sample/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/example/sample/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 10:20:57.562913 openedx-django-pyfs-3.4.0/openedx_django_pyfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4225 2023-07-12 10:20:57.000000 openedx-django-pyfs-3.4.0/openedx_django_pyfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-07-12 10:20:57.000000 openedx-django-pyfs-3.4.0/openedx_django_pyfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 10:20:57.000000 openedx-django-pyfs-3.4.0/openedx_django_pyfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-12 10:20:57.000000 openedx-django-pyfs-3.4.0/openedx_django_pyfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-12 10:20:57.000000 openedx-django-pyfs-3.4.0/openedx_django_pyfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 10:20:57.562913 openedx-django-pyfs-3.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-07-12 10:20:57.562913 openedx-django-pyfs-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5002 2023-07-12 10:20:53.000000 openedx-django-pyfs-3.4.0/setup.py
```

### Comparing `openedx-django-pyfs-3.3.0/LICENSE` & `openedx-django-pyfs-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.3.0/PKG-INFO` & `openedx-django-pyfs-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: openedx-django-pyfs
-Version: 3.3.0
+Version: 3.4.0
 Summary: Django pyfilesystem integration
 Home-page: https://github.com/openedx/django-pyfs
 Author: Open edX
 Author-email: oscm@tcril.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `openedx-django-pyfs-3.3.0/README.rst` & `openedx-django-pyfs-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.3.0/djpyfs/djpyfs.py` & `openedx-django-pyfs-3.4.0/djpyfs/djpyfs.py`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.3.0/djpyfs/models.py` & `openedx-django-pyfs-3.4.0/djpyfs/models.py`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.3.0/djpyfs/tests.py` & `openedx-django-pyfs-3.4.0/djpyfs/tests.py`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.3.0/example/example/settings.py` & `openedx-django-pyfs-3.4.0/example/example/settings.py`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.3.0/example/example/urls.py` & `openedx-django-pyfs-3.4.0/example/example/urls.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from django.conf.urls import patterns, include, url
+from django.urls import path
+from django.conf.urls import patterns
 
 # Uncomment the next two lines to enable the admin:
 # from django.contrib import admin
 # admin.autodiscover()
 
 urlpatterns = patterns('',
     # Examples:
-    url(r'^$', 'sample.views.index', name='index'),
+    path('', 'sample.views.index', name='index'),
     # url(r'^example/', include('example.foo.urls')),
 
     # Uncomment the admin/doc line below to enable admin documentation:
     # url(r'^admin/doc/', include('django.contrib.admindocs.urls')),
 
     # Uncomment the next line to enable the admin:
     # url(r'^admin/', include(admin.site.urls)),
```

### Comparing `openedx-django-pyfs-3.3.0/example/example/wsgi.py` & `openedx-django-pyfs-3.4.0/example/example/wsgi.py`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.3.0/example/sample/views.py` & `openedx-django-pyfs-3.4.0/example/sample/views.py`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/PKG-INFO` & `openedx-django-pyfs-3.4.0/openedx_django_pyfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: openedx-django-pyfs
-Version: 3.3.0
+Version: 3.4.0
 Summary: Django pyfilesystem integration
 Home-page: https://github.com/openedx/django-pyfs
 Author: Open edX
 Author-email: oscm@tcril.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `openedx-django-pyfs-3.3.0/openedx_django_pyfs.egg-info/SOURCES.txt` & `openedx-django-pyfs-3.4.0/openedx_django_pyfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.3.0/requirements/constraints.txt` & `openedx-django-pyfs-3.4.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx-django-pyfs-3.3.0/setup.py` & `openedx-django-pyfs-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     long_description=ld,
     long_description_content_type='text/x-rst',
     classifiers=[
         "Development Status :: 4 - Beta",
         "Framework :: Django",
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: Apache Software License",
     ],
     install_requires=load_requirements('requirements/base.in'),
```


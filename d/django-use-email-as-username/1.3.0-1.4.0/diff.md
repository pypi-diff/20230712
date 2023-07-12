# Comparing `tmp/django_use_email_as_username-1.3.0.tar.gz` & `tmp/django_use_email_as_username-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_use_email_as_username-1.3.0.tar", max compression
+gzip compressed data, was "django_use_email_as_username-1.4.0.tar", last modified: Wed Jul 12 09:58:51 2023, max compression
```

## Comparing `django_use_email_as_username-1.3.0.tar` & `django_use_email_as_username-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,25 @@
--rw-r--r--   0        0        0     1536 2021-07-01 07:01:36.000000 django_use_email_as_username-1.3.0/LICENSE
--rw-r--r--   0        0        0     3309 2021-12-14 22:09:13.000000 django_use_email_as_username-1.3.0/README.rst
--rw-r--r--   0        0        0       22 2023-01-24 10:04:21.031045 django_use_email_as_username-1.3.0/django_use_email_as_username/__init__.py
--rw-r--r--   0        0        0     1080 2021-07-01 07:01:36.000000 django_use_email_as_username-1.3.0/django_use_email_as_username/admin.py
--rw-r--r--   0        0        0      236 2021-07-01 07:01:36.000000 django_use_email_as_username-1.3.0/django_use_email_as_username/apps.py
--rwxr-xr-x   0        0        0        0 2021-07-01 07:01:36.000000 django_use_email_as_username-1.3.0/django_use_email_as_username/management/commands/app_template/__init__.py-tpl
--rwxr-xr-x   0        0        0      162 2021-07-01 07:01:36.000000 django_use_email_as_username-1.3.0/django_use_email_as_username/management/commands/app_template/admin.py-tpl
--rwxr-xr-x   0        0        0      158 2021-07-01 07:01:36.000000 django_use_email_as_username-1.3.0/django_use_email_as_username/management/commands/app_template/apps.py-tpl
--rw-r--r--   0        0        0        0 2021-07-01 07:01:36.000000 django_use_email_as_username-1.3.0/django_use_email_as_username/management/commands/app_template/migrations/__init__.py-tpl
--rwxr-xr-x   0        0        0      130 2021-07-01 07:01:36.000000 django_use_email_as_username-1.3.0/django_use_email_as_username/management/commands/app_template/models.py-tpl
--rw-r--r--   0        0        0     1210 2023-01-24 09:37:54.329059 django_use_email_as_username-1.3.0/django_use_email_as_username/management/commands/create_custom_user_app.py
--rw-r--r--   0        0        0     1995 2021-07-01 07:01:36.000000 django_use_email_as_username-1.3.0/django_use_email_as_username/models.py
--rw-r--r--   0        0        0     1390 2023-01-24 09:59:49.298786 django_use_email_as_username-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4499 1970-01-01 00:00:00.000000 django_use_email_as_username-1.3.0/setup.py
--rw-r--r--   0        0        0     4944 1970-01-01 00:00:00.000000 django_use_email_as_username-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      178 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1536 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3345 2023-07-12 09:07:03.813358 django_use_email_as_username-1.4.0/README.rst
+-rw-r--r--   0        0        0       22 2023-07-12 09:47:48.145493 django_use_email_as_username-1.4.0/django_use_email_as_username/__init__.py
+-rw-r--r--   0        0        0     1080 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/django_use_email_as_username/admin.py
+-rw-r--r--   0        0        0      236 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/django_use_email_as_username/apps.py
+-rwxr-xr-x   0        0        0        0 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/django_use_email_as_username/management/commands/app_template/__init__.py-tpl
+-rwxr-xr-x   0        0        0      162 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/django_use_email_as_username/management/commands/app_template/admin.py-tpl
+-rwxr-xr-x   0        0        0      158 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/django_use_email_as_username/management/commands/app_template/apps.py-tpl
+-rw-r--r--   0        0        0        0 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/django_use_email_as_username/management/commands/app_template/migrations/__init__.py-tpl
+-rwxr-xr-x   0        0        0      130 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/django_use_email_as_username/management/commands/app_template/models.py-tpl
+-rw-r--r--   0        0        0     1210 2023-01-24 09:37:54.000000 django_use_email_as_username-1.4.0/django_use_email_as_username/management/commands/create_custom_user_app.py
+-rw-r--r--   0        0        0     1995 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/django_use_email_as_username/models.py
+-rw-r--r--   0        0        0     2272 2023-07-12 09:58:51.563631 django_use_email_as_username-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/tests/__init__.py
+-rwxr-xr-x   0        0        0        0 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/tests/apps/custom_user_test/__init__.py
+-rwxr-xr-x   0        0        0      162 2021-07-01 07:42:29.000000 django_use_email_as_username-1.4.0/tests/apps/custom_user_test/admin.py
+-rwxr-xr-x   0        0        0      149 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/tests/apps/custom_user_test/apps.py
+-rw-r--r--   0        0        0     2435 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/tests/apps/custom_user_test/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/tests/apps/custom_user_test/migrations/__init__.py
+-rwxr-xr-x   0        0        0      130 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/tests/apps/custom_user_test/models.py
+-rw-r--r--   0        0        0     1289 2021-12-14 22:09:24.000000 django_use_email_as_username-1.4.0/tests/settings.py
+-rw-r--r--   0        0        0    11903 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/tests/test.py
+-rw-r--r--   0        0        0       49 2021-07-01 07:01:36.000000 django_use_email_as_username-1.4.0/tests/urls.py
+-rw-r--r--   0        0        0     4430 1970-01-01 00:00:00.000000 django_use_email_as_username-1.4.0/PKG-INFO
```

### Comparing `django_use_email_as_username-1.3.0/LICENSE` & `django_use_email_as_username-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_use_email_as_username-1.3.0/README.rst` & `django_use_email_as_username-1.4.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ============================
 Django use Email as Username
 ============================
 
 .. image:: https://badge.fury.io/py/django-use-email-as-username.svg
     :target: https://badge.fury.io/py/django-use-email-as-username
 
-.. image:: https://app.travis-ci.com/jmfederico/django-use-email-as-username.svg?branch=main
-    :target: https://app.travis-ci.com/jmfederico/django-use-email-as-username
+.. image:: https://github.com/jmfederico/django-use-email-as-username/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/jmfederico/django-use-email-as-username/actions/workflows/tests.yml
 
 .. image:: https://codecov.io/gh/jmfederico/django-use-email-as-username/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/jmfederico/django-use-email-as-username
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/ambv/black
```

### Comparing `django_use_email_as_username-1.3.0/django_use_email_as_username/admin.py` & `django_use_email_as_username-1.4.0/django_use_email_as_username/admin.py`

 * *Files identical despite different names*

### Comparing `django_use_email_as_username-1.3.0/django_use_email_as_username/management/commands/create_custom_user_app.py` & `django_use_email_as_username-1.4.0/django_use_email_as_username/management/commands/create_custom_user_app.py`

 * *Files identical despite different names*

### Comparing `django_use_email_as_username-1.3.0/django_use_email_as_username/models.py` & `django_use_email_as_username-1.4.0/django_use_email_as_username/models.py`

 * *Files identical despite different names*

### Comparing `django_use_email_as_username-1.3.0/PKG-INFO` & `django_use_email_as_username-1.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,44 @@
 Metadata-Version: 2.1
 Name: django-use-email-as-username
-Version: 1.3.0
+Version: 1.4.0
 Summary: A Django app to use email as username for user authentication.
-Home-page: https://github.com/jmfederico/django-use-email-as-username
+Keywords: django email auth username
+Author-Email: Federico Jaramillo Martínez <federicojaramillom@gmail.com>
 License: BSD-3-Clause
-Keywords: django,email,auth,username
-Author: Federico Jaramillo Martínez
-Author-email: federicojaramillom@gmail.com
-Requires-Python: >=3.5
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: testing
-Requires-Dist: codecov (>=2.0.15); extra == "testing"
-Requires-Dist: coverage (>=4.0); extra == "testing"
-Requires-Dist: django (>=1.11)
 Project-URL: Repository, https://github.com/jmfederico/django-use-email-as-username
+Requires-Python: >=3.7
+Requires-Dist: django>=1.11
+Requires-Dist: codecov; extra == "testing"
+Requires-Dist: coverage; extra == "testing"
+Provides-Extra: testing
 Description-Content-Type: text/x-rst
 
 ============================
 Django use Email as Username
 ============================
 
 .. image:: https://badge.fury.io/py/django-use-email-as-username.svg
     :target: https://badge.fury.io/py/django-use-email-as-username
 
-.. image:: https://app.travis-ci.com/jmfederico/django-use-email-as-username.svg?branch=main
-    :target: https://app.travis-ci.com/jmfederico/django-use-email-as-username
+.. image:: https://github.com/jmfederico/django-use-email-as-username/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/jmfederico/django-use-email-as-username/actions/workflows/tests.yml
 
 .. image:: https://codecov.io/gh/jmfederico/django-use-email-as-username/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/jmfederico/django-use-email-as-username
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/ambv/black
 
@@ -149,8 +138,7 @@
 
 *  Cookiecutter_
 *  `Cookiecutter Django Package`_ by jmfederico_
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`Cookiecutter Django Package`: https://github.com/jmfederico/cookiecutter-djangopackage
 .. _jmfederico: https://github.com/jmfederico
-
```


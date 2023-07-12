# Comparing `tmp/django-timeline-logger-2.1.0.tar.gz` & `tmp/django-timeline-logger-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-timeline-logger-2.1.0.tar", last modified: Wed Apr 13 08:00:24 2022, max compression
+gzip compressed data, was "django-timeline-logger-3.0.0.tar", last modified: Wed Jul 12 09:34:32 2023, max compression
```

## Comparing `django-timeline-logger-2.1.0.tar` & `django-timeline-logger-3.0.0.tar`

### file list

```diff
@@ -1,53 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:24.811571 django-timeline-logger-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-04-13 08:00:24.811571 django-timeline-logger-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:24.807571 django-timeline-logger-2.1.0/django_timeline_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-04-13 08:00:24.000000 django-timeline-logger-2.1.0/django_timeline_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2022-04-13 08:00:24.000000 django-timeline-logger-2.1.0/django_timeline_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-13 08:00:24.000000 django-timeline-logger-2.1.0/django_timeline_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-13 08:00:24.000000 django-timeline-logger-2.1.0/django_timeline_logger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-04-13 08:00:24.000000 django-timeline-logger-2.1.0/django_timeline_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-13 08:00:24.000000 django-timeline-logger-2.1.0/django_timeline_logger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2358 2022-04-13 08:00:24.811571 django-timeline-logger-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:24.807571 django-timeline-logger-2.1.0/timeline_logger/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:24.803571 django-timeline-logger-2.1.0/timeline_logger/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:24.803571 django-timeline-logger-2.1.0/timeline_logger/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:24.807571 django-timeline-logger-2.1.0/timeline_logger/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)     2965 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:24.807571 django-timeline-logger-2.1.0/timeline_logger/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:24.807571 django-timeline-logger-2.1.0/timeline_logger/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3640 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/management/commands/report_mailing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:24.807571 django-timeline-logger-2.1.0/timeline_logger/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/migrations/0002_auto_20160624_1045.py
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/migrations/0003_auto_20171025_1414.py
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/migrations/0004_alter_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/migrations/0005_auto_20220413_0742.py
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/migrations/0006_auto_20220413_0749.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:24.803571 django-timeline-logger-2.1.0/timeline_logger/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:24.811571 django-timeline-logger-2.1.0/timeline_logger/templates/timeline_logger/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/templates/timeline_logger/base.html
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/templates/timeline_logger/created.txt
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/templates/timeline_logger/default.txt
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/templates/timeline_logger/notifications.html
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/templates/timeline_logger/timelinelog_list.html
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/templates/timeline_logger/updated.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:24.811571 django-timeline-logger-2.1.0/timeline_logger/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/templatetags/timeline.py
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-04-13 08:00:20.000000 django-timeline-logger-2.1.0/timeline_logger/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:32.556850 django-timeline-logger-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-12 09:34:32.556850 django-timeline-logger-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:32.552850 django-timeline-logger-3.0.0/django_timeline_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-12 09:34:32.000000 django-timeline-logger-3.0.0/django_timeline_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-12 09:34:32.000000 django-timeline-logger-3.0.0/django_timeline_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:34:32.000000 django-timeline-logger-3.0.0/django_timeline_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 09:34:32.000000 django-timeline-logger-3.0.0/django_timeline_logger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-12 09:34:32.000000 django-timeline-logger-3.0.0/django_timeline_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 09:34:32.000000 django-timeline-logger-3.0.0/django_timeline_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-12 09:34:32.556850 django-timeline-logger-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:32.552850 django-timeline-logger-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/tests/test_management_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:32.552850 django-timeline-logger-3.0.0/timeline_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:32.548850 django-timeline-logger-3.0.0/timeline_logger/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:32.548850 django-timeline-logger-3.0.0/timeline_logger/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:32.552850 django-timeline-logger-3.0.0/timeline_logger/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:32.552850 django-timeline-logger-3.0.0/timeline_logger/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:32.552850 django-timeline-logger-3.0.0/timeline_logger/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/management/commands/report_mailing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:32.556850 django-timeline-logger-3.0.0/timeline_logger/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/migrations/0002_auto_20160624_1045.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/migrations/0003_auto_20171025_1414.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/migrations/0004_alter_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/migrations/0005_auto_20220413_0742.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/migrations/0006_auto_20220413_0749.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:32.548850 django-timeline-logger-3.0.0/timeline_logger/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:32.556850 django-timeline-logger-3.0.0/timeline_logger/templates/timeline_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/templates/timeline_logger/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/templates/timeline_logger/created.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/templates/timeline_logger/default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/templates/timeline_logger/notifications.html
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/templates/timeline_logger/timelinelog_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/templates/timeline_logger/updated.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:32.556850 django-timeline-logger-3.0.0/timeline_logger/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/templatetags/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-12 09:34:25.000000 django-timeline-logger-3.0.0/timeline_logger/views.py
```

### Comparing `django-timeline-logger-2.1.0/LICENSE` & `django-timeline-logger-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-timeline-logger-2.1.0/PKG-INFO` & `django-timeline-logger-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: django-timeline-logger
-Version: 2.1.0
+Version: 3.0.0
 Summary: Generic event logger for Django models.
 Home-page: https://github.com/maykinmedia/django-timeline-logger
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Project-URL: Documentation, http://django-timeline-logger.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/maykinmedia/django-timeline-logger/blob/master/docs/changelog.rst
 Project-URL: Bug Tracker, https://github.com/maykinmedia/django-timeline-logger/issues
 Project-URL: Source Code, https://github.com/maykinmedia/django-timeline-logger
 Keywords: django,generic logging
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: tests
 Provides-Extra: pep8
 Provides-Extra: coverage
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
@@ -41,15 +41,15 @@
 |build-status| |code-quality| |coverage| |black|
 
 |python-versions| |django-versions| |pypi-version|
 
 Prerequisites
 =============
 
-This project uses ``django.contrib.postgres.JSONField``, and as such, you need:
+This project uses ``django.db.models.JSONField``, and as such, you need:
 
 * at least Django 3.2+
 * a database supporting ``django.db.models.JSONField``
 * A modern setuptools version
 
 
 Installation
@@ -113,9 +113,7 @@
 
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/django-timeline-logger.svg
 
 .. |django-versions| image:: https://img.shields.io/pypi/djversions/django-timeline-logger.svg
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/django-timeline-logger.svg
     :target: https://pypi.org/project/django-timeline-logger/
-
-
```

### Comparing `django-timeline-logger-2.1.0/README.rst` & `django-timeline-logger-3.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 |build-status| |code-quality| |coverage| |black|
 
 |python-versions| |django-versions| |pypi-version|
 
 Prerequisites
 =============
 
-This project uses ``django.contrib.postgres.JSONField``, and as such, you need:
+This project uses ``django.db.models.JSONField``, and as such, you need:
 
 * at least Django 3.2+
 * a database supporting ``django.db.models.JSONField``
 * A modern setuptools version
 
 
 Installation
```

### Comparing `django-timeline-logger-2.1.0/django_timeline_logger.egg-info/PKG-INFO` & `django-timeline-logger-3.0.0/django_timeline_logger.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: django-timeline-logger
-Version: 2.1.0
+Version: 3.0.0
 Summary: Generic event logger for Django models.
 Home-page: https://github.com/maykinmedia/django-timeline-logger
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Project-URL: Documentation, http://django-timeline-logger.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/maykinmedia/django-timeline-logger/blob/master/docs/changelog.rst
 Project-URL: Bug Tracker, https://github.com/maykinmedia/django-timeline-logger/issues
 Project-URL: Source Code, https://github.com/maykinmedia/django-timeline-logger
 Keywords: django,generic logging
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: tests
 Provides-Extra: pep8
 Provides-Extra: coverage
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
@@ -41,15 +41,15 @@
 |build-status| |code-quality| |coverage| |black|
 
 |python-versions| |django-versions| |pypi-version|
 
 Prerequisites
 =============
 
-This project uses ``django.contrib.postgres.JSONField``, and as such, you need:
+This project uses ``django.db.models.JSONField``, and as such, you need:
 
 * at least Django 3.2+
 * a database supporting ``django.db.models.JSONField``
 * A modern setuptools version
 
 
 Installation
@@ -113,9 +113,7 @@
 
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/django-timeline-logger.svg
 
 .. |django-versions| image:: https://img.shields.io/pypi/djversions/django-timeline-logger.svg
 
 .. |pypi-version| image:: https://img.shields.io/pypi/v/django-timeline-logger.svg
     :target: https://pypi.org/project/django-timeline-logger/
-
-
```

### Comparing `django-timeline-logger-2.1.0/django_timeline_logger.egg-info/SOURCES.txt` & `django-timeline-logger-3.0.0/django_timeline_logger.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 setup.py
 django_timeline_logger.egg-info/PKG-INFO
 django_timeline_logger.egg-info/SOURCES.txt
 django_timeline_logger.egg-info/dependency_links.txt
 django_timeline_logger.egg-info/not-zip-safe
 django_timeline_logger.egg-info/requires.txt
 django_timeline_logger.egg-info/top_level.txt
+tests/test_management_commands.py
+tests/test_models.py
+tests/test_templatetags.py
+tests/test_urls.py
+tests/test_views.py
 timeline_logger/__init__.py
 timeline_logger/admin.py
 timeline_logger/apps.py
 timeline_logger/compat.py
 timeline_logger/conf.py
 timeline_logger/models.py
 timeline_logger/resources.py
```

### Comparing `django-timeline-logger-2.1.0/setup.cfg` & `django-timeline-logger-3.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-timeline-logger
-version = 2.1.0
+version = 3.0.0
 description = Generic event logger for Django models.
 long_description = file: README.rst
 url = https://github.com/maykinmedia/django-timeline-logger
 project_urls = 
 	Documentation = http://django-timeline-logger.readthedocs.io/en/latest/
 	Changelog = https://github.com/maykinmedia/django-timeline-logger/blob/master/docs/changelog.rst
 	Bug Tracker = https://github.com/maykinmedia/django-timeline-logger/issues
@@ -13,23 +13,24 @@
 author = Maykin Media
 author_email = support@maykinmedia.nl
 keywords = django, generic logging
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
+	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	Operating System :: Unix
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires =
```

### Comparing `django-timeline-logger-2.1.0/timeline_logger/conf.py` & `django-timeline-logger-3.0.0/timeline_logger/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from django.conf import settings  # noqa
 from django.utils.translation import gettext_lazy as _
 
 from appconf import AppConf
 
 
 class TimelineLoggerConf(AppConf):
-
     DEFAULT_TEMPLATE = "timeline_logger/default.txt"
 
     PAGINATE_BY = 25
 
     USER_EMAIL_FIELD = "email"
 
     DIGEST_EMAIL_RECIPIENTS = None
```

### Comparing `django-timeline-logger-2.1.0/timeline_logger/locale/nl/LC_MESSAGES/django.mo` & `django-timeline-logger-3.0.0/timeline_logger/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-timeline-logger-2.1.0/timeline_logger/locale/nl/LC_MESSAGES/django.po` & `django-timeline-logger-3.0.0/timeline_logger/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-timeline-logger-2.1.0/timeline_logger/management/commands/report_mailing.py` & `django-timeline-logger-3.0.0/timeline_logger/management/commands/report_mailing.py`

 * *Files identical despite different names*

### Comparing `django-timeline-logger-2.1.0/timeline_logger/migrations/0001_initial.py` & `django-timeline-logger-3.0.0/timeline_logger/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import django.contrib.postgres.fields.jsonb
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("contenttypes", "0002_remove_content_type_name"),
     ]
```

### Comparing `django-timeline-logger-2.1.0/timeline_logger/migrations/0002_auto_20160624_1045.py` & `django-timeline-logger-3.0.0/timeline_logger/migrations/0002_auto_20160624_1045.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Generated by Django 1.9.4 on 2016-06-24 10:45
 from __future__ import unicode_literals
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("timeline_logger", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
             name="timelinelog",
```

### Comparing `django-timeline-logger-2.1.0/timeline_logger/migrations/0003_auto_20171025_1414.py` & `django-timeline-logger-3.0.0/timeline_logger/migrations/0003_auto_20171025_1414.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("timeline_logger", "0002_auto_20160624_1045"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="timelinelog",
```

### Comparing `django-timeline-logger-2.1.0/timeline_logger/migrations/0004_alter_fields.py` & `django-timeline-logger-3.0.0/timeline_logger/migrations/0004_alter_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import django.contrib.postgres.fields.jsonb
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("timeline_logger", "0003_auto_20171025_1414"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="timelinelog",
```

### Comparing `django-timeline-logger-2.1.0/timeline_logger/migrations/0005_auto_20220413_0742.py` & `django-timeline-logger-3.0.0/timeline_logger/migrations/0005_auto_20220413_0742.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.12 on 2022-04-13 07:42
 
 import django.core.serializers.json
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("timeline_logger", "0004_alter_fields"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="timelinelog",
```

### Comparing `django-timeline-logger-2.1.0/timeline_logger/migrations/0006_auto_20220413_0749.py` & `django-timeline-logger-3.0.0/timeline_logger/migrations/0006_auto_20220413_0749.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.12 on 2022-04-13 07:49
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("timeline_logger", "0005_auto_20220413_0742"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="timelinelog",
```

### Comparing `django-timeline-logger-2.1.0/timeline_logger/models.py` & `django-timeline-logger-3.0.0/timeline_logger/models.py`

 * *Files identical despite different names*

### Comparing `django-timeline-logger-2.1.0/timeline_logger/templates/timeline_logger/notifications.html` & `django-timeline-logger-3.0.0/timeline_logger/templates/timeline_logger/notifications.html`

 * *Files identical despite different names*


# Comparing `tmp/django-toosimple-q-1.0.0b3.tar.gz` & `tmp/django-toosimple-q-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-toosimple-q-1.0.0b3.tar", last modified: Thu Oct 27 22:37:20 2022, max compression
+gzip compressed data, was "dist/django-toosimple-q-1.0.0b4.tar", last modified: Wed Jul 12 21:37:06 2023, max compression
```

## Comparing `django-toosimple-q-1.0.0b3.tar` & `django-toosimple-q-1.0.0b4.tar`

### file list

```diff
@@ -1,67 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15647 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11952 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6483 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/contrib/mail/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/contrib/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/contrib/mail/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/contrib/mail/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     4743 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/contrib/mail/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7453 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/management/commands/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3888 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0002_auto_20191101_1838.py
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0003_task_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0004_auto_20200507_1339.py
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0005_auto_20210302_1748.py
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0006_task_replacement.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0007_schedule_datetime_kwarg.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0008_auto_20210902_2111.py
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0009_auto_20210902_2245.py
--rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0010_auto_20220324_0419.py
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0011_workerstatus.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6006 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     3351 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)     5191 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/task.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/templates/toosimpleq/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/templates/toosimpleq/schedule.html
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/templates/toosimpleq/task.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6065 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/concurrency/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/concurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/concurrency/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/concurrency/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2409 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/tests_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3173 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/tests_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (121)     9711 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/tests_schedules.py
--rw-r--r--   0 runner    (1001) docker     (121)    26230 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/tests_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/tests_worker.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/django_toosimple_q/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15647 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/django_toosimple_q.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-27 22:37:20.000000 django-toosimple-q-1.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-10-27 22:37:13.000000 django-toosimple-q-1.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-12 21:37:05.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/mail/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/mail/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/mail/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/management/commands/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0002_auto_20191101_1838.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0003_task_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0004_auto_20200507_1339.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0005_auto_20210302_1748.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0006_task_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0007_schedule_datetime_kwarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0008_auto_20210902_2111.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0009_auto_20210902_2245.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0010_auto_20220324_0419.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0011_workerstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0012_rename_last_run_scheduleexec_last_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0013_workerstatus_exit_code_workerstatus_exit_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/templates/toosimpleq/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/templates/toosimpleq/schedule.html
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/templates/toosimpleq/task.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/concurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/concurrency/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/demo/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/settings_bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/settings_bg_lag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26230 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/django_toosimple_q/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 21:37:06.000000 django-toosimple-q-1.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-12 21:36:51.000000 django-toosimple-q-1.0.0b4/setup.py
```

### Comparing `django-toosimple-q-1.0.0b3/PKG-INFO` & `django-toosimple-q-1.0.0b4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-toosimple-q
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: A simplistic task queue and cron-like scheduler for Django
 Home-page: https://github.com/olivierdalang/django-toosimple-q
 Author: Olivier Dalang
 Author-email: olivier.dalang@gmail.com
 License: MIT
 Description: # Django Too Simple Queue
         
@@ -17,16 +17,18 @@
         Features :
         
         - no celery/redis/rabbitmq/whatever... just Django !
         - clean decorator syntax to register tasks and schedules
         - simple queuing syntax
         - cron-like scheduling
         - tasks.py autodiscovery
+        - supports autoreload
         - django admin integration
         - tasks results stored using the Django ORM
+        - replacement tasks on interruption
         
         Limitations :
         
         - no multithreading yet (but running multiple workers should work)
         - not well suited for projects spawning a high volume of tasks
         
         Compatibility:
@@ -67,15 +69,15 @@
         my_task.queue("Peter")
         ```
         
         Registered tasks can be scheduled from code using this cron-like syntax :
         ```python
         from django_toosimple_q.decorators import register_task, schedule_task
         
-        # Register and schedule tasks
+        # Register and schedule tasks (each morning at 8:30)
         @schedule_task(cron="30 8 * * *", args=['John'])
         @register_task()
         def morning_routine(name):
             return f"Good morning {name} !"
         ```
         
         To consume the tasks, you need to run at least one worker :
@@ -190,15 +192,15 @@
         @schedule_task(name="afternoon_routine", cron="30 16 * * *", args=['afternoon'])
         @schedule_task(name="morning_routine", cron="30 8 * * *", args=['morning'])
         @register_task()
         def my_task(time_of_day):
             return f"Good {time_of_day} John !"
         ```
         
-        By default, `last_tick` is set to `now()` on schedule creation. This means they will only run on next cron occurence. If you need your schedules to be run as soon as possible after initialisation, you can specify `run_on_creation=True`.
+        By default, `last_run` is set to `now()` on schedule creation. This means they will only run on next cron occurence. If you need your schedules to be run as soon as possible after initialisation, you can specify `run_on_creation=True`.
         
         ```python
         @schedule_task(cron="30 8 * * *", run_on_creation=True)
         @register_task()
         def my_task():
             ...
         ```
@@ -208,21 +210,24 @@
         ```python
         @schedule_task(cron="30 8 * * *", catch_up=True)
         @register_task()
         def my_task():
             ...
         ```
         
-        You may get the schedule's cron datetime provided as a keyword argument to the task using the `datetime_kwarg` argument. This is often useful in combination with catch_up, for things like report generation.
+        You may get the schedule's cron datetime provided as a keyword argument to the task using the `datetime_kwarg` argument. This is often useful in combination with catch_up, for things like report generation. Remember to treat the case where the argument is `None` (which happens when the task is run outside of the schedule).
         
         ```python
         @schedule_task(cron="30 8 * * *", datetime_kwarg="scheduled_on", catch_up=True)
         @register_task()
         def my_task(scheduled_on):
-            return f"This was scheduled for {scheduled_on.isoformat()}."
+            if scheduled_on:
+                return f"This was scheduled for {scheduled_on.isoformat()}."
+            else:
+                return "This was not scheduled."
         ```
         
         Similarly to tasks, you can assign schedules to specific queues, and then have your worker only consume tasks from specific queues using `--queue myqueue` or `--exclude_queue myqueue`.
         
         ```python
         @schedule_task(cron="30 8 * * *", queue='scheduler')
         @register_task(queue='worker')
@@ -230,24 +235,36 @@
             ...
         
         # Then run those with these workers
         # manage.py worker --queue scheduler
         # manage.py worker --queue worker
         ```
         
+        Schedule's cron support a non-standard sixth argument for seconds  :
+        ```python
+        from django_toosimple_q.decorators import register_task, schedule_task
+        
+        # A schedule running every 15 seconds
+        @schedule_task(cron="* * * * * */15")
+        @register_task()
+        def morning_routine():
+            return f"15 seconds passed !"
+        ```
+        
         ### Management comment
         
         Besides standard django management commands arguments, the management command supports following arguments.
         
         ```
         usage: manage.py worker [--queue QUEUE | --exclude_queue EXCLUDE_QUEUE]
                                 [--tick TICK]
                                 [--once | --until_done]
                                 [--label LABEL]
                                 [--timeout TIMEOUT]
+                                [--reload {always,never}]
         
         optional arguments:
           --queue QUEUE         which queue to run (can be used several times, all
                                 queues are run if not provided)
           --exclude_queue EXCLUDE_QUEUE
                                 which queue not to run (can be used several times, all
                                 queues are run if not provided)
@@ -257,29 +274,18 @@
           --until_done          run until no tasks are available then exit (useful for
                                 debugging)
           --label LABEL         the name of the worker to help identifying it ('{pid}'
                                 will be replaced by the process id)
           --timeout TIMEOUT     the time in seconds after which this worker will be considered
                                 offline (set this to a value higher than the longest tasks this
                                 worker will execute)
+          --reload {always,never}
+                                watch for changes (by default, watches if DEBUG=True)
         ```
         
-        ## Demo project
-        
-        A demo project with pre-configured tasks is provided.
-        
-        ```shell
-        python demoproject/manage.py migrate
-        python demoproject/manage.py createsuperuser
-        python demoproject/manage.py runserver
-        python demoproject/manage.py worker  # from a different shell
-        ```
-        
-        Then open http://127.0.0.1:8000/admin in your browser
-        
         ## Contrib apps
         
         ### django_toosimple_q.contrib.mail
         
         A queued email backend to send emails asynchronously, preventing your website from failing completely in case the upstream backend is down.
         
         Enable and configure the app in `settings.py` :
@@ -296,33 +302,49 @@
         TOOSIMPLEQ_EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
         ```
         
         Head to the [Django documentation](https://docs.djangoproject.com/en/4.0/topics/email/) for usage.
         
         ## Dev
         
-        ### Tests
-        
-        To run tests locally (by default, tests runs against an in-memory sqlite database):
+        ### Automated tests
         
+        To run tests, we recommend using Docker :
         ```shell
-        pip install -r requirements-dev.txt
-        python manage.py test
+        docker compose build
+        # run all tests
+        docker compose run django test
+        # or to run just a specific test
+        docker compose run django test django_toosimple_q.tests.tests_worker.TestAutoreloadingWorker
         ```
         
-        To run tests against postgres, run the following commands before :
+        Tests are run automatically on github.
+        
+        ### Manual testing
+        
+        Manual testing can be done like this:
+        
         ```shell
-        # Start a local postgres database
-        docker run -p 5432:5432 -e POSTGRES_PASSWORD=postgres -d postgres
-        # Set and env var
-        export TOOSIMPLEQ_TEST_DB=postgres # on Windows: `$Env:TOOSIMPLEQ_TEST_DB = "postgres"`
+        # start a dev server and a worker
+        docker compose build
+        docker compose run django migrate
+        docker compose run django createsuperuser
+        docker compose up
         ```
         
-        Tests are run automatically on github.
+        Then connect on 127.0.0.1:8000/admin/
         
+        ### Without docker
+        
+        To run tests locally without Docker (by default, tests runs against an in-memory sqlite database):
+        
+        ```shell
+        pip install -r requirements-dev.txt
+        python manage.py test
+        ```
         
         ### Contribute
         
         Code style is done with pre-commit :
         ```shell
         pip install -r requirements-dev.txt
         pre-commit install
@@ -343,29 +365,33 @@
         **Registry**: a dictionary keeping all registered schedules and tasks.
         
         **Worker**: a management command that executes schedules and tasks on a regular basis.
         
         
         ## Changelog
         
-        - 2022-10-28 : v1.0.0b **⚠ BACKWARDS INCOMPATIBLE RELEASE ⚠**
+        - 2023-01-09 : v1.0.0b **⚠ BACKWARDS INCOMPATIBLE RELEASE ⚠**
+          - known issues:
+            - [ ] worker exit status not correctly set with autoreload
           - feature: added workerstatus to the admin, allowing to monitor workers
           - feature: queue tasks for later (`mytask.queue(due=now()+timedelta(hours=2))`)
           - feature: assign queues to schedules (`@schedule_task(queue="schedules")`)
+          - feature: auto-reload when DEBUG is true
           - refactor: removed non-execution related data from the database (clarifying the fact tha the source of truth is the registry)
           - refactor: better support for concurrent workers
           - refactor: better names for models and decorators
           - infra: included a demo project
           - infra: improved testing, including for concurrency behaviour
           - infra: updated compatibility to Django 3.2/4.1 and Python 3.8-3.10
           - quick migration guide:
             - rename `@schedule` -> `@schedule_task`
             - task name must now be provided as a kwarg: `@register_task("mytask")` -> `@register_task(name="mytask")`)
             - replace `@schedule_task(..., last_check=None)` -> `@schedule_task(..., run_on_creation=True)`
             - models: `Schedule` -> `ScheduleExec` and `Task` -> `TaskExec`
+            - renamed `ScheduleExec.last_run` to `ScheduleExec.last_task`
         
         - 2022-03-24 : v0.4.0
           - made `last_check` and `last_run` optional in the admin
           - defined `id` fields
         
         - 2021-07-15 : v0.3.0
           - added `contrib.mail`
```

### Comparing `django-toosimple-q-1.0.0b3/README.md` & `django-toosimple-q-1.0.0b4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 Features :
 
 - no celery/redis/rabbitmq/whatever... just Django !
 - clean decorator syntax to register tasks and schedules
 - simple queuing syntax
 - cron-like scheduling
 - tasks.py autodiscovery
+- supports autoreload
 - django admin integration
 - tasks results stored using the Django ORM
+- replacement tasks on interruption
 
 Limitations :
 
 - no multithreading yet (but running multiple workers should work)
 - not well suited for projects spawning a high volume of tasks
 
 Compatibility:
@@ -59,15 +61,15 @@
 my_task.queue("Peter")
 ```
 
 Registered tasks can be scheduled from code using this cron-like syntax :
 ```python
 from django_toosimple_q.decorators import register_task, schedule_task
 
-# Register and schedule tasks
+# Register and schedule tasks (each morning at 8:30)
 @schedule_task(cron="30 8 * * *", args=['John'])
 @register_task()
 def morning_routine(name):
     return f"Good morning {name} !"
 ```
 
 To consume the tasks, you need to run at least one worker :
@@ -182,15 +184,15 @@
 @schedule_task(name="afternoon_routine", cron="30 16 * * *", args=['afternoon'])
 @schedule_task(name="morning_routine", cron="30 8 * * *", args=['morning'])
 @register_task()
 def my_task(time_of_day):
     return f"Good {time_of_day} John !"
 ```
 
-By default, `last_tick` is set to `now()` on schedule creation. This means they will only run on next cron occurence. If you need your schedules to be run as soon as possible after initialisation, you can specify `run_on_creation=True`.
+By default, `last_run` is set to `now()` on schedule creation. This means they will only run on next cron occurence. If you need your schedules to be run as soon as possible after initialisation, you can specify `run_on_creation=True`.
 
 ```python
 @schedule_task(cron="30 8 * * *", run_on_creation=True)
 @register_task()
 def my_task():
     ...
 ```
@@ -200,21 +202,24 @@
 ```python
 @schedule_task(cron="30 8 * * *", catch_up=True)
 @register_task()
 def my_task():
     ...
 ```
 
-You may get the schedule's cron datetime provided as a keyword argument to the task using the `datetime_kwarg` argument. This is often useful in combination with catch_up, for things like report generation.
+You may get the schedule's cron datetime provided as a keyword argument to the task using the `datetime_kwarg` argument. This is often useful in combination with catch_up, for things like report generation. Remember to treat the case where the argument is `None` (which happens when the task is run outside of the schedule).
 
 ```python
 @schedule_task(cron="30 8 * * *", datetime_kwarg="scheduled_on", catch_up=True)
 @register_task()
 def my_task(scheduled_on):
-    return f"This was scheduled for {scheduled_on.isoformat()}."
+    if scheduled_on:
+        return f"This was scheduled for {scheduled_on.isoformat()}."
+    else:
+        return "This was not scheduled."
 ```
 
 Similarly to tasks, you can assign schedules to specific queues, and then have your worker only consume tasks from specific queues using `--queue myqueue` or `--exclude_queue myqueue`.
 
 ```python
 @schedule_task(cron="30 8 * * *", queue='scheduler')
 @register_task(queue='worker')
@@ -222,24 +227,36 @@
     ...
 
 # Then run those with these workers
 # manage.py worker --queue scheduler
 # manage.py worker --queue worker
 ```
 
+Schedule's cron support a non-standard sixth argument for seconds  :
+```python
+from django_toosimple_q.decorators import register_task, schedule_task
+
+# A schedule running every 15 seconds
+@schedule_task(cron="* * * * * */15")
+@register_task()
+def morning_routine():
+    return f"15 seconds passed !"
+```
+
 ### Management comment
 
 Besides standard django management commands arguments, the management command supports following arguments.
 
 ```
 usage: manage.py worker [--queue QUEUE | --exclude_queue EXCLUDE_QUEUE]
                         [--tick TICK]
                         [--once | --until_done]
                         [--label LABEL]
                         [--timeout TIMEOUT]
+                        [--reload {always,never}]
 
 optional arguments:
   --queue QUEUE         which queue to run (can be used several times, all
                         queues are run if not provided)
   --exclude_queue EXCLUDE_QUEUE
                         which queue not to run (can be used several times, all
                         queues are run if not provided)
@@ -249,29 +266,18 @@
   --until_done          run until no tasks are available then exit (useful for
                         debugging)
   --label LABEL         the name of the worker to help identifying it ('{pid}'
                         will be replaced by the process id)
   --timeout TIMEOUT     the time in seconds after which this worker will be considered
                         offline (set this to a value higher than the longest tasks this
                         worker will execute)
+  --reload {always,never}
+                        watch for changes (by default, watches if DEBUG=True)
 ```
 
-## Demo project
-
-A demo project with pre-configured tasks is provided.
-
-```shell
-python demoproject/manage.py migrate
-python demoproject/manage.py createsuperuser
-python demoproject/manage.py runserver
-python demoproject/manage.py worker  # from a different shell
-```
-
-Then open http://127.0.0.1:8000/admin in your browser
-
 ## Contrib apps
 
 ### django_toosimple_q.contrib.mail
 
 A queued email backend to send emails asynchronously, preventing your website from failing completely in case the upstream backend is down.
 
 Enable and configure the app in `settings.py` :
@@ -288,33 +294,49 @@
 TOOSIMPLEQ_EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
 ```
 
 Head to the [Django documentation](https://docs.djangoproject.com/en/4.0/topics/email/) for usage.
 
 ## Dev
 
-### Tests
-
-To run tests locally (by default, tests runs against an in-memory sqlite database):
+### Automated tests
 
+To run tests, we recommend using Docker :
 ```shell
-pip install -r requirements-dev.txt
-python manage.py test
+docker compose build
+# run all tests
+docker compose run django test
+# or to run just a specific test
+docker compose run django test django_toosimple_q.tests.tests_worker.TestAutoreloadingWorker
 ```
 
-To run tests against postgres, run the following commands before :
+Tests are run automatically on github.
+
+### Manual testing
+
+Manual testing can be done like this:
+
 ```shell
-# Start a local postgres database
-docker run -p 5432:5432 -e POSTGRES_PASSWORD=postgres -d postgres
-# Set and env var
-export TOOSIMPLEQ_TEST_DB=postgres # on Windows: `$Env:TOOSIMPLEQ_TEST_DB = "postgres"`
+# start a dev server and a worker
+docker compose build
+docker compose run django migrate
+docker compose run django createsuperuser
+docker compose up
 ```
 
-Tests are run automatically on github.
+Then connect on 127.0.0.1:8000/admin/
 
+### Without docker
+
+To run tests locally without Docker (by default, tests runs against an in-memory sqlite database):
+
+```shell
+pip install -r requirements-dev.txt
+python manage.py test
+```
 
 ### Contribute
 
 Code style is done with pre-commit :
 ```shell
 pip install -r requirements-dev.txt
 pre-commit install
@@ -335,29 +357,33 @@
 **Registry**: a dictionary keeping all registered schedules and tasks.
 
 **Worker**: a management command that executes schedules and tasks on a regular basis.
 
 
 ## Changelog
 
-- 2022-10-28 : v1.0.0b **⚠ BACKWARDS INCOMPATIBLE RELEASE ⚠**
+- 2023-01-09 : v1.0.0b **⚠ BACKWARDS INCOMPATIBLE RELEASE ⚠**
+  - known issues:
+    - [ ] worker exit status not correctly set with autoreload
   - feature: added workerstatus to the admin, allowing to monitor workers
   - feature: queue tasks for later (`mytask.queue(due=now()+timedelta(hours=2))`)
   - feature: assign queues to schedules (`@schedule_task(queue="schedules")`)
+  - feature: auto-reload when DEBUG is true
   - refactor: removed non-execution related data from the database (clarifying the fact tha the source of truth is the registry)
   - refactor: better support for concurrent workers
   - refactor: better names for models and decorators
   - infra: included a demo project
   - infra: improved testing, including for concurrency behaviour
   - infra: updated compatibility to Django 3.2/4.1 and Python 3.8-3.10
   - quick migration guide:
     - rename `@schedule` -> `@schedule_task`
     - task name must now be provided as a kwarg: `@register_task("mytask")` -> `@register_task(name="mytask")`)
     - replace `@schedule_task(..., last_check=None)` -> `@schedule_task(..., run_on_creation=True)`
     - models: `Schedule` -> `ScheduleExec` and `Task` -> `TaskExec`
+    - renamed `ScheduleExec.last_run` to `ScheduleExec.last_task`
 
 - 2022-03-24 : v0.4.0
   - made `last_check` and `last_run` optional in the admin
   - defined `id` fields
 
 - 2021-07-15 : v0.3.0
   - added `contrib.mail`
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/admin.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from datetime import datetime
+
+from croniter import croniter
 from django.contrib import admin
 from django.contrib.messages.constants import SUCCESS
 from django.template.defaultfilters import truncatechars
 from django.template.loader import render_to_string
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.formats import date_format
@@ -115,51 +118,59 @@
 
 
 @admin.register(ScheduleExec)
 class ScheduleExecAdmin(ReadOnlyAdmin):
     list_display = [
         "icon",
         "name",
-        "last_tick_",
-        "last_run_due_",
-        "last_run_task_",
+        "last_due_",
+        "next_due_",
+        "last_task_",
         "schedule_",
     ]
     list_display_links = ["name"]
-    ordering = ["last_tick"]
+    ordering = ["-last_due"]
     list_filter = ["name", ScheduleQueueListFilter, "state"]
     actions = ["action_force_run"]
-    readonly_fields = ["schedule_", "last_run_due_"]
+    readonly_fields = ["schedule_"]
 
     def schedule_(self, obj):
         if not obj.schedule:
             return None
         return render_to_string("toosimpleq/schedule.html", {"schedule": obj.schedule})
 
-    @admin.display(ordering="last_run__due")
-    def last_run_due_(self, obj):
-        if obj.last_run:
-            return short_naturaltime(obj.last_run.due)
+    def last_task_(self, obj):
+        if obj.last_task:
+            app, model = obj.last_task._meta.app_label, obj.last_task._meta.model_name
+            edit_link = reverse(f"admin:{app}_{model}_change", args=(obj.last_task_id,))
+            return format_html('<a href="{}">{}</a>', edit_link, obj.last_task)
         return "-"
 
-    def last_run_task_(self, obj):
-        if obj.last_run:
-            app, model = obj.last_run._meta.app_label, obj.last_run._meta.model_name
-            edit_link = reverse(f"admin:{app}_{model}_change", args=(obj.last_run_id,))
-            return format_html('<a href="{}">{}</a>', edit_link, obj.last_run)
-        return "-"
-
-    @admin.display(ordering="last_tick")
-    def last_tick_(self, obj):
-        return short_naturaltime(obj.last_tick)
+    @admin.display(ordering="last_due")
+    def last_due_(self, obj):
+        return short_naturaltime(obj.last_due)
+
+    @admin.display()
+    def next_due_(self, obj):
+        if obj.next_dues:
+            next_due = obj.next_dues[0]
+        else:
+            next_due = croniter(obj.schedule.cron, timezone.now()).get_next(datetime)
+
+        formatted_next_due = short_naturaltime(next_due)
+        if len(obj.next_dues) > 1:
+            formatted_next_due += mark_safe(f" [×{len(obj.next_dues)}]")
+        if next_due < timezone.now():
+            return mark_safe(f"<span style='color: red'>{formatted_next_due}</span>")
+        return formatted_next_due
 
     @admin.display(description="Force run schedule")
     def action_force_run(self, request, queryset):
         for schedule_exec in queryset:
-            schedule = schedule_exec.schedule.execute(force=True)
+            schedule_exec.schedule.execute(force=True)
         self.message_user(
             request,
             f"{queryset.count()} schedules successfully executed",
             level=SUCCESS,
         )
 
 
@@ -188,32 +199,33 @@
 
     @admin.display(ordering="stopped")
     def stopped_(self, obj):
         return short_naturaltime(obj.stopped)
 
 
 def short_naturaltime(datetime):
-
     if datetime is None:
         return None
 
-    delta = timezone.now() - datetime
     disps = [
         (60, "s"),
         (60 * 60, "m"),
         (60 * 60 * 24, "h"),
         (60 * 60 * 24 * 7, "D"),
         (60 * 60 * 24 * 30, "W"),
         (60 * 60 * 24 * 365, "M"),
         (float("inf"), "Y"),
     ]
 
+    delta = timezone.now() - datetime
+    seconds = delta.total_seconds()
+
     last_v = 1
     for threshold, abbr in disps:
-        if abs(delta.seconds) < threshold:
-            text = f"{delta.seconds // last_v}{abbr}"
+        if abs(seconds) < threshold:
+            text = f"{int(abs(seconds) // last_v)}{abbr}"
             break
         last_v = threshold
 
-    shorttime = f"in&nbsp;{text}" if delta.seconds < 0 else f"{text}&nbsp;ago"
+    shorttime = f"in&nbsp;{text}" if seconds < 0 else f"{text}&nbsp;ago"
     longtime = date_format(datetime, format="DATETIME_FORMAT", use_l10n=True)
     return mark_safe(f'<span title="{escape(longtime)}">{shorttime}</span>')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/contrib/mail/tests.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/contrib/mail/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         importlib.reload(mail_tasks)
 
     @override_settings(
         EMAIL_BACKEND="django_toosimple_q.contrib.mail.backend.QueueBackend",
         TOOSIMPLEQ_EMAIL_BACKEND="django.core.mail.backends.locmem.EmailBackend",
     )
     def test_queue_mail(self):
-
         self.assertQueue(0)
 
         send_mail(
             "Subject here",
             "Here is the message.",
             "from@example.com",
             ["to@example.com"],
@@ -41,15 +40,14 @@
         self.assertEquals(len(mail.outbox), 1)
 
     @override_settings(
         EMAIL_BACKEND="django_toosimple_q.contrib.mail.backend.QueueBackend",
         TOOSIMPLEQ_EMAIL_BACKEND="django.core.mail.backends.locmem.EmailBackend",
     )
     def test_queue_mail_two(self):
-
         self.assertQueue(0)
 
         send_mail(
             "Subject here",
             "Here is the message.",
             "from@example.com",
             ["to@example.com"],
@@ -72,15 +70,14 @@
         self.assertEquals(len(mail.outbox), 2)
 
     @override_settings(
         EMAIL_BACKEND="django_toosimple_q.contrib.mail.backend.QueueBackend",
         TOOSIMPLEQ_EMAIL_BACKEND="django.core.mail.backends.locmem.EmailBackend",
     )
     def test_queue_mail_duplicate(self):
-
         self.assertQueue(0)
 
         send_mail(
             "Subject here",
             "Here is the message.",
             "from@example.com",
             ["to@example.com"],
@@ -103,15 +100,14 @@
         self.assertEquals(len(mail.outbox), 1)
 
     @override_settings(
         EMAIL_BACKEND="django_toosimple_q.contrib.mail.backend.QueueBackend",
         TOOSIMPLEQ_EMAIL_BACKEND="django.core.mail.backends.locmem.EmailBackend",
     )
     def test_queue_mass_mail(self):
-
         self.assertQueue(0)
 
         send_mass_mail(
             [
                 ("Subject A", "Message.", "from@example.com", ["to@example.com"]),
                 ("Subject B", "Message.", "from@example.com", ["to@example.com"]),
                 ("Subject C", "Message.", "from@example.com", ["to@example.com"]),
@@ -129,15 +125,14 @@
         self.assertEquals(len(mail.outbox), 3)
 
     @override_settings(
         EMAIL_BACKEND="django_toosimple_q.contrib.mail.backend.QueueBackend",
         TOOSIMPLEQ_EMAIL_BACKEND="failing_backend",
     )
     def test_queue_mail_failing_backend(self):
-
         self.assertQueue(0)
 
         send_mail(
             "Subject here",
             "Here is the message.",
             "from@example.com",
             ["to@example.com"],
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/decorators.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/decorators.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/logging.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/logging.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 from .registry import schedules_registry, tasks_registry
 
 formatter = logging.Formatter(
-    fmt="[%(asctime)s %(levelname)s] [toosimpleq] %(message)s"
+    "[%(asctime)s %(levelname)s] [toosimpleq] %(message)s", "%Y-%m-%d %H:%M:%S"
 )
 
 handler = logging.StreamHandler()
 handler.setFormatter(formatter)
 
 logger = logging.getLogger("toosimpleq")
 logger.setLevel(logging.INFO)
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0001_initial.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import django.db.models.deletion
 import django.utils.timezone
 import picklefield.fields
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="Task",
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0002_auto_20191101_1838.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0002_auto_20191101_1838.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.6 on 2019-11-01 17:38
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("toosimpleq", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="task",
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0005_auto_20210302_1748.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0005_auto_20210302_1748.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.0.6 on 2021-03-02 16:48
 
 import django.utils.timezone
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("toosimpleq", "0004_auto_20200507_1339"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="task",
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0006_task_replacement.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0006_task_replacement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.0.6 on 2021-06-14 19:54
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("toosimpleq", "0005_auto_20210302_1748"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="task",
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0008_auto_20210902_2111.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0008_auto_20210902_2111.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import django.db.models.deletion
 import django.utils.timezone
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("toosimpleq", "0007_schedule_datetime_kwarg"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="schedule",
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0009_auto_20210902_2245.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0009_auto_20210902_2245.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.5 on 2021-09-02 20:45
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("toosimpleq", "0008_auto_20210902_2111"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="schedule",
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0010_auto_20220324_0419.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0010_auto_20220324_0419.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.12 on 2022-03-23 20:40
 
 import django
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("toosimpleq", "0009_auto_20210902_2245"),
     ]
 
     operations = [
         migrations.RenameModel(
             old_name="Schedule",
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/migrations/0011_workerstatus.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/migrations/0011_workerstatus.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import django.db.models.deletion
 import django.utils.timezone
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("toosimpleq", "0010_auto_20220324_0419"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="WorkerStatus",
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/tests/concurrency/tasks.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/concurrency/tasks.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from django.contrib.auth.models import User
 from django.db import IntegrityError
 
 from ...decorators import register_task, schedule_task
 
 
-@schedule_task(cron="* * * * *", queue="schedules")
+@schedule_task(cron="* * * * *", queue="schedules", run_on_creation=True)
 @register_task(name="create_user", queue="tasks")
 def create_user():
     time.sleep(0.5)
     retry = 0
     while True:
         suffix = f"-copy{retry}" if retry > 0 else ""
         try:
@@ -22,9 +22,22 @@
     if retry > 0:
         raise Exception("Failed: had to rename the user")
     return 0
 
 
 @register_task(name="sleep_task", queue="tasks")
 def sleep_task(duration):
-    time.sleep(duration)
+    t1 = time.time()
+    while time.time() - t1 < duration:
+        pass
+    return True
+
+
+@register_task(name="output_string_task", queue="tasks")
+def output_string_task():
+    return "***OUTPUT_A***"
+
+
+@schedule_task(cron="* * * * * *", queue="regr_schedule_short")
+@register_task(name="regr_schedule_short", queue="_")
+def regr_schedule_short():
     return True
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/tests/settings.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Settings for running tests"""
 
-"""Settings overrides for testing concurrent workers"""
+import os
 
 from .utils import is_postgres
 
 DEBUG = True
 USE_TZ = True
 TIME_ZONE = "UTC"
 SECRET_KEY = "secret_key"
 
-
 if is_postgres():
     DATABASES = {
         "default": {
             "ENGINE": "django.db.backends.postgresql",
-            "HOST": "127.0.0.1",
-            "PORT": "5432",
+            "HOST": os.environ.get("POSTGRES_HOST", "127.0.0.1"),
+            "PORT": os.environ.get("POSTGRES_PORT", "5432"),
             "NAME": "postgres",
             "USER": "postgres",
             "PASSWORD": "postgres",
             "TEST": {
                 "NAME": "test_postgres",
             },
         }
@@ -33,22 +32,23 @@
             "TEST": {
                 "NAME": "db-test.sqlite3",
             },
         }
     }
 
 INSTALLED_APPS = [
+    "django_toosimple_q.tests.concurrency",
+    "django_toosimple_q.tests.demo",
+    "django_toosimple_q",
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.messages",
     "django.contrib.sessions",
     "django.contrib.staticfiles",
-    "django_toosimple_q",
-    "django_toosimple_q.tests.concurrency",
 ]
 
 ROOT_URLCONF = "django_toosimple_q.tests.urls"
 
 MIDDLEWARE = (
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/tests/tests_admin.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_admin.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/tests/tests_schedules.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_schedules.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q/tests/tests_tasks.py` & `django-toosimple-q-1.0.0b4/django_toosimple_q/tests/tests_tasks.py`

 * *Files identical despite different names*

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q.egg-info/PKG-INFO` & `django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-toosimple-q
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: A simplistic task queue and cron-like scheduler for Django
 Home-page: https://github.com/olivierdalang/django-toosimple-q
 Author: Olivier Dalang
 Author-email: olivier.dalang@gmail.com
 License: MIT
 Description: # Django Too Simple Queue
         
@@ -17,16 +17,18 @@
         Features :
         
         - no celery/redis/rabbitmq/whatever... just Django !
         - clean decorator syntax to register tasks and schedules
         - simple queuing syntax
         - cron-like scheduling
         - tasks.py autodiscovery
+        - supports autoreload
         - django admin integration
         - tasks results stored using the Django ORM
+        - replacement tasks on interruption
         
         Limitations :
         
         - no multithreading yet (but running multiple workers should work)
         - not well suited for projects spawning a high volume of tasks
         
         Compatibility:
@@ -67,15 +69,15 @@
         my_task.queue("Peter")
         ```
         
         Registered tasks can be scheduled from code using this cron-like syntax :
         ```python
         from django_toosimple_q.decorators import register_task, schedule_task
         
-        # Register and schedule tasks
+        # Register and schedule tasks (each morning at 8:30)
         @schedule_task(cron="30 8 * * *", args=['John'])
         @register_task()
         def morning_routine(name):
             return f"Good morning {name} !"
         ```
         
         To consume the tasks, you need to run at least one worker :
@@ -190,15 +192,15 @@
         @schedule_task(name="afternoon_routine", cron="30 16 * * *", args=['afternoon'])
         @schedule_task(name="morning_routine", cron="30 8 * * *", args=['morning'])
         @register_task()
         def my_task(time_of_day):
             return f"Good {time_of_day} John !"
         ```
         
-        By default, `last_tick` is set to `now()` on schedule creation. This means they will only run on next cron occurence. If you need your schedules to be run as soon as possible after initialisation, you can specify `run_on_creation=True`.
+        By default, `last_run` is set to `now()` on schedule creation. This means they will only run on next cron occurence. If you need your schedules to be run as soon as possible after initialisation, you can specify `run_on_creation=True`.
         
         ```python
         @schedule_task(cron="30 8 * * *", run_on_creation=True)
         @register_task()
         def my_task():
             ...
         ```
@@ -208,21 +210,24 @@
         ```python
         @schedule_task(cron="30 8 * * *", catch_up=True)
         @register_task()
         def my_task():
             ...
         ```
         
-        You may get the schedule's cron datetime provided as a keyword argument to the task using the `datetime_kwarg` argument. This is often useful in combination with catch_up, for things like report generation.
+        You may get the schedule's cron datetime provided as a keyword argument to the task using the `datetime_kwarg` argument. This is often useful in combination with catch_up, for things like report generation. Remember to treat the case where the argument is `None` (which happens when the task is run outside of the schedule).
         
         ```python
         @schedule_task(cron="30 8 * * *", datetime_kwarg="scheduled_on", catch_up=True)
         @register_task()
         def my_task(scheduled_on):
-            return f"This was scheduled for {scheduled_on.isoformat()}."
+            if scheduled_on:
+                return f"This was scheduled for {scheduled_on.isoformat()}."
+            else:
+                return "This was not scheduled."
         ```
         
         Similarly to tasks, you can assign schedules to specific queues, and then have your worker only consume tasks from specific queues using `--queue myqueue` or `--exclude_queue myqueue`.
         
         ```python
         @schedule_task(cron="30 8 * * *", queue='scheduler')
         @register_task(queue='worker')
@@ -230,24 +235,36 @@
             ...
         
         # Then run those with these workers
         # manage.py worker --queue scheduler
         # manage.py worker --queue worker
         ```
         
+        Schedule's cron support a non-standard sixth argument for seconds  :
+        ```python
+        from django_toosimple_q.decorators import register_task, schedule_task
+        
+        # A schedule running every 15 seconds
+        @schedule_task(cron="* * * * * */15")
+        @register_task()
+        def morning_routine():
+            return f"15 seconds passed !"
+        ```
+        
         ### Management comment
         
         Besides standard django management commands arguments, the management command supports following arguments.
         
         ```
         usage: manage.py worker [--queue QUEUE | --exclude_queue EXCLUDE_QUEUE]
                                 [--tick TICK]
                                 [--once | --until_done]
                                 [--label LABEL]
                                 [--timeout TIMEOUT]
+                                [--reload {always,never}]
         
         optional arguments:
           --queue QUEUE         which queue to run (can be used several times, all
                                 queues are run if not provided)
           --exclude_queue EXCLUDE_QUEUE
                                 which queue not to run (can be used several times, all
                                 queues are run if not provided)
@@ -257,29 +274,18 @@
           --until_done          run until no tasks are available then exit (useful for
                                 debugging)
           --label LABEL         the name of the worker to help identifying it ('{pid}'
                                 will be replaced by the process id)
           --timeout TIMEOUT     the time in seconds after which this worker will be considered
                                 offline (set this to a value higher than the longest tasks this
                                 worker will execute)
+          --reload {always,never}
+                                watch for changes (by default, watches if DEBUG=True)
         ```
         
-        ## Demo project
-        
-        A demo project with pre-configured tasks is provided.
-        
-        ```shell
-        python demoproject/manage.py migrate
-        python demoproject/manage.py createsuperuser
-        python demoproject/manage.py runserver
-        python demoproject/manage.py worker  # from a different shell
-        ```
-        
-        Then open http://127.0.0.1:8000/admin in your browser
-        
         ## Contrib apps
         
         ### django_toosimple_q.contrib.mail
         
         A queued email backend to send emails asynchronously, preventing your website from failing completely in case the upstream backend is down.
         
         Enable and configure the app in `settings.py` :
@@ -296,33 +302,49 @@
         TOOSIMPLEQ_EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
         ```
         
         Head to the [Django documentation](https://docs.djangoproject.com/en/4.0/topics/email/) for usage.
         
         ## Dev
         
-        ### Tests
-        
-        To run tests locally (by default, tests runs against an in-memory sqlite database):
+        ### Automated tests
         
+        To run tests, we recommend using Docker :
         ```shell
-        pip install -r requirements-dev.txt
-        python manage.py test
+        docker compose build
+        # run all tests
+        docker compose run django test
+        # or to run just a specific test
+        docker compose run django test django_toosimple_q.tests.tests_worker.TestAutoreloadingWorker
         ```
         
-        To run tests against postgres, run the following commands before :
+        Tests are run automatically on github.
+        
+        ### Manual testing
+        
+        Manual testing can be done like this:
+        
         ```shell
-        # Start a local postgres database
-        docker run -p 5432:5432 -e POSTGRES_PASSWORD=postgres -d postgres
-        # Set and env var
-        export TOOSIMPLEQ_TEST_DB=postgres # on Windows: `$Env:TOOSIMPLEQ_TEST_DB = "postgres"`
+        # start a dev server and a worker
+        docker compose build
+        docker compose run django migrate
+        docker compose run django createsuperuser
+        docker compose up
         ```
         
-        Tests are run automatically on github.
+        Then connect on 127.0.0.1:8000/admin/
         
+        ### Without docker
+        
+        To run tests locally without Docker (by default, tests runs against an in-memory sqlite database):
+        
+        ```shell
+        pip install -r requirements-dev.txt
+        python manage.py test
+        ```
         
         ### Contribute
         
         Code style is done with pre-commit :
         ```shell
         pip install -r requirements-dev.txt
         pre-commit install
@@ -343,29 +365,33 @@
         **Registry**: a dictionary keeping all registered schedules and tasks.
         
         **Worker**: a management command that executes schedules and tasks on a regular basis.
         
         
         ## Changelog
         
-        - 2022-10-28 : v1.0.0b **⚠ BACKWARDS INCOMPATIBLE RELEASE ⚠**
+        - 2023-01-09 : v1.0.0b **⚠ BACKWARDS INCOMPATIBLE RELEASE ⚠**
+          - known issues:
+            - [ ] worker exit status not correctly set with autoreload
           - feature: added workerstatus to the admin, allowing to monitor workers
           - feature: queue tasks for later (`mytask.queue(due=now()+timedelta(hours=2))`)
           - feature: assign queues to schedules (`@schedule_task(queue="schedules")`)
+          - feature: auto-reload when DEBUG is true
           - refactor: removed non-execution related data from the database (clarifying the fact tha the source of truth is the registry)
           - refactor: better support for concurrent workers
           - refactor: better names for models and decorators
           - infra: included a demo project
           - infra: improved testing, including for concurrency behaviour
           - infra: updated compatibility to Django 3.2/4.1 and Python 3.8-3.10
           - quick migration guide:
             - rename `@schedule` -> `@schedule_task`
             - task name must now be provided as a kwarg: `@register_task("mytask")` -> `@register_task(name="mytask")`)
             - replace `@schedule_task(..., last_check=None)` -> `@schedule_task(..., run_on_creation=True)`
             - models: `Schedule` -> `ScheduleExec` and `Task` -> `TaskExec`
+            - renamed `ScheduleExec.last_run` to `ScheduleExec.last_task`
         
         - 2022-03-24 : v0.4.0
           - made `last_check` and `last_run` optional in the admin
           - defined `id` fields
         
         - 2021-07-15 : v0.3.0
           - added `contrib.mail`
```

### Comparing `django-toosimple-q-1.0.0b3/django_toosimple_q.egg-info/SOURCES.txt` & `django-toosimple-q-1.0.0b4/django_toosimple_q.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -31,23 +31,29 @@
 django_toosimple_q/migrations/0005_auto_20210302_1748.py
 django_toosimple_q/migrations/0006_task_replacement.py
 django_toosimple_q/migrations/0007_schedule_datetime_kwarg.py
 django_toosimple_q/migrations/0008_auto_20210902_2111.py
 django_toosimple_q/migrations/0009_auto_20210902_2245.py
 django_toosimple_q/migrations/0010_auto_20220324_0419.py
 django_toosimple_q/migrations/0011_workerstatus.py
+django_toosimple_q/migrations/0012_rename_last_run_scheduleexec_last_task.py
+django_toosimple_q/migrations/0013_workerstatus_exit_code_workerstatus_exit_log.py
 django_toosimple_q/migrations/__init__.py
 django_toosimple_q/templates/toosimpleq/schedule.html
 django_toosimple_q/templates/toosimpleq/task.html
 django_toosimple_q/tests/__init__.py
 django_toosimple_q/tests/base.py
 django_toosimple_q/tests/settings.py
+django_toosimple_q/tests/settings_bg.py
+django_toosimple_q/tests/settings_bg_lag.py
 django_toosimple_q/tests/tests_admin.py
 django_toosimple_q/tests/tests_concurrency.py
+django_toosimple_q/tests/tests_regression.py
 django_toosimple_q/tests/tests_schedules.py
 django_toosimple_q/tests/tests_tasks.py
 django_toosimple_q/tests/tests_worker.py
 django_toosimple_q/tests/urls.py
 django_toosimple_q/tests/utils.py
 django_toosimple_q/tests/concurrency/__init__.py
-django_toosimple_q/tests/concurrency/settings.py
-django_toosimple_q/tests/concurrency/tasks.py
+django_toosimple_q/tests/concurrency/tasks.py
+django_toosimple_q/tests/demo/__init__.py
+django_toosimple_q/tests/demo/tasks.py
```

### Comparing `django-toosimple-q-1.0.0b3/setup.py` & `django-toosimple-q-1.0.0b4/setup.py`

 * *Files identical despite different names*


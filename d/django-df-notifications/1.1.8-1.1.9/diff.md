# Comparing `tmp/django-df-notifications-1.1.8.tar.gz` & `tmp/django-df-notifications-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-df-notifications-1.1.8.tar", last modified: Wed Feb 22 18:55:07 2023, max compression
+gzip compressed data, was "django-df-notifications-1.1.9.tar", last modified: Wed Feb 22 19:01:26 2023, max compression
```

## Comparing `django-df-notifications-1.1.8.tar` & `django-df-notifications-1.1.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.647727 django-df-notifications-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-02-22 18:55:07.647727 django-df-notifications-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.643727 django-df-notifications-1.1.8/df_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.643727 django-df-notifications-1.1.8/df_notifications/drf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/drf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/drf/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/drf/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/drf/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.643727 django-df-notifications-1.1.8/df_notifications/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/migrations/0002_remove_notificationhistory_df_notifica_templat_fc63aa_idx_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/migrations/0003_remove_notificationhistory_df_notifica_templat_ec4b48_idx_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.639727 django-df-notifications-1.1.8/df_notifications/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.643727 django-df-notifications-1.1.8/df_notifications/templates/df_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/templates/df_notifications/base_slack.html
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/df_notifications/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.643727 django-df-notifications-1.1.8/django_df_notifications.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-02-22 18:55:07.000000 django-df-notifications-1.1.8/django_df_notifications.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-02-22 18:55:07.000000 django-df-notifications-1.1.8/django_df_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 18:55:07.000000 django-df-notifications-1.1.8/django_df_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-22 18:55:07.000000 django-df-notifications-1.1.8/django_df_notifications.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-22 18:55:07.000000 django-df-notifications-1.1.8/django_df_notifications.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-02-22 18:55:07.647727 django-df-notifications-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.647727 django-df-notifications-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.647727 django-df-notifications-1.1.8/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.647727 django-df-notifications-1.1.8/tests/test_app/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.647727 django-df-notifications-1.1.8/tests/test_app/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/management/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.647727 django-df-notifications-1.1.8/tests/test_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/migrations/0002_alter_postnotificationreminder_history_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/migrations/0003_postnotificationreminder_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/migrations/0004_alter_postnotificationrule_is_published_prev.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/migrations/0005_rename_template_prefix_postnotificationreminder_template_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/migrations/0006_rename_template_postnotificationreminder_template_prefix_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.647727 django-df-notifications-1.1.8/tests/test_app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/templates/base.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 18:55:07.647727 django-df-notifications-1.1.8/tests/test_app/templates/post/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/templates/post/body.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/templates/post/subject.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/test_app/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-02-22 18:54:56.000000 django-df-notifications-1.1.8/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.250712 django-df-notifications-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-02-22 19:01:26.250712 django-df-notifications-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.246712 django-df-notifications-1.1.9/df_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.246712 django-df-notifications-1.1.9/df_notifications/drf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/drf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/drf/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/drf/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/drf/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.250712 django-df-notifications-1.1.9/df_notifications/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/migrations/0002_remove_notificationhistory_df_notifica_templat_fc63aa_idx_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/migrations/0003_remove_notificationhistory_df_notifica_templat_ec4b48_idx_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.246712 django-df-notifications-1.1.9/df_notifications/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.250712 django-df-notifications-1.1.9/df_notifications/templates/df_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/templates/df_notifications/base_slack.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/df_notifications/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.250712 django-df-notifications-1.1.9/django_df_notifications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-02-22 19:01:26.000000 django-df-notifications-1.1.9/django_df_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-02-22 19:01:26.000000 django-df-notifications-1.1.9/django_df_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 19:01:26.000000 django-df-notifications-1.1.9/django_df_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-22 19:01:26.000000 django-df-notifications-1.1.9/django_df_notifications.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-22 19:01:26.000000 django-df-notifications-1.1.9/django_df_notifications.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-02-22 19:01:26.250712 django-df-notifications-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.250712 django-df-notifications-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.250712 django-df-notifications-1.1.9/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.250712 django-df-notifications-1.1.9/tests/test_app/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.250712 django-df-notifications-1.1.9/tests/test_app/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.250712 django-df-notifications-1.1.9/tests/test_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/migrations/0002_alter_postnotificationreminder_history_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/migrations/0003_postnotificationreminder_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/migrations/0004_alter_postnotificationrule_is_published_prev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/migrations/0005_rename_template_prefix_postnotificationreminder_template_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/migrations/0006_rename_template_postnotificationreminder_template_prefix_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.250712 django-df-notifications-1.1.9/tests/test_app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/templates/base.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 19:01:26.250712 django-df-notifications-1.1.9/tests/test_app/templates/post/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/templates/post/body.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/templates/post/subject.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/test_app/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-02-22 19:01:15.000000 django-df-notifications-1.1.9/tests/urls.py
```

### Comparing `django-df-notifications-1.1.8/LICENSE` & `django-df-notifications-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/PKG-INFO` & `django-df-notifications-1.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-df-notifications
-Version: 1.1.8
+Version: 1.1.9
 Summary: Opinionated Django Omnichannel Notifications
 Home-page: https://apexive.com/
 Author: Apexive OSS
 Author-email: open-source@apexive.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-df-notifications-1.1.8/README.md` & `django-df-notifications-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/df_notifications/admin.py` & `django-df-notifications-1.1.9/df_notifications/admin.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/df_notifications/apps.py` & `django-df-notifications-1.1.9/df_notifications/apps.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/df_notifications/channels.py` & `django-df-notifications-1.1.9/df_notifications/channels.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/df_notifications/decorators.py` & `django-df-notifications-1.1.9/df_notifications/decorators.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/df_notifications/migrations/0001_initial.py` & `django-df-notifications-1.1.9/df_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/df_notifications/migrations/0002_remove_notificationhistory_df_notifica_templat_fc63aa_idx_and_more.py` & `django-df-notifications-1.1.9/df_notifications/migrations/0002_remove_notificationhistory_df_notifica_templat_fc63aa_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/df_notifications/migrations/0003_remove_notificationhistory_df_notifica_templat_ec4b48_idx_and_more.py` & `django-df-notifications-1.1.9/df_notifications/migrations/0003_remove_notificationhistory_df_notifica_templat_ec4b48_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/df_notifications/models.py` & `django-df-notifications-1.1.9/df_notifications/models.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/df_notifications/settings.py` & `django-df-notifications-1.1.9/df_notifications/settings.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/df_notifications/tasks.py` & `django-df-notifications-1.1.9/df_notifications/tasks.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/df_notifications/utils.py` & `django-df-notifications-1.1.9/df_notifications/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     channel_instance = get_channel_instance(channel)
     parts = {}
     for part in channel_instance.template_parts:
         templates = []
         for prefix in template_prefixes:
             templates.append(f"{prefix}{channel}__{part}")
             templates.append(f"{prefix}{part}")
-        parts[part] = render_to_string(templates, context=context)
+        parts[part] = render_to_string(templates, context=context).strip()
 
     channel_instance.send(users, {**context, **parts})
 
     notification = NotificationHistory.objects.create(
         channel=channel,
         template_prefix=template_prefixes[0],
         content=parts if settings.DF_NOTIFICATIONS["SAVE_HISTORY_CONTENT"] else "",
```

### Comparing `django-df-notifications-1.1.8/django_df_notifications.egg-info/PKG-INFO` & `django-df-notifications-1.1.9/django_df_notifications.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-df-notifications
-Version: 1.1.8
+Version: 1.1.9
 Summary: Opinionated Django Omnichannel Notifications
 Home-page: https://apexive.com/
 Author: Apexive OSS
 Author-email: open-source@apexive.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-df-notifications-1.1.8/django_df_notifications.egg-info/SOURCES.txt` & `django-df-notifications-1.1.9/django_df_notifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/setup.cfg` & `django-df-notifications-1.1.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 force_alphabetical_sort = True
 force_single_line = True
 lines_after_imports = 2
 line_length = 160
 
 [metadata]
 name = django-df-notifications
-version = 1.1.8
+version = 1.1.9
 description = Opinionated Django Omnichannel Notifications
 long_description = file: README.md
 url = https://apexive.com/
 author = Apexive OSS
 author_email = open-source@apexive.com
 license = MIT
 classifiers =
```

### Comparing `django-df-notifications-1.1.8/tests/settings.py` & `django-df-notifications-1.1.9/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/tests/test_app/migrations/0001_initial.py` & `django-df-notifications-1.1.9/tests/test_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/tests/test_app/migrations/0002_alter_postnotificationreminder_history_and_more.py` & `django-df-notifications-1.1.9/tests/test_app/migrations/0002_alter_postnotificationreminder_history_and_more.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/tests/test_app/migrations/0003_postnotificationreminder_action.py` & `django-df-notifications-1.1.9/tests/test_app/migrations/0003_postnotificationreminder_action.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/tests/test_app/migrations/0005_rename_template_prefix_postnotificationreminder_template_and_more.py` & `django-df-notifications-1.1.9/tests/test_app/migrations/0005_rename_template_prefix_postnotificationreminder_template_and_more.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/tests/test_app/migrations/0006_rename_template_postnotificationreminder_template_prefix_and_more.py` & `django-df-notifications-1.1.9/tests/test_app/migrations/0006_rename_template_postnotificationreminder_template_prefix_and_more.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/tests/test_app/models.py` & `django-df-notifications-1.1.9/tests/test_app/models.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.1.8/tests/test_app/tests.py` & `django-df-notifications-1.1.9/tests/test_app/tests.py`

 * *Files identical despite different names*


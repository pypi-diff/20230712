# Comparing `tmp/django_twined-0.5.1.tar.gz` & `tmp/django_twined-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_twined-0.5.1.tar", max compression
+gzip compressed data, was "django_twined-0.6.0.tar", max compression
```

## Comparing `django_twined-0.5.1.tar` & `django_twined-0.6.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1088 2023-07-10 14:07:19.527984 django_twined-0.5.1/LICENSE
--rw-r--r--   0        0        0     1463 2023-07-10 14:07:19.527984 django_twined-0.5.1/README.md
--rw-r--r--   0        0        0       64 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/__init__.py
--rw-r--r--   0        0        0      257 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/admin/__init__.py
--rw-r--r--   0        0        0     6781 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/admin/admin.py
--rw-r--r--   0        0        0      402 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/admin/fieldsets.py
--rw-r--r--   0        0        0      881 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/admin/mixins.py
--rw-r--r--   0        0        0      682 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/admin/proxy.py
--rw-r--r--   0        0        0      496 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/apps.py
--rw-r--r--   0        0        0      104 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/consumers/__init__.py
--rw-r--r--   0        0        0     3766 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/consumers/analysis.py
--rw-r--r--   0        0        0     1002 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/consumers/analysis_log.py
--rw-r--r--   0        0        0     5823 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/consumers/service.py
--rw-r--r--   0        0        0      130 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/exceptions.py
--rw-r--r--   0        0        0     2358 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/fields.py
--rw-r--r--   0        0        0        0 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/management/commands/__init__.py
--rw-r--r--   0        0        0     2300 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/management/commands/sync_data_stores.py
--rw-r--r--   0        0        0     2991 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/messages.py
--rw-r--r--   0        0        0     2346 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/0001_initial.py
--rw-r--r--   0        0        0      595 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/0002_slug_unique_and_not_editable.py
--rw-r--r--   0        0        0      408 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/0003_rename_slug_to_name.py
--rw-r--r--   0        0        0      670 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/0004_add_timestamps.py
--rw-r--r--   0        0        0      731 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/0005_question_date_help_text.py
--rw-r--r--   0        0        0     4711 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/0006_service_revisions_and_events.py
--rw-r--r--   0        0        0     1476 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/0007_registered_to_revision.py
--rw-r--r--   0        0        0      669 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/0008_registered_relations_to_nullable.py
--rw-r--r--   0        0        0      683 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/0009_remove_registered_services.py
--rw-r--r--   0        0        0      681 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/0010_alter_servicerevision_project_name.py
--rw-r--r--   0        0        0      362 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/0011_remove_servicerevision_topic_id.py
--rw-r--r--   0        0        0      568 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/0012_servicerevision_is_default.py
--rw-r--r--   0        0        0      639 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/0013_alter_serviceusageevent_question.py
--rw-r--r--   0        0        0        0 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/migrations/__init__.py
--rw-r--r--   0        0        0      698 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/models/__init__.py
--rw-r--r--   0        0        0    11441 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/models/datastores.py
--rw-r--r--   0        0        0       85 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/models/querysets/__init__.py
--rw-r--r--   0        0        0     9795 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/models/querysets/datastore_queryset.py
--rw-r--r--   0        0        0     6624 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/models/questions.py
--rw-r--r--   0        0        0     8628 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/models/service_revisions.py
--rw-r--r--   0        0        0     2515 2023-07-10 14:07:19.527984 django_twined-0.5.1/django_twined/models/service_usage_events.py
--rw-r--r--   0        0        0      290 2023-07-10 14:07:19.531984 django_twined-0.5.1/django_twined/routing.py
--rw-r--r--   0        0        0      479 2023-07-10 14:07:19.531984 django_twined-0.5.1/django_twined/signals/__init__.py
--rw-r--r--   0        0        0     3080 2023-07-10 14:07:19.531984 django_twined-0.5.1/django_twined/signals/receivers.py
--rw-r--r--   0        0        0      262 2023-07-10 14:07:19.531984 django_twined-0.5.1/django_twined/signals/senders.py
--rw-r--r--   0        0        0        0 2023-07-10 14:07:19.531984 django_twined-0.5.1/django_twined/static/.gitignore
--rw-r--r--   0        0        0     2667 2023-07-10 14:07:19.531984 django_twined-0.5.1/django_twined/tasks.py
--rw-r--r--   0        0        0     1149 2023-07-10 14:07:19.531984 django_twined-0.5.1/django_twined/templates/admin/question_ask_row.html
--rw-r--r--   0        0        0        0 2023-07-10 14:07:19.531984 django_twined-0.5.1/django_twined/templates/django_twined/.gitignore
--rw-r--r--   0        0        0      343 2023-07-10 14:07:19.531984 django_twined-0.5.1/django_twined/templates/django_twined/question_changeform.html
--rw-r--r--   0        0        0        0 2023-07-10 14:07:19.531984 django_twined-0.5.1/django_twined/templatetags/__init__.py
--rw-r--r--   0        0        0      480 2023-07-10 14:07:19.531984 django_twined-0.5.1/django_twined/templatetags/question_ask_row.py
--rw-r--r--   0        0        0      175 2023-07-10 14:07:19.531984 django_twined-0.5.1/django_twined/urls.py
--rw-r--r--   0        0        0     2419 2023-07-10 14:07:19.531984 django_twined-0.5.1/django_twined/views.py
--rw-r--r--   0        0        0     1556 2023-07-10 14:07:19.535985 django_twined-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2594 1970-01-01 00:00:00.000000 django_twined-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-12 18:25:40.799782 django_twined-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1463 2023-07-12 18:25:40.799782 django_twined-0.6.0/README.md
+-rw-r--r--   0        0        0       64 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/__init__.py
+-rw-r--r--   0        0        0      257 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/admin/__init__.py
+-rw-r--r--   0        0        0     6781 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/admin/admin.py
+-rw-r--r--   0        0        0      402 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/admin/fieldsets.py
+-rw-r--r--   0        0        0      881 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/admin/mixins.py
+-rw-r--r--   0        0        0      682 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/admin/proxy.py
+-rw-r--r--   0        0        0      496 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/apps.py
+-rw-r--r--   0        0        0      104 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/consumers/__init__.py
+-rw-r--r--   0        0        0     3766 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/consumers/analysis.py
+-rw-r--r--   0        0        0     1002 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/consumers/analysis_log.py
+-rw-r--r--   0        0        0     5823 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/consumers/service.py
+-rw-r--r--   0        0        0      130 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/exceptions.py
+-rw-r--r--   0        0        0     2358 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/fields.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/management/commands/__init__.py
+-rw-r--r--   0        0        0     2300 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/management/commands/sync_data_stores.py
+-rw-r--r--   0        0        0     2991 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/messages.py
+-rw-r--r--   0        0        0     2346 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/0002_slug_unique_and_not_editable.py
+-rw-r--r--   0        0        0      408 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/0003_rename_slug_to_name.py
+-rw-r--r--   0        0        0      670 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/0004_add_timestamps.py
+-rw-r--r--   0        0        0      731 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/0005_question_date_help_text.py
+-rw-r--r--   0        0        0     4711 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/0006_service_revisions_and_events.py
+-rw-r--r--   0        0        0     1476 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/0007_registered_to_revision.py
+-rw-r--r--   0        0        0      669 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/0008_registered_relations_to_nullable.py
+-rw-r--r--   0        0        0      683 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/0009_remove_registered_services.py
+-rw-r--r--   0        0        0      681 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/0010_alter_servicerevision_project_name.py
+-rw-r--r--   0        0        0      362 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/0011_remove_servicerevision_topic_id.py
+-rw-r--r--   0        0        0      568 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/0012_servicerevision_is_default.py
+-rw-r--r--   0        0        0      639 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/0013_alter_serviceusageevent_question.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/migrations/__init__.py
+-rw-r--r--   0        0        0      698 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/models/__init__.py
+-rw-r--r--   0        0        0    11441 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/models/datastores.py
+-rw-r--r--   0        0        0       85 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/models/querysets/__init__.py
+-rw-r--r--   0        0        0     9795 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/models/querysets/datastore_queryset.py
+-rw-r--r--   0        0        0     6624 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/models/questions.py
+-rw-r--r--   0        0        0     7716 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/models/service_revisions.py
+-rw-r--r--   0        0        0     2515 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/models/service_usage_events.py
+-rw-r--r--   0        0        0      290 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/routing.py
+-rw-r--r--   0        0        0      479 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/signals/__init__.py
+-rw-r--r--   0        0        0     3080 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/signals/receivers.py
+-rw-r--r--   0        0        0      262 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/signals/senders.py
+-rw-r--r--   0        0        0        0 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/static/.gitignore
+-rw-r--r--   0        0        0     2667 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/tasks.py
+-rw-r--r--   0        0        0     1149 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/templates/admin/question_ask_row.html
+-rw-r--r--   0        0        0        0 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/templates/django_twined/.gitignore
+-rw-r--r--   0        0        0      343 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/templates/django_twined/question_changeform.html
+-rw-r--r--   0        0        0        0 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/templatetags/__init__.py
+-rw-r--r--   0        0        0      480 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/templatetags/question_ask_row.py
+-rw-r--r--   0        0        0      175 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/urls.py
+-rw-r--r--   0        0        0     2419 2023-07-12 18:25:40.799782 django_twined-0.6.0/django_twined/views.py
+-rw-r--r--   0        0        0     1556 2023-07-12 18:25:40.803782 django_twined-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2594 1970-01-01 00:00:00.000000 django_twined-0.6.0/PKG-INFO
```

### Comparing `django_twined-0.5.1/LICENSE` & `django_twined-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/README.md` & `django_twined-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/admin/admin.py` & `django_twined-0.6.0/django_twined/admin/admin.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/admin/mixins.py` & `django_twined-0.6.0/django_twined/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/admin/proxy.py` & `django_twined-0.6.0/django_twined/admin/proxy.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/consumers/analysis.py` & `django_twined-0.6.0/django_twined/consumers/analysis.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/consumers/analysis_log.py` & `django_twined-0.6.0/django_twined/consumers/analysis_log.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/consumers/service.py` & `django_twined-0.6.0/django_twined/consumers/service.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/fields.py` & `django_twined-0.6.0/django_twined/fields.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/management/commands/sync_data_stores.py` & `django_twined-0.6.0/django_twined/management/commands/sync_data_stores.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/messages.py` & `django_twined-0.6.0/django_twined/messages.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/migrations/0001_initial.py` & `django_twined-0.6.0/django_twined/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/migrations/0002_slug_unique_and_not_editable.py` & `django_twined-0.6.0/django_twined/migrations/0002_slug_unique_and_not_editable.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/migrations/0004_add_timestamps.py` & `django_twined-0.6.0/django_twined/migrations/0004_add_timestamps.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/migrations/0005_question_date_help_text.py` & `django_twined-0.6.0/django_twined/migrations/0005_question_date_help_text.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/migrations/0006_service_revisions_and_events.py` & `django_twined-0.6.0/django_twined/migrations/0006_service_revisions_and_events.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/migrations/0007_registered_to_revision.py` & `django_twined-0.6.0/django_twined/migrations/0007_registered_to_revision.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/migrations/0008_registered_relations_to_nullable.py` & `django_twined-0.6.0/django_twined/migrations/0008_registered_relations_to_nullable.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/migrations/0009_remove_registered_services.py` & `django_twined-0.6.0/django_twined/migrations/0009_remove_registered_services.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/migrations/0010_alter_servicerevision_project_name.py` & `django_twined-0.6.0/django_twined/migrations/0010_alter_servicerevision_project_name.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/migrations/0012_servicerevision_is_default.py` & `django_twined-0.6.0/django_twined/migrations/0012_servicerevision_is_default.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/migrations/0013_alter_serviceusageevent_question.py` & `django_twined-0.6.0/django_twined/migrations/0013_alter_serviceusageevent_question.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/models/__init__.py` & `django_twined-0.6.0/django_twined/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/models/datastores.py` & `django_twined-0.6.0/django_twined/models/datastores.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/models/querysets/datastore_queryset.py` & `django_twined-0.6.0/django_twined/models/querysets/datastore_queryset.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/models/questions.py` & `django_twined-0.6.0/django_twined/models/questions.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/models/service_revisions.py` & `django_twined-0.6.0/django_twined/models/service_revisions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 
 import packaging.version
 from django.conf import settings
 from django.db import models, transaction
 from django_gcp.events.utils import get_event_url
 from octue.cloud.pub_sub.service import Service
+from octue.cloud.service_id import convert_service_id_to_pub_sub_form
 from octue.resources.service_backends import get_backend
 
 from .service_usage_events import QUESTION_RESPONSE_UPDATED
 
 
 logger = logging.getLogger(__name__)
 
@@ -60,25 +61,28 @@
     created = models.DateTimeField(
         auto_now_add=True, help_text="When this service revision was created (or, strictly, added to this db)"
     )
 
     namespace = models.SlugField(
         max_length=80,
         default=get_default_namespace,
+        blank=False,
+        null=False,
         help_text="The organisation namespace, eg 'octue'",
     )
 
     name = models.SlugField(
         help_text="The name of the service eg 'example-service'",
     )
 
     tag = models.CharField(
         max_length=80,
         default=get_default_tag,
         blank=False,
+        null=False,
         help_text="The service revision tag that helps to identify the unique deployment",
     )
 
     # GCP provider-specific - will become more flexible over time.
     project_name = models.CharField(
         max_length=80,
         default=get_default_project_name,
@@ -93,59 +97,42 @@
             models.UniqueConstraint(
                 fields=["namespace", "name", "tag"],
                 name="unique_identifier",
             ),
         ]
 
     @property
-    def has_tag(self):
-        """Return true if the instance has a tag"""
-        return (self.tag is not None) and (len(self.tag) > 0)
-
-    @property
-    def has_namespace(self):
-        """Return true if the instance has a namespace"""
-        return (self.namespace is not None) and (len(self.namespace) > 0)
-
-    @property
     def sruid(self):
         """Return the Service Revision Unique Identifier
 
-        Comprises the namespace, name, version, and tag parameters that
-        together uniquely identify a revision (e.g. for the purposes of
-        addressing).
-
-        Using docker image labeling as inspiration, this looks like
-        octue/example-service:0.1.2 or octue/example-service:my-branch
-        or octue/example-service:0.1.2-r1 enabling both routing to specific
-        revisions and things like branches for review
-        """
-        tag = f":{self.tag}" if self.has_tag else ""
-
-        namespace = f"{self.namespace}/" if self.has_namespace else ""
+        Comprises the namespace, name, version, and tag parameters that together uniquely identify a revision (e.g. for
+        the purposes of addressing).
 
-        return f"{namespace}{self.name}{tag}"
-
-    @property
-    def _partial_topic(self):
-        """TODO replace this once the service id has been properly sorted out on the octue side
-        currently this is used to botch the service_id value so that it comes out with the correct topic name format"""
-        tag = f".{self.tag.replace('.', '-')}" if self.has_tag else ""
-        namespace = f"{self.namespace}." if self.has_namespace else ""
-        return f"{namespace}{self.name}{tag}"
+        Using docker image labeling as inspiration, this looks like octue/example-service:0.1.2 or
+        octue/example-service:my-branch or octue/example-service:0.1.2-r1 enabling both routing to specific revisions
+        and things like branches for review.
+        """
+        return f"{self.namespace}/{self.name}:{self.tag}"
 
     @property
     def topic(self):
-        """Return the octue GCP topic address string"""
-        tag = f".{self.tag}" if self.has_tag else ""
-        namespace = f"{self.namespace}." if self.has_namespace else ""
-        return f"octue.services.{namespace}{self.name}{tag}"
+        """Return the octue GCP topic address string.
+
+        :return str:
+        """
+        return "octue.services." + convert_service_id_to_pub_sub_form(self.sruid)
 
     def ask(
-        self, question_id, input_values=None, input_manifest=None, push_url=None, asker_name="django-twined", **kwargs
+        self,
+        question_id,
+        input_values=None,
+        input_manifest=None,
+        push_url=None,
+        asker_name="django-twined",
+        **kwargs,
     ):
         """Ask a question of this service revision
 
         Asks the question and registers a push subscription, to deliver response events on the
         question topic to an endpoint.
         :param Union[str, uuid.UUID] question_id: A uuid to refer to the question by
         :param Union[dict, None] input_values: The input values of the question
@@ -162,33 +149,30 @@
             question_id='some-uuid',
             input_values={},
             input_manifest=Manifest()
         )
         ```
 
         """
-
         if push_url is None:
             push_url = get_event_url(
                 event_kind=QUESTION_RESPONSE_UPDATED,
                 event_reference=question_id,
                 event_parameters={
                     "srid": self.id,  # Adding this (internal) ForeignKey enables creation of ServiceUsageEvents in one DB roundtrip, not two.
                     "sruid": self.sruid,
                 },
                 base_url=settings.TWINED_BASE_URL,
             )
 
-        backend = get_backend()(
-            project_name=self.project_name,
-        )
+        backend = get_backend()(project_name=self.project_name)
+        asker = Service(backend=backend, name=asker_name)
 
-        asker = Service(backend, name=asker_name)
         subscription, _ = asker.ask(
-            service_id=self._partial_topic,  # TODO REFACTOR REQUEST Tidy up in newer versions of octue to give to correct topic name
+            service_id=self.sruid,
             question_uuid=str(question_id),
             input_values=input_values,
             input_manifest=input_manifest,
             push_endpoint=push_url,
             timeout=QUESTION_ASK_TIMEOUT_SECONDS,
             **kwargs,
         )
```

### Comparing `django_twined-0.5.1/django_twined/models/service_usage_events.py` & `django_twined-0.6.0/django_twined/models/service_usage_events.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/signals/receivers.py` & `django_twined-0.6.0/django_twined/signals/receivers.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/tasks.py` & `django_twined-0.6.0/django_twined/tasks.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/templates/admin/question_ask_row.html` & `django_twined-0.6.0/django_twined/templates/admin/question_ask_row.html`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/django_twined/views.py` & `django_twined-0.6.0/django_twined/views.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.5.1/pyproject.toml` & `django_twined-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-twined"
-version = "0.5.1"
+version = "0.6.0"
 description = "A django app to manage octue services"
 authors = ["Tom Clark <tom@octue.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -19,15 +19,15 @@
 keywords = ["django", "services", "octue", "twined"]
 packages = [{ include = "django_twined" },]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 django = ">=3.0,<4.0"
 channels = ">=3.0,<4.0"
-octue = ">=0.39.0,<1"
+octue = ">=0.40.0,<1"
 pika = "^1.2.0"
 django-gcp = ">=0.7.3,<0.11"
 django-jsoneditor = "^0.2.2"
 django-model-utils = "^4.2.0"
 
 [tool.poetry.group.dev.dependencies]
 channels = ">=3.0,<=4.0"
```

### Comparing `django_twined-0.5.1/PKG-INFO` & `django_twined-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-twined
-Version: 0.5.1
+Version: 0.6.0
 Summary: A django app to manage octue services
 Home-page: https://github.com/octue/django-twined
 License: MIT
 Keywords: django,services,octue,twined
 Author: Tom Clark
 Author-email: tom@octue.com
 Requires-Python: >=3.9,<3.11
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: channels (>=3.0,<4.0)
 Requires-Dist: django (>=3.0,<4.0)
 Requires-Dist: django-gcp (>=0.7.3,<0.11)
 Requires-Dist: django-jsoneditor (>=0.2.2,<0.3.0)
 Requires-Dist: django-model-utils (>=4.2.0,<5.0.0)
-Requires-Dist: octue (>=0.39.0,<1)
+Requires-Dist: octue (>=0.40.0,<1)
 Requires-Dist: pika (>=1.2.0,<2.0.0)
 Project-URL: Repository, https://github.com/octue/django-twined
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/django-twined.svg)](https://badge.fury.io/py/django-twined)
 [![codecov](https://codecov.io/gh/octue/django-twined/branch/master/graph/badge.svg)](https://codecov.io/gh/octue/django-twined)
 [![Documentation Status](https://readthedocs.org/projects/django-twined/badge/?version=latest)](https://django-twined.readthedocs.io/en/latest/?badge=latest)
```


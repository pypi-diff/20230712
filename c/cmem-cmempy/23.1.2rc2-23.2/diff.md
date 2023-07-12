# Comparing `tmp/cmem_cmempy-23.1.2rc2.tar.gz` & `tmp/cmem_cmempy-23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_cmempy-23.1.2rc2.tar", max compression
+gzip compressed data, was "cmem_cmempy-23.2.tar", max compression
```

## Comparing `cmem_cmempy-23.1.2rc2.tar` & `cmem_cmempy-23.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    11357 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/LICENSE
--rw-r--r--   0        0        0      651 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/README-public.md
--rw-r--r--   0        0        0      110 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/__init__.py
--rw-r--r--   0        0        0       40 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/__init__.py
--rw-r--r--   0        0        0     4456 2023-03-13 20:41:11.943729 cmem_cmempy-23.1.2rc2/cmem/cmempy/api.py
--rw-r--r--   0        0        0     4970 2023-04-20 02:23:23.487128 cmem_cmempy-23.1.2rc2/cmem/cmempy/config.py
--rw-r--r--   0        0        0     1062 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/custom_tasks/__init__.py
--rw-r--r--   0        0        0       36 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/__init__.py
--rw-r--r--   0        0        0     1029 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/admin/__init__.py
--rw-r--r--   0        0        0     1014 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/admin/backup.py
--rw-r--r--   0        0        0       42 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/authorization/__init__.py
--rw-r--r--   0        0        0     1232 2023-07-12 07:17:10.334193 cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/authorization/conditions.py
--rw-r--r--   0        0        0      477 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/authorization/refresh.py
--rw-r--r--   0        0        0      380 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/proxy/__init__.py
--rw-r--r--   0        0        0     6036 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/proxy/graph.py
--rw-r--r--   0        0        0     4159 2023-04-05 05:40:39.810788 cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/proxy/sparql.py
--rw-r--r--   0        0        0     1244 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/proxy/update.py
--rw-r--r--   0        0        0     1011 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/titles/__init__.py
--rw-r--r--   0        0        0     5905 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/health/__init__.py
--rw-r--r--   0        0        0     1807 2023-07-11 18:28:02.335947 cmem_cmempy-23.1.2rc2/cmem/cmempy/keycloak/client.py
--rw-r--r--   0        0        0      519 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/keycloak/group.py
--rw-r--r--   0        0        0     4500 2023-07-03 04:00:36.674661 cmem_cmempy-23.1.2rc2/cmem/cmempy/keycloak/user.py
--rw-r--r--   0        0        0       31 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/linking/__init__.py
--rw-r--r--   0        0        0     2588 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/linking/linkingtask.py
--rw-r--r--   0        0        0       26 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/plugins/__init__.py
--rw-r--r--   0        0        0     1939 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/plugins/marshalling.py
--rw-r--r--   0        0        0    11190 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/queries/__init__.py
--rw-r--r--   0        0        0       33 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/transform/__init__.py
--rw-r--r--   0        0        0     1090 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/transform/rules/__init__.py
--rw-r--r--   0        0        0     1075 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/transform/rules/transformationrule.py
--rw-r--r--   0        0        0     1240 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/transform/transformationtask.py
--rw-r--r--   0        0        0     3597 2023-02-13 06:43:43.969698 cmem_cmempy-23.1.2rc2/cmem/cmempy/vocabularies/__init__.py
--rw-r--r--   0        0        0      731 2023-06-30 11:48:19.267861 cmem_cmempy-23.1.2rc2/cmem/cmempy/workflow/__init__.py
--rw-r--r--   0        0        0     4891 2023-07-03 04:00:36.674661 cmem_cmempy-23.1.2rc2/cmem/cmempy/workflow/workflow.py
--rw-r--r--   0        0        0      131 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workflow/workflows.py
--rw-r--r--   0        0        0     1873 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/__init__.py
--rw-r--r--   0        0        0      340 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/activities/__init__.py
--rw-r--r--   0        0        0      914 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/activities/projectactivities.py
--rw-r--r--   0        0        0     2281 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/activities/projectactivity.py
--rw-r--r--   0        0        0     3164 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/activities/taskactivities.py
--rw-r--r--   0        0        0     2323 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/activities/taskactivity.py
--rw-r--r--   0        0        0      744 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/export_/__init__.py
--rw-r--r--   0        0        0     1540 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/import_/__init__.py
--rw-r--r--   0        0        0      454 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/__init__.py
--rw-r--r--   0        0        0       45 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/datasets/__init__.py
--rw-r--r--   0        0        0     4150 2023-07-04 11:11:25.112905 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/datasets/dataset.py
--rw-r--r--   0        0        0      748 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/export_.py
--rw-r--r--   0        0        0     4945 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/import_.py
--rw-r--r--   0        0        0     3048 2023-07-12 06:34:06.220418 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/project.py
--rw-r--r--   0        0        0      960 2023-03-13 20:41:11.947729 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/resources/__init__.py
--rw-r--r--   0        0        0     6089 2023-06-30 07:12:28.298457 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/resources/resource.py
--rw-r--r--   0        0        0     2292 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/python.py
--rw-r--r--   0        0        0     1075 2023-02-13 06:43:43.973698 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/search/__init__.py
--rw-r--r--   0        0        0     2087 2023-07-03 04:00:36.674661 cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/tasks/__init__.py
--rw-r--r--   0        0        0     2277 2023-07-12 07:18:39.277978 cmem_cmempy-23.1.2rc2/pyproject.toml
--rw-r--r--   0        0        0     2324 1970-01-01 00:00:00.000000 cmem_cmempy-23.1.2rc2/setup.py
--rw-r--r--   0        0        0     2087 1970-01-01 00:00:00.000000 cmem_cmempy-23.1.2rc2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/LICENSE
+-rw-r--r--   0        0        0      651 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/README-public.md
+-rw-r--r--   0        0        0      110 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/__init__.py
+-rw-r--r--   0        0        0       40 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/__init__.py
+-rw-r--r--   0        0        0     4456 2023-03-13 20:41:10.321409 cmem_cmempy-23.2/cmem/cmempy/api.py
+-rw-r--r--   0        0        0     4970 2023-04-20 02:23:22.587855 cmem_cmempy-23.2/cmem/cmempy/config.py
+-rw-r--r--   0        0        0     1062 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/custom_tasks/__init__.py
+-rw-r--r--   0        0        0       36 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/dp/__init__.py
+-rw-r--r--   0        0        0     1029 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/dp/admin/__init__.py
+-rw-r--r--   0        0        0     1014 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/dp/admin/backup.py
+-rw-r--r--   0        0        0       42 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/dp/authorization/__init__.py
+-rw-r--r--   0        0        0     1232 2023-06-13 04:36:20.815472 cmem_cmempy-23.2/cmem/cmempy/dp/authorization/conditions.py
+-rw-r--r--   0        0        0      477 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/dp/authorization/refresh.py
+-rw-r--r--   0        0        0      380 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/dp/proxy/__init__.py
+-rw-r--r--   0        0        0     6036 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/dp/proxy/graph.py
+-rw-r--r--   0        0        0     4159 2023-04-05 05:42:13.535848 cmem_cmempy-23.2/cmem/cmempy/dp/proxy/sparql.py
+-rw-r--r--   0        0        0     1244 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/dp/proxy/update.py
+-rw-r--r--   0        0        0     1011 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/dp/titles/__init__.py
+-rw-r--r--   0        0        0     5905 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/health/__init__.py
+-rw-r--r--   0        0        0     1807 2023-07-12 06:39:11.632730 cmem_cmempy-23.2/cmem/cmempy/keycloak/client.py
+-rw-r--r--   0        0        0      519 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/keycloak/group.py
+-rw-r--r--   0        0        0     4500 2023-07-03 02:44:15.523722 cmem_cmempy-23.2/cmem/cmempy/keycloak/user.py
+-rw-r--r--   0        0        0       31 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/linking/__init__.py
+-rw-r--r--   0        0        0     2588 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/linking/linkingtask.py
+-rw-r--r--   0        0        0       26 2023-02-07 06:35:02.875189 cmem_cmempy-23.2/cmem/cmempy/plugins/__init__.py
+-rw-r--r--   0        0        0     1939 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/plugins/marshalling.py
+-rw-r--r--   0        0        0    11190 2023-02-08 20:16:15.346057 cmem_cmempy-23.2/cmem/cmempy/queries/__init__.py
+-rw-r--r--   0        0        0       33 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/transform/__init__.py
+-rw-r--r--   0        0        0     1090 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/transform/rules/__init__.py
+-rw-r--r--   0        0        0     1075 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/transform/rules/transformationrule.py
+-rw-r--r--   0        0        0     1240 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/transform/transformationtask.py
+-rw-r--r--   0        0        0     3597 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/vocabularies/__init__.py
+-rw-r--r--   0        0        0      731 2023-06-30 10:59:54.272591 cmem_cmempy-23.2/cmem/cmempy/workflow/__init__.py
+-rw-r--r--   0        0        0     4891 2023-07-03 04:05:53.557967 cmem_cmempy-23.2/cmem/cmempy/workflow/workflow.py
+-rw-r--r--   0        0        0      131 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workflow/workflows.py
+-rw-r--r--   0        0        0     1873 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/__init__.py
+-rw-r--r--   0        0        0      340 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/activities/__init__.py
+-rw-r--r--   0        0        0      914 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/activities/projectactivities.py
+-rw-r--r--   0        0        0     2281 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/activities/projectactivity.py
+-rw-r--r--   0        0        0     3164 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/activities/taskactivities.py
+-rw-r--r--   0        0        0     2323 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/activities/taskactivity.py
+-rw-r--r--   0        0        0      744 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/export_/__init__.py
+-rw-r--r--   0        0        0     1540 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/import_/__init__.py
+-rw-r--r--   0        0        0      454 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/projects/__init__.py
+-rw-r--r--   0        0        0       45 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/projects/datasets/__init__.py
+-rw-r--r--   0        0        0     4150 2023-07-11 06:39:45.826583 cmem_cmempy-23.2/cmem/cmempy/workspace/projects/datasets/dataset.py
+-rw-r--r--   0        0        0      748 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/projects/export_.py
+-rw-r--r--   0        0        0     4945 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/projects/import_.py
+-rw-r--r--   0        0        0     3048 2023-07-12 02:44:41.482542 cmem_cmempy-23.2/cmem/cmempy/workspace/projects/project.py
+-rw-r--r--   0        0        0      960 2023-03-13 20:41:10.321409 cmem_cmempy-23.2/cmem/cmempy/workspace/projects/resources/__init__.py
+-rw-r--r--   0        0        0     6089 2023-06-27 06:16:57.855962 cmem_cmempy-23.2/cmem/cmempy/workspace/projects/resources/resource.py
+-rw-r--r--   0        0        0     2292 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/python.py
+-rw-r--r--   0        0        0     1075 2023-02-07 06:35:02.879189 cmem_cmempy-23.2/cmem/cmempy/workspace/search/__init__.py
+-rw-r--r--   0        0        0     2087 2023-07-03 04:05:53.561967 cmem_cmempy-23.2/cmem/cmempy/workspace/tasks/__init__.py
+-rw-r--r--   0        0        0     2272 2023-07-12 12:34:31.764911 cmem_cmempy-23.2/pyproject.toml
+-rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 cmem_cmempy-23.2/setup.py
+-rw-r--r--   0        0        0     2082 1970-01-01 00:00:00.000000 cmem_cmempy-23.2/PKG-INFO
```

### Comparing `cmem_cmempy-23.1.2rc2/LICENSE` & `cmem_cmempy-23.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/README-public.md` & `cmem_cmempy-23.2/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/api.py` & `cmem_cmempy-23.2/cmem/cmempy/api.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/config.py` & `cmem_cmempy-23.2/cmem/cmempy/config.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/custom_tasks/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/custom_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/admin/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/dp/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/admin/backup.py` & `cmem_cmempy-23.2/cmem/cmempy/dp/admin/backup.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/authorization/conditions.py` & `cmem_cmempy-23.2/cmem/cmempy/dp/authorization/conditions.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/proxy/graph.py` & `cmem_cmempy-23.2/cmem/cmempy/dp/proxy/graph.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/proxy/sparql.py` & `cmem_cmempy-23.2/cmem/cmempy/dp/proxy/sparql.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/proxy/update.py` & `cmem_cmempy-23.2/cmem/cmempy/dp/proxy/update.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/dp/titles/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/dp/titles/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/health/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/health/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/keycloak/client.py` & `cmem_cmempy-23.2/cmem/cmempy/keycloak/client.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/keycloak/group.py` & `cmem_cmempy-23.2/cmem/cmempy/keycloak/group.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/keycloak/user.py` & `cmem_cmempy-23.2/cmem/cmempy/keycloak/user.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/linking/linkingtask.py` & `cmem_cmempy-23.2/cmem/cmempy/linking/linkingtask.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/plugins/marshalling.py` & `cmem_cmempy-23.2/cmem/cmempy/plugins/marshalling.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/queries/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/transform/rules/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/transform/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/transform/rules/transformationrule.py` & `cmem_cmempy-23.2/cmem/cmempy/transform/rules/transformationrule.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/transform/transformationtask.py` & `cmem_cmempy-23.2/cmem/cmempy/transform/transformationtask.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/vocabularies/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workflow/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workflow/workflow.py` & `cmem_cmempy-23.2/cmem/cmempy/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/activities/projectactivities.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/activities/projectactivities.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/activities/projectactivity.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/activities/projectactivity.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/activities/taskactivities.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/activities/taskactivities.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/activities/taskactivity.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/activities/taskactivity.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/export_/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/export_/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/import_/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/import_/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/datasets/dataset.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/projects/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/export_.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/projects/export_.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/import_.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/projects/import_.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/project.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/projects/project.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/resources/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/projects/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/projects/resources/resource.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/projects/resources/resource.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/python.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/python.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/search/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/search/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/cmem/cmempy/workspace/tasks/__init__.py` & `cmem_cmempy-23.2/cmem/cmempy/workspace/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1.2rc2/pyproject.toml` & `cmem_cmempy-23.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-cmempy"
-version = "23.1.2rc2"
+version = "23.2"
 license = "Apache-2.0"
 description = "API for eccenca Corporate Memory"
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 maintainers = ["Sebastian Tramp <sebastian.tramp@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `cmem_cmempy-23.1.2rc2/setup.py` & `cmem_cmempy-23.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
  'requests-toolbelt>=0.10.1,<0.11.0',
  'requests>=2.31.0,<3.0.0',
  'six>=1.16.0,<2.0.0',
  'urllib3>=1.26.15,<2.0.0']
 
 setup_kwargs = {
     'name': 'cmem-cmempy',
-    'version': '23.1.2rc2',
+    'version': '23.2',
     'description': 'API for eccenca Corporate Memory',
     'long_description': '# cmempy\n\ncmempy is a Python API wrapper for [eccenca Corporate Memory](https://documentation.eccenca.com/).\n\n## Installation\n\nTo install the Python library run:\n\n    pip install cmem-cmempy\n\nYou may consider installing the package only for the current user:\n\n    pip install cmem-cmempy --user\n\n## Configuration and Usage\n\ncmempy is intended for Linked Data Experts to interface with the eccenca Corporate Memory backend components DataIntegration and DataPlatform.\n\nThe cmempy manual including basic usage patterns and configuration is available at:\n\n[https://eccenca.com/go/cmempy](https://eccenca.com/go/cmempy)\n\ncmempy is tests with python >3.9.\n',
     'author': 'eccenca GmbH',
     'author_email': 'cmempy-developer@eccenca.com',
     'maintainer': 'Sebastian Tramp',
     'maintainer_email': 'sebastian.tramp@eccenca.com',
     'url': 'https://eccenca.com/go/cmempy',
```

### Comparing `cmem_cmempy-23.1.2rc2/PKG-INFO` & `cmem_cmempy-23.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-cmempy
-Version: 23.1.2rc2
+Version: 23.2
 Summary: API for eccenca Corporate Memory
 Home-page: https://eccenca.com/go/cmempy
 License: Apache-2.0
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Maintainer: Sebastian Tramp
 Maintainer-email: sebastian.tramp@eccenca.com
```


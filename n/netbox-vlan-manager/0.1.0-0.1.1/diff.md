# Comparing `tmp/netbox-vlan-manager-0.1.0.tar.gz` & `tmp/netbox-vlan-manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-vlan-manager-0.1.0.tar", last modified: Wed Jun 28 12:51:33 2023, max compression
+gzip compressed data, was "netbox-vlan-manager-0.1.1.tar", last modified: Wed Jul 12 13:48:05 2023, max compression
```

## Comparing `netbox-vlan-manager-0.1.0.tar` & `netbox-vlan-manager-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:51:33.876083 netbox-vlan-manager-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-28 12:51:33.876083 netbox-vlan-manager-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:51:33.876083 netbox-vlan-manager-0.1.0/netbox_vlan_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:51:33.876083 netbox-vlan-manager-0.1.0/netbox_vlan_manager/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:51:33.876083 netbox-vlan-manager-0.1.0/netbox_vlan_manager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:51:33.876083 netbox-vlan-manager-0.1.0/netbox_vlan_manager/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/templatetags/view_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:51:33.876083 netbox-vlan-manager-0.1.0/netbox_vlan_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-28 12:51:33.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-28 12:51:33.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 12:51:33.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 12:51:33.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-28 12:51:33.000000 netbox-vlan-manager-0.1.0/netbox_vlan_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 12:51:33.876083 netbox-vlan-manager-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-28 12:51:23.000000 netbox-vlan-manager-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:48:05.611223 netbox-vlan-manager-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-12 13:48:05.611223 netbox-vlan-manager-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:48:05.611223 netbox-vlan-manager-0.1.1/netbox_vlan_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:48:05.611223 netbox-vlan-manager-0.1.1/netbox_vlan_manager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:48:05.611223 netbox-vlan-manager-0.1.1/netbox_vlan_manager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:48:05.611223 netbox-vlan-manager-0.1.1/netbox_vlan_manager/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/templatetags/view_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:48:05.611223 netbox-vlan-manager-0.1.1/netbox_vlan_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-12 13:48:05.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-12 13:48:05.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:48:05.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:48:05.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-12 13:48:05.000000 netbox-vlan-manager-0.1.1/netbox_vlan_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:48:05.611223 netbox-vlan-manager-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-12 13:47:55.000000 netbox-vlan-manager-0.1.1/setup.py
```

### Comparing `netbox-vlan-manager-0.1.0/LICENSE` & `netbox-vlan-manager-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.0/PKG-INFO` & `netbox-vlan-manager-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-vlan-manager
-Version: 0.1.0
+Version: 0.1.1
 Summary: VLAN Manager for multiple VLAN Groups
 Home-page: https://github.com/miyuk/netbox-vlan-manager/
 Author: miyuk
 Author-email: miyuk@miyuk.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `netbox-vlan-manager-0.1.0/README.md` & `netbox-vlan-manager-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.0/netbox_vlan_manager/api/serializers.py` & `netbox-vlan-manager-0.1.1/netbox_vlan_manager/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.0/netbox_vlan_manager/api/views.py` & `netbox-vlan-manager-0.1.1/netbox_vlan_manager/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.0/netbox_vlan_manager/forms.py` & `netbox-vlan-manager-0.1.1/netbox_vlan_manager/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.0/netbox_vlan_manager/migrations/0001_initial.py` & `netbox-vlan-manager-0.1.1/netbox_vlan_manager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.0/netbox_vlan_manager/models.py` & `netbox-vlan-manager-0.1.1/netbox_vlan_manager/models.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.0/netbox_vlan_manager/navigation.py` & `netbox-vlan-manager-0.1.1/netbox_vlan_manager/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.0/netbox_vlan_manager/tables.py` & `netbox-vlan-manager-0.1.1/netbox_vlan_manager/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.0/netbox_vlan_manager/urls.py` & `netbox-vlan-manager-0.1.1/netbox_vlan_manager/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.0/netbox_vlan_manager/views.py` & `netbox-vlan-manager-0.1.1/netbox_vlan_manager/views.py`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.0/netbox_vlan_manager.egg-info/PKG-INFO` & `netbox-vlan-manager-0.1.1/netbox_vlan_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-vlan-manager
-Version: 0.1.0
+Version: 0.1.1
 Summary: VLAN Manager for multiple VLAN Groups
 Home-page: https://github.com/miyuk/netbox-vlan-manager/
 Author: miyuk
 Author-email: miyuk@miyuk.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `netbox-vlan-manager-0.1.0/netbox_vlan_manager.egg-info/SOURCES.txt` & `netbox-vlan-manager-0.1.1/netbox_vlan_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-vlan-manager-0.1.0/setup.py` & `netbox-vlan-manager-0.1.1/setup.py`

 * *Files identical despite different names*


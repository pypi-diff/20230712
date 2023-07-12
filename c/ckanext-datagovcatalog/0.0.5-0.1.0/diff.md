# Comparing `tmp/ckanext-datagovcatalog-0.0.5.tar.gz` & `tmp/ckanext-datagovcatalog-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-datagovcatalog-0.0.5.tar", last modified: Wed Oct 26 15:55:23 2022, max compression
+gzip compressed data, was "ckanext-datagovcatalog-0.1.0.tar", last modified: Wed Jul 12 17:30:05 2023, max compression
```

## Comparing `ckanext-datagovcatalog-0.0.5.tar` & `ckanext-datagovcatalog-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:55:23.290128 ckanext-datagovcatalog-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)    34499 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7790 2022-10-26 15:55:23.290128 ckanext-datagovcatalog-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5881 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:55:23.286128 ckanext-datagovcatalog-0.0.5/ckanext/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:55:23.286128 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:55:23.286128 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/harvester/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/harvester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/harvester/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:55:23.290128 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/helpers/packages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2888 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:55:23.290128 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2517 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/tests/test_before_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     3561 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     2716 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/tests/test_package_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/tests/test_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 15:55:23.290128 ckanext-datagovcatalog-0.0.5/ckanext_datagovcatalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7790 2022-10-26 15:55:23.000000 ckanext-datagovcatalog-0.0.5/ckanext_datagovcatalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      857 2022-10-26 15:55:23.000000 ckanext-datagovcatalog-0.0.5/ckanext_datagovcatalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 15:55:23.000000 ckanext-datagovcatalog-0.0.5/ckanext_datagovcatalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-10-26 15:55:23.000000 ckanext-datagovcatalog-0.0.5/ckanext_datagovcatalog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-26 15:55:23.000000 ckanext-datagovcatalog-0.0.5/ckanext_datagovcatalog.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-26 15:55:23.000000 ckanext-datagovcatalog-0.0.5/ckanext_datagovcatalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-10-26 15:55:23.290128 ckanext-datagovcatalog-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3723 2022-10-26 15:55:22.000000 ckanext-datagovcatalog-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:30:05.513079 ckanext-datagovcatalog-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34499 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-12 17:30:05.513079 ckanext-datagovcatalog-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:30:05.513079 ckanext-datagovcatalog-0.1.0/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:30:05.513079 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:30:05.513079 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/harvester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/harvester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/harvester/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:30:05.513079 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/helpers/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:30:05.513079 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/tests/test_before_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/tests/test_package_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:30:05.513079 ckanext-datagovcatalog-0.1.0/ckanext_datagovcatalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-12 17:30:05.000000 ckanext-datagovcatalog-0.1.0/ckanext_datagovcatalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-12 17:30:05.000000 ckanext-datagovcatalog-0.1.0/ckanext_datagovcatalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:30:05.000000 ckanext-datagovcatalog-0.1.0/ckanext_datagovcatalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-12 17:30:05.000000 ckanext-datagovcatalog-0.1.0/ckanext_datagovcatalog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 17:30:05.000000 ckanext-datagovcatalog-0.1.0/ckanext_datagovcatalog.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 17:30:05.000000 ckanext-datagovcatalog-0.1.0/ckanext_datagovcatalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-12 17:30:05.513079 ckanext-datagovcatalog-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-12 17:30:02.000000 ckanext-datagovcatalog-0.1.0/setup.py
```

### Comparing `ckanext-datagovcatalog-0.0.5/LICENSE` & `ckanext-datagovcatalog-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-datagovcatalog-0.0.5/README.md` & `ckanext-datagovcatalog-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 [comment]: <> (Add any additional install steps to the list below.
    For example installing any non-Python dependencies or adding any required
    config settings.)
 
 CKAN version | Compatibility
 ------------ | -------------
 <=2.8        | no
-2.9          | yes
+2.9          | 0.0.5 (last supported)
+2.10         | >=0.1.0
 
 To install ckanext-datagovcatalog:
 
 1. Activate your CKAN virtual environment, for example::
 
      `. /usr/lib/ckan/default/bin/activate`
 
@@ -119,15 +120,15 @@
 The existing development environment assumes a minimal catalog.data.gov test setup. This makes
 it difficult to develop and test against dependencies with other extensions.
 
 In order to support multiple versions of CKAN, or even upgrade to new versions
 of CKAN, we support development and testing through the `CKAN_VERSION`
 environment variable.
 
-    $ make CKAN_VERSION=2.9 test
+    $ make CKAN_VERSION=2.10 test
 
 # Registering ckanext-datagovcatalog on PyPI
 
 ckanext-datagovcatalog should be availabe on PyPI as
 https://pypi.python.org/pypi/ckanext-datagovcatalog. If that link doesn't work, then
 you can register the project on PyPI for the first time by following these
 steps:
```

### Comparing `ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/harvester/notifications.py` & `ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/harvester/notifications.py`

 * *Files identical despite different names*

### Comparing `ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/helpers/packages.py` & `ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/helpers/packages.py`

 * *Files identical despite different names*

### Comparing `ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/plugin.py` & `ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def get_actions(self):
         return {
             "harvest_get_notifications_recipients": harvest_get_notifications_recipients
         }
 
     # IPackageController
 
-    def before_view(self, pkg_dict):
+    def before_dataset_view(self, pkg_dict):
 
         # Add tracking information just for datasets
         if pkg_dict.get("type", "dataset") == "dataset":
             if toolkit.asbool(
                 config.get("ckanext.datagovcatalog.add_packages_tracking_info", True)
             ):
                 # add tracking information.
@@ -60,24 +60,28 @@
         return pkg_dict
 
     # Need to modify the schema to match import
     #  function that customizes tag validation
     def create_package_schema(self):
         # let's grab the default schema from CKAN
         schema = logic.schema.default_create_package_schema()
-        schema["tags"].update({"name": [not_empty, str]})
+        schema["tags"].update({"name": [not_empty, string]})
         return schema
 
     def update_package_schema(self):
         # let's grab the default schema from CKAN
         schema = logic.schema.default_update_package_schema()
-        schema["tags"].update({"name": [not_empty, str]})
+        schema["tags"].update({"name": [not_empty, string]})
         log.error("Trying to update package schema %s" % schema["tags"])
         return schema
 
     def is_fallback(self):
         return True
 
     def package_types(self):
         # This plugin doesn't handle any special package types, it just
         # customizes tag validation (see above)
         return []
+
+
+def string(value):
+    return str(value)
```

### Comparing `ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/tests/test_before_view.py` & `ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/tests/test_before_view.py`

 * *Files identical despite different names*

### Comparing `ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/tests/test_notifications.py` & `ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/tests/test_notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     def test_create_harvest_source_with_no_org(self):
         context, source_id = self._create_harvest_source_with_no_org()
 
         new_rec_action = toolkit.get_action("harvest_get_notifications_recipients")
         new_recipients = new_rec_action(context, {'source_id': source_id})
 
-        assert {'name': u'test.ckan.net', 'email': None} in new_recipients
+        assert new_recipients == []
 
     def _create_harvest_source_with_no_org(self):
         site_user = toolkit.get_action('get_site_user')(
             {'model': model, 'ignore_auth': True}, {})['name']
 
         context = {
             'user': site_user,
```

### Comparing `ckanext-datagovcatalog-0.0.5/ckanext/datagovcatalog/tests/test_package_list.py` & `ckanext-datagovcatalog-0.1.0/ckanext/datagovcatalog/tests/test_package_list.py`

 * *Files identical despite different names*

### Comparing `ckanext-datagovcatalog-0.0.5/ckanext_datagovcatalog.egg-info/SOURCES.txt` & `ckanext-datagovcatalog-0.1.0/ckanext_datagovcatalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-datagovcatalog-0.0.5/setup.cfg` & `ckanext-datagovcatalog-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ckanext-datagovcatalog-0.0.5/setup.py` & `ckanext-datagovcatalog-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 setup(
     name='''ckanext-datagovcatalog''',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version='0.0.5',
+    version='0.1.0',
 
     description='''Catalog customizations''',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
     url='https://github.com/GSA/ckanext-datagovcatalog',
```


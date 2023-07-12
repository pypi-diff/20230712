# Comparing `tmp/os2mo_data_import-5.4.1.tar.gz` & `tmp/os2mo_data_import-5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2mo_data_import-5.4.1.tar", max compression
+gzip compressed data, was "os2mo_data_import-5.4.2.tar", max compression
```

## Comparing `os2mo_data_import-5.4.1.tar` & `os2mo_data_import-5.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0        0        0        0 2023-07-10 12:46:39.778113 os2mo_data_import-5.4.1/LICENSES/
--rw-r--r--   0        0        0    11696 2023-07-10 12:46:39.779114 os2mo_data_import-5.4.1/README.rst
--rw-r--r--   0        0        0      332 2023-07-10 12:46:39.779114 os2mo_data_import-5.4.1/mox_helpers/__init__.py
--rw-r--r--   0        0        0     7243 2023-07-10 12:46:39.779114 os2mo_data_import-5.4.1/mox_helpers/mox_helper.py
--rw-r--r--   0        0        0    20756 2023-07-10 12:46:39.779114 os2mo_data_import-5.4.1/mox_helpers/mox_util.py
--rw-r--r--   0        0        0     2736 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/mox_helpers/payloads.py
--rw-r--r--   0        0        0       40 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/mox_helpers/requirements.txt
--rw-r--r--   0        0        0      899 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/mox_helpers/utils.py
--rw-r--r--   0        0        0      397 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/os2mo_data_import/__init__.py
--rw-r--r--   0        0        0     3799 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/os2mo_data_import/caching_import.py
--rw-r--r--   0        0        0     1300 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/os2mo_data_import/defaults.py
--rw-r--r--   0        0        0    19484 2023-07-10 12:46:39.780114 os2mo_data_import-5.4.1/os2mo_data_import/helpers.py
--rw-r--r--   0        0        0    22987 2023-07-10 12:46:39.781114 os2mo_data_import-5.4.1/os2mo_data_import/mora_data_types.py
--rw-r--r--   0        0        0    13436 2023-07-10 12:46:39.781114 os2mo_data_import-5.4.1/os2mo_data_import/mox_data_types.py
--rw-r--r--   0        0        0       99 2023-07-10 12:46:39.781114 os2mo_data_import-5.4.1/os2mo_data_import/tests/__init__.py
--rw-r--r--   0        0        0     1650 2023-07-10 12:46:39.781114 os2mo_data_import-5.4.1/os2mo_data_import/tests/test_utilities.py
--rw-r--r--   0        0        0    27431 2023-07-10 12:46:39.782114 os2mo_data_import-5.4.1/os2mo_data_import/utilities.py
--rw-r--r--   0        0        0      332 2023-07-10 12:46:39.782114 os2mo_data_import-5.4.1/os2mo_helpers/__init__.py
--rw-r--r--   0        0        0    30591 2023-07-10 12:46:39.782114 os2mo_data_import-5.4.1/os2mo_helpers/mora_helpers.py
--rw-r--r--   0        0        0       41 2023-07-10 12:46:39.782114 os2mo_data_import-5.4.1/os2mo_helpers/requirements.txt
--rw-r--r--   0        0        0     1169 2023-07-10 12:46:39.783114 os2mo_data_import-5.4.1/os2mo_helpers/settings.py
--rw-r--r--   0        0        0       99 2023-07-10 12:46:39.783114 os2mo_data_import-5.4.1/os2mo_helpers/tests/__init__.py
--rw-r--r--   0        0        0     3412 2023-07-10 12:46:39.783114 os2mo_data_import-5.4.1/os2mo_helpers/tests/test_morahelpers.py
--rw-r--r--   0        0        0     1054 2023-07-10 12:46:41.055231 os2mo_data_import-5.4.1/pyproject.toml
--rw-r--r--   0        0        0    13094 1970-01-01 00:00:00.000000 os2mo_data_import-5.4.1/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-07-12 08:33:05.131478 os2mo_data_import-5.4.2/LICENSES/
+-rw-r--r--   0        0        0    11696 2023-07-12 08:33:05.132479 os2mo_data_import-5.4.2/README.rst
+-rw-r--r--   0        0        0      332 2023-07-12 08:33:05.132479 os2mo_data_import-5.4.2/mox_helpers/__init__.py
+-rw-r--r--   0        0        0     7243 2023-07-12 08:33:05.132479 os2mo_data_import-5.4.2/mox_helpers/mox_helper.py
+-rw-r--r--   0        0        0    20756 2023-07-12 08:33:05.133478 os2mo_data_import-5.4.2/mox_helpers/mox_util.py
+-rw-r--r--   0        0        0     2736 2023-07-12 08:33:05.133478 os2mo_data_import-5.4.2/mox_helpers/payloads.py
+-rw-r--r--   0        0        0       40 2023-07-12 08:33:05.133478 os2mo_data_import-5.4.2/mox_helpers/requirements.txt
+-rw-r--r--   0        0        0      899 2023-07-12 08:33:05.133478 os2mo_data_import-5.4.2/mox_helpers/utils.py
+-rw-r--r--   0        0        0      397 2023-07-12 08:33:05.133478 os2mo_data_import-5.4.2/os2mo_data_import/__init__.py
+-rw-r--r--   0        0        0     3799 2023-07-12 08:33:05.133478 os2mo_data_import-5.4.2/os2mo_data_import/caching_import.py
+-rw-r--r--   0        0        0     1300 2023-07-12 08:33:05.133478 os2mo_data_import-5.4.2/os2mo_data_import/defaults.py
+-rw-r--r--   0        0        0    19484 2023-07-12 08:33:05.134479 os2mo_data_import-5.4.2/os2mo_data_import/helpers.py
+-rw-r--r--   0        0        0    22987 2023-07-12 08:33:05.134479 os2mo_data_import-5.4.2/os2mo_data_import/mora_data_types.py
+-rw-r--r--   0        0        0    13436 2023-07-12 08:33:05.134479 os2mo_data_import-5.4.2/os2mo_data_import/mox_data_types.py
+-rw-r--r--   0        0        0       99 2023-07-12 08:33:05.134479 os2mo_data_import-5.4.2/os2mo_data_import/tests/__init__.py
+-rw-r--r--   0        0        0     1650 2023-07-12 08:33:05.135479 os2mo_data_import-5.4.2/os2mo_data_import/tests/test_utilities.py
+-rw-r--r--   0        0        0    27431 2023-07-12 08:33:05.135479 os2mo_data_import-5.4.2/os2mo_data_import/utilities.py
+-rw-r--r--   0        0        0      332 2023-07-12 08:33:05.135479 os2mo_data_import-5.4.2/os2mo_helpers/__init__.py
+-rw-r--r--   0        0        0    30670 2023-07-12 08:33:05.135479 os2mo_data_import-5.4.2/os2mo_helpers/mora_helpers.py
+-rw-r--r--   0        0        0       41 2023-07-12 08:33:05.136479 os2mo_data_import-5.4.2/os2mo_helpers/requirements.txt
+-rw-r--r--   0        0        0     1169 2023-07-12 08:33:05.136479 os2mo_data_import-5.4.2/os2mo_helpers/settings.py
+-rw-r--r--   0        0        0       99 2023-07-12 08:33:05.136479 os2mo_data_import-5.4.2/os2mo_helpers/tests/__init__.py
+-rw-r--r--   0        0        0     3412 2023-07-12 08:33:05.136479 os2mo_data_import-5.4.2/os2mo_helpers/tests/test_morahelpers.py
+-rw-r--r--   0        0        0     1054 2023-07-12 08:33:06.303578 os2mo_data_import-5.4.2/pyproject.toml
+-rw-r--r--   0        0        0    13094 1970-01-01 00:00:00.000000 os2mo_data_import-5.4.2/PKG-INFO
```

### Comparing `os2mo_data_import-5.4.1/README.rst` & `os2mo_data_import-5.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/mox_helpers/mox_helper.py` & `os2mo_data_import-5.4.2/mox_helpers/mox_helper.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/mox_helpers/mox_util.py` & `os2mo_data_import-5.4.2/mox_helpers/mox_util.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/mox_helpers/payloads.py` & `os2mo_data_import-5.4.2/mox_helpers/payloads.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/mox_helpers/utils.py` & `os2mo_data_import-5.4.2/mox_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/os2mo_data_import/caching_import.py` & `os2mo_data_import-5.4.2/os2mo_data_import/caching_import.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/os2mo_data_import/defaults.py` & `os2mo_data_import-5.4.2/os2mo_data_import/defaults.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/os2mo_data_import/helpers.py` & `os2mo_data_import-5.4.2/os2mo_data_import/helpers.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/os2mo_data_import/mora_data_types.py` & `os2mo_data_import-5.4.2/os2mo_data_import/mora_data_types.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/os2mo_data_import/mox_data_types.py` & `os2mo_data_import-5.4.2/os2mo_data_import/mox_data_types.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/os2mo_data_import/tests/test_utilities.py` & `os2mo_data_import-5.4.2/os2mo_data_import/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/os2mo_data_import/utilities.py` & `os2mo_data_import-5.4.2/os2mo_data_import/utilities.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/os2mo_helpers/mora_helpers.py` & `os2mo_data_import-5.4.2/os2mo_helpers/mora_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -624,82 +624,82 @@
             # TODO: Fix this...
             # raise Exception('Too many managers')
         return manager
 
     def read_organisation_people(
         self,
         org_uuid,
-        person_type="engagement",
+        function_type="engagement",
         split_name=True,
         read_all=False,
         skip_past=False,
     ):
         """Read all employees in an ou. If the same employee is listed
         more than once, only the latest listing will be included.
-        :param org_uuid: UUID of the OU to find emplyees in.
+        :param org_uuid: UUID of the OU to find employees in.
         :read_all: Read all engagements, not only the present ones.
-        :return: The list of emplyoees
+        :return: The list of employees
         """
         person_list = {}
         if not read_all:
-            all_persons = self._mo_lookup(org_uuid, "ou/{}/details/" + person_type)
+            all_functions = self._mo_lookup(org_uuid, "ou/{}/details/" + function_type)
         else:
             if skip_past:
                 validity_times = ["present", "future"]
             else:
                 validity_times = ["past", "present", "future"]
 
-            all_persons = []
+            all_functions = []
             for validity in validity_times:
-                persons = self._mo_lookup(
-                    org_uuid, "ou/{}/details/" + person_type, validity=validity
+                functions = self._mo_lookup(
+                    org_uuid, "ou/{}/details/" + function_type, validity=validity
                 )
-                all_persons = all_persons + persons
+                all_functions = all_functions + functions
 
-        for person in all_persons:
-            if not person:
+        for function in all_functions:
+            if function["person"] is None:
                 # Vacant association
                 continue
-            uuid = person["person"]["uuid"]
+            uuid = function["person"]["uuid"]
             data = {
-                "Ansættelse gyldig fra": person["validity"]["from"],
-                "Ansættelse gyldig til": person["validity"]["to"],
+                "Ansættelse gyldig fra": function["validity"]["from"],
+                "Ansættelse gyldig til": function["validity"]["to"],
                 "Person UUID": uuid,
-                "Org-enhed": person["org_unit"]["name"],
-                "Org-enhed UUID": person["org_unit"]["uuid"],
-                "Engagement UUID": person["uuid"],
+                "Org-enhed": function["org_unit"]["name"],
+                "Org-enhed UUID": function["org_unit"]["uuid"],
+                "Engagement UUID": function["uuid"],
             }
-            if "job_function" in person and person["job_function"] is not None:
-                data["Stillingsbetegnelse"] = person["job_function"]["name"]
+            if "job_function" in function and function["job_function"] is not None:
+                data["Stillingsbetegnelse"] = function["job_function"]["name"]
             else:
                 data["Stillingsbetegnelse"] = None
 
-            if "engagement_type" in person and person["engagement_type"] is not None:
-                data["engagement_type_uuid"] = person["engagement_type"]["uuid"]
-                data["Engagementstype"] = person["engagement_type"]["name"]
+            if "engagement_type" in function and function["engagement_type"] is not None:
+                data["engagement_type_uuid"] = function["engagement_type"]["uuid"]
+                data["Engagementstype"] = function["engagement_type"]["name"]
             else:
                 data["engagement_type_uuid"] = None
                 data["Engagementstype"] = None
 
-            if "association_type" in person and person["association_type"] is not None:
-                data["Post"] = person["association_type"]["name"]
+            if "association_type" in function and function["association_type"] is not None:
+                data["Post"] = function["association_type"]["name"]
             else:
                 data["Post"] = None
 
             # Finally, add name
             if split_name:
                 # If a split name i wanted, we prefer to get i directly from MO
                 # rather than an algorithmic split.
-                if person["person"].get("givenname"):
-                    data["Fornavn"] = person["person"].get("givenname")
-                    data["Efternavn"] = person["person"].get("surname")
+                if function["person"].get("givenname"):
+                    data["Fornavn"] = function["person"].get("givenname")
+                    data["Efternavn"] = function["person"].get("surname")
                 else:
                     data.update(self._split_name(person["person"]["name"]))
             else:
-                data["Navn"] = person["person"]["name"]
+                data["Navn"] = function["person"]["name"]
             person_list[uuid] = data
         return person_list
 
     def read_top_units(self, organisation, use_cache=False):
         """Read the ous tha refers directoly to the organisation
         :param organisation: UUID of the organisation
         :return: List of UUIDs of the root OUs in the organisation
```

### Comparing `os2mo_data_import-5.4.1/os2mo_helpers/settings.py` & `os2mo_data_import-5.4.2/os2mo_helpers/settings.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/os2mo_helpers/tests/test_morahelpers.py` & `os2mo_data_import-5.4.2/os2mo_helpers/tests/test_morahelpers.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.4.1/pyproject.toml` & `os2mo_data_import-5.4.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "os2mo_data_import"
-version = "5.4.1"
+version = "5.4.2"
 description = "A set of tools for OS2MO data import and export"
 authors = ["Magenta <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.rst"
 repository = "https://git.magenta.dk/rammearkitektur/os2mo_data_import"
 keywords = ["os2mo", "dipex"]
 packages = [
```

### Comparing `os2mo_data_import-5.4.1/PKG-INFO` & `os2mo_data_import-5.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2mo-data-import
-Version: 5.4.1
+Version: 5.4.2
 Summary: A set of tools for OS2MO data import and export
 Home-page: https://git.magenta.dk/rammearkitektur/os2mo_data_import
 License: MPL-2.0
 Keywords: os2mo,dipex
 Author: Magenta
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
```


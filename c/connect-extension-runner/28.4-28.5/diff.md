# Comparing `tmp/connect_extension_runner-28.4.tar.gz` & `tmp/connect_extension_runner-28.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_extension_runner-28.4.tar", max compression
+gzip compressed data, was "connect_extension_runner-28.5.tar", max compression
```

## Comparing `connect_extension_runner-28.4.tar` & `connect_extension_runner-28.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11357 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/LICENSE
--rw-r--r--   0        0        0     1422 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/README.md
--rw-r--r--   0        0        0       55 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/connect/eaas/dataclasses.py
--rw-r--r--   0        0        0      405 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/connect/eaas/extension.py
--rw-r--r--   0        0        0      143 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/connect/eaas/runner/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/connect/eaas/runner/artworks/__init__.py
--rw-r--r--   0        0        0     9409 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/connect/eaas/runner/artworks/ansi_regular.flf
--rw-r--r--   0        0        0      950 2023-07-07 07:58:30.067178 connect_extension_runner-28.4/connect/eaas/runner/artworks/banner.py
--rw-r--r--   0        0        0    11425 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/artworks/bloody.flf
--rw-r--r--   0        0        0     6483 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/config.py
--rw-r--r--   0        0        0     5708 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/constants.py
--rw-r--r--   0        0        0      320 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/handlers/__init__.py
--rw-r--r--   0        0        0     2692 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/handlers/anvil.py
--rw-r--r--   0        0        0     4391 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/handlers/base.py
--rw-r--r--   0        0        0     3751 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/handlers/events.py
--rw-r--r--   0        0        0     2444 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/handlers/transformations.py
--rw-r--r--   0        0        0     7175 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/handlers/web.py
--rw-r--r--   0        0        0    18982 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/helpers.py
--rw-r--r--   0        0        0     1989 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/main.py
--rw-r--r--   0        0        0      340 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/__init__.py
--rw-r--r--   0        0        0     3190 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/background.py
--rw-r--r--   0        0        0     8100 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/base.py
--rw-r--r--   0        0        0     2225 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/interactive.py
--rw-r--r--   0        0        0     1931 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/scheduled.py
--rw-r--r--   0        0        0    20665 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/transformation.py
--rw-r--r--   0        0        0      533 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/managers/utils.py
--rw-r--r--   0        0        0     7917 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/master.py
--rw-r--r--   0        0        0        0 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/workers/__init__.py
--rw-r--r--   0        0        0     2549 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/workers/anvil.py
--rw-r--r--   0        0        0    11320 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/workers/base.py
--rw-r--r--   0        0        0     8834 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/workers/events.py
--rw-r--r--   0        0        0     6545 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/workers/transformations.py
--rw-r--r--   0        0        0     7038 2023-07-07 07:58:30.071178 connect_extension_runner-28.4/connect/eaas/runner/workers/web.py
--rw-r--r--   0        0        0     2870 2023-07-07 07:59:44.431392 connect_extension_runner-28.4/pyproject.toml
--rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 connect_extension_runner-28.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/LICENSE
+-rw-r--r--   0        0        0     1422 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/README.md
+-rw-r--r--   0        0        0       55 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/dataclasses.py
+-rw-r--r--   0        0        0      405 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/extension.py
+-rw-r--r--   0        0        0      143 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/artworks/__init__.py
+-rw-r--r--   0        0        0     9409 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/artworks/ansi_regular.flf
+-rw-r--r--   0        0        0      950 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/artworks/banner.py
+-rw-r--r--   0        0        0    11425 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/artworks/bloody.flf
+-rw-r--r--   0        0        0     6483 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/config.py
+-rw-r--r--   0        0        0     5708 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/constants.py
+-rw-r--r--   0        0        0      320 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/handlers/__init__.py
+-rw-r--r--   0        0        0     2692 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/handlers/anvil.py
+-rw-r--r--   0        0        0     4391 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/handlers/base.py
+-rw-r--r--   0        0        0     3751 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/handlers/events.py
+-rw-r--r--   0        0        0     2444 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/handlers/transformations.py
+-rw-r--r--   0        0        0     7133 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/handlers/web.py
+-rw-r--r--   0        0        0    18982 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/helpers.py
+-rw-r--r--   0        0        0     1989 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/main.py
+-rw-r--r--   0        0        0      340 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/__init__.py
+-rw-r--r--   0        0        0     3190 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/background.py
+-rw-r--r--   0        0        0     8100 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/base.py
+-rw-r--r--   0        0        0     2225 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/interactive.py
+-rw-r--r--   0        0        0     1931 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/scheduled.py
+-rw-r--r--   0        0        0    20665 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/transformation.py
+-rw-r--r--   0        0        0      533 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/managers/utils.py
+-rw-r--r--   0        0        0     7917 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/master.py
+-rw-r--r--   0        0        0        0 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/workers/__init__.py
+-rw-r--r--   0        0        0     2549 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/workers/anvil.py
+-rw-r--r--   0        0        0    11320 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/workers/base.py
+-rw-r--r--   0        0        0     8834 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/workers/events.py
+-rw-r--r--   0        0        0     6545 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/workers/transformations.py
+-rw-r--r--   0        0        0     7038 2023-07-12 11:06:03.445947 connect_extension_runner-28.5/connect/eaas/runner/workers/web.py
+-rw-r--r--   0        0        0     2870 2023-07-12 11:07:21.439286 connect_extension_runner-28.5/pyproject.toml
+-rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 connect_extension_runner-28.5/PKG-INFO
```

### Comparing `connect_extension_runner-28.4/LICENSE` & `connect_extension_runner-28.5/LICENSE`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/README.md` & `connect_extension_runner-28.5/README.md`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/artworks/ansi_regular.flf` & `connect_extension_runner-28.5/connect/eaas/runner/artworks/ansi_regular.flf`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/artworks/banner.py` & `connect_extension_runner-28.5/connect/eaas/runner/artworks/banner.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/artworks/bloody.flf` & `connect_extension_runner-28.5/connect/eaas/runner/artworks/bloody.flf`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/config.py` & `connect_extension_runner-28.5/connect/eaas/runner/config.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/constants.py` & `connect_extension_runner-28.5/connect/eaas/runner/constants.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/handlers/anvil.py` & `connect_extension_runner-28.5/connect/eaas/runner/handlers/anvil.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/handlers/base.py` & `connect_extension_runner-28.5/connect/eaas/runner/handlers/base.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/handlers/events.py` & `connect_extension_runner-28.5/connect/eaas/runner/handlers/events.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/handlers/transformations.py` & `connect_extension_runner-28.5/connect/eaas/runner/handlers/transformations.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/handlers/web.py` & `connect_extension_runner-28.5/connect/eaas/runner/handlers/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,14 @@
                 'integration_point': 'Installations Admin',
             })
 
         for customer in self.ui_modules.get('customer', []):
             components.append({
                 'name': customer['label'],
                 'url': customer['url'],
-                'icon': customer['icon'],
                 'integration_point': 'Customer Home Page',
             })
 
         return components
 
     def get_endpoints(self):
         auth, no_auth = self.get_application().get_routers()
```

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/helpers.py` & `connect_extension_runner-28.5/connect/eaas/runner/helpers.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/main.py` & `connect_extension_runner-28.5/connect/eaas/runner/main.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/managers/background.py` & `connect_extension_runner-28.5/connect/eaas/runner/managers/background.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/managers/base.py` & `connect_extension_runner-28.5/connect/eaas/runner/managers/base.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/managers/interactive.py` & `connect_extension_runner-28.5/connect/eaas/runner/managers/interactive.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/managers/scheduled.py` & `connect_extension_runner-28.5/connect/eaas/runner/managers/scheduled.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/managers/transformation.py` & `connect_extension_runner-28.5/connect/eaas/runner/managers/transformation.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/managers/utils.py` & `connect_extension_runner-28.5/connect/eaas/runner/managers/utils.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/master.py` & `connect_extension_runner-28.5/connect/eaas/runner/master.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/workers/anvil.py` & `connect_extension_runner-28.5/connect/eaas/runner/workers/anvil.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/workers/base.py` & `connect_extension_runner-28.5/connect/eaas/runner/workers/base.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/workers/events.py` & `connect_extension_runner-28.5/connect/eaas/runner/workers/events.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/workers/transformations.py` & `connect_extension_runner-28.5/connect/eaas/runner/workers/transformations.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/connect/eaas/runner/workers/web.py` & `connect_extension_runner-28.5/connect/eaas/runner/workers/web.py`

 * *Files identical despite different names*

### Comparing `connect_extension_runner-28.4/pyproject.toml` & `connect_extension_runner-28.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-extension-runner"
-version = "28.4"
+version = "28.5"
 description = "CloudBlue Connect EaaS Extension Runner"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "connect" },
 ]
 readme = "./README.md"
```

### Comparing `connect_extension_runner-28.4/PKG-INFO` & `connect_extension_runner-28.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-extension-runner
-Version: 28.4
+Version: 28.5
 Summary: CloudBlue Connect EaaS Extension Runner
 Home-page: https://connect.cloudblue.com
 License: Apache-2.0
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```


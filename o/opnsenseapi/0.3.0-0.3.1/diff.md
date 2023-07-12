# Comparing `tmp/opnsenseapi-0.3.0.tar.gz` & `tmp/opnsenseapi-0.3.1.tar.gz`

## Comparing `opnsenseapi-0.3.0.tar` & `opnsenseapi-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.flake8
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/GITHUB_CHANGELOG.md
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/cog.toml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/package.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/.gitignore
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/misc.xml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/modules.xml
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/opnsenseapi.iml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/vcs.xml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/__init__.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/opnsense.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/ifaces/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/ifaces/opnsense.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/unbound/__init__.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/unbound/host_override.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/unbound/host_override_test.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/LICENSE
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/README.md
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.flake8
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/GITHUB_CHANGELOG.md
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/cog.toml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/package.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/.gitignore
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/modules.xml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/opnsenseapi.iml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/vcs.xml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/__init__.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/opnsense.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/ifaces/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/ifaces/opnsense.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/unbound/__init__.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/unbound/host_override.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/opnsenseapi/unbound/host_override_test.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/LICENSE
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/README.md
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 opnsenseapi-0.3.1/PKG-INFO
```

### Comparing `opnsenseapi-0.3.0/.readthedocs.yaml` & `opnsenseapi-0.3.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.3.0/CHANGELOG.md` & `opnsenseapi-0.3.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 All notable changes to this project will be documented in this file. See [conventional commits](https://www.conventionalcommits.org/) for commit guidelines.
 
 - - -
+## 0.3.1 - 2023-07-12
+#### Bug Fixes
+- issue with mxprio in host overrides - (5a2bf2f) - eBeyond
+- Fixed numeric error while using mxprio - (d9d3e77) - eBeyond
+
+- - -
+
 ## 0.3.0 - 2023-07-12
 #### Continuous Integration
 - restructured ci build - (d420865) - eBeyond
 - restructured ci build - (0c03d01) - eBeyond
 - restructured ci build - (44b8145) - eBeyond
 - restructured ci build - (d957897) - eBeyond
 - restructured ci build - (bdbd0d4) - eBeyond
```

### Comparing `opnsenseapi-0.3.0/cog.toml` & `opnsenseapi-0.3.1/cog.toml`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.3.0/opnsenseapi/opnsense.py` & `opnsenseapi-0.3.1/opnsenseapi/opnsense.py`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.3.0/opnsenseapi/unbound/host_override.py` & `opnsenseapi-0.3.1/opnsenseapi/unbound/host_override.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-
+import math
 from opnsenseapi.ifaces.opnsense import _OpnSense
 
 
 class Host:
     id: str
     enabled: bool
     hostname: str
@@ -27,15 +27,18 @@
         self.enabled = enabled
         self.hostname = hostname
         self.domain = domain
         self.rr = rr
         self.server = server
         self.description = description
         self.mx = mx
-        self.mxprio = mxprio
+        if mxprio:
+            self.mxprio = math.trunc(mxprio)
+        else:
+            self.mxprio = 0
         self.id = id
 
     def __eq__(self, other):
         if isinstance(self, other.__class__):
             return \
                     self.enabled == other.enabled and \
                     self.hostname == other.hostname and \
```

### Comparing `opnsenseapi-0.3.0/opnsenseapi/unbound/host_override_test.py` & `opnsenseapi-0.3.1/opnsenseapi/unbound/host_override_test.py`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.3.0/.gitignore` & `opnsenseapi-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.3.0/LICENSE` & `opnsenseapi-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.3.0/pyproject.toml` & `opnsenseapi-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.3.0/PKG-INFO` & `opnsenseapi-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opnsenseapi
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python API for access the opnsense api
 Project-URL: Documentation, https://opnsenseapi.readthedocs.io/
 Project-URL: Changelog, https://opnsenseapi.readthedocs.io/en/latest/changelog.html
 Project-URL: Homepage, https://opnsenseapi.pypa.io/latest/
 Project-URL: History, https://opnsenseapi.pypa.io/dev/history/opnsenseapi/
 Project-URL: Tracker, https://github.com/oss4u/opnsenseapi/issues
 Project-URL: Source, https://github.com/oss4u/opnsenseapi
```


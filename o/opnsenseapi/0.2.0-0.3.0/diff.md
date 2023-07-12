# Comparing `tmp/opnsenseapi-0.2.0.tar.gz` & `tmp/opnsenseapi-0.3.0.tar.gz`

## Comparing `opnsenseapi-0.2.0.tar` & `opnsenseapi-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/.flake8
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/GITHUB_CHANGELOG.md
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/cog.toml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/package.json
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/.idea/.gitignore
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/.idea/misc.xml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/.idea/modules.xml
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/.idea/opnsenseapi.iml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/.idea/vcs.xml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/opnsenseapi/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/opnsenseapi/__init__.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/opnsenseapi/opnsense.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/opnsenseapi/ifaces/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/opnsenseapi/ifaces/opnsense.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/opnsenseapi/unbound/__init__.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/opnsenseapi/unbound/host_override.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/opnsenseapi/unbound/host_override_test.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/LICENSE
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/README.md
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 opnsenseapi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.flake8
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/GITHUB_CHANGELOG.md
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/cog.toml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/package.json
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/.gitignore
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/modules.xml
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/opnsenseapi.iml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/vcs.xml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/__init__.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/opnsense.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/ifaces/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/ifaces/opnsense.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/unbound/__init__.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/unbound/host_override.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/opnsenseapi/unbound/host_override_test.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/LICENSE
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/README.md
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 opnsenseapi-0.3.0/PKG-INFO
```

### Comparing `opnsenseapi-0.2.0/CHANGELOG.md` & `opnsenseapi-0.3.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # Changelog
 All notable changes to this project will be documented in this file. See [conventional commits](https://www.conventionalcommits.org/) for commit guidelines.
 
 - - -
+## 0.3.0 - 2023-07-12
+#### Continuous Integration
+- restructured ci build - (d420865) - eBeyond
+- restructured ci build - (0c03d01) - eBeyond
+- restructured ci build - (44b8145) - eBeyond
+- restructured ci build - (d957897) - eBeyond
+- restructured ci build - (bdbd0d4) - eBeyond
+- restructured ci build - (71c2b00) - eBeyond
+- restructured ci build - (ba54c20) - eBeyond
+- fixed issues with release - (d3bac6b) - eBeyond
+#### Features
+- modified return of get, read, delete - (c0462d4) - eBeyond
+
+- - -
+
 ## 0.2.0 - 2023-07-12
 #### Features
 - Added functionality to host overrides (CRUD) - (720a51f) - eBeyond
 
 - - -
 
 ## 0.1.0 - 2023-07-12
```

### Comparing `opnsenseapi-0.2.0/cog.toml` & `opnsenseapi-0.3.0/cog.toml`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.2.0/opnsenseapi/opnsense.py` & `opnsenseapi-0.3.0/opnsenseapi/opnsense.py`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.2.0/opnsenseapi/unbound/host_override.py` & `opnsenseapi-0.3.0/opnsenseapi/unbound/host_override.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,44 +69,51 @@
             return host
         else:
             print(f"ERROR: {result}")
             return host
 
     def read(self, id: str):
         result = self.ctrl.non_modifying_request(self.module, self.controller, 'getHostOverride', params=[id])
-        print(result)
+        if len(result) > 0:
+            return self.create_host_from_json(result)
+        else:
+            raise Exception("No hosts found.")
 
     def update(self, host: Host):
         data = self.create_json_from_host(host)
         result = self.ctrl.modifying_request(self.module, self.controller, 'setHostOverride', data=data, params=[host.id])
         print(f"RES: {result}")
         if result['result'] == "saved":
             return host
         else:
-            print(f"ERROR: {result}")
-            return host
+            raise Exception(f"Error updating host: {result}")
 
-    def delete(self, host: Host):
-        result = self.ctrl.modifying_request(self.module, self.controller, 'delHostOverride', params=[host.id])
-        print(result)
+    def delete_by_host(self, host: Host):
+        return self.delete_by_id(host.id)
+
+    def delete_by_id(self, id: str):
+        result = self.ctrl.modifying_request(self.module, self.controller, 'delHostOverride', params=[id])
+        if result['result'] == 'deleted':
+            return True
+        else:
+            return False
 
     def get(self, id):
-        result = self.ctrl.non_modifying_request(self.module, self.controller, 'getHostOverride', params=[id])
-        print(result)
+        return self.read(id)
 
     def list(self):
         result = self.ctrl.non_modifying_request(self.module, self.controller, 'searchHostOverride')
         print(result)
 
     def search(self):
         result = self.ctrl.non_modifying_request(self.module, self.controller, 'searchHostOverride')
         print(result)
 
     def create_host_from_json(self, result_json):
-        host_json = json.loads(result_json)['host']
+        host_json = result_json['host']
         if host_json['enabled'] == "1":
             enabled = True
         else:
             enabled = False
         if len(host_json['mxprio']) > 0:
             mxprio = host_json['mxprio']
         else:
```

### Comparing `opnsenseapi-0.2.0/opnsenseapi/unbound/host_override_test.py` & `opnsenseapi-0.3.0/opnsenseapi/unbound/host_override_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                 "rr": "A",
                 "mxprio": "",
                 "mx": "",
                 "server": "10.10.10.10",
                 "description": "descr"
             }
         }, indent=2)
-        result = ho.create_host_from_json(test)
+        result = ho.create_host_from_json(json.loads(test))
 
         print(result)
         print(expected)
 
         self.assertEqual(result, expected)  # add assertion here
 
     def test_json_to_host(self):
```

### Comparing `opnsenseapi-0.2.0/.gitignore` & `opnsenseapi-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.2.0/LICENSE` & `opnsenseapi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.2.0/pyproject.toml` & `opnsenseapi-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opnsenseapi-0.2.0/PKG-INFO` & `opnsenseapi-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opnsenseapi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python API for access the opnsense api
 Project-URL: Documentation, https://opnsenseapi.readthedocs.io/
 Project-URL: Changelog, https://opnsenseapi.readthedocs.io/en/latest/changelog.html
 Project-URL: Homepage, https://opnsenseapi.pypa.io/latest/
 Project-URL: History, https://opnsenseapi.pypa.io/dev/history/opnsenseapi/
 Project-URL: Tracker, https://github.com/oss4u/opnsenseapi/issues
 Project-URL: Source, https://github.com/oss4u/opnsenseapi
```


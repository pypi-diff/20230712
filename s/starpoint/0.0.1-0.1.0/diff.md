# Comparing `tmp/starpoint-0.0.1.tar.gz` & `tmp/starpoint-0.1.0.tar.gz`

## Comparing `starpoint-0.0.1.tar` & `starpoint-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 starpoint-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starpoint-0.0.1/starpoint/__init__.py
--rw-r--r--   0        0        0     9595 2020-02-02 00:00:00.000000 starpoint-0.0.1/starpoint/db.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 starpoint-0.0.1/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 starpoint-0.0.1/LICENSE
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 starpoint-0.0.1/README.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 starpoint-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 starpoint-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 starpoint-0.1.0/.coverage
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 starpoint-0.1.0/dev-requirements.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 starpoint-0.1.0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starpoint-0.1.0/starpoint/__init__.py
+-rw-r--r--   0        0        0    17838 2020-02-02 00:00:00.000000 starpoint-0.1.0/starpoint/db.py
+-rw-r--r--   0        0        0    26905 2020-02-02 00:00:00.000000 starpoint-0.1.0/tests/test_db.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 starpoint-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 starpoint-0.1.0/LICENSE
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 starpoint-0.1.0/README.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 starpoint-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 starpoint-0.1.0/PKG-INFO
```

### Comparing `starpoint-0.0.1/LICENSE` & `starpoint-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starpoint-0.0.1/README.md` & `starpoint-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `starpoint-0.0.1/PKG-INFO` & `starpoint-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: starpoint
-Version: 0.0.1
+Version: 0.1.0
 Summary: SDK for Starpoint DB
 Project-URL: Homepage, https://github.com/starpoint-ai/sdk
 Project-URL: Bug Tracker, https://github.com/starpoint-ai/sdk/issues
-Author-email: pointable <support@pointable.ai>
+Author-email: pointable <package-maintainers@pointable.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: requests~=2.28
 Requires-Dist: validators~=0.20
```


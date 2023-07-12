# Comparing `tmp/pmg-1.0.0rc4.tar.gz` & `tmp/pmg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmg-1.0.0rc4.tar", last modified: Sun Aug  7 17:54:31 2022, max compression
+gzip compressed data, was "pmg-1.0.1.tar", last modified: Wed Jul 12 17:35:27 2023, max compression
```

## Comparing `pmg-1.0.0rc4.tar` & `pmg-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxrwxr-x   0 gm        (1000) gm        (1000)        0 2022-08-07 17:54:31.221984 pmg-1.0.0rc4/
--rw-rw-r--   0 gm        (1000) gm        (1000)     1086 2022-07-25 11:43:49.000000 pmg-1.0.0rc4/LICENSE
--rw-rw-r--   0 gm        (1000) gm        (1000)     1238 2022-08-07 17:54:31.221984 pmg-1.0.0rc4/PKG-INFO
--rw-rw-r--   0 gm        (1000) gm        (1000)      676 2022-07-25 16:00:44.000000 pmg-1.0.0rc4/README.md
-drwxrwxr-x   0 gm        (1000) gm        (1000)        0 2022-08-07 17:54:31.221984 pmg-1.0.0rc4/pmg/
--rw-rw-r--   0 gm        (1000) gm        (1000)    12579 2022-08-07 17:50:43.000000 pmg-1.0.0rc4/pmg/__init__.py
--rw-rw-r--   0 gm        (1000) gm        (1000)      693 2021-05-02 12:21:23.000000 pmg-1.0.0rc4/pmg/base36.py
--rw-rw-r--   0 gm        (1000) gm        (1000)     1525 2022-08-07 10:36:02.000000 pmg-1.0.0rc4/pmg/db.py
--rw-rw-r--   0 gm        (1000) gm        (1000)      362 2022-07-25 17:39:34.000000 pmg-1.0.0rc4/pmg/latex.py
-drwxrwxr-x   0 gm        (1000) gm        (1000)        0 2022-08-07 17:54:31.221984 pmg-1.0.0rc4/pmg/sqlite/
--rw-rw-r--   0 gm        (1000) gm        (1000)     1461 2022-08-07 17:44:28.000000 pmg-1.0.0rc4/pmg/sqlite/__init__.py
--rw-rw-r--   0 gm        (1000) gm        (1000)      422 2022-07-25 15:16:43.000000 pmg-1.0.0rc4/pmg/sqlite/factories.py
--rw-rw-r--   0 gm        (1000) gm        (1000)     3136 2022-08-07 17:41:07.000000 pmg-1.0.0rc4/pmg/sqlite/queues.py
--rw-rw-r--   0 gm        (1000) gm        (1000)      972 2022-08-07 10:36:02.000000 pmg-1.0.0rc4/pmg/system.py
--rw-rw-r--   0 gm        (1000) gm        (1000)      635 2022-07-25 17:41:28.000000 pmg-1.0.0rc4/pmg/temp.py
-drwxrwxr-x   0 gm        (1000) gm        (1000)        0 2022-08-07 17:54:31.221984 pmg-1.0.0rc4/pmg.egg-info/
--rw-rw-r--   0 gm        (1000) gm        (1000)     1238 2022-08-07 17:54:31.000000 pmg-1.0.0rc4/pmg.egg-info/PKG-INFO
--rw-rw-r--   0 gm        (1000) gm        (1000)      322 2022-08-07 17:54:31.000000 pmg-1.0.0rc4/pmg.egg-info/SOURCES.txt
--rw-rw-r--   0 gm        (1000) gm        (1000)        1 2022-08-07 17:54:31.000000 pmg-1.0.0rc4/pmg.egg-info/dependency_links.txt
--rw-rw-r--   0 gm        (1000) gm        (1000)       26 2022-08-07 17:54:31.000000 pmg-1.0.0rc4/pmg.egg-info/requires.txt
--rw-rw-r--   0 gm        (1000) gm        (1000)        4 2022-08-07 17:54:31.000000 pmg-1.0.0rc4/pmg.egg-info/top_level.txt
--rw-rw-r--   0 gm        (1000) gm        (1000)      748 2022-08-07 10:36:02.000000 pmg-1.0.0rc4/pyproject.toml
--rw-rw-r--   0 gm        (1000) gm        (1000)       38 2022-08-07 17:54:31.221984 pmg-1.0.0rc4/setup.cfg
--rw-rw-r--   0 gm        (1000) gm        (1000)       38 2022-07-25 15:40:08.000000 pmg-1.0.0rc4/setup.py
+drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-12 17:35:27.964714 pmg-1.0.1/
+-rw-rw-r--   0 gm        (1000) gm        (1000)     1086 2022-07-25 11:43:49.000000 pmg-1.0.1/LICENSE
+-rw-r--r--   0 gm        (1000) gm        (1000)     1235 2023-07-12 17:35:27.964714 pmg-1.0.1/PKG-INFO
+-rw-rw-r--   0 gm        (1000) gm        (1000)      676 2022-07-25 16:00:44.000000 pmg-1.0.1/README.md
+drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-12 17:35:27.963714 pmg-1.0.1/pmg/
+-rw-r--r--   0 gm        (1000) gm        (1000)    13150 2023-07-12 17:34:09.000000 pmg-1.0.1/pmg/__init__.py
+-rw-rw-r--   0 gm        (1000) gm        (1000)      693 2021-05-02 12:21:23.000000 pmg-1.0.1/pmg/base36.py
+-rw-r--r--   0 gm        (1000) gm        (1000)     1525 2023-01-13 07:41:58.000000 pmg-1.0.1/pmg/db.py
+-rw-rw-r--   0 gm        (1000) gm        (1000)      362 2022-07-25 17:39:34.000000 pmg-1.0.1/pmg/latex.py
+drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-12 17:35:27.963714 pmg-1.0.1/pmg/sqlite/
+-rw-r--r--   0 gm        (1000) gm        (1000)     1461 2023-01-13 07:41:58.000000 pmg-1.0.1/pmg/sqlite/__init__.py
+-rw-rw-r--   0 gm        (1000) gm        (1000)      422 2022-07-25 15:16:43.000000 pmg-1.0.1/pmg/sqlite/factories.py
+-rw-r--r--   0 gm        (1000) gm        (1000)     3136 2023-01-13 07:41:58.000000 pmg-1.0.1/pmg/sqlite/queues.py
+-rw-r--r--   0 gm        (1000) gm        (1000)     1752 2023-02-12 22:02:56.000000 pmg-1.0.1/pmg/system.py
+-rw-rw-r--   0 gm        (1000) gm        (1000)      635 2022-07-25 17:41:28.000000 pmg-1.0.1/pmg/temp.py
+drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-12 17:35:27.963714 pmg-1.0.1/pmg.egg-info/
+-rw-rw-r--   0 gm        (1000) gm        (1000)     1235 2023-07-12 17:35:27.000000 pmg-1.0.1/pmg.egg-info/PKG-INFO
+-rw-rw-r--   0 gm        (1000) gm        (1000)      420 2023-07-12 17:35:27.000000 pmg-1.0.1/pmg.egg-info/SOURCES.txt
+-rw-rw-r--   0 gm        (1000) gm        (1000)        1 2023-07-12 17:35:27.000000 pmg-1.0.1/pmg.egg-info/dependency_links.txt
+-rw-rw-r--   0 gm        (1000) gm        (1000)       26 2023-07-12 17:35:27.000000 pmg-1.0.1/pmg.egg-info/requires.txt
+-rw-rw-r--   0 gm        (1000) gm        (1000)        4 2023-07-12 17:35:27.000000 pmg-1.0.1/pmg.egg-info/top_level.txt
+-rw-r--r--   0 gm        (1000) gm        (1000)      745 2023-07-12 14:11:15.000000 pmg-1.0.1/pyproject.toml
+-rw-r--r--   0 gm        (1000) gm        (1000)       38 2023-07-12 17:35:27.964714 pmg-1.0.1/setup.cfg
+-rw-rw-r--   0 gm        (1000) gm        (1000)       38 2022-07-25 15:40:08.000000 pmg-1.0.1/setup.py
+drwxr-xr-x   0 gm        (1000) gm        (1000)        0 2023-07-12 17:35:27.964714 pmg-1.0.1/tests/
+-rw-rw-r--   0 gm        (1000) gm        (1000)      372 2022-07-25 17:27:37.000000 pmg-1.0.1/tests/test_base36.py
+-rw-r--r--   0 gm        (1000) gm        (1000)     4604 2023-01-13 07:41:58.000000 pmg-1.0.1/tests/test_common.py
+-rw-r--r--   0 gm        (1000) gm        (1000)     1683 2023-01-13 07:41:58.000000 pmg-1.0.1/tests/test_db.py
+-rw-rw-r--   0 gm        (1000) gm        (1000)      241 2022-07-25 17:56:49.000000 pmg-1.0.1/tests/test_latex.py
+-rw-rw-r--   0 gm        (1000) gm        (1000)      358 2022-07-25 17:58:50.000000 pmg-1.0.1/tests/test_temp.py
```

### Comparing `pmg-1.0.0rc4/LICENSE` & `pmg-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pmg-1.0.0rc4/PKG-INFO` & `pmg-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmg
-Version: 1.0.0rc4
+Version: 1.0.1
 Summary: A toolbox full of handy little helper functions and utilities.
 Author-email: Preston Meyer Group <dev@pmgroup.ch>
 License: MIT
 Keywords: tools,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pmg-1.0.0rc4/README.md` & `pmg-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pmg-1.0.0rc4/pmg/__init__.py` & `pmg-1.0.1/pmg/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 def get_config_keys(pattern):
     return {k[4:]: v for k, v in os.environ.items() if k.startswith('PMG_') and fnmatch.fnmatch(k[4:], pattern)}
 
 
 # Global configuration variables
 
 ASCII_SUB = '\x1a'
+DEFAULT_CSV_DELIMITER = '\t'
 DEFAULT_HASH_ALGO = hashlib.sha1
 TRACE_LOG = get_config('TRACE_LOG', '0') == '1'
 
 # Object Helpers
 
 class Singleton(type):
     _instances = {}
@@ -163,14 +164,17 @@
 
 def hashfile(path, hash_algo=None):
     h = coalesce(hash_algo, DEFAULT_HASH_ALGO())
     with open(path, 'rb') as f:
         h.update(f.read())
     return h.hexdigest()
 
+def writetextfile(path, content):
+    with open(path, 'wt', encoding='utf-8', newline='') as g:
+        g.write(content)
 
 # String Helpers
 
 def mass_replace(s, replace_vars):
     if s is None:
         return s
     if not isinstance(replace_vars, dict):
@@ -288,20 +292,35 @@
     else:
         from_date = coalesce(from_date, datetime.datetime.now().date())
     return from_date + datetime.timedelta((weekday - from_date.weekday()) % 7)
 
 def get_seconds_until(target_dt, from_dt=None):
     return (target_dt - coalesce(from_dt, utcnow())).total_seconds()
 
+
 # System Helpers
 
 def get_exc_info():
     return '\n'.join(traceback.format_exception(*sys.exc_info()))
 
 
+# CSV Helpers
+def csv_to_namedtuples(path, **kwargs):
+    Record = None
+    if 'delimiter' not in kwargs:
+        kwargs.update({'delimiter': DEFAULT_FIELD_DELIMITER})
+    with open(path, 'rt') as f:
+        reader = csv.reader(f, **kwargs)
+        for i, r in enumerate(reader):
+            if i == 0:
+                Record = collections.namedtuple('Record', r)
+                continue
+            yield Record(*r)
+
+
 # JSON Helpers
 
 class FriendlyJsonEncoder(json.JSONEncoder):
     def default(self, o):
         try:
             if isinstance(o, decimal.Decimal):
                 return format(o, 'f')
```

### Comparing `pmg-1.0.0rc4/pmg/base36.py` & `pmg-1.0.1/pmg/base36.py`

 * *Files identical despite different names*

### Comparing `pmg-1.0.0rc4/pmg/db.py` & `pmg-1.0.1/pmg/db.py`

 * *Files identical despite different names*

### Comparing `pmg-1.0.0rc4/pmg/sqlite/__init__.py` & `pmg-1.0.1/pmg/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pmg-1.0.0rc4/pmg/sqlite/queues.py` & `pmg-1.0.1/pmg/sqlite/queues.py`

 * *Files identical despite different names*

### Comparing `pmg-1.0.0rc4/pmg/temp.py` & `pmg-1.0.1/pmg/temp.py`

 * *Files identical despite different names*

### Comparing `pmg-1.0.0rc4/pmg.egg-info/PKG-INFO` & `pmg-1.0.1/pmg.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmg
-Version: 1.0.0rc4
+Version: 1.0.1
 Summary: A toolbox full of handy little helper functions and utilities.
 Author-email: Preston Meyer Group <dev@pmgroup.ch>
 License: MIT
 Keywords: tools,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `pmg-1.0.0rc4/pyproject.toml` & `pmg-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pmg"
-version = "1.0.0rc4"
+version = "1.0.1"
 description = "A toolbox full of handy little helper functions and utilities."
 readme = "README.md"
 authors = [{ name = "Preston Meyer Group", email = "dev@pmgroup.ch" }]
 license = { text = "MIT" }
 classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
```


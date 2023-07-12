# Comparing `tmp/dataset-1.6.0.tar.gz` & `tmp/dataset-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-1.6.0.tar", last modified: Mon Jan 30 08:57:29 2023, max compression
+gzip compressed data, was "dataset-1.6.2.tar", last modified: Wed Jul 12 08:54:06 2023, max compression
```

## Comparing `dataset-1.6.0.tar` & `dataset-1.6.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 08:57:29.710595 dataset-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-30 08:56:58.000000 dataset-1.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-30 08:57:29.710595 dataset-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-30 08:56:58.000000 dataset-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 08:57:29.710595 dataset-1.6.0/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-01-30 08:56:58.000000 dataset-1.6.0/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-01-30 08:56:58.000000 dataset-1.6.0/dataset/chunked.py
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-01-30 08:56:58.000000 dataset-1.6.0/dataset/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    27494 2023-01-30 08:56:58.000000 dataset-1.6.0/dataset/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-01-30 08:56:58.000000 dataset-1.6.0/dataset/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-01-30 08:56:58.000000 dataset-1.6.0/dataset/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 08:57:29.710595 dataset-1.6.0/dataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-30 08:57:29.000000 dataset-1.6.0/dataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-30 08:57:29.000000 dataset-1.6.0/dataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 08:57:29.000000 dataset-1.6.0/dataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 08:57:29.000000 dataset-1.6.0/dataset.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 08:57:16.000000 dataset-1.6.0/dataset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-30 08:57:29.000000 dataset-1.6.0/dataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-30 08:57:29.000000 dataset-1.6.0/dataset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-30 08:57:29.710595 dataset-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-01-30 08:56:58.000000 dataset-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 08:57:29.710595 dataset-1.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    21908 2023-01-30 08:56:58.000000 dataset-1.6.0/test/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:54:06.273362 dataset-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-12 08:53:22.000000 dataset-1.6.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-12 08:54:06.273362 dataset-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-12 08:53:22.000000 dataset-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:54:06.273362 dataset-1.6.2/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-12 08:53:22.000000 dataset-1.6.2/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-12 08:53:22.000000 dataset-1.6.2/dataset/chunked.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-07-12 08:53:22.000000 dataset-1.6.2/dataset/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-07-12 08:53:22.000000 dataset-1.6.2/dataset/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-12 08:53:22.000000 dataset-1.6.2/dataset/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-12 08:53:22.000000 dataset-1.6.2/dataset/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:54:06.273362 dataset-1.6.2/dataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-12 08:54:06.000000 dataset-1.6.2/dataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-12 08:54:06.000000 dataset-1.6.2/dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:54:06.000000 dataset-1.6.2/dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:54:06.000000 dataset-1.6.2/dataset.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 08:53:42.000000 dataset-1.6.2/dataset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-12 08:54:06.000000 dataset-1.6.2/dataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 08:54:06.000000 dataset-1.6.2/dataset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-12 08:54:06.277362 dataset-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-12 08:53:22.000000 dataset-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 08:54:06.273362 dataset-1.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    21908 2023-07-12 08:53:22.000000 dataset-1.6.2/test/test_dataset.py
```

### Comparing `dataset-1.6.0/LICENSE.txt` & `dataset-1.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataset-1.6.0/PKG-INFO` & `dataset-1.6.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset
-Version: 1.6.0
+Version: 1.6.2
 Summary: Toolkit for Python-based database access.
 Home-page: http://github.com/pudo/dataset
 Author: Friedrich Lindenberg, Gregor Aisch, Stefan Wehrmeyer
 Author-email: friedrich.lindenberg@gmail.com
 License: MIT
 Keywords: sql sqlalchemy etl loading utility
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dataset-1.6.0/README.md` & `dataset-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `dataset-1.6.0/dataset/__init__.py` & `dataset-1.6.2/dataset/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # shut up useless SA warning:
 warnings.filterwarnings("ignore", "Unicode type received non-unicode bind param value.")
 warnings.filterwarnings(
     "ignore", "Skipping unsupported ALTER for creation of implicit constraint"
 )
 
 __all__ = ["Database", "Table", "connect"]
-__version__ = "1.6.0"
+__version__ = "1.6.2"
 
 
 def connect(
     url=None,
     schema=None,
     engine_kwargs=None,
     ensure_schema=True,
```

### Comparing `dataset-1.6.0/dataset/chunked.py` & `dataset-1.6.2/dataset/chunked.py`

 * *Files identical despite different names*

### Comparing `dataset-1.6.0/dataset/database.py` & `dataset-1.6.2/dataset/database.py`

 * *Files identical despite different names*

### Comparing `dataset-1.6.0/dataset/table.py` & `dataset-1.6.2/dataset/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,15 @@
                 self._columns = None
         elif len(columns):
             with self.db.lock:
                 self._reflect_table()
                 self._threading_warn()
                 for column in columns:
                     if not self.has_column(column.name):
-                        self.db.op.add_column(self.name, column, self.db.schema)
+                        self.db.op.add_column(self.name, column, schema=self.db.schema)
                 self._reflect_table()
 
     def _sync_columns(self, row, ensure, types=None):
         """Create missing columns (or the table) prior to writes.
 
         If automatic schema generation is disabled (``ensure`` is ``False``),
         this will remove any keys from the ``row`` for which there is no
@@ -505,15 +505,15 @@
         name = self._get_column_name(name)
         with self.db.lock:
             if not self.exists or not self.has_column(name):
                 log.debug("Column does not exist: %s", name)
                 return
 
             self._threading_warn()
-            self.db.op.drop_column(self.table.name, name, self.table.schema)
+            self.db.op.drop_column(self.table.name, name, schema=self.table.schema)
             self._reflect_table()
 
     def drop(self):
         """Drop the table from the database.
 
         Deletes both the schema and all the contents within it.
         """
```

### Comparing `dataset-1.6.0/dataset/types.py` & `dataset-1.6.2/dataset/types.py`

 * *Files identical despite different names*

### Comparing `dataset-1.6.0/dataset/util.py` & `dataset-1.6.2/dataset/util.py`

 * *Files identical despite different names*

### Comparing `dataset-1.6.0/dataset.egg-info/PKG-INFO` & `dataset-1.6.2/dataset.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset
-Version: 1.6.0
+Version: 1.6.2
 Summary: Toolkit for Python-based database access.
 Home-page: http://github.com/pudo/dataset
 Author: Friedrich Lindenberg, Gregor Aisch, Stefan Wehrmeyer
 Author-email: friedrich.lindenberg@gmail.com
 License: MIT
 Keywords: sql sqlalchemy etl loading utility
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dataset-1.6.0/setup.py` & `dataset-1.6.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="dataset",
-    version="1.6.0",
+    version="1.6.2",
     description="Toolkit for Python-based database access.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

### Comparing `dataset-1.6.0/test/test_dataset.py` & `dataset-1.6.2/test/test_dataset.py`

 * *Files identical despite different names*


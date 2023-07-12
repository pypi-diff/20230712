# Comparing `tmp/data-pyetl-1.0.26.tar.gz` & `tmp/data_pyetl-1.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-pyetl-1.0.26.tar", max compression
+gzip compressed data, was "data_pyetl-1.0.27.tar", max compression
```

## Comparing `data-pyetl-1.0.26.tar` & `data_pyetl-1.0.27.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1093 2022-04-11 19:06:26.702203 data-pyetl-1.0.26/LICENSE
--rw-r--r--   0        0        0       22 2022-04-11 19:06:26.702203 data-pyetl-1.0.26/data_pyetl/__init__.py
--rw-r--r--   0        0        0     1934 2022-04-11 19:06:26.702203 data-pyetl-1.0.26/data_pyetl/api_helper.py
--rw-r--r--   0        0        0     2463 2022-04-11 19:06:26.702203 data-pyetl-1.0.26/data_pyetl/connectors.py
--rw-r--r--   0        0        0     3165 2022-04-11 19:06:26.702203 data-pyetl-1.0.26/data_pyetl/database_helper.py
--rw-r--r--   0        0        0     2275 2022-04-11 19:06:26.702203 data-pyetl-1.0.26/data_pyetl/file_helper.py
--rw-r--r--   0        0        0     1142 2022-04-11 19:06:26.702203 data-pyetl-1.0.26/data_pyetl/loggin.py
--rw-r--r--   0        0        0     1125 2022-04-11 19:06:26.702203 data-pyetl-1.0.26/pyproject.toml
--rw-r--r--   0        0        0     1157 2022-04-11 19:08:10.704642 data-pyetl-1.0.26/setup.py
--rw-r--r--   0        0        0     1205 2022-04-11 19:08:10.704900 data-pyetl-1.0.26/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-07-12 14:11:50.761074 data_pyetl-1.0.27/LICENSE
+-rw-r--r--   0        0        0       22 2023-07-12 14:11:50.761074 data_pyetl-1.0.27/data_pyetl/__init__.py
+-rw-r--r--   0        0        0     1934 2023-07-12 14:11:50.761074 data_pyetl-1.0.27/data_pyetl/api_helper.py
+-rw-r--r--   0        0        0     2463 2023-07-12 14:11:50.761074 data_pyetl-1.0.27/data_pyetl/connectors.py
+-rw-r--r--   0        0        0     3165 2023-07-12 14:11:50.761074 data_pyetl-1.0.27/data_pyetl/database_helper.py
+-rw-r--r--   0        0        0     2524 2023-07-12 14:11:50.761074 data_pyetl-1.0.27/data_pyetl/file_helper.py
+-rw-r--r--   0        0        0     1142 2023-07-12 14:11:50.761074 data_pyetl-1.0.27/data_pyetl/loggin.py
+-rw-r--r--   0        0        0     1151 2023-07-12 14:11:50.761074 data_pyetl-1.0.27/pyproject.toml
+-rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 data_pyetl-1.0.27/PKG-INFO
```

### Comparing `data-pyetl-1.0.26/LICENSE` & `data_pyetl-1.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `data-pyetl-1.0.26/data_pyetl/api_helper.py` & `data_pyetl-1.0.27/data_pyetl/api_helper.py`

 * *Files identical despite different names*

### Comparing `data-pyetl-1.0.26/data_pyetl/connectors.py` & `data_pyetl-1.0.27/data_pyetl/connectors.py`

 * *Files identical despite different names*

### Comparing `data-pyetl-1.0.26/data_pyetl/database_helper.py` & `data_pyetl-1.0.27/data_pyetl/database_helper.py`

 * *Files identical despite different names*

### Comparing `data-pyetl-1.0.26/data_pyetl/file_helper.py` & `data_pyetl-1.0.27/data_pyetl/file_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,24 @@
         """
         try:
             df = pd.read_xml(self.filepath)
             return df
         except Exception as e:
             return e
 
+    def read_parquet_to_dataframe(self):
+        """
+        Read parquet file
+        """
+        try:
+            df = pd.read_parquet(self.filepath, engine='fastparquet')
+            return df
+        except Exception as e:
+            return e
+
     def dataframe_to_db(self, df, table_prefix, table_name, dw_con, dw_schema):
         """
         Save the worked pandas DataFrame to the source DW
         """
         df = df.replace("", np.nan)
         df = df.drop_duplicates()
```

### Comparing `data-pyetl-1.0.26/data_pyetl/loggin.py` & `data_pyetl-1.0.27/data_pyetl/loggin.py`

 * *Files identical despite different names*

### Comparing `data-pyetl-1.0.26/pyproject.toml` & `data_pyetl-1.0.27/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-pyetl"
-version = "1.0.26"
+version = "1.0.27"
 description = "Data Pyetl is an python approach to extract and load data from a source to a database"
 authors = ["MacSoares <macario.junior@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^1.4.1"
 numpy = "^1.22.3"
@@ -21,14 +21,15 @@
 requests-mock = "^1.9.3"
 pytest-cov = "^3.0.0"
 flake8 = "^4.0.1"
 openpyxl = "^3.0.9"
 lxml = "^4.8.0"
 odfpy = "^1.4.1"
 xlrd = "^2.0.1"
+fastparquet = "^2023.7.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `data-pyetl-1.0.26/PKG-INFO` & `data_pyetl-1.0.27/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: data-pyetl
-Version: 1.0.26
+Version: 1.0.27
 Summary: Data Pyetl is an python approach to extract and load data from a source to a database
 Author: MacSoares
 Author-email: macario.junior@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyMySQL (>=1.0.2,<2.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.32,<2.0.0)
 Requires-Dist: cx-Oracle (>=8.3.0,<9.0.0)
+Requires-Dist: fastparquet (>=2023.7.0,<2024.0.0)
 Requires-Dist: fdb (>=2.0.2,<3.0.0)
 Requires-Dist: flake8 (>=4.0.1,<5.0.0)
 Requires-Dist: ipython (>=8.1.1,<9.0.0)
 Requires-Dist: lxml (>=4.8.0,<5.0.0)
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: odfpy (>=1.4.1,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.9,<4.0.0)
```


# Comparing `tmp/querychart_package-2.0.4.tar.gz` & `tmp/querychart_package-2.0.5.tar.gz`

## Comparing `querychart_package-2.0.4.tar` & `querychart_package-2.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 querychart_package-2.0.4/test.csv
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 querychart_package-2.0.4/src/querychart_package/.schemawiz_config3
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 querychart_package-2.0.4/src/querychart_package/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 querychart_package-2.0.4/src/querychart_package/data.csv
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 querychart_package-2.0.4/src/querychart_package/fieldcounts.tsv
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 querychart_package-2.0.4/src/querychart_package/gant_data.csv
--rw-r--r--   0        0        0    11206 2020-02-02 00:00:00.000000 querychart_package-2.0.4/src/querychart_package/ganter.py
--rw-r--r--   0        0        0   200704 2020-02-02 00:00:00.000000 querychart_package-2.0.4/src/querychart_package/local_sqlite_db
--rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 querychart_package-2.0.4/src/querychart_package/plan.xlsx
--rw-r--r--   0        0        0    15999 2020-02-02 00:00:00.000000 querychart_package-2.0.4/src/querychart_package/querychart.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 querychart_package-2.0.4/src/querychart_package/sales.csv
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 querychart_package-2.0.4/src/querychart_package/sampledata.csv
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 querychart_package-2.0.4/src/querychart_package/widesales.csv
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 querychart_package-2.0.4/tests/.schemawiz_config3
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 querychart_package-2.0.4/tests/chart_csv_columns.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 querychart_package-2.0.4/tests/chart_csv_rows.py
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 querychart_package-2.0.4/tests/local_sqlite_db
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 querychart_package-2.0.4/tests/sales.csv
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 querychart_package-2.0.4/tests/tester.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 querychart_package-2.0.4/tests/widesales.csv
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 querychart_package-2.0.4/.gitignore
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 querychart_package-2.0.4/README.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 querychart_package-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 querychart_package-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 querychart_package-2.0.5/test.csv
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 querychart_package-2.0.5/src/querychart_package/.schemawiz_config3
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 querychart_package-2.0.5/src/querychart_package/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 querychart_package-2.0.5/src/querychart_package/data.csv
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 querychart_package-2.0.5/src/querychart_package/fieldcounts.tsv
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 querychart_package-2.0.5/src/querychart_package/gant_data.csv
+-rw-r--r--   0        0        0    11206 2020-02-02 00:00:00.000000 querychart_package-2.0.5/src/querychart_package/ganter.py
+-rw-r--r--   0        0        0   200704 2020-02-02 00:00:00.000000 querychart_package-2.0.5/src/querychart_package/local_sqlite_db
+-rw-r--r--   0        0        0     9981 2020-02-02 00:00:00.000000 querychart_package-2.0.5/src/querychart_package/plan.xlsx
+-rw-r--r--   0        0        0    15999 2020-02-02 00:00:00.000000 querychart_package-2.0.5/src/querychart_package/querychart.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 querychart_package-2.0.5/src/querychart_package/sales.csv
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 querychart_package-2.0.5/src/querychart_package/sampledata.csv
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 querychart_package-2.0.5/src/querychart_package/widesales.csv
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 querychart_package-2.0.5/tests/.schemawiz_config3
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 querychart_package-2.0.5/tests/chart_csv_columns.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 querychart_package-2.0.5/tests/chart_csv_rows.py
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 querychart_package-2.0.5/tests/local_sqlite_db
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 querychart_package-2.0.5/tests/sales.csv
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 querychart_package-2.0.5/tests/tester.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 querychart_package-2.0.5/tests/widesales.csv
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 querychart_package-2.0.5/.gitignore
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 querychart_package-2.0.5/README.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 querychart_package-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 querychart_package-2.0.5/PKG-INFO
```

### Comparing `querychart_package-2.0.4/src/querychart_package/data.csv` & `querychart_package-2.0.5/src/querychart_package/data.csv`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.4/src/querychart_package/ganter.py` & `querychart_package-2.0.5/src/querychart_package/ganter.py`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.4/src/querychart_package/local_sqlite_db` & `querychart_package-2.0.5/src/querychart_package/local_sqlite_db`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.4/src/querychart_package/plan.xlsx` & `querychart_package-2.0.5/src/querychart_package/plan.xlsx`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.4/src/querychart_package/querychart.py` & `querychart_package-2.0.5/src/querychart_package/querychart.py`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.4/src/querychart_package/sales.csv` & `querychart_package-2.0.5/src/querychart_package/sales.csv`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.4/src/querychart_package/sampledata.csv` & `querychart_package-2.0.5/src/querychart_package/sampledata.csv`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.4/tests/local_sqlite_db` & `querychart_package-2.0.5/tests/local_sqlite_db`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.4/tests/sales.csv` & `querychart_package-2.0.5/tests/sales.csv`

 * *Files identical despite different names*

### Comparing `querychart_package-2.0.4/pyproject.toml` & `querychart_package-2.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["hatchling","schemawizard_package","pandas"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "querychart_package"
-version = "2.0.4"
+version = "2.0.5"
 dependencies = [
+  'pandas',
   'schemawizard_package >= 2.3.5'
 ]
 authors = [
   { name="Dave Skura", email="dskura@gmail.com" },
 ]
 description = "A wrapper for simplified matplotlib usage"
 readme = "README.md"
```


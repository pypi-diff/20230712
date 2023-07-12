# Comparing `tmp/dq_module-1.1.4.tar.gz` & `tmp/dq_module-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dq_module-1.1.4.tar", last modified: Tue Jul  4 10:27:28 2023, max compression
+gzip compressed data, was "dist/dq_module-1.1.5.tar", last modified: Wed Jul 12 14:02:49 2023, max compression
```

## Comparing `dq_module-1.1.4.tar` & `dq_module-1.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:27:28.000000 dq_module-1.1.4/
--rw-r--r--   0 root         (0) root         (0)    13216 2023-07-04 10:27:28.000000 dq_module-1.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11346 2023-07-04 10:27:11.000000 dq_module-1.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:27:28.000000 dq_module-1.1.4/dataqualitycheck/
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11938 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/commonutilities.py
--rw-rw-rw-   0 root         (0) root         (0)    10482 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/consistencycheck.py
--rw-rw-rw-   0 root         (0) root         (0)    37781 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/dataprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:27:28.000000 dq_module-1.1.4/dataqualitycheck/datasources/
--rw-rw-rw-   0 root         (0) root         (0)     7917 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/datasources/azureblobdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2836 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/datasources/commonutilities.py
--rw-rw-rw-   0 root         (0) root         (0)     5534 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/datasources/databricksfilesystemdf.py
--rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/datasources/databrickssqldf.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/datasources/localfilesystemdf.py
--rw-rw-rw-   0 root         (0) root         (0)     5366 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/enumfile.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/singledatasetqualitycheck.py
--rw-rw-rw-   0 root         (0) root         (0)    42396 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/singledatasetqualitycheckpolars.py
--rw-rw-rw-   0 root         (0) root         (0)    40543 2023-07-04 10:27:11.000000 dq_module-1.1.4/dataqualitycheck/singledatasetqualitycheckspark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 10:27:28.000000 dq_module-1.1.4/dq_module.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13216 2023-07-04 10:27:28.000000 dq_module-1.1.4/dq_module.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      739 2023-07-04 10:27:28.000000 dq_module-1.1.4/dq_module.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 10:27:28.000000 dq_module-1.1.4/dq_module.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-04 10:27:28.000000 dq_module-1.1.4/dq_module.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-04 10:27:28.000000 dq_module-1.1.4/dq_module.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 10:27:28.000000 dq_module-1.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-07-04 10:27:11.000000 dq_module-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:02:49.000000 dq_module-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)    13216 2023-07-12 14:02:49.000000 dq_module-1.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11346 2023-07-12 14:02:39.000000 dq_module-1.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:02:49.000000 dq_module-1.1.5/dataqualitycheck/
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11938 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/commonutilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    10482 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/consistencycheck.py
+-rw-rw-rw-   0 root         (0) root         (0)    37781 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/dataprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:02:49.000000 dq_module-1.1.5/dataqualitycheck/datasources/
+-rw-rw-rw-   0 root         (0) root         (0)     7917 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/datasources/azureblobdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/datasources/commonutilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     5534 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/datasources/databricksfilesystemdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/datasources/databrickssqldf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/datasources/localfilesystemdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5366 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/enumfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/singledatasetqualitycheck.py
+-rw-rw-rw-   0 root         (0) root         (0)    42396 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/singledatasetqualitycheckpolars.py
+-rw-rw-rw-   0 root         (0) root         (0)    50981 2023-07-12 14:02:39.000000 dq_module-1.1.5/dataqualitycheck/singledatasetqualitycheckspark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:02:49.000000 dq_module-1.1.5/dq_module.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13216 2023-07-12 14:02:49.000000 dq_module-1.1.5/dq_module.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      739 2023-07-12 14:02:49.000000 dq_module-1.1.5/dq_module.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 14:02:49.000000 dq_module-1.1.5/dq_module.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-12 14:02:49.000000 dq_module-1.1.5/dq_module.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-12 14:02:49.000000 dq_module-1.1.5/dq_module.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 14:02:49.000000 dq_module-1.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-07-12 14:02:39.000000 dq_module-1.1.5/setup.py
```

### Comparing `dq_module-1.1.4/PKG-INFO` & `dq_module-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_module
-Version: 1.1.4
+Version: 1.1.5
 Summary: data profiling and basic data quality rules check
 Home-page: UNKNOWN
 Author: Sweta
 Author-email: sweta.swami@decisionpoint.in
 License: UNKNOWN
 Description: ### dq-module
         dq-module is a tool which can be used to perform validations and profiling on the datasets.This tool is compatible with two run_engines `pyspark` and `polars`.
```

### Comparing `dq_module-1.1.4/README.md` & `dq_module-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.4/dataqualitycheck/commonutilities.py` & `dq_module-1.1.5/dataqualitycheck/commonutilities.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.4/dataqualitycheck/consistencycheck.py` & `dq_module-1.1.5/dataqualitycheck/consistencycheck.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.4/dataqualitycheck/dataprofile.py` & `dq_module-1.1.5/dataqualitycheck/dataprofile.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.4/dataqualitycheck/datasources/azureblobdf.py` & `dq_module-1.1.5/dataqualitycheck/datasources/azureblobdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.4/dataqualitycheck/datasources/commonutilities.py` & `dq_module-1.1.5/dataqualitycheck/datasources/commonutilities.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.4/dataqualitycheck/datasources/databricksfilesystemdf.py` & `dq_module-1.1.5/dataqualitycheck/datasources/databricksfilesystemdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.4/dataqualitycheck/datasources/databrickssqldf.py` & `dq_module-1.1.5/dataqualitycheck/datasources/databrickssqldf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.4/dataqualitycheck/datasources/localfilesystemdf.py` & `dq_module-1.1.5/dataqualitycheck/datasources/localfilesystemdf.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.4/dataqualitycheck/enumfile.py` & `dq_module-1.1.5/dataqualitycheck/enumfile.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.4/dataqualitycheck/singledatasetqualitycheck.py` & `dq_module-1.1.5/dataqualitycheck/singledatasetqualitycheck.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.4/dataqualitycheck/singledatasetqualitycheckpolars.py` & `dq_module-1.1.5/dataqualitycheck/singledatasetqualitycheckpolars.py`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.4/dataqualitycheck/singledatasetqualitycheckspark.py` & `dq_module-1.1.5/dataqualitycheck/singledatasetqualitycheckspark.py`

 * *Files 23% similar despite different names*

```diff
@@ -111,18 +111,18 @@
             else:
                 column_failed.append(column)
         
         total_failed_records_count = result.count()
 
         if len(column_passed) == len(columnList):
             test_status = "PASS"
-        elif len(column_passed) < len(columnList):
-            test_status = "Passed: {} and Failed: {}".format(", ".join(column_passed), ", ".join(column_failed))
-        else:
+        elif len(column_failed) == len(columnList):
             test_status = "FAIL"
+        else:
+            test_status = "Passed: {} and Failed: {}".format(", ".join(column_passed), ", ".join(column_failed))
 
         failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"])).withColumn("Column_Tested", lit(rule["column_to_be_checked"])).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
      
         failed_records_write_location = self.write_failed_records(rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, total_failed_records_count, failed_records_write_location, start, run_date)
 
@@ -240,14 +240,56 @@
             reason = f', {e}'
             failed_df = df.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit("All columns")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag, False)
         return data_quality_test_summary_tuple(self.job_id, rule, test_status + reason, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
 
+    def range_min_check_V1(self, df, rule, write_failed_records_flag):
+        run_date = date.today().strftime("%Y/%m/%d")
+        start = time.time()
+        total_row_count = df.count()
+        columnList = list(rule["column_to_be_checked"].split(","))
+        valueList = list(rule["value"].split(','))
+
+        if len(columnList)==len(valueList):
+            combined_list = zip(columnList,valueList)
+        else:
+            raise Exception("missing values/columns")
+
+        result = self.spark.createDataFrame([], df.schema)
+        column_passed = []
+        column_failed = []
+        for column_value_tuple in combined_list:
+            df = df.filter(col(column_value_tuple[0]).isNotNull())
+            failed_results = df.filter(col(column_value_tuple[0]) < float(column_value_tuple[1]))
+            result = result.union(failed_results)
+            result = result.dropDuplicates()
+            failed_records_count = failed_results.count()
+            failed_records_write_location = 'N/A'
+            if failed_records_count == 0:
+                column_passed.append(column_value_tuple[0])
+            else:
+                column_failed.append(column_value_tuple[0])
+        
+        total_failed_records_count = result.count()
+
+        if len(column_passed) == len(columnList):
+            test_status = "PASS"
+        elif len(column_failed) == len(columnList):
+            test_status = "FAIL"
+        else:
+            test_status = "Passed: {} and Failed: {}".format(", ".join(column_passed), ", ".join(column_failed))
+
+        failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"])).withColumn("Column_Tested", lit(rule["column_to_be_checked"])).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
+    
+        failed_records_write_location = self.write_failed_records(rule, failed_df, write_failed_records_flag)
+
+        return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, total_failed_records_count, failed_records_write_location, start, run_date)
+
     # ----- Function to check if values not be less than the given value
 
     def range_min_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         df = df.filter(col(rule["column_to_be_checked"]).isNotNull())
@@ -282,15 +324,55 @@
   #          test_status = "FAIL"
   #          failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
   #             .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
   #         failed_records_write_location = self.write_failed_records(
   #             rule, failed_df, write_failed_records_flag)
   #
   #      return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
+    def range_max_check_V1(self, df, rule, write_failed_records_flag):
+        run_date = date.today().strftime("%Y/%m/%d")
+        start = time.time()
+        total_row_count = df.count()
+        columnList = list(rule["column_to_be_checked"].split(","))
+        valueList = list(rule["value"].split(','))
+
+        if len(columnList)==len(valueList):
+            combined_list = zip(columnList,valueList)
+        else:
+            raise Exception("missing values/columns")
+
+        result = self.spark.createDataFrame([], df.schema)
+        column_passed = []
+        column_failed = []
+        for column_value_tuple in combined_list:
+            df = df.filter(col(column_value_tuple[0]).isNotNull())
+            failed_results = df.filter(col(column_value_tuple[0]) > float(column_value_tuple[1]))
+            result = result.union(failed_results)
+            result = result.dropDuplicates()
+            failed_records_count = failed_results.count()
+            failed_records_write_location = 'N/A'
+            if failed_records_count == 0:
+                column_passed.append(column_value_tuple[0])
+            else:
+                column_failed.append(column_value_tuple[0])
+        
+        total_failed_records_count = result.count()
+
+        if len(column_passed) == len(columnList):
+            test_status = "PASS"
+        elif len(column_failed) == len(columnList):
+            test_status = "FAIL"
+        else:
+            test_status = "Passed: {} and Failed: {}".format(", ".join(column_passed), ", ".join(column_failed))
 
+        failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"])).withColumn("Column_Tested", lit(rule["column_to_be_checked"])).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
+    
+        failed_records_write_location = self.write_failed_records(rule, failed_df, write_failed_records_flag)
+
+        return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, total_failed_records_count, failed_records_write_location, start, run_date)
     # ----- Function to check if values should not be greater then the given value
     def range_max_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         df = df.filter(col(rule["column_to_be_checked"]).isNotNull())
         result = df.filter(
@@ -303,15 +385,58 @@
             test_status = "FAIL"
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
+    
+    def length_check_V1(self, df, rule, write_failed_records_flag):
+        run_date = date.today().strftime("%Y/%m/%d")
+        start = time.time()
+        total_row_count = df.count()
+        columnList = list(rule["column_to_be_checked"].split(","))
+        valueList = list(rule["value"].split(','))
 
+        if len(columnList)==len(valueList):
+            combined_list = zip(columnList,valueList)
+        else:
+            raise Exception("missing values/columns")
+
+        result = self.spark.createDataFrame([], df.schema)
+        column_passed = []
+        column_failed = []
+        for column_value_tuple in combined_list:
+            failed_results = df.filter(
+            length(col(column_value_tuple[0])) > int(column_value_tuple[1]))
+            result = result.union(failed_results)
+            result = result.dropDuplicates()
+            failed_records_count = failed_results.count()
+            failed_records_write_location = 'N/A'
+            if failed_records_count == 0:
+                column_passed.append(column_value_tuple[0])
+            else:
+                column_failed.append(column_value_tuple[0])
+        
+        total_failed_records_count = result.count()
+
+        if len(column_passed) == len(columnList):
+            test_status = "PASS"
+        elif len(column_failed) == len(columnList):
+            test_status = "FAIL"
+        else:
+            test_status = "Passed: {} and Failed: {}".format(", ".join(column_passed), ", ".join(column_failed))
+
+        failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"])).withColumn("Column_Tested", lit(rule["column_to_be_checked"])).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
+    
+        failed_records_write_location = self.write_failed_records(rule, failed_df, write_failed_records_flag)
+
+        return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, total_failed_records_count, failed_records_write_location, start, run_date)
+    
+    
     # ----- Function to check if the values in the column have given length or not.
     def length_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(
             length(col(rule["column_to_be_checked"])) > int(rule["value"]))
@@ -388,15 +513,57 @@
             test_status = "FAIL"
             failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"]))\
                 .withColumn("Column_Tested", lit(f"{rule['column_to_be_checked']}:{rule['value']}")).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
             failed_records_write_location = self.write_failed_records(
                 rule, failed_df, write_failed_records_flag)
 
         return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, failed_records_count, failed_records_write_location, start, run_date)
+    
+    def min_length_check_V1(self, df, rule, write_failed_records_flag):
+        run_date = date.today().strftime("%Y/%m/%d")
+        start = time.time()
+        total_row_count = df.count()
+        columnList = list(rule["column_to_be_checked"].split(","))
+        valueList = list(rule["value"].split(','))
+
+        if len(columnList)==len(valueList):
+            combined_list = zip(columnList,valueList)
+        else:
+            raise Exception("missing values/columns")
+
+        result = self.spark.createDataFrame([], df.schema)
+        column_passed = []
+        column_failed = []
+        for column_value_tuple in combined_list:
+            failed_results = df.filter(
+            length(col(column_value_tuple[0])) < int(column_value_tuple[1]))
+            result = result.union(failed_results)
+            result = result.dropDuplicates()
+            failed_records_count = failed_results.count()
+            failed_records_write_location = 'N/A'
+            if failed_records_count == 0:
+                column_passed.append(column_value_tuple[0])
+            else:
+                column_failed.append(column_value_tuple[0])
+        
+        total_failed_records_count = result.count()
+
+        if len(column_passed) == len(columnList):
+            test_status = "PASS"
+        elif len(column_failed) == len(columnList):
+            test_status = "FAIL"
+        else:
+            test_status = "Passed: {} and Failed: {}".format(", ".join(column_passed), ", ".join(column_failed))
 
+        failed_df = result.withColumn("Run_Date", lit(run_date)).withColumn("Rule", lit(rule["rule_name"])).withColumn("Column_Tested", lit(rule["column_to_be_checked"])).withColumn("Mandatory", lit(1 if rule["ruletype"] == 'Mandatory' else 0).cast(LongType())).withColumn("job_id", lit(self.job_id))
+    
+        failed_records_write_location = self.write_failed_records(rule, failed_df, write_failed_records_flag)
+
+        return data_quality_test_summary_tuple(self.job_id, rule, test_status, total_row_count, total_failed_records_count, failed_records_write_location, start, run_date)
+    
     # ----- Function to check that if the values in the column has the required minimum length or not.
     def min_length_check(self, df, rule, write_failed_records_flag):
         run_date = date.today().strftime("%Y/%m/%d")
         start = time.time()
         total_row_count = df.count()
         result = df.filter(
             length(col(rule["column_to_be_checked"])) < int(rule["value"]))
@@ -568,55 +735,84 @@
 
                     if 'active' in rule and int(rule['active']) == 0:
                         run_date = date.today().strftime("%Y/%m/%d")
                         test_summary.append(data_quality_test_summary_tuple(
                             self.job_id, rule, "", "", "", "", 0, run_date))
                         continue
 
-                    if rule["rule_name"] == "null_check":
+                    if rule["rule_name"] == "null_check" and len(list(rule["column_to_be_checked"].split(",")))==1:
+                        result_df = self.null_check(
+                            self.dataframes[source], rule, write_failed_records_flag)
+                        test_summary.append(result_df)
+
+                    elif rule["rule_name"] == "null_check" and len(list(rule["column_to_be_checked"].split(",")))>1:
                         result_df = self.null_check_V1(
                             self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     
                     elif rule["rule_name"] == "schema_check":
                         result_df = self.schema_check(
                             self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
-                    elif rule["rule_name"] == "range_min_check":
+
+                    elif rule["rule_name"] == "range_min_check" and len(list(rule["column_to_be_checked"].split(",")))==1:
                         result_df = self.range_min_check(
                             self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
+
+                    elif rule["rule_name"] == "range_min_check" and len(list(rule["column_to_be_checked"].split(",")))>1:
+                        result_df = self.range_min_check_V1(
+                            self.dataframes[source], rule, write_failed_records_flag)
+                        test_summary.append(result_df)
                     #elif rule["rule_name"] == "range_min_inclusive_check":
                     #    result_df = self.range_min_inclusive_check(
                     #       self.dataframes[source], rule, write_failed_records_flag)
                     #    test_summary.append(result_df)
-                    elif rule["rule_name"] == "range_max_check":
+                    elif rule["rule_name"] == "range_max_check" and len(list(rule["column_to_be_checked"].split(",")))==1:
                         result_df = self.range_max_check(
                             self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
-                    elif rule["rule_name"] == "length_check":
+                    
+                    elif rule["rule_name"] == "range_max_check" and len(list(rule["column_to_be_checked"].split(",")))>1:
+                        result_df = self.range_max_check_V1(
+                            self.dataframes[source], rule, write_failed_records_flag)
+                        test_summary.append(result_df)
+                    
+                    elif rule["rule_name"] == "length_check" and len(list(rule["column_to_be_checked"].split(",")))==1:
                         result_df = self.length_check(
                             self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
+
+                    elif rule["rule_name"] == "length_check" and len(list(rule["column_to_be_checked"].split(",")))>1:
+                        result_df = self.length_check_V1(
+                            self.dataframes[source], rule, write_failed_records_flag)
+                        test_summary.append(result_df)
+
                     elif rule["rule_name"] == "unique_keys_check":
                         result_df = self.unique_keys_check(
                             self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "unique_records_check":
                         result_df = self.unique_records_check(
                             self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "allowed_values_check":
                         result_df = self.allowed_values_check(
                             self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
-                    elif rule["rule_name"] == "min_length_check":
+                    elif rule["rule_name"] == "min_length_check" and len(list(rule["column_to_be_checked"].split(",")))==1 :
                         result_df = self.min_length_check(
                             self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
+                    
+                    elif rule["rule_name"] == "min_length_check" and len(list(rule["column_to_be_checked"].split(",")))>1 :
+                        result_df = self.min_length_check_V1(
+                            self.dataframes[source], rule, write_failed_records_flag)
+                        test_summary.append(result_df)
+                    
                     elif rule["rule_name"] == "column_count_check":
                         result_df = self.column_count_check(
                             self.dataframes[source], rule, write_failed_records_flag)
                         test_summary.append(result_df)
                     elif rule["rule_name"] == "not_allowed_values_check":
                         result_df = self.not_allowed_values_check(
                             self.dataframes[source], rule, write_failed_records_flag)
```

### Comparing `dq_module-1.1.4/dq_module.egg-info/PKG-INFO` & `dq_module-1.1.5/dq_module.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq-module
-Version: 1.1.4
+Version: 1.1.5
 Summary: data profiling and basic data quality rules check
 Home-page: UNKNOWN
 Author: Sweta
 Author-email: sweta.swami@decisionpoint.in
 License: UNKNOWN
 Description: ### dq-module
         dq-module is a tool which can be used to perform validations and profiling on the datasets.This tool is compatible with two run_engines `pyspark` and `polars`.
```

### Comparing `dq_module-1.1.4/dq_module.egg-info/SOURCES.txt` & `dq_module-1.1.5/dq_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dq_module-1.1.4/setup.py` & `dq_module-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # COMMAND ----------
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read() 
     
 setuptools.setup(
     name="dq_module",
-    version="1.1.4",
+    version="1.1.5",
     author="Sweta",
     author_email="sweta.swami@decisionpoint.in",
     description="data profiling and basic data quality rules check",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # packages=setuptools.find_packages(include=['*']),
     packages=['dataqualitycheck', 'dataqualitycheck.datasources'],
```


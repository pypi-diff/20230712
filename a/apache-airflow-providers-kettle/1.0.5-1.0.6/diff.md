# Comparing `tmp/apache_airflow_providers_kettle-1.0.5.tar.gz` & `tmp/apache_airflow_providers_kettle-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_kettle-1.0.5.tar", last modified: Fri Jul  7 11:48:28 2023, max compression
+gzip compressed data, was "apache_airflow_providers_kettle-1.0.6.tar", last modified: Wed Jul 12 20:41:39 2023, max compression
```

## Comparing `apache_airflow_providers_kettle-1.0.5.tar` & `apache_airflow_providers_kettle-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-07 11:48:28.507338 apache_airflow_providers_kettle-1.0.5/
--rw-rw-r--   0 bop       (1000) bop       (1000)    10898 2023-06-25 20:45:53.000000 apache_airflow_providers_kettle-1.0.5/LICENSE
--rw-rw-r--   0 bop       (1000) bop       (1000)     4411 2023-07-07 11:48:28.507338 apache_airflow_providers_kettle-1.0.5/PKG-INFO
--rw-rw-r--   0 bop       (1000) bop       (1000)     4040 2023-07-07 11:47:10.000000 apache_airflow_providers_kettle-1.0.5/README.md
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-07 11:48:28.503338 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/
--rw-rw-r--   0 bop       (1000) bop       (1000)     4411 2023-07-07 11:48:28.000000 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/PKG-INFO
--rw-rw-r--   0 bop       (1000) bop       (1000)      539 2023-07-07 11:48:28.000000 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/SOURCES.txt
--rw-rw-r--   0 bop       (1000) bop       (1000)        1 2023-07-07 11:48:28.000000 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/dependency_links.txt
--rw-rw-r--   0 bop       (1000) bop       (1000)       85 2023-07-07 11:48:28.000000 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/entry_points.txt
--rw-rw-r--   0 bop       (1000) bop       (1000)       20 2023-07-07 11:48:28.000000 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/requires.txt
--rw-rw-r--   0 bop       (1000) bop       (1000)       16 2023-07-07 11:48:28.000000 apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/top_level.txt
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-07 11:48:28.503338 apache_airflow_providers_kettle-1.0.5/kettle_provider/
--rw-rw-r--   0 bop       (1000) bop       (1000)      438 2023-07-07 11:46:20.000000 apache_airflow_providers_kettle-1.0.5/kettle_provider/__init__.py
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-07 11:48:28.503338 apache_airflow_providers_kettle-1.0.5/kettle_provider/hooks/
--rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:36:58.000000 apache_airflow_providers_kettle-1.0.5/kettle_provider/hooks/__init__.py
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-07 11:48:28.503338 apache_airflow_providers_kettle-1.0.5/kettle_provider/operators/
--rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:36:47.000000 apache_airflow_providers_kettle-1.0.5/kettle_provider/operators/__init__.py
--rw-rw-r--   0 bop       (1000) bop       (1000)     8600 2023-07-07 11:46:37.000000 apache_airflow_providers_kettle-1.0.5/kettle_provider/operators/kettle_operator.py
-drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-07 11:48:28.503338 apache_airflow_providers_kettle-1.0.5/kettle_provider/sensors/
--rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:37:07.000000 apache_airflow_providers_kettle-1.0.5/kettle_provider/sensors/__init__.py
--rw-rw-r--   0 bop       (1000) bop       (1000)       38 2023-07-07 11:48:28.507338 apache_airflow_providers_kettle-1.0.5/setup.cfg
--rw-rw-r--   0 bop       (1000) bop       (1000)     1017 2023-07-07 11:46:11.000000 apache_airflow_providers_kettle-1.0.5/setup.py
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-12 20:41:39.060565 apache_airflow_providers_kettle-1.0.6/
+-rw-rw-r--   0 bop       (1000) bop       (1000)    10898 2023-06-25 20:45:53.000000 apache_airflow_providers_kettle-1.0.6/LICENSE
+-rw-rw-r--   0 bop       (1000) bop       (1000)     4411 2023-07-12 20:41:39.060565 apache_airflow_providers_kettle-1.0.6/PKG-INFO
+-rw-rw-r--   0 bop       (1000) bop       (1000)     4040 2023-07-07 11:47:10.000000 apache_airflow_providers_kettle-1.0.6/README.md
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-12 20:41:39.060565 apache_airflow_providers_kettle-1.0.6/apache_airflow_providers_kettle.egg-info/
+-rw-rw-r--   0 bop       (1000) bop       (1000)     4411 2023-07-12 20:41:39.000000 apache_airflow_providers_kettle-1.0.6/apache_airflow_providers_kettle.egg-info/PKG-INFO
+-rw-rw-r--   0 bop       (1000) bop       (1000)      539 2023-07-12 20:41:39.000000 apache_airflow_providers_kettle-1.0.6/apache_airflow_providers_kettle.egg-info/SOURCES.txt
+-rw-rw-r--   0 bop       (1000) bop       (1000)        1 2023-07-12 20:41:39.000000 apache_airflow_providers_kettle-1.0.6/apache_airflow_providers_kettle.egg-info/dependency_links.txt
+-rw-rw-r--   0 bop       (1000) bop       (1000)       85 2023-07-12 20:41:39.000000 apache_airflow_providers_kettle-1.0.6/apache_airflow_providers_kettle.egg-info/entry_points.txt
+-rw-rw-r--   0 bop       (1000) bop       (1000)       20 2023-07-12 20:41:39.000000 apache_airflow_providers_kettle-1.0.6/apache_airflow_providers_kettle.egg-info/requires.txt
+-rw-rw-r--   0 bop       (1000) bop       (1000)       16 2023-07-12 20:41:39.000000 apache_airflow_providers_kettle-1.0.6/apache_airflow_providers_kettle.egg-info/top_level.txt
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-12 20:41:39.060565 apache_airflow_providers_kettle-1.0.6/kettle_provider/
+-rw-rw-r--   0 bop       (1000) bop       (1000)      447 2023-07-12 20:41:16.000000 apache_airflow_providers_kettle-1.0.6/kettle_provider/__init__.py
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-12 20:41:39.060565 apache_airflow_providers_kettle-1.0.6/kettle_provider/hooks/
+-rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:36:58.000000 apache_airflow_providers_kettle-1.0.6/kettle_provider/hooks/__init__.py
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-12 20:41:39.060565 apache_airflow_providers_kettle-1.0.6/kettle_provider/operators/
+-rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:36:47.000000 apache_airflow_providers_kettle-1.0.6/kettle_provider/operators/__init__.py
+-rw-rw-r--   0 bop       (1000) bop       (1000)     8590 2023-07-12 20:40:19.000000 apache_airflow_providers_kettle-1.0.6/kettle_provider/operators/kettle_operator.py
+drwxrwxr-x   0 bop       (1000) bop       (1000)        0 2023-07-12 20:41:39.060565 apache_airflow_providers_kettle-1.0.6/kettle_provider/sensors/
+-rw-rw-r--   0 bop       (1000) bop       (1000)        0 2023-06-25 20:37:07.000000 apache_airflow_providers_kettle-1.0.6/kettle_provider/sensors/__init__.py
+-rw-rw-r--   0 bop       (1000) bop       (1000)       38 2023-07-12 20:41:39.060565 apache_airflow_providers_kettle-1.0.6/setup.cfg
+-rw-rw-r--   0 bop       (1000) bop       (1000)     1017 2023-07-12 20:41:20.000000 apache_airflow_providers_kettle-1.0.6/setup.py
```

### Comparing `apache_airflow_providers_kettle-1.0.5/LICENSE` & `apache_airflow_providers_kettle-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_kettle-1.0.5/PKG-INFO` & `apache_airflow_providers_kettle-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache_airflow_providers_kettle
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple Apache Airflow Kettle Operator that can invoke jobs and transformations for Linux based systems.
 Home-page: 
 Author: Robert Bryśkiewicz
 Author-email: bryskiewiczr@pm.me
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
```

### Comparing `apache_airflow_providers_kettle-1.0.5/README.md` & `apache_airflow_providers_kettle-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/PKG-INFO` & `apache_airflow_providers_kettle-1.0.6/apache_airflow_providers_kettle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-kettle
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple Apache Airflow Kettle Operator that can invoke jobs and transformations for Linux based systems.
 Home-page: 
 Author: Robert Bryśkiewicz
 Author-email: bryskiewiczr@pm.me
 License: Apache License 2.0
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
```

### Comparing `apache_airflow_providers_kettle-1.0.5/apache_airflow_providers_kettle.egg-info/SOURCES.txt` & `apache_airflow_providers_kettle-1.0.6/apache_airflow_providers_kettle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_kettle-1.0.5/kettle_provider/operators/kettle_operator.py` & `apache_airflow_providers_kettle-1.0.6/kettle_provider/operators/kettle_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             -level={self.loglevel} \
             -logfile={self.logfile} \
             -maxloglines={self.maxloglines} \
             -maxlogtimeout={self.maxlogtimeout} \
             -norep=Y '
         # Get additional parameters
         for k, v in self.params.items():
-            pdi_command.append(f'-param:{k}={v} ')
+            pdi_command += f'-param:{k}={v} '
         # Execute the command
         result = self.subprocess_hook.run_command(
             command=[bash_path, '-c', pdi_command],
             output_encoding=self.output_encoding,
             cwd=self.pdipath
         )
         if result.exit_code != 0:
@@ -170,15 +170,15 @@
             -level={self.loglevel} \
             -logfile={self.logfile} \
             -maxloglines={self.maxloglines} \
             -maxlogtimeout={self.maxlogtimeout} \
             -norep=Y '
         # Get additional parameters
         for k, v in self.params.items():
-            pdi_command.append(f'-param:{k}={v} ')
+            pdi_command += f'-param:{k}={v} '
         # Execute the command
         result = self.subprocess_hook.run_command(
             command=[bash_path, '-c', pdi_command],
             output_encoding=self.output_encoding,
             cwd=self.pdipath
         )
         if result.exit_code != 0:
```

### Comparing `apache_airflow_providers_kettle-1.0.5/setup.py` & `apache_airflow_providers_kettle-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 
 """Perform the package airflow-provider-kettle-operator setup."""
 setup(
     name="apache_airflow_providers_kettle",
     version=__version__,
     description="A simple Apache Airflow Kettle Operator that can invoke jobs and transformations for Linux based systems.",
     long_description=long_description,
```


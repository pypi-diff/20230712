# Comparing `tmp/healdata_utils-0.0.8a0.tar.gz` & `tmp/healdata_utils-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healdata_utils-0.0.8a0.tar", last modified: Fri Jun 30 14:53:24 2023, max compression
+gzip compressed data, was "healdata_utils-0.1.1a0.tar", last modified: Wed Jul 12 02:11:32 2023, max compression
```

## Comparing `healdata_utils-0.0.8a0.tar` & `healdata_utils-0.1.1a0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.525761 healdata_utils-0.0.8a0/
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-06-30 14:53:24.525761 healdata_utils-0.0.8a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-06-30 14:53:14.000000 healdata_utils-0.0.8a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:53:24.525761 healdata_utils-0.0.8a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.517761 healdata_utils-0.0.8a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvdata/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvtemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvtemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvtemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvtemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/frictionless/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/frictionless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/frictionless/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/jsontemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/jsontemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/jsontemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/jsontemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/readstat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/readstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/readstat/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/types/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/types/typesets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/validators/frictionless.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/validators/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/src/healdata_utils/validators/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-06-30 14:53:24.000000 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-30 14:53:24.000000 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:53:24.000000 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-30 14:53:24.000000 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-30 14:53:24.000000 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-30 14:53:24.000000 healdata_utils-0.0.8a0/src/healdata_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:53:24.521761 healdata_utils-0.0.8a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-30 14:53:15.000000 healdata_utils-0.0.8a0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.970311 healdata_utils-0.1.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-12 02:11:32.970311 healdata_utils-0.1.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 02:11:32.970311 healdata_utils-0.1.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.958311 healdata_utils-0.1.1a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.962311 healdata_utils-0.1.1a0/src/healdata_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.962311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.962311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvdata/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvtemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvtemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvtemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvtemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/frictionless/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/frictionless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/frictionless/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/jsontemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/jsontemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/jsontemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/jsontemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/readstat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/readstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/readstat/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/types/typesets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/src/healdata_utils/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/validators/frictionless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/validators/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/src/healdata_utils/validators/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.962311 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-12 02:11:32.000000 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-12 02:11:32.000000 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 02:11:32.000000 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 02:11:32.000000 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 02:11:32.000000 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-12 02:11:32.000000 healdata_utils-0.1.1a0/src/healdata_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:11:32.966311 healdata_utils-0.1.1a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-12 02:11:19.000000 healdata_utils-0.1.1a0/tests/test_utils.py
```

### Comparing `healdata_utils-0.0.8a0/PKG-INFO` & `healdata_utils-0.1.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healdata_utils
-Version: 0.0.8a0
+Version: 0.1.1a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
 --8<-- [start:intro]
```

### Comparing `healdata_utils-0.0.8a0/README.md` & `healdata_utils-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/setup.py` & `healdata_utils-0.1.1a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def generate_long_description():
     return Path("README.md").read_text()
 
 
 setup(
     name='healdata_utils',
-    version='0.0.8-alpha',
+    version='0.1.1-alpha',
     author='Michael Kranz',
     author_email='kranz-michael@norc.org',
     long_description=generate_long_description(),
     long_description_content_type="text/markdown",    
     description='Data packaging tools for the HEAL data ecosystem',
     #TODO: change url to HEAL once migrated.
     url='https://github.com/norc-heal/healdata-utils',
```

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/cli.py` & `healdata_utils-0.1.1a0/src/healdata_utils/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 }
 
 def convert_to_vlmd(
     filepath,
     data_dictionary_props={},
     inputtype=None,
     outputdir=None,
-    sas7bcat_filepath=None
+    sas7bcat_filepath=None,
+    csvtemplate_output_quoting=None,
 
     ):
     """
     Writes a data dictionary (i.e. variable level metadata) to a HEAL metadata JSON file using a registered function.
 
     Parameters
     ----------
@@ -61,15 +62,20 @@
         1. Outputdir is a directory, will give standard names,
         2. If path to the to-be-written file is specified, will use this as new outputted filename
     data_dictionary_props : dict, optional
         The other data-dictionary level properties. By default, will give the data_dictionary `title` property as the file name stem.
     inputtype : str, optional
         The input type. If none specified, will default to using the file extension.
         See the currently registered input types in the input_types list.
-
+    sas7bcat_filepath: str,optional
+        [FOR SAS7BDAT ONLY]: Path to a sas catalog file (sas7bcat). Needed for value formats if a sas (sas7bdat) input file
+    csvtemplate_output_quoting: bool, optional
+        If true, all nonnumeric values will be quoted. This helps reduce ambiguity for programs
+        like excel that uses special characters for specific purposes (eg = for formulas)
+    
     Returns
     -------
     dict
         Dictionary with:
          1. csvtemplated array of fields.
          2. jsontemplated data dictionary object as specified by an originally drafted design doc.
             That is, a dictionary with title:<title>,description:<description>,data_dictionary:<fields>
@@ -134,16 +140,17 @@
         
         # print data dictionaries
         jsontemplate_path.write_text(json.dumps(templatejson,indent=4))
 
         # NOTE: quoting non-numeric to allow special characters for nested delimiters within string columns (ie "=")
         (
             etl.fromdicts(templatecsv)
-            .tocsv(csvtemplate_path,
-                quoting=csv.QUOTE_NONNUMERIC)
+            .tocsv(
+                csvtemplate_path,
+                quoting=csv.QUOTE_NONNUMERIC if csvtemplate_output_quoting else csv.QUOTE_MINIMAL)
 
         )
 
         # print errors
 
         if not report_json['valid']:
             print("JSON data dictionary not valid, see heal-json-errors.json for errors.")
@@ -174,21 +181,24 @@
 @click.command()
 @click.option('--filepath',required=True,help='Path to the file you want to convert to a HEAL data dictionary')
 @click.option('--title',default=None,help='The title of your data dictionary. If not specified, then the file name will be used')
 @click.option('--description',default=None,help='Description of data dictionary')
 @click.option('--inputtype',default=None,type=click.Choice(list(choice_fxn.keys())),help='The type of your input file.')
 @click.option('--outputdir',default="",help='The folder where you want to output your HEAL data dictionary')
 @click.option('--sas7bcat-filepath',default=None,help="[FOR SAS7BDAT ONLY]: Path to a sas catalog file (sas7bcat). Needed for value formats if a sas (sas7bdat) input file")
-def main(filepath,title,description,inputtype,outputdir,sas7bcat_filepath):
+@click.option('--csvtemplate-output-quoting',default=None,help="If true, all nonnumeric values will be quoted."
+    " This helps reduce ambiguity for programs like excel that uses special characters for specific purposes (eg = for formulas)")
+def main(filepath,title,description,inputtype,outputdir,sas7bcat_filepath,csvtemplate_output_quoting):
     data_dictionary_props = {'title':title,'description':description}
 
     #save dds and error reports to files
     data_dictionaries = convert_to_vlmd(
         filepath=filepath,
         data_dictionary_props=data_dictionary_props,
         outputdir=outputdir,
         inputtype=inputtype,
-        sas7bcat_filepath=sas7bcat_filepath
+        sas7bcat_filepath=sas7bcat_filepath,
+        csvtemplate_output_quoting=csvtemplate_output_quoting
     )
      
 if __name__=='__main__':
     main()
```

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/io.py` & `healdata_utils-0.1.1a0/src/healdata_utils/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,22 +49,24 @@
 def read_table(file_path,castdtype = "string"):
     """ 
     reads in a tabular file (ie spreadsheet) after detecting
     encoding and file extension without any type casting.
 
     currently supports csv and tsv
 
-    defaults to not casting values (ie all columns are string dtypes).
+    defaults to not casting values (ie all columns are string dtypes)
+    and not parsing strings into NA values (eg "" is kept as "")
     """ 
     ext = Path(file_path).suffix
     if ext==".csv":
         sep = ","
     elif ext==".tsv":
         sep = "\t"
         
     encoding = detect_file_encoding(file_path)
     file_encoding = pd.read_csv(
-        file_path,sep=sep,encoding=encoding,dtype=castdtype)
+        file_path,sep=sep,encoding=encoding,dtype=castdtype,
+        keep_default_na=False)
 
     return file_encoding
```

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/schemas.py` & `healdata_utils-0.1.1a0/src/healdata_utils/schemas.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvdata/conversion.py` & `healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvdata/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/transforms/csvtemplate/mappings.py` & `healdata_utils-0.1.1a0/src/healdata_utils/transforms/csvtemplate/mappings.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from healdata_utils import schemas
 # split array columns
 def split_str_array(string,sep='|'):
     if string:
         return [s.strip() for s in string.split(sep)]
     else:
-        return None
+        return string
 
 # if object within array, assign to properties
 def map_keys_vals(keys,vals):
     ''' zips two lists of the same size as 
     a dictionary
     ''' 
     return dict(zip(keys,vals))
@@ -31,20 +31,22 @@
     if string:
         keys = prop['items']['properties'].keys()
         return [
             map_keys_vals(keys,split_str_array(x,sep='=')) 
             for x in split_str_array(string,sep='|')
         ]
     else:
-        return None
+        return string
 
 def loads_dict(string,item_sep='|',key_val_sep='='):
     if string:
         return dict([split_str_array(s,key_val_sep) 
             for s in split_str_array(string,item_sep)])
+    else:
+        return string
 def mapval(v,mapping):
     v = str(v)
     if v in mapping:
         return mapping[v]
     else:
         return v
 
@@ -72,26 +74,42 @@
 props = schemas.healjsonschema['properties']
     #mappings for array of dicts, arrays, and dicts
 
 
 true_values = ["true","1","yes","required","y"]
 false_values = ["false","0","no","not required","n"]
 
-
+# cast numbers explicitly based on schema
+# this is needed in case there is only one record in a string column that is a number (ie don't want to convert)
+castnumbers = {
+    field["name"]:int if field["type"]=="integer" else float
+    for field in schemas.healcsvschema["fields"]
+    if field.get("type","") in ["integer","number"]
+}
 
 fieldmap = {
     'constraints.required': lambda v: to_bool(v),
     'constraints.enum': lambda v: split_str_array(v),
     # 'constraints.maximum':int,
     # 'constraints.minimum':int, #TODO:need to add to schema
     # 'constraints.maxLength':int,
-    'cde_id': lambda v: split_and_map(v, props['cde_id']),
-    'ontology_id': lambda v: split_and_map(v, props['ontology_id']),
-    'encoding':lambda v: loads_dict(v),
+    'standardsMappings.type': lambda v: split_str_array(v),
+    'standardsMappings.label': lambda v: split_str_array(v),
+    'standardsMappings.source': lambda v: split_str_array(v),
+    'standardsMappings.id': lambda v: split_str_array(v),
+    'standardsMappings.url': lambda v: split_str_array(v),
+    'relatedConcepts.type': lambda v: split_str_array(v),
+    'relatedConcepts.label': lambda v: split_str_array(v),
+    'relatedConcepts.source': lambda v: split_str_array(v),
+    'relatedConcepts.id': lambda v: split_str_array(v),
+    'relatedConcepts.url': lambda v: split_str_array(v),
+    'encodings':lambda v: loads_dict(v),
     'format': lambda v: mapval(v,formatmap),
     'type':lambda v: mapval(v,typemap),
     #'univar_stats.cat_marginals':lambda v: split_and_map(v, prop['univar_stats']['cat_marginals']),
     'missingValues':lambda v: split_str_array(v),
     'trueValues': lambda v: split_str_array(v),
     'falseValues':lambda v: split_str_array(v),
     # TODO: add stats
 }
+
+zipmap = ["standardsMappings","relatedConcepts"]
```

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/transforms/frictionless/conversion.py` & `healdata_utils-0.1.1a0/src/healdata_utils/transforms/frictionless/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/transforms/jsontemplate/conversion.py` & `healdata_utils-0.1.1a0/src/healdata_utils/transforms/jsontemplate/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/transforms/jsontemplate/mappings.py` & `healdata_utils-0.1.1a0/src/healdata_utils/transforms/jsontemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/transforms/readstat/conversion.py` & `healdata_utils-0.1.1a0/src/healdata_utils/transforms/readstat/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/conversion.py` & `healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/headers.py` & `healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/headers.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/mappings.py` & `healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/transforms/redcapcsv/schema.py` & `healdata_utils-0.1.1a0/src/healdata_utils/transforms/redcapcsv/schema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/types/typesets.py` & `healdata_utils-0.1.1a0/src/healdata_utils/types/typesets.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/utils.py` & `healdata_utils-0.1.1a0/src/healdata_utils/utils.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/validators/jsonschema.py` & `healdata_utils-0.1.1a0/src/healdata_utils/validators/jsonschema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils/validators/validate.py` & `healdata_utils-0.1.1a0/src/healdata_utils/validators/validate.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils.egg-info/PKG-INFO` & `healdata_utils-0.1.1a0/src/healdata_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healdata-utils
-Version: 0.0.8a0
+Version: 0.1.1a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
 --8<-- [start:intro]
```

### Comparing `healdata_utils-0.0.8a0/src/healdata_utils.egg-info/SOURCES.txt` & `healdata_utils-0.1.1a0/src/healdata_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/tests/test_cli.py` & `healdata_utils-0.1.1a0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/tests/test_schemas.py` & `healdata_utils-0.1.1a0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.0.8a0/tests/test_utils.py` & `healdata_utils-0.1.1a0/tests/test_utils.py`

 * *Files identical despite different names*


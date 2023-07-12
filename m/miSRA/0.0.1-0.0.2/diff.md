# Comparing `tmp/misra-0.0.1.tar.gz` & `tmp/misra-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misra-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "misra-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `misra-0.0.1.tar` & `misra-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      261 2023-06-30 10:57:04.405539 misra-0.0.1/README.md
--rw-r--r--   0        0        0      831 2023-06-30 10:57:04.125554 misra-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      261 2023-06-30 10:57:05.369490 misra-0.0.1/src/miSRA/README.md
--rw-r--r--   0        0        0        0 2023-06-30 10:57:05.093504 misra-0.0.1/src/miSRA/__init__.py
--rw-r--r--   0        0        0      161 2023-06-30 10:57:05.965459 misra-0.0.1/src/miSRA/example_configs/annotated_miSRA_example_config.json
--rw-r--r--   0        0        0      161 2023-06-30 10:57:05.965459 misra-0.0.1/src/miSRA/example_configs/miSRA_example_config.json
--rw-r--r--   0        0        0    18220 2023-06-30 10:57:05.317492 misra-0.0.1/src/miSRA/miSRA.py
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 misra-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2826 2023-07-12 13:08:31.646185 misra-0.0.2/README.md
+-rw-r--r--   0        0        0      831 2023-07-12 13:08:31.422197 misra-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      261 2023-07-12 13:08:32.670133 misra-0.0.2/src/miSRA/README.md
+-rw-r--r--   0        0        0        0 2023-07-12 13:08:32.406146 misra-0.0.2/src/miSRA/__init__.py
+-rw-r--r--   0        0        0      991 2023-07-12 13:08:33.282101 misra-0.0.2/src/miSRA/example_configs/annotated_miSRA_example_config.json
+-rw-r--r--   0        0        0      161 2023-07-12 13:08:33.282101 misra-0.0.2/src/miSRA/example_configs/miSRA_example_config.json
+-rw-r--r--   0        0        0    18524 2023-07-12 13:08:32.630135 misra-0.0.2/src/miSRA/miSRA.py
+-rw-r--r--   0        0        0     3485 1970-01-01 00:00:00.000000 misra-0.0.2/PKG-INFO
```

### Comparing `misra-0.0.1/pyproject.toml` & `misra-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "miSRA"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Michael Hackenberg", email="hackenberg@go.ugr.es" },
   { name="Ernesto Aparicio", email="eaparicioeaparicio@gmail.com" },
 ]
 description = "A command-line interface to the miSRA API. It allow to remotely query over 90,000 miRNA-seq samples from the Sequence Read Archive"
 readme = "README.md"
 requires-python = ">=3.7.0"
```

### Comparing `misra-0.0.1/src/miSRA/miSRA.py` & `misra-0.0.2/src/miSRA/miSRA.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,38 +7,37 @@
 and do not need to be downloaded by the user. 
 The user needs to provide only reference sequences (like putative novel microRNAs) and the 
 sample (SRX/ERX/DRX) or study IDs (SRP/ERP/DRP) from SRA.  
 The requiered information is specified in a config file (json or key=value format)
 
 Launch the miSRA without paramters to obtain a commented config file
 
-Git hub:
+Git hub: https://github.com/bioinfoUGR/miSRA/
 
-Manual: 
-
-Example config:
+Manual: https://github.com/bioinfoUGR/miSRA/blob/main/manual.pdf
 
+Example config: https://github.com/bioinfoUGR/miSRA/blob/main/examples/mirna/annotated_config.json
 Authors:
 - Ernesto Aparicio Puerta <>
 - Michael Hackenberg <hackenberg@ugr.es>
 
 
 Installation:
 
 All dependencies should be installed already in a standard python installation.
 Installing through pip, will make the script runable from any working directory resolving also dependencies issues.
 
-pip
+pip3 install miSRA
 
 
-Version: 0.9
-Date: June 28, 2023
+Version: 0.0.2
+Date: July 12th, 2023
 
 Dependencies:
-- Python 3.8 or higher
+- Python 3.7 or higher
 
 
 
 """
 from genericpath import isfile
 import requests
 import sys
@@ -232,16 +231,16 @@
                         ' with the name miSRA_example_config.json. ' +
                              'For additional config examples, please refer to https://github.com/bioinfoUGR/miSRA')
 
     parser.add_argument('--db-stat', '-db', action='store_true',
                         help='show database statistics and dump them to miSRAdb_stat.csv')
 
     parser.add_argument('--taxonID', '-t', type=str,
-                        help='show database statistics for a specific NCBI\'s taxon ID and dump them' +
-                             ' to miSRAdb_taxonID_[TAXONID].csv')
+                        help='show database content (studies and samples) for a specific species using its ' +
+                             'NCBI\'s taxon ID and dump them to miSRAdb_taxonID_[TAXONID].csv')
     parser.add_argument('--jobID', '-j', type=str, help='once a job is submitted successfully, you receive a jobID. ' +
                                                         'Use this parameter to retrieve your results if the ' +
                                                         'connection is interrupted.')
 
     # parser.add_argument('-mode', type=str,
     #                     help='possible values: i) profile, ii) query, iii) dbstat')
 
@@ -387,14 +386,16 @@
         backdata["type"] = "profiler"
         print("Detected analysis type: " + data["mode"])
 
         if data['mode'] == "download":
             backdata["mode"] = "download"
             return (backdata, None)
         # check if mode is spike and the file is specified and does exist
+        if (data["mode"] == "exact"):
+            data["mode"] = "spike"
         if (data["mode"] == "spike"):
             if (data.get("spikeFile") and os.path.isfile(data["spikeFile"])):
                 backdata["mode"] = "spike"
                 backdata["fn1"] = os.path.basename(data["spikeFile"])
                 return (backdata, {"spikeFile": data["spikeFile"]})
             else:
                 print("The fasta file (spikeFile=) with localOut spike-in sequences could not be detected")
```


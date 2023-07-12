# Comparing `tmp/tah_data-1.1.1.tar.gz` & `tmp/tah_data-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tah_data-1.1.1.tar", max compression
+gzip compressed data, was "tah_data-1.2.0.tar", max compression
```

## Comparing `tah_data-1.1.1.tar` & `tah_data-1.2.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      324 2023-07-12 11:17:12.558998 tah_data-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3009 2023-07-12 10:57:53.029396 tah_data-1.1.1/src/tah_data.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 tah_data-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      306 2023-07-04 13:12:48.650085 tah_data-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2934 2023-07-04 13:05:41.591737 tah_data-1.2.0/src/tah_data.py
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 tah_data-1.2.0/PKG-INFO
```

### Comparing `tah_data-1.1.1/src/tah_data.py` & `tah_data-1.2.0/src/tah_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,21 +30,16 @@
 
     prepare_creds()
 
 
 def prepare_creds():
     logger.info("checking credentials .....")
     os.chdir(os.environ['repo_dir'])
-    try:
-        subprocess.run('dvc remote modify --local storage access_key_id $AWS_ACCESS_KEY_ID', shell=True,env={'AWS_ACCESS_KEY_ID': os.environ['AWS_ACCESS_KEY_ID']})
-        subprocess.run('dvc remote modify --local storage secret_access_key $AWS_SECRET_ACCESS_KEY', shell=True,env={'AWS_SECRET_ACCESS_KEY': os.environ['AWS_SECRET_ACCESS_KEY']})
-    except KeyError:
-        clean_repo()
-        exit()
-
+    subprocess.run('dvc remote modify --local storage access_key_id $AWS_ACCESS_KEY_ID', shell=True,env={'AWS_ACCESS_KEY_ID': os.environ['AWS_ACCESS_KEY_ID']})
+    subprocess.run('dvc remote modify --local storage secret_access_key $AWS_SECRET_ACCESS_KEY', shell=True,env={'AWS_SECRET_ACCESS_KEY': os.environ['AWS_SECRET_ACCESS_KEY']})
     os.chdir("../")
     logger.info("credentials checked successfully .....")
 
 
 def get_dvc(dir_path,data_version,local_absolute_data_path):
     check_data_exist(data_version,local_absolute_data_path)
     try:
```

### Comparing `tah_data-1.1.1/PKG-INFO` & `tah_data-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tah-data
-Version: 1.1.1
+Version: 1.2.0
 Summary: 
 Author: Ahmed Sherif
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.158,<2.0.0)
 Requires-Dist: dvc (>=3.1.0,<4.0.0)
 Requires-Dist: dvc-s3 (>=2.23.0,<3.0.0)
-Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: pre-commit (>=3.3.2,<4.0.0)
```


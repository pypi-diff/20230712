# Comparing `tmp/tah_data-1.1.4.tar.gz` & `tmp/tah_data-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tah_data-1.1.4.tar", max compression
+gzip compressed data, was "tah_data-1.2.0.tar", max compression
```

## Comparing `tah_data-1.1.4.tar` & `tah_data-1.2.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      324 2023-07-12 11:51:25.478461 tah_data-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     3284 2023-07-12 11:50:55.762287 tah_data-1.1.4/src/tah_data.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 tah_data-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      306 2023-07-04 13:12:48.650085 tah_data-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2934 2023-07-04 13:05:41.591737 tah_data-1.2.0/src/tah_data.py
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 tah_data-1.2.0/PKG-INFO
```

### Comparing `tah_data-1.1.4/src/tah_data.py` & `tah_data-1.2.0/src/tah_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,61 +30,53 @@
 
     prepare_creds()
 
 
 def prepare_creds():
     logger.info("checking credentials .....")
     os.chdir(os.environ['repo_dir'])
-    try:
-        subprocess.run('dvc remote modify --local storage access_key_id $AWS_ACCESS_KEY_ID', executable='/bin/bash',shell=True,env={'AWS_ACCESS_KEY_ID': os.environ['AWS_ACCESS_KEY_ID']})
-        subprocess.run('dvc remote modify --local storage secret_access_key $AWS_SECRET_ACCESS_KEY', executable='/bin/bash', shell=True,env={'AWS_SECRET_ACCESS_KEY': os.environ['AWS_SECRET_ACCESS_KEY']})
-    except Exception as e:
-        clean_repo()
-        logger.error(e)
-        exit()
-
+    subprocess.run('dvc remote modify --local storage access_key_id $AWS_ACCESS_KEY_ID', shell=True,env={'AWS_ACCESS_KEY_ID': os.environ['AWS_ACCESS_KEY_ID']})
+    subprocess.run('dvc remote modify --local storage secret_access_key $AWS_SECRET_ACCESS_KEY', shell=True,env={'AWS_SECRET_ACCESS_KEY': os.environ['AWS_SECRET_ACCESS_KEY']})
     os.chdir("../")
     logger.info("credentials checked successfully .....")
 
 
 def get_dvc(dir_path,data_version,local_absolute_data_path):
     check_data_exist(data_version,local_absolute_data_path)
     try:
-        os.chdir(os.environ['repo_dir']+"/"+dir_path)
+        os.chdir(dir_path)
         logger.info("Cloning Data .....")
-        subprocess.run('dvc pull $dataset', executable='/bin/bash', shell=True,check=True,env={'dataset': data_version})
+        subprocess.run('dvc pull $dataset', shell=True,check=True,env={'dataset': data_version})
     except subprocess.CalledProcessError as e:
         clean_repo()
-        logger.error(e)
         logger.error(" dvc "+ data_version +" not found")
         exit()
     except Exception as e:
         clean_repo()
         logger.error(e)
         exit()
     logger.info("Moving Data .....")
-    subprocess.run('cp -r $src $dst',  executable='/bin/bash',shell=True,check=True,env={'src': data_version ,'dst':local_absolute_data_path })
+    subprocess.run('cp -r $src $dst', shell=True,check=True,env={'src': data_version ,'dst':local_absolute_data_path })
 
 def get_stage(dir_path,stage_name,local_absolute_data_path):
     check_data_exist(stage_name,local_absolute_data_path)
     try:
-        os.chdir(os.environ['repo_dir']+"/"+dir_path)
+        os.chdir(dir_path)
         logger.info("Cloning Data .....")
-        subprocess.run('dvc repro $stage',  executable='/bin/bash',shell=True,check=True,env={'stage': stage_name})
+        subprocess.run('dvc repro $stage', shell=True,check=True,env={'stage': stage_name})
     except subprocess.CalledProcessError as e:
         clean_repo()
-        logger.error(e)
         logger.error(" Stage "+ stage_name +" not found")
         exit()
     except Exception as e:
         clean_repo()
         logger.error(e)
         exit()        
     logger.info("Moving Data .....")
-    subprocess.run('cp -r $src $dst', executable='/bin/bash', shell=True,env={'src': stage_name ,'dst':local_absolute_data_path })
+    subprocess.run('cp -r $src $dst', shell=True,env={'src': stage_name ,'dst':local_absolute_data_path })
 
 def clean_repo():
     os.chdir(os.environ['wd'])
     rmtree(os.environ['repo_dir'])
 
 def check_data_exist(data_version,local_absolute_data_path):
     if (os.path.isdir(local_absolute_data_path+"/"+data_version)):
```

### Comparing `tah_data-1.1.4/PKG-INFO` & `tah_data-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: tah-data
-Version: 1.1.4
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


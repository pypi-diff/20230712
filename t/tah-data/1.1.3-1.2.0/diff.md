# Comparing `tmp/tah_data-1.1.3.tar.gz` & `tmp/tah_data-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tah_data-1.1.3.tar", max compression
+gzip compressed data, was "tah_data-1.2.0.tar", max compression
```

## Comparing `tah_data-1.1.3.tar` & `tah_data-1.2.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      324 2023-07-12 11:41:34.971053 tah_data-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     3141 2023-07-12 11:38:09.649835 tah_data-1.1.3/src/tah_data.py
--rw-r--r--   0        0        0      561 1970-01-01 00:00:00.000000 tah_data-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      306 2023-07-04 13:12:48.650085 tah_data-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2934 2023-07-04 13:05:41.591737 tah_data-1.2.0/src/tah_data.py
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 tah_data-1.2.0/PKG-INFO
```

### Comparing `tah_data-1.1.3/src/tah_data.py` & `tah_data-1.2.0/src/tah_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,53 +30,45 @@
 
     prepare_creds()
 
 
 def prepare_creds():
     logger.info("checking credentials .....")
     os.chdir(os.environ['repo_dir'])
-    try:
-        subprocess.run('dvc remote modify --local storage access_key_id $AWS_ACCESS_KEY_ID', shell=True,env={'AWS_ACCESS_KEY_ID': os.environ['AWS_ACCESS_KEY_ID']})
-        subprocess.run('dvc remote modify --local storage secret_access_key $AWS_SECRET_ACCESS_KEY', shell=True,env={'AWS_SECRET_ACCESS_KEY': os.environ['AWS_SECRET_ACCESS_KEY']})
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
         subprocess.run('dvc pull $dataset', shell=True,check=True,env={'dataset': data_version})
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
     subprocess.run('cp -r $src $dst', shell=True,check=True,env={'src': data_version ,'dst':local_absolute_data_path })
 
 def get_stage(dir_path,stage_name,local_absolute_data_path):
     check_data_exist(stage_name,local_absolute_data_path)
     try:
-        os.chdir(os.environ['repo_dir']+"/"+dir_path)
+        os.chdir(dir_path)
         logger.info("Cloning Data .....")
         subprocess.run('dvc repro $stage', shell=True,check=True,env={'stage': stage_name})
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
```


# Comparing `tmp/driveup-0.7.0.tar.gz` & `tmp/driveup-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "driveup-0.7.0.tar", last modified: Mon May 29 11:16:00 2023, max compression
+gzip compressed data, was "driveup-0.7.1.tar", last modified: Wed Jul 12 12:23:24 2023, max compression
```

## Comparing `driveup-0.7.0.tar` & `driveup-0.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:16:00.446752 driveup-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:16:00.442752 driveup-0.7.0/Driveup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 11:15:48.000000 driveup-0.7.0/Driveup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-29 11:15:48.000000 driveup-0.7.0/Driveup/drive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:16:00.442752 driveup-0.7.0/Driveup/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 11:15:48.000000 driveup-0.7.0/Driveup/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-29 11:15:48.000000 driveup-0.7.0/Driveup/features/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-29 11:15:48.000000 driveup-0.7.0/Driveup/features/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-29 11:15:48.000000 driveup-0.7.0/Driveup/features/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-29 11:15:48.000000 driveup-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-29 11:16:00.446752 driveup-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-29 11:15:48.000000 driveup-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:16:00.446752 driveup-0.7.0/driveup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-29 11:16:00.000000 driveup-0.7.0/driveup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-29 11:16:00.000000 driveup-0.7.0/driveup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 11:16:00.000000 driveup-0.7.0/driveup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-29 11:16:00.000000 driveup-0.7.0/driveup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 11:16:00.000000 driveup-0.7.0/driveup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 11:16:00.446752 driveup-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-29 11:15:48.000000 driveup-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:23:24.216680 driveup-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:23:24.216680 driveup-0.7.1/Driveup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:23:14.000000 driveup-0.7.1/Driveup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-07-12 12:23:14.000000 driveup-0.7.1/Driveup/drive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:23:24.216680 driveup-0.7.1/Driveup/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:23:14.000000 driveup-0.7.1/Driveup/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-12 12:23:14.000000 driveup-0.7.1/Driveup/features/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-12 12:23:14.000000 driveup-0.7.1/Driveup/features/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-12 12:23:14.000000 driveup-0.7.1/Driveup/features/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 12:23:14.000000 driveup-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-12 12:23:24.216680 driveup-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-12 12:23:14.000000 driveup-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:23:24.216680 driveup-0.7.1/driveup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-12 12:23:24.000000 driveup-0.7.1/driveup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 12:23:24.000000 driveup-0.7.1/driveup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:23:24.000000 driveup-0.7.1/driveup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-12 12:23:24.000000 driveup-0.7.1/driveup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 12:23:24.000000 driveup-0.7.1/driveup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:23:24.216680 driveup-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-12 12:23:14.000000 driveup-0.7.1/setup.py
```

### Comparing `driveup-0.7.0/Driveup/drive.py` & `driveup-0.7.1/Driveup/drive.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,26 +90,31 @@
         media = MediaFileUpload(file_path, resumable=True)
         void_metadata = {}
 
         gfile = drive_service.files().update(fileId=file_id, body=void_metadata, media_body=media,supportsAllDrives=True).execute()
 
         return gfile
     
-    def df_update(self,df:Union[pd.DataFrame, List[pd.DataFrame]],id:str,sheet_name:str = None):
+    def df_update(self,df:Union[pd.DataFrame, List[pd.DataFrame]],id:str,sheet_name:str = None,unformat:bool = False):
+
 
         sheets_service = self.sheets_service
 
         sheets = sheets_service.spreadsheets().get(spreadsheetId=id).execute().get('sheets', '')
         # sheet_id = sheets[0].get("properties", {}).get("sheetId", 0)
 
         if isinstance(df, list): 
             for single_df,sheet in zip(df,sheets):
                 sheet_name = sheet.get("properties", {}).get("title", "Sheet1")
                 self.df_update(single_df,id,sheet_name)       
         else:
+            if unformat == True:
+                df = df.fillna('NULL')
+                df = df.astype(str)
+
             if sheet_name == None:
                 sheet_name = sheets[0].get("properties", {}).get("title", "Sheet1")
 
             values = [df.columns.tolist()] + df.values.tolist()
 
             value_range = {
                 'range': sheet_name,  # Specify the range where you want to update the values
```

### Comparing `driveup-0.7.0/Driveup/features/auth.py` & `driveup-0.7.1/Driveup/features/auth.py`

 * *Files identical despite different names*

### Comparing `driveup-0.7.0/Driveup/features/service.py` & `driveup-0.7.1/Driveup/features/service.py`

 * *Files identical despite different names*

### Comparing `driveup-0.7.0/Driveup/features/utils.py` & `driveup-0.7.1/Driveup/features/utils.py`

 * *Files identical despite different names*

### Comparing `driveup-0.7.0/LICENSE` & `driveup-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `driveup-0.7.0/PKG-INFO` & `driveup-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: driveup
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python package for uploading files and folders to Google Drive.
 Home-page: https://github.com/raul-martin-dev/Driveup
 Author: Raúl M.R.
 Author-email: raul.martin4bc@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-Metadata-Version: 2.1 Name: driveup Version: 0.7.0 Summary: Python package for
+Metadata-Version: 2.1 Name: driveup Version: 0.7.1 Summary: Python package for
 uploading files and folders to Google Drive. Home-page: https://github.com/
 raul-martin-dev/Driveup Author: RaÃºl M.R. Author-email:
 raul.martin4bc@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Python package for uploading files and folders to Google
 Drive
                               [PyPI] [downloads]
```

### Comparing `driveup-0.7.0/driveup.egg-info/PKG-INFO` & `driveup-0.7.1/driveup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: driveup
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python package for uploading files and folders to Google Drive.
 Home-page: https://github.com/raul-martin-dev/Driveup
 Author: Raúl M.R.
 Author-email: raul.martin4bc@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-Metadata-Version: 2.1 Name: driveup Version: 0.7.0 Summary: Python package for
+Metadata-Version: 2.1 Name: driveup Version: 0.7.1 Summary: Python package for
 uploading files and folders to Google Drive. Home-page: https://github.com/
 raul-martin-dev/Driveup Author: RaÃºl M.R. Author-email:
 raul.martin4bc@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Python package for uploading files and folders to Google
 Drive
                               [PyPI] [downloads]
```

### Comparing `driveup-0.7.0/setup.py` & `driveup-0.7.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # ...
 
 setup(
     long_description=README_DESCRIPTION,
     long_description_content_type="text/markdown",
     name='driveup',
-    version='0.7.0',
+    version='0.7.1',
     author='Raúl M.R.',
     author_email="raul.martin4bc@gmail.com",
     url="https://github.com/raul-martin-dev/Driveup",
     license="MIT",
     description='Python package for uploading files and folders to Google Drive.',
     packages=find_packages(include=["Driveup","Driveup.features"]),
     install_requires=[
```


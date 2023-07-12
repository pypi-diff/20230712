# Comparing `tmp/FileInfo_Video_Audio-0.1.2.tar.gz` & `tmp/FileInfo_Video_Audio-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileInfo_Video_Audio-0.1.2.tar", last modified: Fri May 19 13:46:31 2023, max compression
+gzip compressed data, was "FileInfo_Video_Audio-0.1.3.tar", last modified: Wed Jul 12 12:15:43 2023, max compression
```

## Comparing `FileInfo_Video_Audio-0.1.2.tar` & `FileInfo_Video_Audio-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-19 13:46:31.304569 FileInfo_Video_Audio-0.1.2/
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-19 13:46:31.300569 FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1496 2023-05-19 13:46:31.000000 FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      321 2023-05-19 13:46:31.000000 FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/SOURCES.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-05-19 13:46:31.000000 FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/dependency_links.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       62 2023-05-19 13:46:31.000000 FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/entry_points.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-05-19 13:46:31.000000 FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/top_level.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1496 2023-05-19 13:46:31.300569 FileInfo_Video_Audio-0.1.2/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1125 2023-05-19 13:36:10.000000 FileInfo_Video_Audio-0.1.2/README.md
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-05-19 13:46:31.304569 FileInfo_Video_Audio-0.1.2/setup.cfg
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      815 2023-05-19 13:46:10.000000 FileInfo_Video_Audio-0.1.2/setup.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-19 13:46:31.300569 FileInfo_Video_Audio-0.1.2/source/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-19 13:31:53.000000 FileInfo_Video_Audio-0.1.2/source/__init__.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-19 13:46:31.300569 FileInfo_Video_Audio-0.1.2/source/lib/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1272 2023-05-19 13:31:53.000000 FileInfo_Video_Audio-0.1.2/source/lib/Argument.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       36 2023-05-19 13:31:53.000000 FileInfo_Video_Audio-0.1.2/source/lib/__init__.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     3875 2023-05-19 13:31:53.000000 FileInfo_Video_Audio-0.1.2/source/main.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-07-12 12:15:43.311082 FileInfo_Video_Audio-0.1.3/
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-07-12 12:15:43.307082 FileInfo_Video_Audio-0.1.3/FileInfo_Video_Audio.egg-info/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1496 2023-07-12 12:15:43.000000 FileInfo_Video_Audio-0.1.3/FileInfo_Video_Audio.egg-info/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      321 2023-07-12 12:15:43.000000 FileInfo_Video_Audio-0.1.3/FileInfo_Video_Audio.egg-info/SOURCES.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-07-12 12:15:43.000000 FileInfo_Video_Audio-0.1.3/FileInfo_Video_Audio.egg-info/dependency_links.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       62 2023-07-12 12:15:43.000000 FileInfo_Video_Audio-0.1.3/FileInfo_Video_Audio.egg-info/entry_points.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-07-12 12:15:43.000000 FileInfo_Video_Audio-0.1.3/FileInfo_Video_Audio.egg-info/top_level.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1496 2023-07-12 12:15:43.307082 FileInfo_Video_Audio-0.1.3/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1125 2023-05-19 14:03:53.000000 FileInfo_Video_Audio-0.1.3/README.md
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-07-12 12:15:43.311082 FileInfo_Video_Audio-0.1.3/setup.cfg
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      815 2023-07-11 18:29:35.000000 FileInfo_Video_Audio-0.1.3/setup.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-07-12 12:15:43.307082 FileInfo_Video_Audio-0.1.3/source/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-05-19 14:03:40.000000 FileInfo_Video_Audio-0.1.3/source/__init__.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-07-12 12:15:43.307082 FileInfo_Video_Audio-0.1.3/source/lib/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1272 2023-05-19 14:03:40.000000 FileInfo_Video_Audio-0.1.3/source/lib/Argument.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       36 2023-05-19 14:03:40.000000 FileInfo_Video_Audio-0.1.3/source/lib/__init__.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     5499 2023-07-12 12:15:41.000000 FileInfo_Video_Audio-0.1.3/source/main.py
```

### Comparing `FileInfo_Video_Audio-0.1.2/FileInfo_Video_Audio.egg-info/PKG-INFO` & `FileInfo_Video_Audio-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: FileInfo-Video-Audio
-Version: 0.1.2
+Name: FileInfo_Video_Audio
+Version: 0.1.3
 Summary: In this tool is help to get the properties of the Audio and Video files
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/collage_sem_4_python_project_cli_file_details
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `FileInfo_Video_Audio-0.1.2/PKG-INFO` & `FileInfo_Video_Audio-0.1.3/FileInfo_Video_Audio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: FileInfo_Video_Audio
-Version: 0.1.2
+Name: FileInfo-Video-Audio
+Version: 0.1.3
 Summary: In this tool is help to get the properties of the Audio and Video files
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/collage_sem_4_python_project_cli_file_details
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `FileInfo_Video_Audio-0.1.2/README.md` & `FileInfo_Video_Audio-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `FileInfo_Video_Audio-0.1.2/setup.py` & `FileInfo_Video_Audio-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = os.popen("/usr/local/bin/pipreqs main --print").read().splitlines()
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='FileInfo_Video_Audio',
-    version='0.1.2',
+    version='0.1.3',
     author='Sridhar',
     author_email='dcsvsridhar@gmail.com',
     description="In this tool is help to get the properties of the Audio and Video files",
     packages=find_packages(),
     url='https://git.selfmade.ninja/SRIDHARDSCV/collage_sem_4_python_project_cli_file_details',
     install_requires=requirements,
     long_description=long_description,
```

### Comparing `FileInfo_Video_Audio-0.1.2/source/lib/Argument.py` & `FileInfo_Video_Audio-0.1.3/source/lib/Argument.py`

 * *Files identical despite different names*


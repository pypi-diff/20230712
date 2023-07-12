# Comparing `tmp/pyanalyticsgit-0.0.1.tar.gz` & `tmp/pyanalyticsgit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanalyticsgit-0.0.1.tar", last modified: Wed Jul 12 13:20:09 2023, max compression
+gzip compressed data, was "pyanalyticsgit-0.0.2.tar", last modified: Wed Jul 12 15:38:08 2023, max compression
```

## Comparing `pyanalyticsgit-0.0.1.tar` & `pyanalyticsgit-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-12 13:20:09.668517 pyanalyticsgit-0.0.1/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1064 2023-07-12 01:24:27.000000 pyanalyticsgit-0.0.1/LICENSE
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6726 2023-07-12 13:20:09.668517 pyanalyticsgit-0.0.1/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6391 2023-07-12 13:13:13.000000 pyanalyticsgit-0.0.1/README.md
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-12 13:20:09.668517 pyanalyticsgit-0.0.1/pyanalyticsgit/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       19 2023-07-12 13:14:32.000000 pyanalyticsgit-0.0.1/pyanalyticsgit/__init__.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      314 2023-07-12 02:11:31.000000 pyanalyticsgit-0.0.1/pyanalyticsgit/monitoramento.py
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-12 13:20:09.668517 pyanalyticsgit-0.0.1/pyanalyticsgit/repo/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-07-12 01:24:27.000000 pyanalyticsgit-0.0.1/pyanalyticsgit/repo/__init__.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4922 2023-07-12 13:03:28.000000 pyanalyticsgit-0.0.1/pyanalyticsgit/repo/automatizar.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4478 2023-07-12 01:24:27.000000 pyanalyticsgit-0.0.1/pyanalyticsgit/repo/commit.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2689 2023-07-12 01:24:27.000000 pyanalyticsgit-0.0.1/pyanalyticsgit/repo/connect.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4141 2023-07-12 01:24:27.000000 pyanalyticsgit-0.0.1/pyanalyticsgit/repo/issue.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3046 2023-07-12 01:24:27.000000 pyanalyticsgit-0.0.1/pyanalyticsgit/repo/milestone.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3408 2023-07-12 01:24:27.000000 pyanalyticsgit-0.0.1/pyanalyticsgit/repo/relatorio.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1361 2023-07-12 02:10:21.000000 pyanalyticsgit-0.0.1/pyanalyticsgit/test_linux.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1363 2023-07-12 02:10:19.000000 pyanalyticsgit-0.0.1/pyanalyticsgit/test_macos.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1063 2023-07-12 02:10:18.000000 pyanalyticsgit-0.0.1/pyanalyticsgit/test_windows.py
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-12 13:20:09.668517 pyanalyticsgit-0.0.1/pyanalyticsgit.egg-info/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6726 2023-07-12 13:20:09.000000 pyanalyticsgit-0.0.1/pyanalyticsgit.egg-info/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      586 2023-07-12 13:20:09.000000 pyanalyticsgit-0.0.1/pyanalyticsgit.egg-info/SOURCES.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-12 13:20:09.000000 pyanalyticsgit-0.0.1/pyanalyticsgit.egg-info/dependency_links.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       92 2023-07-12 13:20:09.000000 pyanalyticsgit-0.0.1/pyanalyticsgit.egg-info/requires.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       35 2023-07-12 13:20:09.000000 pyanalyticsgit-0.0.1/pyanalyticsgit.egg-info/top_level.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       38 2023-07-12 13:20:09.668517 pyanalyticsgit-0.0.1/setup.cfg
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      748 2023-07-12 13:19:11.000000 pyanalyticsgit-0.0.1/setup.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-12 15:38:08.722398 pyanalyticsgit-0.0.2/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1064 2023-07-12 01:24:27.000000 pyanalyticsgit-0.0.2/LICENSE
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6726 2023-07-12 15:38:08.722398 pyanalyticsgit-0.0.2/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6391 2023-07-12 15:34:48.000000 pyanalyticsgit-0.0.2/README.md
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-12 15:38:08.718398 pyanalyticsgit-0.0.2/pyanalyticsgit/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       19 2023-07-12 13:14:32.000000 pyanalyticsgit-0.0.2/pyanalyticsgit/__init__.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      352 2023-07-12 15:35:42.000000 pyanalyticsgit-0.0.2/pyanalyticsgit/monitoramento.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-12 15:38:08.722398 pyanalyticsgit-0.0.2/pyanalyticsgit/repo/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-07-12 01:24:27.000000 pyanalyticsgit-0.0.2/pyanalyticsgit/repo/__init__.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4922 2023-07-12 15:34:48.000000 pyanalyticsgit-0.0.2/pyanalyticsgit/repo/automatizar.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4478 2023-07-12 01:24:27.000000 pyanalyticsgit-0.0.2/pyanalyticsgit/repo/commit.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2764 2023-07-12 15:35:18.000000 pyanalyticsgit-0.0.2/pyanalyticsgit/repo/connect.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4141 2023-07-12 01:24:27.000000 pyanalyticsgit-0.0.2/pyanalyticsgit/repo/issue.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3046 2023-07-12 01:24:27.000000 pyanalyticsgit-0.0.2/pyanalyticsgit/repo/milestone.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3408 2023-07-12 01:24:27.000000 pyanalyticsgit-0.0.2/pyanalyticsgit/repo/relatorio.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1361 2023-07-12 15:34:48.000000 pyanalyticsgit-0.0.2/pyanalyticsgit/test_linux.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1363 2023-07-12 15:34:48.000000 pyanalyticsgit-0.0.2/pyanalyticsgit/test_macos.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1063 2023-07-12 15:34:48.000000 pyanalyticsgit-0.0.2/pyanalyticsgit/test_windows.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-12 15:38:08.722398 pyanalyticsgit-0.0.2/pyanalyticsgit.egg-info/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6726 2023-07-12 15:38:08.000000 pyanalyticsgit-0.0.2/pyanalyticsgit.egg-info/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      586 2023-07-12 15:38:08.000000 pyanalyticsgit-0.0.2/pyanalyticsgit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-12 15:38:08.000000 pyanalyticsgit-0.0.2/pyanalyticsgit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       92 2023-07-12 15:38:08.000000 pyanalyticsgit-0.0.2/pyanalyticsgit.egg-info/requires.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       35 2023-07-12 15:38:08.000000 pyanalyticsgit-0.0.2/pyanalyticsgit.egg-info/top_level.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       38 2023-07-12 15:38:08.722398 pyanalyticsgit-0.0.2/setup.cfg
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      748 2023-07-12 15:36:56.000000 pyanalyticsgit-0.0.2/setup.py
```

### Comparing `pyanalyticsgit-0.0.1/LICENSE` & `pyanalyticsgit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.1/PKG-INFO` & `pyanalyticsgit-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanalyticsgit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Biblioteca PyAnalyticsGit para gerar relatórios Git.
 Home-page: UNKNOWN
 Author: Jefferson Sena
 Author-email: jeffersonsena12144@gmail.com
 License: MIT License
 Keywords: pyAnalyticsGit
 Platform: UNKNOWN
```

### Comparing `pyanalyticsgit-0.0.1/README.md` & `pyanalyticsgit-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.1/pyanalyticsgit/repo/automatizar.py` & `pyanalyticsgit-0.0.2/pyanalyticsgit/repo/automatizar.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.1/pyanalyticsgit/repo/commit.py` & `pyanalyticsgit-0.0.2/pyanalyticsgit/repo/commit.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.1/pyanalyticsgit/repo/connect.py` & `pyanalyticsgit-0.0.2/pyanalyticsgit/repo/connect.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import requests
 from dotenv import load_dotenv
 import os
 
 diretorio_atual = os.getcwd()
 arquivo_env = os.path.join(diretorio_atual,'.env')
 
+api_user = ""
+api_name = ""
+
 load_dotenv(arquivo_env)
 
 if os.path.exists(arquivo_env):
     api_user = os.getenv("user_name")
     api_name = os.getenv("repo_name")
 else:
-    print(f'O arquivo não existe em {diretorio_atual}')
+    print(f'Caso queira automatizar os commits insira o arquivo .env no diretório {diretorio_atual}')
 
 class Connect:
     def __init__(self):
         pass
 
     def connect_issue(self, user = api_user, repo = api_name):
         page = 1
```

### Comparing `pyanalyticsgit-0.0.1/pyanalyticsgit/repo/issue.py` & `pyanalyticsgit-0.0.2/pyanalyticsgit/repo/issue.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.1/pyanalyticsgit/repo/milestone.py` & `pyanalyticsgit-0.0.2/pyanalyticsgit/repo/milestone.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.1/pyanalyticsgit/repo/relatorio.py` & `pyanalyticsgit-0.0.2/pyanalyticsgit/repo/relatorio.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.1/pyanalyticsgit/test_linux.py` & `pyanalyticsgit-0.0.2/pyanalyticsgit/test_linux.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.1/pyanalyticsgit/test_macos.py` & `pyanalyticsgit-0.0.2/pyanalyticsgit/test_macos.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.1/pyanalyticsgit/test_windows.py` & `pyanalyticsgit-0.0.2/pyanalyticsgit/test_windows.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.1/pyanalyticsgit.egg-info/PKG-INFO` & `pyanalyticsgit-0.0.2/pyanalyticsgit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanalyticsgit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Biblioteca PyAnalyticsGit para gerar relatórios Git.
 Home-page: UNKNOWN
 Author: Jefferson Sena
 Author-email: jeffersonsena12144@gmail.com
 License: MIT License
 Keywords: pyAnalyticsGit
 Platform: UNKNOWN
```

### Comparing `pyanalyticsgit-0.0.1/pyanalyticsgit.egg-info/SOURCES.txt` & `pyanalyticsgit-0.0.2/pyanalyticsgit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.1/setup.py` & `pyanalyticsgit-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools.dist import Distribution
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='pyanalyticsgit',
-    version='0.0.1',
+    version='0.0.2',
     license='MIT License',
     author='Jefferson Sena',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='jeffersonsena12144@gmail.com',
     keywords='pyAnalyticsGit',
     description=u'Biblioteca PyAnalyticsGit para gerar relatórios Git.',
```


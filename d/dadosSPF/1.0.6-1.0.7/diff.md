# Comparing `tmp/dadosSPF-1.0.6.tar.gz` & `tmp/dadosSPF-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dadosSPF-1.0.6.tar", last modified: Wed Jul 12 18:22:03 2023, max compression
+gzip compressed data, was "dist/dadosSPF-1.0.7.tar", last modified: Wed Jul 12 18:42:28 2023, max compression
```

## Comparing `dadosSPF-1.0.6.tar` & `dadosSPF-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:22:03.000000 dadosSPF-1.0.6/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-07-12 18:22:03.000000 dadosSPF-1.0.6/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      773 2023-07-11 22:32:57.000000 dadosSPF-1.0.6/README.md
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:22:03.000000 dadosSPF-1.0.6/dadosSPF/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-06-13 13:21:19.000000 dadosSPF-1.0.6/dadosSPF/__init__.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)    41125 2023-07-12 18:21:36.000000 dadosSPF-1.0.6/dadosSPF/dadosSPF.py
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:22:03.000000 dadosSPF-1.0.6/dadosSPF.egg-info/
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:22:03.000000 dadosSPF-1.0.6/dadosSPF.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-07-12 18:21:34.000000 dadosSPF-1.0.6/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      219 2023-06-13 13:21:19.000000 dadosSPF-1.0.6/dadosSPF.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-06-13 13:23:37.000000 dadosSPF-1.0.6/dadosSPF.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-06-13 13:22:59.000000 dadosSPF-1.0.6/dadosSPF.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        8 2023-07-12 17:57:17.000000 dadosSPF-1.0.6/dadosSPF.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-07-12 18:22:03.000000 dadosSPF-1.0.6/dadosSPF.egg-info/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      528 2023-07-12 18:22:03.000000 dadosSPF-1.0.6/dadosSPF.egg-info/SOURCES.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-07-12 18:22:03.000000 dadosSPF-1.0.6/dadosSPF.egg-info/dependency_links.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-07-12 18:22:03.000000 dadosSPF-1.0.6/dadosSPF.egg-info/requires.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-07-12 18:22:03.000000 dadosSPF-1.0.6/dadosSPF.egg-info/top_level.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2023-07-12 18:22:03.000000 dadosSPF-1.0.6/setup.cfg
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      548 2023-07-12 18:21:46.000000 dadosSPF-1.0.6/setup.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:42:28.000000 dadosSPF-1.0.7/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-07-12 18:42:28.000000 dadosSPF-1.0.7/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      773 2023-07-11 22:32:57.000000 dadosSPF-1.0.7/README.md
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:42:28.000000 dadosSPF-1.0.7/dadosSPF/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-06-13 13:21:19.000000 dadosSPF-1.0.7/dadosSPF/__init__.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)    41131 2023-07-12 18:42:00.000000 dadosSPF-1.0.7/dadosSPF/dadosSPF.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:42:28.000000 dadosSPF-1.0.7/dadosSPF.egg-info/
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:42:28.000000 dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-07-12 18:42:20.000000 dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      219 2023-06-13 13:21:19.000000 dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-06-13 13:23:37.000000 dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-06-13 13:22:59.000000 dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        8 2023-07-12 17:57:17.000000 dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-07-12 18:42:27.000000 dadosSPF-1.0.7/dadosSPF.egg-info/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      528 2023-07-12 18:42:27.000000 dadosSPF-1.0.7/dadosSPF.egg-info/SOURCES.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-07-12 18:42:27.000000 dadosSPF-1.0.7/dadosSPF.egg-info/dependency_links.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-07-12 18:42:27.000000 dadosSPF-1.0.7/dadosSPF.egg-info/requires.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-07-12 18:42:27.000000 dadosSPF-1.0.7/dadosSPF.egg-info/top_level.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2023-07-12 18:42:28.000000 dadosSPF-1.0.7/setup.cfg
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      548 2023-07-12 18:42:09.000000 dadosSPF-1.0.7/setup.py
```

### Comparing `dadosSPF-1.0.6/PKG-INFO` & `dadosSPF-1.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.6
+Version: 1.0.7
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
```

### Comparing `dadosSPF-1.0.6/README.md` & `dadosSPF-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dadosSPF-1.0.6/dadosSPF/dadosSPF.py` & `dadosSPF-1.0.7/dadosSPF/dadosSPF.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ =     "CARLOS PIVETA"
 __collaborators__ = "CARLOS PIVETA"
 __license__ =    "DADOS"
-__version__ =    "1.0.6"
+__version__ =    "1.0.7"
 __maintainer__ = "CARLOS PIVETA"
 __status__ =     "Production"
 
 import os
 import re
 import sys
 import glob
@@ -806,22 +806,22 @@
 
                 for tt in range(len(tables)):
                     if tables[tt][1].replace('(','').replace(')','') == '':
                         pass
                     else:
                         schema = tables[tt][1].lower().split('.')[0]
                         tabela = tables[tt][1].lower().split('.')[1]
-                        s.getSpark()
+                        self.getSpark()
                         lp = self.getLastPartition(schema,tabela,dPrint = False)
                         if lp != None:
                             str_where[tables[tt][1].lower().split('.')[1]] = "" + "'" + lp +"'"
 
                 executionPlan = query.format(**str_where).split(';')
 
-                impala = s.getImpala()
+                impala = self.getImpala()
                 for i in range(len(executionPlan)):
                     try:
                         val = executionPlan[i].replace('\n',' ')
                         print(f'Executando : {val}')
                         impala.execute(executionPlan[i])
                         print(f'-----FINALIZADO -----')
                     except Exception as e:
```

### Comparing `dadosSPF-1.0.6/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `dadosSPF-1.0.7/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.6
+Version: 1.0.7
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
```

### Comparing `dadosSPF-1.0.6/dadosSPF.egg-info/PKG-INFO` & `dadosSPF-1.0.7/dadosSPF.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.6
+Version: 1.0.7
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
```

### Comparing `dadosSPF-1.0.6/dadosSPF.egg-info/SOURCES.txt` & `dadosSPF-1.0.7/dadosSPF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dadosSPF-1.0.6/setup.py` & `dadosSPF-1.0.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(
     name='dadosSPF',
-    version='1.0.6',
+    version='1.0.7',
     url='https://gitlab.com.br/dadosSPF',
     license='MIT License',
     author='Carlos Piveta',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='cepo496@gmail.com',
     keywords='Pacote',
```


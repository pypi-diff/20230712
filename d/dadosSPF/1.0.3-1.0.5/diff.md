# Comparing `tmp/dadosSPF-1.0.3.tar.gz` & `tmp/dadosSPF-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dadosSPF-1.0.3.tar", last modified: Tue Jul 11 19:33:40 2023, max compression
+gzip compressed data, was "dist/dadosSPF-1.0.5.tar", last modified: Wed Jul 12 18:02:10 2023, max compression
```

## Comparing `dadosSPF-1.0.3.tar` & `dadosSPF-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-11 19:33:40.000000 dadosSPF-1.0.3/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1309 2023-07-11 19:33:40.000000 dadosSPF-1.0.3/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      781 2023-06-13 13:23:21.000000 dadosSPF-1.0.3/README.md
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-11 19:33:39.000000 dadosSPF-1.0.3/dadosSPF/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-06-13 13:21:19.000000 dadosSPF-1.0.3/dadosSPF/__init__.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)    40912 2023-07-11 19:33:12.000000 dadosSPF-1.0.3/dadosSPF/dadosSPF.py
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-11 19:33:40.000000 dadosSPF-1.0.3/dadosSPF.egg-info/
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-11 19:33:40.000000 dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1328 2023-06-13 13:22:55.000000 dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      219 2023-06-13 13:21:19.000000 dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-06-13 13:23:37.000000 dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-06-13 13:22:59.000000 dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-06-13 13:21:19.000000 dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1309 2023-07-11 19:33:38.000000 dadosSPF-1.0.3/dadosSPF.egg-info/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      528 2023-07-11 19:33:39.000000 dadosSPF-1.0.3/dadosSPF.egg-info/SOURCES.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-07-11 19:33:38.000000 dadosSPF-1.0.3/dadosSPF.egg-info/dependency_links.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-07-11 19:33:38.000000 dadosSPF-1.0.3/dadosSPF.egg-info/requires.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-07-11 19:33:38.000000 dadosSPF-1.0.3/dadosSPF.egg-info/top_level.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2023-07-11 19:33:40.000000 dadosSPF-1.0.3/setup.cfg
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      545 2023-07-11 19:17:28.000000 dadosSPF-1.0.3/setup.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:02:10.000000 dadosSPF-1.0.5/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-07-12 18:02:10.000000 dadosSPF-1.0.5/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      773 2023-07-11 22:32:57.000000 dadosSPF-1.0.5/README.md
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:02:10.000000 dadosSPF-1.0.5/dadosSPF/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-06-13 13:21:19.000000 dadosSPF-1.0.5/dadosSPF/__init__.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)    41128 2023-07-12 18:01:14.000000 dadosSPF-1.0.5/dadosSPF/dadosSPF.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:02:10.000000 dadosSPF-1.0.5/dadosSPF.egg-info/
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-07-12 18:02:10.000000 dadosSPF-1.0.5/dadosSPF.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-07-12 18:01:29.000000 dadosSPF-1.0.5/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      219 2023-06-13 13:21:19.000000 dadosSPF-1.0.5/dadosSPF.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-06-13 13:23:37.000000 dadosSPF-1.0.5/dadosSPF.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-06-13 13:22:59.000000 dadosSPF-1.0.5/dadosSPF.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        8 2023-07-12 17:57:17.000000 dadosSPF-1.0.5/dadosSPF.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1301 2023-07-12 18:02:09.000000 dadosSPF-1.0.5/dadosSPF.egg-info/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      528 2023-07-12 18:02:09.000000 dadosSPF-1.0.5/dadosSPF.egg-info/SOURCES.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-07-12 18:02:09.000000 dadosSPF-1.0.5/dadosSPF.egg-info/dependency_links.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-07-12 18:02:09.000000 dadosSPF-1.0.5/dadosSPF.egg-info/requires.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-07-12 18:02:09.000000 dadosSPF-1.0.5/dadosSPF.egg-info/top_level.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2023-07-12 18:02:10.000000 dadosSPF-1.0.5/setup.cfg
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      548 2023-07-12 18:01:53.000000 dadosSPF-1.0.5/setup.py
```

### Comparing `dadosSPF-1.0.3/PKG-INFO` & `dadosSPF-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.3
+Version: 1.0.5
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
         
         ## Getting Started
         #### Dependencies
         Você precisa do Python 3.7 ou posterior para usar dadosSPF.
         Você pode encontrá-lo em [python.org] (https://www.python.org/).
-        Você precisa do PySpark 2.4.7 para usar safraPyFunctions.
+        Você precisa do PySpark 2.4.7 para usar dadosSPF.
         Você pode encontrá-lo em [spark.apache.org] (https://spark.apache.org/docs/latest/api/python/).
         
         You also need pandas, holidays and impyla packages, which is available from [PyPI](https://pypi.org). If you have pip, just run:
         '''
         pip install pandas
         pip install holidays
         pip install impyla
```

### Comparing `dadosSPF-1.0.3/README.md` & `dadosSPF-1.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # dadosSPF
 
 ## Getting Started
 #### Dependencies
 Você precisa do Python 3.7 ou posterior para usar dadosSPF.
 Você pode encontrá-lo em [python.org] (https://www.python.org/).
-Você precisa do PySpark 2.4.7 para usar safraPyFunctions.
+Você precisa do PySpark 2.4.7 para usar dadosSPF.
 Você pode encontrá-lo em [spark.apache.org] (https://spark.apache.org/docs/latest/api/python/).
 
 You also need pandas, holidays and impyla packages, which is available from [PyPI](https://pypi.org). If you have pip, just run:
 '''
 pip install pandas
 pip install holidays
 pip install impyla
```

### Comparing `dadosSPF-1.0.3/dadosSPF/dadosSPF.py` & `dadosSPF-1.0.5/dadosSPF/dadosSPF.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ =     "CARLOS PIVETA"
 __collaborators__ = "CARLOS PIVETA"
 __license__ =    "DADOS"
-__version__ =    "1.0.3"
+__version__ =    "1.0.5"
 __maintainer__ = "CARLOS PIVETA"
 __status__ =     "Production"
 
 import os
 import re
 import sys
 import glob
@@ -764,77 +764,77 @@
                     move = False
                     print(e)
                 if move == True:
                     shutil.move(file, pasta+'carregados/'+arq)
         else:
             print('Sem arquivos para serem carregados')
     
-def procImpalaSBX(self,strPasta = 'queries', strProc = 'MACRO', variaveis = {"strMes": "202302","strFim":'2023-07-31',"sandbox": self.sandbox}):
-    try:    
-        debugPrint = True
-        path = strPasta
-        files = os.listdir(strPasta)
-        str_where = {}
-        str_where = {**str_where, **variaveis}
-
-        if strProc != None:
-                file = strProc
-                file = file if file[-4:].lower() == '.txt' else file+'.txt'
-                resp = filter(lambda x: x == file, files)
-                resp = list(resp)
-
-                if resp != []:
-                    files = resp
-
-        files = sorted(files)
-        for fls in range(len(files)):
-            if files[fls].endswith(".txt"):
-                proc = files[fls].replace('.txt','')
-                with open(path+r'/'+files[fls], 'r') as file:
-                    query = file.read()
-                    try:
-                        query = query.format(**str_where)
-                    except Exception as e:
-                        print(e)
-                    table = files[fls].replace('.txt','')
-                    tmpTxt = query.replace(';','')
-                    arquivo = files[fls].replace('.txt','')
-                    tmptables = re.findall(r'FROM(.*?)(\S+)',tmpTxt.upper())
-                    tmptables = tmptables+re.findall(r'JOIN(.*?)(\S+)',tmpTxt.upper())
-                    tmptables = tmptables+re.findall(r'JOIN(.*?)(\S+)',tmpTxt.upper())
-                    tables = list(set(tmptables))
-                    tmpTxt = None
+    def procImpalaSBX(self,strPasta = 'queries', strProc = 'MACRO', variaveis = {"strMes": "202302","strFim":'2023-07-31',"sandbox": self.sandbox}):
+        try:    
+            debugPrint = True
+            path = strPasta
+            files = os.listdir(strPasta)
+            str_where = {}
+            str_where = {**str_where, **variaveis}
+
+            if strProc != None:
+                    file = strProc
+                    file = file if file[-4:].lower() == '.txt' else file+'.txt'
+                    resp = filter(lambda x: x == file, files)
+                    resp = list(resp)
+
+                    if resp != []:
+                        files = resp
+
+            files = sorted(files)
+            for fls in range(len(files)):
+                if files[fls].endswith(".txt"):
+                    proc = files[fls].replace('.txt','')
+                    with open(path+r'/'+files[fls], 'r') as file:
+                        query = file.read()
+                        try:
+                            query = query.format(**str_where)
+                        except Exception as e:
+                            print(e)
+                        table = files[fls].replace('.txt','')
+                        tmpTxt = query.replace(';','')
+                        arquivo = files[fls].replace('.txt','')
+                        tmptables = re.findall(r'FROM(.*?)(\S+)',tmpTxt.upper())
+                        tmptables = tmptables+re.findall(r'JOIN(.*?)(\S+)',tmpTxt.upper())
+                        tmptables = tmptables+re.findall(r'JOIN(.*?)(\S+)',tmpTxt.upper())
+                        tables = list(set(tmptables))
+                        tmpTxt = None
+
+                for tt in range(len(tables)):
+                    if tables[tt][1].replace('(','').replace(')','') == '':
+                        pass
+                    else:
+                        schema = tables[tt][1].lower().split('.')[0]
+                        tabela = tables[tt][1].lower().split('.')[1]
+                        s.getSpark()
+                        lp = self.getLastPartition(schema,tabela,dPrint = False)
+                        if lp != None:
+                            str_where[tables[tt][1].lower().split('.')[1]] = "" + "'" + lp +"'"
 
-            for tt in range(len(tables)):
-                if tables[tt][1].replace('(','').replace(')','') == '':
-                    pass
-                else:
-                    schema = tables[tt][1].lower().split('.')[0]
-                    tabela = tables[tt][1].lower().split('.')[1]
-                    s.getSpark()
-                    lp = self.getLastPartition(schema,tabela,dPrint = False)
-                    if lp != None:
-                        str_where[tables[tt][1].lower().split('.')[1]] = "" + "'" + lp +"'"
+                executionPlan = query.format(**str_where).split(';')
 
-            executionPlan = query.format(**str_where).split(';')
+                impala = s.getImpala()
+                for i in range(len(executionPlan)):
+                    try:
+                        val = executionPlan[i].replace('\n',' ')
+                        print(f'Executando : {val}')
+                        impala.execute(executionPlan[i])
+                        print(f'-----FINALIZADO -----')
+                    except Exception as e:
+                        print(f'-----!!! ERRO !!!-----')
+                        print(e)   
+                        pass
 
-            impala = s.getImpala()
-            for i in range(len(executionPlan)):
-                try:
-                    val = executionPlan[i].replace('\n',' ')
-                    print(f'Executando : {val}')
-                    impala.execute(executionPlan[i])
-                    print(f'-----FINALIZADO -----')
-                except Exception as e:
-                    print(f'-----!!! ERRO !!!-----')
-                    print(e)   
-                    pass
-        
-    except Exception as e:
-        print(e)
+        except Exception as e:
+            print(e)
             
 # -------------------------------------------------------------------------------------------------------------------------------
 # | CLASS TOOLS
 # -------------------------------------------------------------------------------------------------------------------------------
 
 class tool():
     """
```

### Comparing `dadosSPF-1.0.3/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `dadosSPF-1.0.5/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.1
+Version: 1.0.5
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
         
         ## Getting Started
         #### Dependencies
-        Você precisa do Python 3.7 ou posterior para usar safraPyFunctions.
+        Você precisa do Python 3.7 ou posterior para usar dadosSPF.
         Você pode encontrá-lo em [python.org] (https://www.python.org/).
-        Você precisa do PySpark 2.4.7 para usar safraPyFunctions.
+        Você precisa do PySpark 2.4.7 para usar dadosSPF.
         Você pode encontrá-lo em [spark.apache.org] (https://spark.apache.org/docs/latest/api/python/).
         
-        You also need pandas, unidecode, holidays and impyla packages, which is available from [PyPI](https://pypi.org). If you have pip, just run:
+        You also need pandas, holidays and impyla packages, which is available from [PyPI](https://pypi.org). If you have pip, just run:
         '''
         pip install pandas
         pip install holidays
         pip install impyla
         pip install unidecode
         '''
         #### Installation
```

### Comparing `dadosSPF-1.0.3/dadosSPF.egg-info/PKG-INFO` & `dadosSPF-1.0.5/dadosSPF.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.3
+Version: 1.0.5
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
         
         ## Getting Started
         #### Dependencies
         Você precisa do Python 3.7 ou posterior para usar dadosSPF.
         Você pode encontrá-lo em [python.org] (https://www.python.org/).
-        Você precisa do PySpark 2.4.7 para usar safraPyFunctions.
+        Você precisa do PySpark 2.4.7 para usar dadosSPF.
         Você pode encontrá-lo em [spark.apache.org] (https://spark.apache.org/docs/latest/api/python/).
         
         You also need pandas, holidays and impyla packages, which is available from [PyPI](https://pypi.org). If you have pip, just run:
         '''
         pip install pandas
         pip install holidays
         pip install impyla
```

### Comparing `dadosSPF-1.0.3/dadosSPF.egg-info/SOURCES.txt` & `dadosSPF-1.0.5/dadosSPF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dadosSPF-1.0.3/setup.py` & `dadosSPF-1.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(
     name='dadosSPF',
-    version='1.0.3',
+    version='1.0.5',
     url='https://gitlab.com.br/dadosSPF',
     license='MIT License',
     author='Carlos Piveta',
-	long_description=readme,
+    long_description=readme,
     long_description_content_type="text/markdown",
     author_email='cepo496@gmail.com',
     keywords='Pacote',
     description='Pacote de funções uteis para o desenvolvimento na cloudera',
     packages=['dadosSPF'],
     install_requires=['pandas','impyla','holidays','unidecode']
 )
```


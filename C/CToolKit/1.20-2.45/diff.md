# Comparing `tmp/CToolKit-1.20.tar.gz` & `tmp/CToolKit-2.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CToolKit-1.20.tar", last modified: Tue Jul  4 19:08:52 2023, max compression
+gzip compressed data, was "dist/CToolKit-2.45.tar", last modified: Wed Jul 12 08:33:49 2023, max compression
```

## Comparing `CToolKit-1.20.tar` & `CToolKit-2.45.tar`

### file list

```diff
@@ -1,29 +1,39 @@
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-07-04 19:08:52.580567 CToolKit-1.20/
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-07-04 19:08:52.576567 CToolKit-1.20/CToolKit/
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      504 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/ComandLineExecution.py
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-07-04 19:08:52.580567 CToolKit-1.20/CToolKit/Errors/
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      306 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/Errors/ComandLineError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      226 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/Errors/ComandLineWarning.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      110 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/Errors/CopilationError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      118 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/Errors/CopilationWarning.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      108 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/Errors/ExecutionError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      205 2023-07-03 20:51:23.000000 CToolKit-1.20/CToolKit/Errors/NotExpectedResult.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      265 2023-07-03 09:56:48.000000 CToolKit-1.20/CToolKit/Errors/ValgrindError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      264 2023-07-03 09:57:03.000000 CToolKit-1.20/CToolKit/Errors/ValgrindLeak.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        0 2023-07-03 09:01:17.000000 CToolKit-1.20/CToolKit/Errors/__init__.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      874 2023-07-03 18:38:00.000000 CToolKit-1.20/CToolKit/__init__.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1470 2023-07-03 18:39:36.000000 CToolKit-1.20/CToolKit/amalgamation.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     7282 2023-07-04 18:42:05.000000 CToolKit-1.20/CToolKit/comand_line_functions.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      445 2023-07-03 20:58:17.000000 CToolKit-1.20/CToolKit/output_formatation.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3168 2023-07-04 18:47:02.000000 CToolKit-1.20/CToolKit/readme_converter.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1427 2023-07-03 20:37:39.000000 CToolKit-1.20/CToolKit/valgrind_parser.py
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-07-04 19:08:52.576567 CToolKit-1.20/CToolKit.egg-info/
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3330 2023-07-04 19:08:52.000000 CToolKit-1.20/CToolKit.egg-info/PKG-INFO
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      662 2023-07-04 19:08:52.000000 CToolKit-1.20/CToolKit.egg-info/SOURCES.txt
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        1 2023-07-04 19:08:52.000000 CToolKit-1.20/CToolKit.egg-info/dependency_links.txt
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        9 2023-07-04 19:08:52.000000 CToolKit-1.20/CToolKit.egg-info/top_level.txt
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1060 2023-06-17 02:11:11.000000 CToolKit-1.20/LICENSE
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3330 2023-07-04 19:08:52.580567 CToolKit-1.20/PKG-INFO
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     2921 2023-07-03 14:26:26.000000 CToolKit-1.20/README.md
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)       38 2023-07-04 19:08:52.580567 CToolKit-1.20/setup.cfg
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      664 2023-07-04 19:07:51.000000 CToolKit-1.20/setup.py
+drwxrwxr-x   0 mateusmoutinho  (1000) mateusmoutinho  (1000)        0 2023-07-12 08:33:49.000000 CToolKit-2.45/
+drwxrwxr-x   0 mateusmoutinho  (1000) mateusmoutinho  (1000)        0 2023-07-12 08:33:49.000000 CToolKit-2.45/CToolKit/
+drwxrwxr-x   0 mateusmoutinho  (1000) mateusmoutinho  (1000)        0 2023-07-12 08:33:49.000000 CToolKit-2.45/CToolKit/Errors/
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      306 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/Errors/ComandLineError.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      226 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/Errors/ComandLineWarning.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)       95 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/Errors/CopilationError.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      103 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/Errors/CopilationWarning.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)       93 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/Errors/ExecutionError.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      319 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/Errors/NotExpectedResult.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      174 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/Errors/SideEffectFolderDiferent.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      250 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/Errors/ValgrindError.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      249 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/Errors/ValgrindLeak.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)        0 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/Errors/__init__.py
+drwxrwxr-x   0 mateusmoutinho  (1000) mateusmoutinho  (1000)        0 2023-07-12 08:33:49.000000 CToolKit-2.45/CToolKit/FolderTestPreset/
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      729 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/FolderTestPreset/Constructor.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)     2785 2023-07-12 07:58:40.000000 CToolKit-2.45/CToolKit/FolderTestPreset/Creation.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)     3967 2023-07-12 07:58:14.000000 CToolKit-2.45/CToolKit/FolderTestPreset/Execution.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)     1374 2023-07-12 07:57:57.000000 CToolKit-2.45/CToolKit/FolderTestPreset/Extras.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      112 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/FolderTestPreset/FolderTestPreset.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      873 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/FolderTestPreset/Print.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)        0 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/FolderTestPreset/__init__.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      672 2023-07-12 06:08:31.000000 CToolKit-2.45/CToolKit/FolderTestPreset/folder_hash.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      443 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/FolderTestPreset/output_formatation.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      496 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/ComandLineExecution.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      766 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/__init__.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)     1467 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/amalgamation.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)     4487 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/comand_line_functions.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)     3168 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/readme_converter.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)     1427 2023-07-11 09:55:11.000000 CToolKit-2.45/CToolKit/valgrind_parser.py
+drwxrwxr-x   0 mateusmoutinho  (1000) mateusmoutinho  (1000)        0 2023-07-12 08:33:49.000000 CToolKit-2.45/CToolKit.egg-info/
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)     3458 2023-07-12 08:33:48.000000 CToolKit-2.45/CToolKit.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)     1037 2023-07-12 08:33:48.000000 CToolKit-2.45/CToolKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)        1 2023-07-12 08:33:48.000000 CToolKit-2.45/CToolKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)        9 2023-07-12 08:33:48.000000 CToolKit-2.45/CToolKit.egg-info/top_level.txt
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)     1060 2023-07-11 09:55:11.000000 CToolKit-2.45/LICENSE
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)     3012 2023-07-12 08:30:12.000000 CToolKit-2.45/README.md
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)      703 2023-07-12 08:22:07.000000 CToolKit-2.45/setup.py
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)     3458 2023-07-12 08:33:49.000000 CToolKit-2.45/PKG-INFO
+-rw-rw-r--   0 mateusmoutinho  (1000) mateusmoutinho  (1000)       38 2023-07-12 08:33:49.000000 CToolKit-2.45/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `CToolKit-1.20/CToolKit/__init__.py` & `CToolKit-2.45/CToolKit/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
-from CToolKit.amalgamation import  generate_amalgamated_code
-from CToolKit.ComandLineExecution import ComandLineExecution
-from CToolKit.comand_line_functions import compile_project_by_command
-from CToolKit.comand_line_functions import compile_project
-from CToolKit.comand_line_functions import test_binary_with_valgrind
-from CToolKit.comand_line_functions import execute_test_for_file
-from CToolKit.comand_line_functions import execute_test_for_folder
+from .amalgamation import  generate_amalgamated_code
+from .ComandLineExecution import ComandLineExecution
+from .comand_line_functions import compile_project_by_command
+from .comand_line_functions import compile_project
+from .comand_line_functions import test_binary_with_valgrind
+from .comand_line_functions import execute_test_for_file
+from .FolderTestPreset.FolderTestPreset import FolderTestPreset
 
+from .Errors.CopilationError import CopilationError
+from .Errors.CopilationWarning import CopilationWarning
+from .Errors.ExecutionError import ExecutionError
+from .Errors.ValgrindError import ValgrindError
+from .Errors.ValgrindLeak import ValgrindLeak
+from .Errors.NotExpectedResult import NotExpectedResult
 
-from CToolKit.Errors.CopilationError import CopilationError
-from CToolKit.Errors.CopilationWarning import CopilationWarning
-from CToolKit.Errors.ExecutionError import ExecutionError
-from CToolKit.Errors.ValgrindError import ValgrindError
-from CToolKit.Errors.ValgrindLeak import ValgrindLeak
-from CToolKit.Errors.NotExpectedResult import NotExpectedResult
-
-from CToolKit.readme_converter import include_code_in_markdown
+from .readme_converter import include_code_in_markdown
```

### Comparing `CToolKit-1.20/CToolKit/amalgamation.py` & `CToolKit-2.45/CToolKit/amalgamation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from os.path import join
 
-
-
 def get_action(referencer_dir: str, line: str) -> str or None:
     line = line.strip()
     if not line.startswith('#include'):
         return None
 
     if '"' in line:
         relative_file = line.split('"')[1]
         return join(referencer_dir, relative_file)
 
 
 
-
 def generate_amalgamated_code(starter: str,output:str=None) -> str:
     """generate an full amalgamated code of the code you pass
     Args:
         starter (str): the started path of your code ex:'test.h'
         output (str): the output you want to save, if its None it will not save nothing
     Raises:
         FileNotFoundError: if some file were not found
```

### Comparing `CToolKit-1.20/CToolKit/readme_converter.py` & `CToolKit-2.45/CToolKit/readme_converter.py`

 * *Files identical despite different names*

### Comparing `CToolKit-1.20/CToolKit/valgrind_parser.py` & `CToolKit-2.45/CToolKit/valgrind_parser.py`

 * *Files identical despite different names*

### Comparing `CToolKit-1.20/CToolKit.egg-info/PKG-INFO` & `CToolKit-2.45/CToolKit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: CToolKit
-Version: 1.20
+Version: 2.45
 Summary: CToolKit to manipulate CPipeLines and Repos
 Home-page: https://oui.tec.br/
 Author: Mateus Moutinho
 Author-email: mateusmoutinho01@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CToolkit
@@ -74,16 +76,16 @@
 
 import CToolKit as ct
 
 COMPILER = 'gcc'
 FILE = 'test.c'
 OUTPUT = 'test.out'
 ct.compile_project(
- COMPILER,
  FILE,
+ COMPILER,
  OUTPUT,
  raise_errors=True,
  raise_warnings=True
 )
 ~~~
 
 #### Testing copilation with valgrind 
@@ -110,27 +112,30 @@
 Executing copilation and test with file with a single comand 
 ~~~python
 import CToolKit as ct
 
 COMPILER = 'gcc'
 FILE = 'test.c'
 
-ct.execute_test_for_file(COMPILER,FILE)
+ct.execute_test_for_file(FILE,COMPILER)
 
 ~~~
 
 Executing Test with all .c or .cpp files in the given folder 
 
 ~~~python 
-
 import CToolKit as ct
 
-COMPILER = 'gcc'
-FOLDER ='test'
-ct.execute_test_for_folder(COMPILER,FOLDER,print_values=True)
+
+test = ct.FolderTestPreset(folder='tests/main_test',side_effect_folder='tests/target')
+# wil create non existent outputs
+test.generate_ouptut()
+# will start the test
+test.start_test()
+
 
 ~~~
 
 #### Execution 
 you can execute an binary with the ComandLine Execution class
 
 ~~~python
@@ -138,16 +143,16 @@
 import CToolKit as ct
 
 COMPILER = 'gcc'
 
 FILE = 'test.c'
 OUTPUT = 'test.out'
 ct.compile_project(
- COMPILER,
  FILE,
+ COMPILER,
  OUTPUT,
  raise_errors=True,
  raise_warnings=True
 )
 
 execution = ct.ComandLineExecution(f'./{OUTPUT}')
 
@@ -172,7 +177,9 @@
 ~~~
 
 
 
 
 
 
+
+
```

### Comparing `CToolKit-1.20/LICENSE` & `CToolKit-2.45/LICENSE`

 * *Files identical despite different names*

### Comparing `CToolKit-1.20/PKG-INFO` & `CToolKit-2.45/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: CToolKit
-Version: 1.20
+Version: 2.45
 Summary: CToolKit to manipulate CPipeLines and Repos
 Home-page: https://oui.tec.br/
 Author: Mateus Moutinho
 Author-email: mateusmoutinho01@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CToolkit
@@ -74,16 +76,16 @@
 
 import CToolKit as ct
 
 COMPILER = 'gcc'
 FILE = 'test.c'
 OUTPUT = 'test.out'
 ct.compile_project(
- COMPILER,
  FILE,
+ COMPILER,
  OUTPUT,
  raise_errors=True,
  raise_warnings=True
 )
 ~~~
 
 #### Testing copilation with valgrind 
@@ -110,27 +112,30 @@
 Executing copilation and test with file with a single comand 
 ~~~python
 import CToolKit as ct
 
 COMPILER = 'gcc'
 FILE = 'test.c'
 
-ct.execute_test_for_file(COMPILER,FILE)
+ct.execute_test_for_file(FILE,COMPILER)
 
 ~~~
 
 Executing Test with all .c or .cpp files in the given folder 
 
 ~~~python 
-
 import CToolKit as ct
 
-COMPILER = 'gcc'
-FOLDER ='test'
-ct.execute_test_for_folder(COMPILER,FOLDER,print_values=True)
+
+test = ct.FolderTestPreset(folder='tests/main_test',side_effect_folder='tests/target')
+# wil create non existent outputs
+test.generate_ouptut()
+# will start the test
+test.start_test()
+
 
 ~~~
 
 #### Execution 
 you can execute an binary with the ComandLine Execution class
 
 ~~~python
@@ -138,16 +143,16 @@
 import CToolKit as ct
 
 COMPILER = 'gcc'
 
 FILE = 'test.c'
 OUTPUT = 'test.out'
 ct.compile_project(
- COMPILER,
  FILE,
+ COMPILER,
  OUTPUT,
  raise_errors=True,
  raise_warnings=True
 )
 
 execution = ct.ComandLineExecution(f'./{OUTPUT}')
 
@@ -172,7 +177,9 @@
 ~~~
 
 
 
 
 
 
+
+
```

### Comparing `CToolKit-1.20/README.md` & `CToolKit-2.45/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 
 import CToolKit as ct
 
 COMPILER = 'gcc'
 FILE = 'test.c'
 OUTPUT = 'test.out'
 ct.compile_project(
- COMPILER,
  FILE,
+ COMPILER,
  OUTPUT,
  raise_errors=True,
  raise_warnings=True
 )
 ~~~
 
 #### Testing copilation with valgrind 
@@ -97,27 +97,30 @@
 Executing copilation and test with file with a single comand 
 ~~~python
 import CToolKit as ct
 
 COMPILER = 'gcc'
 FILE = 'test.c'
 
-ct.execute_test_for_file(COMPILER,FILE)
+ct.execute_test_for_file(FILE,COMPILER)
 
 ~~~
 
 Executing Test with all .c or .cpp files in the given folder 
 
 ~~~python 
-
 import CToolKit as ct
 
-COMPILER = 'gcc'
-FOLDER ='test'
-ct.execute_test_for_folder(COMPILER,FOLDER,print_values=True)
+
+test = ct.FolderTestPreset(folder='tests/main_test',side_effect_folder='tests/target')
+# wil create non existent outputs
+test.generate_ouptut()
+# will start the test
+test.start_test()
+
 
 ~~~
 
 #### Execution 
 you can execute an binary with the ComandLine Execution class
 
 ~~~python
@@ -125,16 +128,16 @@
 import CToolKit as ct
 
 COMPILER = 'gcc'
 
 FILE = 'test.c'
 OUTPUT = 'test.out'
 ct.compile_project(
- COMPILER,
  FILE,
+ COMPILER,
  OUTPUT,
  raise_errors=True,
  raise_warnings=True
 )
 
 execution = ct.ComandLineExecution(f'./{OUTPUT}')
```

### Comparing `CToolKit-1.20/setup.py` & `CToolKit-2.45/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='CToolKit',
-    version='1.20',
+    version='2.45',
     description='CToolKit to manipulate CPipeLines and Repos',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Mateus Moutinho',
     author_email='mateusmoutinho01@gmail.com',
     url='https://oui.tec.br/',
     packages=find_packages(),
     install_requires=[],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
-)
+)
+#python -m build
+#twine upload dist/*
```


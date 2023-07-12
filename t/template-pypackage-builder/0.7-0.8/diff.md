# Comparing `tmp/template_pypackage_builder-0.7.tar.gz` & `tmp/template_pypackage_builder-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "template_pypackage_builder-0.7.tar", last modified: Wed Jul 12 16:00:44 2023, max compression
+gzip compressed data, was "template_pypackage_builder-0.8.tar", last modified: Wed Jul 12 17:16:39 2023, max compression
```

## Comparing `template_pypackage_builder-0.7.tar` & `template_pypackage_builder-0.8.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 16:00:44.056161 template_pypackage_builder-0.7/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       51 2023-07-10 15:52:08.000000 template_pypackage_builder-0.7/MANIFEST.in
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     4272 2023-07-12 16:00:44.056161 template_pypackage_builder-0.7/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     3852 2023-07-12 16:00:26.000000 template_pypackage_builder-0.7/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-12 16:00:44.056161 template_pypackage_builder-0.7/setup.cfg
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      868 2023-07-12 15:56:48.000000 template_pypackage_builder-0.7/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 16:00:44.052161 template_pypackage_builder-0.7/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 16:00:44.056161 template_pypackage_builder-0.7/src/template_pypackage_builder/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    13080 2023-07-10 14:10:03.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 16:00:44.056161 template_pypackage_builder-0.7/src/template_pypackage_builder/types/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    11357 2023-07-09 20:17:56.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/types/Apache Version 2.0.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    35150 2023-07-09 20:14:37.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/types/GNU GPLv3.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1070 2023-07-09 20:15:41.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/types/MIT License.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    16725 2023-07-09 20:21:23.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/types/Mozilla Public License 2.0.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1211 2023-07-09 20:22:37.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/types/The Unlicense.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        0 2023-07-09 21:14:00.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/types/user_defined.txt
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 16:00:44.056161 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     4272 2023-07-12 16:00:43.000000 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      740 2023-07-12 16:00:44.000000 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-12 16:00:43.000000 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      105 2023-07-12 16:00:43.000000 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/entry_points.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       10 2023-07-12 16:00:43.000000 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/requires.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       27 2023-07-12 16:00:43.000000 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:16:39.988858 template_pypackage_builder-0.8/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       51 2023-07-12 16:15:56.000000 template_pypackage_builder-0.8/MANIFEST.in
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4319 2023-07-12 17:16:39.988858 template_pypackage_builder-0.8/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     3900 2023-07-12 16:15:56.000000 template_pypackage_builder-0.8/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-12 17:16:39.988858 template_pypackage_builder-0.8/setup.cfg
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      868 2023-07-12 17:16:04.000000 template_pypackage_builder-0.8/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:16:39.984858 template_pypackage_builder-0.8/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:16:39.984858 template_pypackage_builder-0.8/src/template_pypackage_builder/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    14277 2023-07-12 17:12:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/__init__.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:16:39.988858 template_pypackage_builder-0.8/src/template_pypackage_builder/__pycache__/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    12938 2023-07-12 17:14:02.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/__pycache__/test.cpython-310.pyc
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:16:39.988858 template_pypackage_builder-0.8/src/template_pypackage_builder/types/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    11357 2023-07-09 20:17:56.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/types/Apache Version 2.0.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    35150 2023-07-09 20:14:37.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/types/GNU GPLv3.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1070 2023-07-09 20:15:41.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/types/MIT License.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    16725 2023-07-09 20:21:23.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/types/Mozilla Public License 2.0.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1211 2023-07-09 20:22:37.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/types/The Unlicense.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        0 2023-07-09 21:14:00.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/types/user_defined.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:16:39.988858 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4319 2023-07-12 17:16:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      804 2023-07-12 17:16:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-12 17:16:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      105 2023-07-12 17:16:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       10 2023-07-12 17:16:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       27 2023-07-12 17:16:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/top_level.txt
```

### Comparing `template_pypackage_builder-0.7/PKG-INFO` & `template_pypackage_builder-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template_pypackage_builder
-Version: 0.7
+Version: 0.8
 Summary: A simple tool for packaging python
 Home-page: https://github.com/dipson94/packagemaker
 Author: Dipson
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -48,50 +48,49 @@
 
 * pkg_resources
 * pyperclip
 * os
 
 ## Usage
 
-Direct function from packages. USe main function to start initial package build.
+Direct function from packages. Use main function to start initial package build.
 
 ```
 import template_pypackage_builder as pb
 pb.main()
 ```
 Use pip_code() function to generate pip code to install package from subdirectory of github repo
 ```
 import template_pypackage_builder as pb
 pb.pip_code()
 ```
 Alternatively use key words pysetup and gitpip directly in terminal to execute the main and pip_code functions respectively
 
+@terminal
 ```
 pysetup
-
 ```
 
-
+@terminal
 ```
 gitpip
-
 ```
 
 ### Additional notes on package Building
 Additional info about package building
 
 **including path**
 
 To include path in package file use the following command
 ```
 import pkg_resources
 relative_path=pkg_resources.resource_filename("packagemaker", "types")
 ```
 This command is used if you want to use the path inside package in site-packages folder. Otherwise the path will be relative to the directory where you imported the package (while programming after importing the module).
-Here relative_path refers to the path to types folder inside installed package packagemaker.
+Here relative_path refers to the path to types folder inside installed package template_pypackage_builder.
 
 **`__init__.py` file handeling**
 
 The following is the tree structure of a package showing basic files and directories. From main package directory in source, each modules ( also directories) contain an `__init__.py` file.
 ```
 └── package_name
     ├── License.txt
@@ -132,15 +131,15 @@
 from .module_2 import (function_1,function_2,function_3)
 from .module_3 import (function_1,function_2,function_3)
 ```
 Here we are importing functions directly to main `__init__.py` file, so the functions are readly availble when the main module is called (or imported).
 
 **Final thoughts**
 
-packagemaker only helps with making a template or initial structure of a package. For making better package work on the file manually using the editor.
+template_pypackage_builder only helps with making a template or initial structure of a package. For making better package, work on the files manually using the editor.
 
 ## Author
 
 Dipson
 
 ## License
```

### Comparing `template_pypackage_builder-0.7/README.md` & `template_pypackage_builder-0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,50 +36,49 @@
 
 * pkg_resources
 * pyperclip
 * os
 
 ## Usage
 
-Direct function from packages. USe main function to start initial package build.
+Direct function from packages. Use main function to start initial package build.
 
 ```
 import template_pypackage_builder as pb
 pb.main()
 ```
 Use pip_code() function to generate pip code to install package from subdirectory of github repo
 ```
 import template_pypackage_builder as pb
 pb.pip_code()
 ```
 Alternatively use key words pysetup and gitpip directly in terminal to execute the main and pip_code functions respectively
 
+@terminal
 ```
 pysetup
-
 ```
 
-
+@terminal
 ```
 gitpip
-
 ```
 
 ### Additional notes on package Building
 Additional info about package building
 
 **including path**
 
 To include path in package file use the following command
 ```
 import pkg_resources
 relative_path=pkg_resources.resource_filename("packagemaker", "types")
 ```
 This command is used if you want to use the path inside package in site-packages folder. Otherwise the path will be relative to the directory where you imported the package (while programming after importing the module).
-Here relative_path refers to the path to types folder inside installed package packagemaker.
+Here relative_path refers to the path to types folder inside installed package template_pypackage_builder.
 
 **`__init__.py` file handeling**
 
 The following is the tree structure of a package showing basic files and directories. From main package directory in source, each modules ( also directories) contain an `__init__.py` file.
 ```
 └── package_name
     ├── License.txt
@@ -120,16 +119,16 @@
 from .module_2 import (function_1,function_2,function_3)
 from .module_3 import (function_1,function_2,function_3)
 ```
 Here we are importing functions directly to main `__init__.py` file, so the functions are readly availble when the main module is called (or imported).
 
 **Final thoughts**
 
-packagemaker only helps with making a template or initial structure of a package. For making better package work on the file manually using the editor.
+template_pypackage_builder only helps with making a template or initial structure of a package. For making better package, work on the files manually using the editor.
 
 ## Author
 
 Dipson
 
 ## License
 
-GNU GPL V3
+GNU GPL V3
```

### Comparing `template_pypackage_builder-0.7/setup.py` & `template_pypackage_builder-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 with open("README.md", "r") as f:
     long_description = f.read()
 setup(
     name="template_pypackage_builder",
-    version="0.7",
+    version="0.8",
     description="A simple tool for packaging python",
     package_dir={"": "src"},
     include_package_data=True,
     url="https://github.com/dipson94/packagemaker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Dipson",
```

### Comparing `template_pypackage_builder-0.7/src/template_pypackage_builder/__init__.py` & `template_pypackage_builder-0.8/src/template_pypackage_builder/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -228,14 +228,47 @@
     | >=3.10                               |
     ----------------------------------------
     | only add version if necessary        |
     ----------------------------------------
     
     """)
     pythonrequires=str(input("enter version :"))
+    consol=[]
+    if str(input("""
+    
+    Do you want to run certain functions of the 
+    module directly in console (in terminal) 
+    with user defined keywords (would use this
+    keywords directly in terminal to call function)
+    (y/n)?     
+    
+    """))=="y":
+    	print("""
+    -----------------------------------------------.
+    | Example                                      |
+    ------------------------------------------------
+    | userdef_keywrd = module_name : function_name |
+    ------------------------------------------------
+    | (enter each line one by one)                 |
+    ------------------------------------------------
+    
+    if function is inside submodule then
+    
+    userdef_keywrd = module_name : sub_module_name :function_name
+    
+    Always give unique keyword and make sure it doesnot
+    conflicts with other commands
+    
+    
+    	""")
+    while True:
+            x=str(input("enter console data : "))
+            if x=="":
+                break
+            consol.append(x)
     
     s='''from setuptools import setup
     
     with open("'''
     s=s+readme+'''", "r") as f:
         long_description = f.read()
     
@@ -282,14 +315,21 @@
                 "dev": '''
         exr='['
         for i in extrarequire:
             exr=exr+'"'+i+'",'
         exr=exr[:-1]+']'
         s=s+exr+'''
                 },'''
+    if len(consol)!=0:
+        s=s+"""
+        entry_points={
+        'console_scripts': ["""
+        for i in consol:
+            s=s+"'"+i+"',"
+        s=s+"""],},"""
     if pythonrequires!="":
         s=s+'''
         python_requires="'''+pythonrequires+'''",'''
     s=s+'''    
     )'''
     max=0
     for i in  s.split("\n"):
```

### Comparing `template_pypackage_builder-0.7/src/template_pypackage_builder/types/Apache Version 2.0.txt` & `template_pypackage_builder-0.8/src/template_pypackage_builder/types/Apache Version 2.0.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.7/src/template_pypackage_builder/types/GNU GPLv3.txt` & `template_pypackage_builder-0.8/src/template_pypackage_builder/types/GNU GPLv3.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.7/src/template_pypackage_builder/types/MIT License.txt` & `template_pypackage_builder-0.8/src/template_pypackage_builder/types/MIT License.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.7/src/template_pypackage_builder/types/Mozilla Public License 2.0.txt` & `template_pypackage_builder-0.8/src/template_pypackage_builder/types/Mozilla Public License 2.0.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.7/src/template_pypackage_builder/types/The Unlicense.txt` & `template_pypackage_builder-0.8/src/template_pypackage_builder/types/The Unlicense.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/PKG-INFO` & `template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pypackage-builder
-Version: 0.7
+Version: 0.8
 Summary: A simple tool for packaging python
 Home-page: https://github.com/dipson94/packagemaker
 Author: Dipson
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -48,50 +48,49 @@
 
 * pkg_resources
 * pyperclip
 * os
 
 ## Usage
 
-Direct function from packages. USe main function to start initial package build.
+Direct function from packages. Use main function to start initial package build.
 
 ```
 import template_pypackage_builder as pb
 pb.main()
 ```
 Use pip_code() function to generate pip code to install package from subdirectory of github repo
 ```
 import template_pypackage_builder as pb
 pb.pip_code()
 ```
 Alternatively use key words pysetup and gitpip directly in terminal to execute the main and pip_code functions respectively
 
+@terminal
 ```
 pysetup
-
 ```
 
-
+@terminal
 ```
 gitpip
-
 ```
 
 ### Additional notes on package Building
 Additional info about package building
 
 **including path**
 
 To include path in package file use the following command
 ```
 import pkg_resources
 relative_path=pkg_resources.resource_filename("packagemaker", "types")
 ```
 This command is used if you want to use the path inside package in site-packages folder. Otherwise the path will be relative to the directory where you imported the package (while programming after importing the module).
-Here relative_path refers to the path to types folder inside installed package packagemaker.
+Here relative_path refers to the path to types folder inside installed package template_pypackage_builder.
 
 **`__init__.py` file handeling**
 
 The following is the tree structure of a package showing basic files and directories. From main package directory in source, each modules ( also directories) contain an `__init__.py` file.
 ```
 └── package_name
     ├── License.txt
@@ -132,15 +131,15 @@
 from .module_2 import (function_1,function_2,function_3)
 from .module_3 import (function_1,function_2,function_3)
 ```
 Here we are importing functions directly to main `__init__.py` file, so the functions are readly availble when the main module is called (or imported).
 
 **Final thoughts**
 
-packagemaker only helps with making a template or initial structure of a package. For making better package work on the file manually using the editor.
+template_pypackage_builder only helps with making a template or initial structure of a package. For making better package, work on the files manually using the editor.
 
 ## Author
 
 Dipson
 
 ## License
```

### Comparing `template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/SOURCES.txt` & `template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,13 +4,14 @@
 src/template_pypackage_builder/__init__.py
 src/template_pypackage_builder.egg-info/PKG-INFO
 src/template_pypackage_builder.egg-info/SOURCES.txt
 src/template_pypackage_builder.egg-info/dependency_links.txt
 src/template_pypackage_builder.egg-info/entry_points.txt
 src/template_pypackage_builder.egg-info/requires.txt
 src/template_pypackage_builder.egg-info/top_level.txt
+src/template_pypackage_builder/__pycache__/test.cpython-310.pyc
 src/template_pypackage_builder/types/Apache Version 2.0.txt
 src/template_pypackage_builder/types/GNU GPLv3.txt
 src/template_pypackage_builder/types/MIT License.txt
 src/template_pypackage_builder/types/Mozilla Public License 2.0.txt
 src/template_pypackage_builder/types/The Unlicense.txt
 src/template_pypackage_builder/types/user_defined.txt
```


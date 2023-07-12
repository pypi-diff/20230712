# Comparing `tmp/template_pypackage_builder-0.6.tar.gz` & `tmp/template_pypackage_builder-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "template_pypackage_builder-0.6.tar", last modified: Mon Jul 10 15:59:03 2023, max compression
+gzip compressed data, was "template_pypackage_builder-0.7.tar", last modified: Wed Jul 12 16:00:44 2023, max compression
```

## Comparing `template_pypackage_builder-0.6.tar` & `template_pypackage_builder-0.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:59:03.151734 template_pypackage_builder-0.6/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       51 2023-07-10 15:52:08.000000 template_pypackage_builder-0.6/MANIFEST.in
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     4041 2023-07-10 15:59:03.151734 template_pypackage_builder-0.6/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     3621 2023-07-10 15:58:29.000000 template_pypackage_builder-0.6/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-10 15:59:03.151734 template_pypackage_builder-0.6/setup.cfg
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      702 2023-07-10 15:58:52.000000 template_pypackage_builder-0.6/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:59:03.147734 template_pypackage_builder-0.6/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:59:03.147734 template_pypackage_builder-0.6/src/template_pypackage_builder/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    13080 2023-07-10 14:10:03.000000 template_pypackage_builder-0.6/src/template_pypackage_builder/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:59:03.151734 template_pypackage_builder-0.6/src/template_pypackage_builder/types/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    11357 2023-07-09 20:17:56.000000 template_pypackage_builder-0.6/src/template_pypackage_builder/types/Apache Version 2.0.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    35150 2023-07-09 20:14:37.000000 template_pypackage_builder-0.6/src/template_pypackage_builder/types/GNU GPLv3.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1070 2023-07-09 20:15:41.000000 template_pypackage_builder-0.6/src/template_pypackage_builder/types/MIT License.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    16725 2023-07-09 20:21:23.000000 template_pypackage_builder-0.6/src/template_pypackage_builder/types/Mozilla Public License 2.0.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1211 2023-07-09 20:22:37.000000 template_pypackage_builder-0.6/src/template_pypackage_builder/types/The Unlicense.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        0 2023-07-09 21:14:00.000000 template_pypackage_builder-0.6/src/template_pypackage_builder/types/user_defined.txt
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-10 15:59:03.147734 template_pypackage_builder-0.6/src/template_pypackage_builder.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     4041 2023-07-10 15:59:03.000000 template_pypackage_builder-0.6/src/template_pypackage_builder.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      683 2023-07-10 15:59:03.000000 template_pypackage_builder-0.6/src/template_pypackage_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-10 15:59:03.000000 template_pypackage_builder-0.6/src/template_pypackage_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       10 2023-07-10 15:59:03.000000 template_pypackage_builder-0.6/src/template_pypackage_builder.egg-info/requires.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       27 2023-07-10 15:59:03.000000 template_pypackage_builder-0.6/src/template_pypackage_builder.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 16:00:44.056161 template_pypackage_builder-0.7/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       51 2023-07-10 15:52:08.000000 template_pypackage_builder-0.7/MANIFEST.in
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4272 2023-07-12 16:00:44.056161 template_pypackage_builder-0.7/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     3852 2023-07-12 16:00:26.000000 template_pypackage_builder-0.7/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-12 16:00:44.056161 template_pypackage_builder-0.7/setup.cfg
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      868 2023-07-12 15:56:48.000000 template_pypackage_builder-0.7/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 16:00:44.052161 template_pypackage_builder-0.7/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 16:00:44.056161 template_pypackage_builder-0.7/src/template_pypackage_builder/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    13080 2023-07-10 14:10:03.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/__init__.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 16:00:44.056161 template_pypackage_builder-0.7/src/template_pypackage_builder/types/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    11357 2023-07-09 20:17:56.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/types/Apache Version 2.0.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    35150 2023-07-09 20:14:37.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/types/GNU GPLv3.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1070 2023-07-09 20:15:41.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/types/MIT License.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    16725 2023-07-09 20:21:23.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/types/Mozilla Public License 2.0.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1211 2023-07-09 20:22:37.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/types/The Unlicense.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        0 2023-07-09 21:14:00.000000 template_pypackage_builder-0.7/src/template_pypackage_builder/types/user_defined.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 16:00:44.056161 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4272 2023-07-12 16:00:43.000000 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      740 2023-07-12 16:00:44.000000 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-12 16:00:43.000000 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      105 2023-07-12 16:00:43.000000 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       10 2023-07-12 16:00:43.000000 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       27 2023-07-12 16:00:43.000000 template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/top_level.txt
```

### Comparing `template_pypackage_builder-0.6/PKG-INFO` & `template_pypackage_builder-0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template_pypackage_builder
-Version: 0.6
+Version: 0.7
 Summary: A simple tool for packaging python
 Home-page: https://github.com/dipson94/packagemaker
 Author: Dipson
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -27,19 +27,27 @@
 * LIcense creater
 * setup file creater
 * directory tree builder
 * pip code generater to install package from subdirectory of github repo
 * main function to initial package building from scratch 
 
 ## Installation
+
+Install from pypi
+
+```
+pip install template-pypackage-builder 
+```
+
 Install from GitHub
 
 ```
 pip install git+https://github.com/dipson94/packagemaker
 ```
+
 #### Install requires
 
 * pkg_resources
 * pyperclip
 * os
 
 ## Usage
@@ -51,14 +59,27 @@
 pb.main()
 ```
 Use pip_code() function to generate pip code to install package from subdirectory of github repo
 ```
 import template_pypackage_builder as pb
 pb.pip_code()
 ```
+Alternatively use key words pysetup and gitpip directly in terminal to execute the main and pip_code functions respectively
+
+```
+pysetup
+
+```
+
+
+```
+gitpip
+
+```
+
 ### Additional notes on package Building
 Additional info about package building
 
 **including path**
 
 To include path in package file use the following command
 ```
```

### Comparing `template_pypackage_builder-0.6/README.md` & `template_pypackage_builder-0.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,19 +15,27 @@
 * LIcense creater
 * setup file creater
 * directory tree builder
 * pip code generater to install package from subdirectory of github repo
 * main function to initial package building from scratch 
 
 ## Installation
+
+Install from pypi
+
+```
+pip install template-pypackage-builder 
+```
+
 Install from GitHub
 
 ```
 pip install git+https://github.com/dipson94/packagemaker
 ```
+
 #### Install requires
 
 * pkg_resources
 * pyperclip
 * os
 
 ## Usage
@@ -39,14 +47,27 @@
 pb.main()
 ```
 Use pip_code() function to generate pip code to install package from subdirectory of github repo
 ```
 import template_pypackage_builder as pb
 pb.pip_code()
 ```
+Alternatively use key words pysetup and gitpip directly in terminal to execute the main and pip_code functions respectively
+
+```
+pysetup
+
+```
+
+
+```
+gitpip
+
+```
+
 ### Additional notes on package Building
 Additional info about package building
 
 **including path**
 
 To include path in package file use the following command
 ```
```

### Comparing `template_pypackage_builder-0.6/setup.py` & `template_pypackage_builder-0.7/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from setuptools import setup
 with open("README.md", "r") as f:
     long_description = f.read()
 setup(
     name="template_pypackage_builder",
-    version="0.6",
+    version="0.7",
     description="A simple tool for packaging python",
     package_dir={"": "src"},
     include_package_data=True,
     url="https://github.com/dipson94/packagemaker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Dipson",
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
     install_requires=['pyperclip'],
     python_requires=">=3.10",
+    entry_points={
+        'console_scripts': [
+            'pysetup=template_pypackage_builder:main','gitpip=template_pypackage_builder:pip_code',
+        ],
+    },
 )
```

### Comparing `template_pypackage_builder-0.6/src/template_pypackage_builder/__init__.py` & `template_pypackage_builder-0.7/src/template_pypackage_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.6/src/template_pypackage_builder/types/Apache Version 2.0.txt` & `template_pypackage_builder-0.7/src/template_pypackage_builder/types/Apache Version 2.0.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.6/src/template_pypackage_builder/types/GNU GPLv3.txt` & `template_pypackage_builder-0.7/src/template_pypackage_builder/types/GNU GPLv3.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.6/src/template_pypackage_builder/types/MIT License.txt` & `template_pypackage_builder-0.7/src/template_pypackage_builder/types/MIT License.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.6/src/template_pypackage_builder/types/Mozilla Public License 2.0.txt` & `template_pypackage_builder-0.7/src/template_pypackage_builder/types/Mozilla Public License 2.0.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.6/src/template_pypackage_builder/types/The Unlicense.txt` & `template_pypackage_builder-0.7/src/template_pypackage_builder/types/The Unlicense.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.6/src/template_pypackage_builder.egg-info/PKG-INFO` & `template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pypackage-builder
-Version: 0.6
+Version: 0.7
 Summary: A simple tool for packaging python
 Home-page: https://github.com/dipson94/packagemaker
 Author: Dipson
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -27,19 +27,27 @@
 * LIcense creater
 * setup file creater
 * directory tree builder
 * pip code generater to install package from subdirectory of github repo
 * main function to initial package building from scratch 
 
 ## Installation
+
+Install from pypi
+
+```
+pip install template-pypackage-builder 
+```
+
 Install from GitHub
 
 ```
 pip install git+https://github.com/dipson94/packagemaker
 ```
+
 #### Install requires
 
 * pkg_resources
 * pyperclip
 * os
 
 ## Usage
@@ -51,14 +59,27 @@
 pb.main()
 ```
 Use pip_code() function to generate pip code to install package from subdirectory of github repo
 ```
 import template_pypackage_builder as pb
 pb.pip_code()
 ```
+Alternatively use key words pysetup and gitpip directly in terminal to execute the main and pip_code functions respectively
+
+```
+pysetup
+
+```
+
+
+```
+gitpip
+
+```
+
 ### Additional notes on package Building
 Additional info about package building
 
 **including path**
 
 To include path in package file use the following command
 ```
```

### Comparing `template_pypackage_builder-0.6/src/template_pypackage_builder.egg-info/SOURCES.txt` & `template_pypackage_builder-0.7/src/template_pypackage_builder.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 README.md
 setup.py
 src/template_pypackage_builder/__init__.py
 src/template_pypackage_builder.egg-info/PKG-INFO
 src/template_pypackage_builder.egg-info/SOURCES.txt
 src/template_pypackage_builder.egg-info/dependency_links.txt
+src/template_pypackage_builder.egg-info/entry_points.txt
 src/template_pypackage_builder.egg-info/requires.txt
 src/template_pypackage_builder.egg-info/top_level.txt
 src/template_pypackage_builder/types/Apache Version 2.0.txt
 src/template_pypackage_builder/types/GNU GPLv3.txt
 src/template_pypackage_builder/types/MIT License.txt
 src/template_pypackage_builder/types/Mozilla Public License 2.0.txt
 src/template_pypackage_builder/types/The Unlicense.txt
```


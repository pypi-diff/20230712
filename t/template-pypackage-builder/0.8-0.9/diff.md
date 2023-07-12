# Comparing `tmp/template_pypackage_builder-0.8.tar.gz` & `tmp/template_pypackage_builder-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "template_pypackage_builder-0.8.tar", last modified: Wed Jul 12 17:16:39 2023, max compression
+gzip compressed data, was "template_pypackage_builder-0.9.tar", last modified: Wed Jul 12 17:25:58 2023, max compression
```

## Comparing `template_pypackage_builder-0.8.tar` & `template_pypackage_builder-0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:16:39.988858 template_pypackage_builder-0.8/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       51 2023-07-12 16:15:56.000000 template_pypackage_builder-0.8/MANIFEST.in
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     4319 2023-07-12 17:16:39.988858 template_pypackage_builder-0.8/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     3900 2023-07-12 16:15:56.000000 template_pypackage_builder-0.8/README.md
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-12 17:16:39.988858 template_pypackage_builder-0.8/setup.cfg
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      868 2023-07-12 17:16:04.000000 template_pypackage_builder-0.8/setup.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:16:39.984858 template_pypackage_builder-0.8/src/
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:16:39.984858 template_pypackage_builder-0.8/src/template_pypackage_builder/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    14277 2023-07-12 17:12:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/__init__.py
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:16:39.988858 template_pypackage_builder-0.8/src/template_pypackage_builder/__pycache__/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    12938 2023-07-12 17:14:02.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/__pycache__/test.cpython-310.pyc
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:16:39.988858 template_pypackage_builder-0.8/src/template_pypackage_builder/types/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    11357 2023-07-09 20:17:56.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/types/Apache Version 2.0.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    35150 2023-07-09 20:14:37.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/types/GNU GPLv3.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1070 2023-07-09 20:15:41.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/types/MIT License.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)    16725 2023-07-09 20:21:23.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/types/Mozilla Public License 2.0.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     1211 2023-07-09 20:22:37.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/types/The Unlicense.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        0 2023-07-09 21:14:00.000000 template_pypackage_builder-0.8/src/template_pypackage_builder/types/user_defined.txt
-drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:16:39.988858 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/
--rw-rw-r--   0 dipson    (1000) dipson    (1000)     4319 2023-07-12 17:16:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/PKG-INFO
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      804 2023-07-12 17:16:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-12 17:16:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)      105 2023-07-12 17:16:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/entry_points.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       10 2023-07-12 17:16:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/requires.txt
--rw-rw-r--   0 dipson    (1000) dipson    (1000)       27 2023-07-12 17:16:39.000000 template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/top_level.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:25:58.623112 template_pypackage_builder-0.9/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       51 2023-07-12 16:15:56.000000 template_pypackage_builder-0.9/MANIFEST.in
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4319 2023-07-12 17:25:58.623112 template_pypackage_builder-0.9/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     3900 2023-07-12 16:15:56.000000 template_pypackage_builder-0.9/README.md
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       38 2023-07-12 17:25:58.623112 template_pypackage_builder-0.9/setup.cfg
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      868 2023-07-12 17:25:15.000000 template_pypackage_builder-0.9/setup.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:25:58.619112 template_pypackage_builder-0.9/src/
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:25:58.623112 template_pypackage_builder-0.9/src/template_pypackage_builder/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    14292 2023-07-12 17:24:25.000000 template_pypackage_builder-0.9/src/template_pypackage_builder/__init__.py
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:25:58.623112 template_pypackage_builder-0.9/src/template_pypackage_builder/__pycache__/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    12938 2023-07-12 17:14:02.000000 template_pypackage_builder-0.9/src/template_pypackage_builder/__pycache__/test.cpython-310.pyc
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:25:58.623112 template_pypackage_builder-0.9/src/template_pypackage_builder/types/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    11357 2023-07-09 20:17:56.000000 template_pypackage_builder-0.9/src/template_pypackage_builder/types/Apache Version 2.0.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    35150 2023-07-09 20:14:37.000000 template_pypackage_builder-0.9/src/template_pypackage_builder/types/GNU GPLv3.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1070 2023-07-09 20:15:41.000000 template_pypackage_builder-0.9/src/template_pypackage_builder/types/MIT License.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)    16725 2023-07-09 20:21:23.000000 template_pypackage_builder-0.9/src/template_pypackage_builder/types/Mozilla Public License 2.0.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     1211 2023-07-09 20:22:37.000000 template_pypackage_builder-0.9/src/template_pypackage_builder/types/The Unlicense.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        0 2023-07-09 21:14:00.000000 template_pypackage_builder-0.9/src/template_pypackage_builder/types/user_defined.txt
+drwxrwxr-x   0 dipson    (1000) dipson    (1000)        0 2023-07-12 17:25:58.623112 template_pypackage_builder-0.9/src/template_pypackage_builder.egg-info/
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)     4319 2023-07-12 17:25:58.000000 template_pypackage_builder-0.9/src/template_pypackage_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      804 2023-07-12 17:25:58.000000 template_pypackage_builder-0.9/src/template_pypackage_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)        1 2023-07-12 17:25:58.000000 template_pypackage_builder-0.9/src/template_pypackage_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)      105 2023-07-12 17:25:58.000000 template_pypackage_builder-0.9/src/template_pypackage_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       10 2023-07-12 17:25:58.000000 template_pypackage_builder-0.9/src/template_pypackage_builder.egg-info/requires.txt
+-rw-rw-r--   0 dipson    (1000) dipson    (1000)       27 2023-07-12 17:25:58.000000 template_pypackage_builder-0.9/src/template_pypackage_builder.egg-info/top_level.txt
```

### Comparing `template_pypackage_builder-0.8/PKG-INFO` & `template_pypackage_builder-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template_pypackage_builder
-Version: 0.8
+Version: 0.9
 Summary: A simple tool for packaging python
 Home-page: https://github.com/dipson94/packagemaker
 Author: Dipson
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `template_pypackage_builder-0.8/README.md` & `template_pypackage_builder-0.9/README.md`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.8/setup.py` & `template_pypackage_builder-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 with open("README.md", "r") as f:
     long_description = f.read()
 setup(
     name="template_pypackage_builder",
-    version="0.8",
+    version="0.9",
     description="A simple tool for packaging python",
     package_dir={"": "src"},
     include_package_data=True,
     url="https://github.com/dipson94/packagemaker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Dipson",
```

### Comparing `template_pypackage_builder-0.8/src/template_pypackage_builder/__init__.py` & `template_pypackage_builder-0.9/src/template_pypackage_builder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         x=int(input(intro))
         while x<1 or x>6:
         	x=int(input("""
         enter a value from 1-6  
         """))
     file=["GNU GPLv3","MIT License","Apache Version 2.0","Mozilla Public License 2.0","The Unlicense","user_defined"][x-1]
     import pkg_resources
-    relativepath=pkg_resources.resource_filename("packagemaker", "types")
+    relativepath=pkg_resources.resource_filename("template_pypackage_builder", "types")
     path=relativepath+"/"+file+".txt"
     if x==6:
         path=str(input("enter path to custon License file : "))
     with open(path,"r") as template:
         content=template.read()
     name_author=year=name_program=note=0
     data=[name_author,year,name_program,note]
@@ -394,15 +394,15 @@
 |                                                               |
 |---------------------------------------------------------------|
 |This function will walk you through complete packaging process |
 | Including folder creation and file creation                   |
 -----------------------------------------------------------------
 
 """)
-    if str(input("\nDo you wish to continue (y/n) ?"))!="y":
+    if str(input("\nDo you wish to continue (y/n) ? "))!="y":
        return 0
     print("\n")
     ls=license()
     rd=readme()
     st=setup()
     tree(st,rd,ls)
```

### Comparing `template_pypackage_builder-0.8/src/template_pypackage_builder/__pycache__/test.cpython-310.pyc` & `template_pypackage_builder-0.9/src/template_pypackage_builder/__pycache__/test.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.8/src/template_pypackage_builder/types/Apache Version 2.0.txt` & `template_pypackage_builder-0.9/src/template_pypackage_builder/types/Apache Version 2.0.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.8/src/template_pypackage_builder/types/GNU GPLv3.txt` & `template_pypackage_builder-0.9/src/template_pypackage_builder/types/GNU GPLv3.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.8/src/template_pypackage_builder/types/MIT License.txt` & `template_pypackage_builder-0.9/src/template_pypackage_builder/types/MIT License.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.8/src/template_pypackage_builder/types/Mozilla Public License 2.0.txt` & `template_pypackage_builder-0.9/src/template_pypackage_builder/types/Mozilla Public License 2.0.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.8/src/template_pypackage_builder/types/The Unlicense.txt` & `template_pypackage_builder-0.9/src/template_pypackage_builder/types/The Unlicense.txt`

 * *Files identical despite different names*

### Comparing `template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/PKG-INFO` & `template_pypackage_builder-0.9/src/template_pypackage_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: template-pypackage-builder
-Version: 0.8
+Version: 0.9
 Summary: A simple tool for packaging python
 Home-page: https://github.com/dipson94/packagemaker
 Author: Dipson
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `template_pypackage_builder-0.8/src/template_pypackage_builder.egg-info/SOURCES.txt` & `template_pypackage_builder-0.9/src/template_pypackage_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*


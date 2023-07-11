# Comparing `tmp/whoi_directory_tree-0.0.1.tar.gz` & `tmp/whoi_directory_tree-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whoi_directory_tree-0.0.1.tar", last modified: Tue Jul 11 22:35:13 2023, max compression
+gzip compressed data, was "whoi_directory_tree-0.0.2.tar", last modified: Tue Jul 11 22:44:06 2023, max compression
```

## Comparing `whoi_directory_tree-0.0.1.tar` & `whoi_directory_tree-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-11 22:35:13.411775 whoi_directory_tree-0.0.1/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      582 2023-07-11 18:04:00.000000 whoi_directory_tree-0.0.1/CHANGELOG.md
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     3356 2023-07-11 18:04:00.000000 whoi_directory_tree-0.0.1/CODE_OF_CONDUCT.md
--rw-rw-r--   0 brennan   (1000) brennan   (1000)    35141 2023-07-11 18:04:00.000000 whoi_directory_tree-0.0.1/LICENSE
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       30 2023-07-11 18:04:00.000000 whoi_directory_tree-0.0.1/MANIFEST.in
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      497 2023-07-11 22:35:13.411775 whoi_directory_tree-0.0.1/PKG-INFO
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      179 2023-07-11 22:34:33.000000 whoi_directory_tree-0.0.1/README.md
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       38 2023-07-11 22:35:13.411775 whoi_directory_tree-0.0.1/setup.cfg
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      674 2023-07-11 22:33:31.000000 whoi_directory_tree-0.0.1/setup.py
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-11 22:35:13.411775 whoi_directory_tree-0.0.1/src/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     4831 2023-07-11 18:04:40.000000 whoi_directory_tree-0.0.1/src/directory_tree.py
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-11 22:35:13.411775 whoi_directory_tree-0.0.1/src/whoi_directory_tree.egg-info/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      497 2023-07-11 22:35:13.000000 whoi_directory_tree-0.0.1/src/whoi_directory_tree.egg-info/PKG-INFO
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      280 2023-07-11 22:35:13.000000 whoi_directory_tree-0.0.1/src/whoi_directory_tree.egg-info/SOURCES.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)        1 2023-07-11 22:35:13.000000 whoi_directory_tree-0.0.1/src/whoi_directory_tree.egg-info/dependency_links.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       20 2023-07-11 22:35:13.000000 whoi_directory_tree-0.0.1/src/whoi_directory_tree.egg-info/top_level.txt
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-11 22:44:06.071131 whoi_directory_tree-0.0.2/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      582 2023-07-11 18:04:00.000000 whoi_directory_tree-0.0.2/CHANGELOG.md
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     3356 2023-07-11 18:04:00.000000 whoi_directory_tree-0.0.2/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)    35141 2023-07-11 18:04:00.000000 whoi_directory_tree-0.0.2/LICENSE
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       30 2023-07-11 18:04:00.000000 whoi_directory_tree-0.0.2/MANIFEST.in
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      497 2023-07-11 22:44:06.071131 whoi_directory_tree-0.0.2/PKG-INFO
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      179 2023-07-11 22:34:33.000000 whoi_directory_tree-0.0.2/README.md
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       38 2023-07-11 22:44:06.071131 whoi_directory_tree-0.0.2/setup.cfg
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      600 2023-07-11 22:43:29.000000 whoi_directory_tree-0.0.2/setup.py
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-11 22:44:06.071131 whoi_directory_tree-0.0.2/whoi_directory_tree/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     4831 2023-07-11 18:04:40.000000 whoi_directory_tree-0.0.2/whoi_directory_tree/directory_tree.py
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-11 22:44:06.071131 whoi_directory_tree-0.0.2/whoi_directory_tree.egg-info/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      497 2023-07-11 22:44:06.000000 whoi_directory_tree-0.0.2/whoi_directory_tree.egg-info/PKG-INFO
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      280 2023-07-11 22:44:06.000000 whoi_directory_tree-0.0.2/whoi_directory_tree.egg-info/SOURCES.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)        1 2023-07-11 22:44:06.000000 whoi_directory_tree-0.0.2/whoi_directory_tree.egg-info/dependency_links.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       20 2023-07-11 22:44:06.000000 whoi_directory_tree-0.0.2/whoi_directory_tree.egg-info/top_level.txt
```

### Comparing `whoi_directory_tree-0.0.1/CHANGELOG.md` & `whoi_directory_tree-0.0.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `whoi_directory_tree-0.0.1/CODE_OF_CONDUCT.md` & `whoi_directory_tree-0.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `whoi_directory_tree-0.0.1/LICENSE` & `whoi_directory_tree-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whoi_directory_tree-0.0.1/setup.py` & `whoi_directory_tree-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,22 +5,19 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Configuring Setup
 setup(
 
     name = 'whoi_directory_tree',
-    version = '0.0.1',
+    version = '0.0.2',
     description = 'whoi_directory_tree',
-    url = "https://github.com/rahulbordoloi/Directory-Tree/",
+    url = "https://git.whoi.edu/acomms/whoi_directory_tree/",
     author = "WHOI Acomms Group",
 
-    py_modules = ['whoi_directory_tree'],
-    package_dir = {'': 'src'},
-
     classifiers = [
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     ],
 
     long_description = long_description,
     long_description_content_type = "text/markdown",
```

### Comparing `whoi_directory_tree-0.0.1/src/directory_tree.py` & `whoi_directory_tree-0.0.2/whoi_directory_tree/directory_tree.py`

 * *Files identical despite different names*


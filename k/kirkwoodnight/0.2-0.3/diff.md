# Comparing `tmp/kirkwoodnight-0.2.tar.gz` & `tmp/kirkwoodnight-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kirkwoodnight-0.2.tar", last modified: Wed Jul 12 19:57:32 2023, max compression
+gzip compressed data, was "kirkwoodnight-0.3.tar", last modified: Wed Jul 12 20:16:27 2023, max compression
```

## Comparing `kirkwoodnight-0.2.tar` & `kirkwoodnight-0.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:57:32.308565 kirkwoodnight-0.2/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-0.2/LICENSE.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 19:57:32.308037 kirkwoodnight-0.2/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1768 2023-07-12 19:53:44.000000 kirkwoodnight-0.2/README.md
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:57:32.307240 kirkwoodnight-0.2/kirkwoodnight.egg-info/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 19:57:32.000000 kirkwoodnight-0.2/kirkwoodnight.egg-info/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)      254 2023-07-12 19:57:32.000000 kirkwoodnight-0.2/kirkwoodnight.egg-info/SOURCES.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-12 19:57:32.000000 kirkwoodnight-0.2/kirkwoodnight.egg-info/dependency_links.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       53 2023-07-12 19:57:32.000000 kirkwoodnight-0.2/kirkwoodnight.egg-info/entry_points.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       58 2023-07-12 19:57:32.000000 kirkwoodnight-0.2/kirkwoodnight.egg-info/requires.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-12 19:57:32.000000 kirkwoodnight-0.2/kirkwoodnight.egg-info/top_level.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-12 19:57:32.308744 kirkwoodnight-0.2/setup.cfg
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1076 2023-07-12 19:56:13.000000 kirkwoodnight-0.2/setup.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 20:16:27.326875 kirkwoodnight-0.3/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-0.3/LICENSE.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 20:16:27.326280 kirkwoodnight-0.3/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1768 2023-07-12 19:53:44.000000 kirkwoodnight-0.3/README.md
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 20:16:27.322062 kirkwoodnight-0.3/kirkwoodnight/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-0.3/kirkwoodnight/__init__.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)    18544 2023-07-12 20:15:28.000000 kirkwoodnight-0.3/kirkwoodnight/kirkwoodnight.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-12 20:16:27.325465 kirkwoodnight-0.3/kirkwoodnight.egg-info/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     2229 2023-07-12 20:16:27.000000 kirkwoodnight-0.3/kirkwoodnight.egg-info/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)      311 2023-07-12 20:16:27.000000 kirkwoodnight-0.3/kirkwoodnight.egg-info/SOURCES.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-12 20:16:27.000000 kirkwoodnight-0.3/kirkwoodnight.egg-info/dependency_links.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       53 2023-07-12 20:16:27.000000 kirkwoodnight-0.3/kirkwoodnight.egg-info/entry_points.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       58 2023-07-12 20:16:27.000000 kirkwoodnight-0.3/kirkwoodnight.egg-info/requires.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-12 20:16:27.000000 kirkwoodnight-0.3/kirkwoodnight.egg-info/top_level.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-12 20:16:27.327069 kirkwoodnight-0.3/setup.cfg
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1076 2023-07-12 20:15:42.000000 kirkwoodnight-0.3/setup.py
```

### Comparing `kirkwoodnight-0.2/LICENSE.txt` & `kirkwoodnight-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-0.2/PKG-INFO` & `kirkwoodnight-0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 0.2
+Version: 0.3
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `kirkwoodnight-0.2/README.md` & `kirkwoodnight-0.3/README.md`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-0.2/kirkwoodnight.egg-info/PKG-INFO` & `kirkwoodnight-0.3/kirkwoodnight.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 0.2
+Version: 0.3
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `kirkwoodnight-0.2/setup.py` & `kirkwoodnight-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     reqs = []
     for line in open("requirements.txt", "r").readlines():
         reqs.append(line)
     return reqs
 
 setup(
     name="kirkwoodnight",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
 
     # Metadata
     author="Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang",
     author_email="armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu",
     description="Interactive command line tool to assist with observations at Kirkwood Observatory.",
     long_description=open('README.md').read(),
```


# Comparing `tmp/PySortAlgos-0.4.tar.gz` & `tmp/PySortAlgos-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySortAlgos-0.4.tar", last modified: Wed Jul 12 11:18:37 2023, max compression
+gzip compressed data, was "PySortAlgos-0.5.tar", last modified: Wed Jul 12 11:26:41 2023, max compression
```

## Comparing `PySortAlgos-0.4.tar` & `PySortAlgos-0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 11:18:37.268370 PySortAlgos-0.4/
--rw-rw-rw-   0        0        0     1090 2023-07-12 09:26:51.000000 PySortAlgos-0.4/LICENSE
--rw-rw-rw-   0        0        0      653 2023-07-12 11:18:37.268370 PySortAlgos-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 11:18:37.251916 PySortAlgos-0.4/PySortAlgos/
--rw-rw-rw-   0        0        0      423 2023-07-12 10:42:02.000000 PySortAlgos-0.4/PySortAlgos/BubbleSort.py
--rw-rw-rw-   0        0        0      457 2023-07-12 10:41:40.000000 PySortAlgos-0.4/PySortAlgos/InsertionSort.py
--rw-rw-rw-   0        0        0     1081 2023-07-12 10:41:08.000000 PySortAlgos-0.4/PySortAlgos/MergeSort.py
--rw-rw-rw-   0        0        0      511 2023-07-12 10:39:59.000000 PySortAlgos-0.4/PySortAlgos/QuickSort.py
--rw-rw-rw-   0        0        0      490 2023-07-12 10:40:35.000000 PySortAlgos-0.4/PySortAlgos/SelectionSort.py
--rw-rw-rw-   0        0        0      190 2023-07-12 10:43:16.000000 PySortAlgos-0.4/PySortAlgos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 11:18:37.266358 PySortAlgos-0.4/PySortAlgos.egg-info/
--rw-rw-rw-   0        0        0      653 2023-07-12 11:18:37.000000 PySortAlgos-0.4/PySortAlgos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-07-12 11:18:37.000000 PySortAlgos-0.4/PySortAlgos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 11:18:37.000000 PySortAlgos-0.4/PySortAlgos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-12 11:18:37.000000 PySortAlgos-0.4/PySortAlgos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-07-12 09:37:44.000000 PySortAlgos-0.4/README.md
--rw-rw-rw-   0        0        0       86 2023-07-12 11:18:37.271346 PySortAlgos-0.4/setup.cfg
--rw-rw-rw-   0        0        0      772 2023-07-12 11:18:23.000000 PySortAlgos-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:26:41.152593 PySortAlgos-0.5/
+-rw-rw-rw-   0        0        0     1090 2023-07-12 09:26:51.000000 PySortAlgos-0.5/LICENSE
+-rw-rw-rw-   0        0        0      929 2023-07-12 11:26:41.153590 PySortAlgos-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 11:26:41.140624 PySortAlgos-0.5/PySortAlgos/
+-rw-rw-rw-   0        0        0      423 2023-07-12 10:42:02.000000 PySortAlgos-0.5/PySortAlgos/BubbleSort.py
+-rw-rw-rw-   0        0        0      457 2023-07-12 10:41:40.000000 PySortAlgos-0.5/PySortAlgos/InsertionSort.py
+-rw-rw-rw-   0        0        0     1081 2023-07-12 10:41:08.000000 PySortAlgos-0.5/PySortAlgos/MergeSort.py
+-rw-rw-rw-   0        0        0      511 2023-07-12 10:39:59.000000 PySortAlgos-0.5/PySortAlgos/QuickSort.py
+-rw-rw-rw-   0        0        0      490 2023-07-12 10:40:35.000000 PySortAlgos-0.5/PySortAlgos/SelectionSort.py
+-rw-rw-rw-   0        0        0      190 2023-07-12 10:43:16.000000 PySortAlgos-0.5/PySortAlgos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:26:41.151595 PySortAlgos-0.5/PySortAlgos.egg-info/
+-rw-rw-rw-   0        0        0      929 2023-07-12 11:26:41.000000 PySortAlgos-0.5/PySortAlgos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-07-12 11:26:41.000000 PySortAlgos-0.5/PySortAlgos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:26:41.000000 PySortAlgos-0.5/PySortAlgos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 11:26:41.000000 PySortAlgos-0.5/PySortAlgos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      358 2023-07-12 11:25:35.000000 PySortAlgos-0.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-12 11:26:41.155585 PySortAlgos-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      772 2023-07-12 11:25:51.000000 PySortAlgos-0.5/setup.py
```

### Comparing `PySortAlgos-0.4/LICENSE` & `PySortAlgos-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PySortAlgos-0.4/PKG-INFO` & `PySortAlgos-0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySortAlgos
-Version: 0.4
+Version: 0.5
 Summary: A simple package that contains some commonly used sorting functions
 Home-page: https://github.com/your-username/PySortAlgos
 Author: Bahir Hakimi
 Author-email: bahirhakimy2020@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -12,7 +12,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PySort
 
 ### A simple repo that contains some commonly used sorting functions
+
+# USAGE
+
+```python
+# import your desired sorting function
+from PySortAlgos import bubble_sort
+
+# Example list
+myList = [799,111,1,3,2,,23,6445,4,89,56,566]
+
+# Sort the list
+sorted = bubble_sort(myList)
+
+print(sorted) # [1,2,3,4,7,23,56,89,99,111,566,6445]
+```
```

### Comparing `PySortAlgos-0.4/PySortAlgos/MergeSort.py` & `PySortAlgos-0.5/PySortAlgos/MergeSort.py`

 * *Files identical despite different names*

### Comparing `PySortAlgos-0.4/PySortAlgos.egg-info/PKG-INFO` & `PySortAlgos-0.5/PySortAlgos.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySortAlgos
-Version: 0.4
+Version: 0.5
 Summary: A simple package that contains some commonly used sorting functions
 Home-page: https://github.com/your-username/PySortAlgos
 Author: Bahir Hakimi
 Author-email: bahirhakimy2020@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -12,7 +12,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PySort
 
 ### A simple repo that contains some commonly used sorting functions
+
+# USAGE
+
+```python
+# import your desired sorting function
+from PySortAlgos import bubble_sort
+
+# Example list
+myList = [799,111,1,3,2,,23,6445,4,89,56,566]
+
+# Sort the list
+sorted = bubble_sort(myList)
+
+print(sorted) # [1,2,3,4,7,23,56,89,99,111,566,6445]
+```
```

### Comparing `PySortAlgos-0.4/setup.py` & `PySortAlgos-0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='PySortAlgos',
-    version='0.4',
+    version='0.5',
     author='Bahir Hakimi',
     author_email='bahirhakimy2020@gmail.com',
     description='A simple package that contains some commonly used sorting functions',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/your-username/PySortAlgos',
     packages=['PySortAlgos'],
```


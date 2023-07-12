# Comparing `tmp/PySortAlgos-0.1.tar.gz` & `tmp/PySortAlgos-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySortAlgos-0.1.tar", last modified: Wed Jul 12 09:57:52 2023, max compression
+gzip compressed data, was "PySortAlgos-0.2.tar", last modified: Wed Jul 12 10:44:05 2023, max compression
```

## Comparing `PySortAlgos-0.1.tar` & `PySortAlgos-0.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 09:57:52.058081 PySortAlgos-0.1/
--rw-rw-rw-   0        0        0     1090 2023-07-12 09:26:51.000000 PySortAlgos-0.1/LICENSE
--rw-rw-rw-   0        0        0      669 2023-07-12 09:57:52.059073 PySortAlgos-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 09:57:52.035320 PySortAlgos-0.1/PySortAlgos/
--rw-rw-rw-   0        0        0       33 2023-07-12 09:16:36.000000 PySortAlgos-0.1/PySortAlgos/PySortAlgos.py
--rw-rw-rw-   0        0        0       24 2023-07-12 09:18:11.000000 PySortAlgos-0.1/PySortAlgos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 09:57:52.057073 PySortAlgos-0.1/PySortAlgos.egg-info/
--rw-rw-rw-   0        0        0      669 2023-07-12 09:57:51.000000 PySortAlgos-0.1/PySortAlgos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-07-12 09:57:51.000000 PySortAlgos-0.1/PySortAlgos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 09:57:51.000000 PySortAlgos-0.1/PySortAlgos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-12 09:57:51.000000 PySortAlgos-0.1/PySortAlgos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-07-12 09:37:44.000000 PySortAlgos-0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-07-12 09:57:52.061069 PySortAlgos-0.1/setup.cfg
--rw-rw-rw-   0        0        0      825 2023-07-12 09:57:39.000000 PySortAlgos-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:44:05.678285 PySortAlgos-0.2/
+-rw-rw-rw-   0        0        0     1090 2023-07-12 09:26:51.000000 PySortAlgos-0.2/LICENSE
+-rw-rw-rw-   0        0        0      672 2023-07-12 10:44:05.679284 PySortAlgos-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 10:44:05.656351 PySortAlgos-0.2/PySortAlgos/
+-rw-rw-rw-   0        0        0      423 2023-07-12 10:42:02.000000 PySortAlgos-0.2/PySortAlgos/BubbleSort.py
+-rw-rw-rw-   0        0        0      457 2023-07-12 10:41:40.000000 PySortAlgos-0.2/PySortAlgos/InsertionSort.py
+-rw-rw-rw-   0        0        0     1081 2023-07-12 10:41:08.000000 PySortAlgos-0.2/PySortAlgos/MergeSort.py
+-rw-rw-rw-   0        0        0      511 2023-07-12 10:39:59.000000 PySortAlgos-0.2/PySortAlgos/QuickSort.py
+-rw-rw-rw-   0        0        0      490 2023-07-12 10:40:35.000000 PySortAlgos-0.2/PySortAlgos/SelectionSort.py
+-rw-rw-rw-   0        0        0      190 2023-07-12 10:43:16.000000 PySortAlgos-0.2/PySortAlgos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 10:44:05.676314 PySortAlgos-0.2/PySortAlgos.egg-info/
+-rw-rw-rw-   0        0        0      672 2023-07-12 10:44:05.000000 PySortAlgos-0.2/PySortAlgos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-07-12 10:44:05.000000 PySortAlgos-0.2/PySortAlgos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 10:44:05.000000 PySortAlgos-0.2/PySortAlgos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 10:44:05.000000 PySortAlgos-0.2/PySortAlgos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-07-12 09:37:44.000000 PySortAlgos-0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-12 10:44:05.681278 PySortAlgos-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      828 2023-07-12 10:43:53.000000 PySortAlgos-0.2/setup.py
```

### Comparing `PySortAlgos-0.1/LICENSE` & `PySortAlgos-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PySortAlgos-0.1/PKG-INFO` & `PySortAlgos-0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: PySortAlgos
-Version: 0.1
-Summary: A simple repo that contains some commonly used sorting functions
+Version: 0.2
+Summary: A simple package that contains some commonly used sorting functions
 Home-page: https://github.com/bahirhakimy/PySortAlgos
 Download-URL: https://github.com/BahirHakimy/PySortAlgos/archive/refs/tags/0.1.tar.gz
 Author: Bahir Hakimi
 Author-email: bahirhakimy2020@gmail.com
 License: MIT
 Keywords: sorting,algorithm,quicksort,array
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `PySortAlgos-0.1/PySortAlgos.egg-info/PKG-INFO` & `PySortAlgos-0.2/PySortAlgos.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: PySortAlgos
-Version: 0.1
-Summary: A simple repo that contains some commonly used sorting functions
+Version: 0.2
+Summary: A simple package that contains some commonly used sorting functions
 Home-page: https://github.com/bahirhakimy/PySortAlgos
 Download-URL: https://github.com/BahirHakimy/PySortAlgos/archive/refs/tags/0.1.tar.gz
 Author: Bahir Hakimi
 Author-email: bahirhakimy2020@gmail.com
 License: MIT
 Keywords: sorting,algorithm,quicksort,array
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `PySortAlgos-0.1/setup.py` & `PySortAlgos-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 setup(
   name = 'PySortAlgos',
   packages = ['PySortAlgos'],
-  version = '0.1',
+  version = '0.2',
   license='MIT',
-  description = 'A simple repo that contains some commonly used sorting functions',
+  description = 'A simple package that contains some commonly used sorting functions',
   author = 'Bahir Hakimi',
   author_email = 'bahirhakimy2020@gmail.com',
   url = 'https://github.com/bahirhakimy/PySortAlgos',
   download_url = 'https://github.com/BahirHakimy/PySortAlgos/archive/refs/tags/0.1.tar.gz',
   keywords = ['sorting', 'algorithm', 'quicksort', 'array'],   # Keywords that define your package best
   install_requires=[],
   classifiers=[
```


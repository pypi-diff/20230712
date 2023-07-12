# Comparing `tmp/PySortAlgos-0.2.tar.gz` & `tmp/PySortAlgos-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySortAlgos-0.2.tar", last modified: Wed Jul 12 10:44:05 2023, max compression
+gzip compressed data, was "PySortAlgos-0.4.tar", last modified: Wed Jul 12 11:18:37 2023, max compression
```

## Comparing `PySortAlgos-0.2.tar` & `PySortAlgos-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 10:44:05.678285 PySortAlgos-0.2/
--rw-rw-rw-   0        0        0     1090 2023-07-12 09:26:51.000000 PySortAlgos-0.2/LICENSE
--rw-rw-rw-   0        0        0      672 2023-07-12 10:44:05.679284 PySortAlgos-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 10:44:05.656351 PySortAlgos-0.2/PySortAlgos/
--rw-rw-rw-   0        0        0      423 2023-07-12 10:42:02.000000 PySortAlgos-0.2/PySortAlgos/BubbleSort.py
--rw-rw-rw-   0        0        0      457 2023-07-12 10:41:40.000000 PySortAlgos-0.2/PySortAlgos/InsertionSort.py
--rw-rw-rw-   0        0        0     1081 2023-07-12 10:41:08.000000 PySortAlgos-0.2/PySortAlgos/MergeSort.py
--rw-rw-rw-   0        0        0      511 2023-07-12 10:39:59.000000 PySortAlgos-0.2/PySortAlgos/QuickSort.py
--rw-rw-rw-   0        0        0      490 2023-07-12 10:40:35.000000 PySortAlgos-0.2/PySortAlgos/SelectionSort.py
--rw-rw-rw-   0        0        0      190 2023-07-12 10:43:16.000000 PySortAlgos-0.2/PySortAlgos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 10:44:05.676314 PySortAlgos-0.2/PySortAlgos.egg-info/
--rw-rw-rw-   0        0        0      672 2023-07-12 10:44:05.000000 PySortAlgos-0.2/PySortAlgos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-07-12 10:44:05.000000 PySortAlgos-0.2/PySortAlgos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 10:44:05.000000 PySortAlgos-0.2/PySortAlgos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-12 10:44:05.000000 PySortAlgos-0.2/PySortAlgos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-07-12 09:37:44.000000 PySortAlgos-0.2/README.md
--rw-rw-rw-   0        0        0       86 2023-07-12 10:44:05.681278 PySortAlgos-0.2/setup.cfg
--rw-rw-rw-   0        0        0      828 2023-07-12 10:43:53.000000 PySortAlgos-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:18:37.268370 PySortAlgos-0.4/
+-rw-rw-rw-   0        0        0     1090 2023-07-12 09:26:51.000000 PySortAlgos-0.4/LICENSE
+-rw-rw-rw-   0        0        0      653 2023-07-12 11:18:37.268370 PySortAlgos-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 11:18:37.251916 PySortAlgos-0.4/PySortAlgos/
+-rw-rw-rw-   0        0        0      423 2023-07-12 10:42:02.000000 PySortAlgos-0.4/PySortAlgos/BubbleSort.py
+-rw-rw-rw-   0        0        0      457 2023-07-12 10:41:40.000000 PySortAlgos-0.4/PySortAlgos/InsertionSort.py
+-rw-rw-rw-   0        0        0     1081 2023-07-12 10:41:08.000000 PySortAlgos-0.4/PySortAlgos/MergeSort.py
+-rw-rw-rw-   0        0        0      511 2023-07-12 10:39:59.000000 PySortAlgos-0.4/PySortAlgos/QuickSort.py
+-rw-rw-rw-   0        0        0      490 2023-07-12 10:40:35.000000 PySortAlgos-0.4/PySortAlgos/SelectionSort.py
+-rw-rw-rw-   0        0        0      190 2023-07-12 10:43:16.000000 PySortAlgos-0.4/PySortAlgos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:18:37.266358 PySortAlgos-0.4/PySortAlgos.egg-info/
+-rw-rw-rw-   0        0        0      653 2023-07-12 11:18:37.000000 PySortAlgos-0.4/PySortAlgos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-07-12 11:18:37.000000 PySortAlgos-0.4/PySortAlgos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:18:37.000000 PySortAlgos-0.4/PySortAlgos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 11:18:37.000000 PySortAlgos-0.4/PySortAlgos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-07-12 09:37:44.000000 PySortAlgos-0.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-12 11:18:37.271346 PySortAlgos-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      772 2023-07-12 11:18:23.000000 PySortAlgos-0.4/setup.py
```

### Comparing `PySortAlgos-0.2/LICENSE` & `PySortAlgos-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PySortAlgos-0.2/PKG-INFO` & `PySortAlgos-0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: PySortAlgos
-Version: 0.2
+Version: 0.4
 Summary: A simple package that contains some commonly used sorting functions
-Home-page: https://github.com/bahirhakimy/PySortAlgos
-Download-URL: https://github.com/BahirHakimy/PySortAlgos/archive/refs/tags/0.1.tar.gz
+Home-page: https://github.com/your-username/PySortAlgos
 Author: Bahir Hakimi
 Author-email: bahirhakimy2020@gmail.com
-License: MIT
-Keywords: sorting,algorithm,quicksort,array
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# PySort
+
+### A simple repo that contains some commonly used sorting functions
```

### Comparing `PySortAlgos-0.2/PySortAlgos/MergeSort.py` & `PySortAlgos-0.4/PySortAlgos/MergeSort.py`

 * *Files identical despite different names*

### Comparing `PySortAlgos-0.2/PySortAlgos.egg-info/PKG-INFO` & `PySortAlgos-0.4/PySortAlgos.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: PySortAlgos
-Version: 0.2
+Version: 0.4
 Summary: A simple package that contains some commonly used sorting functions
-Home-page: https://github.com/bahirhakimy/PySortAlgos
-Download-URL: https://github.com/BahirHakimy/PySortAlgos/archive/refs/tags/0.1.tar.gz
+Home-page: https://github.com/your-username/PySortAlgos
 Author: Bahir Hakimi
 Author-email: bahirhakimy2020@gmail.com
-License: MIT
-Keywords: sorting,algorithm,quicksort,array
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# PySort
+
+### A simple repo that contains some commonly used sorting functions
```


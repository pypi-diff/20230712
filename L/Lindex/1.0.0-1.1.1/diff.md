# Comparing `tmp/Lindex-1.0.0.tar.gz` & `tmp/Lindex-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lindex-1.0.0.tar", last modified: Tue May 10 22:54:48 2022, max compression
+gzip compressed data, was "Lindex-1.1.1.tar", last modified: Wed Jul 12 06:14:15 2023, max compression
```

## Comparing `Lindex-1.0.0.tar` & `Lindex-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-05-10 22:54:48.163435 Lindex-1.0.0/
--rw-rw-rw-   0        0        0    18431 2022-05-07 00:23:32.000000 Lindex-1.0.0/LICENSE.md
-drwxrwxrwx   0        0        0        0 2022-05-10 22:54:48.150654 Lindex-1.0.0/Lindex/
--rw-rw-rw-   0        0        0     1957 2022-05-10 22:54:11.000000 Lindex-1.0.0/Lindex/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-10 22:54:48.163435 Lindex-1.0.0/Lindex.egg-info/
--rw-rw-rw-   0        0        0     1382 2022-05-10 22:54:47.000000 Lindex-1.0.0/Lindex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2022-05-10 22:54:48.000000 Lindex-1.0.0/Lindex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-10 22:54:47.000000 Lindex-1.0.0/Lindex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-05-10 22:54:48.000000 Lindex-1.0.0/Lindex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1382 2022-05-10 22:54:48.163435 Lindex-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2022-05-10 22:50:17.000000 Lindex-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2022-05-10 22:54:48.163435 Lindex-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      537 2022-05-10 22:50:23.000000 Lindex-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 06:14:15.840000 Lindex-1.1.1/
+-rw-rw-rw-   0        0        0    35811 2023-07-12 05:16:44.000000 Lindex-1.1.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-12 06:14:15.850000 Lindex-1.1.1/Lindex/
+-rw-rw-rw-   0        0        0     3837 2023-07-12 05:51:42.000000 Lindex-1.1.1/Lindex/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 06:14:15.870000 Lindex-1.1.1/Lindex.egg-info/
+-rw-rw-rw-   0        0        0     1548 2023-07-12 06:14:16.000000 Lindex-1.1.1/Lindex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2023-07-12 06:14:16.000000 Lindex-1.1.1/Lindex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 06:14:16.000000 Lindex-1.1.1/Lindex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 06:14:16.000000 Lindex-1.1.1/Lindex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1548 2023-07-12 06:14:16.000000 Lindex-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1215 2023-07-12 04:20:30.000000 Lindex-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 06:14:16.000000 Lindex-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      519 2023-07-12 06:10:10.000000 Lindex-1.1.1/setup.py
```

### Comparing `Lindex-1.0.0/Lindex.egg-info/PKG-INFO` & `Lindex-1.1.1/Lindex.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: Lindex
-Version: 1.0.0
+Version: 1.1.1
 Summary: A python Library created to improve functionality of Nested Dictionaries in Python
 Author: @some1and2
 Author-email: 04x0xx@gmail.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
+License-File: LICENSE
 
- # Lindex *[List Index]*
- ### by @some1and2
+# Lindex *[List Index]*
+### by @some1and2
 A `python` Library created to improve functionality of Nested Dictionaries in Python
 
- # Functionality::
+# Usage::
+```python
+from Lindex import lindex
+dictionary = {}
+dictionary = lindex(dictionary)
+```
+
+# Functionality::
 
 - Making a Lindex Dictionary
 	```python
 	dictionary = lindex(dictionary)
 	```
 
 - Ability to index Nested Dictionaries by using a list
@@ -25,23 +32,29 @@
 	```
 
 	if `path` is a list of indexes of the dictionary then this will return `dictionary[path[0]][path[1]][path[2]]...`
 
 
 - Ability to change information from a Nested Dictionary through a list
 	```python
-	dictionary.set(*path, num)
+	dictionary.set(*path, value)
 	```
-	if `path` is a list of indexes of the dictionary, then whatever value is at the end of `dictionary[path[0]][path[1]][path[2]]...` will be set to `num`
+	if `path` is a list of indexes of the dictionary, then whatever value is at the end of `dictionary[path[0]][path[1]][path[2]]...` will be set to `value`
 
 - Ability to add to a number from a Nested Dictionary indexed through a list
 	```python
-	dictionary.add(*path, num)
+	dictionary.add(*path, value)
 	```
-	whatever value is at the end of `dictionary[path[0]][path[1]][path[2]]...` will be added added with `num`
+	whatever value is at the end of `dictionary[path[0]][path[1]][path[2]]...` will be added added with `value`
 
 - Ability to pretty print dictionaries
 	```python
 	dictionary.pprint()
 	```
+
+# Installation::
+```python
+pip install Lindex
+```
 ---
+
 **Documentation** *[Coming Soon]*
```

### Comparing `Lindex-1.0.0/PKG-INFO` & `Lindex-1.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: Lindex
-Version: 1.0.0
+Version: 1.1.1
 Summary: A python Library created to improve functionality of Nested Dictionaries in Python
 Author: @some1and2
 Author-email: 04x0xx@gmail.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
+License-File: LICENSE
 
- # Lindex *[List Index]*
- ### by @some1and2
+# Lindex *[List Index]*
+### by @some1and2
 A `python` Library created to improve functionality of Nested Dictionaries in Python
 
- # Functionality::
+# Usage::
+```python
+from Lindex import lindex
+dictionary = {}
+dictionary = lindex(dictionary)
+```
+
+# Functionality::
 
 - Making a Lindex Dictionary
 	```python
 	dictionary = lindex(dictionary)
 	```
 
 - Ability to index Nested Dictionaries by using a list
@@ -25,23 +32,29 @@
 	```
 
 	if `path` is a list of indexes of the dictionary then this will return `dictionary[path[0]][path[1]][path[2]]...`
 
 
 - Ability to change information from a Nested Dictionary through a list
 	```python
-	dictionary.set(*path, num)
+	dictionary.set(*path, value)
 	```
-	if `path` is a list of indexes of the dictionary, then whatever value is at the end of `dictionary[path[0]][path[1]][path[2]]...` will be set to `num`
+	if `path` is a list of indexes of the dictionary, then whatever value is at the end of `dictionary[path[0]][path[1]][path[2]]...` will be set to `value`
 
 - Ability to add to a number from a Nested Dictionary indexed through a list
 	```python
-	dictionary.add(*path, num)
+	dictionary.add(*path, value)
 	```
-	whatever value is at the end of `dictionary[path[0]][path[1]][path[2]]...` will be added added with `num`
+	whatever value is at the end of `dictionary[path[0]][path[1]][path[2]]...` will be added added with `value`
 
 - Ability to pretty print dictionaries
 	```python
 	dictionary.pprint()
 	```
+
+# Installation::
+```python
+pip install Lindex
+```
 ---
+
 **Documentation** *[Coming Soon]*
```

### Comparing `Lindex-1.0.0/README.md` & `Lindex-1.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,50 @@
- # Lindex *[List Index]*
- ### by @some1and2
-A `python` Library created to improve functionality of Nested Dictionaries in Python
-
- # Functionality::
-
-- Making a Lindex Dictionary
-	```python
-	dictionary = lindex(dictionary)
-	```
-
-- Ability to index Nested Dictionaries by using a list
-	```python
-	print(dictionary.RTN(*path))
-	```
-
-	if `path` is a list of indexes of the dictionary then this will return `dictionary[path[0]][path[1]][path[2]]...`
-
-
-- Ability to change information from a Nested Dictionary through a list
-	```python
-	dictionary.set(*path, num)
-	```
-	if `path` is a list of indexes of the dictionary, then whatever value is at the end of `dictionary[path[0]][path[1]][path[2]]...` will be set to `num`
-
-- Ability to add to a number from a Nested Dictionary indexed through a list
-	```python
-	dictionary.add(*path, num)
-	```
-	whatever value is at the end of `dictionary[path[0]][path[1]][path[2]]...` will be added added with `num`
-
-- Ability to pretty print dictionaries
-	```python
-	dictionary.pprint()
-	```
----
+# Lindex *[List Index]*
+### by @some1and2
+A `python` Library created to improve functionality of Nested Dictionaries in Python
+
+# Usage::
+```python
+from Lindex import lindex
+dictionary = {}
+dictionary = lindex(dictionary)
+```
+
+# Functionality::
+
+- Making a Lindex Dictionary
+	```python
+	dictionary = lindex(dictionary)
+	```
+
+- Ability to index Nested Dictionaries by using a list
+	```python
+	print(dictionary.RTN(*path))
+	```
+
+	if `path` is a list of indexes of the dictionary then this will return `dictionary[path[0]][path[1]][path[2]]...`
+
+
+- Ability to change information from a Nested Dictionary through a list
+	```python
+	dictionary.set(*path, value)
+	```
+	if `path` is a list of indexes of the dictionary, then whatever value is at the end of `dictionary[path[0]][path[1]][path[2]]...` will be set to `value`
+
+- Ability to add to a number from a Nested Dictionary indexed through a list
+	```python
+	dictionary.add(*path, value)
+	```
+	whatever value is at the end of `dictionary[path[0]][path[1]][path[2]]...` will be added added with `value`
+
+- Ability to pretty print dictionaries
+	```python
+	dictionary.pprint()
+	```
+
+# Installation::
+```python
+pip install Lindex
+```
+---
+
 **Documentation** *[Coming Soon]*
```


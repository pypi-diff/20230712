# Comparing `tmp/Test-User-Generator-1.0.0.tar.gz` & `tmp/Test-User-Generator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Test-User-Generator-1.0.0.tar", last modified: Wed Jul 12 17:19:21 2023, max compression
+gzip compressed data, was "Test-User-Generator-1.1.0.tar", last modified: Wed Jul 12 17:40:49 2023, max compression
```

## Comparing `Test-User-Generator-1.0.0.tar` & `Test-User-Generator-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 17:19:21.778447 Test-User-Generator-1.0.0/
--rw-rw-rw-   0        0        0       17 2023-07-12 17:13:02.000000 Test-User-Generator-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      217 2023-07-12 17:19:21.778447 Test-User-Generator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      767 2023-07-12 17:18:23.000000 Test-User-Generator-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 17:19:21.771440 Test-User-Generator-1.0.0/Test_User_Generator/
--rw-rw-rw-   0        0        0        0 2023-07-12 02:30:57.000000 Test-User-Generator-1.0.0/Test_User_Generator/__init__.py
--rw-rw-rw-   0        0        0     5414 2023-07-12 17:04:10.000000 Test-User-Generator-1.0.0/Test_User_Generator/user_generator.py
-drwxrwxrwx   0        0        0        0 2023-07-12 17:19:21.778447 Test-User-Generator-1.0.0/Test_User_Generator.egg-info/
--rw-rw-rw-   0        0        0      217 2023-07-12 17:19:21.000000 Test-User-Generator-1.0.0/Test_User_Generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-07-12 17:19:21.000000 Test-User-Generator-1.0.0/Test_User_Generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 17:19:21.000000 Test-User-Generator-1.0.0/Test_User_Generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 17:19:21.000000 Test-User-Generator-1.0.0/Test_User_Generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-12 17:19:21.000000 Test-User-Generator-1.0.0/Test_User_Generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 17:19:21.778447 Test-User-Generator-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      430 2023-07-12 17:12:11.000000 Test-User-Generator-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 17:40:49.663977 Test-User-Generator-1.1.0/
+-rw-rw-rw-   0        0        0       17 2023-07-12 17:13:02.000000 Test-User-Generator-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      217 2023-07-12 17:40:49.663977 Test-User-Generator-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-07-12 17:30:03.000000 Test-User-Generator-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 17:40:49.648221 Test-User-Generator-1.1.0/Test_User_Generator/
+-rw-rw-rw-   0        0        0        0 2023-07-12 02:30:57.000000 Test-User-Generator-1.1.0/Test_User_Generator/__init__.py
+-rw-rw-rw-   0        0        0     5414 2023-07-12 17:04:10.000000 Test-User-Generator-1.1.0/Test_User_Generator/user_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-12 17:40:49.663977 Test-User-Generator-1.1.0/Test_User_Generator.egg-info/
+-rw-rw-rw-   0        0        0      217 2023-07-12 17:40:49.000000 Test-User-Generator-1.1.0/Test_User_Generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-07-12 17:40:49.000000 Test-User-Generator-1.1.0/Test_User_Generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 17:40:49.000000 Test-User-Generator-1.1.0/Test_User_Generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 17:40:49.000000 Test-User-Generator-1.1.0/Test_User_Generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-12 17:40:49.000000 Test-User-Generator-1.1.0/Test_User_Generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 17:40:49.663977 Test-User-Generator-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      430 2023-07-12 17:35:45.000000 Test-User-Generator-1.1.0/setup.py
```

### Comparing `Test-User-Generator-1.0.0/README.md` & `Test-User-Generator-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 
 ## Installation
 
 You can install `Test-User-Generator` using `pip`:
 
 ```bash
 pip install Test-User-Generator
+```
 
 Usage
 Example of usage:
-
+```
 from Test_User_Generator.user_generator import Create_User
 user = Create_User()
 user.get_first_name()
+```
 
 Contributing
 Contributions are welcome! Here's how you can contribute:
 
 Fork the repository.
 Create a new branch.
 Make your changes.
```

### Comparing `Test-User-Generator-1.0.0/Test_User_Generator/user_generator.py` & `Test-User-Generator-1.1.0/Test_User_Generator/user_generator.py`

 * *Files identical despite different names*


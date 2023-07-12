# Comparing `tmp/pyntree-1.2.1.tar.gz` & `tmp/pyntree-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntree-1.2.1.tar", last modified: Tue May 23 22:59:12 2023, max compression
+gzip compressed data, was "pyntree-1.2.2.tar", last modified: Wed Jul 12 03:11:36 2023, max compression
```

## Comparing `pyntree-1.2.1.tar` & `pyntree-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-05-23 22:59:12.838169 pyntree-1.2.1/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    11357 2023-03-27 17:16:15.000000 pyntree-1.2.1/LICENSE.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-05-23 22:59:12.838169 pyntree-1.2.1/PKG-INFO
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1585 2023-03-29 03:58:07.000000 pyntree-1.2.1/README.md
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-05-23 22:59:12.834169 pyntree-1.2.1/pyntree/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     9292 2023-05-23 22:51:03.000000 pyntree-1.2.1/pyntree/__init__.py
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1128 2023-04-17 13:39:08.000000 pyntree-1.2.1/pyntree/encryption.py
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      166 2023-04-10 21:40:01.000000 pyntree-1.2.1/pyntree/errors.py
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     6436 2023-05-23 22:51:02.000000 pyntree-1.2.1/pyntree/file.py
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-05-23 22:59:12.834169 pyntree-1.2.1/pyntree.egg-info/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-05-23 22:59:12.000000 pyntree-1.2.1/pyntree.egg-info/PKG-INFO
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      298 2023-05-23 22:59:12.000000 pyntree-1.2.1/pyntree.egg-info/SOURCES.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        1 2023-05-23 22:59:12.000000 pyntree-1.2.1/pyntree.egg-info/dependency_links.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      126 2023-05-23 22:59:12.000000 pyntree-1.2.1/pyntree.egg-info/requires.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        8 2023-05-23 22:59:12.000000 pyntree-1.2.1/pyntree.egg-info/top_level.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1310 2023-05-23 22:54:39.000000 pyntree-1.2.1/pyproject.toml
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       23 2023-03-27 16:14:00.000000 pyntree-1.2.1/requirements.txt
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       38 2023-05-23 22:59:12.838169 pyntree-1.2.1/setup.cfg
-drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-05-23 22:59:12.838169 pyntree-1.2.1/tests/
--rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    11430 2023-05-23 22:52:34.000000 pyntree-1.2.1/tests/tests.py
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-07-12 03:11:36.054600 pyntree-1.2.2/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    11357 2023-03-27 17:16:15.000000 pyntree-1.2.2/LICENSE.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-07-12 03:11:36.054600 pyntree-1.2.2/PKG-INFO
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1585 2023-03-29 03:58:07.000000 pyntree-1.2.2/README.md
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-07-12 03:11:36.050600 pyntree-1.2.2/pyntree/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     9292 2023-05-23 22:51:03.000000 pyntree-1.2.2/pyntree/__init__.py
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1128 2023-04-17 13:39:08.000000 pyntree-1.2.2/pyntree/encryption.py
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      166 2023-04-10 21:40:01.000000 pyntree-1.2.2/pyntree/errors.py
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     6575 2023-07-12 03:09:18.000000 pyntree-1.2.2/pyntree/file.py
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-07-12 03:11:36.054600 pyntree-1.2.2/pyntree.egg-info/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    15475 2023-07-12 03:11:36.000000 pyntree-1.2.2/pyntree.egg-info/PKG-INFO
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      298 2023-07-12 03:11:36.000000 pyntree-1.2.2/pyntree.egg-info/SOURCES.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        1 2023-07-12 03:11:36.000000 pyntree-1.2.2/pyntree.egg-info/dependency_links.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)      126 2023-07-12 03:11:36.000000 pyntree-1.2.2/pyntree.egg-info/requires.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)        8 2023-07-12 03:11:36.000000 pyntree-1.2.2/pyntree.egg-info/top_level.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)     1310 2023-07-12 03:11:14.000000 pyntree-1.2.2/pyproject.toml
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       23 2023-03-27 16:14:00.000000 pyntree-1.2.2/requirements.txt
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)       38 2023-07-12 03:11:36.054600 pyntree-1.2.2/setup.cfg
+drwxrwxr-x   0 jvadair   (1000) jvadair   (1000)        0 2023-07-12 03:11:36.054600 pyntree-1.2.2/tests/
+-rw-rw-r--   0 jvadair   (1000) jvadair   (1000)    11577 2023-07-12 03:09:18.000000 pyntree-1.2.2/tests/tests.py
```

### Comparing `pyntree-1.2.1/LICENSE.txt` & `pyntree-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyntree-1.2.1/PKG-INFO` & `pyntree-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntree
-Version: 1.2.1
+Version: 1.2.2
 Summary: pyntree is a python package which allows you to easily and syntactically save your data. Not only that, it also lets you save in multiple formats, and even serialize and compress data by merely changing a few characters.
 Author-email: jvadair <dev@jvadair.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pyntree-1.2.1/README.md` & `pyntree-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyntree-1.2.1/pyntree/__init__.py` & `pyntree-1.2.2/pyntree/__init__.py`

 * *Files identical despite different names*

### Comparing `pyntree-1.2.1/pyntree/encryption.py` & `pyntree-1.2.2/pyntree/encryption.py`

 * *Files identical despite different names*

### Comparing `pyntree-1.2.1/pyntree/file.py` & `pyntree-1.2.2/pyntree/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         """
         Sets the data object for the file to the data stored in the file
         :return:
         """
         self.data = self.read_data()
 
     # noinspection PyUnboundLocalVariable
-    def save(self, filename=None) -> None:
+    def save(self, filename=None, password=None) -> None:
         """
         Saves the data to the file
         :param filename: If set, the Node will save to the specified file and then reload its original file object
         """
         if filename:  # Only keeps 1 file in memory at a time
             old_filename = self.name
             self.switch_to_file(filename)
@@ -146,15 +146,18 @@
         elif self.filetype == 'txt':
             to_write = str(self.data).encode()
         elif self.filetype in pickle.get_known_compressions():
             to_write = pickle.dumps(self.data, self.filetype)
 
         if self.password:
             encryption.check()
-            to_write = encryption.encrypt(to_write, self.password, self.salt)
+            if password:
+                to_write = encryption.encrypt(to_write, password, self.salt)
+            else:
+                to_write = encryption.encrypt(to_write, self.password, self.salt)
         
         self.file.seek(0)
         self.file.write(to_write)
         self.file.truncate()
         if filename and old_filename:  # If the old filename was None, then it can't be switched back to
             self.switch_to_file(old_filename)
```

### Comparing `pyntree-1.2.1/pyntree.egg-info/PKG-INFO` & `pyntree-1.2.2/pyntree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntree
-Version: 1.2.1
+Version: 1.2.2
 Summary: pyntree is a python package which allows you to easily and syntactically save your data. Not only that, it also lets you save in multiple formats, and even serialize and compress data by merely changing a few characters.
 Author-email: jvadair <dev@jvadair.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pyntree-1.2.1/pyproject.toml` & `pyntree-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["dependencies"]
 name = "pyntree"
-version = "1.2.1"
+version = "1.2.2"
 description = "pyntree is a python package which allows you to easily and syntactically save your data. Not only that, it also lets you save in multiple formats, and even serialize and compress data by merely changing a few characters."
 readme = "README.md"
 authors = [{ name = "jvadair", email = "dev@jvadair.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `pyntree-1.2.1/tests/tests.py` & `pyntree-1.2.2/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,18 @@
     def test_encrypted_save(self):
         for ext in EXTENSIONS:
             with self.subTest(msg=ext):
                 db = Node({'a': 1, 'b': {'c': 2}}, password='testing')
                 db.save(f'tests/newdb.{ext}')
                 os.remove(f'tests/newdb.{ext}')
 
+    def test_encrypted_save_method(self):
+        Node({'a': 1}).save('tests/newdb.pyn', password='testing')
+        os.remove('tests/newdb.pyn')
+
     def test_save_to_alternate_file(self):
         # Initial data
         db = Node({'a': 1, 'b': {'c': 2}})
         db.switch_to_file('tests/testing_output.txt')
         db.save()
         del db
         # Overwrite, but maintain original file object
```


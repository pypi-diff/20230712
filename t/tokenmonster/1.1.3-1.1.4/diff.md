# Comparing `tmp/tokenmonster-1.1.3.tar.gz` & `tmp/tokenmonster-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenmonster-1.1.3.tar", last modified: Wed Jul 12 14:07:31 2023, max compression
+gzip compressed data, was "tokenmonster-1.1.4.tar", last modified: Wed Jul 12 14:21:10 2023, max compression
```

## Comparing `tokenmonster-1.1.3.tar` & `tokenmonster-1.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:07:31.357601 tokenmonster-1.1.3/
--rw-r--r--   0 root         (0) root         (0)    16622 2023-07-12 14:07:31.357601 tokenmonster-1.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16887 2023-07-12 14:01:39.000000 tokenmonster-1.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 14:07:31.357601 tokenmonster-1.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      550 2023-07-12 14:00:34.000000 tokenmonster-1.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:07:31.357601 tokenmonster-1.1.3/tokenmonster.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16622 2023-07-12 14:07:31.000000 tokenmonster-1.1.3/tokenmonster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-12 14:07:31.000000 tokenmonster-1.1.3/tokenmonster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 14:07:31.000000 tokenmonster-1.1.3/tokenmonster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 14:07:31.000000 tokenmonster-1.1.3/tokenmonster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    49036 2023-07-12 14:03:25.000000 tokenmonster-1.1.3/tokenmonster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:21:10.009109 tokenmonster-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)    16622 2023-07-12 14:21:10.009109 tokenmonster-1.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16887 2023-07-12 14:01:39.000000 tokenmonster-1.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 14:21:10.009109 tokenmonster-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      550 2023-07-12 14:19:35.000000 tokenmonster-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:21:10.009109 tokenmonster-1.1.4/tokenmonster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16622 2023-07-12 14:21:09.000000 tokenmonster-1.1.4/tokenmonster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-12 14:21:09.000000 tokenmonster-1.1.4/tokenmonster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 14:21:09.000000 tokenmonster-1.1.4/tokenmonster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 14:21:09.000000 tokenmonster-1.1.4/tokenmonster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    49041 2023-07-12 14:19:11.000000 tokenmonster-1.1.4/tokenmonster.py
```

### Comparing `tokenmonster-1.1.3/PKG-INFO` & `tokenmonster-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.1.3
+Version: 1.1.4
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `tokenmonster-1.1.3/README.md` & `tokenmonster-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tokenmonster-1.1.3/setup.py` & `tokenmonster-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tokenmonster',
-    version='1.1.3',
+    version='1.1.4',
     py_modules=['tokenmonster'],
     author='Alasdair Forsythe',
     author_email='77910352+alasdairforsythe@users.noreply.github.com',
     description='Tokenize and decode text with TokenMonster vocabularies.',
     url='https://github.com/alasdairforsythe/tokenmonster',
     license='MIT',
     long_description=long_description,
```

### Comparing `tokenmonster-1.1.3/tokenmonster.egg-info/PKG-INFO` & `tokenmonster-1.1.4/tokenmonster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.1.3
+Version: 1.1.4
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `tokenmonster-1.1.3/tokenmonster.py` & `tokenmonster-1.1.4/tokenmonster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1026,19 +1026,19 @@
             os.makedirs(dir)
             if not os.path.exists(dir):
                 raise RuntimeError("Unable to create directory: {}".format(dir))
         cls._dir = dir
 
     @classmethod
     def _disconnect(cls):
-        if cls.process is not None:
-            cls.process.stdin.close()
-            cls.process.stdout.close()
-            cls.process.kill()
-            cls.process = None
+        if cls._process is not None:
+            cls._process.stdin.close()
+            cls._process.stdout.close()
+            cls._process.kill()
+            cls._process = None
             for i in range(len(cls._vocabs)):
                 cls._vocabs[i]._modified_id = -1
             cls._vocabs = []
 
     @classmethod
     def _download(cls, url, fname):
         urllib.request.urlretrieve(url, os.path.join(cls._dir, fname))
```


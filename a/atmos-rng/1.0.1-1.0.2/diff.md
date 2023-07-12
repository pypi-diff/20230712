# Comparing `tmp/atmos-rng-1.0.1.tar.gz` & `tmp/atmos-rng-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmos-rng-1.0.1.tar", last modified: Tue Jul 11 04:50:01 2023, max compression
+gzip compressed data, was "atmos-rng-1.0.2.tar", last modified: Wed Jul 12 18:22:48 2023, max compression
```

## Comparing `atmos-rng-1.0.1.tar` & `atmos-rng-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:50:01.785056 atmos-rng-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 04:49:51.000000 atmos-rng-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-11 04:50:01.785056 atmos-rng-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-11 04:49:51.000000 atmos-rng-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-11 04:49:51.000000 atmos-rng-1.0.1/atmos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:50:01.785056 atmos-rng-1.0.1/atmos_rng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-11 04:50:01.000000 atmos-rng-1.0.1/atmos_rng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-11 04:50:01.000000 atmos-rng-1.0.1/atmos_rng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 04:50:01.000000 atmos-rng-1.0.1/atmos_rng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 04:50:01.000000 atmos-rng-1.0.1/atmos_rng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 04:50:01.000000 atmos-rng-1.0.1/atmos_rng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 04:50:01.785056 atmos-rng-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-11 04:49:51.000000 atmos-rng-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:22:48.959219 atmos-rng-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 18:22:36.000000 atmos-rng-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-12 18:22:48.959219 atmos-rng-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-12 18:22:36.000000 atmos-rng-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-12 18:22:36.000000 atmos-rng-1.0.2/atmos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:22:48.959219 atmos-rng-1.0.2/atmos_rng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-12 18:22:48.000000 atmos-rng-1.0.2/atmos_rng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-12 18:22:48.000000 atmos-rng-1.0.2/atmos_rng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:22:48.000000 atmos-rng-1.0.2/atmos_rng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 18:22:48.000000 atmos-rng-1.0.2/atmos_rng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 18:22:48.000000 atmos-rng-1.0.2/atmos_rng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:22:48.959219 atmos-rng-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-12 18:22:36.000000 atmos-rng-1.0.2/setup.py
```

### Comparing `atmos-rng-1.0.1/LICENSE` & `atmos-rng-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atmos-rng-1.0.1/PKG-INFO` & `atmos-rng-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmos-rng
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple random generator based off of atmospheric noise instead of math.
 Home-page: https://github.com/therealOri/atmos-rng
 Author: therealOri
 Author-email: therealOri@duck.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -45,16 +45,22 @@
     stuff = [69, True, False, 420, 'Apples', 'Bananas', 'Cats', 'Dogs']
     choice = atmos.choice(stuff)
     print(choice)
 
     scrambled = atmos.shuffle(stuff)
     print(scrambled)
 
-    random_bytes = gen_bytes(32)
+    random_bytes = atmos.gen_bytes(32)
     print(f"{random_bytes}\n{len(random_bytes)}")
+
+    random_bits = atmos.gen_bits(25)
+    print(random_bits)
+
+    urlsafe_bytes = atmos.bytes_urlsafe(20)
+    print(urlsafe_bytes)
 ```
 You can find more information here: [Documentation](https://github.com/therealOri/atmos-rng/blob/main/DOCS.md).
 __ __
 
 <br />
 <br />
 <br />
```

### Comparing `atmos-rng-1.0.1/README.md` & `atmos-rng-1.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -34,16 +34,22 @@
     stuff = [69, True, False, 420, 'Apples', 'Bananas', 'Cats', 'Dogs']
     choice = atmos.choice(stuff)
     print(choice)
 
     scrambled = atmos.shuffle(stuff)
     print(scrambled)
 
-    random_bytes = gen_bytes(32)
+    random_bytes = atmos.gen_bytes(32)
     print(f"{random_bytes}\n{len(random_bytes)}")
+
+    random_bits = atmos.gen_bits(25)
+    print(random_bits)
+
+    urlsafe_bytes = atmos.bytes_urlsafe(20)
+    print(urlsafe_bytes)
 ```
 You can find more information here: [Documentation](https://github.com/therealOri/atmos-rng/blob/main/DOCS.md).
 __ __
 
 <br />
 <br />
 <br />
```

### Comparing `atmos-rng-1.0.1/atmos_rng.egg-info/PKG-INFO` & `atmos-rng-1.0.2/atmos_rng.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmos-rng
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple random generator based off of atmospheric noise instead of math.
 Home-page: https://github.com/therealOri/atmos-rng
 Author: therealOri
 Author-email: therealOri@duck.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -45,16 +45,22 @@
     stuff = [69, True, False, 420, 'Apples', 'Bananas', 'Cats', 'Dogs']
     choice = atmos.choice(stuff)
     print(choice)
 
     scrambled = atmos.shuffle(stuff)
     print(scrambled)
 
-    random_bytes = gen_bytes(32)
+    random_bytes = atmos.gen_bytes(32)
     print(f"{random_bytes}\n{len(random_bytes)}")
+
+    random_bits = atmos.gen_bits(25)
+    print(random_bits)
+
+    urlsafe_bytes = atmos.bytes_urlsafe(20)
+    print(urlsafe_bytes)
 ```
 You can find more information here: [Documentation](https://github.com/therealOri/atmos-rng/blob/main/DOCS.md).
 __ __
 
 <br />
 <br />
 <br />
```

### Comparing `atmos-rng-1.0.1/setup.py` & `atmos-rng-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="atmos-rng",
-    version="1.0.1",
+    version="1.0.2",
     author="therealOri",
     license="GPL-3.0",
     install_requires=[
         "requests",
     ],
     author_email="therealOri@duck.com",
     description="A simple random generator based off of atmospheric noise instead of math.",
```


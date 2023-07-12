# Comparing `tmp/chamd-0.5.7.tar.gz` & `tmp/chamd-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chamd-0.5.7.tar", last modified: Wed May 18 06:58:13 2022, max compression
+gzip compressed data, was "dist/chamd-0.5.8.tar", last modified: Thu May 19 08:14:07 2022, max compression
```

## Comparing `chamd-0.5.7.tar` & `chamd-0.5.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-05-18 06:58:13.000000 chamd-0.5.7/
--rw-r--r--   0 3248526    (502) staff       (20)     1878 2022-05-18 06:58:13.000000 chamd-0.5.7/PKG-INFO
-drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-05-18 06:58:13.000000 chamd-0.5.7/chamd.egg-info/
--rw-r--r--   0 3248526    (502) staff       (20)     1878 2022-05-18 06:58:12.000000 chamd-0.5.7/chamd.egg-info/PKG-INFO
--rw-r--r--   0 3248526    (502) staff       (20)        1 2020-09-09 09:13:44.000000 chamd-0.5.7/chamd.egg-info/zip-safe
--rw-r--r--   0 3248526    (502) staff       (20)      272 2022-05-18 06:58:13.000000 chamd-0.5.7/chamd.egg-info/SOURCES.txt
--rw-r--r--   0 3248526    (502) staff       (20)       47 2022-05-18 06:58:12.000000 chamd-0.5.7/chamd.egg-info/entry_points.txt
--rw-r--r--   0 3248526    (502) staff       (20)        6 2022-05-18 06:58:12.000000 chamd-0.5.7/chamd.egg-info/top_level.txt
--rw-r--r--   0 3248526    (502) staff       (20)        1 2022-05-18 06:58:12.000000 chamd-0.5.7/chamd.egg-info/dependency_links.txt
--rw-r--r--   0 3248526    (502) staff       (20)      661 2022-05-18 06:57:43.000000 chamd-0.5.7/setup.py
-drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-05-18 06:58:13.000000 chamd-0.5.7/chamd/
--rw-r--r--   0 3248526    (502) staff       (20)    12694 2022-01-31 14:46:23.000000 chamd-0.5.7/chamd/cleanCHILDESMD.py
--rw-r--r--   0 3248526    (502) staff       (20)      114 2022-01-31 14:46:23.000000 chamd-0.5.7/chamd/__init__.py
--rw-r--r--   0 3248526    (502) staff       (20)    23845 2022-05-18 06:57:31.000000 chamd-0.5.7/chamd/chat_reader.py
--rw-r--r--   0 3248526    (502) staff       (20)     6068 2022-01-31 14:46:23.000000 chamd-0.5.7/chamd/__main__.py
--rw-r--r--   0 3248526    (502) staff       (20)       38 2022-05-18 06:58:13.000000 chamd-0.5.7/setup.cfg
--rw-r--r--   0 3248526    (502) staff       (20)     1103 2022-02-03 12:38:32.000000 chamd-0.5.7/README.rst
+drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-05-19 08:14:07.000000 chamd-0.5.8/
+-rw-r--r--   0 3248526    (502) staff       (20)     1878 2022-05-19 08:14:07.000000 chamd-0.5.8/PKG-INFO
+drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-05-19 08:14:07.000000 chamd-0.5.8/chamd.egg-info/
+-rw-r--r--   0 3248526    (502) staff       (20)     1878 2022-05-19 08:14:07.000000 chamd-0.5.8/chamd.egg-info/PKG-INFO
+-rw-r--r--   0 3248526    (502) staff       (20)        1 2020-09-09 09:13:44.000000 chamd-0.5.8/chamd.egg-info/zip-safe
+-rw-r--r--   0 3248526    (502) staff       (20)      280 2022-05-19 08:14:07.000000 chamd-0.5.8/chamd.egg-info/SOURCES.txt
+-rw-r--r--   0 3248526    (502) staff       (20)       47 2022-05-19 08:14:07.000000 chamd-0.5.8/chamd.egg-info/entry_points.txt
+-rw-r--r--   0 3248526    (502) staff       (20)        6 2022-05-19 08:14:07.000000 chamd-0.5.8/chamd.egg-info/top_level.txt
+-rw-r--r--   0 3248526    (502) staff       (20)        1 2022-05-19 08:14:07.000000 chamd-0.5.8/chamd.egg-info/dependency_links.txt
+-rw-r--r--   0 3248526    (502) staff       (20)     1082 2019-11-18 13:08:43.000000 chamd-0.5.8/LICENSE
+-rw-r--r--   0 3248526    (502) staff       (20)      661 2022-05-19 08:13:33.000000 chamd-0.5.8/setup.py
+drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-05-19 08:14:07.000000 chamd-0.5.8/chamd/
+-rw-r--r--   0 3248526    (502) staff       (20)    12694 2022-01-31 14:46:23.000000 chamd-0.5.8/chamd/cleanCHILDESMD.py
+-rw-r--r--   0 3248526    (502) staff       (20)      114 2022-01-31 14:46:23.000000 chamd-0.5.8/chamd/__init__.py
+-rw-r--r--   0 3248526    (502) staff       (20)    23934 2022-05-19 08:13:33.000000 chamd-0.5.8/chamd/chat_reader.py
+-rw-r--r--   0 3248526    (502) staff       (20)     6068 2022-01-31 14:46:23.000000 chamd-0.5.8/chamd/__main__.py
+-rw-r--r--   0 3248526    (502) staff       (20)       38 2022-05-19 08:14:07.000000 chamd-0.5.8/setup.cfg
+-rw-r--r--   0 3248526    (502) staff       (20)     1103 2022-02-03 12:38:32.000000 chamd-0.5.8/README.rst
```

### Comparing `chamd-0.5.7/PKG-INFO` & `chamd-0.5.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: chamd
-Version: 0.5.7
+Version: 0.5.8
 Summary: Conversion and cleaning of CHILDES CHA files into PaQu Plaintext Metadata Format
 Home-page: https://github.com/UUDigitalHumanitieslab/chamd
 Author: Digital Humanities Lab, Utrecht University
 Author-email: digitalhumanities@uu.nl
 License: MIT
 Description: [![Python package](https://github.com/UUDigitalHumanitieslab/chamd/actions/workflows/python-package.yml/badge.svg?branch=develop)](https://github.com/UUDigitalHumanitieslab/chamd/actions/workflows/python-package.yml)
```

### Comparing `chamd-0.5.7/chamd.egg-info/PKG-INFO` & `chamd-0.5.8/chamd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: chamd
-Version: 0.5.7
+Version: 0.5.8
 Summary: Conversion and cleaning of CHILDES CHA files into PaQu Plaintext Metadata Format
 Home-page: https://github.com/UUDigitalHumanitieslab/chamd
 Author: Digital Humanities Lab, Utrecht University
 Author-email: digitalhumanities@uu.nl
 License: MIT
 Description: [![Python package](https://github.com/UUDigitalHumanitieslab/chamd/actions/workflows/python-package.yml/badge.svg?branch=develop)](https://github.com/UUDigitalHumanitieslab/chamd/actions/workflows/python-package.yml)
```

### Comparing `chamd-0.5.7/setup.py` & `chamd-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.rst') as file:
     long_description = file.read()
 
 setup(
     name='chamd',
     python_requires='>=3.5, <4',
-    version='0.5.7',
+    version='0.5.8',
     description='Conversion and cleaning of CHILDES CHA files into PaQu Plaintext Metadata Format',
     long_description=long_description,
     author='Digital Humanities Lab, Utrecht University',
     author_email='digitalhumanities@uu.nl',
     url='https://github.com/UUDigitalHumanitieslab/chamd',
     license='MIT',
     packages=['chamd'],
```

### Comparing `chamd-0.5.7/chamd/cleanCHILDESMD.py` & `chamd-0.5.8/chamd/cleanCHILDESMD.py`

 * *Files identical despite different names*

### Comparing `chamd-0.5.7/chamd/chat_reader.py` & `chamd-0.5.8/chamd/chat_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -681,16 +681,19 @@
                 else:
                     prev_header = False
 
         try:
             for line in content.splitlines():
                 prevlineno = lineno
                 lineno += 1
-                if line.lstrip()[0] == dependent_tier_char:
-                    line = re.sub(r'^(\s+)?%', '%', line)
+                try:
+                    if line.lstrip()[0] == dependent_tier_char:
+                        line = re.sub(r'^(\s+)?%', '%', line)
+                except IndexError:
+                    pass
                 startchar = line[0:1]
                 if startchar in ['\t', ' ']:
                     linetoprocess = combine(linetoprocess, line)
                     contlinecount += 1
                 elif startchar in [mdchar, uttchar, dependent_tier_char, space]:
                     entrystartno = prevlineno - contlinecount
                     contlinecount = 0
```

### Comparing `chamd-0.5.7/chamd/__main__.py` & `chamd-0.5.8/chamd/__main__.py`

 * *Files identical despite different names*

### Comparing `chamd-0.5.7/README.rst` & `chamd-0.5.8/README.rst`

 * *Files identical despite different names*


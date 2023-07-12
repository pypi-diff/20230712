# Comparing `tmp/phoenixtools-0.0.6.tar.gz` & `tmp/phoenixtools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phoenixtools-0.0.6.tar", last modified: Wed Jun 28 23:09:49 2023, max compression
+gzip compressed data, was "phoenixtools-0.0.7.tar", last modified: Wed Jul 12 00:12:55 2023, max compression
```

## Comparing `phoenixtools-0.0.6.tar` & `phoenixtools-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-28 23:09:49.649887 phoenixtools-0.0.6/
--rw-r--r--   0 runner    (1000) runner    (1000)      453 2023-06-28 23:09:49.649887 phoenixtools-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-28 23:09:49.645887 phoenixtools-0.0.6/phoenixtools/
--rw-r--r--   0 runner    (1000) runner    (1000)     1145 2023-06-28 23:09:00.000000 phoenixtools-0.0.6/phoenixtools/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      234 2023-06-28 23:08:01.000000 phoenixtools-0.0.6/phoenixtools/iptools.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-28 23:09:49.649887 phoenixtools-0.0.6/phoenixtools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      453 2023-06-28 23:09:49.000000 phoenixtools-0.0.6/phoenixtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      201 2023-06-28 23:09:49.000000 phoenixtools-0.0.6/phoenixtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-28 23:09:49.000000 phoenixtools-0.0.6/phoenixtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-06-28 23:09:49.000000 phoenixtools-0.0.6/phoenixtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-28 23:09:49.649887 phoenixtools-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      964 2023-06-28 23:09:25.000000 phoenixtools-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 00:12:55.567905 phoenixtools-0.0.7/
+-rw-r--r--   0 runner    (1000) runner    (1000)      491 2023-07-12 00:12:55.567905 phoenixtools-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 00:12:55.567905 phoenixtools-0.0.7/phoenixtools/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1172 2023-07-12 00:04:12.000000 phoenixtools-0.0.7/phoenixtools/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      203 2023-07-12 00:09:54.000000 phoenixtools-0.0.7/phoenixtools/colors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      234 2023-06-28 23:08:01.000000 phoenixtools-0.0.7/phoenixtools/iptools.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      280 2023-07-12 00:11:34.000000 phoenixtools-0.0.7/phoenixtools/math.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 00:12:55.567905 phoenixtools-0.0.7/phoenixtools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      491 2023-07-12 00:12:55.000000 phoenixtools-0.0.7/phoenixtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      245 2023-07-12 00:12:55.000000 phoenixtools-0.0.7/phoenixtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-12 00:12:55.000000 phoenixtools-0.0.7/phoenixtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-07-12 00:12:55.000000 phoenixtools-0.0.7/phoenixtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-12 00:12:55.567905 phoenixtools-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1002 2023-07-12 00:12:31.000000 phoenixtools-0.0.7/setup.py
```

### Comparing `phoenixtools-0.0.6/phoenixtools/__init__.py` & `phoenixtools-0.0.7/phoenixtools/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .iptools import iptools
+from .colors import colors
 def convertToLetters(number):
     if number==1:
       letter="A"
     elif number==2: 
       letter="B"
     elif number==3: 
       letter="C"
```

### Comparing `phoenixtools-0.0.6/setup.py` & `phoenixtools-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6' 
+VERSION = '0.0.7' 
 DESCRIPTION = 'Easy hacking tools'
-LONG_DESCRIPTION = 'Easy hacking tools used for educational purposes'
+LONG_DESCRIPTION = 'Easy hacking tools used for educational purposes. Update notes: Added math and colors.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="phoenixtools", 
         version=VERSION,
         author="Jack B.",
```


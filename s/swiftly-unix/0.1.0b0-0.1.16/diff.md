# Comparing `tmp/swiftly-unix-0.1.0.beta.tar.gz` & `tmp/swiftly-unix-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.1.0.beta.tar", last modified: Tue Jul 11 22:45:14 2023, max compression
+gzip compressed data, was "swiftly-unix-0.1.16.tar", last modified: Tue Jul 11 22:47:05 2023, max compression
```

## Comparing `swiftly-unix-0.1.0.beta.tar` & `swiftly-unix-0.1.16.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 22:45:14.901395 swiftly-unix-0.1.0.beta/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.0.beta/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       83 2023-07-11 22:45:14.901265 swiftly-unix-0.1.0.beta/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 22:45:14.899068 swiftly-unix-0.1.0.beta/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     5413 2023-07-11 22:43:03.000000 swiftly-unix-0.1.0.beta/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-11 22:45:14.901435 swiftly-unix-0.1.0.beta/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      167 2023-07-11 22:44:22.000000 swiftly-unix-0.1.0.beta/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 22:45:14.900444 swiftly-unix-0.1.0.beta/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.0.beta/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.0.beta/swiftly_unix/config.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.0.beta/swiftly_unix/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3010 2023-07-11 18:42:17.000000 swiftly-unix-0.1.0.beta/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.0.beta/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.0.beta/swiftly_unix/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 22:45:14.901088 swiftly-unix-0.1.0.beta/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       83 2023-07-11 22:45:14.000000 swiftly-unix-0.1.0.beta/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-11 22:45:14.000000 swiftly-unix-0.1.0.beta/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-11 22:45:14.000000 swiftly-unix-0.1.0.beta/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-11 22:45:14.000000 swiftly-unix-0.1.0.beta/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 22:47:05.717960 swiftly-unix-0.1.16/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.16/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-11 22:47:05.717834 swiftly-unix-0.1.16/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 22:47:05.715485 swiftly-unix-0.1.16/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     5413 2023-07-11 22:43:03.000000 swiftly-unix-0.1.16/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-11 22:47:05.717998 swiftly-unix-0.1.16/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-11 22:46:59.000000 swiftly-unix-0.1.16/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 22:47:05.716992 swiftly-unix-0.1.16/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.16/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.16/swiftly_unix/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.16/swiftly_unix/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3010 2023-07-11 18:42:17.000000 swiftly-unix-0.1.16/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.16/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.16/swiftly_unix/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 22:47:05.717668 swiftly-unix-0.1.16/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-11 22:47:05.000000 swiftly-unix-0.1.16/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-11 22:47:05.000000 swiftly-unix-0.1.16/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-11 22:47:05.000000 swiftly-unix-0.1.16/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-11 22:47:05.000000 swiftly-unix-0.1.16/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.1.0.beta/LICENSE` & `swiftly-unix-0.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.0.beta/scripts/swiftly` & `swiftly-unix-0.1.16/scripts/swiftly`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.0.beta/swiftly_unix/gitignore.py` & `swiftly-unix-0.1.16/swiftly_unix/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.0.beta/swiftly_unix/init.py` & `swiftly-unix-0.1.16/swiftly_unix/init.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.0.beta/swiftly_unix/makeapp.py` & `swiftly-unix-0.1.16/swiftly_unix/makeapp.py`

 * *Files identical despite different names*


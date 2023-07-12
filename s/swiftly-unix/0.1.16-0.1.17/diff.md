# Comparing `tmp/swiftly-unix-0.1.16.tar.gz` & `tmp/swiftly-unix-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.1.16.tar", last modified: Tue Jul 11 22:47:05 2023, max compression
+gzip compressed data, was "swiftly-unix-0.1.17.tar", last modified: Wed Jul 12 09:58:52 2023, max compression
```

## Comparing `swiftly-unix-0.1.16.tar` & `swiftly-unix-0.1.17.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 22:47:05.717960 swiftly-unix-0.1.16/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.16/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-11 22:47:05.717834 swiftly-unix-0.1.16/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 22:47:05.715485 swiftly-unix-0.1.16/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     5413 2023-07-11 22:43:03.000000 swiftly-unix-0.1.16/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-11 22:47:05.717998 swiftly-unix-0.1.16/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-11 22:46:59.000000 swiftly-unix-0.1.16/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 22:47:05.716992 swiftly-unix-0.1.16/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.16/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.16/swiftly_unix/config.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.16/swiftly_unix/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3010 2023-07-11 18:42:17.000000 swiftly-unix-0.1.16/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.16/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.16/swiftly_unix/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 22:47:05.717668 swiftly-unix-0.1.16/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-11 22:47:05.000000 swiftly-unix-0.1.16/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-11 22:47:05.000000 swiftly-unix-0.1.16/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-11 22:47:05.000000 swiftly-unix-0.1.16/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-11 22:47:05.000000 swiftly-unix-0.1.16/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 09:58:52.910786 swiftly-unix-0.1.17/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.17/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 09:58:52.910629 swiftly-unix-0.1.17/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 09:58:52.908809 swiftly-unix-0.1.17/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     6830 2023-07-12 09:55:35.000000 swiftly-unix-0.1.17/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 09:58:52.910831 swiftly-unix-0.1.17/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 09:58:16.000000 swiftly-unix-0.1.17/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 09:58:52.909949 swiftly-unix-0.1.17/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.17/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.17/swiftly_unix/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.17/swiftly_unix/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.17/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.17/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.17/swiftly_unix/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 09:58:52.910440 swiftly-unix-0.1.17/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 09:58:52.000000 swiftly-unix-0.1.17/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 09:58:52.000000 swiftly-unix-0.1.17/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 09:58:52.000000 swiftly-unix-0.1.17/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 09:58:52.000000 swiftly-unix-0.1.17/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.1.16/LICENSE` & `swiftly-unix-0.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.16/swiftly_unix/gitignore.py` & `swiftly-unix-0.1.17/swiftly_unix/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.16/swiftly_unix/init.py` & `swiftly-unix-0.1.17/swiftly_unix/init.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,14 +57,22 @@
 
 def is_repo(name):
     repo_markers = ["https://", "http://", ".git", "git@"]
     
     repo_check = [marker in name for marker in repo_markers]
     return True in repo_check
 
+def clone_successful(git_clone):
+    if "ERROR:" in git_clone or "fatal:" in git_clone:
+        lines = git_clone.split('=')
+        error_lines = [line for line in lines if line.startswith(("ERROR:", "fatal:"))]
+        return ' '.join(error_lines)
+    else:
+        return True
+
 def initialise(name, in_place=False):
     if is_repo(name):
         name = name.split('/')[-1].replace('.git', '')
 
     if not os.path.exists(name):
         os.makedirs(name)
```

### Comparing `swiftly-unix-0.1.16/swiftly_unix/makeapp.py` & `swiftly-unix-0.1.17/swiftly_unix/makeapp.py`

 * *Files identical despite different names*


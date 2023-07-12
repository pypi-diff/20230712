# Comparing `tmp/swiftly-unix-0.1.26.tar.gz` & `tmp/swiftly-unix-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.1.26.tar", last modified: Wed Jul 12 12:10:26 2023, max compression
+gzip compressed data, was "swiftly-unix-0.1.27.tar", last modified: Wed Jul 12 12:20:33 2023, max compression
```

## Comparing `swiftly-unix-0.1.26.tar` & `swiftly-unix-0.1.27.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:10:26.089573 swiftly-unix-0.1.26/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.26/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 12:10:26.089430 swiftly-unix-0.1.26/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:10:26.087832 swiftly-unix-0.1.26/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     6902 2023-07-12 12:09:18.000000 swiftly-unix-0.1.26/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 12:10:26.092047 swiftly-unix-0.1.26/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 12:10:14.000000 swiftly-unix-0.1.26/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:10:26.088709 swiftly-unix-0.1.26/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.26/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.26/swiftly_unix/config.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.26/swiftly_unix/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.26/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.26/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.26/swiftly_unix/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:10:26.089260 swiftly-unix-0.1.26/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 12:10:26.000000 swiftly-unix-0.1.26/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 12:10:26.000000 swiftly-unix-0.1.26/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 12:10:26.000000 swiftly-unix-0.1.26/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 12:10:26.000000 swiftly-unix-0.1.26/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:20:33.576922 swiftly-unix-0.1.27/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.27/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 12:20:33.576786 swiftly-unix-0.1.27/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:20:33.575252 swiftly-unix-0.1.27/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     6904 2023-07-12 12:17:41.000000 swiftly-unix-0.1.27/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 12:20:33.576960 swiftly-unix-0.1.27/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 12:20:31.000000 swiftly-unix-0.1.27/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:20:33.576164 swiftly-unix-0.1.27/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.27/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.27/swiftly_unix/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.27/swiftly_unix/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.27/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.27/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.27/swiftly_unix/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:20:33.576627 swiftly-unix-0.1.27/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 12:20:33.000000 swiftly-unix-0.1.27/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 12:20:33.000000 swiftly-unix-0.1.27/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 12:20:33.000000 swiftly-unix-0.1.27/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 12:20:33.000000 swiftly-unix-0.1.27/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.1.26/LICENSE` & `swiftly-unix-0.1.27/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.26/scripts/swiftly` & `swiftly-unix-0.1.27/scripts/swiftly`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
     echo "✨ Project '$PROJECT_NAME' initiated successfully :)"
 }
 
 
 function makeapp(){
     python -c "from swiftly_unix.makeapp import makeapp; makeapp('$1', '$PROJECT_VENV_LOCATION')"
     sleep 1
-    printf "\033[0;32m✓\033[0m %s\n" "App ${1} created successfully"
+    printf "\033[0;32m✓\033[0m %s\n" "App '${1}' created successfully"
 }
 
 function run(){
     path=$(python -c "from swiftly_unix.runapp import run_app; print(run_app('$1', '$PROJECT_NAME'))")
     python -m $path
 }
```

### Comparing `swiftly-unix-0.1.26/swiftly_unix/gitignore.py` & `swiftly-unix-0.1.27/swiftly_unix/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.26/swiftly_unix/init.py` & `swiftly-unix-0.1.27/swiftly_unix/init.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.26/swiftly_unix/makeapp.py` & `swiftly-unix-0.1.27/swiftly_unix/makeapp.py`

 * *Files identical despite different names*


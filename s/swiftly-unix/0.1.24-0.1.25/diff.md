# Comparing `tmp/swiftly-unix-0.1.24.tar.gz` & `tmp/swiftly-unix-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.1.24.tar", last modified: Wed Jul 12 11:22:54 2023, max compression
+gzip compressed data, was "swiftly-unix-0.1.25.tar", last modified: Wed Jul 12 11:30:55 2023, max compression
```

## Comparing `swiftly-unix-0.1.24.tar` & `swiftly-unix-0.1.25.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:22:54.059722 swiftly-unix-0.1.24/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.24/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 11:22:54.059575 swiftly-unix-0.1.24/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:22:54.057723 swiftly-unix-0.1.24/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     6990 2023-07-12 11:22:36.000000 swiftly-unix-0.1.24/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 11:22:54.059785 swiftly-unix-0.1.24/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 11:22:41.000000 swiftly-unix-0.1.24/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:22:54.058724 swiftly-unix-0.1.24/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.24/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.24/swiftly_unix/config.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.24/swiftly_unix/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.24/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.24/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.24/swiftly_unix/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:22:54.059368 swiftly-unix-0.1.24/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 11:22:53.000000 swiftly-unix-0.1.24/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 11:22:54.000000 swiftly-unix-0.1.24/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 11:22:53.000000 swiftly-unix-0.1.24/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 11:22:53.000000 swiftly-unix-0.1.24/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:30:55.389541 swiftly-unix-0.1.25/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.25/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 11:30:55.389403 swiftly-unix-0.1.25/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:30:55.387958 swiftly-unix-0.1.25/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     6902 2023-07-12 11:30:24.000000 swiftly-unix-0.1.25/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 11:30:55.389578 swiftly-unix-0.1.25/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 11:30:37.000000 swiftly-unix-0.1.25/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:30:55.388786 swiftly-unix-0.1.25/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.25/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.25/swiftly_unix/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.25/swiftly_unix/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.25/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.25/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.25/swiftly_unix/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:30:55.389234 swiftly-unix-0.1.25/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 11:30:55.000000 swiftly-unix-0.1.25/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 11:30:55.000000 swiftly-unix-0.1.25/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 11:30:55.000000 swiftly-unix-0.1.25/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 11:30:55.000000 swiftly-unix-0.1.25/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.1.24/LICENSE` & `swiftly-unix-0.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.24/scripts/swiftly` & `swiftly-unix-0.1.25/scripts/swiftly`

 * *Files 4% similar despite different names*

```diff
@@ -219,19 +219,14 @@
 
 function push(){
     git add *
     git commit -m "$*"
     git push
 }
 
-function close(){
-    deactivate
-    cd ..
-}
-
 if [ "$1" = "init" ]
 then
     init $2
 elif [ "$1" = "makeapp" ]
 then
     makeapp $2
 elif [ "$1" = "run" ]
@@ -242,11 +237,8 @@
     install $2
 elif [ "$1" = "uninstall" ]
 then
     uninstall $2
 elif [ "$1" = "push" ]
 then
     push $2
-elif [ "$1" = "close" ]
-then
-    close $2
 fi
```

### Comparing `swiftly-unix-0.1.24/swiftly_unix/gitignore.py` & `swiftly-unix-0.1.25/swiftly_unix/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.24/swiftly_unix/init.py` & `swiftly-unix-0.1.25/swiftly_unix/init.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.24/swiftly_unix/makeapp.py` & `swiftly-unix-0.1.25/swiftly_unix/makeapp.py`

 * *Files identical despite different names*


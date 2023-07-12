# Comparing `tmp/swiftly-unix-0.1.21.tar.gz` & `tmp/swiftly-unix-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.1.21.tar", last modified: Wed Jul 12 11:03:28 2023, max compression
+gzip compressed data, was "swiftly-unix-0.1.22.tar", last modified: Wed Jul 12 11:09:49 2023, max compression
```

## Comparing `swiftly-unix-0.1.21.tar` & `swiftly-unix-0.1.22.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:03:28.180002 swiftly-unix-0.1.21/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.21/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 11:03:28.179870 swiftly-unix-0.1.21/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:03:28.178472 swiftly-unix-0.1.21/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     6900 2023-07-12 11:02:45.000000 swiftly-unix-0.1.21/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 11:03:28.180039 swiftly-unix-0.1.21/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 11:03:18.000000 swiftly-unix-0.1.21/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:03:28.179258 swiftly-unix-0.1.21/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.21/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.21/swiftly_unix/config.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.21/swiftly_unix/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.21/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.21/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.21/swiftly_unix/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:03:28.179715 swiftly-unix-0.1.21/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 11:03:28.000000 swiftly-unix-0.1.21/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 11:03:28.000000 swiftly-unix-0.1.21/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 11:03:28.000000 swiftly-unix-0.1.21/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 11:03:28.000000 swiftly-unix-0.1.21/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:09:49.981036 swiftly-unix-0.1.22/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.22/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 11:09:49.980888 swiftly-unix-0.1.22/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:09:49.979128 swiftly-unix-0.1.22/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     6902 2023-07-12 11:09:36.000000 swiftly-unix-0.1.22/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 11:09:49.981080 swiftly-unix-0.1.22/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 11:09:39.000000 swiftly-unix-0.1.22/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:09:49.980166 swiftly-unix-0.1.22/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.22/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.22/swiftly_unix/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.22/swiftly_unix/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.22/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.22/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.22/swiftly_unix/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:09:49.980703 swiftly-unix-0.1.22/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 11:09:49.000000 swiftly-unix-0.1.22/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 11:09:49.000000 swiftly-unix-0.1.22/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 11:09:49.000000 swiftly-unix-0.1.22/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 11:09:49.000000 swiftly-unix-0.1.22/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.1.21/LICENSE` & `swiftly-unix-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.21/scripts/swiftly` & `swiftly-unix-0.1.22/scripts/swiftly`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
     updated_packages=$(pip freeze)
     requirements_path=$PROJECT_VENV_LOCATION/../requirements.txt
     echo "$updated_packages" > $requirements_path
 }
 
 function push(){
     git add *
-    git commit -m $@
+    git commit -m "$@"
     git push
 }
 
 if [ "$1" = "init" ]
 then
     init $2
 elif [ "$1" = "makeapp" ]
```

### Comparing `swiftly-unix-0.1.21/swiftly_unix/gitignore.py` & `swiftly-unix-0.1.22/swiftly_unix/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.21/swiftly_unix/init.py` & `swiftly-unix-0.1.22/swiftly_unix/init.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.21/swiftly_unix/makeapp.py` & `swiftly-unix-0.1.22/swiftly_unix/makeapp.py`

 * *Files identical despite different names*


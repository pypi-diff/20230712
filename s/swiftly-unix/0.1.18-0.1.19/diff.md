# Comparing `tmp/swiftly-unix-0.1.18.tar.gz` & `tmp/swiftly-unix-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.1.18.tar", last modified: Wed Jul 12 10:03:44 2023, max compression
+gzip compressed data, was "swiftly-unix-0.1.19.tar", last modified: Wed Jul 12 10:05:42 2023, max compression
```

## Comparing `swiftly-unix-0.1.18.tar` & `swiftly-unix-0.1.19.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:03:44.062492 swiftly-unix-0.1.18/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.18/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 10:03:44.062147 swiftly-unix-0.1.18/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:03:44.056207 swiftly-unix-0.1.18/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     6891 2023-07-12 10:03:05.000000 swiftly-unix-0.1.18/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 10:03:44.062558 swiftly-unix-0.1.18/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 10:03:29.000000 swiftly-unix-0.1.18/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:03:44.059394 swiftly-unix-0.1.18/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.18/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.18/swiftly_unix/config.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.18/swiftly_unix/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.18/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.18/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.18/swiftly_unix/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:03:44.061716 swiftly-unix-0.1.18/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 10:03:43.000000 swiftly-unix-0.1.18/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 10:03:43.000000 swiftly-unix-0.1.18/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 10:03:43.000000 swiftly-unix-0.1.18/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 10:03:43.000000 swiftly-unix-0.1.18/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:05:42.433156 swiftly-unix-0.1.19/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.19/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 10:05:42.433017 swiftly-unix-0.1.19/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:05:42.431312 swiftly-unix-0.1.19/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     6888 2023-07-12 10:05:18.000000 swiftly-unix-0.1.19/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 10:05:42.433194 swiftly-unix-0.1.19/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 10:05:28.000000 swiftly-unix-0.1.19/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:05:42.432342 swiftly-unix-0.1.19/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.19/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.19/swiftly_unix/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.19/swiftly_unix/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.19/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.19/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.19/swiftly_unix/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:05:42.432852 swiftly-unix-0.1.19/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 10:05:42.000000 swiftly-unix-0.1.19/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 10:05:42.000000 swiftly-unix-0.1.19/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 10:05:42.000000 swiftly-unix-0.1.19/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 10:05:42.000000 swiftly-unix-0.1.19/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.1.18/LICENSE` & `swiftly-unix-0.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.18/scripts/swiftly` & `swiftly-unix-0.1.19/scripts/swiftly`

 * *Files 0% similar despite different names*

```diff
@@ -234,12 +234,11 @@
     run $2
 elif [ "$1" = "install" ]
 then
     install $2
 elif [ "$1" = "uninstall" ]
 then
     uninstall $2
-fi
 elif [ "$1" = "push" ]
 then
     push $2
 fi
```

### Comparing `swiftly-unix-0.1.18/swiftly_unix/gitignore.py` & `swiftly-unix-0.1.19/swiftly_unix/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.18/swiftly_unix/init.py` & `swiftly-unix-0.1.19/swiftly_unix/init.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.18/swiftly_unix/makeapp.py` & `swiftly-unix-0.1.19/swiftly_unix/makeapp.py`

 * *Files identical despite different names*


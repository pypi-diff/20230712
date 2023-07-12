# Comparing `tmp/swiftly-unix-0.1.20.tar.gz` & `tmp/swiftly-unix-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.1.20.tar", last modified: Wed Jul 12 10:48:35 2023, max compression
+gzip compressed data, was "swiftly-unix-0.1.21.tar", last modified: Wed Jul 12 11:03:28 2023, max compression
```

## Comparing `swiftly-unix-0.1.20.tar` & `swiftly-unix-0.1.21.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:48:35.498364 swiftly-unix-0.1.20/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.20/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 10:48:35.498235 swiftly-unix-0.1.20/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:48:35.496904 swiftly-unix-0.1.20/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     6900 2023-07-12 10:45:59.000000 swiftly-unix-0.1.20/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 10:48:35.498398 swiftly-unix-0.1.20/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 10:48:24.000000 swiftly-unix-0.1.20/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:48:35.497653 swiftly-unix-0.1.20/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.20/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.20/swiftly_unix/config.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.20/swiftly_unix/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.20/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.20/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.20/swiftly_unix/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:48:35.498089 swiftly-unix-0.1.20/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 10:48:35.000000 swiftly-unix-0.1.20/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 10:48:35.000000 swiftly-unix-0.1.20/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 10:48:35.000000 swiftly-unix-0.1.20/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 10:48:35.000000 swiftly-unix-0.1.20/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:03:28.180002 swiftly-unix-0.1.21/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.21/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 11:03:28.179870 swiftly-unix-0.1.21/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:03:28.178472 swiftly-unix-0.1.21/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     6900 2023-07-12 11:02:45.000000 swiftly-unix-0.1.21/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 11:03:28.180039 swiftly-unix-0.1.21/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 11:03:18.000000 swiftly-unix-0.1.21/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:03:28.179258 swiftly-unix-0.1.21/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.21/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.21/swiftly_unix/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.21/swiftly_unix/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.21/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.21/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.21/swiftly_unix/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:03:28.179715 swiftly-unix-0.1.21/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 11:03:28.000000 swiftly-unix-0.1.21/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 11:03:28.000000 swiftly-unix-0.1.21/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 11:03:28.000000 swiftly-unix-0.1.21/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 11:03:28.000000 swiftly-unix-0.1.21/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.1.20/LICENSE` & `swiftly-unix-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.20/scripts/swiftly` & `swiftly-unix-0.1.21/scripts/swiftly`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -102,27 +102,27 @@
             git pull > /dev/null
             spin_stop "Pulled remote changes"
 
         else
             spin_stop "Codebase up-to-date"
         fi
 
+        spin_start "Checking your project"
+        project_name=$(python -c 'from swiftly_unix.init import get_project_name; print(get_project_name())')
+        export PROJECT_NAME=$project_name
+        spin_stop "Project '$PROJECT_NAME' ready"
+
         spin_start "Activating virtual environment"
         venv_location=$(python -c 'from swiftly_unix.init import get_venv_location; print(get_venv_location())')
         source $venv_location/bin/activate
         export PROJECT_VENV_LOCATION=$venv_location
 
         pip install swiftly-unix --upgrade > /dev/null 2>&1
         spin_stop "Activated virtual environment"
 
-        spin_start "Checking your project"
-        project_name=$(python -c 'from swiftly_unix.init import get_project_name; print(get_project_name())')
-        export PROJECT_NAME=$project_name
-        spin_stop "Project '$PROJECT_NAME' ready"
-
         spin_start "Checking for new packages"
         available_packages=$(pip freeze | tr '\n' ' ')
         new_packages=$(python -c "from swiftly_unix.init import check_new_packages; print(check_new_packages('$available_packages'))")
 
         if [ "$new_packages" = "True" ]
         then
             pip install -r requirements.txt > /dev/null
```

### Comparing `swiftly-unix-0.1.20/swiftly_unix/gitignore.py` & `swiftly-unix-0.1.21/swiftly_unix/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.20/swiftly_unix/init.py` & `swiftly-unix-0.1.21/swiftly_unix/init.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.20/swiftly_unix/makeapp.py` & `swiftly-unix-0.1.21/swiftly_unix/makeapp.py`

 * *Files identical despite different names*


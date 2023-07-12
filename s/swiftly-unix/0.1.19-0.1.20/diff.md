# Comparing `tmp/swiftly-unix-0.1.19.tar.gz` & `tmp/swiftly-unix-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.1.19.tar", last modified: Wed Jul 12 10:05:42 2023, max compression
+gzip compressed data, was "swiftly-unix-0.1.20.tar", last modified: Wed Jul 12 10:48:35 2023, max compression
```

## Comparing `swiftly-unix-0.1.19.tar` & `swiftly-unix-0.1.20.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:05:42.433156 swiftly-unix-0.1.19/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.19/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 10:05:42.433017 swiftly-unix-0.1.19/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:05:42.431312 swiftly-unix-0.1.19/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     6888 2023-07-12 10:05:18.000000 swiftly-unix-0.1.19/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 10:05:42.433194 swiftly-unix-0.1.19/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 10:05:28.000000 swiftly-unix-0.1.19/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:05:42.432342 swiftly-unix-0.1.19/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.19/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.19/swiftly_unix/config.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.19/swiftly_unix/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.19/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.19/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.19/swiftly_unix/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:05:42.432852 swiftly-unix-0.1.19/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 10:05:42.000000 swiftly-unix-0.1.19/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 10:05:42.000000 swiftly-unix-0.1.19/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 10:05:42.000000 swiftly-unix-0.1.19/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 10:05:42.000000 swiftly-unix-0.1.19/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:48:35.498364 swiftly-unix-0.1.20/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.20/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 10:48:35.498235 swiftly-unix-0.1.20/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:48:35.496904 swiftly-unix-0.1.20/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     6900 2023-07-12 10:45:59.000000 swiftly-unix-0.1.20/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 10:48:35.498398 swiftly-unix-0.1.20/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 10:48:24.000000 swiftly-unix-0.1.20/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:48:35.497653 swiftly-unix-0.1.20/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.20/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.20/swiftly_unix/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.20/swiftly_unix/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.20/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.20/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.20/swiftly_unix/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 10:48:35.498089 swiftly-unix-0.1.20/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 10:48:35.000000 swiftly-unix-0.1.20/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 10:48:35.000000 swiftly-unix-0.1.20/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 10:48:35.000000 swiftly-unix-0.1.20/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 10:48:35.000000 swiftly-unix-0.1.20/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.1.19/LICENSE` & `swiftly-unix-0.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.19/scripts/swiftly` & `swiftly-unix-0.1.20/scripts/swiftly`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 # Define the stop spinner function
 spin_stop() {
     local msg="$1"
     local operation_status="${2:-success}"
 
     # Only try to kill the process if it's still running
     if kill -0 "${SPIN_JOB}" 2>/dev/null; then
-        kill -9 "${SPIN_JOB}"
+        kill -9 "${SPIN_JOB}" > /dev/null 2>&1
     fi
 
     # Clear the final spinner character and message
     printf " \r"
 
     # Clear the line
     tput el
@@ -58,14 +58,15 @@
     if [ "$operation_status" = "fail" ]; then
         printf "\033[0;31m✗\033[0m %s\n" "${msg}"
     else
         printf "\033[0;32m✓\033[0m %s\n" "${msg}"
     fi
 }
 
+
 # Define a function to handle the SIGINT signal
 handle_sigint() {
     # Stop the spinner
     spin_stop "Interrupted" "fail"
 
     # If the script is being sourced, return from the script
     # Otherwise, exit the script
@@ -188,18 +189,17 @@
     fi
 
     echo "✨ Project '$PROJECT_NAME' initiated successfully :)"
 }
 
 
 function makeapp(){
-    spin_start "Creating app $1"
     python -c "from swiftly_unix.makeapp import makeapp; makeapp('$1', '$PROJECT_VENV_LOCATION')"
     sleep 1
-    spin_stop "App $1 created successfully"
+    printf "\033[0;32m✓\033[0m %s\n" "App ${1} created successfully"
 }
 
 function run(){
     path=$(python -c "from swiftly_unix.runapp import run_app; print(run_app('$1', '$PROJECT_NAME'))")
     python -m $path
 }
```

### Comparing `swiftly-unix-0.1.19/swiftly_unix/gitignore.py` & `swiftly-unix-0.1.20/swiftly_unix/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.19/swiftly_unix/init.py` & `swiftly-unix-0.1.20/swiftly_unix/init.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.19/swiftly_unix/makeapp.py` & `swiftly-unix-0.1.20/swiftly_unix/makeapp.py`

 * *Files identical despite different names*


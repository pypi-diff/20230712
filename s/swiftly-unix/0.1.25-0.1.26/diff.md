# Comparing `tmp/swiftly-unix-0.1.25.tar.gz` & `tmp/swiftly-unix-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.1.25.tar", last modified: Wed Jul 12 11:30:55 2023, max compression
+gzip compressed data, was "swiftly-unix-0.1.26.tar", last modified: Wed Jul 12 12:10:26 2023, max compression
```

## Comparing `swiftly-unix-0.1.25.tar` & `swiftly-unix-0.1.26.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:30:55.389541 swiftly-unix-0.1.25/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.25/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 11:30:55.389403 swiftly-unix-0.1.25/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:30:55.387958 swiftly-unix-0.1.25/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     6902 2023-07-12 11:30:24.000000 swiftly-unix-0.1.25/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 11:30:55.389578 swiftly-unix-0.1.25/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 11:30:37.000000 swiftly-unix-0.1.25/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:30:55.388786 swiftly-unix-0.1.25/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.25/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.25/swiftly_unix/config.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.25/swiftly_unix/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.25/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.25/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.25/swiftly_unix/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 11:30:55.389234 swiftly-unix-0.1.25/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 11:30:55.000000 swiftly-unix-0.1.25/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 11:30:55.000000 swiftly-unix-0.1.25/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 11:30:55.000000 swiftly-unix-0.1.25/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 11:30:55.000000 swiftly-unix-0.1.25/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:10:26.089573 swiftly-unix-0.1.26/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.26/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 12:10:26.089430 swiftly-unix-0.1.26/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:10:26.087832 swiftly-unix-0.1.26/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     6902 2023-07-12 12:09:18.000000 swiftly-unix-0.1.26/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 12:10:26.092047 swiftly-unix-0.1.26/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 12:10:14.000000 swiftly-unix-0.1.26/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:10:26.088709 swiftly-unix-0.1.26/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.26/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.26/swiftly_unix/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.26/swiftly_unix/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.26/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.26/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.26/swiftly_unix/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:10:26.089260 swiftly-unix-0.1.26/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 12:10:26.000000 swiftly-unix-0.1.26/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 12:10:26.000000 swiftly-unix-0.1.26/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 12:10:26.000000 swiftly-unix-0.1.26/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 12:10:26.000000 swiftly-unix-0.1.26/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.1.25/LICENSE` & `swiftly-unix-0.1.26/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.25/scripts/swiftly` & `swiftly-unix-0.1.26/scripts/swiftly`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
         git_status=$(git status -uno | tr '\n' ' ' | sed 's/"/\\"/g')
 
         pull_changes=$(python -c 'from swiftly_unix.init import pull_changes; print(pull_changes("'$git_status'"))')
         if [ "$pull_changes" = "True" ]
         then
             git pull > /dev/null
-            spin_stop "Pulled remote changes"
+            spin_stop "Remote changes pulled"
 
         else
             spin_stop "Codebase up-to-date"
         fi
 
         spin_start "Checking your project"
         project_name=$(python -c 'from swiftly_unix.init import get_project_name; print(get_project_name())')
@@ -113,46 +113,46 @@
 
         spin_start "Activating virtual environment"
         venv_location=$(python -c 'from swiftly_unix.init import get_venv_location; print(get_venv_location())')
         source $venv_location/bin/activate
         export PROJECT_VENV_LOCATION=$venv_location
 
         pip install swiftly-unix --upgrade > /dev/null 2>&1
-        spin_stop "Activated virtual environment"
+        spin_stop "Virtual environment activated"
 
         spin_start "Checking for new packages"
         available_packages=$(pip freeze | tr '\n' ' ')
         new_packages=$(python -c "from swiftly_unix.init import check_new_packages; print(check_new_packages('$available_packages'))")
 
         if [ "$new_packages" = "True" ]
         then
             pip install -r requirements.txt > /dev/null
-            spin_stop "Installed new packages"
+            spin_stop "New packages installed"
         else
             spin_stop "All packages already installed"
         fi
 
         spin_start "Checking swiftly"
         pip install --upgrade pip > /dev/null 2>&1
 
         install swiftly-unix --upgrade > /dev/null 2>&1
-        spin_stop "All checks swiftly completed"
+        spin_stop "All checks completed swiftly"
 
     else
         is_github_repo=$(python -c "from swiftly_unix.init import is_repo; print(is_repo('$1'))")
         if [ "$is_github_repo" = "True" ]
         then
             spin_start "Cloning git repository"
             git_clone=$(git clone $1 2>&1 | tr '\n' '=' | sed 's/"/\\"/g')
 
             clone_successful=$(python -c 'from swiftly_unix.init import clone_successful; print(clone_successful("'$git_clone'"))')
 
             if [ "$clone_successful" = "True" ]
             then
-                spin_stop "Cloned git repository"
+                spin_stop "Git repository cloned"
             else
                 spin_stop "$clone_successful" "fail"
                 echo "Do you want to create a new project? (y/n)"
                 read user_input
                 user_input=$(echo "$user_input" | tr '[:upper:]' '[:lower:]' | cut -c 1)
                 if [ "$user_input" != "y" ]
                 then
@@ -177,19 +177,19 @@
 
         spin_stop "Project '$PROJECT_NAME' ready"
 
         spin_start "Installing requirements"
         pip install --upgrade pip > /dev/null 2>&1
 
         pip install -r requirements.txt > /dev/null
-        spin_stop "Installed requirements"
+        spin_stop "Requirements installed"
 
         spin_start "Checking swiftly"
         install swiftly-unix --upgrade > /dev/null 2>&1
-        spin_stop "All checks swiftly completed"
+        spin_stop "All checks completed swiftly"
     fi
 
     echo "✨ Project '$PROJECT_NAME' initiated successfully :)"
 }
 
 
 function makeapp(){
```

### Comparing `swiftly-unix-0.1.25/swiftly_unix/gitignore.py` & `swiftly-unix-0.1.26/swiftly_unix/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.25/swiftly_unix/init.py` & `swiftly-unix-0.1.26/swiftly_unix/init.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.25/swiftly_unix/makeapp.py` & `swiftly-unix-0.1.26/swiftly_unix/makeapp.py`

 * *Files identical despite different names*


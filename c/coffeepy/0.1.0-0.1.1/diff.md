# Comparing `tmp/coffeepy-0.1.0.tar.gz` & `tmp/coffeepy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffeepy-0.1.0.tar", last modified: Tue Jul 11 23:43:55 2023, max compression
+gzip compressed data, was "coffeepy-0.1.1.tar", last modified: Wed Jul 12 17:21:58 2023, max compression
```

## Comparing `coffeepy-0.1.0.tar` & `coffeepy-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 jukka      (501) staff       (20)        0 2023-07-11 23:43:55.430134 coffeepy-0.1.0/
--rw-r--r--   0 jukka      (501) staff       (20)     1069 2023-07-11 23:22:38.000000 coffeepy-0.1.0/LICENSE
--rw-r--r--   0 jukka      (501) staff       (20)     1009 2023-07-11 23:43:55.429781 coffeepy-0.1.0/PKG-INFO
--rw-r--r--   0 jukka      (501) staff       (20)      488 2023-07-11 23:32:30.000000 coffeepy-0.1.0/README.md
-drwxr-xr-x   0 jukka      (501) staff       (20)        0 2023-07-11 23:43:55.427182 coffeepy-0.1.0/coffeepy/
--rw-r--r--   0 jukka      (501) staff       (20)        0 2023-07-11 23:22:38.000000 coffeepy-0.1.0/coffeepy/__init__.py
--rw-r--r--   0 jukka      (501) staff       (20)     2643 2023-07-11 23:23:29.000000 coffeepy-0.1.0/coffeepy/main.py
-drwxr-xr-x   0 jukka      (501) staff       (20)        0 2023-07-11 23:43:55.429315 coffeepy-0.1.0/coffeepy.egg-info/
--rw-r--r--   0 jukka      (501) staff       (20)     1009 2023-07-11 23:43:55.000000 coffeepy-0.1.0/coffeepy.egg-info/PKG-INFO
--rw-r--r--   0 jukka      (501) staff       (20)      233 2023-07-11 23:43:55.000000 coffeepy-0.1.0/coffeepy.egg-info/SOURCES.txt
--rw-r--r--   0 jukka      (501) staff       (20)        1 2023-07-11 23:43:55.000000 coffeepy-0.1.0/coffeepy.egg-info/dependency_links.txt
--rw-r--r--   0 jukka      (501) staff       (20)       48 2023-07-11 23:43:55.000000 coffeepy-0.1.0/coffeepy.egg-info/entry_points.txt
--rw-r--r--   0 jukka      (501) staff       (20)        9 2023-07-11 23:43:55.000000 coffeepy-0.1.0/coffeepy.egg-info/top_level.txt
--rw-r--r--   0 jukka      (501) staff       (20)      648 2023-07-11 23:24:08.000000 coffeepy-0.1.0/pyproject.toml
--rw-r--r--   0 jukka      (501) staff       (20)       38 2023-07-11 23:43:55.430229 coffeepy-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:21:58.306758 coffeepy-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 17:21:44.000000 coffeepy-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-12 17:21:58.306758 coffeepy-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-12 17:21:44.000000 coffeepy-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-12 17:21:44.000000 coffeepy-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:21:58.306758 coffeepy-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:21:58.306758 coffeepy-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:21:58.306758 coffeepy-0.1.1/src/coffeepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 17:21:44.000000 coffeepy-0.1.1/src/coffeepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-12 17:21:44.000000 coffeepy-0.1.1/src/coffeepy/coffeepy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:21:58.306758 coffeepy-0.1.1/src/coffeepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-12 17:21:58.000000 coffeepy-0.1.1/src/coffeepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-12 17:21:58.000000 coffeepy-0.1.1/src/coffeepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:21:58.000000 coffeepy-0.1.1/src/coffeepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 17:21:58.000000 coffeepy-0.1.1/src/coffeepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 17:21:58.000000 coffeepy-0.1.1/src/coffeepy.egg-info/top_level.txt
```

### Comparing `coffeepy-0.1.0/LICENSE` & `coffeepy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coffeepy-0.1.0/PKG-INFO` & `coffeepy-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.0
-Summary: Coffee prevents the system from sleeping
-Author-email: Jukka Maatta <kuvaus@users.noreply.github.com>
+Version: 0.1.1
+Summary: Coffeepy prevents the system from sleeping
+Author-email: kuvaus <kuvaus@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# coffeepy
+# Coffeepy
 
-Coffeepy ☕️ prevents the system from sleeping.
+Coffeepy ☕️ is a small program that prevents the system from sleeping.
+Works on MacOS, Windows and Linux.
+
+<img alt="coffeepy" src="https://github.com/kuvaus/coffeepy/assets/22169537/d2954958-4c92-4791-92b9-36e46f448abc.gif" width="600" />
 
 ## Installation
 
 ```sh
-pip install coffeepy
+pip install -U coffeepy
 ```
 
 ## Usage
 
 Simply run the program from command line
 ```sh
 coffeepy
@@ -33,13 +36,23 @@
 
 Optional: You can set the time in minutes with `-t` flag. To run the program for 1 hour, use
 
 ```sh
 coffeepy -t 60
 ```
 
+## Python module
+
+You can also import coffeepy as a python module
+
+```python
+import coffeepy
+
+coffeepy.run()
+```
+
 
 ## License
 
 This project is licensed under the MIT [License](https://github.com/kuvaus/coffeepy/blob/main/LICENSE)
```

### Comparing `coffeepy-0.1.0/coffeepy/main.py` & `coffeepy-0.1.1/src/coffeepy/coffeepy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+
+from importlib.metadata import version
+
 import ctypes
 import sys
 import subprocess
 import time
 import argparse
 
 
@@ -11,30 +14,30 @@
     "  ☕️   ",
     "  ☕️☁️  ",
     " ☁️☕️   ",
     "  ☕️   ",
 ]
 
 
-def display_animation(animation):
+def display_animation(animation=animation):
     for frame in animation:
         print('\r' + frame, end='')
         time.sleep(0.5)  # Adjust the delay time as desired
 
 
 def check_caffeinate():
     try:
         subprocess.check_output(['which', 'caffeinate'])
         return True
     except subprocess.CalledProcessError:
         return False
 
 
-def main():
-    parser = argparse.ArgumentParser(description='Coffeepy ☕️ prevents the system from sleeping.\n'
+def run():
+    parser = argparse.ArgumentParser(description='Coffeepy (v'+version('coffeepy')+') ☕️ prevents the system from sleeping.\n'
                                                  'You can set the time with -t flag\n'
                                                  'Made by kuvaus',
                                                  formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument('-t', '--time', type=int, default=0, help='Optional: Duration of animation in minutes. Use 0 for indefinite duration')
     args = parser.parse_args()
 
@@ -62,15 +65,15 @@
         ctypes.windll.kernel32.SetThreadExecutionState(0x80000002)
 
     print('Press Ctrl-C to quit')
     
     try:
         start_time = time.time()
         while time.time() - start_time < duration or duration == float('inf'):
-            display_animation(animation)
+            display_animation()
     except KeyboardInterrupt:
         print('\nExiting')
 
     finally:
         if proc:
             proc.terminate()
         if 'linux' in sys.platform and not check_caffeinate():
@@ -79,8 +82,8 @@
             subprocess.Popen(['xset', '+dpms'])
         if 'win32' in sys.platform:
             ctypes.windll.kernel32.SetThreadExecutionState(0x80000000)
         sys.exit()
 
 
 if __name__ == "__main__":
-    main()
+    run()
```

### Comparing `coffeepy-0.1.0/coffeepy.egg-info/PKG-INFO` & `coffeepy-0.1.1/src/coffeepy.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.0
-Summary: Coffee prevents the system from sleeping
-Author-email: Jukka Maatta <kuvaus@users.noreply.github.com>
+Version: 0.1.1
+Summary: Coffeepy prevents the system from sleeping
+Author-email: kuvaus <kuvaus@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# coffeepy
+# Coffeepy
 
-Coffeepy ☕️ prevents the system from sleeping.
+Coffeepy ☕️ is a small program that prevents the system from sleeping.
+Works on MacOS, Windows and Linux.
+
+<img alt="coffeepy" src="https://github.com/kuvaus/coffeepy/assets/22169537/d2954958-4c92-4791-92b9-36e46f448abc.gif" width="600" />
 
 ## Installation
 
 ```sh
-pip install coffeepy
+pip install -U coffeepy
 ```
 
 ## Usage
 
 Simply run the program from command line
 ```sh
 coffeepy
@@ -33,13 +36,23 @@
 
 Optional: You can set the time in minutes with `-t` flag. To run the program for 1 hour, use
 
 ```sh
 coffeepy -t 60
 ```
 
+## Python module
+
+You can also import coffeepy as a python module
+
+```python
+import coffeepy
+
+coffeepy.run()
+```
+
 
 ## License
 
 This project is licensed under the MIT [License](https://github.com/kuvaus/coffeepy/blob/main/LICENSE)
```

### Comparing `coffeepy-0.1.0/pyproject.toml` & `coffeepy-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coffeepy"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
-  { name="Jukka Maatta", email="kuvaus@users.noreply.github.com" },
+  { name="kuvaus", email="kuvaus@users.noreply.github.com" },
 ]
-description = "Coffee prevents the system from sleeping"
+description = "Coffeepy prevents the system from sleeping"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
-coffeepy = "coffeepy.main:main"
+coffeepy = "coffeepy.coffeepy:run"
 
 [project.urls]
 "Homepage" = "https://github.com/kuvaus/coffeepy"
 "Bug Tracker" = "https://github.com/kuvaus/coffeepy/issues"
```


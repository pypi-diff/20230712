# Comparing `tmp/pacman-prompts-1.4.4.tar.gz` & `tmp/pacman-prompts-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pacman-prompts-1.4.4.tar", last modified: Tue Jul 11 18:39:14 2023, max compression
+gzip compressed data, was "pacman-prompts-1.4.5.tar", last modified: Wed Jul 12 18:18:14 2023, max compression
```

## Comparing `pacman-prompts-1.4.4.tar` & `pacman-prompts-1.4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-07-11 18:39:14.054155 pacman-prompts-1.4.4/
--rw-r--r--   0 anishthite   (501) staff       (20)      575 2023-07-11 18:39:14.053985 pacman-prompts-1.4.4/PKG-INFO
--rw-r--r--   0 anishthite   (501) staff       (20)     2044 2023-03-27 18:03:15.000000 pacman-prompts-1.4.4/README.md
-drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-07-11 18:39:14.053026 pacman-prompts-1.4.4/pacman/
--rw-r--r--   0 anishthite   (501) staff       (20)       56 2023-03-15 16:30:00.000000 pacman-prompts-1.4.4/pacman/__init__.py
--rw-r--r--   0 anishthite   (501) staff       (20)      121 2023-03-17 18:53:13.000000 pacman-prompts-1.4.4/pacman/file_utils.py
--rw-r--r--   0 anishthite   (501) staff       (20)      637 2023-04-25 19:15:29.000000 pacman-prompts-1.4.4/pacman/pacman.py
--rw-r--r--   0 anishthite   (501) staff       (20)     3319 2023-07-09 00:33:44.000000 pacman-prompts-1.4.4/pacman/prompt.py
-drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-07-11 18:39:14.053800 pacman-prompts-1.4.4/pacman_prompts.egg-info/
--rw-r--r--   0 anishthite   (501) staff       (20)      575 2023-07-11 18:39:14.000000 pacman-prompts-1.4.4/pacman_prompts.egg-info/PKG-INFO
--rw-r--r--   0 anishthite   (501) staff       (20)      281 2023-07-11 18:39:14.000000 pacman-prompts-1.4.4/pacman_prompts.egg-info/SOURCES.txt
--rw-r--r--   0 anishthite   (501) staff       (20)        1 2023-07-11 18:39:14.000000 pacman-prompts-1.4.4/pacman_prompts.egg-info/dependency_links.txt
--rw-r--r--   0 anishthite   (501) staff       (20)       43 2023-07-11 18:39:14.000000 pacman-prompts-1.4.4/pacman_prompts.egg-info/requires.txt
--rw-r--r--   0 anishthite   (501) staff       (20)        7 2023-07-11 18:39:14.000000 pacman-prompts-1.4.4/pacman_prompts.egg-info/top_level.txt
--rw-r--r--   0 anishthite   (501) staff       (20)       38 2023-07-11 18:39:14.054237 pacman-prompts-1.4.4/setup.cfg
--rw-r--r--   0 anishthite   (501) staff       (20)      883 2023-07-11 18:39:04.000000 pacman-prompts-1.4.4/setup.py
+drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-07-12 18:18:14.357464 pacman-prompts-1.4.5/
+-rw-r--r--   0 anishthite   (501) staff       (20)      575 2023-07-12 18:18:14.357297 pacman-prompts-1.4.5/PKG-INFO
+-rw-r--r--   0 anishthite   (501) staff       (20)     2044 2023-03-27 18:03:15.000000 pacman-prompts-1.4.5/README.md
+drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-07-12 18:18:14.355899 pacman-prompts-1.4.5/pacman/
+-rw-r--r--   0 anishthite   (501) staff       (20)       56 2023-03-15 16:30:00.000000 pacman-prompts-1.4.5/pacman/__init__.py
+-rw-r--r--   0 anishthite   (501) staff       (20)      121 2023-03-17 18:53:13.000000 pacman-prompts-1.4.5/pacman/file_utils.py
+-rw-r--r--   0 anishthite   (501) staff       (20)      637 2023-04-25 19:15:29.000000 pacman-prompts-1.4.5/pacman/pacman.py
+-rw-r--r--   0 anishthite   (501) staff       (20)     3318 2023-07-12 17:48:30.000000 pacman-prompts-1.4.5/pacman/prompt.py
+drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-07-12 18:18:14.357062 pacman-prompts-1.4.5/pacman_prompts.egg-info/
+-rw-r--r--   0 anishthite   (501) staff       (20)      575 2023-07-12 18:18:14.000000 pacman-prompts-1.4.5/pacman_prompts.egg-info/PKG-INFO
+-rw-r--r--   0 anishthite   (501) staff       (20)      281 2023-07-12 18:18:14.000000 pacman-prompts-1.4.5/pacman_prompts.egg-info/SOURCES.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)        1 2023-07-12 18:18:14.000000 pacman-prompts-1.4.5/pacman_prompts.egg-info/dependency_links.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)       43 2023-07-12 18:18:14.000000 pacman-prompts-1.4.5/pacman_prompts.egg-info/requires.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)        7 2023-07-12 18:18:14.000000 pacman-prompts-1.4.5/pacman_prompts.egg-info/top_level.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)       38 2023-07-12 18:18:14.357504 pacman-prompts-1.4.5/setup.cfg
+-rw-r--r--   0 anishthite   (501) staff       (20)      883 2023-07-12 18:18:08.000000 pacman-prompts-1.4.5/setup.py
```

### Comparing `pacman-prompts-1.4.4/PKG-INFO` & `pacman-prompts-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pacman-prompts
-Version: 1.4.4
+Version: 1.4.5
 Summary: Prompts As Code, man
 Home-page: https://github.com/anishthite/pacman
 Author: Anish Thite
 Author-email: anishthite@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pacman-prompts-1.4.4/README.md` & `pacman-prompts-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pacman-prompts-1.4.4/pacman/pacman.py` & `pacman-prompts-1.4.5/pacman/pacman.py`

 * *Files identical despite different names*

### Comparing `pacman-prompts-1.4.4/pacman/prompt.py` & `pacman-prompts-1.4.5/pacman/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from reliablegpt import reliableGPT
 
 openai.api_key = os.getenv('OPENAI_API_KEY')
 if openai.api_key is None:
     raise Exception("OpenAI API key not set")
 
 openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create,
-    user_email='claros@claros.com',
+    user_email='claros@claros.so',
     #model_limits_dir = {"gpt-3.5-turbo-0613": {"max_token_capacity": 90000, "max_request_capacity": 3500}},
     fallback_strategy=['gpt-3.5-turbo-0613', 'gpt-3.5-turbo-0613', 'gpt-3.5-turbo', 'gpt-3.5-turbo-16k'],
     caching=False)
 
 class PromptConfig:
     def __init__(self, config):
         #set attributes from config
```

### Comparing `pacman-prompts-1.4.4/pacman_prompts.egg-info/PKG-INFO` & `pacman-prompts-1.4.5/pacman_prompts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pacman-prompts
-Version: 1.4.4
+Version: 1.4.5
 Summary: Prompts As Code, man
 Home-page: https://github.com/anishthite/pacman
 Author: Anish Thite
 Author-email: anishthite@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pacman-prompts-1.4.4/setup.py` & `pacman-prompts-1.4.5/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'pacman-prompts',
   packages = find_packages(exclude=['examples']),
-  version = '1.4.4',
+  version = '1.4.5',
   license='MIT',
   description = 'Prompts As Code, man',
   long_description_content_type = 'text/markdown',
   author = 'Anish Thite',
   author_email = 'anishthite@gmail.com',
   url = 'https://github.com/anishthite/pacman',
   keywords = [
```


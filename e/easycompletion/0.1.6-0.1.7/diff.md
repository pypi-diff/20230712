# Comparing `tmp/easycompletion-0.1.6.tar.gz` & `tmp/easycompletion-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.1.6.tar", last modified: Wed Jul 12 02:47:06 2023, max compression
+gzip compressed data, was "easycompletion-0.1.7.tar", last modified: Wed Jul 12 02:51:40 2023, max compression
```

## Comparing `easycompletion-0.1.6.tar` & `easycompletion-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-12 02:47:06.670928 easycompletion-0.1.6/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.1.6/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)     6663 2023-07-12 02:47:06.670769 easycompletion-0.1.6/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     5917 2023-07-10 21:51:01.000000 easycompletion-0.1.6/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-12 02:47:06.669770 easycompletion-0.1.6/easycompletion/
--rw-r--r--   0 shawwalters   (501) staff       (20)      746 2023-07-12 02:47:02.000000 easycompletion-0.1.6/easycompletion/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)      511 2023-07-10 21:02:57.000000 easycompletion-0.1.6/easycompletion/constants.py
--rw-r--r--   0 shawwalters   (501) staff       (20)    13812 2023-07-10 21:51:51.000000 easycompletion-0.1.6/easycompletion/model.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     5245 2023-07-10 21:05:34.000000 easycompletion-0.1.6/easycompletion/prompt.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     4499 2023-07-10 21:35:20.000000 easycompletion-0.1.6/easycompletion/test.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-12 02:47:06.670557 easycompletion-0.1.6/easycompletion.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)     6663 2023-07-12 02:47:06.000000 easycompletion-0.1.6/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      342 2023-07-12 02:47:06.000000 easycompletion-0.1.6/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-12 02:47:06.000000 easycompletion-0.1.6/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       23 2023-07-12 02:47:06.000000 easycompletion-0.1.6/easycompletion.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-12 02:47:06.000000 easycompletion-0.1.6/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-12 02:47:06.670981 easycompletion-0.1.6/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1408 2023-07-12 02:47:02.000000 easycompletion-0.1.6/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-12 02:51:40.700489 easycompletion-0.1.7/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.1.7/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)     6663 2023-07-12 02:51:40.700332 easycompletion-0.1.7/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5917 2023-07-10 21:51:01.000000 easycompletion-0.1.7/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-12 02:51:40.699358 easycompletion-0.1.7/easycompletion/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      746 2023-07-12 02:51:36.000000 easycompletion-0.1.7/easycompletion/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)      511 2023-07-10 21:02:57.000000 easycompletion-0.1.7/easycompletion/constants.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)    13812 2023-07-10 21:51:51.000000 easycompletion-0.1.7/easycompletion/model.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5245 2023-07-10 21:05:34.000000 easycompletion-0.1.7/easycompletion/prompt.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     4499 2023-07-10 21:35:20.000000 easycompletion-0.1.7/easycompletion/test.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-12 02:51:40.700119 easycompletion-0.1.7/easycompletion.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     6663 2023-07-12 02:51:40.000000 easycompletion-0.1.7/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      342 2023-07-12 02:51:40.000000 easycompletion-0.1.7/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-12 02:51:40.000000 easycompletion-0.1.7/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       30 2023-07-12 02:51:40.000000 easycompletion-0.1.7/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-12 02:51:40.000000 easycompletion-0.1.7/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-12 02:51:40.700537 easycompletion-0.1.7/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1415 2023-07-12 02:51:36.000000 easycompletion-0.1.7/setup.py
```

### Comparing `easycompletion-0.1.6/LICENSE` & `easycompletion-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.6/PKG-INFO` & `easycompletion-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.1.6
+Version: 0.1.7
 Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/lalalune/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.1.6/README.md` & `easycompletion-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.6/easycompletion/__init__.py` & `easycompletion-0.1.7/easycompletion/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 easycompletion
 
 Leveraging conversational AI for bicameral decision making.
 """
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 __author__ = "Moon (https://github.com/lalalune)"
 __credits__ = "https://github.com/lalalune/easycompletion"
 
 from .model import (
     openai_function_call,
     openai_text_call,
     compose_function,
```

### Comparing `easycompletion-0.1.6/easycompletion/model.py` & `easycompletion-0.1.7/easycompletion/model.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.6/easycompletion/prompt.py` & `easycompletion-0.1.7/easycompletion/prompt.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.6/easycompletion/test.py` & `easycompletion-0.1.7/easycompletion/test.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.1.6/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.1.7/easycompletion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.1.6
+Version: 0.1.7
 Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/lalalune/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.1.6/setup.py` & `easycompletion-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="easycompletion",
-    version='0.1.6',
+    version='0.1.7',
     description="Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/lalalune/easycompletion",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
     packages=["easycompletion"],
-    install_requires=["openai", "tiktoken", "dotenv"],
+    install_requires=["openai", "tiktoken", "python-dotenv"],
     readme="README.md",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
```


# Comparing `tmp/code_to_text-0.1.tar.gz` & `tmp/code_to_text-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_to_text-0.1.tar", last modified: Wed Jul 12 02:08:33 2023, max compression
+gzip compressed data, was "code_to_text-0.2.tar", last modified: Wed Jul 12 02:39:12 2023, max compression
```

## Comparing `code_to_text-0.1.tar` & `code_to_text-0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 davidvanderbyl   (501) staff       (20)        0 2023-07-12 02:08:33.787092 code_to_text-0.1/
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)     2188 2023-07-12 02:08:33.786960 code_to_text-0.1/PKG-INFO
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)     1714 2023-07-07 08:30:16.000000 code_to_text-0.1/README.md
-drwxr-xr-x   0 davidvanderbyl   (501) staff       (20)        0 2023-07-12 02:08:33.785302 code_to_text-0.1/code_to_text/
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)       66 2023-07-07 08:07:35.000000 code_to_text-0.1/code_to_text/__init__.py
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)     4737 2023-07-07 08:16:46.000000 code_to_text-0.1/code_to_text/main.py
-drwxr-xr-x   0 davidvanderbyl   (501) staff       (20)        0 2023-07-12 02:08:33.786400 code_to_text-0.1/code_to_text.egg-info/
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)     2188 2023-07-12 02:08:33.000000 code_to_text-0.1/code_to_text.egg-info/PKG-INFO
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)      319 2023-07-12 02:08:33.000000 code_to_text-0.1/code_to_text.egg-info/SOURCES.txt
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)        1 2023-07-12 02:08:33.000000 code_to_text-0.1/code_to_text.egg-info/dependency_links.txt
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)       52 2023-07-12 02:08:33.000000 code_to_text-0.1/code_to_text.egg-info/entry_points.txt
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)        9 2023-07-12 02:08:33.000000 code_to_text-0.1/code_to_text.egg-info/requires.txt
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)       19 2023-07-12 02:08:33.000000 code_to_text-0.1/code_to_text.egg-info/top_level.txt
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)       38 2023-07-12 02:08:33.787138 code_to_text-0.1/setup.cfg
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)      880 2023-07-07 23:30:07.000000 code_to_text-0.1/setup.py
-drwxr-xr-x   0 davidvanderbyl   (501) staff       (20)        0 2023-07-12 02:08:33.786648 code_to_text-0.1/tests/
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)        0 2023-07-07 07:22:32.000000 code_to_text-0.1/tests/__init__.py
--rw-r--r--   0 davidvanderbyl   (501) staff       (20)     3203 2023-07-07 08:19:54.000000 code_to_text-0.1/tests/test_main.py
+drwxr-xr-x   0 davidvanderbyl   (501) staff       (20)        0 2023-07-12 02:39:12.795020 code_to_text-0.2/
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)     2182 2023-07-12 02:39:12.794890 code_to_text-0.2/PKG-INFO
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)     1708 2023-07-12 02:34:18.000000 code_to_text-0.2/README.md
+drwxr-xr-x   0 davidvanderbyl   (501) staff       (20)        0 2023-07-12 02:39:12.793383 code_to_text-0.2/code_to_text/
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)       66 2023-07-07 08:07:35.000000 code_to_text-0.2/code_to_text/__init__.py
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)     4737 2023-07-07 08:16:46.000000 code_to_text-0.2/code_to_text/main.py
+drwxr-xr-x   0 davidvanderbyl   (501) staff       (20)        0 2023-07-12 02:39:12.794315 code_to_text-0.2/code_to_text.egg-info/
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)     2182 2023-07-12 02:39:12.000000 code_to_text-0.2/code_to_text.egg-info/PKG-INFO
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)      319 2023-07-12 02:39:12.000000 code_to_text-0.2/code_to_text.egg-info/SOURCES.txt
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)        1 2023-07-12 02:39:12.000000 code_to_text-0.2/code_to_text.egg-info/dependency_links.txt
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)       52 2023-07-12 02:39:12.000000 code_to_text-0.2/code_to_text.egg-info/entry_points.txt
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)        9 2023-07-12 02:39:12.000000 code_to_text-0.2/code_to_text.egg-info/requires.txt
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)       13 2023-07-12 02:39:12.000000 code_to_text-0.2/code_to_text.egg-info/top_level.txt
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)       38 2023-07-12 02:39:12.795072 code_to_text-0.2/setup.cfg
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)      859 2023-07-12 02:38:25.000000 code_to_text-0.2/setup.py
+drwxr-xr-x   0 davidvanderbyl   (501) staff       (20)        0 2023-07-12 02:39:12.794638 code_to_text-0.2/tests/
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)        0 2023-07-07 07:22:32.000000 code_to_text-0.2/tests/__init__.py
+-rw-r--r--   0 davidvanderbyl   (501) staff       (20)     3203 2023-07-07 08:19:54.000000 code_to_text-0.2/tests/test_main.py
```

### Comparing `code_to_text-0.1/PKG-INFO` & `code_to_text-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code_to_text
-Version: 0.1
+Version: 0.2
 Summary: Extracts and combines all code from a project into a markdown or txt file.
 Home-page: https://github.com/David-vanderByl/code_to_text.git
 Author: David van der Byl
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -44,15 +44,15 @@
 
 ```
 
 
 Specify the files and directories to exclude:
 
 ```shell
-code_extractor --exclude-files init.py setup.py --exclude-dirs .git __pycache__ dist
+all_code --exclude-files init.py setup.py --exclude-dirs .git __pycache__ dist
 ```
 
 
 By default, code_extractor uses a set of common code file extensions, excludes a list of common files (like __init__.py and setup.py), and excludes a list of common directories (like .git and __pycache__). These defaults are defined in main.py, and you can change them by editing the file. For example, to change the default code file extensions, edit the DEFAULT_CODE_EXTENSIONS variable:
 
 ```python
 DEFAULT_CODE_EXTENSIONS = ['py', 'java', 'js', 'cpp', 'c', 'rb', 'go', 'rs']
```

### Comparing `code_to_text-0.1/README.md` & `code_to_text-0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 ```
 
 
 Specify the files and directories to exclude:
 
 ```shell
-code_extractor --exclude-files init.py setup.py --exclude-dirs .git __pycache__ dist
+all_code --exclude-files init.py setup.py --exclude-dirs .git __pycache__ dist
 ```
 
 
 By default, code_extractor uses a set of common code file extensions, excludes a list of common files (like __init__.py and setup.py), and excludes a list of common directories (like .git and __pycache__). These defaults are defined in main.py, and you can change them by editing the file. For example, to change the default code file extensions, edit the DEFAULT_CODE_EXTENSIONS variable:
 
 ```python
 DEFAULT_CODE_EXTENSIONS = ['py', 'java', 'js', 'cpp', 'c', 'rb', 'go', 'rs']
```

### Comparing `code_to_text-0.1/code_to_text/main.py` & `code_to_text-0.2/code_to_text/main.py`

 * *Files identical despite different names*

### Comparing `code_to_text-0.1/code_to_text.egg-info/PKG-INFO` & `code_to_text-0.2/code_to_text.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-to-text
-Version: 0.1
+Version: 0.2
 Summary: Extracts and combines all code from a project into a markdown or txt file.
 Home-page: https://github.com/David-vanderByl/code_to_text.git
 Author: David van der Byl
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -44,15 +44,15 @@
 
 ```
 
 
 Specify the files and directories to exclude:
 
 ```shell
-code_extractor --exclude-files init.py setup.py --exclude-dirs .git __pycache__ dist
+all_code --exclude-files init.py setup.py --exclude-dirs .git __pycache__ dist
 ```
 
 
 By default, code_extractor uses a set of common code file extensions, excludes a list of common files (like __init__.py and setup.py), and excludes a list of common directories (like .git and __pycache__). These defaults are defined in main.py, and you can change them by editing the file. For example, to change the default code file extensions, edit the DEFAULT_CODE_EXTENSIONS variable:
 
 ```python
 DEFAULT_CODE_EXTENSIONS = ['py', 'java', 'js', 'cpp', 'c', 'rb', 'go', 'rs']
```

### Comparing `code_to_text-0.1/setup.py` & `code_to_text-0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="code_to_text",
-    version="0.1",
-    packages=find_packages(include=['code_to_text', 'code_to_text.*', 'tests', 'tests.*']),
+    version="0.2",
+    packages=find_packages(include=['code_to_text', 'code_to_text.*']),
     description="Extracts and combines all code from a project into a markdown or txt file.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author="David van der Byl",
     author_email="your.email@example.com",
     url="https://github.com/David-vanderByl/code_to_text.git",
     classifiers=[
@@ -17,11 +17,11 @@
     ],
     python_requires='>=3.6',
     install_requires=[
         'pygments',
     ],
     entry_points={
         'console_scripts': [
-            'my_package=my_package.main:main',
+            'all_code=code_to_text.main:main',
         ],
     },
-)
+)
```

### Comparing `code_to_text-0.1/tests/test_main.py` & `code_to_text-0.2/tests/test_main.py`

 * *Files identical despite different names*


# Comparing `tmp/1on1-0.0.tar.gz` & `tmp/1on1-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1on1-0.0.tar", last modified: Mon Jul 10 14:35:40 2023, max compression
+gzip compressed data, was "1on1-0.1.tar", last modified: Wed Jul 12 15:03:33 2023, max compression
```

## Comparing `1on1-0.0.tar` & `1on1-0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-10 14:35:40.233265 1on1-0.0/
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-10 14:35:40.231181 1on1-0.0/1on1/
--rw-r--r--   0 sohinib    (501) staff       (20)      111 2023-07-10 13:21:21.000000 1on1-0.0/1on1/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 1on1-0.0/1on1/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    14296 2023-07-10 13:11:12.000000 1on1-0.0/1on1/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:02:49.000000 1on1-0.0/1on1/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 1on1-0.0/1on1/questionanswer.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-10 14:35:40.232458 1on1-0.0/1on1.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)      466 2023-07-10 14:35:40.000000 1on1-0.0/1on1.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      240 2023-07-10 14:35:40.000000 1on1-0.0/1on1.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-10 14:35:40.000000 1on1-0.0/1on1.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        5 2023-07-10 14:35:40.000000 1on1-0.0/1on1.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 1on1-0.0/LICENSE
--rw-r--r--   0 sohinib    (501) staff       (20)      466 2023-07-10 14:35:40.232909 1on1-0.0/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)        7 2023-07-10 14:29:42.000000 1on1-0.0/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-10 14:35:40.233375 1on1-0.0/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)      696 2023-07-10 14:35:19.000000 1on1-0.0/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-12 15:03:33.735375 1on1-0.1/
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-12 15:03:33.732880 1on1-0.1/1on1/
+-rw-r--r--   0 sohinib    (501) staff       (20)    14296 2023-07-12 14:59:10.000000 1on1-0.1/1on1/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 1on1-0.1/1on1/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    14296 2023-07-10 13:11:12.000000 1on1-0.1/1on1/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:02:49.000000 1on1-0.1/1on1/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)        0 2023-07-10 11:03:09.000000 1on1-0.1/1on1/questionanswer.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-12 15:03:33.734463 1on1-0.1/1on1.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)      466 2023-07-12 15:03:33.000000 1on1-0.1/1on1.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      240 2023-07-12 15:03:33.000000 1on1-0.1/1on1.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-12 15:03:33.000000 1on1-0.1/1on1.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        5 2023-07-12 15:03:33.000000 1on1-0.1/1on1.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 1on1-0.1/LICENSE
+-rw-r--r--   0 sohinib    (501) staff       (20)      466 2023-07-12 15:03:33.734979 1on1-0.1/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)        7 2023-07-10 14:29:42.000000 1on1-0.1/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-12 15:03:33.735489 1on1-0.1/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)      699 2023-07-12 15:03:25.000000 1on1-0.1/setup.py
```

### Comparing `1on1-0.0/1on1/classes.py` & `1on1-0.1/1on1/classes.py`

 * *Files identical despite different names*

### Comparing `1on1-0.0/1on1/classification.py` & `1on1-0.1/1on1/__init__.py`

 * *Files identical despite different names*

### Comparing `1on1-0.0/LICENSE` & `1on1-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `1on1-0.0/setup.py` & `1on1-0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup, find_packages
 
-VERSION=0.0
+VERSION=0.1
+
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION=""
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
-setup(name="1on1",version='0.0',author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","cifar10"],classifiers=CLASSIFIERS)
+setup(name="1on1",version=VERSION,author="Sohini Bhattacharya",author_email="mail.sohinibhattacharya@gmail.com",License="MIT",packages=find_packages(),keywords=["python","image-classification","active-learning-sampling","question-answering","pre-trained models","tiny-image-net","cifar10"],classifiers=CLASSIFIERS)
```


# Comparing `tmp/maadstml-3.43.tar.gz` & `tmp/maadstml-3.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadstml-3.43.tar", last modified: Wed Jun 28 20:05:20 2023, max compression
+gzip compressed data, was "maadstml-3.44.tar", last modified: Wed Jul 12 18:29:59 2023, max compression
```

## Comparing `maadstml-3.43.tar` & `maadstml-3.44.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 20:05:20.803553 maadstml-3.43/
--rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.43/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.43/MANIFEST.in
--rw-rw-rw-   0        0        0   173465 2023-06-28 20:05:20.803553 maadstml-3.43/PKG-INFO
--rw-rw-rw-   0        0        0   172868 2023-06-26 14:42:26.000000 maadstml-3.43/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 20:05:20.783851 maadstml-3.43/maadstml/
--rw-rw-rw-   0        0        0     2303 2023-06-28 20:01:15.000000 maadstml-3.43/maadstml/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.43/maadstml/readpdf.py
--rw-rw-rw-   0        0        0    82502 2023-06-28 20:04:50.000000 maadstml-3.43/maadstml/sendfiles.py
--rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.43/maadstml/tmltextsummary.py
-drwxrwxrwx   0        0        0        0 2023-06-28 20:05:20.800039 maadstml-3.43/maadstml.egg-info/
--rw-rw-rw-   0        0        0   173465 2023-06-28 20:05:20.000000 maadstml-3.43/maadstml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-06-28 20:05:20.000000 maadstml-3.43/maadstml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 20:05:20.000000 maadstml-3.43/maadstml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      189 2023-06-28 20:05:20.000000 maadstml-3.43/maadstml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-28 20:05:20.000000 maadstml-3.43/maadstml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      204 2023-06-24 18:15:22.000000 maadstml-3.43/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 20:05:20.803553 maadstml-3.43/setup.cfg
--rw-rw-rw-   0        0        0     1088 2023-06-28 20:05:00.000000 maadstml-3.43/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:29:59.741104 maadstml-3.44/
+-rw-rw-rw-   0        0        0      852 2020-02-09 18:05:54.000000 maadstml-3.44/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadstml-3.44/MANIFEST.in
+-rw-rw-rw-   0        0        0   173465 2023-07-12 18:29:59.741104 maadstml-3.44/PKG-INFO
+-rw-rw-rw-   0        0        0   172868 2023-06-26 14:42:26.000000 maadstml-3.44/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 18:29:59.711951 maadstml-3.44/maadstml/
+-rw-rw-rw-   0        0        0     2303 2023-06-28 20:01:15.000000 maadstml-3.44/maadstml/__init__.py
+-rw-rw-rw-   0        0        0     4871 2023-06-10 19:44:05.000000 maadstml-3.44/maadstml/readpdf.py
+-rw-rw-rw-   0        0        0    82502 2023-06-28 20:04:50.000000 maadstml-3.44/maadstml/sendfiles.py
+-rw-rw-rw-   0        0        0    10850 2023-06-10 19:08:28.000000 maadstml-3.44/maadstml/tmltextsummary.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:29:59.741104 maadstml-3.44/maadstml.egg-info/
+-rw-rw-rw-   0        0        0   173465 2023-07-12 18:29:59.000000 maadstml-3.44/maadstml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-12 18:29:59.000000 maadstml-3.44/maadstml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 18:29:59.000000 maadstml-3.44/maadstml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      202 2023-07-12 18:29:59.000000 maadstml-3.44/maadstml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 18:29:59.000000 maadstml-3.44/maadstml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      218 2023-07-12 18:27:45.000000 maadstml-3.44/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 18:29:59.741104 maadstml-3.44/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2023-07-12 18:28:37.000000 maadstml-3.44/setup.py
```

### Comparing `maadstml-3.43/LICENSE.txt` & `maadstml-3.44/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadstml-3.43/PKG-INFO` & `maadstml-3.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.43
+Version: 3.44
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadstml-3.43/README.md` & `maadstml-3.44/README.md`

 * *Files identical despite different names*

### Comparing `maadstml-3.43/maadstml/__init__.py` & `maadstml-3.44/maadstml/__init__.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.43/maadstml/readpdf.py` & `maadstml-3.44/maadstml/readpdf.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.43/maadstml/sendfiles.py` & `maadstml-3.44/maadstml/sendfiles.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.43/maadstml/tmltextsummary.py` & `maadstml-3.44/maadstml/tmltextsummary.py`

 * *Files identical despite different names*

### Comparing `maadstml-3.43/maadstml.egg-info/PKG-INFO` & `maadstml-3.44/maadstml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maadstml
-Version: 3.43
+Version: 3.44
 Summary: Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning
 Home-page: https://github.com/smaurice101/transactionalmachinelearning
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
```

### Comparing `maadstml-3.43/setup.py` & `maadstml-3.44/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadstml',
-    version='3.43',
+    version='3.44',
     description='Multi-Agent Accelerator for Data Science (MAADS): Transactional Machine Learning',
     license='MIT License',
     packages=['maadstml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, transactional machine learning, data streams, data science, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
```


# Comparing `tmp/Scrapset-4.1.1.tar.gz` & `tmp/Scrapset-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapset-4.1.1.tar", last modified: Wed Jul 12 16:28:08 2023, max compression
+gzip compressed data, was "Scrapset-4.2.1.tar", last modified: Wed Jul 12 16:38:48 2023, max compression
```

## Comparing `Scrapset-4.1.1.tar` & `Scrapset-4.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 16:28:08.810793 Scrapset-4.1.1/
--rw-rw-rw-   0        0        0     4648 2023-07-12 16:28:08.810793 Scrapset-4.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4417 2023-07-12 16:15:55.000000 Scrapset-4.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 16:28:08.798218 Scrapset-4.1.1/Scrapset/
--rw-rw-rw-   0        0        0     8754 2023-07-12 16:27:13.000000 Scrapset-4.1.1/Scrapset/Scrapset.py
--rw-rw-rw-   0        0        0       49 2023-06-06 18:47:28.000000 Scrapset-4.1.1/Scrapset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:28:08.809809 Scrapset-4.1.1/Scrapset.egg-info/
--rw-rw-rw-   0        0        0     4648 2023-07-12 16:28:08.000000 Scrapset-4.1.1/Scrapset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-12 16:28:08.000000 Scrapset-4.1.1/Scrapset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 16:28:08.000000 Scrapset-4.1.1/Scrapset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-12 16:28:08.000000 Scrapset-4.1.1/Scrapset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-12 16:28:08.000000 Scrapset-4.1.1/Scrapset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 16:28:08.000000 Scrapset-4.1.1/Scrapset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-4.1.1/licence.txt
--rw-rw-rw-   0        0        0      158 2023-07-12 16:28:08.811791 Scrapset-4.1.1/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-07-12 16:26:36.000000 Scrapset-4.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:38:48.355127 Scrapset-4.2.1/
+-rw-rw-rw-   0        0        0     4648 2023-07-12 16:38:48.356135 Scrapset-4.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4417 2023-07-12 16:15:55.000000 Scrapset-4.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 16:38:48.347157 Scrapset-4.2.1/Scrapset/
+-rw-rw-rw-   0        0        0     8754 2023-07-12 16:27:13.000000 Scrapset-4.2.1/Scrapset/Scrapset.py
+-rw-rw-rw-   0        0        0       57 2023-07-12 16:37:03.000000 Scrapset-4.2.1/Scrapset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:38:48.354131 Scrapset-4.2.1/Scrapset.egg-info/
+-rw-rw-rw-   0        0        0     4648 2023-07-12 16:38:48.000000 Scrapset-4.2.1/Scrapset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-12 16:38:48.000000 Scrapset-4.2.1/Scrapset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:38:48.000000 Scrapset-4.2.1/Scrapset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-12 16:38:48.000000 Scrapset-4.2.1/Scrapset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-12 16:38:48.000000 Scrapset-4.2.1/Scrapset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 16:38:48.000000 Scrapset-4.2.1/Scrapset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-4.2.1/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-07-12 16:38:48.357122 Scrapset-4.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-07-12 16:38:35.000000 Scrapset-4.2.1/setup.py
```

### Comparing `Scrapset-4.1.1/PKG-INFO` & `Scrapset-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 4.1.1
+Version: 4.2.1
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-4.1.1/README.md` & `Scrapset-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Scrapset-4.1.1/Scrapset/Scrapset.py` & `Scrapset-4.2.1/Scrapset/Scrapset.py`

 * *Files identical despite different names*

### Comparing `Scrapset-4.1.1/Scrapset.egg-info/PKG-INFO` & `Scrapset-4.2.1/Scrapset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 4.1.1
+Version: 4.2.1
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-4.1.1/licence.txt` & `Scrapset-4.2.1/licence.txt`

 * *Files identical despite different names*


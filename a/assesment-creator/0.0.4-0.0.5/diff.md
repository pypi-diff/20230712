# Comparing `tmp/assesment_creator-0.0.4.tar.gz` & `tmp/assesment_creator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assesment_creator-0.0.4.tar", last modified: Wed Jul 12 15:33:38 2023, max compression
+gzip compressed data, was "assesment_creator-0.0.5.tar", last modified: Wed Jul 12 16:02:03 2023, max compression
```

## Comparing `assesment_creator-0.0.4.tar` & `assesment_creator-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:38.499461 assesment_creator-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 15:33:02.000000 assesment_creator-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-12 15:33:38.499461 assesment_creator-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-12 15:33:02.000000 assesment_creator-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-12 15:33:02.000000 assesment_creator-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-12 15:33:38.499461 assesment_creator-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-12 15:33:02.000000 assesment_creator-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:38.495461 assesment_creator-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:38.499461 assesment_creator-0.0.4/src/assesment_creator/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 15:33:02.000000 assesment_creator-0.0.4/src/assesment_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-12 15:33:02.000000 assesment_creator-0.0.4/src/assesment_creator/cutom_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-12 15:33:02.000000 assesment_creator-0.0.4/src/assesment_creator/get_assesment.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-12 15:33:02.000000 assesment_creator-0.0.4/src/assesment_creator/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-12 15:33:02.000000 assesment_creator-0.0.4/src/assesment_creator/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:38.499461 assesment_creator-0.0.4/src/assesment_creator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-12 15:33:38.000000 assesment_creator-0.0.4/src/assesment_creator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-12 15:33:38.000000 assesment_creator-0.0.4/src/assesment_creator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:33:38.000000 assesment_creator-0.0.4/src/assesment_creator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-12 15:33:38.000000 assesment_creator-0.0.4/src/assesment_creator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 15:33:38.000000 assesment_creator-0.0.4/src/assesment_creator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:02:03.350409 assesment_creator-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-12 16:01:31.000000 assesment_creator-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-12 16:02:03.350409 assesment_creator-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-12 16:01:31.000000 assesment_creator-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-12 16:01:31.000000 assesment_creator-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-12 16:02:03.350409 assesment_creator-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-12 16:01:31.000000 assesment_creator-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:02:03.346409 assesment_creator-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:02:03.350409 assesment_creator-0.0.5/src/assesment_creator/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 16:01:31.000000 assesment_creator-0.0.5/src/assesment_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-12 16:01:31.000000 assesment_creator-0.0.5/src/assesment_creator/cutom_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-12 16:01:31.000000 assesment_creator-0.0.5/src/assesment_creator/get_assesment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-12 16:01:31.000000 assesment_creator-0.0.5/src/assesment_creator/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-12 16:01:31.000000 assesment_creator-0.0.5/src/assesment_creator/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:02:03.350409 assesment_creator-0.0.5/src/assesment_creator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-12 16:02:03.000000 assesment_creator-0.0.5/src/assesment_creator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-12 16:02:03.000000 assesment_creator-0.0.5/src/assesment_creator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:02:03.000000 assesment_creator-0.0.5/src/assesment_creator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-12 16:02:03.000000 assesment_creator-0.0.5/src/assesment_creator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 16:02:03.000000 assesment_creator-0.0.5/src/assesment_creator.egg-info/top_level.txt
```

### Comparing `assesment_creator-0.0.4/LICENSE` & `assesment_creator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `assesment_creator-0.0.4/PKG-INFO` & `assesment_creator-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assesment_creator
-Version: 0.0.4
+Version: 0.0.5
 Summary: assesment creator python package
 Home-page: https://github.com/SachinMishra-ux/assesment_creator
 Author: SachinMishra-ux
 Author-email: sachin19566@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/SachinMishra-ux/assesment_creator/issues
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `assesment_creator-0.0.4/setup.cfg` & `assesment_creator-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `assesment_creator-0.0.4/setup.py` & `assesment_creator-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 import io
 
 with io.open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 REPO_NAME = "assesment_creator"
 AUTHOR_USER_NAME = "SachinMishra-ux"
 SRC_REPO = "assesment_creator"
 AUTHOR_EMAIL = "sachin19566@gmail.com"
 
 setuptools.setup(
```

### Comparing `assesment_creator-0.0.4/src/assesment_creator/get_assesment.py` & `assesment_creator-0.0.5/src/assesment_creator/get_assesment.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,31 +15,31 @@
     sleep(3)
     soup = BeautifulSoup(page.content, "html.parser")
     content = soup.find_all(class_="geS5n")
     content = [pair for pair in content]
     content = str(content)
     mixed_pattern = r'M7eMe">(.*?)\<|auto">(.*?)\<\/span>'
     qno_list = re.findall(mixed_pattern, content)
-    return qno_list
+    if len(qno_list)==0:
+        raise InvalidURLException(
+                    "No data found! Please check the link provided"
+                )
+    else:
+        return qno_list
 
 
 @ensure_annotations
 def create_assesment(form_link: str, file_name: str) -> str:
     try:
         if form_link and file_name is not None:
             output_file(file_name)
             content_list = get_data(form_link)
-            if content_list is not None:
-                ans = create_docx(content_list, file_name)
-                if ans is not None:
-                    return f"Scraping done successfully! Check {file_name} 😀 Thank you!"
-                else:
-                    raise InvalidURLException(
-                        "No data found! Please check the link provided"
-                    )
+            ans = create_docx(content_list, file_name)
+            if ans is not None:
+                return f"Scraping done successfully! Check {file_name} 😀 Thank you!"
             else:
                 raise InvalidURLException(
                     "No data found! Please check the link provided"
                 )
         else:
             return "Url or file_name cannot be empty"
```

### Comparing `assesment_creator-0.0.4/src/assesment_creator/helper.py` & `assesment_creator-0.0.5/src/assesment_creator/helper.py`

 * *Files identical despite different names*

### Comparing `assesment_creator-0.0.4/src/assesment_creator.egg-info/PKG-INFO` & `assesment_creator-0.0.5/src/assesment_creator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assesment-creator
-Version: 0.0.4
+Version: 0.0.5
 Summary: assesment creator python package
 Home-page: https://github.com/SachinMishra-ux/assesment_creator
 Author: SachinMishra-ux
 Author-email: sachin19566@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/SachinMishra-ux/assesment_creator/issues
 Classifier: Programming Language :: Python :: 3.7
```


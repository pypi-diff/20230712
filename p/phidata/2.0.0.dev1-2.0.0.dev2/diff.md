# Comparing `tmp/phidata-2.0.0.dev1.tar.gz` & `tmp/phidata-2.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-2.0.0.dev1.tar", last modified: Tue Jul 11 15:04:04 2023, max compression
+gzip compressed data, was "phidata-2.0.0.dev2.tar", last modified: Tue Jul 11 23:43:15 2023, max compression
```

## Comparing `phidata-2.0.0.dev1.tar` & `phidata-2.0.0.dev2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-11 15:04:04.866521 phidata-2.0.0.dev1/
--rw-r--r--   0 zu         (501) staff       (20)    16759 2022-11-08 02:12:00.000000 phidata-2.0.0.dev1/LICENSE
--rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-11 15:04:04.866369 phidata-2.0.0.dev1/PKG-INFO
--rw-r--r--   0 zu         (501) staff       (20)     2742 2023-06-21 12:59:34.000000 phidata-2.0.0.dev1/README.md
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-11 15:04:04.864357 phidata-2.0.0.dev1/phi/
--rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev1/phi/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     5696 2023-07-11 15:02:10.000000 phidata-2.0.0.dev1/phi/base.py
--rw-r--r--   0 zu         (501) staff       (20)      696 2023-07-11 15:02:10.000000 phidata-2.0.0.dev1/phi/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-11 15:04:04.865134 phidata-2.0.0.dev1/phidata/
--rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev1/phidata/__init__.py
--rw-r--r--   0 zu         (501) staff       (20)     1305 2023-06-15 14:48:05.000000 phidata-2.0.0.dev1/phidata/base.py
--rw-r--r--   0 zu         (501) staff       (20)     1178 2023-01-04 19:03:10.000000 phidata-2.0.0.dev1/phidata/constants.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-11 15:04:04.865925 phidata-2.0.0.dev1/phidata.egg-info/
--rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-11 15:04:04.000000 phidata-2.0.0.dev1/phidata.egg-info/PKG-INFO
--rw-r--r--   0 zu         (501) staff       (20)      357 2023-07-11 15:04:04.000000 phidata-2.0.0.dev1/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 zu         (501) staff       (20)        1 2023-07-11 15:04:04.000000 phidata-2.0.0.dev1/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 zu         (501) staff       (20)       51 2023-07-11 15:04:04.000000 phidata-2.0.0.dev1/phidata.egg-info/entry_points.txt
--rw-r--r--   0 zu         (501) staff       (20)      179 2023-07-11 15:04:04.000000 phidata-2.0.0.dev1/phidata.egg-info/requires.txt
--rw-r--r--   0 zu         (501) staff       (20)       12 2023-07-11 15:04:04.000000 phidata-2.0.0.dev1/phidata.egg-info/top_level.txt
--rw-r--r--   0 zu         (501) staff       (20)     1579 2023-07-11 15:02:10.000000 phidata-2.0.0.dev1/pyproject.toml
--rw-r--r--   0 zu         (501) staff       (20)       38 2023-07-11 15:04:04.866560 phidata-2.0.0.dev1/setup.cfg
--rw-r--r--   0 zu         (501) staff       (20)       98 2022-04-14 17:46:27.000000 phidata-2.0.0.dev1/setup.py
-drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-11 15:04:04.866034 phidata-2.0.0.dev1/tests/
--rw-r--r--   0 zu         (501) staff       (20)       40 2022-11-02 01:40:20.000000 phidata-2.0.0.dev1/tests/test_placeholder.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-11 23:43:15.348780 phidata-2.0.0.dev2/
+-rw-r--r--   0 zu         (501) staff       (20)    16759 2022-11-08 02:12:00.000000 phidata-2.0.0.dev2/LICENSE
+-rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-11 23:43:15.348641 phidata-2.0.0.dev2/PKG-INFO
+-rw-r--r--   0 zu         (501) staff       (20)     2742 2023-06-21 12:59:34.000000 phidata-2.0.0.dev2/README.md
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-11 23:43:15.346785 phidata-2.0.0.dev2/phi/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2023-07-11 15:02:10.000000 phidata-2.0.0.dev2/phi/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     5696 2023-07-11 15:02:10.000000 phidata-2.0.0.dev2/phi/base.py
+-rw-r--r--   0 zu         (501) staff       (20)      696 2023-07-11 15:02:10.000000 phidata-2.0.0.dev2/phi/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-11 23:43:15.347427 phidata-2.0.0.dev2/phidata/
+-rw-r--r--   0 zu         (501) staff       (20)        0 2022-02-28 02:08:34.000000 phidata-2.0.0.dev2/phidata/__init__.py
+-rw-r--r--   0 zu         (501) staff       (20)     1305 2023-06-15 14:48:05.000000 phidata-2.0.0.dev2/phidata/base.py
+-rw-r--r--   0 zu         (501) staff       (20)     1178 2023-01-04 19:03:10.000000 phidata-2.0.0.dev2/phidata/constants.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-11 23:43:15.348218 phidata-2.0.0.dev2/phidata.egg-info/
+-rw-r--r--   0 zu         (501) staff       (20)     3126 2023-07-11 23:43:15.000000 phidata-2.0.0.dev2/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 zu         (501) staff       (20)      357 2023-07-11 23:43:15.000000 phidata-2.0.0.dev2/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 zu         (501) staff       (20)        1 2023-07-11 23:43:15.000000 phidata-2.0.0.dev2/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 zu         (501) staff       (20)       51 2023-07-11 23:43:15.000000 phidata-2.0.0.dev2/phidata.egg-info/entry_points.txt
+-rw-r--r--   0 zu         (501) staff       (20)      179 2023-07-11 23:43:15.000000 phidata-2.0.0.dev2/phidata.egg-info/requires.txt
+-rw-r--r--   0 zu         (501) staff       (20)       12 2023-07-11 23:43:15.000000 phidata-2.0.0.dev2/phidata.egg-info/top_level.txt
+-rw-r--r--   0 zu         (501) staff       (20)     1579 2023-07-11 23:42:39.000000 phidata-2.0.0.dev2/pyproject.toml
+-rw-r--r--   0 zu         (501) staff       (20)       38 2023-07-11 23:43:15.348817 phidata-2.0.0.dev2/setup.cfg
+-rw-r--r--   0 zu         (501) staff       (20)       98 2022-04-14 17:46:27.000000 phidata-2.0.0.dev2/setup.py
+drwxr-xr-x   0 zu         (501) staff       (20)        0 2023-07-11 23:43:15.348324 phidata-2.0.0.dev2/tests/
+-rw-r--r--   0 zu         (501) staff       (20)       40 2022-11-02 01:40:20.000000 phidata-2.0.0.dev2/tests/test_placeholder.py
```

### Comparing `phidata-2.0.0.dev1/LICENSE` & `phidata-2.0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev1/PKG-INFO` & `phidata-2.0.0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: A toolkit for building applications using OSS
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev1 Summary: A toolkit for
+Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev2 Summary: A toolkit for
 building applications using OSS Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                       Run open source tools using python
```

### Comparing `phidata-2.0.0.dev1/README.md` & `phidata-2.0.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev1/phi/base.py` & `phidata-2.0.0.dev2/phi/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev1/phi/constants.py` & `phidata-2.0.0.dev2/phi/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev1/phidata/base.py` & `phidata-2.0.0.dev2/phidata/base.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev1/phidata/constants.py` & `phidata-2.0.0.dev2/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-2.0.0.dev1/phidata.egg-info/PKG-INFO` & `phidata-2.0.0.dev2/phidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: A toolkit for building applications using OSS
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev1 Summary: A toolkit for
+Metadata-Version: 2.1 Name: phidata Version: 2.0.0.dev2 Summary: A toolkit for
 building applications using OSS Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                       Run open source tools using python
```

### Comparing `phidata-2.0.0.dev1/pyproject.toml` & `phidata-2.0.0.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phidata"
-version = "2.0.0.dev1"
+version = "2.0.0.dev2"
 description = "A toolkit for building applications using OSS"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
```


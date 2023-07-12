# Comparing `tmp/kandinsky.py-1.0.tar.gz` & `tmp/kandinsky.py-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kandinsky.py-1.0.tar", last modified: Fri Jun 30 08:30:34 2023, max compression
+gzip compressed data, was "kandinsky.py-2.2.tar", last modified: Wed Jul 12 12:37:40 2023, max compression
```

## Comparing `kandinsky.py-1.0.tar` & `kandinsky.py-2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 08:30:34.005063 kandinsky.py-1.0/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 kandinsky.py-1.0/LICENSE
--rw-rw-rw-   0        0        0      512 2023-06-30 08:30:34.003968 kandinsky.py-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-30 08:17:15.000000 kandinsky.py-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 08:30:33.991250 kandinsky.py-1.0/kandinsky/
--rw-rw-rw-   0        0        0       41 2023-06-30 08:29:30.000000 kandinsky.py-1.0/kandinsky/__init__.py
--rw-rw-rw-   0        0        0     3511 2023-05-28 05:08:25.000000 kandinsky.py-1.0/kandinsky/api.py
-drwxrwxrwx   0        0        0        0 2023-06-30 08:30:34.002914 kandinsky.py-1.0/kandinsky.py.egg-info/
--rw-rw-rw-   0        0        0      512 2023-06-30 08:30:33.000000 kandinsky.py-1.0/kandinsky.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-30 08:30:33.000000 kandinsky.py-1.0/kandinsky.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 08:30:33.000000 kandinsky.py-1.0/kandinsky.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-30 08:30:33.000000 kandinsky.py-1.0/kandinsky.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-30 08:30:33.000000 kandinsky.py-1.0/kandinsky.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 08:30:34.005063 kandinsky.py-1.0/setup.cfg
--rw-rw-rw-   0        0        0      410 2023-06-30 08:30:03.000000 kandinsky.py-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:37:40.014548 kandinsky.py-2.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 kandinsky.py-2.2/LICENSE
+-rw-rw-rw-   0        0        0      512 2023-07-12 12:37:40.014548 kandinsky.py-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-30 08:17:15.000000 kandinsky.py-2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 12:37:39.997933 kandinsky.py-2.2/kandinsky/
+-rw-rw-rw-   0        0        0       41 2023-06-30 08:29:30.000000 kandinsky.py-2.2/kandinsky/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-07-12 12:19:25.000000 kandinsky.py-2.2/kandinsky/api.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:37:40.013540 kandinsky.py-2.2/kandinsky.py.egg-info/
+-rw-rw-rw-   0        0        0      512 2023-07-12 12:37:39.000000 kandinsky.py-2.2/kandinsky.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-07-12 12:37:39.000000 kandinsky.py-2.2/kandinsky.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:37:39.000000 kandinsky.py-2.2/kandinsky.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-12 12:37:39.000000 kandinsky.py-2.2/kandinsky.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 12:37:39.000000 kandinsky.py-2.2/kandinsky.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 12:37:40.015548 kandinsky.py-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      431 2023-07-12 12:29:13.000000 kandinsky.py-2.2/setup.py
```

### Comparing `kandinsky.py-1.0/LICENSE` & `kandinsky.py-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kandinsky.py-1.0/PKG-INFO` & `kandinsky.py-2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kandinsky.py
-Version: 1.0
-Summary: Reverse Engineered Kandinskt 2.1 API
+Version: 2.2
+Summary: Reverse Engineered Kandinskt 2.2 API
 Author: zenafey
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # kandinsky.py
```

### Comparing `kandinsky.py-1.0/kandinsky.py.egg-info/PKG-INFO` & `kandinsky.py-2.2/kandinsky.py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kandinsky.py
-Version: 1.0
-Summary: Reverse Engineered Kandinskt 2.1 API
+Version: 2.2
+Summary: Reverse Engineered Kandinskt 2.2 API
 Author: zenafey
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # kandinsky.py
```


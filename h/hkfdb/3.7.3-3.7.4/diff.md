# Comparing `tmp/hkfdb-3.7.3.tar.gz` & `tmp/hkfdb-3.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.7.3.tar", last modified: Mon Jul 10 02:50:02 2023, max compression
+gzip compressed data, was "hkfdb-3.7.4.tar", last modified: Tue Jul 11 23:35:29 2023, max compression
```

## Comparing `hkfdb-3.7.3.tar` & `hkfdb-3.7.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-10 02:50:02.194467 hkfdb-3.7.3/
--rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.7.3/LICENSE
--rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-07-10 02:50:02.194203 hkfdb-3.7.3/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.7.3/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-10 02:50:02.193163 hkfdb-3.7.3/hkfdb/
--rw-rw-rw-   0 cmw        (501) staff       (20)   109294 2023-07-09 04:51:35.000000 hkfdb-3.7.3/hkfdb/Database.py
--rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.7.3/hkfdb/__init__.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-10 02:50:02.193894 hkfdb-3.7.3/hkfdb.egg-info/
--rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-07-10 02:50:01.000000 hkfdb-3.7.3/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-07-10 02:50:01.000000 hkfdb-3.7.3/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-07-10 02:50:01.000000 hkfdb-3.7.3/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-07-10 02:50:01.000000 hkfdb-3.7.3/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-07-10 02:50:01.000000 hkfdb-3.7.3/hkfdb.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-10 02:50:02.194517 hkfdb-3.7.3/setup.cfg
--rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-07-10 02:49:12.000000 hkfdb-3.7.3/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-11 23:35:29.804363 hkfdb-3.7.4/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.7.4/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-07-11 23:35:29.804033 hkfdb-3.7.4/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.7.4/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-11 23:35:29.802664 hkfdb-3.7.4/hkfdb/
+-rw-rw-rw-   0 cmw        (501) staff       (20)   109573 2023-07-11 23:33:26.000000 hkfdb-3.7.4/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.7.4/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-11 23:35:29.803754 hkfdb-3.7.4/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-07-11 23:35:29.000000 hkfdb-3.7.4/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-07-11 23:35:29.000000 hkfdb-3.7.4/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-07-11 23:35:29.000000 hkfdb-3.7.4/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-07-11 23:35:29.000000 hkfdb-3.7.4/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-07-11 23:35:29.000000 hkfdb-3.7.4/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-11 23:35:29.804431 hkfdb-3.7.4/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-07-11 23:34:36.000000 hkfdb-3.7.4/setup.py
```

### Comparing `hkfdb-3.7.3/LICENSE` & `hkfdb-3.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.7.3/PKG-INFO` & `hkfdb-3.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.7.3
+Version: 3.7.4
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.7.3/README.md` & `hkfdb-3.7.4/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.7.3/hkfdb/Database.py` & `hkfdb-3.7.4/hkfdb/Database.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,14 +402,19 @@
                     df_list = []
                     for item in result_list:
                         date_int = item['_id']
                         df = pd.DataFrame(item['content'], columns=columns)
                         if len(df) > 0:
                             df['date'] = str(date_int)
                             df_list.append(df)
+                    if len(df_list) == 0:
+                        column_names = ['datetime', 'date', 'time', 'open', 'high', 'low', 'close', 'volume', 'expiry_date', 'roll_diff']
+                        df = pd.DataFrame(columns=column_names)
+                        return df
+
                     df = pd.concat(df_list, )
 
                     df['datetime'] = pd.to_datetime(df['datetime'])
 
                     df = df.copy()
                     df['date'] = pd.to_datetime(df['datetime']).dt.strftime('%Y%m%d').astype(int)
                     df['time'] = pd.to_datetime(df['datetime']).dt.strftime('%H%M%S').astype(int)
```

### Comparing `hkfdb-3.7.3/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.7.4/hkfdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.7.3
+Version: 3.7.4
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.7.3/setup.py` & `hkfdb-3.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="3.7.3",
+    version="3.7.4",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```


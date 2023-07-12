# Comparing `tmp/idbadapter-1.7.tar.gz` & `tmp/idbadapter-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.7.tar", last modified: Tue Jul 11 13:07:02 2023, max compression
+gzip compressed data, was "idbadapter-1.8.tar", last modified: Wed Jul 12 15:18:52 2023, max compression
```

## Comparing `idbadapter-1.7.tar` & `idbadapter-1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 13:07:02.060124 idbadapter-1.7/
--rw-rw-rw-   0        0        0    11558 2023-06-20 07:34:13.000000 idbadapter-1.7/LICENSE
--rw-rw-rw-   0        0        0      695 2023-07-11 13:07:02.060124 idbadapter-1.7/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-20 07:34:13.000000 idbadapter-1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 13:07:02.029022 idbadapter-1.7/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-06-20 07:34:13.000000 idbadapter-1.7/idbadapter/__init__.py
--rw-rw-rw-   0        0        0    11984 2023-07-06 12:00:25.000000 idbadapter-1.7/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-07-11 13:07:02.054106 idbadapter-1.7/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      695 2023-07-11 13:07:01.000000 idbadapter-1.7/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-11 13:07:01.000000 idbadapter-1.7/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 13:07:01.000000 idbadapter-1.7/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-11 13:07:01.000000 idbadapter-1.7/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-11 13:07:01.000000 idbadapter-1.7/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 13:07:02.062131 idbadapter-1.7/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-07-11 13:06:56.000000 idbadapter-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:18:52.375835 idbadapter-1.8/
+-rw-rw-rw-   0        0        0    11558 2023-06-20 07:34:13.000000 idbadapter-1.8/LICENSE
+-rw-rw-rw-   0        0        0      695 2023-07-12 15:18:52.375835 idbadapter-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-20 07:34:13.000000 idbadapter-1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 15:18:52.341720 idbadapter-1.8/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-06-20 07:34:13.000000 idbadapter-1.8/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0    12044 2023-07-12 15:10:41.000000 idbadapter-1.8/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:18:52.368811 idbadapter-1.8/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      695 2023-07-12 15:18:52.000000 idbadapter-1.8/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-12 15:18:52.000000 idbadapter-1.8/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 15:18:52.000000 idbadapter-1.8/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-12 15:18:52.000000 idbadapter-1.8/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-12 15:18:52.000000 idbadapter-1.8/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 15:18:52.379847 idbadapter-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-07-12 15:18:49.000000 idbadapter-1.8/setup.py
```

### Comparing `idbadapter-1.7/LICENSE` & `idbadapter-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.7/PKG-INFO` & `idbadapter-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.7
+Version: 1.8
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.7/idbadapter/schedule_loader.py` & `idbadapter-1.8/idbadapter/schedule_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,20 +193,22 @@
                 
             if len(resource_list) != 0:
                 query += f""" and rnm.name in ({",".join(map(lambda x: f"'{x}'", resource_list))})"""   
             try:
                 df = self._execute_query(query)
             except ValueError:
                 print("jsondecodeerror occurred", pull)
+                yield None
                 continue 
 
             if df.empty:
                 with open(self.path_to_log, "a", encoding="UTF-8") as f:
                     print("pull not found", pull, file=f)
                     print("empty df. pull not found")
+                    yield None
                 continue
                 
             df["full_fraction"] = df["physical_volume"]
                       
                 
             yield SchedulesIterator.convert_df(df)
```

### Comparing `idbadapter-1.7/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.8/idbadapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.7
+Version: 1.8
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.7/setup.py` & `idbadapter-1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '1.7'
+version = '1.8'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.7',
+      version='1.8',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```


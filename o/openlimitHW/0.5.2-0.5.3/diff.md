# Comparing `tmp/openlimitHW-0.5.2.tar.gz` & `tmp/openlimitHW-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlimitHW-0.5.2.tar", last modified: Wed Jul 12 08:19:05 2023, max compression
+gzip compressed data, was "openlimitHW-0.5.3.tar", last modified: Wed Jul 12 08:25:34 2023, max compression
```

## Comparing `openlimitHW-0.5.2.tar` & `openlimitHW-0.5.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 08:19:05.558328 openlimitHW-0.5.2/
--rw-rw-rw-   0        0        0    35823 2023-05-15 06:56:00.000000 openlimitHW-0.5.2/LICENSE
--rw-rw-rw-   0        0        0     1835 2023-07-12 08:19:05.557688 openlimitHW-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     1181 2023-07-06 02:39:10.000000 openlimitHW-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 08:19:05.539980 openlimitHW-0.5.2/openlimit/
--rw-rw-rw-   0        0        0      172 2023-07-06 03:24:36.000000 openlimitHW-0.5.2/openlimit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 08:19:05.550949 openlimitHW-0.5.2/openlimit/buckets/
--rw-rw-rw-   0        0        0      113 2023-07-06 03:24:36.000000 openlimitHW-0.5.2/openlimit/buckets/__init__.py
--rw-rw-rw-   0        0        0     3590 2023-07-06 03:24:36.000000 openlimitHW-0.5.2/openlimit/buckets/bucket.py
--rw-rw-rw-   0        0        0     1929 2023-07-06 03:24:36.000000 openlimitHW-0.5.2/openlimit/buckets/redis_bucket.py
--rw-rw-rw-   0        0        0     3544 2023-07-12 08:18:01.000000 openlimitHW-0.5.2/openlimit/rate_limiters.py
--rw-rw-rw-   0        0        0     2622 2023-07-06 03:24:36.000000 openlimitHW-0.5.2/openlimit/redis_rate_limiters.py
--rw-rw-rw-   0        0        0        0 2023-07-06 03:24:36.000000 openlimitHW-0.5.2/openlimit/test.py
-drwxrwxrwx   0        0        0        0 2023-07-12 08:19:05.555950 openlimitHW-0.5.2/openlimit/utilities/
--rw-rw-rw-   0        0        0      267 2023-07-06 03:24:36.000000 openlimitHW-0.5.2/openlimit/utilities/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-07-06 03:24:36.000000 openlimitHW-0.5.2/openlimit/utilities/context_decorators.py
--rw-rw-rw-   0        0        0     1247 2023-07-06 03:24:36.000000 openlimitHW-0.5.2/openlimit/utilities/token_counters.py
-drwxrwxrwx   0        0        0        0 2023-07-12 08:19:05.546951 openlimitHW-0.5.2/openlimitHW.egg-info/
--rw-rw-rw-   0        0        0     1835 2023-07-12 08:19:05.000000 openlimitHW-0.5.2/openlimitHW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2023-07-12 08:19:05.000000 openlimitHW-0.5.2/openlimitHW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 08:19:05.000000 openlimitHW-0.5.2/openlimitHW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-12 08:19:05.000000 openlimitHW-0.5.2/openlimitHW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 08:19:05.000000 openlimitHW-0.5.2/openlimitHW.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      474 2023-07-12 08:18:49.000000 openlimitHW-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 08:19:05.558328 openlimitHW-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      608 2023-07-12 08:18:45.000000 openlimitHW-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:25:34.009956 openlimitHW-0.5.3/
+-rw-rw-rw-   0        0        0    35823 2023-05-15 06:56:00.000000 openlimitHW-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0     1835 2023-07-12 08:25:34.008987 openlimitHW-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1181 2023-07-06 02:39:10.000000 openlimitHW-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 08:25:33.987017 openlimitHW-0.5.3/openlimit/
+-rw-rw-rw-   0        0        0      172 2023-07-12 08:23:18.000000 openlimitHW-0.5.3/openlimit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:25:34.000947 openlimitHW-0.5.3/openlimit/buckets/
+-rw-rw-rw-   0        0        0      113 2023-07-12 08:23:18.000000 openlimitHW-0.5.3/openlimit/buckets/__init__.py
+-rw-rw-rw-   0        0        0     3590 2023-07-12 08:23:18.000000 openlimitHW-0.5.3/openlimit/buckets/bucket.py
+-rw-rw-rw-   0        0        0     1929 2023-07-12 08:23:18.000000 openlimitHW-0.5.3/openlimit/buckets/redis_bucket.py
+-rw-rw-rw-   0        0        0     3545 2023-07-12 08:24:07.000000 openlimitHW-0.5.3/openlimit/rate_limiters.py
+-rw-rw-rw-   0        0        0     2622 2023-07-12 08:23:18.000000 openlimitHW-0.5.3/openlimit/redis_rate_limiters.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 08:23:18.000000 openlimitHW-0.5.3/openlimit/test.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:25:34.005983 openlimitHW-0.5.3/openlimit/utilities/
+-rw-rw-rw-   0        0        0      267 2023-07-12 08:23:18.000000 openlimitHW-0.5.3/openlimit/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-07-12 08:23:18.000000 openlimitHW-0.5.3/openlimit/utilities/context_decorators.py
+-rw-rw-rw-   0        0        0     1247 2023-07-12 08:23:18.000000 openlimitHW-0.5.3/openlimit/utilities/token_counters.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:25:33.995157 openlimitHW-0.5.3/openlimitHW.egg-info/
+-rw-rw-rw-   0        0        0     1835 2023-07-12 08:25:33.000000 openlimitHW-0.5.3/openlimitHW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2023-07-12 08:25:33.000000 openlimitHW-0.5.3/openlimitHW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 08:25:33.000000 openlimitHW-0.5.3/openlimitHW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-12 08:25:33.000000 openlimitHW-0.5.3/openlimitHW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 08:25:33.000000 openlimitHW-0.5.3/openlimitHW.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      474 2023-07-12 08:25:02.000000 openlimitHW-0.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 08:25:34.009956 openlimitHW-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      608 2023-07-12 08:25:11.000000 openlimitHW-0.5.3/setup.py
```

### Comparing `openlimitHW-0.5.2/LICENSE` & `openlimitHW-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.5.2/PKG-INFO` & `openlimitHW-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlimitHW
-Version: 0.5.2
+Version: 0.5.3
 Summary: Rate limiter for the OpenAI API (modified by HW)
 Home-page: https://github.com/williamxhero/openlimitHW
 Author: williamxhero
 Author-email: williamxhero <williamxhero@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/williamxhero/openlimitHW
 Keywords: openai,rate-limit,limit,api,request,token,leaky-bucket,gcra,redis,asyncio
```

### Comparing `openlimitHW-0.5.2/README.md` & `openlimitHW-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.5.2/openlimit/buckets/bucket.py` & `openlimitHW-0.5.3/openlimit/buckets/bucket.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.5.2/openlimit/buckets/redis_bucket.py` & `openlimitHW-0.5.3/openlimit/buckets/redis_bucket.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.5.2/openlimit/rate_limiters.py` & `openlimitHW-0.5.3/openlimit/rate_limiters.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                  token_counter, 
                  resp_token_count, 
                  resources:list[str],
                  per_minutes=1,
                  verbose=False):
         
         if not resources:
-            resource = ['default']
+            resources = ['default']
         
         # Token counter
         self.token_counter = token_counter
         self.response_token_count = resp_token_count
 
         # Buckets
         self.res_q = []
```

### Comparing `openlimitHW-0.5.2/openlimit/redis_rate_limiters.py` & `openlimitHW-0.5.3/openlimit/redis_rate_limiters.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.5.2/openlimit/utilities/context_decorators.py` & `openlimitHW-0.5.3/openlimit/utilities/context_decorators.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.5.2/openlimit/utilities/token_counters.py` & `openlimitHW-0.5.3/openlimit/utilities/token_counters.py`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.5.2/openlimitHW.egg-info/PKG-INFO` & `openlimitHW-0.5.3/openlimitHW.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlimitHW
-Version: 0.5.2
+Version: 0.5.3
 Summary: Rate limiter for the OpenAI API (modified by HW)
 Home-page: https://github.com/williamxhero/openlimitHW
 Author: williamxhero
 Author-email: williamxhero <williamxhero@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/williamxhero/openlimitHW
 Keywords: openai,rate-limit,limit,api,request,token,leaky-bucket,gcra,redis,asyncio
```

### Comparing `openlimitHW-0.5.2/openlimitHW.egg-info/SOURCES.txt` & `openlimitHW-0.5.3/openlimitHW.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openlimitHW-0.5.2/setup.py` & `openlimitHW-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from setuptools import setup
 
 setup(
     name="openlimitHW",
     description="Rate limiter for the OpenAI API (modified by HW)",
-    version="v0.5.2",
+    version="v0.5.3",
     packages=["openlimit", "openlimit.utilities", "openlimit.buckets"],
     python_requires=">=3",
     url="https://github.com/williamxhero/openlimitHW",
     author="williamxhero",
     author_email="williamxhero@gmail.com",
     # classifiers=[],
     install_requires=["redis", "tiktoken"],
```


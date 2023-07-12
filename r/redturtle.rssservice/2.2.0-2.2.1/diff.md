# Comparing `tmp/redturtle.rssservice-2.2.0.tar.gz` & `tmp/redturtle.rssservice-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.rssservice-2.2.0.tar", last modified: Tue Mar 21 11:08:35 2023, max compression
+gzip compressed data, was "redturtle.rssservice-2.2.1.tar", last modified: Wed Jul 12 07:43:19 2023, max compression
```

## Comparing `redturtle.rssservice-2.2.0.tar` & `redturtle.rssservice-2.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-21 11:08:35.571863 redturtle.rssservice-2.2.0/
--rw-r--r--   0 cekk       (501) staff       (20)      970 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       62 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      660 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      140 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     7770 2023-03-21 11:08:35.572043 redturtle.rssservice-2.2.0/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     4002 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)       27 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)       62 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/constraints_plone52.txt
--rw-r--r--   0 cekk       (501) staff       (20)      412 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/constraints_plone60.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-21 11:08:35.566177 redturtle.rssservice-2.2.0/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7901 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)       83 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)       42 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)       50 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/requirements_plone52.txt
--rw-r--r--   0 cekk       (501) staff       (20)      475 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/requirements_plone60.txt
--rw-r--r--   0 cekk       (501) staff       (20)      383 2023-03-21 11:08:35.572555 redturtle.rssservice-2.2.0/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2611 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-21 11:08:35.561491 redturtle.rssservice-2.2.0/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-21 11:08:35.566727 redturtle.rssservice-2.2.0/src/redturtle/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/src/redturtle/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-21 11:08:35.571153 redturtle.rssservice-2.2.0/src/redturtle/rssservice/
--rw-r--r--   0 cekk       (501) staff       (20)      140 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/src/redturtle/rssservice/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      408 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/src/redturtle/rssservice/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1242 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/src/redturtle/rssservice/interfaces.py
--rw-r--r--   0 cekk       (501) staff       (20)    11829 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/src/redturtle/rssservice/rss_mixer.py
--rw-r--r--   0 cekk       (501) staff       (20)     2535 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/src/redturtle/rssservice/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-21 11:08:35.571625 redturtle.rssservice-2.2.0/src/redturtle/rssservice/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/src/redturtle/rssservice/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)    11976 2023-03-21 11:08:34.000000 redturtle.rssservice-2.2.0/src/redturtle/rssservice/tests/test_rss_mixer.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-03-21 11:08:35.569833 redturtle.rssservice-2.2.0/src/redturtle.rssservice.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     7770 2023-03-21 11:08:35.000000 redturtle.rssservice-2.2.0/src/redturtle.rssservice.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)      967 2023-03-21 11:08:35.000000 redturtle.rssservice-2.2.0/src/redturtle.rssservice.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-03-21 11:08:35.000000 redturtle.rssservice-2.2.0/src/redturtle.rssservice.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      145 2023-03-21 11:08:35.000000 redturtle.rssservice-2.2.0/src/redturtle.rssservice.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       10 2023-03-21 11:08:35.000000 redturtle.rssservice-2.2.0/src/redturtle.rssservice.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-03-21 11:08:35.000000 redturtle.rssservice-2.2.0/src/redturtle.rssservice.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      222 2023-03-21 11:08:35.000000 redturtle.rssservice-2.2.0/src/redturtle.rssservice.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       10 2023-03-21 11:08:35.000000 redturtle.rssservice-2.2.0/src/redturtle.rssservice.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-07-12 07:43:19.302273 redturtle.rssservice-2.2.1/
+-rw-r--r--   0 cekk       (501) staff       (20)     1163 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       62 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      660 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      140 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     8027 2023-07-12 07:43:19.302435 redturtle.rssservice-2.2.1/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     4002 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       62 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/constraints_plone52.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      412 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/constraints_plone60.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-07-12 07:43:19.297703 redturtle.rssservice-2.2.1/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7901 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)       83 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       42 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       50 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/requirements_plone52.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      475 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/requirements_plone60.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      383 2023-07-12 07:43:19.302955 redturtle.rssservice-2.2.1/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2611 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-07-12 07:43:19.292838 redturtle.rssservice-2.2.1/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-07-12 07:43:19.297964 redturtle.rssservice-2.2.1/src/redturtle/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/src/redturtle/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-07-12 07:43:19.301611 redturtle.rssservice-2.2.1/src/redturtle/rssservice/
+-rw-r--r--   0 cekk       (501) staff       (20)      140 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/src/redturtle/rssservice/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      408 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/src/redturtle/rssservice/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1242 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/src/redturtle/rssservice/interfaces.py
+-rw-r--r--   0 cekk       (501) staff       (20)    11949 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/src/redturtle/rssservice/rss_mixer.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2535 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/src/redturtle/rssservice/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-07-12 07:43:19.302054 redturtle.rssservice-2.2.1/src/redturtle/rssservice/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/src/redturtle/rssservice/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)    11976 2023-07-12 07:43:18.000000 redturtle.rssservice-2.2.1/src/redturtle/rssservice/tests/test_rss_mixer.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-07-12 07:43:19.300263 redturtle.rssservice-2.2.1/src/redturtle.rssservice.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     8027 2023-07-12 07:43:19.000000 redturtle.rssservice-2.2.1/src/redturtle.rssservice.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)      967 2023-07-12 07:43:19.000000 redturtle.rssservice-2.2.1/src/redturtle.rssservice.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-07-12 07:43:19.000000 redturtle.rssservice-2.2.1/src/redturtle.rssservice.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      145 2023-07-12 07:43:19.000000 redturtle.rssservice-2.2.1/src/redturtle.rssservice.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       10 2023-07-12 07:43:19.000000 redturtle.rssservice-2.2.1/src/redturtle.rssservice.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-07-12 07:43:19.000000 redturtle.rssservice-2.2.1/src/redturtle.rssservice.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      222 2023-07-12 07:43:19.000000 redturtle.rssservice-2.2.1/src/redturtle.rssservice.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       10 2023-07-12 07:43:19.000000 redturtle.rssservice-2.2.1/src/redturtle.rssservice.egg-info/top_level.txt
```

### Comparing `redturtle.rssservice-2.2.0/CHANGES.rst` & `redturtle.rssservice-2.2.1/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+2.2.1 (2023-07-12)
+------------------
+
+- Handle case when feed url is an internal url with resolveuid.
+  [cekk]
+- Do not print exception on log, but use warning because it's handled.
+  [cekk]
+
 2.2.0 (2023-03-21)
 ------------------
 
 - Allow configuring the User-Agent for the requests to get feeds,
   via the REQUESTS_USER_AGENT environment variable.
   [davisagli]
```

### Comparing `redturtle.rssservice-2.2.0/DEVELOP.rst` & `redturtle.rssservice-2.2.1/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `redturtle.rssservice-2.2.0/LICENSE.GPL` & `redturtle.rssservice-2.2.1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.rssservice-2.2.0/LICENSE.rst` & `redturtle.rssservice-2.2.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.rssservice-2.2.0/PKG-INFO` & `redturtle.rssservice-2.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.rssservice
-Version: 2.2.0
+Version: 2.2.1
 Summary: An add-on for Plone
 Home-page: https://github.com/collective/redturtle.rssservice
 Author: RedTurtle
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/redturtle.rssservice
 Project-URL: Source, https://github.com/collective/redturtle.rssservice
@@ -152,14 +152,22 @@
         
         - RedTurtle, sviluppo@redturtle.it
         
         
         Changelog
         =========
         
+        2.2.1 (2023-07-12)
+        ------------------
+        
+        - Handle case when feed url is an internal url with resolveuid.
+          [cekk]
+        - Do not print exception on log, but use warning because it's handled.
+          [cekk]
+        
         2.2.0 (2023-03-21)
         ------------------
         
         - Allow configuring the User-Agent for the requests to get feeds,
           via the REQUESTS_USER_AGENT environment variable.
           [davisagli]
```

### Comparing `redturtle.rssservice-2.2.0/README.rst` & `redturtle.rssservice-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.rssservice-2.2.0/docs/conf.py` & `redturtle.rssservice-2.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redturtle.rssservice-2.2.0/setup.py` & `redturtle.rssservice-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="redturtle.rssservice",
-    version="2.2.0",
+    version="2.2.1",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `redturtle.rssservice-2.2.0/src/redturtle/rssservice/interfaces.py` & `redturtle.rssservice-2.2.1/src/redturtle/rssservice/interfaces.py`

 * *Files identical despite different names*

### Comparing `redturtle.rssservice-2.2.0/src/redturtle/rssservice/rss_mixer.py` & `redturtle.rssservice-2.2.1/src/redturtle/rssservice/rss_mixer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 from DateTime import DateTime
 from DateTime.interfaces import SyntaxError
 from os import environ
 from plone.dexterity.utils import iterSchemata
 from plone.restapi.serializer.converters import json_compatible
+from plone.restapi.serializer.utils import uid_to_url
 from plone.restapi.services import Service
 from redturtle.rssservice import _
 from redturtle.rssservice.interfaces import IRSSMixerFeed
 from requests.exceptions import RequestException
 from requests.exceptions import Timeout
 from time import time
 from zExceptions import BadRequest
 from zExceptions import NotFound
 from zope.i18n import translate
 from zope.interface import implementer
 from zope.schema import getFields
 
-
 import feedparser
 import json
 import logging
 import requests
 
 logger = logging.getLogger(__name__)
 
@@ -223,25 +223,26 @@
         return self.ok
 
     def _getFeedFromUrl(self, url):
         """
         Use urllib to retrieve an rss feed.
         In this way, we can manage timeouts.
         """
+        url = uid_to_url(url)
         headers = {}
         if REQUESTS_USER_AGENT:
             headers["User-Agent"] = REQUESTS_USER_AGENT
         try:
             response = requests.get(
                 url,
                 headers=headers,
                 timeout=REQUESTS_TIMEOUT,
             )
         except (Timeout, RequestException) as e:
-            logger.exception(e)
+            logger.warning("exception %s during %s request", e, url)
             return None
         if response.status_code != 200:
             message = response.text or response.reason
             logger.error(
                 "Unable to retrieve feed from {url}: {message}".format(
                     url=url, message=message
                 )
```

### Comparing `redturtle.rssservice-2.2.0/src/redturtle/rssservice/testing.py` & `redturtle.rssservice-2.2.1/src/redturtle/rssservice/testing.py`

 * *Files identical despite different names*

### Comparing `redturtle.rssservice-2.2.0/src/redturtle/rssservice/tests/test_rss_mixer.py` & `redturtle.rssservice-2.2.1/src/redturtle/rssservice/tests/test_rss_mixer.py`

 * *Files identical despite different names*

### Comparing `redturtle.rssservice-2.2.0/src/redturtle.rssservice.egg-info/PKG-INFO` & `redturtle.rssservice-2.2.1/src/redturtle.rssservice.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.rssservice
-Version: 2.2.0
+Version: 2.2.1
 Summary: An add-on for Plone
 Home-page: https://github.com/collective/redturtle.rssservice
 Author: RedTurtle
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/redturtle.rssservice
 Project-URL: Source, https://github.com/collective/redturtle.rssservice
@@ -152,14 +152,22 @@
         
         - RedTurtle, sviluppo@redturtle.it
         
         
         Changelog
         =========
         
+        2.2.1 (2023-07-12)
+        ------------------
+        
+        - Handle case when feed url is an internal url with resolveuid.
+          [cekk]
+        - Do not print exception on log, but use warning because it's handled.
+          [cekk]
+        
         2.2.0 (2023-03-21)
         ------------------
         
         - Allow configuring the User-Agent for the requests to get feeds,
           via the REQUESTS_USER_AGENT environment variable.
           [davisagli]
```

### Comparing `redturtle.rssservice-2.2.0/src/redturtle.rssservice.egg-info/SOURCES.txt` & `redturtle.rssservice-2.2.1/src/redturtle.rssservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*


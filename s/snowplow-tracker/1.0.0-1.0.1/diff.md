# Comparing `tmp/snowplow-tracker-1.0.0.tar.gz` & `tmp/snowplow-tracker-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowplow-tracker-1.0.0.tar", last modified: Fri Jun 16 14:30:22 2023, max compression
+gzip compressed data, was "snowplow-tracker-1.0.1.tar", last modified: Wed Jul 12 15:26:34 2023, max compression
```

## Comparing `snowplow-tracker-1.0.0.tar` & `snowplow-tracker-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:22.037680 snowplow-tracker-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     9341 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5517 2023-06-16 14:30:22.037680 snowplow-tracker-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4452 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:22.033680 snowplow-tracker-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 14:30:22.037680 snowplow-tracker-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:22.033680 snowplow-tracker-1.0.0/snowplow_tracker/
--rw-r--r--   0 runner    (1001) docker     (122)      731 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      885 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/contracts.py
--rw-r--r--   0 runner    (1001) docker     (122)     9408 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/emitter_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    21443 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/emitters.py
--rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/event_store.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:22.037680 snowplow-tracker-1.0.0/snowplow_tracker/events/
--rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4830 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     5122 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/page_ping.py
--rw-r--r--   0 runner    (1001) docker     (122)     3236 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/page_view.py
--rw-r--r--   0 runner    (1001) docker     (122)     7120 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/screen_view.py
--rw-r--r--   0 runner    (1001) docker     (122)     4034 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/self_describing.py
--rw-r--r--   0 runner    (1001) docker     (122)     4680 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/events/structured_event.py
--rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/payload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/self_describing_json.py
--rw-r--r--   0 runner    (1001) docker     (122)     5600 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/snowplow.py
--rw-r--r--   0 runner    (1001) docker     (122)     6029 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/subject.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:22.037680 snowplow-tracker-1.0.0/snowplow_tracker/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    38419 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/tracker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2318 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/tracker_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     1993 2023-06-16 14:30:17.000000 snowplow-tracker-1.0.0/snowplow_tracker/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:30:22.037680 snowplow-tracker-1.0.0/snowplow_tracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5517 2023-06-16 14:30:22.000000 snowplow-tracker-1.0.0/snowplow_tracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-06-16 14:30:22.000000 snowplow-tracker-1.0.0/snowplow_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 14:30:22.000000 snowplow-tracker-1.0.0/snowplow_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-16 14:30:22.000000 snowplow-tracker-1.0.0/snowplow_tracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-16 14:30:22.000000 snowplow-tracker-1.0.0/snowplow_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:26:34.626486 snowplow-tracker-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     9476 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5517 2023-07-12 15:26:34.626486 snowplow-tracker-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4452 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:26:34.622485 snowplow-tracker-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 15:26:34.626486 snowplow-tracker-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:26:34.626486 snowplow-tracker-1.0.1/snowplow_tracker/
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9408 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/emitter_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21443 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/emitters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/event_store.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:26:34.626486 snowplow-tracker-1.0.1/snowplow_tracker/events/
+-rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4830 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/events/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5122 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/events/page_ping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3236 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/events/page_view.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7120 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/events/screen_view.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4034 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/events/self_describing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4680 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/events/structured_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/payload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/self_describing_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5600 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/snowplow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6029 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/subject.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:26:34.626486 snowplow-tracker-1.0.1/snowplow_tracker/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38355 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2318 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/tracker_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1993 2023-07-12 15:26:29.000000 snowplow-tracker-1.0.1/snowplow_tracker/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 15:26:34.626486 snowplow-tracker-1.0.1/snowplow_tracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5517 2023-07-12 15:26:34.000000 snowplow-tracker-1.0.1/snowplow_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-07-12 15:26:34.000000 snowplow-tracker-1.0.1/snowplow_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 15:26:34.000000 snowplow-tracker-1.0.1/snowplow_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-12 15:26:34.000000 snowplow-tracker-1.0.1/snowplow_tracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-12 15:26:34.000000 snowplow-tracker-1.0.1/snowplow_tracker.egg-info/top_level.txt
```

### Comparing `snowplow-tracker-1.0.0/CHANGES.txt` & `snowplow-tracker-1.0.1/CHANGES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+Version 1.0.1 (2023-07-12)
+--------------------------
+Fix tstamp parameter in track_self_describing_event (#350) (Thanks to @andehen)
+
 Version 1.0.0 (2023-06-16)
 --------------------------
 Remove Redis and Celery Emitters (#335)
 Make tracker namespace mandatory (#337) 
 Track function to return event_id (#338) 
 Fix namespace assignment in Snowplow API (#341) 
 Refactor track_xxx() methods (#343)
```

### Comparing `snowplow-tracker-1.0.0/LICENSE` & `snowplow-tracker-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/PKG-INFO` & `snowplow-tracker-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowplow-tracker
-Version: 1.0.0
+Version: 1.0.1
 Summary: Snowplow event tracker for Python. Add analytics to your Python and Django apps, webapps and games
 Home-page: http://snowplow.io
 Author: Anuj More, Alexander Dean, Fred Blundun, Paul Boocock, Matus Tomlein, Jack Keene
 Author-email: support@snowplow.io
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `snowplow-tracker-1.0.0/README.md` & `snowplow-tracker-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/setup.py` & `snowplow-tracker-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 authors_email_list = [
     "support@snowplow.io",
 ]
 authors_email_str = ", ".join(authors_email_list)
 
 setup(
     name="snowplow-tracker",
-    version="1.0.0",
+    version="1.0.1",
     author=authors_str,
     author_email=authors_email_str,
     packages=["snowplow_tracker", "snowplow_tracker.test", "snowplow_tracker.events"],
     url="http://snowplow.io",
     license="Apache License 2.0",
     description="Snowplow event tracker for Python. Add analytics to your Python and Django apps, webapps and games",
     long_description=open("README.md").read(),
```

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/__init__.py` & `snowplow-tracker-1.0.1/snowplow_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/_version.py` & `snowplow-tracker-1.0.1/snowplow_tracker/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 #     Unless required by applicable law or agreed to in writing,
 #     software distributed under the Apache License Version 2.0 is distributed on
 #     an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 #     express or implied. See the Apache License Version 2.0 for the specific
 #     language governing permissions and limitations there under.
 # """
 
-__version_info__ = (1, 0, 0)
+__version_info__ = (1, 0, 1)
 __version__ = ".".join(str(x) for x in __version_info__)
 __build_version__ = __version__ + ""
```

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/constants.py` & `snowplow-tracker-1.0.1/snowplow_tracker/constants.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/contracts.py` & `snowplow-tracker-1.0.1/snowplow_tracker/contracts.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/emitter_configuration.py` & `snowplow-tracker-1.0.1/snowplow_tracker/emitter_configuration.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/emitters.py` & `snowplow-tracker-1.0.1/snowplow_tracker/emitters.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/event_store.py` & `snowplow-tracker-1.0.1/snowplow_tracker/event_store.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/events/__init__.py` & `snowplow-tracker-1.0.1/snowplow_tracker/events/__init__.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/events/event.py` & `snowplow-tracker-1.0.1/snowplow_tracker/events/event.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/events/page_ping.py` & `snowplow-tracker-1.0.1/snowplow_tracker/events/page_ping.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/events/page_view.py` & `snowplow-tracker-1.0.1/snowplow_tracker/events/page_view.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/events/screen_view.py` & `snowplow-tracker-1.0.1/snowplow_tracker/events/screen_view.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/events/self_describing.py` & `snowplow-tracker-1.0.1/snowplow_tracker/events/self_describing.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/events/structured_event.py` & `snowplow-tracker-1.0.1/snowplow_tracker/events/structured_event.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/payload.py` & `snowplow-tracker-1.0.1/snowplow_tracker/payload.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/self_describing_json.py` & `snowplow-tracker-1.0.1/snowplow_tracker/self_describing_json.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/snowplow.py` & `snowplow-tracker-1.0.1/snowplow_tracker/snowplow.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/subject.py` & `snowplow-tracker-1.0.1/snowplow_tracker/subject.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/tracker.py` & `snowplow-tracker-1.0.1/snowplow_tracker/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,15 +312,15 @@
         event_json = SelfDescribingJson(
             "%s/link_click/%s/1-0-1" % (BASE_SCHEMA_PATH, SCHEMA_TAG), properties
         )
 
         self.track_self_describing_event(
             event_json=event_json,
             context=context,
-            true_timestamp=tstamp,
+            tstamp=tstamp,
             event_subject=event_subject,
         )
         return self
 
     def track_add_to_cart(
         self,
         sku: str,
@@ -376,15 +376,15 @@
         event_json = SelfDescribingJson(
             "%s/add_to_cart/%s/1-0-0" % (BASE_SCHEMA_PATH, SCHEMA_TAG), properties
         )
 
         self.track_self_describing_event(
             event_json=event_json,
             context=context,
-            true_timestamp=tstamp,
+            tstamp=tstamp,
             event_subject=event_subject,
         )
         return self
 
     def track_remove_from_cart(
         self,
         sku: str,
@@ -440,15 +440,15 @@
         event_json = SelfDescribingJson(
             "%s/remove_from_cart/%s/1-0-0" % (BASE_SCHEMA_PATH, SCHEMA_TAG), properties
         )
 
         self.track_self_describing_event(
             event_json=event_json,
             context=context,
-            true_timestamp=tstamp,
+            tstamp=tstamp,
             event_subject=event_subject,
         )
         return self
 
     def track_form_change(
         self,
         form_id: str,
@@ -506,15 +506,15 @@
         event_json = SelfDescribingJson(
             "%s/change_form/%s/1-0-0" % (BASE_SCHEMA_PATH, SCHEMA_TAG), properties
         )
 
         self.track_self_describing_event(
             event_json=event_json,
             context=context,
-            true_timestamp=tstamp,
+            tstamp=tstamp,
             event_subject=event_subject,
         )
         return self
 
     def track_form_submit(
         self,
         form_id: str,
@@ -559,15 +559,15 @@
         event_json = SelfDescribingJson(
             "%s/submit_form/%s/1-0-0" % (BASE_SCHEMA_PATH, SCHEMA_TAG), properties
         )
 
         self.track_self_describing_event(
             event_json=event_json,
             context=context,
-            true_timestamp=tstamp,
+            tstamp=tstamp,
             event_subject=event_subject,
         )
         return self
 
     def track_site_search(
         self,
         terms: Sequence[str],
@@ -614,15 +614,15 @@
         event_json = SelfDescribingJson(
             "%s/site_search/%s/1-0-0" % (BASE_SCHEMA_PATH, SCHEMA_TAG), properties
         )
 
         self.track_self_describing_event(
             event_json=event_json,
             context=context,
-            true_timestamp=tstamp,
+            tstamp=tstamp,
             event_subject=event_subject,
         )
         return self
 
     def track_ecommerce_transaction_item(
         self,
         order_id: str,
@@ -803,15 +803,15 @@
             "%s/screen_view/%s/1-0-0" % (BASE_SCHEMA_PATH, SCHEMA_TAG),
             screen_view_properties,
         )
 
         self.track_self_describing_event(
             event_json=event_json,
             context=context,
-            true_timestamp=tstamp,
+            tstamp=tstamp,
             event_subject=event_subject,
         )
         return self
 
     def track_mobile_screen_view(
         self,
         name: str,
@@ -988,15 +988,15 @@
             DeprecationWarning,
             stacklevel=2,
         )
 
         self.track_self_describing_event(
             event_json=event_json,
             context=context,
-            true_timestamp=tstamp,
+            tstamp=tstamp,
             event_subject=event_subject,
         )
         return self
 
     def flush(self, is_async: bool = False) -> "Tracker":
         """
         Flush the emitter
```

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/tracker_configuration.py` & `snowplow-tracker-1.0.1/snowplow_tracker/tracker_configuration.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker/typing.py` & `snowplow-tracker-1.0.1/snowplow_tracker/typing.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker.egg-info/PKG-INFO` & `snowplow-tracker-1.0.1/snowplow_tracker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowplow-tracker
-Version: 1.0.0
+Version: 1.0.1
 Summary: Snowplow event tracker for Python. Add analytics to your Python and Django apps, webapps and games
 Home-page: http://snowplow.io
 Author: Anuj More, Alexander Dean, Fred Blundun, Paul Boocock, Matus Tomlein, Jack Keene
 Author-email: support@snowplow.io
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `snowplow-tracker-1.0.0/snowplow_tracker.egg-info/SOURCES.txt` & `snowplow-tracker-1.0.1/snowplow_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*


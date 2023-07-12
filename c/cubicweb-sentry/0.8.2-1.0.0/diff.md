# Comparing `tmp/cubicweb-sentry-0.8.2.tar.gz` & `tmp/cubicweb-sentry-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-sentry-0.8.2.tar", last modified: Wed Jun 21 15:46:35 2023, max compression
+gzip compressed data, was "cubicweb-sentry-1.0.0.tar", last modified: Wed Jul 12 10:53:29 2023, max compression
```

## Comparing `cubicweb-sentry-0.8.2.tar` & `cubicweb-sentry-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nspanti   (1000) nspanti   (1000)        0 2023-06-21 15:46:35.548277 cubicweb-sentry-0.8.2/
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)      313 2023-06-13 15:36:55.000000 cubicweb-sentry-0.8.2/MANIFEST.in
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)      989 2023-06-21 15:46:35.548277 cubicweb-sentry-0.8.2/PKG-INFO
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)      311 2023-06-20 13:53:01.000000 cubicweb-sentry-0.8.2/README.md
-drwxr-xr-x   0 nspanti   (1000) nspanti   (1000)        0 2023-06-21 15:46:35.548277 cubicweb-sentry-0.8.2/cubicweb_sentry/
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)     1125 2023-06-13 15:36:55.000000 cubicweb-sentry-0.8.2/cubicweb_sentry/__init__.py
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)      776 2023-06-20 13:53:01.000000 cubicweb-sentry-0.8.2/cubicweb_sentry/__pkginfo__.py
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)      890 2023-06-13 15:36:55.000000 cubicweb-sentry-0.8.2/cubicweb_sentry/entities.py
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)     1166 2023-06-13 15:36:55.000000 cubicweb-sentry-0.8.2/cubicweb_sentry/site_cubicweb.py
-drwxr-xr-x   0 nspanti   (1000) nspanti   (1000)        0 2023-06-21 15:46:35.548277 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)      989 2023-06-21 15:46:35.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/PKG-INFO
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)      432 2023-06-21 15:46:35.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/SOURCES.txt
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)        1 2023-06-21 15:46:35.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/dependency_links.txt
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)       43 2023-06-21 15:46:35.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/entry_points.txt
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)        1 2023-06-20 13:34:43.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/not-zip-safe
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)       43 2023-06-21 15:46:35.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/requires.txt
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)       16 2023-06-21 15:46:35.000000 cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/top_level.txt
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)       38 2023-06-21 15:46:35.548277 cubicweb-sentry-0.8.2/setup.cfg
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)     2604 2023-06-20 15:46:41.000000 cubicweb-sentry-0.8.2/setup.py
--rw-r--r--   0 nspanti   (1000) nspanti   (1000)     1021 2023-06-13 15:36:55.000000 cubicweb-sentry-0.8.2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:53:29.726749 cubicweb-sentry-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-07-12 10:52:04.000000 cubicweb-sentry-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      846 2023-07-12 10:53:29.726749 cubicweb-sentry-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-07-12 10:52:04.000000 cubicweb-sentry-1.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:53:29.722749 cubicweb-sentry-1.0.0/cubicweb_sentry/
+-rw-rw-rw-   0 root         (0) root         (0)     1125 2023-07-12 10:52:04.000000 cubicweb-sentry-1.0.0/cubicweb_sentry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      771 2023-07-12 10:52:04.000000 cubicweb-sentry-1.0.0/cubicweb_sentry/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2023-07-12 10:52:04.000000 cubicweb-sentry-1.0.0/cubicweb_sentry/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2023-07-12 10:52:04.000000 cubicweb-sentry-1.0.0/cubicweb_sentry/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:53:29.726749 cubicweb-sentry-1.0.0/cubicweb_sentry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      846 2023-07-12 10:53:29.000000 cubicweb-sentry-1.0.0/cubicweb_sentry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2023-07-12 10:53:29.000000 cubicweb-sentry-1.0.0/cubicweb_sentry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 10:53:29.000000 cubicweb-sentry-1.0.0/cubicweb_sentry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-12 10:53:29.000000 cubicweb-sentry-1.0.0/cubicweb_sentry.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 10:53:29.000000 cubicweb-sentry-1.0.0/cubicweb_sentry.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2023-07-12 10:53:29.000000 cubicweb-sentry-1.0.0/cubicweb_sentry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-12 10:53:29.000000 cubicweb-sentry-1.0.0/cubicweb_sentry.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 10:53:29.726749 cubicweb-sentry-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-12 10:52:04.000000 cubicweb-sentry-1.0.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2023-07-12 10:52:04.000000 cubicweb-sentry-1.0.0/tox.ini
```

### Comparing `cubicweb-sentry-0.8.2/PKG-INFO` & `cubicweb-sentry-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cubicweb-sentry
-Version: 0.8.2
+Version: 1.0.0
 Summary: support for Sentry (getsentry.com)
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-sentry
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Description: # CubicWeb-Sentry
-        
-        ## Summary
-        
-        This cube add support of [Sentry](https://sentry.io/) for [CubicWeb](https://www.cubicweb.org/). It is a plug-in for the framework.
-        
-        ## Install it
-        
-        1. `pip3 install cubicweb-sentry`
-        2. `add_cube("sentry")`.
-        
-        ## Configure it
-        
-        See `~/etc/cubicweb.d/<instance-name>/all-in-one.conf`
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: JavaScript
+
+# CubicWeb-Sentry
+
+## Summary
+
+This cube add support of [Sentry](https://sentry.io/) for [CubicWeb](https://www.cubicweb.org/). It is a plug-in for the framework.
+
+## Install it
+
+1. `pip3 install cubicweb-sentry`
+2. `add_cube("sentry")`.
+
+## Configure it
+
+See `~/etc/cubicweb.d/<instance-name>/all-in-one.conf`
```

### Comparing `cubicweb-sentry-0.8.2/cubicweb_sentry/__init__.py` & `cubicweb-sentry-1.0.0/cubicweb_sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-sentry-0.8.2/cubicweb_sentry/__pkginfo__.py` & `cubicweb-sentry-1.0.0/cubicweb_sentry/__pkginfo__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # pylint: disable=W0622
 """cubicweb-sentry application packaging information"""
 
 modname = "sentry"
 distname = "cubicweb-sentry"
 
-numversion = (0, 8, 2)
+numversion = (1, 0, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "support for Sentry (getsentry.com)"
-web = "https://forge.extranet.logilab.fr/cubicweb/cubes/%s" % distname
+web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
 
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: CubicWeb",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: JavaScript",
 ]
 
-__depends__ = {"cubicweb": ">= 3.38.9, < 3.39.0", "sentry-sdk": "<1.26.0"}
+__depends__ = {"cubicweb": ">= 4.0.0,< 5.0.0", "sentry-sdk": "<1.26.0"}
 __recommends__ = {}
```

### Comparing `cubicweb-sentry-0.8.2/cubicweb_sentry/entities.py` & `cubicweb-sentry-1.0.0/cubicweb_sentry/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-sentry-0.8.2/cubicweb_sentry/site_cubicweb.py` & `cubicweb-sentry-1.0.0/cubicweb_sentry/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-sentry-0.8.2/cubicweb_sentry.egg-info/PKG-INFO` & `cubicweb-sentry-1.0.0/cubicweb_sentry.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cubicweb-sentry
-Version: 0.8.2
+Version: 1.0.0
 Summary: support for Sentry (getsentry.com)
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-sentry
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Description: # CubicWeb-Sentry
-        
-        ## Summary
-        
-        This cube add support of [Sentry](https://sentry.io/) for [CubicWeb](https://www.cubicweb.org/). It is a plug-in for the framework.
-        
-        ## Install it
-        
-        1. `pip3 install cubicweb-sentry`
-        2. `add_cube("sentry")`.
-        
-        ## Configure it
-        
-        See `~/etc/cubicweb.d/<instance-name>/all-in-one.conf`
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: JavaScript
+
+# CubicWeb-Sentry
+
+## Summary
+
+This cube add support of [Sentry](https://sentry.io/) for [CubicWeb](https://www.cubicweb.org/). It is a plug-in for the framework.
+
+## Install it
+
+1. `pip3 install cubicweb-sentry`
+2. `add_cube("sentry")`.
+
+## Configure it
+
+See `~/etc/cubicweb.d/<instance-name>/all-in-one.conf`
```

### Comparing `cubicweb-sentry-0.8.2/setup.py` & `cubicweb-sentry-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,15 @@
 # get optional metadatas
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = [
-    "{} {}".format(d, v and v or "").strip() for d, v in requires.items()
-]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
```

### Comparing `cubicweb-sentry-0.8.2/tox.ini` & `cubicweb-sentry-1.0.0/tox.ini`

 * *Files identical despite different names*


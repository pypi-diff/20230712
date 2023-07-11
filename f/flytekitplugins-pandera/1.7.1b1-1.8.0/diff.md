# Comparing `tmp/flytekitplugins-pandera-1.7.1b1.tar.gz` & `tmp/flytekitplugins-pandera-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-pandera-1.7.1b1.tar", last modified: Tue Jun 27 22:00:59 2023, max compression
+gzip compressed data, was "flytekitplugins-pandera-1.8.0.tar", last modified: Tue Jul 11 22:07:23 2023, max compression
```

## Comparing `flytekitplugins-pandera-1.7.1b1.tar` & `flytekitplugins-pandera-1.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:59.056732 flytekitplugins-pandera-1.7.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-27 22:00:59.056732 flytekitplugins-pandera-1.7.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-27 22:00:35.000000 flytekitplugins-pandera-1.7.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:59.052731 flytekitplugins-pandera-1.7.1b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:59.052731 flytekitplugins-pandera-1.7.1b1/flytekitplugins/pandera/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-27 22:00:35.000000 flytekitplugins-pandera-1.7.1b1/flytekitplugins/pandera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-06-27 22:00:35.000000 flytekitplugins-pandera-1.7.1b1/flytekitplugins/pandera/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:59.056732 flytekitplugins-pandera-1.7.1b1/flytekitplugins_pandera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-27 22:00:59.000000 flytekitplugins-pandera-1.7.1b1/flytekitplugins_pandera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-27 22:00:59.000000 flytekitplugins-pandera-1.7.1b1/flytekitplugins_pandera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:00:59.000000 flytekitplugins-pandera-1.7.1b1/flytekitplugins_pandera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:59.000000 flytekitplugins-pandera-1.7.1b1/flytekitplugins_pandera.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-27 22:00:59.000000 flytekitplugins-pandera-1.7.1b1/flytekitplugins_pandera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:59.000000 flytekitplugins-pandera-1.7.1b1/flytekitplugins_pandera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:00:59.056732 flytekitplugins-pandera-1.7.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-27 22:00:50.000000 flytekitplugins-pandera-1.7.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:23.415742 flytekitplugins-pandera-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-11 22:07:23.415742 flytekitplugins-pandera-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-11 22:06:52.000000 flytekitplugins-pandera-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:23.411742 flytekitplugins-pandera-1.8.0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:23.415742 flytekitplugins-pandera-1.8.0/flytekitplugins/pandera/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 22:06:52.000000 flytekitplugins-pandera-1.8.0/flytekitplugins/pandera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-11 22:06:52.000000 flytekitplugins-pandera-1.8.0/flytekitplugins/pandera/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:23.415742 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-11 22:07:23.000000 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-11 22:07:23.000000 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:07:23.000000 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:23.000000 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 22:07:23.000000 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:23.000000 flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:07:23.415742 flytekitplugins-pandera-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-11 22:07:11.000000 flytekitplugins-pandera-1.8.0/setup.py
```

### Comparing `flytekitplugins-pandera-1.7.1b1/PKG-INFO` & `flytekitplugins-pandera-1.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pandera
-Version: 1.7.1b1
+Version: 1.8.0
 Summary: Pandera plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-pandera-1.7.1b1/README.md` & `flytekitplugins-pandera-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-pandera-1.7.1b1/flytekitplugins/pandera/schema.py` & `flytekitplugins-pandera-1.8.0/flytekitplugins/pandera/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-pandera-1.7.1b1/flytekitplugins_pandera.egg-info/PKG-INFO` & `flytekitplugins-pandera-1.8.0/flytekitplugins_pandera.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pandera
-Version: 1.7.1b1
+Version: 1.8.0
 Summary: Pandera plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-pandera-1.7.1b1/setup.py` & `flytekitplugins-pandera-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "pandera"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "pandera>=0.7.1"]
 
-__version__ = "1.7.1b1"
+__version__ = "1.8.0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Pandera plugin for flytekit",
```


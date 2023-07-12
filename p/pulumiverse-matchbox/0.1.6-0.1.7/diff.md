# Comparing `tmp/pulumiverse_matchbox-0.1.6.tar.gz` & `tmp/pulumiverse_matchbox-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_matchbox-0.1.6.tar", last modified: Thu Jun 22 13:20:34 2023, max compression
+gzip compressed data, was "pulumiverse_matchbox-0.1.7.tar", last modified: Wed Jul 12 18:06:14 2023, max compression
```

## Comparing `pulumiverse_matchbox-0.1.6.tar` & `pulumiverse_matchbox-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:20:34.303060 pulumiverse_matchbox-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    19520 2023-06-22 13:20:34.303060 pulumiverse_matchbox-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:20:34.303060 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:20:34.303060 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12910 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:20:34.303060 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19520 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/pulumiverse_matchbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 13:20:34.303060 pulumiverse_matchbox-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-22 13:20:34.000000 pulumiverse_matchbox-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:06:14.975169 pulumiverse_matchbox-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    19520 2023-07-12 18:06:14.975169 pulumiverse_matchbox-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:06:14.971168 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:06:14.975169 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12910 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:06:14.975169 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19520 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/pulumiverse_matchbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:06:14.975169 pulumiverse_matchbox-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-12 18:06:14.000000 pulumiverse_matchbox-0.1.7/setup.py
```

### Comparing `pulumiverse_matchbox-0.1.6/PKG-INFO` & `pulumiverse_matchbox-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_matchbox
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Pulumi package for creating and managing the Matchbox iPXE server.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-matchbox
 Keywords: pulumi matchbox category/network
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_matchbox-0.1.6/README.md` & `pulumiverse_matchbox-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/__init__.py` & `pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/_utilities.py` & `pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/config/vars.py` & `pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/group.py` & `pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/profile.py` & `pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/profile.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_matchbox-0.1.6/pulumiverse_matchbox/provider.py` & `pulumiverse_matchbox-0.1.7/pulumiverse_matchbox/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_matchbox-0.1.6/pulumiverse_matchbox.egg-info/PKG-INFO` & `pulumiverse_matchbox-0.1.7/pulumiverse_matchbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-matchbox
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Pulumi package for creating and managing the Matchbox iPXE server.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-matchbox
 Keywords: pulumi matchbox category/network
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_matchbox-0.1.6/pulumiverse_matchbox.egg-info/SOURCES.txt` & `pulumiverse_matchbox-0.1.7/pulumiverse_matchbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_matchbox-0.1.6/setup.py` & `pulumiverse_matchbox-0.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.6"
-PLUGIN_VERSION = "0.1.6"
+VERSION = "0.1.7"
+PLUGIN_VERSION = "0.1.7"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'matchbox', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse'])
         except OSError as error:
```


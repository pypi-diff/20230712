# Comparing `tmp/progfiguration-0.0.1.tar.gz` & `tmp/progfiguration-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progfiguration-0.0.1.tar", last modified: Wed Jul 12 04:25:33 2023, max compression
+gzip compressed data, was "progfiguration-0.0.2a1.tar", last modified: Wed Jul 12 20:07:47 2023, max compression
```

## Comparing `progfiguration-0.0.1.tar` & `progfiguration-0.0.2a1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.563647 progfiguration-0.0.1/
--rw-------   0 mrled      (501) staff       (20)      923 2023-07-12 04:25:33.562933 progfiguration-0.0.1/PKG-INFO
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.533526 progfiguration-0.0.1/progfiguration/
--rw-------   0 mrled      (501) staff       (20)      504 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/__init__.py
--rw-------   0 mrled      (501) staff       (20)     2908 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/age.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.539538 progfiguration-0.0.1/progfiguration/cli/
--rw-------   0 mrled      (501) staff       (20)     3713 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/cli/__init__.py
--rw-------   0 mrled      (501) staff       (20)    21788 2023-07-11 17:10:43.000000 progfiguration-0.0.1/progfiguration/cli/progfiguration_cmd.py
--rw-------   0 mrled      (501) staff       (20)     5023 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/cmd.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.543003 progfiguration-0.0.1/progfiguration/example_site/
--rw-r--r--   0 mrled      (501) staff       (20)      345 2023-07-11 17:14:18.000000 progfiguration-0.0.1/progfiguration/example_site/__init__.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.545621 progfiguration-0.0.1/progfiguration/example_site/groups/
--rw-r--r--   0 mrled      (501) staff       (20)        0 2023-07-11 17:16:30.000000 progfiguration-0.0.1/progfiguration/example_site/groups/__init__.py
--rw-r--r--   0 mrled      (501) staff       (20)      172 2023-07-11 17:29:06.000000 progfiguration-0.0.1/progfiguration/example_site/groups/group1.py
--rw-r--r--   0 mrled      (501) staff       (20)      397 2023-07-11 17:32:05.000000 progfiguration-0.0.1/progfiguration/example_site/groups/universal.py
--rw-r--r--   0 mrled      (501) staff       (20)     1007 2023-07-11 17:29:52.000000 progfiguration-0.0.1/progfiguration/example_site/inventory.yml
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.547200 progfiguration-0.0.1/progfiguration/example_site/nodes/
--rw-r--r--   0 mrled      (501) staff       (20)        0 2023-07-11 17:16:37.000000 progfiguration-0.0.1/progfiguration/example_site/nodes/__init__.py
--rw-r--r--   0 mrled      (501) staff       (20)      353 2023-07-11 17:29:01.000000 progfiguration-0.0.1/progfiguration/example_site/nodes/node1.py
--rw-r--r--   0 mrled      (501) staff       (20)      244 2023-07-12 03:27:25.000000 progfiguration-0.0.1/progfiguration/example_site/readme.md
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.548591 progfiguration-0.0.1/progfiguration/example_site/roles/
--rw-r--r--   0 mrled      (501) staff       (20)        0 2023-07-11 17:16:43.000000 progfiguration-0.0.1/progfiguration/example_site/roles/__init__.py
--rw-r--r--   0 mrled      (501) staff       (20)      515 2023-07-11 17:26:59.000000 progfiguration-0.0.1/progfiguration/example_site/roles/settz.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.549237 progfiguration-0.0.1/progfiguration/example_site/sitelib/
--rw-r--r--   0 mrled      (501) staff       (20)        0 2023-07-11 17:37:09.000000 progfiguration-0.0.1/progfiguration/example_site/sitelib/__init__.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.551656 progfiguration-0.0.1/progfiguration/inventory/
--rw-------   0 mrled      (501) staff       (20)    14395 2023-07-11 17:11:32.000000 progfiguration-0.0.1/progfiguration/inventory/__init__.py
--rw-------   0 mrled      (501) staff       (20)      835 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/inventory/nodes.py
--rw-------   0 mrled      (501) staff       (20)     4431 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/inventory/roles.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.555014 progfiguration-0.0.1/progfiguration/localhost/
--rw-------   0 mrled      (501) staff       (20)    11080 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/localhost/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1184 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/localhost/authorized_keys.py
--rw-------   0 mrled      (501) staff       (20)     6062 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/localhost/disks.py
--rw-------   0 mrled      (501) staff       (20)     3044 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/localhost/localusers.py
--rw-------   0 mrled      (501) staff       (20)      593 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/progfigtypes.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.555798 progfiguration-0.0.1/progfiguration/remotebrute/
--rw-------   0 mrled      (501) staff       (20)     3067 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/remotebrute/__init__.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.557548 progfiguration-0.0.1/progfiguration/remoting/
--rw-------   0 mrled      (501) staff       (20)     6265 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/remoting/__init__.py
--rw-------   0 mrled      (501) staff       (20)      222 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/remoting/rfuncs.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.558579 progfiguration-0.0.1/progfiguration/sitewrapper/
--rw-r--r--   0 mrled      (501) staff       (20)      475 2023-07-11 18:05:49.000000 progfiguration-0.0.1/progfiguration/sitewrapper/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1072 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/ssh.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.559812 progfiguration-0.0.1/progfiguration/temple/
--rw-------   0 mrled      (501) staff       (20)      744 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/temple/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1406 2023-06-28 22:11:55.000000 progfiguration-0.0.1/progfiguration/version.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.538054 progfiguration-0.0.1/progfiguration.egg-info/
--rw-------   0 mrled      (501) staff       (20)      923 2023-07-12 04:25:33.000000 progfiguration-0.0.1/progfiguration.egg-info/PKG-INFO
--rw-------   0 mrled      (501) staff       (20)     1458 2023-07-12 04:25:33.000000 progfiguration-0.0.1/progfiguration.egg-info/SOURCES.txt
--rw-------   0 mrled      (501) staff       (20)        1 2023-07-12 04:25:33.000000 progfiguration-0.0.1/progfiguration.egg-info/dependency_links.txt
--rw-------   0 mrled      (501) staff       (20)       78 2023-07-12 04:25:33.000000 progfiguration-0.0.1/progfiguration.egg-info/entry_points.txt
--rw-------   0 mrled      (501) staff       (20)       74 2023-07-12 04:25:33.000000 progfiguration-0.0.1/progfiguration.egg-info/requires.txt
--rw-------   0 mrled      (501) staff       (20)       15 2023-07-12 04:25:33.000000 progfiguration-0.0.1/progfiguration.egg-info/top_level.txt
--rw-------   0 mrled      (501) staff       (20)      771 2023-07-12 04:23:28.000000 progfiguration-0.0.1/pyproject.toml
--rw-------   0 mrled      (501) staff       (20)      569 2023-07-12 04:25:13.000000 progfiguration-0.0.1/readme.md
--rw-------   0 mrled      (501) staff       (20)       38 2023-07-12 04:25:33.563944 progfiguration-0.0.1/setup.cfg
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 04:25:33.561973 progfiguration-0.0.1/tests/
--rw-------   0 mrled      (501) staff       (20)     1170 2023-06-28 22:11:56.000000 progfiguration-0.0.1/tests/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1332 2023-06-28 22:11:56.000000 progfiguration-0.0.1/tests/test_cmd.py
--rw-------   0 mrled      (501) staff       (20)     1061 2023-06-28 22:11:56.000000 progfiguration-0.0.1/tests/test_site.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.884193 progfiguration-0.0.2a1/
+-rw-------   0 mrled      (501) staff       (20)     1180 2023-07-12 20:07:47.883654 progfiguration-0.0.2a1/PKG-INFO
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.845552 progfiguration-0.0.2a1/progfiguration/
+-rw-------   0 mrled      (501) staff       (20)      504 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     2908 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/age.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.851546 progfiguration-0.0.2a1/progfiguration/cli/
+-rw-------   0 mrled      (501) staff       (20)     3713 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/cli/__init__.py
+-rw-------   0 mrled      (501) staff       (20)    21793 2023-07-12 19:14:06.000000 progfiguration-0.0.2a1/progfiguration/cli/progfiguration_cmd.py
+-rw-------   0 mrled      (501) staff       (20)     5023 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/cmd.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.855663 progfiguration-0.0.2a1/progfiguration/example_site/
+-rw-r--r--   0 mrled      (501) staff       (20)      345 2023-07-11 17:14:18.000000 progfiguration-0.0.2a1/progfiguration/example_site/__init__.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.858852 progfiguration-0.0.2a1/progfiguration/example_site/groups/
+-rw-r--r--   0 mrled      (501) staff       (20)        0 2023-07-11 17:16:30.000000 progfiguration-0.0.2a1/progfiguration/example_site/groups/__init__.py
+-rw-r--r--   0 mrled      (501) staff       (20)      172 2023-07-11 17:29:06.000000 progfiguration-0.0.2a1/progfiguration/example_site/groups/group1.py
+-rw-r--r--   0 mrled      (501) staff       (20)      397 2023-07-11 17:32:05.000000 progfiguration-0.0.2a1/progfiguration/example_site/groups/universal.py
+-rw-r--r--   0 mrled      (501) staff       (20)     1007 2023-07-11 17:29:52.000000 progfiguration-0.0.2a1/progfiguration/example_site/inventory.yml
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.860547 progfiguration-0.0.2a1/progfiguration/example_site/nodes/
+-rw-r--r--   0 mrled      (501) staff       (20)        0 2023-07-11 17:16:37.000000 progfiguration-0.0.2a1/progfiguration/example_site/nodes/__init__.py
+-rw-r--r--   0 mrled      (501) staff       (20)      395 2023-07-12 19:12:41.000000 progfiguration-0.0.2a1/progfiguration/example_site/nodes/node1.py
+-rw-r--r--   0 mrled      (501) staff       (20)      244 2023-07-12 03:27:25.000000 progfiguration-0.0.2a1/progfiguration/example_site/readme.md
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.862360 progfiguration-0.0.2a1/progfiguration/example_site/roles/
+-rw-r--r--   0 mrled      (501) staff       (20)        0 2023-07-11 17:16:43.000000 progfiguration-0.0.2a1/progfiguration/example_site/roles/__init__.py
+-rw-r--r--   0 mrled      (501) staff       (20)      515 2023-07-11 17:26:59.000000 progfiguration-0.0.2a1/progfiguration/example_site/roles/settz.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.863565 progfiguration-0.0.2a1/progfiguration/example_site/sitelib/
+-rw-r--r--   0 mrled      (501) staff       (20)        0 2023-07-11 17:37:09.000000 progfiguration-0.0.2a1/progfiguration/example_site/sitelib/__init__.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.866672 progfiguration-0.0.2a1/progfiguration/inventory/
+-rw-------   0 mrled      (501) staff       (20)    14074 2023-07-12 19:13:35.000000 progfiguration-0.0.2a1/progfiguration/inventory/__init__.py
+-rw-------   0 mrled      (501) staff       (20)      835 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/inventory/nodes.py
+-rw-------   0 mrled      (501) staff       (20)     4431 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/inventory/roles.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.871391 progfiguration-0.0.2a1/progfiguration/localhost/
+-rw-------   0 mrled      (501) staff       (20)    11080 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/localhost/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     1184 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/localhost/authorized_keys.py
+-rw-------   0 mrled      (501) staff       (20)     6062 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/localhost/disks.py
+-rw-------   0 mrled      (501) staff       (20)     3044 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/localhost/localusers.py
+-rw-------   0 mrled      (501) staff       (20)      593 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/progfigtypes.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.872860 progfiguration-0.0.2a1/progfiguration/remotebrute/
+-rw-------   0 mrled      (501) staff       (20)     3067 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/remotebrute/__init__.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.875850 progfiguration-0.0.2a1/progfiguration/remoting/
+-rw-------   0 mrled      (501) staff       (20)     6265 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/remoting/__init__.py
+-rw-------   0 mrled      (501) staff       (20)      222 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/remoting/rfuncs.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.877620 progfiguration-0.0.2a1/progfiguration/sitewrapper/
+-rw-r--r--   0 mrled      (501) staff       (20)     2271 2023-07-12 20:00:14.000000 progfiguration-0.0.2a1/progfiguration/sitewrapper/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     1072 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/ssh.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.878906 progfiguration-0.0.2a1/progfiguration/temple/
+-rw-------   0 mrled      (501) staff       (20)      744 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/temple/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     1406 2023-06-28 22:11:55.000000 progfiguration-0.0.2a1/progfiguration/version.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.849623 progfiguration-0.0.2a1/progfiguration.egg-info/
+-rw-------   0 mrled      (501) staff       (20)     1180 2023-07-12 20:07:47.000000 progfiguration-0.0.2a1/progfiguration.egg-info/PKG-INFO
+-rw-------   0 mrled      (501) staff       (20)     1458 2023-07-12 20:07:47.000000 progfiguration-0.0.2a1/progfiguration.egg-info/SOURCES.txt
+-rw-------   0 mrled      (501) staff       (20)        1 2023-07-12 20:07:47.000000 progfiguration-0.0.2a1/progfiguration.egg-info/dependency_links.txt
+-rw-------   0 mrled      (501) staff       (20)       78 2023-07-12 20:07:47.000000 progfiguration-0.0.2a1/progfiguration.egg-info/entry_points.txt
+-rw-------   0 mrled      (501) staff       (20)       82 2023-07-12 20:07:47.000000 progfiguration-0.0.2a1/progfiguration.egg-info/requires.txt
+-rw-------   0 mrled      (501) staff       (20)       15 2023-07-12 20:07:47.000000 progfiguration-0.0.2a1/progfiguration.egg-info/top_level.txt
+-rw-------   0 mrled      (501) staff       (20)      740 2023-07-12 20:06:27.000000 progfiguration-0.0.2a1/pyproject.toml
+-rw-------   0 mrled      (501) staff       (20)      823 2023-07-12 20:07:27.000000 progfiguration-0.0.2a1/readme.md
+-rw-------   0 mrled      (501) staff       (20)       38 2023-07-12 20:07:47.884378 progfiguration-0.0.2a1/setup.cfg
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-12 20:07:47.882249 progfiguration-0.0.2a1/tests/
+-rw-------   0 mrled      (501) staff       (20)     1170 2023-06-28 22:11:56.000000 progfiguration-0.0.2a1/tests/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     1332 2023-06-28 22:11:56.000000 progfiguration-0.0.2a1/tests/test_cmd.py
+-rw-------   0 mrled      (501) staff       (20)     1088 2023-07-12 04:46:25.000000 progfiguration-0.0.2a1/tests/test_site.py
```

### Comparing `progfiguration-0.0.1/PKG-INFO` & `progfiguration-0.0.2a1/readme.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: progfiguration
-Version: 0.0.1
-Summary: PROGramatic conFIGURATION for your infrastructure
-Author-email: Micah R Ledbetter <me@micahrl.com>
-License: MIT
-Project-URL: Homepage, https://github.com/mrled/progfiguration
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: ssh
-Provides-Extra: development
-
 # progfiguration
 
 PROGrammatic conFIGURATION.
 I'm tired of writing YAML when what I want to write is Python.
 
 ## Building and publishing
 
@@ -22,12 +10,18 @@
 python3 -m venv venv
 # Enter the venv
 . venv/bin/activate
 # Make sure pip is recent - required for our pyproject.toml-only package
 python3 -m pip install --upgrade pip
 # Install this directory as editable, and include development dependencies
 python3 -m pip install --editable '.[development]'
-# Build the packagej
-python3 -m build
+# Run unit tests
+python3 -m unittest
+# Build a source-only distribution of the package
+python3 -m build -s
 # Upload it to PyPI
-python3 -m twine upload --repository testpypi dist/*
+twine upload dist/*
 ```
+
+We only actually need to build a source version of the package,
+because progfiguration expects that your progfigsite package will pull in the source code.
+We avoid building the binary version because it takes longer.
```

### Comparing `progfiguration-0.0.1/progfiguration/age.py` & `progfiguration-0.0.2a1/progfiguration/age.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/cli/__init__.py` & `progfiguration-0.0.2a1/progfiguration/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/cli/progfiguration_cmd.py` & `progfiguration-0.0.2a1/progfiguration/cli/progfiguration_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
         default="CRITICAL",
         choices=progfiguration_log_levels,
         help="Log level for mitogen IO messages to stderr. Only used for remote commands from the controller.",
     )
     parser.add_argument(
         "--inventory-file",
         "-f",
-        default=sitewrapper.package_inventory_file,
+        default=sitewrapper.site.package_inventory_file,
         help="The path to an inventory yaml file. By default, use the one in the package",
     )
     parser.add_argument(
         "--age-private-key", "-k", help="The path to an age private key that decrypts inventory secrets"
     )
 
     # node/group related options
```

### Comparing `progfiguration-0.0.1/progfiguration/cmd.py` & `progfiguration-0.0.2a1/progfiguration/cmd.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/example_site/inventory.yml` & `progfiguration-0.0.2a1/progfiguration/example_site/inventory.yml`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/example_site/roles/settz.py` & `progfiguration-0.0.2a1/progfiguration/example_site/roles/settz.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/inventory/__init__.py` & `progfiguration-0.0.2a1/progfiguration/inventory/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """The progfiguration inventory"""
 
 from dataclasses import dataclass
 import os
-import importlib
 from importlib.abc import Traversable
-from importlib.resources import files as importlib_resources_files
 from pathlib import Path
 from types import ModuleType
 from typing import Any, Dict, List, Optional
 
 import yaml
 
 from progfiguration import age
 from progfiguration.inventory.roles import ProgfigurationRole, collect_role_arguments
 from progfiguration.localhost import LocalhostLinuxPsyopsOs
 from progfiguration.progfigtypes import AnyPathOrStr
+from progfiguration import sitewrapper
 
 
 @dataclass
 class Controller:
     age: Optional[age.AgeKey]
     agepub: str
     agepath: str
@@ -164,29 +163,29 @@
     def node_rolename_list(self, nodename: str) -> List[str]:
         """A list of all rolenames for a given node"""
         return self.function_roles[self.node_function[nodename]]
 
     def node(self, name: str) -> ModuleType:
         """The Python module for a given node"""
         if name not in self._node_modules:
-            module = importlib.import_module(f"progfiguration.sitewrapper.nodes.{name}")
+            module = sitewrapper.site_submodule(f"nodes.{name}")
             self._node_modules[name] = module
         return self._node_modules[name]
 
     def group(self, name: str) -> ModuleType:
         """The Python module for a given group"""
         if name not in self._group_modules:
-            module = importlib.import_module(f"progfiguration.sitewrapper.groups.{name}")
+            module = sitewrapper.site_submodule(f"groups.{name}")
             self._group_modules[name] = module
         return self._group_modules[name]
 
     def role_module(self, name: str) -> ModuleType:
         """The Python module for a given role"""
         if name not in self._role_modules:
-            module = importlib.import_module(f"progfiguration.sitewrapper.roles.{name}")
+            module = sitewrapper.site_submodule(f"roles.{name}")
             self._role_modules[name] = module
         return self._role_modules[name]
 
     def node_role(self, nodename: str, rolename: str) -> ProgfigurationRole:
         """A dict of {nodename: {rolename: ProgfigurationRole}}
 
         Get an instantiated ProgfigurationRole object for a given node and role.
@@ -199,15 +198,15 @@
 
         Results are cached for subsequent calls.
         """
         if nodename not in self._node_roles:
             self._node_roles[nodename] = {}
         if rolename not in self._node_roles[nodename]:
 
-            # rolepkg is a string containing the package name of the role, like progfiguration.sitewrapper.roles.role_name
+            # rolepkg is a string containing the package name of the role, like progfiguration.sitewrapper.site.roles.role_name
             rolepkg = self.role_module(rolename).__package__
 
             # The class it the subclass of ProgfigurationRole that implements the role
             role_cls = self.role_module(rolename).Role
 
             # Get a list of all the groups this node is a member of so that we can get any role arg definitions they may have
             groupmods = {}
@@ -253,45 +252,45 @@
                 return encrypted_secrets
         except FileNotFoundError:
             return {}
 
     def get_node_secrets(self, nodename: str) -> Dict[str, Any]:
         """A Dict of secrets for a given node"""
         if nodename not in self._node_secrets:
-            sfile = importlib_resources_files("progfiguration.sitewrapper.nodes").joinpath(f"{nodename}.secrets.yml")
-            self._node_secrets[nodename] = self.get_secrets(sfile)
+            self._node_secrets[nodename] = self.get_secrets(self.node_secrets_file(nodename))
         return self._node_secrets[nodename]
 
     def get_group_secrets(self, groupname: str) -> Dict[str, Any]:
         """A Dict of secrets for a given group"""
         if groupname not in self._group_secrets:
-            sfile = importlib_resources_files("progfiguration.sitewrapper.groups").joinpath(f"{groupname}.secrets.yml")
-            self._group_secrets[groupname] = self.get_secrets(sfile)
+            self._group_secrets[groupname] = self.get_secrets(self.group_secrets_file(groupname))
         return self._group_secrets[groupname]
 
     def get_controller_secrets(self) -> Dict[str, Any]:
         """A Dict of secrets for the controller"""
         if not self._controller_secrets:
-            sfile = importlib_resources_files("progfiguration.site").joinpath(f"controller.secrets.yml")
+            sfile = sitewrapper.site_submodule_resource("", "controller.secrets.yml")
             self._controller_secrets = self.get_secrets(sfile)
         return self._controller_secrets
 
     def _set_secrets(self, filename: str, secrets: Dict[str, age.AgeSecret]):
         """Set the contents of a secrets file"""
         file_contents = {k: v.secret for k, v in secrets.items()}
         with open(filename, "w") as fp:
             yaml.dump(file_contents, fp, default_style="|")
 
     def group_secrets_file(self, group: str) -> Path:
         """The path to the secrets file for a given group"""
-        return importlib_resources_files("progfiguration.sitewrapper.groups").joinpath(f"{group}.secrets.yml")
+        sfile = sitewrapper.site_submodule_resource("groups", f"{group}.secrets.yml")
+        return sfile
 
     def node_secrets_file(self, node: str) -> Path:
         """The path to the secrets file for a given node"""
-        return importlib_resources_files("progfiguration.sitewrapper.nodes").joinpath(f"{node}.secrets.yml")
+        sfile = sitewrapper.site_submodule_resource("nodes", f"{node}.secrets.yml")
+        return sfile
 
     def set_node_secret(self, nodename: str, secretname: str, encrypted_value: str):
         """Set a secret for a node"""
         self.get_node_secrets(nodename)  # Ensure it's cached
         self._node_secrets[nodename][secretname] = age.AgeSecret(encrypted_value)
         self._set_secrets(self.node_secrets_file(nodename), self._node_secrets[nodename])
```

### Comparing `progfiguration-0.0.1/progfiguration/inventory/nodes.py` & `progfiguration-0.0.2a1/progfiguration/inventory/nodes.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/inventory/roles.py` & `progfiguration-0.0.2a1/progfiguration/inventory/roles.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/localhost/__init__.py` & `progfiguration-0.0.2a1/progfiguration/localhost/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/localhost/authorized_keys.py` & `progfiguration-0.0.2a1/progfiguration/localhost/authorized_keys.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/localhost/disks.py` & `progfiguration-0.0.2a1/progfiguration/localhost/disks.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/localhost/localusers.py` & `progfiguration-0.0.2a1/progfiguration/localhost/localusers.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/progfigtypes.py` & `progfiguration-0.0.2a1/progfiguration/progfigtypes.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/remotebrute/__init__.py` & `progfiguration-0.0.2a1/progfiguration/remotebrute/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/remoting/__init__.py` & `progfiguration-0.0.2a1/progfiguration/remoting/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/ssh.py` & `progfiguration-0.0.2a1/progfiguration/ssh.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/temple/__init__.py` & `progfiguration-0.0.2a1/progfiguration/temple/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration/version.py` & `progfiguration-0.0.2a1/progfiguration/version.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/progfiguration.egg-info/SOURCES.txt` & `progfiguration-0.0.2a1/progfiguration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/pyproject.toml` & `progfiguration-0.0.2a1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 [build-system]
 requires = [
-    "build",
-    "installer",
     "setuptools",
-    "twine",
-    "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "progfiguration"
-version = "0.0.1"
+version = "0.0.2a1"
 description = "PROGramatic conFIGURATION for your infrastructure"
 license = {text = "MIT"}
 readme = "readme.md"
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 dependencies = [
     "PyYAML",
     "pytz",
     "requests",
 ]
 
 [[project.authors]]
 name = "Micah R Ledbetter"
 email = "me@micahrl.com"
 
 [project.scripts]
 progfiguration = "progfiguration.cli.progfiguration_cmd:main"
 
 [project.optional-dependencies]
-ssh = ["mitogen"]
+ssh = [
+    "mitogen",
+]
 development = [
     "black",
     "build",
+    "mitogen",
     "mypy",
     "twine",
 ]
 
 [project.urls]
 Homepage = "https://github.com/mrled/progfiguration"
```

### Comparing `progfiguration-0.0.1/tests/__init__.py` & `progfiguration-0.0.2a1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/tests/test_cmd.py` & `progfiguration-0.0.2a1/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.1/tests/test_site.py` & `progfiguration-0.0.2a1/tests/test_site.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Site-specific tests"""
 
 import pdb
 import unittest
 
-from progfiguration import site
+from progfiguration import sitewrapper
 from progfiguration.inventory import Inventory
 
 from tests import PdbTestCase, pdbexc
 
 
 class TestRun(PdbTestCase):
     @classmethod
     @pdbexc
     def setUpClass(cls):
-        cls.inventory = Inventory(site.package_inventory_file, None)
-        if not cls.inventory.controller.age:
-            raise Exception(
-                "Controller age is not set - are you running this from the controller with a decrypted secrets volume?"
-            )
+        cls.inventory = Inventory(sitewrapper.site.package_inventory_file, None)
+        # if not cls.inventory.controller.age:
+        #     raise Exception(
+        #         "Controller age is not set - are you running this from the controller with a decrypted secrets volume?"
+        #     )
 
     @pdbexc
     def test_inventory_all_roles(self):
         """Test that all roles can be instantiated
 
         Instantiation requires decrypting secrets (which requires the controller age),
         and properly dereferencing secrets and role results.
```


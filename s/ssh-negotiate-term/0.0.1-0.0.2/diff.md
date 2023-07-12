# Comparing `tmp/ssh_negotiate_term-0.0.1.tar.gz` & `tmp/ssh_negotiate_term-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_negotiate_term-0.0.1.tar", last modified: Wed Jul 12 01:15:05 2023, max compression
+gzip compressed data, was "ssh_negotiate_term-0.0.2.tar", last modified: Wed Jul 12 01:23:33 2023, max compression
```

## Comparing `ssh_negotiate_term-0.0.1.tar` & `ssh_negotiate_term-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tejr      (1000) tejr      (1000)        0 2023-07-12 01:15:05.769340 ssh_negotiate_term-0.0.1/
--rw-r--r--   0 tejr      (1000) tejr      (1000)    35149 2023-07-12 01:08:43.000000 ssh_negotiate_term-0.0.1/LICENSE
--rw-r--r--   0 tejr      (1000) tejr      (1000)      901 2023-07-12 01:15:05.769340 ssh_negotiate_term-0.0.1/PKG-INFO
--rw-r--r--   0 tejr      (1000) tejr      (1000)      332 2023-07-12 01:08:43.000000 ssh_negotiate_term-0.0.1/README.md
--rw-r--r--   0 tejr      (1000) tejr      (1000)      709 2023-07-12 01:08:43.000000 ssh_negotiate_term-0.0.1/pyproject.toml
--rw-r--r--   0 tejr      (1000) tejr      (1000)       38 2023-07-12 01:15:05.769340 ssh_negotiate_term-0.0.1/setup.cfg
-drwxr-xr-x   0 tejr      (1000) tejr      (1000)        0 2023-07-12 01:15:05.757340 ssh_negotiate_term-0.0.1/src/
-drwxr-xr-x   0 tejr      (1000) tejr      (1000)        0 2023-07-12 01:15:05.765340 ssh_negotiate_term-0.0.1/src/ssh_negotiate_term.egg-info/
--rw-r--r--   0 tejr      (1000) tejr      (1000)      901 2023-07-12 01:15:05.000000 ssh_negotiate_term-0.0.1/src/ssh_negotiate_term.egg-info/PKG-INFO
--rw-r--r--   0 tejr      (1000) tejr      (1000)      324 2023-07-12 01:15:05.000000 ssh_negotiate_term-0.0.1/src/ssh_negotiate_term.egg-info/SOURCES.txt
--rw-r--r--   0 tejr      (1000) tejr      (1000)        1 2023-07-12 01:15:05.000000 ssh_negotiate_term-0.0.1/src/ssh_negotiate_term.egg-info/dependency_links.txt
--rw-r--r--   0 tejr      (1000) tejr      (1000)       63 2023-07-12 01:15:05.000000 ssh_negotiate_term-0.0.1/src/ssh_negotiate_term.egg-info/entry_points.txt
--rw-r--r--   0 tejr      (1000) tejr      (1000)       19 2023-07-12 01:15:05.000000 ssh_negotiate_term-0.0.1/src/ssh_negotiate_term.egg-info/top_level.txt
--rw-r--r--   0 tejr      (1000) tejr      (1000)     4967 2023-07-12 01:08:43.000000 ssh_negotiate_term-0.0.1/src/ssh_negotiate_term.py
-drwxr-xr-x   0 tejr      (1000) tejr      (1000)        0 2023-07-12 01:15:05.765340 ssh_negotiate_term-0.0.1/tests/
--rw-r--r--   0 tejr      (1000) tejr      (1000)     3964 2023-07-12 01:08:43.000000 ssh_negotiate_term-0.0.1/tests/test_ssh_negotiate_term.py
+drwxr-xr-x   0 tejr      (1000) tejr      (1000)        0 2023-07-12 01:23:33.201235 ssh_negotiate_term-0.0.2/
+-rw-r--r--   0 tejr      (1000) tejr      (1000)    35149 2023-07-12 01:08:43.000000 ssh_negotiate_term-0.0.2/LICENSE
+-rw-r--r--   0 tejr      (1000) tejr      (1000)      906 2023-07-12 01:23:33.197235 ssh_negotiate_term-0.0.2/PKG-INFO
+-rw-r--r--   0 tejr      (1000) tejr      (1000)      332 2023-07-12 01:08:43.000000 ssh_negotiate_term-0.0.2/README.md
+-rw-r--r--   0 tejr      (1000) tejr      (1000)      714 2023-07-12 01:20:47.000000 ssh_negotiate_term-0.0.2/pyproject.toml
+-rw-r--r--   0 tejr      (1000) tejr      (1000)       38 2023-07-12 01:23:33.201235 ssh_negotiate_term-0.0.2/setup.cfg
+drwxr-xr-x   0 tejr      (1000) tejr      (1000)        0 2023-07-12 01:23:33.193235 ssh_negotiate_term-0.0.2/src/
+drwxr-xr-x   0 tejr      (1000) tejr      (1000)        0 2023-07-12 01:23:33.197235 ssh_negotiate_term-0.0.2/src/ssh_negotiate_term.egg-info/
+-rw-r--r--   0 tejr      (1000) tejr      (1000)      906 2023-07-12 01:23:33.000000 ssh_negotiate_term-0.0.2/src/ssh_negotiate_term.egg-info/PKG-INFO
+-rw-r--r--   0 tejr      (1000) tejr      (1000)      324 2023-07-12 01:23:33.000000 ssh_negotiate_term-0.0.2/src/ssh_negotiate_term.egg-info/SOURCES.txt
+-rw-r--r--   0 tejr      (1000) tejr      (1000)        1 2023-07-12 01:23:33.000000 ssh_negotiate_term-0.0.2/src/ssh_negotiate_term.egg-info/dependency_links.txt
+-rw-r--r--   0 tejr      (1000) tejr      (1000)       63 2023-07-12 01:23:33.000000 ssh_negotiate_term-0.0.2/src/ssh_negotiate_term.egg-info/entry_points.txt
+-rw-r--r--   0 tejr      (1000) tejr      (1000)       19 2023-07-12 01:23:33.000000 ssh_negotiate_term-0.0.2/src/ssh_negotiate_term.egg-info/top_level.txt
+-rw-r--r--   0 tejr      (1000) tejr      (1000)     4967 2023-07-12 01:08:43.000000 ssh_negotiate_term-0.0.2/src/ssh_negotiate_term.py
+drwxr-xr-x   0 tejr      (1000) tejr      (1000)        0 2023-07-12 01:23:33.197235 ssh_negotiate_term-0.0.2/tests/
+-rw-r--r--   0 tejr      (1000) tejr      (1000)     3964 2023-07-12 01:08:43.000000 ssh_negotiate_term-0.0.2/tests/test_ssh_negotiate_term.py
```

### Comparing `ssh_negotiate_term-0.0.1/LICENSE` & `ssh_negotiate_term-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_negotiate_term-0.0.1/PKG-INFO` & `ssh_negotiate_term-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ssh_negotiate_term
-Version: 0.0.1
+Version: 0.0.2
 Summary: Downgrade TERM strings when connecting to selected SSH servers
 Author-email: Tom Ryder <tom@sanctum.geek.nz>
 Project-URL: Homepage, https://sanctum.geek.nz/
-Project-URL: Source, https://dev.sanctum.geek.nz/ssh_negotiate_term.git/
+Project-URL: Source, https://dev.sanctum.geek.nz/cgit/ssh_negotiate_term.git/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ssh_negotiate_term-0.0.1/pyproject.toml` & `ssh_negotiate_term-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_negotiate_term"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Tom Ryder", email="tom@sanctum.geek.nz" },
 ]
 description = "Downgrade TERM strings when connecting to selected SSH servers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,8 +18,8 @@
 ]
 
 [project.scripts]
 ssh-negotiate-term = "ssh_negotiate_term:main"
 
 [project.urls]
 "Homepage" = "https://sanctum.geek.nz/"
-"Source" = "https://dev.sanctum.geek.nz/ssh_negotiate_term.git/"
+"Source" = "https://dev.sanctum.geek.nz/cgit/ssh_negotiate_term.git/"
```

### Comparing `ssh_negotiate_term-0.0.1/src/ssh_negotiate_term.egg-info/PKG-INFO` & `ssh_negotiate_term-0.0.2/src/ssh_negotiate_term.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ssh-negotiate-term
-Version: 0.0.1
+Version: 0.0.2
 Summary: Downgrade TERM strings when connecting to selected SSH servers
 Author-email: Tom Ryder <tom@sanctum.geek.nz>
 Project-URL: Homepage, https://sanctum.geek.nz/
-Project-URL: Source, https://dev.sanctum.geek.nz/ssh_negotiate_term.git/
+Project-URL: Source, https://dev.sanctum.geek.nz/cgit/ssh_negotiate_term.git/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ssh_negotiate_term-0.0.1/src/ssh_negotiate_term.py` & `ssh_negotiate_term-0.0.2/src/ssh_negotiate_term.py`

 * *Files identical despite different names*

### Comparing `ssh_negotiate_term-0.0.1/tests/test_ssh_negotiate_term.py` & `ssh_negotiate_term-0.0.2/tests/test_ssh_negotiate_term.py`

 * *Files identical despite different names*


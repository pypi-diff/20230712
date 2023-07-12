# Comparing `tmp/saracenpypacks-1.1.tar.gz` & `tmp/saracenpypacks-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saracenpypacks-1.1.tar", last modified: Wed Jul 12 14:23:58 2023, max compression
+gzip compressed data, was "saracenpypacks-1.2.tar", last modified: Wed Jul 12 14:25:37 2023, max compression
```

## Comparing `saracenpypacks-1.1.tar` & `saracenpypacks-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 14:23:58.542366 saracenpypacks-1.1/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      449 2023-07-12 14:23:58.542228 saracenpypacks-1.1/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       17 2023-07-12 14:19:13.000000 saracenpypacks-1.1/README.md
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 14:23:58.541297 saracenpypacks-1.1/saracenpypacks/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 14:23:40.000000 saracenpypacks-1.1/saracenpypacks/__init__.py
-drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 14:23:58.542030 saracenpypacks-1.1/saracenpypacks.egg-info/
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      449 2023-07-12 14:23:58.000000 saracenpypacks-1.1/saracenpypacks.egg-info/PKG-INFO
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      234 2023-07-12 14:23:58.000000 saracenpypacks-1.1/saracenpypacks.egg-info/SOURCES.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-12 14:23:58.000000 saracenpypacks-1.1/saracenpypacks.egg-info/dependency_links.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      113 2023-07-12 14:23:58.000000 saracenpypacks-1.1/saracenpypacks.egg-info/requires.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       15 2023-07-12 14:23:58.000000 saracenpypacks-1.1/saracenpypacks.egg-info/top_level.txt
--rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-12 14:23:58.542403 saracenpypacks-1.1/setup.cfg
--rw-r--r--   0 richardkammermeier   (501) staff       (20)      995 2023-07-12 14:21:55.000000 saracenpypacks-1.1/setup.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 14:25:37.857357 saracenpypacks-1.2/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      449 2023-07-12 14:25:37.857230 saracenpypacks-1.2/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       17 2023-07-12 14:19:13.000000 saracenpypacks-1.2/README.md
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 14:25:37.856263 saracenpypacks-1.2/saracenpypacks/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 14:23:40.000000 saracenpypacks-1.2/saracenpypacks/__init__.py
+drwxr-xr-x   0 richardkammermeier   (501) staff       (20)        0 2023-07-12 14:25:37.857031 saracenpypacks-1.2/saracenpypacks.egg-info/
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      449 2023-07-12 14:25:37.000000 saracenpypacks-1.2/saracenpypacks.egg-info/PKG-INFO
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      234 2023-07-12 14:25:37.000000 saracenpypacks-1.2/saracenpypacks.egg-info/SOURCES.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)        1 2023-07-12 14:25:37.000000 saracenpypacks-1.2/saracenpypacks.egg-info/dependency_links.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      106 2023-07-12 14:25:37.000000 saracenpypacks-1.2/saracenpypacks.egg-info/requires.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       15 2023-07-12 14:25:37.000000 saracenpypacks-1.2/saracenpypacks.egg-info/top_level.txt
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)       38 2023-07-12 14:25:37.857393 saracenpypacks-1.2/setup.cfg
+-rw-r--r--   0 richardkammermeier   (501) staff       (20)      995 2023-07-12 14:25:24.000000 saracenpypacks-1.2/setup.py
```

### Comparing `saracenpypacks-1.1/setup.py` & `saracenpypacks-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 with open("packages.json", "r") as f:
     packages = json.load(f)
 
-VERSION = '1.1'
+VERSION = '1.2'
 DESCRIPTION = ''
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="saracenpypacks",
     version=VERSION,
```


# Comparing `tmp/ki-aikido-0.0.1.tar.gz` & `tmp/ki-aikido-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ki-aikido-0.0.1.tar", last modified: Wed Jul 12 12:57:33 2023, max compression
+gzip compressed data, was "ki-aikido-0.0.2.tar", last modified: Wed Jul 12 13:39:06 2023, max compression
```

## Comparing `ki-aikido-0.0.1.tar` & `ki-aikido-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwx------   0 gabrielfalcao   (501) staff       (20)        0 2023-07-12 12:57:33.972627 ki-aikido-0.0.1/
--rw-------   0 gabrielfalcao   (501) staff       (20)    35149 2023-07-12 00:33:58.000000 ki-aikido-0.0.1/COPYING
--rw-------   0 gabrielfalcao   (501) staff       (20)      617 2023-07-12 08:09:14.000000 ki-aikido-0.0.1/Cargo.toml
--rw-r--r--   0 gabrielfalcao   (501) staff       (20)      119 2023-07-12 07:43:44.000000 ki-aikido-0.0.1/MANIFEST.in
--rw-------   0 gabrielfalcao   (501) staff       (20)     2024 2023-07-12 12:57:33.972488 ki-aikido-0.0.1/PKG-INFO
--rw-------   0 gabrielfalcao   (501) staff       (20)      214 2023-07-12 08:05:37.000000 ki-aikido-0.0.1/README.rst
-drwx------   0 gabrielfalcao   (501) staff       (20)        0 2023-07-12 12:57:33.967986 ki-aikido-0.0.1/docs/
-drwx------   0 gabrielfalcao   (501) staff       (20)        0 2023-07-12 12:57:33.970653 ki-aikido-0.0.1/docs/source/
--rw-------   0 gabrielfalcao   (501) staff       (20)     1011 2023-07-12 02:11:02.000000 ki-aikido-0.0.1/docs/source/conf.py
--rw-------   0 gabrielfalcao   (501) staff       (20)      329 2023-07-12 07:36:39.000000 ki-aikido-0.0.1/docs/source/index.rst
--rw-r--r--   0 gabrielfalcao   (501) staff       (20)      294 2023-07-12 06:43:32.000000 ki-aikido-0.0.1/docs/source/setting-up.rst
-drwx------   0 gabrielfalcao   (501) staff       (20)        0 2023-07-12 12:57:33.971554 ki-aikido-0.0.1/ki_aikido.egg-info/
--rw-------   0 gabrielfalcao   (501) staff       (20)     2024 2023-07-12 12:57:33.000000 ki-aikido-0.0.1/ki_aikido.egg-info/PKG-INFO
--rw-------   0 gabrielfalcao   (501) staff       (20)      346 2023-07-12 12:57:33.000000 ki-aikido-0.0.1/ki_aikido.egg-info/SOURCES.txt
--rw-------   0 gabrielfalcao   (501) staff       (20)        1 2023-07-12 12:57:33.000000 ki-aikido-0.0.1/ki_aikido.egg-info/dependency_links.txt
--rw-------   0 gabrielfalcao   (501) staff       (20)       41 2023-07-12 12:57:33.000000 ki-aikido-0.0.1/ki_aikido.egg-info/entry_points.txt
--rw-------   0 gabrielfalcao   (501) staff       (20)        4 2023-07-12 12:57:33.000000 ki-aikido-0.0.1/ki_aikido.egg-info/top_level.txt
--rw-------   0 gabrielfalcao   (501) staff       (20)        0 2023-07-12 07:38:37.000000 ki-aikido-0.0.1/requirements.txt
--rw-------   0 gabrielfalcao   (501) staff       (20)       38 2023-07-12 12:57:33.972679 ki-aikido-0.0.1/setup.cfg
--rwx------   0 gabrielfalcao   (501) staff       (20)     4978 2023-07-12 12:55:59.000000 ki-aikido-0.0.1/setup.py
-drwx------   0 gabrielfalcao   (501) staff       (20)        0 2023-07-12 12:57:33.972246 ki-aikido-0.0.1/src/
--rw-r--r--   0 gabrielfalcao   (501) staff       (20)       24 2023-07-12 01:40:23.000000 ki-aikido-0.0.1/src/__init__.py
--rw-r--r--   0 gabrielfalcao   (501) staff       (20)      325 2023-07-12 06:32:07.000000 ki-aikido-0.0.1/src/cli.py
--rw-r--r--   0 gabrielfalcao   (501) staff       (20)       18 2023-07-12 06:32:07.000000 ki-aikido-0.0.1/src/version.py
+drwx------   0 gabrielfalcao   (501) staff       (20)        0 2023-07-12 13:39:06.918097 ki-aikido-0.0.2/
+-rw-------   0 gabrielfalcao   (501) staff       (20)    35149 2023-07-12 00:33:58.000000 ki-aikido-0.0.2/COPYING
+-rw-------   0 gabrielfalcao   (501) staff       (20)      617 2023-07-12 13:28:51.000000 ki-aikido-0.0.2/Cargo.toml
+-rw-r--r--   0 gabrielfalcao   (501) staff       (20)      119 2023-07-12 07:43:44.000000 ki-aikido-0.0.2/MANIFEST.in
+-rw-------   0 gabrielfalcao   (501) staff       (20)     2497 2023-07-12 13:39:06.917945 ki-aikido-0.0.2/PKG-INFO
+-rw-------   0 gabrielfalcao   (501) staff       (20)      527 2023-07-12 13:31:11.000000 ki-aikido-0.0.2/README.rst
+drwx------   0 gabrielfalcao   (501) staff       (20)        0 2023-07-12 13:39:06.913634 ki-aikido-0.0.2/docs/
+drwx------   0 gabrielfalcao   (501) staff       (20)        0 2023-07-12 13:39:06.916244 ki-aikido-0.0.2/docs/source/
+-rw-------   0 gabrielfalcao   (501) staff       (20)     1011 2023-07-12 13:31:51.000000 ki-aikido-0.0.2/docs/source/conf.py
+-rw-------   0 gabrielfalcao   (501) staff       (20)      329 2023-07-12 07:36:39.000000 ki-aikido-0.0.2/docs/source/index.rst
+-rw-r--r--   0 gabrielfalcao   (501) staff       (20)      467 2023-07-12 13:31:35.000000 ki-aikido-0.0.2/docs/source/setting-up.rst
+drwx------   0 gabrielfalcao   (501) staff       (20)        0 2023-07-12 13:39:06.916943 ki-aikido-0.0.2/ki_aikido.egg-info/
+-rw-------   0 gabrielfalcao   (501) staff       (20)     2497 2023-07-12 13:39:06.000000 ki-aikido-0.0.2/ki_aikido.egg-info/PKG-INFO
+-rw-------   0 gabrielfalcao   (501) staff       (20)      346 2023-07-12 13:39:06.000000 ki-aikido-0.0.2/ki_aikido.egg-info/SOURCES.txt
+-rw-------   0 gabrielfalcao   (501) staff       (20)        1 2023-07-12 13:39:06.000000 ki-aikido-0.0.2/ki_aikido.egg-info/dependency_links.txt
+-rw-------   0 gabrielfalcao   (501) staff       (20)       41 2023-07-12 13:39:06.000000 ki-aikido-0.0.2/ki_aikido.egg-info/entry_points.txt
+-rw-------   0 gabrielfalcao   (501) staff       (20)        4 2023-07-12 13:39:06.000000 ki-aikido-0.0.2/ki_aikido.egg-info/top_level.txt
+-rw-------   0 gabrielfalcao   (501) staff       (20)        0 2023-07-12 07:38:37.000000 ki-aikido-0.0.2/requirements.txt
+-rw-------   0 gabrielfalcao   (501) staff       (20)       38 2023-07-12 13:39:06.918154 ki-aikido-0.0.2/setup.cfg
+-rwx------   0 gabrielfalcao   (501) staff       (20)     4978 2023-07-12 12:55:59.000000 ki-aikido-0.0.2/setup.py
+drwx------   0 gabrielfalcao   (501) staff       (20)        0 2023-07-12 13:39:06.917691 ki-aikido-0.0.2/src/
+-rw-r--r--   0 gabrielfalcao   (501) staff       (20)       24 2023-07-12 01:40:23.000000 ki-aikido-0.0.2/src/__init__.py
+-rw-r--r--   0 gabrielfalcao   (501) staff       (20)      325 2023-07-12 06:32:07.000000 ki-aikido-0.0.2/src/cli.py
+-rw-r--r--   0 gabrielfalcao   (501) staff       (20)       18 2023-07-12 13:32:00.000000 ki-aikido-0.0.2/src/version.py
```

### Comparing `ki-aikido-0.0.1/COPYING` & `ki-aikido-0.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `ki-aikido-0.0.1/Cargo.toml` & `ki-aikido-0.0.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "aikido"
-version = "0.0.1"
+version = "0.0.2"
 edition = "2021"
 authors = ["Gabriel Falcão <gabriel@nacaolivre.org>"]
 description = "Aikido is a set of tools for the self-defense of MacOS users"
 license = "GPL-3.0-or-later"
 # license-file = "COPYING"
 documentation = "https://docs.rs/aikido"
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `ki-aikido-0.0.1/docs/source/conf.py` & `ki-aikido-0.0.2/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'Aikido'
 copyright = '2023, Gabriel Falcão'
 author = 'Gabriel Falcão'
-release = '0.0.1'
+release = '0.0.2'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 # https://pypi.org/project/sphinx-immaterial/
 extensions = [
     "sphinx_immaterial"
```

### Comparing `ki-aikido-0.0.1/setup.py` & `ki-aikido-0.0.2/setup.py`

 * *Files identical despite different names*


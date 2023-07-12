# Comparing `tmp/duckyshell-0.0.5.tar.gz` & `tmp/duckyshell-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckyshell-0.0.5.tar", last modified: Wed Jul 12 19:51:06 2023, max compression
+gzip compressed data, was "duckyshell-0.0.6.tar", last modified: Wed Jul 12 20:06:20 2023, max compression
```

## Comparing `duckyshell-0.0.5.tar` & `duckyshell-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:26:57.833303 duckyshell-0.0.5/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      244 2023-07-12 20:26:57.824539 duckyshell-0.0.5/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      604 2023-07-11 19:48:42.000000 duckyshell-0.0.5/README.md
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:26:57.498608 duckyshell-0.0.5/duckyshell/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       36 2023-07-12 20:25:12.000000 duckyshell-0.0.5/duckyshell/__init__.py
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     3593 2023-07-11 20:10:07.000000 duckyshell-0.0.5/duckyshell/duckyshell.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:26:57.757990 duckyshell-0.0.5/duckyshell.egg-info/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      244 2023-07-12 20:26:57.000000 duckyshell-0.0.5/duckyshell.egg-info/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      202 2023-07-12 20:26:57.000000 duckyshell-0.0.5/duckyshell.egg-info/SOURCES.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-12 20:26:57.000000 duckyshell-0.0.5/duckyshell.egg-info/dependency_links.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       11 2023-07-12 20:26:57.000000 duckyshell-0.0.5/duckyshell.egg-info/top_level.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-07-12 20:26:57.835657 duckyshell-0.0.5/setup.cfg
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      290 2023-07-12 20:26:54.000000 duckyshell-0.0.5/setup.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:41:01.567814 duckyshell-0.0.6/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      244 2023-07-12 20:41:01.557214 duckyshell-0.0.6/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      604 2023-07-11 19:48:42.000000 duckyshell-0.0.6/README.md
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:41:01.154397 duckyshell-0.0.6/duckyshell/
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:41:01.484361 duckyshell-0.0.6/duckyshell/duckyshell.egg-info/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      244 2023-07-12 20:41:00.000000 duckyshell-0.0.6/duckyshell/duckyshell.egg-info/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      198 2023-07-12 20:41:01.000000 duckyshell-0.0.6/duckyshell/duckyshell.egg-info/SOURCES.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-12 20:41:00.000000 duckyshell-0.0.6/duckyshell/duckyshell.egg-info/dependency_links.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-12 20:41:00.000000 duckyshell-0.0.6/duckyshell/duckyshell.egg-info/top_level.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-07-12 20:41:01.570479 duckyshell-0.0.6/setup.cfg
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      297 2023-07-12 20:40:58.000000 duckyshell-0.0.6/setup.py
```

### Comparing `duckyshell-0.0.5/README.md` & `duckyshell-0.0.6/README.md`

 * *Files identical despite different names*


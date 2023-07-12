# Comparing `tmp/duckyshell-0.0.6.tar.gz` & `tmp/duckyshell-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckyshell-0.0.6.tar", last modified: Wed Jul 12 20:06:20 2023, max compression
+gzip compressed data, was "duckyshell-0.0.7.tar", last modified: Wed Jul 12 20:10:31 2023, max compression
```

## Comparing `duckyshell-0.0.6.tar` & `duckyshell-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:41:01.567814 duckyshell-0.0.6/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      244 2023-07-12 20:41:01.557214 duckyshell-0.0.6/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      604 2023-07-11 19:48:42.000000 duckyshell-0.0.6/README.md
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:41:01.154397 duckyshell-0.0.6/duckyshell/
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:41:01.484361 duckyshell-0.0.6/duckyshell/duckyshell.egg-info/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      244 2023-07-12 20:41:00.000000 duckyshell-0.0.6/duckyshell/duckyshell.egg-info/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      198 2023-07-12 20:41:01.000000 duckyshell-0.0.6/duckyshell/duckyshell.egg-info/SOURCES.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-12 20:41:00.000000 duckyshell-0.0.6/duckyshell/duckyshell.egg-info/dependency_links.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-12 20:41:00.000000 duckyshell-0.0.6/duckyshell/duckyshell.egg-info/top_level.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-07-12 20:41:01.570479 duckyshell-0.0.6/setup.cfg
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      297 2023-07-12 20:40:58.000000 duckyshell-0.0.6/setup.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:44:52.826965 duckyshell-0.0.7/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      244 2023-07-12 20:44:52.824259 duckyshell-0.0.7/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      604 2023-07-11 19:48:42.000000 duckyshell-0.0.7/README.md
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:44:52.477242 duckyshell-0.0.7/duckyshell/
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:44:52.750134 duckyshell-0.0.7/duckyshell/duckyshell.egg-info/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      244 2023-07-12 20:44:52.000000 duckyshell-0.0.7/duckyshell/duckyshell.egg-info/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      223 2023-07-12 20:44:52.000000 duckyshell-0.0.7/duckyshell/duckyshell.egg-info/SOURCES.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-12 20:44:52.000000 duckyshell-0.0.7/duckyshell/duckyshell.egg-info/dependency_links.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-12 20:44:52.000000 duckyshell-0.0.7/duckyshell/duckyshell.egg-info/top_level.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     3593 2023-07-11 20:10:07.000000 duckyshell-0.0.7/duckyshell/duckyshell.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-07-12 20:44:52.833867 duckyshell-0.0.7/setup.cfg
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      342 2023-07-12 20:44:50.000000 duckyshell-0.0.7/setup.py
```

### Comparing `duckyshell-0.0.6/README.md` & `duckyshell-0.0.7/README.md`

 * *Files identical despite different names*


# Comparing `tmp/duckyshell-0.0.3.tar.gz` & `tmp/duckyshell-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckyshell-0.0.3.tar", last modified: Tue Jul 11 20:18:05 2023, max compression
+gzip compressed data, was "duckyshell-0.0.4.tar", last modified: Wed Jul 12 19:44:54 2023, max compression
```

## Comparing `duckyshell-0.0.3.tar` & `duckyshell-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:18:05.017789 duckyshell-0.0.3/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      211 2023-07-11 20:18:05.009420 duckyshell-0.0.3/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      604 2023-07-11 19:48:42.000000 duckyshell-0.0.3/README.md
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      347 2023-07-11 20:17:46.000000 duckyshell-0.0.3/__init__.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:18:04.632079 duckyshell-0.0.3/duckyshell/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)     3593 2023-07-11 20:10:07.000000 duckyshell-0.0.3/duckyshell/main.py
-drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:18:04.938027 duckyshell-0.0.3/duckyshell.egg-info/
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      211 2023-07-11 20:18:04.000000 duckyshell-0.0.3/duckyshell.egg-info/PKG-INFO
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)      213 2023-07-11 20:18:04.000000 duckyshell-0.0.3/duckyshell.egg-info/SOURCES.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-11 20:18:04.000000 duckyshell-0.0.3/duckyshell.egg-info/dependency_links.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       45 2023-07-11 20:18:04.000000 duckyshell-0.0.3/duckyshell.egg-info/entry_points.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       11 2023-07-11 20:18:04.000000 duckyshell-0.0.3/duckyshell.egg-info/top_level.txt
--rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-07-11 20:18:05.021582 duckyshell-0.0.3/setup.cfg
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:21:14.166735 duckyshell-0.0.4/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      244 2023-07-12 20:21:14.158239 duckyshell-0.0.4/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      604 2023-07-11 19:48:42.000000 duckyshell-0.0.4/README.md
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:21:13.824406 duckyshell-0.0.4/duckyshell/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       26 2023-07-12 20:19:37.000000 duckyshell-0.0.4/duckyshell/__init__.py
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)     3593 2023-07-11 20:10:07.000000 duckyshell-0.0.4/duckyshell/duckyshell.py
+drwxrwxrwx   0 daniel    (1000) daniel    (1000)        0 2023-07-12 20:21:14.093749 duckyshell-0.0.4/duckyshell.egg-info/
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      244 2023-07-12 20:21:13.000000 duckyshell-0.0.4/duckyshell.egg-info/PKG-INFO
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      202 2023-07-12 20:21:13.000000 duckyshell-0.0.4/duckyshell.egg-info/SOURCES.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)        1 2023-07-12 20:21:13.000000 duckyshell-0.0.4/duckyshell.egg-info/dependency_links.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       11 2023-07-12 20:21:13.000000 duckyshell-0.0.4/duckyshell.egg-info/top_level.txt
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)       38 2023-07-12 20:21:14.166735 duckyshell-0.0.4/setup.cfg
+-rwxrwxrwx   0 daniel    (1000) daniel    (1000)      290 2023-07-12 20:20:19.000000 duckyshell-0.0.4/setup.py
```

### Comparing `duckyshell-0.0.3/README.md` & `duckyshell-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `duckyshell-0.0.3/duckyshell/main.py` & `duckyshell-0.0.4/duckyshell/duckyshell.py`

 * *Files identical despite different names*


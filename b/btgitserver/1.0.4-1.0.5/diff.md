# Comparing `tmp/btgitserver-1.0.4.tar.gz` & `tmp/btgitserver-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btgitserver-1.0.4.tar", last modified: Tue Jun 27 17:51:57 2023, max compression
+gzip compressed data, was "btgitserver-1.0.5.tar", last modified: Wed Jul 12 13:56:54 2023, max compression
```

## Comparing `btgitserver-1.0.4.tar` & `btgitserver-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:51:57.307683 btgitserver-1.0.4/
--rwx------   0 etejeda    (501) staff       (20)     1442 2023-06-25 15:47:07.000000 btgitserver-1.0.4/.gitignore
--rwx------   0 etejeda    (501) staff       (20)      445 2019-11-19 14:59:57.000000 btgitserver-1.0.4/Dockerfile
--rw-r--r--   0 etejeda    (501) staff       (20)     2363 2023-06-27 17:51:57.307903 btgitserver-1.0.4/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     1730 2023-06-27 12:45:34.000000 btgitserver-1.0.4/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-06-27 17:51:39.000000 btgitserver-1.0.4/VERSION.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:51:57.303810 btgitserver-1.0.4/btgitserver/
--rw-r--r--   0 etejeda    (501) staff       (20)      214 2023-06-25 19:24:10.000000 btgitserver-1.0.4/btgitserver/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     6119 2023-06-27 17:51:03.000000 btgitserver-1.0.4/btgitserver/app.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2206 2023-06-27 12:46:04.000000 btgitserver-1.0.4/btgitserver/args.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1004 2023-06-25 15:50:24.000000 btgitserver-1.0.4/btgitserver/config.py
--rw-r--r--   0 etejeda    (501) staff       (20)      595 2023-06-27 12:39:08.000000 btgitserver-1.0.4/btgitserver/defaults.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1444 2023-06-25 19:36:10.000000 btgitserver-1.0.4/btgitserver/logger.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:51:57.306786 btgitserver-1.0.4/btgitserver.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)     2363 2023-06-27 17:51:57.000000 btgitserver-1.0.4/btgitserver.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      455 2023-06-27 17:51:57.000000 btgitserver-1.0.4/btgitserver.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-27 17:51:57.000000 btgitserver-1.0.4/btgitserver.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       52 2023-06-27 17:51:57.000000 btgitserver-1.0.4/btgitserver.egg-info/entry_points.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-25 19:26:41.000000 btgitserver-1.0.4/btgitserver.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)      173 2023-06-27 17:51:57.000000 btgitserver-1.0.4/btgitserver.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       12 2023-06-27 17:51:57.000000 btgitserver-1.0.4/btgitserver.egg-info/top_level.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-06-27 17:51:57.307098 btgitserver-1.0.4/etc/
--rwx------   0 etejeda    (501) staff       (20)      162 2023-06-27 17:44:31.000000 btgitserver-1.0.4/etc/config.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)     1236 2023-06-27 17:51:57.308911 btgitserver-1.0.4/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)      780 2023-06-26 00:48:02.000000 btgitserver-1.0.4/setup.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-12 13:56:54.325730 btgitserver-1.0.5/
+-rwx------   0 etejeda    (501) staff       (20)     1442 2023-06-25 15:47:07.000000 btgitserver-1.0.5/.gitignore
+-rwx------   0 etejeda    (501) staff       (20)      445 2019-11-19 14:59:57.000000 btgitserver-1.0.5/Dockerfile
+-rw-r--r--   0 etejeda    (501) staff       (20)     2363 2023-07-12 13:56:54.325963 btgitserver-1.0.5/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     1730 2023-06-27 12:45:34.000000 btgitserver-1.0.5/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-07-12 13:56:33.000000 btgitserver-1.0.5/VERSION.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-12 13:56:54.321282 btgitserver-1.0.5/btgitserver/
+-rw-r--r--   0 etejeda    (501) staff       (20)      214 2023-06-25 19:24:10.000000 btgitserver-1.0.5/btgitserver/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     6117 2023-07-12 13:56:09.000000 btgitserver-1.0.5/btgitserver/app.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2206 2023-06-27 12:46:04.000000 btgitserver-1.0.5/btgitserver/args.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1004 2023-06-25 15:50:24.000000 btgitserver-1.0.5/btgitserver/config.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      595 2023-06-27 12:39:08.000000 btgitserver-1.0.5/btgitserver/defaults.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1444 2023-06-25 19:36:10.000000 btgitserver-1.0.5/btgitserver/logger.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-12 13:56:54.324490 btgitserver-1.0.5/btgitserver.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2363 2023-07-12 13:56:54.000000 btgitserver-1.0.5/btgitserver.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      455 2023-07-12 13:56:54.000000 btgitserver-1.0.5/btgitserver.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-07-12 13:56:54.000000 btgitserver-1.0.5/btgitserver.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       52 2023-07-12 13:56:54.000000 btgitserver-1.0.5/btgitserver.egg-info/entry_points.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-25 19:26:41.000000 btgitserver-1.0.5/btgitserver.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)      173 2023-07-12 13:56:54.000000 btgitserver-1.0.5/btgitserver.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       12 2023-07-12 13:56:54.000000 btgitserver-1.0.5/btgitserver.egg-info/top_level.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-12 13:56:54.325016 btgitserver-1.0.5/etc/
+-rwx------   0 etejeda    (501) staff       (20)      162 2023-06-27 17:44:31.000000 btgitserver-1.0.5/etc/config.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)     1236 2023-07-12 13:56:54.326897 btgitserver-1.0.5/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)      780 2023-06-26 00:48:02.000000 btgitserver-1.0.5/setup.py
```

### Comparing `btgitserver-1.0.4/.gitignore` & `btgitserver-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.4/PKG-INFO` & `btgitserver-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgitserver
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python-based Git Server
 Home-page: https://github.com/berttejeda/bert.git-server
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btgitserver-1.0.4/README.md` & `btgitserver-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.4/btgitserver/app.py` & `btgitserver-1.0.5/btgitserver/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
   logger.info(f'Adding git repos under {fq_git_search_path}')
   for p in Path(fq_git_search_path).rglob("*"):
       if p.is_dir() and p.name == '.git':
         git_directory = p.parent.as_posix()
         git_directory_name = p.parent.name
         if git_directory_name:
           git_repo_map[git_directory_name] = git_directory
-  logger.info(f'Finished building git repo map!')
+logger.info(f'Finished building git repo map!')
 
 numrepos = len(list(git_repo_map.keys()))
 logger.info(f'Found {numrepos} repo(s)')
 
 authorized_users = app_config.auth.users
 users = [u[0] for u in authorized_users.items()]
 available_repos = list(git_repo_map.keys())
```

### Comparing `btgitserver-1.0.4/btgitserver/args.py` & `btgitserver-1.0.5/btgitserver/args.py`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.4/btgitserver/config.py` & `btgitserver-1.0.5/btgitserver/config.py`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.4/btgitserver/defaults.py` & `btgitserver-1.0.5/btgitserver/defaults.py`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.4/btgitserver/logger.py` & `btgitserver-1.0.5/btgitserver/logger.py`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.4/btgitserver.egg-info/PKG-INFO` & `btgitserver-1.0.5/btgitserver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgitserver
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python-based Git Server
 Home-page: https://github.com/berttejeda/bert.git-server
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btgitserver-1.0.4/setup.cfg` & `btgitserver-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.4/setup.py` & `btgitserver-1.0.5/setup.py`

 * *Files identical despite different names*


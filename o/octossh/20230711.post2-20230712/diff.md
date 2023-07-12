# Comparing `tmp/octossh-20230711.post2.tar.gz` & `tmp/octossh-20230712.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octossh-20230711.post2.tar", last modified: Tue Jul 11 21:50:46 2023, max compression
+gzip compressed data, was "octossh-20230712.tar", last modified: Wed Jul 12 20:01:56 2023, max compression
```

## Comparing `octossh-20230711.post2.tar` & `octossh-20230712.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-11 21:50:46.863648 octossh-20230711.post2/
--rw-rw-r--   0 l         (1000) l         (1000)     3401 2023-07-11 21:50:46.863648 octossh-20230711.post2/PKG-INFO
--rw-rw-r--   0 l         (1000) l         (1000)     3068 2023-07-09 12:44:05.000000 octossh-20230711.post2/README.md
--rw-rw-r--   0 l         (1000) l         (1000)      665 2023-07-07 15:12:59.000000 octossh-20230711.post2/pyproject.toml
--rw-rw-r--   0 l         (1000) l         (1000)       38 2023-07-11 21:50:46.863648 octossh-20230711.post2/setup.cfg
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-11 21:50:46.863648 octossh-20230711.post2/src/
--rwxrwxr-x   0 l         (1000) l         (1000)    12915 2023-07-11 21:50:38.000000 octossh-20230711.post2/src/ocsh.py
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-11 21:50:46.863648 octossh-20230711.post2/src/octossh.egg-info/
--rw-rw-r--   0 l         (1000) l         (1000)     3401 2023-07-11 21:50:46.000000 octossh-20230711.post2/src/octossh.egg-info/PKG-INFO
--rw-rw-r--   0 l         (1000) l         (1000)      248 2023-07-11 21:50:46.000000 octossh-20230711.post2/src/octossh.egg-info/SOURCES.txt
--rw-rw-r--   0 l         (1000) l         (1000)        1 2023-07-11 21:50:46.000000 octossh-20230711.post2/src/octossh.egg-info/dependency_links.txt
--rw-rw-r--   0 l         (1000) l         (1000)       35 2023-07-11 21:50:46.000000 octossh-20230711.post2/src/octossh.egg-info/entry_points.txt
--rw-rw-r--   0 l         (1000) l         (1000)       54 2023-07-11 21:50:46.000000 octossh-20230711.post2/src/octossh.egg-info/requires.txt
--rw-rw-r--   0 l         (1000) l         (1000)        5 2023-07-11 21:50:46.000000 octossh-20230711.post2/src/octossh.egg-info/top_level.txt
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-12 20:01:56.285085 octossh-20230712/
+-rw-rw-r--   0 l         (1000) l         (1000)     3395 2023-07-12 20:01:56.285085 octossh-20230712/PKG-INFO
+-rw-rw-r--   0 l         (1000) l         (1000)     3068 2023-07-09 12:44:05.000000 octossh-20230712/README.md
+-rw-rw-r--   0 l         (1000) l         (1000)      665 2023-07-07 15:12:59.000000 octossh-20230712/pyproject.toml
+-rw-rw-r--   0 l         (1000) l         (1000)       38 2023-07-12 20:01:56.285085 octossh-20230712/setup.cfg
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-12 20:01:56.284085 octossh-20230712/src/
+-rwxrwxr-x   0 l         (1000) l         (1000)    12910 2023-07-12 20:01:26.000000 octossh-20230712/src/ocsh.py
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-12 20:01:56.285085 octossh-20230712/src/octossh.egg-info/
+-rw-rw-r--   0 l         (1000) l         (1000)     3395 2023-07-12 20:01:56.000000 octossh-20230712/src/octossh.egg-info/PKG-INFO
+-rw-rw-r--   0 l         (1000) l         (1000)      248 2023-07-12 20:01:56.000000 octossh-20230712/src/octossh.egg-info/SOURCES.txt
+-rw-rw-r--   0 l         (1000) l         (1000)        1 2023-07-12 20:01:56.000000 octossh-20230712/src/octossh.egg-info/dependency_links.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       35 2023-07-12 20:01:56.000000 octossh-20230712/src/octossh.egg-info/entry_points.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       54 2023-07-12 20:01:56.000000 octossh-20230712/src/octossh.egg-info/requires.txt
+-rw-rw-r--   0 l         (1000) l         (1000)        5 2023-07-12 20:01:56.000000 octossh-20230712/src/octossh.egg-info/top_level.txt
```

### Comparing `octossh-20230711.post2/PKG-INFO` & `octossh-20230712/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octossh
-Version: 20230711.post2
+Version: 20230712
 Summary: SSH password log-in and command automator
 Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/looran/octossh
 Keywords: ssh,bouncer,pass
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `octossh-20230711.post2/README.md` & `octossh-20230712/README.md`

 * *Files identical despite different names*

### Comparing `octossh-20230711.post2/pyproject.toml` & `octossh-20230712/pyproject.toml`

 * *Files identical despite different names*

### Comparing `octossh-20230711.post2/src/ocsh.py` & `octossh-20230712/src/ocsh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 # 2013, 2023 Laurent Ghigonis <ooookiwi@gmail.com>
 # 2013, Pierre-Olivier Vauboin
 
 DESCRIPTION = "octossh - SSH password log-in and command automator"
-VERSION = "20230711-2"
+VERSION = "20230712"
 SUMMARY = f"""octossh automates SSH password login and command execution through annotations on `ssh_config(5)` Hosts:
 * password authentication, reading password from pass[1]:
   * config:  `# ocsh pass <pass-name>`
   * command: `$ ocsh host`
 * post-login command execution:
   * config:  `# ocsh post <action> "<cmd>"`
   * command: `$ ocsh host[action]`
@@ -228,15 +228,15 @@
                 for action in usr['post'].split(','):
                     if action in conf['post']:
                         post[action] = conf['post'][action]
                     else:
                         raise self._err("invalid action '%s' for host '%s'" % (action, usr['host']))
                 
         # construct command to reach target
-        ssh_cmd = "ssh -v"
+        ssh_cmd = "ssh"
         if self.conf.conf_path:
             ssh_cmd += " -F %s" % self.conf.conf_path
         passname = None
         if 'pass' in conf:
             passname = conf['pass']
         if 'ProxyJump' in conf:
             # if ProxyJump in ssh_config(5), replace with ocsh
```

### Comparing `octossh-20230711.post2/src/octossh.egg-info/PKG-INFO` & `octossh-20230712/src/octossh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octossh
-Version: 20230711.post2
+Version: 20230712
 Summary: SSH password log-in and command automator
 Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/looran/octossh
 Keywords: ssh,bouncer,pass
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```


# Comparing `tmp/riotee_probe-1.0.1.tar.gz` & `tmp/riotee_probe-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riotee_probe-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "riotee_probe-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `riotee_probe-1.0.1.tar` & `riotee_probe-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1116 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0      515 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      376 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/__init__.py
--rw-r--r--   0        0        0     3056 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/cli.py
--rw-r--r--   0        0        0     1668 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/intelhex.py
--rw-r--r--   0        0        0     2591 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/probe.py
--rw-r--r--   0        0        0      893 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/protocol.py
--rw-r--r--   0        0        0      965 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/session.py
--rw-r--r--   0        0        0     4223 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/target.py
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 riotee_probe-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1116 2023-07-12 10:05:19.524224 riotee_probe-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      515 2023-07-12 10:05:19.524224 riotee_probe-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      376 2023-07-12 10:05:19.524224 riotee_probe-1.0.2/riotee_probe/__init__.py
+-rw-r--r--   0        0        0     3056 2023-07-12 10:05:19.524224 riotee_probe-1.0.2/riotee_probe/cli.py
+-rw-r--r--   0        0        0     1668 2023-07-12 10:05:19.524224 riotee_probe-1.0.2/riotee_probe/intelhex.py
+-rw-r--r--   0        0        0     2591 2023-07-12 10:05:19.524224 riotee_probe-1.0.2/riotee_probe/probe.py
+-rw-r--r--   0        0        0      893 2023-07-12 10:05:19.524224 riotee_probe-1.0.2/riotee_probe/protocol.py
+-rw-r--r--   0        0        0      965 2023-07-12 10:05:19.524224 riotee_probe-1.0.2/riotee_probe/session.py
+-rw-r--r--   0        0        0     4228 2023-07-12 10:05:19.524224 riotee_probe-1.0.2/riotee_probe/target.py
+-rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 riotee_probe-1.0.2/PKG-INFO
```

### Comparing `riotee_probe-1.0.1/LICENSE.txt` & `riotee_probe-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `riotee_probe-1.0.1/pyproject.toml` & `riotee_probe-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `riotee_probe-1.0.1/riotee_probe/cli.py` & `riotee_probe-1.0.2/riotee_probe/cli.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-1.0.1/riotee_probe/intelhex.py` & `riotee_probe-1.0.2/riotee_probe/intelhex.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-1.0.1/riotee_probe/probe.py` & `riotee_probe-1.0.2/riotee_probe/probe.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-1.0.1/riotee_probe/protocol.py` & `riotee_probe-1.0.2/riotee_probe/protocol.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-1.0.1/riotee_probe/session.py` & `riotee_probe-1.0.2/riotee_probe/session.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-1.0.1/riotee_probe/target.py` & `riotee_probe-1.0.2/riotee_probe/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
     def program(self, fw_path: Path, progress: Callable = None):
         if progress is None:
 
             def progress(arg):
                 pass
 
-        FileProgrammer(self._session, progress=progress).program(fw_path)
+        FileProgrammer(self._session, progress=progress).program(str(fw_path))
 
     def halt(self):
         self._session.board.target.halt()
 
     def reset(self):
         self._session.board.target.reset()
```


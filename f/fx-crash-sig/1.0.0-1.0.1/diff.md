# Comparing `tmp/fx-crash-sig-1.0.0.tar.gz` & `tmp/fx-crash-sig-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fx-crash-sig-1.0.0.tar", last modified: Tue Dec  6 17:36:41 2022, max compression
+gzip compressed data, was "fx-crash-sig-1.0.1.tar", last modified: Wed Jul 12 18:27:44 2023, max compression
```

## Comparing `fx-crash-sig-1.0.0.tar` & `fx-crash-sig-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-12-06 17:36:41.275657 fx-crash-sig-1.0.0/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    15977 2019-05-23 20:39:20.000000 fx-crash-sig-1.0.0/LICENSE
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2938 2022-12-06 17:36:41.275657 fx-crash-sig-1.0.0/PKG-INFO
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2239 2022-12-06 17:35:14.000000 fx-crash-sig-1.0.0/README.md
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-12-06 17:36:41.275657 fx-crash-sig-1.0.0/fx_crash_sig/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      902 2022-12-06 16:43:03.000000 fx-crash-sig-1.0.0/fx_crash_sig/__init__.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     1487 2022-12-06 16:43:03.000000 fx-crash-sig-1.0.0/fx_crash_sig/cmd_get_crash_sig.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     4670 2022-12-06 16:43:03.000000 fx-crash-sig-1.0.0/fx_crash_sig/crash_processor.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     1070 2022-12-06 16:43:03.000000 fx-crash-sig-1.0.0/fx_crash_sig/example.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)   135420 2022-11-23 17:31:36.000000 fx-crash-sig-1.0.0/fx_crash_sig/sample_traces.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     8193 2022-12-06 16:43:03.000000 fx-crash-sig-1.0.0/fx_crash_sig/symbolicate.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      726 2022-12-06 17:18:53.000000 fx-crash-sig-1.0.0/fx_crash_sig/utils.py
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-12-06 17:36:41.275657 fx-crash-sig-1.0.0/fx_crash_sig.egg-info/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2938 2022-12-06 17:36:41.000000 fx-crash-sig-1.0.0/fx_crash_sig.egg-info/PKG-INFO
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      449 2022-12-06 17:36:41.000000 fx-crash-sig-1.0.0/fx_crash_sig.egg-info/SOURCES.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)        1 2022-12-06 17:36:41.000000 fx-crash-sig-1.0.0/fx_crash_sig.egg-info/dependency_links.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       72 2022-12-06 17:36:41.000000 fx-crash-sig-1.0.0/fx_crash_sig.egg-info/entry_points.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       55 2022-12-06 17:36:41.000000 fx-crash-sig-1.0.0/fx_crash_sig.egg-info/requires.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       13 2022-12-06 17:36:41.000000 fx-crash-sig-1.0.0/fx_crash_sig.egg-info/top_level.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      215 2022-12-06 17:36:41.279657 fx-crash-sig-1.0.0/setup.cfg
--rwxrwxr-x   0 willkg    (1000) willkg    (1000)     1444 2022-12-06 17:35:14.000000 fx-crash-sig-1.0.0/setup.py
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-07-12 18:27:44.168553 fx-crash-sig-1.0.1/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    15977 2019-05-23 20:39:20.000000 fx-crash-sig-1.0.1/LICENSE
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2570 2023-07-12 18:27:44.168553 fx-crash-sig-1.0.1/PKG-INFO
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1871 2023-04-21 01:56:04.000000 fx-crash-sig-1.0.1/README.md
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-07-12 18:27:44.168553 fx-crash-sig-1.0.1/fx_crash_sig/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      902 2022-12-06 16:43:03.000000 fx-crash-sig-1.0.1/fx_crash_sig/__init__.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1487 2022-12-06 16:43:03.000000 fx-crash-sig-1.0.1/fx_crash_sig/cmd_get_crash_sig.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     4700 2023-07-12 18:23:15.000000 fx-crash-sig-1.0.1/fx_crash_sig/crash_processor.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1070 2022-12-06 16:43:03.000000 fx-crash-sig-1.0.1/fx_crash_sig/example.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)   135420 2022-11-23 17:31:36.000000 fx-crash-sig-1.0.1/fx_crash_sig/sample_traces.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     8209 2023-05-31 23:42:19.000000 fx-crash-sig-1.0.1/fx_crash_sig/symbolicate.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      726 2022-12-06 17:18:53.000000 fx-crash-sig-1.0.1/fx_crash_sig/utils.py
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-07-12 18:27:44.168553 fx-crash-sig-1.0.1/fx_crash_sig.egg-info/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2570 2023-07-12 18:27:44.000000 fx-crash-sig-1.0.1/fx_crash_sig.egg-info/PKG-INFO
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      501 2023-07-12 18:27:44.000000 fx-crash-sig-1.0.1/fx_crash_sig.egg-info/SOURCES.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)        1 2023-07-12 18:27:44.000000 fx-crash-sig-1.0.1/fx_crash_sig.egg-info/dependency_links.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       72 2023-07-12 18:27:44.000000 fx-crash-sig-1.0.1/fx_crash_sig.egg-info/entry_points.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       55 2023-07-12 18:27:44.000000 fx-crash-sig-1.0.1/fx_crash_sig.egg-info/requires.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       13 2023-07-12 18:27:44.000000 fx-crash-sig-1.0.1/fx_crash_sig.egg-info/top_level.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      822 2023-05-31 23:42:19.000000 fx-crash-sig-1.0.1/pyproject.toml
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       38 2023-07-12 18:27:44.168553 fx-crash-sig-1.0.1/setup.cfg
+-rwxrwxr-x   0 willkg    (1000) willkg    (1000)     1444 2023-07-12 18:27:22.000000 fx-crash-sig-1.0.1/setup.py
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2023-07-12 18:27:44.168553 fx-crash-sig-1.0.1/tests/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     1266 2022-11-23 01:39:03.000000 fx-crash-sig-1.0.1/tests/test_symbolicator.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      530 2022-12-06 16:43:03.000000 fx-crash-sig-1.0.1/tests/test_utils.py
```

### Comparing `fx-crash-sig-1.0.0/LICENSE` & `fx-crash-sig-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fx-crash-sig-1.0.0/PKG-INFO` & `fx-crash-sig-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fx-crash-sig
-Version: 1.0.0
+Version: 1.0.1
 Summary: Get crash signature from Firefox crash ping
 Home-page: https://github.com/mozilla/fx-crash-sig
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -114,24 +114,7 @@
 ```
 
 Test:
 
 ```sh
 make test
 ```
-
-
-## Release process
-
-1. Create a `release_X_Y_Z` branch
-2. Update version in `setup.py` and update `HISTORY.md`
-3. Run tests
-4. Push branch to GitHub, create a PR, review it, and merge it
-5. Create a signed tag, push to GitHub:
-   ```sh
-   git tag -s vX.Y.Z
-   git push --tags REMOTE TAGNAME
-   ```
-6. Build and release package files:
-   ```sh
-   make release
-   ```
```

### Comparing `fx-crash-sig-1.0.0/README.md` & `fx-crash-sig-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -97,24 +97,7 @@
 ```
 
 Test:
 
 ```sh
 make test
 ```
-
-
-## Release process
-
-1. Create a `release_X_Y_Z` branch
-2. Update version in `setup.py` and update `HISTORY.md`
-3. Run tests
-4. Push branch to GitHub, create a PR, review it, and merge it
-5. Create a signed tag, push to GitHub:
-   ```sh
-   git tag -s vX.Y.Z
-   git push --tags REMOTE TAGNAME
-   ```
-6. Build and release package files:
-   ```sh
-   make release
-   ```
```

### Comparing `fx-crash-sig-1.0.0/fx_crash_sig/__init__.py` & `fx-crash-sig-1.0.1/fx_crash_sig/__init__.py`

 * *Files identical despite different names*

### Comparing `fx-crash-sig-1.0.0/fx_crash_sig/cmd_get_crash_sig.py` & `fx-crash-sig-1.0.1/fx_crash_sig/cmd_get_crash_sig.py`

 * *Files identical despite different names*

### Comparing `fx-crash-sig-1.0.0/fx_crash_sig/crash_processor.py` & `fx-crash-sig-1.0.1/fx_crash_sig/crash_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,21 +26,22 @@
         :returns: signature result
 
         """
         symbolicated = self.symbolicate(crash_ping)
         if self.verbose:
             print("Symbolicated stack:")
             for frame in symbolicated["threads"][0]["frames"]:
-                if frame.get("filename") and frame.get("line"):
-                    # FIXME(willkg): find actual keys
-                    print(
-                        f"   {frame['frame']}    {frame['function']}  ({frame['filename']}:{frame['line']})"
-                    )
+                frame_idx = frame.get("frame", "")
+                line = frame.get("line", "")
+                filename = frame.get("filename", "")
+                function = frame.get("function", "")
+                if filename and line:
+                    print(f"   {frame_idx}    {function}  ({filename}:{line})")
                 else:
-                    print(f"   {frame['frame']}    {frame['function']}")
+                    print(f"   {frame_idx}    {function}")
         signature_result = self.get_signature_from_symbolicated(symbolicated)
         if self.verbose and len(signature_result.signature) == 0:
             print(
                 f"fx-crash-sig: Failed siggen: {signature_result.notes}",
                 file=sys.stderr,
             )
         return signature_result
```

### Comparing `fx-crash-sig-1.0.0/fx_crash_sig/example.py` & `fx-crash-sig-1.0.1/fx_crash_sig/example.py`

 * *Files identical despite different names*

### Comparing `fx-crash-sig-1.0.0/fx_crash_sig/sample_traces.py` & `fx-crash-sig-1.0.1/fx_crash_sig/sample_traces.py`

 * *Files identical despite different names*

### Comparing `fx-crash-sig-1.0.0/fx_crash_sig/symbolicate.py` & `fx-crash-sig-1.0.1/fx_crash_sig/symbolicate.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,18 +91,18 @@
                 module = modules[module_index]
 
                 if "base_addr" not in module:
                     raise ValueError(f"missing base_addr for module {module_index}")
 
                 try:
                     module_offset_int = ip_int - int(module["base_addr"], 16)
-                except ValueError:
+                except ValueError as exc:
                     raise ValueError(
                         f"bad base_addr {module['base_addr']} for module {module_index}"
-                    )
+                    ) from exc
 
                 if "filename" in module:
                     out_frame["module"] = module["filename"]
                 out_frame["module_offset"] = "0x%x" % module_offset_int
 
                 # prepare this frame for symbol lookup
```

### Comparing `fx-crash-sig-1.0.0/fx_crash_sig/utils.py` & `fx-crash-sig-1.0.1/fx_crash_sig/utils.py`

 * *Files identical despite different names*

### Comparing `fx-crash-sig-1.0.0/fx_crash_sig.egg-info/PKG-INFO` & `fx-crash-sig-1.0.1/fx_crash_sig.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fx-crash-sig
-Version: 1.0.0
+Version: 1.0.1
 Summary: Get crash signature from Firefox crash ping
 Home-page: https://github.com/mozilla/fx-crash-sig
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -114,24 +114,7 @@
 ```
 
 Test:
 
 ```sh
 make test
 ```
-
-
-## Release process
-
-1. Create a `release_X_Y_Z` branch
-2. Update version in `setup.py` and update `HISTORY.md`
-3. Run tests
-4. Push branch to GitHub, create a PR, review it, and merge it
-5. Create a signed tag, push to GitHub:
-   ```sh
-   git tag -s vX.Y.Z
-   git push --tags REMOTE TAGNAME
-   ```
-6. Build and release package files:
-   ```sh
-   make release
-   ```
```

### Comparing `fx-crash-sig-1.0.0/setup.py` & `fx-crash-sig-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def read_file(name):
     with open(name) as f:
         return f.read().strip()
 
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 INSTALL_REQUIRES = [
     "requests<3.0.0",
     "siggen>=1.0.0, <2.0.0",
     "importlib_metadata",
 ]
```


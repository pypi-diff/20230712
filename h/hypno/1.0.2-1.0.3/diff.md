# Comparing `tmp/hypno-1.0.2.tar.gz` & `tmp/hypno-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypno-1.0.2.tar", last modified: Tue Jul  4 22:34:10 2023, max compression
+gzip compressed data, was "hypno-1.0.3.tar", last modified: Tue Jul 11 22:45:38 2023, max compression
```

## Comparing `hypno-1.0.2.tar` & `hypno-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 22:34:10.568107 hypno-1.0.2/
--rw-rw-rw-   0        0        0     1092 2023-07-04 22:32:36.000000 hypno-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       29 2023-07-04 22:32:36.000000 hypno-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2706 2023-07-04 22:34:10.568107 hypno-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1793 2023-07-04 22:32:36.000000 hypno-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 22:34:10.562203 hypno-1.0.2/hypno/
--rw-rw-rw-   0        0        0       50 2023-07-04 22:32:36.000000 hypno-1.0.2/hypno/__init__.py
--rw-rw-rw-   0        0        0      675 2023-07-04 22:32:36.000000 hypno-1.0.2/hypno/__main__.py
--rw-rw-rw-   0        0        0     2636 2023-07-04 22:32:36.000000 hypno-1.0.2/hypno/api.py
--rw-rw-rw-   0        0        0     1054 2023-07-04 22:32:36.000000 hypno-1.0.2/hypno/injection.c
-drwxrwxrwx   0        0        0        0 2023-07-04 22:34:10.566821 hypno-1.0.2/hypno.egg-info/
--rw-rw-rw-   0        0        0     2706 2023-07-04 22:34:10.000000 hypno-1.0.2/hypno.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-04 22:34:10.000000 hypno-1.0.2/hypno.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 22:34:10.000000 hypno-1.0.2/hypno.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-04 22:34:10.000000 hypno-1.0.2/hypno.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-04 22:33:30.000000 hypno-1.0.2/hypno.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-07-04 22:34:10.000000 hypno-1.0.2/hypno.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-04 22:34:10.000000 hypno-1.0.2/hypno.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      989 2023-07-04 22:34:10.570202 hypno-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      203 2023-07-04 22:32:36.000000 hypno-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 22:34:10.568107 hypno-1.0.2/tests/
--rw-rw-rw-   0        0        0     1114 2023-07-04 22:32:36.000000 hypno-1.0.2/tests/test_hypno.py
+drwxrwxrwx   0        0        0        0 2023-07-11 22:45:38.686725 hypno-1.0.3/
+-rw-rw-rw-   0        0        0     1092 2023-07-11 22:44:13.000000 hypno-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       29 2023-07-11 22:44:13.000000 hypno-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2711 2023-07-11 22:45:38.686725 hypno-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1798 2023-07-11 22:44:13.000000 hypno-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 22:45:38.678343 hypno-1.0.3/hypno/
+-rw-rw-rw-   0        0        0       50 2023-07-11 22:44:13.000000 hypno-1.0.3/hypno/__init__.py
+-rw-rw-rw-   0        0        0      675 2023-07-11 22:44:13.000000 hypno-1.0.3/hypno/__main__.py
+-rw-rw-rw-   0        0        0     2636 2023-07-11 22:44:13.000000 hypno-1.0.3/hypno/api.py
+-rw-rw-rw-   0        0        0     1063 2023-07-11 22:44:13.000000 hypno-1.0.3/hypno/injection.c
+drwxrwxrwx   0        0        0        0 2023-07-11 22:45:38.684628 hypno-1.0.3/hypno.egg-info/
+-rw-rw-rw-   0        0        0     2711 2023-07-11 22:45:38.000000 hypno-1.0.3/hypno.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-07-11 22:45:38.000000 hypno-1.0.3/hypno.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 22:45:38.000000 hypno-1.0.3/hypno.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-11 22:45:38.000000 hypno-1.0.3/hypno.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-11 22:44:58.000000 hypno-1.0.3/hypno.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-07-11 22:45:38.000000 hypno-1.0.3/hypno.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-11 22:45:38.000000 hypno-1.0.3/hypno.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      989 2023-07-11 22:45:38.687766 hypno-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      203 2023-07-11 22:44:13.000000 hypno-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 22:45:38.685665 hypno-1.0.3/tests/
+-rw-rw-rw-   0        0        0     1114 2023-07-11 22:44:13.000000 hypno-1.0.3/tests/test_hypno.py
```

### Comparing `hypno-1.0.2/LICENSE.txt` & `hypno-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hypno-1.0.2/PKG-INFO` & `hypno-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypno
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool/library allowing to inject python code into a running python process.
 Home-page: https://github.com/kmaork/hypno
 Author: Maor Kleinberger
 Author-email: kmaork@gmail.com
 Keywords: injection library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -33,15 +33,15 @@
 
 If you are trying to debug a python process, check out [kmaork/madbg](https://github.com/kmaork/madbg).
 
 ### Installation
 ```shell script
 pip install hypno
 ```
-Both source distributions, manylinux, musslinux and windows wheels are uploaded to pypi for every release.
+Both source distributions, manylinux, musslinux, mac and windows wheels are uploaded to pypi for every release.
 
 ### Usage
 #### CLI
 ```shell script
 hypno <pid> <python_code>
 ```
```

### Comparing `hypno-1.0.2/README.md` & `hypno-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 If you are trying to debug a python process, check out [kmaork/madbg](https://github.com/kmaork/madbg).
 
 ### Installation
 ```shell script
 pip install hypno
 ```
-Both source distributions, manylinux, musslinux and windows wheels are uploaded to pypi for every release.
+Both source distributions, manylinux, musslinux, mac and windows wheels are uploaded to pypi for every release.
 
 ### Usage
 #### CLI
 ```shell script
 hypno <pid> <python_code>
 ```
```

### Comparing `hypno-1.0.2/hypno/__main__.py` & `hypno-1.0.3/hypno/__main__.py`

 * *Files identical despite different names*

### Comparing `hypno-1.0.2/hypno/api.py` & `hypno-1.0.3/hypno/api.py`

 * *Files identical despite different names*

### Comparing `hypno-1.0.2/hypno/injection.c` & `hypno-1.0.3/hypno/injection.c`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 #define MAX_PYTHON_CODE_SIZE 60500
 #define STR_EXPAND(tok) #tok
 #define STR(tok) STR_EXPAND(tok)
 
 PyMODINIT_FUNC PyInit_injection(void) {return NULL;}
 
-char PYTHON_CODE[MAX_PYTHON_CODE_SIZE + 1] = "\0--- hypno code start ---" STR(MAX_PYTHON_CODE_SIZE);
+volatile char PYTHON_CODE[MAX_PYTHON_CODE_SIZE + 1] = "\0--- hypno code start ---" STR(MAX_PYTHON_CODE_SIZE);
 
 void run_python_code() {
     if (PYTHON_CODE[0]) {
         int saved_errno = errno;
         PyGILState_STATE gstate = PyGILState_Ensure();
         PyRun_SimpleString(PYTHON_CODE);
         PyGILState_Release(gstate);
```

### Comparing `hypno-1.0.2/hypno.egg-info/PKG-INFO` & `hypno-1.0.3/hypno.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypno
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool/library allowing to inject python code into a running python process.
 Home-page: https://github.com/kmaork/hypno
 Author: Maor Kleinberger
 Author-email: kmaork@gmail.com
 Keywords: injection library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -33,15 +33,15 @@
 
 If you are trying to debug a python process, check out [kmaork/madbg](https://github.com/kmaork/madbg).
 
 ### Installation
 ```shell script
 pip install hypno
 ```
-Both source distributions, manylinux, musslinux and windows wheels are uploaded to pypi for every release.
+Both source distributions, manylinux, musslinux, mac and windows wheels are uploaded to pypi for every release.
 
 ### Usage
 #### CLI
 ```shell script
 hypno <pid> <python_code>
 ```
```

### Comparing `hypno-1.0.2/setup.cfg` & `hypno-1.0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
 00000030: 3d33 2e37 0d0a 7061 636b 6167 6573 203d  =3.7..packages =
 00000040: 2068 7970 6e6f 0d0a 696e 7374 616c 6c5f   hypno..install_
 00000050: 7265 7175 6972 6573 203d 200d 0a09 7079  requires = ...py
 00000060: 696e 6a65 6374 6f72 3e3d 302e 312e 320d  injector>=0.1.2.
 00000070: 0a0d 0a5b 6d65 7461 6461 7461 5d0d 0a6e  ...[metadata]..n
 00000080: 616d 6520 3d20 6879 706e 6f0d 0a76 6572  ame = hypno..ver
-00000090: 7369 6f6e 203d 2031 2e30 2e32 0d0a 6465  sion = 1.0.2..de
+00000090: 7369 6f6e 203d 2031 2e30 2e33 0d0a 6465  sion = 1.0.3..de
 000000a0: 7363 7269 7074 696f 6e20 3d20 4120 746f  scription = A to
 000000b0: 6f6c 2f6c 6962 7261 7279 2061 6c6c 6f77  ol/library allow
 000000c0: 696e 6720 746f 2069 6e6a 6563 7420 7079  ing to inject py
 000000d0: 7468 6f6e 2063 6f64 6520 696e 746f 2061  thon code into a
 000000e0: 2072 756e 6e69 6e67 2070 7974 686f 6e20   running python 
 000000f0: 7072 6f63 6573 732e 0d0a 6175 7468 6f72  process...author
 00000100: 203d 204d 616f 7220 4b6c 6569 6e62 6572   = Maor Kleinber
```

### Comparing `hypno-1.0.2/tests/test_hypno.py` & `hypno-1.0.3/tests/test_hypno.py`

 * *Files identical despite different names*


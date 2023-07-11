# Comparing `tmp/pyinjector-1.2.0.tar.gz` & `tmp/pyinjector-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinjector-1.2.0.tar", last modified: Sun Jul  2 22:54:31 2023, max compression
+gzip compressed data, was "pyinjector-1.2.1.tar", last modified: Tue Jul 11 21:59:02 2023, max compression
```

## Comparing `pyinjector-1.2.0.tar` & `pyinjector-1.2.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 22:54:31.788044 pyinjector-1.2.0/
--rw-rw-rw-   0        0        0     1092 2023-07-02 22:52:52.000000 pyinjector-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       83 2023-07-02 22:52:52.000000 pyinjector-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2597 2023-07-02 22:54:31.788044 pyinjector-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1675 2023-07-02 22:52:52.000000 pyinjector-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 22:54:31.768305 pyinjector-1.2.0/injector/
-drwxrwxrwx   0        0        0        0 2023-07-02 22:54:31.772457 pyinjector-1.2.0/injector/include/
--rw-rw-rw-   0        0        0     2764 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/include/injector.h
-drwxrwxrwx   0        0        0        0 2023-07-02 22:54:31.768305 pyinjector-1.2.0/injector/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 22:54:31.776690 pyinjector-1.2.0/injector/src/linux/
--rw-rw-rw-   0        0        0    15496 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/linux/elf.c
--rw-rw-rw-   0        0        0     6904 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/linux/injector.c
--rw-rw-rw-   0        0        0     4472 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/linux/injector_internal.h
--rw-rw-rw-   0        0        0     4511 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/linux/ptrace.c
--rw-rw-rw-   0        0        0    29132 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/linux/remote_call.c
--rw-rw-rw-   0        0        0     2479 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/linux/util.c
-drwxrwxrwx   0        0        0        0 2023-07-02 22:54:31.780816 pyinjector-1.2.0/injector/src/macos/
--rw-rw-rw-   0        0        0    11461 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/macos/exc_handler.c
--rw-rw-rw-   0        0        0     8987 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/macos/injector.c
--rw-rw-rw-   0        0        0     4012 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/macos/injector_internal.h
--rw-rw-rw-   0        0        0     3677 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/macos/mach.c
--rw-rw-rw-   0        0        0     9445 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/macos/mach_exc.h
--rw-rw-rw-   0        0        0    27231 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/macos/mach_excServer.c
--rw-rw-rw-   0        0        0     2519 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/macos/ptrace.c
--rw-rw-rw-   0        0        0     7540 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/macos/remote_call.c
--rw-rw-rw-   0        0        0     4260 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/macos/util.c
-drwxrwxrwx   0        0        0        0 2023-07-02 22:54:31.781849 pyinjector-1.2.0/injector/src/windows/
--rw-rw-rw-   0        0        0    28741 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/src/windows/injector.c
-drwxrwxrwx   0        0        0        0 2023-07-02 22:54:31.782909 pyinjector-1.2.0/injector/util/
--rw-rw-rw-   0        0        0     2872 2023-07-02 22:52:55.000000 pyinjector-1.2.0/injector/util/ya_getopt.h
--rw-rw-rw-   0        0        0       79 2023-07-02 22:52:52.000000 pyinjector-1.2.0/libinjector.c
-drwxrwxrwx   0        0        0        0 2023-07-02 22:54:31.782909 pyinjector-1.2.0/pyinjector/
--rw-rw-rw-   0        0        0      463 2023-07-02 22:52:52.000000 pyinjector-1.2.0/pyinjector/__init__.py
--rw-rw-rw-   0        0        0      727 2023-07-02 22:52:52.000000 pyinjector-1.2.0/pyinjector/__main__.py
--rw-rw-rw-   0        0        0     4184 2023-07-02 22:52:52.000000 pyinjector-1.2.0/pyinjector/api.py
-drwxrwxrwx   0        0        0        0 2023-07-02 22:54:31.786993 pyinjector-1.2.0/pyinjector.egg-info/
--rw-rw-rw-   0        0        0     2597 2023-07-02 22:54:31.000000 pyinjector-1.2.0/pyinjector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      905 2023-07-02 22:54:31.000000 pyinjector-1.2.0/pyinjector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 22:54:31.000000 pyinjector-1.2.0/pyinjector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-02 22:54:31.000000 pyinjector-1.2.0/pyinjector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-02 22:54:14.000000 pyinjector-1.2.0/pyinjector.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-07-02 22:54:31.000000 pyinjector-1.2.0/pyinjector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      962 2023-07-02 22:54:31.789072 pyinjector-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1035 2023-07-02 22:52:52.000000 pyinjector-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 22:54:31.788044 pyinjector-1.2.0/tests/
--rw-rw-rw-   0        0        0     1173 2023-07-02 22:52:52.000000 pyinjector-1.2.0/tests/test_pyinjector.py
+drwxrwxrwx   0        0        0        0 2023-07-11 21:59:02.431914 pyinjector-1.2.1/
+-rw-rw-rw-   0        0        0     1092 2023-07-11 21:56:53.000000 pyinjector-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0       83 2023-07-11 21:56:53.000000 pyinjector-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2603 2023-07-11 21:59:02.431914 pyinjector-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1681 2023-07-11 21:56:53.000000 pyinjector-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 21:59:02.411056 pyinjector-1.2.1/injector/
+drwxrwxrwx   0        0        0        0 2023-07-11 21:59:02.415200 pyinjector-1.2.1/injector/include/
+-rw-rw-rw-   0        0        0     2764 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/include/injector.h
+drwxrwxrwx   0        0        0        0 2023-07-11 21:59:02.409992 pyinjector-1.2.1/injector/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 21:59:02.419450 pyinjector-1.2.1/injector/src/linux/
+-rw-rw-rw-   0        0        0    15496 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/linux/elf.c
+-rw-rw-rw-   0        0        0     6904 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/linux/injector.c
+-rw-rw-rw-   0        0        0     4472 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/linux/injector_internal.h
+-rw-rw-rw-   0        0        0     4511 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/linux/ptrace.c
+-rw-rw-rw-   0        0        0    29132 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/linux/remote_call.c
+-rw-rw-rw-   0        0        0     2479 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/linux/util.c
+drwxrwxrwx   0        0        0        0 2023-07-11 21:59:02.424944 pyinjector-1.2.1/injector/src/macos/
+-rw-rw-rw-   0        0        0    11461 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/macos/exc_handler.c
+-rw-rw-rw-   0        0        0     8987 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/macos/injector.c
+-rw-rw-rw-   0        0        0     4012 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/macos/injector_internal.h
+-rw-rw-rw-   0        0        0     3677 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/macos/mach.c
+-rw-rw-rw-   0        0        0     9445 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/macos/mach_exc.h
+-rw-rw-rw-   0        0        0    27231 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/macos/mach_excServer.c
+-rw-rw-rw-   0        0        0     2519 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/macos/ptrace.c
+-rw-rw-rw-   0        0        0     7540 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/macos/remote_call.c
+-rw-rw-rw-   0        0        0     4260 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/macos/util.c
+drwxrwxrwx   0        0        0        0 2023-07-11 21:59:02.424944 pyinjector-1.2.1/injector/src/windows/
+-rw-rw-rw-   0        0        0    28741 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/src/windows/injector.c
+drwxrwxrwx   0        0        0        0 2023-07-11 21:59:02.425958 pyinjector-1.2.1/injector/util/
+-rw-rw-rw-   0        0        0     2872 2023-07-11 21:56:55.000000 pyinjector-1.2.1/injector/util/ya_getopt.h
+-rw-rw-rw-   0        0        0       79 2023-07-11 21:56:53.000000 pyinjector-1.2.1/libinjector.c
+drwxrwxrwx   0        0        0        0 2023-07-11 21:59:02.427431 pyinjector-1.2.1/pyinjector/
+-rw-rw-rw-   0        0        0      463 2023-07-11 21:56:53.000000 pyinjector-1.2.1/pyinjector/__init__.py
+-rw-rw-rw-   0        0        0      923 2023-07-11 21:56:53.000000 pyinjector-1.2.1/pyinjector/__main__.py
+-rw-rw-rw-   0        0        0     4913 2023-07-11 21:56:53.000000 pyinjector-1.2.1/pyinjector/api.py
+drwxrwxrwx   0        0        0        0 2023-07-11 21:59:02.430849 pyinjector-1.2.1/pyinjector.egg-info/
+-rw-rw-rw-   0        0        0     2603 2023-07-11 21:59:02.000000 pyinjector-1.2.1/pyinjector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      905 2023-07-11 21:59:02.000000 pyinjector-1.2.1/pyinjector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 21:59:02.000000 pyinjector-1.2.1/pyinjector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-11 21:59:02.000000 pyinjector-1.2.1/pyinjector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-11 21:58:47.000000 pyinjector-1.2.1/pyinjector.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-07-11 21:59:02.000000 pyinjector-1.2.1/pyinjector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      962 2023-07-11 21:59:02.432983 pyinjector-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2023-07-11 21:56:53.000000 pyinjector-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 21:59:02.430849 pyinjector-1.2.1/tests/
+-rw-rw-rw-   0        0        0     1173 2023-07-11 21:56:53.000000 pyinjector-1.2.1/tests/test_pyinjector.py
```

### Comparing `pyinjector-1.2.0/LICENSE` & `pyinjector-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/PKG-INFO` & `pyinjector-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinjector
-Version: 1.2.0
+Version: 1.2.1
 Summary: A tool/library allowing dynamic library injection into running processes
 Home-page: https://github.com/kmaork/pyinjector
 Author: Maor Kleinberger
 Author-email: kmaork@gmail.com
 Keywords: injection dll so library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -52,8 +52,8 @@
 
 inject(pid, path_to_so_file)
 ```
 
 ### How it works
 We build [kubo/injector](https://github.com/kubo/injector) as a C-extension and use its interface using `ctypes`.
 [kubo/injector](https://github.com/kubo/injector) is an awesome repo allowing to inject shared libraries into running
-processes both on windows (`CreateRemoteThread`+`LoadLibrary`) and on linux (`ptrace`).
+processes both on Windows (`CreateRemoteThread`), Linux (`ptrace`), and Mac (`task_for_pid`).
```

### Comparing `pyinjector-1.2.0/README.md` & `pyinjector-1.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 
 inject(pid, path_to_so_file)
 ```
 
 ### How it works
 We build [kubo/injector](https://github.com/kubo/injector) as a C-extension and use its interface using `ctypes`.
 [kubo/injector](https://github.com/kubo/injector) is an awesome repo allowing to inject shared libraries into running
-processes both on windows (`CreateRemoteThread`+`LoadLibrary`) and on linux (`ptrace`).
+processes both on Windows (`CreateRemoteThread`), Linux (`ptrace`), and Mac (`task_for_pid`).
```

### Comparing `pyinjector-1.2.0/injector/include/injector.h` & `pyinjector-1.2.1/injector/include/injector.h`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/linux/elf.c` & `pyinjector-1.2.1/injector/src/linux/elf.c`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/linux/injector.c` & `pyinjector-1.2.1/injector/src/linux/injector.c`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/linux/injector_internal.h` & `pyinjector-1.2.1/injector/src/linux/injector_internal.h`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/linux/ptrace.c` & `pyinjector-1.2.1/injector/src/linux/ptrace.c`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/linux/remote_call.c` & `pyinjector-1.2.1/injector/src/linux/remote_call.c`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/linux/util.c` & `pyinjector-1.2.1/injector/src/linux/util.c`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/macos/exc_handler.c` & `pyinjector-1.2.1/injector/src/macos/exc_handler.c`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/macos/injector.c` & `pyinjector-1.2.1/injector/src/macos/injector.c`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/macos/injector_internal.h` & `pyinjector-1.2.1/injector/src/macos/injector_internal.h`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/macos/mach.c` & `pyinjector-1.2.1/injector/src/macos/mach.c`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/macos/mach_exc.h` & `pyinjector-1.2.1/injector/src/macos/mach_exc.h`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/macos/mach_excServer.c` & `pyinjector-1.2.1/injector/src/macos/mach_excServer.c`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/macos/ptrace.c` & `pyinjector-1.2.1/injector/src/macos/ptrace.c`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/macos/remote_call.c` & `pyinjector-1.2.1/injector/src/macos/remote_call.c`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/macos/util.c` & `pyinjector-1.2.1/injector/src/macos/util.c`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/src/windows/injector.c` & `pyinjector-1.2.1/injector/src/windows/injector.c`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/injector/util/ya_getopt.h` & `pyinjector-1.2.1/injector/util/ya_getopt.h`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/pyinjector/__main__.py` & `pyinjector-1.2.1/pyinjector/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+import sys
 from argparse import ArgumentParser, Namespace
 from typing import List, Optional
 from pyinjector import inject
+from pyinjector.api import PyInjectorError
 
 
 def parse_args(args: Optional[List[str]]) -> Namespace:
     parser = ArgumentParser(description='Inject a dynamic library to a running process.')
     parser.add_argument('pid', type=int, help='pid of the process to inject the library into')
     parser.add_argument('library_path', type=str.encode, help='path of the library to inject')
     return parser.parse_args(args)
 
 
 def main(args: Optional[List[str]] = None) -> None:
     parsed_args = parse_args(args)
-    handle = inject(parsed_args.pid, parsed_args.library_path)
-    print(f"Handle: {handle}")
+    try:
+        handle = inject(parsed_args.pid, parsed_args.library_path)
+    except PyInjectorError as e:
+        print("pyinjector failed to inject: {}".format(e), file=sys.stderr)
+    else:
+        print(f"Handle: {handle}")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pyinjector-1.2.0/pyinjector.egg-info/PKG-INFO` & `pyinjector-1.2.1/pyinjector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinjector
-Version: 1.2.0
+Version: 1.2.1
 Summary: A tool/library allowing dynamic library injection into running processes
 Home-page: https://github.com/kmaork/pyinjector
 Author: Maor Kleinberger
 Author-email: kmaork@gmail.com
 Keywords: injection dll so library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -52,8 +52,8 @@
 
 inject(pid, path_to_so_file)
 ```
 
 ### How it works
 We build [kubo/injector](https://github.com/kubo/injector) as a C-extension and use its interface using `ctypes`.
 [kubo/injector](https://github.com/kubo/injector) is an awesome repo allowing to inject shared libraries into running
-processes both on windows (`CreateRemoteThread`+`LoadLibrary`) and on linux (`ptrace`).
+processes both on Windows (`CreateRemoteThread`), Linux (`ptrace`), and Mac (`task_for_pid`).
```

### Comparing `pyinjector-1.2.0/pyinjector.egg-info/SOURCES.txt` & `pyinjector-1.2.1/pyinjector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyinjector-1.2.0/setup.cfg` & `pyinjector-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b6f 7074 696f 6e73 5d0d 0a7a 6970 5f73  [options]..zip_s
 00000010: 6166 6520 3d20 4661 6c73 650d 0a70 7974  afe = False..pyt
 00000020: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
 00000030: 3d33 2e37 0d0a 7061 636b 6167 6573 203d  =3.7..packages =
 00000040: 2070 7969 6e6a 6563 746f 720d 0a0d 0a5b   pyinjector....[
 00000050: 6d65 7461 6461 7461 5d0d 0a6e 616d 6520  metadata]..name 
 00000060: 3d20 7079 696e 6a65 6374 6f72 0d0a 7665  = pyinjector..ve
-00000070: 7273 696f 6e20 3d20 312e 322e 300d 0a64  rsion = 1.2.0..d
+00000070: 7273 696f 6e20 3d20 312e 322e 310d 0a64  rsion = 1.2.1..d
 00000080: 6573 6372 6970 7469 6f6e 203d 2041 2074  escription = A t
 00000090: 6f6f 6c2f 6c69 6272 6172 7920 616c 6c6f  ool/library allo
 000000a0: 7769 6e67 2064 796e 616d 6963 206c 6962  wing dynamic lib
 000000b0: 7261 7279 2069 6e6a 6563 7469 6f6e 2069  rary injection i
 000000c0: 6e74 6f20 7275 6e6e 696e 6720 7072 6f63  nto running proc
 000000d0: 6573 7365 730d 0a61 7574 686f 7220 3d20  esses..author = 
 000000e0: 4d61 6f72 204b 6c65 696e 6265 7267 6572  Maor Kleinberger
```

### Comparing `pyinjector-1.2.0/setup.py` & `pyinjector-1.2.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from sys import platform
 from pathlib import Path
 from setuptools import setup, Extension
 
-WINDOWS = platform == 'win32'
 PROJECT_ROOT = Path(__file__).parent.resolve()
 LIBINJECTOR_DIR = PROJECT_ROOT / 'injector'
-LIBINJECTOR_SRC = LIBINJECTOR_DIR / 'src' / ('windows' if WINDOWS else 'linux')
+DIR_MAPPING = {
+    'linux': 'linux',
+    'win32': 'windows',
+    'darwin': 'macos',
+}
+LIBINJECTOR_SRC = LIBINJECTOR_DIR / 'src' / DIR_MAPPING[platform]
 LIBINJECTOR_WRAPPER = PROJECT_ROOT / 'libinjector.c'
 SOURCES = [str(c.relative_to(PROJECT_ROOT))
            for c in [LIBINJECTOR_WRAPPER, *LIBINJECTOR_SRC.iterdir()]
            if c.suffix == '.c']
 
 libinjector = Extension('pyinjector.libinjector',
                         sources=SOURCES,
```

### Comparing `pyinjector-1.2.0/tests/test_pyinjector.py` & `pyinjector-1.2.1/tests/test_pyinjector.py`

 * *Files identical despite different names*


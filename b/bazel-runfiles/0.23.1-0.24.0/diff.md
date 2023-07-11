# Comparing `tmp/bazel_runfiles-0.23.1-py3-none-any.whl.zip` & `tmp/bazel_runfiles-0.24.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 6980 bytes, number of entries: 5
--rw-r--r--  2.0 unx      628 b- defN 23-Jun-13 17:44 runfiles/__init__.py
--rw-r--r--  2.0 unx    14668 b- defN 23-Jun-13 17:44 runfiles/runfiles.py
-?rw-------  2.0 unx       91 b- defN 23-Jun-13 17:45 bazel_runfiles-0.23.1.dist-info/WHEEL
-?rw-------  2.0 unx     2066 b- defN 23-Jun-13 17:45 bazel_runfiles-0.23.1.dist-info/METADATA
-?rw-------  2.0 unx      384 b- defN 23-Jun-13 17:45 bazel_runfiles-0.23.1.dist-info/RECORD
-5 files, 17837 bytes uncompressed, 6268 bytes compressed:  64.9%
+Zip file size: 7003 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      628 b- defN 23-Jul-11 22:30 runfiles/__init__.py
+-rw-r--r--  2.0 unx    14668 b- defN 23-Jul-11 22:30 runfiles/runfiles.py
+?rw-------  2.0 unx       91 b- defN 23-Jul-11 22:31 bazel_runfiles-0.24.0.dist-info/WHEEL
+?rw-------  2.0 unx     2103 b- defN 23-Jul-11 22:31 bazel_runfiles-0.24.0.dist-info/METADATA
+?rw-------  2.0 unx      384 b- defN 23-Jul-11 22:31 bazel_runfiles-0.24.0.dist-info/RECORD
+5 files, 17874 bytes uncompressed, 6291 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: runfiles/__init__.py
 Comment: 
 
 Filename: runfiles/runfiles.py
 Comment: 
 
-Filename: bazel_runfiles-0.23.1.dist-info/WHEEL
+Filename: bazel_runfiles-0.24.0.dist-info/WHEEL
 Comment: 
 
-Filename: bazel_runfiles-0.23.1.dist-info/METADATA
+Filename: bazel_runfiles-0.24.0.dist-info/METADATA
 Comment: 
 
-Filename: bazel_runfiles-0.23.1.dist-info/RECORD
+Filename: bazel_runfiles-0.24.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bazel_runfiles-0.23.1.dist-info/METADATA` & `bazel_runfiles-0.24.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: bazel_runfiles
 Home-page: https://github.com/bazelbuild/rules_python
+Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
-Version: 0.23.1
+Version: 0.24.0
 
 bazel-runfiles library
 ======================
 
 This is a Bazel Runfiles lookup library for Bazel-built Python binaries and tests.
 
 Learn about runfiles: read `Runfiles guide <https://bazel.build/extending/rules#runfiles>`_
```


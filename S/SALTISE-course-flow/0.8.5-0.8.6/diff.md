# Comparing `tmp/SALTISE_course_flow-0.8.5.tar.gz` & `tmp/SALTISE_course_flow-0.8.6.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SALTISE_course_flow-0.8.5.tar", last modified: Mon Jun  5 03:24:28 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


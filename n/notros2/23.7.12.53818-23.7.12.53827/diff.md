# Comparing `tmp/notros2-23.7.12.53818.tar.gz` & `tmp/notros2-23.7.12.53827-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notros2-23.7.12.53818.tar", last modified: Wed Jul 12 05:38:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


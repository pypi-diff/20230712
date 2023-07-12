# Comparing `tmp/labcams-0.6.5.tar.gz` & `tmp/labcams-0.6.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labcams-0.6.5.tar", last modified: Wed Aug 17 02:16:26 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


# Comparing `tmp/notros2-23.7.12.65325.tar.gz` & `tmp/notros2-23.7.12.65333-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notros2-23.7.12.65325.tar", last modified: Wed Jul 12 06:53:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


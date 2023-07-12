# Comparing `tmp/mobicontrol-0.2.0.tar.gz` & `tmp/mobicontrol-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobicontrol-0.2.0.tar", last modified: Fri May 12 07:37:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


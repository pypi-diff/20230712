# Comparing `tmp/androidMemoryTool-0.4.tar.gz` & `tmp/androidMemoryTool-0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "androidMemoryTool-0.4.tar", last modified: Tue Nov 22 17:42:24 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


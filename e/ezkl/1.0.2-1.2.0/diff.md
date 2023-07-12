# Comparing `tmp/ezkl-1.0.2.tar.gz` & `tmp/ezkl-1.2.0-cp37-abi3-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezkl-1.0.2.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


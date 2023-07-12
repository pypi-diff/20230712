# Comparing `tmp/botocore-a-la-carte-braket-1.31.1.tar.gz` & `tmp/botocore_a_la_carte_braket-1.31.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-braket-1.31.1.tar", last modified: Sat Jul  8 01:42:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


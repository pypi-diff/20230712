# Comparing `tmp/symbolica-0.0.1.tar.gz` & `tmp/symbolica-0.0.2-cp311-cp311-manylinux_2_34_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


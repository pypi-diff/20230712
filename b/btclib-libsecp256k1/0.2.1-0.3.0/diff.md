# Comparing `tmp/btclib_libsecp256k1-0.2.1.tar.gz` & `tmp/btclib_libsecp256k1-0.3.0-py3-none-macosx_10_16_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/btclib_libsecp256k1-0.2.1.tar", last modified: Mon Jan 30 17:56:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


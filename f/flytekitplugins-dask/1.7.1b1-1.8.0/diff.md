# Comparing `tmp/flytekitplugins-dask-1.7.1b1.tar.gz` & `tmp/flytekitplugins_dask-1.8.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-dask-1.7.1b1.tar", last modified: Tue Jun 27 22:00:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


# Comparing `tmp/confluent-kafka-2.1.1.tar.gz` & `tmp/confluent_kafka-2.2.0-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/confluent-kafka-2.1.1.tar", last modified: Thu May  4 10:28:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


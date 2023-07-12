# Comparing `tmp/ML_Algo-1.0.9.tar.gz` & `tmp/ML_Algo-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ML_Algo-1.0.9.tar", last modified: Wed Jul 12 12:31:05 2023, max compression
+gzip compressed data, was "ML_Algo-1.2.tar", last modified: Wed Jul 12 12:42:55 2023, max compression
```

## Comparing `ML_Algo-1.0.9.tar` & `ML_Algo-1.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 12:31:05.080212 ML_Algo-1.0.9/
--rw-rw-rw-   0        0        0      164 2023-07-12 12:31:05.078214 ML_Algo-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-12 12:31:05.080212 ML_Algo-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      331 2023-07-12 12:30:40.000000 ML_Algo-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:31:05.062662 ML_Algo-1.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 12:31:05.077214 ML_Algo-1.0.9/src/ML_Algo.egg-info/
--rw-rw-rw-   0        0        0      164 2023-07-12 12:31:04.000000 ML_Algo-1.0.9/src/ML_Algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-07-12 12:31:04.000000 ML_Algo-1.0.9/src/ML_Algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 12:31:04.000000 ML_Algo-1.0.9/src/ML_Algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 12:31:04.000000 ML_Algo-1.0.9/src/ML_Algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 12:31:04.000000 ML_Algo-1.0.9/src/ML_Algo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 12:42:55.761444 ML_Algo-1.2/
+drwxrwxrwx   0        0        0        0 2023-07-12 12:42:55.759409 ML_Algo-1.2/ML_Algo.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-07-12 12:42:55.000000 ML_Algo-1.2/ML_Algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-07-12 12:42:55.000000 ML_Algo-1.2/ML_Algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:42:55.000000 ML_Algo-1.2/ML_Algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-12 12:42:55.000000 ML_Algo-1.2/ML_Algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:42:55.000000 ML_Algo-1.2/ML_Algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      162 2023-07-12 12:42:55.760420 ML_Algo-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-12 12:42:55.761444 ML_Algo-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      257 2023-07-12 12:42:33.000000 ML_Algo-1.2/setup.py
```


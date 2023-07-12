# Comparing `tmp/ML_Algo-1.0.8.tar.gz` & `tmp/ML_Algo-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ML_Algo-1.0.8.tar", last modified: Wed Jul 12 12:07:27 2023, max compression
+gzip compressed data, was "ML_Algo-1.0.9.tar", last modified: Wed Jul 12 12:31:05 2023, max compression
```

## Comparing `ML_Algo-1.0.8.tar` & `ML_Algo-1.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 12:07:27.069578 ML_Algo-1.0.8/
--rw-rw-rw-   0        0        0      164 2023-07-12 12:07:27.069578 ML_Algo-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-12 12:07:27.069578 ML_Algo-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      331 2023-07-12 12:06:53.000000 ML_Algo-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:07:27.062573 ML_Algo-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 12:07:27.068580 ML_Algo-1.0.8/src/ML_Algo.egg-info/
--rw-rw-rw-   0        0        0      164 2023-07-12 12:07:26.000000 ML_Algo-1.0.8/src/ML_Algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-07-12 12:07:26.000000 ML_Algo-1.0.8/src/ML_Algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 12:07:26.000000 ML_Algo-1.0.8/src/ML_Algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 12:07:26.000000 ML_Algo-1.0.8/src/ML_Algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 12:07:26.000000 ML_Algo-1.0.8/src/ML_Algo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 12:31:05.080212 ML_Algo-1.0.9/
+-rw-rw-rw-   0        0        0      164 2023-07-12 12:31:05.078214 ML_Algo-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-12 12:31:05.080212 ML_Algo-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      331 2023-07-12 12:30:40.000000 ML_Algo-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:31:05.062662 ML_Algo-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 12:31:05.077214 ML_Algo-1.0.9/src/ML_Algo.egg-info/
+-rw-rw-rw-   0        0        0      164 2023-07-12 12:31:04.000000 ML_Algo-1.0.9/src/ML_Algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-07-12 12:31:04.000000 ML_Algo-1.0.9/src/ML_Algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:31:04.000000 ML_Algo-1.0.9/src/ML_Algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 12:31:04.000000 ML_Algo-1.0.9/src/ML_Algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:31:04.000000 ML_Algo-1.0.9/src/ML_Algo.egg-info/top_level.txt
```


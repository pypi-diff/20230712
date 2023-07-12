# Comparing `tmp/ML_Algo-1.0.5.tar.gz` & `tmp/ML_Algo-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ML_Algo-1.0.5.tar", last modified: Tue Jul 11 17:57:24 2023, max compression
+gzip compressed data, was "ML_Algo-1.0.6.tar", last modified: Wed Jul 12 09:49:38 2023, max compression
```

## Comparing `ML_Algo-1.0.5.tar` & `ML_Algo-1.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 17:57:24.722843 ML_Algo-1.0.5/
--rw-rw-rw-   0        0        0      164 2023-07-11 17:57:24.722843 ML_Algo-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-11 17:57:24.722843 ML_Algo-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      331 2023-07-11 17:57:06.000000 ML_Algo-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:57:24.715845 ML_Algo-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 17:57:24.721866 ML_Algo-1.0.5/src/ML_Algo.egg-info/
--rw-rw-rw-   0        0        0      164 2023-07-11 17:57:24.000000 ML_Algo-1.0.5/src/ML_Algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-07-11 17:57:24.000000 ML_Algo-1.0.5/src/ML_Algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 17:57:24.000000 ML_Algo-1.0.5/src/ML_Algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 17:57:24.000000 ML_Algo-1.0.5/src/ML_Algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 17:57:24.000000 ML_Algo-1.0.5/src/ML_Algo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 09:49:38.076620 ML_Algo-1.0.6/
+-rw-rw-rw-   0        0        0      164 2023-07-12 09:49:38.075595 ML_Algo-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-12 09:49:38.076620 ML_Algo-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      331 2023-07-12 09:49:19.000000 ML_Algo-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 09:49:38.065580 ML_Algo-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 09:49:38.074586 ML_Algo-1.0.6/src/ML_Algo.egg-info/
+-rw-rw-rw-   0        0        0      164 2023-07-12 09:49:37.000000 ML_Algo-1.0.6/src/ML_Algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-07-12 09:49:37.000000 ML_Algo-1.0.6/src/ML_Algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 09:49:37.000000 ML_Algo-1.0.6/src/ML_Algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 09:49:37.000000 ML_Algo-1.0.6/src/ML_Algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 09:49:37.000000 ML_Algo-1.0.6/src/ML_Algo.egg-info/top_level.txt
```


# Comparing `tmp/histoencoder-0.1.0.tar.gz` & `tmp/histoencoder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histoencoder-0.1.0.tar", max compression
+gzip compressed data, was "histoencoder-0.1.1.tar", max compression
```

## Comparing `histoencoder-0.1.0.tar` & `histoencoder-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2759 2023-06-14 10:31:09.625455 histoencoder-0.1.0/README.md
--rw-r--r--   0        0        0       86 2023-04-28 11:25:04.501204 histoencoder-0.1.0/histoencoder/__init__.py
--rw-r--r--   0        0        0       60 2023-05-02 15:04:07.266112 histoencoder-0.1.0/histoencoder/_cli/__init__.py
--rw-r--r--   0        0        0     2918 2023-05-30 08:02:16.298516 histoencoder-0.1.0/histoencoder/_cli/_cluster.py
--rw-r--r--   0        0        0     8776 2023-05-04 10:40:47.723906 histoencoder-0.1.0/histoencoder/_cli/_extract.py
--rw-r--r--   0        0        0      810 2023-05-30 08:01:34.857070 histoencoder-0.1.0/histoencoder/_cli/_run.py
--rw-r--r--   0        0        0      456 2023-05-03 07:37:01.508057 histoencoder-0.1.0/histoencoder/_cli/_utils.py
--rw-r--r--   0        0        0      566 2023-05-02 13:52:20.308906 histoencoder-0.1.0/histoencoder/functional/__init__.py
--rw-r--r--   0        0        0      269 2023-04-28 11:25:26.373968 histoencoder-0.1.0/histoencoder/functional/_check.py
--rw-r--r--   0        0        0     2203 2023-05-03 09:22:56.468638 histoencoder-0.1.0/histoencoder/functional/_cluster.py
--rw-r--r--   0        0        0     4336 2023-05-30 13:51:44.048630 histoencoder-0.1.0/histoencoder/functional/_features.py
--rw-r--r--   0        0        0     2970 2023-04-19 10:57:04.844368 histoencoder-0.1.0/histoencoder/functional/_freeze.py
--rw-r--r--   0        0        0     1243 2023-05-30 08:12:09.195215 histoencoder-0.1.0/histoencoder/functional/_model.py
--rw-r--r--   0        0        0     3141 2023-04-19 11:47:02.841651 histoencoder-0.1.0/histoencoder/functional/_params.py
--rw-r--r--   0        0        0     5912 2023-05-04 10:40:44.839805 histoencoder-0.1.0/histoencoder/functional/_writer.py
--rw-r--r--   0        0        0      573 2023-06-14 10:33:30.310353 histoencoder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3390 1970-01-01 00:00:00.000000 histoencoder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5778 2023-07-09 12:35:19.071762 histoencoder-0.1.1/README.md
+-rw-r--r--   0        0        0       86 2023-04-28 11:25:04.501204 histoencoder-0.1.1/histoencoder/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-02 15:04:07.266112 histoencoder-0.1.1/histoencoder/_cli/__init__.py
+-rw-r--r--   0        0        0     2918 2023-05-30 08:02:16.298516 histoencoder-0.1.1/histoencoder/_cli/_cluster.py
+-rw-r--r--   0        0        0     8776 2023-05-04 10:40:47.723906 histoencoder-0.1.1/histoencoder/_cli/_extract.py
+-rw-r--r--   0        0        0      810 2023-05-30 08:01:34.857070 histoencoder-0.1.1/histoencoder/_cli/_run.py
+-rw-r--r--   0        0        0      456 2023-05-03 07:37:01.508057 histoencoder-0.1.1/histoencoder/_cli/_utils.py
+-rw-r--r--   0        0        0      566 2023-05-02 13:52:20.308906 histoencoder-0.1.1/histoencoder/functional/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-28 11:25:26.373968 histoencoder-0.1.1/histoencoder/functional/_check.py
+-rw-r--r--   0        0        0     2203 2023-05-03 09:22:56.468638 histoencoder-0.1.1/histoencoder/functional/_cluster.py
+-rw-r--r--   0        0        0     4336 2023-05-30 13:51:44.048630 histoencoder-0.1.1/histoencoder/functional/_features.py
+-rw-r--r--   0        0        0     2970 2023-04-19 10:57:04.844368 histoencoder-0.1.1/histoencoder/functional/_freeze.py
+-rw-r--r--   0        0        0     1243 2023-05-30 08:12:09.195215 histoencoder-0.1.1/histoencoder/functional/_model.py
+-rw-r--r--   0        0        0     3141 2023-04-19 11:47:02.841651 histoencoder-0.1.1/histoencoder/functional/_params.py
+-rw-r--r--   0        0        0     5912 2023-05-04 10:40:44.839805 histoencoder-0.1.1/histoencoder/functional/_writer.py
+-rw-r--r--   0        0        0      576 2023-07-12 08:49:15.719666 histoencoder-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6422 1970-01-01 00:00:00.000000 histoencoder-0.1.1/PKG-INFO
```

### Comparing `histoencoder-0.1.0/histoencoder/_cli/_cluster.py` & `histoencoder-0.1.1/histoencoder/_cli/_cluster.py`

 * *Files identical despite different names*

### Comparing `histoencoder-0.1.0/histoencoder/_cli/_extract.py` & `histoencoder-0.1.1/histoencoder/_cli/_extract.py`

 * *Files identical despite different names*

### Comparing `histoencoder-0.1.0/histoencoder/_cli/_run.py` & `histoencoder-0.1.1/histoencoder/_cli/_run.py`

 * *Files identical despite different names*

### Comparing `histoencoder-0.1.0/histoencoder/functional/__init__.py` & `histoencoder-0.1.1/histoencoder/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `histoencoder-0.1.0/histoencoder/functional/_cluster.py` & `histoencoder-0.1.1/histoencoder/functional/_cluster.py`

 * *Files identical despite different names*

### Comparing `histoencoder-0.1.0/histoencoder/functional/_features.py` & `histoencoder-0.1.1/histoencoder/functional/_features.py`

 * *Files identical despite different names*

### Comparing `histoencoder-0.1.0/histoencoder/functional/_freeze.py` & `histoencoder-0.1.1/histoencoder/functional/_freeze.py`

 * *Files identical despite different names*

### Comparing `histoencoder-0.1.0/histoencoder/functional/_model.py` & `histoencoder-0.1.1/histoencoder/functional/_model.py`

 * *Files identical despite different names*

### Comparing `histoencoder-0.1.0/histoencoder/functional/_params.py` & `histoencoder-0.1.1/histoencoder/functional/_params.py`

 * *Files identical despite different names*

### Comparing `histoencoder-0.1.0/histoencoder/functional/_writer.py` & `histoencoder-0.1.1/histoencoder/functional/_writer.py`

 * *Files identical despite different names*

### Comparing `histoencoder-0.1.0/pyproject.toml` & `histoencoder-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "histoencoder"
-version = "0.1.0"
+version = "0.1.1"
 description = "Foundation models for digital pathology."
 authors = ["jopo666 <jopo@birdlover.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 HistoEncoder = 'histoencoder._cli:run'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 timm = "^0.5"
 torch = "^2"
 torchvision = "^0.15"
 histoprep = "^2"
 rich-click = "^1.6"
-scikit-learn = "*"
+scikit-learn = "^1.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 pytest-console-scripts = "^1.3.1"
 pdoc = "^13.1.1"
 
 [build-system]
```


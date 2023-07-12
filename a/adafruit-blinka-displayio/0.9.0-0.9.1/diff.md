# Comparing `tmp/adafruit-blinka-displayio-0.9.0.tar.gz` & `tmp/adafruit-blinka-displayio-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-blinka-displayio-0.9.0.tar", last modified: Tue Feb  8 14:57:26 2022, max compression
+gzip compressed data, was "adafruit-blinka-displayio-0.9.1.tar", last modified: Wed Mar 23 18:44:56 2022, max compression
```

## Comparing `adafruit-blinka-displayio-0.9.0.tar` & `adafruit-blinka-displayio-0.9.1.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 14:57:26.718295 adafruit-blinka-displayio-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 14:57:26.706296 adafruit-blinka-displayio-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 14:57:26.710296 adafruit-blinka-displayio-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16271 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6225 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 14:57:26.710296 adafruit-blinka-displayio-0.9.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-02-08 14:57:26.718295 adafruit-blinka-displayio-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1960 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 14:57:26.714295 adafruit-blinka-displayio-0.9.0/adafruit_blinka_displayio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-02-08 14:57:26.000000 adafruit-blinka-displayio-0.9.0/adafruit_blinka_displayio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-02-08 14:57:26.000000 adafruit-blinka-displayio-0.9.0/adafruit_blinka_displayio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-08 14:57:26.000000 adafruit-blinka-displayio-0.9.0/adafruit_blinka_displayio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-02-08 14:57:26.000000 adafruit-blinka-displayio-0.9.0/adafruit_blinka_displayio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-02-08 14:57:26.000000 adafruit-blinka-displayio-0.9.0/adafruit_blinka_displayio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 14:57:26.714295 adafruit-blinka-displayio-0.9.0/displayio/
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4061 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_area.py
--rw-r--r--   0 runner    (1001) docker     (121)     4830 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_bitmap.py
--rw-r--r--   0 runner    (1001) docker     (121)     4343 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_colorconverter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_colorspace.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    16559 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_display.py
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_displaybus.py
--rw-r--r--   0 runner    (1001) docker     (121)     9665 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_displaycore.py
--rw-r--r--   0 runner    (1001) docker     (121)     6508 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_epaperdisplay.py
--rw-r--r--   0 runner    (1001) docker     (121)     4504 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_fourwire.py
--rw-r--r--   0 runner    (1001) docker     (121)     8873 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     3588 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_i2cdisplay.py
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_ondiskbitmap.py
--rw-r--r--   0 runner    (1001) docker     (121)     4177 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_palette.py
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_shape.py
--rw-r--r--   0 runner    (1001) docker     (121)     1428 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_structs.py
--rw-r--r--   0 runner    (1001) docker     (121)    14959 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/displayio/_tilegrid.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 14:57:26.718295 adafruit-blinka-displayio-0.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 14:57:26.718295 adafruit-blinka-displayio-0.9.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5662 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     3045 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/fontio.py
--rw-r--r--   0 runner    (1001) docker     (121)     2389 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/paralleldisplay.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-08 14:57:26.718295 adafruit-blinka-displayio-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-02-08 14:57:04.000000 adafruit-blinka-displayio-0.9.0/terminalio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:44:56.360346 adafruit-blinka-displayio-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:44:56.348346 adafruit-blinka-displayio-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:44:56.352346 adafruit-blinka-displayio-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16271 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6225 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:44:56.356346 adafruit-blinka-displayio-0.9.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-03-23 18:44:56.360346 adafruit-blinka-displayio-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1960 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:44:56.356346 adafruit-blinka-displayio-0.9.1/adafruit_blinka_displayio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-03-23 18:44:56.000000 adafruit-blinka-displayio-0.9.1/adafruit_blinka_displayio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-03-23 18:44:56.000000 adafruit-blinka-displayio-0.9.1/adafruit_blinka_displayio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 18:44:56.000000 adafruit-blinka-displayio-0.9.1/adafruit_blinka_displayio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-03-23 18:44:56.000000 adafruit-blinka-displayio-0.9.1/adafruit_blinka_displayio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-03-23 18:44:56.000000 adafruit-blinka-displayio-0.9.1/adafruit_blinka_displayio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:44:56.360346 adafruit-blinka-displayio-0.9.1/displayio/
+-rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4061 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_area.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4830 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4343 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_colorconverter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16611 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_display.py
+-rw-r--r--   0 runner    (1001) docker     (121)      665 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_displaybus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9767 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_displaycore.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6597 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_epaperdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4624 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_fourwire.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8873 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_i2cdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_ondiskbitmap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4203 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_palette.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_shape.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1428 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_structs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14959 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/displayio/_tilegrid.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:44:56.360346 adafruit-blinka-displayio-0.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:44:56.360346 adafruit-blinka-displayio-0.9.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5662 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      858 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     3045 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/fontio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/paralleldisplay.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-23 18:44:56.360346 adafruit-blinka-displayio-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1956 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2022-03-23 18:44:42.000000 adafruit-blinka-displayio-0.9.1/terminalio.py
```

### Comparing `adafruit-blinka-displayio-0.9.0/.github/workflows/build.yml` & `adafruit-blinka-displayio-0.9.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/.github/workflows/release.yml` & `adafruit-blinka-displayio-0.9.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/.pre-commit-config.yaml` & `adafruit-blinka-displayio-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/.pylintrc` & `adafruit-blinka-displayio-0.9.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/CODE_OF_CONDUCT.md` & `adafruit-blinka-displayio-0.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/LICENSE` & `adafruit-blinka-displayio-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/LICENSES/CC-BY-4.0.txt` & `adafruit-blinka-displayio-0.9.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/LICENSES/MIT.txt` & `adafruit-blinka-displayio-0.9.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/LICENSES/Unlicense.txt` & `adafruit-blinka-displayio-0.9.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/PKG-INFO` & `adafruit-blinka-displayio-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-blinka-displayio
-Version: 0.9.0
+Version: 0.9.1
 Summary: displayio for Blinka
 Home-page: https://github.com/adafruit/Adafruit_Blinka_Displayio
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython displayio lcd tft display pitft
 Platform: UNKNOWN
```

### Comparing `adafruit-blinka-displayio-0.9.0/README.rst` & `adafruit-blinka-displayio-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/adafruit_blinka_displayio.egg-info/PKG-INFO` & `adafruit-blinka-displayio-0.9.1/adafruit_blinka_displayio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-blinka-displayio
-Version: 0.9.0
+Version: 0.9.1
 Summary: displayio for Blinka
 Home-page: https://github.com/adafruit/Adafruit_Blinka_Displayio
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython displayio lcd tft display pitft
 Platform: UNKNOWN
```

### Comparing `adafruit-blinka-displayio-0.9.0/adafruit_blinka_displayio.egg-info/SOURCES.txt` & `adafruit-blinka-displayio-0.9.1/adafruit_blinka_displayio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
-_typing.py
 fontio.py
 paralleldisplay.py
 requirements.txt
 setup.py
 terminalio.py
 .github/workflows/build.yml
 .github/workflows/release.yml
```

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/__init__.py` & `adafruit-blinka-displayio-0.9.1/displayio/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_area.py` & `adafruit-blinka-displayio-0.9.1/displayio/_area.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_bitmap.py` & `adafruit-blinka-displayio-0.9.1/displayio/_bitmap.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_colorconverter.py` & `adafruit-blinka-displayio-0.9.1/displayio/_colorconverter.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_colorspace.py` & `adafruit-blinka-displayio-0.9.1/displayio/_colorspace.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_display.py` & `adafruit-blinka-displayio-0.9.1/displayio/_display.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import threading
 from typing import Optional
 from dataclasses import astuple
 import digitalio
 from PIL import Image
 import numpy
 import microcontroller
-import _typing
+import circuitpython_typing
 from ._displaycore import _DisplayCore
 from ._displaybus import _DisplayBus
 from ._colorconverter import ColorConverter
 from ._group import Group
 from ._structs import RectangleStruct
 from ._constants import (
     CHIP_SELECT_TOGGLE_EVERY_BYTE,
@@ -56,15 +56,15 @@
     Most people should not use this class directly. Use a specific display driver instead
     that will contain the initialization sequence at minimum.
     """
 
     def __init__(
         self,
         display_bus: _DisplayBus,
-        init_sequence: _typing.ReadableBuffer,
+        init_sequence: circuitpython_typing.ReadableBuffer,
         *,
         width: int,
         height: int,
         colstart: int = 0,
         rowstart: int = 0,
         rotation: int = 0,
         color_depth: int = 16,
@@ -363,16 +363,16 @@
         return rectangle
 
     def _encode_pos(self, x, y):
         """Encode a postion into bytes."""
         return struct.pack(self._bounds_encoding, x, y)  # pylint: disable=no-member
 
     def fill_row(
-        self, y: int, buffer: _typing.WriteableBuffer
-    ) -> _typing.WriteableBuffer:
+        self, y: int, buffer: circuitpython_typing.WriteableBuffer
+    ) -> circuitpython_typing.WriteableBuffer:
         """Extract the pixels from a single row"""
         for x in range(0, self._width):
             _rgb_565 = self._colorconverter.convert(self._buffer.getpixel((x, y)))
             buffer[x * 2] = (_rgb_565 >> 8) & 0xFF
             buffer[x * 2 + 1] = _rgb_565 & 0xFF
         return buffer
```

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_displaybus.py` & `adafruit-blinka-displayio-0.9.1/displayio/_displaybus.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_displaycore.py` & `adafruit-blinka-displayio-0.9.1/displayio/_displaycore.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_Displayio.git"
 
 
 from typing import Union
-import _typing
+import circuitpython_typing
 from paralleldisplay import ParallelBus
 from ._fourwire import FourWire
 from ._group import Group
 from ._i2cdisplay import I2CDisplay
 from ._structs import ColorspaceStruct, TransformStruct, RectangleStruct
 from ._area import Area
 
@@ -223,15 +223,18 @@
         """Release the display from the current group"""
         # pylint: disable=protected-access
 
         if self._current_group is not None:
             self._current_group._in_group = False
 
     def fill_area(
-        self, area: Area, mask: _typing.WriteableBuffer, buffer: _typing.WriteableBuffer
+        self,
+        area: Area,
+        mask: circuitpython_typing.WriteableBuffer,
+        buffer: circuitpython_typing.WriteableBuffer,
     ) -> bool:
         # pylint: disable=protected-access
         """Call the current group's fill area function"""
 
         return self._current_group._fill_area(self._colorspace, area, mask, buffer)
 
     def clip_area(self, area: Area, clipped: Area) -> bool:
@@ -257,15 +260,18 @@
                     clipped.y1 -= clipped.y1 % pixels_per_byte
                 if clipped.y2 % pixels_per_byte != 0:
                     clipped.y2 += pixels_per_byte - clipped.y2 % pixels_per_byte
 
         return True
 
     def send(
-        self, data_type: int, chip_select: int, data: _typing.ReadableBuffer
+        self,
+        data_type: int,
+        chip_select: int,
+        data: circuitpython_typing.ReadableBuffer,
     ) -> None:
         """
         Send the data to the current bus
         """
         self._send(data_type, chip_select, data)
 
     def begin_transaction(self) -> None:
```

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_epaperdisplay.py` & `adafruit-blinka-displayio-0.9.1/displayio/_epaperdisplay.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 * Author(s): Melissa LeBlanc-Williams
 
 """
 
 from typing import Optional
 import microcontroller
-import _typing
+import circuitpython_typing
 from ._group import Group
 from ._displaybus import _DisplayBus
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_displayio.git"
 
 
@@ -38,16 +38,16 @@
     Most people should not use this class directly. Use a specific display driver instead
     that will contain the startup and shutdown sequences at minimum.
     """
 
     def __init__(
         self,
         display_bus: _DisplayBus,
-        start_sequence: _typing.ReadableBuffer,
-        stop_sequence: _typing.ReadableBuffer,
+        start_sequence: circuitpython_typing.ReadableBuffer,
+        stop_sequence: circuitpython_typing.ReadableBuffer,
         *,
         width: int,
         height: int,
         ram_width: int,
         ram_height: int,
         colstart: int = 0,
         rowstart: int = 0,
@@ -80,16 +80,18 @@
         next byte will be the delay time in milliseconds. The remaining 7 bits are the
         parameter count excluding any delay byte. The third through final bytes are the
         remaining command parameters. The next byte will begin a new command definition.
 
 
         :param display_bus: The bus that the display is connected to
         :type _DisplayBus: displayio.FourWire or displayio.ParallelBus
-        :param ~_typing.ReadableBuffer start_sequence: Byte-packed initialization sequence.
-        :param ~_typing.ReadableBuffer stop_sequence: Byte-packed initialization sequence.
+        :param ~circuitpython_typing.ReadableBuffer start_sequence: Byte-packed
+            initialization sequence.
+        :param ~circuitpython_typing.ReadableBuffer stop_sequence: Byte-packed
+            initialization sequence.
         :param int width: Width in pixels
         :param int height: Height in pixels
         :param int ram_width: RAM width in pixels
         :param int ram_height: RAM height in pixels
         :param int colstart: The index if the first visible column
         :param int rowstart: The index if the first visible row
         :param int rotation: The rotation of the display in degrees clockwise. Must be in
```

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_fourwire.py` & `adafruit-blinka-displayio-0.9.1/displayio/_fourwire.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 
 import time
 from typing import Optional
 import digitalio
 import busio
 import microcontroller
-import _typing
+import circuitpython_typing
 from ._constants import (
     CHIP_SELECT_TOGGLE_EVERY_BYTE,
     CHIP_SELECT_UNTOUCHED,
     DISPLAY_COMMAND,
     DISPLAY_DATA,
 )
 
@@ -89,34 +89,43 @@
         if self._reset is not None:
             self._reset.value = False
             time.sleep(0.001)
             self._reset.value = True
             time.sleep(0.001)
 
     def send(
-        self, command, data: _typing.ReadableBuffer, *, toggle_every_byte: bool = False
+        self,
+        command,
+        data: circuitpython_typing.ReadableBuffer,
+        *,
+        toggle_every_byte: bool = False,
     ) -> None:
         """
         Sends the given command value followed by the full set of data. Display state,
         such as vertical scroll, set via ``send`` may or may not be reset once the code is
         done.
         """
         if not 0 <= command <= 255:
             raise ValueError("Command must be an int between 0 and 255")
         chip_select = (
             CHIP_SELECT_TOGGLE_EVERY_BYTE
             if toggle_every_byte
             else CHIP_SELECT_UNTOUCHED
         )
         self._begin_transaction()
-        self._send(DISPLAY_COMMAND, chip_select, command)
+        self._send(DISPLAY_COMMAND, chip_select, bytes([command]))
         self._send(DISPLAY_DATA, chip_select, data)
         self._end_transaction()
 
-    def _send(self, data_type: int, chip_select: int, data: _typing.ReadableBuffer):
+    def _send(
+        self,
+        data_type: int,
+        chip_select: int,
+        data: circuitpython_typing.ReadableBuffer,
+    ):
         self._dc.value = data_type == DISPLAY_DATA
         if chip_select == CHIP_SELECT_TOGGLE_EVERY_BYTE:
             for byte in data:
                 self._spi.write(bytes([byte]))
                 self._chip_select.value = True
                 time.sleep(0.000001)
                 self._chip_select.value = False
```

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_group.py` & `adafruit-blinka-displayio-0.9.1/displayio/_group.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_i2cdisplay.py` & `adafruit-blinka-displayio-0.9.1/displayio/_i2cdisplay.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 * Author(s): Melissa LeBlanc-Williams, Erik Tollerud, James Carr
 
 """
 
 import time
 import busio
 import digitalio
-import _typing
+import circuitpython_typing
 from ._constants import CHIP_SELECT_UNTOUCHED, DISPLAY_COMMAND
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_displayio.git"
 
 
 class I2CDisplay:
@@ -72,25 +72,30 @@
         self._reset.value = True
 
     def _begin_transaction(self) -> None:
         """Lock the bus before sending data."""
         while not self._i2c.try_lock():
             pass
 
-    def send(self, command: int, data: _typing.ReadableBuffer) -> None:
+    def send(self, command: int, data: circuitpython_typing.ReadableBuffer) -> None:
         """
         Sends the given command value followed by the full set of data. Display state,
         such as vertical scroll, set via ``send`` may or may not be reset once the code is
         done.
         """
         self._begin_transaction()
         self._send(DISPLAY_COMMAND, CHIP_SELECT_UNTOUCHED, bytes([command] + data))
         self._end_transaction()
 
-    def _send(self, data_type: int, chip_select: int, data: _typing.ReadableBuffer):
+    def _send(
+        self,
+        data_type: int,
+        chip_select: int,
+        data: circuitpython_typing.ReadableBuffer,
+    ):
         # pylint: disable=unused-argument
         if data_type == DISPLAY_COMMAND:
             n = len(data)
             if n > 0:
                 command_bytes = bytearray(n * 2)
                 for i in range(n):
                     command_bytes[2 * i] = 0x80
```

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_ondiskbitmap.py` & `adafruit-blinka-displayio-0.9.1/displayio/_ondiskbitmap.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_palette.py` & `adafruit-blinka-displayio-0.9.1/displayio/_palette.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   https://github.com/adafruit/Adafruit_Blinka/releases
 
 * Author(s): Melissa LeBlanc-Williams
 
 """
 
 from typing import Optional, Union, Tuple
-import _typing
+import circuitpython_typing
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_displayio.git"
 
 
 class Palette:
     """Map a pixel palette_index to a full color. Colors are transformed to the display’s
@@ -69,15 +69,15 @@
     def __len__(self) -> int:
         """Returns the number of colors in a Palette"""
         return len(self._colors)
 
     def __setitem__(
         self,
         index: int,
-        value: Union[int, _typing.ReadableBuffer, Tuple[int, int, int]],
+        value: Union[int, circuitpython_typing.ReadableBuffer, Tuple[int, int, int]],
     ) -> None:
         """Sets the pixel color at the given index. The index should be
         an integer in the range 0 to color_count-1.
 
         The value argument represents a color, and can be from 0x000000 to 0xFFFFFF
         (to represent an RGB value). Value can be an int, bytes (3 bytes (RGB) or
         4 bytes (RGB + pad byte)), bytearray, or a tuple or list of 3 integers.
```

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_shape.py` & `adafruit-blinka-displayio-0.9.1/displayio/_shape.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_structs.py` & `adafruit-blinka-displayio-0.9.1/displayio/_structs.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/displayio/_tilegrid.py` & `adafruit-blinka-displayio-0.9.1/displayio/_tilegrid.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/docs/_static/favicon.ico` & `adafruit-blinka-displayio-0.9.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/docs/api.rst` & `adafruit-blinka-displayio-0.9.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/docs/conf.py` & `adafruit-blinka-displayio-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/docs/index.rst` & `adafruit-blinka-displayio-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/fontio.py` & `adafruit-blinka-displayio-0.9.1/fontio.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-displayio-0.9.0/paralleldisplay.py` & `adafruit-blinka-displayio-0.9.1/paralleldisplay.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   https://github.com/adafruit/Adafruit_Blinka/releases
 
 * Author(s): Melissa LeBlanc-Williams
 
 """
 
 import microcontroller
-import _typing
+import circuitpython_typing
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_displayio.git"
 
 
 class ParallelBus:
     """Manage updating a display over 8-bit parallel bus in the background while Python code
@@ -57,13 +57,13 @@
 
     def reset(self) -> None:
         """Performs a hardware reset via the reset pin. Raises an exception if called when
         no reset pin is available.
         """
         raise NotImplementedError("ParallelBus reset has not been implemented yet")
 
-    def send(self, command: int, data: _typing.ReadableBuffer) -> None:
+    def send(self, command: int, data: circuitpython_typing.ReadableBuffer) -> None:
         """Sends the given command value followed by the full set of data. Display state,
         such as vertical scroll, set via ``send`` may or may not be reset once the code is
         done.
         """
         raise NotImplementedError("ParallelBus send has not been implemented yet")
```

### Comparing `adafruit-blinka-displayio-0.9.0/setup.py` & `adafruit-blinka-displayio-0.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     long_description_content_type="text/x-rst",
     # The project's main homepage.
     url="https://github.com/adafruit/Adafruit_Blinka_Displayio",
     # Author details
     author="Adafruit Industries",
     author_email="circuitpython@adafruit.com",
     install_requires=[
-        "Adafruit-Blinka",
+        "Adafruit-Blinka>=7.0.0",
+        "adafruit-circuitpython-typing",
         "pillow",
         "numpy",
     ],
     # Choose your license
     license="MIT",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
@@ -50,10 +51,10 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
     ],
     # What does your project relate to?
     keywords="adafruit blinka circuitpython micropython displayio lcd tft display pitft",
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
-    py_modules=["fontio", "terminalio", "paralleldisplay", "_typing"],
+    py_modules=["fontio", "terminalio", "paralleldisplay"],
     packages=["displayio"],
 )
```

### Comparing `adafruit-blinka-displayio-0.9.0/terminalio.py` & `adafruit-blinka-displayio-0.9.1/terminalio.py`

 * *Files identical despite different names*


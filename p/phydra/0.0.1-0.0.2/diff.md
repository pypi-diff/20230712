# Comparing `tmp/phydra-0.0.1.tar.gz` & `tmp/phydra-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phydra-0.0.1.tar", last modified: Mon May  4 02:29:28 2020, max compression
+gzip compressed data, was "phydra-0.0.2.tar", max compression
```

## Comparing `phydra-0.0.1.tar` & `phydra-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,28 @@
-drwxr-xr-x   0 bpo        (502) staff       (20)        0 2020-05-04 02:29:28.000000 phydra-0.0.1/
--rw-r--r--   0 bpo        (502) staff       (20)      336 2020-05-04 02:29:28.000000 phydra-0.0.1/PKG-INFO
-drwxr-xr-x   0 bpo        (502) staff       (20)        0 2020-05-04 02:29:28.000000 phydra-0.0.1/phydra.egg-info/
--rw-r--r--   0 bpo        (502) staff       (20)      336 2020-05-04 02:29:28.000000 phydra-0.0.1/phydra.egg-info/PKG-INFO
--rw-r--r--   0 bpo        (502) staff       (20)      128 2020-05-04 02:29:28.000000 phydra-0.0.1/phydra.egg-info/SOURCES.txt
--rw-r--r--   0 bpo        (502) staff       (20)        1 2020-05-04 02:29:28.000000 phydra-0.0.1/phydra.egg-info/dependency_links.txt
--rw-r--r--   0 bpo        (502) staff       (20)        1 2020-05-04 02:29:28.000000 phydra-0.0.1/phydra.egg-info/top_level.txt
--rw-r--r--   0 bpo        (502) staff       (20)       38 2020-05-04 02:29:28.000000 phydra-0.0.1/setup.cfg
--rw-r--r--   0 bpo        (502) staff       (20)      406 2020-05-04 02:27:08.000000 phydra-0.0.1/setup.py
+-rwxr-xr-x   0        0        0     1516 2023-03-03 22:41:48.786498 phydra-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3279 2023-07-10 12:28:00.696790 phydra-0.0.2/README.md
+-rw-r--r--   0        0        0      388 2023-07-11 13:40:05.618873 phydra-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-05 20:14:23.170393 phydra-0.0.2/src/phydra/__init__.py
+-rw-r--r--   0        0        0      151 2023-07-05 21:47:35.421493 phydra-0.0.2/src/phydra/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-07-05 21:00:33.844637 phydra-0.0.2/src/phydra/models/chemostat/__init__.py
+-rw-r--r--   0        0        0      574 2023-07-09 21:57:07.501198 phydra-0.0.2/src/phydra/models/chemostat/_models.py
+-rw-r--r--   0        0        0     1489 2023-07-09 21:59:15.775970 phydra-0.0.2/src/phydra/models/chemostat/fluxes.py
+-rw-r--r--   0        0        0     2138 2023-07-09 21:41:30.710652 phydra-0.0.2/src/phydra/models/chemostat/forcings.py
+-rw-r--r--   0        0        0      243 2023-07-09 21:57:07.497914 phydra-0.0.2/src/phydra/models/chemostat/variables.py
+-rw-r--r--   0        0        0       77 2023-07-09 14:22:28.542899 phydra-0.0.2/src/phydra/models/sizebased/__init__.py
+-rw-r--r--   0        0        0      871 2023-07-09 21:17:08.964780 phydra-0.0.2/src/phydra/models/sizebased/_models.py
+-rw-r--r--   0        0        0       36 2023-07-09 14:22:28.546637 phydra-0.0.2/src/phydra/models/sizebased/fluxes/__init__.py
+-rw-r--r--   0        0        0     1580 2023-07-10 20:58:46.727552 phydra-0.0.2/src/phydra/models/sizebased/fluxes/basic.py
+-rw-r--r--   0        0        0     3175 2023-07-09 13:53:24.456465 phydra-0.0.2/src/phydra/models/sizebased/fluxes/grazing.py
+-rw-r--r--   0        0        0      666 2023-07-09 13:48:15.749045 phydra-0.0.2/src/phydra/models/sizebased/fluxes/growth.py
+-rw-r--r--   0        0        0      574 2023-07-08 09:28:20.415189 phydra-0.0.2/src/phydra/models/sizebased/forcings.py
+-rw-r--r--   0        0        0     1619 2023-07-09 21:16:56.110420 phydra-0.0.2/src/phydra/models/sizebased/variables.py
+-rw-r--r--   0        0        0       56 2023-07-05 21:58:54.236897 phydra-0.0.2/src/phydra/models/slabocean/__init__.py
+-rw-r--r--   0        0        0     1593 2023-07-05 21:47:35.425415 phydra-0.0.2/src/phydra/models/slabocean/_models.py
+-rw-r--r--   0        0        0        1 2023-07-05 21:34:36.736474 phydra-0.0.2/src/phydra/models/slabocean/fluxes/__init__.py
+-rw-r--r--   0        0        0     1023 2023-07-05 21:34:36.728780 phydra-0.0.2/src/phydra/models/slabocean/fluxes/basic.py
+-rw-r--r--   0        0        0     1825 2023-07-05 21:47:35.423633 phydra-0.0.2/src/phydra/models/slabocean/fluxes/grazing.py
+-rw-r--r--   0        0        0     8109 2023-07-05 21:34:36.740285 phydra-0.0.2/src/phydra/models/slabocean/fluxes/growth.py
+-rw-r--r--   0        0        0     1706 2023-07-05 21:34:36.734878 phydra-0.0.2/src/phydra/models/slabocean/fluxes/mixing.py
+-rw-r--r--   0        0        0     6187 2023-07-05 21:34:36.738382 phydra-0.0.2/src/phydra/models/slabocean/forcings.py
+-rw-r--r--   0        0        0      162 2023-07-05 21:34:36.741325 phydra-0.0.2/src/phydra/models/slabocean/variables.py
+-rw-r--r--   0        0        0     3783 1970-01-01 00:00:00.000000 phydra-0.0.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```


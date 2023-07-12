# Comparing `tmp/xso-0.0.1.tar.gz` & `tmp/xso-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xso-0.0.1.tar", last modified: Wed Feb 24 12:32:57 2021, max compression
+gzip compressed data, was "xso-0.0.2.tar", max compression
```

## Comparing `xso-0.0.1.tar` & `xso-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxr-xr-x   0 bpo        (502) staff       (20)        0 2021-02-24 12:32:57.833231 xso-0.0.1/
--rw-r--r--   0 bpo        (502) staff       (20)      352 2021-02-24 12:32:57.832834 xso-0.0.1/PKG-INFO
--rw-r--r--   0 bpo        (502) staff       (20)       38 2021-02-24 12:32:57.833462 xso-0.0.1/setup.cfg
--rw-r--r--   0 bpo        (502) staff       (20)      422 2021-02-24 12:30:11.000000 xso-0.0.1/setup.py
-drwxr-xr-x   0 bpo        (502) staff       (20)        0 2021-02-24 12:32:57.832325 xso-0.0.1/xso.egg-info/
--rw-r--r--   0 bpo        (502) staff       (20)      352 2021-02-24 12:32:56.000000 xso-0.0.1/xso.egg-info/PKG-INFO
--rw-r--r--   0 bpo        (502) staff       (20)      116 2021-02-24 12:32:56.000000 xso-0.0.1/xso.egg-info/SOURCES.txt
--rw-r--r--   0 bpo        (502) staff       (20)        1 2021-02-24 12:32:56.000000 xso-0.0.1/xso.egg-info/dependency_links.txt
--rw-r--r--   0 bpo        (502) staff       (20)        1 2021-02-24 12:32:56.000000 xso-0.0.1/xso.egg-info/top_level.txt
+-rwxr-xr-x   0        0        0     1514 2023-03-03 22:41:01.663778 xso-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3048 2023-03-03 22:41:01.663882 xso-0.0.2/README.md
+-rw-r--r--   0        0        0      673 2023-07-11 13:40:05.620809 xso-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-09 14:16:37.934652 xso-0.0.2/src/xso/__init__.py
+-rw-r--r--   0        0        0     7702 2023-07-10 19:15:07.487130 xso-0.0.2/src/xso/backendcomps.py
+-rw-r--r--   0        0        0    23120 2023-07-09 19:41:12.784520 xso-0.0.2/src/xso/component.py
+-rw-r--r--   0        0        0     5132 2023-03-03 22:41:01.666823 xso-0.0.2/src/xso/core.py
+-rw-r--r--   0        0        0     7344 2023-07-10 21:29:49.567155 xso-0.0.2/src/xso/model.py
+-rw-r--r--   0        0        0    16340 2023-07-10 21:55:30.098011 xso-0.0.2/src/xso/solvers.py
+-rw-r--r--   0        0        0     9027 2023-07-09 14:26:51.963518 xso-0.0.2/src/xso/variables.py
+-rw-r--r--   0        0        0     6227 2023-07-09 21:12:25.451042 xso-0.0.2/src/xso/xsimlabwrappers.py
+-rw-r--r--   0        0        0     3771 1970-01-01 00:00:00.000000 xso-0.0.2/PKG-INFO
```


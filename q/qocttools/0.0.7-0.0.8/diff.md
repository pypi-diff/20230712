# Comparing `tmp/qocttools-0.0.7.tar.gz` & `tmp/qocttools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qocttools-0.0.7.tar", last modified: Thu Feb  9 16:48:35 2023, max compression
+gzip compressed data, was "qocttools-0.0.8.tar", last modified: Fri Feb 17 19:47:38 2023, max compression
```

## Comparing `qocttools-0.0.7.tar` & `qocttools-0.0.8.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.563756 qocttools-0.0.7/
--rw-r--r--   0 alberto   (1000) alberto   (1000)    35149 2023-02-09 16:25:26.000000 qocttools-0.0.7/LICENSE
--rw-r--r--   0 alberto   (1000) alberto   (1000)       90 2023-02-09 16:25:26.000000 qocttools-0.0.7/MANIFEST.in
--rw-r--r--   0 alberto   (1000) alberto   (1000)     1236 2023-02-09 16:48:35.563756 qocttools-0.0.7/PKG-INFO
--rw-r--r--   0 alberto   (1000) alberto   (1000)      404 2023-02-09 16:25:26.000000 qocttools-0.0.7/Pipfile
--rw-r--r--   0 alberto   (1000) alberto   (1000)      664 2023-02-09 16:25:26.000000 qocttools-0.0.7/README.rst
--rw-r--r--   0 alberto   (1000) alberto   (1000)     1030 2023-02-09 16:47:59.000000 qocttools-0.0.7/pyproject.toml
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.547756 qocttools-0.0.7/qocttools/
--rw-r--r--   0 alberto   (1000) alberto   (1000)     2276 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/__init__.py
--rw-r--r--   0 alberto   (1000) alberto   (1000)   835835 2023-02-09 16:48:34.000000 qocttools-0.0.7/qocttools/cythonfuncs.c
--rw-r--r--   0 alberto   (1000) alberto   (1000)     1559 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/cythonfuncs.pyx
--rw-r--r--   0 alberto   (1000) alberto   (1000)    14349 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/floquet.py
--rw-r--r--   0 alberto   (1000) alberto   (1000)     5740 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/hamiltonians.py
--rw-r--r--   0 alberto   (1000) alberto   (1000)    17507 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/krotov.py
--rw-r--r--   0 alberto   (1000) alberto   (1000)    11378 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/math_extra.py
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.555756 qocttools-0.0.7/qocttools/models/
--rw-r--r--   0 alberto   (1000) alberto   (1000)     2602 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/models/GdW30.py
--rw-r--r--   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/models/__init__.py
--rw-r--r--   0 alberto   (1000) alberto   (1000)     2943 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/models/graphene.py
--rw-r--r--   0 alberto   (1000) alberto   (1000)     4478 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/models/hBN.py
--rw-r--r--   0 alberto   (1000) alberto   (1000)     7189 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/models/tmd.py
--rw-r--r--   0 alberto   (1000) alberto   (1000)    21038 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/pulses.py
--rw-r--r--   0 alberto   (1000) alberto   (1000)    28074 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/qoct.py
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.543756 qocttools-0.0.7/qocttools/sampleruns/
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.555756 qocttools-0.0.7/qocttools/sampleruns/dissipation/
--rw-r--r--   0 alberto   (1000) alberto   (1000)     6233 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/dissipation/GdW30_Toffoli_Syvstime_15dB.dat
--rw-r--r--   0 alberto   (1000) alberto   (1000)       43 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/dissipation/data.ref
--rw-r--r--   0 alberto   (1000) alberto   (1000)    12214 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/dissipation/dissipation.ipynb
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.555756 qocttools-0.0.7/qocttools/sampleruns/floquet/
--rw-r--r--   0 alberto   (1000) alberto   (1000)      243 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/floquet/Ax0
--rw-r--r--   0 alberto   (1000) alberto   (1000)      244 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/floquet/Ay0
--rw-r--r--   0 alberto   (1000) alberto   (1000)      109 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/floquet/data.ref
--rw-r--r--   0 alberto   (1000) alberto   (1000)    98380 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/floquet/floquet.ipynb
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.555756 qocttools-0.0.7/qocttools/sampleruns/gradient/
--rw-r--r--   0 alberto   (1000) alberto   (1000)     2319 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/gradient/V
--rw-r--r--   0 alberto   (1000) alberto   (1000)      130 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/gradient/data.ref
--rw-r--r--   0 alberto   (1000) alberto   (1000)    20388 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/gradient/gradient.ipynb
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.555756 qocttools-0.0.7/qocttools/sampleruns/gradient-2perts/
--rw-r--r--   0 alberto   (1000) alberto   (1000)      132 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/gradient-2perts/data.ref
--rw-r--r--   0 alberto   (1000) alberto   (1000)    48216 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/gradient-2perts/gradient-2perts.ipynb
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.559756 qocttools-0.0.7/qocttools/sampleruns/gradient-dissipation/
--rw-r--r--   0 alberto   (1000) alberto   (1000)     2319 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/gradient-dissipation/V
--rw-r--r--   0 alberto   (1000) alberto   (1000)      107 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/gradient-dissipation/data.ref
--rw-r--r--   0 alberto   (1000) alberto   (1000)    25348 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/gradient-dissipation/gradient-dissipation.ipynb
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.559756 qocttools-0.0.7/qocttools/sampleruns/gradient-dissipation-multitarget/
--rw-r--r--   0 alberto   (1000) alberto   (1000)       22 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/gradient-dissipation-multitarget/data.ref
--rw-r--r--   0 alberto   (1000) alberto   (1000)    12253 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/gradient-dissipation-multitarget/gradient-dissipation-multitarget.ipynb
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.559756 qocttools-0.0.7/qocttools/sampleruns/model/
--rw-r--r--   0 alberto   (1000) alberto   (1000)      344 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/model/data.ref
--rw-r--r--   0 alberto   (1000) alberto   (1000)     4573 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/model/model.ipynb
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.559756 qocttools-0.0.7/qocttools/sampleruns/pipulse/
--rw-r--r--   0 alberto   (1000) alberto   (1000)       42 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/pipulse/data.ref
--rw-r--r--   0 alberto   (1000) alberto   (1000)    17793 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/pipulse/pipulse.ipynb
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.559756 qocttools-0.0.7/qocttools/sampleruns/propagators/
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.559756 qocttools-0.0.7/qocttools/sampleruns/propagators/.ipynb_checkpoints/
--rw-r--r--   0 alberto   (1000) alberto   (1000)    45412 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/propagators/.ipynb_checkpoints/generic_propagation-checkpoint.ipynb
--rw-r--r--   0 alberto   (1000) alberto   (1000)      210 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/propagators/data.ref
--rw-r--r--   0 alberto   (1000) alberto   (1000)    21234 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/propagators/propagators.ipynb
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.559756 qocttools-0.0.7/qocttools/sampleruns/qoctbasic/
--rw-r--r--   0 alberto   (1000) alberto   (1000)     2319 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/qoctbasic/V
--rw-r--r--   0 alberto   (1000) alberto   (1000)       64 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/qoctbasic/data.ref
--rw-r--r--   0 alberto   (1000) alberto   (1000)    14778 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/qoctbasic/qoctbasic.ipynb
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.559756 qocttools-0.0.7/qocttools/sampleruns/qoctbasic-krotov/
--rw-r--r--   0 alberto   (1000) alberto   (1000)     2319 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/qoctbasic-krotov/V
--rw-r--r--   0 alberto   (1000) alberto   (1000)       42 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/qoctbasic-krotov/data.ref
--rw-r--r--   0 alberto   (1000) alberto   (1000)    13061 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/qoctbasic-krotov/qoctbasic-krotov.ipynb
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.559756 qocttools-0.0.7/qocttools/sampleruns/qocttoffoli/
--rw-r--r--   0 alberto   (1000) alberto   (1000)     2319 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/qocttoffoli/V
--rw-r--r--   0 alberto   (1000) alberto   (1000)       21 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/qocttoffoli/data.ref
--rw-r--r--   0 alberto   (1000) alberto   (1000)     4417 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/qocttoffoli/optimal-pulse.csv
--rw-r--r--   0 alberto   (1000) alberto   (1000)    19174 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/sampleruns/qocttoffoli/qocttoffoli.ipynb
--rw-r--r--   0 alberto   (1000) alberto   (1000)    17582 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/solvers.py
--rw-r--r--   0 alberto   (1000) alberto   (1000)     9370 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/target.py
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.563756 qocttools-0.0.7/qocttools/tests/
--rw-r--r--   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/tests/__init__.py
--rw-r--r--   0 alberto   (1000) alberto   (1000)     2070 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/tests/long.py
--rw-r--r--   0 alberto   (1000) alberto   (1000)     3682 2023-02-09 16:25:26.000000 qocttools-0.0.7/qocttools/tests/short.py
-drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-09 16:48:35.547756 qocttools-0.0.7/qocttools.egg-info/
--rw-r--r--   0 alberto   (1000) alberto   (1000)     1236 2023-02-09 16:48:35.000000 qocttools-0.0.7/qocttools.egg-info/PKG-INFO
--rw-r--r--   0 alberto   (1000) alberto   (1000)     2308 2023-02-09 16:48:35.000000 qocttools-0.0.7/qocttools.egg-info/SOURCES.txt
--rw-r--r--   0 alberto   (1000) alberto   (1000)        1 2023-02-09 16:48:35.000000 qocttools-0.0.7/qocttools.egg-info/dependency_links.txt
--rw-r--r--   0 alberto   (1000) alberto   (1000)      140 2023-02-09 16:48:35.000000 qocttools-0.0.7/qocttools.egg-info/requires.txt
--rw-r--r--   0 alberto   (1000) alberto   (1000)       10 2023-02-09 16:48:35.000000 qocttools-0.0.7/qocttools.egg-info/top_level.txt
--rw-r--r--   0 alberto   (1000) alberto   (1000)       38 2023-02-09 16:48:35.563756 qocttools-0.0.7/setup.cfg
--rw-r--r--   0 alberto   (1000) alberto   (1000)      350 2023-02-09 16:25:26.000000 qocttools-0.0.7/setup.py
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.102016 qocttools-0.0.8/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    35149 2023-02-17 19:20:22.000000 qocttools-0.0.8/LICENSE
+-rw-r--r--   0 alberto   (1000) alberto   (1000)       90 2023-02-17 19:20:22.000000 qocttools-0.0.8/MANIFEST.in
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     1236 2023-02-17 19:47:38.098016 qocttools-0.0.8/PKG-INFO
+-rw-r--r--   0 alberto   (1000) alberto   (1000)      404 2023-02-17 19:20:22.000000 qocttools-0.0.8/Pipfile
+-rw-r--r--   0 alberto   (1000) alberto   (1000)      664 2023-02-17 19:20:22.000000 qocttools-0.0.8/README.rst
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     1030 2023-02-17 19:45:19.000000 qocttools-0.0.8/pyproject.toml
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.094016 qocttools-0.0.8/qocttools/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     2276 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/__init__.py
+-rw-r--r--   0 alberto   (1000) alberto   (1000)   835835 2023-02-17 19:47:37.000000 qocttools-0.0.8/qocttools/cythonfuncs.c
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     1559 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/cythonfuncs.pyx
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    14621 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/floquet.py
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     5740 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/hamiltonians.py
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    17546 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/krotov.py
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    11378 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/math_extra.py
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.094016 qocttools-0.0.8/qocttools/models/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     2602 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/models/GdW30.py
+-rw-r--r--   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/models/__init__.py
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     2943 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/models/graphene.py
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     4478 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/models/hBN.py
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     7189 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/models/tmd.py
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    21038 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/pulses.py
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    28074 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/qoct.py
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.090016 qocttools-0.0.8/qocttools/sampleruns/
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.094016 qocttools-0.0.8/qocttools/sampleruns/dissipation/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     6233 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/dissipation/GdW30_Toffoli_Syvstime_15dB.dat
+-rw-r--r--   0 alberto   (1000) alberto   (1000)       43 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/dissipation/data.ref
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    12191 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/dissipation/dissipation.ipynb
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.094016 qocttools-0.0.8/qocttools/sampleruns/floquet/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)      243 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/floquet/Ax0
+-rw-r--r--   0 alberto   (1000) alberto   (1000)      244 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/floquet/Ay0
+-rw-r--r--   0 alberto   (1000) alberto   (1000)      109 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/floquet/data.ref
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    29454 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/floquet/floquet.ipynb
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.098016 qocttools-0.0.8/qocttools/sampleruns/gradient/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     2319 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/gradient/V
+-rw-r--r--   0 alberto   (1000) alberto   (1000)      130 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/gradient/data.ref
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    20622 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/gradient/gradient.ipynb
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.098016 qocttools-0.0.8/qocttools/sampleruns/gradient-2perts/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)      132 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/gradient-2perts/data.ref
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    17161 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/gradient-2perts/gradient-2perts.ipynb
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.098016 qocttools-0.0.8/qocttools/sampleruns/gradient-dissipation/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     2319 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/gradient-dissipation/V
+-rw-r--r--   0 alberto   (1000) alberto   (1000)      107 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/gradient-dissipation/data.ref
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    25325 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/gradient-dissipation/gradient-dissipation.ipynb
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.098016 qocttools-0.0.8/qocttools/sampleruns/gradient-dissipation-multitarget/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)       21 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/gradient-dissipation-multitarget/data.ref
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    11763 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/gradient-dissipation-multitarget/gradient-dissipation-multitarget.ipynb
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.098016 qocttools-0.0.8/qocttools/sampleruns/model/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)      344 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/model/data.ref
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     4550 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/model/model.ipynb
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.098016 qocttools-0.0.8/qocttools/sampleruns/pipulse/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)       42 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/pipulse/data.ref
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    17770 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/pipulse/pipulse.ipynb
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.098016 qocttools-0.0.8/qocttools/sampleruns/propagators/
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.098016 qocttools-0.0.8/qocttools/sampleruns/propagators/.ipynb_checkpoints/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    45412 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/propagators/.ipynb_checkpoints/generic_propagation-checkpoint.ipynb
+-rw-r--r--   0 alberto   (1000) alberto   (1000)      210 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/propagators/data.ref
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    21211 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/propagators/propagators.ipynb
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.098016 qocttools-0.0.8/qocttools/sampleruns/qoctbasic/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     2319 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/qoctbasic/V
+-rw-r--r--   0 alberto   (1000) alberto   (1000)       64 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/qoctbasic/data.ref
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    15063 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/qoctbasic/qoctbasic.ipynb
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.098016 qocttools-0.0.8/qocttools/sampleruns/qoctbasic-krotov/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     2319 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/qoctbasic-krotov/V
+-rw-r--r--   0 alberto   (1000) alberto   (1000)       42 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/qoctbasic-krotov/data.ref
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    13018 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/qoctbasic-krotov/qoctbasic-krotov.ipynb
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.098016 qocttools-0.0.8/qocttools/sampleruns/qocttoffoli/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     2319 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/qocttoffoli/V
+-rw-r--r--   0 alberto   (1000) alberto   (1000)       21 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/qocttoffoli/data.ref
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     4417 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/qocttoffoli/optimal-pulse.csv
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    19151 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/sampleruns/qocttoffoli/qocttoffoli.ipynb
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    17582 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/solvers.py
+-rw-r--r--   0 alberto   (1000) alberto   (1000)    11836 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/target.py
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.098016 qocttools-0.0.8/qocttools/tests/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/tests/__init__.py
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     2070 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/tests/long.py
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     3682 2023-02-17 19:20:22.000000 qocttools-0.0.8/qocttools/tests/short.py
+drwxr-xr-x   0 alberto   (1000) alberto   (1000)        0 2023-02-17 19:47:38.094016 qocttools-0.0.8/qocttools.egg-info/
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     1236 2023-02-17 19:47:38.000000 qocttools-0.0.8/qocttools.egg-info/PKG-INFO
+-rw-r--r--   0 alberto   (1000) alberto   (1000)     2308 2023-02-17 19:47:38.000000 qocttools-0.0.8/qocttools.egg-info/SOURCES.txt
+-rw-r--r--   0 alberto   (1000) alberto   (1000)        1 2023-02-17 19:47:38.000000 qocttools-0.0.8/qocttools.egg-info/dependency_links.txt
+-rw-r--r--   0 alberto   (1000) alberto   (1000)      140 2023-02-17 19:47:38.000000 qocttools-0.0.8/qocttools.egg-info/requires.txt
+-rw-r--r--   0 alberto   (1000) alberto   (1000)       10 2023-02-17 19:47:38.000000 qocttools-0.0.8/qocttools.egg-info/top_level.txt
+-rw-r--r--   0 alberto   (1000) alberto   (1000)       38 2023-02-17 19:47:38.102016 qocttools-0.0.8/setup.cfg
+-rw-r--r--   0 alberto   (1000) alberto   (1000)      350 2023-02-17 19:20:22.000000 qocttools-0.0.8/setup.py
```

### Comparing `qocttools-0.0.7/LICENSE` & `qocttools-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/PKG-INFO` & `qocttools-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qocttools
-Version: 0.0.7
+Version: 0.0.8
 Summary: A set of tools to do quantum optimal control calculations
 Author-email: Alberto Castro <alberto.castro.barrigon@gmail.com>
 Project-URL: Homepage, https://qocttools.readthedocs.io/
 Project-URL: Bug Tracker, https://gitlab.com/acbarrigon/qocttools/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `qocttools-0.0.7/README.rst` & `qocttools-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/pyproject.toml` & `qocttools-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qocttools"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Alberto Castro", email="alberto.castro.barrigon@gmail.com" },
 ]
 description = "A set of tools to do quantum optimal control calculations"
 readme = "README.rst"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `qocttools-0.0.7/qocttools/__init__.py` & `qocttools-0.0.8/qocttools/__init__.py`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/cythonfuncs.c` & `qocttools-0.0.8/qocttools/cythonfuncs.c`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/cythonfuncs.pyx` & `qocttools-0.0.8/qocttools/cythonfuncs.pyx`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/floquet.py` & `qocttools-0.0.8/qocttools/floquet.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,31 @@
 ## but WITHOUT ANY WARRANTY; without even the implied warranty of
 ## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ## GNU General Public License for more details.
 ##
 ## You should have received a copy of the GNU General Public License
 ## along with qocttools.  If not, see <https://www.gnu.org/licenses/>.
 
+"""This module contains all the procedures needed to do Floquet optimization.
+
+(...)
+"""
+
 import qutip as qt
 import numpy as np
 import scipy as scp
 import scipy.linalg as la
 import qocttools.pulses as pulses
 from qocttools.math_extra import diff_ridders
 
 
 def epsi(UT, T):
+    """
+    (...)
+    """
     # In principle, one needs the eigenvalues. But what if UT cannot be diagonalized?
     # We will use then the Schur decomposition, and use the diagonal elements of the
     # Schur matrix.
     #evals, evecs = la.eig(UT)
     dim = UT.shape[0]
     S, Z = la.schur(UT)
     evals = np.zeros(dim, dtype = complex)
@@ -36,32 +44,41 @@
     eargs = np.angle(evals)
     eargs += (eargs <= -np.pi) * (2 * np.pi) + (eargs > np.pi) * (-2 * np.pi)
     epsilon = -eargs / T
     return np.sort(epsilon)
 
 
 def epsilon(H, T, args = None):
+    """
+    (...)
+    """
     options = qt.Options(nsteps = 10000)
     #U = qt.propagator(H, T, args = args, options = options)
     ntsteps = 5
     dim = 3
     #print(ntsteps)
     U = (qt.sesolve(H, qt.qeye(dim), np.linspace(0, T, ntsteps), options = options, args = args)).states[-1]
     ualpha, epsilon = qt.floquet_modes(H, T, U = U)
     idx = epsilon.argsort()
     return epsilon[idx]
 
 
 def epsilon2(H0, H1, H2, Ax, Ay, u, T):
+    """
+    (...)
+    """
     pulses.pulse_collection_set_parameters([Ax, Ay], u)
     H = [H0, [H1, Ax.f], [H2, Ay.f]]
     return epsilon(H, T)
 
 
 def epsilon3(H, f, u, T):
+    """
+    (...)
+    """
     pulses.pulse_collection_set_parameters(f, u)
     if H.function:
         args = { "f": [f[l].fu for l in range(len(f))] }
         H_ = H.H0
     else:
         args = None
         H_ = [H.H0]
@@ -69,14 +86,17 @@
         for V in H.V:
             H_.append([V, f[k].f])
             k = k + 1
     return epsilon(H_, T, args = args)
 
 
 def gradepsilon(H, f, u, T):
+    """
+    (...)
+    """
     dim = H.dim
     pulses.pulse_collection_set_parameters(f, u)
 
     if H.function:
         options = qt.Options(nsteps = 10000)
         args = { "f": [f[l].fu for l in range(len(f))] }
         H_ = H.H0
@@ -139,14 +159,17 @@
                     res[alpha, m] = res[alpha, m] + 0.5 * (qt.expect(V, ualphat[-1][alpha]) * ft.dfu(times[-1], k) )
             m = m + 1
 
     return res * dt/T
 
 
 def vectortodm(rhovec):
+    """
+    (...)
+    """
     dim = round(np.sqrt(rhovec.shape[0]))
     return qt.vector_to_operator(qt.Qobj(rhovec, dims = [[[dim], [dim]], [1]]))
 
 
 def dmtovector(rho):
     """
     Transforms a Qobj density matrix object into a Qobj vector
@@ -165,14 +188,17 @@
     dim = rho.dims[0][0]
     #return qt.Qobj(qt.operator_to_vector(rho), dims = [[4], [1]])
     return qt.Qobj(qt.operator_to_vector(rho), dims = [[dim**2], [1]])
 
 
 #def fourier_steady_state2(T, ntsteps, L0, LVlist, nu = None, dgt = None):
 def fourier_steady_state2(T, ntsteps, L, f, nu = None, dgt = None):
+    """
+    (...)
+    """
     compute_gradient = False
     if nu is not None:
         compute_gradient = True
 
     L0 = L.H0.full()
     LVlist = []
     for k in range(len(L.V)):
```

### Comparing `qocttools-0.0.7/qocttools/hamiltonians.py` & `qocttools-0.0.8/qocttools/hamiltonians.py`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/krotov.py` & `qocttools-0.0.8/qocttools/krotov.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     f_initial:
         pulse class defined in typical_pulse.py, specifically 'Realtime' parametrization
     psi0:
         initial state.
     time:
         array that contain each time step.
     O:
-        Target operator that we want to optimice <ψ(T)|O|ψ(T)>
+        Target operator that we want to optimize :math:`\\langle\\Psi(T)\\vert O\\vert\\Psi(T)\\rangle`
     S:
         Penalty function
     tolerance:
         Precision for the algorithm
     alpha:
         Penalty factor
```

### Comparing `qocttools-0.0.7/qocttools/math_extra.py` & `qocttools-0.0.8/qocttools/math_extra.py`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/models/GdW30.py` & `qocttools-0.0.8/qocttools/models/GdW30.py`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/models/graphene.py` & `qocttools-0.0.8/qocttools/models/graphene.py`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/models/hBN.py` & `qocttools-0.0.8/qocttools/models/hBN.py`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/models/tmd.py` & `qocttools-0.0.8/qocttools/models/tmd.py`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/pulses.py` & `qocttools-0.0.8/qocttools/pulses.py`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/qoct.py` & `qocttools-0.0.8/qocttools/qoct.py`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/sampleruns/dissipation/GdW30_Toffoli_Syvstime_15dB.dat` & `qocttools-0.0.8/qocttools/sampleruns/dissipation/GdW30_Toffoli_Syvstime_15dB.dat`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/sampleruns/dissipation/dissipation.ipynb` & `qocttools-0.0.8/qocttools/sampleruns/dissipation/dissipation.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970238095238095%*

 * *Differences: {"'metadata'": "{'language_info': {delete: ['version']}}"}*

```diff
@@ -460,16 +460,15 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.7.3"
+            "pygments_lexer": "ipython3"
         },
         "latex_metadata": {
             "affiliation": " ",
             "author": " ",
             "title": "pi-pulses for state-to-state transitions on the GdW30 model"
         }
     },
```

### Comparing `qocttools-0.0.7/qocttools/sampleruns/gradient/V` & `qocttools-0.0.8/qocttools/sampleruns/gradient/V`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/sampleruns/gradient/gradient.ipynb` & `qocttools-0.0.8/qocttools/sampleruns/gradient/gradient.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944655837163241%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(15, 'import qutip as qt')], delete: [15]}}, 13: {'source': "*

 * *            '{insert: [(6, \'V = qt.Qobj(qt.fileio.file_data_read("V"))\')], delete: [6]}}, 28: '*

 * *            "{'source': {insert: [(2, 'def Pfunction(u):\\n'), (3, '    return - lambda_ * "*

 * *            "sp.integrate.simps(f.fu(time) * f.fu(time), time)\\n'), (4, '\\n'), (5, 'def dPdu(u, "*

 * *            "m):\\n'), (8, 'def Fyu(y, u):\\n'), (9, '    return qt.expect(qt.fock_dm(dim, "*

 * *            "target_level),  […]*

```diff
@@ -24,15 +24,15 @@
                 "import numpy as np\n",
                 "import scipy as sp\n",
                 "import matplotlib\n",
                 "if not isnotebook:\n",
                 "    matplotlib.use('Agg')\n",
                 "import matplotlib.pyplot as plt\n",
                 "import time\n",
-                "from qutip import *"
+                "import qutip as qt"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -171,15 +171,15 @@
             "source": [
                 "# In principle, we could just transform V with the recently obtained eigenstates. Unfortunately, that\n",
                 "# would make the test results different in different computers, as the eigenstates can have different phases.\n",
                 "# Therefore, we use the V that was computed once, and stored in file \"V\". The commented code was used\n",
                 "# to generate and store V.\n",
                 "#V = V.transform(eigenstates)\n",
                 "#fileio.file_data_store(\"V\", V, numformat = 'exp')\n",
-                "V = Qobj(fileio.file_data_read(\"V\"))"
+                "V = qt.Qobj(qt.fileio.file_data_read(\"V\"))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -375,37 +375,46 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "lambda_ = 0.1 / sp.integrate.simps(f.fu(time)*f.fu(time), time)\n",
                 "\n",
-                "def dFdu(u, m):\n",
+                "def Pfunction(u):\n",
+                "    return - lambda_ * sp.integrate.simps(f.fu(time) * f.fu(time), time)\n",
+                "\n",
+                "def dPdu(u, m):\n",
                 "    return - 2.0 * lambda_ * sp.integrate.simps(f.dfu(time, m) * f.fu(time), time)\n",
                 "\n",
-                "def Pfunction(u):\n",
-                "    return - lambda_ * sp.integrate.simps(f.fu(time) * f.fu(time), time)"
+                "def Fyu(y, u):\n",
+                "    return qt.expect(qt.fock_dm(dim, target_level), y) + Pfunction(u)\n",
+                "\n",
+                "def dFdy(y, u):\n",
+                "    return qt.fock_dm(dim, target_level) * y\n",
+                "\n",
+                "def dFdu(u, m):\n",
+                "    return dPdu(u, m)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "tg = target.Target('expectationvalue', operator = fock_dm(dim, target_level), dFdu = dFdu, Pu = Pfunction)"
+                "tg = target.Target('generic', Fyu = Fyu, dFdy = dFdy, dFdu = dFdu)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "state_0 = basis(dim, 0) #initial state"
+                "state_0 = qt.basis(dim, 0) #initial state"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Comparison, Schr\u00f6dinger picture"
@@ -553,24 +562,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "state_0 = basis(dim, 0) #initial state"
+                "state_0 = qt.basis(dim, 0) #initial state"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "tg = target.Target('expectationvalue', operator = fock_dm(dim, target_level))"
+                "tg = target.Target('expectationvalue', operator = qt.fock_dm(dim, target_level))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -655,19 +664,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "U_target = Qobj(qip.operations.toffoli().data)\n",
+                "U_target = qt.Qobj(qt.qip.operations.toffoli().data)\n",
                 "U_target_int = (1j*T*H0).expm() * \\\n",
-                "               Qobj(qip.operations.toffoli().data)\n",
+                "               qt.Qobj(qt.qip.operations.toffoli().data)\n",
                 "\n",
-                "U_0 = qeye(dim) #initial state"
+                "U_0 = qt.qeye(dim) #initial state"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Comparison, Schr\u00f6dinger picture"
@@ -792,14 +801,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `qocttools-0.0.7/qocttools/sampleruns/gradient-dissipation/V` & `qocttools-0.0.8/qocttools/sampleruns/gradient-dissipation/V`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/sampleruns/gradient-dissipation/gradient-dissipation.ipynb` & `qocttools-0.0.8/qocttools/sampleruns/gradient-dissipation/gradient-dissipation.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'metadata'": "{'language_info': {delete: ['version']}}"}*

```diff
@@ -974,14 +974,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.7.3"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `qocttools-0.0.7/qocttools/sampleruns/gradient-dissipation-multitarget/gradient-dissipation-multitarget.ipynb` & `qocttools-0.0.8/qocttools/sampleruns/gradient-dissipation-multitarget/gradient-dissipation-multitarget.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9865283613445378%*

 * *Differences: {"'cells'": '{29: {\'source\': {insert: [(0, "tg = target.Target(\'expectationvalue\', operator = '*

 * *            'rho_target)\\n")], delete: [0]}}, delete: [28]}',*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3 (ipykernel)'}, 'language_info': {delete: "*

 * *               "['version']}}"}*

```diff
@@ -369,39 +369,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "lambda_ = 0.1 / sp.integrate.simps(f.fu(time)*f.fu(time), time)\n",
-                "\n",
-                "def Pfunction(u): # Penalty\n",
-                "    return - lambda_ * sp.integrate.simps(f.fu(time, u) * f.fu(time, u), time)\n",
-                "\n",
-                "def dFdu(u, m):\n",
-                "    return - 2.0 * lambda_ * sp.integrate.simps(f.dfu(time, m) * f.fu(time), time)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "H = hamiltonians.hamiltonian(H0, [V], [A])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "tg = target.Target('expectationvalue', operator = rho_target, Pu = Pfunction, dFdu = dFdu)\n",
+                "tg = target.Target('expectationvalue', operator = rho_target)\n",
                 "\n",
                 "opt = qoct.Qoct(H, T, time.shape[0], tg, f, rho_ini,\n",
                 "                interaction_picture = True,\n",
                 "                solve_method = 'cfmagnus4')"
             ]
         },
         {
@@ -433,27 +418,26 @@
                 "    for i in data:\n",
                 "        f.write(\"{:.14e}\\n\".format(i))"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.7.3"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `qocttools-0.0.7/qocttools/sampleruns/model/model.ipynb` & `qocttools-0.0.8/qocttools/sampleruns/model/model.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'metadata'": "{'language_info': {delete: ['version']}}"}*

```diff
@@ -182,14 +182,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.7.3"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `qocttools-0.0.7/qocttools/sampleruns/pipulse/pipulse.ipynb` & `qocttools-0.0.8/qocttools/sampleruns/pipulse/pipulse.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970238095238095%*

 * *Differences: {"'metadata'": "{'language_info': {delete: ['version']}}"}*

```diff
@@ -567,16 +567,15 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.7.3"
+            "pygments_lexer": "ipython3"
         },
         "latex_metadata": {
             "affiliation": " ",
             "author": " ",
             "title": "pi-pulses for state-to-state transitions on the GdW30 model"
         }
     },
```

### Comparing `qocttools-0.0.7/qocttools/sampleruns/propagators/.ipynb_checkpoints/generic_propagation-checkpoint.ipynb` & `qocttools-0.0.8/qocttools/sampleruns/propagators/.ipynb_checkpoints/generic_propagation-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/sampleruns/propagators/propagators.ipynb` & `qocttools-0.0.8/qocttools/sampleruns/propagators/propagators.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'metadata'": "{'language_info': {delete: ['version']}}"}*

```diff
@@ -892,14 +892,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.9.2"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `qocttools-0.0.7/qocttools/sampleruns/qoctbasic/V` & `qocttools-0.0.8/qocttools/sampleruns/qoctbasic/V`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/sampleruns/qoctbasic/qoctbasic.ipynb` & `qocttools-0.0.8/qocttools/sampleruns/qoctbasic/qoctbasic.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9896552613293379%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(15, 'import qutip as qt')], delete: [15]}}, 13: {'source': "*

 * *            '{insert: [(6, \'V = qt.Qobj(qt.fileio.file_data_read("V"))\')], delete: [6]}}, 26: '*

 * *            "{'source': {insert: [(10, 'def Fyu(y, u):\\n'), (11, '    return "*

 * *            "qt.expect(qt.fock_dm(dim, target_level), y) + Pfunction(u)\\n'), (12, '\\n'), (13, "*

 * *            "'def dFdy(y, u):\\n'), (14, '    return qt.fock_dm(dim, target_level) * y\\n'), (15, "*

 * *            "'\\n'), (16, 'state_0 = […]*

```diff
@@ -24,15 +24,15 @@
                 "import numpy as np\n",
                 "import scipy as sp\n",
                 "import matplotlib\n",
                 "if not isnotebook:\n",
                 "    matplotlib.use('Agg')\n",
                 "import matplotlib.pyplot as plt\n",
                 "import nlopt\n",
-                "from qutip import *"
+                "import qutip as qt"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -168,15 +168,15 @@
             "source": [
                 "# In principle, we could just transform V with the recently obtained eigenstates. Unfortunately, that\n",
                 "# would make the test results different in different computers, as the eigenstates can have different phases.\n",
                 "# Therefore, we use the V that was computed once, and stored in file \"V\". The commented code was used\n",
                 "# to generate and store V.\n",
                 "#V = V.transform(eigenstates)\n",
                 "#fileio.file_data_store(\"V\", V, numformat = 'exp')\n",
-                "V = Qobj(fileio.file_data_read(\"V\"))"
+                "V = qt.Qobj(qt.fileio.file_data_read(\"V\"))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -355,24 +355,31 @@
                 "\n",
                 "def Pfunction(u):\n",
                 "    return - lambda_ * sp.integrate.simps(f.fu(time, u) * f.fu(time, u), time)\n",
                 "\n",
                 "def dFdu(u, m):\n",
                 "    return - 2.0 * lambda_ * sp.integrate.simps(f.dfu(time, m, u) * f.fu(time, u), time)\n",
                 "\n",
-                "state_0 = basis(dim, 0)"
+                "def Fyu(y, u):\n",
+                "    return qt.expect(qt.fock_dm(dim, target_level), y) + Pfunction(u)\n",
+                "\n",
+                "def dFdy(y, u):\n",
+                "    return qt.fock_dm(dim, target_level) * y\n",
+                "\n",
+                "state_0 = qt.basis(dim, 0)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "tg = target.Target('expectationvalue', dFdu = dFdu, operator = fock_dm(dim, target_level), Pu = Pfunction)\n",
+                "#tg = target.Target('expectationvalue', dFdu = dFdu, operator = fock_dm(dim, target_level), Pu = Pfunction)\n",
+                "tg = target.Target('generic', Fyu = Fyu, dFdy = dFdy, dFdu = dFdu)\n",
                 "\n",
                 "opt = qoct.Qoct(H, T, time.shape[0], tg, f, state_0,\n",
                 "                interaction_picture = True)"
             ]
         },
         {
             "cell_type": "code",
@@ -471,16 +478,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "U_target = Qobj(qip.operations.toffoli().data)\n",
-                "U_0 = qeye(dim) #initial state"
+                "U_target = qt.Qobj(qt.qip.operations.toffoli().data)\n",
+                "U_0 = qt.qeye(dim) #initial state"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We will ask each frequency component not to be larger than 30 mT."
@@ -544,27 +551,26 @@
                 "    for i in data:\n",
                 "        f.write(\"{:.14e}\\n\".format(i))"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.7.3"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `qocttools-0.0.7/qocttools/sampleruns/qoctbasic-krotov/V` & `qocttools-0.0.8/qocttools/sampleruns/qoctbasic-krotov/V`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/sampleruns/qoctbasic-krotov/qoctbasic-krotov.ipynb` & `qocttools-0.0.8/qocttools/sampleruns/qoctbasic-krotov/qoctbasic-krotov.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9900370209059234%*

 * *Differences: {"'cells'": "{28: {'source': {insert: [(1, '                   operator = fock_dm(dim, "*

 * *            "target_level), S = S, alpha = alpha)')], delete: [1]}}, 38: {'source': {insert: [(1, "*

 * *            "'                   S = S, alpha = 0.1 * alpha)\\n')], delete: [1]}}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3 (ipykernel)'}, 'language_info': {delete: "*

 * *               "['version']}}"}*

```diff
@@ -360,15 +360,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "tg = target.Target('expectationvalue',\n",
-                "                   operator = fock_dm(dim, target_level), Pu = Pfunction, S = S, alpha = alpha)"
+                "                   operator = fock_dm(dim, target_level), S = S, alpha = alpha)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -467,15 +467,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "tg = target.Target('evolutionoperator', operator = U_target, Utarget = U_target, \n",
-                "                   Pu = Pfunction, S = S, alpha = 0.1 * alpha)\n",
+                "                   S = S, alpha = 0.1 * alpha)\n",
                 "\n",
                 "opt = qoct.Qoct(H, T, time.shape[0], tg, ft, U_0,\n",
                 "                interaction_picture = True,\n",
                 "                solve_method = 'rk4')"
             ]
         },
         {
@@ -498,27 +498,26 @@
                 "     for i in data:\n",
                 "         datafile.write(\"{:.14e}\\n\".format(i))"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.7.3"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `qocttools-0.0.7/qocttools/sampleruns/qocttoffoli/V` & `qocttools-0.0.8/qocttools/sampleruns/qocttoffoli/V`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/sampleruns/qocttoffoli/optimal-pulse.csv` & `qocttools-0.0.8/qocttools/sampleruns/qocttoffoli/optimal-pulse.csv`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/sampleruns/qocttoffoli/qocttoffoli.ipynb` & `qocttools-0.0.8/qocttools/sampleruns/qocttoffoli/qocttoffoli.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'metadata'": "{'language_info': {delete: ['version']}}"}*

```diff
@@ -706,14 +706,13 @@
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.7.3"
+            "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `qocttools-0.0.7/qocttools/solvers.py` & `qocttools-0.0.8/qocttools/solvers.py`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/target.py` & `qocttools-0.0.8/qocttools/target.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,38 +11,108 @@
 ## but WITHOUT ANY WARRANTY; without even the implied warranty of
 ## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ## GNU General Public License for more details.
 ##
 ## You should have received a copy of the GNU General Public License
 ## along with qocttools.  If not, see <https://www.gnu.org/licenses/>.
 
+"""This module contains the Target class, and associated procedures.
+
+"""
+
+
 import numpy as np
 import qocttools.math_extra as math_extra
 import qocttools.floquet as floquet
 import qutip as qt
 
-"""This module contains the Target class, and associated procedures.
-
-"""
 
 class Target:
     """The class that holds the definition of the target
 
-    ...
-
     Parameters
     ----------
     targettype: string
-        The code admits the following types of characters: ...
+        The code admits the following types of characters:
+
+        1. generic
+
+           The user may input any function as target, defined by
+           the driver program, using the `Fyu` parameter (see below).
+
+        2. expectationvalue
+
+           The target is the expectation value of some operator:
+
+           .. math::
+
+              F(y, u) = \\langle \\Psi(T)\\vert O \\vert \\Psi(T)\\rangle
+
+           or, if the multitarget option is used,
+
+           .. math::
+
+              F(y, u) = \\frac{1}{Q} \\sum_i \\langle \\Psi_i(T)\\vert O_i \\vert \\Psi_i(T)\\rangle
+
+           Here, :math:`Q` is the number of targets. The operator(s) should be provided 
+           using the `operator` argument (below).
+
+        3. evolutionoperator
+
+           The goal now is to find a set of control parameters that leads to an evolution of
+           the system characterized by a fixed target evolution operator. This target evolution
+           operator (or operators, if a multitarget setup is used), is provided by the argument
+           `Utarget`. The target definition is:
+
+           .. math::
+
+              F(U, u) = \\frac{1}{Q} \\sum_i \\vert U(T) \\cdot U^{(i)}_{\\rm target} \\vert^2
+
+        4. floquet
+
+    Fyu: function
+
+        If `targettype == "generic"`, the user should pass the function used to 
+        define the target. The interface should be:
+
+        .. code-block:: python
+
+           def Fyu(y: qutip.Qobj or list of qutip.Qobj, u: ndarray) -> float:
+
+        The function `Fyu` should receive as argument a system state (be it a Hilbert
+        state, evolution operator, or density matrix), that is supposed to be the state
+        at the end of the propagation, and a control parameters set. It should output
+        the target functional value. It may also take as argument a list of states, if
+        one is running the optimizaion in *multitarget* mode.
+
+    dFdy: function
+
+        If `targettype == "generic"`, the user should pass the function used to 
+        define the target (`Fyu`), **and** the derivative of that function with respect to
+        the state, which would be given by this `dFdy` parameter. The interface should be:
+
+        .. code-block:: python
+
+           def dFdy(y: qutip.Qobj or list of qutip.Qobj, u: ndarray) -> list of float:
+
+    dFdu: function
+
+        If `targettype == "generic"`, the user should pass the function used to 
+        define the target (`Fyu`), **and, if it is not zero**, the derivative of that function with respect to
+        the control parameters, which would be given by this `dFdu` parameter. The interface should be:
+
+        .. code-block:: python
+
+           def dFdu(u: ndarray, m: int) -> float:
+
     """
     def __init__(self, targettype, 
                  Fyu = None,
                  dFdy = None,
                  dFdu = None,
-                 Pu = None,
                  operator = None,
                  Utarget = None,
                  alpha = None,
                  S = None,
                  targeteps = None,
                  T = None,
                  fepsilon = None,
@@ -51,25 +121,23 @@
         if targettype == 'generic':
             self.Fyu_ = Fyu
             self.dFdy_ = dFdy
             self.operator = operator
             self.S = S
             self.alpha = alpha
         elif targettype == 'expectationvalue':
-            self.Pu = Pu
             if isinstance(operator, list):
                 self.operator = []
                 for i in range(len(operator)):
                     self.operator.append(operator[i].copy())
             else:
                 self.operator = [operator.copy()]
             self.alpha = alpha
             self.S = S
         elif targettype == 'evolutionoperator':
-            self.Pu = Pu
             if isinstance(Utarget, list):
                 self.Utarget = []
                 for i in range(len(Utarget)):
                     self.Utarget.append(Utarget[i].copy())
             else:
                 self.Utarget = [Utarget.copy()]
             self.operator = operator
@@ -127,18 +195,15 @@
                 ntgs = len(y)
                 x = 0.0
                 for j in range(len(y)):
                     x = x + qt.expect(self.operator[j], y[j])
             else:
                 ntgs = 1
                 x = qt.expect(self.operator[0], y)
-            x = x / ntgs
-            if self.Pu is not None:
-                x = x + self.Pu(u)
-            return x
+            return x / ntgs
 
         elif self.targettype == 'evolutionoperator':
             if isinstance(y, list):
                 ntgs = len(y)
                 x = 0.0
                 for j in range(ntgs):
                     dim = y[j].shape[0]
```

### Comparing `qocttools-0.0.7/qocttools/tests/long.py` & `qocttools-0.0.8/qocttools/tests/long.py`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools/tests/short.py` & `qocttools-0.0.8/qocttools/tests/short.py`

 * *Files identical despite different names*

### Comparing `qocttools-0.0.7/qocttools.egg-info/PKG-INFO` & `qocttools-0.0.8/qocttools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qocttools
-Version: 0.0.7
+Version: 0.0.8
 Summary: A set of tools to do quantum optimal control calculations
 Author-email: Alberto Castro <alberto.castro.barrigon@gmail.com>
 Project-URL: Homepage, https://qocttools.readthedocs.io/
 Project-URL: Bug Tracker, https://gitlab.com/acbarrigon/qocttools/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `qocttools-0.0.7/qocttools.egg-info/SOURCES.txt` & `qocttools-0.0.8/qocttools.egg-info/SOURCES.txt`

 * *Files identical despite different names*


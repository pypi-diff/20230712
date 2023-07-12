# Comparing `tmp/calcos-3.4.6.tar.gz` & `tmp/calcos-3.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcos-3.4.6.tar", last modified: Wed Jun 28 13:55:19 2023, max compression
+gzip compressed data, was "calcos-3.4.7.tar", last modified: Wed Jul 12 14:02:20 2023, max compression
```

## Comparing `calcos-3.4.6.tar` & `calcos-3.4.7.tar`

### file list

```diff
@@ -1,85 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:55:19.637626 calcos-3.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-28 13:55:07.000000 calcos-3.4.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:55:19.629626 calcos-3.4.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-28 13:55:07.000000 calcos-3.4.6/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:55:19.629626 calcos-3.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-28 13:55:07.000000 calcos-3.4.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-28 13:55:07.000000 calcos-3.4.6/.github/workflows/python_testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-28 13:55:07.000000 calcos-3.4.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-28 13:55:07.000000 calcos-3.4.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-28 13:55:07.000000 calcos-3.4.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-28 13:55:07.000000 calcos-3.4.6/Jenkinsfile
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-28 13:55:07.000000 calcos-3.4.6/JenkinsfileRT
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-28 13:55:19.637626 calcos-3.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-28 13:55:07.000000 calcos-3.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:55:19.633626 calcos-3.4.6/calcos/
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25421 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/accum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/airglow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/average.py
--rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/burst.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/calcos.help
--rwxr-xr-x   0 runner    (1001) docker     (123)   139904 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/calcos.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/calcosparam.py
--rw-r--r--   0 runner    (1001) docker     (123)    82085 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/concurrent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   128867 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/cosutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (123)   115243 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    35355 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/findshift1.py
--rw-r--r--   0 runner    (1001) docker     (123)    49417 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/fpavg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13126 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/getinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/orbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/osmstep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:55:19.633626 calcos-3.4.6/calcos/pars/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/pars/calcos.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/pars/calcos.cfgspc
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/phot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/shiftfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/splittag.py
--rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/spwcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25999 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)   187336 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/timetag.py
--rw-r--r--   0 runner    (1001) docker     (123)    27796 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-28 13:55:19.000000 calcos-3.4.6/calcos/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    37980 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/wavecal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21305 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/x1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-06-28 13:55:07.000000 calcos-3.4.6/calcos/xd_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:55:19.633626 calcos-3.4.6/calcos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-28 13:55:19.000000 calcos-3.4.6/calcos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-28 13:55:19.000000 calcos-3.4.6/calcos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 13:55:19.000000 calcos-3.4.6/calcos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-28 13:55:19.000000 calcos-3.4.6/calcos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-28 13:55:19.000000 calcos-3.4.6/calcos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-28 13:55:19.000000 calcos-3.4.6/calcos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:55:19.633626 calcos-3.4.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-28 13:55:07.000000 calcos-3.4.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-28 13:55:07.000000 calcos-3.4.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-28 13:55:07.000000 calcos-3.4.6/docs/rtd_environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:55:19.633626 calcos-3.4.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-06-28 13:55:07.000000 calcos-3.4.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-28 13:55:07.000000 calcos-3.4.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-28 13:55:07.000000 calcos-3.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 13:55:19.637626 calcos-3.4.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      943 2023-06-28 13:55:07.000000 calcos-3.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:55:19.633626 calcos-3.4.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)   129422 2023-06-28 13:55:07.000000 calcos-3.4.6/src/ccos.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:55:19.637626 calcos-3.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/generate_tempfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_airglow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_average.py
--rw-r--r--   0 runner    (1001) docker     (123)    36822 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_cosutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_dark_fuva.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_dark_fuvb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_dark_nuv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_flat_fuva.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_flat_nuv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_flat_relmvreq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_fuv_timetag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_shiftfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_wavecal_fuva_f140l.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-28 13:55:07.000000 calcos-3.4.6/tests/test_wavecal_fuva_g130m.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-28 13:55:07.000000 calcos-3.4.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:02:20.546002 calcos-3.4.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:02:20.522000 calcos-3.4.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 14:02:02.000000 calcos-3.4.7/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:02:20.522000 calcos-3.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-12 14:02:02.000000 calcos-3.4.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-12 14:02:02.000000 calcos-3.4.7/.github/workflows/python_testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-12 14:02:02.000000 calcos-3.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-12 14:02:02.000000 calcos-3.4.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-12 14:02:02.000000 calcos-3.4.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-12 14:02:02.000000 calcos-3.4.7/Jenkinsfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-12 14:02:02.000000 calcos-3.4.7/JenkinsfileRT
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-12 14:02:20.546002 calcos-3.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-12 14:02:02.000000 calcos-3.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:02:20.534001 calcos-3.4.7/calcos/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25421 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/accum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/airglow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/average.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/burst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/calcos.help
+-rwxr-xr-x   0 runner    (1001) docker     (123)   139904 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/calcos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/calcosparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82085 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/concurrent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   128867 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/cosutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115243 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35355 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/findshift1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49417 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/fpavg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13126 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/getinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/osmstep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:02:20.538001 calcos-3.4.7/calcos/pars/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/pars/calcos.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/pars/calcos.cfgspc
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/phot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/shiftfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/splittag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/spwcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25999 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187336 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/timetag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27796 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-12 14:02:20.000000 calcos-3.4.7/calcos/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37980 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/wavecal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21305 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/x1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-12 14:02:02.000000 calcos-3.4.7/calcos/xd_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:02:20.534001 calcos-3.4.7/calcos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-12 14:02:20.000000 calcos-3.4.7/calcos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-12 14:02:20.000000 calcos-3.4.7/calcos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:02:20.000000 calcos-3.4.7/calcos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-12 14:02:20.000000 calcos-3.4.7/calcos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-12 14:02:20.000000 calcos-3.4.7/calcos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 14:02:20.000000 calcos-3.4.7/calcos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:02:20.538001 calcos-3.4.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-12 14:02:02.000000 calcos-3.4.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-12 14:02:02.000000 calcos-3.4.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 14:02:02.000000 calcos-3.4.7/docs/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:02:20.538001 calcos-3.4.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-12 14:02:02.000000 calcos-3.4.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-12 14:02:02.000000 calcos-3.4.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-12 14:02:02.000000 calcos-3.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-12 14:02:20.546002 calcos-3.4.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2273 2023-07-12 14:02:02.000000 calcos-3.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:02:20.538001 calcos-3.4.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)   129422 2023-07-12 14:02:02.000000 calcos-3.4.7/src/ccos.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:02:20.546002 calcos-3.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/generate_tempfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_airglow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36822 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_cosutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_dark_fuva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_dark_fuvb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_dark_nuv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_flat_fuva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_flat_nuv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_flat_relmvreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_fuv_timetag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_shiftfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_wavecal_fuva_f140l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-12 14:02:02.000000 calcos-3.4.7/tests/test_wavecal_fuva_g130m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-12 14:02:02.000000 calcos-3.4.7/tox.ini
```

### Comparing `calcos-3.4.6/.github/workflows/publish-to-pypi.yml` & `calcos-3.4.7/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/.github/workflows/python_testing.yml` & `calcos-3.4.7/.github/workflows/python_testing.yml`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/.readthedocs.yml` & `calcos-3.4.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/CODE_OF_CONDUCT.md` & `calcos-3.4.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/Jenkinsfile` & `calcos-3.4.7/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/JenkinsfileRT` & `calcos-3.4.7/JenkinsfileRT`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/PKG-INFO` & `calcos-3.4.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 Metadata-Version: 2.1
 Name: calcos
-Version: 3.4.6
+Version: 3.4.7
 Summary: Calibration software for COS (Cosmic Origins Spectrograph)
+Home-page: https://github.com/spacetelescope/calcos
 Author: Phil Hodge, Robert Jedrzejewski
+Author-email: help@stsci.edu
+License: BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: test
 
-# CALCOS
-
-[![Jenkins CI](https://ssbjenkins.stsci.edu/job/STScI/job/calcos/job/master/badge/icon)](https://ssbjenkins.stsci.edu/job/STScI/job/calcos/job/master/)
-
-Calibration software for HST/COS.
-
-Nightly regression test results are available only from within the STScI
-network at this time.
-https://plwishmaster.stsci.edu:8081/job/RT/job/calcos/test_results_analyzer/
+README.md
```

### Comparing `calcos-3.4.6/calcos/__init__.py` & `calcos-3.4.7/calcos/__init__.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/accum.py` & `calcos-3.4.7/calcos/accum.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/airglow.py` & `calcos-3.4.7/calcos/airglow.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/average.py` & `calcos-3.4.7/calcos/average.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/burst.py` & `calcos-3.4.7/calcos/burst.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/calcos.help` & `calcos-3.4.7/calcos/calcos.help`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/calcos.py` & `calcos-3.4.7/calcos/calcos.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/calcosparam.py` & `calcos-3.4.7/calcos/calcosparam.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/concurrent.py` & `calcos-3.4.7/calcos/concurrent.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/cosutil.py` & `calcos-3.4.7/calcos/cosutil.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/dispersion.py` & `calcos-3.4.7/calcos/dispersion.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/extract.py` & `calcos-3.4.7/calcos/extract.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/findshift1.py` & `calcos-3.4.7/calcos/findshift1.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/fpavg.py` & `calcos-3.4.7/calcos/fpavg.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/getinfo.py` & `calcos-3.4.7/calcos/getinfo.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/orbit.py` & `calcos-3.4.7/calcos/orbit.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/osmstep.py` & `calcos-3.4.7/calcos/osmstep.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/pars/calcos.cfgspc` & `calcos-3.4.7/calcos/pars/calcos.cfgspc`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/phot.py` & `calcos-3.4.7/calcos/phot.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/shiftfile.py` & `calcos-3.4.7/calcos/shiftfile.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/splittag.py` & `calcos-3.4.7/calcos/splittag.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/spwcs.py` & `calcos-3.4.7/calcos/spwcs.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/timeline.py` & `calcos-3.4.7/calcos/timeline.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/timetag.py` & `calcos-3.4.7/calcos/timetag.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/trace.py` & `calcos-3.4.7/calcos/trace.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/wavecal.py` & `calcos-3.4.7/calcos/wavecal.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/x1d.py` & `calcos-3.4.7/calcos/x1d.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos/xd_search.py` & `calcos-3.4.7/calcos/xd_search.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/calcos.egg-info/PKG-INFO` & `calcos-3.4.7/calcos.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 Metadata-Version: 2.1
 Name: calcos
-Version: 3.4.6
+Version: 3.4.7
 Summary: Calibration software for COS (Cosmic Origins Spectrograph)
+Home-page: https://github.com/spacetelescope/calcos
 Author: Phil Hodge, Robert Jedrzejewski
+Author-email: help@stsci.edu
+License: BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: test
 
-# CALCOS
-
-[![Jenkins CI](https://ssbjenkins.stsci.edu/job/STScI/job/calcos/job/master/badge/icon)](https://ssbjenkins.stsci.edu/job/STScI/job/calcos/job/master/)
-
-Calibration software for HST/COS.
-
-Nightly regression test results are available only from within the STScI
-network at this time.
-https://plwishmaster.stsci.edu:8081/job/RT/job/calcos/test_results_analyzer/
+README.md
```

### Comparing `calcos-3.4.6/calcos.egg-info/SOURCES.txt` & `calcos-3.4.7/calcos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-.flake8
 .gitignore
 .readthedocs.yml
 CODE_OF_CONDUCT.md
 Jenkinsfile
 JenkinsfileRT
 README.md
 pyproject.toml
+setup.cfg
 setup.py
 tox.ini
 .github/CODEOWNERS
 .github/workflows/publish-to-pypi.yml
 .github/workflows/python_testing.yml
 calcos/__init__.py
 calcos/accum.py
```

### Comparing `calcos-3.4.6/docs/Makefile` & `calcos-3.4.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/docs/make.bat` & `calcos-3.4.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/docs/source/conf.py` & `calcos-3.4.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/src/ccos.c` & `calcos-3.4.7/src/ccos.c`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/README.md` & `calcos-3.4.7/tests/README.md`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/conftest.py` & `calcos-3.4.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/generate_tempfiles.py` & `calcos-3.4.7/tests/generate_tempfiles.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/helpers.py` & `calcos-3.4.7/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_airglow.py` & `calcos-3.4.7/tests/test_airglow.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_average.py` & `calcos-3.4.7/tests/test_average.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_cosutil.py` & `calcos-3.4.7/tests/test_cosutil.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_dark_fuva.py` & `calcos-3.4.7/tests/test_dark_fuva.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_dark_fuvb.py` & `calcos-3.4.7/tests/test_dark_fuvb.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_dark_nuv.py` & `calcos-3.4.7/tests/test_dark_nuv.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_extract.py` & `calcos-3.4.7/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_flat_fuva.py` & `calcos-3.4.7/tests/test_flat_fuva.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_flat_nuv.py` & `calcos-3.4.7/tests/test_flat_nuv.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_flat_relmvreq.py` & `calcos-3.4.7/tests/test_flat_relmvreq.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_fuv_timetag.py` & `calcos-3.4.7/tests/test_fuv_timetag.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_shiftfile.py` & `calcos-3.4.7/tests/test_shiftfile.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_wavecal_fuva_f140l.py` & `calcos-3.4.7/tests/test_wavecal_fuva_f140l.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tests/test_wavecal_fuva_g130m.py` & `calcos-3.4.7/tests/test_wavecal_fuva_g130m.py`

 * *Files identical despite different names*

### Comparing `calcos-3.4.6/tox.ini` & `calcos-3.4.7/tox.ini`

 * *Files identical despite different names*


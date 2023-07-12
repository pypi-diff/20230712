# Comparing `tmp/mcmc_statphys-0.4.3.tar.gz` & `tmp/mcmc_statphys-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcmc_statphys-0.4.3.tar", last modified: Sun May 21 09:27:48 2023, max compression
+gzip compressed data, was "mcmc_statphys-1.0.0.tar", last modified: Wed Jul 12 12:53:02 2023, max compression
```

## Comparing `mcmc_statphys-0.4.3.tar` & `mcmc_statphys-1.0.0.tar`

### file list

```diff
@@ -1,50 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.245245 mcmc_statphys-0.4.3/
--rw-rw-rw-   0        0        0      170 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/AUTHORS.rst
--rw-rw-rw-   0        0        0     3726 2023-05-18 15:41:51.000000 mcmc_statphys-0.4.3/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1592 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4623 2023-05-21 09:27:48.245245 mcmc_statphys-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     2193 2023-05-18 15:41:51.000000 mcmc_statphys-0.4.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.150984 mcmc_statphys-0.4.3/docs/
--rw-rw-rw-   0        0        0      634 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/authors.rst
--rw-rw-rw-   0        0        0     4923 2023-05-21 09:26:39.000000 mcmc_statphys-0.4.3/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/history.rst
-drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.152979 mcmc_statphys-0.4.3/docs/img/
--rw-rw-rw-   0        0        0    12977 2023-05-17 14:16:19.000000 mcmc_statphys-0.4.3/docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png
--rw-rw-rw-   0        0        0      333 2023-05-16 16:00:10.000000 mcmc_statphys-0.4.3/docs/index.rst
--rw-rw-rw-   0        0        0     1209 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/installation.rst
--rwxrwxrwx   0        0        0      811 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/make.bat
--rw-rw-rw-   0        0        0    10277 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/docs/modules.rst
--rw-rw-rw-   0        0        0       28 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/docs/readme.rst
--rw-rw-rw-   0        0        0    17406 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.167939 mcmc_statphys-0.4.3/mcmc_statphys/
--rw-rw-rw-   0        0        0      247 2023-05-21 09:26:39.000000 mcmc_statphys-0.4.3/mcmc_statphys/__init__.py
--rw-rw-rw-   0        0        0    14689 2023-05-21 09:26:19.000000 mcmc_statphys-0.4.3/mcmc_statphys/algorithm.py
--rw-rw-rw-   0        0        0     2582 2023-05-20 10:32:21.000000 mcmc_statphys-0.4.3/mcmc_statphys/analysis.py
--rw-rw-rw-   0        0        0      434 2023-05-14 12:02:25.000000 mcmc_statphys-0.4.3/mcmc_statphys/cli.py
--rw-rw-rw-   0        0        0     5788 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/mcmc_statphys/draw.py
--rw-rw-rw-   0        0        0     8776 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/mcmc_statphys/model.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.211822 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/
--rw-rw-rw-   0        0        0     4623 2023-05-21 09:27:47.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      914 2023-05-21 09:27:48.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 09:27:47.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-21 09:27:47.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-14 13:46:13.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-05-21 09:27:47.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-21 09:27:47.000000 mcmc_statphys-0.4.3/mcmc_statphys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      520 2023-05-21 09:27:48.249237 mcmc_statphys-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1556 2023-05-21 09:26:39.000000 mcmc_statphys-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.228776 mcmc_statphys-0.4.3/tests/
--rw-rw-rw-   0        0        0       44 2023-05-14 13:37:58.000000 mcmc_statphys-0.4.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 09:27:48.243250 mcmc_statphys-0.4.3/tests/one/
--rw-rw-rw-   0        0        0      229 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/one/__init__.py
--rw-rw-rw-   0        0        0    14945 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/one/algorithm.py
--rw-rw-rw-   0        0        0     1406 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/one/analysis.py
--rw-rw-rw-   0        0        0      434 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/one/cli.py
--rw-rw-rw-   0        0        0     5788 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/one/draw.py
--rw-rw-rw-   0        0        0     8776 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/one/model.py
--rw-rw-rw-   0        0        0     2891 2023-05-21 04:30:43.000000 mcmc_statphys-0.4.3/tests/test.ipynb
--rw-rw-rw-   0        0        0      952 2023-05-18 15:41:51.000000 mcmc_statphys-0.4.3/tests/test_mcmc_statphys.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:53:02.946151 mcmc_statphys-1.0.0/
+-rw-rw-rw-   0        0        0      189 2023-07-12 12:44:59.000000 mcmc_statphys-1.0.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3598 2023-07-01 03:10:01.000000 mcmc_statphys-1.0.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1509 2023-07-01 03:10:01.000000 mcmc_statphys-1.0.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1067 2023-07-01 03:10:01.000000 mcmc_statphys-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      262 2023-07-01 03:10:01.000000 mcmc_statphys-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4647 2023-07-12 12:53:02.946151 mcmc_statphys-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2124 2023-07-12 12:44:59.000000 mcmc_statphys-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-12 12:53:02.849408 mcmc_statphys-1.0.0/docs/
+-rw-rw-rw-   0        0        0      614 2023-07-01 03:10:01.000000 mcmc_statphys-1.0.0/docs/Makefile
+-rw-rw-rw-   0        0        0       28 2023-07-01 03:10:01.000000 mcmc_statphys-1.0.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     4776 2023-07-12 12:44:59.000000 mcmc_statphys-1.0.0/docs/conf.py
+-rw-rw-rw-   0        0        0       33 2023-07-01 03:10:01.000000 mcmc_statphys-1.0.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       28 2023-07-01 03:10:01.000000 mcmc_statphys-1.0.0/docs/history.rst
+drwxrwxrwx   0        0        0        0 2023-07-12 12:53:02.862374 mcmc_statphys-1.0.0/docs/img/
+-rw-rw-rw-   0        0        0    12977 2023-05-17 14:16:19.000000 mcmc_statphys-1.0.0/docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png
+-rw-rw-rw-   0        0        0      313 2023-07-01 03:10:01.000000 mcmc_statphys-1.0.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1158 2023-07-01 03:10:02.000000 mcmc_statphys-1.0.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      775 2023-07-01 03:10:02.000000 mcmc_statphys-1.0.0/docs/make.bat
+-rw-rw-rw-   0        0        0     9618 2023-07-01 03:10:02.000000 mcmc_statphys-1.0.0/docs/modules.rst
+-rw-rw-rw-   0        0        0       27 2023-07-01 03:10:02.000000 mcmc_statphys-1.0.0/docs/readme.rst
+-rw-rw-rw-   0        0        0    16988 2023-07-01 03:10:02.000000 mcmc_statphys-1.0.0/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-07-12 12:53:02.874343 mcmc_statphys-1.0.0/mcmc_statphys/
+-rw-rw-rw-   0        0        0      313 2023-07-12 12:49:00.000000 mcmc_statphys-1.0.0/mcmc_statphys/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:53:02.899276 mcmc_statphys-1.0.0/mcmc_statphys/algorithm/
+-rw-rw-rw-   0        0        0     4648 2023-07-12 12:45:51.000000 mcmc_statphys-1.0.0/mcmc_statphys/algorithm/Anneal.py
+-rw-rw-rw-   0        0        0     3793 2023-07-12 12:45:51.000000 mcmc_statphys-1.0.0/mcmc_statphys/algorithm/Demon.py
+-rw-rw-rw-   0        0        0     3990 2023-07-12 12:45:51.000000 mcmc_statphys-1.0.0/mcmc_statphys/algorithm/HamiltonianMC.py
+-rw-rw-rw-   0        0        0     1931 2023-07-12 12:45:51.000000 mcmc_statphys-1.0.0/mcmc_statphys/algorithm/Kawasaki.py
+-rw-rw-rw-   0        0        0    19268 2023-07-12 12:45:51.000000 mcmc_statphys-1.0.0/mcmc_statphys/algorithm/Metropolis.py
+-rw-rw-rw-   0        0        0     4452 2023-07-12 12:45:52.000000 mcmc_statphys-1.0.0/mcmc_statphys/algorithm/Tempering.py
+-rw-rw-rw-   0        0        0     7633 2023-07-12 12:45:52.000000 mcmc_statphys-1.0.0/mcmc_statphys/algorithm/WangLandau.py
+-rw-rw-rw-   0        0        0     4901 2023-07-12 12:45:52.000000 mcmc_statphys-1.0.0/mcmc_statphys/algorithm/Wolff.py
+-rw-rw-rw-   0        0        0      324 2023-07-12 12:45:25.000000 mcmc_statphys-1.0.0/mcmc_statphys/algorithm/__init__.py
+-rw-rw-rw-   0        0        0      419 2023-07-01 03:10:02.000000 mcmc_statphys-1.0.0/mcmc_statphys/cli.py
+-rw-rw-rw-   0        0        0    11105 2023-07-12 12:49:19.000000 mcmc_statphys-1.0.0/mcmc_statphys/method.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:53:02.906257 mcmc_statphys-1.0.0/mcmc_statphys/model/
+-rw-rw-rw-   0        0        0     2307 2023-07-12 12:47:44.000000 mcmc_statphys-1.0.0/mcmc_statphys/model/Heisenberg.py
+-rw-rw-rw-   0        0        0     3939 2023-07-12 12:47:53.000000 mcmc_statphys-1.0.0/mcmc_statphys/model/Ice.py
+-rw-rw-rw-   0        0        0    10707 2023-07-12 12:47:56.000000 mcmc_statphys-1.0.0/mcmc_statphys/model/Ising.py
+-rw-rw-rw-   0        0        0     3616 2023-07-12 12:48:09.000000 mcmc_statphys-1.0.0/mcmc_statphys/model/NVT.py
+-rw-rw-rw-   0        0        0     3450 2023-07-12 12:48:17.000000 mcmc_statphys-1.0.0/mcmc_statphys/model/Potts.py
+-rw-rw-rw-   0        0        0     4331 2023-07-12 12:48:18.000000 mcmc_statphys-1.0.0/mcmc_statphys/model/RFIsing.py
+-rw-rw-rw-   0        0        0     5539 2023-07-12 12:48:36.000000 mcmc_statphys-1.0.0/mcmc_statphys/model/SKmodel.py
+-rw-rw-rw-   0        0        0     3815 2023-07-12 12:48:42.000000 mcmc_statphys-1.0.0/mcmc_statphys/model/Staurss.py
+-rw-rw-rw-   0        0        0     2728 2023-07-12 12:48:46.000000 mcmc_statphys-1.0.0/mcmc_statphys/model/XY.py
+-rw-rw-rw-   0        0        0      331 2023-07-12 12:46:22.000000 mcmc_statphys-1.0.0/mcmc_statphys/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:53:02.892294 mcmc_statphys-1.0.0/mcmc_statphys.egg-info/
+-rw-rw-rw-   0        0        0     4647 2023-07-12 12:53:02.000000 mcmc_statphys-1.0.0/mcmc_statphys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2026 2023-07-12 12:53:02.000000 mcmc_statphys-1.0.0/mcmc_statphys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:53:02.000000 mcmc_statphys-1.0.0/mcmc_statphys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-12 12:53:02.000000 mcmc_statphys-1.0.0/mcmc_statphys.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-14 13:46:13.000000 mcmc_statphys-1.0.0/mcmc_statphys.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      141 2023-07-12 12:53:02.000000 mcmc_statphys-1.0.0/mcmc_statphys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-12 12:53:02.000000 mcmc_statphys-1.0.0/mcmc_statphys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      520 2023-07-12 12:53:02.947148 mcmc_statphys-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1697 2023-07-12 12:51:19.000000 mcmc_statphys-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:53:02.914235 mcmc_statphys-1.0.0/tests/
+-rw-rw-rw-   0        0        0       43 2023-07-01 03:10:02.000000 mcmc_statphys-1.0.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:53:02.917227 mcmc_statphys-1.0.0/tests/one/
+-rw-rw-rw-   0        0        0      313 2023-07-01 03:10:02.000000 mcmc_statphys-1.0.0/tests/one/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:53:02.937173 mcmc_statphys-1.0.0/tests/one/algorithm/
+-rw-rw-rw-   0        0        0     3084 2023-07-12 12:46:29.000000 mcmc_statphys-1.0.0/tests/one/algorithm/Anneal.py
+-rw-rw-rw-   0        0        0     2629 2023-07-12 12:46:29.000000 mcmc_statphys-1.0.0/tests/one/algorithm/Demon.py
+-rw-rw-rw-   0        0        0     3990 2023-07-12 12:46:29.000000 mcmc_statphys-1.0.0/tests/one/algorithm/HamiltonianMC.py
+-rw-rw-rw-   0        0        0     1735 2023-07-12 12:46:29.000000 mcmc_statphys-1.0.0/tests/one/algorithm/Kawasaki.py
+-rw-rw-rw-   0        0        0    16114 2023-07-12 12:46:29.000000 mcmc_statphys-1.0.0/tests/one/algorithm/Metropolis.py
+-rw-rw-rw-   0        0        0     2031 2023-07-12 12:46:29.000000 mcmc_statphys-1.0.0/tests/one/algorithm/Tempering.py
+-rw-rw-rw-   0        0        0     4653 2023-07-12 12:46:29.000000 mcmc_statphys-1.0.0/tests/one/algorithm/WangLandau.py
+-rw-rw-rw-   0        0        0     4772 2023-07-12 12:46:29.000000 mcmc_statphys-1.0.0/tests/one/algorithm/Wolff.py
+-rw-rw-rw-   0        0        0      314 2023-07-01 03:10:02.000000 mcmc_statphys-1.0.0/tests/one/algorithm/__init__.py
+-rw-rw-rw-   0        0        0      419 2023-07-01 03:10:02.000000 mcmc_statphys-1.0.0/tests/one/cli.py
+-rw-rw-rw-   0        0        0    11105 2023-07-12 12:51:08.000000 mcmc_statphys-1.0.0/tests/one/method.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:53:02.945152 mcmc_statphys-1.0.0/tests/one/model/
+-rw-rw-rw-   0        0        0     3824 2023-07-12 12:44:59.000000 mcmc_statphys-1.0.0/tests/one/model/BaseModel.txt
+-rw-rw-rw-   0        0        0     2771 2023-07-12 12:50:21.000000 mcmc_statphys-1.0.0/tests/one/model/Heisenberg.py
+-rw-rw-rw-   0        0        0     3939 2023-07-12 12:44:59.000000 mcmc_statphys-1.0.0/tests/one/model/Ice.py
+-rw-rw-rw-   0        0        0    10707 2023-07-12 12:50:25.000000 mcmc_statphys-1.0.0/tests/one/model/Ising.py
+-rw-rw-rw-   0        0        0     3616 2023-07-12 12:50:31.000000 mcmc_statphys-1.0.0/tests/one/model/NVT.py
+-rw-rw-rw-   0        0        0     3450 2023-07-12 12:50:35.000000 mcmc_statphys-1.0.0/tests/one/model/Potts.py
+-rw-rw-rw-   0        0        0     4331 2023-07-12 12:50:47.000000 mcmc_statphys-1.0.0/tests/one/model/RFIsing.py
+-rw-rw-rw-   0        0        0     5539 2023-07-12 12:50:55.000000 mcmc_statphys-1.0.0/tests/one/model/SKmodel.py
+-rw-rw-rw-   0        0        0     3815 2023-07-12 12:44:59.000000 mcmc_statphys-1.0.0/tests/one/model/Staurss.py
+-rw-rw-rw-   0        0        0     2728 2023-07-12 12:50:59.000000 mcmc_statphys-1.0.0/tests/one/model/XY.py
+-rw-rw-rw-   0        0        0      331 2023-07-12 12:46:33.000000 mcmc_statphys-1.0.0/tests/one/model/__init__.py
+-rw-rw-rw-   0        0        0   182245 2023-07-12 12:44:59.000000 mcmc_statphys-1.0.0/tests/test-DESKTOP-KD1PM0R.ipynb
+-rw-rw-rw-   0        0        0  2007115 2023-07-12 12:44:59.000000 mcmc_statphys-1.0.0/tests/test.gif
+-rw-rw-rw-   0        0        0     3375 2023-07-12 12:51:03.000000 mcmc_statphys-1.0.0/tests/test.ipynb
+-rw-rw-rw-   0        0        0      920 2023-07-01 03:10:02.000000 mcmc_statphys-1.0.0/tests/test_mcmc_statphys.py
```

### Comparing `mcmc_statphys-0.4.3/CONTRIBUTING.rst` & `mcmc_statphys-1.0.0/CONTRIBUTING.rst`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-.. highlight:: shell
-
-============
-Contributing
-============
-
-Contributions are welcome, and they are greatly appreciated! Every little bit
-helps, and credit will always be given.
-
-You can contribute in many ways:
-
-Types of Contributions
-----------------------
-
-Report Bugs
-~~~~~~~~~~~
-
-Report bugs at https://github.com/uynajgi/mcmc_statphys/issues.
-
-If you are reporting a bug, please include:
-
-* Your operating system name and version.
-* Any details about your local setup that might be helpful in troubleshooting.
-* Detailed steps to reproduce the bug.
-
-Fix Bugs
-~~~~~~~~
-
-Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
-wanted" is open to whoever wants to implement it.
-
-Implement Features
-~~~~~~~~~~~~~~~~~~
-
-Look through the GitHub issues for features. Anything tagged with "enhancement"
-and "help wanted" is open to whoever wants to implement it.
-
-Write Documentation
-~~~~~~~~~~~~~~~~~~~
-
-mcmc_statphys could always use more documentation, whether as part of the
-official mcmc_statphys docs, in docstrings, or even on the web in blog posts,
-articles, and such.
-
-Submit Feedback
-~~~~~~~~~~~~~~~
-
-The best way to send feedback is to file an issue at https://github.com/uynajgi/mcmc_statphys/issues.
-
-If you are proposing a feature:
-
-* Explain in detail how it would work.
-* Keep the scope as narrow as possible, to make it easier to implement.
-* Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
-
-Get Started!
-------------
-
-Ready to contribute? Here's how to set up `mcmc_statphys` for local development.
-
-1. Fork the `mcmc_statphys` repo on GitHub.
-2. Clone your fork locally::
-
-    $ git clone git@github.com:your_name_here/mcmc_statphys.git
-
-3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
-
-    $ mkvirtualenv mcmc_statphys
-    $ cd mcmc_statphys/
-    $ python setup.py develop
-
-4. Create a branch for local development::
-
-    $ git checkout -b name-of-your-bugfix-or-feature
-
-   Now you can make your changes locally.
-
-5. When you're done making changes, check that your changes pass flake8 and the
-   tests, including testing other Python versions with tox::
-
-    $ flake8 mcmc_statphys tests
-    $ python setup.py test or pytest
-    $ tox
-
-   To get flake8 and tox, just pip install them into your virtualenv.
-
-6. Commit your changes and push your branch to GitHub::
-
-    $ git add .
-    $ git commit -m "Your detailed description of your changes."
-    $ git push origin name-of-your-bugfix-or-feature
-
-7. Submit a pull request through the GitHub website.
-
-Pull Request Guidelines
------------------------
-
-Before you submit a pull request, check that it meets these guidelines:
-
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
-3. The pull request should work for Python 3.5, 3.6, 3.7, 3.8 and 3.9, and for PyPy. Check
-   https://travis-ci.com/uynajgi/mcmc_statphys/pull_requests
-   and make sure that the tests pass for all supported Python versions.
-
-Tips
-----
-
-To run a subset of tests::
-
-
-    $ python -m unittest tests.test_mcmc_statphys
-
-Deploying
----------
-
-A reminder for the maintainers on how to deploy.
-Make sure all your changes are committed (including an entry in HISTORY.rst).
-Then run::
-
-$ bump2version patch # possible: major / minor / patch
-$ git push
-$ git push --tags
-
-Travis will then deploy to PyPI if tests pass.
+.. highlight:: shell
+
+============
+Contributing
+============
+
+Contributions are welcome, and they are greatly appreciated! Every little bit
+helps, and credit will always be given.
+
+You can contribute in many ways:
+
+Types of Contributions
+----------------------
+
+Report Bugs
+~~~~~~~~~~~
+
+Report bugs at https://github.com/uynajgi/mcmc_statphys/issues.
+
+If you are reporting a bug, please include:
+
+* Your operating system name and version.
+* Any details about your local setup that might be helpful in troubleshooting.
+* Detailed steps to reproduce the bug.
+
+Fix Bugs
+~~~~~~~~
+
+Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
+wanted" is open to whoever wants to implement it.
+
+Implement Features
+~~~~~~~~~~~~~~~~~~
+
+Look through the GitHub issues for features. Anything tagged with "enhancement"
+and "help wanted" is open to whoever wants to implement it.
+
+Write Documentation
+~~~~~~~~~~~~~~~~~~~
+
+mcmc_statphys could always use more documentation, whether as part of the
+official mcmc_statphys docs, in docstrings, or even on the web in blog posts,
+articles, and such.
+
+Submit Feedback
+~~~~~~~~~~~~~~~
+
+The best way to send feedback is to file an issue at https://github.com/uynajgi/mcmc_statphys/issues.
+
+If you are proposing a feature:
+
+* Explain in detail how it would work.
+* Keep the scope as narrow as possible, to make it easier to implement.
+* Remember that this is a volunteer-driven project, and that contributions
+  are welcome :)
+
+Get Started!
+------------
+
+Ready to contribute? Here's how to set up `mcmc_statphys` for local development.
+
+1. Fork the `mcmc_statphys` repo on GitHub.
+2. Clone your fork locally::
+
+    $ git clone git@github.com:your_name_here/mcmc_statphys.git
+
+3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
+
+    $ mkvirtualenv mcmc_statphys
+    $ cd mcmc_statphys/
+    $ python setup.py develop
+
+4. Create a branch for local development::
+
+    $ git checkout -b name-of-your-bugfix-or-feature
+
+   Now you can make your changes locally.
+
+5. When you're done making changes, check that your changes pass flake8 and the
+   tests, including testing other Python versions with tox::
+
+    $ flake8 mcmc_statphys tests
+    $ python setup.py test or pytest
+    $ tox
+
+   To get flake8 and tox, just pip install them into your virtualenv.
+
+6. Commit your changes and push your branch to GitHub::
+
+    $ git add .
+    $ git commit -m "Your detailed description of your changes."
+    $ git push origin name-of-your-bugfix-or-feature
+
+7. Submit a pull request through the GitHub website.
+
+Pull Request Guidelines
+-----------------------
+
+Before you submit a pull request, check that it meets these guidelines:
+
+1. The pull request should include tests.
+2. If the pull request adds functionality, the docs should be updated. Put
+   your new functionality into a function with a docstring, and add the
+   feature to the list in README.rst.
+3. The pull request should work for Python 3.5, 3.6, 3.7, 3.8 and 3.9, and for PyPy. Check
+   https://travis-ci.com/uynajgi/mcmc_statphys/pull_requests
+   and make sure that the tests pass for all supported Python versions.
+
+Tips
+----
+
+To run a subset of tests::
+
+
+    $ python -m unittest tests.test_mcmc_statphys
+
+Deploying
+---------
+
+A reminder for the maintainers on how to deploy.
+Make sure all your changes are committed (including an entry in HISTORY.rst).
+Then run::
+
+$ bump2version patch # possible: major / minor / patch
+$ git push
+$ git push --tags
+
+Travis will then deploy to PyPI if tests pass.
```

### Comparing `mcmc_statphys-0.4.3/LICENSE` & `mcmc_statphys-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023, Uynaj GI
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2023, Uynaj GI
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `mcmc_statphys-0.4.3/PKG-INFO` & `mcmc_statphys-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: mcmc_statphys
-Version: 0.4.3
+Version: 1.0.0
 Summary: A library project of Monte Carlo simulation algorithms for some statistical physics models (in particular, the Ising model and its variants).
 Home-page: https://github.com/uynajgi/mcmc_statphys
 Author: Uynaj GI
 Author-email: suquan12148@outlook.com
 License: MIT license
 Keywords: mcmc_statphys
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -49,23 +50,23 @@
 
 A simple Ising model simulation.
 
 .. code-block:: python
 
     >>> import mcmc_statphys as mcsp
     >>> model = mcsp.model.Ising(12) # 12x12 Ising model
-    >>> algorithm = mcsp.method.Metropolis(model) # Metropolis algorithm
+    >>> algorithm = mcsp.algorithm.Metropolis(model) # Metropolis algorithm
     >>> uid = algorithm.equil_sample(T=1, max_iter=1000) # sample until equilibrium
-    >>> fig = mcsp.draw.Plot(algorithm) 
+    >>> fig = mcsp.draw.Plot(algorithm)
     >>> fig.curve(uid=uid, comlumn='energy') # plot the energy curve
 
 Install
 -------
 
-the latest version of mcmc_statphys: 
+the latest version of mcmc_statphys:
 
 .. code-block:: console
 
     $ pip install mcmc_statphys
 
 upgrade to the latest version:
 
@@ -170,7 +171,9 @@
 
 * Add documentation to README
 
 [0.1.1] - 2023-05-14
 --------------------
 
 * First release on PyPI.
+
+
```

### Comparing `mcmc_statphys-0.4.3/README.rst` & `mcmc_statphys-1.0.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-=============
-mcmc_statphys
-=============
-
-
-.. image:: https://img.shields.io/pypi/v/mcmc_statphys.svg
-        :target: https://pypi.python.org/pypi/mcmc_statphys
-
-.. image:: https://img.shields.io/travis/uynajgi/mcmc_statphys.svg
-        :target: https://travis-ci.com/uynajgi/mcmc_statphys
-
-.. image:: https://readthedocs.org/projects/mcmc-statphys/badge/?version=latest
-        :target: https://mcmc-statphys.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-
-
-
-A Python package of Monte Carlo simulation algorithms for some statistical physics models (in particular, the Ising model and its variants).
-
-
-* Free software: MIT license
-* Documentation: https://mcmc-statphys.readthedocs.io.
-
-
-Features
---------
-
-A simple Ising model simulation.
-
-.. code-block:: python
-
-    >>> import mcmc_statphys as mcsp
-    >>> model = mcsp.model.Ising(12) # 12x12 Ising model
-    >>> algorithm = mcsp.method.Metropolis(model) # Metropolis algorithm
-    >>> uid = algorithm.equil_sample(T=1, max_iter=1000) # sample until equilibrium
-    >>> fig = mcsp.draw.Plot(algorithm) 
-    >>> fig.curve(uid=uid, comlumn='energy') # plot the energy curve
-
-Install
--------
-
-the latest version of mcmc_statphys: 
-
-.. code-block:: console
-
-    $ pip install mcmc_statphys
-
-upgrade to the latest version:
-
-.. code-block:: console
-
-    $ pip install --upgrade mcmc_statphys
-
-Bugs
-----
-
-Please report any bugs that you find `here`_. Or, even better, fork the repository on `GitHub`_ and create a pull request (PR). We welcome all changes, big or small, and we will help you make the PR if you are new to git (just ask on the issue and/or see `CONTRIBUTING`_).
-
-.. _here: https://github.com/uynajgi/mcmc_statphys/issues
-.. _GitHub: https://github.com/uynajgi/mcmc_statphys/
-.. _CONTRIBUTING: https://mcmc-statphys.readthedocs.io/en/latest/contributing.html
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+=============
+mcmc_statphys
+=============
+
+
+.. image:: https://img.shields.io/pypi/v/mcmc_statphys.svg
+        :target: https://pypi.python.org/pypi/mcmc_statphys
+
+.. image:: https://img.shields.io/travis/uynajgi/mcmc_statphys.svg
+        :target: https://travis-ci.com/uynajgi/mcmc_statphys
+
+.. image:: https://readthedocs.org/projects/mcmc-statphys/badge/?version=latest
+        :target: https://mcmc-statphys.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+
+
+
+A Python package of Monte Carlo simulation algorithms for some statistical physics models (in particular, the Ising model and its variants).
+
+
+* Free software: MIT license
+* Documentation: https://mcmc-statphys.readthedocs.io.
+
+
+Features
+--------
+
+A simple Ising model simulation.
+
+.. code-block:: python
+
+    >>> import mcmc_statphys as mcsp
+    >>> model = mcsp.model.Ising(12) # 12x12 Ising model
+    >>> algorithm = mcsp.algorithm.Metropolis(model) # Metropolis algorithm
+    >>> uid = algorithm.equil_sample(T=1, max_iter=1000) # sample until equilibrium
+    >>> fig = mcsp.draw.Plot(algorithm)
+    >>> fig.curve(uid=uid, comlumn='energy') # plot the energy curve
+
+Install
+-------
+
+the latest version of mcmc_statphys:
+
+.. code-block:: console
+
+    $ pip install mcmc_statphys
+
+upgrade to the latest version:
+
+.. code-block:: console
+
+    $ pip install --upgrade mcmc_statphys
+
+Bugs
+----
+
+Please report any bugs that you find `here`_. Or, even better, fork the repository on `GitHub`_ and create a pull request (PR). We welcome all changes, big or small, and we will help you make the PR if you are new to git (just ask on the issue and/or see `CONTRIBUTING`_).
+
+.. _here: https://github.com/uynajgi/mcmc_statphys/issues
+.. _GitHub: https://github.com/uynajgi/mcmc_statphys/
+.. _CONTRIBUTING: https://mcmc-statphys.readthedocs.io/en/latest/contributing.html
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `mcmc_statphys-0.4.3/docs/Makefile` & `mcmc_statphys-1.0.0/docs/Makefile`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line.
-SPHINXOPTS    =
-SPHINXBUILD   = python -msphinx
-SPHINXPROJ    = mcmc_statphys
-SOURCEDIR     = .
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line.
+SPHINXOPTS    =
+SPHINXBUILD   = python -msphinx
+SPHINXPROJ    = mcmc_statphys
+SOURCEDIR     = .
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `mcmc_statphys-0.4.3/docs/conf.py` & `mcmc_statphys-1.0.0/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-#!/usr/bin/env python
-#
-# mcmc_statphys documentation build configuration file, created by
-# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
-#
-# This file is execfile()d with the current directory set to its
-# containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-# If extensions (or modules to document with autodoc) are in another
-# directory, add these directories to sys.path here. If the directory is
-# relative to the documentation root, use os.path.abspath to make it
-# absolute, like shown here.
-#
-
-import os
-import sys
-
-sys.path.insert(0, os.path.abspath('..'))
-
-# import mcmc_statphys
-# -- General configuration ---------------------------------------------
-
-# If your documentation needs a minimal Sphinx version, state it here.
-#
-# needs_sphinx = '1.0'
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
-
-# The suffix(es) of source filenames.
-# You can specify multiple suffix as a list of string:
-#
-# source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
-
-# The master toctree document.
-master_doc = 'index'
-
-# General information about the project.
-project = 'mcmc_statphys'
-copyright = "2023, Uynaj GI"
-author = "Uynaj GI"
-
-# The version info for the project you're documenting, acts as replacement
-# for |version| and |release|, also used in various other places throughout
-# the built documents.
-#
-# The short X.Y version.
-version = '0.4.3'
-# The full version, including alpha/beta/rc tags.
-release = version
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-#
-# This is also used if you do content translation via gettext catalogs.
-# Usually you set "language" from the command line for these cases.
-language = None
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = False
-
-# -- Options for HTML output -------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-#
-html_theme = 'alabaster'
-
-# Theme options are theme-specific and customize the look and feel of a
-# theme further.  For a list of options available for each theme, see the
-# documentation.
-#
-# html_theme_options = {}
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
-
-# -- Options for HTMLHelp output ---------------------------------------
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = 'mcmc_statphysdoc'
-
-# -- Options for LaTeX output ------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #
-    # 'papersize': 'letterpaper',
-
-    # The font size ('10pt', '11pt' or '12pt').
-    #
-    # 'pointsize': '10pt',
-
-    # Additional stuff for the LaTeX preamble.
-    #
-    # 'preamble': '',
-
-    # Latex figure (float) alignment
-    #
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass
-# [howto, manual, or own class]).
-latex_documents = [
-    (master_doc, 'mcmc_statphys.tex', 'mcmc_statphys Documentation',
-     'Uynaj GI', 'manual'),
-]
-
-# -- Options for manual page output ------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [(master_doc, 'mcmc_statphys', 'mcmc_statphys Documentation',
-              [author], 1)]
-
-# -- Options for Texinfo output ----------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (master_doc, 'mcmc_statphys', 'mcmc_statphys Documentation', author,
-     'mcmc_statphys', 'One line description of project.', 'Miscellaneous'),
-]
+#!/usr/bin/env python
+#
+# mcmc_statphys documentation build configuration file, created by
+# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
+#
+# This file is execfile()d with the current directory set to its
+# containing dir.
+#
+# Note that not all possible configuration values are present in this
+# autogenerated file.
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+
+# If extensions (or modules to document with autodoc) are in another
+# directory, add these directories to sys.path here. If the directory is
+# relative to the documentation root, use os.path.abspath to make it
+# absolute, like shown here.
+#
+
+import os
+import sys
+
+sys.path.insert(0, os.path.abspath('..'))
+
+# import mcmc_statphys
+# -- General configuration ---------------------------------------------
+
+# If your documentation needs a minimal Sphinx version, state it here.
+#
+# needs_sphinx = '1.0'
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ['_templates']
+
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+#
+# source_suffix = ['.rst', '.md']
+source_suffix = '.rst'
+
+# The master toctree document.
+master_doc = 'index'
+
+# General information about the project.
+project = 'mcmc_statphys'
+copyright = "2023, Uynaj GI"
+author = "Uynaj GI"
+
+# The version info for the project you're documenting, acts as replacement
+# for |version| and |release|, also used in various other places throughout
+# the built documents.
+#
+# The short X.Y version.
+version = '1.0.0'
+# The full version, including alpha/beta/rc tags.
+release = version
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+#
+# This is also used if you do content translation via gettext catalogs.
+# Usually you set "language" from the command line for these cases.
+language = None
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This patterns also effect to html_static_path and html_extra_path
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = 'sphinx'
+
+# If true, `todo` and `todoList` produce output, else they produce nothing.
+todo_include_todos = False
+
+# -- Options for HTML output -------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+#
+html_theme = 'alabaster'
+
+# Theme options are theme-specific and customize the look and feel of a
+# theme further.  For a list of options available for each theme, see the
+# documentation.
+#
+# html_theme_options = {}
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ['_static']
+
+# -- Options for HTMLHelp output ---------------------------------------
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = 'mcmc_statphysdoc'
+
+# -- Options for LaTeX output ------------------------------------------
+
+latex_elements = {
+    # The paper size ('letterpaper' or 'a4paper').
+    #
+    # 'papersize': 'letterpaper',
+
+    # The font size ('10pt', '11pt' or '12pt').
+    #
+    # 'pointsize': '10pt',
+
+    # Additional stuff for the LaTeX preamble.
+    #
+    # 'preamble': '',
+
+    # Latex figure (float) alignment
+    #
+    # 'figure_align': 'htbp',
+}
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title, author, documentclass
+# [howto, manual, or own class]).
+latex_documents = [
+    (master_doc, 'mcmc_statphys.tex', 'mcmc_statphys Documentation',
+     'Uynaj GI', 'manual'),
+]
+
+# -- Options for manual page output ------------------------------------
+
+# One entry per manual page. List of tuples
+# (source start file, name, description, authors, manual section).
+man_pages = [(master_doc, 'mcmc_statphys', 'mcmc_statphys Documentation',
+              [author], 1)]
+
+# -- Options for Texinfo output ----------------------------------------
+
+# Grouping the document tree into Texinfo files. List of tuples
+# (source start file, target name, title, author,
+#  dir menu entry, description, category)
+texinfo_documents = [
+    (master_doc, 'mcmc_statphys', 'mcmc_statphys Documentation', author,
+     'mcmc_statphys', 'One line description of project.', 'Miscellaneous'),
+]
```

### Comparing `mcmc_statphys-0.4.3/docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png` & `mcmc_statphys-1.0.0/docs/img/energy-73cbe80ef4b811ed9b0400e04c6807cc.png`

 * *Files identical despite different names*

### Comparing `mcmc_statphys-0.4.3/docs/modules.rst` & `mcmc_statphys-1.0.0/docs/modules.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,267 +1,270 @@
-Module
-======
-
-In the lastest version(0.3.0) of ``mcmc_statphys``, we have these modules:
-
-``mcmc_statphys.model``
------------------------
-
-In this subpackage, we have Ising model, Heisenberg model, Potts model, and XY model.
-
-``Ising``
-~~~~~~~~~
-
-The Ising model is a mathematical model of ferromagnetism in statistical mechanics. The model consists of discrete variables that represent magnetic dipole moments of atomic spins that can be in one of two states (+1 or −1). The spins are arranged in a graph, usually a lattice, allowing each spin to interact with its neighbors. The model allows the identification of phase transitions, as a simplified model of reality.
-
-The detial of the Ising model can be found in `Wikipedia <https://en.wikipedia.org/wiki/Ising_model>`__.
-
--  attribute
-
-   -  L: ``int``, the length of the lattice
-   -  dim: ``int``, the dimension of the lattice
-   -  J: ``float``, the interaction strength
-   -  H: ``float``, the external field strength
-   -  spin: ``numpy.ndarray``, the spin configuration
-   -  energy: ``float``, the energy of the spin configuration
-   -  magnetization: ``float``, the magnetization of the spin
-      configuration
-   -  type: ``str``, the type of the model
-
--  method
-
-   -  ``__init__(self, L, dim, J, H)``: initialize the Ising model
-   -  ``set_spin(self, spin)``: set the spin configuration Args: spin:
-      ``numpy.ndarray``, the spin configuration
-   -  ``get_energy(self)``: get the energy of the spin configuration
-      Returns: energy\ ``float``: The total energy of the system
-   -  ``get_magnetization(self)``: get the magnetization of the spin
-      configuration Returns: magnetization\ ``float``: The total
-      magnetization of the system
-
-``Heisenberg``
-~~~~~~~~~~~~~~
-
-The Heisenberg model is a mathematical model in quantum mechanics used to explain the magnetic properties of materials. It arises from the exchange interaction between the spins of electrons. The spins in a Heisenberg model are treated as classical vectors. The spins are typically taken to be three-component vectors (x, y, z), but other representations are possible. The Heisenberg model is a type of an Ising model, namely, a model of interacting spins. 
-
-The detial of the Heisenberg model can be found in `Wikipedia <https://en.wikipedia.org/wiki/Classical_Heisenberg_model>`__.
-
-Attribute and method are the same as ``Ising``.
-
-``Potts``
-~~~~~~~~~
-
-The Potts model, a generalization of the Ising model, is a model in statistical mechanics that describes a collection of spins that can take on q different states on a regular lattice. It was introduced by the English mathematician R. B. Potts in 1952. The states of the spins are denoted s = 1, …, q. 
-
-The detial of the Potts model can be found in `Wikipedia <https://en.wikipedia.org/wiki/Potts_model>`__.
-
-Attribute and method are the same as ``Ising``.
-
-``XY``
-~~~~~~
-
-The XY model is a model of a magnet where the spins lie on a plane and interact with each other only through their orientation. It is named after the two-dimensional XY model, but the same name is also used to describe related models in different numbers of dimensions. The XY model  is one of the simplest statistical models exhibiting a phase transition with a continuous symmetry group.
-
-The detial of the XY model can be found in `Wikipedia <https://en.wikipedia.org/wiki/Classical_XY_model>`__.
-
-Attribute and method are the same as ``Ising``.
-
-``mcmc_statphys.algorithm``
----------------------------
-
-In this subpackage, we have Metropolis algorithm, Wolff algorithm, and Annelaing algorithm.
-
-``Metropolis``
-~~~~~~~~~~~~~~
-
-The Metropolis algorithm, also referred to as the Metropolis Monte Carlo algorithm, is a Monte Carlo method used to generate an approximate probability distribution through a sequence of random samples. The Metropolis algorithm is often used in statistical physics to compute the canonical ensemble and in chemistry to simulate the behavior of atoms in a material.
-
-The detial of the Metropolis algorithm can be found in `Wikipedia <https://en.wikipedia.org/wiki/Metropolis%E2%80%93Hastings_algorithm>`__.
-
--  attribute
-
-   -  model: ``mcmc_statphys.model``, the model to simulate
-   -  name: ``str``, the name of the algorithm
-   -  iter_data: ``dict``, the data of the iteration(with the unique
-      ``uid`` for each iteration)
-   -  parameter: ``str``, the name of the parameter
-
--  method
-
-   -  ``iter_sample(self, T: float, uid: str = None) -> str``: 
-      
-      Do one iteration of the algorithm
-      
-      Args: 
-
-      - T: ``float``, the temperature
-      - uid: ``str``, the unique id of the iteration
-      
-      Returns:
-
-      - uid: ``str``, the unique id of the iteration
-   
-   -  ``equil_sample(self, T: float, max_iter: int = 1000, uid: str = None) -> str``:
-      
-      Do the equilibration of the algorithm 
-      
-      Args: 
-
-      - T: ``float``, the temperature of sample 
-      - max_iter: ``int``, the maximum number of iterations (Default: 1000) 
-      - uid: ``str``, the unique id of the iteration
-      
-      Returns:
-
-      - uid: ``str``, the unique id of the iteration
-
-   -  ``param_sample(self, max_iter: int = 1000) -> Dict``: 
-
-      Do the parameter sampling of the algorithm 
-
-      Args:
-
-      - max_iter: ``int``, the maximum number of iterations (Default: 1000) 
-
-      Returns: 
-      
-      - param_data: ``dict``, the data of the parameter sampling
-
-``Wolff``
-~~~~~~~~~
-
-The Wolff algorithm is a Monte Carlo algorithm for generating configurations of an Ising model or Potts model. It was invented by Ulli Wolff in 1989.
-
-The detial of the Wolff algorithm can be found in `Wikipedia <https://en.wikipedia.org/wiki/Wolff_algorithm>`__.
-
-Attribute and method are the same as ``Metropolis``.
-
-``Anneal``
-~~~~~~~~~~
-
-Simulated annealing is a probabilistic technique for approximating the global optimum of a given function. Specifically, it is a metaheuristic to approximate global optimization in a large search space for an optimization problem. It is often used when the search space is discrete (e.g., all tours that visit a given set of cities). For problems where finding an approximate global optimum is more important than finding a precise local optimum in a fixed amount of time, simulated annealing may be preferable to alternatives such as gradient descent.
-
-The detial of the Annelaing algorithm can be found in `Wikipedia <https://en.wikipedia.org/wiki/Simulated_annealing>`__.
-
-Attribute and method are the same as ``Metropolis``, except of ``equil_sample``.
-
--  method
-   - ``equil_sample(self, targetT: float, max_iter: int = 1000, highT=None, dencyT=0.9, uid: str = None, ) -> str``:
-
-      Do the equilibration of the algorithm 
-      
-      Args: 
-      
-      - targetT: ``float``, the target temperature of sample 
-      - max_iter: ``int``, the maximum number of iterations (Default: 1000) 
-      - highT: ``float``, the high temperature of the annealing (Default: 2 \* targetT) 
-      - dencyT: ``float``, the density of the annealing (Default: 0.9) 
-      - uid: ``str``, the unique id of the iteration 
-      
-      Returns: 
-      
-      - uid: ``str``, the unique id of the iteration
-
-``mcmc_statphys.analysis``
---------------------------
-
-In this subpackage, we have the analysis of the data.
-
--  ``mean(algorithm: object, uid: str, column: str) -> float``:
-
-   Calculate the mean of the data
-   
-   Args: 
-   
-   - algorithm: ``object``, the ``mcmc_statphys.algorithm`` object 
-   - uid: ``str``, the unique id of the iteration
-   - column: ``str``, the name of the column 
-
-   Returns: 
-   
-   - mean: ``float``, the mean of the data
-
--  ``std(algorithm: object, uid: str, column: str) -> float``: 
-   
-   Calculate the standard deviation of the data
-   
-   Args: 
-   
-   - algorithm: ``object``, the ``mcmc_statphys.algorithm`` object 
-   - uid: ``str``, the unique id of the iteration
-   -  column: ``str``, the name of the column 
-
-   Returns: 
-   
-   - std: ``float``, the standard deviation of the data
-
--  ``cv(algorithm: object, uid: str, column: str) -> float``: 
-
-   Calculate the coefficient of variation of the data 
-   
-   Args: 
-   
-   - algorithm: ``object``, the ``mcmc_statphys.algorithm`` object
-   -  uid: ``str``, the unique id of the iteration 
-   -  column: ``str``, the name of the column
-
-   Returns:
-   
-   - cv: ``float``, the coefficient of variation
-
--  ``diff(algorithm: object, uid: str, column: str) -> float``: 
-   
-   Calculate the difference of the data
-   
-   Args:
-   
-   - algorithm: ``object``, the ``mcmc_statphys.algorithm`` object 
-   - uid: ``str``, the unique id of the iteration column: ``str``, the name of the column 
-   
-   Returns: 
-   
-   - diff: ``float``, the difference of the data
-
--  ``getcolumn(algorithm: object, uid: str, column: str) -> numpy.ndarray``:
-
-   Get the column of the data
-   
-   Args:
-   
-   - algorithm: ``object``, the ``mcmc_statphys.algorithm`` object 
-   - uid: ``str``, the unique id of the iteration 
-   - column: ``str``, the name of the column 
-
-   Returns:
-   
-   - column: ``numpy.ndarray``, the column of the data
-
--  ``spin2svd(algorithm: object, uid: str) -> float``: 
-
-   Convert the spin configuration to the singular value decomposition
-   
-   Args:
-   
-   - algorithm: ``object``, the ``mcmc_statphys.algorithm`` object
-   -  uid: ``str``, the unique id of the iteration 
-   -  column: ``str``, the name of the column
-
-   Returns:
-   - max_v: ``float``, the maximum singular value of the spin configuration
-
--  ``uid2svd(algorithm: object, uid_lst: List[int] or Dict) -> List[float]``:
-
-   Convert the spin configuration to the singular value decomposition
-   
-   Args: 
-
-   - algorithm: ``object``, the ``mcmc_statphys.algorithm`` object 
-   - uid_lst: ``List[int]`` or ``Dict``, the unique id of the iteration
-
-   Returns:
-   
-   - max_v_lst: ``List[float]``, the list of the maximum singular value of the spin configuration
-
-``mcmc_statphys.draw``
-----------------------
-
-In this subpackage, we have the draw of the data.
+Module
+======
+
+In the lastest version(0.3.0) of ``mcmc_statphys``, we have these modules:
+
+``mcmc_statphys.model``
+-----------------------
+
+In this subpackage, we have Ising model, Heisenberg model, Potts model, and XY model.
+
+``Ising``
+~~~~~~~~~
+
+The Ising model is a mathematical model of ferromagnetism in statistical mechanics. The model consists of discrete variables that represent magnetic dipole moments of atomic spins that can be in one of two states (+1 or −1). The spins are arranged in a graph, usually a lattice, allowing each spin to interact with its neighbors. The model allows the identification of phase transitions, as a simplified model of reality.
+
+The detial of the Ising model can be found in `Wikipedia <https://en.wikipedia.org/wiki/Ising_model>`__.
+
+-  attribute
+
+   -  L: ``int``, the length of the lattice
+   -  dim: ``int``, the dimension of the lattice
+   -  J: ``float``, the interaction strength
+   -  H: ``float``, the external field strength
+   -  spin: ``numpy.ndarray``, the spin configuration
+   -  energy: ``float``, the energy of the spin configuration
+   -  magnetization: ``float``, the magnetization of the spin
+      configuration
+   -  type: ``str``, the type of the model
+
+-  method
+
+   -  ``__init__(self, L, dim, J, H)``: initialize the Ising model
+   -  ``set_spin(self, spin)``: set the spin configuration Args: spin:
+      ``numpy.ndarray``, the spin configuration
+   -  ``get_energy(self)``: get the energy of the spin configuration
+      Returns: energy\ ``float``: The total energy of the system
+   -  ``get_magnetization(self)``: get the magnetization of the spin
+      configuration Returns: magnetization\ ``float``: The total
+      magnetization of the system
+
+``Heisenberg``
+~~~~~~~~~~~~~~
+
+The Heisenberg model is a mathematical model in quantum mechanics used to explain the magnetic properties of materials. It arises from the exchange interaction between the spins of electrons. The spins in a Heisenberg model are treated as classical vectors. The spins are typically taken to be three-component vectors (x, y, z), but other representations are possible. The Heisenberg model is a type of an Ising model, namely, a model of interacting spins. 
+
+The detial of the Heisenberg model can be found in `Wikipedia <https://en.wikipedia.org/wiki/Classical_Heisenberg_model>`__.
+
+Attribute and method are the same as ``Ising``.
+
+``Potts``
+~~~~~~~~~
+
+The Potts model, a generalization of the Ising model, is a model in statistical mechanics that describes a collection of spins that can take on q different states on a regular lattice. It was introduced by the English mathematician R. B. Potts in 1952. The states of the spins are denoted s = 1, …, q. 
+
+The detial of the Potts model can be found in `Wikipedia <https://en.wikipedia.org/wiki/Potts_model>`__.
+
+Attribute and method are the same as ``Ising``.
+
+``XY``
+~~~~~~
+
+The XY model is a model of a magnet where the spins lie on a plane and interact with each other only through their orientation. It is named after the two-dimensional XY model, but the same name is also used to describe related models in different numbers of dimensions. The XY model  is one of the simplest statistical models exhibiting a phase transition with a continuous symmetry group.
+
+The detial of the XY model can be found in `Wikipedia <https://en.wikipedia.org/wiki/Classical_XY_model>`__.
+
+Attribute and method are the same as ``Ising``.
+
+``mcmc_statphys.algorithm``
+---------------------------
+
+In this subpackage, we have Metropolis algorithm, Wolff algorithm, and Annelaing algorithm.
+
+``Metropolis``
+~~~~~~~~~~~~~~
+
+The Metropolis algorithm, also referred to as the Metropolis Monte Carlo algorithm, is a Monte Carlo method used to generate an approximate probability distribution through a sequence of random samples. The Metropolis algorithm is often used in statistical physics to compute the canonical ensemble and in chemistry to simulate the behavior of atoms in a material.
+
+The detial of the Metropolis algorithm can be found in `Wikipedia <https://en.wikipedia.org/wiki/Metropolis%E2%80%93Hastings_algorithm>`__.
+
+-  attribute
+
+   -  model: ``mcmc_statphys.model``, the model to simulate
+   -  name: ``str``, the name of the algorithm
+   -  data: ``dict``, the data of the iteration(with the unique
+      ``uid`` for each iteration)
+   -  parameter: ``str``, the name of the parameter
+
+-  method
+
+   -  ``iter_sample(self, T: float, uid: str = None) -> str``: 
+      
+      Do one iteration of the algorithm
+      
+      Args: 
+
+      - T: ``float``, the temperature
+      - uid: ``str``, the unique id of the iteration
+      
+      Returns:
+
+      - uid: ``str``, the unique id of the iteration
+   
+   -  ``equil_sample(self, T: float, max_iter: int = 1000, uid: str = None) -> str``:
+      
+      Do the equilibration of the algorithm 
+      
+      Args: 
+
+      - T: ``float``, the temperature of sample 
+      - max_iter: ``int``, the maximum number of iterations (Default: 1000) 
+      - uid: ``str``, the unique id of the iteration
+      
+      Returns:
+
+      - uid: ``str``, the unique id of the iteration
+
+   -  ``param_sample(self, max_iter: int = 1000) -> Dict``: 
+
+      Do the parameter sampling of the algorithm 
+
+      Args:
+
+      - max_iter: ``int``, the maximum number of iterations (Default: 1000) 
+
+      Returns: 
+      
+      - param_data: ``dict``, the data of the parameter sampling
+
+``Wolff``
+~~~~~~~~~
+
+The Wolff algorithm is a Monte Carlo algorithm for generating configurations of an Ising model or Potts model. It was invented by Ulli Wolff in 1989.
+
+The detial of the Wolff algorithm can be found in `Wikipedia <https://en.wikipedia.org/wiki/Wolff_algorithm>`__.
+
+Attribute and method are the same as ``Metropolis``.
+
+``Anneal``
+~~~~~~~~~~
+
+Simulated annealing is a probabilistic technique for approximating the global optimum of a given function. Specifically, it is a metaheuristic to approximate global optimization in a large search space for an optimization problem. It is often used when the search space is discrete (e.g., all tours that visit a given set of cities). For problems where finding an approximate global optimum is more important than finding a precise local optimum in a fixed amount of time, simulated annealing may be preferable to alternatives such as gradient descent.
+
+The detial of the Annelaing algorithm can be found in `Wikipedia <https://en.wikipedia.org/wiki/Simulated_annealing>`__.
+
+Attribute and method are the same as ``Metropolis``, except of ``equil_sample``.
+
+-  method
+   - ``equil_sample(self, targetT: float, max_iter: int = 1000, highT=None, dencyT=0.9, uid: str = None, ) -> str``:
+
+      Do the equilibration of the algorithm 
+      
+      Args: 
+      
+      - targetT: ``float``, the target temperature of sample 
+      - max_iter: ``int``, the maximum number of iterations (Default: 1000) 
+      - highT: ``float``, the high temperature of the annealing (Default: 2 \* targetT) 
+      - dencyT: ``float``, the density of the annealing (Default: 0.9) 
+      - uid: ``str``, the unique id of the iteration 
+      
+      Returns: 
+      
+      - uid: ``str``, the unique id of the iteration
+
+
+In ``algorithm`` subpackage, we also have same analysis method
+
+-  ``mean(uid: str, column: str) -> float``:
+
+   Calculate the mean of the data
+   
+   Args: 
+   
+   - uid: ``str``, the unique id of the iteration
+   - column: ``str``, the name of the column 
+
+   Returns: 
+   
+   - mean: ``float``, the mean of the data
+
+-  ``std(uid: str, column: str) -> float``: 
+   
+   Calculate the standard deviation of the data
+   
+   Args: 
+   
+   - uid: ``str``, the unique id of the iteration
+   - column: ``str``, the name of the column 
+
+   Returns: 
+   
+   - std: ``float``, the standard deviation of the data
+
+-  ``var(uid: str, column: str) -> float``: 
+   
+   Calculate the variance of the data
+   
+   Args: 
+   
+   - uid: ``str``, the unique id of the iteration
+   - column: ``str``, the name of the column 
+
+   Returns: 
+   
+   - var: ``float``, the variance of the data
+
+- ``norm(uid: str, column: str) -> float``: 
+   
+   Calculate the norm of the data
+   
+   Args: 
+   - uid: ``str``, the unique id of the iteration
+   - column: ``str``, the name of the column 
+
+   Returns: 
+   
+   - norm: ``float``, the norm of the data
+
+-  ``cv(uid: str, column: str) -> float``: 
+
+   Calculate the coefficient of variation of the data 
+   
+   Args: 
+   - uid: ``str``, the unique id of the iteration 
+   - column: ``str``, the name of the column
+
+   Returns:
+   
+   - cv: ``float``, the coefficient of variation
+
+-  ``diff(uid: str, column: str) -> float``: 
+   
+   Calculate the difference of the data
+   
+   Args:
+   
+   - uid: ``str``, the unique id of the iteration column: ``str``, the name of the column 
+   
+   Returns: 
+   
+   - diff: ``float``, the difference of the data
+
+-  ``getcolumn(uid: str, column: str) -> numpy.ndarray``:
+
+   Get the column of the data
+   
+   Args:
+   - uid: ``str``, the unique id of the iteration 
+   - column: ``str``, the name of the column 
+
+   Returns:
+   
+   - column: ``numpy.ndarray``, the column of the data
+
+-  ``svd(self, uid: str or Dict or List[str], norm: bool = True) -> np.array:``: 
+   
+   Calculate the singular value decomposition of the data
+   
+   Args: 
+   
+   - uid: ``str`` or ``Dict`` or ``List[str]``, the unique id of the iteration
+   - norm: ``bool``, whether to normalize the data (Default: True)
+
+   Returns: 
+   
+   - svd: ``numpy.ndarray``, the singular value decomposition of the data
+
+``mcmc_statphys.draw``
+----------------------
+
+In this subpackage, we have the draw of the data.
```

### Comparing `mcmc_statphys-0.4.3/mcmc_statphys.egg-info/PKG-INFO` & `mcmc_statphys-1.0.0/mcmc_statphys.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: mcmc-statphys
-Version: 0.4.3
+Version: 1.0.0
 Summary: A library project of Monte Carlo simulation algorithms for some statistical physics models (in particular, the Ising model and its variants).
 Home-page: https://github.com/uynajgi/mcmc_statphys
 Author: Uynaj GI
 Author-email: suquan12148@outlook.com
 License: MIT license
 Keywords: mcmc_statphys
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -49,23 +50,23 @@
 
 A simple Ising model simulation.
 
 .. code-block:: python
 
     >>> import mcmc_statphys as mcsp
     >>> model = mcsp.model.Ising(12) # 12x12 Ising model
-    >>> algorithm = mcsp.method.Metropolis(model) # Metropolis algorithm
+    >>> algorithm = mcsp.algorithm.Metropolis(model) # Metropolis algorithm
     >>> uid = algorithm.equil_sample(T=1, max_iter=1000) # sample until equilibrium
-    >>> fig = mcsp.draw.Plot(algorithm) 
+    >>> fig = mcsp.draw.Plot(algorithm)
     >>> fig.curve(uid=uid, comlumn='energy') # plot the energy curve
 
 Install
 -------
 
-the latest version of mcmc_statphys: 
+the latest version of mcmc_statphys:
 
 .. code-block:: console
 
     $ pip install mcmc_statphys
 
 upgrade to the latest version:
 
@@ -170,7 +171,9 @@
 
 * Add documentation to README
 
 [0.1.1] - 2023-05-14
 --------------------
 
 * First release on PyPI.
+
+
```

### Comparing `mcmc_statphys-0.4.3/setup.cfg` & `mcmc_statphys-1.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [bumpversion]
-current_version = 0.4.3
+current_version = 1.0.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
-search = version='{current_version}'
-replace = version='{new_version}'
+search = version="{current_version}"
+replace = version="{new_version}"
 
 [bumpversion:file:mcmc_statphys/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
 
 [bumpversion:file:docs/conf.py]
 search = version = '{current_version}'
```

### Comparing `mcmc_statphys-0.4.3/tests/test_mcmc_statphys.py` & `mcmc_statphys-1.0.0/tests/test_mcmc_statphys.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-#!/usr/bin/env python
-"""Tests for `mcmc_statphys` package."""
-
-import unittest
-from click.testing import CliRunner
-
-from mcmc_statphys import algorithm
-from mcmc_statphys import model
-from mcmc_statphys import cli
-
-
-class TestMcmc_statphys(unittest.TestCase):
-    """Tests for `mcmc_statphys` package."""
-
-    def setUp(self):
-        """Set up test fixtures, if any."""
-
-    def tearDown(self):
-        """Tear down test fixtures, if any."""
-
-    def test_000_something(self):
-        """Test something."""
-
-    def test_command_line_interface(self):
-        """Test the CLI."""
-        runner = CliRunner()
-        result = runner.invoke(cli.main)
-        assert result.exit_code == 0
-        assert 'mcmc_statphys.cli.main' in result.output
-        help_result = runner.invoke(cli.main, ['--help'])
-        assert help_result.exit_code == 0
-        assert '--help  Show this message and exit.' in help_result.output
+#!/usr/bin/env python
+"""Tests for `mcmc_statphys` package."""
+
+import unittest
+from click.testing import CliRunner
+
+from mcmc_statphys import algorithm
+from mcmc_statphys import model
+from mcmc_statphys import cli
+
+
+class TestMcmc_statphys(unittest.TestCase):
+    """Tests for `mcmc_statphys` package."""
+
+    def setUp(self):
+        """Set up test fixtures, if any."""
+
+    def tearDown(self):
+        """Tear down test fixtures, if any."""
+
+    def test_000_something(self):
+        """Test something."""
+
+    def test_command_line_interface(self):
+        """Test the CLI."""
+        runner = CliRunner()
+        result = runner.invoke(cli.main)
+        assert result.exit_code == 0
+        assert 'mcmc_statphys.cli.main' in result.output
+        help_result = runner.invoke(cli.main, ['--help'])
+        assert help_result.exit_code == 0
+        assert '--help  Show this message and exit.' in help_result.output
```


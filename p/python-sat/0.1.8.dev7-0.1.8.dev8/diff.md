# Comparing `tmp/python-sat-0.1.8.dev7.tar.gz` & `tmp/python-sat-0.1.8.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sat-0.1.8.dev7.tar", last modified: Fri Jun  9 06:06:03 2023, max compression
+gzip compressed data, was "python-sat-0.1.8.dev8.tar", last modified: Wed Jul 12 00:36:48 2023, max compression
```

## Comparing `python-sat-0.1.8.dev7.tar` & `python-sat-0.1.8.dev8.tar`

### file list

```diff
@@ -1,94 +1,96 @@
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.666219 python-sat-0.1.8.dev7/
--rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/LICENSE.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/MANIFEST.in
--rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-06-09 06:06:03.666314 python-sat-0.1.8.dev7/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567    14137 2023-04-21 08:05:23.000000 python-sat-0.1.8.dev7/README.rst
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.634205 python-sat-0.1.8.dev7/allies/
--rw-------   0 aign0002 (892519254) 907548567        0 2023-04-14 00:41:27.000000 python-sat-0.1.8.dev7/allies/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    13572 2023-05-09 14:01:54.000000 python-sat-0.1.8.dev7/allies/approxmc.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.637763 python-sat-0.1.8.dev7/cardenc/
--rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/bitwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev7/cardenc/card.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/clset.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/common.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/itot.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/ladder.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/mto.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/pairwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/ptypes.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/pycard.cc
--rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/seqcounter.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/sortcard.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/cardenc/utils.hh
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.641838 python-sat-0.1.8.dev7/examples/
--rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/examples/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/examples/fm.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev7/examples/genhard.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    25406 2023-06-04 07:07:20.000000 python-sat-0.1.8.dev7/examples/hitman.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/examples/lbx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev7/examples/lsu.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/examples/mcsls.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev7/examples/models.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/examples/musx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    25636 2023-06-04 07:39:47.000000 python-sat-0.1.8.dev7/examples/optux.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    67270 2023-06-09 06:00:18.000000 python-sat-0.1.8.dev7/examples/rc2.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/examples/usage.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.644785 python-sat-0.1.8.dev7/pysat/
--rw-r--r--   0 aign0002 (892519254) 907548567      653 2023-06-09 06:01:09.000000 python-sat-0.1.8.dev7/pysat/__init__.py
--rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/pysat/_fileio.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/pysat/_utils.py
--rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/pysat/card.py
--rw-r--r--   0 aign0002 (892519254) 907548567    95959 2023-05-19 07:25:29.000000 python-sat-0.1.8.dev7/pysat/formula.py
--rw-r--r--   0 aign0002 (892519254) 907548567    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/pysat/pb.py
--rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev7/pysat/process.py
--rw-r--r--   0 aign0002 (892519254) 907548567   175975 2023-06-04 02:20:27.000000 python-sat-0.1.8.dev7/pysat/solvers.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.646113 python-sat-0.1.8.dev7/python_sat.egg-info/
--rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-06-09 06:06:03.000000 python-sat-0.1.8.dev7/python_sat.egg-info/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567     1863 2023-06-09 06:06:03.000000 python-sat-0.1.8.dev7/python_sat.egg-info/SOURCES.txt
--rw-r--r--   0 aign0002 (892519254) 907548567        1 2023-06-09 06:06:03.000000 python-sat-0.1.8.dev7/python_sat.egg-info/dependency_links.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       87 2023-06-09 06:06:03.000000 python-sat-0.1.8.dev7/python_sat.egg-info/requires.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       23 2023-06-09 06:06:03.000000 python-sat-0.1.8.dev7/python_sat.egg-info/top_level.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/requirements.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      107 2023-06-09 06:06:03.666606 python-sat-0.1.8.dev7/setup.cfg
--rw-r--r--   0 aign0002 (892519254) 907548567     6549 2023-04-21 07:47:02.000000 python-sat-0.1.8.dev7/setup.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.656003 python-sat-0.1.8.dev7/solvers/
--rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev7/solvers/cadical103.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev7/solvers/cadical153.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/glucose30.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/glucose41.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/lingeling.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/maplechrono.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/maplecm.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/maplesat.zip
--rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/mergesat3.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/minicard.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/minisat22.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/minisatgh.zip
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.663515 python-sat-0.1.8.dev7/solvers/patches/
--rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev7/solvers/patches/cadical103.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    66092 2023-06-03 01:29:02.000000 python-sat-0.1.8.dev7/solvers/patches/cadical153.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/glucose30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/glucose41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/gluecard30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/gluecard41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/lingeling.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev7/solvers/patches/maplechrono.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev7/solvers/patches/maplecm.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/maplesat.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev7/solvers/patches/mergesat3.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/minicard.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/minisat22.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/solvers/patches/minisatgh.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    25391 2023-06-03 01:04:24.000000 python-sat-0.1.8.dev7/solvers/prepare.py
--rw-r--r--   0 aign0002 (892519254) 907548567   223063 2023-06-04 02:10:25.000000 python-sat-0.1.8.dev7/solvers/pysolvers.cc
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-06-09 06:06:03.665915 python-sat-0.1.8.dev7/tests/
--rw-r--r--   0 aign0002 (892519254) 907548567      948 2023-03-05 08:16:22.000000 python-sat-0.1.8.dev7/tests/test_accum_stats.py
--rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/tests/test_atmost.py
--rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/tests/test_atmost1.py
--rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/tests/test_atmostk.py
--rw-r--r--   0 aign0002 (892519254) 907548567     2408 2023-03-05 08:17:09.000000 python-sat-0.1.8.dev7/tests/test_cnfplus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/tests/test_equals1.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev7/tests/test_process.py
--rw-r--r--   0 aign0002 (892519254) 907548567      866 2023-03-05 08:17:46.000000 python-sat-0.1.8.dev7/tests/test_unique_model.py
--rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev7/tests/test_unique_mus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      643 2023-01-14 22:33:39.000000 python-sat-0.1.8.dev7/tests/test_warmstart.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.163040 python-sat-0.1.8.dev8/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/LICENSE.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/MANIFEST.in
+-rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-07-12 00:36:48.163135 python-sat-0.1.8.dev8/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567    14204 2023-07-12 00:06:38.000000 python-sat-0.1.8.dev8/README.rst
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.131056 python-sat-0.1.8.dev8/allies/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-04-14 00:41:27.000000 python-sat-0.1.8.dev8/allies/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    13572 2023-05-09 14:01:54.000000 python-sat-0.1.8.dev8/allies/approxmc.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.133831 python-sat-0.1.8.dev8/cardenc/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/bitwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev8/cardenc/card.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/clset.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/common.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/itot.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/ladder.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/mto.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/pairwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/ptypes.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/pycard.cc
+-rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/seqcounter.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/sortcard.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/cardenc/utils.hh
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.137786 python-sat-0.1.8.dev8/examples/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/examples/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/examples/fm.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev8/examples/genhard.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    25406 2023-06-04 07:07:20.000000 python-sat-0.1.8.dev8/examples/hitman.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/examples/lbx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev8/examples/lsu.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/examples/mcsls.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev8/examples/models.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/examples/musx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    25636 2023-06-04 07:39:47.000000 python-sat-0.1.8.dev8/examples/optux.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    67270 2023-06-09 06:00:18.000000 python-sat-0.1.8.dev8/examples/rc2.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/examples/usage.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.141240 python-sat-0.1.8.dev8/pysat/
+-rw-r--r--   0 aign0002 (892519254) 907548567      653 2023-07-12 00:28:24.000000 python-sat-0.1.8.dev8/pysat/__init__.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/pysat/_fileio.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/pysat/_utils.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/pysat/card.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    95959 2023-05-19 07:25:29.000000 python-sat-0.1.8.dev8/pysat/formula.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/pysat/pb.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev8/pysat/process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   185523 2023-07-12 00:05:58.000000 python-sat-0.1.8.dev8/pysat/solvers.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.143056 python-sat-0.1.8.dev8/python_sat.egg-info/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1193 2023-07-12 00:36:48.000000 python-sat-0.1.8.dev8/python_sat.egg-info/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567     1922 2023-07-12 00:36:48.000000 python-sat-0.1.8.dev8/python_sat.egg-info/SOURCES.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567        1 2023-07-12 00:36:48.000000 python-sat-0.1.8.dev8/python_sat.egg-info/dependency_links.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       87 2023-07-12 00:36:48.000000 python-sat-0.1.8.dev8/python_sat.egg-info/requires.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       23 2023-07-12 00:36:48.000000 python-sat-0.1.8.dev8/python_sat.egg-info/top_level.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/requirements.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      107 2023-07-12 00:36:48.163496 python-sat-0.1.8.dev8/setup.cfg
+-rw-r--r--   0 aign0002 (892519254) 907548567     6596 2023-07-11 23:32:23.000000 python-sat-0.1.8.dev8/setup.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.153193 python-sat-0.1.8.dev8/solvers/
+-rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev8/solvers/cadical103.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev8/solvers/cadical153.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/glucose30.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/glucose41.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    88105 2023-07-11 23:37:13.000000 python-sat-0.1.8.dev8/solvers/glucose421.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/lingeling.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/maplechrono.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/maplecm.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/maplesat.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/mergesat3.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/minicard.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/minisat22.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/minisatgh.zip
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.160068 python-sat-0.1.8.dev8/solvers/patches/
+-rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev8/solvers/patches/cadical103.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    66092 2023-06-03 01:29:02.000000 python-sat-0.1.8.dev8/solvers/patches/cadical153.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/glucose30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/glucose41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    66579 2023-07-11 23:55:20.000000 python-sat-0.1.8.dev8/solvers/patches/glucose421.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/gluecard30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/gluecard41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/lingeling.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev8/solvers/patches/maplechrono.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev8/solvers/patches/maplecm.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/maplesat.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev8/solvers/patches/mergesat3.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/minicard.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/minisat22.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/solvers/patches/minisatgh.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    25883 2023-07-11 23:55:38.000000 python-sat-0.1.8.dev8/solvers/prepare.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   240042 2023-07-11 23:31:01.000000 python-sat-0.1.8.dev8/solvers/pysolvers.cc
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-07-12 00:36:48.162679 python-sat-0.1.8.dev8/tests/
+-rw-r--r--   0 aign0002 (892519254) 907548567      987 2023-07-12 00:04:49.000000 python-sat-0.1.8.dev8/tests/test_accum_stats.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/tests/test_atmost.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/tests/test_atmost1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/tests/test_atmostk.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     2432 2023-07-12 00:04:57.000000 python-sat-0.1.8.dev8/tests/test_cnfplus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/tests/test_equals1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev8/tests/test_process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      890 2023-07-12 00:05:05.000000 python-sat-0.1.8.dev8/tests/test_unique_model.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev8/tests/test_unique_mus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      650 2023-07-12 00:05:10.000000 python-sat-0.1.8.dev8/tests/test_warmstart.py
```

### Comparing `python-sat-0.1.8.dev7/LICENSE.txt` & `python-sat-0.1.8.dev8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/PKG-INFO` & `python-sat-0.1.8.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev7
+Version: 0.1.8.dev8
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
```

### Comparing `python-sat-0.1.8.dev7/README.rst` & `python-sat-0.1.8.dev8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 Currently, the following SAT solvers are supported (at this point, for
 Minisat-based solvers only *core* versions are integrated):
 
 -  CaDiCaL (`rel-1.0.3 <https://github.com/arminbiere/cadical>`__)
 -  CaDiCaL (`rel-1.5.3 <https://github.com/arminbiere/cadical>`__)
 -  Glucose (`3.0 <http://www.labri.fr/perso/lsimon/glucose/>`__)
 -  Glucose (`4.1 <http://www.labri.fr/perso/lsimon/glucose/>`__)
+-  Glucose (`4.2.1 <http://www.labri.fr/perso/lsimon/glucose/>`__)
 -  Lingeling (`bbc-9230380-160707 <http://fmv.jku.at/lingeling/>`__)
 -  MapleLCMDistChronoBT (`SAT competition 2018 version <http://sat2018.forsyte.tuwien.ac.at/solvers/main_and_glucose_hack/>`__)
 -  MapleCM (`SAT competition 2018 version <http://sat2018.forsyte.tuwien.ac.at/solvers/main_and_glucose_hack/>`__)
 -  Maplesat (`MapleCOMSPS_LRB <https://sites.google.com/a/gsd.uwaterloo.ca/maplesat/>`__)
 -  Mergesat (`3.0 <https://github.com/conp-solutions/mergesat>`__)
 -  Minicard (`1.2 <https://github.com/liffiton/minicard>`__)
 -  Minisat (`2.2 release <http://minisat.se/MiniSat.html>`__)
```

### Comparing `python-sat-0.1.8.dev7/allies/approxmc.py` & `python-sat-0.1.8.dev8/allies/approxmc.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/cardenc/bitwise.hh` & `python-sat-0.1.8.dev8/cardenc/bitwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/cardenc/card.hh` & `python-sat-0.1.8.dev8/cardenc/card.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/cardenc/clset.hh` & `python-sat-0.1.8.dev8/cardenc/clset.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/cardenc/common.hh` & `python-sat-0.1.8.dev8/cardenc/common.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/cardenc/itot.hh` & `python-sat-0.1.8.dev8/cardenc/itot.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/cardenc/ladder.hh` & `python-sat-0.1.8.dev8/cardenc/ladder.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/cardenc/mto.hh` & `python-sat-0.1.8.dev8/cardenc/mto.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/cardenc/pairwise.hh` & `python-sat-0.1.8.dev8/cardenc/pairwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/cardenc/ptypes.hh` & `python-sat-0.1.8.dev8/cardenc/ptypes.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/cardenc/pycard.cc` & `python-sat-0.1.8.dev8/cardenc/pycard.cc`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/cardenc/seqcounter.hh` & `python-sat-0.1.8.dev8/cardenc/seqcounter.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/cardenc/sortcard.hh` & `python-sat-0.1.8.dev8/cardenc/sortcard.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/cardenc/utils.hh` & `python-sat-0.1.8.dev8/cardenc/utils.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/examples/fm.py` & `python-sat-0.1.8.dev8/examples/fm.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/examples/genhard.py` & `python-sat-0.1.8.dev8/examples/genhard.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/examples/hitman.py` & `python-sat-0.1.8.dev8/examples/hitman.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/examples/lbx.py` & `python-sat-0.1.8.dev8/examples/lbx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/examples/lsu.py` & `python-sat-0.1.8.dev8/examples/lsu.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/examples/mcsls.py` & `python-sat-0.1.8.dev8/examples/mcsls.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/examples/models.py` & `python-sat-0.1.8.dev8/examples/models.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/examples/musx.py` & `python-sat-0.1.8.dev8/examples/musx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/examples/optux.py` & `python-sat-0.1.8.dev8/examples/optux.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/examples/rc2.py` & `python-sat-0.1.8.dev8/examples/rc2.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/examples/usage.py` & `python-sat-0.1.8.dev8/examples/usage.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/pysat/_fileio.py` & `python-sat-0.1.8.dev8/pysat/_fileio.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/pysat/_utils.py` & `python-sat-0.1.8.dev8/pysat/_utils.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/pysat/card.py` & `python-sat-0.1.8.dev8/pysat/card.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/pysat/formula.py` & `python-sat-0.1.8.dev8/pysat/formula.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/pysat/pb.py` & `python-sat-0.1.8.dev8/pysat/pb.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/pysat/process.py` & `python-sat-0.1.8.dev8/pysat/process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/pysat/solvers.py` & `python-sat-0.1.8.dev8/pysat/solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         Solver
         Cadical103
         Cadical153
         Gluecard3
         Gluecard4
         Glucose3
         Glucose4
+        Glucose42
         Lingeling
         MapleChrono
         MapleCM
         Maplesat
         Mergesat3
         Minicard
         Minisat22
@@ -39,14 +40,15 @@
 
     This module provides *incremental* access to a few modern SAT solvers. The
     solvers supported by PySAT are:
 
     -  CaDiCaL (`rel-1.0.3 <https://github.com/arminbiere/cadical>`__)
     -  Glucose (`3.0 <http://www.labri.fr/perso/lsimon/glucose/>`__)
     -  Glucose (`4.1 <http://www.labri.fr/perso/lsimon/glucose/>`__)
+    -  Glucose (`4.2.1 <http://www.labri.fr/perso/lsimon/glucose/>`__)
     -  Lingeling (`bbc-9230380-160707 <http://fmv.jku.at/lingeling/>`__)
     -  MapleLCMDistChronoBT (`SAT competition 2018 version <http://sat2018.forsyte.tuwien.ac.at/solvers/main_and_glucose_hack/>`__)
     -  MapleCM (`SAT competition 2018 version <http://sat2018.forsyte.tuwien.ac.at/solvers/main_and_glucose_hack/>`__)
     -  Maplesat (`MapleCOMSPS_LRB <https://sites.google.com/a/gsd.uwaterloo.ca/maplesat/>`__)
     -  Mergesat (`3.0 <https://github.com/conp-solutions/mergesat>`__)
     -  Minicard (`1.2 <https://github.com/liffiton/minicard>`__)
     -  Minisat (`2.2 release <http://minisat.se/MiniSat.html>`__)
@@ -136,19 +138,20 @@
         False
         >>> s.get_core()  # extracting an unsatisfiable core
         [3, 1]
 
     In order to shorten the description of the module, the classes providing
     direct access to the individual solvers, i.e. classes :class:`Cadical103`,
     :class:`Cadical153`, :class:`Gluecard3`, :class:`Gluecard4`,
-    :class:`Glucose3`, :class:`Glucose4`, :class:`Lingeling`,
-    :class:`MapleChrono`, :class:`MapleCM`, :class:`Maplesat`,
-    :class:`Mergesat3`, :class:`Minicard`, :class:`Minisat22`, and
-    :class:`MinisatGH`, are **omitted**. They replicate the interface of
-    the base class :class:`Solver` and, thus, can be used the same exact way.
+    :class:`Glucose3`, :class:`Glucose4`, :class:`Glucose42`,
+    :class:`Lingeling`, :class:`MapleChrono`, :class:`MapleCM`,
+    :class:`Maplesat`, :class:`Mergesat3`, :class:`Minicard`,
+    :class:`Minisat22`, and :class:`MinisatGH`, are **omitted**. They
+    replicate the interface of the base class :class:`Solver` and, thus, can
+    be used the same exact way.
 
     ==============
     Module details
     ==============
 """
 
 #
@@ -168,15 +171,15 @@
 #
 #==============================================================================
 class NoSuchSolverError(Exception):
     """
         This exception is raised when creating a new SAT solver whose name
         does not match any name in :class:`SolverNames`. The list of *known*
         solvers includes the names `'cadical103'`, `'cadical153'`,
-        `'gluecard3'`, `'gluecard4'`, `'glucose3'`, `'glucose4'`,
+        `'gluecard3'`, `'gluecard4'`, `'glucose3'`, `'glucose4'`, `glucose42`,
         `'lingeling'`, `'maplechrono'`, `'maplecm'`, `'maplesat'`,
         `'mergesat3'`, `'minicard'`, `'minisat22'`, and `'minisatgh'`.
     """
 
     pass
 
 
@@ -192,14 +195,15 @@
 
             cadical103  = ('cd', 'cd103', 'cdl', 'cdl103', 'cadical103')
             cadical153  = ('cd15', 'cd153', 'cdl15', 'cdl153', 'cadical153')
             gluecard3   = ('gc3', 'gc30', 'gluecard3', 'gluecard30')
             gluecard41  = ('gc4', 'gc41', 'gluecard4', 'gluecard41')
             glucose3    = ('g3', 'g30', 'glucose3', 'glucose30')
             glucose4    = ('g4', 'g41', 'glucose4', 'glucose41')
+            glucose42   = ('g42', 'g421', 'glucose42', 'glucose421')
             lingeling   = ('lgl', 'lingeling')
             maplechrono = ('mcb', 'chrono', 'maplechrono')
             maplecm     = ('mcm', 'maplecm')
             maplesat    = ('mpl', 'maple', 'maplesat')
             mergesat3   = ('mg3', 'mgs3', 'mergesat3', 'mergesat30')
             minicard    = ('mc', 'mcard', 'minicard')
             minisat22   = ('m22', 'msat22', 'minisat22')
@@ -213,14 +217,15 @@
 
     cadical103  = ('cd', 'cd103', 'cdl', 'cdl103', 'cadical103')
     cadical153  = ('cd15', 'cd153', 'cdl15', 'cdl153', 'cadical153')
     gluecard3   = ('gc3', 'gc30', 'gluecard3', 'gluecard30')
     gluecard4   = ('gc4', 'gc41', 'gluecard4', 'gluecard41')
     glucose3    = ('g3', 'g30', 'glucose3', 'glucose30')
     glucose4    = ('g4', 'g41', 'glucose4', 'glucose41')
+    glucose42   = ('g42', 'g421', 'glucose42', 'glucose421')
     lingeling   = ('lgl', 'lingeling')
     maplechrono = ('mcb', 'chrono', 'chronobt', 'maplechrono')
     maplecm     = ('mcm', 'maplecm')
     maplesat    = ('mpl', 'maple', 'maplesat')
     mergesat3   = ('mg3', 'mgs3', 'mergesat3', 'mergesat30')
     minicard    = ('mc', 'mcard', 'minicard')
     minisat22   = ('m22', 'msat22', 'minisat22')
@@ -283,17 +288,17 @@
             ...     print(m.get_model())
             [-1, -2]
 
         Note that while all explicit solver classes necessarily have default
         arguments ``bootstrap_with`` and ``use_timer``, solvers
         :class:`Cadical103`, :class:`Cadical153`, :class:`Lingeling`,
         :class:`Gluecard3`, :class:`Gluecard4`, :class:`Glucose3`,
-        :class:`Glucose4`, :class:`MapleChrono`, :class:`MapleCM`, and
-        :class:`Maplesat` can have additional default arguments. One such
-        argument supported by is `DRUP proof
+        :class:`Glucose4`, :class:`Glucose42`, :class:`MapleChrono`,
+        :class:`MapleCM`, and :class:`Maplesat` can have additional default
+        arguments. One such argument supported by is `DRUP proof
         <http://www.cs.utexas.edu/~marijn/drup/>`__ logging. This can be
         enabled by setting the ``with_proof`` argument to ``True`` (``False``
         by default):
 
         .. code-block:: python
 
             >>> from pysat.solvers import Lingeling
@@ -304,18 +309,18 @@
             >>> with Lingeling(bootstrap_with=cnf.clauses, with_proof=True) as l:
             ...     l.solve()
             False
             ...     l.get_proof()
             ['-5 0', '6 0', '-2 0', '-4 0', '1 0', '3 0', '0']
 
         Additionally, Glucose-based solvers, namely :class:`Glucose3`,
-        :class:`Glucose4`, :class:`Gluecard3`, and :class:`Gluecard4` have one
-        more default argument ``incr`` (``False`` by default), which enables
-        incrementality features introduced in Glucose3 [3]_. To summarize, the
-        additional arguments of Glucose are:
+        :class:`Glucose4`, :class:`Glucose42`, :class:`Gluecard3`, and
+        :class:`Gluecard4` have one more default argument ``incr`` (``False``
+        by default), which enables incrementality features introduced in
+        Glucose3 [3]_. To summarize, the additional arguments of Glucose are:
 
         :param incr: enable the incrementality features of Glucose3 [3]_.
         :param with_proof: enable proof logging in the `DRUP format <http://www.cs.utexas.edu/~marijn/drup/>`__.
 
         :type incr: bool
         :type with_proof: bool
 
@@ -384,14 +389,16 @@
                 self.solver = Gluecard3(bootstrap_with, use_timer, **kwargs)
             elif name_ in SolverNames.gluecard4:
                 self.solver = Gluecard4(bootstrap_with, use_timer, **kwargs)
             elif name_ in SolverNames.glucose3:
                 self.solver = Glucose3(bootstrap_with, use_timer, **kwargs)
             elif name_ in SolverNames.glucose4:
                 self.solver = Glucose4(bootstrap_with, use_timer, **kwargs)
+            elif name_ in SolverNames.glucose42:
+                self.solver = Glucose42(bootstrap_with, use_timer, **kwargs)
             elif name_ in SolverNames.lingeling:
                 self.solver = Lingeling(bootstrap_with, use_timer, **kwargs)
             elif name_ in SolverNames.maplechrono:
                 self.solver = MapleChrono(bootstrap_with, use_timer, **kwargs)
             elif name_ in SolverNames.maplecm:
                 self.solver = MapleCM(bootstrap_with, use_timer, **kwargs)
             elif name_ in SolverNames.maplesat:
@@ -3290,14 +3297,346 @@
         """
 
         return False
 
 
 #
 #==============================================================================
+class Glucose42(object):
+    """
+        Glucose 4.2.1 SAT solver.
+    """
+
+    def __init__(self, bootstrap_with=None, use_timer=False, incr=False,
+            with_proof=False, warm_start=False):
+        """
+            Basic constructor.
+        """
+
+        self.glucose = None
+        self.status = None
+        self.prfile = None
+
+        self.new(bootstrap_with, use_timer, incr, with_proof, warm_start)
+
+    def __enter__(self):
+        """
+            'with' constructor.
+        """
+
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        """
+            'with' destructor.
+        """
+
+        self.delete()
+        self.glucose = None
+
+    def new(self, bootstrap_with=None, use_timer=False, incr=False,
+            with_proof=False, warm_start=False):
+        """
+            Actual constructor of the solver.
+        """
+
+        assert not incr or not with_proof, 'Incremental mode and proof tracing cannot be set together.'
+
+        if not self.glucose:
+            self.glucose = pysolvers.glucose421_new()
+
+            if bootstrap_with:
+                if type(bootstrap_with) == CNFPlus and bootstrap_with.atmosts:
+                    raise NotImplementedError('Atmost constraints are not supported by Glucose4')
+
+                for clause in bootstrap_with:
+                    self.add_clause(clause)
+
+            self.use_timer = use_timer
+            self.call_time = 0.0  # time spent for the last call to oracle
+            self.accu_time = 0.0  # time accumulated for all calls to oracle
+
+            if incr:
+                pysolvers.glucose421_setincr(self.glucose)
+
+            if with_proof:
+                self.prfile = tempfile.TemporaryFile()
+                pysolvers.glucose421_tracepr(self.glucose, self.prfile)
+
+            if warm_start:
+                self.start_mode(warm=True)
+
+    def start_mode(self, warm=False):
+        """
+            Set start mode: either warm or standard.
+        """
+
+        if self.glucose:
+            pysolvers.glucose421_set_start(self.glucose, int(warm))
+
+    def delete(self):
+        """
+            Destructor.
+        """
+
+        if self.glucose:
+            pysolvers.glucose421_del(self.glucose)
+            self.glucose = None
+
+            if self.prfile:
+                self.prfile.close()
+
+    def solve(self, assumptions=[]):
+        """
+            Solve internal formula.
+        """
+
+        if self.glucose:
+            if self.use_timer:
+                 start_time = process_time()
+
+            self.status = pysolvers.glucose421_solve(self.glucose, assumptions,
+                    int(MainThread.check()))
+
+            if self.use_timer:
+                self.call_time = process_time() - start_time
+                self.accu_time += self.call_time
+
+            return self.status
+
+    def solve_limited(self, assumptions=[], expect_interrupt=False):
+        """
+            Solve internal formula using given budgets for conflicts and
+            propagations.
+        """
+
+        if self.glucose:
+            if self.use_timer:
+                 start_time = process_time()
+
+            self.status = pysolvers.glucose421_solve_lim(self.glucose,
+                    assumptions, int(MainThread.check()), int(expect_interrupt))
+
+            if self.use_timer:
+                self.call_time = process_time() - start_time
+                self.accu_time += self.call_time
+
+            return self.status
+
+    def conf_budget(self, budget):
+        """
+            Set limit on the number of conflicts.
+        """
+
+        if self.glucose:
+            pysolvers.glucose421_cbudget(self.glucose, budget)
+
+    def prop_budget(self, budget):
+        """
+            Set limit on the number of propagations.
+        """
+
+        if self.glucose:
+            pysolvers.glucose421_pbudget(self.glucose, budget)
+
+    def dec_budget(self, budget):
+        """
+            Set limit on the number of decisions.
+        """
+
+        raise NotImplementedError('Limit on decisions is unsupported by Glucose4.')
+
+    def interrupt(self):
+        """
+            Interrupt solver execution.
+        """
+
+        if self.glucose:
+            pysolvers.glucose421_interrupt(self.glucose)
+
+    def clear_interrupt(self):
+        """
+            Clears an interruption.
+        """
+
+        if self.glucose:
+            pysolvers.glucose421_clearint(self.glucose)
+
+    def propagate(self, assumptions=[], phase_saving=0):
+        """
+            Propagate a given set of assumption literals.
+        """
+
+        if self.glucose:
+            if self.use_timer:
+                 start_time = process_time()
+
+            st, props = pysolvers.glucose421_propagate(self.glucose,
+                    assumptions, phase_saving, int(MainThread.check()))
+
+            if self.use_timer:
+                self.call_time = process_time() - start_time
+                self.accu_time += self.call_time
+
+            return bool(st), props if props != None else []
+
+    def set_phases(self, literals=[]):
+        """
+            Sets polarities of a given list of variables.
+        """
+
+        if self.glucose:
+            pysolvers.glucose421_setphases(self.glucose, literals)
+
+    def get_status(self):
+        """
+            Returns solver's status.
+        """
+
+        if self.glucose:
+            return self.status
+
+    def get_model(self):
+        """
+            Get a model if the formula was previously satisfied.
+        """
+
+        if self.glucose and self.status == True:
+            model = pysolvers.glucose421_model(self.glucose)
+            return model if model != None else []
+
+    def get_core(self):
+        """
+            Get an unsatisfiable core if the formula was previously
+            unsatisfied.
+        """
+
+        if self.glucose and self.status == False:
+            return pysolvers.glucose421_core(self.glucose)
+
+    def get_proof(self):
+        """
+            Get a proof produced when deciding the formula.
+        """
+
+        if self.glucose and self.prfile:
+            self.prfile.seek(0)
+            return [line.rstrip().decode('ascii') for line in self.prfile.readlines()]
+
+    def time(self):
+        """
+            Get time spent for the last call to oracle.
+        """
+
+        if self.glucose:
+            return self.call_time
+
+    def time_accum(self):
+        """
+            Get time accumulated for all calls to oracle.
+        """
+
+        if self.glucose:
+            return self.accu_time
+
+    def nof_vars(self):
+        """
+            Get number of variables currently used by the solver.
+        """
+
+        if self.glucose:
+            return pysolvers.glucose421_nof_vars(self.glucose)
+
+    def nof_clauses(self):
+        """
+            Get number of clauses currently used by the solver.
+        """
+
+        if self.glucose:
+            return pysolvers.glucose421_nof_cls(self.glucose)
+
+    def accum_stats(self):
+        """
+            Get accumulated low-level stats from the solver. This includes
+            the number of restarts, conflicts, decisions and propagations.
+        """
+
+        if self.glucose:
+            return pysolvers.glucose421_acc_stats(self.glucose)
+
+    def enum_models(self, assumptions=[]):
+        """
+            Iterate over models of the internal formula.
+        """
+
+        if self.glucose:
+            done = False
+            while not done:
+                self.status = self.solve(assumptions=assumptions)
+                model = self.get_model()
+
+                if model is not None:
+                    self.add_clause([-l for l in model])  # blocking model
+                    yield model
+                else:
+                    done = True
+
+    def add_clause(self, clause, no_return=True):
+        """
+            Add a new clause to solver's internal formula.
+        """
+
+        if self.glucose:
+            res = pysolvers.glucose421_add_cl(self.glucose, clause)
+
+            if res == False:
+                self.status = False
+
+            if not no_return:
+                return res
+
+    def add_atmost(self, lits, k, no_return=True):
+        """
+            Atmost constraints are not supported by Glucose.
+        """
+
+        raise NotImplementedError('Atmost constraints are not supported by Glucose.')
+
+    def append_formula(self, formula, no_return=True):
+        """
+            Appends list of clauses to solver's internal formula.
+        """
+
+        if self.glucose:
+            res = None
+
+            if type(formula) == CNFPlus and formula.atmosts:
+                raise NotImplementedError('Atmost constraints are not supported by Glucose4')
+
+            for clause in formula:
+                res = self.add_clause(clause, no_return)
+
+                if not no_return and res == False:
+                    return res
+
+            if not no_return:
+                return res
+
+    def supports_atmost(self):
+        """
+            This method can be called to determine whether the solver supports
+            native AtMostK (see :mod:`pysat.card`) constraints.
+        """
+
+        return False
+
+
+
+#
+#==============================================================================
 class Lingeling(object):
     """
         Lingeling SAT solver.
     """
 
     def __init__(self, bootstrap_with=None, use_timer=False, incr=False,
             with_proof=False, warm_start=False):
```

### Comparing `python-sat-0.1.8.dev7/python_sat.egg-info/PKG-INFO` & `python-sat-0.1.8.dev8/python_sat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev7
+Version: 0.1.8.dev8
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
```

### Comparing `python-sat-0.1.8.dev7/python_sat.egg-info/SOURCES.txt` & `python-sat-0.1.8.dev8/python_sat.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,28 +44,30 @@
 python_sat.egg-info/dependency_links.txt
 python_sat.egg-info/requires.txt
 python_sat.egg-info/top_level.txt
 solvers/cadical103.tar.gz
 solvers/cadical153.tar.gz
 solvers/glucose30.tar.gz
 solvers/glucose41.tar.gz
+solvers/glucose421.tar.gz
 solvers/lingeling.tar.gz
 solvers/maplechrono.zip
 solvers/maplecm.zip
 solvers/maplesat.zip
 solvers/mergesat3.tar.gz
 solvers/minicard.tar.gz
 solvers/minisat22.tar.gz
 solvers/minisatgh.zip
 solvers/prepare.py
 solvers/pysolvers.cc
 solvers/patches/cadical103.patch
 solvers/patches/cadical153.patch
 solvers/patches/glucose30.patch
 solvers/patches/glucose41.patch
+solvers/patches/glucose421.patch
 solvers/patches/gluecard30.patch
 solvers/patches/gluecard41.patch
 solvers/patches/lingeling.patch
 solvers/patches/maplechrono.patch
 solvers/patches/maplecm.patch
 solvers/patches/maplesat.patch
 solvers/patches/mergesat3.patch
```

### Comparing `python-sat-0.1.8.dev7/setup.py` & `python-sat-0.1.8.dev8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 Details can be found at `https://pysathq.github.io <https://pysathq.github.io>`__.
 """
 
 
 # solvers to install
 #==============================================================================
 to_install = ['cadical103', 'cadical153', 'gluecard30', 'gluecard41',
-              'glucose30', 'glucose41', 'lingeling', 'maplechrono', 'maplecm',
+              'glucose30', 'glucose41', 'glucose421', 'lingeling', 'maplechrono', 'maplecm',
               'maplesat', 'mergesat3', 'minicard', 'minisat22', 'minisatgh']
 
 # example and allies scripts to install as standalone executables
 #==============================================================================
 example_scripts = ['fm', 'genhard', 'lbx', 'lsu', 'mcsls', 'models', 'musx',
                    'optux', 'rc2']
 allies_scripts = ['approxmc']
@@ -180,15 +180,16 @@
     license='MIT',
     author='Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado',
     author_email='alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com',
     url='https://github.com/pysathq/pysat',
     ext_modules=[pycard_ext, pysolvers_ext],
     scripts=['examples/{0}.py'.format(s) for s in example_scripts] + \
             ['allies/{0}.py'.format(s) for s in allies_scripts],
-    cmdclass={'build': build, 'build_ext': build_ext},
+    cmdclass={'build': build},
+    # cmdclass={'build': build, 'build_ext': build_ext},
     install_requires=['six'],
     extras_require = {
         'aiger': ['py-aiger-cnf>=2.0.0'],
         'approxmc': ['pyapproxmc>=4.1.8'],
         'pblib': ['pypblib>=0.0.3']
     }
 )
```

### Comparing `python-sat-0.1.8.dev7/solvers/cadical103.tar.gz` & `python-sat-0.1.8.dev8/solvers/cadical103.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/cadical153.tar.gz` & `python-sat-0.1.8.dev8/solvers/cadical153.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/glucose30.tar.gz` & `python-sat-0.1.8.dev8/solvers/glucose30.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/glucose41.tar.gz` & `python-sat-0.1.8.dev8/solvers/glucose41.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/lingeling.tar.gz` & `python-sat-0.1.8.dev8/solvers/lingeling.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/maplechrono.zip` & `python-sat-0.1.8.dev8/solvers/maplechrono.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/maplecm.zip` & `python-sat-0.1.8.dev8/solvers/maplecm.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/maplesat.zip` & `python-sat-0.1.8.dev8/solvers/maplesat.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/mergesat3.tar.gz` & `python-sat-0.1.8.dev8/solvers/mergesat3.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/minicard.tar.gz` & `python-sat-0.1.8.dev8/solvers/minicard.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/minisat22.tar.gz` & `python-sat-0.1.8.dev8/solvers/minisat22.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/minisatgh.zip` & `python-sat-0.1.8.dev8/solvers/minisatgh.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/cadical103.patch` & `python-sat-0.1.8.dev8/solvers/patches/cadical103.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/cadical153.patch` & `python-sat-0.1.8.dev8/solvers/patches/cadical153.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/glucose30.patch` & `python-sat-0.1.8.dev8/solvers/patches/glucose30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/glucose41.patch` & `python-sat-0.1.8.dev8/solvers/patches/glucose41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/gluecard30.patch` & `python-sat-0.1.8.dev8/solvers/patches/gluecard30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/gluecard41.patch` & `python-sat-0.1.8.dev8/solvers/patches/gluecard41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/lingeling.patch` & `python-sat-0.1.8.dev8/solvers/patches/lingeling.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/maplechrono.patch` & `python-sat-0.1.8.dev8/solvers/patches/maplechrono.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/maplecm.patch` & `python-sat-0.1.8.dev8/solvers/patches/maplecm.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/maplesat.patch` & `python-sat-0.1.8.dev8/solvers/patches/maplesat.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/mergesat3.patch` & `python-sat-0.1.8.dev8/solvers/patches/mergesat3.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/minicard.patch` & `python-sat-0.1.8.dev8/solvers/patches/minicard.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/minisat22.patch` & `python-sat-0.1.8.dev8/solvers/patches/minisat22.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/patches/minisatgh.patch` & `python-sat-0.1.8.dev8/solvers/patches/minisatgh.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/solvers/prepare.py` & `python-sat-0.1.8.dev8/solvers/prepare.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,18 @@
         'http://www.labri.fr/perso/lsimon/downloads/softwares/glucose-3.0.tgz',
         'solvers/glucose30.tar.gz'
     ),
     'glucose41': (
         'http://www.labri.fr/perso/lsimon/downloads/softwares/glucose-syrup-4.1.tgz',
         'solvers/glucose41.tar.gz'
     ),
+    'glucose421': (
+        'https://github.com/audemard/glucose/archive/refs/tags/4.2.1.tar.gz',
+        'solvers/glucose421.tar.gz'
+    ),
     'lingeling': (
         'http://fmv.jku.at/lingeling/lingeling-bbc-9230380-160707-druplig-009.tar.gz',
         'solvers/lingeling.tar.gz'
     ),
     'maplechrono': (
         'http://sat2018.forsyte.tuwien.ac.at/solvers/main_and_glucose_hack/MapleLCMDistChronoBT.zip',
         'solvers/maplechrono.zip'
@@ -93,14 +97,15 @@
 to_extract = {
     'cadical103': [],
     'cadical153': [],
     'gluecard30': [],
     'gluecard41': [],
     'glucose30': [],
     'glucose41': [],
+    'glucose421': [],
     'lingeling': ['druplig-009.zip', 'lingeling-bbc-9230380-160707.tar.gz'],
     'maplechrono': [],
     'maplecm': [],
     'maplesat': [],
     'mergesat3': [],
     'minicard': [],
     'minisat22': [],
@@ -354,14 +359,15 @@
         ('src/watch.hpp', 'watch.hpp'),
         ('VERSION', 'VERSION.txt')
     ],
     'gluecard30': [],
     'gluecard41': [],
     'glucose30': [],
     'glucose41': [],
+    'glucose421': [],
     'lingeling': [
         ('druplig-009/druplig.c', 'druplig.c'),
         ('druplig-009/druplig.h', 'druplig.h'),
         ('lingeling-bbc-9230380-160707/lglconst.h', 'lglconst.h'),
         ('lingeling-bbc-9230380-160707/lglib.c', 'lglib.c'),
         ('lingeling-bbc-9230380-160707/lglib.h', 'lglib.h'),
         ('lingeling-bbc-9230380-160707/lgloptl.h', 'lgloptl.h'),
@@ -536,14 +542,28 @@
         'utils/._Options.cc',
         'utils/._Options.h',
         'utils/._ParseUtils.h',
         'utils/._System.cc',
         'utils/._System.h',
         'utils/Makefile'
     ],
+    'glucose421': [
+        'CHANGELOG',
+        'CMakeLists.txt',
+        '.gitignore',
+        'LICENSE',
+        'README.md',
+        'simp',
+        'parallel',
+        'mtl/template.mk',
+        'mtl/config.mk',
+        'core/Dimacs.h',
+        'core/Makefile',
+        'utils/Makefile'
+    ],
     'lingeling': [
         'druplig-009',
         'druplig-009.zip',
         'lingeling-bbc-9230380-160707',
         'lingeling-bbc-9230380-160707.tar.gz',
         'extract-and-compile.sh',
         '.tar.gz',
@@ -658,15 +678,15 @@
     for solver in to_install:
         print('preparing {0}'.format(solver))
 
         download_archive(sources[solver])
         extract_archive(sources[solver][-1], solver)
         adapt_files(solver)
         patch_solver(solver)
-
+        
         if platform.system() != 'Windows':
             compile_solver(solver)
 
 #
 #==============================================================================
 def download_archive(sources):
     """
```

### Comparing `python-sat-0.1.8.dev7/solvers/pysolvers.cc` & `python-sat-0.1.8.dev8/solvers/pysolvers.cc`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,18 @@
 #include "glucose30/core/Solver.h"
 #endif
 
 #ifdef WITH_GLUCOSE41
 #include "glucose41/core/Solver.h"
 #endif
 
+#ifdef WITH_GLUCOSE421
+#include "glucose421/core/Solver.h"
+#endif
+
 #ifdef WITH_LINGELING
 #include "lingeling/lglib.h"
 #endif
 
 #ifdef WITH_MAPLECHRONO
 #include "maplechrono/core/Solver.h"
 #endif
@@ -232,14 +236,35 @@
 	static PyObject *py_glucose41_core      (PyObject *, PyObject *);
 	static PyObject *py_glucose41_model     (PyObject *, PyObject *);
 	static PyObject *py_glucose41_nof_vars  (PyObject *, PyObject *);
 	static PyObject *py_glucose41_nof_cls   (PyObject *, PyObject *);
 	static PyObject *py_glucose41_del       (PyObject *, PyObject *);
 	static PyObject *py_glucose41_acc_stats (PyObject *, PyObject *);
 #endif
+#ifdef WITH_GLUCOSE421
+	static PyObject *py_glucose421_new       (PyObject *, PyObject *);
+	static PyObject *py_glucose421_set_start (PyObject *, PyObject *);
+	static PyObject *py_glucose421_add_cl    (PyObject *, PyObject *);
+	static PyObject *py_glucose421_solve     (PyObject *, PyObject *);
+	static PyObject *py_glucose421_solve_lim (PyObject *, PyObject *);
+	static PyObject *py_glucose421_propagate (PyObject *, PyObject *);
+	static PyObject *py_glucose421_setphases (PyObject *, PyObject *);
+	static PyObject *py_glucose421_cbudget   (PyObject *, PyObject *);
+	static PyObject *py_glucose421_pbudget   (PyObject *, PyObject *);
+	static PyObject *py_glucose421_interrupt (PyObject *, PyObject *);
+	static PyObject *py_glucose421_clearint  (PyObject *, PyObject *);
+	static PyObject *py_glucose421_setincr   (PyObject *, PyObject *);
+	static PyObject *py_glucose421_tracepr   (PyObject *, PyObject *);
+	static PyObject *py_glucose421_core      (PyObject *, PyObject *);
+	static PyObject *py_glucose421_model     (PyObject *, PyObject *);
+	static PyObject *py_glucose421_nof_vars  (PyObject *, PyObject *);
+	static PyObject *py_glucose421_nof_cls   (PyObject *, PyObject *);
+	static PyObject *py_glucose421_del       (PyObject *, PyObject *);
+	static PyObject *py_glucose421_acc_stats (PyObject *, PyObject *);
+#endif
 #ifdef WITH_LINGELING
 	static PyObject *py_lingeling_new       (PyObject *, PyObject *);
 	static PyObject *py_lingeling_add_cl    (PyObject *, PyObject *);
 	static PyObject *py_lingeling_solve     (PyObject *, PyObject *);
 	static PyObject *py_lingeling_setphases (PyObject *, PyObject *);
 	static PyObject *py_lingeling_tracepr   (PyObject *, PyObject *);
 	static PyObject *py_lingeling_core      (PyObject *, PyObject *);
@@ -505,14 +530,35 @@
 	{ "glucose41_core",      py_glucose41_core,      METH_VARARGS,      core_docstring },
 	{ "glucose41_model",     py_glucose41_model,     METH_VARARGS,     model_docstring },
 	{ "glucose41_nof_vars",  py_glucose41_nof_vars,  METH_VARARGS,     nvars_docstring },
 	{ "glucose41_nof_cls",   py_glucose41_nof_cls,   METH_VARARGS,      ncls_docstring },
 	{ "glucose41_del",       py_glucose41_del,       METH_VARARGS,       del_docstring },
 	{ "glucose41_acc_stats", py_glucose41_acc_stats, METH_VARARGS,  acc_stat_docstring },
 #endif
+#ifdef WITH_GLUCOSE421
+	{ "glucose421_new",       py_glucose421_new,       METH_VARARGS,       new_docstring },
+	{ "glucose421_set_start", py_glucose421_set_start, METH_VARARGS,  setstart_docstring },
+	{ "glucose421_add_cl",    py_glucose421_add_cl,    METH_VARARGS,     addcl_docstring },
+	{ "glucose421_solve",     py_glucose421_solve,     METH_VARARGS,     solve_docstring },
+	{ "glucose421_solve_lim", py_glucose421_solve_lim, METH_VARARGS,       lim_docstring },
+	{ "glucose421_propagate", py_glucose421_propagate, METH_VARARGS,      prop_docstring },
+	{ "glucose421_setphases", py_glucose421_setphases, METH_VARARGS,    phases_docstring },
+	{ "glucose421_cbudget",   py_glucose421_cbudget,   METH_VARARGS,   cbudget_docstring },
+	{ "glucose421_pbudget",   py_glucose421_pbudget,   METH_VARARGS,   pbudget_docstring },
+	{ "glucose421_interrupt", py_glucose421_interrupt, METH_VARARGS, interrupt_docstring },
+	{ "glucose421_clearint",  py_glucose421_clearint,  METH_VARARGS,  clearint_docstring },
+	{ "glucose421_setincr",   py_glucose421_setincr,   METH_VARARGS,   setincr_docstring },
+	{ "glucose421_tracepr",   py_glucose421_tracepr,   METH_VARARGS,   tracepr_docstring },
+	{ "glucose421_core",      py_glucose421_core,      METH_VARARGS,      core_docstring },
+	{ "glucose421_model",     py_glucose421_model,     METH_VARARGS,     model_docstring },
+	{ "glucose421_nof_vars",  py_glucose421_nof_vars,  METH_VARARGS,     nvars_docstring },
+	{ "glucose421_nof_cls",   py_glucose421_nof_cls,   METH_VARARGS,      ncls_docstring },
+	{ "glucose421_del",       py_glucose421_del,       METH_VARARGS,       del_docstring },
+	{ "glucose421_acc_stats", py_glucose421_acc_stats, METH_VARARGS,  acc_stat_docstring },
+#endif
 #ifdef WITH_LINGELING
 	{ "lingeling_new",       py_lingeling_new,       METH_VARARGS,      new_docstring },
 	{ "lingeling_add_cl",    py_lingeling_add_cl,    METH_VARARGS,    addcl_docstring },
 	{ "lingeling_solve",     py_lingeling_solve,     METH_VARARGS,    solve_docstring },
 	{ "lingeling_setphases", py_lingeling_setphases, METH_VARARGS,   phases_docstring },
 	{ "lingeling_tracepr",   py_lingeling_tracepr,   METH_VARARGS,  tracepr_docstring },
 	{ "lingeling_core",      py_lingeling_core,      METH_VARARGS,     core_docstring },
@@ -4212,14 +4258,588 @@
 		"conflicts", (Py_ssize_t)s->conflicts,
 		"decisions", (Py_ssize_t)s->decisions,
 		"propagations", (Py_ssize_t)s->propagations
 	);
 }
 #endif  // WITH_GLUCOSE41
 
+
+// API for Glucose 4.1
+//=============================================================================
+#ifdef WITH_GLUCOSE421
+static PyObject *py_glucose421_new(PyObject *self, PyObject *args)
+{
+	Glucose421::Solver *s = new Glucose421::Solver();
+
+	if (s == NULL) {
+		PyErr_SetString(PyExc_RuntimeError,
+				"Cannot create a new solver.");
+		return NULL;
+	}
+
+	return void_to_pyobj((void *)s);
+}
+
+// auxiliary function for declaring new variables
+//=============================================================================
+static inline void glucose421_declare_vars(Glucose421::Solver *s, const int max_id)
+{
+	while (s->nVars() < max_id + 1)
+		s->newVar();
+}
+
+// translating an iterable to vec<Lit>
+//=============================================================================
+static inline bool glucose421_iterate(
+	PyObject *obj,
+	Glucose421::vec<Glucose421::Lit>& v,
+	int& max_var
+)
+{
+	// iterator object
+	PyObject *i_obj = PyObject_GetIter(obj);
+	if (i_obj == NULL) {
+		PyErr_SetString(PyExc_RuntimeError,
+				"Object does not seem to be an iterable.");
+		return false;
+	}
+
+	PyObject *l_obj;
+	while ((l_obj = PyIter_Next(i_obj)) != NULL) {
+		if (!pyint_check(l_obj)) {
+			Py_DECREF(l_obj);
+			Py_DECREF(i_obj);
+			PyErr_SetString(PyExc_TypeError, "integer expected");
+			return false;
+		}
+
+		int l = pyint_to_cint(l_obj);
+		Py_DECREF(l_obj);
+
+		if (l == 0) {
+			Py_DECREF(i_obj);
+			PyErr_SetString(PyExc_ValueError, "non-zero integer expected");
+			return false;
+		}
+
+		v.push((l > 0) ? Glucose421::mkLit(l, false) : Glucose421::mkLit(-l, true));
+
+		if (abs(l) > max_var)
+			max_var = abs(l);
+	}
+
+	Py_DECREF(i_obj);
+	return true;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_set_start(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	int warm_start;
+
+	if (!PyArg_ParseTuple(args, "Oi", &s_obj, &warm_start))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+
+	s->setStartMode((bool)warm_start);
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_add_cl(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	PyObject *c_obj;
+
+	if (!PyArg_ParseTuple(args, "OO", &s_obj, &c_obj))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+	Glucose421::vec<Glucose421::Lit> cl;
+	int max_var = -1;
+
+	if (glucose421_iterate(c_obj, cl, max_var) == false)
+		return NULL;
+
+	if (max_var > 0)
+		glucose421_declare_vars(s, max_var);
+
+	bool res = s->addClause(cl);
+
+	PyObject *ret = PyBool_FromLong((long)res);
+	return ret;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_solve(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	PyObject *a_obj;  // assumptions
+	int main_thread;
+
+	if (!PyArg_ParseTuple(args, "OOi", &s_obj, &a_obj, &main_thread))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+	Glucose421::vec<Glucose421::Lit> a;
+	int max_var = -1;
+
+	if (glucose421_iterate(a_obj, a, max_var) == false)
+		return NULL;
+
+	if (max_var > 0)
+		glucose421_declare_vars(s, max_var);
+
+	PyOS_sighandler_t sig_save;
+	if (main_thread) {
+		sig_save = PyOS_setsig(SIGINT, sigint_handler);
+
+		if (setjmp(env) != 0) {
+			PyErr_SetString(SATError, "Caught keyboard interrupt");
+			return NULL;
+		}
+	}
+
+	bool res = s->solve(a);
+
+	if (main_thread)
+		PyOS_setsig(SIGINT, sig_save);
+
+	PyObject *ret = PyBool_FromLong((long)res);
+	return ret;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_solve_lim(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	PyObject *a_obj;  // assumptions
+	int main_thread;
+	int expect_interrupt;
+
+	if (!PyArg_ParseTuple(args, "OOii", &s_obj, &a_obj, &main_thread,
+				&expect_interrupt))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+	Glucose421::vec<Glucose421::Lit> a;
+	int max_var = -1;
+
+	if (glucose421_iterate(a_obj, a, max_var) == false)
+		return NULL;
+
+	if (max_var > 0)
+		glucose421_declare_vars(s, max_var);
+
+	Glucose421::lbool res = Glucose421::lbool((uint8_t)2);  // l_Undef
+	if (expect_interrupt == 0) {
+		PyOS_sighandler_t sig_save;
+		if (main_thread) {
+			sig_save = PyOS_setsig(SIGINT, sigint_handler);
+
+			if (setjmp(env) != 0) {
+				PyErr_SetString(SATError, "Caught keyboard interrupt");
+				return NULL;
+			}
+		}
+
+		res = s->solveLimited(a);
+
+		if (main_thread)
+			PyOS_setsig(SIGINT, sig_save);
+	}
+	else {
+		Py_BEGIN_ALLOW_THREADS
+		res = s->solveLimited(a);
+		Py_END_ALLOW_THREADS
+	}
+
+	if (res != Glucose421::lbool((uint8_t)2))  // l_Undef
+		return PyBool_FromLong((long)!(Glucose421::toInt(res)));
+
+	Py_RETURN_NONE; // return Python's None if l_Undef
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_propagate(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	PyObject *a_obj;  // assumptions
+	int save_phases;
+	int main_thread;
+
+	if (!PyArg_ParseTuple(args, "OOii", &s_obj, &a_obj, &save_phases,
+				&main_thread))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+	Glucose421::vec<Glucose421::Lit> a;
+	int max_var = -1;
+
+	if (glucose421_iterate(a_obj, a, max_var) == false)
+		return NULL;
+
+	if (max_var > 0)
+		glucose421_declare_vars(s, max_var);
+
+	PyOS_sighandler_t sig_save;
+	if (main_thread) {
+		sig_save = PyOS_setsig(SIGINT, sigint_handler);
+
+		if (setjmp(env) != 0) {
+			PyErr_SetString(SATError, "Caught keyboard interrupt");
+			return NULL;
+		}
+	}
+
+	Glucose421::vec<Glucose421::Lit> p;
+	bool res = s->prop_check(a, p, save_phases);
+
+	if (main_thread)
+		PyOS_setsig(SIGINT, sig_save);
+
+	PyObject *propagated = PyList_New(p.size());
+	for (int i = 0; i < p.size(); ++i) {
+		int l = Glucose421::var(p[i]) * (Glucose421::sign(p[i]) ? -1 : 1);
+		PyObject *lit = pyint_from_cint(l);
+		PyList_SetItem(propagated, i, lit);
+	}
+
+	PyObject *ret = Py_BuildValue("nO", (Py_ssize_t)res, propagated);
+	Py_DECREF(propagated);
+
+	return ret;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_setphases(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	PyObject *p_obj;  // polarities given as a list of integer literals
+
+	if (!PyArg_ParseTuple(args, "OO", &s_obj, &p_obj))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+	vector<int> p;
+	int max_var = -1;
+
+	if (pyiter_to_vector(p_obj, p, max_var) == false)
+		return NULL;
+
+	if (max_var > 0)
+		glucose421_declare_vars(s, max_var);
+
+	for (size_t i = 0; i < p.size(); ++i)
+		s->setPolarity(abs(p[i]), p[i] < 0);
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_cbudget(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	int64_t budget;
+
+	if (!PyArg_ParseTuple(args, "Ol", &s_obj, &budget))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+
+	if (budget != 0 && budget != -1)  // it is 0 by default
+		s->setConfBudget(budget);
+	else
+		s->budgetOff();
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_pbudget(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	int64_t budget;
+
+	if (!PyArg_ParseTuple(args, "Ol", &s_obj, &budget))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+
+	if (budget != 0 && budget != -1)  // it is 0 by default
+		s->setPropBudget(budget);
+	else
+		s->budgetOff();
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_interrupt(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+
+	if (!PyArg_ParseTuple(args, "O", &s_obj))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+
+	s->interrupt();
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_clearint(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+
+	if (!PyArg_ParseTuple(args, "O", &s_obj))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+
+	s->clearInterrupt();
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_setincr(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+
+	if (!PyArg_ParseTuple(args, "O", &s_obj))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+
+	s->setIncrementalMode();
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_tracepr(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+	PyObject *p_obj;
+
+	if (!PyArg_ParseTuple(args, "OO", &s_obj, &p_obj))
+		return NULL;
+
+	// get pointer to solver
+#if PY_MAJOR_VERSION < 3
+	Glucose421::Solver *s = (Glucose421::Solver *)PyCObject_AsVoidPtr(s_obj);
+
+	s->certifiedOutput = PyFile_AsFile(p_obj);
+	PyFile_IncUseCount((PyFileObject *)p_obj);
+#else
+	Glucose421::Solver *s = (Glucose421::Solver *)PyCapsule_GetPointer(s_obj, NULL);
+
+	int fd = PyObject_AsFileDescriptor(p_obj);
+	if (fd == -1) {
+		PyErr_SetString(SATError, "Cannot create proof file descriptor!");
+		return NULL;
+	}
+
+	s->certifiedOutput = fdopen(fd, "w+");
+	if (s->certifiedOutput == 0) {
+		PyErr_SetString(SATError, "Cannot create proof file pointer!");
+		return NULL;
+	}
+
+	setlinebuf(s->certifiedOutput);
+	Py_INCREF(p_obj);
+#endif
+
+	s->certifiedUNSAT  = true;
+	s->certifiedPyFile = (void *)p_obj;
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_core(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+
+	if (!PyArg_ParseTuple(args, "O", &s_obj))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+
+	Glucose421::vec<Glucose421::Lit> *c = &(s->conflict);  // minisat's conflict
+
+	PyObject *core = PyList_New(c->size());
+	for (int i = 0; i < c->size(); ++i) {
+		int l = Glucose421::var((*c)[i]) * (Glucose421::sign((*c)[i]) ? 1 : -1);
+		PyObject *lit = pyint_from_cint(l);
+		PyList_SetItem(core, i, lit);
+	}
+
+	if (c->size()) {
+		PyObject *ret = Py_BuildValue("O", core);
+		Py_DECREF(core);
+		return ret;
+	}
+
+	Py_DECREF(core);
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_model(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+
+	if (!PyArg_ParseTuple(args, "O", &s_obj))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+
+	// minisat's model
+	Glucose421::vec<Glucose421::lbool> *m = &(s->model);
+
+	if (m->size()) {
+		// l_True fails to work
+		Glucose421::lbool True = Glucose421::lbool((uint8_t)0);
+
+		PyObject *model = PyList_New(m->size() - 1);
+		for (int i = 1; i < m->size(); ++i) {
+			int l = i * ((*m)[i] == True ? 1 : -1);
+			PyObject *lit = pyint_from_cint(l);
+			PyList_SetItem(model, i - 1, lit);
+		}
+
+		PyObject *ret = Py_BuildValue("O", model);
+		Py_DECREF(model);
+		return ret;
+	}
+
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_nof_vars(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+
+	if (!PyArg_ParseTuple(args, "O", &s_obj))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+
+	int nof_vars = s->nVars() - 1;  // 0 is a dummy variable
+
+	PyObject *ret = Py_BuildValue("n", (Py_ssize_t)nof_vars);
+	return ret;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_nof_cls(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+
+	if (!PyArg_ParseTuple(args, "O", &s_obj))
+		return NULL;
+
+	// get pointer to solver
+	Glucose421::Solver *s = (Glucose421::Solver *)pyobj_to_void(s_obj);
+
+	int nof_cls = s->nClauses();
+
+	PyObject *ret = Py_BuildValue("n", (Py_ssize_t)nof_cls);
+	return ret;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_del(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+
+	if (!PyArg_ParseTuple(args, "O", &s_obj))
+		return NULL;
+
+	// get pointer to solver
+#if PY_MAJOR_VERSION < 3
+	Glucose421::Solver *s = (Glucose421::Solver *)PyCObject_AsVoidPtr(s_obj);
+
+	if (s->certifiedUNSAT == true)
+		PyFile_DecUseCount((PyFileObject *)(s->certifiedPyFile));
+#else
+	Glucose421::Solver *s = (Glucose421::Solver *)PyCapsule_GetPointer(s_obj, NULL);
+
+	if (s->certifiedUNSAT == true)
+		Py_DECREF((PyObject *)s->certifiedPyFile);
+#endif
+
+	delete s;
+	Py_RETURN_NONE;
+}
+
+//
+//=============================================================================
+static PyObject *py_glucose421_acc_stats(PyObject *self, PyObject *args)
+{
+	PyObject *s_obj;
+
+	if (!PyArg_ParseTuple(args, "O", &s_obj))
+		return NULL;
+
+	// get pointer to solver
+#if PY_MAJOR_VERSION < 3
+	Glucose421::Solver *s = (Glucose421::Solver *)PyCObject_AsVoidPtr(s_obj);
+#else
+	Glucose421::Solver *s = (Glucose421::Solver *)PyCapsule_GetPointer(s_obj, NULL);
+#endif
+
+	return Py_BuildValue("{s:n,s:n,s:n,s:n}",
+		"restarts", (Py_ssize_t)s->starts,
+		"conflicts", (Py_ssize_t)s->conflicts,
+		"decisions", (Py_ssize_t)s->decisions,
+		"propagations", (Py_ssize_t)s->propagations
+	);
+}
+#endif  // WITH_GLUCOSE421
+
 // API for Lingeling
 //=============================================================================
 #ifdef WITH_LINGELING
 static PyObject *py_lingeling_new(PyObject *self, PyObject *args)
 {
 	LGL *s = lglinit();
```

### Comparing `python-sat-0.1.8.dev7/tests/test_accum_stats.py` & `python-sat-0.1.8.dev8/tests/test_accum_stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 from pysat.formula import CNF
 
 solvers = ['cadical103',
            'cadical153',
            'gluecard30',
            'gluecard41',
            'glucose30',
-           'glucose41',
+           'glucose42',
            'lingeling',
            'maplechrono',
            'maplecm',
            'maplesat',
            'mergesat3',
            'minicard',
            'minisat22',
            'minisat-gh']
 
 def test_solvers():
     cnf = CNF(from_clauses=[[1, 2, 3], [-1, 2], [-2]])
 
     for name in solvers:
+        print("Name = {}".format(name))
         with Solver(name=name, bootstrap_with=cnf) as solver:
             solver.solve()
             stats = solver.accum_stats()
             assert 'conflicts' in stats, 'No conflicts for {0}'.format(name)
             assert 'decisions' in stats, 'No decisions for {0}'.format(name)
             assert 'propagations' in stats, 'No propagations for {0}'.format(name)
             assert 'restarts' in stats, 'No restarts for {0}'.format(name)
-
```

### Comparing `python-sat-0.1.8.dev7/tests/test_atmost1.py` & `python-sat-0.1.8.dev8/tests/test_atmost1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/tests/test_atmostk.py` & `python-sat-0.1.8.dev8/tests/test_atmostk.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/tests/test_cnfplus.py` & `python-sat-0.1.8.dev8/tests/test_cnfplus.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # all available solvers
 solvers = ['cadical103',
            'cadical153',
            'gluecard30',
            'gluecard41',
            'glucose30',
            'glucose41',
+           'glucose42',
            'lingeling',
            'maplechrono',
            'maplecm',
            'maplesat',
            'mergesat3',
            'minicard',
            'minisat22',
```

### Comparing `python-sat-0.1.8.dev7/tests/test_equals1.py` & `python-sat-0.1.8.dev8/tests/test_equals1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/tests/test_process.py` & `python-sat-0.1.8.dev8/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/tests/test_unique_model.py` & `python-sat-0.1.8.dev8/tests/test_unique_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 solvers = ['cadical103',
            'cadical153',
            'gluecard30',
            'gluecard41',
            'glucose30',
            'glucose41',
+           'glucose42',
            'lingeling',
            'maplechrono',
            'maplecm',
            'maplesat',
            'minicard',
            'mergesat3',
            'minisat22',
```

### Comparing `python-sat-0.1.8.dev7/tests/test_unique_mus.py` & `python-sat-0.1.8.dev8/tests/test_unique_mus.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev7/tests/test_warmstart.py` & `python-sat-0.1.8.dev8/tests/test_warmstart.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pysat.solvers import Solver
 
 def test_warmstart():
     n, b = 5, 3
 
     cnf = CardEnc.atmost(range(1, n + 1), b)
 
-    for name in ['m22', 'mgh', 'mpl', 'mcm', 'mc', 'g30', 'g41', 'gc30', 'gc41']:
+    for name in ['m22', 'mgh', 'mpl', 'mcm', 'mc', 'g30', 'g41', 'gc30', 'gc41', 'g42']:
         models1 = []
         with Solver(name=name, bootstrap_with=cnf, warm_start=False) as solver:
             models1 = [model for model in solver.enum_models()]
 
         with Solver(name=name, bootstrap_with=cnf, warm_start=True) as solver:
             models2 = [model for model in solver.enum_models()]
```


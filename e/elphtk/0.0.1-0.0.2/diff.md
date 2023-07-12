# Comparing `tmp/elphtk-0.0.1.tar.gz` & `tmp/elphtk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elphtk-0.0.1.tar", last modified: Sat Jun 17 16:34:03 2023, max compression
+gzip compressed data, was "elphtk-0.0.2.tar", last modified: Wed Jul 12 09:18:57 2023, max compression
```

## Comparing `elphtk-0.0.1.tar` & `elphtk-0.0.2.tar`

### file list

```diff
@@ -1,76 +1,80 @@
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-17 16:34:03.198237 elphtk-0.0.1/
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-17 16:34:03.188237 elphtk-0.0.1/Examples/
--rw-r--r--   0 shz       (1000) shz       (1000)      992 2023-06-17 12:30:03.000000 elphtk-0.0.1/Examples/README.md
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-17 16:34:03.188237 elphtk-0.0.1/Examples/example1/
--rw-r--r--   0 shz       (1000) shz       (1000)    11162 2023-06-17 09:08:46.000000 elphtk-0.0.1/Examples/example1/FORCE_SETS
--rw-r--r--   0 shz       (1000) shz       (1000)      124 2023-06-17 09:08:46.000000 elphtk-0.0.1/Examples/example1/band.conf
--rw-r--r--   0 shz       (1000) shz       (1000)   105801 2023-06-17 09:09:17.000000 elphtk-0.0.1/Examples/example1/band.yaml
--rw-r--r--   0 shz       (1000) shz       (1000)    29529 2023-06-17 16:09:55.000000 elphtk-0.0.1/Examples/example1/phonopy.freq.gp
--rw-r--r--   0 shz       (1000) shz       (1000)     9381 2023-06-17 09:09:22.000000 elphtk-0.0.1/Examples/example1/phonopy.yaml
--rw-r--r--   0 shz       (1000) shz       (1000)     9576 2023-06-17 09:08:46.000000 elphtk-0.0.1/Examples/example1/phonopy_disp.yaml
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-17 16:34:03.188237 elphtk-0.0.1/Examples/example2/
--rw-r--r--   0 shz       (1000) shz       (1000)      237 2023-06-17 10:19:20.000000 elphtk-0.0.1/Examples/example2/ZrN.dyn0
--rw-r--r--   0 shz       (1000) shz       (1000)     8701 2023-06-17 10:19:20.000000 elphtk-0.0.1/Examples/example2/ZrN.dyn1
--rw-r--r--   0 shz       (1000) shz       (1000)    20620 2023-06-17 10:19:21.000000 elphtk-0.0.1/Examples/example2/ZrN.dyn2
--rw-r--r--   0 shz       (1000) shz       (1000)    20620 2023-06-17 10:19:21.000000 elphtk-0.0.1/Examples/example2/ZrN.dyn3
--rw-r--r--   0 shz       (1000) shz       (1000)    45660 2023-06-17 10:19:21.000000 elphtk-0.0.1/Examples/example2/ZrN.fc
--rw-r--r--   0 shz       (1000) shz       (1000)    14862 2023-06-17 10:19:21.000000 elphtk-0.0.1/Examples/example2/ZrN.freq
--rw-r--r--   0 shz       (1000) shz       (1000)    12194 2023-06-17 10:19:21.000000 elphtk-0.0.1/Examples/example2/ZrN.freq.gp
--rw-r--r--   0 shz       (1000) shz       (1000)      260 2023-06-17 11:04:38.000000 elphtk-0.0.1/Examples/example2/matdyn.in
--rw-r--r--   0 shz       (1000) shz       (1000)      193 2023-06-17 10:19:19.000000 elphtk-0.0.1/Examples/example2/ph.in
--rw-r--r--   0 shz       (1000) shz       (1000)   141685 2023-06-17 10:19:20.000000 elphtk-0.0.1/Examples/example2/ph.out
--rw-r--r--   0 shz       (1000) shz       (1000)       75 2023-06-17 10:19:19.000000 elphtk-0.0.1/Examples/example2/q2r.in
--rw-r--r--   0 shz       (1000) shz       (1000)      702 2023-06-17 10:19:19.000000 elphtk-0.0.1/Examples/example2/scf.in
--rw-r--r--   0 shz       (1000) shz       (1000)    19082 2023-06-17 10:19:20.000000 elphtk-0.0.1/Examples/example2/scf.out
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-17 16:34:03.188237 elphtk-0.0.1/Examples/example3/
--rw-r--r--   0 shz       (1000) shz       (1000)    66919 2023-06-17 10:51:28.000000 elphtk-0.0.1/Examples/example3/ZrN.a2f
--rw-r--r--   0 shz       (1000) shz       (1000)    66919 2023-06-17 10:51:28.000000 elphtk-0.0.1/Examples/example3/ZrN.a2f.01
--rw-r--r--   0 shz       (1000) shz       (1000)    84566 2023-06-17 10:51:29.000000 elphtk-0.0.1/Examples/example3/ZrN.a2f_iso
--rw-r--r--   0 shz       (1000) shz       (1000)    66919 2023-06-17 10:51:30.000000 elphtk-0.0.1/Examples/example3/ZrN.a2f_tr.01
--rw-r--r--   0 shz       (1000) shz       (1000)     1539 2023-06-17 10:52:20.000000 elphtk-0.0.1/Examples/example3/ZrN.kmap
--rw-r--r--   0 shz       (1000) shz       (1000)    52726 2023-06-17 12:30:29.000000 elphtk-0.0.1/Examples/example3/ZrN.lambda_FS
--rw-r--r--   0 shz       (1000) shz       (1000)     3483 2023-06-17 10:52:21.000000 elphtk-0.0.1/Examples/example3/ZrN.lambda_k_pairs
--rw-r--r--   0 shz       (1000) shz       (1000)    19565 2023-06-17 10:52:35.000000 elphtk-0.0.1/Examples/example3/ZrN.nnkp
--rw-r--r--   0 shz       (1000) shz       (1000)    81500 2023-06-17 11:00:13.000000 elphtk-0.0.1/Examples/example3/ZrN.phdos
--rw-r--r--   0 shz       (1000) shz       (1000)    66500 2023-06-17 10:52:35.000000 elphtk-0.0.1/Examples/example3/ZrN.phdos.01
--rw-r--r--   0 shz       (1000) shz       (1000)   104000 2023-06-17 10:59:04.000000 elphtk-0.0.1/Examples/example3/ZrN.phdos_proj
--rw-r--r--   0 shz       (1000) shz       (1000)    13131 2023-06-17 12:31:01.000000 elphtk-0.0.1/Examples/example3/ZrN.res.01
--rw-r--r--   0 shz       (1000) shz       (1000)     2324 2023-06-17 10:52:40.000000 elphtk-0.0.1/Examples/example3/ZrN.win
--rw-r--r--   0 shz       (1000) shz       (1000)     2144 2023-06-17 14:20:25.000000 elphtk-0.0.1/Examples/example3/epw.in
--rw-r--r--   0 shz       (1000) shz       (1000)     4947 2023-06-17 10:49:58.000000 elphtk-0.0.1/Examples/example3/nscf.in
--rw-r--r--   0 shz       (1000) shz       (1000)    70036 2023-06-17 10:50:00.000000 elphtk-0.0.1/Examples/example3/nscf.out
--rw-r--r--   0 shz       (1000) shz       (1000)      720 2023-06-17 10:49:58.000000 elphtk-0.0.1/Examples/example3/scf.in
--rw-r--r--   0 shz       (1000) shz       (1000)    19082 2023-06-17 10:50:00.000000 elphtk-0.0.1/Examples/example3/scf.out
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-17 16:34:03.188237 elphtk-0.0.1/Examples/example4/
--rw-r--r--   0 shz       (1000) shz       (1000)    23760 2023-06-17 16:33:07.000000 elphtk-0.0.1/Examples/example4/freq.txt
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-17 16:34:03.188237 elphtk-0.0.1/Examples/example4/tmp/
--rw-r--r--   0 shz       (1000) shz       (1000)    48744 2023-06-17 11:02:44.000000 elphtk-0.0.1/Examples/example4/tmp/ZrN.egnv
--rw-r--r--   0 shz       (1000) shz       (1000)   179728 2023-06-17 13:11:51.000000 elphtk-0.0.1/Examples/example4/tmp/ZrN.ephmat1
--rw-r--r--   0 shz       (1000) shz       (1000)    32272 2023-06-17 11:02:44.000000 elphtk-0.0.1/Examples/example4/tmp/ZrN.freq
--rw-r--r--   0 shz       (1000) shz       (1000)    15564 2023-06-17 13:25:15.000000 elphtk-0.0.1/Examples/example4/tmp/ZrN.ikmap
--rw-r--r--   0 shz       (1000) shz       (1000)     1058 2023-06-17 07:04:09.000000 elphtk-0.0.1/LICENSE.txt
--rw-r--r--   0 shz       (1000) shz       (1000)      161 2023-06-17 14:16:37.000000 elphtk-0.0.1/MANIFEST.in
--rw-r--r--   0 shz       (1000) shz       (1000)      447 2023-06-17 16:34:03.198237 elphtk-0.0.1/PKG-INFO
--rw-r--r--   0 shz       (1000) shz       (1000)     1881 2023-06-17 16:00:40.000000 elphtk-0.0.1/README.md
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-17 16:34:03.188237 elphtk-0.0.1/elphtk/
--rw-r--r--   0 shz       (1000) shz       (1000)      268 2023-06-17 16:32:56.000000 elphtk-0.0.1/elphtk/__init__.py
--rw-r--r--   0 shz       (1000) shz       (1000)    14279 2023-06-17 15:28:58.000000 elphtk-0.0.1/elphtk/arguments.py
--rw-r--r--   0 shz       (1000) shz       (1000)    14323 2023-06-17 16:32:51.000000 elphtk-0.0.1/elphtk/epw_binary.py
--rw-r--r--   0 shz       (1000) shz       (1000)    24893 2023-06-17 15:14:12.000000 elphtk-0.0.1/elphtk/epw_tool.py
--rw-r--r--   0 shz       (1000) shz       (1000)     7603 2023-06-17 15:57:41.000000 elphtk-0.0.1/elphtk/phonon_plot.py
--rw-r--r--   0 shz       (1000) shz       (1000)      404 2023-06-17 16:03:40.000000 elphtk-0.0.1/elphtk/pkg_info.py
--rw-r--r--   0 shz       (1000) shz       (1000)     9944 2023-06-17 15:55:48.000000 elphtk-0.0.1/elphtk/qe_phonon.py
--rw-r--r--   0 shz       (1000) shz       (1000)     3960 2023-06-17 07:53:30.000000 elphtk-0.0.1/elphtk/wgauss.py
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-17 16:34:03.198237 elphtk-0.0.1/elphtk.egg-info/
--rw-r--r--   0 shz       (1000) shz       (1000)      447 2023-06-17 16:34:03.000000 elphtk-0.0.1/elphtk.egg-info/PKG-INFO
--rw-r--r--   0 shz       (1000) shz       (1000)     1632 2023-06-17 16:34:03.000000 elphtk-0.0.1/elphtk.egg-info/SOURCES.txt
--rw-r--r--   0 shz       (1000) shz       (1000)        1 2023-06-17 16:34:03.000000 elphtk-0.0.1/elphtk.egg-info/dependency_links.txt
--rw-r--r--   0 shz       (1000) shz       (1000)       38 2023-06-17 16:34:03.000000 elphtk-0.0.1/elphtk.egg-info/requires.txt
--rw-r--r--   0 shz       (1000) shz       (1000)      133 2023-06-17 16:34:03.000000 elphtk-0.0.1/elphtk.egg-info/top_level.txt
-drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-06-17 16:34:03.198237 elphtk-0.0.1/scripts/
--rwxr-xr-x   0 shz       (1000) shz       (1000)     5693 2023-06-17 16:07:01.000000 elphtk-0.0.1/scripts/phplot
--rwxr-xr-x   0 shz       (1000) shz       (1000)     6737 2023-06-17 16:28:39.000000 elphtk-0.0.1/scripts/post_epw
--rwxr-xr-x   0 shz       (1000) shz       (1000)    10991 2023-06-17 16:08:45.000000 elphtk-0.0.1/scripts/qe2epw
--rwxr-xr-x   0 shz       (1000) shz       (1000)    13730 2023-06-17 16:05:45.000000 elphtk-0.0.1/scripts/qe_lambda
--rw-r--r--   0 shz       (1000) shz       (1000)       38 2023-06-17 16:34:03.198237 elphtk-0.0.1/setup.cfg
--rwxr-xr-x   0 shz       (1000) shz       (1000)     2902 2023-06-17 16:24:26.000000 elphtk-0.0.1/setup.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.142871 elphtk-0.0.2/
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.122871 elphtk-0.0.2/Examples/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      973 2023-07-12 08:22:30.000000 elphtk-0.0.2/Examples/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.126871 elphtk-0.0.2/Examples/example1/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    11162 2023-06-17 09:08:46.000000 elphtk-0.0.2/Examples/example1/FORCE_SETS
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      104 2023-07-12 08:24:25.000000 elphtk-0.0.2/Examples/example1/README
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      124 2023-06-17 09:08:46.000000 elphtk-0.0.2/Examples/example1/band.conf
+-rw-r--r--   0 zsh       (1000) zsh       (1000)   105801 2023-06-17 09:09:17.000000 elphtk-0.0.2/Examples/example1/band.yaml
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    29529 2023-07-12 08:23:11.000000 elphtk-0.0.2/Examples/example1/phonopy.freq.gp
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     9381 2023-06-17 09:09:22.000000 elphtk-0.0.2/Examples/example1/phonopy.yaml
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     9576 2023-06-17 09:08:46.000000 elphtk-0.0.2/Examples/example1/phonopy_disp.yaml
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.130871 elphtk-0.0.2/Examples/example2/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      110 2023-07-12 08:25:32.000000 elphtk-0.0.2/Examples/example2/README
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      237 2023-06-17 10:19:20.000000 elphtk-0.0.2/Examples/example2/ZrN.dyn0
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     8701 2023-06-17 10:19:20.000000 elphtk-0.0.2/Examples/example2/ZrN.dyn1
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    20620 2023-06-17 10:19:21.000000 elphtk-0.0.2/Examples/example2/ZrN.dyn2
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    20620 2023-06-17 10:19:21.000000 elphtk-0.0.2/Examples/example2/ZrN.dyn3
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    45660 2023-06-17 10:19:21.000000 elphtk-0.0.2/Examples/example2/ZrN.fc
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    14862 2023-06-17 10:19:21.000000 elphtk-0.0.2/Examples/example2/ZrN.freq
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    12194 2023-06-17 10:19:21.000000 elphtk-0.0.2/Examples/example2/ZrN.freq.gp
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      260 2023-06-17 11:04:38.000000 elphtk-0.0.2/Examples/example2/matdyn.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      193 2023-06-17 10:19:19.000000 elphtk-0.0.2/Examples/example2/ph.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)   141685 2023-06-17 10:19:20.000000 elphtk-0.0.2/Examples/example2/ph.out
+-rw-r--r--   0 zsh       (1000) zsh       (1000)       75 2023-06-17 10:19:19.000000 elphtk-0.0.2/Examples/example2/q2r.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      702 2023-06-17 10:19:19.000000 elphtk-0.0.2/Examples/example2/scf.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    19082 2023-06-17 10:19:20.000000 elphtk-0.0.2/Examples/example2/scf.out
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.138871 elphtk-0.0.2/Examples/example3/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      245 2023-07-12 08:47:33.000000 elphtk-0.0.2/Examples/example3/README
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:28.000000 elphtk-0.0.2/Examples/example3/ZrN.a2f
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:28.000000 elphtk-0.0.2/Examples/example3/ZrN.a2f.01
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    84566 2023-06-17 10:51:29.000000 elphtk-0.0.2/Examples/example3/ZrN.a2f_iso
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    66919 2023-06-17 10:51:30.000000 elphtk-0.0.2/Examples/example3/ZrN.a2f_tr.01
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1539 2023-06-17 10:52:20.000000 elphtk-0.0.2/Examples/example3/ZrN.kmap
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    52726 2023-06-17 12:30:29.000000 elphtk-0.0.2/Examples/example3/ZrN.lambda_FS
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     3483 2023-06-17 10:52:21.000000 elphtk-0.0.2/Examples/example3/ZrN.lambda_k_pairs
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    19565 2023-06-17 10:52:35.000000 elphtk-0.0.2/Examples/example3/ZrN.nnkp
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    81500 2023-06-17 11:00:13.000000 elphtk-0.0.2/Examples/example3/ZrN.phdos
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    66500 2023-06-17 10:52:35.000000 elphtk-0.0.2/Examples/example3/ZrN.phdos.01
+-rw-r--r--   0 zsh       (1000) zsh       (1000)   104000 2023-06-17 10:59:04.000000 elphtk-0.0.2/Examples/example3/ZrN.phdos_proj
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    13131 2023-06-17 12:31:01.000000 elphtk-0.0.2/Examples/example3/ZrN.res.01
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     2324 2023-06-17 10:52:40.000000 elphtk-0.0.2/Examples/example3/ZrN.win
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     2144 2023-06-17 14:20:25.000000 elphtk-0.0.2/Examples/example3/epw.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     4947 2023-06-17 10:49:58.000000 elphtk-0.0.2/Examples/example3/nscf.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    70036 2023-06-17 10:50:00.000000 elphtk-0.0.2/Examples/example3/nscf.out
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      720 2023-06-17 10:49:58.000000 elphtk-0.0.2/Examples/example3/scf.in
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    19082 2023-06-17 10:50:00.000000 elphtk-0.0.2/Examples/example3/scf.out
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.138871 elphtk-0.0.2/Examples/example4/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      118 2023-07-12 09:06:35.000000 elphtk-0.0.2/Examples/example4/README
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)    23760 2023-07-12 09:06:43.000000 elphtk-0.0.2/Examples/example4/freq.txt
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.138871 elphtk-0.0.2/Examples/example4/tmp/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    48744 2023-06-17 11:02:44.000000 elphtk-0.0.2/Examples/example4/tmp/ZrN.egnv
+-rw-r--r--   0 zsh       (1000) zsh       (1000)   179728 2023-06-17 13:11:51.000000 elphtk-0.0.2/Examples/example4/tmp/ZrN.ephmat1
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    32272 2023-06-17 11:02:44.000000 elphtk-0.0.2/Examples/example4/tmp/ZrN.freq
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    15564 2023-06-17 13:25:15.000000 elphtk-0.0.2/Examples/example4/tmp/ZrN.ikmap
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1058 2023-06-17 07:04:09.000000 elphtk-0.0.2/LICENSE.txt
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      161 2023-06-17 14:16:37.000000 elphtk-0.0.2/MANIFEST.in
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      285 2023-07-12 09:18:57.142871 elphtk-0.0.2/PKG-INFO
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     1881 2023-06-17 16:00:40.000000 elphtk-0.0.2/README.md
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.142871 elphtk-0.0.2/elphtk/
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      299 2023-07-12 09:18:30.000000 elphtk-0.0.2/elphtk/__init__.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    14279 2023-07-12 08:41:38.000000 elphtk-0.0.2/elphtk/arguments.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    14325 2023-07-12 09:05:50.000000 elphtk-0.0.2/elphtk/epw_binary.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)    26012 2023-07-12 08:55:02.000000 elphtk-0.0.2/elphtk/epw_tool.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     7603 2023-06-17 15:57:41.000000 elphtk-0.0.2/elphtk/phonon_plot.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      404 2023-06-18 05:08:44.000000 elphtk-0.0.2/elphtk/pkg_info.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     9906 2023-07-12 08:39:33.000000 elphtk-0.0.2/elphtk/qe_phonon.py
+-rw-r--r--   0 zsh       (1000) zsh       (1000)     3922 2023-07-12 08:39:49.000000 elphtk-0.0.2/elphtk/wgauss.py
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.142871 elphtk-0.0.2/elphtk.egg-info/
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)      285 2023-07-12 09:18:56.000000 elphtk-0.0.2/elphtk.egg-info/PKG-INFO
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)     1742 2023-07-12 09:18:57.000000 elphtk-0.0.2/elphtk.egg-info/SOURCES.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-07-12 09:18:56.000000 elphtk-0.0.2/elphtk.egg-info/dependency_links.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-07-12 09:18:56.000000 elphtk-0.0.2/elphtk.egg-info/requires.txt
+-rw-rw-r--   0 zsh       (1000) zsh       (1000)        7 2023-07-12 09:18:56.000000 elphtk-0.0.2/elphtk.egg-info/top_level.txt
+drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-07-12 09:18:57.142871 elphtk-0.0.2/scripts/
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5655 2023-07-12 08:39:15.000000 elphtk-0.0.2/scripts/phplot
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6960 2023-07-12 09:05:46.000000 elphtk-0.0.2/scripts/post_epw
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    10991 2023-07-12 09:02:25.000000 elphtk-0.0.2/scripts/qe2epw
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13693 2023-07-12 08:39:06.000000 elphtk-0.0.2/scripts/qe_lambda
+-rw-r--r--   0 zsh       (1000) zsh       (1000)      574 2023-07-12 09:18:57.146871 elphtk-0.0.2/setup.cfg
+-rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2608 2023-07-12 09:16:39.000000 elphtk-0.0.2/setup.py
```

### Comparing `elphtk-0.0.1/Examples/README.md` & `elphtk-0.0.2/Examples/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-## Some examples to demonstrate the usages
+# Some examples to demonstrate the usages
 
-# example1: plot phonon spectrum generated by Phonopy
+## example1: plot phonon spectrum generated by Phonopy
 
     The phonopy package provides a script phonopy-bandplot to plot phonon bands
-
     We here provide an alternative script with more flexible arguments to optimize plots
 
-# example2: plot phonon spectrum generated by Quantum ESPRESSO
+## example2: plot phonon spectrum generated by Quantum ESPRESSO
 
     Read the phonon output from QE and plot phonon bands
 
-# example3: plot phonon spectrum generated by EPW
+## example3: plot phonon spectrum generated by EPW
 
     Read the phonon output from EPW and plot phonon bands
 
-# exmaple4: plot some electron-phonon-coupling related properties by EPW
+## exmaple4: plot some electron-phonon-coupling related properties by EPW
 
     Read some binary files such as elphmat generated by EPW, for analysis
 
-# example5: Use qe_lambda to calculate the superconductivity transition temperature
+## example5: Use qe_lambda to calculate the superconducting Tc
 
     This example demonstrate how to calculate the phonon-mediated superconductivity transition temperature
 
     with electron-phonon-coupling constants calculated by Quantum ESPRESSO, PH module
 
     It can exclude imaginary modes and only counts real ones
```

### Comparing `elphtk-0.0.1/Examples/example1/FORCE_SETS` & `elphtk-0.0.2/Examples/example1/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example1/band.yaml` & `elphtk-0.0.2/Examples/example1/band.yaml`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example1/phonopy.freq.gp` & `elphtk-0.0.2/Examples/example1/phonopy.freq.gp`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example1/phonopy.yaml` & `elphtk-0.0.2/Examples/example1/phonopy.yaml`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example1/phonopy_disp.yaml` & `elphtk-0.0.2/Examples/example1/phonopy_disp.yaml`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example2/ZrN.dyn1` & `elphtk-0.0.2/Examples/example2/ZrN.dyn1`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example2/ZrN.dyn2` & `elphtk-0.0.2/Examples/example2/ZrN.dyn2`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example2/ZrN.dyn3` & `elphtk-0.0.2/Examples/example2/ZrN.dyn3`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example2/ZrN.fc` & `elphtk-0.0.2/Examples/example2/ZrN.fc`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example2/ZrN.freq` & `elphtk-0.0.2/Examples/example2/ZrN.freq`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example2/ZrN.freq.gp` & `elphtk-0.0.2/Examples/example2/ZrN.freq.gp`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example2/ph.out` & `elphtk-0.0.2/Examples/example2/ph.out`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example2/scf.in` & `elphtk-0.0.2/Examples/example2/scf.in`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example2/scf.out` & `elphtk-0.0.2/Examples/example2/scf.out`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/ZrN.a2f` & `elphtk-0.0.2/Examples/example3/ZrN.a2f`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/ZrN.a2f.01` & `elphtk-0.0.2/Examples/example3/ZrN.a2f.01`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/ZrN.a2f_iso` & `elphtk-0.0.2/Examples/example3/ZrN.a2f_iso`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/ZrN.a2f_tr.01` & `elphtk-0.0.2/Examples/example3/ZrN.a2f_tr.01`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/ZrN.kmap` & `elphtk-0.0.2/Examples/example3/ZrN.kmap`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/ZrN.lambda_FS` & `elphtk-0.0.2/Examples/example3/ZrN.lambda_FS`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/ZrN.lambda_k_pairs` & `elphtk-0.0.2/Examples/example3/ZrN.lambda_k_pairs`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/ZrN.nnkp` & `elphtk-0.0.2/Examples/example3/ZrN.nnkp`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/ZrN.phdos` & `elphtk-0.0.2/Examples/example3/ZrN.phdos`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/ZrN.phdos.01` & `elphtk-0.0.2/Examples/example3/ZrN.phdos.01`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/ZrN.phdos_proj` & `elphtk-0.0.2/Examples/example3/ZrN.phdos_proj`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/ZrN.res.01` & `elphtk-0.0.2/Examples/example3/ZrN.res.01`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/ZrN.win` & `elphtk-0.0.2/Examples/example3/ZrN.win`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/epw.in` & `elphtk-0.0.2/Examples/example3/epw.in`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/nscf.in` & `elphtk-0.0.2/Examples/example3/nscf.in`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/nscf.out` & `elphtk-0.0.2/Examples/example3/nscf.out`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/scf.in` & `elphtk-0.0.2/Examples/example3/scf.in`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example3/scf.out` & `elphtk-0.0.2/Examples/example3/scf.out`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example4/freq.txt` & `elphtk-0.0.2/Examples/example4/freq.txt`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example4/tmp/ZrN.egnv` & `elphtk-0.0.2/Examples/example4/tmp/ZrN.egnv`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example4/tmp/ZrN.ephmat1` & `elphtk-0.0.2/Examples/example4/tmp/ZrN.ephmat1`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example4/tmp/ZrN.freq` & `elphtk-0.0.2/Examples/example4/tmp/ZrN.freq`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/Examples/example4/tmp/ZrN.ikmap` & `elphtk-0.0.2/Examples/example4/tmp/ZrN.ikmap`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/LICENSE.txt` & `elphtk-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/README.md` & `elphtk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/elphtk/arguments.py` & `elphtk-0.0.2/elphtk/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                         help='Filename for the plot. It accepts all image formats supported by matplotlib.')
     parser.add_argument('--verbosity',type=int,default=1,help='level of verbosity')
 
 
 def add_fig_arguments(parser):
     parser.add_argument('--figname',type=str,default='phband',
                         help='file name for the figure saved')
-    parser.add_argument('--figsize', type=eval, default=(4, 4),
+    parser.add_argument('--figsize', type=eval, default=(5, 4),
                        help='Figure size. Default: %(default)s')
     parser.add_argument('--dpi', type=float, default=600,
                        help='Plot resolution. Default: %(default)s')
     parser.add_argument('--subplot',type=str2bool,nargs='?',const=False,default=False,
                        help='whether or not to plot in subplots. Default: %(default)s')
     parser.add_argument('--marker', type=str, default='o',
                        help='Marker for the fatband plot. Default: %(default)s.')
```

### Comparing `elphtk-0.0.1/elphtk/epw_binary.py` & `elphtk-0.0.2/elphtk/epw_binary.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,16 +56,16 @@
         for iq in range(nqtotf):
             qpts[iq]=f.read_record('f8',shape=3)
             for imode in range(nmodes): wf[iq,imode]=f.read_record('f8')
     print ('Freqs in units of eV')
     return qpts,wf*units.Rydberg
 
 
-def write_freq(qpts,freq,filfreqtxt='freq.txt'):
-    data =np.concatenate((qpts,freq),axis=1)
+def write_freq(qpts,freqs,filfreqtxt='freq.txt'):
+    data =np.concatenate((qpts,freqs),axis=1)
     np.savetxt(filfreqtxt,data,fmt='%10.5f')
 
 
 def read_egnv(outdir='./tmp',seedname='wannier90'):
     with fortio.FortranFile('{0}/{1}.egnv'.format(outdir,seedname)) as f:
         nkftot,nkf1,nkf2,nkf3,nkfs=f.read_record('i4')
         recl=f.get_record_size()
```

### Comparing `elphtk-0.0.1/elphtk/epw_tool.py` & `elphtk-0.0.2/elphtk/epw_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 #  Usage:      processing data from EPW for plot and analysis               #      
 #  Author:     Shunhong Zhang <szhang2@ustc.edu.cn>                         #
 #  Date:       Sep 28, 2019                                                 #
 #                                                                           #
 #===========================================================================#
 
 
-from __future__ import print_function
 import os
 import matplotlib.pyplot as plt
 import numpy as np
 import matplotlib as mpl
 import itertools
 import collections
 import phonopy.units as units
@@ -54,15 +53,17 @@
         kgmap=np.fromfile(f,count=nq*3,sep=' ',dtype=float).reshape(nq,3)
     fig=plt.figure(figsize=args.figsize)
     ax=fig.add_subplot(111)
     ax.scatter(qpts[:,0],qpts[:,1],s=20,facecolor='r',edgecolor='none')
     ax.scatter(kgmap[:,0],kgmap[:,1],s=10,facecolor='b',edgecolor='none')
     ax.set_aspect('equal')
     fig.tight_layout()
-    fig.savefig('kgmap',dpi=400)
+    fig.savefig('kgmap',dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
 
 
 def plot_specfun(args):
     print ('plot spectral function')
     fil='specfun.elself'
     nlne=500
     data=[]
@@ -87,16 +88,17 @@
     ax.set_xlim(1,nkpt)
     ax.set_ylabel('$\omega$ (eV)')
     ax=fig.add_subplot(211)
     ax.plot(np.arange(201),int_spec,'r-')
     ax.set_yticks(np.arange(5))
     ax.set_ylabel('electron linewidth (meV)')
     fig.tight_layout()
-    fig.savefig('specfun',dpi=400)
-    return fig,ax
+    fig.savefig('specfun',dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
 
 
 def plot_specfun_sup(args):
     print ('plot spectral function')
     fil='specfun_sup.elself'
     nlne=500
     f=open(fil)
@@ -114,16 +116,17 @@
         my_extent=[1,nkpt,np.min(data[iband,:,:,3]),np.max(data[iband,:,:,3])]
         im=ax.imshow(data[iband,:,:,4],extent=my_extent,cmap='viridis',aspect='auto',origin='lower')
         ax.axhline(0,c='w',ls='--',alpha=0.8)
         ax.set_xlim(1,nkpt)
         if iband==0: ax.set_ylabel('$\omega$ (eV)')
     fig.colorbar(im)
     fig.tight_layout()
-    fig.savefig('specfun_sup',dpi=400)
-    return fig,ax
+    fig.savefig('specfun_sup',dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
 
 
 def plot_phself(args):
     print ('plot phonon self-energy')
     fil='linewidth.phself'
     with open(fil) as f:
         f.readline()
@@ -159,16 +162,18 @@
         data=data.reshape(nkpt,nmode,data.shape[-1])
         if args.sum_modes: fc=np.sum(data[:,:,-1],axis=1)
         else: fc=data[:,args.imode,-1]
         cax=ax.scatter(qf[:,0],qf[:,1],s=args.markersize,facecolor=fc,edgecolor='none')
         cbar=fig.colorbar(cax)
         ax.set_aspect('equal')
     fig.tight_layout()
-    fig.savefig('{0}_linewidth'.format(args.task),dpi=400)
-    return fig,ax
+    figname = '{}_linewidth'.format(args.task)
+    fig.savefig(figname,dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
 
 
 def plot_elself(args):
     print ('plot electron self-energy')
     fil='linewidth.elself'
     with open(fil) as f:
         f.readline()
@@ -206,16 +211,18 @@
         data=data.reshape(nkpt,nbnd,nmode,data.shape[-1])
         if args.sum_modes: fc=np.sum(data[:,:,:,-1],axis=(1,2))
         else: fc=data[:,args.iband,args.imode,-1]
         cax=ax.scatter(kf[:,0],kf[:,1],s=args.markersize,facecolor=fc,edgecolor='none')
         cbar=fig.colorbar(cax)
         ax.set_aspect('equal')
     fig.tight_layout()
-    fig.savefig('{0}_linewidth'.format(args.task),dpi=400)
-    return fig,ax
+    figname = '{0}_linewidth'.format(args.task)
+    fig.savefig(figname,dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
 
 
 def plot_lambda_phself():
     print ('plot lambda phonon self-energy')
     print ('under development')
 
 
@@ -228,69 +235,74 @@
         data=np.loadtxt(f)
     bands=set(data[:,1])
     modes=set(data[:,-2])
     nbnd=len(bands)
     nmode=len(modes)
     kf=get_kf_from_out()
     nkpt=len(kf)
-    print ('fermi energy read from fine k-mesh: {0:10.5f} eV'.format(efermi))
-    print ('no. of bands: {0:3d}'.format(nbnd))
-    print ('no. of branches: {0:2d}'.format(nmode))
-    print ('no. of kpts: {0:6d}'.format(nkpt))
+    print ('Fermi energy read from fine k-mesh: {:10.5f} eV'.format(efermi))
+    print ('No. of bands: {0:3d}'.format(nbnd))
+    print ('No. of branches: {0:2d}'.format(nmode))
+    print ('No. of kpts: {0:6d}'.format(nkpt))
     data=data.reshape(nkpt,nbnd,nmode,data.shape[-1])
     evals=data[:,:,0,-1]-efermi
     #abs_evals=np.abs(evals)
     #ibnd = [(np.where(abs_evals[ik]==np.min(abs_evals[ik]))[0]) for ik in range(nkpt)]
     #print (ibnd[:40])
     for ibnd in range(nbnd):
         fc=evals[:,ibnd]
         fig,ax=plt.subplots(1,1,figsize=args.figsize)
         cax=ax.scatter(kf[:,0],kf[:,1],s=args.markersize,facecolor=fc,edgecolor='none',vmin=-1,vmax=1,cmap='bwr')
         cbar=fig.colorbar(cax)
         ax.set_aspect('equal')
         fig.tight_layout()
-        fig.savefig('fermi_surface_bnd_{0}'.format(ibnd),dpi=400)
-    return fig,ax
-
+        figname = 'fermi_surface_bnd_{}'.format(ibnd)
+        fig.savefig(figname,dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
 
 
 def get_smearing(prefix):
     get_lines=os.popen("grep -A 1 smearing {0}.a2f".format(prefix)).readlines()
     ph_smearing=np.array([float(item) for item in get_lines[1].split()[1:]])
     el_smearing=float(get_lines[2].split()[-1])
     return ph_smearing,el_smearing
 
+
 def plot_phmesh(args,ikz=0):
     import spcd
     qpts,freqs=spcd.read_freq(seedname=args.prefix)
     freq=freqs[:,args.imode]
     freq_THz=freq*units.Rydberg/units.THzToEv
     print ('\nfrequencies range for mode {0}'.format(args.imode))
-    print ('[{0:12.7f},{1:12.7f}] eV'.format(np.min(freq),np.max(freq)))
-    print ('[{0:12.7f},{1:12.7f}] THz'.format(np.min(freq_THz),np.max(freq_THz)))
+    print ('[{:12.7f}, {:12.7f}] eV'.format(np.min(freq),np.max(freq)))
+    print ('[{:12.7f}, {:12.7f}] THz'.format(np.min(freq_THz),np.max(freq_THz)))
     print ('')
     cx=collections.Counter(qpts[:,0])
     cy=collections.Counter(qpts[:,1])
     cz=collections.Counter(qpts[:,2])
-    print ('plot phmesh in kz={0} plane'.format(qpts[ikz,2]))
+    print ('Plotting phmesh in kz={:8.3f} plane'.format(qpts[ikz,2]))
     #plot_data=data[:,iband].reshape(nqx,nqy,nqz)[:,:,ikz].T
     fig=plt.figure(figsize=args.figsize)
     ax=fig.add_subplot(111)
     #my_extent=[0,1,0,1] # need refinement
     #im = ax.imshow(plot_data,extent=my_extent,cmap='viridis',origin='lower')
     im=ax.scatter(qpts[:,0],qpts[:,1],s=30,facecolor=freq_THz,edgecolor='none',cmap='viridis')
     ax.set_xticks([])
     ax.set_xlabel('$k_x$')
     ax.set_ylabel('$k_y$')
     ax.set_aspect('equal')
     cbar = fig.colorbar(im)
     cbar.ax.set_title('$\omega\ \mathrm{(THz)}$')
     fig.tight_layout()
-    fig.savefig('phmesh_{0}'.format(args.imode),dpi=400)
-    
+    figna,e = 'phmesh_{}'.format(args.imode)
+    fig.savefig(figname,dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig 
+
 
 def plot_phband(args):
     print ('plot phonon band')
     fil='{}.freq'.format(args.prefix)
     with open(fil) as f:
         line=f.readline().split()
         nband=int(line[2].rstrip(','))
@@ -303,15 +315,18 @@
     fig=plt.figure(figsize=args.figsize)
     ax=fig.add_subplot(111)
     for iband in range(nband): ax.plot(np.arange(nkpt),data[:,iband],'g-')
     ax.set_xlim(0,nkpt)
     ax.set_xticks([])
     ax.set_ylabel('$\omega$ ($meV$)')
     fig.tight_layout()
-    fig.savefig('phband',dpi=400)
+    fig.savefig('phband',dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
+
 
 def plot_phdos(args):
     print ('plot phonon density of states')
     try: 
         ph_smearing,el_smearing=get_smearing(args.prefix)
         print ('ph smearing: {0} meV'.format(ph_smearing[args.ismear]))
     except: pass
@@ -322,15 +337,18 @@
     fig=plt.figure(figsize=args.figsize)
     ax=fig.add_subplot(111)
     ax.set_xlabel('$\omega$ ($meV$)')
     ax.set_ylabel('$phdos$ ($\omega^{-1}$)')
     ax.plot(freq,phdos[:,args.ismear],'g-')
     ax.set_xlim(freq[0],freq[-1])
     fig.tight_layout()
-    fig.savefig('{0}_phdos'.format(args.prefix),dpi=args.dpi)
+    figname = '{}_phdos'.format(args.prefix)
+    fig.savefig(figname,dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
     
 
 def plot_lambda_FS(args):
     with open('{}.lambda_FS'.format(args.seedname)) as f:
         f.readline()
         data=np.loadtxt(f)
     kpt=data[:,:3]
@@ -356,19 +374,20 @@
     lambda_all=np.sum(band_lambda,axis=0)
     if args.sum_modes:
         fig=plt.figure(figsize=(6,4))
         ax=fig.add_subplot(111)
         fig.subplots_adjust(right=0.8)
         cb=ax.scatter(kpt_fs[:,0],kpt_fs[:,1],s=args.markersize,c=lambda_all,cmap='rainbow')
         fig.subplots_adjust(right=0.8)
-        cbar_ax = fig.add_axes([0.85, 0.1, 0.05, 0.8])
+        cbar_ax = fig.add_axes([0.85, 0.1, 0.03, 0.7])
         fig.colorbar(cb,cax=cbar_ax)
         ax.set_aspect('equal')
-        fig.savefig('lambda_all',dpi=400)
-        return 1
+        fig.savefig('lambda_all',dpi=args.dpi)
+        if args.show_plot: plt.show()
+        return fig
 
     for ib in range(nband):
         fig=plt.figure(figsize=(6,4))
         ax=fig.add_subplot(111)
         #subset=np.where(band_idx==idx+1)[0]
         if args.mesh_style=='interp':
             #colors=np.zeros((len(ky),len(kx)),float)
@@ -388,27 +407,31 @@
         margin_y=(np.max(kpt[:,1])-np.min(kpt[:,1]))*0.0
         ax.set_xlim(np.min(kpt[:,0])-margin_x,np.max(kpt[:,0])+margin_y)
         ax.set_ylim(np.min(kpt[:,1])-margin_y,np.max(kpt[:,1])+margin_y)
         ax.set_xlabel('$k_x$')
         ax.set_title('band {0}'.format(ib+1))
         ax.set_ylabel('$k_y$')
         fig.subplots_adjust(right=0.8)
-        cbar_ax = fig.add_axes([0.85, 0.1, 0.05, 0.8])
+        cbar_ax = fig.add_axes([0.85, 0.1, 0.03, 0.7])
         fig.colorbar(cb,cax=cbar_ax)
-        fig.savefig('lambda_band_{0}_{1}'.format(args.mesh_style,ib),dpi=400)
+        figname = 'lambda_band_{}_{}'.format(args.mesh_style,ib)
+        fig.savefig(figname,dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
      
 
 def read_a2f(args,iso=False):
     ncol=11
     nrow=500
-    fil='{0}.a2f.01'.format(args.prefix)
-    if iso: fil='{0}_iso'.format(fil)
-    print ('reading data from {0}'.format(fil))
+    fil='{}.a2f.01'.format(args.prefix)
+    if iso: fil='{}_iso'.format(fil)
+    print ('Reading data from {}'.format(fil))
     f=open(fil,'r')
-    data=np.fromfile(f,count=ncol*nrow,dtype=float,sep=' ').reshape(nrow,ncol)
+    data=np.fromfile(f,count=ncol*nrow,dtype=float,sep=' ')
+    data = data.reshape(nrow,ncol)
     freq=data[:,0]
     a2f=data[:,1:]
     print ('a2f shape:',a2f.shape)
     # times 2 to include the spin degeneracy, for spin case please double check it
     cum_epc=np.array([np.trapz(a2f[:iw,args.ismear]/freq[:iw],x=freq[:iw]) for iw in range(nrow)])*2
     print ('integrated el-ph strength:{0:10.7f}'.format(cum_epc[-1]))
 
@@ -422,39 +445,44 @@
         [f.readline() for i in range(3)]
         fermi_win=float(f.readline().split()[-1])
         sum_epc=float(f.readline().split()[-1])
     return freq,a2f,cum_epc,int_epc,sum_epc
 
 
 def plot_a2f(args):
-    print ('plot Eliashberg spectral function')
+    print ('Plotting Eliashberg spectral function')
     data=read_a2f(args,args.iso)
     freq=data[0]
     a2f=data[1]
     cum_epc=data[2]
     fig=plt.figure(figsize=args.figsize)
     ax=fig.add_subplot(111)
     ax.set_xlabel('$\omega$ ($meV$)')
     if args.freq_unit=='cm-1':
         print ('transfer unit of frequency to cm-1')
         freq=freq*1e-3/units.THzToEv*units.THzToCm
         ax.set_xlabel('$\omega$ ($cm^{-1}$)')
     ax.set_ylabel('$\\alpha^2F$ ($\omega$), $\lambda$ ($\omega$)')
-    ax.plot(freq,a2f[:,args.ismear],'g-')
+    ax.plot(freq,a2f[:,args.ismear],'g-',label='$\\alpha^2F$ ($\omega$)')
     ax.set_xlim(freq[0],freq[-1])
-    ax.plot(freq,cum_epc,'r--')
+    ax.plot(freq,cum_epc,'r--',label='$\lambda$ ($\omega$)')
+    ax.legend(fontsize=12)
     if args.max_freq>0: ax.set_xlim(0,args.max_freq)
     fig.tight_layout()
     if args.iso: 
        iso='iso'
     else: 
        iso='aniso'
        ph_smearing,el_smearing=get_smearing(args.prefix)
-       print ('ph smearing:{0:8.5f}'.format(ph_smearing[args.ismear]))
-    fig.savefig('{0}_a2f_{1}_{2}'.format(args.prefix,iso,args.ismear),dpi=args.dpi)
+       print ('Phononic smearing:{:8.5f}'.format(ph_smearing[args.ismear]))
+    figname = '{}_a2f_{}_{}'.format(args.prefix,iso,args.ismear)
+    fig.savefig(figname,dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
+
 
 def plot_gap(args):
     print ('plot superconducting gap')
     fil_head='{0}.{1}_aniso_gap0_'.format(args.prefix,args.gtype)
     fils=[fil.rstrip('\n') for fil in os.popen('ls {0}*'.format(fil_head)).readlines()]
     fig=plt.figure(figsize=args.figsize)
     ax=fig.add_subplot(111)
@@ -464,15 +492,19 @@
         nskip={'imag':1,'pade':0}
         data=np.loadtxt(open(fil),skiprows=nskip[args.gtype])
         ax.plot(data[:,0],data[:,1]*1e3,'b-')
         ax.axvline(temp,c='b',alpha=0.8)
     ax.set_xlabel('$T\ \mathrm{(K)}$')
     ax.set_ylabel('$\Delta_{n\\bf{k}}(\omega=0) \mathrm{(meV)}$')
     fig.tight_layout()
-    fig.savefig('{0}_gap_{1}'.format(args.prefix,args.gtype),dpi=args.dpi)
+    figname = '{}_gap_{}'.format(args.prefix,args.gtype)
+    fig.savefig(figname,dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
+
 
 def plot_qpr(args):
     print ('plot quasiparticle renormalization')
     fil_head='{0}.*_aniso_'.format(args.prefix)
     fils=[fil.rstrip('\n') for fil in os.popen('ls {0}*'.format(fil_head)).readlines()]
     rm=[item for item in fils if 'gap' in item]
     for item in rm: fils.remove(item)
@@ -494,15 +526,19 @@
     ax2.set_xlim(0,200)
     ax1.set_ylim(-2,13)
     ax2.set_ylim(-20,33)
     ax2.set_xlabel('$\omega$ (meV)')
     ax1.set_ylabel('$\Delta_{n\\bf{k}}(i\omega)$ ($meV$)')
     ax2.set_ylabel('$\Delta_{n\\bf{k}}(\omega)$ ($meV$)')
     fig.tight_layout()
-    fig.savefig('{0}_qp_renormalization'.format(args.prefix),dpi=args.dpi)
+    fignmae = '{}_qp_renormalization'.format(args.prefix)
+    fig.savefig(figname,dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
+
 
 def plot_qdos(args):
     print ('plot quasiparticle dos')
     fil_head='{0}.qdos_'.format(args.prefix,args.gtype)
     fils=[fil.rstrip('\n') for fil in os.popen('ls {0}*'.format(fil_head)).readlines()]
     fig=plt.figure(figsize=args.figsize)
     ax=fig.add_subplot(111)
@@ -515,15 +551,18 @@
         ax.plot(data[:,0]*1e3,data[:,1],c=colors[i],ls='-',label='T={0}'.format(temp))
     ax.set_xlabel('$\omega$ (meV)')
     ax.set_ylabel('$N_s (\omega) / N(\epsilon_F)$')
     ax.set_xlim(0,10)
     ax.legend(loc='upper left',ncol=2)
     ax.set_title('quasiparticle density of statres')
     fig.tight_layout()
-    fig.savefig('{0}_qdos'.format(args.prefix),dpi=args.dpi)
+    figname = '{0}_qdos'.format(args.prefix)
+    fig.savefig(figname,dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
 
 
 def plot_nest_fn(args):
     lines = os.popen('grep "Adimensional" epw.out').readlines()
     nest=np.array([float(line.split()[3]) for line in lines])
     print ('max value of nesting fn: {0}'.format(np.max(nest)))
     ndim=int(np.sqrt(nest.shape[0]))
@@ -537,15 +576,17 @@
     #print 'extent for plot: ', my_extent
     my_extent=[0,1,0,1]
     cax=ax.imshow(nest,extent=my_extent,origin='lower',cmap=args.cmap)
     ax.set_xlabel('$k_x (2\pi/a)$',fontsize=20)
     ax.set_ylabel('$k_y (2\pi/b)$',fontsize=20)
     fig.colorbar(cax)
     fig.savefig('nest')
-    return fig, ax 
+    if args.show_plot: plt.show()
+    return fig
+
 
 def plot_wan_band(args):
     labels=None
     xsym=None
     #if os.path.isfile('{0}.win'.format(args.seedname)):
     #    get_labels=os.popen('grep -n kpoint_path {0}.win 2>/dev/null'.format(args.seedname)).readlines()
     #    if len(get_labels)>0:
@@ -576,16 +617,17 @@
     else: ax.set_xticks([])
     ax.set_xlim(np.min(data[:,0]),np.max(data[:,0]))
     ax.axhline(args.wan_efermi,c='g',ls='--',lw=1,alpha=0.8,zorder=-1)
     ewin=np.max(data[:,1])-np.min(data[:,1])
     ax.set_ylim(np.min(data[:,1])-ewin*0.1,np.max(data[:,1])+ewin*0.1)
     if args.elim[1]>args.elim[0]: ax.set_ylim(args.elim)
     fig.tight_layout()
-    fig.savefig('epw_wan_band',dpi=400)
-    return fig, ax
+    fig.savefig('epw_wan_band',dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
 
 
 def plot_gap_FS(args):
     fils=os.popen('ls *.imag_aniso_gap_FS*').readlines()
     nrow=int(round(sqrt(len(fils))))
     fig,ax=plt.subplots(nrow,len(fils)/nrow,figsize=args.figsize,sharex=True,sharey=True)
     for ifil,fil in enumerate(fils):
@@ -600,16 +642,18 @@
         ax[i,j].set_xticks([0,1])
         ax[i,j].set_yticks([0,1])
         ax[i,j].set_title('$T =\ \mathrm{'+'{0:5.2f}'.format(float(fil.rstrip('\n').split('_')[-1]))+'}$',fontsize=10)
     fig.subplots_adjust(left=0.1,right=0.85)
     cbar_ax = fig.add_axes([0.9, 0.09, 0.02, 0.8])
     cbar=fig.colorbar(sc, cax=cbar_ax)
     cbar.ax.set_title('$\Delta\ \mathrm{(meV)}$')
-    fig.savefig('gap_FS',dpi=500)
-    return fig,ax
+    fig.savefig('gap_FS',dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
+
 
 def plot_gap_freq(args):
     fils=os.popen('ls *.imag_aniso_0*').readlines()
     nrow=int(round(np.sqrt(len(fils))))
     fig,ax=plt.subplots(nrow,int(len(fils)/nrow),figsize=args.figsize,sharex=True,sharey=True)
     for ifil,fil in enumerate(fils):
         j=int(ifil/nrow)
@@ -617,9 +661,11 @@
         data=np.loadtxt(open(fil.rstrip('\n')),skiprows=1)
         print ('gap range: {0:6.3f} to {1:6.3f} meV'.format(np.min(data[:,3]*1e3),np.max(data[:,3]*1e3)))
         ax[i,j].scatter(data[:,0]*1e3,data[:,3]*1e3,facecolor='g',edgecolor='none',s=2)
         ax[i,j].set_title('$T =\ \mathrm{'+'{0:5.2f}'.format(float(fil.rstrip('\n').split('_')[-1]))+'}$',fontsize=10)
         if i==ax.shape[0]-1:    ax[i,j].set_xlabel('$\omega\ \mathrm{(meV)}$')
         if j==0:    ax[i,j].set_ylabel('$\Delta\ \mathrm{(meV)}$')
     fig.tight_layout()
-    fig.savefig('gap_freq',dpi=500)
-    return fig,ax
+    fig.savefig('gap_freq',dpi=args.dpi)
+    if args.show_plot: plt.show()
+    return fig
+
```

### Comparing `elphtk-0.0.1/elphtk/phonon_plot.py` & `elphtk-0.0.2/elphtk/phonon_plot.py`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/elphtk/qe_phonon.py` & `elphtk-0.0.2/elphtk/qe_phonon.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # related to phonon calculations
 # Shunhong Zhang
 # szhang2@ustc.edu.cn
 # Date: Jun 19, 2020
 #=======================================
 
 
-from __future__ import print_function
 import numpy as np
 import os
 import sys
 import re
 import phonopy.units as units
 from collections import Counter
```

### Comparing `elphtk-0.0.1/elphtk/wgauss.py` & `elphtk-0.0.2/elphtk/wgauss.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # Author: Shunhong Zhang
 # Email: szhang2@ustc.edu.cn'
 # Date: Mar 06, 2020
 #
 #=====================================================================================
 
 
-from __future__ import print_function
 import numpy as np
 from scipy.special import erf,erfc
 
 r2=np.sqrt(2.)
 sqrtpm1=1./np.sqrt(np.pi)
 
 def gauss_freq(x):
```

### Comparing `elphtk-0.0.1/elphtk.egg-info/SOURCES.txt` & `elphtk-0.0.2/elphtk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+setup.cfg
 setup.py
 Examples/README.md
 Examples/example1/FORCE_SETS
+Examples/example1/README
 Examples/example1/band.conf
 Examples/example1/band.yaml
 Examples/example1/phonopy.freq.gp
 Examples/example1/phonopy.yaml
 Examples/example1/phonopy_disp.yaml
+Examples/example2/README
 Examples/example2/ZrN.dyn0
 Examples/example2/ZrN.dyn1
 Examples/example2/ZrN.dyn2
 Examples/example2/ZrN.dyn3
 Examples/example2/ZrN.fc
 Examples/example2/ZrN.freq
 Examples/example2/ZrN.freq.gp
 Examples/example2/matdyn.in
 Examples/example2/ph.in
 Examples/example2/ph.out
 Examples/example2/q2r.in
 Examples/example2/scf.in
 Examples/example2/scf.out
+Examples/example3/README
 Examples/example3/ZrN.a2f
 Examples/example3/ZrN.a2f.01
 Examples/example3/ZrN.a2f_iso
 Examples/example3/ZrN.a2f_tr.01
 Examples/example3/ZrN.kmap
 Examples/example3/ZrN.lambda_FS
 Examples/example3/ZrN.lambda_k_pairs
@@ -36,14 +40,15 @@
 Examples/example3/ZrN.res.01
 Examples/example3/ZrN.win
 Examples/example3/epw.in
 Examples/example3/nscf.in
 Examples/example3/nscf.out
 Examples/example3/scf.in
 Examples/example3/scf.out
+Examples/example4/README
 Examples/example4/freq.txt
 Examples/example4/tmp/ZrN.egnv
 Examples/example4/tmp/ZrN.ephmat1
 Examples/example4/tmp/ZrN.freq
 Examples/example4/tmp/ZrN.ikmap
 elphtk/__init__.py
 elphtk/arguments.py
```

### Comparing `elphtk-0.0.1/scripts/phplot` & `elphtk-0.0.2/scripts/phplot`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #  Dependence: none                                                         #
 #  Usage:      parse data from band.yaml and plot the phonon spectra        #      
 #  Author:     Shunhong Zhang <szhang2@ustc.edu.cn>                         #
 #  Date:       Jan 31, 2020                                                 #
 #                                                                           #
 #===========================================================================#
 
-from __future__ import print_function
 import numpy as np
 import os
 import re
 import phonopy.units as units
 try:    import yaml
 except: ImportError("You need to install python-yaml")
 try:
```

### Comparing `elphtk-0.0.1/scripts/post_epw` & `elphtk-0.0.2/scripts/post_epw`

 * *Files 8% similar despite different names*

```diff
@@ -98,17 +98,17 @@
     parser.add_argument('--imode',type=int,default=0,help='mode index specified for plot')
     parser.add_argument('--iband',type=int,default=0,help='band index specified for plot')
     parser.add_argument('--kmode',type=str,default='mesh',help='mode of kpts, mesh or band')
     args = parser.parse_args()
     return args  
 
 def print_task_list(task_list):
-    print ('\n{0}\nlist of tasks\n{0}'.format('-'*20))
-    print ('\n'.join(['{0}'.format(item) for item in task_list]))
-    print ('{0}\n'.format('-'*20))
+    print ('\n{}\nlist of tasks\n{}'.format('='*20,'-'*20))
+    print ('\n'.join(['{}'.format(item) for item in task_list]))
+    print ('{}\n'.format('='*20))
 
 
 def dryrun():
     print('use --task to specify your task')
 
 
 task_list=[
@@ -127,14 +127,15 @@
 'lambda.phself',
 'specfun',
 'specfun_sup',
 'kgmap',
 'plot_nest_fn',
 'elph',
 'mpi_elph',
+'freq',
 'kqmap_demo',
 None,
 ]
 
 
 def main():
     print ('{0}\n'.format(desc_str))
@@ -155,21 +156,30 @@
     elif args.task=='lambda.phself':    plot_lambda.phself(args)
     elif args.task=='specfun':          plot_specfun(args)
     elif args.task=='specfun_sup':      plot_specfun_sup(args)
     elif args.task=='phdos':            plot_phdos(args)
     elif args.task=='kqmap_demo':       test_kpmq()
     elif args.task=='elph':             read_elph(**kws)
     elif args.task=='mpi_elph':         mpi_read_elph(**kws)
+    elif args.task=='freq':
+        qpts,freqs = read_freq_scipy(**kws)
+        qpts,freqs = read_freq(**kws)
+        write_freq(qpts,freqs)
+    else: exit('Unavaialble taks {} specified!'.format(args.task))
 
 
 
 nqf1,nqf2,nqf3=(12,12,1)
 desc_str = 'post-processing for EPW'
 args=get_args(desc_str)
-kws = dict(outdir=args.outdir,prefix=args.prefix,seedname=args.seedname)
+
+kws = dict(
+outdir=args.outdir,
+prefix=args.prefix,
+seedname=args.seedname)
  
 
 if __name__=='__main__':
     from elphtk import __version__
     from elphtk.pkg_info import verbose_pkg_info
     verbose_pkg_info(__version__)
     print (__note__)
```

### Comparing `elphtk-0.0.1/scripts/qe2epw` & `elphtk-0.0.2/scripts/qe2epw`

 * *Files identical despite different names*

### Comparing `elphtk-0.0.1/scripts/qe_lambda` & `elphtk-0.0.2/scripts/qe_lambda`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 #
 # Shunhong Zhang
 # shzang2@ustc.edu.cn
 # Date: Mar 15, 2020
 #
 #======================================
 
-from __future__ import print_function
 import os
 import numpy as np
 from elphtk.arguments import *
 import pickle
 import glob
 import re
 
+
 def write_lambda_in(fil='lambda.in',mustar=0.1,filph='ph.out',elph_method='interpolated'):
     if elph_method=='interpolated':
         elph_dir='elph_dir'
         elph_prefix='elph.inp_lambda'
         elph_fils=glob.glob('{0}/{1}'.format(elph_dir,elph_prefix))
     qpts,qweights=qe_phonon.get_qpt_from_phout(filph=filph)
     nq=qpts.shape[0]
```

### Comparing `elphtk-0.0.1/setup.py` & `elphtk-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -61,43 +61,26 @@
 scripts_pysupercell = glob.glob('scripts/*')
 
 long_desc="An open-source Python library for phonon-related data processing"
 
 
 kwargs_setup=dict(
 name='elphtk',
-version='0.0.1',
+version='0.0.2',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
-url='',
-download_url='',
+url='https://pypi.org/project/elphtk',
+download_url='https://pypi.org/project/elphtk',
 keywords=['Python','Phonon','Electron-phonon'],
 py_modules=core_modules,
 license="MIT License",
 description='Python library for (electron)-phonon-related analysis',
 long_description=long_desc,
 platforms=[platform.system()],
-install_requires=[
-'numpy',
-'matplotlib',
-'scipy',
-'phonopy',
-'fortio',
-],
-provides=[
-'qe_lambda',
-'phplot',
-'qe2epw',
-'post_epw',
-],
-scripts=scripts_pysupercell,
 )
 
 
 if __name__=='__main__':
-    print ('{0}\nOperating System: {1}'.format('-'*50,platform.system()))
-    print ('\n{0}\nINSTALL\n{0}\n'.format('-'*50))
-    setup(**kwargs_setup)
-    print ('{0}'.format('-'*50))
+    #setup(**kwargs_setup)
+    setup()
     write_code_info(kwargs_setup)
     test_modules(core_modules,'core modules')
-    print ('\n{0}\nDone\n{0}\n'.format('-'*50))
```


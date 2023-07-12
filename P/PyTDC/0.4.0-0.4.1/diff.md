# Comparing `tmp/PyTDC-0.4.0.tar.gz` & `tmp/PyTDC-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTDC-0.4.0.tar", last modified: Mon Apr 17 23:34:18 2023, max compression
+gzip compressed data, was "PyTDC-0.4.1.tar", last modified: Wed Jul 12 05:43:41 2023, max compression
```

## Comparing `PyTDC-0.4.0.tar` & `PyTDC-0.4.1.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.132928 PyTDC-0.4.0/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1069 2023-04-15 16:25:42.000000 PyTDC-0.4.0/LICENSE
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      102 2023-04-15 16:25:42.000000 PyTDC-0.4.0/MANIFEST.in
--rw-r--r--   0 kexinhuang   (502) staff       (20)    17667 2023-04-17 23:34:18.133002 PyTDC-0.4.0/PKG-INFO
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.125131 PyTDC-0.4.0/PyTDC.egg-info/
--rw-r--r--   0 kexinhuang   (502) staff       (20)    17667 2023-04-17 23:34:17.000000 PyTDC-0.4.0/PyTDC.egg-info/PKG-INFO
--rw-r--r--   0 kexinhuang   (502) staff       (20)     2170 2023-04-17 23:34:18.000000 PyTDC-0.4.0/PyTDC.egg-info/SOURCES.txt
--rw-r--r--   0 kexinhuang   (502) staff       (20)        1 2023-04-17 23:34:17.000000 PyTDC-0.4.0/PyTDC.egg-info/dependency_links.txt
--rw-r--r--   0 kexinhuang   (502) staff       (20)        1 2023-04-17 23:34:17.000000 PyTDC-0.4.0/PyTDC.egg-info/not-zip-safe
--rw-r--r--   0 kexinhuang   (502) staff       (20)       98 2023-04-17 23:34:18.000000 PyTDC-0.4.0/PyTDC.egg-info/requires.txt
--rw-r--r--   0 kexinhuang   (502) staff       (20)        4 2023-04-17 23:34:18.000000 PyTDC-0.4.0/PyTDC.egg-info/top_level.txt
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    17381 2023-04-15 16:25:42.000000 PyTDC-0.4.0/README.md
--rw-rw-r--   0 kexinhuang   (502) staff       (20)       98 2023-04-15 16:25:42.000000 PyTDC-0.4.0/requirements.txt
--rw-rw-r--   0 kexinhuang   (502) staff       (20)       79 2023-04-17 23:34:18.133275 PyTDC-0.4.0/setup.cfg
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1141 2023-04-15 16:25:42.000000 PyTDC-0.4.0/setup.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.126037 PyTDC-0.4.0/tdc/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      147 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     8277 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/base_dataset.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    21837 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_deprecated.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.126673 PyTDC-0.4.0/tdc/benchmark_group/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      162 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_group/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      449 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_group/admet_group.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    10178 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_group/base_group.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    15827 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_group/docking_group.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      441 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_group/drugcombo_group.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      453 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/benchmark_group/dti_dg_group.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.126881 PyTDC-0.4.0/tdc/chem_utils/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1021 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    13620 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/evaluator.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.127450 PyTDC-0.4.0/tdc/chem_utils/featurize/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)        0 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/featurize/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    28488 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/featurize/_smartsPatts.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    23693 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/featurize/_smiles2pubchem.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    21707 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/featurize/_xyz2mol.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    27045 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/featurize/molconvert.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.127860 PyTDC-0.4.0/tdc/chem_utils/oracle/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)        0 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/oracle/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1121 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/oracle/docking.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     6080 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/oracle/filter.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    59584 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/chem_utils/oracle/oracle.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    15901 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/evaluator.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.128712 PyTDC-0.4.0/tdc/generation/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      112 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     3750 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/bi_generation_dataset.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     9843 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/generation_dataset.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      817 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/ligandmolgen.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      993 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/molgen.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1147 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/reaction.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     2508 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/retrosyn.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     5776 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/generation/sbdd.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    27239 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/metadata.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.130224 PyTDC-0.4.0/tdc/multi_pred/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      348 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1492 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/antibodyaff.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    13146 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/bi_pred_dataset.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1404 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/catalyst.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1985 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/ddi.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1944 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/drugres.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1239 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/drugsyn.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     3034 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/dti.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1457 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/gda.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1502 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/mti.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     4028 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/multi_pred_dataset.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1545 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/peptidemhc.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     2008 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/ppi.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1253 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/tcr_epi.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1164 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/multi_pred/test_multi_pred.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    25879 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/oracles.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.130453 PyTDC-0.4.0/tdc/resource/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)       29 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/resource/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1321 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/resource/primekg.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.131871 PyTDC-0.4.0/tdc/single_pred/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      287 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     4106 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/adme.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1561 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/crispr_outcome.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     5632 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/develop.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1555 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/epitope.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1474 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/hts.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1560 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/paratope.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1588 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/qm.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     6783 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/single_pred_dataset.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1485 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/test_single_pred.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1518 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/tox.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1584 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/single_pred/yields.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     3327 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/tdc_hf.py
-drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-04-17 23:34:18.132826 PyTDC-0.4.0/tdc/utils/
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     1072 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/__init__.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     8168 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/label.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    19104 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/label_name_list.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    36203 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/load.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     3398 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/misc.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     3054 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/query.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)     3563 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/retrieve.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)    12788 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/utils/split.py
--rw-rw-r--   0 kexinhuang   (502) staff       (20)      535 2023-04-15 16:25:42.000000 PyTDC-0.4.0/tdc/version.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-07-12 05:43:41.691641 PyTDC-0.4.1/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1069 2023-07-11 06:01:10.000000 PyTDC-0.4.1/LICENSE
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      102 2023-07-11 06:01:10.000000 PyTDC-0.4.1/MANIFEST.in
+-rw-r--r--   0 kexinhuang   (502) staff       (20)    17667 2023-07-12 05:43:41.691725 PyTDC-0.4.1/PKG-INFO
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-07-12 05:43:41.683700 PyTDC-0.4.1/PyTDC.egg-info/
+-rw-r--r--   0 kexinhuang   (502) staff       (20)    17667 2023-07-12 05:43:41.000000 PyTDC-0.4.1/PyTDC.egg-info/PKG-INFO
+-rw-r--r--   0 kexinhuang   (502) staff       (20)     2201 2023-07-12 05:43:41.000000 PyTDC-0.4.1/PyTDC.egg-info/SOURCES.txt
+-rw-r--r--   0 kexinhuang   (502) staff       (20)        1 2023-07-12 05:43:41.000000 PyTDC-0.4.1/PyTDC.egg-info/dependency_links.txt
+-rw-r--r--   0 kexinhuang   (502) staff       (20)        1 2023-07-12 05:43:41.000000 PyTDC-0.4.1/PyTDC.egg-info/not-zip-safe
+-rw-r--r--   0 kexinhuang   (502) staff       (20)       98 2023-07-12 05:43:41.000000 PyTDC-0.4.1/PyTDC.egg-info/requires.txt
+-rw-r--r--   0 kexinhuang   (502) staff       (20)        4 2023-07-12 05:43:41.000000 PyTDC-0.4.1/PyTDC.egg-info/top_level.txt
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    17381 2023-07-11 06:01:10.000000 PyTDC-0.4.1/README.md
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)       98 2023-07-11 06:01:10.000000 PyTDC-0.4.1/requirements.txt
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)       79 2023-07-12 05:43:41.692005 PyTDC-0.4.1/setup.cfg
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1141 2023-07-11 06:01:10.000000 PyTDC-0.4.1/setup.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-07-12 05:43:41.684601 PyTDC-0.4.1/tdc/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      147 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     8277 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/base_dataset.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    21837 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/benchmark_deprecated.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-07-12 05:43:41.685245 PyTDC-0.4.1/tdc/benchmark_group/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      162 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/benchmark_group/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      449 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/benchmark_group/admet_group.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    10178 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/benchmark_group/base_group.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    15827 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/benchmark_group/docking_group.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      759 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/benchmark_group/drugcombo_group.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      453 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/benchmark_group/dti_dg_group.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-07-12 05:43:41.685466 PyTDC-0.4.1/tdc/chem_utils/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1021 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/chem_utils/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    13620 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/chem_utils/evaluator.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-07-12 05:43:41.686024 PyTDC-0.4.1/tdc/chem_utils/featurize/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)        0 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/chem_utils/featurize/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    28488 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/chem_utils/featurize/_smartsPatts.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    23693 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/chem_utils/featurize/_smiles2pubchem.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    21707 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/chem_utils/featurize/_xyz2mol.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    27045 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/chem_utils/featurize/molconvert.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-07-12 05:43:41.686450 PyTDC-0.4.1/tdc/chem_utils/oracle/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)        0 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/chem_utils/oracle/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1121 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/chem_utils/oracle/docking.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     6080 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/chem_utils/oracle/filter.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    59584 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/chem_utils/oracle/oracle.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    15901 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/evaluator.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-07-12 05:43:41.687314 PyTDC-0.4.1/tdc/generation/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      112 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/generation/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     3750 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/generation/bi_generation_dataset.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     9843 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/generation/generation_dataset.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      817 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/generation/ligandmolgen.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      993 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/generation/molgen.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1147 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/generation/reaction.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     2508 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/generation/retrosyn.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     5776 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/generation/sbdd.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    27647 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/metadata.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-07-12 05:43:41.688979 PyTDC-0.4.1/tdc/multi_pred/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      387 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1492 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/antibodyaff.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    13146 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/bi_pred_dataset.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1404 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/catalyst.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1985 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/ddi.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1944 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/drugres.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1239 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/drugsyn.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     3034 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/dti.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1457 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/gda.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1502 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/mti.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     4028 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/multi_pred_dataset.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1545 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/peptidemhc.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     2008 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/ppi.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1253 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/tcr_epi.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1164 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/test_multi_pred.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1564 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/multi_pred/trialoutcome.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    25879 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/oracles.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-07-12 05:43:41.689182 PyTDC-0.4.1/tdc/resource/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)       29 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/resource/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1321 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/resource/primekg.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-07-12 05:43:41.690445 PyTDC-0.4.1/tdc/single_pred/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      287 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/single_pred/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     4106 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/single_pred/adme.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1561 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/single_pred/crispr_outcome.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     5632 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/single_pred/develop.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1555 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/single_pred/epitope.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1474 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/single_pred/hts.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1560 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/single_pred/paratope.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1588 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/single_pred/qm.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     6783 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/single_pred/single_pred_dataset.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1485 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/single_pred/test_single_pred.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1518 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/single_pred/tox.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1584 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/single_pred/yields.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     3327 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/tdc_hf.py
+drwxr-xr-x   0 kexinhuang   (502) staff       (20)        0 2023-07-12 05:43:41.691511 PyTDC-0.4.1/tdc/utils/
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     1072 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/utils/__init__.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     8168 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/utils/label.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    19104 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/utils/label_name_list.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    36203 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/utils/load.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     3398 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/utils/misc.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     3054 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/utils/query.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)     3563 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/utils/retrieve.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)    12788 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/utils/split.py
+-rw-rw-r--   0 kexinhuang   (502) staff       (20)      535 2023-07-11 06:01:10.000000 PyTDC-0.4.1/tdc/version.py
```

### Comparing `PyTDC-0.4.0/LICENSE` & `PyTDC-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/PKG-INFO` & `PyTDC-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTDC
-Version: 0.4.0
+Version: 0.4.1
 Summary: Therapeutics Data Commons
 Home-page: https://github.com/mims-harvard/TDC
 Author: TDC Team
 Author-email: kexinhuang@hsph.harvard.edu
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PyTDC-0.4.0/PyTDC.egg-info/PKG-INFO` & `PyTDC-0.4.1/PyTDC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTDC
-Version: 0.4.0
+Version: 0.4.1
 Summary: Therapeutics Data Commons
 Home-page: https://github.com/mims-harvard/TDC
 Author: TDC Team
 Author-email: kexinhuang@hsph.harvard.edu
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PyTDC-0.4.0/PyTDC.egg-info/SOURCES.txt` & `PyTDC-0.4.1/PyTDC.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 tdc/multi_pred/gda.py
 tdc/multi_pred/mti.py
 tdc/multi_pred/multi_pred_dataset.py
 tdc/multi_pred/peptidemhc.py
 tdc/multi_pred/ppi.py
 tdc/multi_pred/tcr_epi.py
 tdc/multi_pred/test_multi_pred.py
+tdc/multi_pred/trialoutcome.py
 tdc/resource/__init__.py
 tdc/resource/primekg.py
 tdc/single_pred/__init__.py
 tdc/single_pred/adme.py
 tdc/single_pred/crispr_outcome.py
 tdc/single_pred/develop.py
 tdc/single_pred/epitope.py
```

### Comparing `PyTDC-0.4.0/README.md` & `PyTDC-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/setup.py` & `PyTDC-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/base_dataset.py` & `PyTDC-0.4.1/tdc/base_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/benchmark_deprecated.py` & `PyTDC-0.4.1/tdc/benchmark_deprecated.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/benchmark_group/base_group.py` & `PyTDC-0.4.1/tdc/benchmark_group/base_group.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/benchmark_group/docking_group.py` & `PyTDC-0.4.1/tdc/benchmark_group/docking_group.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/chem_utils/__init__.py` & `PyTDC-0.4.1/tdc/chem_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/chem_utils/evaluator.py` & `PyTDC-0.4.1/tdc/chem_utils/evaluator.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/chem_utils/featurize/_smartsPatts.py` & `PyTDC-0.4.1/tdc/chem_utils/featurize/_smartsPatts.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/chem_utils/featurize/_smiles2pubchem.py` & `PyTDC-0.4.1/tdc/chem_utils/featurize/_smiles2pubchem.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/chem_utils/featurize/_xyz2mol.py` & `PyTDC-0.4.1/tdc/chem_utils/featurize/_xyz2mol.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/chem_utils/featurize/molconvert.py` & `PyTDC-0.4.1/tdc/chem_utils/featurize/molconvert.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/chem_utils/oracle/docking.py` & `PyTDC-0.4.1/tdc/chem_utils/oracle/docking.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/chem_utils/oracle/filter.py` & `PyTDC-0.4.1/tdc/chem_utils/oracle/filter.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/chem_utils/oracle/oracle.py` & `PyTDC-0.4.1/tdc/chem_utils/oracle/oracle.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/evaluator.py` & `PyTDC-0.4.1/tdc/evaluator.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/generation/bi_generation_dataset.py` & `PyTDC-0.4.1/tdc/generation/bi_generation_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/generation/generation_dataset.py` & `PyTDC-0.4.1/tdc/generation/generation_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/generation/ligandmolgen.py` & `PyTDC-0.4.1/tdc/generation/ligandmolgen.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/generation/molgen.py` & `PyTDC-0.4.1/tdc/generation/molgen.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/generation/reaction.py` & `PyTDC-0.4.1/tdc/generation/reaction.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/generation/retrosyn.py` & `PyTDC-0.4.1/tdc/generation/retrosyn.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/generation/sbdd.py` & `PyTDC-0.4.1/tdc/generation/sbdd.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/metadata.py` & `PyTDC-0.4.1/tdc/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,16 @@
 
 yield_dataset_names = ["uspto_yields", "buchwald-hartwig"]
 
 catalyst_dataset_names = ["uspto_catalyst"]
 
 tcr_epi_dataset_names = ["weber"]
 
+trial_outcome_dataset_names = ['phase1', 'phase2', 'phase3']
+
 ####################################
 # generation
 
 
 retrosyn_dataset_names = ["uspto50k", "uspto"]
 
 forwardsyn_dataset_names = ["uspto"]
@@ -551,14 +553,15 @@
         "DrugRes",
         "AntibodyAff",
         "DrugSyn",
         "MTI",
         "GDA",
         "Catalyst",
         "TCR_Epitope_Binding",
+        "TrialOutcome", 
     ],
     "generation": ["RetroSyn", "Reaction", "MolGen"],
 }
 
 
 def get_task2category():
     task2category = {}
@@ -590,15 +593,16 @@
     "GDA": gda_dataset_names,
     "Paratope": paratope_dataset_names,
     "Yields": yield_dataset_names,
     "Catalyst": catalyst_dataset_names,
     "CRISPROutcome": crisproutcome_dataset_names,
     "test_single_pred": test_single_pred_dataset_names,
     "test_multi_pred": test_multi_pred_dataset_names,
-    "TCREpitopeBinding": tcr_epi_dataset_names,
+    "TCREpitopeBinding": tcr_epi_dataset_names, 
+    "TrialOutcome": trial_outcome_dataset_names, 
 }
 
 benchmark_names = {
     "admet_group": admet_benchmark,
     "drugcombo_group": drugsyn_benchmark,
     "docking_group": docking_benchmark,
     "dti_dg_group": dti_dg_benchmark,
@@ -723,14 +727,18 @@
     "test_single_pred": "tab",
     "test_multi_pred": "tab",
     "gdsc_gene_symbols": "tab",
     "weber": "tab",
     "primekg": "tab",
     "primekg_drug_feature": "tab",
     "primekg_disease_feature": "tab",
+    "drug_comb_meta_data": "pkl", 
+    "phase1": "tab",
+    "phase2": "tab", 
+    "phase3": "tab",  
 }
 
 name2id = {
     "bbb_adenot": 4259565,
     "bbb_martins": 4259566,
     "bindingdb_ic50": 4291560,
     "bindingdb_kd": 4291555,
@@ -831,14 +839,18 @@
     "test_single_pred": 4832455,
     "test_multi_pred": 4832456,
     "gdsc_gene_symbols": 5255026,
     "weber": 5790963,
     "primekg": 6180626,
     "primekg_drug_feature": 6180619,
     "primekg_disease_feature": 6180618,
+    "drug_comb_meta_data": 7104245, 
+    "phase1": 7163779, 
+    "phase2": 7163778, 
+    "phase3": 7163780, 
 }
 
 oracle2type = {
     "drd2": "pkl",
     "jnk3": "pkl",
     "gsk3b": "pkl",
     "fpscores": "pkl",
@@ -956,13 +968,16 @@
     "mirtarbase": 400082,
     "uspto_catalyst": 721799,
     "moses": 1936962,
     "zinc": 249455,
     "chembl": 1961462,
     "uspto50k": 50036,
     "uspto": 1939253,
+    "phase1": 1787,
+    "phase2": 6102,
+    "phase3": 4576,
 }
 
 name2idlist = {
     "dude": [6429245, 6429251],
     "scpdb": [6431629, 6431631],
 }
```

### Comparing `PyTDC-0.4.0/tdc/multi_pred/antibodyaff.py` & `PyTDC-0.4.1/tdc/multi_pred/antibodyaff.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/multi_pred/bi_pred_dataset.py` & `PyTDC-0.4.1/tdc/multi_pred/bi_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/multi_pred/catalyst.py` & `PyTDC-0.4.1/tdc/multi_pred/catalyst.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/multi_pred/ddi.py` & `PyTDC-0.4.1/tdc/multi_pred/ddi.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/multi_pred/drugres.py` & `PyTDC-0.4.1/tdc/multi_pred/drugres.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/multi_pred/drugsyn.py` & `PyTDC-0.4.1/tdc/multi_pred/drugsyn.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/multi_pred/dti.py` & `PyTDC-0.4.1/tdc/multi_pred/dti.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/multi_pred/gda.py` & `PyTDC-0.4.1/tdc/multi_pred/gda.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/multi_pred/mti.py` & `PyTDC-0.4.1/tdc/multi_pred/mti.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/multi_pred/multi_pred_dataset.py` & `PyTDC-0.4.1/tdc/multi_pred/multi_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/multi_pred/peptidemhc.py` & `PyTDC-0.4.1/tdc/multi_pred/peptidemhc.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/multi_pred/ppi.py` & `PyTDC-0.4.1/tdc/multi_pred/ppi.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/multi_pred/tcr_epi.py` & `PyTDC-0.4.1/tdc/multi_pred/tcr_epi.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/multi_pred/test_multi_pred.py` & `PyTDC-0.4.1/tdc/multi_pred/test_multi_pred.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/oracles.py` & `PyTDC-0.4.1/tdc/oracles.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/resource/primekg.py` & `PyTDC-0.4.1/tdc/resource/primekg.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/single_pred/adme.py` & `PyTDC-0.4.1/tdc/single_pred/adme.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/single_pred/crispr_outcome.py` & `PyTDC-0.4.1/tdc/single_pred/crispr_outcome.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/single_pred/develop.py` & `PyTDC-0.4.1/tdc/single_pred/develop.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/single_pred/epitope.py` & `PyTDC-0.4.1/tdc/single_pred/epitope.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/single_pred/hts.py` & `PyTDC-0.4.1/tdc/single_pred/hts.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/single_pred/paratope.py` & `PyTDC-0.4.1/tdc/single_pred/paratope.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/single_pred/qm.py` & `PyTDC-0.4.1/tdc/single_pred/qm.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/single_pred/single_pred_dataset.py` & `PyTDC-0.4.1/tdc/single_pred/single_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/single_pred/test_single_pred.py` & `PyTDC-0.4.1/tdc/single_pred/test_single_pred.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/single_pred/tox.py` & `PyTDC-0.4.1/tdc/single_pred/tox.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/single_pred/yields.py` & `PyTDC-0.4.1/tdc/single_pred/yields.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/tdc_hf.py` & `PyTDC-0.4.1/tdc/tdc_hf.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/utils/__init__.py` & `PyTDC-0.4.1/tdc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/utils/label.py` & `PyTDC-0.4.1/tdc/utils/label.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/utils/label_name_list.py` & `PyTDC-0.4.1/tdc/utils/label_name_list.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/utils/load.py` & `PyTDC-0.4.1/tdc/utils/load.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/utils/misc.py` & `PyTDC-0.4.1/tdc/utils/misc.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/utils/query.py` & `PyTDC-0.4.1/tdc/utils/query.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/utils/retrieve.py` & `PyTDC-0.4.1/tdc/utils/retrieve.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/utils/split.py` & `PyTDC-0.4.1/tdc/utils/split.py`

 * *Files identical despite different names*

### Comparing `PyTDC-0.4.0/tdc/version.py` & `PyTDC-0.4.1/tdc/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.4.0"  # pragma: no cover
+__version__ = "0.4.1"  # pragma: no cover
```


# Comparing `tmp/siman-1.3.3.tar.gz` & `tmp/siman-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siman-1.3.3.tar", last modified: Mon Jul 10 09:36:03 2023, max compression
+gzip compressed data, was "dist/siman-1.3.4.tar", last modified: Wed Jul 12 15:48:56 2023, max compression
```

## Comparing `siman-1.3.3.tar` & `siman-1.3.4.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.473662 siman-1.3.3/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.3/LICENSE
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.3/MANIFEST.in
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-10 09:36:03.473662 siman-1.3.3/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.3/README.md
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-07-10 09:36:03.473662 siman-1.3.3/setup.cfg
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-07-10 09:35:57.000000 siman-1.3.3/setup.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.471662 siman-1.3.3/siman/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2022-03-05 17:22:57.000000 siman-1.3.3/siman/3d_plot.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2022-03-05 17:22:57.000000 siman-1.3.3/siman/SSHTools.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)       32 2021-02-17 13:28:25.000000 siman-1.3.3/siman/__init__.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49648 2023-06-26 19:04:41.000000 siman-1.3.3/siman/analysis.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2022-03-05 17:22:57.000000 siman-1.3.3/siman/analysis_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.471662 siman-1.3.3/siman/analyze/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.3/siman/analyze/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.3/siman/analyze/segregation.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2022-03-05 17:22:57.000000 siman-1.3.3/siman/approximation.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2022-03-05 17:22:57.000000 siman-1.3.3/siman/bands.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   126491 2023-06-26 19:03:27.000000 siman-1.3.3/siman/calc_manage.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2022-03-05 17:22:57.000000 siman-1.3.3/siman/calcul.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.472662 siman-1.3.3/siman/calculators/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.3/siman/calculators/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.3/siman/calculators/aims.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.3/siman/calculators/gaussian.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.3/siman/calculators/qe.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56510 2023-04-04 10:46:17.000000 siman-1.3.3/siman/calculators/vasp.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.3/siman/calculators/vasp_old.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.472662 siman-1.3.3/siman/chg/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.3/siman/chg/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.3/siman/chg/chg_func.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.3/siman/chg/vasputil_chgarith_module.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    11072 2022-09-20 15:22:50.000000 siman-1.3.3/siman/classes.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.473662 siman-1.3.3/siman/core/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.3/siman/core/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53311 2023-07-10 09:35:43.000000 siman-1.3.3/siman/core/calculation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.3/siman/core/calculation_old.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33337 2023-02-13 17:12:02.000000 siman-1.3.3/siman/core/cluster_batch_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.3.3/siman/core/cluster_run_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2127 2022-09-20 15:22:50.000000 siman-1.3.3/siman/core/molecule.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   118275 2023-06-08 13:38:57.000000 siman-1.3.3/siman/core/structure.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    20203 2023-06-26 18:28:07.000000 siman-1.3.3/siman/database.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2022-03-05 17:22:57.000000 siman-1.3.3/siman/default_project_conf.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2022-03-05 17:22:57.000000 siman-1.3.3/siman/dev_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    32406 2022-12-09 18:12:22.000000 siman-1.3.3/siman/dos_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2022-03-05 17:22:57.000000 siman-1.3.3/siman/fit_hex.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-05-24 11:04:51.000000 siman-1.3.3/siman/functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   113841 2023-03-06 17:27:57.000000 siman-1.3.3/siman/geo.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    14499 2023-06-01 09:41:19.000000 siman-1.3.3/siman/header.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      286 2022-03-05 17:22:57.000000 siman-1.3.3/siman/helper_for_writing_beatiful_code.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    40223 2022-09-20 15:22:50.000000 siman-1.3.3/siman/impurity.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    80578 2023-07-03 11:35:20.000000 siman-1.3.3/siman/inout.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2022-03-05 17:22:57.000000 siman-1.3.3/siman/kpoints_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.473662 siman-1.3.3/siman/mat_prop/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.3/siman/mat_prop/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.3/siman/mat_prop/mat_prop.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    45055 2022-09-29 10:57:16.000000 siman-1.3.3/siman/matproj_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2022-09-20 15:22:50.000000 siman-1.3.3/siman/monte.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      980 2022-03-05 17:22:57.000000 siman-1.3.3/siman/monte_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31643 2022-09-20 15:22:50.000000 siman-1.3.3/siman/neb.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2021-02-17 13:28:25.000000 siman-1.3.3/siman/pairs.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49712 2023-01-25 18:10:57.000000 siman-1.3.3/siman/picture_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2022-03-05 17:22:57.000000 siman-1.3.3/siman/plot_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-06-08 13:41:02.000000 siman-1.3.3/siman/polaron.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2022-03-05 17:22:57.000000 siman-1.3.3/siman/polaron_hop.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2022-09-29 10:57:16.000000 siman-1.3.3/siman/polaron_mod.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   194580 2022-09-29 10:57:16.000000 siman-1.3.3/siman/project_funcs.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2022-03-05 17:22:57.000000 siman-1.3.3/siman/properties_2d.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2022-03-05 17:22:57.000000 siman-1.3.3/siman/properties_energy.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2022-03-05 17:22:57.000000 siman-1.3.3/siman/properties_lattice.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    30666 2023-04-04 10:53:58.000000 siman-1.3.3/siman/set_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2022-03-05 17:22:57.000000 siman-1.3.3/siman/simanrc.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      174 2022-03-05 17:22:57.000000 siman-1.3.3/siman/small_classes.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     6565 2022-09-29 10:57:16.000000 siman-1.3.3/siman/small_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2022-03-05 17:22:57.000000 siman-1.3.3/siman/structure_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2022-03-05 17:22:57.000000 siman-1.3.3/siman/table_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2022-03-05 17:22:57.000000 siman-1.3.3/siman/thermo.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2022-03-05 17:22:57.000000 siman-1.3.3/siman/workflow_utilities.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-10 09:36:03.471662 siman-1.3.3/siman.egg-info/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-10 09:36:03.000000 siman-1.3.3/siman.egg-info/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-07-10 09:36:03.000000 siman-1.3.3/siman.egg-info/SOURCES.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-07-10 09:36:03.000000 siman-1.3.3/siman.egg-info/dependency_links.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-07-10 09:36:03.000000 siman-1.3.3/siman.egg-info/requires.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-07-10 09:36:03.000000 siman-1.3.3/siman.egg-info/top_level.txt
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.846702 siman-1.3.4/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.4/LICENSE
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.4/MANIFEST.in
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-12 15:48:56.846702 siman-1.3.4/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.4/README.md
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-07-12 15:48:56.846702 siman-1.3.4/setup.cfg
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-07-12 15:48:51.000000 siman-1.3.4/setup.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.844702 siman-1.3.4/siman/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2022-03-05 17:22:57.000000 siman-1.3.4/siman/3d_plot.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2022-03-05 17:22:57.000000 siman-1.3.4/siman/SSHTools.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)       32 2021-02-17 13:28:25.000000 siman-1.3.4/siman/__init__.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49648 2023-07-12 15:40:54.000000 siman-1.3.4/siman/analysis.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2022-03-05 17:22:57.000000 siman-1.3.4/siman/analysis_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.844702 siman-1.3.4/siman/analyze/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.4/siman/analyze/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.4/siman/analyze/segregation.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2022-03-05 17:22:57.000000 siman-1.3.4/siman/approximation.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2022-03-05 17:22:57.000000 siman-1.3.4/siman/bands.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   122152 2023-07-12 15:40:43.000000 siman-1.3.4/siman/calc_manage.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   127097 2023-07-12 15:40:43.000000 siman-1.3.4/siman/calc_manage_AB.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2022-03-05 17:22:57.000000 siman-1.3.4/siman/calcul.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.845702 siman-1.3.4/siman/calculators/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.4/siman/calculators/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.4/siman/calculators/aims.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.4/siman/calculators/gaussian.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.4/siman/calculators/qe.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56510 2023-07-12 15:40:54.000000 siman-1.3.4/siman/calculators/vasp.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.4/siman/calculators/vasp_old.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.845702 siman-1.3.4/siman/chg/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.4/siman/chg/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.4/siman/chg/chg_func.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.4/siman/chg/vasputil_chgarith_module.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    11072 2023-07-12 15:40:54.000000 siman-1.3.4/siman/classes.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.846702 siman-1.3.4/siman/core/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.4/siman/core/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53311 2023-07-12 15:40:54.000000 siman-1.3.4/siman/core/calculation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.4/siman/core/calculation_old.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33337 2023-07-12 15:40:54.000000 siman-1.3.4/siman/core/cluster_batch_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.3.4/siman/core/cluster_run_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2127 2022-09-20 15:22:50.000000 siman-1.3.4/siman/core/molecule.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   118466 2023-07-12 08:46:06.000000 siman-1.3.4/siman/core/structure.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    20203 2023-07-12 08:46:06.000000 siman-1.3.4/siman/database.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2022-03-05 17:22:57.000000 siman-1.3.4/siman/default_project_conf.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2022-03-05 17:22:57.000000 siman-1.3.4/siman/dev_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    32406 2023-07-12 15:40:54.000000 siman-1.3.4/siman/dos_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2022-03-05 17:22:57.000000 siman-1.3.4/siman/fit_hex.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-07-12 08:46:06.000000 siman-1.3.4/siman/functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   113841 2023-07-12 15:40:54.000000 siman-1.3.4/siman/geo.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    14530 2023-07-12 15:40:54.000000 siman-1.3.4/siman/header.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      286 2022-03-05 17:22:57.000000 siman-1.3.4/siman/helper_for_writing_beatiful_code.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    40223 2023-07-12 15:40:54.000000 siman-1.3.4/siman/impurity.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    86006 2023-07-12 15:40:43.000000 siman-1.3.4/siman/inout.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2022-03-05 17:22:57.000000 siman-1.3.4/siman/kpoints_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.846702 siman-1.3.4/siman/mat_prop/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.4/siman/mat_prop/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.4/siman/mat_prop/mat_prop.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    45055 2023-07-12 15:40:54.000000 siman-1.3.4/siman/matproj_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2022-09-20 15:22:50.000000 siman-1.3.4/siman/monte.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      980 2022-03-05 17:22:57.000000 siman-1.3.4/siman/monte_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31643 2022-09-20 15:22:50.000000 siman-1.3.4/siman/neb.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2021-02-17 13:28:25.000000 siman-1.3.4/siman/pairs.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49712 2023-07-12 08:46:06.000000 siman-1.3.4/siman/picture_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2022-03-05 17:22:57.000000 siman-1.3.4/siman/plot_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-12 08:46:06.000000 siman-1.3.4/siman/polaron.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2022-03-05 17:22:57.000000 siman-1.3.4/siman/polaron_hop.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2022-09-29 10:57:16.000000 siman-1.3.4/siman/polaron_mod.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   194580 2022-09-29 10:57:16.000000 siman-1.3.4/siman/project_funcs.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2022-03-05 17:22:57.000000 siman-1.3.4/siman/properties_2d.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2022-03-05 17:22:57.000000 siman-1.3.4/siman/properties_energy.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2022-03-05 17:22:57.000000 siman-1.3.4/siman/properties_lattice.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    30666 2023-07-12 15:40:54.000000 siman-1.3.4/siman/set_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2022-03-05 17:22:57.000000 siman-1.3.4/siman/simanrc.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      174 2022-03-05 17:22:57.000000 siman-1.3.4/siman/small_classes.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     6565 2022-09-29 10:57:16.000000 siman-1.3.4/siman/small_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2022-03-05 17:22:57.000000 siman-1.3.4/siman/structure_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2022-03-05 17:22:57.000000 siman-1.3.4/siman/table_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2022-03-05 17:22:57.000000 siman-1.3.4/siman/thermo.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2022-03-05 17:22:57.000000 siman-1.3.4/siman/workflow_utilities.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-12 15:48:56.844702 siman-1.3.4/siman.egg-info/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-12 15:48:56.000000 siman-1.3.4/siman.egg-info/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1701 2023-07-12 15:48:56.000000 siman-1.3.4/siman.egg-info/SOURCES.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-07-12 15:48:56.000000 siman-1.3.4/siman.egg-info/dependency_links.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-07-12 15:48:56.000000 siman-1.3.4/siman.egg-info/requires.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-07-12 15:48:56.000000 siman-1.3.4/siman.egg-info/top_level.txt
```

### Comparing `siman-1.3.3/LICENSE` & `siman-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/PKG-INFO` & `siman-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.3
+Version: 1.3.4
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.3/setup.py` & `siman-1.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="siman",
-    version="1.3.3",
+    version="1.3.4",
     author="Dmitry Aksenov",
     author_email="dimonaks@gmail.com",
     description="Manager for DFT calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dimonaks/siman",
     license = 'GPL',
```

### Comparing `siman-1.3.3/siman/3d_plot.py` & `siman-1.3.4/siman/3d_plot.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/SSHTools.py` & `siman-1.3.4/siman/SSHTools.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/analysis.py` & `siman-1.3.4/siman/analysis.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/analysis_functions.py` & `siman-1.3.4/siman/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/analyze/segregation.py` & `siman-1.3.4/siman/analyze/segregation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/approximation.py` & `siman-1.3.4/siman/approximation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/bands.py` & `siman-1.3.4/siman/bands.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/calc_manage.py` & `siman-1.3.4/siman/calc_manage_AB.py`

 * *Files 0% similar despite different names*

```diff
@@ -1055,16 +1055,16 @@
         #print(calc_method)
         #sys.exit()
         if calc_method and ('c_scale' in calc_method or 'scale' in calc_method or 'uniform_scale' in calc_method):
             #print('Scale')
             #sys.exit()
             if 'uniform_scale' in calc_method:
                 u_scale_flag = True
-
                 it_new = it+'.su' #scale uniformly  
+
             elif 'c_scale' in calc_method:
                 it_new = it+'.sc' #scale along c
                 u_scale_flag = True
             else:
                 it_new = it+'.sm' #scale according to mul_matrix
                 #may not work correctly 
 
@@ -1133,27 +1133,28 @@
                     st = smart_structure_read(curver = v, input_folder = struct_des[it].sfolder+'/'+it, 
                         input_geo_format = input_geo_format, input_geo_file = input_geo_file)
                     pname = st.name
 
                 st = copy.deepcopy(st)
                 st.magmom = [None] # added on 24.06.2017
 
-                write_xyz(st, file_name = st.name+'_used_for_scaling')
+                write_xyz(st, file_name = st.name+'_used_for_scaling',path = '.'.join([it_new,id_s[1]])) #AB_HERE
                 # print(scale_region)
                 # sys.exit()
                 if scale_region is None:
                     scale_region = (-4,4)
 
                 printlog('Scale_region is', scale_region, imp = 'y')
                 
                 # printlog('Calc_method', calc_method, 'uniform_scale' in calc_method, imp = 'y')
 
                 if 'uniform_scale' in calc_method:
 
                     sts = scale_cell_uniformly(st, scale_region = scale_region, n_scale_images = n_scale_images, parent_calc_name = pname)
+                    
                 elif 'c_scale' in calc_method:
                     #print('scale_start')
                     #sys.exit()
                     sts = scale_cell_by_matrix(st, scale_region = scale_region, n_scale_images = n_scale_images, parent_calc_name = pname, mul_matrix = [[1,0,0],[0,1,0],[0,0,1.01]])
                 else:
                     sts = scale_cell_by_matrix(st, scale_region = scale_region, n_scale_images = n_scale_images, parent_calc_name = pname, mul_matrix = mul_matrix)
 
@@ -1169,27 +1170,28 @@
                     cl_temp = CalculationVasp(varset[inputset], id_s)
 
                 for i, s in enumerate(sts):
                     ver_new = i+ 1 # start from 1; before it was v+i
                     s.name = it_new+'.'+s.name
                     cl_temp.init = s
                     cl_temp.version = ver_new
+                    # cl_temp.path["input_geo"] = header.geo_folder + struct_des[it_new].sfolder + '/' + \
+                                                # it_new+"/"+it_new+'.auto_created_scaled_image'+'.'+str(ver_new)+'.'+'geo'
                     cl_temp.path["input_geo"] = header.geo_folder + struct_des[it_new].sfolder + '/' + \
-                                                it_new+"/"+it_new+'.auto_created_scaled_image'+'.'+str(ver_new)+'.'+'geo'
-
+                                                it_new+'.'+id_s[1]+"/"+it_new+'.auto_created_scaled_image'+'.'+str(ver_new)+'.'+'geo'  #AB_here
                     cl_temp.write_siman_geo(geotype = "init", 
                         description = s.des, override = True)
-                    write_xyz(s)
+                    write_xyz(s, path = '.'.join([it_new,id_s[1]]))   #AB_here
                     verlist_new.append(ver_new)
+                    # sys.exit()
 
 
 
                 if 'uniform_scale' in calc_method or 'c_scale' in calc_method:
                     #print('Create 100')
-                    #sys.exit()
                     #make version 100
                     cl_temp.version = 100
                     cl_temp.des = 'fitted with fit_tool.py on cluster, init is incorrect'
                     cl_temp.id = (it_new, inputset, 100)
                     cl_temp.state = '2. separately prepared'
                     blockdir = struct_des[it_new].sfolder+"/"+varset[inputset].blockfolder #calculation folder
                     # iid = cl_temp.id          
@@ -1513,26 +1515,25 @@
     add_loop_modify()
 
     add_loop_prepare2()
 
     """Main Loop by setlist and verlist"""
     output_files_names = []
     input_folder = add_loop_choose_input_folder()
-
-
     for inputset in setlist:
 
         prevcalcver = None # version of previous calculation in verlist
 
         for v in verlist:
             id = (it,inputset,v)
 
             
            
             blockdir = header.struct_des[it].sfolder+"/"+varset[inputset].blockfolder #calculation folder
+            
 
 
             add_calculation(it,inputset,v, verlist[0], verlist[-1], 
                 input_folder, blockdir, calc, varset, up, 
                 inherit_option, prevcalcver, coord, savefile, input_geo_format, input_geo_file, 
                 input_kpoints=input_kpoints, 
                 calc_method = calc_method, 
@@ -1734,15 +1735,14 @@
     if 'show' not in params:
         params['show'] = ''
 
     if 'update_set_dic' not in params:
         params['update_set_dic'] = {}
 
 
-
     if id in calc: 
         cl = calc[id]
         status = "exist"
         printlog('add_calculation():',str(calc[id].name), " has been already created and has state: ", str(calc[id].state),)# imp = 'y')
 
         # print(cl.state)
 
@@ -1839,17 +1839,21 @@
 
 
         cl.calc_method = calc_method
 
         # print(input_st)
         if input_st:
             if not isinstance(input_st, Molecule) and not isinstance(input_st, Structure):
+
                 printlog('Error! input_st should be of type Structure() or Molecule')
             cl.init  = input_st
         else:
+            print(cl.path, cl.dir,input_geo_file)
+            input_folder =  cl.dir
+            # sys.exit()
             cl.init = smart_structure_read(curver = cl.id[2], calcul = cl, input_folder = input_folder, 
                 input_geo_format = input_geo_format, input_geo_file = input_geo_file)
 
 
 
         setseq = [cl.set]                                                                                                    
         if hasattr(cl.set, 'set_sequence') and cl.set.set_sequence:
@@ -1925,16 +1929,19 @@
 
             calc_geofile_path = os.path.join(cl.dir, os.path.basename(cl.path["input_geo"]) )
             
             # sys.exit()
             if cl.path["input_geo"] != calc_geofile_path: # copy initial geo file and other files to calc folder
 
                 makedir(calc_geofile_path)
+                try:  #AB_here
+                    shutil.copyfile(cl.path["input_geo"] , calc_geofile_path)
+                except shutil.SameFileError:
+                    ''
 
-                shutil.copyfile(cl.path["input_geo"] , calc_geofile_path)
 
                 #copy OCCMATRIX file as well             
                 dir_1 = os.path.dirname(cl.path["input_geo"] )
                 dir_2 = cl.dir
                 # sys.exit()
 
         if 'occmatrix' in params or ('OCCEXT' in cl.set.vasp_params and cl.set.vasp_params['OCCEXT'] == 1): #copy occfile
@@ -2627,15 +2634,15 @@
 
     if isinstance(st, Structure):
         new.write_geometry('init', des, override = override)
         printlog('Write_geometry using VASP object, please make more general', imp = 'n')
     if geo_folder:
         st.write_xyz(filename=geo_folder + '/' + it_new+"/"+it_new+'.inherit.'+inherit_type+'.'+str(ver_new))
     else:
-        st.write_xyz()
+        st.write_xyz()#path=path) AB_here
 
     # sys.exit()
 
 
 
     return
```

### Comparing `siman-1.3.3/siman/calcul.py` & `siman-1.3.4/siman/calcul.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/calculators/aims.py` & `siman-1.3.4/siman/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/calculators/gaussian.py` & `siman-1.3.4/siman/calculators/gaussian.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/calculators/qe.py` & `siman-1.3.4/siman/calculators/qe.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/calculators/vasp.py` & `siman-1.3.4/siman/calculators/vasp.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/calculators/vasp_old.py` & `siman-1.3.4/siman/calculators/vasp_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/chg/chg_func.py` & `siman-1.3.4/siman/chg/chg_func.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/chg/vasputil_chgarith_module.py` & `siman-1.3.4/siman/chg/vasputil_chgarith_module.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/classes.py` & `siman-1.3.4/siman/classes.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/core/calculation.py` & `siman-1.3.4/siman/core/calculation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/core/calculation_old.py` & `siman-1.3.4/siman/core/calculation_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/core/cluster_batch_script.py` & `siman-1.3.4/siman/core/cluster_batch_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/core/cluster_run_script.py` & `siman-1.3.4/siman/core/cluster_run_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/core/molecule.py` & `siman-1.3.4/siman/core/molecule.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/core/structure.py` & `siman-1.3.4/siman/core/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,29 +383,35 @@
     def get_symmetry_positions(self, *args, **kwargs):
         #just another name
         from siman.geo import determine_symmetry_positions
 
         return determine_symmetry_positions(self, *args, **kwargs)
 
 
-    def get_maglist(self):
+    def get_maglist(self, zels = None):
         """
         return bool list of which  elements are magnetic (here all transition metals are searched!)
         and dictionary with numbers in lists for each transition metal
         
+        INPUT:
+            - zels (list) - list of elements z, which should be returned in addition to transition elements
+
+
         RETURN:
             ifmaglist (list of bool) - magnetic or not
             mag_numbers (dict of int) - for each element using z, their numbers
         """
 
+        if not zels:
+            zels = []
         ifmaglist = []
         zlist = self.get_elements_z()
         mag_numbers = {}
         for i, z in enumerate(zlist): #
-            if z in header.TRANSITION_ELEMENTS:
+            if z in header.TRANSITION_ELEMENTS + zels:
                 if z not in mag_numbers:
                     mag_numbers[z] = []
                 ifmaglist.append(True)
                 mag_numbers[z].append(i)
             else:
                 ifmaglist.append(False)
         ifmaglist = np.array(ifmaglist)
@@ -451,15 +457,15 @@
         return groups_size, groups_nums
 
 
     def get_mag_tran(self, to_ox = None, silent = 0):
         #show formatted mag moments of transition metals 
         #to_ox - convert to oxidation state, substract from to_ox
         # if to_ox is negative, then m-to_ox
-        l, mag_numbers = self.get_maglist()
+        l, mag_numbers = self.get_maglist([8])
 
         keys = list(mag_numbers.keys())#[0]
         print('The following TM are found:', keys)
 
         mag = list(np.array(self.magmom)[l])
         magnetic = None
         magnetic_all = []
```

### Comparing `siman-1.3.3/siman/database.py` & `siman-1.3.4/siman/database.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/default_project_conf.py` & `siman-1.3.4/siman/default_project_conf.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/dev_functions.py` & `siman-1.3.4/siman/dev_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/dos_functions.py` & `siman-1.3.4/siman/dos_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/fit_hex.py` & `siman-1.3.4/siman/fit_hex.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/functions.py` & `siman-1.3.4/siman/functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/geo.py` & `siman-1.3.4/siman/geo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/header.py` & `siman-1.3.4/siman/header.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 history = []
 
 #Defaults to some project_conf values
 PBS_PROCS = False # if true than #PBS -l procs="+str(number_cores) is used
 WALLTIME_LIMIT = False # now only for PBS if True 72 hours limit is used
 CIF2CELL = False
-
+SIMAN_WEB = False
 
 # warnings = 'neyY'
 warnings = 'yY' # level of warnings to show: n - all, e - normal, y - important, Y - very important
 
 #Global constants, can be overriden in project_conf.py and simanrc.py
 FROM_ONE = None # atom numbering convention; allows to override the default behaviour of functions where atomic numbers are provided as arguments
 PATH2ARCHIVE_LOCAL  = None
@@ -85,21 +85,21 @@
     # if 'n' in war
     print(simanrc, 'was read')
     sys.path.insert(0, os.path.dirname(simanrc))
     from simanrc import *
 
 #3. Read project specific
 if os.path.exists('./project_conf.py'):
-    print('Reading ./project_conf.py')
+    print('Reading project_conf.py from', os.getcwd())
 
     from project_conf import *
     siman_run = True
     log = open('log','a')
 else:
-    # print('Some module is used separately; default_project_conf.py is used')
+    print('Some module is used separately; default_project_conf.py is used')
     if mpl and not os.path.exists(simanrc):
         mpl.use('agg') #switch matplotlib on or off; for running script using ssh
     siman_run = False
     history.append('separate run')
```

### Comparing `siman-1.3.3/siman/impurity.py` & `siman-1.3.4/siman/impurity.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/inout.py` & `siman-1.3.4/siman/inout.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #Copyright Aksyonov D.A
 from __future__ import division, unicode_literals, absolute_import 
-import os, io, re, math, sys
+import os, io, re, math, sys, glob
 from csv import reader
 
 
 import numpy  as np
 try:
     import pandas as pd 
 except:
@@ -13,23 +13,22 @@
 try:
     from tabulate import tabulate 
 except:
     print('inout.py: Cant import tabulate')
 
 
 
-from siman import header
+# from siman import header
 from siman.header import printlog, runBash, plt
 from siman.functions import element_name_inv, unique_elements, smoother
 from siman.small_functions import makedir, is_list_like, list2string, red_prec
 from siman.small_classes import empty_struct
 from siman.geo import local_surrounding, replic
 
 
-
 def determine_file_format(input_geo_file):
 
     supported_file_formats = {'abinit':'.geo',   'vasp':'POSCAR',   'cif':'.cif', 'xyz':'.xyz'} #format name:format specifier
 
     if ('POSCAR' in input_geo_file or 'CONTCAR' in input_geo_file) and not '.geo' in input_geo_file:
         input_geo_format = 'vasp'
     elif '.vasp' in input_geo_file:
@@ -48,14 +47,188 @@
         printlog("Attention! File format of",input_geo_file ,"is unknown, should be from ", supported_file_formats, 'skipping')
         input_geo_format = None
     return input_geo_format
 
 
 
 
+
+def get_file_by_version(geofilelist, version):
+
+    """
+    Find file with needed version from filelist according to certain rules
+    """
+    curv = None
+    
+    matched_files = []
+    # print(geofilelist)
+
+    for input_geofile in geofilelist: 
+        
+        input_geofile = os.path.normpath(input_geofile)
+
+
+        input_geo_format = determine_file_format(input_geofile)
+        # sys.exit()
+
+        printlog('For file', input_geofile, input_geo_format, ' format was detected', imp = 'n')
+
+        if input_geo_format in ['abinit',]: #version determined from token 
+            # curv = int( runBash("grep version "+str(input_geofile) ).split()[1] )
+            
+            with open(input_geofile, 'r') as f:
+                for line in f:
+                    if 'version' in line:
+                        curv = int(line.split()[1])
+
+
+        elif input_geo_format == 'vasp': #from filename
+            if '-' in input_geofile:
+                # print('create calculation for structure',input_geofile)
+                curv = int(input_geofile.split('-')[-1] ) #!Applied only for phonopy POSCAR-n naming convention
+                # print('create calculation for structure with version',curv)
+            # try: 
+            #     curv = int(input_geofile.split('-')[-1] ) #!Applied only for phonopy POSCAR-n naming convention
+            # except:
+            #     printlog('Error! Could not determine version of poscar file')
+
+        elif input_geo_format == 'cif': #from filename
+            printlog('I found cif file ', input_geofile)
+            try:
+                curv = int(os.path.basename(input_geofile).split('.')[0] )
+            except:
+                curv = None
+                printlog('Failed to determine version, skipping')
+        else:
+            curv = None
+
+        if curv == version:
+            # print('curv = ',curv,' version = ',version)
+            printlog('match', curv, version)
+            matched_files.append(input_geofile)
+
+    if len(matched_files) > 1:
+        printlog('get_file_by_version(): Error! Several files have same versions:', matched_files)
+    elif len(matched_files) == 0:
+        input_geofile = None
+    else:
+        input_geofile = matched_files[0]
+
+
+    return input_geofile
+
+
+
+
+
+def smart_structure_read(filename = None, curver = 1, calcul = None, input_folder = None, input_geo_format = None, input_geo_file = None, ):
+    """
+    Wrapper for reading geometry files (use new reader read_structure() from siman.inout )
+    calcul (Calculation()) - object to which the path and version read
+
+    curver (int) - version of file to be read
+    input_geo_file or filename (str) - explicitly provided input file, has higher priority
+    input_folder (str)   - folder with several input files, the names doesnot matter only versions
+    input_geo_format (str) - explicitly provided format of input file 
+
+
+
+    returns Structure()
+    """
+
+    search_templates =       {'abinit':'*.geo*', 'vasp':'*POSCAR*', 'vasp-phonopy': 'POSCAR*', 'cif':'*.cif'}
+
+    if filename:
+        input_geo_file = filename
+
+    if input_geo_file:
+
+        printlog("You provided the following geo file explicitly ", input_geo_file, 
+            '; Version of file does not matter, I use *curver*=',curver, 'as a new version' )
+        
+    elif input_folder:
+
+        printlog("I am searching for geofiles in folder "+input_folder+"\n" )
+
+        if input_geo_format: 
+            geofilelist = glob.glob(input_folder+'/'+search_templates[input_geo_format]) #Find input_geofile of specific format
+        else:
+            geofilelist = glob.glob(input_folder+'/*') 
+
+        geofilelist = [file for file in geofilelist if os.path.basename(file)[0] != '.'   ]  #skip hidden files
+
+        printlog('List of files:', geofilelist)
+
+        input_geo_file = get_file_by_version(geofilelist, curver)
+        # sys.exit()
+
+        printlog('The result of getting by version', input_geo_file)
+
+        if input_geo_file:
+            printlog('File ', input_geo_file, 'was found')
+        else:
+            printlog('Error! No input file with version ', curver, 'was found in', input_folder)
+    
+    else:
+        printlog('Neither *input_geo_file* nor *input_folder* were provided')
+
+
+    input_geo_format = determine_file_format(input_geo_file)
+    printlog(input_geo_format,' format is detected')
+
+    from siman.calculators.vasp import CalculationVasp
+    if calcul:
+        cl = calcul
+    else:
+        cl = CalculationVasp()
+
+
+    if input_geo_format   == 'abinit':
+        cl.read_geometry(input_geo_file)
+
+    
+    elif input_geo_format == 'vasp':
+        cl.read_poscar(input_geo_file, version = curver)
+
+
+    elif input_geo_format == 'cif':
+        
+        cif2poscar(input_geo_file, input_geo_file.replace('.cif', '.POSCAR'))
+        input_geo_file = input_geo_file.replace('.cif', '.POSCAR')
+        cl.read_poscar(input_geo_file)
+
+    elif input_geo_format == 'xyz':
+        #version = 1
+        st = cl.init
+        st = read_xyz(st, input_geo_file)
+        cl.init = st
+        cl.path["input_geo"] = input_geo_file
+        cl.version = 1
+
+    else:
+        print_and_log("Error! smart_structure_read(): File format", input_geo_format, "is unknown")
+
+
+    if cl.path["input_geo"] == None: 
+        printlog("Error! Input file was not properly read for some reason")
+    
+
+    return cl.init
+
+
+
+
+
+
+
+
+
+
+
+
 def read_csv(filename, delimiter =','):
     with open(filename, 'r') as read_obj:
         # pass the file object to reader() to get the reader object
         csv_reader = reader(read_obj, delimiter = delimiter)
         # Pass reader object to list() to get a list of lists
         list_of_rows = list(csv_reader)
         # print(list_of_rows)
@@ -502,14 +675,15 @@
 
         
         # f.write('write image 2800 2800 png "'+pngfile+'"')
         f.write('write image 1800 1800 png "'+pngfile+'"')
     
     # print(header.PATH2JMOL)
     # sys.exit()
+    from siman import header
     printlog( runBash(header.PATH2JMOL+' -ions '+scriptfile) )
     # print runBash('convert '+pngfile+' -shave 0x5% -trim '+pngfile) #cut by 5% from up and down (shave) and that trim left background
     printlog( pngfile )
     printlog( runBash('convert '+pngfile+' -trim '+pngfile)  ) # trim background
     printlog('png file by Jmol',pngfile, 'was written', imp = 'y' )
     # print(header.PATH2JMOL)
     return pngfile
@@ -2182,14 +2356,15 @@
 
     # sys.exit()
 
 
     printlog("Reading of results completed\n\n", imp = 'n')
     self.end.outfile = path_to_outcar
     
+    from siman import header
 
     if header.pymatgen_flag:
         ''
         # self.end.write_cif(os.path.join(self.dir,self.name))
     
 
     # print(out_type)
```

### Comparing `siman-1.3.3/siman/kpoints_functions.py` & `siman-1.3.4/siman/kpoints_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/mat_prop/mat_prop.py` & `siman-1.3.4/siman/mat_prop/mat_prop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/matproj_functions.py` & `siman-1.3.4/siman/matproj_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/monte.py` & `siman-1.3.4/siman/monte.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/monte_functions.py` & `siman-1.3.4/siman/monte_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/neb.py` & `siman-1.3.4/siman/neb.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/pairs.py` & `siman-1.3.4/siman/pairs.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/picture_functions.py` & `siman-1.3.4/siman/picture_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/plot_functions.py` & `siman-1.3.4/siman/plot_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/polaron.py` & `siman-1.3.4/siman/polaron.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/polaron_hop.py` & `siman-1.3.4/siman/polaron_hop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/polaron_mod.py` & `siman-1.3.4/siman/polaron_mod.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/project_funcs.py` & `siman-1.3.4/siman/project_funcs.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/properties_2d.py` & `siman-1.3.4/siman/properties_2d.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/properties_energy.py` & `siman-1.3.4/siman/properties_energy.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/properties_lattice.py` & `siman-1.3.4/siman/properties_lattice.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/set_functions.py` & `siman-1.3.4/siman/set_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/simanrc.py` & `siman-1.3.4/siman/simanrc.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/small_functions.py` & `siman-1.3.4/siman/small_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/structure_functions.py` & `siman-1.3.4/siman/structure_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/table_functions.py` & `siman-1.3.4/siman/table_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/thermo.py` & `siman-1.3.4/siman/thermo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman/workflow_utilities.py` & `siman-1.3.4/siman/workflow_utilities.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.3/siman.egg-info/PKG-INFO` & `siman-1.3.4/siman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.3
+Version: 1.3.4
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.3/siman.egg-info/SOURCES.txt` & `siman-1.3.4/siman.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 siman/SSHTools.py
 siman/__init__.py
 siman/analysis.py
 siman/analysis_functions.py
 siman/approximation.py
 siman/bands.py
 siman/calc_manage.py
+siman/calc_manage_AB.py
 siman/calcul.py
 siman/classes.py
 siman/database.py
 siman/default_project_conf.py
 siman/dev_functions.py
 siman/dos_functions.py
 siman/fit_hex.py
```


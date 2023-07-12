# Comparing `tmp/PDielec-7.2.1.tar.gz` & `tmp/PDielec-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDielec-7.2.1.tar", last modified: Tue Jul  4 12:53:23 2023, max compression
+gzip compressed data, was "PDielec-7.2.2.tar", last modified: Wed Jul 12 08:19:36 2023, max compression
```

## Comparing `PDielec-7.2.1.tar` & `PDielec-7.2.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-07-04 12:53:23.896868 PDielec-7.2.1/
--rw-rw-r--   0 john      (1000) john      (1000)     1080 2015-11-17 09:07:58.000000 PDielec-7.2.1/LICENSE.md
--rw-r--r--   0 john      (1000) john      (1000)     1080 2018-03-01 08:29:24.000000 PDielec-7.2.1/LICENSE.txt
--rw-r--r--   0 john      (1000) john      (1000)       17 2021-12-04 13:46:41.000000 PDielec-7.2.1/MANIFEST.in
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-07-04 12:53:23.894868 PDielec-7.2.1/PDielec/
--rw-r--r--   0 john      (1000) john      (1000)    10508 2021-11-18 17:01:07.000000 PDielec-7.2.1/PDielec/AbinitOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)    71022 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/Calculator.py
--rw-r--r--   0 john      (1000) john      (1000)    15442 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/CastepOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)    23360 2021-11-18 17:01:23.000000 PDielec-7.2.1/PDielec/Constants.py
--rw-r--r--   0 john      (1000) john      (1000)    14706 2022-03-25 15:49:33.000000 PDielec-7.2.1/PDielec/CrystalOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)    14648 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/DielectricFunction.py
--rw-r--r--   0 john      (1000) john      (1000)    17991 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/ExperimentOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)    44231 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/GTMcore.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-07-04 12:53:23.896868 PDielec-7.2.1/PDielec/GUI/
--rw-r--r--   0 john      (1000) john      (1000)    23910 2022-03-24 15:19:32.000000 PDielec-7.2.1/PDielec/GUI/AnalysisTab.py
--rw-r--r--   0 john      (1000) john      (1000)     9875 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/GUI/App.py
--rw-r--r--   0 john      (1000) john      (1000)    38940 2021-12-28 18:32:44.000000 PDielec-7.2.1/PDielec/GUI/FitterTab.py
--rw-r--r--   0 john      (1000) john      (1000)    27046 2022-03-24 14:59:26.000000 PDielec-7.2.1/PDielec/GUI/MainTab.py
--rw-r--r--   0 john      (1000) john      (1000)    21764 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/GUI/NoteBook.py
--rw-r--r--   0 john      (1000) john      (1000)    20745 2023-07-03 18:31:52.000000 PDielec-7.2.1/PDielec/GUI/OpenGLWidget.py
--rw-r--r--   0 john      (1000) john      (1000)    32111 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/GUI/PlottingTab.py
--rw-r--r--   0 john      (1000) john      (1000)    39204 2022-02-02 17:58:16.000000 PDielec-7.2.1/PDielec/GUI/PowderScenarioTab.py
--rw-r--r--   0 john      (1000) john      (1000)     4331 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/GUI/ScenarioTab.py
--rw-r--r--   0 john      (1000) john      (1000)    34276 2022-03-26 09:51:30.000000 PDielec-7.2.1/PDielec/GUI/SettingsTab.py
--rw-r--r--   0 john      (1000) john      (1000)    25673 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/GUI/SingleCrystalScenarioTab.py
--rw-r--r--   0 john      (1000) john      (1000)     2814 2023-07-04 08:24:54.000000 PDielec-7.2.1/PDielec/GUI/SpreadSheetManager.py
--rw-r--r--   0 john      (1000) john      (1000)    33329 2022-03-24 15:43:39.000000 PDielec-7.2.1/PDielec/GUI/ViewerTab.py
--rw-r--r--   0 john      (1000) john      (1000)       80 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec/GUI/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)    31376 2020-05-05 17:36:05.000000 PDielec-7.2.1/PDielec/GUI/splash.png
--rw-r--r--   0 john      (1000) john      (1000)    23965 2022-02-02 14:29:45.000000 PDielec-7.2.1/PDielec/GenericOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)    15555 2021-11-18 17:01:42.000000 PDielec-7.2.1/PDielec/GulpOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)     1078 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/IO.py
--rw-r--r--   0 john      (1000) john      (1000)    20827 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/Mie.py
--rw-r--r--   0 john      (1000) john      (1000)     5676 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/PhonopyOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)     2395 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/Plotter.py
--rw-r--r--   0 john      (1000) john      (1000)    14124 2021-11-18 17:02:14.000000 PDielec-7.2.1/PDielec/QEOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)     7854 2022-03-23 14:21:38.000000 PDielec-7.2.1/PDielec/SuperCell.py
--rw-r--r--   0 john      (1000) john      (1000)    23459 2022-03-23 14:21:43.000000 PDielec-7.2.1/PDielec/UnitCell.py
--rw-r--r--   0 john      (1000) john      (1000)     9784 2022-03-24 15:05:17.000000 PDielec-7.2.1/PDielec/Utilities.py
--rw-r--r--   0 john      (1000) john      (1000)    15876 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/VaspOutputReader.py
--rw-r--r--   0 john      (1000) john      (1000)       80 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec/__init__.py
--rwxr-xr-x   0 john      (1000) john      (1000)     7283 2022-01-21 11:41:10.000000 PDielec-7.2.1/PDielec/checkcsv.py
--rwxr-xr-x   0 john      (1000) john      (1000)     5880 2022-01-21 11:41:10.000000 PDielec-7.2.1/PDielec/checkexcel.py
--rwxr-xr-x   0 john      (1000) john      (1000)     5188 2021-11-18 17:01:37.000000 PDielec-7.2.1/PDielec/graphdatagenerator.py
--rwxr-xr-x   0 john      (1000) john      (1000)     3741 2021-12-04 12:53:52.000000 PDielec-7.2.1/PDielec/p1reader.py
--rwxr-xr-x   0 john      (1000) john      (1000)     4422 2022-01-21 11:41:10.000000 PDielec-7.2.1/PDielec/p2cif.py
--rwxr-xr-x   0 john      (1000) john      (1000)     6768 2021-11-18 17:01:58.000000 PDielec-7.2.1/PDielec/pdcompare.py
--rwxr-xr-x   0 john      (1000) john      (1000)     2711 2022-02-03 11:08:20.000000 PDielec-7.2.1/PDielec/pdgui.py
--rwxr-xr-x   0 john      (1000) john      (1000)    27840 2023-07-04 12:51:45.000000 PDielec-7.2.1/PDielec/pdmake.py
--rwxr-xr-x   0 john      (1000) john      (1000)     1689 2021-11-18 17:02:06.000000 PDielec-7.2.1/PDielec/pickled_reader.py
--rwxr-xr-x   0 john      (1000) john      (1000)    21219 2022-01-21 11:41:10.000000 PDielec-7.2.1/PDielec/preader.py
--rw-r--r--   0 john      (1000) john      (1000)     3751 2021-12-04 12:53:53.000000 PDielec-7.2.1/PDielec/test_gtm.py
--rw-r--r--   0 john      (1000) john      (1000)    12091 2021-12-04 12:53:53.000000 PDielec-7.2.1/PDielec/test_ttm.py
--rwxr-xr-x   0 john      (1000) john      (1000)    70967 2022-01-21 11:41:10.000000 PDielec-7.2.1/PDielec/vibanalysis.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-07-04 12:53:23.895868 PDielec-7.2.1/PDielec.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     4000 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     1421 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)      266 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec.egg-info/entry_points.txt
--rw-r--r--   0 john      (1000) john      (1000)      167 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)       20 2023-07-04 12:53:23.000000 PDielec-7.2.1/PDielec.egg-info/top_level.txt
--rw-r--r--   0 john      (1000) john      (1000)     4000 2023-07-04 12:53:23.896868 PDielec-7.2.1/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     2994 2020-05-05 17:36:05.000000 PDielec-7.2.1/README.md
--rw-r--r--   0 john      (1000) john      (1000)       79 2023-07-04 12:53:23.896868 PDielec-7.2.1/setup.cfg
--rw-r--r--   0 john      (1000) john      (1000)     2681 2023-07-04 08:30:08.000000 PDielec-7.2.1/setup.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-07-12 08:19:36.683596 PDielec-7.2.2/
+-rw-r--r--   0 john      (1000) john      (1000)     1080 2023-07-11 19:53:08.000000 PDielec-7.2.2/LICENSE.md
+-rw-r--r--   0 john      (1000) john      (1000)     1080 2023-07-11 19:53:08.000000 PDielec-7.2.2/LICENSE.txt
+-rw-r--r--   0 john      (1000) john      (1000)       17 2023-07-11 19:53:08.000000 PDielec-7.2.2/MANIFEST.in
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-07-12 08:19:36.680263 PDielec-7.2.2/PDielec/
+-rw-r--r--   0 john      (1000) john      (1000)    10508 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/AbinitOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)    71022 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/Calculator.py
+-rw-r--r--   0 john      (1000) john      (1000)    15442 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/CastepOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)    23360 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/Constants.py
+-rw-r--r--   0 john      (1000) john      (1000)    14706 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/CrystalOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)    14648 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/DielectricFunction.py
+-rw-r--r--   0 john      (1000) john      (1000)    17991 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/ExperimentOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)    44225 2023-07-11 19:53:40.000000 PDielec-7.2.2/PDielec/GTMcore.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-07-12 08:19:36.683596 PDielec-7.2.2/PDielec/GUI/
+-rw-r--r--   0 john      (1000) john      (1000)    23910 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/AnalysisTab.py
+-rw-r--r--   0 john      (1000) john      (1000)     9875 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/App.py
+-rw-r--r--   0 john      (1000) john      (1000)    38940 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/FitterTab.py
+-rw-r--r--   0 john      (1000) john      (1000)    27046 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/MainTab.py
+-rw-r--r--   0 john      (1000) john      (1000)    21764 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/NoteBook.py
+-rw-r--r--   0 john      (1000) john      (1000)    20745 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/OpenGLWidget.py
+-rw-r--r--   0 john      (1000) john      (1000)    32111 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/PlottingTab.py
+-rw-r--r--   0 john      (1000) john      (1000)    39204 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/PowderScenarioTab.py
+-rw-r--r--   0 john      (1000) john      (1000)     4331 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/ScenarioTab.py
+-rw-r--r--   0 john      (1000) john      (1000)    34276 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/SettingsTab.py
+-rw-r--r--   0 john      (1000) john      (1000)    25673 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/SingleCrystalScenarioTab.py
+-rw-r--r--   0 john      (1000) john      (1000)     2814 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/SpreadSheetManager.py
+-rw-r--r--   0 john      (1000) john      (1000)    33329 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/ViewerTab.py
+-rw-r--r--   0 john      (1000) john      (1000)       80 2023-07-12 08:19:36.000000 PDielec-7.2.2/PDielec/GUI/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)    31376 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GUI/splash.png
+-rw-r--r--   0 john      (1000) john      (1000)    23965 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GenericOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)    15555 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/GulpOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)     1078 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/IO.py
+-rw-r--r--   0 john      (1000) john      (1000)    20827 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/Mie.py
+-rw-r--r--   0 john      (1000) john      (1000)     5676 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/PhonopyOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)     2395 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/Plotter.py
+-rw-r--r--   0 john      (1000) john      (1000)    14124 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/QEOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)     7854 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/SuperCell.py
+-rw-r--r--   0 john      (1000) john      (1000)    23459 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/UnitCell.py
+-rw-r--r--   0 john      (1000) john      (1000)     9784 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/Utilities.py
+-rw-r--r--   0 john      (1000) john      (1000)    15876 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/VaspOutputReader.py
+-rw-r--r--   0 john      (1000) john      (1000)       80 2023-07-12 08:19:36.000000 PDielec-7.2.2/PDielec/__init__.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     7283 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/checkcsv.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     5880 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/checkexcel.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     5188 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/graphdatagenerator.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     3741 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/p1reader.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     4422 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/p2cif.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     6768 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/pdcompare.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     2711 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/pdgui.py
+-rwxr-xr-x   0 john      (1000) john      (1000)    27840 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/pdmake.py
+-rwxr-xr-x   0 john      (1000) john      (1000)     1689 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/pickled_reader.py
+-rwxr-xr-x   0 john      (1000) john      (1000)    21219 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/preader.py
+-rw-r--r--   0 john      (1000) john      (1000)     3751 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/test_gtm.py
+-rw-r--r--   0 john      (1000) john      (1000)    12091 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/test_ttm.py
+-rwxr-xr-x   0 john      (1000) john      (1000)    70967 2023-07-11 19:53:08.000000 PDielec-7.2.2/PDielec/vibanalysis.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-07-12 08:19:36.680263 PDielec-7.2.2/PDielec.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     4000 2023-07-12 08:19:36.000000 PDielec-7.2.2/PDielec.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     1421 2023-07-12 08:19:36.000000 PDielec-7.2.2/PDielec.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2023-07-12 08:19:36.000000 PDielec-7.2.2/PDielec.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)      266 2023-07-12 08:19:36.000000 PDielec-7.2.2/PDielec.egg-info/entry_points.txt
+-rw-r--r--   0 john      (1000) john      (1000)      167 2023-07-12 08:19:36.000000 PDielec-7.2.2/PDielec.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)       20 2023-07-12 08:19:36.000000 PDielec-7.2.2/PDielec.egg-info/top_level.txt
+-rw-r--r--   0 john      (1000) john      (1000)     4000 2023-07-12 08:19:36.683596 PDielec-7.2.2/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     2994 2023-07-11 19:53:08.000000 PDielec-7.2.2/README.md
+-rw-r--r--   0 john      (1000) john      (1000)       79 2023-07-12 08:19:36.683596 PDielec-7.2.2/setup.cfg
+-rw-r--r--   0 john      (1000) john      (1000)     2681 2023-07-12 08:14:33.000000 PDielec-7.2.2/setup.py
```

### Comparing `PDielec-7.2.1/LICENSE.md` & `PDielec-7.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/LICENSE.txt` & `PDielec-7.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/AbinitOutputReader.py` & `PDielec-7.2.2/PDielec/AbinitOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/Calculator.py` & `PDielec-7.2.2/PDielec/Calculator.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/CastepOutputReader.py` & `PDielec-7.2.2/PDielec/CastepOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/Constants.py` & `PDielec-7.2.2/PDielec/Constants.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/CrystalOutputReader.py` & `PDielec-7.2.2/PDielec/CrystalOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/DielectricFunction.py` & `PDielec-7.2.2/PDielec/DielectricFunction.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/ExperimentOutputReader.py` & `PDielec-7.2.2/PDielec/ExperimentOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GTMcore.py` & `PDielec-7.2.2/PDielec/GTMcore.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,16 +450,16 @@
         -----
         From this we also get the Poynting vectors.
         Wavevectors are sorted according to (trans-p, trans-s, refl-p, refl-s)
         Birefringence is determined according to a threshold value `qsd_thr`
         set at the beginning of the script.
         """
         Delta_loc = np.zeros((4,4), dtype=np.complex128)
-        transmode = np.zeros((2), dtype=np.int)
-        reflmode = np.zeros((2), dtype=np.int)
+        transmode = np.zeros((2), dtype=int)
+        reflmode = np.zeros((2), dtype=int)
 
         Delta_loc = self.Delta.copy()
         ## eigenvals // eigenvects as of eqn (11)
         qsunsorted, psiunsorted = lag.eig(Delta_loc)
 
         kt = 0
         kr = 0;
```

### Comparing `PDielec-7.2.1/PDielec/GUI/AnalysisTab.py` & `PDielec-7.2.2/PDielec/GUI/AnalysisTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GUI/App.py` & `PDielec-7.2.2/PDielec/GUI/App.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GUI/FitterTab.py` & `PDielec-7.2.2/PDielec/GUI/FitterTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GUI/MainTab.py` & `PDielec-7.2.2/PDielec/GUI/MainTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GUI/NoteBook.py` & `PDielec-7.2.2/PDielec/GUI/NoteBook.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GUI/OpenGLWidget.py` & `PDielec-7.2.2/PDielec/GUI/OpenGLWidget.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GUI/PlottingTab.py` & `PDielec-7.2.2/PDielec/GUI/PlottingTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GUI/PowderScenarioTab.py` & `PDielec-7.2.2/PDielec/GUI/PowderScenarioTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GUI/ScenarioTab.py` & `PDielec-7.2.2/PDielec/GUI/ScenarioTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GUI/SettingsTab.py` & `PDielec-7.2.2/PDielec/GUI/SettingsTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GUI/SingleCrystalScenarioTab.py` & `PDielec-7.2.2/PDielec/GUI/SingleCrystalScenarioTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GUI/SpreadSheetManager.py` & `PDielec-7.2.2/PDielec/GUI/SpreadSheetManager.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GUI/ViewerTab.py` & `PDielec-7.2.2/PDielec/GUI/ViewerTab.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GUI/splash.png` & `PDielec-7.2.2/PDielec/GUI/splash.png`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GenericOutputReader.py` & `PDielec-7.2.2/PDielec/GenericOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/GulpOutputReader.py` & `PDielec-7.2.2/PDielec/GulpOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/IO.py` & `PDielec-7.2.2/PDielec/IO.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/Mie.py` & `PDielec-7.2.2/PDielec/Mie.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/PhonopyOutputReader.py` & `PDielec-7.2.2/PDielec/PhonopyOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/Plotter.py` & `PDielec-7.2.2/PDielec/Plotter.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/QEOutputReader.py` & `PDielec-7.2.2/PDielec/QEOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/SuperCell.py` & `PDielec-7.2.2/PDielec/SuperCell.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/UnitCell.py` & `PDielec-7.2.2/PDielec/UnitCell.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/Utilities.py` & `PDielec-7.2.2/PDielec/Utilities.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/VaspOutputReader.py` & `PDielec-7.2.2/PDielec/VaspOutputReader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/checkcsv.py` & `PDielec-7.2.2/PDielec/checkcsv.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/checkexcel.py` & `PDielec-7.2.2/PDielec/checkexcel.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/graphdatagenerator.py` & `PDielec-7.2.2/PDielec/graphdatagenerator.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/p1reader.py` & `PDielec-7.2.2/PDielec/p1reader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/p2cif.py` & `PDielec-7.2.2/PDielec/p2cif.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/pdcompare.py` & `PDielec-7.2.2/PDielec/pdcompare.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/pdgui.py` & `PDielec-7.2.2/PDielec/pdgui.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/pdmake.py` & `PDielec-7.2.2/PDielec/pdmake.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/pickled_reader.py` & `PDielec-7.2.2/PDielec/pickled_reader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/preader.py` & `PDielec-7.2.2/PDielec/preader.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/test_gtm.py` & `PDielec-7.2.2/PDielec/test_gtm.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/test_ttm.py` & `PDielec-7.2.2/PDielec/test_ttm.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec/vibanalysis.py` & `PDielec-7.2.2/PDielec/vibanalysis.py`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PDielec.egg-info/PKG-INFO` & `PDielec-7.2.2/PDielec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDielec
-Version: 7.2.1
+Version: 7.2.2
 Summary: PDielec package for the calculation of THz and infrared spectra
 Home-page: https://github.com/JohnKendrick/PDielec
 Author: John Kendrick and Andrew Burnett
 Author-email: john@kendrick.co.uk
 License: MIT
 Keywords: Infrared, Infrared Spectroscopy,THz Spectroscopy,Terahertz Spectroscopy,Bruggeman,Maxwell-Garnett,Effective Medium
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PDielec-7.2.1/PDielec.egg-info/SOURCES.txt` & `PDielec-7.2.2/PDielec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/PKG-INFO` & `PDielec-7.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDielec
-Version: 7.2.1
+Version: 7.2.2
 Summary: PDielec package for the calculation of THz and infrared spectra
 Home-page: https://github.com/JohnKendrick/PDielec
 Author: John Kendrick and Andrew Burnett
 Author-email: john@kendrick.co.uk
 License: MIT
 Keywords: Infrared, Infrared Spectroscopy,THz Spectroscopy,Terahertz Spectroscopy,Bruggeman,Maxwell-Garnett,Effective Medium
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PDielec-7.2.1/README.md` & `PDielec-7.2.2/README.md`

 * *Files identical despite different names*

### Comparing `PDielec-7.2.1/setup.py` & `PDielec-7.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 # Update this for every PyPi release
-version = "7.2.1"
+version = "7.2.2"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 init_lines = ["# Created by setup.py, whilst creating a new PyPi release\n","__version__ = \"{}\"\n".format(version)]
 with open("PDielec/__init__.py", "w") as fh:
```


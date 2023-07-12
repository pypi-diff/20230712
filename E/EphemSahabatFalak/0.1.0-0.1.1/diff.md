# Comparing `tmp/EphemSahabatFalak-0.1.0.tar.gz` & `tmp/EphemSahabatFalak-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EphemSahabatFalak-0.1.0.tar", last modified: Sun Jun 25 03:32:11 2023, max compression
+gzip compressed data, was "EphemSahabatFalak-0.1.1.tar", last modified: Wed Jul 12 02:09:02 2023, max compression
```

## Comparing `EphemSahabatFalak-0.1.0.tar` & `EphemSahabatFalak-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-25 03:32:11.812730 EphemSahabatFalak-0.1.0/
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-25 03:32:11.811098 EphemSahabatFalak-0.1.0/EphemSahabatFalak/
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)   100342 2023-06-25 03:09:48.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak/KiraanWaktuSolat.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    49515 2023-06-24 23:21:37.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak/Takwim_Madinah_Awal_Bulan_Mabims2021.csv
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    49659 2023-06-23 14:51:37.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak/Tarikh_Hijri_Awal_Tahun_Pulau_Pinang.csv
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       53 2023-06-11 17:41:20.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak/__init__.py
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-25 03:32:11.812263 EphemSahabatFalak-0.1.0/EphemSahabatFalak.egg-info/
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1463 2023-06-25 03:32:11.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak.egg-info/PKG-INFO
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      420 2023-06-25 03:32:11.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak.egg-info/SOURCES.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        1 2023-06-25 03:32:11.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak.egg-info/dependency_links.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       78 2023-06-25 03:32:11.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak.egg-info/requires.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       18 2023-06-25 03:32:11.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak.egg-info/top_level.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      152 2023-06-25 03:25:43.000000 EphemSahabatFalak-0.1.0/MANIFEST.in
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1463 2023-06-25 03:32:11.812562 EphemSahabatFalak-0.1.0/PKG-INFO
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      876 2023-06-25 03:26:42.000000 EphemSahabatFalak-0.1.0/README.md
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       38 2023-06-25 03:32:11.812799 EphemSahabatFalak-0.1.0/setup.cfg
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1302 2023-06-25 03:27:48.000000 EphemSahabatFalak-0.1.0/setup.py
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-07-12 02:09:02.870256 EphemSahabatFalak-0.1.1/
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-07-12 02:09:02.866655 EphemSahabatFalak-0.1.1/EphemSahabatFalak/
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)   224320 2023-07-12 01:45:22.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak/KiraanWaktuSolat.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    49515 2023-06-24 23:21:37.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak/Takwim_Madinah_Awal_Bulan_Mabims2021.csv
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    49659 2023-06-23 14:51:37.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak/Tarikh_Hijri_Awal_Tahun_Pulau_Pinang.csv
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       82 2023-07-12 01:46:40.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak/__init__.py
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-07-12 02:09:02.869241 EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1463 2023-07-12 02:09:02.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/PKG-INFO
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      420 2023-07-12 02:09:02.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/SOURCES.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        1 2023-07-12 02:09:02.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/dependency_links.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       78 2023-07-12 02:09:02.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/requires.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       18 2023-07-12 02:09:02.000000 EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/top_level.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      152 2023-06-25 03:25:43.000000 EphemSahabatFalak-0.1.1/MANIFEST.in
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1463 2023-07-12 02:09:02.869926 EphemSahabatFalak-0.1.1/PKG-INFO
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      876 2023-06-25 03:26:42.000000 EphemSahabatFalak-0.1.1/README.md
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       38 2023-07-12 02:09:02.870396 EphemSahabatFalak-0.1.1/setup.cfg
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1302 2023-07-12 02:08:08.000000 EphemSahabatFalak-0.1.1/setup.py
```

### Comparing `EphemSahabatFalak-0.1.0/EphemSahabatFalak/Takwim_Madinah_Awal_Bulan_Mabims2021.csv` & `EphemSahabatFalak-0.1.1/EphemSahabatFalak/Takwim_Madinah_Awal_Bulan_Mabims2021.csv`

 * *Files identical despite different names*

### Comparing `EphemSahabatFalak-0.1.0/EphemSahabatFalak/Tarikh_Hijri_Awal_Tahun_Pulau_Pinang.csv` & `EphemSahabatFalak-0.1.1/EphemSahabatFalak/Tarikh_Hijri_Awal_Tahun_Pulau_Pinang.csv`

 * *Files identical despite different names*

### Comparing `EphemSahabatFalak-0.1.0/EphemSahabatFalak.egg-info/PKG-INFO` & `EphemSahabatFalak-0.1.1/EphemSahabatFalak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EphemSahabatFalak
-Version: 0.1.0
+Version: 0.1.1
 Summary: Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak
 Author: cartcosine (izzatzubir)
 Author-email: <cart.cosine.0x@icloud.com>
 Keywords: falak,solat,hilal,waktu,matahari,bulan,kiblat
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EphemSahabatFalak-0.1.0/PKG-INFO` & `EphemSahabatFalak-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EphemSahabatFalak
-Version: 0.1.0
+Version: 0.1.1
 Summary: Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak
 Author: cartcosine (izzatzubir)
 Author-email: <cart.cosine.0x@icloud.com>
 Keywords: falak,solat,hilal,waktu,matahari,bulan,kiblat
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `EphemSahabatFalak-0.1.0/README.md` & `EphemSahabatFalak-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `EphemSahabatFalak-0.1.0/setup.py` & `EphemSahabatFalak-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak'
 LONG_DESCRIPTION = 'Sebuah pakej python yang menggunakan ephemeris dari JPL Horizon bagi menghasilkan hitungan falak'
 
 # Setting up
 setup(
     name="EphemSahabatFalak",
     version=VERSION,
```


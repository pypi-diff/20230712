# Comparing `tmp/pybppibridge-0.4.7-py3-none-any.whl.zip` & `tmp/pybppibridge-0.4.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 50069 bytes, number of entries: 40
+Zip file size: 50076 bytes, number of entries: 40
 -rw-r--r--  2.0 unx     1730 b- defN 20-Feb-02 00:00 setup-old.py
--rw-r--r--  2.0 unx      391 b- defN 20-Feb-02 00:00 src/__init__.py
+-rw-r--r--  2.0 unx      391 b- defN 20-Feb-02 00:00 src/__init__.py.py
 -rw-r--r--  2.0 unx      145 b- defN 20-Feb-02 00:00 src/bppibridge.py
 -rw-r--r--  2.0 unx      401 b- defN 20-Feb-02 00:00 src/bppibridgesq.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 src/bppiapi/__init__.py
 -rw-r--r--  2.0 unx     9566 b- defN 20-Feb-02 00:00 src/bppiapi/bppiPipeline.py
 -rw-r--r--  2.0 unx     1188 b- defN 20-Feb-02 00:00 src/bppiapi/uploadConfig.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 src/bppiapi/project/__init__.py
 -rw-r--r--  2.0 unx      930 b- defN 20-Feb-02 00:00 src/bppiapi/project/bppiApiProjectWrapper.py
@@ -30,13 +30,13 @@
 -rw-r--r--  2.0 unx     1606 b- defN 20-Feb-02 00:00 src/pipelines/repository/bppiPLRExcelFile.py
 -rw-r--r--  2.0 unx     2437 b- defN 20-Feb-02 00:00 src/pipelines/repository/bppiPLRODBC.py
 -rw-r--r--  2.0 unx     5067 b- defN 20-Feb-02 00:00 src/pipelines/repository/bppiPLRSAPRfcTable.py
 -rw-r--r--  2.0 unx     1331 b- defN 20-Feb-02 00:00 src/pipelines/repository/bppiPLRXESFile.py
 -rw-r--r--  2.0 unx      537 b- defN 20-Feb-02 00:00 src/utils/__init__.py
 -rw-r--r--  2.0 unx     8851 b- defN 20-Feb-02 00:00 src/utils/constants.py
 -rw-r--r--  2.0 unx     2016 b- defN 20-Feb-02 00:00 src/utils/log.py
-?rw-r--r--  2.0 unx     3997 b- defN 20-Feb-02 00:00 pybppibridge-0.4.7.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pybppibridge-0.4.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx       47 b- defN 20-Feb-02 00:00 pybppibridge-0.4.7.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 pybppibridge-0.4.7.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     3527 b- defN 20-Feb-02 00:00 pybppibridge-0.4.7.dist-info/RECORD
-40 files, 139089 bytes uncompressed, 44343 bytes compressed:  68.1%
+?rw-r--r--  2.0 unx     3997 b- defN 20-Feb-02 00:00 pybppibridge-0.4.8.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pybppibridge-0.4.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx       36 b- defN 20-Feb-02 00:00 pybppibridge-0.4.8.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 pybppibridge-0.4.8.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     3530 b- defN 20-Feb-02 00:00 pybppibridge-0.4.8.dist-info/RECORD
+40 files, 139081 bytes uncompressed, 44344 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
 Filename: setup-old.py
 Comment: 
 
-Filename: src/__init__.py
+Filename: src/__init__.py.py
 Comment: 
 
 Filename: src/bppibridge.py
 Comment: 
 
 Filename: src/bppibridgesq.py
 Comment: 
@@ -99,23 +99,23 @@
 
 Filename: src/utils/constants.py
 Comment: 
 
 Filename: src/utils/log.py
 Comment: 
 
-Filename: pybppibridge-0.4.7.dist-info/METADATA
+Filename: pybppibridge-0.4.8.dist-info/METADATA
 Comment: 
 
-Filename: pybppibridge-0.4.7.dist-info/WHEEL
+Filename: pybppibridge-0.4.8.dist-info/WHEEL
 Comment: 
 
-Filename: pybppibridge-0.4.7.dist-info/entry_points.txt
+Filename: pybppibridge-0.4.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: pybppibridge-0.4.7.dist-info/licenses/LICENSE
+Filename: pybppibridge-0.4.8.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: pybppibridge-0.4.7.dist-info/RECORD
+Filename: pybppibridge-0.4.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pybppibridge-0.4.7.dist-info/METADATA` & `pybppibridge-0.4.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBPPIBridge
-Version: 0.4.7
+Version: 0.4.8
 Summary: This solution builds a bridge between Blue Prism Process Intelligence (alias BPPI) and some external data sources (like files, databases via ODBC, SAP and Blue Prism).
 Project-URL: Source, https://github.com/datacorner/pyBPPIBridge
 Project-URL: Bug Tracker, https://github.com/datacorner/pyBPPIBridge/issues
 Project-URL: Homepage, https://github.com/datacorner/pyBPPIBridge/wiki
 Author-email: Benoit Cayla <benoit@datacorner.fr>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
```

## Comparing `pybppibridge-0.4.7.dist-info/licenses/LICENSE` & `pybppibridge-0.4.8.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `pybppibridge-0.4.7.dist-info/RECORD` & `pybppibridge-0.4.8.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 setup-old.py,sha256=gIRT-uidnfhTF-W0Q1I6w439b7jJ5wu4czTbkmfy3Dg,1730
-src/__init__.py,sha256=9kGcRfJu36qnjJnaXXUZI3gt2gVkJqLDJOPMPjignDU,391
+src/__init__.py.py,sha256=9kGcRfJu36qnjJnaXXUZI3gt2gVkJqLDJOPMPjignDU,391
 src/bppibridge.py,sha256=8oD8tN4SpSfRi4dgfTX4PBPUF-9QhKJoezzx0ek9w44,145
 src/bppibridgesq.py,sha256=Bvwp-W6S6O1HYdUmiwL6cM5MYHcTbyKUAQDpmDj5Rnw,401
 src/bppiapi/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/bppiapi/bppiPipeline.py,sha256=fahyQhu2WFmIM8-QetUPxMlIVIIbkvUcDXVbRv3FYsc,9566
 src/bppiapi/uploadConfig.py,sha256=wwR3Ky1GKLnbVmntfCI7st5Ldc2Rw7oJNoeIFJoz5V0,1188
 src/bppiapi/project/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/bppiapi/project/bppiApiProjectWrapper.py,sha256=3hHLCSg0h7DOqcCp-dtlbB73jP1w734No0fnM7SQiEI,930
@@ -29,12 +29,12 @@
 src/pipelines/repository/bppiPLRExcelFile.py,sha256=A_neAsONhb43hMwi6ThE5ZsAPhYS35ekgatcIpDfMPE,1606
 src/pipelines/repository/bppiPLRODBC.py,sha256=-eDrXOt3TvCKPbqGz6sigflSzztaIgWUdOBJ-eIuCBU,2437
 src/pipelines/repository/bppiPLRSAPRfcTable.py,sha256=oIgi9DY9w_22bHZja_Mq_wnJhAjos191y9_JUWRtoeE,5067
 src/pipelines/repository/bppiPLRXESFile.py,sha256=d-3EqwE57ve4Ky0yM9tb-SkeFnD8fODO9c-c0MO7FYg,1331
 src/utils/__init__.py,sha256=nGIxdrhitBu5XgEjM5Q0sBnWby1TIwhpGU22MCyoKE0,537
 src/utils/constants.py,sha256=ZKGSiu7S9eUWBxGhSCNPnYp4zIzFsSgC4NRjHP6DdSs,8851
 src/utils/log.py,sha256=i1bNdQV9wOlNjjUFlT5iTxKxgI-li26DI4-IGhU0cI8,2016
-pybppibridge-0.4.7.dist-info/METADATA,sha256=HDplxfdZkjlfboXGC-TA2Zz0mQqjnjz86-hkZ-tFMmQ,3997
-pybppibridge-0.4.7.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-pybppibridge-0.4.7.dist-info/entry_points.txt,sha256=pBbss7e8g9wopGxcuuy7UkA9WeAxvcVkP-TxlNaPYag,47
-pybppibridge-0.4.7.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-pybppibridge-0.4.7.dist-info/RECORD,,
+pybppibridge-0.4.8.dist-info/METADATA,sha256=Ll1YYh9PPbHkX1xPhnXbX1DAaPT_tTqZJEHLV3-sw7w,3997
+pybppibridge-0.4.8.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+pybppibridge-0.4.8.dist-info/entry_points.txt,sha256=LHCV5aK-I0TQeTisLah1Bg5Bc8N5z4ucB6FBnjX4_Fc,36
+pybppibridge-0.4.8.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+pybppibridge-0.4.8.dist-info/RECORD,,
```


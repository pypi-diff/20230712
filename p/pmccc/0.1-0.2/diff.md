# Comparing `tmp/pmccc-0.1-py3-none-any.whl.zip` & `tmp/pmccc-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5982 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       40 b- defN 23-Jul-10 05:43 pmcll/__init__.py
--rw-rw-rw-  2.0 fat       94 b- defN 23-Jul-11 06:38 pmcll/errors.py
--rw-rw-rw-  2.0 fat     4053 b- defN 23-Jul-11 11:02 pmcll/func.py
--rw-rw-rw-  2.0 fat     8462 b- defN 23-Jul-11 11:42 pmcll/main.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-11 23:56 pmccc-0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      578 b- defN 23-Jul-11 23:56 pmccc-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 23:56 pmccc-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-11 23:56 pmccc-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      646 b- defN 23-Jul-11 23:56 pmccc-0.1.dist-info/RECORD
-9 files, 15037 bytes uncompressed, 4882 bytes compressed:  67.5%
+Zip file size: 5974 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       40 b- defN 23-Jul-10 05:43 pmccc/__init__.py
+-rw-rw-rw-  2.0 fat       94 b- defN 23-Jul-11 06:38 pmccc/errors.py
+-rw-rw-rw-  2.0 fat     4053 b- defN 23-Jul-11 11:02 pmccc/func.py
+-rw-rw-rw-  2.0 fat     8462 b- defN 23-Jul-11 23:59 pmccc/main.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-12 00:00 pmccc-0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      576 b- defN 23-Jul-12 00:00 pmccc-0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 00:00 pmccc-0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-12 00:00 pmccc-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      646 b- defN 23-Jul-12 00:00 pmccc-0.2.dist-info/RECORD
+9 files, 15035 bytes uncompressed, 4874 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: pmcll/__init__.py
+Filename: pmccc/__init__.py
 Comment: 
 
-Filename: pmcll/errors.py
+Filename: pmccc/errors.py
 Comment: 
 
-Filename: pmcll/func.py
+Filename: pmccc/func.py
 Comment: 
 
-Filename: pmcll/main.py
+Filename: pmccc/main.py
 Comment: 
 
-Filename: pmccc-0.1.dist-info/LICENSE
+Filename: pmccc-0.2.dist-info/LICENSE
 Comment: 
 
-Filename: pmccc-0.1.dist-info/METADATA
+Filename: pmccc-0.2.dist-info/METADATA
 Comment: 
 
-Filename: pmccc-0.1.dist-info/WHEEL
+Filename: pmccc-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pmccc-0.1.dist-info/top_level.txt
+Filename: pmccc-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pmccc-0.1.dist-info/RECORD
+Filename: pmccc-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pmcll/func.py` & `pmccc/func.py`

 * *Files identical despite different names*

## Comparing `pmcll/main.py` & `pmccc/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     def __init__( self , cp_lib : list[ dict ] , natives_lib : list[ dict ] ) -> None :
         self.libs = [ i[ "path" ] for i in cp_lib ]
         self.natives = [ i[ "path" ] for i in natives_lib ]
 
 class main :
     """
-    pmcll
+    pmccc
     """
 
     def __init__( self , path : str = ".minecraft" , name : str = "" , version : str = "" ) -> None :
         """
         init
         """
         path = os.path.abspath( path )
```

## Comparing `pmccc-0.1.dist-info/LICENSE` & `pmccc-0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pmccc-0.1.dist-info/METADATA` & `pmccc-0.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pmccc
-Version: 0.1
+Version: 0.2
 Summary: python minecraft launcher library
-Home-page: https://github.com/cueavy/pmcll
+Home-page: https://github.com/cueavy/pmccc
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align = "center" >
-    <h1>pmcll</h1>
+    <h1>pmccc</h1>
 
-*python minecraft launcher library*
+python minecraft launcher library
 
 ---
 
 [
 en_us
 |
 [zh_cn](./README-zh_cn.md)
```

## Comparing `pmccc-0.1.dist-info/RECORD` & `pmccc-0.2.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pmcll/__init__.py,sha256=3zgfLJXjSnQLtr4sbH6RNObbfrkZqiP_NoyZlM6QVic,40
-pmcll/errors.py,sha256=lSj1d9fuMp_yvTjRgSVhLWWhmSIPatCE03aFJZGDUoM,94
-pmcll/func.py,sha256=bV35xm_7jB01-QoYjRwPKJ_FesV_rphkc-5iO6l93es,4053
-pmcll/main.py,sha256=QbaW3ymJt8u_SODjJEF3DR5RBfTllfyDik0dRA92HJA,8462
-pmccc-0.1.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
-pmccc-0.1.dist-info/METADATA,sha256=7vOjd1FpsdwVQsoa5Yq-fMd9QCCPfq4PdQM6M-F-Qas,578
-pmccc-0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pmccc-0.1.dist-info/top_level.txt,sha256=WFR05F06T0-dH7fUHwbISS0gv8TvOCNaPF8HTgmD65I,6
-pmccc-0.1.dist-info/RECORD,,
+pmccc/__init__.py,sha256=3zgfLJXjSnQLtr4sbH6RNObbfrkZqiP_NoyZlM6QVic,40
+pmccc/errors.py,sha256=lSj1d9fuMp_yvTjRgSVhLWWhmSIPatCE03aFJZGDUoM,94
+pmccc/func.py,sha256=bV35xm_7jB01-QoYjRwPKJ_FesV_rphkc-5iO6l93es,4053
+pmccc/main.py,sha256=3_zR4UWo6TxewN5RumSMWEvpV-YFFMUZjpq3PzytHEs,8462
+pmccc-0.2.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
+pmccc-0.2.dist-info/METADATA,sha256=4EgSgM-_GXQUMM9fq-Ws6TdbqRdANzi3Jlk0LUjT9Qw,576
+pmccc-0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pmccc-0.2.dist-info/top_level.txt,sha256=O0b_1G066AzCf9WK2XauqnZq8yActFXV2qkqv93i1ck,6
+pmccc-0.2.dist-info/RECORD,,
```


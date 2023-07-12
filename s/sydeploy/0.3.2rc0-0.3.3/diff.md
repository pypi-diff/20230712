# Comparing `tmp/sydeploy-0.3.2rc0-py3-none-any.whl.zip` & `tmp/sydeploy-0.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,20 @@
-Zip file size: 5926 bytes, number of entries: 16
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:39 sydeploy/__init__.py
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-12 07:39 sydeploy/errors.py
--rw-r--r--  2.0 unx      132 b- defN 23-Jul-12 07:39 sydeploy/run.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:39 sydeploy/commands/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:39 sydeploy/commands/authenticate/__init__.py
--rw-r--r--  2.0 unx     2813 b- defN 23-Jul-12 07:39 sydeploy/commands/authenticate/aws.py
--rw-r--r--  2.0 unx      388 b- defN 23-Jul-12 07:39 sydeploy/templates/meta.yaml.dist
--rw-r--r--  2.0 unx      291 b- defN 23-Jul-12 07:39 sydeploy/templates/setup.py.dist
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:39 sydeploy/utils/__init__.py
--rw-r--r--  2.0 unx     2031 b- defN 23-Jul-12 07:39 sydeploy/utils/simple.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Jul-12 07:40 sydeploy-0.3.2rc0.dist-info/LICENSE
--rw-r--r--  2.0 unx      285 b- defN 23-Jul-12 07:40 sydeploy-0.3.2rc0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 07:40 sydeploy-0.3.2rc0.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 07:40 sydeploy-0.3.2rc0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-12 07:40 sydeploy-0.3.2rc0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1333 b- defN 23-Jul-12 07:40 sydeploy-0.3.2rc0.dist-info/RECORD
-16 files, 8638 bytes uncompressed, 3690 bytes compressed:  57.3%
+Zip file size: 8113 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:56 sydeploy/__init__.py
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-12 07:56 sydeploy/errors.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jul-12 07:56 sydeploy/run.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:56 sydeploy/commands/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:56 sydeploy/commands/authenticate/__init__.py
+-rw-r--r--  2.0 unx     2813 b- defN 23-Jul-12 07:56 sydeploy/commands/authenticate/aws.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:56 sydeploy/commands/build/__init__.py
+-rw-r--r--  2.0 unx     6552 b- defN 23-Jul-12 07:56 sydeploy/commands/build/python_package.py
+-rw-r--r--  2.0 unx      388 b- defN 23-Jul-12 07:56 sydeploy/templates/meta.yaml.dist
+-rw-r--r--  2.0 unx      291 b- defN 23-Jul-12 07:56 sydeploy/templates/setup.py.dist
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-12 07:56 sydeploy/utils/__init__.py
+-rw-r--r--  2.0 unx     2031 b- defN 23-Jul-12 07:56 sydeploy/utils/simple.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jul-12 07:57 sydeploy-0.3.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      282 b- defN 23-Jul-12 07:57 sydeploy-0.3.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 07:57 sydeploy-0.3.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 07:57 sydeploy-0.3.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-12 07:57 sydeploy-0.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1502 b- defN 23-Jul-12 07:57 sydeploy-0.3.3.dist-info/RECORD
+18 files, 15356 bytes uncompressed, 5609 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -12,38 +12,44 @@
 
 Filename: sydeploy/commands/authenticate/__init__.py
 Comment: 
 
 Filename: sydeploy/commands/authenticate/aws.py
 Comment: 
 
+Filename: sydeploy/commands/build/__init__.py
+Comment: 
+
+Filename: sydeploy/commands/build/python_package.py
+Comment: 
+
 Filename: sydeploy/templates/meta.yaml.dist
 Comment: 
 
 Filename: sydeploy/templates/setup.py.dist
 Comment: 
 
 Filename: sydeploy/utils/__init__.py
 Comment: 
 
 Filename: sydeploy/utils/simple.py
 Comment: 
 
-Filename: sydeploy-0.3.2rc0.dist-info/LICENSE
+Filename: sydeploy-0.3.3.dist-info/LICENSE
 Comment: 
 
-Filename: sydeploy-0.3.2rc0.dist-info/METADATA
+Filename: sydeploy-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: sydeploy-0.3.2rc0.dist-info/WHEEL
+Filename: sydeploy-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: sydeploy-0.3.2rc0.dist-info/entry_points.txt
+Filename: sydeploy-0.3.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: sydeploy-0.3.2rc0.dist-info/top_level.txt
+Filename: sydeploy-0.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: sydeploy-0.3.2rc0.dist-info/RECORD
+Filename: sydeploy-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sydeploy-0.3.2rc0.dist-info/LICENSE` & `sydeploy-0.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sydeploy-0.3.2rc0.dist-info/RECORD` & `sydeploy-0.3.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 sydeploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/errors.py,sha256=BU5F1x81--SV7aVxynoUEHlu6b9LDFiQf2GnNazcs9c,149
 sydeploy/run.py,sha256=xBsWk4Qstmslp8XZGyEiZSd8_gMfPR8lCaX7BQ-hbWg,132
 sydeploy/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/commands/authenticate/aws.py,sha256=_rzQx_fvSQwmEZHvZM8SlvLuD78dsy2I1MmRBodLkCU,2813
+sydeploy/commands/build/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+sydeploy/commands/build/python_package.py,sha256=Mhjbl8wAcZXCPTgK6vBuqihgldCns049viPPfhBFXqY,6552
 sydeploy/templates/meta.yaml.dist,sha256=XkJkfyrFwtMQqhrZaRNiCx_1TCbSMT1gz7TX0ngQcmc,388
 sydeploy/templates/setup.py.dist,sha256=0GlvFdAMVQNftMm3mpJkxhJCNn6vUXc2K9nUWIbNQq4,291
 sydeploy/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sydeploy/utils/simple.py,sha256=PyKPFVZmqpnS5yXe6j3CO3h5PoIPg_TOqo71qnFIPgo,2031
-sydeploy-0.3.2rc0.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
-sydeploy-0.3.2rc0.dist-info/METADATA,sha256=ze8dildN-uVTRfiex8xByPLOJ7awHVAN9ZHcUomAPy4,285
-sydeploy-0.3.2rc0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sydeploy-0.3.2rc0.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
-sydeploy-0.3.2rc0.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
-sydeploy-0.3.2rc0.dist-info/RECORD,,
+sydeploy-0.3.3.dist-info/LICENSE,sha256=pmd0NHLeCsH7lpQg9c9Jpnwa_aJJ7WGt0BqNsuLgxms,1068
+sydeploy-0.3.3.dist-info/METADATA,sha256=5rh8qCSfoOyCQX8bAeu0PLWYuJSdcu0zZrQoVdpBs-0,282
+sydeploy-0.3.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sydeploy-0.3.3.dist-info/entry_points.txt,sha256=tcEB8hDNecfsMI9wjFFyBlT_rqbyrQJysC37mnVJh_k,47
+sydeploy-0.3.3.dist-info/top_level.txt,sha256=O0Z6wX9X7D0NIUa35bKUU1UTaTS_QxPh0yE2HXdG5QE,9
+sydeploy-0.3.3.dist-info/RECORD,,
```


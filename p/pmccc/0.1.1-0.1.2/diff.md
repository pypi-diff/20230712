# Comparing `tmp/pmccc-0.1.1-py3-none-any.whl.zip` & `tmp/pmccc-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7325 bytes, number of entries: 10
+Zip file size: 7473 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Jul-12 03:13 pmccc/__init__.py
 -rw-rw-rw-  2.0 fat      920 b- defN 23-Jul-12 04:03 pmccc/__main__.py
 -rw-rw-rw-  2.0 fat      137 b- defN 23-Jul-12 02:17 pmccc/errors.py
 -rw-rw-rw-  2.0 fat     4118 b- defN 23-Jul-12 03:58 pmccc/func.py
--rw-rw-rw-  2.0 fat    11497 b- defN 23-Jul-12 04:05 pmccc/main.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-12 04:11 pmccc-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      578 b- defN 23-Jul-12 04:11 pmccc-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 04:11 pmccc-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-12 04:11 pmccc-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      731 b- defN 23-Jul-12 04:11 pmccc-0.1.1.dist-info/RECORD
-10 files, 19185 bytes uncompressed, 6095 bytes compressed:  68.2%
+-rw-rw-rw-  2.0 fat    11524 b- defN 23-Jul-12 05:03 pmccc/main.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-12 05:09 pmccc-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      883 b- defN 23-Jul-12 05:09 pmccc-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 05:09 pmccc-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-12 05:09 pmccc-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      731 b- defN 23-Jul-12 05:09 pmccc-0.1.2.dist-info/RECORD
+10 files, 19517 bytes uncompressed, 6243 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pmccc/func.py
 Comment: 
 
 Filename: pmccc/main.py
 Comment: 
 
-Filename: pmccc-0.1.1.dist-info/LICENSE
+Filename: pmccc-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: pmccc-0.1.1.dist-info/METADATA
+Filename: pmccc-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: pmccc-0.1.1.dist-info/WHEEL
+Filename: pmccc-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: pmccc-0.1.1.dist-info/top_level.txt
+Filename: pmccc-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pmccc-0.1.1.dist-info/RECORD
+Filename: pmccc-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmccc/main.py

```diff
@@ -82,15 +82,15 @@
 
     def get_manifest( self ) -> dict :
         """
         get manifest
         """
         return func.json_get( self.url_replace( self.urls[ "minecraft" ][ "manifest" ] ) , os.path.join( self.path[ "versions" ] , "manifest.json" ) )
 
-    def get_javas( self ) -> list :
+    def java_get( self ) -> list :
         """
         get_javas
         """
         self.javas = {}
         for i in os.environ[ "PATH" ].split( self.cp_split ) :
             if "bin" in i and os.path.exists( i ) :
                 for file in os.listdir( i ) :
@@ -180,14 +180,15 @@
             json_data = json.load( file )
         natives_lib = []
         cp_lib = []
         files = []
         for i in json_data[ "libraries" ] :
             use = True
             if "rules" in i :
+                use = False
                 for r in i["rules"] :
                     if "os" in r :
                         if self.os not in r[ "os" ].values() :
                             continue
                     use = func.use_dict[ r[ "action" ] ]
             if not use :
                 continue
@@ -228,15 +229,15 @@
         return self.args( lib , player , version )
 
     def run( self , player : player , version : str , java : str = None ) :
         """
         run
         """
         if java == None :
-            self.get_javas()
+            self.java_get()
             java = os.path.join( self.java( version )[ 0 ] , "java" )
         args = self.get( player , version )
         os.system( f"{ java } {args}" )
 
     def args( self , lib : libs , player : player , version : str ) :
         """
         args
```

## Comparing `pmccc-0.1.1.dist-info/LICENSE` & `pmccc-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*


# Comparing `tmp/pmccc-0.1-py3-none-any.whl.zip` & `tmp/pmccc-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
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
+Zip file size: 7325 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat       40 b- defN 23-Jul-12 03:13 pmccc/__init__.py
+-rw-rw-rw-  2.0 fat      920 b- defN 23-Jul-12 04:03 pmccc/__main__.py
+-rw-rw-rw-  2.0 fat      137 b- defN 23-Jul-12 02:17 pmccc/errors.py
+-rw-rw-rw-  2.0 fat     4118 b- defN 23-Jul-12 03:58 pmccc/func.py
+-rw-rw-rw-  2.0 fat    11497 b- defN 23-Jul-12 04:05 pmccc/main.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-12 04:11 pmccc-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      578 b- defN 23-Jul-12 04:11 pmccc-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 04:11 pmccc-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-12 04:11 pmccc-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      731 b- defN 23-Jul-12 04:11 pmccc-0.1.1.dist-info/RECORD
+10 files, 19185 bytes uncompressed, 6095 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
-Filename: pmcll/__init__.py
+Filename: pmccc/__init__.py
 Comment: 
 
-Filename: pmcll/errors.py
+Filename: pmccc/__main__.py
 Comment: 
 
-Filename: pmcll/func.py
+Filename: pmccc/errors.py
 Comment: 
 
-Filename: pmcll/main.py
+Filename: pmccc/func.py
 Comment: 
 
-Filename: pmccc-0.1.dist-info/LICENSE
+Filename: pmccc/main.py
 Comment: 
 
-Filename: pmccc-0.1.dist-info/METADATA
+Filename: pmccc-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pmccc-0.1.dist-info/WHEEL
+Filename: pmccc-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pmccc-0.1.dist-info/top_level.txt
+Filename: pmccc-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pmccc-0.1.dist-info/RECORD
+Filename: pmccc-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: pmccc-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pmcll/func.py` & `pmccc/func.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,19 @@
             "libraries" : "download.mcbbs.net/maven" ,
             "forge" : "download.mcbbs.net/maven" ,
             "fabric-meta" : "download.mcbbs.net/fabric-meta" ,
             "fabric" : "download.mcbbs.net/maven"
     }
 }
 
+use_dict = {
+    "allow" : True ,
+    "disallow" : False
+}
+
 def hash( data : str ) -> str :
     hash = hashlib.sha1()
     hash.update( data )
     return hash.hexdigest().lower()
 
 def file_hash( path : str ) -> str :
     """
```

## Comparing `pmcll/main.py` & `pmccc/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,128 @@
 """
 main
 """
 
 from .errors import *
 from . import func
 
-import requests
+import subprocess
 import zipfile
 import json
 import sys
 import os
 
 class libs :
     """
     libs
     """
 
     def __init__( self , cp_lib : list[ dict ] , natives_lib : list[ dict ] ) -> None :
         self.libs = [ i[ "path" ] for i in cp_lib ]
         self.natives = [ i[ "path" ] for i in natives_lib ]
 
+
+class player :
+    """
+    player
+    """
+
+    def __init__( self , name : str , uuid : str = None ) -> None :
+        self.online = False
+        if uuid == None :
+            self.uuid = "a0a1a2a3a4a5a6a7fb1b2b3b4b5b6b7f"
+        self.token = self.uuid
+        self.name = name
+
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
         self.path = {
             "libraries" : os.path.join( path , "libraries" ) ,
             "versions" : os.path.join( path , "versions" ) ,
             "assets" : os.path.join( path , "assets" ) ,
             "root" : path
         }
+        self.java_use = {
+            8 : [ "1.8" ] ,
+            16 : [ "16" , "17" ] ,
+            17 : [ "17" , "18" , "19" ] ,
+        }
         for path in self.path.values() :
             func.mkdir( path )
         os_type = sys.platform
+        self.cp_split = ":"
         if os_type == "win32" :
             self.os = "windows"
+            self.cp_split = ";"
         elif os_type == "linux" :
             self.os = "linux"
         else :
             self.os = "osx"
         self.use_url = "minecraft"
         self.urls = func.url_dict
         self.version = version
         self.name = name
+        self.javas = {}
 
     def url_replace( self , url : str ) -> str :
         """
         url replace
         """
         if self.use_url == "minecraft" :
             return url
         else :
             return func.url_replace( url , self.urls[ self.use_url ] , self.urls )
 
     def get_manifest( self ) -> dict :
         """
         get manifest
         """
-        data = requests.get( self.url_replace( self.urls[ "minecraft" ][ "manifest" ] ) )
-        if data.status_code == 200 :
-            return data.json()
-        else :
-            raise StatusError( data.status_code )
+        return func.json_get( self.url_replace( self.urls[ "minecraft" ][ "manifest" ] ) , os.path.join( self.path[ "versions" ] , "manifest.json" ) )
+
+    def get_javas( self ) -> list :
+        """
+        get_javas
+        """
+        self.javas = {}
+        for i in os.environ[ "PATH" ].split( self.cp_split ) :
+            if "bin" in i and os.path.exists( i ) :
+                for file in os.listdir( i ) :
+                    if file in [ "javaw.exe" , "javaw" ] :
+                        for l in subprocess.check_output( [ os.path.join( i , "java" ) , "-version" ] , stderr = subprocess.STDOUT ).decode().split( "\"" ) :
+                            for s in l :
+                                if s not in [ str( n ) for n in range( 10 ) ] + [ "." , "_" , "-" ] :
+                                    break
+                            else :
+                                self.javas[ l ] = i
+        if not len( self.javas.items() ) :
+            raise func.JavaNotFindError()
+        return self.javas
+
+    def java( self , version : str ) -> str :
+        path = os.path.join( self.path[ "versions" ] , version , version + ".json" )
+        with open( path , "rb" ) as file :
+            json_data = json.load( file )
+        java_version = json_data[ "javaVersion" ][ "majorVersion" ]
+        javas = self.java_use[ java_version ]
+        ret = []
+        for key , value in self.javas.items() :
+            for i in javas :
+                if i in key :
+                    ret.append( value )
+        if not len( ret ) :
+            raise JavaNotFindError( javas )
+        return ret
 
     def install_version( self , mc_version : str , version : str , manifest : dict = None , jar_type : str = "client" ) -> None :
         """
         install version
         """
         name = version
         if not os.path.isabs( name ) :
@@ -127,16 +178,25 @@
         path = self.path[ "libraries" ]
         with open( os.path.join( self.path[ "versions" ] , name , name + ".json" ) , "r" , encoding = "utf-8" ) as file :
             json_data = json.load( file )
         natives_lib = []
         cp_lib = []
         files = []
         for i in json_data[ "libraries" ] :
+            use = True
+            if "rules" in i :
+                for r in i["rules"] :
+                    if "os" in r :
+                        if self.os not in r[ "os" ].values() :
+                            continue
+                    use = func.use_dict[ r[ "action" ] ]
+            if not use :
+                continue
             if "classifiers" in i[ "downloads" ] :
-                if self.os in i[ "natives" ] :
+                if self.os in i[ "natives" ] and i[ "natives" ][ self.os ] in i[ "downloads" ][ "classifiers" ] :
                     natives_lib.append( i[ "downloads" ][ "classifiers" ][ i[ "natives" ][ self.os ] ] )
                     natives_lib[ -1 ][ "path" ] = os.path.join( path , natives_lib[ -1 ][ "path" ] )
             else :
                 cp_lib.append( i[ "downloads" ][ "artifact" ] )
                 cp_lib[ -1 ][ "path" ] = os.path.join( path , cp_lib[ -1 ][ "path" ] )
         for i in natives_lib + cp_lib :
             files.append( {
@@ -144,26 +204,51 @@
                 "path" : os.path.join( path , i[ "path" ] ) ,
                 "sha1" : i[ "sha1" ]
                 } )
         func.files_get( files )
         return libs( cp_lib , natives_lib )
 
     def unzip_natives( self , lib : libs , version : str ) -> None :
+        """
+        unzip natives
+        """
         name = version
         path = os.path.join( self.path[ "versions" ] , name , f"{ name }-natives" )
         func.mkdir( path )
         for i in lib.natives :
             with zipfile.ZipFile( i ) as file :
                 file.extractall( path )
 
-    def args( self , lib : libs , version : str ) :
+    def get( self , player : player , version : str ) :
+        """
+        get
+        """
+        lib = self.install_libraries( version )
+        self.install_assets( version )
+        self.unzip_natives( lib , version )
+        return self.args( lib , player , version )
+
+    def run( self , player : player , version : str , java : str = None ) :
+        """
+        run
+        """
+        if java == None :
+            self.get_javas()
+            java = os.path.join( self.java( version )[ 0 ] , "java" )
+        args = self.get( player , version )
+        os.system( f"{ java } {args}" )
+
+    def args( self , lib : libs , player : player , version : str ) :
+        """
+        args
+        """
         lib_str = ""
         args = ""
         for i in lib.libs :
-            lib_str += i + ";"
+            lib_str += i + self.cp_split
         path = os.path.join( self.path[ "versions" ] , version )
         natives = os.path.join( path , f"{ version }-natives" )
         with open( os.path.join( path , version + ".json" ) , "rb" ) as file :
             json_data = json.load( file )
         main_class = json_data[ "mainClass" ]
         lib_str = f"""\"{ lib_str }{ os.path.join( path , version + ".jar" ) }\" { main_class }"""
 
@@ -199,16 +284,16 @@
 
         return args.replace("${auth_player_name}" , "Dev" ) \
         .replace("${version_name}" , version ) \
         .replace("${game_directory}" , f"\"{ path }\"" ) \
         .replace("${assets_root}" , f"""\"{ self.path[ "assets" ] }\"""" ) \
         .replace("${game_assets}" , f"""\"{ self.path[ "assets" ] }\"""" ) \
         .replace("${assets_index_name}" , json_data["assets"] ) \
-        .replace("${auth_uuid}" , "0000000000003006998F555B11390A71" ) \
-        .replace("${auth_access_token}" , "0000000000003006998F555B11390A71" ) \
+        .replace("${auth_uuid}" , player.uuid ) \
+        .replace("${auth_access_token}" , player.token ) \
         .replace("${user_type}" , "msa" ) \
         .replace("${version_type}" , self.name ) \
         .replace("${natives_directory}" , f"\"{ natives }\"" ) \
         .replace("${launcher_name}" , self.name ) \
         .replace("${launcher_version}" , self.version ) \
         .replace("${classpath}" , lib_str ) \
         .replace("${library_directory}" , f"""\"{ self.path[ "libraries" ] }\"""" ) \
```

## Comparing `pmccc-0.1.dist-info/LICENSE` & `pmccc-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pmccc-0.1.dist-info/METADATA` & `pmccc-0.1.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pmccc
-Version: 0.1
+Version: 0.1.1
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


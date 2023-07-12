# Comparing `tmp/sbpack-2023.6.20rc1-py3-none-any.whl.zip` & `tmp/sbpack-2023.6.20rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 29377 bytes, number of entries: 17
+Zip file size: 29559 bytes, number of entries: 17
 -rw-r--r--  2.0 unx        0 b- defN 23-May-09 11:19 sbpack/__init__.py
 -rw-r--r--  2.0 unx     5781 b- defN 23-May-09 11:19 sbpack/lib.py
 -rw-r--r--  2.0 unx    13365 b- defN 23-May-09 11:19 sbpack/pack.py
 -rw-r--r--  2.0 unx     7929 b- defN 23-Jun-22 11:09 sbpack/schemadef.py
 -rw-r--r--  2.0 unx     3064 b- defN 23-May-09 11:19 sbpack/unpack.py
--rw-r--r--  2.0 unx       30 b- defN 23-Jun-26 10:29 sbpack/version.py
+-rw-r--r--  2.0 unx       30 b- defN 23-Jul-12 10:22 sbpack/version.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-09 11:19 sbpack/noncwl/__init__.py
 -rw-r--r--  2.0 unx     1591 b- defN 23-May-09 11:19 sbpack/noncwl/copy.py
--rw-r--r--  2.0 unx    18891 b- defN 23-Jun-20 11:52 sbpack/noncwl/nextflow.py
--rw-r--r--  2.0 unx     5591 b- defN 23-Jun-16 09:21 sbpack/noncwl/utils.py
+-rw-r--r--  2.0 unx    19256 b- defN 23-Jul-12 08:37 sbpack/noncwl/nextflow.py
+-rw-r--r--  2.0 unx     5666 b- defN 23-Jul-12 08:39 sbpack/noncwl/utils.py
 -rw-r--r--  2.0 unx    10528 b- defN 23-May-09 11:19 sbpack/noncwl/wdl.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-26 10:29 sbpack-2023.6.20rc1.dist-info/LICENSE
--rw-r--r--  2.0 unx     7479 b- defN 23-Jun-26 10:29 sbpack-2023.6.20rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 10:29 sbpack-2023.6.20rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx      214 b- defN 23-Jun-26 10:29 sbpack-2023.6.20rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-26 10:29 sbpack-2023.6.20rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1350 b- defN 23-Jun-26 10:29 sbpack-2023.6.20rc1.dist-info/RECORD
-17 files, 87269 bytes uncompressed, 27173 bytes compressed:  68.9%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-12 10:22 sbpack-2023.6.20rc2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7479 b- defN 23-Jul-12 10:22 sbpack-2023.6.20rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 10:22 sbpack-2023.6.20rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      214 b- defN 23-Jul-12 10:22 sbpack-2023.6.20rc2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-12 10:22 sbpack-2023.6.20rc2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1350 b- defN 23-Jul-12 10:22 sbpack-2023.6.20rc2.dist-info/RECORD
+17 files, 87709 bytes uncompressed, 27355 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: sbpack/noncwl/utils.py
 Comment: 
 
 Filename: sbpack/noncwl/wdl.py
 Comment: 
 
-Filename: sbpack-2023.6.20rc1.dist-info/LICENSE
+Filename: sbpack-2023.6.20rc2.dist-info/LICENSE
 Comment: 
 
-Filename: sbpack-2023.6.20rc1.dist-info/METADATA
+Filename: sbpack-2023.6.20rc2.dist-info/METADATA
 Comment: 
 
-Filename: sbpack-2023.6.20rc1.dist-info/WHEEL
+Filename: sbpack-2023.6.20rc2.dist-info/WHEEL
 Comment: 
 
-Filename: sbpack-2023.6.20rc1.dist-info/entry_points.txt
+Filename: sbpack-2023.6.20rc2.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbpack-2023.6.20rc1.dist-info/top_level.txt
+Filename: sbpack-2023.6.20rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: sbpack-2023.6.20rc1.dist-info/RECORD
+Filename: sbpack-2023.6.20rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbpack/version.py

```diff
@@ -1 +1 @@
-__version__ = "2023.06.20rc1"
+__version__ = "2023.06.20rc2"
```

## sbpack/noncwl/nextflow.py

```diff
@@ -16,14 +16,15 @@
     get_readme,
     update_schema_code_package,
     install_or_upgrade_app,
     validate_inputs,
     GENERIC_FILE_ARRAY_INPUT,
     GENERIC_OUTPUT_DIRECTORY,
     WRAPPER_REQUIREMENTS,
+    SKIP_NEXTFLOW_TOWER_KEYS,
 )
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 PACKAGE_SIZE_LIMIT = 100 * 1024 * 1024  # MB
 NF_SCHEMA_DEFAULT_NAME = 'nextflow_schema.json'
@@ -328,14 +329,20 @@
         :param yml_file: path to YAML file.
         :return: list of outputs in CWL format.
         """
         outputs = list()
         yml_schema = ruamel.yaml.safe_load(yml_file)
 
         for key, value in yml_schema.items():
+            # Tower yml file can use "tower" key in the yml file to designate
+            # some of the configurations tower uses. Since these are not output
+            # definitions, we skip these.
+            if key in SKIP_NEXTFLOW_TOWER_KEYS and \
+                    yml_file == 'tower.yml':
+                continue
             outputs.append(
                 self.make_output_type(key, value)
             )
 
         return outputs
 
     @staticmethod
@@ -489,16 +496,16 @@
         help="Revision note to be placed in the CWL schema if the app is "
              "uploaded to the sbg platform.",
     )
     parser.add_argument(
         "--manual-validation", required=False, action="store_true",
         default=False,
         help="You will have to provide validation for all 'string' type inputs"
-             " if are string (s), file (f), directory (d), list of file (lf),"
-             " or list of directory (ld) type inputs.",
+             " if are string (str), file (file), directory (dir), list of file"
+             " (files), or list of directory (dirs) type inputs.",
     )
 
     args = parser.parse_args()
 
     # Preprocess CLI parameter values
 
     sb_doc = None
```

## sbpack/noncwl/utils.py

```diff
@@ -43,14 +43,20 @@
         "listing": [
             "$(inputs.auxiliary_files)"
         ]
     }
 ]
 
 
+SKIP_NEXTFLOW_TOWER_KEYS = [
+    'tower',
+    'mail',
+]
+
+
 def validate_inputs(inputs):
     types = {
         'str': 'string',
         'file': 'File',
         'dir': 'Directory',
         'files': 'File[]',
         'dirs': 'Directory[]'
@@ -100,15 +106,15 @@
 
 def zip_and_push_to_sb(api, workflow_path, project_id, folder_name):
     """
     Create .zip package file. Upload .zip file to the designated folder
     for packages on SevenBridges Platform. Delete local .zip file.
     """
 
-    basename = os.path.basename(workflow_path) + '_' + \
+    basename = os.path.basename(os.path.abspath(workflow_path)) + '_' + \
                time.strftime("%Y%m%d-%H%M%S")
 
     zip_path = os.path.join(os.path.dirname(workflow_path), basename + '.zip')
     shutil.make_archive(zip_path[:-4], 'zip', root_dir=workflow_path,
                         base_dir='./')
 
     if os.path.getsize(zip_path) > PACKAGE_SIZE_LIMIT:
```

## Comparing `sbpack-2023.6.20rc1.dist-info/LICENSE` & `sbpack-2023.6.20rc2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbpack-2023.6.20rc1.dist-info/METADATA` & `sbpack-2023.6.20rc2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbpack
-Version: 2023.6.20rc1
+Version: 2023.6.20rc2
 Summary: Command line tool to upload and download CWL to and from SB powered platforms.
 Home-page: UNKNOWN
 Author: Seven Bridges
 Author-email: pavle.marinkovic@velsera.com
 Maintainer: Seven Bridges
 Maintainer-email: pavle.marinkovic@velsera.com
 License: UNKNOWN
```

## Comparing `sbpack-2023.6.20rc1.dist-info/RECORD` & `sbpack-2023.6.20rc2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 sbpack/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sbpack/lib.py,sha256=iLN5s31rS9Mg64teYZLk0Cicdjuyb6KdwCjL52r1nrQ,5781
 sbpack/pack.py,sha256=4vutKrWeas4NhtaLcHKIWfp-8pHMo3hkWR75oz6GTZw,13365
 sbpack/schemadef.py,sha256=9UVZNi5nUMJz5ZZM9j4z53X8Svizmc_eUTtl0mTapB8,7929
 sbpack/unpack.py,sha256=amyfuytRxvsz0-RARfP1Hm4tbpmMVCfLSaM8U3woh-o,3064
-sbpack/version.py,sha256=OwPQPMX4sRGU4qQqC9EXc0uItdURyTTo_Edsm1g7qAo,30
+sbpack/version.py,sha256=cbvH7ow8kBCTtMJ_Hx1HXp7gj58hLztjgRdMM6LU6mg,30
 sbpack/noncwl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sbpack/noncwl/copy.py,sha256=oMAJrGJ6FiU4BF2pyqUOcdTam9Ft64vL8n-ywAKIne8,1591
-sbpack/noncwl/nextflow.py,sha256=ggLKOOYzrbJzfsu3ei4Olq28MvTXRzalywfHuNTrGwo,18891
-sbpack/noncwl/utils.py,sha256=jdjyFvJK_-82iNNhU7QRtWCYWqXwxwODt1VXret5EqY,5591
+sbpack/noncwl/nextflow.py,sha256=hyabWMHRYMquFfuc0RKNeW6QhcLQJFK5HlqwE9V1Wt8,19256
+sbpack/noncwl/utils.py,sha256=Pfojwv5FYqJ-TZ1ZrkMytAUkgBB5IHwhdL0aOvUWrfo,5666
 sbpack/noncwl/wdl.py,sha256=-CqDLqbCiGOhnG5iEUJC2FMXZmorFggtGpeDtBpHWgU,10528
-sbpack-2023.6.20rc1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbpack-2023.6.20rc1.dist-info/METADATA,sha256=yXVkvN0myqHH5zBWhrOwRk6QXIGWoOV1JdtWnsvY2Ag,7479
-sbpack-2023.6.20rc1.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sbpack-2023.6.20rc1.dist-info/entry_points.txt,sha256=FkTSv3CUlZDSBAYV9d12g1Xn5baiWk0-w1giWiP7QtU,214
-sbpack-2023.6.20rc1.dist-info/top_level.txt,sha256=jYfNbA_EM0kCUdebAs2xxFukxE1XlzB_BbAr4t25Jmg,7
-sbpack-2023.6.20rc1.dist-info/RECORD,,
+sbpack-2023.6.20rc2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbpack-2023.6.20rc2.dist-info/METADATA,sha256=4wGl5vDVxLmb5oosqeKcQVYDkijcxKbaHnhn0x2IKVc,7479
+sbpack-2023.6.20rc2.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sbpack-2023.6.20rc2.dist-info/entry_points.txt,sha256=FkTSv3CUlZDSBAYV9d12g1Xn5baiWk0-w1giWiP7QtU,214
+sbpack-2023.6.20rc2.dist-info/top_level.txt,sha256=jYfNbA_EM0kCUdebAs2xxFukxE1XlzB_BbAr4t25Jmg,7
+sbpack-2023.6.20rc2.dist-info/RECORD,,
```


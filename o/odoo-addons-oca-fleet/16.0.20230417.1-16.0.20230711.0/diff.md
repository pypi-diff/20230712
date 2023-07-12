# Comparing `tmp/odoo_addons_oca_fleet-16.0.20230417.1-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_fleet-16.0.20230711.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1374 bytes, number of entries: 4
--rw-r--r--  2.0 unx      748 b- defN 23-Apr-18 04:13 odoo_addons_oca_fleet-16.0.20230417.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 04:13 odoo_addons_oca_fleet-16.0.20230417.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-18 04:13 odoo_addons_oca_fleet-16.0.20230417.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      392 b- defN 23-Apr-18 04:13 odoo_addons_oca_fleet-16.0.20230417.1.dist-info/RECORD
-4 files, 1233 bytes uncompressed, 600 bytes compressed:  51.3%
+Zip file size: 1383 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      823 b- defN 23-Jul-12 03:26 odoo_addons_oca_fleet-16.0.20230711.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 03:26 odoo_addons_oca_fleet-16.0.20230711.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-12 03:26 odoo_addons_oca_fleet-16.0.20230711.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      392 b- defN 23-Jul-12 03:26 odoo_addons_oca_fleet-16.0.20230711.0.dist-info/RECORD
+4 files, 1308 bytes uncompressed, 609 bytes compressed:  53.4%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_fleet-16.0.20230417.1.dist-info/METADATA
+Filename: odoo_addons_oca_fleet-16.0.20230711.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_fleet-16.0.20230417.1.dist-info/WHEEL
+Filename: odoo_addons_oca_fleet-16.0.20230711.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_fleet-16.0.20230417.1.dist-info/top_level.txt
+Filename: odoo_addons_oca_fleet-16.0.20230711.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_fleet-16.0.20230417.1.dist-info/RECORD
+Filename: odoo_addons_oca_fleet-16.0.20230711.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_fleet-16.0.20230417.1.dist-info/METADATA` & `odoo_addons_oca_fleet-16.0.20230711.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-fleet
-Version: 16.0.20230417.1
+Version: 16.0.20230711.0
 Summary: Meta package for oca-fleet Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-fleet-vehicle-calendar-year (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-fleet-vehicle-configuration (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-fleet-vehicle-fuel-capacity (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-fleet-vehicle-fuel-type-ethanol (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-fleet-vehicle-service-kanban (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-fleet-vehicle-service-services (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-fleet-vehicle-stock (<16.1dev,>=16.0dev)
 
 UNKNOWN
```


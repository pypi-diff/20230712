# Comparing `tmp/odoo_addons_oca_partner_contact-16.0.20230705.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_partner_contact-16.0.20230711.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1797 bytes, number of entries: 4
--rw-r--r--  2.0 unx     3273 b- defN 23-Jul-06 04:30 odoo_addons_oca_partner_contact-16.0.20230705.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 04:30 odoo_addons_oca_partner_contact-16.0.20230705.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-06 04:30 odoo_addons_oca_partner_contact-16.0.20230705.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      433 b- defN 23-Jul-06 04:30 odoo_addons_oca_partner_contact-16.0.20230705.0.dist-info/RECORD
-4 files, 3799 bytes uncompressed, 943 bytes compressed:  75.2%
+Zip file size: 1806 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     3423 b- defN 23-Jul-12 04:33 odoo_addons_oca_partner_contact-16.0.20230711.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 04:33 odoo_addons_oca_partner_contact-16.0.20230711.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-12 04:33 odoo_addons_oca_partner_contact-16.0.20230711.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      433 b- defN 23-Jul-12 04:33 odoo_addons_oca_partner_contact-16.0.20230711.1.dist-info/RECORD
+4 files, 3949 bytes uncompressed, 952 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_partner_contact-16.0.20230705.0.dist-info/METADATA
+Filename: odoo_addons_oca_partner_contact-16.0.20230711.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_partner_contact-16.0.20230705.0.dist-info/WHEEL
+Filename: odoo_addons_oca_partner_contact-16.0.20230711.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_partner_contact-16.0.20230705.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_partner_contact-16.0.20230711.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_partner_contact-16.0.20230705.0.dist-info/RECORD
+Filename: odoo_addons_oca_partner_contact-16.0.20230711.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_partner_contact-16.0.20230705.0.dist-info/METADATA` & `odoo_addons_oca_partner_contact-16.0.20230711.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-partner-contact
-Version: 16.0.20230705.0
+Version: 16.0.20230711.1
 Summary: Meta package for oca-partner-contact Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
+Requires-Dist: odoo-addon-account-partner-company-group (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-country-state-translatable (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-location (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-location-geonames-import (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-partner-company-group (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-base-partner-sequence (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-crm-partner-company-group (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-accreditation (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-address-split (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-address-street3 (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-address-two-lines (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-affiliate (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-bank-acc-type-constraint (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-capital (<16.1dev,>=16.0dev)
```


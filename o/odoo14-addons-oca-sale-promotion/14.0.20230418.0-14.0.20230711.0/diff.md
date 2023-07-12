# Comparing `tmp/odoo14_addons_oca_sale_promotion-14.0.20230418.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_sale_promotion-14.0.20230711.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1526 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1084 b- defN 23-Apr-19 06:28 odoo14_addons_oca_sale_promotion-14.0.20230418.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 06:28 odoo14_addons_oca_sale_promotion-14.0.20230418.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-19 06:28 odoo14_addons_oca_sale_promotion-14.0.20230418.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      437 b- defN 23-Apr-19 06:28 odoo14_addons_oca_sale_promotion-14.0.20230418.0.dist-info/RECORD
-4 files, 1614 bytes uncompressed, 664 bytes compressed:  58.9%
+Zip file size: 1538 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1171 b- defN 23-Jul-12 04:59 odoo14_addons_oca_sale_promotion-14.0.20230711.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 04:59 odoo14_addons_oca_sale_promotion-14.0.20230711.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-12 04:59 odoo14_addons_oca_sale_promotion-14.0.20230711.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      437 b- defN 23-Jul-12 04:59 odoo14_addons_oca_sale_promotion-14.0.20230711.0.dist-info/RECORD
+4 files, 1701 bytes uncompressed, 676 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_sale_promotion-14.0.20230418.0.dist-info/METADATA
+Filename: odoo14_addons_oca_sale_promotion-14.0.20230711.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_sale_promotion-14.0.20230418.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_sale_promotion-14.0.20230711.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_sale_promotion-14.0.20230418.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_sale_promotion-14.0.20230711.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_sale_promotion-14.0.20230418.0.dist-info/RECORD
+Filename: odoo14_addons_oca_sale_promotion-14.0.20230711.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_sale_promotion-14.0.20230418.0.dist-info/METADATA` & `odoo14_addons_oca_sale_promotion-14.0.20230711.0.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-sale-promotion
-Version: 14.0.20230418.0
+Version: 14.0.20230711.0
 Summary: Meta package for oca-sale-promotion Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
+Requires-Dist: odoo14-addon-coupon-limit
 Requires-Dist: odoo14-addon-sale-coupon-auto-refresh
 Requires-Dist: odoo14-addon-sale-coupon-criteria-multi-product
 Requires-Dist: odoo14-addon-sale-coupon-criteria-order-based
 Requires-Dist: odoo14-addon-sale-coupon-delivery-auto-refresh
 Requires-Dist: odoo14-addon-sale-coupon-domain-product-discount
 Requires-Dist: odoo14-addon-sale-coupon-domain-product-discount-in-field
+Requires-Dist: odoo14-addon-sale-coupon-limit
 Requires-Dist: odoo14-addon-sale-coupon-multi-gift
 Requires-Dist: odoo14-addon-sale-coupon-order-line-link
 Requires-Dist: odoo14-addon-sale-coupon-partner
 Requires-Dist: odoo14-addon-sale-coupon-product-exclude
 Requires-Dist: odoo14-addon-sale-coupon-reward-add-product
 Requires-Dist: odoo14-addon-sale-coupon-reward-fixed-price
 Requires-Dist: odoo14-addon-sale-promotion-discount-in-field
```


# Comparing `tmp/xaitk-saliency-demo-2.1.0.tar.gz` & `tmp/xaitk-saliency-demo-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xaitk-saliency-demo-2.1.0.tar", last modified: Wed Sep 14 18:17:36 2022, max compression
+gzip compressed data, was "xaitk-saliency-demo-2.2.0.tar", last modified: Wed Jul 12 15:21:24 2023, max compression
```

## Comparing `xaitk-saliency-demo-2.1.0.tar` & `xaitk-saliency-demo-2.2.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2022-09-14 18:17:36.166431 xaitk-saliency-demo-2.1.0/
--rw-rw-r--   0 seb       (1000) seb       (1000)     1504 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/LICENSE
--rw-rw-r--   0 seb       (1000) seb       (1000)       44 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/MANIFEST.in
--rw-rw-r--   0 seb       (1000) seb       (1000)     1992 2022-09-14 18:17:36.166431 xaitk-saliency-demo-2.1.0/PKG-INFO
--rw-rw-r--   0 seb       (1000) seb       (1000)     1171 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/README.rst
--rw-rw-r--   0 seb       (1000) seb       (1000)     1251 2022-09-14 18:17:36.166431 xaitk-saliency-demo-2.1.0/setup.cfg
--rw-rw-r--   0 seb       (1000) seb       (1000)       38 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/setup.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2022-09-14 18:17:36.166431 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/
--rw-rw-r--   0 seb       (1000) seb       (1000)       49 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/__init__.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2022-09-14 18:17:36.166431 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/
--rw-rw-r--   0 seb       (1000) seb       (1000)       50 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/__init__.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2022-09-14 18:17:36.166431 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/
--rw-rw-r--   0 seb       (1000) seb       (1000)      197 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/__init__.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2022-09-14 18:17:36.166431 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/assets/
--rw-rw-r--   0 seb       (1000) seb       (1000)      498 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/assets/__init__.py
--rw-rw-r--   0 seb       (1000) seb       (1000)    10472 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt
--rw-rw-r--   0 seb       (1000) seb       (1000)     1974 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/main.py
--rw-rw-r--   0 seb       (1000) seb       (1000)     9723 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/ml_models.py
--rw-rw-r--   0 seb       (1000) seb       (1000)     5535 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/ml_xai.py
--rw-rw-r--   0 seb       (1000) seb       (1000)     2375 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/options.py
--rw-rw-r--   0 seb       (1000) seb       (1000)     4774 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/trame_exec.py
--rw-rw-r--   0 seb       (1000) seb       (1000)     4031 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/trame_state.py
--rw-rw-r--   0 seb       (1000) seb       (1000)      969 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/jupyter.py
--rw-rw-r--   0 seb       (1000) seb       (1000)      689 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/main.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2022-09-14 18:17:36.166431 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/ui/
--rw-rw-r--   0 seb       (1000) seb       (1000)       62 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/ui/__init__.py
--rw-rw-r--   0 seb       (1000) seb       (1000)     4115 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/ui/main.py
--rw-rw-r--   0 seb       (1000) seb       (1000)     1092 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/ui/options.py
--rw-rw-r--   0 seb       (1000) seb       (1000)    15420 2022-09-14 18:12:38.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/ui/ui_helper.py
-drwxrwxr-x   0 seb       (1000) seb       (1000)        0 2022-09-14 18:17:36.166431 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo.egg-info/
--rw-rw-r--   0 seb       (1000) seb       (1000)     1992 2022-09-14 18:17:36.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo.egg-info/PKG-INFO
--rw-rw-r--   0 seb       (1000) seb       (1000)     1005 2022-09-14 18:17:36.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo.egg-info/SOURCES.txt
--rw-rw-r--   0 seb       (1000) seb       (1000)        1 2022-09-14 18:17:36.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo.egg-info/dependency_links.txt
--rw-rw-r--   0 seb       (1000) seb       (1000)       66 2022-09-14 18:17:36.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo.egg-info/entry_points.txt
--rw-rw-r--   0 seb       (1000) seb       (1000)      309 2022-09-14 18:17:36.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo.egg-info/requires.txt
--rw-rw-r--   0 seb       (1000) seb       (1000)       20 2022-09-14 18:17:36.000000 xaitk-saliency-demo-2.1.0/xaitk_saliency_demo.egg-info/top_level.txt
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1504 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/LICENSE
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       44 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/MANIFEST.in
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1953 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/PKG-INFO
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1171 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/README.rst
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1282 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/setup.cfg
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       38 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/setup.py
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       49 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/__init__.py
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       50 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/__init__.py
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      197 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/__init__.py
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/assets/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      498 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/assets/__init__.py
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/assets/__pycache__/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      707 2023-07-06 21:36:39.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/assets/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)    10472 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1974 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/main.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     9702 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/ml_models.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     5561 2023-07-07 00:51:07.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/ml_xai.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     2443 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/options.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     5323 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/trame_exec.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     4031 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/trame_state.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1085 2023-07-07 00:51:07.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/jupyter.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      689 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/main.py
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       62 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/__init__.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     4178 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/main.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1092 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/options.py
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)    16390 2023-07-07 00:51:02.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/ui_helper.py
+drwxrwxr-x   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        0 2023-07-12 15:21:24.076617 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1953 2023-07-12 15:21:24.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)     1079 2023-07-12 15:21:24.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)        1 2023-07-12 15:21:24.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       65 2023-07-12 15:21:24.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/entry_points.txt
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)      330 2023-07-12 15:21:24.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/requires.txt
+-rw-rw-r--   0 sebastien.jourdain  (1000) sebastien.jourdain  (1000)       20 2023-07-12 15:21:24.000000 xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/top_level.txt
```

### Comparing `xaitk-saliency-demo-2.1.0/LICENSE` & `xaitk-saliency-demo-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.1.0/PKG-INFO` & `xaitk-saliency-demo-2.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xaitk-saliency-demo
-Version: 2.1.0
+Version: 2.2.0
 Summary: Web application demonstrating XAITK Saliency functionality
-Home-page: UNKNOWN
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: JavaScript
@@ -70,9 +68,7 @@
   :width: 20%
 .. |image_2| image:: gallery/xaitk-classification-sliding-window.jpg
   :width: 20%
 .. |image_3| image:: gallery/xaitk-detection-retina.jpg
   :width: 20%
 .. |image_4| image:: gallery/xaitk-similarity-1.jpg
   :width: 20%
-
-
```

### Comparing `xaitk-saliency-demo-2.1.0/README.rst` & `xaitk-saliency-demo-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.1.0/setup.cfg` & `xaitk-saliency-demo-2.2.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xaitk-saliency-demo
-version = 2.1.0
+version = 2.2.0
 description = Web application demonstrating XAITK Saliency functionality
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = BSD License
 classifiers = 
 	Development Status :: 5 - Production/Stable
@@ -25,26 +25,32 @@
 
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
 	trame>=2.1.0
 	trame-components>=2.0.4
-	altair==4.1.0
+	plotly==5.15.0
+	pandas
+	
 	smqtk-classifier==0.19.0
-	smqtk-core==0.18.1
-	smqtk-dataprovider==0.16.0
-	smqtk-descriptors==0.18.1
-	smqtk-detection[torch,centernet]==0.19.0
-	smqtk-image-io==0.16.2
-	xaitk-saliency==0.6.1
-	torchvision==0.11.2
-	scikit-learn==0.24.2
-	scikit-image==0.18.3
-	ubelt==1.1.1
+	smqtk-core==0.19.0
+	smqtk-dataprovider==0.18.0
+	smqtk-descriptors==0.19.0
+	smqtk-detection[torch,centernet]==0.20.0
+	smqtk-image-io==0.17.1
+	
+	xaitk-saliency==0.7.0
+	ubelt==1.3.2
+	
+	torch==1.10.2
+	torchvision==0.11.3
+	
+	scikit-learn==1.3.0
+	scikit-image==0.21.0
 
 [options.entry_points]
 console_scripts = 
 	xaitk-saliency-demo = xaitk_saliency_demo:main
 
 [egg_info]
 tag_build =
```

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/main.py` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/main.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/ml_models.py` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/ml_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 # -----------------------------------------------------------------------------
 
 CENTERNET_RESNET50 = grabdata(
     "https://data.kitware.com/api/v1/item/623259f64acac99f426f21db/download",
     fname="centernet-resnet50.pth",
     appname="xaitk-saliency-demo",
     hash_prefix="a0083ec55d46c420d06c414e5ecc1863d6ad9b6a1732acff5c9dba28158a4"
-                "c5a04f43541415d503fa776031a7329e3912864ae2348b3bee035df0d1e7a"
-                "cefa49"
+    "c5a04f43541415d503fa776031a7329e3912864ae2348b3bee035df0d1e7a"
+    "cefa49",
 )
 
 # -----------------------------------------------------------------------------
 # Class normalizing model usage
 # -----------------------------------------------------------------------------
 
 
@@ -103,14 +103,15 @@
         return self._model
 
 
 # -----------------------------------------------------------------------------
 # Classification
 # -----------------------------------------------------------------------------
 
+
 class ResNetPredict:
     @torch.no_grad()
     def predict(self, input) -> np.ndarray:
         """
         Run prediction with the set model and return the final output layer
         as a vector for one image.
         """
@@ -198,14 +199,15 @@
         )
 
 
 # -----------------------------------------------------------------------------
 # Detection
 # -----------------------------------------------------------------------------
 
+
 class DetectionPredict:
     def predict(self, input: np.ndarray) -> Tuple[np.ndarray, np.ndarray, List[str]]:
         """
         Predict detections for a single image, returning bounding-boxes, scores
         and labels as arrays (in that order).
         Bounding boxes are in (minX, minY, maxX, maxY) format.
         Boxes array is of shape (nDets x 4).
@@ -253,28 +255,28 @@
         }
 
 
 class DetectionFRCNN(AbstractModel, DetectionPredict, DetectionRun):
     def __init__(self, server):
         d = DEVICE
         model = ResNetFRCNN(
-            use_cuda=True if 'cuda' in d.type.lower() else False,
+            use_cuda=True if "cuda" in d.type.lower() else False,
             cuda_device=d.type + (f":{d.index}" if d.index is not None else ""),
         )
         super().__init__(server, model)
 
 
 class DetectionCenterNetVisdrone(AbstractModel, DetectionPredict, DetectionRun):
     def __init__(self, server):
         d = DEVICE
         model = CenterNetVisdrone(
             arch="resnet50",
             model_file=CENTERNET_RESNET50,
             max_dets=500,
-            use_cuda=True if 'cuda' in d.type.lower() else False,
+            use_cuda=True if "cuda" in d.type.lower() else False,
         )
         super().__init__(server, model)
 
 
 # -----------------------------------------------------------------------------
 # Factory instance maps
 # -----------------------------------------------------------------------------
```

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/ml_xai.py` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/ml_xai.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     SlidingWindowStack,
 )
 from xaitk_saliency.impls.gen_object_detector_blackbox_sal.drise import DRISEStack
 from xaitk_saliency.impls.gen_object_detector_blackbox_sal.drise import RandomGridStack
 
 # smqtk-*
 from smqtk_classifier import ClassifyImage
-from smqtk_descriptors.interfaces.image_descriptor_generator import ImageDescriptorGenerator
+from smqtk_descriptors.interfaces.image_descriptor_generator import (
+    ImageDescriptorGenerator,
+)
 from smqtk_detection import DetectImageObjects
 
 # labels
 from .assets import imagenet_categories, imagenet_model_loader
 
 import logging
 
@@ -45,33 +47,23 @@
         },
     },
     "SlidingWindowStack": {
         "_saliency": {
             "class": SlidingWindowStack,
         },
     },
-
     # Similarity
     "SBSMStack": {
         "_saliency": {
             "class": SBSMStack,
         }
     },
-
     # Object Detection
-    "DRISEStack": {
-        "_saliency": {
-            "class": DRISEStack
-        }
-    },
-    "RandomGridStack": {
-        "_saliency": {
-            "class": RandomGridStack
-        }
-    },
+    "DRISEStack": {"_saliency": {"class": DRISEStack}},
+    "RandomGridStack": {"_saliency": {"class": RandomGridStack}},
 }
 
 
 # SMQTK black-box classifier
 class ClfModel(ClassifyImage):
     def __init__(self, model, idx):
         self.model = model
@@ -91,20 +83,21 @@
     def get_config(self):
         # Required by a parent class. Will not be used in this context.
         return {}
 
 
 # SMQTK black-box descriptor generator
 class DescrModel(ImageDescriptorGenerator):
-
     def __init__(self, model):
         self.model = model
 
     @torch.no_grad()
-    def generate_arrays_from_images(self, img_mat_iter: Iterable[np.ndarray]) -> Iterable[np.ndarray]:
+    def generate_arrays_from_images(
+        self, img_mat_iter: Iterable[np.ndarray]
+    ) -> Iterable[np.ndarray]:
         for img in img_mat_iter:
             inp = imagenet_model_loader(img).unsqueeze(0).to(self.model.device)
             vec = self.model(inp).cpu().numpy().squeeze()
             yield vec
 
     def get_config(self) -> Dict[str, Any]:
         # Required by a parent class. Will not be used in this context.
@@ -119,15 +112,17 @@
             kv_pairs = SALIENCY_TYPES[name].items()
         except IndexError:
             logger.info(f"Could not find {name} in {list(SALIENCY_TYPES.keys())}")
             return
         for key, value in kv_pairs:
             constructor = value.get("class")
             param_keys = value.get("params", params.keys())
-            setattr(self, key, constructor(**{k: params[k] for k in param_keys}))
+            kwargs = {k: params[k] for k in param_keys}
+            logger.info(f"XAI ran with {kwargs}")
+            setattr(self, key, constructor(**kwargs))
 
 
 class ClassificationSaliency(Saliency):
     def run(self, input, *_):
         topk = self._model.topk
         self._saliency.fill = FILL
         sal = self._saliency(input, ClfModel(self._model, topk))
```

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/options.py` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         "input_expected": 2,
     },
     "detection": {
         # Task => saliency
         "saliency_active": "DRISEStack",
         "saliency_available": [
             {"text": "DRISE", "value": "DRISEStack"},
-            {"text": "RandomGridStack", "value": "RandomGridStack"}
+            {"text": "RandomGridStack", "value": "RandomGridStack"},
         ],
         # Task => model
         "model_active": "DetectionFRCNN",
         "model_available": [
             {"text": "FRCNN (COCO)", "value": "DetectionFRCNN"},
             {"text": "CenterNet (VisDrone)", "value": "DetectionCenterNetVisdrone"},
         ],
@@ -51,24 +51,27 @@
 }
 
 SALIENCY_PARAMS = {
     # similarity
     "SBSMStack": ["window_size", "stride", "proximity_metric", "threads"],
     # detection
     "DRISEStack": ["n", "s", "p1", "seed", "threads"],
-    "RandomGridStack": ["n", "s", "p1", "seed", "threads"],
+    "RandomGridStack": ["n", "s_tuple", "p1", "seed", "threads"],
     # classification
     "RISEStack": ["n", "s", "p1", "seed", "threads", "debiased"],
     "SlidingWindowStack": ["window_size", "stride", "threads"],
 }
 
 ALL_SALIENCY_PARAMS = {
     "window_size": int,
     "stride": int,
     "n": int,
     "s": int,
+    "s_tuple": int,
     "p1": float,
     "seed": int,
     "threads": int,
     "proximity_metric": str,
     "debiased": bool,
 }
+
+SALINECY_PARAM_REMAP = {"s": "s_tuple"}
```

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/trame_exec.py` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/trame_exec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pandas as pd
-import altair as alt
+import plotly.express as px
 
 from . import options
 from trame_client.encoders import numpy
 
 
 import logging
 
@@ -32,14 +32,25 @@
                 value = state[f"xai_param__{name}"]
                 convert = options.ALL_SALIENCY_PARAMS[name]
                 if isinstance(value, list):
                     params[name] = [convert(v) for v in value]
                 else:
                     params[name] = convert(value)
 
+            # Handle rename to support different structure for conflicting names
+            for new_name, from_value in options.SALINECY_PARAM_REMAP.items():
+                if from_value in params:
+                    if isinstance(from_value, (list, tuple)):
+                        result = []
+                        for name in from_value:
+                            result.append(params.pop(name))
+                        params[new_name] = result
+                    else:
+                        params[new_name] = params.pop(from_value)
+
             ctrl.xai_set_saliency_method(state.saliency_active, params)
 
     def update_model_execution():
         """Executed when:
         -> btn press in model section
         -> state.change(TOP_K, input_file, model_active)
         """
@@ -47,25 +58,26 @@
 
         if ctrl.xai_can_run():
             results = ctrl.xai_run_model()
 
         # classes
         classes = results.get("classes", [])
         df = pd.DataFrame(classes, columns=["Class", "Score"])
-        chart = (
-            alt.Chart(df)
-            .mark_bar()
-            .encode(
-                x=alt.X("Score", axis=alt.Axis(format="%", title=None)),
-                y=alt.Y("Class", axis=alt.Axis(title=None), sort="-x"),
-            )
-            .properties(width="container", height=145)
-        )
+        df.sort_values("Score", ascending=True, inplace=True)
 
+        chart = px.bar(df, x="Score", y="Class")
+        chart.update_layout(
+            xaxis_title="",
+            yaxis_title="",
+            showlegend=False,
+            margin=dict(b=0, l=0, r=0, t=0),
+            height=192,
+        )
         ctrl.classification_chart_update(chart)
+
         state.xai_viz_classification_selected = "heatmap_0"
         state.xai_viz_classification_selected_available = list(
             map(
                 lambda t: {
                     "text": t[1][0],
                     "score": int(100 * t[1][1]),
                     "value": f"heatmap_{t[0]}",
```

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/engine/trame_state.py` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/engine/trame_state.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/jupyter.py` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/jupyter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from trame.app import get_server, jupyter
 from . import engine, ui
+from .engine.ml_models import update_ml_device
 
 
 def show(server=None, **kwargs):
     """Run and display the trame application in jupyter's event loop
     The kwargs are forwarded to IPython.display.IFrame()
     """
     new_server = False
@@ -24,12 +25,15 @@
     import logging
 
     engine_logger = logging.getLogger("xaitks_saliency_demo")
     engine_logger.setLevel(logging.ERROR)
 
     # Initilize app
     if new_server:
+        # Try to use GPU by default
+        update_ml_device(False)
+
         engine.initialize(server)
         ui.initialize(server)
 
     # Show as cell result
     jupyter.show(server, **kwargs)
```

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/main.py` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/main.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/ui/main.py` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,23 +34,23 @@
             "input_file": None,
             "input_1_name": "Reference",
             "input_2_name": "Query",
             #
             "xai_params_to_show": [],
             "xai_param__window_size": [50, 50],
             "xai_param__stride": [20, 20],
+            "xai_param__s_tuple": [8, 8],
             #
             "xai_viz_type": "",
             #
             "full_range": [-1, 1],
         }
     )
     server.state.client_only("xai_viz_heatmap_opacity")
 
-
     # -----------------------------------------------------------------------------
     # Computed variable for heatmap
     # -----------------------------------------------------------------------------
 
     @state.change("xai_viz_color_min", "xai_viz_color_max")
     def xai_viz_color_range_change(xai_viz_color_min, xai_viz_color_max, **kwargs):
         try:
@@ -91,15 +91,15 @@
                 v_show="saliency_available.length > 1",
                 v_model=("saliency_active", ""),
                 items=("saliency_available", []),
                 **ui_helper.compact_styles,
                 **ui_helper.combo_styles,
             )
             vuetify.VSelect(
-                v_show=("task_active == 'classification'",),
+                v_show=("['classification', 'detection'].includes(task_active)",),
                 label="Top classes",
                 v_model=("TOP_K", 5),
                 items=("TOP_K_available", list(range(5, 11))),
                 **ui_helper.compact_styles,
                 style="max-width: 70px",
             )
             vuetify.VProgressLinear(
```

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/ui/options.py` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/options.py`

 * *Files identical despite different names*

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo/app/ui/ui_helper.py` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo/app/ui/ui_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from trame.widgets import html, vuetify, vega, trame
+from trame.widgets import html, vuetify, plotly, trame
 
 from . import options
 
 import multiprocessing
 
 NB_THREADS = int(multiprocessing.cpu_count() / 2 + 0.5)
 
@@ -147,17 +147,18 @@
             classes="mr-2",
             click=ctrl.run_model,
         )
         _header.add_child("Model execution")
 
     with _content:
         # classes UI
-        _chart = vega.Figure(
-            style="width: calc(100% - 32px)",
+        _chart = plotly.Figure(
+            style="width: 100%; height: 100%;",
             v_show=("task_active === 'classification'",),
+            display_mode_bar=False,
         )
         ctrl.classification_chart_update = _chart.update
 
         # similarity UI
         vuetify.VProgressCircular(
             "{{ Math.round(model_viz_similarity) }} %",
             v_show=("task_active === 'similarity'",),
@@ -177,16 +178,16 @@
                 area_opacity=0.25,
                 area_selected_opacity=1,
                 area_key="id",
                 max_height=216,
                 area_style=("{ 'stroke-width': 3, rx: 10 }",),
             )
             with vuetify.VRow(
-                classes="flex-shrink-1 justify-start align-start no-gutters",
-                style="width: 25px;",
+                classes="d-flex flex-shrink-1 align-content-start flex-wrap no-gutters",
+                style="width: 25px; height: 100%;",
             ):
                 with vuetify.VSheet(
                     v_for=("item, idx in model_viz_detection_areas",),
                     key="idx",
                     classes="ma-2",
                     style="cursor: pointer",
                     elevation=4,
@@ -256,14 +257,33 @@
         )
         vuetify.VTextField(
             label="Spatial resolution of the small masking grid",
             v_show=("xai_params_to_show.includes('s')",),
             v_model=("xai_param__s", 8),
             type="number",
         )
+        with vuetify.VCol(v_show=("xai_params_to_show.includes('s_tuple')",)):
+            vuetify.VRow(
+                "Spatial resolution of the small masking grid (x, y)",
+                classes="text-caption text--secondary",
+                style="line-height: 20px; height: 20px; letter-spacing: normal !important;",
+            )
+            with vuetify.VRow(classes="mt-0 pt-0"):
+                vuetify.VTextField(
+                    v_model_number=("xai_param__s_tuple[0]",),
+                    change="flushState('xai_param__s_tuple')",
+                    type="number",
+                    classes="mr-1 pt-1",
+                )
+                vuetify.VTextField(
+                    v_model_number=("xai_param__s_tuple[1]",),
+                    change="flushState('xai_param__s_tuple')",
+                    type="number",
+                    classes="ml-1 pt-1",
+                )
         vuetify.VSlider(
             label="P1",
             persistent_hint=True,
             hint="Probability of the grid cell being set to 1 (otherwise 0). This should be a float value in the [0, 1] range.",
             v_show=("xai_params_to_show.includes('p1')",),
             v_model=("xai_param__p1", 0.5),
             min="0",
```

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo.egg-info/PKG-INFO` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: xaitk-saliency-demo
-Version: 2.1.0
+Version: 2.2.0
 Summary: Web application demonstrating XAITK Saliency functionality
-Home-page: UNKNOWN
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: JavaScript
@@ -70,9 +68,7 @@
   :width: 20%
 .. |image_2| image:: gallery/xaitk-classification-sliding-window.jpg
   :width: 20%
 .. |image_3| image:: gallery/xaitk-detection-retina.jpg
   :width: 20%
 .. |image_4| image:: gallery/xaitk-similarity-1.jpg
   :width: 20%
-
-
```

### Comparing `xaitk-saliency-demo-2.1.0/xaitk_saliency_demo.egg-info/SOURCES.txt` & `xaitk-saliency-demo-2.2.0/xaitk_saliency_demo.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,11 +18,12 @@
 xaitk_saliency_demo/app/engine/ml_models.py
 xaitk_saliency_demo/app/engine/ml_xai.py
 xaitk_saliency_demo/app/engine/options.py
 xaitk_saliency_demo/app/engine/trame_exec.py
 xaitk_saliency_demo/app/engine/trame_state.py
 xaitk_saliency_demo/app/engine/assets/__init__.py
 xaitk_saliency_demo/app/engine/assets/imagenet_classes.txt
+xaitk_saliency_demo/app/engine/assets/__pycache__/__init__.cpython-39.pyc
 xaitk_saliency_demo/app/ui/__init__.py
 xaitk_saliency_demo/app/ui/main.py
 xaitk_saliency_demo/app/ui/options.py
 xaitk_saliency_demo/app/ui/ui_helper.py
```


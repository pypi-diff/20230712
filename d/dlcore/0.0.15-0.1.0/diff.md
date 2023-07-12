# Comparing `tmp/dlcore-0.0.15.tar.gz` & `tmp/dlcore-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlcore-0.0.15.tar", last modified: Wed Jul 12 11:33:00 2023, max compression
+gzip compressed data, was "dlcore-0.1.0.tar", last modified: Tue Jul 11 14:00:07 2023, max compression
```

## Comparing `dlcore-0.0.15.tar` & `dlcore-0.1.0.tar`

### file list

```diff
@@ -1,47 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:33:00.467980 dlcore-0.0.15/
--rw-r--r--   0 root         (0) root         (0)      390 2023-07-12 11:33:00.464647 dlcore-0.0.15/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:33:00.454647 dlcore-0.0.15/dlcore/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 13:17:42.000000 dlcore-0.0.15/dlcore/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:33:00.457981 dlcore-0.0.15/dlcore/config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 12:41:07.000000 dlcore-0.0.15/dlcore/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-07-03 12:46:04.000000 dlcore-0.0.15/dlcore/config/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:33:00.457981 dlcore-0.0.15/dlcore/datasets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 12:41:07.000000 dlcore-0.0.15/dlcore/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-07-05 11:30:40.000000 dlcore-0.0.15/dlcore/datasets/image_data_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-05 14:09:41.000000 dlcore-0.0.15/dlcore/datasets/image_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:33:00.461314 dlcore-0.0.15/dlcore/evaluation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 12:41:07.000000 dlcore-0.0.15/dlcore/evaluation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3316 2023-07-11 10:54:03.000000 dlcore-0.0.15/dlcore/evaluation/score_evaluation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:33:00.461314 dlcore-0.0.15/dlcore/evaluation/score_fn/
--rw-r--r--   0 root         (0) root         (0)      195 2023-07-11 10:25:15.000000 dlcore-0.0.15/dlcore/evaluation/score_fn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      299 2023-07-11 10:13:21.000000 dlcore-0.0.15/dlcore/evaluation/score_fn/accuracy_score.py
--rw-r--r--   0 root         (0) root         (0)      469 2023-07-11 10:12:06.000000 dlcore-0.0.15/dlcore/evaluation/score_fn/auc_score.py
--rw-r--r--   0 root         (0) root         (0)      237 2023-07-11 10:27:47.000000 dlcore-0.0.15/dlcore/evaluation/score_fn/f1_score.py
--rw-r--r--   0 root         (0) root         (0)      272 2023-07-11 10:26:40.000000 dlcore-0.0.15/dlcore/evaluation/score_fn/precision_score.py
--rw-r--r--   0 root         (0) root         (0)      259 2023-07-11 10:27:28.000000 dlcore-0.0.15/dlcore/evaluation/score_fn/recall_score.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-07-11 10:00:44.000000 dlcore-0.0.15/dlcore/evaluation/score_fn.py
--rw-r--r--   0 root         (0) root         (0)      205 2023-07-11 10:18:09.000000 dlcore-0.0.15/dlcore/evaluation/score_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:33:00.461314 dlcore-0.0.15/dlcore/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 13:50:14.000000 dlcore-0.0.15/dlcore/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:33:00.464647 dlcore-0.0.15/dlcore/models/cnn_image_classification/
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-16 15:44:45.000000 dlcore-0.0.15/dlcore/models/cnn_image_classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:33:00.464647 dlcore-0.0.15/dlcore/models/cnn_image_classification/cnn_backbone/
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-16 15:38:09.000000 dlcore-0.0.15/dlcore/models/cnn_image_classification/cnn_backbone/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2991 2023-07-11 10:16:39.000000 dlcore-0.0.15/dlcore/models/cnn_image_classification/cnn_backbone/cnn_backbone.py
--rw-r--r--   0 root         (0) root         (0)     1331 2023-07-10 13:38:10.000000 dlcore-0.0.15/dlcore/models/cnn_image_classification/cnn_backbone/cnn_layers.py
--rw-r--r--   0 root         (0) root         (0)     2304 2023-07-10 16:35:11.000000 dlcore-0.0.15/dlcore/models/cnn_image_classification/custom_cnn_image_classification.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-10 16:22:37.000000 dlcore-0.0.15/dlcore/models/cnn_image_classification/custom_cnn_image_classification_multylabel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:33:00.464647 dlcore-0.0.15/dlcore/models/neural_network/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 11:29:58.000000 dlcore-0.0.15/dlcore/models/neural_network/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-06-16 13:38:48.000000 dlcore-0.0.15/dlcore/models/neural_network/custom_nn.py
--rw-r--r--   0 root         (0) root         (0)     4449 2023-07-11 14:07:10.000000 dlcore-0.0.15/dlcore/models/nn_trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:33:00.457981 dlcore-0.0.15/dlcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      390 2023-07-12 11:33:00.000000 dlcore-0.0.15/dlcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1276 2023-07-12 11:33:00.000000 dlcore-0.0.15/dlcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 11:33:00.000000 dlcore-0.0.15/dlcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-12 11:33:00.000000 dlcore-0.0.15/dlcore.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 11:33:00.464647 dlcore-0.0.15/services/
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-20 15:22:02.000000 dlcore-0.0.15/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1388 2023-07-05 10:43:18.000000 dlcore-0.0.15/services/dynamogram_service.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 11:33:00.467980 dlcore-0.0.15/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      706 2023-07-12 11:32:55.000000 dlcore-0.0.15/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:00:07.774107 dlcore-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)      389 2023-07-11 14:00:07.774107 dlcore-0.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:00:07.767440 dlcore-0.1.0/dlcore/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 13:17:42.000000 dlcore-0.1.0/dlcore/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:00:07.770774 dlcore-0.1.0/dlcore/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 12:41:07.000000 dlcore-0.1.0/dlcore/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-07-03 12:46:04.000000 dlcore-0.1.0/dlcore/config/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:00:07.770774 dlcore-0.1.0/dlcore/datasets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 12:41:07.000000 dlcore-0.1.0/dlcore/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-07-05 11:30:40.000000 dlcore-0.1.0/dlcore/datasets/image_data_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-05 14:09:41.000000 dlcore-0.1.0/dlcore/datasets/image_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:00:07.770774 dlcore-0.1.0/dlcore/evaluation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 12:41:07.000000 dlcore-0.1.0/dlcore/evaluation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2023-07-11 10:54:03.000000 dlcore-0.1.0/dlcore/evaluation/score_evaluation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:00:07.770774 dlcore-0.1.0/dlcore/evaluation/score_fn/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-07-11 10:25:15.000000 dlcore-0.1.0/dlcore/evaluation/score_fn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      299 2023-07-11 10:13:21.000000 dlcore-0.1.0/dlcore/evaluation/score_fn/accuracy_score.py
+-rw-r--r--   0 root         (0) root         (0)      469 2023-07-11 10:12:06.000000 dlcore-0.1.0/dlcore/evaluation/score_fn/auc_score.py
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-11 10:27:47.000000 dlcore-0.1.0/dlcore/evaluation/score_fn/f1_score.py
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-11 10:26:40.000000 dlcore-0.1.0/dlcore/evaluation/score_fn/precision_score.py
+-rw-r--r--   0 root         (0) root         (0)      259 2023-07-11 10:27:28.000000 dlcore-0.1.0/dlcore/evaluation/score_fn/recall_score.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-07-11 10:00:44.000000 dlcore-0.1.0/dlcore/evaluation/score_fn.py
+-rw-r--r--   0 root         (0) root         (0)      205 2023-07-11 10:18:09.000000 dlcore-0.1.0/dlcore/evaluation/score_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:00:07.770774 dlcore-0.1.0/dlcore/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 13:50:14.000000 dlcore-0.1.0/dlcore/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:00:07.774107 dlcore-0.1.0/dlcore/models/cnn_image_classification/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-16 15:44:45.000000 dlcore-0.1.0/dlcore/models/cnn_image_classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:00:07.774107 dlcore-0.1.0/dlcore/models/cnn_image_classification/cnn_backbone/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-16 15:38:09.000000 dlcore-0.1.0/dlcore/models/cnn_image_classification/cnn_backbone/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-07-11 10:16:39.000000 dlcore-0.1.0/dlcore/models/cnn_image_classification/cnn_backbone/cnn_backbone.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-07-10 13:38:10.000000 dlcore-0.1.0/dlcore/models/cnn_image_classification/cnn_backbone/cnn_layers.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2023-07-10 16:35:11.000000 dlcore-0.1.0/dlcore/models/cnn_image_classification/custom_cnn_image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-10 16:22:37.000000 dlcore-0.1.0/dlcore/models/cnn_image_classification/custom_cnn_image_classification_multylabel.py
+-rw-r--r--   0 root         (0) root         (0)     4449 2023-07-10 10:25:01.000000 dlcore-0.1.0/dlcore/models/nn_trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:00:07.767440 dlcore-0.1.0/dlcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      389 2023-07-11 14:00:07.000000 dlcore-0.1.0/dlcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-07-11 14:00:07.000000 dlcore-0.1.0/dlcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 14:00:07.000000 dlcore-0.1.0/dlcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-11 14:00:07.000000 dlcore-0.1.0/dlcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 14:00:07.774107 dlcore-0.1.0/services/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-20 15:22:02.000000 dlcore-0.1.0/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-07-05 10:43:18.000000 dlcore-0.1.0/services/dynamogram_service.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 14:00:07.774107 dlcore-0.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      705 2023-07-11 13:59:42.000000 dlcore-0.1.0/setup.py
```

### Comparing `dlcore-0.0.15/dlcore/config/config.py` & `dlcore-0.1.0/dlcore/config/config.py`

 * *Files identical despite different names*

### Comparing `dlcore-0.0.15/dlcore/datasets/image_data_wrapper.py` & `dlcore-0.1.0/dlcore/datasets/image_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `dlcore-0.0.15/dlcore/datasets/image_dataset.py` & `dlcore-0.1.0/dlcore/datasets/image_dataset.py`

 * *Files identical despite different names*

### Comparing `dlcore-0.0.15/dlcore/evaluation/score_evaluation.py` & `dlcore-0.1.0/dlcore/evaluation/score_evaluation.py`

 * *Files identical despite different names*

### Comparing `dlcore-0.0.15/dlcore/evaluation/score_fn.py` & `dlcore-0.1.0/dlcore/evaluation/score_fn.py`

 * *Files identical despite different names*

### Comparing `dlcore-0.0.15/dlcore/models/cnn_image_classification/cnn_backbone/cnn_backbone.py` & `dlcore-0.1.0/dlcore/models/cnn_image_classification/cnn_backbone/cnn_backbone.py`

 * *Files identical despite different names*

### Comparing `dlcore-0.0.15/dlcore/models/cnn_image_classification/cnn_backbone/cnn_layers.py` & `dlcore-0.1.0/dlcore/models/cnn_image_classification/cnn_backbone/cnn_layers.py`

 * *Files identical despite different names*

### Comparing `dlcore-0.0.15/dlcore/models/cnn_image_classification/custom_cnn_image_classification.py` & `dlcore-0.1.0/dlcore/models/cnn_image_classification/custom_cnn_image_classification.py`

 * *Files identical despite different names*

### Comparing `dlcore-0.0.15/dlcore/models/cnn_image_classification/custom_cnn_image_classification_multylabel.py` & `dlcore-0.1.0/dlcore/models/cnn_image_classification/custom_cnn_image_classification_multylabel.py`

 * *Files identical despite different names*

### Comparing `dlcore-0.0.15/dlcore/models/nn_trainer.py` & `dlcore-0.1.0/dlcore/models/nn_trainer.py`

 * *Files identical despite different names*

### Comparing `dlcore-0.0.15/dlcore.egg-info/SOURCES.txt` & `dlcore-0.1.0/dlcore.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,11 +23,9 @@
 dlcore/models/nn_trainer.py
 dlcore/models/cnn_image_classification/__init__.py
 dlcore/models/cnn_image_classification/custom_cnn_image_classification.py
 dlcore/models/cnn_image_classification/custom_cnn_image_classification_multylabel.py
 dlcore/models/cnn_image_classification/cnn_backbone/__init__.py
 dlcore/models/cnn_image_classification/cnn_backbone/cnn_backbone.py
 dlcore/models/cnn_image_classification/cnn_backbone/cnn_layers.py
-dlcore/models/neural_network/__init__.py
-dlcore/models/neural_network/custom_nn.py
 services/__init__.py
 services/dynamogram_service.py
```

### Comparing `dlcore-0.0.15/services/dynamogram_service.py` & `dlcore-0.1.0/services/dynamogram_service.py`

 * *Files identical despite different names*

### Comparing `dlcore-0.0.15/setup.py` & `dlcore-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("/app/deepsinai/dlcore/Readme.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="dlcore",
-    version="0.0.15",
+    version="0.1.0",
     description="Deep Learning core in pytroch",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Milos Bijanic",
     author_email="bijanicmilos996@gmail.com",
```


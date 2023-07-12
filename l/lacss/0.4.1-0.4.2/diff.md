# Comparing `tmp/lacss-0.4.1.tar.gz` & `tmp/lacss-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacss-0.4.1.tar", max compression
+gzip compressed data, was "lacss-0.4.2.tar", max compression
```

## Comparing `lacss-0.4.1.tar` & `lacss-0.4.2.tar`

### file list

```diff
@@ -1,97 +1,102 @@
--rw-r--r--   0        0        0     1062 2023-06-22 13:00:42.813886 lacss-0.4.1/LICENSE
--rw-r--r--   0        0        0     2428 2023-06-22 13:00:42.825176 lacss-0.4.1/README.md
--rw-r--r--   0        0        0       65 2023-06-22 13:00:42.925221 lacss-0.4.1/lacss/__init__.py
--rw-r--r--   0        0        0       48 2023-06-27 19:54:42.795534 lacss-0.4.1/lacss/data/__init__.py
--rw-r--r--   0        0        0      190 2023-06-27 19:47:56.226635 lacss-0.4.1/lacss/data/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7981 2023-06-26 19:53:37.181410 lacss-0.4.1/lacss/data/__pycache__/augment.cpython-38.pyc
--rw-r--r--   0        0        0     5839 2023-06-26 19:53:37.207035 lacss-0.4.1/lacss/data/__pycache__/generator.cpython-38.pyc
--rw-r--r--   0        0        0     5681 2023-06-27 16:23:45.927971 lacss-0.4.1/lacss/data/__pycache__/parser.cpython-38.pyc
--rw-r--r--   0        0        0    11408 2023-06-26 19:35:53.107988 lacss-0.4.1/lacss/data/augment.py
--rw-r--r--   0        0        0     7747 2023-06-26 19:35:53.116426 lacss-0.4.1/lacss/data/generator.py
--rw-r--r--   0        0        0     8975 2023-06-27 19:54:42.804698 lacss-0.4.1/lacss/deploy.py
--rw-r--r--   0        0        0       74 2023-06-22 13:00:42.985435 lacss-0.4.1/lacss/losses/__init__.py
--rw-r--r--   0        0        0      214 2023-06-22 13:02:41.734572 lacss-0.4.1/lacss/losses/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5053 2023-06-26 19:53:37.570269 lacss-0.4.1/lacss/losses/__pycache__/auxiliary.cpython-38.pyc
--rw-r--r--   0        0        0     3294 2023-06-26 19:53:37.842923 lacss-0.4.1/lacss/losses/__pycache__/detection.cpython-38.pyc
--rw-r--r--   0        0        0     4905 2023-06-27 19:48:13.187810 lacss-0.4.1/lacss/losses/__pycache__/instance.cpython-38.pyc
--rw-r--r--   0        0        0     5248 2023-06-26 19:35:53.135636 lacss-0.4.1/lacss/losses/auxiliary.py
--rw-r--r--   0        0        0     2423 2023-06-26 19:35:53.144009 lacss-0.4.1/lacss/losses/detection.py
--rw-r--r--   0        0        0     5601 2023-06-27 19:54:42.814188 lacss-0.4.1/lacss/losses/instance.py
--rw-r--r--   0        0        0       56 2023-06-22 13:00:43.028217 lacss-0.4.1/lacss/metrics/__init__.py
--rw-r--r--   0        0        0      219 2023-06-22 13:02:43.184589 lacss-0.4.1/lacss/metrics/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5311 2023-06-26 19:53:38.336584 lacss-0.4.1/lacss/metrics/__pycache__/ranked.cpython-38.pyc
--rw-r--r--   0        0        0     5103 2023-06-26 19:35:53.161969 lacss-0.4.1/lacss/metrics/ranked.py
--rw-r--r--   0        0        0      216 2023-06-22 13:00:43.059681 lacss-0.4.1/lacss/modules/__init__.py
--rw-r--r--   0        0        0      435 2023-06-22 13:02:43.238041 lacss-0.4.1/lacss/modules/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2245 2023-06-26 19:53:38.371089 lacss-0.4.1/lacss/modules/__pycache__/auxiliary.cpython-38.pyc
--rw-r--r--   0        0        0     3049 2023-06-22 13:02:43.270904 lacss-0.4.1/lacss/modules/__pycache__/common.cpython-38.pyc
--rw-r--r--   0        0        0     6420 2023-06-22 13:02:43.307157 lacss-0.4.1/lacss/modules/__pycache__/convnext.cpython-38.pyc
--rw-r--r--   0        0        0     4814 2023-06-22 13:02:43.323531 lacss-0.4.1/lacss/modules/__pycache__/detector.cpython-38.pyc
--rw-r--r--   0        0        0     3443 2023-06-26 21:02:19.236756 lacss-0.4.1/lacss/modules/__pycache__/lacss.cpython-38.pyc
--rw-r--r--   0        0        0     2932 2023-06-22 13:02:43.350421 lacss-0.4.1/lacss/modules/__pycache__/lpn.cpython-38.pyc
--rw-r--r--   0        0        0     3578 2023-06-22 13:02:43.367407 lacss-0.4.1/lacss/modules/__pycache__/resnet.cpython-38.pyc
--rw-r--r--   0        0        0     4253 2023-06-27 17:33:27.254646 lacss-0.4.1/lacss/modules/__pycache__/segmentor.cpython-38.pyc
--rw-r--r--   0        0        0     2211 2023-06-22 13:02:43.288536 lacss-0.4.1/lacss/modules/__pycache__/unet.cpython-38.pyc
--rw-r--r--   0        0        0     2075 2023-06-26 19:35:53.170430 lacss-0.4.1/lacss/modules/auxiliary.py
--rw-r--r--   0        0        0     2261 2023-06-22 13:00:43.114039 lacss-0.4.1/lacss/modules/common.py
--rw-r--r--   0        0        0     6646 2023-06-22 13:00:43.126366 lacss-0.4.1/lacss/modules/convnext.py
--rw-r--r--   0        0        0     6580 2023-06-22 13:00:43.134266 lacss-0.4.1/lacss/modules/detector.py
--rw-r--r--   0        0        0     4120 2023-06-26 19:59:28.277578 lacss-0.4.1/lacss/modules/lacss.py
--rw-r--r--   0        0        0     3339 2023-06-22 13:00:43.156519 lacss-0.4.1/lacss/modules/lpn.py
--rw-r--r--   0        0        0     3771 2023-06-22 13:00:43.167303 lacss-0.4.1/lacss/modules/resnet.py
--rw-r--r--   0        0        0     5254 2023-06-27 17:32:18.960037 lacss-0.4.1/lacss/modules/segmentor.py
--rw-r--r--   0        0        0     1979 2023-06-22 13:00:43.193776 lacss-0.4.1/lacss/modules/unet.py
--rw-r--r--   0        0        0      174 2023-06-22 13:00:43.204051 lacss-0.4.1/lacss/ops/__init__.py
--rw-r--r--   0        0        0      270 2023-06-22 13:02:42.172883 lacss-0.4.1/lacss/ops/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2142 2023-06-26 19:53:37.599646 lacss-0.4.1/lacss/ops/__pycache__/boxes.cpython-38.pyc
--rw-r--r--   0        0        0     3480 2023-06-26 19:53:37.613942 lacss-0.4.1/lacss/ops/__pycache__/image.cpython-38.pyc
--rw-r--r--   0        0        0     2457 2023-06-26 19:53:37.639373 lacss-0.4.1/lacss/ops/__pycache__/locations.cpython-38.pyc
--rw-r--r--   0        0        0     5806 2023-06-22 13:02:42.251931 lacss-0.4.1/lacss/ops/__pycache__/masks.cpython-38.pyc
--rw-r--r--   0        0        0     3885 2023-06-26 19:53:37.704140 lacss-0.4.1/lacss/ops/__pycache__/nms.cpython-38.pyc
--rw-r--r--   0        0        0    10189 2023-06-26 19:53:37.661239 lacss-0.4.1/lacss/ops/__pycache__/patches.cpython-38.pyc
--rw-r--r--   0        0        0      672 2023-06-22 13:02:42.295307 lacss-0.4.1/lacss/ops/__pycache__/uda.cpython-38.pyc
--rw-r--r--   0        0        0     2321 2023-06-26 19:35:53.190870 lacss-0.4.1/lacss/ops/boxes.py
--rw-r--r--   0        0        0     3289 2023-06-26 19:35:53.198904 lacss-0.4.1/lacss/ops/image.py
--rw-r--r--   0        0        0     2843 2023-06-26 19:35:53.211864 lacss-0.4.1/lacss/ops/locations.py
--rw-r--r--   0        0        0     5967 2023-06-22 13:00:43.238207 lacss-0.4.1/lacss/ops/masks.py
--rw-r--r--   0        0        0     4732 2023-06-26 19:35:53.222000 lacss-0.4.1/lacss/ops/nms.py
--rw-r--r--   0        0        0    11768 2023-06-26 19:35:53.231134 lacss-0.4.1/lacss/ops/patches.py
--rw-r--r--   0        0        0      225 2023-06-22 13:00:43.270685 lacss-0.4.1/lacss/ops/uda.py
--rw-r--r--   0        0        0       63 2023-06-27 18:55:24.517866 lacss-0.4.1/lacss/tracking/__init__.py
--rw-r--r--   0        0        0     3340 2023-06-22 13:00:43.292844 lacss-0.4.1/lacss/tracking/predict.py
--rw-r--r--   0        0        0    12669 2023-06-27 19:54:42.820854 lacss-0.4.1/lacss/tracking/seqnms.py
--rw-r--r--   0        0        0     6741 2023-06-22 13:00:43.306733 lacss-0.4.1/lacss/tracking/smc.py
--rw-r--r--   0        0        0     5646 2023-06-22 13:00:43.323766 lacss-0.4.1/lacss/tracking/utils.py
--rw-r--r--   0        0        0       99 2023-06-22 13:00:43.333394 lacss-0.4.1/lacss/train/__init__.py
--rw-r--r--   0        0        0      257 2023-06-22 13:02:42.316230 lacss-0.4.1/lacss/train/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6686 2023-06-22 13:02:42.529439 lacss-0.4.1/lacss/train/__pycache__/loss.cpython-38.pyc
--rw-r--r--   0        0        0      648 2023-06-22 13:02:43.199772 lacss-0.4.1/lacss/train/__pycache__/metric.cpython-38.pyc
--rw-r--r--   0        0        0     4118 2023-06-27 19:48:09.272553 lacss-0.4.1/lacss/train/__pycache__/strategy.cpython-38.pyc
--rw-r--r--   0        0        0    12131 2023-06-27 19:48:09.311593 lacss-0.4.1/lacss/train/__pycache__/trainer.cpython-38.pyc
--rw-r--r--   0        0        0      718 2023-06-22 13:00:43.345992 lacss-0.4.1/lacss/train/data/__init__.py
--rw-r--r--   0        0        0      851 2023-06-22 13:02:42.337930 lacss-0.4.1/lacss/train/data/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4005 2023-06-22 13:02:42.353245 lacss-0.4.1/lacss/train/data/__pycache__/array_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     6093 2023-06-22 13:02:42.371233 lacss-0.4.1/lacss/train/data/__pycache__/data_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     5561 2023-06-22 13:02:42.399155 lacss-0.4.1/lacss/train/data/__pycache__/data_handler.cpython-38.pyc
--rw-r--r--   0        0        0    11577 2023-06-22 13:02:42.414539 lacss-0.4.1/lacss/train/data/__pycache__/dataset.cpython-38.pyc
--rw-r--r--   0        0        0     3319 2023-06-22 13:02:42.437553 lacss-0.4.1/lacss/train/data/__pycache__/generator_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     2515 2023-06-22 13:02:42.454501 lacss-0.4.1/lacss/train/data/__pycache__/list_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     3562 2023-06-22 13:02:42.482462 lacss-0.4.1/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     3167 2023-06-22 13:02:42.502701 lacss-0.4.1/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-38.pyc
--rw-r--r--   0        0        0     6796 2023-06-22 13:02:42.385721 lacss-0.4.1/lacss/train/data/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     4076 2023-06-22 13:00:43.353833 lacss-0.4.1/lacss/train/data/array_adapter.py
--rw-r--r--   0        0        0     5529 2023-06-22 13:00:43.360856 lacss-0.4.1/lacss/train/data/data_adapter.py
--rw-r--r--   0        0        0     6287 2023-06-22 13:00:43.369351 lacss-0.4.1/lacss/train/data/data_handler.py
--rw-r--r--   0        0        0    10656 2023-06-22 13:00:43.388157 lacss-0.4.1/lacss/train/data/dataset.py
--rw-r--r--   0        0        0     2599 2023-06-22 13:00:43.431971 lacss-0.4.1/lacss/train/data/generator_adapter.py
--rw-r--r--   0        0        0     2105 2023-06-22 13:00:43.446554 lacss-0.4.1/lacss/train/data/list_adapter.py
--rw-r--r--   0        0        0     3440 2023-06-22 13:00:43.456684 lacss-0.4.1/lacss/train/data/tf_dataset_adapter.py
--rw-r--r--   0        0        0     2566 2023-06-22 13:00:43.469261 lacss-0.4.1/lacss/train/data/torch_dataloader_adapter.py
--rw-r--r--   0        0        0     6394 2023-06-22 13:00:43.494227 lacss-0.4.1/lacss/train/data/utils.py
--rw-r--r--   0        0        0     6834 2023-06-22 13:00:43.502914 lacss-0.4.1/lacss/train/loss.py
--rw-r--r--   0        0        0      222 2023-06-22 13:00:43.517371 lacss-0.4.1/lacss/train/metric.py
--rw-r--r--   0        0        0     4018 2023-06-27 19:00:57.668124 lacss-0.4.1/lacss/train/strategy.py
--rw-r--r--   0        0        0    12919 2023-06-27 19:54:42.831348 lacss-0.4.1/lacss/train/trainer.py
--rw-r--r--   0        0        0     6392 2023-06-26 19:35:53.249659 lacss-0.4.1/lacss/utils.py
--rw-r--r--   0        0        0      810 2023-06-27 19:55:50.890419 lacss-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3115 1970-01-01 00:00:00.000000 lacss-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-28 18:47:53.571706 lacss-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2428 2023-06-28 18:47:53.578644 lacss-0.4.2/README.md
+-rw-r--r--   0        0        0       65 2023-06-28 18:47:53.899762 lacss-0.4.2/lacss/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-08 17:32:02.064648 lacss-0.4.2/lacss/data/__init__.py
+-rw-r--r--   0        0        0      190 2023-07-08 19:27:31.610725 lacss-0.4.2/lacss/data/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8032 2023-07-08 19:27:31.632495 lacss-0.4.2/lacss/data/__pycache__/augment.cpython-38.pyc
+-rw-r--r--   0        0        0     9231 2023-07-11 16:28:54.691314 lacss-0.4.2/lacss/data/__pycache__/generator.cpython-38.pyc
+-rw-r--r--   0        0        0     5681 2023-07-07 21:18:56.916693 lacss-0.4.2/lacss/data/__pycache__/parser.cpython-38.pyc
+-rw-r--r--   0        0        0    11600 2023-07-08 17:32:02.079356 lacss-0.4.2/lacss/data/augment.py
+-rw-r--r--   0        0        0    11146 2023-07-12 00:50:46.739025 lacss-0.4.2/lacss/data/generator.py
+-rw-r--r--   0        0        0     9281 2023-07-12 00:50:46.759730 lacss-0.4.2/lacss/deploy.py
+-rw-r--r--   0        0        0       74 2023-06-28 18:47:53.972115 lacss-0.4.2/lacss/losses/__init__.py
+-rw-r--r--   0        0        0      214 2023-06-28 21:50:59.406844 lacss-0.4.2/lacss/losses/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5177 2023-07-11 16:28:55.891597 lacss-0.4.2/lacss/losses/__pycache__/auxiliary.cpython-38.pyc
+-rw-r--r--   0        0        0     3294 2023-06-28 21:51:00.768928 lacss-0.4.2/lacss/losses/__pycache__/detection.cpython-38.pyc
+-rw-r--r--   0        0        0     5558 2023-07-09 18:24:34.810810 lacss-0.4.2/lacss/losses/__pycache__/instance.cpython-38.pyc
+-rw-r--r--   0        0        0     5464 2023-07-12 00:50:46.785030 lacss-0.4.2/lacss/losses/auxiliary.py
+-rw-r--r--   0        0        0     2423 2023-06-28 18:47:54.027008 lacss-0.4.2/lacss/losses/detection.py
+-rw-r--r--   0        0        0     6264 2023-07-12 00:50:46.810982 lacss-0.4.2/lacss/losses/instance.py
+-rw-r--r--   0        0        0       56 2023-06-28 18:47:54.050267 lacss-0.4.2/lacss/metrics/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-28 21:51:02.525934 lacss-0.4.2/lacss/metrics/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5311 2023-06-28 21:51:02.565585 lacss-0.4.2/lacss/metrics/__pycache__/ranked.cpython-38.pyc
+-rw-r--r--   0        0        0     5103 2023-06-28 18:47:54.111477 lacss-0.4.2/lacss/metrics/ranked.py
+-rw-r--r--   0        0        0      216 2023-06-28 18:47:54.159295 lacss-0.4.2/lacss/modules/__init__.py
+-rw-r--r--   0        0        0      435 2023-06-28 21:51:02.593407 lacss-0.4.2/lacss/modules/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1899 2023-07-11 16:28:56.927723 lacss-0.4.2/lacss/modules/__pycache__/auxiliary.cpython-38.pyc
+-rw-r--r--   0        0        0     3065 2023-07-11 16:28:56.943013 lacss-0.4.2/lacss/modules/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0        0        0     7504 2023-07-11 16:28:56.976521 lacss-0.4.2/lacss/modules/__pycache__/convnext.cpython-38.pyc
+-rw-r--r--   0        0        0     6006 2023-07-11 16:28:56.993007 lacss-0.4.2/lacss/modules/__pycache__/detector.cpython-38.pyc
+-rw-r--r--   0        0        0     3065 2023-07-11 16:28:57.007417 lacss-0.4.2/lacss/modules/__pycache__/lacss.cpython-38.pyc
+-rw-r--r--   0        0        0     2996 2023-07-11 16:28:57.022357 lacss-0.4.2/lacss/modules/__pycache__/lpn.cpython-38.pyc
+-rw-r--r--   0        0        0     3578 2023-06-28 21:51:02.783672 lacss-0.4.2/lacss/modules/__pycache__/resnet.cpython-38.pyc
+-rw-r--r--   0        0        0     4451 2023-07-11 16:28:57.048172 lacss-0.4.2/lacss/modules/__pycache__/segmentor.cpython-38.pyc
+-rw-r--r--   0        0        0     2245 2023-07-11 16:28:56.958798 lacss-0.4.2/lacss/modules/__pycache__/unet.cpython-38.pyc
+-rw-r--r--   0        0        0     1615 2023-07-12 00:50:46.829704 lacss-0.4.2/lacss/modules/auxiliary.py
+-rw-r--r--   0        0        0     2304 2023-07-12 00:50:46.844074 lacss-0.4.2/lacss/modules/common.py
+-rw-r--r--   0        0        0     7924 2023-07-12 00:50:46.860520 lacss-0.4.2/lacss/modules/convnext.py
+-rw-r--r--   0        0        0     7761 2023-07-12 00:50:46.876928 lacss-0.4.2/lacss/modules/detector.py
+-rw-r--r--   0        0        0     3514 2023-07-12 00:50:46.896680 lacss-0.4.2/lacss/modules/lacss.py
+-rw-r--r--   0        0        0     3289 2023-07-12 00:50:46.921773 lacss-0.4.2/lacss/modules/lpn.py
+-rw-r--r--   0        0        0     3771 2023-06-28 18:47:54.334941 lacss-0.4.2/lacss/modules/resnet.py
+-rw-r--r--   0        0        0     5460 2023-07-12 00:50:46.945019 lacss-0.4.2/lacss/modules/segmentor.py
+-rw-r--r--   0        0        0     2018 2023-07-12 00:50:46.965128 lacss-0.4.2/lacss/modules/unet.py
+-rw-r--r--   0        0        0      153 2023-07-12 00:50:46.984893 lacss-0.4.2/lacss/ops/__init__.py
+-rw-r--r--   0        0        0      253 2023-07-11 16:28:56.271477 lacss-0.4.2/lacss/ops/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2241 2023-07-11 16:28:56.289400 lacss-0.4.2/lacss/ops/__pycache__/boxes.cpython-38.pyc
+-rw-r--r--   0        0        0     3709 2023-07-11 16:28:56.558395 lacss-0.4.2/lacss/ops/__pycache__/image.cpython-38.pyc
+-rw-r--r--   0        0        0     2656 2023-07-11 16:28:56.582064 lacss-0.4.2/lacss/ops/__pycache__/locations.cpython-38.pyc
+-rw-r--r--   0        0        0     5806 2023-06-28 21:51:00.025138 lacss-0.4.2/lacss/ops/__pycache__/masks.cpython-38.pyc
+-rw-r--r--   0        0        0     4243 2023-07-11 16:28:56.604408 lacss-0.4.2/lacss/ops/__pycache__/nms.cpython-38.pyc
+-rw-r--r--   0        0        0    10132 2023-07-11 20:38:22.163010 lacss-0.4.2/lacss/ops/__pycache__/patches.cpython-38.pyc
+-rw-r--r--   0        0        0      674 2023-07-08 19:27:33.665462 lacss-0.4.2/lacss/ops/__pycache__/uda.cpython-38.pyc
+-rw-r--r--   0        0        0     2477 2023-07-12 00:50:47.008977 lacss-0.4.2/lacss/ops/boxes.py
+-rw-r--r--   0        0        0     3520 2023-07-12 00:50:47.032424 lacss-0.4.2/lacss/ops/image.py
+-rw-r--r--   0        0        0     3058 2023-07-12 00:50:47.053280 lacss-0.4.2/lacss/ops/locations.py
+-rw-r--r--   0        0        0     5967 2023-06-28 18:47:54.419954 lacss-0.4.2/lacss/ops/masks.py
+-rw-r--r--   0        0        0     5364 2023-07-12 00:50:47.066459 lacss-0.4.2/lacss/ops/nms.py
+-rw-r--r--   0        0        0    11731 2023-07-12 00:50:47.083525 lacss-0.4.2/lacss/ops/patches.py
+-rw-r--r--   0        0        0      482 2023-07-08 17:32:02.313196 lacss-0.4.2/lacss/ops/uda.py
+-rw-r--r--   0        0        0       63 2023-06-28 18:47:54.514459 lacss-0.4.2/lacss/tracking/__init__.py
+-rw-r--r--   0        0        0      205 2023-07-08 20:24:33.662770 lacss-0.4.2/lacss/tracking/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2689 2023-07-08 20:24:33.673606 lacss-0.4.2/lacss/tracking/__pycache__/predict.cpython-38.pyc
+-rw-r--r--   0        0        0     3340 2023-06-28 18:47:54.529736 lacss-0.4.2/lacss/tracking/predict.py
+-rw-r--r--   0        0        0    12669 2023-07-08 17:32:02.356138 lacss-0.4.2/lacss/tracking/seqnms.py
+-rw-r--r--   0        0        0     6741 2023-06-28 18:47:54.589306 lacss-0.4.2/lacss/tracking/smc.py
+-rw-r--r--   0        0        0     5646 2023-06-28 18:47:54.594114 lacss-0.4.2/lacss/tracking/utils.py
+-rw-r--r--   0        0        0      128 2023-07-12 00:50:47.107041 lacss-0.4.2/lacss/train/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-09 16:29:57.840757 lacss-0.4.2/lacss/train/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    11255 2023-07-11 16:28:56.709068 lacss-0.4.2/lacss/train/__pycache__/lacss_trainer.cpython-38.pyc
+-rw-r--r--   0        0        0     6686 2023-06-28 21:51:00.309749 lacss-0.4.2/lacss/train/__pycache__/loss.cpython-38.pyc
+-rw-r--r--   0        0        0      648 2023-06-28 21:51:02.541986 lacss-0.4.2/lacss/train/__pycache__/metric.cpython-38.pyc
+-rw-r--r--   0        0        0     4324 2023-07-10 15:48:25.988474 lacss-0.4.2/lacss/train/__pycache__/strategy.cpython-38.pyc
+-rw-r--r--   0        0        0    11605 2023-07-11 16:28:57.079209 lacss-0.4.2/lacss/train/__pycache__/trainer.cpython-38.pyc
+-rw-r--r--   0        0        0      718 2023-06-28 18:47:54.645358 lacss-0.4.2/lacss/train/data/__init__.py
+-rw-r--r--   0        0        0      851 2023-06-28 21:51:00.134440 lacss-0.4.2/lacss/train/data/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4005 2023-06-28 21:51:00.158605 lacss-0.4.2/lacss/train/data/__pycache__/array_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     6093 2023-06-28 21:51:00.175019 lacss-0.4.2/lacss/train/data/__pycache__/data_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     5561 2023-06-28 21:51:00.209885 lacss-0.4.2/lacss/train/data/__pycache__/data_handler.cpython-38.pyc
+-rw-r--r--   0        0        0    11577 2023-06-28 21:51:00.227323 lacss-0.4.2/lacss/train/data/__pycache__/dataset.cpython-38.pyc
+-rw-r--r--   0        0        0     3319 2023-06-28 21:51:00.243986 lacss-0.4.2/lacss/train/data/__pycache__/generator_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     2515 2023-06-28 21:51:00.258749 lacss-0.4.2/lacss/train/data/__pycache__/list_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     3562 2023-06-28 21:51:00.276389 lacss-0.4.2/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     3167 2023-06-28 21:51:00.292169 lacss-0.4.2/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-38.pyc
+-rw-r--r--   0        0        0     6796 2023-06-28 21:51:00.191450 lacss-0.4.2/lacss/train/data/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     4076 2023-06-28 18:47:54.657752 lacss-0.4.2/lacss/train/data/array_adapter.py
+-rw-r--r--   0        0        0     5529 2023-06-28 18:47:54.663888 lacss-0.4.2/lacss/train/data/data_adapter.py
+-rw-r--r--   0        0        0     6287 2023-06-28 18:47:54.682440 lacss-0.4.2/lacss/train/data/data_handler.py
+-rw-r--r--   0        0        0    10656 2023-06-28 18:47:54.688930 lacss-0.4.2/lacss/train/data/dataset.py
+-rw-r--r--   0        0        0     2599 2023-06-28 18:47:54.695077 lacss-0.4.2/lacss/train/data/generator_adapter.py
+-rw-r--r--   0        0        0     2105 2023-06-28 18:47:54.703830 lacss-0.4.2/lacss/train/data/list_adapter.py
+-rw-r--r--   0        0        0     3440 2023-06-28 18:47:54.711785 lacss-0.4.2/lacss/train/data/tf_dataset_adapter.py
+-rw-r--r--   0        0        0     2566 2023-06-28 18:47:54.718782 lacss-0.4.2/lacss/train/data/torch_dataloader_adapter.py
+-rw-r--r--   0        0        0     6394 2023-06-28 18:47:54.724036 lacss-0.4.2/lacss/train/data/utils.py
+-rw-r--r--   0        0        0    12877 2023-07-12 00:50:47.127056 lacss-0.4.2/lacss/train/lacss_trainer.py
+-rw-r--r--   0        0        0     6834 2023-06-28 18:47:54.733331 lacss-0.4.2/lacss/train/loss.py
+-rw-r--r--   0        0        0      222 2023-06-28 18:47:54.751027 lacss-0.4.2/lacss/train/metric.py
+-rw-r--r--   0        0        0     4228 2023-07-11 21:05:33.247706 lacss-0.4.2/lacss/train/strategy.py
+-rw-r--r--   0        0        0    13159 2023-07-12 00:50:47.146322 lacss-0.4.2/lacss/train/trainer.py
+-rw-r--r--   0        0        0     1051 2023-07-12 00:50:47.159425 lacss-0.4.2/lacss/types.py
+-rw-r--r--   0        0        0     6681 2023-07-12 00:50:47.175397 lacss-0.4.2/lacss/utils.py
+-rw-r--r--   0        0        0      981 2023-07-12 00:51:22.208637 lacss-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3165 1970-01-01 00:00:00.000000 lacss-0.4.2/PKG-INFO
```

### Comparing `lacss-0.4.1/LICENSE` & `lacss-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/README.md` & `lacss-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/data/__pycache__/augment.cpython-38.pyc` & `lacss-0.4.2/lacss/data/__pycache__/augment.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 19:35:53 2023 UTC, .py size: 11408 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 99e8 9964 902c 0000  U..........d.,..
+00000000: 550d 0d0a 0000 0000 929d a964 502d 0000  U..........dP-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 da00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6403 6404 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6405 6406 8400 5a05 6407  m.Z...d.d...Z.d.
 00000050: 6408 8400 5a06 6409 640a 8400 5a07 640b  d...Z.d.d...Z.d.
 00000060: 640c 9c01 640d 640e 8402 5a08 640f 640b  d...d.d...Z.d.d.
 00000070: 6410 9c02 6411 6412 8402 5a09 640b 640b  d...d.d...Z.d.d.
@@ -129,34 +129,34 @@
 00000800: 2061 2072 616e 6765 206f 6620 7363 616c   a range of scal
 00000810: 6572 1a00 0000 7202 0000 0072 1c00 0000  er....r....r....
 00000820: 7229 0000 004e 2909 7207 0000 0072 2d00  r)...N).r....r-.
 00000830: 0000 722e 0000 0072 1200 0000 7219 0000  ..r....r....r...
 00000840: 00da 0572 6f75 6e64 7223 0000 0072 2400  ...roundr#...r$.
 00000850: 0000 7225 0000 0029 0c72 0b00 0000 da07  ..r%...).r......
 00000860: 7363 616c 696e 6772 2f00 0000 721b 0000  scalingr/...r...
-00000870: 00da 096d 696e 5f73 6361 6c65 5a09 6d61  ...min_scaleZ.ma
+00000870: 005a 096d 696e 5f73 6361 6c65 5a09 6d61  .Z.min_scaleZ.ma
 00000880: 785f 7363 616c 6572 1700 0000 7218 0000  x_scaler....r...
 00000890: 0072 2700 0000 7228 0000 00da 0874 6172  .r'...r(.....tar
 000008a0: 6765 745f 68da 0874 6172 6765 745f 7772  get_h..target_wr
 000008b0: 0c00 0000 720c 0000 0072 0d00 0000 da0d  ....r....r......
 000008c0: 7261 6e64 6f6d 5f72 6573 697a 6550 0000  random_resizeP..
 000008d0: 0073 1e00 0000 0003 1801 0403 0c01 1001  .s..............
 000008e0: 0801 0802 1002 0401 1001 0602 1001 1002  ................
-000008f0: 1801 1802 7235 0000 0029 02da 1461 7265  ....r5...)...are
+000008f0: 1801 1802 7234 0000 0029 02da 1461 7265  ....r4...)...are
 00000900: 615f 7261 7469 6f5f 7468 7265 7368 6f6c  a_ratio_threshol
 00000910: 6472 1b00 0000 6301 0000 0000 0000 0003  dr....c.........
 00000920: 0000 0005 0000 0003 0000 0003 0000 0073  ...............s
 00000930: 3600 0000 8700 8701 6602 6401 6402 8408  6.......f.d.d...
 00000940: 7d04 7c03 6403 6b00 722a 7400 6a01 a002  }.|.d.k.r*t.j...
 00000950: 6700 a101 7c03 6b05 722a 7c00 5300 7c04  g...|.k.r*|.S.|.
 00000960: 7c00 8301 5300 6404 5300 2905 7a1e 4372  |...S.d.S.).z.Cr
 00000970: 6f70 2069 6d61 6765 2074 6f20 626f 756e  op image to boun
 00000980: 6469 6e67 2d62 6f78 2052 4f49 6301 0000  ding-box ROIc...
 00000990: 0000 0000 0000 0000 0013 0000 0009 0000  ................
-000009a0: 0013 0000 0073 0603 0000 8801 5c04 7d01  .....s......\.}.
+000009a0: 0013 0000 0073 2403 0000 8801 5c04 7d01  .....s$.....\.}.
 000009b0: 7d02 7d03 7d04 7400 a001 7c03 7c01 1800  }.}.}.t...|.|...
 000009c0: 7400 6a02 a102 7d05 7400 a001 7c04 7c02  t.j...}.t...|.|.
 000009d0: 1800 7400 6a02 a102 7d06 7c00 6401 1900  ..t.j...}.|.d...
 000009e0: 7c01 7c03 8502 7c02 7c04 8502 6400 6400  |.|...|.|...d.d.
 000009f0: 8502 6603 1900 7c00 6401 3c00 6402 7c00  ..f...|.d.<.d.|.
 00000a00: 6b06 7276 7c00 6402 1900 7c01 7c03 8502  k.rv|.d...|.|...
 00000a10: 7c02 7c04 8502 6602 1900 7c00 6402 3c00  |.|...f...|.d.<.
@@ -177,323 +177,326 @@
 00000b00: 7c09 7400 a001 7c05 7c06 7c05 7c06 6704  |.t...|.|.|.|.g.
 00000b10: 7400 6a02 a102 a102 7d09 7400 a006 7c09  t.j.....}.t...|.
 00000b20: 6404 a102 7d09 7c09 6400 6400 8502 6409  d...}.|.d.d...d.
 00000b30: 6602 1900 7c09 6400 6400 8502 6404 6602  f...|.d.d...d.f.
 00000b40: 1900 1800 7c09 6400 6400 8502 640a 6602  ....|.d.d...d.f.
 00000b50: 1900 7c09 6400 6400 8502 6407 6602 1900  ..|.d.d...d.f...
 00000b60: 1800 1400 7d0b 7c07 7c0b 7c0a 1b00 8800  ....}.|.|.|.....
-00000b70: 6b05 4d00 7d07 6403 7c00 6b06 9001 72e2  k.M.}.d.|.k...r.
-00000b80: 7c08 7c07 1900 7c00 6403 3c00 6408 7c00  |.|...|.d.<.d.|.
-00000b90: 6b06 9003 7202 7c00 6408 1900 7c07 1900  k...r.|.d...|...
-00000ba0: 7d0c 7c09 7c07 1900 7c00 6408 3c00 640b  }.|.|...|.d.<.d.
-00000bb0: 7c00 6b06 9003 7202 7c00 640b 1900 6a07  |.k...r.|.d...j.
-00000bc0: 6407 640a 8502 1900 7d0d 7c0c 6400 6400  d.d.....}.|.d.d.
-00000bd0: 8502 6404 6602 1900 7400 a001 7c01 7c0c  ..d.f...t...|.|.
-00000be0: 6a08 a102 1800 7d0e 7c0c 6400 6400 8502  j.....}.|.d.d...
-00000bf0: 6407 6602 1900 7400 a001 7c02 7c0c 6a08  d.f...t...|.|.j.
-00000c00: a102 1800 7d0f 7c0c 6400 6400 8502 6409  ....}.|.d.d...d.
-00000c10: 6602 1900 7c0c 6400 6400 8502 6404 6602  f...|.d.d...d.f.
-00000c20: 1900 1800 7d10 7c0c 6400 6400 8502 640a  ....}.|.d.d...d.
-00000c30: 6602 1900 7c0c 6400 6400 8502 6407 6602  f...|.d.d...d.f.
-00000c40: 1900 1800 7d11 7c00 6408 1900 7400 6a09  ....}.|.d...t.j.
-00000c50: 7c0e 7c0f 7c0e 7c0f 6704 6405 6406 8d02  |.|.|.|.g.d.d...
-00000c60: 1800 7d12 7c12 7400 6a09 7c10 7c11 7c10  ..}.|.t.j.|.|.|.
-00000c70: 7c11 6704 6405 6406 8d02 1b00 7d12 7c12  |.g.d.d.....}.|.
-00000c80: 7400 a001 7c0d 7c0d 1700 7c12 6a08 a102  t...|.|...|.j...
-00000c90: 1400 7d12 740a 7c00 640b 1900 7c07 1900  ..}.t.|.d...|...
-00000ca0: 7c12 7c0d 8303 7c00 640b 3c00 7c00 5300  |.|...|.d.<.|.S.
-00000cb0: 290c 4e72 1c00 0000 721e 0000 0072 0400  ).Nr....r....r..
-00000cc0: 0000 7201 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
-00000cd0: 0072 0200 0000 7206 0000 00e9 0200 0000  .r....r.........
-00000ce0: e903 0000 00da 056d 6173 6b73 290b 7207  .......masks).r.
-00000cf0: 0000 0072 2300 0000 7224 0000 0072 0e00  ...r#...r$...r..
-00000d00: 0000 da0a 7265 6475 6365 5f61 6c6c da07  ....reduce_all..
-00000d10: 6d69 6e69 6d75 6dda 076d 6178 696d 756d  minimum..maximum
-00000d20: 7215 0000 0072 0500 0000 da05 7374 6163  r....r......stac
-00000d30: 6b72 0300 0000 2913 720b 0000 00da 0279  kr....).r......y
-00000d40: 30da 0278 30da 0279 31da 0278 315a 0572  0..x0..y1..x1Z.r
-00000d50: 6f69 5f68 5a05 726f 695f 77da 0c62 6f6f  oi_hZ.roi_w..boo
-00000d60: 6c65 616e 5f6d 6173 6b5a 0563 7472 6473  lean_maskZ.ctrds
-00000d70: 7206 0000 00da 0561 7265 6173 5a09 6e65  r......areasZ.ne
-00000d80: 775f 6172 6561 735a 0b6f 7269 675f 6262  w_areasZ.orig_bb
-00000d90: 6f78 6573 da0c 7461 7267 6574 5f73 6861  oxes..target_sha
-00000da0: 7065 5a07 6f72 6967 5f79 305a 076f 7269  peZ.orig_y0Z.ori
-00000db0: 675f 7830 5a06 6f72 6967 5f68 5a06 6f72  g_x0Z.orig_hZ.or
-00000dc0: 6967 5f77 5a08 6e65 775f 6262 6f78 a902  ig_wZ.new_bbox..
-00000dd0: 7236 0000 00da 0372 6f69 720c 0000 0072  r6.....roir....r
-00000de0: 0d00 0000 da0c 5f63 726f 705f 746f 5f72  ......_crop_to_r
-00000df0: 6f69 6e00 0000 7372 0000 0000 010c 0112  oin...sr........
-00000e00: 0112 0222 0208 011c 0208 0208 0104 0208  ..."............
-00000e10: 011a 0102 0110 0112 ff02 0212 fe02 ff04  ................
-00000e20: 060a 011e 0140 0204 0102 0014 ff04 030c  .....@..........
-00000e30: 0140 0210 020a 010c 020a 010c 010c 020a  .@..............
-00000e40: 0112 021e 011e 0120 0120 020a 010a 0002  ....... . ......
-00000e50: ff08 0306 010a 0002 ff08 0306 0106 0004  ................
-00000e60: ff06 0402 010a 0102 0102 fd08 067a 2163  .............z!c
-00000e70: 726f 705f 746f 5f72 6f69 2e3c 6c6f 6361  rop_to_roi.<loca
-00000e80: 6c73 3e2e 5f63 726f 705f 746f 5f72 6f69  ls>._crop_to_roi
-00000e90: 721a 0000 004e 722c 0000 0029 0572 0b00  r....Nr,...).r..
-00000ea0: 0000 7246 0000 0072 3600 0000 721b 0000  ..rF...r6...r...
-00000eb0: 0072 4700 0000 720c 0000 0072 4500 0000  .rG...r....rE...
-00000ec0: 720d 0000 00da 0b63 726f 705f 746f 5f72  r......crop_to_r
-00000ed0: 6f69 6b00 0000 7308 0000 0000 030e 4418  oik...s.......D.
-00000ee0: 0104 0372 4800 0000 6301 0000 0000 0000  ...rH...c.......
-00000ef0: 0003 0000 000a 0000 0007 0000 0043 0000  .............C..
-00000f00: 0073 9e00 0000 7400 7c00 6401 1900 8301  .s....t.|.d.....
-00000f10: 5c02 7d04 7d05 7401 7c01 8301 5c02 7d06  \.}.}.t.|...\.}.
-00000f20: 7d07 7c03 6402 6b00 7238 7402 6a03 a004  }.|.d.k.r8t.j...
-00000f30: 6700 a101 7c03 6b05 7238 7c00 5300 7405  g...|.k.r8|.S.t.
-00000f40: 7402 6a03 a004 6700 a101 7402 a006 7c04  t.j...g...t...|.
-00000f50: 7c06 1800 7402 6a07 a102 1400 8301 7d08  |...t.j.......}.
-00000f60: 7405 7402 6a03 a004 6700 a101 7402 a006  t.t.j...g...t...
-00000f70: 7c05 7c07 1800 7402 6a07 a102 1400 8301  |.|...t.j.......
-00000f80: 7d09 7408 7c00 7c08 7c09 7c08 7c06 1700  }.t.|.|.|.|.|...
-00000f90: 7c09 7c07 1700 6604 7c02 6403 8d03 5300  |.|...f.|.d...S.
-00000fa0: 6404 5300 2905 7a20 5261 6e64 6f6d 2063  d.S.).z Random c
-00000fb0: 726f 7020 746f 2061 2073 6574 2074 6172  rop to a set tar
-00000fc0: 6765 7420 7369 7a65 721c 0000 0072 1a00  get sizer....r..
-00000fd0: 0000 2902 7246 0000 0072 3600 0000 4e29  ..).rF...r6...N)
-00000fe0: 0972 1900 0000 7212 0000 0072 0700 0000  .r....r....r....
-00000ff0: 722d 0000 0072 2e00 0000 da03 696e 7472  r-...r......intr
-00001000: 2300 0000 7224 0000 0072 4800 0000 290a  #...r$...rH...).
-00001010: 720b 0000 0072 2a00 0000 7236 0000 0072  r....r*...r6...r
-00001020: 1b00 0000 7217 0000 0072 1800 0000 7233  ....r....r....r3
-00001030: 0000 0072 3400 0000 723e 0000 0072 3f00  ...r4...r>...r?.
-00001040: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00001050: 00da 0b72 616e 646f 6d5f 6372 6f70 b900  ...random_crop..
-00001060: 0000 7316 0000 0000 0310 020c 0218 0104  ..s.............
-00001070: 0322 0122 0202 0102 0112 0102 fd72 4a00  .".".........rJ.
-00001080: 0000 2902 da0f 636f 6e73 7461 6e74 5f76  ..)...constant_v
-00001090: 616c 7565 7372 1b00 0000 6301 0000 0000  aluesr....c.....
-000010a0: 0000 0003 0000 0005 0000 0003 0000 0003  ................
-000010b0: 0000 0073 3600 0000 8700 8701 6602 6401  ...s6.......f.d.
-000010c0: 6402 8408 7d04 7c03 6403 6b00 722a 7400  d...}.|.d.k.r*t.
-000010d0: 6a01 a002 6700 a101 7c03 6b05 722a 7c00  j...g...|.k.r*|.
-000010e0: 5300 7c04 7c00 8301 5300 6404 5300 2905  S.|.|...S.d.S.).
-000010f0: 7a15 5061 6420 696d 6167 6520 616e 6420  z.Pad image and 
-00001100: 6c61 6265 6c73 2e63 0100 0000 0000 0000  labels.c........
-00001110: 0000 0000 0900 0000 0900 0000 1300 0000  ................
-00001120: 7300 0100 0074 0088 0183 015c 027d 017d  s....t.....\.}.}
-00001130: 0274 007c 0183 015c 027d 037d 0474 007c  .t.|...\.}.}.t.|
-00001140: 0283 015c 027d 057d 0674 016a 027c 0064  ...\.}.}.t.j.|.d
-00001150: 0119 007c 037c 0467 027c 057c 0667 0264  ...|.|.g.|.|.g.d
-00001160: 0264 0267 0267 0388 0064 038d 037c 0064  .d.g.g...d...|.d
-00001170: 013c 0064 047c 006b 0672 ac7c 0064 0419  .<.d.|.k.r.|.d..
-00001180: 007d 0774 037c 076a 0483 0164 056b 0272  .}.t.|.j...d.k.r
-00001190: 7e7c 037c 0467 027c 057c 0667 0267 027d  ~|.|.g.|.|.g.g.}
-000011a0: 086e 1664 0264 0267 027c 037c 0467 027c  .n.d.d.g.|.|.g.|
-000011b0: 057c 0667 0267 037d 0874 016a 027c 0064  .|.g.g.}.t.j.|.d
-000011c0: 0419 007c 0888 0064 038d 037c 0064 043c  ...|...d...|.d.<
-000011d0: 0064 067c 006b 0672 d27c 0064 0605 0019  .d.|.k.r.|.d....
-000011e0: 0074 01a0 057c 037c 0567 0274 016a 06a1  .t...|.|.g.t.j..
-000011f0: 0237 0003 003c 0064 077c 006b 0672 fc7c  .7...<.d.|.k.r.|
-00001200: 0064 0705 0019 0074 01a0 057c 037c 057c  .d.....t...|.|.|
-00001210: 037c 0567 0474 016a 06a1 0237 0003 003c  .|.g.t.j...7...<
-00001220: 007c 0053 0029 084e 721c 0000 0072 0100  .|.S.).Nr....r..
-00001230: 0000 2901 724b 0000 0072 1e00 0000 7237  ..).rK...r....r7
-00001240: 0000 0072 0400 0000 7206 0000 0029 0772  ...r....r....).r
-00001250: 1200 0000 7207 0000 00da 0370 6164 7209  ....r......padr.
-00001260: 0000 0072 1500 0000 7223 0000 0072 2400  ...r....r#...r$.
-00001270: 0000 2909 720b 0000 005a 0970 6164 6469  ..).r....Z.paddi
-00001280: 6e67 5f79 5a09 7061 6464 696e 675f 785a  ng_yZ.padding_xZ
-00001290: 0a70 6164 6469 6e67 5f79 305a 0a70 6164  .padding_y0Z.pad
-000012a0: 6469 6e67 5f79 315a 0a70 6164 6469 6e67  ding_y1Z.padding
-000012b0: 5f78 305a 0a70 6164 6469 6e67 5f78 3172  _x0Z.padding_x1r
-000012c0: 1e00 0000 da0e 7061 6464 696e 675f 7661  ......padding_va
-000012d0: 6c75 6573 a902 724b 0000 00da 0870 6164  lues..rK.....pad
-000012e0: 6469 6e67 7372 0c00 0000 720d 0000 00da  dingsr....r.....
-000012f0: 045f 7061 64d1 0000 0073 3a00 0000 0001  ._pad....s:.....
-00001300: 0c01 0c01 0c02 0401 0601 1401 02fd 0a06  ................
-00001310: 0801 0801 0e01 1203 0601 0601 06fd 0405  ................
-00001320: 0401 0601 0201 02fd 0a06 0801 1e02 0801  ................
-00001330: 0c01 0a00 04ff 0804 7a11 7061 642e 3c6c  ........z.pad.<l
-00001340: 6f63 616c 733e 2e5f 7061 6472 1a00 0000  ocals>._padr....
-00001350: 4e72 2c00 0000 2905 720b 0000 0072 4f00  Nr,...).r....rO.
-00001360: 0000 724b 0000 0072 1b00 0000 7250 0000  ..rK...r....rP..
-00001370: 0072 0c00 0000 724e 0000 0072 0d00 0000  .r....rN...r....
-00001380: 724c 0000 00ce 0000 0073 0800 0000 0003  rL.......s......
-00001390: 0e25 1801 0403 724c 0000 0063 0100 0000  .%....rL...c....
-000013a0: 0000 0000 0300 0000 0a00 0000 0500 0000  ................
-000013b0: 4300 0000 7382 0000 007c 0364 016b 0072  C...s....|.d.k.r
-000013c0: 1c74 006a 01a0 0267 00a1 017c 036b 0572  .t.j...g...|.k.r
-000013d0: 1c7c 0053 0074 037c 0064 0219 0083 015c  .|.S.t.|.d.....\
-000013e0: 027d 047d 0574 047c 0183 015c 027d 067d  .}.}.t.|...\.}.}
-000013f0: 077c 067c 0418 007d 087c 0864 031a 007c  .|.|...}.|.d...|
-00001400: 087c 0864 031a 0018 0067 027d 087c 077c  .|.d.....g.}.|.|
-00001410: 0518 007d 097c 0964 031a 007c 097c 0964  ...}.|.d...|.|.d
-00001420: 031a 0018 0067 027d 0974 057c 007c 087c  .....g.}.t.|.|.|
-00001430: 0967 027c 0264 048d 0353 0029 054e 721a  .g.|.d...S.).Nr.
-00001440: 0000 0072 1c00 0000 7237 0000 0029 0272  ...r....r7...).r
-00001450: 4f00 0000 724b 0000 0029 0672 0700 0000  O...rK...).r....
-00001460: 722d 0000 0072 2e00 0000 7219 0000 0072  r-...r....r....r
-00001470: 1200 0000 724c 0000 0029 0a72 0b00 0000  ....rL...).r....
-00001480: 722a 0000 0072 4b00 0000 721b 0000 0072  r*...rK...r....r
-00001490: 1700 0000 7218 0000 0072 3300 0000 7234  ....r....r3...r4
-000014a0: 0000 005a 0970 6164 6469 6e67 5f68 5a09  ...Z.padding_hZ.
-000014b0: 7061 6464 696e 675f 7772 0c00 0000 720c  padding_wr....r.
-000014c0: 0000 0072 0d00 0000 da0b 7061 645f 746f  ...r......pad_to
-000014d0: 5f73 697a 65fd 0000 0073 1200 0000 0001  _size....s......
-000014e0: 1801 0402 1001 0c02 0801 1401 0801 1402  ................
-000014f0: 7251 0000 0029 0372 4b00 0000 7236 0000  rQ...).rK...r6..
-00001500: 0072 1b00 0000 6301 0000 0000 0000 0004  .r....c.........
-00001510: 0000 000b 0000 0006 0000 0043 0000 0073  ...........C...s
-00001520: 8c00 0000 7c04 6401 6b00 721c 7400 6a01  ....|.d.k.r.t.j.
-00001530: a002 6700 a101 7c04 6b05 721c 7c00 5300  ..g...|.k.r.|.S.
-00001540: 7403 7c00 6402 1900 8301 5c02 7d05 7d06  t.|.d.....\.}.}.
-00001550: 7404 7c01 8301 5c02 7d07 7d08 7400 a005  t.|...\.}.}.t...
-00001560: 7400 a006 7c05 7c07 a102 7c05 6a07 a102  t...|.|...|.j...
-00001570: 7d09 7400 a005 7400 a006 7c06 7c08 a102  }.t...t...|.|...
-00001580: 7c06 6a07 a102 7d0a 7408 7c00 7c09 7c0a  |.j...}.t.|.|.|.
-00001590: 6602 7c02 6403 8d03 7d00 7409 7c00 7c01  f.|.d...}.t.|.|.
-000015a0: 7c03 6404 8d03 7d00 7c00 5300 6405 5300  |.d...}.|.S.d.S.
-000015b0: 2906 7a27 5261 6e64 6f6d 2063 726f 7020  ).z'Random crop 
-000015c0: 6f72 2070 6164 2069 6d61 6765 2074 6f20  or pad image to 
-000015d0: 7461 7267 6574 5f73 697a 6572 1a00 0000  target_sizer....
-000015e0: 721c 0000 0029 0272 2a00 0000 724b 0000  r....).r*...rK..
-000015f0: 0029 0272 2a00 0000 7236 0000 004e 290a  .).r*...r6...N).
-00001600: 7207 0000 0072 2d00 0000 722e 0000 0072  r....r-...r....r
-00001610: 1900 0000 7212 0000 0072 2300 0000 723c  ....r....r#...r<
-00001620: 0000 0072 0500 0000 7251 0000 0072 4a00  ...r....rQ...rJ.
-00001630: 0000 290b 720b 0000 0072 2a00 0000 724b  ..).r....r*...rK
-00001640: 0000 0072 3600 0000 721b 0000 0072 1700  ...r6...r....r..
-00001650: 0000 7218 0000 0072 3300 0000 7234 0000  ..r....r3...r4..
-00001660: 00da 0168 da01 7772 0c00 0000 720c 0000  ...h..wr....r...
-00001670: 0072 0d00 0000 da12 7261 6e64 6f6d 5f63  .r......random_c
-00001680: 726f 705f 6f72 5f70 6164 0c01 0000 7322  rop_or_pad....s"
-00001690: 0000 0000 0518 0104 0310 020c 0216 0116  ................
-000016a0: 0202 0102 0006 0002 ff06 0402 0102 0002  ................
-000016b0: 0002 ff06 0472 5400 0000 6301 0000 0000  .....rT...c.....
-000016c0: 0000 0001 0000 0003 0000 0003 0000 0043  ...............C
-000016d0: 0000 0073 3000 0000 6401 6402 8400 7d02  ...s0...d.d...}.
-000016e0: 7c01 6403 6b00 7224 7400 6a01 a002 6700  |.d.k.r$t.j...g.
-000016f0: a101 7c01 6b05 7224 7c00 5300 7c02 7c00  ..|.k.r$|.S.|.|.
-00001700: 8301 5300 6400 5300 2904 4e63 0100 0000  ..S.d.S.).Nc....
-00001710: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00001720: 5300 0000 73a6 0000 0074 007c 0064 0119  S...s....t.|.d..
-00001730: 0083 015c 027d 017d 0274 016a 02a0 037c  ...\.}.}.t.j...|
-00001740: 0064 0119 00a1 017c 0064 013c 0064 027c  .d.....|.d.<.d.|
-00001750: 006b 0672 527c 0064 0219 0064 0319 007d  .k.rR|.d...d...}
-00001760: 0374 016a 0474 016a 02a0 037c 03a1 0164  .t.j.t.j...|...d
-00001770: 0464 058d 027c 0064 023c 0064 067c 006b  .d...|.d.<.d.|.k
-00001780: 0672 767c 0064 0619 0064 0764 0467 0214  .rv|.d...d.d.g..
-00001790: 0064 087c 0267 0217 007c 0064 063c 0064  .d.|.g...|.d.<.d
-000017a0: 097c 006b 0672 a27c 0064 0919 0064 0764  .|.k.r.|.d...d.d
-000017b0: 0464 0764 0467 0414 0064 087c 0264 087c  .d.d.g...d.|.d.|
-000017c0: 0267 0417 007c 0064 093c 007c 0053 00a9  .g...|.d.<.|.S..
-000017d0: 0a4e 721c 0000 0072 1e00 0000 721f 0000  .Nr....r....r...
-000017e0: 0072 2000 0000 7221 0000 0072 0400 0000  .r ...r!...r....
-000017f0: 7202 0000 0072 0100 0000 7206 0000 0029  r....r....r....)
-00001800: 0572 1900 0000 7207 0000 0072 1c00 0000  .r....r....r....
-00001810: da0f 666c 6970 5f6c 6566 745f 7269 6768  ..flip_left_righ
-00001820: 7472 2600 0000 a904 720b 0000 0072 1700  tr&.....r....r..
-00001830: 0000 7218 0000 0072 1e00 0000 720c 0000  ..r....r....r...
-00001840: 0072 0c00 0000 720d 0000 00da 105f 666c  .r....r......_fl
-00001850: 6970 5f6c 6566 745f 7269 6768 7428 0100  ip_left_right(..
-00001860: 0073 1a00 0000 0001 1002 1402 0801 0c01  .s..............
-00001870: 0401 0a01 02fe 0a05 0801 1c02 0801 2405  ..............$.
-00001880: 7a29 666c 6970 5f6c 6566 745f 7269 6768  z)flip_left_righ
-00001890: 742e 3c6c 6f63 616c 733e 2e5f 666c 6970  t.<locals>._flip
-000018a0: 5f6c 6566 745f 7269 6768 7472 1a00 0000  _left_rightr....
-000018b0: 722c 0000 0029 0372 0b00 0000 721b 0000  r,...).r....r...
-000018c0: 0072 5800 0000 720c 0000 0072 0c00 0000  .rX...r....r....
-000018d0: 720d 0000 0072 5600 0000 2701 0000 7308  r....rV...'...s.
-000018e0: 0000 0000 0108 1718 0104 0372 5600 0000  ...........rV...
-000018f0: 6301 0000 0000 0000 0001 0000 0003 0000  c...............
-00001900: 0003 0000 0043 0000 0073 3000 0000 6401  .....C...s0...d.
-00001910: 6402 8400 7d02 7c01 6403 6b00 7224 7400  d...}.|.d.k.r$t.
-00001920: 6a01 a002 6700 a101 7c01 6b05 7224 7c00  j...g...|.k.r$|.
-00001930: 5300 7c02 7c00 8301 5300 6400 5300 2904  S.|.|...S.d.S.).
-00001940: 4e63 0100 0000 0000 0000 0000 0000 0400  Nc..............
-00001950: 0000 0500 0000 5300 0000 73a6 0000 0074  ......S...s....t
-00001960: 007c 0064 0119 0083 015c 027d 017d 0274  .|.d.....\.}.}.t
-00001970: 016a 02a0 037c 0064 0119 00a1 017c 0064  .j...|.d.....|.d
-00001980: 013c 0064 027c 006b 0672 527c 0064 0219  .<.d.|.k.rR|.d..
-00001990: 0064 0319 007d 0374 016a 0474 016a 02a0  .d...}.t.j.t.j..
-000019a0: 037c 03a1 0164 0464 058d 027c 0064 023c  .|...d.d...|.d.<
-000019b0: 0064 067c 006b 0672 767c 0064 0619 0064  .d.|.k.rv|.d...d
-000019c0: 0464 0767 0214 007c 0164 0867 0217 007c  .d.g...|.d.g...|
-000019d0: 0064 063c 0064 097c 006b 0672 a27c 0064  .d.<.d.|.k.r.|.d
-000019e0: 0919 0064 0464 0764 0464 0767 0414 007c  ...d.d.d.d.g...|
-000019f0: 0164 087c 0164 0867 0417 007c 0064 093c  .d.|.d.g...|.d.<
-00001a00: 007c 0053 0072 5500 0000 2905 7219 0000  .|.S.rU...).r...
-00001a10: 0072 0700 0000 721c 0000 00da 0c66 6c69  .r....r......fli
-00001a20: 705f 7570 5f64 6f77 6e72 2600 0000 7257  p_up_downr&...rW
-00001a30: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00001a40: 0000 da0d 5f66 6c69 705f 7570 5f64 6f77  ...._flip_up_dow
-00001a50: 6e47 0100 0073 1a00 0000 0001 1002 1402  nG...s..........
-00001a60: 0801 0c01 0401 0a01 02fe 0a05 0801 1c02  ................
-00001a70: 0801 2405 7a23 666c 6970 5f75 705f 646f  ..$.z#flip_up_do
-00001a80: 776e 2e3c 6c6f 6361 6c73 3e2e 5f66 6c69  wn.<locals>._fli
-00001a90: 705f 7570 5f64 6f77 6e72 1a00 0000 722c  p_up_downr....r,
-00001aa0: 0000 0029 0372 0b00 0000 721b 0000 0072  ...).r....r....r
-00001ab0: 5a00 0000 720c 0000 0072 0c00 0000 720d  Z...r....r....r.
-00001ac0: 0000 0072 5900 0000 4601 0000 7308 0000  ...rY...F...s...
-00001ad0: 0000 0108 1718 0104 0372 5900 0000 6301  .........rY...c.
-00001ae0: 0000 0000 0000 0000 0000 0005 0000 0005  ................
-00001af0: 0000 0043 0000 0073 4c00 0000 6401 6400  ...C...sL...d.d.
-00001b00: 6c00 7d01 6401 6402 6c01 6d02 7d02 0100  l.}.d.d.l.m.}...
-00001b10: 7c01 a003 6403 6404 8400 7c02 7c00 8301  |...d.d...|.|...
-00001b20: 4400 8301 a101 7d03 7c01 a003 6405 6404  D.....}.|...d.d.
-00001b30: 8400 7c02 7c00 8301 4400 8301 a101 7d04  ..|.|...D.....}.
-00001b40: 7c03 7c04 6602 5300 2906 4e72 0100 0000  |.|.f.S.).Nr....
-00001b50: 2901 da0b 7265 6769 6f6e 7072 6f70 7363  )...regionpropsc
-00001b60: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001b70: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-00001b80: 005d 0c7d 017c 0164 0019 0091 0271 0453  .].}.|.d.....q.S
-00001b90: 0029 01da 0462 626f 7872 0c00 0000 a902  .)...bboxr......
-00001ba0: da02 2e30 da01 7272 0c00 0000 720c 0000  ...0..rr....r...
-00001bb0: 0072 0d00 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
-00001bc0: 703e 6901 0000 7304 0000 0006 0002 007a  p>i...s........z
-00001bd0: 245f 6262 6f78 5f66 726f 6d5f 6c61 6265  $_bbox_from_labe
-00001be0: 6c2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  l.<locals>.<list
-00001bf0: 636f 6d70 3e63 0100 0000 0000 0000 0000  comp>c..........
-00001c00: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
-00001c10: 0000 0067 007c 005d 0c7d 017c 0164 0019  ...g.|.].}.|.d..
-00001c20: 0091 0271 0453 0029 0172 0400 0000 720c  ...q.S.).r....r.
-00001c30: 0000 0072 5d00 0000 720c 0000 0072 0c00  ...r]...r....r..
-00001c40: 0000 720d 0000 0072 6000 0000 6a01 0000  ..r....r`...j...
-00001c50: 7304 0000 0006 0002 0029 04da 056e 756d  s........)...num
-00001c60: 7079 5a0f 736b 696d 6167 652e 6d65 6173  pyZ.skimage.meas
-00001c70: 7572 6572 5b00 0000 da07 6173 6172 7261  urer[.....asarra
-00001c80: 7929 05da 056c 6162 656c da02 6e70 725b  y)...label..npr[
-00001c90: 0000 0072 0600 0000 7204 0000 0072 0c00  ...r....r....r..
-00001ca0: 0000 720c 0000 0072 0d00 0000 da10 5f62  ..r....r......_b
-00001cb0: 626f 785f 6672 6f6d 5f6c 6162 656c 6501  box_from_labele.
-00001cc0: 0000 730a 0000 0000 0108 010c 0218 0118  ..s.............
-00001cd0: 0272 6500 0000 e930 0000 0029 01da 0a6d  .re....0...)...m
-00001ce0: 6173 6b5f 7368 6170 6563 0100 0000 0000  ask_shapec......
-00001cf0: 0000 0100 0000 0500 0000 0800 0000 4300  ..............C.
-00001d00: 0000 738e 0000 007c 0064 0119 007d 0264  ..s....|.d...}.d
-00001d10: 027c 006b 0773 1864 037c 006b 0772 3e74  .|.k.s.d.|.k.r>t
-00001d20: 00a0 0174 027c 0267 0174 006a 0374 006a  ...t.|.g.t.j.t.j
-00001d30: 0367 0264 04a1 045c 027c 0064 023c 007c  .g.d...\.|.d.<.|
-00001d40: 0064 033c 0074 047c 0064 0219 0083 017d  .d.<.t.|.d.....}
-00001d50: 0374 00a0 057c 0274 00a0 0664 057c 0364  .t...|.t...d.|.d
-00001d60: 0517 00a1 0264 0064 0085 0264 0064 0066  .....d.d...d.d.f
-00001d70: 0319 006b 0274 006a 07a1 027d 0474 087c  ...k.t.j...}.t.|
-00001d80: 047c 0064 0219 007c 0183 037c 0064 063c  .|.d...|...|.d.<
-00001d90: 007c 0053 0029 074e 7263 0000 0072 0600  .|.S.).Nrc...r..
-00001da0: 0000 7204 0000 0046 7202 0000 0072 3900  ..r....Fr....r9.
-00001db0: 0000 2909 7207 0000 005a 0a6e 756d 7079  ..).r....Z.numpy
-00001dc0: 5f66 756e 6372 6500 0000 7224 0000 0072  _funcre...r$...r
-00001dd0: 0900 0000 7223 0000 00da 0572 616e 6765  ....r#.....range
-00001de0: da05 696e 7433 3272 0300 0000 2905 720b  ..int32r....).r.
-00001df0: 0000 0072 6700 0000 7263 0000 005a 0b6e  ...rg...rc...Z.n
-00001e00: 5f69 6e73 7461 6e63 6573 5a0e 6c61 6265  _instancesZ.labe
-00001e10: 6c5f 6578 7061 6e64 6564 720c 0000 0072  l_expandedr....r
-00001e20: 0c00 0000 720d 0000 00da 0f6d 6173 6b5f  ....r......mask_
-00001e30: 6672 6f6d 5f6c 6162 656c 6f01 0000 7326  from_labelo...s&
-00001e40: 0000 0000 0108 0210 0104 0102 0104 010a  ................
-00001e50: 0102 fc10 070c 0204 0120 0104 fe04 0502  ......... ......
-00001e60: 0102 0106 0102 fd08 0672 6a00 0000 2913  .........rj...).
-00001e70: da07 5f5f 646f 635f 5fda 0a74 656e 736f  ..__doc__..tenso
-00001e80: 7266 6c6f 7772 0700 0000 da09 6765 6e65  rflowr......gene
-00001e90: 7261 746f 7272 0300 0000 720e 0000 0072  ratorr....r....r
-00001ea0: 1200 0000 7219 0000 0072 2500 0000 7235  ....r....r%...r5
-00001eb0: 0000 0072 4800 0000 724a 0000 0072 4c00  ...rH...rJ...rL.
-00001ec0: 0000 7251 0000 0072 5400 0000 7256 0000  ..rQ...rT...rV..
-00001ed0: 0072 5900 0000 7265 0000 0072 6a00 0000  .rY...re...rj...
-00001ee0: 720c 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
-00001ef0: 0d00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00001f00: 0000 7326 0000 0004 0308 020c 0308 0908  ..s&............
-00001f10: 0a08 070e 2d10 1b10 4e10 1510 2f10 1002  ....-...N.../...
-00001f20: 0002 0002 ff0c 1b0e 1f0e 1f08 0a         .............
+00000b70: 6b05 4d00 7d07 7400 a007 7c07 6400 6701  k.M.}.t...|.d.g.
+00000b80: a102 7d07 6403 7c00 6b06 9001 72f4 7400  ..}.d.|.k...r.t.
+00000b90: a008 7c08 7c07 a102 7c00 6403 3c00 6408  ..|.|...|.d.<.d.
+00000ba0: 7c00 6b06 9003 7220 7400 a008 7c00 6408  |.k...r t...|.d.
+00000bb0: 1900 7c07 a102 7d0c 7400 a008 7c09 7c07  ..|...}.t...|.|.
+00000bc0: a102 7c00 6408 3c00 640b 7c00 6b06 9003  ..|.d.<.d.|.k...
+00000bd0: 7220 7c00 640b 1900 6a09 6407 640a 8502  r |.d...j.d.d...
+00000be0: 1900 7d0d 7c0c 6400 6400 8502 6404 6602  ..}.|.d.d...d.f.
+00000bf0: 1900 7400 a001 7c01 7c0c 6a0a a102 1800  ..t...|.|.j.....
+00000c00: 7d0e 7c0c 6400 6400 8502 6407 6602 1900  }.|.d.d...d.f...
+00000c10: 7400 a001 7c02 7c0c 6a0a a102 1800 7d0f  t...|.|.j.....}.
+00000c20: 7c0c 6400 6400 8502 6409 6602 1900 7c0c  |.d.d...d.f...|.
+00000c30: 6400 6400 8502 6404 6602 1900 1800 7d10  d.d...d.f.....}.
+00000c40: 7c0c 6400 6400 8502 640a 6602 1900 7c0c  |.d.d...d.f...|.
+00000c50: 6400 6400 8502 6407 6602 1900 1800 7d11  d.d...d.f.....}.
+00000c60: 7c00 6408 1900 7400 6a0b 7c0e 7c0f 7c0e  |.d...t.j.|.|.|.
+00000c70: 7c0f 6704 6405 6406 8d02 1800 7d12 7c12  |.g.d.d.....}.|.
+00000c80: 7400 6a0b 7c10 7c11 7c10 7c11 6704 6405  t.j.|.|.|.|.g.d.
+00000c90: 6406 8d02 1b00 7d12 7c12 7400 a001 7c0d  d.....}.|.t...|.
+00000ca0: 7c0d 1700 7c12 6a0a a102 1400 7d12 740c  |...|.j.....}.t.
+00000cb0: 7400 a008 7c00 640b 1900 7c07 a102 7c12  t...|.d...|...|.
+00000cc0: 7c0d 8303 7c00 640b 3c00 7c00 5300 290c  |...|.d.<.|.S.).
+00000cd0: 4e72 1c00 0000 721e 0000 0072 0400 0000  Nr....r....r....
+00000ce0: 7201 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
+00000cf0: 0200 0000 7206 0000 00e9 0200 0000 e903  ....r...........
+00000d00: 0000 00da 056d 6173 6b73 290d 7207 0000  .....masks).r...
+00000d10: 0072 2300 0000 7224 0000 0072 0e00 0000  .r#...r$...r....
+00000d20: da0a 7265 6475 6365 5f61 6c6c da07 6d69  ..reduce_all..mi
+00000d30: 6e69 6d75 6dda 076d 6178 696d 756d da0c  nimum..maximum..
+00000d40: 656e 7375 7265 5f73 6861 7065 da0c 626f  ensure_shape..bo
+00000d50: 6f6c 6561 6e5f 6d61 736b 7215 0000 0072  olean_maskr....r
+00000d60: 0500 0000 da05 7374 6163 6b72 0300 0000  ......stackr....
+00000d70: 2913 720b 0000 00da 0279 30da 0278 30da  ).r......y0..x0.
+00000d80: 0279 31da 0278 315a 0572 6f69 5f68 5a05  .y1..x1Z.roi_hZ.
+00000d90: 726f 695f 7772 3d00 0000 5a05 6374 7264  roi_wr=...Z.ctrd
+00000da0: 7372 0600 0000 5a05 6172 6561 735a 096e  sr....Z.areasZ.n
+00000db0: 6577 5f61 7265 6173 5a0b 6f72 6967 5f62  ew_areasZ.orig_b
+00000dc0: 626f 7865 73da 0c74 6172 6765 745f 7368  boxes..target_sh
+00000dd0: 6170 655a 076f 7269 675f 7930 5a07 6f72  apeZ.orig_y0Z.or
+00000de0: 6967 5f78 305a 066f 7269 675f 685a 066f  ig_x0Z.orig_hZ.o
+00000df0: 7269 675f 775a 086e 6577 5f62 626f 78a9  rig_wZ.new_bbox.
+00000e00: 0272 3500 0000 da03 726f 6972 0c00 0000  .r5.....roir....
+00000e10: 720d 0000 00da 0c5f 6372 6f70 5f74 6f5f  r......_crop_to_
+00000e20: 726f 696e 0000 0073 7400 0000 0001 0c01  roin...st.......
+00000e30: 1201 1202 2202 0801 1c02 0802 0801 0402  ...."...........
+00000e40: 0801 1a01 0201 1001 12ff 0202 12fe 02ff  ................
+00000e50: 0406 0a01 1e01 4002 0401 0200 14ff 0403  ......@.........
+00000e60: 0c01 4002 1003 0e02 0a01 1002 0a01 1001  ..@.............
+00000e70: 1002 0a01 1202 1e01 1e01 2001 2002 0a01  .......... . ...
+00000e80: 0a00 02ff 0803 0601 0a00 02ff 0803 0601  ................
+00000e90: 0600 04ff 0604 0201 0e01 0201 02fd 0806  ................
+00000ea0: 7a21 6372 6f70 5f74 6f5f 726f 692e 3c6c  z!crop_to_roi.<l
+00000eb0: 6f63 616c 733e 2e5f 6372 6f70 5f74 6f5f  ocals>._crop_to_
+00000ec0: 726f 6972 1a00 0000 4e72 2c00 0000 2905  roir....Nr,...).
+00000ed0: 720b 0000 0072 4500 0000 7235 0000 0072  r....rE...r5...r
+00000ee0: 1b00 0000 7246 0000 0072 0c00 0000 7244  ....rF...r....rD
+00000ef0: 0000 0072 0d00 0000 da0b 6372 6f70 5f74  ...r......crop_t
+00000f00: 6f5f 726f 696b 0000 0073 0800 0000 0003  o_roik...s......
+00000f10: 0e47 1801 0403 7247 0000 0063 0100 0000  .G....rG...c....
+00000f20: 0000 0000 0300 0000 0a00 0000 0700 0000  ................
+00000f30: 4300 0000 739e 0000 0074 007c 0064 0119  C...s....t.|.d..
+00000f40: 0083 015c 027d 047d 0574 017c 0183 015c  ...\.}.}.t.|...\
+00000f50: 027d 067d 077c 0364 026b 0072 3874 026a  .}.}.|.d.k.r8t.j
+00000f60: 03a0 0467 00a1 017c 036b 0572 387c 0053  ...g...|.k.r8|.S
+00000f70: 0074 0574 026a 03a0 0467 00a1 0174 02a0  .t.t.j...g...t..
+00000f80: 067c 047c 0618 0074 026a 07a1 0214 0083  .|.|...t.j......
+00000f90: 017d 0874 0574 026a 03a0 0467 00a1 0174  .}.t.t.j...g...t
+00000fa0: 02a0 067c 057c 0718 0074 026a 07a1 0214  ...|.|...t.j....
+00000fb0: 0083 017d 0974 087c 007c 087c 097c 087c  ...}.t.|.|.|.|.|
+00000fc0: 0617 007c 097c 0717 0066 047c 0264 038d  ...|.|...f.|.d..
+00000fd0: 0353 0064 0453 0029 057a 2052 616e 646f  .S.d.S.).z Rando
+00000fe0: 6d20 6372 6f70 2074 6f20 6120 7365 7420  m crop to a set 
+00000ff0: 7461 7267 6574 2073 697a 6572 1c00 0000  target sizer....
+00001000: 721a 0000 0029 0272 4500 0000 7235 0000  r....).rE...r5..
+00001010: 004e 2909 7219 0000 0072 1200 0000 7207  .N).r....r....r.
+00001020: 0000 0072 2d00 0000 722e 0000 00da 0369  ...r-...r......i
+00001030: 6e74 7223 0000 0072 2400 0000 7247 0000  ntr#...r$...rG..
+00001040: 0029 0a72 0b00 0000 722a 0000 0072 3500  .).r....r*...r5.
+00001050: 0000 721b 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00001060: 0072 3200 0000 7233 0000 0072 3f00 0000  .r2...r3...r?...
+00001070: 7240 0000 0072 0c00 0000 720c 0000 0072  r@...r....r....r
+00001080: 0d00 0000 da0b 7261 6e64 6f6d 5f63 726f  ......random_cro
+00001090: 70bc 0000 0073 1600 0000 0003 1002 0c02  p....s..........
+000010a0: 1801 0403 2201 2202 0201 0201 1201 02fd  ....".".........
+000010b0: 7249 0000 0029 02da 0f63 6f6e 7374 616e  rI...)...constan
+000010c0: 745f 7661 6c75 6573 721b 0000 0063 0100  t_valuesr....c..
+000010d0: 0000 0000 0000 0300 0000 0500 0000 0300  ................
+000010e0: 0000 0300 0000 7336 0000 0087 0087 0166  ......s6.......f
+000010f0: 0264 0164 0284 087d 047c 0364 036b 0072  .d.d...}.|.d.k.r
+00001100: 2a74 006a 01a0 0267 00a1 017c 036b 0572  *t.j...g...|.k.r
+00001110: 2a7c 0053 007c 047c 0083 0153 0064 0453  *|.S.|.|...S.d.S
+00001120: 0029 057a 1550 6164 2069 6d61 6765 2061  .).z.Pad image a
+00001130: 6e64 206c 6162 656c 732e 6301 0000 0000  nd labels.c.....
+00001140: 0000 0000 0000 0009 0000 0009 0000 0013  ................
+00001150: 0000 0073 0001 0000 7400 8801 8301 5c02  ...s....t.....\.
+00001160: 7d01 7d02 7400 7c01 8301 5c02 7d03 7d04  }.}.t.|...\.}.}.
+00001170: 7400 7c02 8301 5c02 7d05 7d06 7401 6a02  t.|...\.}.}.t.j.
+00001180: 7c00 6401 1900 7c03 7c04 6702 7c05 7c06  |.d...|.|.g.|.|.
+00001190: 6702 6402 6402 6702 6703 8800 6403 8d03  g.d.d.g.g...d...
+000011a0: 7c00 6401 3c00 6404 7c00 6b06 72ac 7c00  |.d.<.d.|.k.r.|.
+000011b0: 6404 1900 7d07 7403 7c07 6a04 8301 6405  d...}.t.|.j...d.
+000011c0: 6b02 727e 7c03 7c04 6702 7c05 7c06 6702  k.r~|.|.g.|.|.g.
+000011d0: 6702 7d08 6e16 6402 6402 6702 7c03 7c04  g.}.n.d.d.g.|.|.
+000011e0: 6702 7c05 7c06 6702 6703 7d08 7401 6a02  g.|.|.g.g.}.t.j.
+000011f0: 7c00 6404 1900 7c08 8800 6403 8d03 7c00  |.d...|...d...|.
+00001200: 6404 3c00 6406 7c00 6b06 72d2 7c00 6406  d.<.d.|.k.r.|.d.
+00001210: 0500 1900 7401 a005 7c03 7c05 6702 7401  ....t...|.|.g.t.
+00001220: 6a06 a102 3700 0300 3c00 6407 7c00 6b06  j...7...<.d.|.k.
+00001230: 72fc 7c00 6407 0500 1900 7401 a005 7c03  r.|.d.....t...|.
+00001240: 7c05 7c03 7c05 6704 7401 6a06 a102 3700  |.|.|.g.t.j...7.
+00001250: 0300 3c00 7c00 5300 2908 4e72 1c00 0000  ..<.|.S.).Nr....
+00001260: 7201 0000 0029 0172 4a00 0000 721e 0000  r....).rJ...r...
+00001270: 0072 3600 0000 7204 0000 0072 0600 0000  .r6...r....r....
+00001280: 2907 7212 0000 0072 0700 0000 da03 7061  ).r....r......pa
+00001290: 6472 0900 0000 7215 0000 0072 2300 0000  dr....r....r#...
+000012a0: 7224 0000 0029 0972 0b00 0000 5a09 7061  r$...).r....Z.pa
+000012b0: 6464 696e 675f 795a 0970 6164 6469 6e67  dding_yZ.padding
+000012c0: 5f78 5a0a 7061 6464 696e 675f 7930 5a0a  _xZ.padding_y0Z.
+000012d0: 7061 6464 696e 675f 7931 5a0a 7061 6464  padding_y1Z.padd
+000012e0: 696e 675f 7830 5a0a 7061 6464 696e 675f  ing_x0Z.padding_
+000012f0: 7831 721e 0000 00da 0e70 6164 6469 6e67  x1r......padding
+00001300: 5f76 616c 7565 73a9 0272 4a00 0000 da08  _values..rJ.....
+00001310: 7061 6464 696e 6773 720c 0000 0072 0d00  paddingsr....r..
+00001320: 0000 da04 5f70 6164 d400 0000 733a 0000  ...._pad....s:..
+00001330: 0000 010c 010c 010c 0204 0106 0114 0102  ................
+00001340: fd0a 0608 0108 010e 0112 0306 0106 0106  ................
+00001350: fd04 0504 0106 0102 0102 fd0a 0608 011e  ................
+00001360: 0208 010c 010a 0004 ff08 047a 1170 6164  ...........z.pad
+00001370: 2e3c 6c6f 6361 6c73 3e2e 5f70 6164 721a  .<locals>._padr.
+00001380: 0000 004e 722c 0000 0029 0572 0b00 0000  ...Nr,...).r....
+00001390: 724e 0000 0072 4a00 0000 721b 0000 0072  rN...rJ...r....r
+000013a0: 4f00 0000 720c 0000 0072 4d00 0000 720d  O...r....rM...r.
+000013b0: 0000 0072 4b00 0000 d100 0000 7308 0000  ...rK.......s...
+000013c0: 0000 030e 2518 0104 0372 4b00 0000 6301  ....%....rK...c.
+000013d0: 0000 0000 0000 0003 0000 000a 0000 0005  ................
+000013e0: 0000 0043 0000 0073 8200 0000 7c03 6401  ...C...s....|.d.
+000013f0: 6b00 721c 7400 6a01 a002 6700 a101 7c03  k.r.t.j...g...|.
+00001400: 6b05 721c 7c00 5300 7403 7c00 6402 1900  k.r.|.S.t.|.d...
+00001410: 8301 5c02 7d04 7d05 7404 7c01 8301 5c02  ..\.}.}.t.|...\.
+00001420: 7d06 7d07 7c06 7c04 1800 7d08 7c08 6403  }.}.|.|...}.|.d.
+00001430: 1a00 7c08 7c08 6403 1a00 1800 6702 7d08  ..|.|.d.....g.}.
+00001440: 7c07 7c05 1800 7d09 7c09 6403 1a00 7c09  |.|...}.|.d...|.
+00001450: 7c09 6403 1a00 1800 6702 7d09 7405 7c00  |.d.....g.}.t.|.
+00001460: 7c08 7c09 6702 7c02 6404 8d03 5300 2905  |.|.g.|.d...S.).
+00001470: 4e72 1a00 0000 721c 0000 0072 3600 0000  Nr....r....r6...
+00001480: 2902 724e 0000 0072 4a00 0000 2906 7207  ).rN...rJ...).r.
+00001490: 0000 0072 2d00 0000 722e 0000 0072 1900  ...r-...r....r..
+000014a0: 0000 7212 0000 0072 4b00 0000 290a 720b  ..r....rK...).r.
+000014b0: 0000 0072 2a00 0000 724a 0000 0072 1b00  ...r*...rJ...r..
+000014c0: 0000 7217 0000 0072 1800 0000 7232 0000  ..r....r....r2..
+000014d0: 0072 3300 0000 5a09 7061 6464 696e 675f  .r3...Z.padding_
+000014e0: 685a 0970 6164 6469 6e67 5f77 720c 0000  hZ.padding_wr...
+000014f0: 0072 0c00 0000 720d 0000 00da 0b70 6164  .r....r......pad
+00001500: 5f74 6f5f 7369 7a65 0001 0000 7312 0000  _to_size....s...
+00001510: 0000 0118 0104 0210 010c 0208 0114 0108  ................
+00001520: 0114 0272 5000 0000 2903 724a 0000 0072  ...rP...).rJ...r
+00001530: 3500 0000 721b 0000 0063 0100 0000 0000  5...r....c......
+00001540: 0000 0400 0000 0b00 0000 0600 0000 4300  ..............C.
+00001550: 0000 738c 0000 007c 0464 016b 0072 1c74  ..s....|.d.k.r.t
+00001560: 006a 01a0 0267 00a1 017c 046b 0572 1c7c  .j...g...|.k.r.|
+00001570: 0053 0074 037c 0064 0219 0083 015c 027d  .S.t.|.d.....\.}
+00001580: 057d 0674 047c 0183 015c 027d 077d 0874  .}.t.|...\.}.}.t
+00001590: 00a0 0574 00a0 067c 057c 07a1 027c 056a  ...t...|.|...|.j
+000015a0: 07a1 027d 0974 00a0 0574 00a0 067c 067c  ...}.t...t...|.|
+000015b0: 08a1 027c 066a 07a1 027d 0a74 087c 007c  ...|.j...}.t.|.|
+000015c0: 097c 0a66 027c 0264 038d 037d 0074 097c  .|.f.|.d...}.t.|
+000015d0: 007c 017c 0364 048d 037d 007c 0053 0064  .|.|.d...}.|.S.d
+000015e0: 0553 0029 067a 2752 616e 646f 6d20 6372  .S.).z'Random cr
+000015f0: 6f70 206f 7220 7061 6420 696d 6167 6520  op or pad image 
+00001600: 746f 2074 6172 6765 745f 7369 7a65 721a  to target_sizer.
+00001610: 0000 0072 1c00 0000 2902 722a 0000 0072  ...r....).r*...r
+00001620: 4a00 0000 2902 722a 0000 0072 3500 0000  J...).r*...r5...
+00001630: 4e29 0a72 0700 0000 722d 0000 0072 2e00  N).r....r-...r..
+00001640: 0000 7219 0000 0072 1200 0000 7223 0000  ..r....r....r#..
+00001650: 0072 3b00 0000 7205 0000 0072 5000 0000  .r;...r....rP...
+00001660: 7249 0000 0029 0b72 0b00 0000 722a 0000  rI...).r....r*..
+00001670: 0072 4a00 0000 7235 0000 0072 1b00 0000  .rJ...r5...r....
+00001680: 7217 0000 0072 1800 0000 7232 0000 0072  r....r....r2...r
+00001690: 3300 0000 da01 68da 0177 720c 0000 0072  3.....h..wr....r
+000016a0: 0c00 0000 720d 0000 00da 1272 616e 646f  ....r......rando
+000016b0: 6d5f 6372 6f70 5f6f 725f 7061 640f 0100  m_crop_or_pad...
+000016c0: 0073 2200 0000 0005 1801 0403 1002 0c02  .s".............
+000016d0: 1601 1602 0201 0200 0600 02ff 0604 0201  ................
+000016e0: 0200 0200 02ff 0604 7253 0000 0063 0100  ........rS...c..
+000016f0: 0000 0000 0000 0100 0000 0300 0000 0300  ................
+00001700: 0000 4300 0000 7330 0000 0064 0164 0284  ..C...s0...d.d..
+00001710: 007d 027c 0164 036b 0072 2474 006a 01a0  .}.|.d.k.r$t.j..
+00001720: 0267 00a1 017c 016b 0572 247c 0053 007c  .g...|.k.r$|.S.|
+00001730: 027c 0083 0153 0064 0053 0029 044e 6301  .|...S.d.S.).Nc.
+00001740: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+00001750: 0000 0053 0000 0073 a600 0000 7400 7c00  ...S...s....t.|.
+00001760: 6401 1900 8301 5c02 7d01 7d02 7401 6a02  d.....\.}.}.t.j.
+00001770: a003 7c00 6401 1900 a101 7c00 6401 3c00  ..|.d.....|.d.<.
+00001780: 6402 7c00 6b06 7252 7c00 6402 1900 6403  d.|.k.rR|.d...d.
+00001790: 1900 7d03 7401 6a04 7401 6a02 a003 7c03  ..}.t.j.t.j...|.
+000017a0: a101 6404 6405 8d02 7c00 6402 3c00 6406  ..d.d...|.d.<.d.
+000017b0: 7c00 6b06 7276 7c00 6406 1900 6407 6404  |.k.rv|.d...d.d.
+000017c0: 6702 1400 6408 7c02 6702 1700 7c00 6406  g...d.|.g...|.d.
+000017d0: 3c00 6409 7c00 6b06 72a2 7c00 6409 1900  <.d.|.k.r.|.d...
+000017e0: 6407 6404 6407 6404 6704 1400 6408 7c02  d.d.d.d.g...d.|.
+000017f0: 6408 7c02 6704 1700 7c00 6409 3c00 7c00  d.|.g...|.d.<.|.
+00001800: 5300 a90a 4e72 1c00 0000 721e 0000 0072  S...Nr....r....r
+00001810: 1f00 0000 7220 0000 0072 2100 0000 7204  ....r ...r!...r.
+00001820: 0000 0072 0200 0000 7201 0000 0072 0600  ...r....r....r..
+00001830: 0000 2905 7219 0000 0072 0700 0000 721c  ..).r....r....r.
+00001840: 0000 00da 0f66 6c69 705f 6c65 6674 5f72  .....flip_left_r
+00001850: 6967 6874 7226 0000 00a9 0472 0b00 0000  ightr&.....r....
+00001860: 7217 0000 0072 1800 0000 721e 0000 0072  r....r....r....r
+00001870: 0c00 0000 720c 0000 0072 0d00 0000 da10  ....r....r......
+00001880: 5f66 6c69 705f 6c65 6674 5f72 6967 6874  _flip_left_right
+00001890: 2b01 0000 731a 0000 0000 0110 0214 0208  +...s...........
+000018a0: 010c 0104 010a 0102 fe0a 0508 011c 0208  ................
+000018b0: 0124 057a 2966 6c69 705f 6c65 6674 5f72  .$.z)flip_left_r
+000018c0: 6967 6874 2e3c 6c6f 6361 6c73 3e2e 5f66  ight.<locals>._f
+000018d0: 6c69 705f 6c65 6674 5f72 6967 6874 721a  lip_left_rightr.
+000018e0: 0000 0072 2c00 0000 2903 720b 0000 0072  ...r,...).r....r
+000018f0: 1b00 0000 7257 0000 0072 0c00 0000 720c  ....rW...r....r.
+00001900: 0000 0072 0d00 0000 7255 0000 002a 0100  ...r....rU...*..
+00001910: 0073 0800 0000 0001 0817 1801 0403 7255  .s............rU
+00001920: 0000 0063 0100 0000 0000 0000 0100 0000  ...c............
+00001930: 0300 0000 0300 0000 4300 0000 7330 0000  ........C...s0..
+00001940: 0064 0164 0284 007d 027c 0164 036b 0072  .d.d...}.|.d.k.r
+00001950: 2474 006a 01a0 0267 00a1 017c 016b 0572  $t.j...g...|.k.r
+00001960: 247c 0053 007c 027c 0083 0153 0064 0053  $|.S.|.|...S.d.S
+00001970: 0029 044e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00001980: 0004 0000 0005 0000 0053 0000 0073 a600  .........S...s..
+00001990: 0000 7400 7c00 6401 1900 8301 5c02 7d01  ..t.|.d.....\.}.
+000019a0: 7d02 7401 6a02 a003 7c00 6401 1900 a101  }.t.j...|.d.....
+000019b0: 7c00 6401 3c00 6402 7c00 6b06 7252 7c00  |.d.<.d.|.k.rR|.
+000019c0: 6402 1900 6403 1900 7d03 7401 6a04 7401  d...d...}.t.j.t.
+000019d0: 6a02 a003 7c03 a101 6404 6405 8d02 7c00  j...|...d.d...|.
+000019e0: 6402 3c00 6406 7c00 6b06 7276 7c00 6406  d.<.d.|.k.rv|.d.
+000019f0: 1900 6404 6407 6702 1400 7c01 6408 6702  ..d.d.g...|.d.g.
+00001a00: 1700 7c00 6406 3c00 6409 7c00 6b06 72a2  ..|.d.<.d.|.k.r.
+00001a10: 7c00 6409 1900 6404 6407 6404 6407 6704  |.d...d.d.d.d.g.
+00001a20: 1400 7c01 6408 7c01 6408 6704 1700 7c00  ..|.d.|.d.g...|.
+00001a30: 6409 3c00 7c00 5300 7254 0000 0029 0572  d.<.|.S.rT...).r
+00001a40: 1900 0000 7207 0000 0072 1c00 0000 da0c  ....r....r......
+00001a50: 666c 6970 5f75 705f 646f 776e 7226 0000  flip_up_downr&..
+00001a60: 0072 5600 0000 720c 0000 0072 0c00 0000  .rV...r....r....
+00001a70: 720d 0000 00da 0d5f 666c 6970 5f75 705f  r......_flip_up_
+00001a80: 646f 776e 4a01 0000 731a 0000 0000 0110  downJ...s.......
+00001a90: 0214 0208 010c 0104 010a 0102 fe0a 0508  ................
+00001aa0: 011c 0208 0124 057a 2366 6c69 705f 7570  .....$.z#flip_up
+00001ab0: 5f64 6f77 6e2e 3c6c 6f63 616c 733e 2e5f  _down.<locals>._
+00001ac0: 666c 6970 5f75 705f 646f 776e 721a 0000  flip_up_downr...
+00001ad0: 0072 2c00 0000 2903 720b 0000 0072 1b00  .r,...).r....r..
+00001ae0: 0000 7259 0000 0072 0c00 0000 720c 0000  ..rY...r....r...
+00001af0: 0072 0d00 0000 7258 0000 0049 0100 0073  .r....rX...I...s
+00001b00: 0800 0000 0001 0817 1801 0403 7258 0000  ............rX..
+00001b10: 0063 0100 0000 0000 0000 0000 0000 0500  .c..............
+00001b20: 0000 0500 0000 4300 0000 734c 0000 0064  ......C...sL...d
+00001b30: 0164 006c 007d 0164 0164 026c 016d 027d  .d.l.}.d.d.l.m.}
+00001b40: 0201 007c 01a0 0364 0364 0484 007c 027c  ...|...d.d...|.|
+00001b50: 0083 0144 0083 01a1 017d 037c 01a0 0364  ...D.....}.|...d
+00001b60: 0564 0484 007c 027c 0083 0144 0083 01a1  .d...|.|...D....
+00001b70: 017d 047c 037c 0466 0253 0029 064e 7201  .}.|.|.f.S.).Nr.
+00001b80: 0000 0029 01da 0b72 6567 696f 6e70 726f  ...)...regionpro
+00001b90: 7073 6301 0000 0000 0000 0000 0000 0002  psc.............
+00001ba0: 0000 0004 0000 0053 0000 0073 1400 0000  .......S...s....
+00001bb0: 6700 7c00 5d0c 7d01 7c01 6400 1900 9102  g.|.].}.|.d.....
+00001bc0: 7104 5300 2901 da04 6262 6f78 720c 0000  q.S.)...bboxr...
+00001bd0: 00a9 02da 022e 30da 0172 720c 0000 0072  ......0..rr....r
+00001be0: 0c00 0000 720d 0000 00da 0a3c 6c69 7374  ....r......<list
+00001bf0: 636f 6d70 3e6c 0100 0073 0400 0000 0600  comp>l...s......
+00001c00: 0200 7a24 5f62 626f 785f 6672 6f6d 5f6c  ..z$_bbox_from_l
+00001c10: 6162 656c 2e3c 6c6f 6361 6c73 3e2e 3c6c  abel.<locals>.<l
+00001c20: 6973 7463 6f6d 703e 6301 0000 0000 0000  istcomp>c.......
+00001c30: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00001c40: 0073 1400 0000 6700 7c00 5d0c 7d01 7c01  .s....g.|.].}.|.
+00001c50: 6400 1900 9102 7104 5300 2901 7204 0000  d.....q.S.).r...
+00001c60: 0072 0c00 0000 725c 0000 0072 0c00 0000  .r....r\...r....
+00001c70: 720c 0000 0072 0d00 0000 725f 0000 006d  r....r....r_...m
+00001c80: 0100 0073 0400 0000 0600 0200 2904 da05  ...s........)...
+00001c90: 6e75 6d70 795a 0f73 6b69 6d61 6765 2e6d  numpyZ.skimage.m
+00001ca0: 6561 7375 7265 725a 0000 00da 0761 7361  easurerZ.....asa
+00001cb0: 7272 6179 2905 da05 6c61 6265 6cda 026e  rray)...label..n
+00001cc0: 7072 5a00 0000 7206 0000 0072 0400 0000  prZ...r....r....
+00001cd0: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00001ce0: 105f 6262 6f78 5f66 726f 6d5f 6c61 6265  ._bbox_from_labe
+00001cf0: 6c68 0100 0073 0a00 0000 0001 0801 0c02  lh...s..........
+00001d00: 1801 1802 7264 0000 00e9 3000 0000 2901  ....rd....0...).
+00001d10: da0a 6d61 736b 5f73 6861 7065 6301 0000  ..mask_shapec...
+00001d20: 0000 0000 0001 0000 0005 0000 0008 0000  ................
+00001d30: 0043 0000 0073 8e00 0000 7c00 6401 1900  .C...s....|.d...
+00001d40: 7d02 6402 7c00 6b07 7318 6403 7c00 6b07  }.d.|.k.s.d.|.k.
+00001d50: 723e 7400 a001 7402 7c02 6701 7400 6a03  r>t...t.|.g.t.j.
+00001d60: 7400 6a03 6702 6404 a104 5c02 7c00 6402  t.j.g.d...\.|.d.
+00001d70: 3c00 7c00 6403 3c00 7404 7c00 6402 1900  <.|.d.<.t.|.d...
+00001d80: 8301 7d03 7400 a005 7c02 7400 a006 6405  ..}.t...|.t...d.
+00001d90: 7c03 6405 1700 a102 6400 6400 8502 6400  |.d.....d.d...d.
+00001da0: 6400 6603 1900 6b02 7400 6a07 a102 7d04  d.f...k.t.j...}.
+00001db0: 7408 7c04 7c00 6402 1900 7c01 8303 7c00  t.|.|.d...|...|.
+00001dc0: 6406 3c00 7c00 5300 2907 4e72 6200 0000  d.<.|.S.).Nrb...
+00001dd0: 7206 0000 0072 0400 0000 4672 0200 0000  r....r....Fr....
+00001de0: 7238 0000 0029 0972 0700 0000 5a0a 6e75  r8...).r....Z.nu
+00001df0: 6d70 795f 6675 6e63 7264 0000 0072 2400  mpy_funcrd...r$.
+00001e00: 0000 7209 0000 0072 2300 0000 da05 7261  ..r....r#.....ra
+00001e10: 6e67 65da 0569 6e74 3332 7203 0000 0029  nge..int32r....)
+00001e20: 0572 0b00 0000 7266 0000 0072 6200 0000  .r....rf...rb...
+00001e30: 5a0b 6e5f 696e 7374 616e 6365 735a 0e6c  Z.n_instancesZ.l
+00001e40: 6162 656c 5f65 7870 616e 6465 6472 0c00  abel_expandedr..
+00001e50: 0000 720c 0000 0072 0d00 0000 da0f 6d61  ..r....r......ma
+00001e60: 736b 5f66 726f 6d5f 6c61 6265 6c72 0100  sk_from_labelr..
+00001e70: 0073 2600 0000 0001 0802 1001 0401 0201  .s&.............
+00001e80: 0401 0a01 02fc 1007 0c02 0401 2001 04fe  ............ ...
+00001e90: 0405 0201 0201 0601 02fd 0806 7269 0000  ............ri..
+00001ea0: 0029 13da 075f 5f64 6f63 5f5f da0a 7465  .)...__doc__..te
+00001eb0: 6e73 6f72 666c 6f77 7207 0000 00da 0967  nsorflowr......g
+00001ec0: 656e 6572 6174 6f72 7203 0000 0072 0e00  eneratorr....r..
+00001ed0: 0000 7212 0000 0072 1900 0000 7225 0000  ..r....r....r%..
+00001ee0: 0072 3400 0000 7247 0000 0072 4900 0000  .r4...rG...rI...
+00001ef0: 724b 0000 0072 5000 0000 7253 0000 0072  rK...rP...rS...r
+00001f00: 5500 0000 7258 0000 0072 6400 0000 7269  U...rX...rd...ri
+00001f10: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
+00001f20: 0000 720d 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00001f30: 3e01 0000 0073 2600 0000 0403 0802 0c03  >....s&.........
+00001f40: 0809 080a 0807 0e2d 101b 1051 1015 102f  .......-...Q.../
+00001f50: 1010 0200 0200 02ff 0c1b 0e1f 0e1f 080a  ................
```

### Comparing `lacss-0.4.1/lacss/data/__pycache__/parser.cpython-38.pyc` & `lacss-0.4.2/lacss/data/__pycache__/parser.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun 27 16:22:07 2023 UTC, .py size: 9160 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 af0c 9b64 c823 0000  U..........d.#..
+00000000: 550d 0d0a 0000 0000 c375 a864 c823 0000  U........u.d.#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 8400 5a04 6412 6407 6408 8401 5a05  d...Z.d.d.d...Z.
 00000050: 6413 6409 640a 8401 5a06 6414 640c 640d  d.d.d...Z.d.d.d.
 00000060: 8401 5a07 640e 640f 8400 5a08 6415 6410  ..Z.d.d...Z.d.d.
 00000070: 6411 8401 5a09 6401 5300 2916 e900 0000  d...Z.d.S.).....
@@ -98,29 +98,29 @@
 00000610: 3332 da05 7a65 726f 73da 1874 656e 736f  32..zeros..tenso
 00000620: 725f 7363 6174 7465 725f 6e64 5f75 7064  r_scatter_nd_upd
 00000630: 6174 65da 0974 7261 6e73 706f 7365 2911  ate..transpose).
 00000640: da04 6461 7461 da07 6175 676d 656e 745a  ..data..augmentZ
 00000650: 0d6d 696e 5f6d 6173 6b5f 6172 6561 720d  .min_mask_arear.
 00000660: 0000 0072 0e00 0000 7209 0000 00da 056d  ...r....r......m
 00000670: 6173 6b73 5a0c 6d61 736b 5f72 6f77 5f69  asksZ.mask_row_i
-00000680: 6473 da0b 6d61 736b 5f76 616c 7565 7372  ds..mask_valuesr
+00000680: 6473 5a0b 6d61 736b 5f76 616c 7565 7372  dsZ.mask_valuesr
 00000690: 1200 0000 7213 0000 005a 0a76 616c 6964  ....r....Z.valid
 000006a0: 5f72 6f77 735a 106d 6173 6b5f 726f 775f  _rowsZ.mask_row_
 000006b0: 6c65 6e67 7468 735a 0b76 616c 6964 5f6d  lengthsZ.valid_m
 000006c0: 6173 6b73 721c 0000 00da 0772 6f77 5f69  asksr......row_i
 000006d0: 6473 da06 6c61 6265 6c73 7203 0000 0072  ds..labelsr....r
 000006e0: 0300 0000 7214 0000 00da 2570 6172 7365  ....r.....%parse
 000006f0: 5f74 7261 696e 5f64 6174 615f 6675 6e63  _train_data_func
 00000700: 5f66 756c 6c5f 616e 6e6f 7461 7469 6f6e  _full_annotation
 00000710: 1d00 0000 734c 0000 0000 0308 0108 0108  ....sL..........
 00000720: 0106 0208 0108 0212 0116 0104 0110 010c  ................
 00000730: 0118 0110 010c 0118 0204 012a 012a fe04  ...........*.*..
 00000740: 040c 010c 010e 0108 0108 010e 0218 020c  ................
 00000750: 0112 0110 0210 0112 010c 0112 010a 0302  ................
-00000760: 0102 0102 fd72 3600 0000 6305 0000 0000  .....r6...c.....
+00000760: 0102 0102 fd72 3500 0000 6305 0000 0000  .....r5...c.....
 00000770: 0000 0000 0000 000f 0000 0009 0000 0043  ...............C
 00000780: 0000 0073 3e02 0000 7c00 6401 1900 7d05  ...s>...|.d...}.
 00000790: 7400 a001 7c00 6402 1900 6403 a102 7d06  t...|.d...d...}.
 000007a0: 7c00 6404 1900 7d07 7400 a002 7c05 7400  |.d...}.t...|.t.
 000007b0: a003 7c06 7400 6a04 a102 6702 6403 a102  ..|.t.j...g.d...
 000007c0: 7d08 7c02 6400 6b09 72b8 7400 a003 7400  }.|.d.k.r.t...t.
 000007d0: a005 7c08 a101 6405 1900 7400 6a04 a102  ..|...d...t.j...
@@ -157,36 +157,36 @@
 000009c0: 6410 9c03 5300 2911 4e72 0900 0000 da0b  d...S.).Nr......
 000009d0: 6269 6e61 7279 5f6d 6173 6b72 1a00 0000  binary_maskr....
 000009e0: 721c 0000 00e9 fdff ffff e9fe ffff ff72  r..............r
 000009f0: 0100 0000 7202 0000 0054 a901 da09 616e  ....r....T....an
 00000a00: 7469 616c 6961 7372 1900 0000 e700 0000  tialiasr........
 00000a10: 0000 00f0 3fe7 0000 0000 0000 f0bf 2ea9  ....?...........
 00000a20: 022e 721a 0000 0029 0372 0900 0000 721c  ..r....).r....r.
-00000a30: 0000 0072 3700 0000 2911 7204 0000 00da  ...r7...).r.....
+00000a30: 0000 0072 3600 0000 2911 7204 0000 00da  ...r6...).r.....
 00000a40: 0b65 7870 616e 645f 6469 6d73 da06 636f  .expand_dims..co
 00000a50: 6e63 6174 7221 0000 0072 2c00 0000 7205  ncatr!...r,...r.
 00000a60: 0000 0072 0600 0000 7207 0000 0072 0900  ...r....r....r..
 00000a70: 0000 da06 7265 7369 7a65 7220 0000 0072  ....resizer ...r
 00000a80: 1500 0000 7223 0000 0072 2400 0000 722f  ....r#...r$...r/
 00000a90: 0000 0072 2500 0000 7226 0000 0029 0f72  ...r%...r&...).r
 00000aa0: 3000 0000 7231 0000 00da 0b73 697a 655f  0...r1.....size_
 00000ab0: 6a69 7474 6572 720d 0000 0072 0e00 0000  jitterr....r....
-00000ac0: 7209 0000 0072 3700 0000 721c 0000 00da  r....r7...r.....
+00000ac0: 7209 0000 0072 3600 0000 721c 0000 00da  r....r6...r.....
 00000ad0: 0d69 6d67 5f61 6e64 5f6c 6162 656c da01  .img_and_label..
 00000ae0: 68da 0177 da07 7363 616c 696e 6772 1200  h..w..scalingr..
 00000af0: 0000 7213 0000 00da 0869 735f 7661 6c69  ..r......is_vali
 00000b00: 6472 0300 0000 7203 0000 0072 1400 0000  dr....r....r....
 00000b10: da15 7061 7273 655f 7472 6169 6e5f 6461  ..parse_train_da
 00000b20: 7461 5f66 756e 6350 0000 0073 5800 0000  ta_funcP...sX...
 00000b30: 0003 0801 1001 0802 1a01 0801 1801 1801  ................
 00000b40: 1801 0601 0200 1600 02ff 0603 0802 0201  ................
 00000b50: 0200 0200 02ff 0a03 1602 0601 1201 0c01  ................
 00000b60: 1401 1201 0c01 1402 0a01 1201 0c01 1602  ................
 00000b70: 1001 0a01 1802 0803 0401 2e01 2efe 0404  ................
-00000b80: 0c07 0201 0201 02fd 7248 0000 00e9 2000  ........rH.... .
+00000b80: 0c07 0201 0201 02fd 7247 0000 00e9 2000  ........rG.... .
 00000b90: 0000 6302 0000 0000 0000 0000 0000 000e  ..c.............
 00000ba0: 0000 0009 0000 0043 0000 0073 1801 0000  .......C...s....
 00000bb0: 7c00 6401 1900 7d02 7400 a001 7c00 6402  |.d...}.t...|.d.
 00000bc0: 1900 6403 a102 7d03 7c00 6404 1900 7d04  ..d...}.|.d...}.
 00000bd0: 7c00 6405 1900 7d05 7c00 6406 1900 7d06  |.d...}.|.d...}.
 00000be0: 7400 a002 7c02 a101 6407 1900 7d07 7400  t...|...d...}.t.
 00000bf0: a002 7c02 a101 6408 1900 7d08 7c07 6408  ..|...d...}.|.d.
@@ -199,62 +199,62 @@
 00000c60: 7d03 6409 7c00 6b06 72c2 7c00 6409 1900  }.d.|.k.r.|.d...
 00000c70: 6e0c 7400 a008 640a 7400 6a06 a102 7d0b  n.t...d.t.j...}.
 00000c80: 7c06 a009 a100 6408 1700 7d0c 7400 a00a  |.....d...}.t...
 00000c90: 7c09 7c0a 6702 7c0c 6a0b a102 7d0d 7400  |.|.g.|.j...}.t.
 00000ca0: a00c 7c0d 7c06 6a0d 7c0c a103 7d0d 7c02  ..|.|.j.|...}.|.
 00000cb0: 7c04 7c05 7c00 640b 1900 7c0b 7c03 7c06  |.|.|.d...|.|.|.
 00000cc0: 7c0d 640c 9c08 5300 290d 4e72 0900 0000  |.d...S.).Nr....
-00000cd0: 7237 0000 0072 1a00 0000 da06 6262 6f78  r7...r......bbox
+00000cd0: 7236 0000 0072 1a00 0000 da06 6262 6f78  r6...r......bbox
 00000ce0: 6573 721c 0000 0072 1800 0000 7201 0000  esr....r....r...
-00000cf0: 0072 0200 0000 7246 0000 0072 3c00 0000  .r....rF...r<...
+00000cf0: 0072 0200 0000 7245 0000 0072 3b00 0000  .r....rE...r;...
 00000d00: da06 696d 675f 6964 2908 7209 0000 0072  ..img_id).r....r
-00000d10: 4a00 0000 721c 0000 0072 4b00 0000 7246  J...r....rK...rF
-00000d20: 0000 0072 3700 0000 7218 0000 0072 1d00  ...r7...r....r..
-00000d30: 0000 290e 7204 0000 0072 3f00 0000 7205  ..).r....r?...r.
+00000d10: 4900 0000 721c 0000 0072 4a00 0000 7245  I...r....rJ...rE
+00000d20: 0000 0072 3600 0000 7218 0000 0072 1d00  ...r6...r....r..
+00000d30: 0000 290e 7204 0000 0072 3e00 0000 7205  ..).r....r>...r.
 00000d40: 0000 0072 0900 0000 720b 0000 0072 2100  ...r....r....r!.
 00000d50: 0000 722c 0000 00da 0773 7175 6565 7a65  ..r,.....squeeze
 00000d60: da08 636f 6e73 7461 6e74 721e 0000 0072  ..constantr....r
 00000d70: 2d00 0000 7222 0000 0072 2e00 0000 721f  -...r"...r....r.
 00000d80: 0000 0029 0e72 3000 0000 5a0c 6469 6d5f  ...).r0...Z.dim_
-00000d90: 6d75 6c74 6970 6c65 7209 0000 0072 3700  multipler....r7.
-00000da0: 0000 724a 0000 0072 1c00 0000 7232 0000  ..rJ...r....r2..
+00000d90: 6d75 6c74 6970 6c65 7209 0000 0072 3600  multipler....r6.
+00000da0: 0000 7249 0000 0072 1c00 0000 7232 0000  ..rI...r....r2..
 00000db0: 0072 0f00 0000 7210 0000 0072 0d00 0000  .r....r....r....
-00000dc0: 720e 0000 0072 4600 0000 7234 0000 0072  r....rF...r4...r
-00000dd0: 3500 0000 7203 0000 0072 0300 0000 7214  5...r....r....r.
+00000dc0: 720e 0000 0072 4500 0000 7233 0000 0072  r....rE...r3...r
+00000dd0: 3400 0000 7203 0000 0072 0300 0000 7214  4...r....r....r.
 00000de0: 0000 00da 1470 6172 7365 5f74 6573 745f  .....parse_test_
 00000df0: 6461 7461 5f66 756e 638b 0000 0073 3800  data_func....s8.
 00000e00: 0000 0001 0801 1001 0801 0801 0802 0e01  ................
 00000e10: 0e01 1401 1402 1401 0401 1201 04fe 0404  ................
 00000e20: 0c02 1e02 0c01 1201 1003 0201 0201 0201  ................
-00000e30: 0601 0201 0201 0201 02f8 724e 0000 0063  ..........rN...c
+00000e30: 0601 0201 0201 0201 02f8 724d 0000 0063  ..........rM...c
 00000e40: 0100 0000 0000 0000 0000 0000 0400 0000  ................
 00000e50: 0300 0000 4300 0000 732c 0000 0064 0164  ....C...s,...d.d
 00000e60: 026c 006d 017d 0101 007c 017c 0083 017d  .l.m.}...|.|...}
 00000e70: 0264 0364 0484 007c 0244 0083 017d 0374  .d.d...|.D...}.t
 00000e80: 02a0 037c 03a1 0153 0029 054e 7201 0000  ...|...S.).Nr...
 00000e90: 0029 01da 0b72 6567 696f 6e70 726f 7073  .)...regionprops
 00000ea0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
 00000eb0: 0006 0000 0053 0000 0073 1a00 0000 6700  .....S...s....g.
 00000ec0: 7c00 5d12 7d01 7400 a001 7c01 6400 1900  |.].}.t...|.d...
 00000ed0: a101 9102 7104 5300 2901 da08 6365 6e74  ....q.S.)...cent
-00000ee0: 726f 6964 2902 7204 0000 0072 4d00 0000  roid).r....rM...
+00000ee0: 726f 6964 2902 7204 0000 0072 4c00 0000  roid).r....rL...
 00000ef0: 2902 da02 2e30 da02 7270 7203 0000 0072  )....0..rpr....r
 00000f00: 0300 0000 7214 0000 00da 0a3c 6c69 7374  ....r......<list
 00000f10: 636f 6d70 3eb4 0000 0073 0400 0000 0600  comp>....s......
 00000f20: 0200 7a2d 6765 745f 6c6f 6361 7469 6f6e  ..z-get_location
 00000f30: 735f 6672 6f6d 5f6c 6162 656c 732e 3c6c  s_from_labels.<l
 00000f40: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
 00000f50: 3e29 04da 0f73 6b69 6d61 6765 2e6d 6561  >)...skimage.mea
-00000f60: 7375 7265 724f 0000 0072 0400 0000 da05  surerO...r......
-00000f70: 7374 6163 6b29 04da 056c 6162 656c 724f  stack)...labelrO
+00000f60: 7375 7265 724e 0000 0072 0400 0000 da05  surerN...r......
+00000f70: 7374 6163 6b29 04da 056c 6162 656c 724e  stack)...labelrN
 00000f80: 0000 005a 0372 7073 da04 6c6f 6373 7203  ...Z.rps..locsr.
 00000f90: 0000 0072 0300 0000 7214 0000 00da 1967  ...r....r......g
 00000fa0: 6574 5f6c 6f63 6174 696f 6e73 5f66 726f  et_locations_fro
 00000fb0: 6d5f 6c61 6265 6c73 b000 0000 7308 0000  m_labels....s...
-00000fc0: 0000 010c 0208 010e 0272 5800 0000 6304  .........rX...c.
+00000fc0: 0000 010c 0208 010e 0272 5700 0000 6304  .........rW...c.
 00000fd0: 0000 0000 0000 0000 0000 0011 0000 0009  ................
 00000fe0: 0000 0043 0000 0073 2203 0000 7400 7c00  ...C...s"...t.|.
 00000ff0: 7401 8302 7314 7c00 7d04 6900 7d05 6e08  t...s.|.}.i.}.n.
 00001000: 7c00 5c02 7d04 7d05 7402 a003 7c04 6401  |.\.}.}.t...|.d.
 00001010: 1900 6402 a102 7d06 7404 7402 a005 7c06  ..d...}.t.t...|.
 00001020: a101 8301 6403 6b02 7254 7c06 6400 6400  ....d.k.rT|.d.d.
 00001030: 8502 6400 6400 8502 6400 6603 1900 7d06  ..d.d...d.f...}.
@@ -307,50 +307,50 @@
 00001320: e903 0000 00da 0c67 745f 6c6f 6361 7469  .......gt_locati
 00001330: 6f6e 7372 1d00 0000 7a4a 5472 6169 6e69  onsr....zJTraini
 00001340: 6e67 2064 6174 6120 7265 7175 6972 6573  ng data requires
 00001350: 2067 745f 6c6f 6361 7469 6f6e 7320 696e   gt_locations in
 00001360: 2074 6865 2069 6e70 7574 206f 7220 6d61   the input or ma
 00001370: 736b 5f6c 6162 656c 7320 696e 206c 6162  sk_labels in lab
 00001380: 656c 732e da04 6d61 736b 721a 0000 0072  els...maskr....r
-00001390: 3800 0000 7239 0000 0072 0100 0000 7202  8...r9...r....r.
-000013a0: 0000 0054 723a 0000 0072 1900 0000 723c  ...Tr:...r....r<
-000013b0: 0000 0072 3d00 0000 723e 0000 002e 6733  ...r=...r>....g3
+00001390: 3700 0000 7238 0000 0072 0100 0000 7202  7...r8...r....r.
+000013a0: 0000 0054 7239 0000 0072 1900 0000 723b  ...Tr9...r....r;
+000013b0: 0000 0072 3c00 0000 723d 0000 002e 6733  ...r<...r=....g3
 000013c0: 3333 3333 33e3 3f67 6666 6666 6666 f63f  33333.?gffffff.?
 000013d0: 6733 3333 3333 33d3 3f29 18da 0a69 7369  g333333.?)...isi
 000013e0: 6e73 7461 6e63 65da 0574 7570 6c65 7204  nstance..tupler.
 000013f0: 0000 0072 2100 0000 da03 6c65 6e72 0500  ...r!.....lenr..
 00001400: 0000 da0e 4173 7365 7274 696f 6e45 7272  ....AssertionErr
-00001410: 6f72 7258 0000 00da 0a56 616c 7565 4572  orrX.....ValueEr
-00001420: 726f 7272 4000 0000 722c 0000 0072 0600  rorr@...r,...r..
-00001430: 0000 7207 0000 0072 0900 0000 7241 0000  ..r....r....rA..
+00001410: 6f72 7257 0000 00da 0a56 616c 7565 4572  orrW.....ValueEr
+00001420: 726f 7272 3f00 0000 722c 0000 0072 0600  rorr?...r,...r..
+00001430: 0000 7207 0000 0072 0900 0000 7240 0000  ..r....r....r@..
 00001440: 0072 2000 0000 7215 0000 0072 2300 0000  .r ...r....r#...
 00001450: 7224 0000 0072 2f00 0000 7225 0000 0072  r$...r/...r%...r
 00001460: 2600 0000 da0f 7261 6e64 6f6d 5f63 6f6e  &.....random_con
 00001470: 7472 6173 74da 1172 616e 646f 6d5f 6272  trast..random_br
 00001480: 6967 6874 6e65 7373 2911 7230 0000 0072  ightness).r0...r
-00001490: 4200 0000 720d 0000 0072 0e00 0000 da06  B...r....r......
-000014a0: 696e 7075 7473 7235 0000 0072 0900 0000  inputsr5...r....
-000014b0: 725b 0000 0072 5c00 0000 7243 0000 0072  r[...r\...rC...r
-000014c0: 4400 0000 7245 0000 0072 4600 0000 7212  D...rE...rF...r.
-000014d0: 0000 0072 1300 0000 721c 0000 0072 4700  ...r....r....rG.
+00001490: 4100 0000 720d 0000 0072 0e00 0000 da06  A...r....r......
+000014a0: 696e 7075 7473 7234 0000 0072 0900 0000  inputsr4...r....
+000014b0: 725a 0000 0072 5b00 0000 7242 0000 0072  rZ...r[...rB...r
+000014c0: 4300 0000 7244 0000 0072 4500 0000 7212  C...rD...rE...r.
+000014d0: 0000 0072 1300 0000 721c 0000 0072 4600  ...r....r....rF.
 000014e0: 0000 7203 0000 0072 0300 0000 7214 0000  ..r....r....r...
 000014f0: 0072 3100 0000 b900 0000 7378 0000 0000  .r1.......sx....
 00001500: 020a 0104 0106 0208 0210 0212 0116 0216  ................
 00001510: 0208 0112 0108 010e 0202 0102 ff04 0408  ................
 00001520: 0110 0212 0116 0212 0404 020a 0118 0118  ................
 00001530: 0118 0106 0102 0016 0002 ff06 0308 0202  ................
 00001540: 0102 0002 0002 ff0a 0316 0212 010c 0114  ................
 00001550: 0112 010c 0114 021c 010c 0116 0204 012e  ................
 00001560: 012e fe04 040c 020a 011a 0112 0204 0210  ................
 00001570: 010e 0208 0108 0272 3100 0000 2904 5472  .......r1...).Tr
 00001580: 1600 0000 7217 0000 0072 1700 0000 2904  ....r....r....).
-00001590: 544e 7217 0000 0072 1700 0000 2901 7249  TNr....r....).rI
+00001590: 544e 7217 0000 0072 1700 0000 2901 7248  TNr....r....).rH
 000015a0: 0000 0029 034e 7217 0000 0072 1700 0000  ...).Nr....r....
 000015b0: 290a da05 6e75 6d70 79da 026e 70da 0a74  )...numpy..np..t
 000015c0: 656e 736f 7266 6c6f 7772 0400 0000 7215  ensorflowr....r.
-000015d0: 0000 0072 3600 0000 7248 0000 0072 4e00  ...r6...rH...rN.
-000015e0: 0000 7258 0000 0072 3100 0000 7203 0000  ..rX...r1...r...
+000015d0: 0000 0072 3500 0000 7247 0000 0072 4d00  ...r5...rG...rM.
+000015e0: 0000 7257 0000 0072 3100 0000 7203 0000  ..rW...r1...r...
 000015f0: 0072 0300 0000 7203 0000 0072 1400 0000  .r....r....r....
 00001600: da08 3c6d 6f64 756c 653e 0100 0000 731e  ..<module>....s.
 00001610: 0000 0008 0108 0308 1900 0000 0000 0000  ................
 00001620: ff0a 3400 0000 0000 0000 ff0a 3b0a 2508  ..4.........;.%.
 00001630: 09                                       .
```

### Comparing `lacss-0.4.1/lacss/data/augment.py` & `lacss-0.4.2/lacss/data/augment.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,20 +138,23 @@
                 bboxes, tf.cast([roi_h, roi_w, roi_h, roi_w], tf.float32)
             )
             bboxes = tf.maximum(bboxes, 0)
             new_areas = (bboxes[:, 2] - bboxes[:, 0]) * (bboxes[:, 3] - bboxes[:, 1])
 
             boolean_mask &= (new_areas / areas) >= area_ratio_threshold
 
+        # so that TF won't complain boolean_mask has no shape
+        boolean_mask = tf.ensure_shape(boolean_mask, [None])
+
         if "centroids" in inputs:
-            inputs["centroids"] = ctrds[boolean_mask]
+            inputs["centroids"] = tf.boolean_mask(ctrds, boolean_mask)
 
         if "bboxes" in inputs:
-            orig_bboxes = inputs["bboxes"][boolean_mask]
-            inputs["bboxes"] = bboxes[boolean_mask]
+            orig_bboxes = tf.boolean_mask(inputs["bboxes"], boolean_mask)
+            inputs["bboxes"] = tf.boolean_mask(bboxes, boolean_mask)
 
             if "masks" in inputs:
                 target_shape = inputs["masks"].shape[1:3]
 
                 orig_y0 = orig_bboxes[:, 0] - tf.cast(y0, orig_bboxes.dtype)
                 orig_x0 = orig_bboxes[:, 1] - tf.cast(x0, orig_bboxes.dtype)
                 orig_h = orig_bboxes[:, 2] - orig_bboxes[:, 0]
@@ -164,15 +167,15 @@
                     [orig_h, orig_w, orig_h, orig_w], axis=-1
                 )
                 new_bbox = new_bbox * tf.cast(
                     (target_shape + target_shape), new_bbox.dtype
                 )
 
                 inputs["masks"] = _crop_and_resize(
-                    inputs["masks"][boolean_mask],
+                    tf.boolean_mask(inputs["masks"], boolean_mask),
                     new_bbox,
                     target_shape,
                 )
 
         return inputs
 
     if p < 1.0 and tf.random.uniform([]) >= p:
```

### Comparing `lacss-0.4.1/lacss/deploy.py` & `lacss-0.4.2/lacss/deploy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,259 +1,261 @@
-import dataclasses
-import json
+""" 
+Attributes:
+    model_urls: URLs for build-in pretrain models. e.g model_urls["livecell"].
+"""
+from __future__ import annotations
+
 import logging
 import os
 import pickle
-import typing as tp
 from functools import lru_cache, partial
-from logging.config import valid_ident
-from os.path import join
 
 import flax.linen as nn
 import jax
 import jax.numpy as jnp
-import numpy as np
 from flax.core.frozen_dict import freeze, unfreeze
-from flax.training.train_state import TrainState
 
 import lacss.modules
-import lacss.train.strategy as strategy
 from lacss.ops import patches_to_label
 from lacss.train import Inputs
+from lacss.types import *
 
 _cached_partial = lru_cache(partial)
 
-Image = tp.Any
-
-model_urls = {
+model_urls: Mapping[str, str] = {
     "livecell": "https://data.mendeley.com/public-files/datasets/sj3vrvm6w3/files/439e524f-e4e9-4f97-9f38-c22cb85adbd1/file_downloaded",
     "tissuenet": "https://data.mendeley.com/public-files/datasets/sj3vrvm6w3/files/1e0a839d-f564-4ee0-a4f3-34792df7c613/file_downloaded",
 }
 
 
 def load_from_pretrained(pretrained):
     if os.path.isdir(pretrained):
-        import json
+        from lacss.train import LacssTrainer
 
-        try:
-            with open(join(pretrained, "config.in")) as f:
-                cfg = json.load(f)
-        except:
-            raise ValueError(
-                f"Cannot open 'config.in' in {pretrained} as a json config file."
-            )
-        with open(join(pretrained, "weights.pkl")) as f:
-            params = pickle.load(f)
+        trainer = LacssTrainer.from_checkpoint(pretrained)
+        module = trainer.model.principal
+        params = trainer.params["principal"]
 
     else:
+
         if os.path.isfile(pretrained):
             with open(pretrained, "rb") as f:
                 thingy = pickle.load(f)
 
         else:
-            from urllib.request import Request, urlopen
             import io
+            from urllib.request import Request, urlopen
 
             headers = {"User-Agent": "Wget/1.13.4 (linux-gnu)"}
             req = Request(url=pretrained, headers=headers)
 
             bytes = urlopen(req).read()
             thingy = pickle.loads(bytes)
 
         if isinstance(thingy, lacss.train.Trainer):
             module = thingy.model
             params = thingy.params
 
-            if not isinstance(module, lacss.modules.Lacss):
-                module = module.bind(dict(params=params))
-                module, params = module.lacss.unbind()
-                params = params["params"]
-
-            cfg = module
-
         else:
             cfg, params = thingy
 
+            if isinstance(cfg, lacss.modules.Lacss):
+                module = cfg
+            else:
+                module = lacss.modules.Lacss(**cfg)
+
     if "params" in params and len(params) == 1:
         params = params["params"]
 
-    # making a round-trip of module->cfg->module to icnrease backward-compatibility
-    # if isinstance(cfg, nn.Module):
+    return module, freeze(params)
 
-    #     cfg = dataclasses.asdict(cfg)
 
-    # module = lacss.modules.Lacss(**cfg)
+@partial(jax.jit, static_argnums=(0, 3))
+def _predict(apply_fn, params, image, scaling):
+    if scaling != 1:
+        h, w, c = image.shape
+        image = jax.image.resize(
+            image, [round(h * scaling), round(w * scaling), c], "linear"
+        )
+
+    preds = apply_fn(dict(params=params), image)
+    preds["pred_bboxes"] = lacss.ops.bboxes_of_patches(preds)
 
-    return cfg, freeze(params)
+    del preds["encoder_features"]
+    del preds["decoder_features"]
+    del preds["lpn_features"]
+    del preds["lpn_scores"]
+    del preds["lpn_regressions"]
+    del preds["instance_logit"]
+
+    if scaling != 1:
+        (
+            preds["instance_output"],
+            preds["instance_yc"],
+            preds["instance_xc"],
+        ) = lacss.ops.rescale_patches(preds, 1 / scaling)
 
+        preds["pred_locations"] = preds["pred_locations"] / scaling
+        preds["pred_bboxes"] = preds["pred_bboxes"] / scaling
 
-@partial(jax.jit, static_argnums=0)
-def _predict(apply_fn, params, image):
-    return apply_fn(dict(params=params), image)
+    return preds
 
 
 class Predictor:
-    """ Main interface for model deployment.
+    """Main class interface for model deployment. This is the only class you
+    need if you don't train your own model
+
+    Examples:
+        The most common use case is to use a build-in pretrained model.
+
+            ```
+            import lacss.deploy
 
+            # look up the url of a build-in mode
+            url = lacss.deploy.model_urls["livecell"]
+
+            # create the predictor instance
+            predictor = lacss.deploy.Predictor(url)
+
+            # make a prediction
+            label = predictor.predict_label(image)
+
+            ```
     Attributes:
-        module: The underlying FLAX module 
+        module: The underlying FLAX module
         params: Model weights.
-        detector: The detector submodule for convinence. It is common to 
-            modidify this submodule to find optimal parameters for detection.
-            Note this submodule is weight-less.
-    
-    Constructor:
-        url: A URL of the saved model. URLs for build-in pretrained models can be found
-            in lacss.deploy.model_urls
-        precompile_shape: Optionally supply the image shape for precompiling. Otherwise 
-            the model will be recompiled for every new input image shape.
-    
-    Usage Example:
-        url = lacss.deploy.model_urls["livecell"]
-        predictor = lacss.deploy.Predictor(url)
-        label = predictor.predict_label(image)
+        detector: The detector submodule for convinence. A common use case
+            is to customize this submodule during inference. e.g.
+            ```
+            predictor.detector['test_min_score"] = 0.5
+            ```
+            Detector submodule has no trained paramters.
     """
-    def __init__(self, url, precompile_shape=None):
+
+    def __init__(self, url: str, precompile_shape: Optional[Shape] = None):
+        """Construct Predictor
+
+        Args:
+            url: A URL or local path to the saved model.
+                URLs for build-in pretrained models can be found in lacss.deploy.model_urls
+            precompile_shape: Image shape(s) for precompiling. Otherwise
+                the model will be recompiled for every new input image shape.
+
+        """
         self.model = load_from_pretrained(url)
 
         if precompile_shape is not None:
             logging.info("Prcompile the predictor for image shape {precompile_shape}.")
             logging.info("This will take several minutes.")
 
             try:
                 iter(precompile_shape[0])
             except:
                 precompile_shape = [precompile_shape]
             for shape in precompile_shape:
-                x = np.zeros(shape)
+                x = jnp.zeros(shape)
                 _ = self.predict(x)
 
     def __call__(self, inputs, **kwargs):
-        """ Perform model prediction
-        """
         inputs_obj = Inputs.from_value(inputs)
 
         return self.predict(*inputs_obj.args, **inputs_obj.kwargs, **kwargs)
 
     def predict(
         self,
-        image: Image,
+        image: ArrayLike,
         min_area: float = 0,
         remove_out_of_bound: bool = False,
         scaling: float = 1.0,
         **kwargs,
-    ):
+    ) -> dict:
         """Predict segmentation.
 
         Args:
             image: A ndarray of (h,w,c) format. Value of c must be 1-3
-            min_area: Minimum area of a valid prediction. Default is 0
+            min_area: Minimum area of a valid prediction.
             remove_out_of_bound: Whether to remove out-of-bound predictions. Default is False.
             scaling: A image scaling factor. If not 1, the input image will be resized internally before fed
                 to the model. The results will be resized back to the scale of the orginal input image.
 
         Returns:
-            Raw model prediction as a dict. Most important keys are
+            Model predictions with following elements:
 
-            instance_output: Segmentation instances. (N, S, S) array
-            instance_yc: The meshgrid y-coordinates of the instances. (N, S, S) array
-            instance_xc: The meshgrid x-coordinates of the instances. (N, S, S) array
-            pred_scores: The prediction scores of each instance. (N) array. -1 indicating invalid predictions.
-            pred_locations: The prediction centroids of each instances. (N, 2) array
+                - pred_scores: The prediction scores of each instance.
+                - pred_bboxes: The bounding-boxes of detected instances in y0x0y1x1 format
+                - instance_output: A 3d array representing segmentation instances.
+                - instance_yc: The meshgrid y-coordinates of the instances.
+                - instance_xc: The meshgrid x-coordinates of the instances.
+                - instance_mask: a masking tensor. Invalid instances are maked with 0.
         """
 
         module, params = self.model
 
         if len(kwargs) > 0:
             apply_fn = _cached_partial(module.apply, **kwargs)
         else:
             apply_fn = module.apply
 
-        if scaling != 1.0:
-            h, w, c = image.shape
-            image = jax.image.resize(
-                image, [round(h * scaling), round(w * scaling), c], "linear"
-            )
+        preds = _predict(apply_fn, params, image, scaling)
 
-        preds = _predict(apply_fn, params, image)
-        del preds["encoder_features"]
-        del preds["decoder_features"]
-        del preds["lpn_features"]
-        del preds["lpn_scores"]
-        del preds["lpn_regressions"]
+        # check prediction validity
+        instance_mask = preds["instance_mask"].squeeze(axis=(1, 2))
 
         if min_area > 0:
-            areas = jnp.count_nonzero(preds["instance_logit"] > 0, axis=(1, 2))
-            preds["pred_scores"] = jnp.where(
-                areas > min_area,
-                preds["pred_scores"],
-                -1,
-            )
+            areas = np.count_nonzero(preds["instance_logit"] > 0, axis=(1, 2))
+            instance_mask &= areas > min_area
 
         if remove_out_of_bound:
             pred_locations = preds["pred_locations"]
             h, w, _ = image.shape
             valid_locs = (pred_locations >= 0).all(axis=-1)
             valid_locs &= pred_locations[:, 0] < h
             valid_locs &= pred_locations[:, 1] < w
-            preds["pred_locations"] = jnp.where(
-                valid_locs[:, None],
-                preds["pred_locations"],
-                -1,
-            )
-            preds["pred_scores"] = jnp.where(
-                valid_locs,
-                preds["pred_scores"],
-                -1,
-            )
+            instance_mask &= valid_locs
 
-        if scaling != 1.0:
-            (
-                preds["instance_output"],
-                preds["instance_yc"],
-                preds["instance_xc"],
-            ) = lacss.ops.rescale_patches(preds, 1 / scaling)
-            preds["pred_locations"] = preds["pred_locations"] / scaling
+        preds["instance_mask"] = instance_mask.reshape(-1, 1, 1)
 
         return preds
 
-    def predict_label(self, image, *, score_threshold=0.5, **kwargs):
-        """ A convinent funciton to obtain prediction in image label format
+    def predict_label(
+        self, image: ArrayLike, *, score_threshold: float = 0.5, **kwargs
+    ) -> Array:
+        """Predict segmentation in image label format
 
         Args:
             image: Input image.
-            score_threshold: The minimal prediction scores. Default is 0.5
+            score_threshold: The minimal prediction scores.
 
         Returns:
-            label: A [H, W] array. The values indicate the id of the cells. For cells
+            A [H, W] array. The values indicate the id of the cells. For cells
                 with overlapping areas, the pixel is assigned for the cell with higher
                 prediction scores.
         """
         preds = self.predict(image, **kwargs)
 
         return patches_to_label(
-            preds, 
-            input_size=image.shape[:2], 
+            preds,
+            input_size=image.shape[:2],
             score_threshold=score_threshold,
         )
 
     @property
-    def module(self):
+    def module(self) -> nn.Module:
         return self.model[0]
-    
+
     @property
-    def params(self):
+    def params(self) -> Params:
         return self.model[1]
-    
+
     @params.setter
     def params(self, new_params):
         self.model = self.module, new_params
 
     @property
-    def detector(self):
+    def detector(self) -> lacss.modules.Detector:
         return self.module.detector
 
     # FIXME Change the detector without first compile the mode will result
     # in error. This is a hidden gotcha. Need to setup warning to the user.
     @detector.setter
     def detector(self, new_detector):
         from .modules import Detector
@@ -271,7 +273,20 @@
                     new_detector,
                     self.module.segmentor,
                 ),
                 self.model[1],
             )
         else:
             raise ValueError(f"{new_detector} is not a Lacss Detector")
+
+    def pickle(self, save_path) -> None:
+        """Save the model by pickling.
+            In the form of (model_config:dict, weights:FrozenDict).
+
+        Args:
+            save_path: Path to the pkl file
+        """
+        _cfg = self.model[0].get_config()
+        _params = self.model[1]
+
+        with open(save_path, "wb") as f:
+            pickle.dump((_cfg, _params), f)
```

### Comparing `lacss-0.4.1/lacss/losses/__pycache__/auxiliary.cpython-38.pyc` & `lacss-0.4.2/lacss/losses/__pycache__/auxiliary.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 19:35:53 2023 UTC, .py size: 5248 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 99e8 9964 8014 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 e17d ad64 5815 0000  U........}.dX...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 6d04 5a05 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6402 6c06 5a06 6403 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6403 6405 6c09 6d0a 5a0a 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 0100 6505 a00d 6408  d.l.m.Z...e...d.
@@ -57,260 +57,268 @@
 00000380: 0272 1d00 0000 6302 0000 0000 0000 0000  .r....c.........
 00000390: 0000 000b 0000 0006 0000 004b 0000 0073  ...........K...s
 000003a0: 5800 0000 7c00 6401 1900 7d03 7c00 6402  X...|.d...}.|.d.
 000003b0: 1900 7d04 7c00 6403 1900 7d05 7c01 6404  ..}.|.d...}.|.d.
 000003c0: 1900 6a00 5c03 7d06 7d07 7d08 7401 7c03  ..j.\.}.}.}.t.|.
 000003d0: 7c04 7c05 7c06 7c07 8305 7d09 7402 6a03  |.|.|.|...}.t.j.
 000003e0: a004 7c00 6405 1900 a101 7d0a 7405 a006  ..|.d.....}.t...
-000003f0: 7c0a 7c09 a102 a007 a100 5300 2906 7a22  |.|.......S.).z"
-00000400: 4c41 4353 5320 6365 6c6c 2062 6f72 6465  LACSS cell borde
-00000410: 7220 636f 6e73 6973 7465 6e63 7920 6c6f  r consistency lo
-00000420: 7373 7213 0000 0072 1400 0000 7215 0000  ssr....r....r...
-00000430: 00da 0569 6d61 6765 5a09 6564 6765 5f70  ...imageZ.edge_p
-00000440: 7265 6429 0872 0a00 0000 721d 0000 00da  red).r....r.....
-00000450: 036a 6178 da02 6e6e da07 7369 676d 6f69  .jax..nn..sigmoi
-00000460: 64da 056f 7074 6178 da07 6c32 5f6c 6f73  d..optax..l2_los
-00000470: 73da 046d 6561 6e29 0bda 0570 7265 6473  s..mean)...preds
-00000480: da06 696e 7075 7473 da06 6b77 6172 6773  ..inputs..kwargs
-00000490: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-000004a0: 1600 0000 7217 0000 0072 1800 0000 5a0d  ....r....r....Z.
-000004b0: 696e 7374 616e 6365 5f65 6467 655a 1269  instance_edgeZ.i
-000004c0: 6e73 7461 6e63 655f 6564 6765 5f70 7265  nstance_edge_pre
-000004d0: 6472 1b00 0000 721b 0000 0072 1c00 0000  dr....r....r....
-000004e0: da19 7365 6c66 5f73 7570 6572 7669 7365  ..self_supervise
-000004f0: 645f 6564 6765 5f6c 6f73 7322 0000 0073  d_edge_loss"...s
-00000500: 1a00 0000 0003 0801 0801 0801 1001 0201  ................
-00000510: 0200 0200 0200 0200 02ff 0403 1002 7228  ..............r(
-00000520: 0000 00e7 0000 0000 0000 2440 6700 0000  ..........$@g...
-00000530: 0000 0000 4029 02da 0c6f 6666 7365 745f  ....@)...offset_
-00000540: 7369 676d 61da 0c6f 6666 7365 745f 7363  sigma..offset_sc
-00000550: 616c 6563 0200 0000 0000 0000 0200 0000  alec............
-00000560: 0b00 0000 0600 0000 0b00 0000 73da 0000  ............s...
-00000570: 0088 0164 0119 006a 005c 0389 0089 057d  ...d...j.\.....}
-00000580: 057c 0064 0219 006a 005c 037d 0589 047d  .|.d...j.\.}...}
-00000590: 0587 0087 0187 0287 0387 0487 0566 0664  .............f.d
-000005a0: 0364 0484 087d 0674 016a 02a0 037c 0064  .d...}.t.j...|.d
-000005b0: 0519 00a1 017d 0774 016a 04a0 0574 016a  .....}.t.j...t.j
-000005c0: 02a0 037c 067c 0083 01a1 01a1 017d 0874  ...|.|.......}.t
-000005d0: 06a0 0788 0164 0619 0064 0717 00a1 017d  .....d...d.....}
-000005e0: 097c 09a0 0874 09a1 017d 097c 086a 0a7c  .|...t...}.|.j.|
-000005f0: 0964 0864 0885 0264 0966 0219 007c 0964  .d.d...d.f...|.d
-00000600: 0864 0885 0264 0a66 0219 0066 0219 00a0  .d...d.f...f....
-00000610: 0b64 0ba1 017d 087c 076a 007c 086a 006b  .d...}.|.j.|.j.k
-00000620: 0273 b674 0c82 0164 0b7c 0818 007c 0714  .s.t...d.|...|..
-00000630: 007c 0864 0b7c 0718 0014 0017 007d 0a7c  .|.d.|.......}.|
-00000640: 0aa0 0da1 007d 0a7c 0a53 0029 0c7a 294c  .....}.|.S.).z)L
-00000650: 4143 5353 2069 6d61 6765 2073 6567 6d65  ACSS image segme
-00000660: 6e74 6174 696f 6e20 636f 6e73 6973 7465  ntation consiste
-00000670: 6e63 7420 6c6f 7373 721e 0000 0072 1400  nct lossr....r..
-00000680: 0000 6301 0000 0000 0000 0000 0000 0009  ..c.............
-00000690: 0000 0005 0000 0013 0000 0073 1201 0000  ...........s....
-000006a0: 7400 a001 8800 8804 1700 8805 8804 1700  t...............
-000006b0: 6702 a101 6401 1800 7d01 7c00 6402 1900  g...d...}.|.d...
-000006c0: 7c00 6403 1900 0200 7d02 7d03 7c00 6404  |.d.....}.}.|.d.
-000006d0: 1900 7d04 6405 8801 6b06 725c 8801 6405  ..}.d...k.r\..d.
-000006e0: 1900 6400 6b09 725c 8801 6405 1900 a002  ..d.k.r\..d.....
-000006f0: 7403 a101 a004 a100 7d05 6e04 6406 7d05  t.......}.n.d.}.
-00000700: 8803 7c05 1900 7d06 8802 7c05 1900 7d07  ..|...}...|...}.
-00000710: 7400 6a05 6400 8804 8502 6400 8804 8502  t.j.d.....d.....
-00000720: 6602 1900 8804 6407 1800 6408 1b00 1800  f.....d...d.....
-00000730: 6408 1300 6408 7c06 1400 7c06 1400 1b00  d...d.|...|.....
-00000740: 7d08 7400 a006 7c08 6a07 6406 6409 8d01  }.t...|.j.d.d...
-00000750: 0b00 a101 7c07 1400 7d08 7c04 7c08 3700  ....|...}.|.|.7.
-00000760: 7d04 7c01 6a08 7c02 8804 6408 1a00 1700  }.|.j.|...d.....
-00000770: 7c03 8804 6408 1a00 1700 6602 1900 a009  |...d.....f.....
-00000780: 7c04 a101 7d01 7c01 8804 6408 1a00 8804  |...}.|...d.....
-00000790: 0b00 6408 1a00 8502 8804 6408 1a00 8804  ..d.......d.....
-000007a0: 0b00 6408 1a00 8502 6602 1900 7d01 7c01  ..d.....f...}.|.
-000007b0: 5300 290a 4ee7 0000 0000 8084 2e41 7214  S.).N........Ar.
-000007c0: 0000 0072 1500 0000 5a0e 696e 7374 616e  ...r....Z.instan
-000007d0: 6365 5f6c 6f67 6974 da08 6361 7465 676f  ce_logit..catego
-000007e0: 7279 7201 0000 0072 0600 0000 7203 0000  ryr....r....r...
-000007f0: 0029 01da 0461 7869 7329 0a72 0b00 0000  .)...axis).r....
-00000800: 720f 0000 00da 0661 7374 7970 65da 0369  r......astype..i
-00000810: 6e74 da07 7371 7565 657a 65da 056d 6772  nt..squeeze..mgr
-00000820: 6964 da03 6578 70da 0373 756d 7210 0000  id..exp..sumr...
-00000830: 00da 036d 6178 2909 da04 7072 6564 da05  ...max)...pred..
-00000840: 6c61 6265 6cda 0279 63da 0278 63da 056c  label..yc..xc..l
-00000850: 6f67 6974 da01 63da 0573 6967 6d61 da05  ogit..c..sigma..
-00000860: 7363 616c 65da 066f 6666 7365 74a9 0672  scale..offset..r
-00000870: 1600 0000 7226 0000 0072 2b00 0000 722a  ....r&...r+...r*
-00000880: 0000 0072 1900 0000 7217 0000 0072 1b00  ...r....r....r..
-00000890: 0000 721c 0000 00da 0a5f 6d61 785f 6d65  ..r......_max_me
-000008a0: 7267 653e 0000 0073 1c00 0000 0001 1a01  rge>...s........
-000008b0: 1201 0802 1401 1402 0402 0801 0801 3201  ..............2.
-000008c0: 1801 0802 2401 2802 7a35 7365 6c66 5f73  ....$.(.z5self_s
-000008d0: 7570 6572 7669 7365 645f 7365 676d 656e  upervised_segmen
-000008e0: 7461 7469 6f6e 5f6c 6f73 732e 3c6c 6f63  tation_loss.<loc
-000008f0: 616c 733e 2e5f 6d61 785f 6d65 7267 65da  als>._max_merge.
-00000900: 0766 675f 7072 6564 da0c 6774 5f6c 6f63  .fg_pred..gt_loc
-00000910: 6174 696f 6e73 6700 0000 0000 00e0 3f4e  ationsg.......?N
-00000920: 7201 0000 0072 0600 0000 7209 0000 0029  r....r....r....)
-00000930: 0e72 0a00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00000940: 7221 0000 00da 036c 6178 da0d 7374 6f70  r!.....lax..stop
-00000950: 5f67 7261 6469 656e 7472 0b00 0000 da05  _gradientr......
-00000960: 666c 6f6f 7272 2f00 0000 7230 0000 0072  floorr/...r0...r
-00000970: 1000 0000 da03 7365 74da 0e41 7373 6572  ......set..Asser
-00000980: 7469 6f6e 4572 726f 7272 2400 0000 290b  tionErrorr$...).
-00000990: 7225 0000 0072 2600 0000 722a 0000 0072  r%...r&...r*...r
-000009a0: 2b00 0000 7227 0000 0072 1800 0000 7240  +...r'...r....r@
-000009b0: 0000 0072 4100 0000 5a08 6667 5f6c 6162  ...rA...Z.fg_lab
-000009c0: 656c da04 6c6f 6373 da04 6c6f 7373 721b  el..locs..lossr.
-000009d0: 0000 0072 3f00 0000 721c 0000 00da 2173  ...r?...r.....!s
-000009e0: 656c 665f 7375 7065 7276 6973 6564 5f73  elf_supervised_s
-000009f0: 6567 6d65 6e74 6174 696f 6e5f 6c6f 7373  egmentation_loss
-00000a00: 3100 0000 7318 0000 0000 0a10 0110 0216  1...s...........
-00000a10: 1710 0118 0212 010a 012c 0210 0318 0208  .........,......
-00000a20: 0272 4a00 0000 e77b 14ae 47e1 7a84 3fa9  .rJ....{..G.z.?.
-00000a30: 01da 0677 6569 6768 7463 0200 0000 0000  ...weightc......
-00000a40: 0000 0100 0000 0c00 0000 0600 0000 4b00  ..............K.
-00000a50: 0000 73ac 0000 007c 0164 0119 006a 005c  ..s....|.d...j.\
-00000a60: 037d 047d 057d 067c 0064 0219 0064 036b  .}.}.}.|.d...d.k
-00000a70: 057c 0064 0219 007c 046b 0040 007c 0064  .|.d...|.k.@.|.d
-00000a80: 0419 0064 036b 0540 007c 0064 0419 007c  ...d.k.@.|.d...|
-00000a90: 056b 0040 007d 0774 016a 027c 0064 0519  .k.@.}.t.j.|.d..
-00000aa0: 0064 067c 0764 0764 088d 047d 0874 01a0  .d.|.d.d...}.t..
-00000ab0: 037c 0874 0464 09a1 037d 0874 056a 06a0  .|.t.d...}.t.j..
-00000ac0: 077c 08a1 017c 0064 0519 006a 0064 0a19  .|...|.d...j.d..
-00000ad0: 0014 007d 097c 0064 0b19 007d 0a74 01a0  ...}.|.d...}.t..
-00000ae0: 087c 0aa1 0174 0417 007d 0b7c 096a 027c  .|...t...}.|.j.|
-00000af0: 0a64 0c8d 017c 0b1b 007d 097c 097c 0214  .d...|...}.|.|..
-00000b00: 0053 0029 0d7a 2861 7578 696c 6c61 7279  .S.).z(auxillary
-00000b10: 206c 6f73 7320 746f 2070 7265 7665 6e74   loss to prevent
-00000b20: 206d 6f64 656c 2063 6f6c 6c61 7073 6572   model collapser
-00000b30: 1e00 0000 7214 0000 0072 0100 0000 7215  ....r....r....r.
-00000b40: 0000 0072 1300 0000 2902 e9ff ffff ffe9  ...r....).......
-00000b50: feff ffff 5429 0372 2e00 0000 da05 7768  ....T).r......wh
-00000b60: 6572 65da 086b 6565 7064 696d 7372 2c00  ere..keepdimsr,.
-00000b70: 0000 724e 0000 005a 0d69 6e73 7461 6e63  ..rN...Z.instanc
-00000b80: 655f 6d61 736b 2901 7250 0000 0029 0972  e_mask).rP...).r
-00000b90: 0a00 0000 720b 0000 0072 3400 0000 720e  ....r....r4...r.
-00000ba0: 0000 00da 0345 5053 721f 0000 0072 4300  .....EPSr....rC.
-00000bb0: 0000 da05 7273 7172 74da 0d63 6f75 6e74  ....rsqrt..count
-00000bc0: 5f6e 6f6e 7a65 726f 290c 7225 0000 0072  _nonzero).r%...r
-00000bd0: 2600 0000 724d 0000 0072 2700 0000 7216  &...rM...r'...r.
-00000be0: 0000 0072 1700 0000 7218 0000 005a 0a76  ...r....r....Z.v
-00000bf0: 616c 6964 5f6c 6f63 73da 0561 7265 6173  alid_locs..areas
-00000c00: 7249 0000 00da 046d 6173 6bda 0b6e 5f69  rI.....mask..n_i
-00000c10: 6e73 7461 6e63 6573 721b 0000 0072 1b00  nstancesr....r..
-00000c20: 0000 721c 0000 00da 0d61 7578 5f73 697a  ..r......aux_siz
-00000c30: 655f 6c6f 7373 6600 0000 732a 0000 0000  e_lossf...s*....
-00000c40: 0310 030a 010a ff02 020a fe02 030a fd02  ................
-00000c50: ff02 0704 0106 0002 0002 0002 ff06 030e  ................
-00000c60: 011a 0208 010e 0110 0272 5800 0000 6302  .........rX...c.
-00000c70: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-00000c80: 0000 004b 0000 0073 3e00 0000 6401 7c01  ...K...s>...d.|.
-00000c90: 6b06 721c 7c01 6401 1900 6402 6b04 a000  k.r.|.d...d.k...
-00000ca0: 6403 a101 7d03 6e0e 7c01 6404 1900 a000  d...}.n.|.d.....
-00000cb0: 6403 a101 7d03 7401 a002 7c00 6405 1900  d...}.t...|.d...
-00000cc0: 7c03 a102 a003 a100 5300 2906 4e5a 0967  |.......S.).NZ.g
-00000cd0: 745f 6c61 6265 6c73 7201 0000 0072 0800  t_labelsr....r..
-00000ce0: 0000 5a07 6774 5f6d 6173 6b72 4100 0000  ..Z.gt_maskrA...
-00000cf0: 2904 722f 0000 0072 2200 0000 da1c 7369  ).r/...r".....si
-00000d00: 676d 6f69 645f 6269 6e61 7279 5f63 726f  gmoid_binary_cro
-00000d10: 7373 5f65 6e74 726f 7079 7224 0000 0029  ss_entropyr$...)
-00000d20: 0472 2500 0000 da06 6c61 6265 6c73 7227  .r%.....labelsr'
-00000d30: 0000 0072 5600 0000 721b 0000 0072 1b00  ...rV...r....r..
-00000d40: 0000 721c 0000 00da 1c73 7570 6572 7669  ..r......supervi
-00000d50: 7365 645f 7365 676d 656e 7461 7469 6f6e  sed_segmentation
-00000d60: 5f6c 6f73 737f 0000 0073 0800 0000 0002  _loss....s......
-00000d70: 0802 1404 0e02 725b 0000 0063 0000 0000  ......r[...c....
-00000d80: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000d90: 4000 0000 731c 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00000da0: 0265 0365 0364 019c 0264 0264 0384 045a  .e.e.d...d.d...Z
-00000db0: 0464 0453 0029 05da 0b41 7578 4564 6765  .d.S.)...AuxEdge
-00000dc0: 4c6f 7373 2902 7226 0000 0072 2500 0000  Loss).r&...r%...
-00000dd0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-00000de0: 0003 0000 004b 0000 0073 1600 0000 6401  .....K...s....d.
-00000df0: 7c02 6b07 720c 6402 5300 7400 7c02 7c01  |.k.r.d.S.t.|.|.
-00000e00: 8302 5300 2903 4e5a 1274 7261 696e 696e  ..S.).NZ.trainin
-00000e10: 675f 6c6f 6361 7469 6f6e 7367 0000 0000  g_locationsg....
-00000e20: 0000 0000 2901 7228 0000 00a9 04da 0473  ....).r(.......s
-00000e30: 656c 6672 2600 0000 7225 0000 0072 2700  elfr&...r%...r'.
-00000e40: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-00000e50: 00da 0463 616c 6c8d 0000 0073 0600 0000  ...call....s....
-00000e60: 0006 0801 0402 7a10 4175 7845 6467 654c  ......z.AuxEdgeL
-00000e70: 6f73 732e 6361 6c6c 4e29 05da 085f 5f6e  oss.callN)...__n
-00000e80: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000e90: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00000ea0: 0464 6963 7472 5f00 0000 721b 0000 0072  .dictr_...r....r
-00000eb0: 1b00 0000 721b 0000 0072 1c00 0000 725c  ....r....r....r\
-00000ec0: 0000 008c 0000 0073 0600 0000 0803 0201  .......s........
-00000ed0: 02fd 725c 0000 0063 0000 0000 0000 0000  ..r\...c........
-00000ee0: 0000 0000 0000 0000 0400 0000 0000 0000  ................
-00000ef0: 7326 0000 0065 005a 0164 005a 0264 0687  s&...e.Z.d.Z.d..
-00000f00: 0066 0164 0264 0384 095a 0364 0464 0584  .f.d.d...Z.d.d..
-00000f10: 005a 0487 0004 005a 0553 0029 07da 0b41  .Z.....Z.S.)...A
-00000f20: 7578 5369 7a65 4c6f 7373 724b 0000 0063  uxSizeLossrK...c
-00000f30: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000f40: 0200 0000 0300 0000 7314 0000 0074 0083  ........s....t..
-00000f50: 00a0 01a1 0001 007c 017c 005f 0264 0053  .......|.|._.d.S
-00000f60: 0029 014e 2903 da05 7375 7065 72da 085f  .).N)...super.._
-00000f70: 5f69 6e69 745f 5fda 0161 2902 725e 0000  _init__..a).r^..
-00000f80: 00da 0561 6c70 6861 a901 da09 5f5f 636c  ...alpha....__cl
-00000f90: 6173 735f 5f72 1b00 0000 721c 0000 0072  ass__r....r....r
-00000fa0: 6600 0000 9a00 0000 7304 0000 0000 010a  f.......s.......
-00000fb0: 017a 1441 7578 5369 7a65 4c6f 7373 2e5f  .z.AuxSizeLoss._
-00000fc0: 5f69 6e69 745f 5f63 0300 0000 0000 0000  _init__c........
-00000fd0: 0000 0000 0400 0000 0500 0000 4b00 0000  ............K...
-00000fe0: 7310 0000 0074 007c 027c 017c 006a 0164  s....t.|.|.|.j.d
-00000ff0: 018d 0353 0029 024e 724c 0000 0029 0272  ...S.).NrL...).r
-00001000: 5800 0000 7267 0000 0072 5d00 0000 721b  X...rg...r]...r.
-00001010: 0000 0072 1b00 0000 721c 0000 0072 5f00  ...r....r....r_.
-00001020: 0000 9e00 0000 7302 0000 0000 027a 1041  ......s......z.A
-00001030: 7578 5369 7a65 4c6f 7373 2e63 616c 6c29  uxSizeLoss.call)
-00001040: 0172 4b00 0000 a906 7260 0000 0072 6100  .rK.....r`...ra.
-00001050: 0000 7262 0000 0072 6600 0000 725f 0000  ..rb...rf...r_..
-00001060: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00001070: 721b 0000 0072 1b00 0000 7269 0000 0072  r....r....ri...r
-00001080: 1c00 0000 7264 0000 0099 0000 0073 0400  ....rd.......s..
-00001090: 0000 0801 0e04 7264 0000 0063 0000 0000  ......rd...c....
-000010a0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-000010b0: 0000 0000 7326 0000 0065 005a 0164 005a  ....s&...e.Z.d.Z
-000010c0: 0264 0787 0066 0164 0364 0484 095a 0364  .d...f.d.d...Z.d
-000010d0: 0564 0684 005a 0487 0004 005a 0553 0029  .d...Z.....Z.S.)
-000010e0: 08da 0a41 7578 5365 674c 6f73 7372 2900  ...AuxSegLossr).
-000010f0: 0000 e700 0000 0000 0014 4063 0300 0000  ..........@c....
-00001100: 0000 0000 0000 0000 0400 0000 0600 0000  ................
-00001110: 0b00 0000 736a 0000 0074 0083 006a 0166  ....sj...t...j.f
-00001120: 007c 038e 0101 007a 0c7c 0164 0119 0001  .|.....z.|.d....
-00001130: 0057 006e 1201 0001 0001 007c 0166 017d  .W.n.......|.f.}
-00001140: 0159 006e 0258 007a 0c7c 0264 0119 0001  .Y.n.X.z.|.d....
-00001150: 0057 006e 1201 0001 0001 007c 0266 017d  .W.n.......|.f.}
-00001160: 0259 006e 0258 0074 02a0 037c 02a1 017c  .Y.n.X.t...|...|
-00001170: 005f 0474 02a0 037c 01a1 017c 005f 0564  ._.t...|...|._.d
-00001180: 0053 0029 024e 7201 0000 0029 0672 6500  .S.).Nr....).re.
-00001190: 0000 7266 0000 0072 0b00 0000 da05 6172  ..rf...r......ar
-000011a0: 7261 7972 2b00 0000 722a 0000 0029 0472  rayr+...r*...).r
-000011b0: 5e00 0000 722a 0000 0072 2b00 0000 7227  ^...r*...r+...r'
-000011c0: 0000 0072 6900 0000 721b 0000 0072 1c00  ...ri...r....r..
-000011d0: 0000 7266 0000 00a4 0000 0073 1600 0000  ..rf.......s....
-000011e0: 0001 0e01 0201 0c01 0601 0c02 0201 0c01  ................
-000011f0: 0601 0c02 0c01 7a13 4175 7853 6567 4c6f  ......z.AuxSegLo
-00001200: 7373 2e5f 5f69 6e69 745f 5f63 0300 0000  ss.__init__c....
-00001210: 0000 0000 0000 0000 0400 0000 0600 0000  ................
-00001220: 4b00 0000 7314 0000 0074 007c 027c 017c  K...s....t.|.|.|
-00001230: 006a 017c 006a 0264 018d 0453 0029 024e  .j.|.j.d...S.).N
-00001240: 2902 722b 0000 0072 2a00 0000 2903 724a  ).r+...r*...).rJ
-00001250: 0000 0072 2b00 0000 722a 0000 0072 5d00  ...r+...r*...r].
-00001260: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-00001270: 0072 5f00 0000 b300 0000 730c 0000 0000  .r_.......s.....
-00001280: 0202 0102 0102 0104 0104 fc7a 0f41 7578  ...........z.Aux
-00001290: 5365 674c 6f73 732e 6361 6c6c 2902 7229  SegLoss.call).r)
-000012a0: 0000 0072 6e00 0000 726b 0000 0072 1b00  ...rn...rk...r..
-000012b0: 0000 721b 0000 0072 6900 0000 721c 0000  ..r....ri...r...
-000012c0: 0072 6d00 0000 a300 0000 7304 0000 0008  .rm.......s.....
-000012d0: 010e 0f72 6d00 0000 2919 da09 6675 6e63  ...rm...)...func
-000012e0: 746f 6f6c 7372 0200 0000 721f 0000 00da  toolsr....r.....
-000012f0: 096a 6178 2e6e 756d 7079 da05 6e75 6d70  .jax.numpy..nump
-00001300: 7972 0b00 0000 7222 0000 00da 036f 7073  yr....r".....ops
-00001310: 7204 0000 005a 0a74 7261 696e 2e6c 6f73  r....Z.train.los
-00001320: 7372 0500 0000 da09 6465 7465 6374 696f  sr......detectio
-00001330: 6e72 0700 0000 da05 6669 6e66 6fda 0365  nr......finfo..e
-00001340: 7073 7252 0000 0072 1d00 0000 7228 0000  psrR...r....r(..
-00001350: 0072 6f00 0000 724a 0000 0072 5800 0000  .ro...rJ...rX...
-00001360: 725b 0000 0072 5c00 0000 7264 0000 0072  r[...r\...rd...r
-00001370: 6d00 0000 721b 0000 0072 1b00 0000 721b  m...r....r....r.
-00001380: 0000 0072 1c00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00001390: 653e 0100 0000 7322 0000 000c 0208 010c  e>....s"........
-000013a0: 0108 020c 010c 010c 020c 0308 1408 130a  ................
-000013b0: 010a fb0c 350e 1908 0d10 0d10 0a         ....5........
+000003f0: 7c0a 7c09 a102 a007 a100 5300 2906 7a27  |.|.......S.).z'
+00000400: 4365 6c6c 2062 6f72 6465 7220 7072 6564  Cell border pred
+00000410: 6963 7469 6f6e 2063 6f6e 7369 7374 656e  iction consisten
+00000420: 6379 206c 6f73 7372 1300 0000 7214 0000  cy lossr....r...
+00000430: 0072 1500 0000 da05 696d 6167 655a 0965  .r......imageZ.e
+00000440: 6467 655f 7072 6564 2908 720a 0000 0072  dge_pred).r....r
+00000450: 1d00 0000 da03 6a61 78da 026e 6eda 0773  ......jax..nn..s
+00000460: 6967 6d6f 6964 da05 6f70 7461 78da 076c  igmoid..optax..l
+00000470: 325f 6c6f 7373 da04 6d65 616e 290b da05  2_loss..mean)...
+00000480: 7072 6564 73da 0669 6e70 7574 73da 066b  preds..inputs..k
+00000490: 7761 7267 7372 1300 0000 7214 0000 0072  wargsr....r....r
+000004a0: 1500 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
+000004b0: 0000 005a 0d69 6e73 7461 6e63 655f 6564  ...Z.instance_ed
+000004c0: 6765 5a12 696e 7374 616e 6365 5f65 6467  geZ.instance_edg
+000004d0: 655f 7072 6564 721b 0000 0072 1b00 0000  e_predr....r....
+000004e0: 721c 0000 00da 1973 656c 665f 7375 7065  r......self_supe
+000004f0: 7276 6973 6564 5f65 6467 655f 6c6f 7373  rvised_edge_loss
+00000500: 2200 0000 731a 0000 0000 0308 0108 0108  "...s...........
+00000510: 0110 0102 0102 0002 0002 0002 0002 ff04  ................
+00000520: 0310 0272 2800 0000 e700 0000 0000 0024  ...r(..........$
+00000530: 4067 0000 0000 0000 0040 2902 da0c 6f66  @g.......@)...of
+00000540: 6673 6574 5f73 6967 6d61 da0c 6f66 6673  fset_sigma..offs
+00000550: 6574 5f73 6361 6c65 6302 0000 0000 0000  et_scalec.......
+00000560: 0002 0000 000b 0000 0006 0000 000b 0000  ................
+00000570: 0073 fa00 0000 8801 6401 1900 6a00 5c03  .s......d...j.\.
+00000580: 8900 8905 7d05 7c00 6402 1900 6a00 5c03  ....}.|.d...j.\.
+00000590: 7d05 8904 7d05 7401 a002 8803 a101 a003  }...}.t.........
+000005a0: 6403 a101 8903 7401 a002 8802 a101 a003  d.....t.........
+000005b0: 6403 a101 8902 8700 8701 8702 8703 8704  d...............
+000005c0: 8705 6606 6404 6405 8408 7d06 7404 6a05  ..f.d.d...}.t.j.
+000005d0: a006 7c00 6406 1900 a101 7d07 7404 6a07  ..|.d.....}.t.j.
+000005e0: a008 7404 6a05 a006 7c06 7c00 8301 a101  ..t.j...|.|.....
+000005f0: a101 7d08 7401 a009 8801 6407 1900 6408  ..}.t.....d...d.
+00000600: 1700 a101 7d09 7c09 a00a 740b a101 7d09  ....}.|...t...}.
+00000610: 7c08 6a0c 7c09 6409 6409 8502 640a 6602  |.j.|.d.d...d.f.
+00000620: 1900 7c09 6409 6409 8502 640b 6602 1900  ..|.d.d...d.f...
+00000630: 6602 1900 a00d 640c a101 7d08 7c07 6a00  f.....d...}.|.j.
+00000640: 7c08 6a00 6b02 73d6 740e 8201 640c 7c08  |.j.k.s.t...d.|.
+00000650: 1800 7c07 1400 7c08 640c 7c07 1800 1400  ..|...|.d.|.....
+00000660: 1700 7d0a 7c0a a00f a100 7d0a 7c0a 5300  ..}.|.....}.|.S.
+00000670: 290d 7a3d 496d 6167 6520 7365 676d 656e  ).z=Image segmen
+00000680: 7461 7469 6f6e 2063 6f6e 7369 7374 656e  tation consisten
+00000690: 6374 206c 6f73 7320 666f 7220 7468 6520  ct loss for the 
+000006a0: 636f 6c6c 6162 6f72 616f 7220 6d6f 6465  collaboraor mode
+000006b0: 6c72 1e00 0000 7214 0000 00e9 ffff ffff  lr....r.........
+000006c0: 6301 0000 0000 0000 0000 0000 0009 0000  c...............
+000006d0: 0005 0000 0013 0000 0073 1c01 0000 7400  .........s....t.
+000006e0: a001 8800 8804 1700 8805 8804 1700 6702  ..............g.
+000006f0: a101 6401 1800 7d01 7c00 6402 1900 7c00  ..d...}.|.d...|.
+00000700: 6403 1900 0200 7d02 7d03 7c00 6404 1900  d.....}.}.|.d...
+00000710: 7d04 8803 6a02 6405 6b04 7266 6406 8801  }...j.d.k.rfd...
+00000720: 6b06 7266 8801 6406 1900 6400 6b09 7266  k.rf..d...d.k.rf
+00000730: 8801 6407 1900 a003 7404 a101 a005 a100  ..d.....t.......
+00000740: 7d05 6e04 6408 7d05 8803 7c05 1900 7d06  }.n.d.}...|...}.
+00000750: 8802 7c05 1900 7d07 7400 6a06 6400 8804  ..|...}.t.j.d...
+00000760: 8502 6400 8804 8502 6602 1900 8804 6405  ..d.....f.....d.
+00000770: 1800 6409 1b00 1800 6409 1300 6409 7c06  ..d.....d...d.|.
+00000780: 1400 7c06 1400 1b00 7d08 7400 a007 7c08  ..|.....}.t...|.
+00000790: 6a08 6408 640a 8d01 0b00 a101 7c07 1400  j.d.d.......|...
+000007a0: 7d08 7c04 7c08 3700 7d04 7c01 6a09 7c02  }.|.|.7.}.|.j.|.
+000007b0: 8804 6409 1a00 1700 7c03 8804 6409 1a00  ..d.....|...d...
+000007c0: 1700 6602 1900 a00a 7c04 a101 7d01 7c01  ..f.....|...}.|.
+000007d0: 8804 6409 1a00 8804 0b00 6409 1a00 8502  ..d.......d.....
+000007e0: 8804 6409 1a00 8804 0b00 6409 1a00 8502  ..d.......d.....
+000007f0: 6602 1900 7d01 7c01 5300 290b 4ee7 0000  f...}.|.S.).N...
+00000800: 0000 8084 2e41 7214 0000 0072 1500 0000  .....Ar....r....
+00000810: 5a0e 696e 7374 616e 6365 5f6c 6f67 6974  Z.instance_logit
+00000820: 7206 0000 005a 0663 6c73 5f69 64da 0863  r....Z.cls_id..c
+00000830: 6174 6567 6f72 7972 0100 0000 7203 0000  ategoryr....r...
+00000840: 0029 01da 0461 7869 7329 0b72 0b00 0000  .)...axis).r....
+00000850: 720f 0000 00da 0473 697a 65da 0661 7374  r......size..ast
+00000860: 7970 65da 0369 6e74 da07 7371 7565 657a  ype..int..squeez
+00000870: 65da 056d 6772 6964 da03 6578 70da 0373  e..mgrid..exp..s
+00000880: 756d 7210 0000 00da 036d 6178 2909 da04  umr......max)...
+00000890: 7072 6564 da05 6c61 6265 6cda 0279 63da  pred..label..yc.
+000008a0: 0278 63da 056c 6f67 6974 da01 63da 0573  .xc..logit..c..s
+000008b0: 6967 6d61 da05 7363 616c 65da 066f 6666  igma..scale..off
+000008c0: 7365 74a9 0672 1600 0000 7226 0000 0072  set..r....r&...r
+000008d0: 2b00 0000 722a 0000 0072 1900 0000 7217  +...r*...r....r.
+000008e0: 0000 0072 1b00 0000 721c 0000 00da 0a5f  ...r....r......_
+000008f0: 6d61 785f 6d65 7267 6541 0000 0073 2600  max_mergeA...s&.
+00000900: 0000 0001 1a01 1201 0803 08ff 0202 06fe  ................
+00000910: 0203 0afd 0205 1402 0402 0801 0801 3201  ..............2.
+00000920: 1801 0802 2401 2802 7a35 7365 6c66 5f73  ....$.(.z5self_s
+00000930: 7570 6572 7669 7365 645f 7365 676d 656e  upervised_segmen
+00000940: 7461 7469 6f6e 5f6c 6f73 732e 3c6c 6f63  tation_loss.<loc
+00000950: 616c 733e 2e5f 6d61 785f 6d65 7267 65da  als>._max_merge.
+00000960: 0766 675f 7072 6564 5a0c 6774 5f6c 6f63  .fg_predZ.gt_loc
+00000970: 6174 696f 6e73 6700 0000 0000 00e0 3f4e  ationsg.......?N
+00000980: 7201 0000 0072 0600 0000 7209 0000 0029  r....r....r....)
+00000990: 1072 0a00 0000 720b 0000 00da 0761 7361  .r....r......asa
+000009a0: 7272 6179 da07 7265 7368 6170 6572 1f00  rray..reshaper..
+000009b0: 0000 7220 0000 0072 2100 0000 da03 6c61  ..r ...r!.....la
+000009c0: 78da 0d73 746f 705f 6772 6164 6965 6e74  x..stop_gradient
+000009d0: da05 666c 6f6f 7272 3100 0000 7232 0000  ..floorr1...r2..
+000009e0: 0072 1000 0000 da03 7365 74da 0e41 7373  .r......set..Ass
+000009f0: 6572 7469 6f6e 4572 726f 7272 2400 0000  ertionErrorr$...
+00000a00: 290b 7225 0000 0072 2600 0000 722a 0000  ).r%...r&...r*..
+00000a10: 0072 2b00 0000 7227 0000 0072 1800 0000  .r+...r'...r....
+00000a20: 7242 0000 0072 4300 0000 5a08 6667 5f6c  rB...rC...Z.fg_l
+00000a30: 6162 656c da04 6c6f 6373 da04 6c6f 7373  abel..locs..loss
+00000a40: 721b 0000 0072 4100 0000 721c 0000 00da  r....rA...r.....
+00000a50: 2173 656c 665f 7375 7065 7276 6973 6564  !self_supervised
+00000a60: 5f73 6567 6d65 6e74 6174 696f 6e5f 6c6f  _segmentation_lo
+00000a70: 7373 3100 0000 731c 0000 0000 0a10 0110  ss1...s.........
+00000a80: 0210 0110 0216 1b10 0118 0212 010a 012c  ...............,
+00000a90: 0210 0318 0208 0272 4d00 0000 e77b 14ae  .......rM....{..
+00000aa0: 47e1 7a84 3fa9 01da 0677 6569 6768 7463  G.z.?....weightc
+00000ab0: 0200 0000 0000 0000 0100 0000 0c00 0000  ................
+00000ac0: 0600 0000 4b00 0000 73ac 0000 007c 0164  ....K...s....|.d
+00000ad0: 0119 006a 005c 037d 047d 057d 067c 0064  ...j.\.}.}.}.|.d
+00000ae0: 0219 0064 036b 057c 0064 0219 007c 046b  ...d.k.|.d...|.k
+00000af0: 0040 007c 0064 0419 0064 036b 0540 007c  .@.|.d...d.k.@.|
+00000b00: 0064 0419 007c 056b 0040 007d 0774 016a  .d...|.k.@.}.t.j
+00000b10: 027c 0064 0519 0064 067c 0764 0764 088d  .|.d...d.|.d.d..
+00000b20: 047d 0874 01a0 037c 0874 0464 09a1 037d  .}.t...|.t.d...}
+00000b30: 0874 056a 06a0 077c 08a1 017c 0064 0519  .t.j...|...|.d..
+00000b40: 006a 0064 0a19 0014 007d 097c 0064 0b19  .j.d.....}.|.d..
+00000b50: 007d 0a74 01a0 087c 0aa1 0174 0417 007d  .}.t...|...t...}
+00000b60: 0b7c 096a 027c 0a64 0c8d 017c 0b1b 007d  .|.j.|.d...|...}
+00000b70: 097c 097c 0214 0053 0029 0d7a 2841 7578  .|.|...S.).z(Aux
+00000b80: 696c 6c61 7279 206c 6f73 7320 746f 2070  illary loss to p
+00000b90: 7265 7665 6e74 206d 6f64 656c 2063 6f6c  revent model col
+00000ba0: 6c61 7073 6572 1e00 0000 7214 0000 0072  lapser....r....r
+00000bb0: 0100 0000 7215 0000 0072 1300 0000 2902  ....r....r....).
+00000bc0: 722c 0000 00e9 feff ffff 5429 0372 2f00  r,........T).r/.
+00000bd0: 0000 da05 7768 6572 65da 086b 6565 7064  ....where..keepd
+00000be0: 696d 7372 2d00 0000 722c 0000 005a 0d69  imsr-...r,...Z.i
+00000bf0: 6e73 7461 6e63 655f 6d61 736b 2901 7252  nstance_mask).rR
+00000c00: 0000 0029 0972 0a00 0000 720b 0000 0072  ...).r....r....r
+00000c10: 3600 0000 720e 0000 00da 0345 5053 721f  6...r......EPSr.
+00000c20: 0000 0072 4600 0000 da05 7273 7172 74da  ...rF.....rsqrt.
+00000c30: 0d63 6f75 6e74 5f6e 6f6e 7a65 726f 290c  .count_nonzero).
+00000c40: 7225 0000 0072 2600 0000 7250 0000 0072  r%...r&...rP...r
+00000c50: 2700 0000 7216 0000 0072 1700 0000 7218  '...r....r....r.
+00000c60: 0000 005a 0a76 616c 6964 5f6c 6f63 73da  ...Z.valid_locs.
+00000c70: 0561 7265 6173 724c 0000 00da 046d 6173  .areasrL.....mas
+00000c80: 6bda 0b6e 5f69 6e73 7461 6e63 6573 721b  k..n_instancesr.
+00000c90: 0000 0072 1b00 0000 721c 0000 00da 0d61  ...r....r......a
+00000ca0: 7578 5f73 697a 655f 6c6f 7373 6d00 0000  ux_size_lossm...
+00000cb0: 732a 0000 0000 0310 030a 010a ff02 020a  s*..............
+00000cc0: fe02 030a fd02 ff02 0704 0106 0002 0002  ................
+00000cd0: 0002 ff06 030e 011a 0208 010e 0110 0272  ...............r
+00000ce0: 5a00 0000 6302 0000 0000 0000 0000 0000  Z...c...........
+00000cf0: 0004 0000 0004 0000 004b 0000 0073 3e00  .........K...s>.
+00000d00: 0000 6401 7c01 6b06 721c 7c01 6401 1900  ..d.|.k.r.|.d...
+00000d10: 6402 6b04 a000 6403 a101 7d03 6e0e 7c01  d.k...d...}.n.|.
+00000d20: 6404 1900 a000 6403 a101 7d03 7401 a002  d.....d...}.t...
+00000d30: 7c00 6405 1900 7c03 a102 a003 a100 5300  |.d...|.......S.
+00000d40: 2906 4e5a 0967 745f 6c61 6265 6c73 7201  ).NZ.gt_labelsr.
+00000d50: 0000 0072 0800 0000 5a0d 6774 5f69 6d61  ...r....Z.gt_ima
+00000d60: 6765 5f6d 6173 6b72 4300 0000 2904 7231  ge_maskrC...).r1
+00000d70: 0000 0072 2200 0000 5a1c 7369 676d 6f69  ...r"...Z.sigmoi
+00000d80: 645f 6269 6e61 7279 5f63 726f 7373 5f65  d_binary_cross_e
+00000d90: 6e74 726f 7079 7224 0000 0029 0472 2500  ntropyr$...).r%.
+00000da0: 0000 da06 6c61 6265 6c73 7227 0000 0072  ....labelsr'...r
+00000db0: 5800 0000 721b 0000 0072 1b00 0000 721c  X...r....r....r.
+00000dc0: 0000 00da 1c73 7570 6572 7669 7365 645f  .....supervised_
+00000dd0: 7365 676d 656e 7461 7469 6f6e 5f6c 6f73  segmentation_los
+00000de0: 7386 0000 0073 0800 0000 0002 0802 1404  s....s..........
+00000df0: 0e02 725c 0000 0063 0000 0000 0000 0000  ..r\...c........
+00000e00: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000e10: 731c 0000 0065 005a 0164 005a 0265 0365  s....e.Z.d.Z.e.e
+00000e20: 0364 019c 0264 0264 0384 045a 0464 0453  .d...d.d...Z.d.S
+00000e30: 0029 05da 0b41 7578 4564 6765 4c6f 7373  .)...AuxEdgeLoss
+00000e40: 2902 7226 0000 0072 2500 0000 6303 0000  ).r&...r%...c...
+00000e50: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+00000e60: 004b 0000 0073 1600 0000 6401 7c02 6b07  .K...s....d.|.k.
+00000e70: 720c 6402 5300 7400 7c02 7c01 8302 5300  r.d.S.t.|.|...S.
+00000e80: 2903 4e5a 1274 7261 696e 696e 675f 6c6f  ).NZ.training_lo
+00000e90: 6361 7469 6f6e 7367 0000 0000 0000 0000  cationsg........
+00000ea0: 2901 7228 0000 00a9 04da 0473 656c 6672  ).r(.......selfr
+00000eb0: 2600 0000 7225 0000 0072 2700 0000 721b  &...r%...r'...r.
+00000ec0: 0000 0072 1b00 0000 721c 0000 00da 0463  ...r....r......c
+00000ed0: 616c 6c94 0000 0073 0600 0000 0006 0801  all....s........
+00000ee0: 0402 7a10 4175 7845 6467 654c 6f73 732e  ..z.AuxEdgeLoss.
+00000ef0: 6361 6c6c 4e29 05da 085f 5f6e 616d 655f  callN)...__name_
+00000f00: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000f10: 5f71 7561 6c6e 616d 655f 5fda 0464 6963  _qualname__..dic
+00000f20: 7472 6000 0000 721b 0000 0072 1b00 0000  tr`...r....r....
+00000f30: 721b 0000 0072 1c00 0000 725d 0000 0093  r....r....r]....
+00000f40: 0000 0073 0600 0000 0803 0201 02fd 725d  ...s..........r]
+00000f50: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000f60: 0000 0000 0400 0000 0000 0000 7326 0000  ............s&..
+00000f70: 0065 005a 0164 005a 0264 0687 0066 0164  .e.Z.d.Z.d...f.d
+00000f80: 0264 0384 095a 0364 0464 0584 005a 0487  .d...Z.d.d...Z..
+00000f90: 0004 005a 0553 0029 07da 0b41 7578 5369  ...Z.S.)...AuxSi
+00000fa0: 7a65 4c6f 7373 724e 0000 0063 0200 0000  zeLossrN...c....
+00000fb0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00000fc0: 0300 0000 7314 0000 0074 0083 00a0 01a1  ....s....t......
+00000fd0: 0001 007c 017c 005f 0264 0053 0029 014e  ...|.|._.d.S.).N
+00000fe0: 2903 da05 7375 7065 72da 085f 5f69 6e69  )...super..__ini
+00000ff0: 745f 5fda 0161 2902 725f 0000 00da 0561  t__..a).r_.....a
+00001000: 6c70 6861 a901 da09 5f5f 636c 6173 735f  lpha....__class_
+00001010: 5f72 1b00 0000 721c 0000 0072 6700 0000  _r....r....rg...
+00001020: a100 0000 7304 0000 0000 010a 017a 1441  ....s........z.A
+00001030: 7578 5369 7a65 4c6f 7373 2e5f 5f69 6e69  uxSizeLoss.__ini
+00001040: 745f 5f63 0300 0000 0000 0000 0000 0000  t__c............
+00001050: 0400 0000 0500 0000 4b00 0000 7310 0000  ........K...s...
+00001060: 0074 007c 027c 017c 006a 0164 018d 0353  .t.|.|.|.j.d...S
+00001070: 0029 024e 724f 0000 0029 0272 5a00 0000  .).NrO...).rZ...
+00001080: 7268 0000 0072 5e00 0000 721b 0000 0072  rh...r^...r....r
+00001090: 1b00 0000 721c 0000 0072 6000 0000 a500  ....r....r`.....
+000010a0: 0000 7302 0000 0000 027a 1041 7578 5369  ..s......z.AuxSi
+000010b0: 7a65 4c6f 7373 2e63 616c 6c29 0172 4e00  zeLoss.call).rN.
+000010c0: 0000 a906 7261 0000 0072 6200 0000 7263  ....ra...rb...rc
+000010d0: 0000 0072 6700 0000 7260 0000 00da 0d5f  ...rg...r`....._
+000010e0: 5f63 6c61 7373 6365 6c6c 5f5f 721b 0000  _classcell__r...
+000010f0: 0072 1b00 0000 726a 0000 0072 1c00 0000  .r....rj...r....
+00001100: 7265 0000 00a0 0000 0073 0400 0000 0801  re.......s......
+00001110: 0e04 7265 0000 0063 0000 0000 0000 0000  ..re...c........
+00001120: 0000 0000 0000 0000 0400 0000 0000 0000  ................
+00001130: 7326 0000 0065 005a 0164 005a 0264 0787  s&...e.Z.d.Z.d..
+00001140: 0066 0164 0364 0484 095a 0364 0564 0684  .f.d.d...Z.d.d..
+00001150: 005a 0487 0004 005a 0553 0029 08da 0a41  .Z.....Z.S.)...A
+00001160: 7578 5365 674c 6f73 7372 2900 0000 e700  uxSegLossr).....
+00001170: 0000 0000 0014 4063 0300 0000 0000 0000  ......@c........
+00001180: 0000 0000 0400 0000 0600 0000 0b00 0000  ................
+00001190: 736a 0000 0074 0083 006a 0166 007c 038e  sj...t...j.f.|..
+000011a0: 0101 007a 0c7c 0164 0119 0001 0057 006e  ...z.|.d.....W.n
+000011b0: 1201 0001 0001 007c 0166 017d 0159 006e  .......|.f.}.Y.n
+000011c0: 0258 007a 0c7c 0264 0119 0001 0057 006e  .X.z.|.d.....W.n
+000011d0: 1201 0001 0001 007c 0266 017d 0259 006e  .......|.f.}.Y.n
+000011e0: 0258 0074 02a0 037c 02a1 017c 005f 0474  .X.t...|...|._.t
+000011f0: 02a0 037c 01a1 017c 005f 0564 0053 0029  ...|...|._.d.S.)
+00001200: 024e 7201 0000 0029 0672 6600 0000 7267  .Nr....).rf...rg
+00001210: 0000 0072 0b00 0000 da05 6172 7261 7972  ...r......arrayr
+00001220: 2b00 0000 722a 0000 0029 0472 5f00 0000  +...r*...).r_...
+00001230: 722a 0000 0072 2b00 0000 7227 0000 0072  r*...r+...r'...r
+00001240: 6a00 0000 721b 0000 0072 1c00 0000 7267  j...r....r....rg
+00001250: 0000 00ab 0000 0073 1600 0000 0001 0e01  .......s........
+00001260: 0201 0c01 0601 0c02 0201 0c01 0601 0c02  ................
+00001270: 0c01 7a13 4175 7853 6567 4c6f 7373 2e5f  ..z.AuxSegLoss._
+00001280: 5f69 6e69 745f 5f63 0300 0000 0000 0000  _init__c........
+00001290: 0000 0000 0400 0000 0600 0000 4b00 0000  ............K...
+000012a0: 7314 0000 0074 007c 027c 017c 006a 017c  s....t.|.|.|.j.|
+000012b0: 006a 0264 018d 0453 0029 024e 2902 722b  .j.d...S.).N).r+
+000012c0: 0000 0072 2a00 0000 2903 724d 0000 0072  ...r*...).rM...r
+000012d0: 2b00 0000 722a 0000 0072 5e00 0000 721b  +...r*...r^...r.
+000012e0: 0000 0072 1b00 0000 721c 0000 0072 6000  ...r....r....r`.
+000012f0: 0000 ba00 0000 730c 0000 0000 0202 0102  ......s.........
+00001300: 0102 0104 0104 fc7a 0f41 7578 5365 674c  .......z.AuxSegL
+00001310: 6f73 732e 6361 6c6c 2902 7229 0000 0072  oss.call).r)...r
+00001320: 6f00 0000 726c 0000 0072 1b00 0000 721b  o...rl...r....r.
+00001330: 0000 0072 6a00 0000 721c 0000 0072 6e00  ...rj...r....rn.
+00001340: 0000 aa00 0000 7304 0000 0008 010e 0f72  ......s........r
+00001350: 6e00 0000 2919 da09 6675 6e63 746f 6f6c  n...)...functool
+00001360: 7372 0200 0000 721f 0000 00da 096a 6178  sr....r......jax
+00001370: 2e6e 756d 7079 da05 6e75 6d70 7972 0b00  .numpy..numpyr..
+00001380: 0000 7222 0000 00da 036f 7073 7204 0000  ..r".....opsr...
+00001390: 005a 0a74 7261 696e 2e6c 6f73 7372 0500  .Z.train.lossr..
+000013a0: 0000 da09 6465 7465 6374 696f 6e72 0700  ....detectionr..
+000013b0: 0000 da05 6669 6e66 6fda 0365 7073 7254  ....finfo..epsrT
+000013c0: 0000 0072 1d00 0000 7228 0000 0072 7000  ...r....r(...rp.
+000013d0: 0000 724d 0000 0072 5a00 0000 725c 0000  ..rM...rZ...r\..
+000013e0: 0072 5d00 0000 7265 0000 0072 6e00 0000  .r]...re...rn...
+000013f0: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
+00001400: 1c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00001410: 0000 7322 0000 000c 0208 010c 0108 020c  ..s"............
+00001420: 010c 010c 020c 0308 1408 130a 010a fb0c  ................
+00001430: 3c0e 1908 0d10 0d10 0a                   <........
```

### Comparing `lacss-0.4.1/lacss/losses/__pycache__/detection.cpython-38.pyc` & `lacss-0.4.2/lacss/losses/__pycache__/detection.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 19:35:53 2023 UTC, .py size: 2423 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 99e8 9964 7709 0000  U..........dw...
+00000000: 550d 0d0a 0000 0000 5a80 9c64 7709 0000  U.......Z..dw...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6404 6405 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6504 6a08 5a09 6509 a00a 6406 a101  ..e.j.Z.e...d...
 00000070: 6a0b 5a0c 6417 6408 6409 8401 5a0d 6418  j.Z.d.d.d...Z.d.
```

### Comparing `lacss-0.4.1/lacss/losses/__pycache__/instance.cpython-38.pyc` & `lacss-0.4.2/lacss/losses/__pycache__/instance.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun 27 18:55:24 2023 UTC, .py size: 5601 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c30 9b64 e115 0000  U........0.d....
+00000000: 550d 0d0a 0000 0000 45fb aa64 7818 0000  U.......E..dx...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 6d04 5a05 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6402 6c06 5a06 6403 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6403 6405 6c09 6d0a 5a0a 0100 6505  ..d.d.l.m.Z...e.
 00000070: a00b 6406 a101 6a0c 5a0d 6407 6408 8400  ..d...j.Z.d.d...
@@ -62,246 +62,287 @@
 000003d0: 0966 0319 001b 007d 057c 067c 0d64 0964  .f.....}.|.|.d.d
 000003e0: 0985 0264 0964 0966 0319 0018 0064 1117  ...d.d.f.....d..
 000003f0: 007c 1364 0964 0985 0264 0964 0966 0319  .|.d.d...d.d.f..
 00000400: 001b 007d 0674 0aa0 0b74 0ca1 017c 1074  ...}.t...t...|.t
 00000410: 046a 0d7c 057c 0667 0264 1064 128d 0264  .j.|.|.g.d.d...d
 00000420: 1118 0083 027d 0b7c 0b64 116b 05a0 0264  .....}.|.d.k...d
 00000430: 0ba1 017d 0b74 0ea0 0f7c 047c 0ba1 027d  ...}.t...|.|...}
-00000440: 1474 107c 147c 0383 0253 0029 137a 374c  .t.|.|...S.).z7L
-00000450: 4143 5353 2069 6e73 7461 6e63 6520 6c6f  ACSS instance lo
-00000460: 7373 2c20 7375 7065 7276 6973 6564 2077  ss, supervised w
-00000470: 6974 6820 7365 676d 656e 7461 7469 6f6e  ith segmentation
-00000480: 206c 6162 656c da0d 696e 7374 616e 6365   label..instance
-00000490: 5f6d 6173 6bda 0e69 6e73 7461 6e63 655f  _mask..instance_
-000004a0: 6c6f 6769 74da 0b69 6e73 7461 6e63 655f  logit..instance_
-000004b0: 7963 da0b 696e 7374 616e 6365 5f78 6329  yc..instance_xc)
-000004c0: 01da 0967 745f 6c61 6265 6c73 721d 0000  ...gt_labelsr...
-000004d0: 00da 0569 6e74 3332 7203 0000 004e 7207  ...int32r....Nr.
-000004e0: 0000 0072 0600 0000 5a09 6774 5f62 626f  ...r....Z.gt_bbo
-000004f0: 7865 7372 0100 0000 da08 6774 5f6d 6173  xesr......gt_mas
-00000500: 6b73 e904 0000 0072 0800 0000 e700 0000  ks.....r........
-00000510: 0000 00e0 3f29 0172 0900 0000 2911 da0a  ....?).r....)...
-00000520: 6973 696e 7374 616e 6365 da04 6469 6374  isinstance..dict
-00000530: da06 6173 7479 7065 720d 0000 0072 0e00  ..astyper....r..
-00000540: 0000 da03 7061 64da 0661 7261 6e67 65da  ....pad..arange.
-00000550: 0873 7761 7061 7865 73da 036c 656e da07  .swapaxes..len..
-00000560: 7371 7565 657a 65da 036a 6178 da04 766d  squeeze..jax..vm
-00000570: 6170 7204 0000 00da 0573 7461 636b da05  apr......stack..
-00000580: 6f70 7461 78da 1c73 6967 6d6f 6964 5f62  optax..sigmoid_b
-00000590: 696e 6172 795f 6372 6f73 735f 656e 7472  inary_cross_entr
-000005a0: 6f70 7972 1800 0000 2915 da05 7072 6564  opyr....)...pred
-000005b0: 73da 066c 6162 656c 73da 066b 7761 7267  s..labels..kwarg
-000005c0: 7372 1900 0000 721a 0000 00da 0279 63da  sr....r......yc.
-000005d0: 0278 6372 1d00 0000 da09 6e5f 7061 7463  .xcr......n_patc
-000005e0: 6865 73da 0270 73da 015f da0a 6774 5f70  hes..ps.._..gt_p
-000005f0: 6174 6368 6573 da02 7930 da02 7830 da02  atches..y0..x0..
-00000600: 7931 da02 7831 5a07 6774 5f73 6567 735a  y1..x1Z.gt_segsZ
-00000610: 0873 6567 5f73 697a 65da 0268 73da 0277  .seg_size..hs..w
-00000620: 7372 1300 0000 7216 0000 0072 1600 0000  sr....r....r....
-00000630: 7217 0000 00da 1873 7570 6572 7669 7365  r......supervise
-00000640: 645f 696e 7374 616e 6365 5f6c 6f73 7318  d_instance_loss.
-00000650: 0000 0073 3c00 0000 0003 0801 0801 0801  ...s<...........
-00000660: 0802 0a01 0a02 0801 0e02 0c02 1001 1a01  ................
-00000670: 1aff 0403 0c03 1a01 0801 0e01 0a01 0a03  ................
-00000680: 0c01 0c03 2c01 2c03 0801 0201 14fe 0404  ....,.,.........
-00000690: 0e02 0c02 723e 0000 0054 a901 da0a 736f  ....r>...T....so
-000006a0: 6674 5f6c 6162 656c 6301 0000 0000 0000  ft_labelc.......
-000006b0: 0001 0000 0011 0000 0006 0000 0043 0000  .............C..
-000006c0: 0073 5e01 0000 7c00 6401 1900 7d02 7c00  .s^...|.d...}.|.
-000006d0: 6402 1900 7d03 7c00 6403 1900 7d04 7c00  d...}.|.d...}.|.
-000006e0: 6404 1900 7d05 7c00 6405 1900 7d06 7c03  d...}.|.d...}.|.
-000006f0: 6a00 6406 1900 7d07 7c07 6407 1a00 6407  j.d...}.|.d...d.
-00000700: 1700 7d08 7c05 7c08 3700 7d05 7c06 7c08  ..}.|.|.7.}.|.|.
-00000710: 3700 7d06 7401 6a02 a003 7401 6a04 a005  7.}.t.j...t.j...
-00000720: 7c00 6408 1900 a101 a101 7d09 7406 a007  |.d.......}.t...
-00000730: 7c09 7c08 a102 7d0a 7c01 72d6 7c0a 7c05  |.|...}.|.r.|.|.
-00000740: 7c06 6602 1900 7d0b 6409 7c0b 1800 7c03  |.f...}.d.|...|.
-00000750: 1400 7c0b 6409 7c03 1800 1400 1700 7d0c  ..|.d.|.......}.
-00000760: 7406 a008 7c0a a101 7d0d 7c0d 6a09 7c05  t...|...}.|.j.|.
-00000770: 7c06 6602 1900 a00a 7c03 a101 7d0d 7c0d  |.f.....|...}.|.
-00000780: 7c05 7c06 6602 1900 7c03 1800 7d0e 7c0c  |.|.f...|...}.|.
-00000790: 7c03 7c0e 1400 1700 7d0c 6e7e 7c0a 640a  |.|.....}.n~|.d.
-000007a0: 6b04 a00b 7c03 6a0c a101 7d0a 7c0a 7c05  k...|.j...}.|.|.
-000007b0: 7c06 6602 1900 7d0b 6409 7c0b 1800 7c03  |.f...}.d.|...|.
-000007c0: 1400 7c0b 6409 7c03 1800 1400 1700 7d0c  ..|.d.|.......}.
-000007d0: 7406 a008 7c0a a101 7d0f 7401 6a04 a00d  t...|...}.t.j...
-000007e0: 7c04 0b00 a101 0b00 7d10 7c0f 6a09 7c05  |.......}.|.j.|.
-000007f0: 7c06 6602 1900 a00a 7c10 a101 7d0f 7c0f  |.f.....|...}.|.
-00000800: 7c05 7c06 6602 1900 7c10 1800 7d10 7c0c  |.|.f...|...}.|.
-00000810: 7c03 7c10 1400 1700 7d0c 740e 7c0c 7c02  |.|.....}.t.|.|.
-00000820: 8302 5300 290b 7a21 4c41 4353 5320 696e  ..S.).z!LACSS in
-00000830: 7374 616e 6365 206c 6f73 732c 2075 6e73  stance loss, uns
-00000840: 7570 6572 7669 7365 6472 1900 0000 da0f  upervisedr......
-00000850: 696e 7374 616e 6365 5f6f 7574 7075 7472  instance_outputr
-00000860: 1a00 0000 721b 0000 0072 1c00 0000 7208  ....r....r....r.
-00000870: 0000 0072 0300 0000 da07 6667 5f70 7265  ...r......fg_pre
-00000880: 64e7 0000 0000 0000 f03f 7221 0000 0029  d........?r!...)
-00000890: 0f72 0d00 0000 722a 0000 00da 036c 6178  .r....r*.....lax
-000008a0: da0d 7374 6f70 5f67 7261 6469 656e 74da  ..stop_gradient.
-000008b0: 026e 6eda 0773 6967 6d6f 6964 720e 0000  .nn..sigmoidr...
-000008c0: 0072 2500 0000 da0a 7a65 726f 735f 6c69  .r%.....zeros_li
-000008d0: 6b65 da02 6174 da03 6164 6472 2400 0000  ke..at..addr$...
-000008e0: da05 6474 7970 65da 0b6c 6f67 5f73 6967  ..dtype..log_sig
-000008f0: 6d6f 6964 7218 0000 0029 1172 2f00 0000  moidr....).r/...
-00000900: 7240 0000 0072 1900 0000 da09 696e 7374  r@...r......inst
-00000910: 616e 6365 7372 1a00 0000 7232 0000 0072  ancesr....r2...r
-00000920: 3300 0000 da0a 7061 7463 685f 7369 7a65  3.....patch_size
-00000930: da0c 7061 6464 696e 675f 7369 7a65 da0b  ..padding_size..
-00000940: 6269 6e61 7279 5f6d 6173 6bda 0373 6567  binary_mask..seg
-00000950: da09 7365 675f 7061 7463 6872 1300 0000  ..seg_patchr....
-00000960: 5a0c 696e 7374 616e 6365 5f73 756d 5a0e  Z.instance_sumZ.
-00000970: 696e 7374 616e 6365 5f73 756d 5f69 da0a  instance_sum_i..
-00000980: 6c6f 675f 7969 5f73 756d da06 6c6f 675f  log_yi_sum..log_
-00000990: 7969 7216 0000 0072 1600 0000 7217 0000  yir....r....r...
-000009a0: 00da 1d73 656c 665f 7375 7065 7276 6973  ...self_supervis
-000009b0: 6564 5f69 6e73 7461 6e63 655f 6c6f 7373  ed_instance_loss
-000009c0: 4900 0000 7336 0000 0000 0308 0108 0108  I...s6..........
-000009d0: 0108 0108 020a 010c 0108 0108 0218 010c  ................
-000009e0: 0204 010c 0218 020a 0114 0110 020e 0310  ................
-000009f0: 010c 0218 020a 0110 0114 0110 020c 0272  ...............r
-00000a00: 5500 0000 46a9 01da 0b69 676e 6f72 655f  U...F....ignore_
-00000a10: 6d61 736b 6303 0000 0000 0000 0001 0000  maskc...........
-00000a20: 0011 0000 0005 0000 004b 0000 0073 2a01  .........K...s*.
-00000a30: 0000 7c00 6401 1900 7d05 7c00 6402 1900  ..|.d...}.|.d...
-00000a40: 7d06 7c00 6403 1900 7d07 7c00 6404 1900  }.|.d...}.|.d...
-00000a50: 7d08 7c00 6405 1900 7d09 7c06 6a00 6406  }.|.d...}.|.j.d.
-00000a60: 1900 7d0a 7c0a 6407 1a00 6407 1700 7d0b  ..}.|.d...d...}.
-00000a70: 7c08 7c0b 3700 7d08 7c09 7c0b 3700 7d09  |.|.7.}.|.|.7.}.
-00000a80: 7c03 7282 7401 a002 7c02 6408 1900 6a00  |.r.t...|.d...j.
-00000a90: 6409 6406 8502 1900 a101 7d0c 7401 a003  d.d.......}.t...
-00000aa0: 7c0c 7c0b a102 7d0c 7401 a004 7c06 a101  |.|...}.t...|...
-00000ab0: 7d0d 6e54 7405 7c01 7406 8302 729c 7c01  }.nTt.|.t...r.|.
-00000ac0: 640a 1900 a007 640b a101 7d0c 6e0a 7c01  d.....d...}.n.|.
-00000ad0: a007 640b a101 7d0c 7401 a003 7c0c 7c0b  ..d...}.t...|.|.
-00000ae0: a102 7d0c 7c0c 7c08 7c09 6602 1900 7d0e  ..}.|.|.|.f...}.
-00000af0: 640c 7c0e 1800 7c06 1400 7c0e 640c 7c06  d.|...|...|.d.|.
-00000b00: 1800 1400 1700 7d0d 7401 a004 7c0c a101  ......}.t...|...
-00000b10: 7d0f 7408 6a09 a00a 7c07 0b00 a101 0b00  }.t.j...|.......
-00000b20: 7d10 7c0f 6a0b 7c08 7c09 6602 1900 a00c  }.|.j.|.|.f.....
-00000b30: 7c10 a101 7d0f 7c0f 7c08 7c09 6602 1900  |...}.|.|.|.f...
-00000b40: 7c10 1800 7d10 7c0d 7c06 7c10 1400 1700  |...}.|.|.|.....
-00000b50: 7d0d 740d 7c0d 7c05 8302 5300 290d 7a2f  }.t.|.|...S.).z/
-00000b60: 4c61 6373 7320 696e 7374 616e 6365 206c  Lacss instance l
-00000b70: 6f73 732c 2073 7570 6572 7669 7365 6420  oss, supervised 
-00000b80: 7769 7468 2069 6d61 6765 206d 6173 6b72  with image maskr
-00000b90: 1900 0000 7241 0000 0072 1a00 0000 721b  ....rA...r....r.
-00000ba0: 0000 0072 1c00 0000 7208 0000 0072 0300  ...r....r....r..
-00000bb0: 0000 da05 696d 6167 654e da07 6774 5f6d  ....imageN..gt_m
-00000bc0: 6173 6b72 0600 0000 7243 0000 0029 0e72  askr....rC...).r
-00000bd0: 0d00 0000 720e 0000 00da 057a 6572 6f73  ....r......zeros
-00000be0: 7225 0000 0072 4800 0000 7222 0000 0072  r%...rH...r"...r
-00000bf0: 2300 0000 7224 0000 0072 2a00 0000 7246  #...r$...r*...rF
-00000c00: 0000 0072 4c00 0000 7249 0000 0072 4a00  ...rL...rI...rJ.
-00000c10: 0000 7218 0000 0029 1172 2f00 0000 7230  ..r....).r/...r0
-00000c20: 0000 00da 0669 6e70 7574 7372 5700 0000  .....inputsrW...
-00000c30: 7231 0000 0072 1900 0000 724d 0000 0072  r1...r....rM...r
-00000c40: 1a00 0000 7232 0000 0072 3300 0000 724e  ....r2...r3...rN
-00000c50: 0000 0072 4f00 0000 7251 0000 0072 1300  ...rO...rQ...r..
-00000c60: 0000 7252 0000 0072 5300 0000 7254 0000  ..rR...rS...rT..
-00000c70: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00000c80: da1f 7765 616b 6c79 5f73 7570 6572 7669  ..weakly_supervi
-00000c90: 7365 645f 696e 7374 616e 6365 5f6c 6f73  sed_instance_los
-00000ca0: 7375 0000 0073 3200 0000 0005 0801 0801  su...s2.........
-00000cb0: 0801 0801 0802 0a01 0c01 0801 0802 0401  ................
-00000cc0: 1801 0c01 0c02 0a01 1002 0a01 0c01 0c01  ................
-00000cd0: 1802 0a02 1001 1401 1002 0c02 725c 0000  ............r\..
-00000ce0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000cf0: 0000 0300 0000 4000 0000 731c 0000 0065  ......@...s....e
-00000d00: 005a 0164 005a 0265 0365 0364 019c 0264  .Z.d.Z.e.e.d...d
-00000d10: 0264 0384 045a 0464 0453 0029 05da 1653  .d...Z.d.S.)...S
-00000d20: 7570 6572 7669 7365 6449 6e73 7461 6e63  upervisedInstanc
-00000d30: 654c 6f73 7329 0272 2f00 0000 7230 0000  eLoss).r/...r0..
-00000d40: 0063 0300 0000 0000 0000 0000 0000 0400  .c..............
-00000d50: 0000 0300 0000 4b00 0000 730a 0000 0074  ......K...s....t
-00000d60: 007c 017c 0283 0253 00a9 014e 2901 723e  .|.|...S...N).r>
-00000d70: 0000 0029 04da 0473 656c 6672 2f00 0000  ...)...selfr/...
-00000d80: 7230 0000 0072 3100 0000 7216 0000 0072  r0...r1...r....r
-00000d90: 1600 0000 7217 0000 00da 0463 616c 6c9e  ....r......call.
-00000da0: 0000 0073 0200 0000 0001 7a1b 5375 7065  ...s......z.Supe
-00000db0: 7276 6973 6564 496e 7374 616e 6365 4c6f  rvisedInstanceLo
-00000dc0: 7373 2e63 616c 6c4e 2905 da08 5f5f 6e61  ss.callN)...__na
-00000dd0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000de0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7223  ..__qualname__r#
-00000df0: 0000 0072 6000 0000 7216 0000 0072 1600  ...r`...r....r..
-00000e00: 0000 7216 0000 0072 1700 0000 725d 0000  ..r....r....r]..
-00000e10: 009d 0000 0073 0200 0000 0801 725d 0000  .....s......r]..
-00000e20: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000e30: 0000 0500 0000 0000 0000 7332 0000 0065  ..........s2...e
-00000e40: 005a 0164 005a 0264 0865 0364 029c 0187  .Z.d.Z.d.e.d....
-00000e50: 0066 0164 0364 0484 0d5a 0465 0564 059c  .f.d.d...Z.e.d..
-00000e60: 0164 0664 0784 045a 0687 0004 005a 0753  .d.d...Z.....Z.S
-00000e70: 0029 09da 1a53 656c 6653 7570 6572 7669  .)...SelfSupervi
-00000e80: 7365 6449 6e73 7461 6e63 654c 6f73 7354  sedInstanceLossT
-00000e90: 723f 0000 0063 0200 0000 0000 0000 0000  r?...c..........
-00000ea0: 0000 0400 0000 0300 0000 0f00 0000 7318  ..............s.
-00000eb0: 0000 0074 0083 006a 017c 027c 038e 0101  ...t...j.|.|....
-00000ec0: 007c 017c 005f 0264 0053 0072 5e00 0000  .|.|._.d.S.r^...
-00000ed0: 2903 da05 7375 7065 72da 085f 5f69 6e69  )...super..__ini
-00000ee0: 745f 5f72 4000 0000 2904 725f 0000 0072  t__r@...).r_...r
-00000ef0: 4000 0000 da04 6172 6773 7231 0000 00a9  @.....argsr1....
-00000f00: 01da 095f 5f63 6c61 7373 5f5f 7216 0000  ...__class__r...
-00000f10: 0072 1700 0000 7266 0000 00a3 0000 0073  .r....rf.......s
-00000f20: 0400 0000 0001 0e01 7a23 5365 6c66 5375  ........z#SelfSu
-00000f30: 7065 7276 6973 6564 496e 7374 616e 6365  pervisedInstance
-00000f40: 4c6f 7373 2e5f 5f69 6e69 745f 5f29 0172  Loss.__init__).r
-00000f50: 2f00 0000 6302 0000 0000 0000 0000 0000  /...c...........
-00000f60: 0003 0000 0004 0000 004b 0000 0073 0e00  .........K...s..
-00000f70: 0000 7400 7c01 7c00 6a01 6401 8d02 5300  ..t.|.|.j.d...S.
-00000f80: 2902 4e72 3f00 0000 2902 7255 0000 0072  ).Nr?...).rU...r
-00000f90: 4000 0000 2903 725f 0000 0072 2f00 0000  @...).r_...r/...
-00000fa0: 7231 0000 0072 1600 0000 7216 0000 0072  r1...r....r....r
-00000fb0: 1700 0000 7260 0000 00a7 0000 0073 0200  ....r`.......s..
-00000fc0: 0000 0001 7a1f 5365 6c66 5375 7065 7276  ....z.SelfSuperv
-00000fd0: 6973 6564 496e 7374 616e 6365 4c6f 7373  isedInstanceLoss
-00000fe0: 2e63 616c 6c29 0154 2908 7261 0000 0072  .call).T).ra...r
-00000ff0: 6200 0000 7263 0000 00da 0462 6f6f 6c72  b...rc.....boolr
-00001000: 6600 0000 7223 0000 0072 6000 0000 da0d  f...r#...r`.....
-00001010: 5f5f 636c 6173 7363 656c 6c5f 5f72 1600  __classcell__r..
-00001020: 0000 7216 0000 0072 6800 0000 7217 0000  ..r....rh...r...
-00001030: 0072 6400 0000 a200 0000 7304 0000 0008  .rd.......s.....
-00001040: 0114 0472 6400 0000 6300 0000 0000 0000  ...rd...c.......
-00001050: 0000 0000 0000 0000 0005 0000 0000 0000  ................
-00001060: 0073 2c00 0000 6500 5a01 6400 5a02 6407  .s,...e.Z.d.Z.d.
-00001070: 6503 6402 9c01 8700 6601 6403 6404 840d  e.d.....f.d.d...
-00001080: 5a04 6405 6406 8400 5a05 8700 0400 5a06  Z.d.d...Z.....Z.
-00001090: 5300 2908 da1c 5765 616b 6c79 5375 7065  S.)...WeaklySupe
-000010a0: 7276 6973 6564 496e 7374 616e 6365 4c6f  rvisedInstanceLo
-000010b0: 7373 4672 5600 0000 6302 0000 0000 0000  ssFrV...c.......
-000010c0: 0000 0000 0004 0000 0003 0000 000f 0000  ................
-000010d0: 0073 1800 0000 7400 8300 6a01 7c02 7c03  .s....t...j.|.|.
-000010e0: 8e01 0100 7c01 7c00 5f02 6400 5300 725e  ....|.|._.d.S.r^
-000010f0: 0000 0029 0372 6500 0000 7266 0000 0072  ...).re...rf...r
-00001100: 5700 0000 2904 725f 0000 0072 5700 0000  W...).r_...rW...
-00001110: 7267 0000 0072 3100 0000 7268 0000 0072  rg...r1...rh...r
-00001120: 1600 0000 7217 0000 0072 6600 0000 ac00  ....r....rf.....
-00001130: 0000 7304 0000 0000 010e 017a 2557 6561  ..s........z%Wea
-00001140: 6b6c 7953 7570 6572 7669 7365 6449 6e73  klySupervisedIns
-00001150: 7461 6e63 654c 6f73 732e 5f5f 696e 6974  tanceLoss.__init
-00001160: 5f5f 6301 0000 0000 0000 0003 0000 0004  __c.............
-00001170: 0000 0006 0000 0043 0000 0073 1200 0000  .......C...s....
-00001180: 7400 7c01 7c02 7c03 7c00 6a01 6401 8d04  t.|.|.|.|.j.d...
-00001190: 5300 2902 4e72 5600 0000 2902 725c 0000  S.).NrV...).r\..
-000011a0: 0072 5700 0000 2904 725f 0000 0072 2f00  .rW...).r_...r/.
-000011b0: 0000 7230 0000 0072 5b00 0000 7216 0000  ..r0...r[...r...
-000011c0: 0072 1600 0000 7217 0000 0072 6000 0000  .r....r....r`...
-000011d0: b000 0000 730c 0000 0000 0102 0102 0002  ....s...........
-000011e0: 0002 0004 ff7a 2157 6561 6b6c 7953 7570  .....z!WeaklySup
-000011f0: 6572 7669 7365 6449 6e73 7461 6e63 654c  ervisedInstanceL
-00001200: 6f73 732e 6361 6c6c 2901 4629 0772 6100  oss.call).F).ra.
-00001210: 0000 7262 0000 0072 6300 0000 726a 0000  ..rb...rc...rj..
-00001220: 0072 6600 0000 7260 0000 0072 6b00 0000  .rf...r`...rk...
-00001230: 7216 0000 0072 1600 0000 7268 0000 0072  r....r....rh...r
-00001240: 1700 0000 726c 0000 00ab 0000 0073 0400  ....rl.......s..
-00001250: 0000 0801 1404 726c 0000 0029 16da 0966  ......rl...)...f
-00001260: 756e 6374 6f6f 6c73 7202 0000 0072 2a00  unctoolsr....r*.
-00001270: 0000 da09 6a61 782e 6e75 6d70 79da 056e  ....jax.numpy..n
-00001280: 756d 7079 720e 0000 0072 2d00 0000 da03  umpyr....r-.....
-00001290: 6f70 7372 0400 0000 da0a 7472 6169 6e2e  opsr......train.
-000012a0: 6c6f 7373 7205 0000 00da 0566 696e 666f  lossr......finfo
-000012b0: da03 6570 7372 1000 0000 7218 0000 0072  ..epsr....r....r
-000012c0: 3e00 0000 726a 0000 0072 5500 0000 725c  >...rj...rU...r\
-000012d0: 0000 0072 5d00 0000 7264 0000 0072 6c00  ...r]...rd...rl.
-000012e0: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
-000012f0: 0072 1700 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00001300: 0100 0000 7320 0000 000c 0208 010c 0108  ....s ..........
-00001310: 020c 010c 020c 0308 0b08 3114 2d02 ff04  ..........1.-...
-00001320: 0102 ff0c 2810 0510 09                   ....(....
+00000440: 1474 107c 147c 0383 0253 0029 1361 f601  .t.|.|...S.).a..
+00000450: 0000 4c41 4353 5320 696e 7374 616e 6365  ..LACSS instance
+00000460: 206c 6f73 732c 2073 7570 6572 7669 7365   loss, supervise
+00000470: 6420 7769 7468 2073 6567 6d65 6e74 6174  d with segmentat
+00000480: 696f 6e20 6c61 6265 6c0a 0a20 2020 2041  ion label..    A
+00000490: 7267 733a 0a20 2020 2020 2020 2070 7265  rgs:.        pre
+000004a0: 6473 3a20 4d6f 6465 6c20 7072 6564 6963  ds: Model predic
+000004b0: 7469 6f6e 730a 2020 2020 2020 2020 6c61  tions.        la
+000004c0: 6265 6c73 3a20 4c61 6265 6c20 6469 6374  bels: Label dict
+000004d0: 696f 6e61 7279 2e20 5477 6f20 7479 7065  ionary. Two type
+000004e0: 7320 6f66 2073 6567 6d65 6e74 6174 696f  s of segmentatio
+000004f0: 6e20 6c61 6265 6c73 2061 7265 2061 6363  n labels are acc
+00000500: 6570 7465 642e 0a20 2020 2020 2020 2020  epted..         
+00000510: 2020 2049 6620 6060 606c 6162 656c 735b     If ```labels[
+00000520: 2267 745f 6c61 6265 6c73 225d 6060 6020  "gt_labels"]``` 
+00000530: 6973 2070 726f 7669 6465 642c 2069 7473  is provided, its
+00000540: 2076 616c 7565 2069 7320 7472 6561 7465   value is treate
+00000550: 6420 6173 2070 6978 656c 0a20 2020 2020  d as pixel.     
+00000560: 2020 2020 2020 206c 6162 656c 7320 6f66         labels of
+00000570: 2074 6865 2069 6d61 6765 2e20 4f74 6865   the image. Othe
+00000580: 7277 6973 6465 2c20 6f6e 6520 6d75 6368  rwisde, one much
+00000590: 2073 7570 706c 7920 626f 7468 2060 6060   supply both ```
+000005a0: 6c61 6265 6c73 5b22 6774 5f62 626f 7865  labels["gt_bboxe
+000005b0: 7322 5d60 6060 0a20 2020 2020 2020 2020  s"]```.         
+000005c0: 2020 2061 6e64 2060 6060 6c61 6265 6c73     and ```labels
+000005d0: 5b22 6774 5f6d 6173 6b73 225d 6060 602e  ["gt_masks"]```.
+000005e0: 2054 6865 2067 745f 6d61 736b 7320 6973   The gt_masks is
+000005f0: 2061 2033 4420 6172 7261 7920 7265 7072   a 3D array repr
+00000600: 6573 656e 7469 6e67 2061 6c6c 0a20 2020  esenting all.   
+00000610: 2020 2020 2020 2020 2073 6567 6d65 6e74           segment
+00000620: 6174 696f 6e20 7265 7369 7a65 6420 746f  ation resized to
+00000630: 2061 2066 6978 6564 2064 696d 656e 7369   a fixed dimensi
+00000640: 6f6e 2e0a 2020 2020 da0d 696e 7374 616e  on..    ..instan
+00000650: 6365 5f6d 6173 6bda 0e69 6e73 7461 6e63  ce_mask..instanc
+00000660: 655f 6c6f 6769 74da 0b69 6e73 7461 6e63  e_logit..instanc
+00000670: 655f 7963 da0b 696e 7374 616e 6365 5f78  e_yc..instance_x
+00000680: 6329 01da 0967 745f 6c61 6265 6c73 721d  c)...gt_labelsr.
+00000690: 0000 00da 0569 6e74 3332 7203 0000 004e  .....int32r....N
+000006a0: 7207 0000 0072 0600 0000 da09 6774 5f62  r....r......gt_b
+000006b0: 626f 7865 7372 0100 0000 da08 6774 5f6d  boxesr......gt_m
+000006c0: 6173 6b73 e904 0000 0072 0800 0000 e700  asks.....r......
+000006d0: 0000 0000 00e0 3f29 0172 0900 0000 2911  ......?).r....).
+000006e0: da0a 6973 696e 7374 616e 6365 da04 6469  ..isinstance..di
+000006f0: 6374 da06 6173 7479 7065 720d 0000 0072  ct..astyper....r
+00000700: 0e00 0000 da03 7061 64da 0661 7261 6e67  ......pad..arang
+00000710: 65da 0873 7761 7061 7865 73da 036c 656e  e..swapaxes..len
+00000720: da07 7371 7565 657a 65da 036a 6178 da04  ..squeeze..jax..
+00000730: 766d 6170 7204 0000 00da 0573 7461 636b  vmapr......stack
+00000740: da05 6f70 7461 78da 1c73 6967 6d6f 6964  ..optax..sigmoid
+00000750: 5f62 696e 6172 795f 6372 6f73 735f 656e  _binary_cross_en
+00000760: 7472 6f70 7972 1800 0000 2915 da05 7072  tropyr....)...pr
+00000770: 6564 73da 066c 6162 656c 73da 066b 7761  eds..labels..kwa
+00000780: 7267 7372 1900 0000 721a 0000 00da 0279  rgsr....r......y
+00000790: 63da 0278 6372 1d00 0000 da09 6e5f 7061  c..xcr......n_pa
+000007a0: 7463 6865 73da 0270 73da 015f da0a 6774  tches..ps.._..gt
+000007b0: 5f70 6174 6368 6573 da02 7930 da02 7830  _patches..y0..x0
+000007c0: da02 7931 da02 7831 5a07 6774 5f73 6567  ..y1..x1Z.gt_seg
+000007d0: 735a 0873 6567 5f73 697a 65da 0268 73da  sZ.seg_size..hs.
+000007e0: 0277 7372 1300 0000 7216 0000 0072 1600  .wsr....r....r..
+000007f0: 0000 7217 0000 00da 1873 7570 6572 7669  ..r......supervi
+00000800: 7365 645f 696e 7374 616e 6365 5f6c 6f73  sed_instance_los
+00000810: 7318 0000 0073 3c00 0000 000c 0801 0801  s....s<.........
+00000820: 0801 0802 0a01 0a02 0801 0e02 0c02 1001  ................
+00000830: 1a01 1aff 0403 0c03 1a01 0801 0e01 0a01  ................
+00000840: 0a03 0c01 0c03 2c01 2c03 0801 0201 14fe  ......,.,.......
+00000850: 0404 0e02 0c02 723f 0000 0054 a901 da0a  ......r?...T....
+00000860: 736f 6674 5f6c 6162 656c 6301 0000 0000  soft_labelc.....
+00000870: 0000 0001 0000 0012 0000 0006 0000 004b  ...............K
+00000880: 0000 0073 5e01 0000 7c00 6401 1900 7d03  ...s^...|.d...}.
+00000890: 7c00 6402 1900 7d04 7c00 6403 1900 7d05  |.d...}.|.d...}.
+000008a0: 7c00 6404 1900 7d06 7c00 6405 1900 7d07  |.d...}.|.d...}.
+000008b0: 7c04 6a00 6406 1900 7d08 7c08 6407 1a00  |.j.d...}.|.d...
+000008c0: 6407 1700 7d09 7c06 7c09 3700 7d06 7c07  d...}.|.|.7.}.|.
+000008d0: 7c09 3700 7d07 7401 6a02 a003 7401 6a04  |.7.}.t.j...t.j.
+000008e0: a005 7c00 6408 1900 a101 a101 7d0a 7406  ..|.d.......}.t.
+000008f0: a007 7c0a 7c09 a102 7d0b 7c01 72d6 7c0b  ..|.|...}.|.r.|.
+00000900: 7c06 7c07 6602 1900 7d0c 6409 7c0c 1800  |.|.f...}.d.|...
+00000910: 7c04 1400 7c0c 6409 7c04 1800 1400 1700  |...|.d.|.......
+00000920: 7d0d 7406 a008 7c0b a101 7d0e 7c0e 6a09  }.t...|...}.|.j.
+00000930: 7c06 7c07 6602 1900 a00a 7c04 a101 7d0e  |.|.f.....|...}.
+00000940: 7c0e 7c06 7c07 6602 1900 7c04 1800 7d0f  |.|.|.f...|...}.
+00000950: 7c0d 7c04 7c0f 1400 1700 7d0d 6e7e 7c0b  |.|.|.....}.n~|.
+00000960: 640a 6b04 a00b 7c04 6a0c a101 7d0b 7c0b  d.k...|.j...}.|.
+00000970: 7c06 7c07 6602 1900 7d0c 6409 7c0c 1800  |.|.f...}.d.|...
+00000980: 7c04 1400 7c0c 6409 7c04 1800 1400 1700  |...|.d.|.......
+00000990: 7d0d 7406 a008 7c0b a101 7d10 7401 6a04  }.t...|...}.t.j.
+000009a0: a00d 7c05 0b00 a101 0b00 7d11 7c10 6a09  ..|.......}.|.j.
+000009b0: 7c06 7c07 6602 1900 a00a 7c11 a101 7d10  |.|.f.....|...}.
+000009c0: 7c10 7c06 7c07 6602 1900 7c11 1800 7d11  |.|.|.f...|...}.
+000009d0: 7c0d 7c04 7c11 1400 1700 7d0d 740e 7c0d  |.|.|.....}.t.|.
+000009e0: 7c03 8302 5300 290b 7ad0 556e 7375 7065  |...S.).z.Unsupe
+000009f0: 7276 6973 6564 2069 6e73 7461 6e63 6520  rvised instance 
+00000a00: 6c6f 7373 0a0a 2020 2020 4172 6773 3a0a  loss..    Args:.
+00000a10: 2020 2020 2020 2020 7072 6564 733a 204d          preds: M
+00000a20: 6f64 656c 2070 7265 6469 6374 696f 6e20  odel prediction 
+00000a30: 6469 6374 2e0a 2020 2020 2020 2020 736f  dict..        so
+00000a40: 6674 5f6c 6162 656c 3a20 4966 2046 616c  ft_label: If Fal
+00000a50: 7365 2c20 6974 2063 6f6e 7665 7274 6573  se, it convertes
+00000a60: 2069 6d61 6765 206d 6173 6b20 7072 6564   image mask pred
+00000a70: 6963 7469 6f6e 2074 6f20 6861 7264 206c  iction to hard l
+00000a80: 6162 656c 0a20 2020 2020 2020 2020 2020  abel.           
+00000a90: 2028 6965 2e20 3020 6f72 2031 292c 2062   (ie. 0 or 1), b
+00000aa0: 6566 6f72 6520 636f 6d70 7574 696e 6720  efore computing 
+00000ab0: 6c6f 7373 2e0a 2020 2020 7219 0000 00da  loss..    r.....
+00000ac0: 0f69 6e73 7461 6e63 655f 6f75 7470 7574  .instance_output
+00000ad0: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+00000ae0: 0800 0000 7203 0000 00da 0766 675f 7072  ....r......fg_pr
+00000af0: 6564 e700 0000 0000 00f0 3f72 2200 0000  ed........?r"...
+00000b00: 290f 720d 0000 0072 2b00 0000 da03 6c61  ).r....r+.....la
+00000b10: 78da 0d73 746f 705f 6772 6164 6965 6e74  x..stop_gradient
+00000b20: da02 6e6e da07 7369 676d 6f69 6472 0e00  ..nn..sigmoidr..
+00000b30: 0000 7226 0000 00da 0a7a 6572 6f73 5f6c  ..r&.....zeros_l
+00000b40: 696b 65da 0261 74da 0361 6464 7225 0000  ike..at..addr%..
+00000b50: 00da 0564 7479 7065 da0b 6c6f 675f 7369  ...dtype..log_si
+00000b60: 676d 6f69 6472 1800 0000 2912 7230 0000  gmoidr....).r0..
+00000b70: 0072 4100 0000 7232 0000 0072 1900 0000  .rA...r2...r....
+00000b80: da09 696e 7374 616e 6365 7372 1a00 0000  ..instancesr....
+00000b90: 7233 0000 0072 3400 0000 da0a 7061 7463  r3...r4.....patc
+00000ba0: 685f 7369 7a65 da0c 7061 6464 696e 675f  h_size..padding_
+00000bb0: 7369 7a65 da0b 6269 6e61 7279 5f6d 6173  size..binary_mas
+00000bc0: 6bda 0373 6567 da09 7365 675f 7061 7463  k..seg..seg_patc
+00000bd0: 6872 1300 0000 5a0c 696e 7374 616e 6365  hr....Z.instance
+00000be0: 5f73 756d 5a0e 696e 7374 616e 6365 5f73  _sumZ.instance_s
+00000bf0: 756d 5f69 da0a 6c6f 675f 7969 5f73 756d  um_i..log_yi_sum
+00000c00: da06 6c6f 675f 7969 7216 0000 0072 1600  ..log_yir....r..
+00000c10: 0000 7217 0000 00da 1d73 656c 665f 7375  ..r......self_su
+00000c20: 7065 7276 6973 6564 5f69 6e73 7461 6e63  pervised_instanc
+00000c30: 655f 6c6f 7373 5200 0000 7336 0000 0000  e_lossR...s6....
+00000c40: 0908 0108 0108 0108 0108 020a 010c 0108  ................
+00000c50: 0108 0218 010c 0204 010c 0218 020a 0114  ................
+00000c60: 0110 020e 0310 010c 0218 020a 0110 0114  ................
+00000c70: 0110 020c 0272 5600 0000 46a9 01da 0b69  .....rV...F....i
+00000c80: 676e 6f72 655f 6d61 736b 6303 0000 0000  gnore_maskc.....
+00000c90: 0000 0001 0000 0011 0000 0005 0000 004b  ...............K
+00000ca0: 0000 0073 2a01 0000 7c00 6401 1900 7d05  ...s*...|.d...}.
+00000cb0: 7c00 6402 1900 7d06 7c00 6403 1900 7d07  |.d...}.|.d...}.
+00000cc0: 7c00 6404 1900 7d08 7c00 6405 1900 7d09  |.d...}.|.d...}.
+00000cd0: 7c06 6a00 6406 1900 7d0a 7c0a 6407 1a00  |.j.d...}.|.d...
+00000ce0: 6407 1700 7d0b 7c08 7c0b 3700 7d08 7c09  d...}.|.|.7.}.|.
+00000cf0: 7c0b 3700 7d09 7c03 7282 7401 a002 7c02  |.7.}.|.r.t...|.
+00000d00: 6408 1900 6a00 6409 6406 8502 1900 a101  d...j.d.d.......
+00000d10: 7d0c 7401 a003 7c0c 7c0b a102 7d0c 7401  }.t...|.|...}.t.
+00000d20: a004 7c06 a101 7d0d 6e54 7405 7c01 7406  ..|...}.nTt.|.t.
+00000d30: 8302 729c 7c01 640a 1900 a007 640b a101  ..r.|.d.....d...
+00000d40: 7d0c 6e0a 7c01 a007 640b a101 7d0c 7401  }.n.|...d...}.t.
+00000d50: a003 7c0c 7c0b a102 7d0c 7c0c 7c08 7c09  ..|.|...}.|.|.|.
+00000d60: 6602 1900 7d0e 640c 7c0e 1800 7c06 1400  f...}.d.|...|...
+00000d70: 7c0e 640c 7c06 1800 1400 1700 7d0d 7401  |.d.|.......}.t.
+00000d80: a004 7c0c a101 7d0f 7408 6a09 a00a 7c07  ..|...}.t.j...|.
+00000d90: 0b00 a101 0b00 7d10 7c0f 6a0b 7c08 7c09  ......}.|.j.|.|.
+00000da0: 6602 1900 a00c 7c10 a101 7d0f 7c0f 7c08  f.....|...}.|.|.
+00000db0: 7c09 6602 1900 7c10 1800 7d10 7c0d 7c06  |.f...|...}.|.|.
+00000dc0: 7c10 1400 1700 7d0d 740d 7c0d 7c05 8302  |.....}.t.|.|...
+00000dd0: 5300 290d 7a40 496e 7374 616e 6365 206c  S.).z@Instance l
+00000de0: 6f73 7320 7375 7065 7276 6973 6564 2062  oss supervised b
+00000df0: 7920 696d 6167 6520 6d61 736b 2069 6e73  y image mask ins
+00000e00: 7465 6164 206f 6620 696e 7374 616e 6365  tead of instance
+00000e10: 206d 6173 6b73 7219 0000 0072 4200 0000   masksr....rB...
+00000e20: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+00000e30: 0800 0000 7203 0000 00da 0569 6d61 6765  ....r......image
+00000e40: 4eda 0d67 745f 696d 6167 655f 6d61 736b  N..gt_image_mask
+00000e50: 7206 0000 0072 4400 0000 290e 720d 0000  r....rD...).r...
+00000e60: 0072 0e00 0000 da05 7a65 726f 7372 2600  .r......zerosr&.
+00000e70: 0000 7249 0000 0072 2300 0000 7224 0000  ..rI...r#...r$..
+00000e80: 0072 2500 0000 722b 0000 0072 4700 0000  .r%...r+...rG...
+00000e90: 724d 0000 0072 4a00 0000 724b 0000 0072  rM...rJ...rK...r
+00000ea0: 1800 0000 2911 7230 0000 0072 3100 0000  ....).r0...r1...
+00000eb0: da06 696e 7075 7473 7258 0000 0072 3200  ..inputsrX...r2.
+00000ec0: 0000 7219 0000 0072 4e00 0000 721a 0000  ..r....rN...r...
+00000ed0: 0072 3300 0000 7234 0000 0072 4f00 0000  .r3...r4...rO...
+00000ee0: 7250 0000 0072 5200 0000 7213 0000 0072  rP...rR...r....r
+00000ef0: 5300 0000 7254 0000 0072 5500 0000 7216  S...rT...rU...r.
+00000f00: 0000 0072 1600 0000 7217 0000 00da 1f77  ...r....r......w
+00000f10: 6561 6b6c 795f 7375 7065 7276 6973 6564  eakly_supervised
+00000f20: 5f69 6e73 7461 6e63 655f 6c6f 7373 8400  _instance_loss..
+00000f30: 0000 7332 0000 0000 0508 0108 0108 0108  ..s2............
+00000f40: 0108 020a 010c 0108 0108 0204 0118 010c  ................
+00000f50: 010c 020a 0110 020a 010c 010c 0118 020a  ................
+00000f60: 0210 0114 0110 020c 0272 5d00 0000 6300  .........r]...c.
+00000f70: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000f80: 0000 0040 0000 0073 1c00 0000 6500 5a01  ...@...s....e.Z.
+00000f90: 6400 5a02 6503 6503 6401 9c02 6402 6403  d.Z.e.e.d...d.d.
+00000fa0: 8404 5a04 6404 5300 2905 da16 5375 7065  ..Z.d.S.)...Supe
+00000fb0: 7276 6973 6564 496e 7374 616e 6365 4c6f  rvisedInstanceLo
+00000fc0: 7373 2902 7230 0000 0072 3100 0000 6303  ss).r0...r1...c.
+00000fd0: 0000 0000 0000 0000 0000 0004 0000 0003  ................
+00000fe0: 0000 004b 0000 0073 0a00 0000 7400 7c01  ...K...s....t.|.
+00000ff0: 7c02 8302 5300 a901 4e29 0172 3f00 0000  |...S...N).r?...
+00001000: 2904 da04 7365 6c66 7230 0000 0072 3100  )...selfr0...r1.
+00001010: 0000 7232 0000 0072 1600 0000 7216 0000  ..r2...r....r...
+00001020: 0072 1700 0000 da04 6361 6c6c ad00 0000  .r......call....
+00001030: 7302 0000 0000 017a 1b53 7570 6572 7669  s......z.Supervi
+00001040: 7365 6449 6e73 7461 6e63 654c 6f73 732e  sedInstanceLoss.
+00001050: 6361 6c6c 4e29 05da 085f 5f6e 616d 655f  callN)...__name_
+00001060: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00001070: 5f71 7561 6c6e 616d 655f 5f72 2400 0000  _qualname__r$...
+00001080: 7261 0000 0072 1600 0000 7216 0000 0072  ra...r....r....r
+00001090: 1600 0000 7217 0000 0072 5e00 0000 ac00  ....r....r^.....
+000010a0: 0000 7302 0000 0008 0172 5e00 0000 6300  ..s......r^...c.
+000010b0: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+000010c0: 0000 0000 0000 0073 3200 0000 6500 5a01  .......s2...e.Z.
+000010d0: 6400 5a02 6408 6503 6402 9c01 8700 6601  d.Z.d.e.d.....f.
+000010e0: 6403 6404 840d 5a04 6505 6405 9c01 6406  d.d...Z.e.d...d.
+000010f0: 6407 8404 5a06 8700 0400 5a07 5300 2909  d...Z.....Z.S.).
+00001100: da1a 5365 6c66 5375 7065 7276 6973 6564  ..SelfSupervised
+00001110: 496e 7374 616e 6365 4c6f 7373 5472 4000  InstanceLossTr@.
+00001120: 0000 6302 0000 0000 0000 0000 0000 0004  ..c.............
+00001130: 0000 0003 0000 000f 0000 0073 1800 0000  ...........s....
+00001140: 7400 8300 6a01 7c02 7c03 8e01 0100 7c01  t...j.|.|.....|.
+00001150: 7c00 5f02 6400 5300 725f 0000 0029 03da  |._.d.S.r_...)..
+00001160: 0573 7570 6572 da08 5f5f 696e 6974 5f5f  .super..__init__
+00001170: 7241 0000 0029 0472 6000 0000 7241 0000  rA...).r`...rA..
+00001180: 00da 0461 7267 7372 3200 0000 a901 da09  ...argsr2.......
+00001190: 5f5f 636c 6173 735f 5f72 1600 0000 7217  __class__r....r.
+000011a0: 0000 0072 6700 0000 b200 0000 7304 0000  ...rg.......s...
+000011b0: 0000 010e 017a 2353 656c 6653 7570 6572  .....z#SelfSuper
+000011c0: 7669 7365 6449 6e73 7461 6e63 654c 6f73  visedInstanceLos
+000011d0: 732e 5f5f 696e 6974 5f5f 2901 7230 0000  s.__init__).r0..
+000011e0: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
+000011f0: 0000 0400 0000 4b00 0000 730e 0000 0074  ......K...s....t
+00001200: 007c 017c 006a 0164 018d 0253 0029 024e  .|.|.j.d...S.).N
+00001210: 7240 0000 0029 0272 5600 0000 7241 0000  r@...).rV...rA..
+00001220: 0029 0372 6000 0000 7230 0000 0072 3200  .).r`...r0...r2.
+00001230: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00001240: 0072 6100 0000 b600 0000 7302 0000 0000  .ra.......s.....
+00001250: 017a 1f53 656c 6653 7570 6572 7669 7365  .z.SelfSupervise
+00001260: 6449 6e73 7461 6e63 654c 6f73 732e 6361  dInstanceLoss.ca
+00001270: 6c6c 2901 5429 0872 6200 0000 7263 0000  ll).T).rb...rc..
+00001280: 0072 6400 0000 da04 626f 6f6c 7267 0000  .rd.....boolrg..
+00001290: 0072 2400 0000 7261 0000 00da 0d5f 5f63  .r$...ra.....__c
+000012a0: 6c61 7373 6365 6c6c 5f5f 7216 0000 0072  lasscell__r....r
+000012b0: 1600 0000 7269 0000 0072 1700 0000 7265  ....ri...r....re
+000012c0: 0000 00b1 0000 0073 0400 0000 0801 1404  .......s........
+000012d0: 7265 0000 0063 0000 0000 0000 0000 0000  re...c..........
+000012e0: 0000 0000 0000 0500 0000 0000 0000 732c  ..............s,
+000012f0: 0000 0065 005a 0164 005a 0264 0765 0364  ...e.Z.d.Z.d.e.d
+00001300: 029c 0187 0066 0164 0364 0484 0d5a 0464  .....f.d.d...Z.d
+00001310: 0564 0684 005a 0587 0004 005a 0653 0029  .d...Z.....Z.S.)
+00001320: 08da 1c57 6561 6b6c 7953 7570 6572 7669  ...WeaklySupervi
+00001330: 7365 6449 6e73 7461 6e63 654c 6f73 7346  sedInstanceLossF
+00001340: 7257 0000 0063 0200 0000 0000 0000 0000  rW...c..........
+00001350: 0000 0400 0000 0300 0000 0f00 0000 7318  ..............s.
+00001360: 0000 0074 0083 006a 017c 027c 038e 0101  ...t...j.|.|....
+00001370: 007c 017c 005f 0264 0053 0072 5f00 0000  .|.|._.d.S.r_...
+00001380: 2903 7266 0000 0072 6700 0000 7258 0000  ).rf...rg...rX..
+00001390: 0029 0472 6000 0000 7258 0000 0072 6800  .).r`...rX...rh.
+000013a0: 0000 7232 0000 0072 6900 0000 7216 0000  ..r2...ri...r...
+000013b0: 0072 1700 0000 7267 0000 00bb 0000 0073  .r....rg.......s
+000013c0: 0400 0000 0001 0e01 7a25 5765 616b 6c79  ........z%Weakly
+000013d0: 5375 7065 7276 6973 6564 496e 7374 616e  SupervisedInstan
+000013e0: 6365 4c6f 7373 2e5f 5f69 6e69 745f 5f63  ceLoss.__init__c
+000013f0: 0100 0000 0000 0000 0300 0000 0400 0000  ................
+00001400: 0600 0000 4300 0000 7312 0000 0074 007c  ....C...s....t.|
+00001410: 017c 027c 037c 006a 0164 018d 0453 0029  .|.|.|.j.d...S.)
+00001420: 024e 7257 0000 0029 0272 5d00 0000 7258  .NrW...).r]...rX
+00001430: 0000 0029 0472 6000 0000 7230 0000 0072  ...).r`...r0...r
+00001440: 3100 0000 725c 0000 0072 1600 0000 7216  1...r\...r....r.
+00001450: 0000 0072 1700 0000 7261 0000 00bf 0000  ...r....ra......
+00001460: 0073 0c00 0000 0001 0201 0200 0200 0200  .s..............
+00001470: 04ff 7a21 5765 616b 6c79 5375 7065 7276  ..z!WeaklySuperv
+00001480: 6973 6564 496e 7374 616e 6365 4c6f 7373  isedInstanceLoss
+00001490: 2e63 616c 6c29 0146 2907 7262 0000 0072  .call).F).rb...r
+000014a0: 6300 0000 7264 0000 0072 6b00 0000 7267  c...rd...rk...rg
+000014b0: 0000 0072 6100 0000 726c 0000 0072 1600  ...ra...rl...r..
+000014c0: 0000 7216 0000 0072 6900 0000 7217 0000  ..r....ri...r...
+000014d0: 0072 6d00 0000 ba00 0000 7304 0000 0008  .rm.......s.....
+000014e0: 0114 0472 6d00 0000 2916 da09 6675 6e63  ...rm...)...func
+000014f0: 746f 6f6c 7372 0200 0000 722b 0000 00da  toolsr....r+....
+00001500: 096a 6178 2e6e 756d 7079 da05 6e75 6d70  .jax.numpy..nump
+00001510: 7972 0e00 0000 722e 0000 00da 036f 7073  yr....r......ops
+00001520: 7204 0000 00da 0a74 7261 696e 2e6c 6f73  r......train.los
+00001530: 7372 0500 0000 da05 6669 6e66 6fda 0365  sr......finfo..e
+00001540: 7073 7210 0000 0072 1800 0000 723f 0000  psr....r....r?..
+00001550: 0072 6b00 0000 7256 0000 0072 5d00 0000  .rk...rV...r]...
+00001560: 725e 0000 0072 6500 0000 726d 0000 0072  r^...re...rm...r
+00001570: 1600 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
+00001580: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00001590: 0073 2000 0000 0c02 0801 0c01 0802 0c01  .s .............
+000015a0: 0c02 0c03 080b 083a 1433 02ff 0401 02ff  .......:.3......
+000015b0: 0c28 1005 1009                           .(....
```

### Comparing `lacss-0.4.1/lacss/losses/auxiliary.py` & `lacss-0.4.2/lacss/losses/auxiliary.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     ]
     combined_edges = jnp.tanh(combined_edges)
 
     return combined_edges
 
 
 def self_supervised_edge_loss(preds, inputs, **kwargs):
-    """LACSS cell border consistency loss"""
+    """Cell border prediction consistency loss"""
 
     instance_output = preds["instance_output"]
     instance_yc = preds["instance_yc"]
     instance_xc = preds["instance_xc"]
     height, width, _ = inputs["image"].shape
     instance_edge = _compute_edge(
         instance_output, instance_yc, instance_xc, height, width
@@ -50,25 +50,32 @@
     preds,
     inputs,
     *,
     offset_sigma=jnp.array([10.0]),
     offset_scale=jnp.array([2.0]),
     **kwargs,
 ):
-    """LACSS image segmentation consistenct loss"""
+    """Image segmentation consistenct loss for the collaboraor model"""
 
     height, width, _ = inputs["image"].shape
     _, ps, _ = preds["instance_yc"].shape
 
+    offset_sigma = jnp.asarray(offset_sigma).reshape(-1)
+    offset_scale = jnp.asarray(offset_scale).reshape(-1)
+
     def _max_merge(pred):
         label = jnp.zeros([height + ps, width + ps]) - 1.0e6
         yc, xc = pred["instance_yc"], pred["instance_xc"]
         logit = pred["instance_logit"]
 
-        if "category" in inputs and inputs["category"] is not None:
+        if (
+            offset_sigma.size > 1
+            and "cls_id" in inputs
+            and inputs["cls_id"] is not None
+        ):
             c = inputs["category"].astype(int).squeeze()
         else:
             c = 0
 
         sigma = offset_sigma[c]
         scale = offset_scale[c]
         offset = (jnp.mgrid[:ps, :ps] - (ps - 1) / 2) ** 2 / (2 * sigma * sigma)
@@ -96,15 +103,15 @@
 
     loss = loss.mean()
 
     return loss
 
 
 def aux_size_loss(preds, inputs, *, weight=0.01, **kwargs):
-    """auxillary loss to prevent model collapse"""
+    """Auxillary loss to prevent model collapse"""
 
     height, width, _ = inputs["image"].shape
 
     valid_locs = (
         (preds["instance_yc"] >= 0)
         & (preds["instance_yc"] < height)
         & (preds["instance_xc"] >= 0)
@@ -128,15 +135,15 @@
 
     if "gt_labels" in labels:
 
         mask = (labels["gt_labels"] > 0).astype("float32")
 
     else:
 
-        mask = labels["gt_mask"].astype("float32")
+        mask = labels["gt_image_mask"].astype("float32")
 
     return optax.sigmoid_binary_cross_entropy(preds["fg_pred"], mask).mean()
 
 
 class AuxEdgeLoss(Loss):
     def call(
         self,
```

### Comparing `lacss-0.4.1/lacss/losses/detection.py` & `lacss-0.4.2/lacss/losses/detection.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/losses/instance.py` & `lacss-0.4.2/lacss/losses/instance.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,64 +18,79 @@
     loss = loss.mean(axis=1, keepdims=True).sum(where=mask)
     loss /= n_instances
 
     return loss
 
 
 def supervised_instance_loss(preds, labels, **kwargs):
-    """LACSS instance loss, supervised with segmentation label"""
+    """LACSS instance loss, supervised with segmentation label
+
+    Args:
+        preds: Model predictions
+        labels: Label dictionary. Two types of segmentation labels are accepted.
+            If ```labels["gt_labels"]``` is provided, its value is treated as pixel
+            labels of the image. Otherwisde, one much supply both ```labels["gt_bboxes"]```
+            and ```labels["gt_masks"]```. The gt_masks is a 3D array representing all
+            segmentation resized to a fixed dimension.
+    """
 
     instance_mask = preds["instance_mask"]
     instance_logit = preds["instance_logit"]
     yc = preds["instance_yc"]
     xc = preds["instance_xc"]
 
     if not isinstance(labels, dict):
         labels = dict(gt_labels=labels)
 
-    if "gt_labels" in labels: # labeled with image label
+    if "gt_labels" in labels:  # labeled with image label
         gt_labels = labels["gt_labels"].astype("int32")
 
         n_patches, ps, _ = yc.shape
 
         gt_labels = jnp.pad(gt_labels, ps // 2)
         gt_patches = gt_labels[yc + ps // 2, xc + ps // 2] == (
             jnp.arange(n_patches)[:, None, None] + 1
         )
         gt_patches = gt_patches.astype("float32")
 
-    else: # labeled with bboxes and rescaled segmentation masks, ie, coco
+    else:  # labeled with bboxes and rescaled segmentation masks, ie, coco
         y0, x0, y1, x1 = jnp.swapaxes(labels["gt_bboxes"], 0, 1)
         gt_segs = labels["gt_masks"]
-        if len(gt_segs.shape) == 4: # either NxHxWx1 or NxHxW
-            gt_segs = gt_segs.squeeze(-1) 
+        if len(gt_segs.shape) == 4:  # either NxHxWx1 or NxHxW
+            gt_segs = gt_segs.squeeze(-1)
         seg_size = gt_segs.shape[1]
 
         # pixel size of the gt mask labels
-        hs = (y1 - y0) / seg_size 
+        hs = (y1 - y0) / seg_size
         ws = (x1 - x0) / seg_size
 
         # compute rescaled coorinats in edge indexing
-        yc = (yc - y0[:, None, None] + .5) / hs[:, None, None]
-        xc = (xc - x0[:, None, None] + .5) / ws[:, None, None]
+        yc = (yc - y0[:, None, None] + 0.5) / hs[:, None, None]
+        xc = (xc - x0[:, None, None] + 0.5) / ws[:, None, None]
 
         # resample the label to match model coordinates
         gt_patches = jax.vmap(sub_pixel_samples)(
             gt_segs,
-            jnp.stack([yc, xc], axis=-1) - .5, # default is center indexing
+            jnp.stack([yc, xc], axis=-1) - 0.5,  # default is center indexing
         )
-        gt_patches = (gt_patches>=.5).astype("float32")
+        gt_patches = (gt_patches >= 0.5).astype("float32")
 
     loss = optax.sigmoid_binary_cross_entropy(instance_logit, gt_patches)
 
     return _mean_over_boolean_mask(loss, instance_mask)
 
 
-def self_supervised_instance_loss(preds, *, soft_label: bool = True):
-    """LACSS instance loss, unsupervised"""
+def self_supervised_instance_loss(preds, *, soft_label: bool = True, **kwargs):
+    """Unsupervised instance loss
+
+    Args:
+        preds: Model prediction dict.
+        soft_label: If False, it convertes image mask prediction to hard label
+            (ie. 0 or 1), before computing loss.
+    """
 
     instance_mask = preds["instance_mask"]
     instances = preds["instance_output"]
     instance_logit = preds["instance_logit"]
     yc = preds["instance_yc"]
     xc = preds["instance_xc"]
 
@@ -113,15 +128,15 @@
 
     return _mean_over_boolean_mask(loss, instance_mask)
 
 
 def weakly_supervised_instance_loss(
     preds, labels, inputs, *, ignore_mask: bool = False, **kwargs
 ):
-    """Lacss instance loss, supervised with image mask"""
+    """Instance loss supervised by image mask instead of instance masks"""
 
     instance_mask = preds["instance_mask"]
     instances = preds["instance_output"]
     instance_logit = preds["instance_logit"]
     yc = preds["instance_yc"]
     xc = preds["instance_xc"]
 
@@ -132,15 +147,15 @@
 
     if ignore_mask:
         seg = jnp.zeros(inputs["image"].shape[:-1])
         seg = jnp.pad(seg, padding_size)
         loss = jnp.zeros_like(instances)
     else:
         if isinstance(labels, dict):
-            seg = labels["gt_mask"].astype("float32")
+            seg = labels["gt_image_mask"].astype("float32")
         else:
             seg = labels.astype("float32")
         seg = jnp.pad(seg, padding_size)
         seg_patch = seg[yc, xc]
         loss = (1.0 - seg_patch) * instances + seg_patch * (1.0 - instances)
 
     log_yi_sum = jnp.zeros_like(seg)
```

### Comparing `lacss-0.4.1/lacss/metrics/__pycache__/ranked.cpython-38.pyc` & `lacss-0.4.2/lacss/metrics/__pycache__/ranked.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 19:35:53 2023 UTC, .py size: 5103 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 99e8 9964 ef13 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 5a80 9c64 ef13 0000  U.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a04 0100 6401 6402 6c03 5a05 6403  m.Z...d.d.l.Z.d.
 00000050: 6404 6c06 5400 6403 6405 6c07 6d08 5a08  d.l.T.d.d.l.m.Z.
 00000060: 0100 6403 6406 6c09 6d0a 5a0a 0100 6407  ..d.d.l.m.Z...d.
 00000070: 6408 8400 5a0b 6409 640a 8400 5a0c 4700  d...Z.d.d...Z.G.
```

### Comparing `lacss-0.4.1/lacss/metrics/ranked.py` & `lacss-0.4.2/lacss/metrics/ranked.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/modules/__pycache__/auxiliary.cpython-38.pyc` & `lacss-0.4.2/lacss/modules/__pycache__/auxiliary.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 19:35:53 2023 UTC, .py size: 2075 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,141 +1,119 @@
-00000000: 550d 0d0a 0000 0000 99e8 9964 1b08 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 e67d ad64 4f06 0000  U........}.dO...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
-00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 5a04  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6401 6c05 5a05 6400 6401 6c06  ..d.d.l.Z.d.d.l.
-00000050: 6d07 5a08 0100 6402 6403 6c09 5400 6402  m.Z...d.d.l.T.d.
-00000060: 6404 6c0a 6d0b 5a0b 0100 4700 6405 6406  d.l.m.Z...G.d.d.
-00000070: 8400 6406 6504 6a0c 8303 5a0d 4700 6407  ..d.e.j...Z.G.d.
-00000080: 6408 8400 6408 6504 6a0c 8303 5a0e 6401  d...d.e.j...Z.d.
-00000090: 5300 2909 e900 0000 004e e901 0000 0029  S.)......N.....)
-000000a0: 01da 012a 2901 da04 554e 6574 6300 0000  ...*)...UNetc...
-000000b0: 0000 0000 0000 0000 0000 0000 0006 0000  ................
-000000c0: 0040 0000 0073 5600 0000 6500 5a01 6400  .@...sV...e.Z.d.
-000000d0: 5a02 5500 6401 5a03 6504 6a05 6506 1900  Z.U.d.Z.e.j.e...
-000000e0: 6507 6402 3c00 6403 5a08 6506 6507 6404  e.d.<.d.Z.e.e.d.
-000000f0: 3c00 6509 6a0a 6405 6406 9c01 650b 6a0c  <.e.j.d.d...e.j.
-00000100: 6504 6a0d 650b 6a0c 1900 650b 6a0c 6407  e.j.e.j...e.j.d.
-00000110: 9c03 6408 6409 8406 8301 5a0e 6405 5300  ..d.d.....Z.d.S.
-00000120: 290a da0f 4175 7849 6e73 7461 6e63 6545  )...AuxInstanceE
-00000130: 6467 6529 03e9 1800 0000 e940 0000 0072  dge).......@...r
-00000140: 0700 0000 da09 636f 6e76 5f73 7065 6372  ......conv_specr
-00000150: 0200 0000 da08 6e5f 6772 6f75 7073 4ea9  ......n_groupsN.
-00000160: 01da 0863 6174 6567 6f72 79a9 03da 0178  ...category....x
-00000170: 720b 0000 00da 0672 6574 7572 6e63 0200  r......returnc..
-00000180: 0000 0000 0000 0100 0000 0500 0000 0600  ................
-00000190: 0000 4300 0000 738a 0000 007c 006a 0044  ..C...s....|.j.D
-000001a0: 005d 407d 0374 016a 027c 0364 0164 0264  .]@}.t.j.|.d.d.d
-000001b0: 038d 037c 0183 017d 0174 016a 0364 0064  ...|...}.t.j.d.d
-000001c0: 0464 0264 058d 037c 0164 0619 0083 0164  .d.d...|.d.....d
-000001d0: 0719 007d 0174 046a 01a0 057c 01a1 017d  ...}.t.j...|...}
-000001e0: 0171 0674 01a0 027c 006a 0664 01a1 027c  .q.t...|.j.d...|
-000001f0: 0183 017d 017c 0264 006b 0972 707c 02a0  ...}.|.d.k.rp|..
-00000200: 0774 08a1 01a0 09a1 006e 0264 077d 047c  .t.......n.d.}.|
-00000210: 0164 087c 0466 0219 007d 0174 0a7c 0164  .d.|.f...}.t.|.d
-00000220: 098d 0153 0029 0a4e a902 e903 0000 0072  ...S.).N.......r
-00000230: 1000 0000 4629 01da 0875 7365 5f62 6961  ....F)...use_bia
-00000240: 7372 0200 0000 2903 da0a 6e75 6d5f 6772  sr....)...num_gr
-00000250: 6f75 7073 da0a 6772 6f75 705f 7369 7a65  oups..group_size
-00000260: da09 7573 655f 7363 616c 6529 024e 2e72  ..use_scale).N.r
-00000270: 0100 0000 2ea9 01da 0965 6467 655f 7072  .........edge_pr
-00000280: 6564 290b 7208 0000 00da 026e 6eda 0443  ed).r......nn..C
-00000290: 6f6e 76da 0947 726f 7570 4e6f 726d da03  onv..GroupNorm..
-000002a0: 6a61 78da 0472 656c 7572 0900 0000 da06  jax..relur......
-000002b0: 6173 7479 7065 da03 696e 74da 0773 7175  astype..int..squ
-000002c0: 6565 7a65 da04 6469 6374 2905 da04 7365  eeze..dict)...se
-000002d0: 6c66 720d 0000 0072 0b00 0000 da01 6eda  lfr....r......n.
-000002e0: 0163 a900 7223 0000 00fa 3a2f 686f 6d65  .c..r#....:/home
-000002f0: 2f46 4341 4d2f 6a79 752f 7072 6f6a 5f6c  /FCAM/jyu/proj_l
-00000300: 6163 7373 2f6c 6163 7373 2f6c 6163 7373  acss/lacss/lacss
-00000310: 2f6d 6f64 756c 6573 2f61 7578 696c 6961  /modules/auxilia
-00000320: 7279 2e70 79da 085f 5f63 616c 6c5f 5f10  ry.py..__call__.
-00000330: 0000 0073 1c00 0000 0004 0a01 1401 0e01  ...s............
-00000340: 06ff 0202 02fe 0403 0e02 1201 1a01 0c04  ................
-00000350: 0201 02ff 7a18 4175 7849 6e73 7461 6e63  ....z.AuxInstanc
-00000360: 6545 6467 652e 5f5f 6361 6c6c 5f5f 290f  eEdge.__call__).
-00000370: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000380: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000390: 6d65 5f5f 7208 0000 00da 0274 70da 0853  me__r......tp..S
-000003a0: 6571 7565 6e63 6572 1d00 0000 da0f 5f5f  equencer......__
-000003b0: 616e 6e6f 7461 7469 6f6e 735f 5f72 0900  annotations__r..
-000003c0: 0000 7217 0000 00da 0763 6f6d 7061 6374  ..r......compact
-000003d0: da03 6a6e 70da 076e 6461 7272 6179 da08  ..jnp..ndarray..
-000003e0: 4f70 7469 6f6e 616c 7225 0000 0072 2300  Optionalr%...r#.
-000003f0: 0000 7223 0000 0072 2300 0000 7224 0000  ..r#...r#...r$..
-00000400: 0072 0500 0000 0b00 0000 7312 0000 000a  .r........s.....
-00000410: 0112 010c 0304 0202 ff04 0104 000a 0104  ................
-00000420: fe72 0500 0000 6300 0000 0000 0000 0000  .r....c.........
-00000430: 0000 0000 0000 0006 0000 0040 0000 0073  ...........@...s
-00000440: 7400 0000 6500 5a01 6400 5a02 5500 6401  t...e.Z.d.Z.U.d.
-00000450: 5a03 6504 6a05 6506 1900 6507 6402 3c00  Z.e.j.e...e.d.<.
-00000460: 6403 5a08 6504 6a05 6506 1900 6507 6404  d.Z.e.j.e...e.d.
-00000470: 3c00 6403 5a09 6506 6507 6405 3c00 6406  <.d.Z.e.e.d.<.d.
-00000480: 5a0a 650b 6507 6407 3c00 650c 6a0d 6408  Z.e.e.d.<.e.j.d.
-00000490: 6409 9c01 650e 6a0f 6504 6a10 650e 6a0f  d...e.j.e.j.e.j.
-000004a0: 1900 650e 6a0f 640a 9c03 640b 640c 8406  ..e.j.d...d.d...
-000004b0: 8301 5a11 6408 5300 290d da0d 4175 7846  ..Z.d.S.)...AuxF
-000004c0: 6f72 6567 726f 756e 6429 0272 0600 0000  oreground).r....
-000004d0: 7207 0000 0072 0800 0000 7202 0000 00da  r....r....r.....
-000004e0: 0a70 6174 6368 5f73 697a 6572 0900 0000  .patch_sizer....
-000004f0: 46da 0d73 6861 7265 5f77 6569 6768 7473  F..share_weights
-00000500: 4e72 0a00 0000 720c 0000 0063 0200 0000  Nr....r....c....
-00000510: 0000 0000 0100 0000 0b00 0000 0600 0000  ................
-00000520: 4300 0000 7318 0100 007c 0264 006b 0973  C...s....|.d.k.s
-00000530: 167c 006a 0064 016b 0273 1674 0182 0174  .|.j.d.k.s.t...t
-00000540: 027c 006a 037c 006a 0483 027d 037c 037c  .|.j.|.j...}.|.|
-00000550: 0183 015c 027d 047d 057c 0574 057c 036a  ...\.}.}.|.t.|.j
-00000560: 0683 0119 007d 067c 0264 006b 0972 547c  .....}.|.d.k.rT|
-00000570: 02a0 0774 08a1 01a0 09a1 006e 0264 027d  ...t.......n.d.}
-00000580: 0774 0aa0 0b7c 006a 0064 03a1 027c 0683  .t...|.j.d...|..
-00000590: 017d 087c 0864 047c 0766 0219 007d 087c  .}.|.d.|.f...}.|
-000005a0: 086a 0c7c 016a 0c64 0064 0585 0219 006b  .j.|.j.d.d.....k
-000005b0: 0372 a474 0d6a 0ea0 0f7c 087c 016a 0c64  .r.t.j...|.|.j.d
-000005c0: 0064 0585 0219 0064 06a1 037d 0874 107c  .d.....d...}.t.|
-000005d0: 0864 078d 017d 097c 006a 1190 0172 1474  .d...}.|.j...r.t
-000005e0: 0aa0 0b7c 006a 0064 03a1 027c 0683 017d  ...|.j.d...|...}
-000005f0: 0a7c 0a64 047c 0766 0219 007d 0a7c 0a6a  .|.d.|.f...}.|.j
-00000600: 0c7c 016a 0c64 0064 0585 0219 006b 0390  .|.j.d.d.....k..
-00000610: 0172 0474 0d6a 0ea0 0f7c 0a7c 016a 0c64  .r.t.j...|.|.j.d
-00000620: 0064 0585 0219 0064 06a1 037d 0a7c 09a0  .d.....d...}.|..
-00000630: 1274 107c 0a64 088d 01a1 0101 007c 0953  .t.|.d.......|.S
-00000640: 0029 094e 7202 0000 0072 0100 0000 720f  .).Nr....r....r.
-00000650: 0000 002e e9ff ffff ffda 066c 696e 6561  ...........linea
-00000660: 7229 01da 0766 675f 7072 6564 7215 0000  r)...fg_predr...
-00000670: 0029 1372 0900 0000 da0e 4173 7365 7274  .).r......Assert
-00000680: 696f 6e45 7272 6f72 7204 0000 0072 0800  ionErrorr....r..
-00000690: 0000 7231 0000 00da 0373 7472 5a0b 7374  ..r1.....strZ.st
-000006a0: 6172 745f 6c65 7665 6c72 1c00 0000 721d  art_levelr....r.
-000006b0: 0000 0072 1e00 0000 7217 0000 0072 1800  ...r....r....r..
-000006c0: 0000 da05 7368 6170 6572 1a00 0000 da05  ....shaper......
-000006d0: 696d 6167 65da 0672 6573 697a 6572 1f00  image..resizer..
-000006e0: 0000 7232 0000 00da 0675 7064 6174 6529  ..r2.....update)
-000006f0: 0b72 2000 0000 720d 0000 0072 0b00 0000  .r ...r....r....
-00000700: da03 6e65 74da 015f 5a0b 6465 636f 6465  ..net.._Z.decode
-00000710: 725f 6f75 74da 0179 7222 0000 00da 0266  r_out..yr".....f
-00000720: 67da 066f 7574 7075 74da 0465 6467 6572  g..output..edger
-00000730: 2300 0000 7223 0000 0072 2400 0000 7225  #...r#...r$...r%
-00000740: 0000 002d 0000 0073 2a00 0000 0007 1602  ...-...s*.......
-00000750: 0e01 0c02 0e02 1a02 1201 0c02 1401 1a02  ................
-00000760: 0a02 0801 1201 0c02 1601 1a02 0401 0201  ................
-00000770: 02ff 04ff 0406 7a16 4175 7846 6f72 6567  ......z.AuxForeg
-00000780: 726f 756e 642e 5f5f 6361 6c6c 5f5f 2912  round.__call__).
-00000790: 7226 0000 0072 2700 0000 7228 0000 0072  r&...r'...r(...r
-000007a0: 0800 0000 7229 0000 0072 2a00 0000 721d  ....r)...r*...r.
-000007b0: 0000 0072 2b00 0000 7231 0000 0072 0900  ...r+...r1...r..
-000007c0: 0000 7232 0000 00da 0462 6f6f 6c72 1700  ..r2.....boolr..
-000007d0: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
-000007e0: 0072 2f00 0000 7225 0000 0072 2300 0000  .r/...r%...r#...
-000007f0: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
-00000800: 3000 0000 2600 0000 7316 0000 000a 0112  0...&...s.......
-00000810: 0112 010c 010c 0304 0502 fc04 0204 020a  ................
-00000820: 0104 fb72 3000 0000 290f da06 7479 7069  ...r0...)...typi
-00000830: 6e67 7229 0000 00da 0a66 6c61 782e 6c69  ngr).....flax.li
-00000840: 6e65 6eda 056c 696e 656e 7217 0000 0072  nen..linenr....r
-00000850: 1a00 0000 da09 6a61 782e 6e75 6d70 79da  ......jax.numpy.
-00000860: 056e 756d 7079 722d 0000 00da 0663 6f6d  .numpyr-.....com
-00000870: 6d6f 6eda 0475 6e65 7472 0400 0000 da06  mon..unetr......
-00000880: 4d6f 6475 6c65 7205 0000 0072 3000 0000  Moduler....r0...
-00000890: 7223 0000 0072 2300 0000 7223 0000 0072  r#...r#...r#...r
-000008a0: 2400 0000 da08 3c6d 6f64 756c 653e 0100  $.....<module>..
-000008b0: 0000 730e 0000 0008 020c 0108 010c 0208  ..s.............
-000008c0: 010c 0312 1b                             .....
+00000020: 0004 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
+00000030: 6401 6c00 6d01 5a02 0100 6400 6401 6c03  d.l.m.Z...d.d.l.
+00000040: 5a03 6400 6401 6c04 6d05 5a06 0100 6400  Z.d.d.l.m.Z...d.
+00000050: 6402 6c07 5400 6403 6402 6c08 5400 6403  d.l.T.d.d.l.T.d.
+00000060: 6404 6c09 6d0a 5a0a 0100 4700 6405 6406  d.l.m.Z...G.d.d.
+00000070: 8400 6406 6502 6a0b 8303 5a0c 6401 5300  ..d.e.j...Z.d.S.
+00000080: 2907 e900 0000 004e 2901 da01 2ae9 0100  )......N)...*...
+00000090: 0000 2901 da04 554e 6574 6300 0000 0000  ..)...UNetc.....
+000000a0: 0000 0000 0000 0000 0000 0006 0000 0040  ...............@
+000000b0: 0000 0073 6800 0000 6500 5a01 6400 5a02  ...sh...e.Z.d.Z.
+000000c0: 5500 6401 5a03 6402 5a04 6505 6506 1900  U.d.Z.d.Z.e.e...
+000000d0: 6507 6403 3c00 6404 5a08 6505 6506 1900  e.d.<.d.Z.e.e...
+000000e0: 6507 6405 3c00 6406 5a09 6506 6507 6407  e.d.<.d.Z.e.e.d.
+000000f0: 3c00 6406 5a0a 6506 6507 6408 3c00 650b  <.d.Z.e.e.d.<.e.
+00000100: 6a0c 640d 650d 650e 650d 1900 650f 640a  j.d.e.e.e...e.d.
+00000110: 9c03 640b 640c 8405 8301 5a10 6409 5300  ..d.d.....Z.d.S.
+00000120: 290e da11 4c61 6373 7343 6f6c 6c61 626f  )...LacssCollabo
+00000130: 7261 746f 7261 4701 0000 436f 6c6c 6162  ratoraG...Collab
+00000140: 6f72 6174 6f72 206d 6f64 756c 6520 666f  orator module fo
+00000150: 7220 7365 6d69 2d73 7570 6572 7669 7365  r semi-supervise
+00000160: 6420 4c61 6373 7320 7472 6169 6e69 6e67  d Lacss training
+00000170: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
+00000180: 3a0a 2020 2020 2020 2020 636f 6e76 5f73  :.        conv_s
+00000190: 7065 633a 2063 6f6e 762d 6e65 7420 7370  pec: conv-net sp
+000001a0: 6563 6966 6963 6169 746f 6e20 666f 7220  ecificaiton for 
+000001b0: 6365 6c6c 2062 6f72 6465 7220 7072 6564  cell border pred
+000001c0: 6963 6974 696f 6e0a 2020 2020 2020 2020  icition.        
+000001d0: 756e 6574 5f73 7065 633a 2073 7065 6369  unet_spec: speci
+000001e0: 6669 6361 7469 6f6e 2066 6f72 2075 6e65  fication for une
+000001f0: 742c 2075 7365 6420 746f 2070 7265 6469  t, used to predi
+00000200: 6374 2063 656c 6c20 666f 7265 6772 6f75  ct cell foregrou
+00000210: 6e64 0a20 2020 2020 2020 2070 6174 6368  nd.        patch
+00000220: 5f73 697a 653a 2070 6174 6368 2073 697a  _size: patch siz
+00000230: 6520 666f 7220 7468 6520 756e 6574 0a20  e for the unet. 
+00000240: 2020 2020 2020 206e 5f63 6c73 3a20 6e75         n_cls: nu
+00000250: 6d62 6572 206f 6620 636c 6173 7365 7320  mber of classes 
+00000260: 2863 656c 6c20 7479 7065 7329 206f 6620  (cell types) of 
+00000270: 696e 7075 7420 696d 6167 6573 0a20 2020  input images.   
+00000280: 2029 02e9 2000 0000 7206 0000 00da 0963   ).. ...r......c
+00000290: 6f6e 765f 7370 6563 2903 e910 0000 0072  onv_spec)......r
+000002a0: 0600 0000 e940 0000 00da 0975 6e65 745f  .....@.....unet_
+000002b0: 7370 6563 7203 0000 00da 0a70 6174 6368  specr......patch
+000002c0: 5f73 697a 65da 056e 5f63 6c73 4e29 03da  _size..n_clsN)..
+000002d0: 0569 6d61 6765 da06 636c 735f 6964 da06  .image..cls_id..
+000002e0: 7265 7475 726e 6303 0000 0000 0000 0000  returnc.........
+000002f0: 0000 000b 0000 0006 0000 0043 0000 0073  ...........C...s
+00000300: 1a01 0000 7c02 6400 6b09 7316 7c00 6a00  ....|.d.k.s.|.j.
+00000310: 6401 6b02 7316 7401 8201 7c02 6400 6b09  d.k.s.t...|.d.k.
+00000320: 722c 7c02 a002 7403 a101 a004 a100 6e02  r,|...t.......n.
+00000330: 6402 7d03 7405 7c00 6a06 7c00 6a07 8302  d.}.t.|.j.|.j...
+00000340: 7d04 7c04 7c01 8301 5c02 7d05 7d06 7c06  }.|.|...\.}.}.|.
+00000350: 7408 7c04 6a09 8301 1900 7d07 740a a00b  t.|.j.....}.t...
+00000360: 7c00 6a00 6403 a102 7c07 8301 7d08 7c08  |.j.d...|...}.|.
+00000370: 6404 7c03 6602 1900 7d08 7c08 6a0c 7c01  d.|.f...}.|.j.|.
+00000380: 6a0c 6400 6405 8502 1900 6b03 72a4 740d  j.d.d.....k.r.t.
+00000390: 6a0e a00f 7c08 7c01 6a0c 6400 6405 8502  j...|.|.j.d.d...
+000003a0: 1900 6406 a103 7d08 7c01 7d07 7c00 6a10  ..d...}.|.}.|.j.
+000003b0: 4400 5d40 7d09 740a 6a0b 7c09 6403 6407  D.]@}.t.j.|.d.d.
+000003c0: 6408 8d03 7c07 8301 7d07 740a 6a11 6400  d...|...}.t.j.d.
+000003d0: 6401 6407 6409 8d03 7c07 640a 1900 8301  d.d.d...|.d.....
+000003e0: 6402 1900 7d07 740d 6a0a a012 7c07 a101  d...}.t.j...|...
+000003f0: 7d07 71ae 740a a00b 7c00 6a00 6403 a102  }.q.t...|.j.d...
+00000400: 7c07 8301 7d07 7c07 6404 7c03 6602 1900  |...}.|.d.|.f...
+00000410: 7d0a 7413 7c08 7c0a 640b 8d02 5300 290c  }.t.|.|.d...S.).
+00000420: 4e72 0300 0000 7201 0000 0029 02e9 0300  Nr....r....)....
+00000430: 0000 7210 0000 002e e9ff ffff ffda 066c  ..r............l
+00000440: 696e 6561 7246 2901 da08 7573 655f 6269  inearF)...use_bi
+00000450: 6173 2903 da0a 6e75 6d5f 6772 6f75 7073  as)...num_groups
+00000460: da0a 6772 6f75 705f 7369 7a65 da09 7573  ..group_size..us
+00000470: 655f 7363 616c 6529 024e 2e29 02da 0766  e_scale).N.)...f
+00000480: 675f 7072 6564 da09 6564 6765 5f70 7265  g_pred..edge_pre
+00000490: 6429 1472 0c00 0000 da0e 4173 7365 7274  d).r......Assert
+000004a0: 696f 6e45 7272 6f72 da06 6173 7479 7065  ionError..astype
+000004b0: da03 696e 74da 0773 7175 6565 7a65 7204  ..int..squeezer.
+000004c0: 0000 0072 0700 0000 720b 0000 00da 0373  ...r....r......s
+000004d0: 7472 5a0b 7374 6172 745f 6c65 7665 6cda  trZ.start_level.
+000004e0: 026e 6eda 0443 6f6e 76da 0573 6861 7065  .nn..Conv..shape
+000004f0: da03 6a61 7872 0d00 0000 da06 7265 7369  ..jaxr......resi
+00000500: 7a65 720a 0000 00da 0947 726f 7570 4e6f  zer......GroupNo
+00000510: 726d da04 7265 6c75 da04 6469 6374 290b  rm..relu..dict).
+00000520: da04 7365 6c66 720d 0000 0072 0e00 0000  ..selfr....r....
+00000530: da01 63da 036e 6574 da01 5f5a 0875 6e65  ..c..net.._Z.une
+00000540: 745f 6f75 74da 0179 da02 6667 da0a 6e5f  t_out..y..fg..n_
+00000550: 6665 6174 7572 6573 da02 6362 a900 722e  features..cb..r.
+00000560: 0000 00fa 3a2f 686f 6d65 2f46 4341 4d2f  ....:/home/FCAM/
+00000570: 6a79 752f 7072 6f6a 5f6c 6163 7373 2f6c  jyu/proj_lacss/l
+00000580: 6163 7373 2f6c 6163 7373 2f6d 6f64 756c  acss/lacss/modul
+00000590: 6573 2f61 7578 696c 6961 7279 2e70 79da  es/auxiliary.py.
+000005a0: 085f 5f63 616c 6c5f 5f1a 0000 0073 3000  .__call__....s0.
+000005b0: 0000 0004 1601 1a02 0e01 0c02 0e02 1201  ................
+000005c0: 0c02 1401 1a02 0401 0a01 1401 0e01 06ff  ................
+000005d0: 0202 02fe 0403 0e02 1201 0c02 0201 0201  ................
+000005e0: 02fe 7a1a 4c61 6373 7343 6f6c 6c61 626f  ..z.LacssCollabo
+000005f0: 7261 746f 722e 5f5f 6361 6c6c 5f5f 2901  rator.__call__).
+00000600: 4e29 11da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000610: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000620: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00000630: 7207 0000 00da 0853 6571 7565 6e63 6572  r......Sequencer
+00000640: 1b00 0000 da0f 5f5f 616e 6e6f 7461 7469  ......__annotati
+00000650: 6f6e 735f 5f72 0a00 0000 720b 0000 0072  ons__r....r....r
+00000660: 0c00 0000 721e 0000 00da 0763 6f6d 7061  ....r......compa
+00000670: 6374 da09 4172 7261 794c 696b 65da 084f  ct..ArrayLike..O
+00000680: 7074 696f 6e61 6cda 0844 6174 6144 6963  ptional..DataDic
+00000690: 7472 3000 0000 722e 0000 0072 2e00 0000  tr0...r....r....
+000006a0: 722e 0000 0072 2f00 0000 7205 0000 000b  r....r/...r.....
+000006b0: 0000 0073 1800 0000 0a01 0409 1001 1001  ...s............
+000006c0: 0c01 0c02 0402 00ff 0201 0200 0601 02fe  ................
+000006d0: 7205 0000 0029 0dda 0a66 6c61 782e 6c69  r....)...flax.li
+000006e0: 6e65 6eda 056c 696e 656e 721e 0000 0072  nen..linenr....r
+000006f0: 2100 0000 da09 6a61 782e 6e75 6d70 79da  !.....jax.numpy.
+00000700: 056e 756d 7079 da03 6a6e 70da 0b6c 6163  .numpy..jnp..lac
+00000710: 7373 2e74 7970 6573 da06 636f 6d6d 6f6e  ss.types..common
+00000720: da04 756e 6574 7204 0000 00da 064d 6f64  ..unetr......Mod
+00000730: 756c 6572 0500 0000 722e 0000 0072 2e00  uler....r....r..
+00000740: 0000 722e 0000 0072 2f00 0000 da08 3c6d  ..r....r/.....<m
+00000750: 6f64 756c 653e 0100 0000 730c 0000 000c  odule>....s.....
+00000760: 0108 010c 0208 0208 010c 03              ...........
```

### Comparing `lacss-0.4.1/lacss/modules/__pycache__/convnext.cpython-38.pyc` & `lacss-0.4.2/lacss/modules/__pycache__/convnext.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 6646 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,402 +1,469 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 f619 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 e67d ad64 f41e 0000  U........}.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6402 6c07 5a07 6400 6402 6c08 6d09 5a0a  d.l.Z.d.d.l.m.Z.
-00000060: 0100 6403 6404 6c0b 5400 4700 6405 6406  ..d.d.l.T.G.d.d.
-00000070: 8400 6406 6506 6a0c 8303 5a0d 4700 6407  ..d.e.j...Z.G.d.
-00000080: 6408 8400 6408 6506 6a0c 8303 5a0e 6409  d...d.e.j...Z.d.
-00000090: 640a 640b 640c 640d 640e 640f 6410 6411  d.d.d.d.d.d.d.d.
-000000a0: 6412 9c09 5a0f 6413 6414 8400 5a10 6402  d...Z.d.d...Z.d.
-000000b0: 5300 2915 e900 0000 0029 03da 044c 6973  S.)......)...Lis
+00000060: 0100 6400 6403 6c0b 5400 6404 6403 6c0c  ..d.d.l.T.d.d.l.
+00000070: 5400 4700 6405 6406 8400 6406 6506 6a0d  T.G.d.d...d.e.j.
+00000080: 8303 5a0e 6407 6408 6409 640a 640b 640c  ..Z.d.d.d.d.d.d.
+00000090: 640d 640e 640f 6410 9c09 5a0f 4700 6411  d.d.d.d...Z.G.d.
+000000a0: 6412 8400 6412 6506 6a0d 8303 5a10 6402  d...d.e.j...Z.d.
+000000b0: 5300 2913 e900 0000 0029 03da 044c 6973  S.)......)...Lis
 000000c0: 74da 0853 6571 7565 6e63 65da 0555 6e69  t..Sequence..Uni
-000000d0: 6f6e 4ee9 0100 0000 2901 da01 2a63 0000  onN.....)...*c..
-000000e0: 0000 0000 0000 0000 0000 0000 0000 0500  ................
-000000f0: 0000 4000 0000 7356 0000 0065 005a 0164  ..@...sV...e.Z.d
+000000d0: 6f6e 4e29 01da 012a e901 0000 0063 0000  onN)...*.....c..
+000000e0: 0000 0000 0000 0000 0000 0000 0000 0600  ................
+000000f0: 0000 4000 0000 7358 0000 0065 005a 0164  ..@...sX...e.Z.d
 00000100: 005a 0255 0064 015a 0364 025a 0465 0565  .Z.U.d.Z.d.Z.e.e
 00000110: 0664 033c 0064 045a 0765 0865 0664 053c  .d.<.d.Z.e.e.d.<
 00000120: 0064 065a 0965 0565 0664 073c 0065 0a6a  .d.Z.e.e.d.<.e.j
-00000130: 0b64 0864 099c 0165 0c6a 0d65 0c6a 0d64  .d.d...e.j.e.j.d
-00000140: 0a9c 0264 0b64 0c84 0683 015a 0e64 0853  ...d.d.....Z.d.S
-00000150: 0029 0dda 065f 426c 6f63 6b7a b043 6f6e  .)..._Blockz.Con
-00000160: 764e 6558 7420 426c 6f63 6b2e 0a20 2020  vNeXt Block..   
-00000170: 2041 7267 733a 0a20 2020 2020 2020 2064   Args:.        d
-00000180: 726f 705f 7061 7468 2028 666c 6f61 7429  rop_path (float)
-00000190: 3a20 5374 6f63 6861 7374 6963 2064 6570  : Stochastic dep
-000001a0: 7468 2072 6174 652e 2044 6566 6175 6c74  th rate. Default
-000001b0: 3a20 302e 300a 2020 2020 2020 2020 6c61  : 0.0.        la
-000001c0: 7965 725f 7363 616c 655f 696e 6974 5f76  yer_scale_init_v
-000001d0: 616c 7565 2028 666c 6f61 7429 3a20 496e  alue (float): In
-000001e0: 6974 2076 616c 7565 2066 6f72 204c 6179  it value for Lay
-000001f0: 6572 2053 6361 6c65 2e20 4465 6661 756c  er Scale. Defaul
-00000200: 743a 2031 652d 362e 0a20 2020 20e7 0000  t: 1e-6..    ...
-00000210: 0000 0000 0000 da09 6472 6f70 5f72 6174  ........drop_rat
-00000220: 65e7 8ded b5a0 f7c6 b03e da16 6c61 7965  e........>..laye
-00000230: 725f 7363 616c 655f 696e 6974 5f76 616c  r_scale_init_val
-00000240: 7565 e907 0000 00da 0b6b 6572 6e65 6c5f  ue.......kernel_
-00000250: 7369 7a65 4ea9 01da 0874 7261 696e 696e  sizeN....trainin
-00000260: 6729 02da 0178 da06 7265 7475 726e 6302  g)...x..returnc.
-00000270: 0000 0000 0000 0001 0000 0008 0000 0006  ................
-00000280: 0000 0003 0000 0073 c600 0000 7c01 6a00  .......s....|.j.
-00000290: 6401 1900 7d03 7c00 6a01 7d04 7c00 6a02  d...}.|.j.}.|.j.
-000002a0: 8900 7c01 7d05 7403 6a04 7c03 7c04 7c04  ..|.}.t.j.|.|.|.
-000002b0: 6602 7c03 6402 8d03 7c01 8301 7d01 7403  f.|.d...|...}.t.
-000002c0: 6a05 6403 6404 8d01 7c01 8301 7d01 7403  j.d.d...|...}.t.
-000002d0: a006 7c03 6405 1400 a101 7c01 8301 7d01  ..|.d.....|...}.
-000002e0: 7407 6a03 a008 7c01 a101 7d01 7403 a006  t.j...|...}.t...
-000002f0: 7c03 a101 7c01 8301 7d01 8800 6406 6b04  |...|...}...d.k.
-00000300: 729a 7c00 a009 6407 8700 6601 6408 6409  r.|...d...f.d.d.
-00000310: 8408 7c01 6a00 6401 1900 a103 7d06 7c01  ..|.j.d.....}.|.
-00000320: 7c06 1400 7d01 7c02 6400 6b08 70a6 7c02  |...}.|.d.k.p.|.
-00000330: 0c00 7d07 740a 7c00 6a0b 8301 7c01 7c07  ..}.t.|.j...|.|.
-00000340: 640a 8d02 7d01 7c01 7c05 1700 7d01 7c01  d...}.|.|...}.|.
-00000350: 5300 290b 4ee9 ffff ffff 2901 da13 6665  S.).N.....)...fe
-00000360: 6174 7572 655f 6772 6f75 705f 636f 756e  ature_group_coun
-00000370: 7472 0a00 0000 a901 da07 6570 7369 6c6f  tr........epsilo
-00000380: 6ee9 0400 0000 7201 0000 00da 0567 616d  n.....r......gam
-00000390: 6d61 6302 0000 0000 0000 0000 0000 0002  mac.............
-000003a0: 0000 0004 0000 0013 0000 0073 0e00 0000  ...........s....
-000003b0: 8800 7400 a001 7c01 a101 1400 5300 a901  ..t...|.....S...
-000003c0: 4e29 02da 036a 6e70 da04 6f6e 6573 2902  N)...jnp..ones).
-000003d0: da03 726e 67da 0573 6861 7065 a901 da05  ..rng..shape....
-000003e0: 7363 616c 65a9 00fa 392f 686f 6d65 2f46  scale...9/home/F
-000003f0: 4341 4d2f 6a79 752f 7072 6f6a 5f6c 6163  CAM/jyu/proj_lac
-00000400: 7373 2f6c 6163 7373 2f6c 6163 7373 2f6d  ss/lacss/lacss/m
-00000410: 6f64 756c 6573 2f63 6f6e 766e 6578 742e  odules/convnext.
-00000420: 7079 da08 3c6c 616d 6264 613e 2900 0000  py..<lambda>)...
-00000430: f300 0000 007a 215f 426c 6f63 6b2e 5f5f  .....z!_Block.__
-00000440: 6361 6c6c 5f5f 2e3c 6c6f 6361 6c73 3e2e  call__.<locals>.
-00000450: 3c6c 616d 6264 613e 2901 da0d 6465 7465  <lambda>)...dete
-00000460: 726d 696e 6973 7469 6329 0c72 1c00 0000  rministic).r....
-00000470: 720d 0000 0072 0b00 0000 da02 6e6e da04  r....r......nn..
-00000480: 436f 6e76 da09 4c61 7965 724e 6f72 6dda  Conv..LayerNorm.
-00000490: 0544 656e 7365 da03 6a61 78da 0467 656c  .Dense..jax..gel
-000004a0: 75da 0570 6172 616d da08 4472 6f70 5061  u..param..DropPa
-000004b0: 7468 7209 0000 0029 08da 0473 656c 6672  thr....)...selfr
-000004c0: 1000 0000 720f 0000 00da 0364 696d da02  ....r......dim..
-000004d0: 6b73 da08 7368 6f72 7463 7574 7217 0000  ks..shortcutr...
-000004e0: 0072 2300 0000 721f 0000 0072 1d00 0000  .r#...r....r....
-000004f0: 7220 0000 00da 085f 5f63 616c 6c5f 5f19  r .....__call__.
-00000500: 0000 0073 2800 0000 0002 0a01 0601 0602  ...s(...........
-00000510: 0402 1801 1001 1201 0c01 0e02 0801 0401  ................
-00000520: 0200 0a00 08ff 0403 0802 0e01 1202 0802  ................
-00000530: 7a0f 5f42 6c6f 636b 2e5f 5f63 616c 6c5f  z._Block.__call_
-00000540: 5f29 0fda 085f 5f6e 616d 655f 5fda 0a5f  _)...__name__.._
-00000550: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000560: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-00000570: 7209 0000 00da 0369 6e74 da0f 5f5f 616e  r......int..__an
-00000580: 6e6f 7461 7469 6f6e 735f 5f72 0b00 0000  notations__r....
-00000590: da05 666c 6f61 7472 0d00 0000 7224 0000  ..floatr....r$..
-000005a0: 00da 0763 6f6d 7061 6374 7219 0000 00da  ...compactr.....
-000005b0: 076e 6461 7272 6179 7230 0000 0072 1f00  .ndarrayr0...r..
-000005c0: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-000005d0: 0072 0700 0000 0e00 0000 730c 0000 000a  .r........s.....
-000005e0: 0104 060c 010c 010c 0204 0172 0700 0000  ...........r....
-000005f0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000600: 0006 0000 0040 0000 0073 8400 0000 6500  .....@...s....e.
-00000610: 5a01 6400 5a02 5500 6401 5a03 6402 5a04  Z.d.Z.U.d.Z.d.Z.
-00000620: 6505 6506 6403 3c00 6404 5a07 6508 6505  e.e.d.<.d.Z.e.e.
-00000630: 1900 6506 6405 3c00 6406 5a09 6508 6505  ..e.d.<.d.Z.e.e.
-00000640: 1900 6506 6407 3c00 6408 5a0a 650b 6506  ..e.d.<.d.Z.e.e.
-00000650: 6409 3c00 640a 5a0c 650b 6506 640b 3c00  d.<.d.Z.e.e.d.<.
-00000660: 640c 5a0d 6505 6506 640d 3c00 650e 6a0f  d.Z.e.e.d.<.e.j.
-00000670: 640e 640f 9c01 6510 6a11 6512 6510 6a11  d.d...e.j.e.e.j.
-00000680: 6410 9c03 6411 6412 8406 8301 5a13 640e  d...d.d.....Z.d.
-00000690: 5300 2913 da08 436f 6e76 4e65 5874 61b7  S.)...ConvNeXta.
-000006a0: 0100 0043 6f6e 764e 6558 740a 2020 2020  ...ConvNeXt.    
-000006b0: 4172 6773 3a0a 2020 2020 2020 2020 7061  Args:.        pa
-000006c0: 7463 685f 7369 7a65 3a20 666f 7220 7374  tch_size: for st
-000006d0: 656d 2064 6566 6175 6c74 2034 0a20 2020  em default 4.   
-000006e0: 2020 2020 2064 6570 7468 7320 2874 7570       depths (tup
-000006f0: 6c65 2869 6e74 2929 3a20 4e75 6d62 6572  le(int)): Number
-00000700: 206f 6620 626c 6f63 6b73 2061 7420 6561   of blocks at ea
-00000710: 6368 2073 7461 6765 2e20 4465 6661 756c  ch stage. Defaul
-00000720: 743a 205b 332c 2033 2c20 392c 2033 5d0a  t: [3, 3, 9, 3].
-00000730: 2020 2020 2020 2020 6469 6d73 2028 696e          dims (in
-00000740: 7429 3a20 4665 6174 7572 6520 6469 6d65  t): Feature dime
-00000750: 6e73 696f 6e20 6174 2065 6163 6820 7374  nsion at each st
-00000760: 6167 652e 2044 6566 6175 6c74 3a20 5b39  age. Default: [9
-00000770: 362c 2031 3932 2c20 3338 342c 2037 3638  6, 192, 384, 768
-00000780: 5d0a 2020 2020 2020 2020 6472 6f70 5f70  ].        drop_p
-00000790: 6174 685f 7261 7465 2028 666c 6f61 7429  ath_rate (float)
-000007a0: 3a20 5374 6f63 6861 7374 6963 2064 6570  : Stochastic dep
-000007b0: 7468 2072 6174 652e 2044 6566 6175 6c74  th rate. Default
-000007c0: 3a20 302e 0a20 2020 2020 2020 206c 6179  : 0..        lay
-000007d0: 6572 5f73 6361 6c65 5f69 6e69 745f 7661  er_scale_init_va
-000007e0: 6c75 6520 2866 6c6f 6174 293a 2049 6e69  lue (float): Ini
-000007f0: 7420 7661 6c75 6520 666f 7220 4c61 7965  t value for Laye
-00000800: 7220 5363 616c 652e 2044 6566 6175 6c74  r Scale. Default
-00000810: 3a20 3165 2d36 2e0a 2020 2020 2020 2020  : 1e-6..        
-00000820: 6f75 745f 6368 616e 6e65 6c73 2028 696e  out_channels (in
-00000830: 7429 3a20 4650 4e20 6f75 7470 7574 2063  t): FPN output c
-00000840: 6861 6e6e 656c 732e 2044 6566 6175 6c74  hannels. Default
-00000850: 3a20 3235 360a 2020 2020 7216 0000 00da  : 256.    r.....
-00000860: 0a70 6174 6368 5f73 697a 6529 04e9 0300  .patch_size)....
-00000870: 0000 723c 0000 00e9 1b00 0000 723c 0000  ..r<........r<..
-00000880: 00da 0664 6570 7468 7329 04e9 6000 0000  ...depths)..`...
-00000890: e9c0 0000 00e9 8001 0000 6900 0300 00da  ..........i.....
-000008a0: 0464 696d 7372 0800 0000 da0e 6472 6f70  .dimsr......drop
-000008b0: 5f70 6174 685f 7261 7465 720a 0000 0072  _path_rater....r
-000008c0: 0b00 0000 7241 0000 00da 0c6f 7574 5f63  ....rA.....out_c
-000008d0: 6861 6e6e 656c 734e 720e 0000 0029 0372  hannelsNr....).r
-000008e0: 1000 0000 720f 0000 0072 1100 0000 6302  ....r....r....c.
-000008f0: 0000 0000 0000 0001 0000 000b 0000 0006  ................
-00000900: 0000 0003 0000 0073 2c01 0000 6401 7d03  .......s,...d.}.
-00000910: 6700 7d04 7400 7401 8800 6a02 8301 8301  g.}.t.t...j.....
-00000920: 4400 5dba 7d05 7c05 6401 6b02 725c 8800  D.].}.|.d.k.r\..
-00000930: 6a03 7d06 7404 6a05 8800 6a06 7c05 1900  j.}.t.j...j.|...
-00000940: 7c06 7c06 6602 7c06 7c06 6602 6402 8d03  |.|.f.|.|.f.d...
-00000950: 7c01 8301 7d01 7404 6a07 6403 6404 8d01  |...}.t.j.d.d...
-00000960: 7c01 8301 7d01 6e2a 7404 6a07 6403 6404  |...}.n*t.j.d.d.
-00000970: 8d01 7c01 8301 7d01 7404 6a05 8800 6a06  ..|...}.t.j...j.
-00000980: 7c05 1900 6405 6405 6402 8d03 7c01 8301  |...d.d.d...|...
-00000990: 7d01 7400 8800 6a02 7c05 1900 8301 4400  }.t...j.|.....D.
-000009a0: 5d30 7d07 7408 7c03 8800 6a09 8302 7c01  ]0}.t.|...j...|.
-000009b0: 7c02 6406 8d02 7d01 7c03 8800 6a0a 740b  |.d...}.|...j.t.
-000009c0: 8800 6a02 8301 6407 1800 1b00 3700 7d03  ..j...d.....7.}.
-000009d0: 7194 7c04 a00c 7c01 a101 0100 7116 8700  q.|...|.....q...
-000009e0: 6601 6408 6409 8408 7400 640a 8301 4400  f.d.d...t.d...D.
-000009f0: 8301 7d08 740d 740e 7c08 7c04 8302 8301  ..}.t.t.|.|.....
-00000a00: 7d09 8800 6a0f 6401 6b04 9001 7220 7410  }...j.d.k...r t.
-00000a10: 8800 6a0f 8301 7c04 8301 7d0a 740d 740e  ..j...|...}.t.t.
-00000a20: 7c08 7c0a 8302 8301 7d0a 6e04 6400 7d0a  |.|.....}.n.d.}.
-00000a30: 7c09 7c0a 6602 5300 290b 4e72 0100 0000  |.|.f.S.).Nr....
-00000a40: 2901 da07 7374 7269 6465 7372 0a00 0000  )...stridesr....
-00000a50: 7214 0000 0029 02e9 0200 0000 7246 0000  r....)......rF..
-00000a60: 0072 0e00 0000 7205 0000 0063 0100 0000  .r....r....c....
-00000a70: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00000a80: 1300 0000 732a 0000 0067 007c 005d 227d  ....s*...g.|.]"}
-00000a90: 0174 0088 006a 0164 006b 0272 1c7c 0164  .t...j.d.k.r.|.d
-00000aa0: 0117 006e 067c 0164 0017 0083 0191 0271  ...n.|.d.......q
-00000ab0: 0453 0029 0272 4600 0000 7205 0000 0029  .S.).rF...r....)
-00000ac0: 02da 0373 7472 723b 0000 0029 02da 022e  ...strr;...)....
-00000ad0: 30da 016b a901 722c 0000 0072 1f00 0000  0..k..r,...r....
-00000ae0: 7220 0000 00da 0a3c 6c69 7374 636f 6d70  r .....<listcomp
-00000af0: 3e5a 0000 0073 0400 0000 0600 0200 7a25  >Z...s........z%
-00000b00: 436f 6e76 4e65 5874 2e5f 5f63 616c 6c5f  ConvNeXt.__call_
-00000b10: 5f2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  _.<locals>.<list
-00000b20: 636f 6d70 3e72 1600 0000 2911 da05 7261  comp>r....)...ra
-00000b30: 6e67 65da 036c 656e 723e 0000 0072 3b00  nge..lenr>...r;.
-00000b40: 0000 7224 0000 0072 2500 0000 7242 0000  ..r$...r%...rB..
-00000b50: 0072 2600 0000 7207 0000 0072 0b00 0000  .r&...r....r....
-00000b60: 7243 0000 00da 0373 756d da06 6170 7065  rC.....sum..appe
-00000b70: 6e64 da04 6469 6374 da03 7a69 7072 4400  nd..dict..ziprD.
-00000b80: 0000 da03 4650 4e29 0b72 2c00 0000 7210  ....FPN).r,...r.
-00000b90: 0000 0072 0f00 0000 5a07 6470 5f72 6174  ...r....Z.dp_rat
-00000ba0: 65da 076f 7574 7075 7473 7249 0000 00da  e..outputsrI....
-00000bb0: 0270 73da 015f da04 6b65 7973 da0b 656e  .ps.._..keys..en
-00000bc0: 636f 6465 725f 6f75 74da 0b64 6563 6f64  coder_out..decod
-00000bd0: 6572 5f6f 7574 721f 0000 0072 4a00 0000  er_outr....rJ...
-00000be0: 7220 0000 0072 3000 0000 4700 0000 7328  r ...r0...G...s(
-00000bf0: 0000 0000 0204 0104 0112 0108 0106 0122  ..............."
-00000c00: 0112 0210 011a 0212 0114 011a 020c 0216  ................
-00000c10: 010e 020c 010e 0110 0204 027a 1143 6f6e  ...........z.Con
-00000c20: 764e 6558 742e 5f5f 6361 6c6c 5f5f 2914  vNeXt.__call__).
-00000c30: 7231 0000 0072 3200 0000 7233 0000 0072  r1...r2...r3...r
-00000c40: 3400 0000 723b 0000 0072 3500 0000 7236  4...r;...r5...r6
-00000c50: 0000 0072 3e00 0000 7203 0000 0072 4200  ...r>...r....rB.
-00000c60: 0000 7243 0000 0072 3700 0000 720b 0000  ..rC...r7...r...
-00000c70: 0072 4400 0000 7224 0000 0072 3800 0000  .rD...r$...r8...
-00000c80: 7219 0000 0072 3900 0000 da04 626f 6f6c  r....r9.....bool
-00000c90: 7230 0000 0072 1f00 0000 721f 0000 0072  r0...r....r....r
-00000ca0: 1f00 0000 7220 0000 0072 3a00 0000 3500  ....r ...r:...5.
-00000cb0: 0000 7312 0000 000a 0104 0a0c 0110 0110  ..s.............
-00000cc0: 010c 010c 010c 0204 0172 3a00 0000 7a44  .........r:...zD
-00000cd0: 6874 7470 733a 2f2f 646c 2e66 6261 6970  https://dl.fbaip
-00000ce0: 7562 6c69 6366 696c 6573 2e63 6f6d 2f63  ublicfiles.com/c
-00000cf0: 6f6e 766e 6578 742f 636f 6e76 6e65 7874  onvnext/convnext
-00000d00: 5f74 696e 795f 316b 5f32 3234 5f65 6d61  _tiny_1k_224_ema
-00000d10: 2e70 7468 7a45 6874 7470 733a 2f2f 646c  .pthzEhttps://dl
-00000d20: 2e66 6261 6970 7562 6c69 6366 696c 6573  .fbaipublicfiles
-00000d30: 2e63 6f6d 2f63 6f6e 766e 6578 742f 636f  .com/convnext/co
-00000d40: 6e76 6e65 7874 5f73 6d61 6c6c 5f31 6b5f  nvnext_small_1k_
-00000d50: 3232 345f 656d 612e 7074 687a 4468 7474  224_ema.pthzDhtt
-00000d60: 7073 3a2f 2f64 6c2e 6662 6169 7075 626c  ps://dl.fbaipubl
-00000d70: 6963 6669 6c65 732e 636f 6d2f 636f 6e76  icfiles.com/conv
-00000d80: 6e65 7874 2f63 6f6e 766e 6578 745f 6261  next/convnext_ba
-00000d90: 7365 5f31 6b5f 3232 345f 656d 612e 7074  se_1k_224_ema.pt
-00000da0: 687a 4568 7474 7073 3a2f 2f64 6c2e 6662  hzEhttps://dl.fb
-00000db0: 6169 7075 626c 6963 6669 6c65 732e 636f  aipublicfiles.co
-00000dc0: 6d2f 636f 6e76 6e65 7874 2f63 6f6e 766e  m/convnext/convn
-00000dd0: 6578 745f 6c61 7267 655f 316b 5f32 3234  ext_large_1k_224
-00000de0: 5f65 6d61 2e70 7468 7a41 6874 7470 733a  _ema.pthzAhttps:
-00000df0: 2f2f 646c 2e66 6261 6970 7562 6c69 6366  //dl.fbaipublicf
-00000e00: 696c 6573 2e63 6f6d 2f63 6f6e 766e 6578  iles.com/convnex
-00000e10: 742f 636f 6e76 6e65 7874 5f74 696e 795f  t/convnext_tiny_
-00000e20: 3232 6b5f 3232 342e 7074 687a 4268 7474  22k_224.pthzBhtt
-00000e30: 7073 3a2f 2f64 6c2e 6662 6169 7075 626c  ps://dl.fbaipubl
-00000e40: 6963 6669 6c65 732e 636f 6d2f 636f 6e76  icfiles.com/conv
-00000e50: 6e65 7874 2f63 6f6e 766e 6578 745f 736d  next/convnext_sm
-00000e60: 616c 6c5f 3232 6b5f 3232 342e 7074 687a  all_22k_224.pthz
-00000e70: 4168 7474 7073 3a2f 2f64 6c2e 6662 6169  Ahttps://dl.fbai
-00000e80: 7075 626c 6963 6669 6c65 732e 636f 6d2f  publicfiles.com/
-00000e90: 636f 6e76 6e65 7874 2f63 6f6e 766e 6578  convnext/convnex
-00000ea0: 745f 6261 7365 5f32 326b 5f32 3234 2e70  t_base_22k_224.p
-00000eb0: 7468 7a42 6874 7470 733a 2f2f 646c 2e66  thzBhttps://dl.f
-00000ec0: 6261 6970 7562 6c69 6366 696c 6573 2e63  baipublicfiles.c
-00000ed0: 6f6d 2f63 6f6e 766e 6578 742f 636f 6e76  om/convnext/conv
-00000ee0: 6e65 7874 5f6c 6172 6765 5f32 326b 5f32  next_large_22k_2
-00000ef0: 3234 2e70 7468 7a43 6874 7470 733a 2f2f  24.pthzChttps://
-00000f00: 646c 2e66 6261 6970 7562 6c69 6366 696c  dl.fbaipublicfil
-00000f10: 6573 2e63 6f6d 2f63 6f6e 766e 6578 742f  es.com/convnext/
-00000f20: 636f 6e76 6e65 7874 5f78 6c61 7267 655f  convnext_xlarge_
-00000f30: 3232 6b5f 3232 342e 7074 6829 095a 1063  22k_224.pth).Z.c
-00000f40: 6f6e 766e 6578 745f 7469 6e79 5f31 6b5a  onvnext_tiny_1kZ
-00000f50: 1163 6f6e 766e 6578 745f 736d 616c 6c5f  .convnext_small_
-00000f60: 316b 5a10 636f 6e76 6e65 7874 5f62 6173  1kZ.convnext_bas
-00000f70: 655f 316b 5a11 636f 6e76 6e65 7874 5f6c  e_1kZ.convnext_l
-00000f80: 6172 6765 5f31 6b5a 1163 6f6e 766e 6578  arge_1kZ.convnex
-00000f90: 745f 7469 6e79 5f32 326b 5a12 636f 6e76  t_tiny_22kZ.conv
-00000fa0: 6e65 7874 5f73 6d61 6c6c 5f32 326b 5a11  next_small_22kZ.
-00000fb0: 636f 6e76 6e65 7874 5f62 6173 655f 3232  convnext_base_22
-00000fc0: 6b5a 1263 6f6e 766e 6578 745f 6c61 7267  kZ.convnext_larg
-00000fd0: 655f 3232 6b5a 1363 6f6e 766e 6578 745f  e_22kZ.convnext_
-00000fe0: 786c 6172 6765 5f32 326b 6303 0000 0000  xlarge_22kc.....
-00000ff0: 0000 0000 0000 000f 0000 000a 0000 0043  ...............C
-00001000: 0000 0073 ea02 0000 6401 6402 6c00 7d03  ...s....d.d.l.}.
-00001010: 6401 6403 6c01 6d02 7d04 6d03 7d05 0100  d.d.l.m.}.m.}...
-00001020: 6404 6405 8400 7d06 7c03 6a04 6a05 7c02  d.d...}.|.j.j.|.
-00001030: 6406 6407 8d02 7d07 7c07 6408 1900 7d08  d.d...}.|.d...}.
-00001040: 7c05 7c01 8301 7d01 6401 7d09 7406 6409  |.|...}.d.}.t.d.
-00001050: 8301 4400 9001 5d8c 7d0a 7406 7c00 6a07  ..D...].}.t.|.j.
-00001060: 7c0a 1900 8301 4400 9001 5d76 7d0b 7c01  |.....D...]v}.|.
-00001070: 640a 7c09 9b00 9d02 1900 7d0c 7c06 7c0c  d.|.......}.|.|.
-00001080: 640b 1900 7c08 640c 7c0a 9b00 640d 7c0b  d...|.d.|...d.|.
-00001090: 9b00 640e 9d05 1900 8302 0100 7c06 7c0c  ..d.........|.|.
-000010a0: 640f 1900 6410 1900 7c08 640c 7c0a 9b00  d...d...|.d.|...
-000010b0: 640d 7c0b 9b00 6411 9d05 1900 8302 0100  d.|...d.........
-000010c0: 7c06 7c0c 640f 1900 6412 1900 7c08 640c  |.|.d...d...|.d.
-000010d0: 7c0a 9b00 640d 7c0b 9b00 6413 9d05 1900  |...d.|...d.....
-000010e0: a008 6414 6415 6416 6401 a104 8302 0100  ..d.d.d.d.......
-000010f0: 7c06 7c0c 6417 1900 6410 1900 7c08 640c  |.|.d...d...|.d.
-00001100: 7c0a 9b00 640d 7c0b 9b00 6418 9d05 1900  |...d.|...d.....
-00001110: 8302 0100 7c06 7c0c 6417 1900 6419 1900  ....|.|.d...d...
-00001120: 7c08 640c 7c0a 9b00 640d 7c0b 9b00 641a  |.d.|...d.|...d.
-00001130: 9d05 1900 8302 0100 7c06 7c0c 641b 1900  ........|.|.d...
-00001140: 6410 1900 7c08 640c 7c0a 9b00 640d 7c0b  d...|.d.|...d.|.
-00001150: 9b00 641c 9d05 1900 8302 0100 7c06 7c0c  ..d.........|.|.
-00001160: 641b 1900 6412 1900 7c08 640c 7c0a 9b00  d...d...|.d.|...
-00001170: 640d 7c0b 9b00 641d 9d05 1900 a009 6401  d.|...d.......d.
-00001180: 6416 a102 8302 0100 7c06 7c0c 641e 1900  d.......|.|.d...
-00001190: 6410 1900 7c08 640c 7c0a 9b00 640d 7c0b  d...|.d.|...d.|.
-000011a0: 9b00 641f 9d05 1900 8302 0100 7c06 7c0c  ..d.........|.|.
-000011b0: 641e 1900 6412 1900 7c08 640c 7c0a 9b00  d...d...|.d.|...
-000011c0: 640d 7c0b 9b00 6420 9d05 1900 a009 6401  d.|...d ......d.
-000011d0: 6416 a102 8302 0100 7c09 6416 3700 7d09  d.......|.d.7.}.
-000011e0: 7160 714c 7c01 6417 1900 7d0d 7c06 7c0d  q`qL|.d...}.|.|.
-000011f0: 6410 1900 7c08 6421 1900 8302 0100 7c06  d...|.d!......|.
-00001200: 7c0d 6419 1900 7c08 6422 1900 8302 0100  |.d...|.d"......
-00001210: 7c01 640f 1900 7d0e 7c06 7c0e 6410 1900  |.d...}.|.|.d...
-00001220: 7c08 6423 1900 8302 0100 7c06 7c0e 6412  |.d#......|.|.d.
-00001230: 1900 7c08 6424 1900 a008 6414 6415 6416  ..|.d$....d.d.d.
-00001240: 6401 a104 8302 0100 7406 6416 6409 8302  d.......t.d.d...
-00001250: 4400 5d96 7d0a 7c01 6425 7c0a 9b00 9d02  D.].}.|.d%|.....
-00001260: 1900 7d0d 7c06 7c0d 6410 1900 7c08 6426  ..}.|.|.d...|.d&
-00001270: 7c0a 9b00 6427 9d03 1900 8302 0100 7c06  |...d'........|.
-00001280: 7c0d 6419 1900 7c08 6426 7c0a 9b00 6428  |.d...|.d&|...d(
-00001290: 9d03 1900 8302 0100 7c01 6429 7c0a 9b00  ........|.d)|...
-000012a0: 9d02 1900 7d0e 7c06 7c0e 6410 1900 7c08  ....}.|.|.d...|.
-000012b0: 6426 7c0a 9b00 642a 9d03 1900 8302 0100  d&|...d*........
-000012c0: 7c06 7c0e 6412 1900 7c08 6426 7c0a 9b00  |.|.d...|.d&|...
-000012d0: 642b 9d03 1900 a008 6414 6415 6416 6401  d+......d.d.d.d.
-000012e0: a104 8302 0100 9002 714a 7c04 7c01 8301  ........qJ|.|...
-000012f0: 5300 292c 6176 0100 004c 6f61 6420 7072  S.),av...Load pr
-00001300: 6574 7261 696e 6564 2063 6f6e 766e 6578  etrained convnex
-00001310: 7420 6d6f 6465 6c73 0a20 2020 2073 7065  t models.    spe
-00001320: 6373 2066 6f72 2070 7265 7472 6169 6e65  cs for pretraine
-00001330: 6420 6d6f 6465 6c73 2061 7265 3a0a 2020  d models are:.  
-00001340: 2020 2020 2020 7469 6e79 3a20 6469 6d73        tiny: dims
-00001350: 3d28 3936 2c20 3139 322c 2033 3834 2c20  =(96, 192, 384, 
-00001360: 3736 3829 2c20 6465 7074 6873 3d28 332c  768), depths=(3,
-00001370: 332c 392c 3329 0a20 2020 2020 2020 2073  3,9,3).        s
-00001380: 6d61 6c6c 3a20 6469 6d73 3d28 3936 2c20  mall: dims=(96, 
-00001390: 3139 322c 2033 3834 2c20 3736 3829 2c20  192, 384, 768), 
-000013a0: 6465 7074 6873 3d28 332c 332c 3237 2c33  depths=(3,3,27,3
-000013b0: 290a 2020 2020 2020 2020 6261 7365 3a20  ).        base: 
-000013c0: 6469 6d73 3d28 3132 382c 2032 3536 2c20  dims=(128, 256, 
-000013d0: 3531 322c 2031 3032 3429 2c20 6465 7074  512, 1024), dept
-000013e0: 6873 3d28 332c 332c 3237 2c33 290a 2020  hs=(3,3,27,3).  
-000013f0: 2020 2020 2020 6c61 7267 653a 2064 696d        large: dim
-00001400: 733d 2831 3932 2c20 3338 342c 2037 3638  s=(192, 384, 768
-00001410: 2c20 3135 3336 292c 2064 6570 7468 733d  , 1536), depths=
-00001420: 2833 2c33 2c32 372c 3329 0a20 2020 2020  (3,3,27,3).     
-00001430: 2020 2058 2d6c 6172 6765 3a20 6469 6d73     X-large: dims
-00001440: 3d28 3235 362c 2035 3132 2c20 3130 3234  =(256, 512, 1024
-00001450: 2c20 3230 3438 292c 2064 6570 7468 733d  , 2048), depths=
-00001460: 2833 2c33 2c32 372c 3329 0a20 2020 2072  (3,3,27,3).    r
-00001470: 0100 0000 4e29 02da 0666 7265 657a 65da  ....N)...freeze.
-00001480: 0875 6e66 7265 657a 6563 0200 0000 0000  .unfreezec......
-00001490: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
-000014a0: 0000 7322 0000 0074 00a0 017c 01a1 017d  ..s"...t...|...}
-000014b0: 017c 006a 027c 016a 026b 0273 1a74 0382  .|.j.|.j.k.s.t..
-000014c0: 017c 017d 0064 0053 0072 1800 0000 2904  .|.}.d.S.r....).
-000014d0: 7219 0000 00da 0561 7272 6179 721c 0000  r......arrayr...
-000014e0: 00da 0e41 7373 6572 7469 6f6e 4572 726f  ...AssertionErro
-000014f0: 7229 02da 016d da09 6e65 775f 7661 6c75  r)...m..new_valu
-00001500: 6572 1f00 0000 721f 0000 0072 2000 0000  er....r....r ...
-00001510: da01 7481 0000 0073 0600 0000 0001 0a01  ..t....s........
-00001520: 1001 7a16 6c6f 6164 5f77 6569 6768 742e  ..z.load_weight.
-00001530: 3c6c 6f63 616c 733e 2e74 da03 6370 7529  <locals>.t..cpu)
-00001540: 02da 0375 726c 5a0c 6d61 705f 6c6f 6361  ...urlZ.map_loca
-00001550: 7469 6f6e da05 6d6f 6465 6c72 1600 0000  tion..modelr....
-00001560: 5a07 5f42 6c6f 636b 5f72 1700 0000 7a07  Z._Block_r....z.
-00001570: 7374 6167 6573 2eda 012e 7a06 2e67 616d  stages....z..gam
-00001580: 6d61 5a06 436f 6e76 5f30 da04 6269 6173  maZ.Conv_0..bias
-00001590: 7a0c 2e64 7763 6f6e 762e 6269 6173 da06  z..dwconv.bias..
-000015a0: 6b65 726e 656c 7a0e 2e64 7763 6f6e 762e  kernelz..dwconv.
-000015b0: 7765 6967 6874 7246 0000 0072 3c00 0000  weightrF...r<...
-000015c0: 7205 0000 005a 0b4c 6179 6572 4e6f 726d  r....Z.LayerNorm
-000015d0: 5f30 7a0a 2e6e 6f72 6d2e 6269 6173 721e  _0z..norm.biasr.
-000015e0: 0000 007a 0c2e 6e6f 726d 2e77 6569 6768  ...z..norm.weigh
-000015f0: 745a 0744 656e 7365 5f30 7a0d 2e70 7763  tZ.Dense_0z..pwc
-00001600: 6f6e 7631 2e62 6961 737a 0f2e 7077 636f  onv1.biasz..pwco
-00001610: 6e76 312e 7765 6967 6874 5a07 4465 6e73  nv1.weightZ.Dens
-00001620: 655f 317a 0d2e 7077 636f 6e76 322e 6269  e_1z..pwconv2.bi
-00001630: 6173 7a0f 2e70 7763 6f6e 7632 2e77 6569  asz..pwconv2.wei
-00001640: 6768 747a 1a64 6f77 6e73 616d 706c 655f  ghtz.downsample_
-00001650: 6c61 7965 7273 2e30 2e31 2e62 6961 737a  layers.0.1.biasz
-00001660: 1c64 6f77 6e73 616d 706c 655f 6c61 7965  .downsample_laye
-00001670: 7273 2e30 2e31 2e77 6569 6768 747a 1a64  rs.0.1.weightz.d
-00001680: 6f77 6e73 616d 706c 655f 6c61 7965 7273  ownsample_layers
-00001690: 2e30 2e30 2e62 6961 737a 1c64 6f77 6e73  .0.0.biasz.downs
-000016a0: 616d 706c 655f 6c61 7965 7273 2e30 2e30  ample_layers.0.0
-000016b0: 2e77 6569 6768 745a 0a4c 6179 6572 4e6f  .weightZ.LayerNo
-000016c0: 726d 5f7a 1264 6f77 6e73 616d 706c 655f  rm_z.downsample_
-000016d0: 6c61 7965 7273 2e7a 072e 302e 6269 6173  layers.z..0.bias
-000016e0: 7a09 2e30 2e77 6569 6768 745a 0543 6f6e  z..0.weightZ.Con
-000016f0: 765f 7a07 2e31 2e62 6961 737a 092e 312e  v_z..1.biasz..1.
-00001700: 7765 6967 6874 290a da05 746f 7263 685a  weight)...torchZ
-00001710: 1566 6c61 782e 636f 7265 2e66 726f 7a65  .flax.core.froze
-00001720: 6e5f 6469 6374 725a 0000 0072 5b00 0000  n_dictrZ...r[...
-00001730: 5a03 6875 625a 186c 6f61 645f 7374 6174  Z.hubZ.load_stat
-00001740: 655f 6469 6374 5f66 726f 6d5f 7572 6c72  e_dict_from_urlr
-00001750: 4c00 0000 723e 0000 00da 0770 6572 6d75  L...r>.....permu
-00001760: 7465 da09 7472 616e 7370 6f73 6529 0f5a  te..transpose).Z
-00001770: 096a 6178 5f6d 6f64 656c 5a0a 6a61 785f  .jax_modelZ.jax_
-00001780: 7061 7261 6d73 7262 0000 0072 6700 0000  paramsrb...rg...
-00001790: 725a 0000 0072 5b00 0000 7260 0000 00da  rZ...r[...r`....
-000017a0: 0a63 6865 636b 706f 696e 74da 0670 6172  .checkpoint..par
-000017b0: 616d 73da 0363 6e74 da01 6972 4900 0000  ams..cnt..irI...
-000017c0: da05 626c 6f63 6bda 046e 6f72 6dda 0463  ..block..norm..c
-000017d0: 6f6e 7672 1f00 0000 721f 0000 0072 2000  onvr....r....r .
-000017e0: 0000 da0b 6c6f 6164 5f77 6569 6768 7475  ....load_weightu
-000017f0: 0000 0073 5600 0000 0009 0801 1002 0805  ...sV...........
-00001800: 1001 0801 0802 0401 0e01 1401 0e01 2001  .............. .
-00001810: 2401 0201 0a01 20fe 0404 2401 2401 2401  $..... ...$.$.$.
-00001820: 0201 0a01 1cfe 0404 2401 0201 0a01 1cfe  ........$.......
-00001830: 0405 0c02 0801 1201 1202 0801 1201 1e02  ................
-00001840: 0e01 0e01 1a01 1a01 0e01 1a01 2a02 7271  ............*.rq
-00001850: 0000 0029 11da 0674 7970 696e 6772 0200  ...)...typingr..
-00001860: 0000 7203 0000 0072 0400 0000 da0a 666c  ..r....r......fl
-00001870: 6178 2e6c 696e 656e da05 6c69 6e65 6e72  ax.linen..linenr
-00001880: 2400 0000 7228 0000 00da 096a 6178 2e6e  $...r(.....jax.n
-00001890: 756d 7079 da05 6e75 6d70 7972 1900 0000  umpy..numpyr....
-000018a0: da06 636f 6d6d 6f6e da06 4d6f 6475 6c65  ..common..Module
-000018b0: 7207 0000 0072 3a00 0000 5a0a 6d6f 6465  r....r:...Z.mode
-000018c0: 6c5f 7572 6c73 7271 0000 0072 1f00 0000  l_urlsrq...r....
-000018d0: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
-000018e0: 083c 6d6f 6475 6c65 3e01 0000 0073 2200  .<module>....s".
-000018f0: 0000 1402 0c01 0801 0c02 0807 1227 1234  .............'.4
-00001900: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00001910: 02f7 060d                                ....
+00000130: 0b64 0864 099c 0165 0c65 0d65 0e19 0065  .d.d...e.e.e...e
+00000140: 0f64 0a9c 0364 0b64 0c84 0683 015a 1064  .d...d.d.....Z.d
+00000150: 0853 0029 0dda 065f 426c 6f63 6b7a b043  .S.)..._Blockz.C
+00000160: 6f6e 764e 6558 7420 426c 6f63 6b2e 0a20  onvNeXt Block.. 
+00000170: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00000180: 2064 726f 705f 7061 7468 2028 666c 6f61   drop_path (floa
+00000190: 7429 3a20 5374 6f63 6861 7374 6963 2064  t): Stochastic d
+000001a0: 6570 7468 2072 6174 652e 2044 6566 6175  epth rate. Defau
+000001b0: 6c74 3a20 302e 300a 2020 2020 2020 2020  lt: 0.0.        
+000001c0: 6c61 7965 725f 7363 616c 655f 696e 6974  layer_scale_init
+000001d0: 5f76 616c 7565 2028 666c 6f61 7429 3a20  _value (float): 
+000001e0: 496e 6974 2076 616c 7565 2066 6f72 204c  Init value for L
+000001f0: 6179 6572 2053 6361 6c65 2e20 4465 6661  ayer Scale. Defa
+00000200: 756c 743a 2031 652d 362e 0a20 2020 20e7  ult: 1e-6..    .
+00000210: 0000 0000 0000 0000 da09 6472 6f70 5f72  ..........drop_r
+00000220: 6174 65e7 8ded b5a0 f7c6 b03e da16 6c61  ate........>..la
+00000230: 7965 725f 7363 616c 655f 696e 6974 5f76  yer_scale_init_v
+00000240: 616c 7565 e907 0000 00da 0b6b 6572 6e65  alue.......kerne
+00000250: 6c5f 7369 7a65 4ea9 01da 0874 7261 696e  l_sizeN....train
+00000260: 696e 67a9 03da 0178 720f 0000 00da 0672  ing....xr......r
+00000270: 6574 7572 6e63 0200 0000 0000 0000 0100  eturnc..........
+00000280: 0000 0800 0000 0600 0000 0300 0000 73c6  ..............s.
+00000290: 0000 007c 016a 0064 0119 007d 037c 006a  ...|.j.d...}.|.j
+000002a0: 017d 047c 006a 0289 007c 017d 0574 036a  .}.|.j...|.}.t.j
+000002b0: 047c 037c 047c 0466 027c 0364 028d 037c  .|.|.|.f.|.d...|
+000002c0: 0183 017d 0174 036a 0564 0364 048d 017c  ...}.t.j.d.d...|
+000002d0: 0183 017d 0174 03a0 067c 0364 0514 00a1  ...}.t...|.d....
+000002e0: 017c 0183 017d 0174 076a 03a0 087c 01a1  .|...}.t.j...|..
+000002f0: 017d 0174 03a0 067c 03a1 017c 0183 017d  .}.t...|...|...}
+00000300: 0188 0064 066b 0472 9a7c 00a0 0964 0787  ...d.k.r.|...d..
+00000310: 0066 0164 0864 0984 087c 016a 0064 0119  .f.d.d...|.j.d..
+00000320: 00a1 037d 067c 017c 0614 007d 017c 0264  ...}.|.|...}.|.d
+00000330: 006b 0870 a67c 020c 007d 0774 0a7c 006a  .k.p.|...}.t.|.j
+00000340: 0b83 017c 017c 0764 0a8d 027d 017c 017c  ...|.|.d...}.|.|
+00000350: 0517 007d 017c 0153 0029 0b4e e9ff ffff  ...}.|.S.).N....
+00000360: ff29 01da 1366 6561 7475 7265 5f67 726f  .)...feature_gro
+00000370: 7570 5f63 6f75 6e74 720a 0000 00a9 01da  up_countr.......
+00000380: 0765 7073 696c 6f6e e904 0000 0072 0100  .epsilon.....r..
+00000390: 0000 da05 6761 6d6d 6163 0200 0000 0000  ....gammac......
+000003a0: 0000 0000 0000 0200 0000 0400 0000 1300  ................
+000003b0: 0000 730e 0000 0088 0074 00a0 017c 01a1  ..s......t...|..
+000003c0: 0114 0053 00a9 014e 2902 da03 6a6e 70da  ...S...N)...jnp.
+000003d0: 046f 6e65 7329 02da 0372 6e67 da05 7368  .ones)...rng..sh
+000003e0: 6170 65a9 01da 0573 6361 6c65 a900 fa39  ape....scale...9
+000003f0: 2f68 6f6d 652f 4643 414d 2f6a 7975 2f70  /home/FCAM/jyu/p
+00000400: 726f 6a5f 6c61 6373 732f 6c61 6373 732f  roj_lacss/lacss/
+00000410: 6c61 6373 732f 6d6f 6475 6c65 732f 636f  lacss/modules/co
+00000420: 6e76 6e65 7874 2e70 79da 083c 6c61 6d62  nvnext.py..<lamb
+00000430: 6461 3e2b 0000 00f3 0000 0000 7a21 5f42  da>+........z!_B
+00000440: 6c6f 636b 2e5f 5f63 616c 6c5f 5f2e 3c6c  lock.__call__.<l
+00000450: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e29  ocals>.<lambda>)
+00000460: 01da 0d64 6574 6572 6d69 6e69 7374 6963  ...deterministic
+00000470: 290c 721d 0000 0072 0d00 0000 720b 0000  ).r....r....r...
+00000480: 00da 026e 6eda 0443 6f6e 76da 094c 6179  ...nn..Conv..Lay
+00000490: 6572 4e6f 726d da05 4465 6e73 65da 036a  erNorm..Dense..j
+000004a0: 6178 da04 6765 6c75 da05 7061 7261 6dda  ax..gelu..param.
+000004b0: 0844 726f 7050 6174 6872 0900 0000 2908  .DropPathr....).
+000004c0: da04 7365 6c66 7211 0000 0072 0f00 0000  ..selfr....r....
+000004d0: da03 6469 6dda 026b 73da 0873 686f 7274  ..dim..ks..short
+000004e0: 6375 7472 1800 0000 7224 0000 0072 2000  cutr....r$...r .
+000004f0: 0000 721e 0000 0072 2100 0000 da08 5f5f  ..r....r!.....__
+00000500: 6361 6c6c 5f5f 1b00 0000 7328 0000 0000  call__....s(....
+00000510: 020a 0106 0106 0204 0218 0110 0112 010c  ................
+00000520: 010e 0208 0104 0102 000a 0008 ff04 0308  ................
+00000530: 020e 0112 0208 027a 0f5f 426c 6f63 6b2e  .......z._Block.
+00000540: 5f5f 6361 6c6c 5f5f 2911 da08 5f5f 6e61  __call__)...__na
+00000550: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000560: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+00000570: 5f5f 646f 635f 5f72 0900 0000 da03 696e  __doc__r......in
+00000580: 74da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  t..__annotations
+00000590: 5f5f 720b 0000 00da 0566 6c6f 6174 720d  __r......floatr.
+000005a0: 0000 0072 2500 0000 da07 636f 6d70 6163  ...r%.....compac
+000005b0: 74da 0941 7272 6179 4c69 6b65 da08 4f70  t..ArrayLike..Op
+000005c0: 7469 6f6e 616c da04 626f 6f6c da05 4172  tional..bool..Ar
+000005d0: 7261 7972 3100 0000 7220 0000 0072 2000  rayr1...r ...r .
+000005e0: 0000 7220 0000 0072 2100 0000 7207 0000  ..r ...r!...r...
+000005f0: 0010 0000 0073 0c00 0000 0a01 0406 0c01  .....s..........
+00000600: 0c01 0c02 0401 7207 0000 007a 4468 7474  ......r....zDhtt
+00000610: 7073 3a2f 2f64 6c2e 6662 6169 7075 626c  ps://dl.fbaipubl
+00000620: 6963 6669 6c65 732e 636f 6d2f 636f 6e76  icfiles.com/conv
+00000630: 6e65 7874 2f63 6f6e 766e 6578 745f 7469  next/convnext_ti
+00000640: 6e79 5f31 6b5f 3232 345f 656d 612e 7074  ny_1k_224_ema.pt
+00000650: 687a 4568 7474 7073 3a2f 2f64 6c2e 6662  hzEhttps://dl.fb
+00000660: 6169 7075 626c 6963 6669 6c65 732e 636f  aipublicfiles.co
+00000670: 6d2f 636f 6e76 6e65 7874 2f63 6f6e 766e  m/convnext/convn
+00000680: 6578 745f 736d 616c 6c5f 316b 5f32 3234  ext_small_1k_224
+00000690: 5f65 6d61 2e70 7468 7a44 6874 7470 733a  _ema.pthzDhttps:
+000006a0: 2f2f 646c 2e66 6261 6970 7562 6c69 6366  //dl.fbaipublicf
+000006b0: 696c 6573 2e63 6f6d 2f63 6f6e 766e 6578  iles.com/convnex
+000006c0: 742f 636f 6e76 6e65 7874 5f62 6173 655f  t/convnext_base_
+000006d0: 316b 5f32 3234 5f65 6d61 2e70 7468 7a45  1k_224_ema.pthzE
+000006e0: 6874 7470 733a 2f2f 646c 2e66 6261 6970  https://dl.fbaip
+000006f0: 7562 6c69 6366 696c 6573 2e63 6f6d 2f63  ublicfiles.com/c
+00000700: 6f6e 766e 6578 742f 636f 6e76 6e65 7874  onvnext/convnext
+00000710: 5f6c 6172 6765 5f31 6b5f 3232 345f 656d  _large_1k_224_em
+00000720: 612e 7074 687a 4168 7474 7073 3a2f 2f64  a.pthzAhttps://d
+00000730: 6c2e 6662 6169 7075 626c 6963 6669 6c65  l.fbaipublicfile
+00000740: 732e 636f 6d2f 636f 6e76 6e65 7874 2f63  s.com/convnext/c
+00000750: 6f6e 766e 6578 745f 7469 6e79 5f32 326b  onvnext_tiny_22k
+00000760: 5f32 3234 2e70 7468 7a42 6874 7470 733a  _224.pthzBhttps:
+00000770: 2f2f 646c 2e66 6261 6970 7562 6c69 6366  //dl.fbaipublicf
+00000780: 696c 6573 2e63 6f6d 2f63 6f6e 766e 6578  iles.com/convnex
+00000790: 742f 636f 6e76 6e65 7874 5f73 6d61 6c6c  t/convnext_small
+000007a0: 5f32 326b 5f32 3234 2e70 7468 7a41 6874  _22k_224.pthzAht
+000007b0: 7470 733a 2f2f 646c 2e66 6261 6970 7562  tps://dl.fbaipub
+000007c0: 6c69 6366 696c 6573 2e63 6f6d 2f63 6f6e  licfiles.com/con
+000007d0: 766e 6578 742f 636f 6e76 6e65 7874 5f62  vnext/convnext_b
+000007e0: 6173 655f 3232 6b5f 3232 342e 7074 687a  ase_22k_224.pthz
+000007f0: 4268 7474 7073 3a2f 2f64 6c2e 6662 6169  Bhttps://dl.fbai
+00000800: 7075 626c 6963 6669 6c65 732e 636f 6d2f  publicfiles.com/
+00000810: 636f 6e76 6e65 7874 2f63 6f6e 766e 6578  convnext/convnex
+00000820: 745f 6c61 7267 655f 3232 6b5f 3232 342e  t_large_22k_224.
+00000830: 7074 687a 4368 7474 7073 3a2f 2f64 6c2e  pthzChttps://dl.
+00000840: 6662 6169 7075 626c 6963 6669 6c65 732e  fbaipublicfiles.
+00000850: 636f 6d2f 636f 6e76 6e65 7874 2f63 6f6e  com/convnext/con
+00000860: 766e 6578 745f 786c 6172 6765 5f32 326b  vnext_xlarge_22k
+00000870: 5f32 3234 2e70 7468 2909 5a10 636f 6e76  _224.pth).Z.conv
+00000880: 6e65 7874 5f74 696e 795f 316b 5a11 636f  next_tiny_1kZ.co
+00000890: 6e76 6e65 7874 5f73 6d61 6c6c 5f31 6b5a  nvnext_small_1kZ
+000008a0: 1063 6f6e 766e 6578 745f 6261 7365 5f31  .convnext_base_1
+000008b0: 6b5a 1163 6f6e 766e 6578 745f 6c61 7267  kZ.convnext_larg
+000008c0: 655f 316b 5a11 636f 6e76 6e65 7874 5f74  e_1kZ.convnext_t
+000008d0: 696e 795f 3232 6b5a 1263 6f6e 766e 6578  iny_22kZ.convnex
+000008e0: 745f 736d 616c 6c5f 3232 6b5a 1163 6f6e  t_small_22kZ.con
+000008f0: 766e 6578 745f 6261 7365 5f32 326b 5a12  vnext_base_22kZ.
+00000900: 636f 6e76 6e65 7874 5f6c 6172 6765 5f32  convnext_large_2
+00000910: 326b 5a13 636f 6e76 6e65 7874 5f78 6c61  2kZ.convnext_xla
+00000920: 7267 655f 3232 6b63 0000 0000 0000 0000  rge_22kc........
+00000930: 0000 0000 0000 0000 0700 0000 4000 0000  ............@...
+00000940: 73a4 0000 0065 005a 0164 005a 0255 0064  s....e.Z.d.Z.U.d
+00000950: 015a 0364 025a 0465 0565 0664 033c 0064  .Z.d.Z.e.e.d.<.d
+00000960: 045a 0765 0865 0519 0065 0664 053c 0064  .Z.e.e...e.d.<.d
+00000970: 065a 0965 0865 0519 0065 0664 073c 0064  .Z.e.e...e.d.<.d
+00000980: 085a 0a65 0b65 0664 093c 0064 0a5a 0c65  .Z.e.e.d.<.d.Z.e
+00000990: 0b65 0664 0b3c 0064 0c5a 0d65 0565 0664  .e.d.<.d.Z.e.e.d
+000009a0: 0d3c 0065 0e6a 0f64 0e64 0f9c 0165 1065  .<.e.j.d.d...e.e
+000009b0: 1165 1219 0065 1365 1465 1466 0219 0064  .e...e.e.e.f...d
+000009c0: 109c 0364 1164 1284 0683 015a 1564 1364  ...d.d.....Z.d.d
+000009d0: 1484 005a 1665 1765 1864 159c 0264 1664  ...Z.e.e.d...d.d
+000009e0: 1784 045a 1964 0e53 0029 18da 0843 6f6e  ...Z.d.S.)...Con
+000009f0: 764e 6558 7461 b501 0000 436f 6e76 4e65  vNeXta....ConvNe
+00000a00: 5874 2043 4e4e 2062 6163 6b62 6f6e 650a  Xt CNN backbone.
+00000a10: 0a20 2020 2041 7474 7269 6275 7465 733a  .    Attributes:
+00000a20: 0a20 2020 2020 2020 2070 6174 6368 5f73  .        patch_s
+00000a30: 697a 653a 2053 7465 6d20 7061 7463 6820  ize: Stem patch 
+00000a40: 7369 7a65 0a20 2020 2020 2020 2064 6570  size.        dep
+00000a50: 7468 733a 204e 756d 6265 7220 6f66 2062  ths: Number of b
+00000a60: 6c6f 636b 7320 6174 2065 6163 6820 7374  locks at each st
+00000a70: 6167 652e 0a20 2020 2020 2020 2064 696d  age..        dim
+00000a80: 733a 2046 6561 7475 7265 2064 696d 656e  s: Feature dimen
+00000a90: 7369 6f6e 2061 7420 6561 6368 2073 7461  sion at each sta
+00000aa0: 6765 2e0a 2020 2020 2020 2020 6472 6f70  ge..        drop
+00000ab0: 5f70 6174 685f 7261 7465 3a20 5374 6f63  _path_rate: Stoc
+00000ac0: 6861 7374 6963 2064 6570 7468 2072 6174  hastic depth rat
+00000ad0: 652e 0a20 2020 2020 2020 206c 6179 6572  e..        layer
+00000ae0: 5f73 6361 6c65 5f69 6e69 745f 7661 6c75  _scale_init_valu
+00000af0: 653a 2049 6e69 7420 7661 6c75 6520 666f  e: Init value fo
+00000b00: 7220 4c61 7965 7220 5363 616c 652e 0a20  r Layer Scale.. 
+00000b10: 2020 2020 2020 206f 7574 5f63 6861 6e6e         out_chann
+00000b20: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
+00000b30: 2046 504e 206f 7574 7075 7420 6368 616e   FPN output chan
+00000b40: 6e65 6c73 2e20 5365 7474 696e 6720 7468  nels. Setting th
+00000b50: 6973 2074 6f20 2d31 2064 6973 6162 6c65  is to -1 disable
+00000b60: 2074 6865 2046 504e 2c20 696e 2077 6869   the FPN, in whi
+00000b70: 6368 2063 6173 650a 2020 2020 2020 2020  ch case.        
+00000b80: 2020 2020 7468 6520 6d6f 6465 6c20 6f75      the model ou
+00000b90: 7470 7574 206f 6e6c 7920 656e 636f 6465  tput only encode
+00000ba0: 7220 6f75 7470 7574 732e 0a20 2020 2072  r outputs..    r
+00000bb0: 1700 0000 da0a 7061 7463 685f 7369 7a65  ......patch_size
+00000bc0: 2904 e903 0000 0072 4000 0000 e91b 0000  )......r@.......
+00000bd0: 0072 4000 0000 da06 6465 7074 6873 2904  .r@.....depths).
+00000be0: e960 0000 00e9 c000 0000 e980 0100 0069  .`.............i
+00000bf0: 0003 0000 da04 6469 6d73 7208 0000 00da  ......dimsr.....
+00000c00: 0e64 726f 705f 7061 7468 5f72 6174 6572  .drop_path_rater
+00000c10: 0a00 0000 720b 0000 0072 4500 0000 da0c  ....r....rE.....
+00000c20: 6f75 745f 6368 616e 6e65 6c73 4e72 0e00  out_channelsNr..
+00000c30: 0000 7210 0000 0063 0200 0000 0000 0000  ..r....c........
+00000c40: 0100 0000 0b00 0000 0600 0000 0300 0000  ................
+00000c50: 732c 0100 0064 017d 0367 007d 0474 0074  s,...d.}.g.}.t.t
+00000c60: 0188 006a 0283 0183 0144 005d ba7d 057c  ...j.....D.].}.|
+00000c70: 0564 016b 0272 5c88 006a 037d 0674 046a  .d.k.r\..j.}.t.j
+00000c80: 0588 006a 067c 0519 007c 067c 0666 027c  ...j.|...|.|.f.|
+00000c90: 067c 0666 0264 028d 037c 0183 017d 0174  .|.f.d...|...}.t
+00000ca0: 046a 0764 0364 048d 017c 0183 017d 016e  .j.d.d...|...}.n
+00000cb0: 2a74 046a 0764 0364 048d 017c 0183 017d  *t.j.d.d...|...}
+00000cc0: 0174 046a 0588 006a 067c 0519 0064 0564  .t.j...j.|...d.d
+00000cd0: 0564 028d 037c 0183 017d 0174 0088 006a  .d...|...}.t...j
+00000ce0: 027c 0519 0083 0144 005d 307d 0774 087c  .|.....D.]0}.t.|
+00000cf0: 0388 006a 0983 027c 017c 0264 068d 027d  ...j...|.|.d...}
+00000d00: 017c 0388 006a 0a74 0b88 006a 0283 0164  .|...j.t...j...d
+00000d10: 0718 001b 0037 007d 0371 947c 04a0 0c7c  .....7.}.q.|...|
+00000d20: 01a1 0101 0071 1687 0066 0164 0864 0984  .....q...f.d.d..
+00000d30: 0874 0064 0a83 0144 0083 017d 0874 0d74  .t.d...D...}.t.t
+00000d40: 0e7c 087c 0483 0283 017d 0988 006a 0f64  .|.|.....}...j.d
+00000d50: 016b 0490 0172 2074 1088 006a 0f83 017c  .k...r t...j...|
+00000d60: 0483 017d 0a74 0d74 0e7c 087c 0a83 0283  ...}.t.t.|.|....
+00000d70: 017d 0a6e 0464 0b7d 0a7c 097c 0a66 0253  .}.n.d.}.|.|.f.S
+00000d80: 0029 0c61 7301 0000 0a20 2020 2020 2020  .).as....       
+00000d90: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00000da0: 2020 2078 3a20 496d 6167 6520 696e 7075     x: Image inpu
+00000db0: 742e 0a20 2020 2020 2020 2020 2020 2074  t..            t
+00000dc0: 7261 696e 696e 673a 2057 6865 7468 6572  raining: Whether
+00000dd0: 2072 756e 2074 6865 206e 6574 776f 726b   run the network
+00000de0: 2069 6e20 7472 6169 6e69 6e67 206d 6f64   in training mod
+00000df0: 6520 2869 2e65 2e20 7769 7468 2073 746f  e (i.e. with sto
+00000e00: 6368 6173 7469 6320 6465 7074 6829 0a0a  chastic depth)..
+00000e10: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00000e20: 0a20 2020 2020 2020 2020 2020 2041 2074  .            A t
+00000e30: 7570 6c65 206f 6620 2865 6e63 6f64 6572  uple of (encoder
+00000e40: 5f6f 7574 7075 7473 2c20 6465 636f 6465  _outputs, decode
+00000e50: 725f 6f75 7470 7574 7329 2e20 426f 7468  r_outputs). Both
+00000e60: 2061 7265 2064 6963 7469 6f6e 6172 6965   are dictionarie
+00000e70: 7320 6d61 7070 696e 670a 2020 2020 2020  s mapping.      
+00000e80: 2020 2020 2020 2020 2020 6665 6174 7572            featur
+00000e90: 6520 7363 616c 6520 2865 2e67 2e20 2232  e scale (e.g. "2
+00000ea0: 2229 2074 6f20 6665 6174 7572 6573 2e20  ") to features. 
+00000eb0: 4966 206f 7574 5f63 6861 6e6e 656c 7320  If out_channels 
+00000ec0: 6973 202d 312c 2074 6865 2064 6563 6f64  is -1, the decod
+00000ed0: 6572 5f6f 7574 7075 740a 2020 2020 2020  er_output.      
+00000ee0: 2020 2020 2020 2020 2020 6973 204e 6f6e            is Non
+00000ef0: 652e 0a20 2020 2020 2020 2072 0100 0000  e..        r....
+00000f00: 2901 da07 7374 7269 6465 7372 0a00 0000  )...stridesr....
+00000f10: 7215 0000 0029 02e9 0200 0000 724a 0000  r....)......rJ..
+00000f20: 0072 0e00 0000 7206 0000 0063 0100 0000  .r....r....c....
+00000f30: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00000f40: 1300 0000 732a 0000 0067 007c 005d 227d  ....s*...g.|.]"}
+00000f50: 0174 0088 006a 0164 006b 0272 1c7c 0164  .t...j.d.k.r.|.d
+00000f60: 0117 006e 067c 0164 0017 0083 0191 0271  ...n.|.d.......q
+00000f70: 0453 0029 0272 4a00 0000 7206 0000 0029  .S.).rJ...r....)
+00000f80: 02da 0373 7472 723f 0000 0029 02da 022e  ...strr?...)....
+00000f90: 30da 016b a901 722d 0000 0072 2000 0000  0..k..r-...r ...
+00000fa0: 7221 0000 00da 0a3c 6c69 7374 636f 6d70  r!.....<listcomp
+00000fb0: 3e7a 0000 0073 0400 0000 0600 0200 7a25  >z...s........z%
+00000fc0: 436f 6e76 4e65 5874 2e5f 5f63 616c 6c5f  ConvNeXt.__call_
+00000fd0: 5f2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  _.<locals>.<list
+00000fe0: 636f 6d70 3e72 1700 0000 4e29 11da 0572  comp>r....N)...r
+00000ff0: 616e 6765 da03 6c65 6e72 4200 0000 723f  ange..lenrB...r?
+00001000: 0000 0072 2500 0000 7226 0000 0072 4600  ...r%...r&...rF.
+00001010: 0000 7227 0000 0072 0700 0000 720b 0000  ..r'...r....r...
+00001020: 0072 4700 0000 da03 7375 6dda 0661 7070  .rG.....sum..app
+00001030: 656e 64da 0464 6963 74da 037a 6970 7248  end..dict..ziprH
+00001040: 0000 00da 0346 504e 290b 722d 0000 0072  .....FPN).r-...r
+00001050: 1100 0000 720f 0000 005a 0764 705f 7261  ....r....Z.dp_ra
+00001060: 7465 da07 6f75 7470 7574 7372 4d00 0000  te..outputsrM...
+00001070: da02 7073 da01 5fda 046b 6579 73da 0b65  ..ps.._..keys..e
+00001080: 6e63 6f64 6572 5f6f 7574 da0b 6465 636f  ncoder_out..deco
+00001090: 6465 725f 6f75 7472 2000 0000 724e 0000  der_outr ...rN..
+000010a0: 0072 2100 0000 7231 0000 005b 0000 0073  .r!...r1...[...s
+000010b0: 2800 0000 000e 0401 0401 1201 0801 0601  (...............
+000010c0: 2201 1202 1001 1a02 1201 1401 1a02 0c02  "...............
+000010d0: 1601 0e02 0c01 0e01 1002 0402 7a11 436f  ............z.Co
+000010e0: 6e76 4e65 5874 2e5f 5f63 616c 6c5f 5f63  nvNeXt.__call__c
+000010f0: 0300 0000 0000 0000 0000 0000 0f00 0000  ................
+00001100: 0a00 0000 4300 0000 73ea 0200 0064 0164  ....C...s....d.d
+00001110: 006c 007d 0364 0164 026c 016d 027d 046d  .l.}.d.d.l.m.}.m
+00001120: 037d 0501 0064 0364 0484 007d 067c 036a  .}...d.d...}.|.j
+00001130: 046a 057c 0264 0564 068d 027d 077c 0764  .j.|.d.d...}.|.d
+00001140: 0719 007d 087c 057c 0183 017d 0164 017d  ...}.|.|...}.d.}
+00001150: 0974 0664 0883 0144 0090 015d 8c7d 0a74  .t.d...D...].}.t
+00001160: 067c 006a 077c 0a19 0083 0144 0090 015d  .|.j.|.....D...]
+00001170: 767d 0b7c 0164 097c 099b 009d 0219 007d  v}.|.d.|.......}
+00001180: 0c7c 067c 0c64 0a19 007c 0864 0b7c 0a9b  .|.|.d...|.d.|..
+00001190: 0064 0c7c 0b9b 0064 0d9d 0519 0083 0201  .d.|...d........
+000011a0: 007c 067c 0c64 0e19 0064 0f19 007c 0864  .|.|.d...d...|.d
+000011b0: 0b7c 0a9b 0064 0c7c 0b9b 0064 109d 0519  .|...d.|...d....
+000011c0: 0083 0201 007c 067c 0c64 0e19 0064 1119  .....|.|.d...d..
+000011d0: 007c 0864 0b7c 0a9b 0064 0c7c 0b9b 0064  .|.d.|...d.|...d
+000011e0: 129d 0519 00a0 0864 1364 1464 1564 01a1  .......d.d.d.d..
+000011f0: 0483 0201 007c 067c 0c64 1619 0064 0f19  .....|.|.d...d..
+00001200: 007c 0864 0b7c 0a9b 0064 0c7c 0b9b 0064  .|.d.|...d.|...d
+00001210: 179d 0519 0083 0201 007c 067c 0c64 1619  .........|.|.d..
+00001220: 0064 1819 007c 0864 0b7c 0a9b 0064 0c7c  .d...|.d.|...d.|
+00001230: 0b9b 0064 199d 0519 0083 0201 007c 067c  ...d.........|.|
+00001240: 0c64 1a19 0064 0f19 007c 0864 0b7c 0a9b  .d...d...|.d.|..
+00001250: 0064 0c7c 0b9b 0064 1b9d 0519 0083 0201  .d.|...d........
+00001260: 007c 067c 0c64 1a19 0064 1119 007c 0864  .|.|.d...d...|.d
+00001270: 0b7c 0a9b 0064 0c7c 0b9b 0064 1c9d 0519  .|...d.|...d....
+00001280: 00a0 0964 0164 15a1 0283 0201 007c 067c  ...d.d.......|.|
+00001290: 0c64 1d19 0064 0f19 007c 0864 0b7c 0a9b  .d...d...|.d.|..
+000012a0: 0064 0c7c 0b9b 0064 1e9d 0519 0083 0201  .d.|...d........
+000012b0: 007c 067c 0c64 1d19 0064 1119 007c 0864  .|.|.d...d...|.d
+000012c0: 0b7c 0a9b 0064 0c7c 0b9b 0064 1f9d 0519  .|...d.|...d....
+000012d0: 00a0 0964 0164 15a1 0283 0201 007c 0964  ...d.d.......|.d
+000012e0: 1537 007d 0971 6071 4c7c 0164 1619 007d  .7.}.q`qL|.d...}
+000012f0: 0d7c 067c 0d64 0f19 007c 0864 2019 0083  .|.|.d...|.d ...
+00001300: 0201 007c 067c 0d64 1819 007c 0864 2119  ...|.|.d...|.d!.
+00001310: 0083 0201 007c 0164 0e19 007d 0e7c 067c  .....|.d...}.|.|
+00001320: 0e64 0f19 007c 0864 2219 0083 0201 007c  .d...|.d"......|
+00001330: 067c 0e64 1119 007c 0864 2319 00a0 0864  .|.d...|.d#....d
+00001340: 1364 1464 1564 01a1 0483 0201 0074 0664  .d.d.d.......t.d
+00001350: 1564 0883 0244 005d 967d 0a7c 0164 247c  .d...D.].}.|.d$|
+00001360: 0a9b 009d 0219 007d 0d7c 067c 0d64 0f19  .......}.|.|.d..
+00001370: 007c 0864 257c 0a9b 0064 269d 0319 0083  .|.d%|...d&.....
+00001380: 0201 007c 067c 0d64 1819 007c 0864 257c  ...|.|.d...|.d%|
+00001390: 0a9b 0064 279d 0319 0083 0201 007c 0164  ...d'........|.d
+000013a0: 287c 0a9b 009d 0219 007d 0e7c 067c 0e64  (|.......}.|.|.d
+000013b0: 0f19 007c 0864 257c 0a9b 0064 299d 0319  ...|.d%|...d)...
+000013c0: 0083 0201 007c 067c 0e64 1119 007c 0864  .....|.|.d...|.d
+000013d0: 257c 0a9b 0064 2a9d 0319 00a0 0864 1364  %|...d*......d.d
+000013e0: 1464 1564 01a1 0483 0201 0090 0271 4a7c  .d.d.........qJ|
+000013f0: 047c 0183 0153 0029 2b4e 7201 0000 0029  .|...S.)+Nr....)
+00001400: 02da 0666 7265 657a 65da 0875 6e66 7265  ...freeze..unfre
+00001410: 657a 6563 0200 0000 0000 0000 0000 0000  ezec............
+00001420: 0200 0000 0300 0000 5300 0000 7322 0000  ........S...s"..
+00001430: 0074 00a0 017c 01a1 017d 017c 006a 027c  .t...|...}.|.j.|
+00001440: 016a 026b 0273 1a74 0382 017c 017d 0064  .j.k.s.t...|.}.d
+00001450: 0053 0072 1900 0000 2904 721a 0000 00da  .S.r....).r.....
+00001460: 0561 7272 6179 721d 0000 00da 0e41 7373  .arrayr......Ass
+00001470: 6572 7469 6f6e 4572 726f 7229 02da 016d  ertionError)...m
+00001480: da09 6e65 775f 7661 6c75 6572 2000 0000  ..new_valuer ...
+00001490: 7220 0000 0072 2100 0000 da01 7489 0000  r ...r!.....t...
+000014a0: 0073 0600 0000 0001 0a01 1001 7a20 436f  .s..........z Co
+000014b0: 6e76 4e65 5874 2e5f 6c6f 6164 5f77 6569  nvNeXt._load_wei
+000014c0: 6768 742e 3c6c 6f63 616c 733e 2e74 da03  ght.<locals>.t..
+000014d0: 6370 7529 02da 0375 726c 5a0c 6d61 705f  cpu)...urlZ.map_
+000014e0: 6c6f 6361 7469 6f6e da05 6d6f 6465 6c72  location..modelr
+000014f0: 1700 0000 5a07 5f42 6c6f 636b 5f72 1800  ....Z._Block_r..
+00001500: 0000 7a07 7374 6167 6573 2eda 012e 7a06  ..z.stages....z.
+00001510: 2e67 616d 6d61 5a06 436f 6e76 5f30 da04  .gammaZ.Conv_0..
+00001520: 6269 6173 7a0c 2e64 7763 6f6e 762e 6269  biasz..dwconv.bi
+00001530: 6173 da06 6b65 726e 656c 7a0e 2e64 7763  as..kernelz..dwc
+00001540: 6f6e 762e 7765 6967 6874 724a 0000 0072  onv.weightrJ...r
+00001550: 4000 0000 7206 0000 005a 0b4c 6179 6572  @...r....Z.Layer
+00001560: 4e6f 726d 5f30 7a0a 2e6e 6f72 6d2e 6269  Norm_0z..norm.bi
+00001570: 6173 721f 0000 007a 0c2e 6e6f 726d 2e77  asr....z..norm.w
+00001580: 6569 6768 745a 0744 656e 7365 5f30 7a0d  eightZ.Dense_0z.
+00001590: 2e70 7763 6f6e 7631 2e62 6961 737a 0f2e  .pwconv1.biasz..
+000015a0: 7077 636f 6e76 312e 7765 6967 6874 5a07  pwconv1.weightZ.
+000015b0: 4465 6e73 655f 317a 0d2e 7077 636f 6e76  Dense_1z..pwconv
+000015c0: 322e 6269 6173 7a0f 2e70 7763 6f6e 7632  2.biasz..pwconv2
+000015d0: 2e77 6569 6768 747a 1a64 6f77 6e73 616d  .weightz.downsam
+000015e0: 706c 655f 6c61 7965 7273 2e30 2e31 2e62  ple_layers.0.1.b
+000015f0: 6961 737a 1c64 6f77 6e73 616d 706c 655f  iasz.downsample_
+00001600: 6c61 7965 7273 2e30 2e31 2e77 6569 6768  layers.0.1.weigh
+00001610: 747a 1a64 6f77 6e73 616d 706c 655f 6c61  tz.downsample_la
+00001620: 7965 7273 2e30 2e30 2e62 6961 737a 1c64  yers.0.0.biasz.d
+00001630: 6f77 6e73 616d 706c 655f 6c61 7965 7273  ownsample_layers
+00001640: 2e30 2e30 2e77 6569 6768 745a 0a4c 6179  .0.0.weightZ.Lay
+00001650: 6572 4e6f 726d 5f7a 1264 6f77 6e73 616d  erNorm_z.downsam
+00001660: 706c 655f 6c61 7965 7273 2e7a 072e 302e  ple_layers.z..0.
+00001670: 6269 6173 7a09 2e30 2e77 6569 6768 745a  biasz..0.weightZ
+00001680: 0543 6f6e 765f 7a07 2e31 2e62 6961 737a  .Conv_z..1.biasz
+00001690: 092e 312e 7765 6967 6874 290a da05 746f  ..1.weight)...to
+000016a0: 7263 68da 1566 6c61 782e 636f 7265 2e66  rch..flax.core.f
+000016b0: 726f 7a65 6e5f 6469 6374 725d 0000 0072  rozen_dictr]...r
+000016c0: 5e00 0000 5a03 6875 625a 186c 6f61 645f  ^...Z.hubZ.load_
+000016d0: 7374 6174 655f 6469 6374 5f66 726f 6d5f  state_dict_from_
+000016e0: 7572 6c72 5000 0000 7242 0000 00da 0770  urlrP...rB.....p
+000016f0: 6572 6d75 7465 da09 7472 616e 7370 6f73  ermute..transpos
+00001700: 6529 0f72 2d00 0000 5a0a 6a61 785f 7061  e).r-...Z.jax_pa
+00001710: 7261 6d73 7265 0000 0072 6a00 0000 725d  ramsre...rj...r]
+00001720: 0000 0072 5e00 0000 7263 0000 00da 0a63  ...r^...rc.....c
+00001730: 6865 636b 706f 696e 74da 0670 6172 616d  heckpoint..param
+00001740: 73da 0363 6e74 da01 6972 4d00 0000 da05  s..cnt..irM.....
+00001750: 626c 6f63 6bda 046e 6f72 6dda 0463 6f6e  block..norm..con
+00001760: 7672 2000 0000 7220 0000 0072 2100 0000  vr ...r ...r!...
+00001770: da0c 5f6c 6f61 645f 7765 6967 6874 8500  .._load_weight..
+00001780: 0000 735c 0000 0000 0108 0110 0208 0510  ..s\............
+00001790: 0108 0108 0204 010e 0114 010e 0120 0124  ............. .$
+000017a0: 0102 010a 0120 fe04 0424 0124 0124 0102  ..... ...$.$.$..
+000017b0: 010a 011c fe04 0424 0102 010a 011c fe04  .......$........
+000017c0: 050c 0208 0112 0112 0208 0112 011e 020e  ................
+000017d0: 010e 011a 011a 010e 011a 0102 0106 011a  ................
+000017e0: fe08 057a 1543 6f6e 764e 6558 742e 5f6c  ...z.ConvNeXt._l
+000017f0: 6f61 645f 7765 6967 6874 2902 da0a 6d6f  oad_weight)...mo
+00001800: 6465 6c5f 7479 7065 7212 0000 0063 0200  del_typer....c..
+00001810: 0000 0000 0000 0000 0000 0400 0000 0800  ................
+00001820: 0000 4300 0000 7344 0000 007c 00a0 0074  ..C...sD...|...t
+00001830: 016a 02a0 0364 01a1 0174 04a0 0564 0264  .j...d...t...d.d
+00001840: 0264 0367 03a1 01a1 027d 027c 0264 0419  .d.g.....}.|.d..
+00001850: 007d 027c 00a0 067c 0274 0764 057c 019b  .}.|...|.t.d.|..
+00001860: 0064 069d 0319 00a1 027d 037c 0353 0029  .d.......}.|.S.)
+00001870: 0761 5e02 0000 4765 7420 696d 6167 656e  .a^...Get imagen
+00001880: 6574 2077 6569 6768 7473 0a0a 2020 2020  et weights..    
+00001890: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+000018a0: 2020 2020 2020 6d6f 6465 6c5f 7479 7065        model_type
+000018b0: 3a20 5468 6520 6578 7065 6374 6564 206d  : The expected m
+000018c0: 6f64 656c 2073 7065 6369 6669 6361 7469  odel specificati
+000018d0: 6f6e 2e20 5468 6973 206d 7573 7420 6d61  on. This must ma
+000018e0: 7463 6820 7468 6520 6375 7272 656e 740a  tch the current.
+000018f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001900: 696e 7374 616e 6365 2061 7474 7269 6275  instance attribu
+00001910: 7465 732e 0a0a 2020 2020 2020 2020 2020  tes...          
+00001920: 2020 2020 2020 2a20 7469 6e79 3a20 6469        * tiny: di
+00001930: 6d73 3d28 3936 2c20 3139 322c 2033 3834  ms=(96, 192, 384
+00001940: 2c20 3736 3829 2c20 6465 7074 6873 3d28  , 768), depths=(
+00001950: 332c 332c 392c 3329 0a20 2020 2020 2020  3,3,9,3).       
+00001960: 2020 2020 2020 2020 202a 2073 6d61 6c6c           * small
+00001970: 3a20 6469 6d73 3d28 3936 2c20 3139 322c  : dims=(96, 192,
+00001980: 2033 3834 2c20 3736 3829 2c20 6465 7074   384, 768), dept
+00001990: 6873 3d28 332c 332c 3237 2c33 290a 2020  hs=(3,3,27,3).  
+000019a0: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+000019b0: 6261 7365 3a20 6469 6d73 3d28 3132 382c  base: dims=(128,
+000019c0: 2032 3536 2c20 3531 322c 2031 3032 3429   256, 512, 1024)
+000019d0: 2c20 6465 7074 6873 3d28 332c 332c 3237  , depths=(3,3,27
+000019e0: 2c33 290a 2020 2020 2020 2020 2020 2020  ,3).            
+000019f0: 2020 2020 2a20 6c61 7267 653a 2064 696d      * large: dim
+00001a00: 733d 2831 3932 2c20 3338 342c 2037 3638  s=(192, 384, 768
+00001a10: 2c20 3135 3336 292c 2064 6570 7468 733d  , 1536), depths=
+00001a20: 2833 2c33 2c32 372c 3329 0a20 2020 2020  (3,3,27,3).     
+00001a30: 2020 2020 2020 2020 2020 202a 2058 2d6c             * X-l
+00001a40: 6172 6765 3a20 6469 6d73 3d28 3235 362c  arge: dims=(256,
+00001a50: 2035 3132 2c20 3130 3234 2c20 3230 3438   512, 1024, 2048
+00001a60: 292c 2064 6570 7468 733d 2833 2c33 2c32  ), depths=(3,3,2
+00001a70: 372c 3329 0a0a 2020 2020 2020 2020 5265  7,3)..        Re
+00001a80: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00001a90: 2020 2041 2066 726f 7a65 6e20 6469 6374     A frozen dict
+00001aa0: 2072 6570 7265 7365 6e74 696e 6720 7765   representing we
+00001ab0: 6967 6874 7320 6f66 2074 6865 2063 7572  ights of the cur
+00001ac0: 7265 6e74 206d 6f64 756c 650a 2020 2020  rent module.    
+00001ad0: 2020 2020 7201 0000 00e9 4000 0000 7240      r.....@...r@
+00001ae0: 0000 0072 6f00 0000 5a09 636f 6e76 6e65  ...ro...Z.convne
+00001af0: 7874 5f5a 045f 3232 6b29 08da 0469 6e69  xt_Z._22k)...ini
+00001b00: 7472 2900 0000 da06 7261 6e64 6f6d da07  tr).....random..
+00001b10: 5052 4e47 4b65 7972 1a00 0000 da05 7a65  PRNGKeyr......ze
+00001b20: 726f 7372 7500 0000 da16 5f69 6d61 6765  rosru....._image
+00001b30: 6e65 745f 7765 6967 6874 735f 7572 6c73  net_weights_urls
+00001b40: 2904 722d 0000 0072 7600 0000 5a0b 696e  ).r-...rv...Z.in
+00001b50: 6974 5f70 6172 616d 7372 6f00 0000 7220  it_paramsro...r 
+00001b60: 0000 0072 2000 0000 7221 0000 00da 1467  ...r ...r!.....g
+00001b70: 6574 5f69 6d61 6765 6e65 745f 7765 6967  et_imagenet_weig
+00001b80: 6874 73c0 0000 0073 0e00 0000 0011 2001  hts....s...... .
+00001b90: 0801 0401 0201 0efe 0405 7a1d 436f 6e76  ..........z.Conv
+00001ba0: 4e65 5874 2e67 6574 5f69 6d61 6765 6e65  NeXt.get_imagene
+00001bb0: 745f 7765 6967 6874 7329 1a72 3200 0000  t_weights).r2...
+00001bc0: 7233 0000 0072 3400 0000 7235 0000 0072  r3...r4...r5...r
+00001bd0: 3f00 0000 7236 0000 0072 3700 0000 7242  ?...r6...r7...rB
+00001be0: 0000 0072 0300 0000 7246 0000 0072 4700  ...r....rF...rG.
+00001bf0: 0000 7238 0000 0072 0b00 0000 7248 0000  ..r8...r....rH..
+00001c00: 0072 2500 0000 7239 0000 0072 3a00 0000  .r%...r9...r:...
+00001c10: 723b 0000 0072 3c00 0000 da05 5475 706c  r;...r<.....Tupl
+00001c20: 65da 0844 6174 6144 6963 7472 3100 0000  e..DataDictr1...
+00001c30: 7275 0000 0072 4b00 0000 da06 5061 7261  ru...rK.....Para
+00001c40: 6d73 727d 0000 0072 2000 0000 7220 0000  msr}...r ...r ..
+00001c50: 0072 2000 0000 7221 0000 0072 3e00 0000  .r ...r!...r>...
+00001c60: 4600 0000 7320 0000 000a 0104 0d0c 0110  F...s ..........
+00001c70: 0110 010c 010c 010c 0204 0202 ff04 0102  ................
+00001c80: 0006 010a fe0e 2908 3b72 3e00 0000 2911  ......).;r>...).
+00001c90: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
+00001ca0: 0000 7204 0000 00da 0a66 6c61 782e 6c69  ..r......flax.li
+00001cb0: 6e65 6eda 056c 696e 656e 7225 0000 0072  nen..linenr%...r
+00001cc0: 2900 0000 da09 6a61 782e 6e75 6d70 79da  ).....jax.numpy.
+00001cd0: 056e 756d 7079 721a 0000 00da 0b6c 6163  .numpyr......lac
+00001ce0: 7373 2e74 7970 6573 da06 636f 6d6d 6f6e  ss.types..common
+00001cf0: da06 4d6f 6475 6c65 7207 0000 0072 7c00  ..Moduler....r|.
+00001d00: 0000 723e 0000 0072 2000 0000 7220 0000  ..r>...r ...r ..
+00001d10: 0072 2000 0000 7221 0000 00da 083c 6d6f  .r ...r!.....<mo
+00001d20: 6475 6c65 3e01 0000 0073 2200 0000 1402  dule>....s".....
+00001d30: 0c01 0801 0c02 0802 0807 122a 0201 0201  ...........*....
+00001d40: 0201 0201 0201 0201 0201 0201 02f7 060d  ................
```

### Comparing `lacss-0.4.1/lacss/modules/__pycache__/lacss.cpython-38.pyc` & `lacss-0.4.2/lacss/modules/__pycache__/lacss.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 19:59:28 2023 UTC, .py size: 4120 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,216 +1,192 @@
-00000000: 550d 0d0a 0000 0000 20ee 9964 1810 0000  U....... ..d....
+00000000: 550d 0d0a 0000 0000 7181 ad64 ba0d 0000  U.......q..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 6d04 5a04 0100 6400 6403 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6401 6c07 6d08 5a09 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6401 6c0a 5a0a 6400 6401 6c0b 6d0c 5a0d  d.l.Z.d.d.l.m.Z.
-00000070: 0100 6404 6405 6c0e 5400 6406 6405 6c0f  ..d.d.l.T.d.d.l.
-00000080: 5400 6406 6407 6c10 6d11 5a11 0100 6406  T.d.d.l.m.Z...d.
-00000090: 6408 6c12 6d13 5a13 0100 6406 6409 6c14  d.l.m.Z...d.d.l.
-000000a0: 6d15 5a15 0100 6406 640a 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
-000000b0: 0100 6406 640b 6c18 6d19 5a19 0100 4700  ..d.d.l.m.Z...G.
-000000c0: 640c 640d 8400 640d 6509 6a1a 8303 5a1b  d.d...d.e.j...Z.
-000000d0: 4700 640e 640f 8400 640f 6509 6a1a 8303  G.d.d...d.e.j...
-000000e0: 5a1c 6401 5300 2910 e900 0000 004e 2902  Z.d.S.)......N).
-000000f0: da06 6173 6469 6374 da05 6669 656c 6429  ..asdict..field)
-00000100: 01da 0770 6172 7469 616c e902 0000 0029  ...partial.....)
-00000110: 01da 012a e901 0000 0029 01da 0843 6f6e  ...*.....)...Con
-00000120: 764e 6558 7429 01da 0844 6574 6563 746f  vNeXt)...Detecto
-00000130: 7229 01da 034c 504e 2901 da06 5265 734e  r)...LPN)...ResN
-00000140: 6574 2901 da09 5365 676d 656e 746f 7263  et)...Segmentorc
-00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000160: 0700 0000 4000 0000 737a 0000 0065 005a  ....@...sz...e.Z
-00000170: 0164 005a 0255 0065 0383 005a 0465 056a  .d.Z.U.e...Z.e.j
-00000180: 0665 0764 013c 0065 0883 005a 0965 056a  .e.d.<.e...Z.e.j
-00000190: 0665 0764 023c 0065 0a83 005a 0b65 056a  .e.d.<.e...Z.e.j
-000001a0: 0665 0764 033c 0065 0c83 005a 0d65 056a  .e.d.<.e...Z.e.j
-000001b0: 0665 0764 043c 0065 0e64 0564 0684 0083  .e.d.<.e.d.d....
-000001c0: 015a 0f64 0c64 0764 089c 0165 106a 1165  .Z.d.d.d...e.j.e
-000001d0: 106a 1165 1265 1364 099c 0464 0a64 0b84  .j.e.e.d...d.d..
-000001e0: 075a 1464 0753 0029 0dda 054c 6163 7373  .Z.d.S.)...Lacss
-000001f0: da08 6261 636b 626f 6e65 da03 6c70 6eda  ..backbone..lpn.
-00000200: 0864 6574 6563 746f 72da 0973 6567 6d65  .detector..segme
-00000210: 6e74 6f72 6302 0000 0000 0000 0000 0000  ntorc...........
-00000220: 0003 0000 0004 0000 0043 0000 0073 7600  .........C...sv.
-00000230: 0000 6900 7d02 6401 7c01 6b06 721e 7400  ..i.}.d.|.k.r.t.
-00000240: 6600 7c01 6401 1900 8e01 7c02 6401 3c00  f.|.d.....|.d.<.
-00000250: 6402 7c01 6b06 7238 7401 6600 7c01 6402  d.|.k.r8t.f.|.d.
-00000260: 1900 8e01 7c02 6402 3c00 6403 7c01 6b06  ....|.d.<.d.|.k.
-00000270: 7252 7402 6600 7c01 6403 1900 8e01 7c02  rRt.f.|.d.....|.
-00000280: 6403 3c00 6404 7c01 6b06 726c 7403 6600  d.<.d.|.k.rlt.f.
-00000290: 7c01 6404 1900 8e01 7c02 6404 3c00 7c00  |.d.....|.d.<.|.
-000002a0: 6600 7c02 8e01 5300 2905 4e72 0e00 0000  f.|...S.).Nr....
-000002b0: 720f 0000 0072 1000 0000 7211 0000 0029  r....r....r....)
-000002c0: 0472 0800 0000 720a 0000 0072 0900 0000  .r....r....r....
-000002d0: 720c 0000 0029 03da 0363 6c73 da06 636f  r....)...cls..co
-000002e0: 6e66 6967 da0b 636f 6e66 6967 5f64 6963  nfig..config_dic
-000002f0: 74a9 0072 1500 0000 fa36 2f68 6f6d 652f  t..r.....6/home/
-00000300: 4643 414d 2f6a 7975 2f70 726f 6a5f 6c61  FCAM/jyu/proj_la
-00000310: 6373 732f 6c61 6373 732f 6c61 6373 732f  css/lacss/lacss/
-00000320: 6d6f 6475 6c65 732f 6c61 6373 732e 7079  modules/lacss.py
-00000330: da0b 6672 6f6d 5f63 6f6e 6669 6718 0000  ..from_config...
-00000340: 0073 1400 0000 0002 0401 0801 1201 0801  .s..............
-00000350: 1201 0801 1201 0801 1202 7a11 4c61 6373  ..........z.Lacs
-00000360: 732e 6672 6f6d 5f63 6f6e 6669 674e a901  s.from_configN..
-00000370: da08 7472 6169 6e69 6e67 2904 da05 696d  ..training)...im
-00000380: 6167 65da 0c67 745f 6c6f 6361 7469 6f6e  age..gt_location
-00000390: 7372 1900 0000 da06 7265 7475 726e 6303  sr......returnc.
-000003a0: 0000 0000 0000 0001 0000 000f 0000 0008  ................
-000003b0: 0000 0043 0000 0073 6e01 0000 7c01 6a00  ...C...sn...|.j.
-000003c0: 5c03 7d04 7d05 7d06 7c06 6401 6b02 7226  \.}.}.}.|.d.k.r&
-000003d0: 7401 6a02 7c01 6402 6403 6404 8d03 7d01  t.j.|.d.d.d...}.
-000003e0: 6e2c 7c06 6405 6b02 7252 7401 6a03 7c01  n,|.d.k.rRt.j.|.
-000003f0: 7401 a004 7c01 6406 6407 6401 8502 6602  t...|.d.d.d...f.
-00000400: 1900 a101 6702 6403 6404 8d02 7d01 7c01  ....g.d.d...}.|.
-00000410: 6a00 6403 1900 6402 6b02 7364 7405 8201  j.d...d.k.sdt...
-00000420: 7c04 6401 1800 6408 1a00 6401 1700 6408  |.d...d...d...d.
-00000430: 1400 7d07 7c05 6401 1800 6408 1a00 6401  ..}.|.d...d...d.
-00000440: 1700 6408 1400 7d08 7401 a006 7c01 6409  ..d...}.t...|.d.
-00000450: 7c07 7c04 1800 6702 6409 7c08 7c05 1800  |.|...g.d.|.|...
-00000460: 6702 6409 6409 6702 6703 a102 7d01 7c00  g.d.d.g.g...}.|.
-00000470: 6a07 7c01 7c03 640a 8d02 5c02 7d09 7d0a  j.|.|.d...\.}.}.
-00000480: 7408 7c09 7c0a 640b 8d02 7d0b 7c02 6407  t.|.|.d...}.|.d.
-00000490: 6b09 72ea 7c02 7401 a009 7c07 7c08 6702  k.r.|.t...|.|.g.
-000004a0: a101 1b00 6e02 6407 7d0c 7c0b a00a 7c00  ....n.d.}.|...|.
-000004b0: 6a0b 7c0a 7c0c 640c 8d02 a101 0100 7c02  j.|.|.d.......|.
-000004c0: 6407 6b09 9001 7312 7c03 9001 736a 7c0b  d.k...s.|...sj|.
-000004d0: a00a 7c00 6a0c 7c0b 640d 1900 7c0b 640e  ..|.j.|.d...|.d.
-000004e0: 1900 7c02 7c03 640f 8d04 a101 0100 7c0b  ..|.|.d.......|.
-000004f0: 7c03 9001 723e 6410 6e02 6411 1900 7d0d  |...r>d.n.d...}.
-00000500: 7c0d 7401 a009 7c07 7c08 6702 a101 1b00  |.t...|.|.g.....
-00000510: 7d0e 7c0b a00a 7c00 6a0d 7c0a 7c0e 6412  }.|...|.j.|.|.d.
-00000520: 8d02 a101 0100 7c0b 5300 2913 7aa6 0a20  ......|.S.).z.. 
-00000530: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00000540: 2020 2020 2020 2020 2069 6d61 6765 3a20           image: 
-00000550: 5b48 2c20 572c 2043 5d0a 2020 2020 2020  [H, W, C].      
-00000560: 2020 2020 2020 6774 5f6c 6f63 6174 696f        gt_locatio
-00000570: 6e73 3a20 5b4d 2c20 325d 2069 6620 7472  ns: [M, 2] if tr
-00000580: 6169 6e69 6e67 2c20 6f74 6865 7277 6973  aining, otherwis
-00000590: 6520 4e6f 6e65 0a20 2020 2020 2020 2052  e None.        R
-000005a0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-000005b0: 2020 2020 6120 6469 6374 206f 6620 6d6f      a dict of mo
-000005c0: 6465 6c20 6f75 7470 7574 730a 2020 2020  del outputs.    
-000005d0: 2020 2020 7207 0000 00e9 0300 0000 e9ff      r...........
-000005e0: ffff ff29 01da 0461 7869 7372 0500 0000  ...)...axisr....
-000005f0: 2e4e e920 0000 0072 0100 0000 7218 0000  .N. ...r....r...
-00000600: 0029 02da 1065 6e63 6f64 6572 5f66 6561  .)...encoder_fea
-00000610: 7475 7265 735a 1064 6563 6f64 6572 5f66  turesZ.decoder_f
-00000620: 6561 7475 7265 7329 02da 0669 6e70 7574  eatures)...input
-00000630: 73da 1373 6361 6c65 645f 6774 5f6c 6f63  s..scaled_gt_loc
-00000640: 6174 696f 6e73 da0a 6c70 6e5f 7363 6f72  ations..lpn_scor
-00000650: 6573 da0f 6c70 6e5f 7265 6772 6573 7369  es..lpn_regressi
-00000660: 6f6e 7329 04da 0673 636f 7265 73da 0b72  ons)...scores..r
-00000670: 6567 7265 7373 696f 6e73 721b 0000 0072  egressionsr....r
-00000680: 1900 0000 da12 7472 6169 6e69 6e67 5f6c  ......training_l
-00000690: 6f63 6174 696f 6e73 da0e 7072 6564 5f6c  ocations..pred_l
-000006a0: 6f63 6174 696f 6e73 2902 da08 6665 6174  ocations)...feat
-000006b0: 7572 6573 da09 6c6f 6361 7469 6f6e 7329  ures..locations)
-000006c0: 0eda 0573 6861 7065 da03 6a6e 70da 0672  ...shape..jnp..r
-000006d0: 6570 6561 74da 0b63 6f6e 6361 7465 6e61  epeat..concatena
-000006e0: 7465 da0a 7a65 726f 735f 6c69 6b65 da0e  te..zeros_like..
-000006f0: 4173 7365 7274 696f 6e45 7272 6f72 da03  AssertionError..
-00000700: 7061 6472 0e00 0000 da04 6469 6374 da05  padr......dict..
-00000710: 6172 7261 79da 0675 7064 6174 6572 0f00  array..updater..
-00000720: 0000 7210 0000 0072 1100 0000 290f da04  ..r....r....)...
-00000730: 7365 6c66 721a 0000 0072 1b00 0000 7219  selfr....r....r.
-00000740: 0000 005a 0b6f 7269 675f 6865 6967 6874  ...Z.orig_height
-00000750: 5a0a 6f72 6967 5f77 6964 7468 da02 6368  Z.orig_width..ch
-00000760: da06 6865 6967 6874 da05 7769 6474 6872  ..height..widthr
-00000770: 2100 0000 722a 0000 005a 0c6d 6f64 656c  !...r*...Z.model
-00000780: 5f6f 7574 7075 7472 2300 0000 722b 0000  _outputr#...r+..
-00000790: 005a 0b73 6361 6c65 645f 6c6f 6373 7215  .Z.scaled_locsr.
-000007a0: 0000 0072 1500 0000 7216 0000 00da 085f  ...r....r......_
-000007b0: 5f63 616c 6c5f 5f26 0000 0073 5e00 0000  _call__&...s^...
-000007c0: 000e 0c01 0801 1201 0801 2402 1203 1401  ..........$.....
-000007d0: 1401 0401 0200 1cff 0405 1201 0201 0201  ................
-000007e0: 02fe 0608 06ff 1402 02fd 0205 0401 0401  ................
-000007f0: 0201 02fe 04ff 0407 1002 0401 0401 0601  ................
-00000800: 0601 0201 02fc 04ff 040a 0201 0cff 0403  ................
-00000810: 1201 0401 0401 0201 02fe 04ff 0407 7a0e  ..............z.
-00000820: 4c61 6373 732e 5f5f 6361 6c6c 5f5f 2901  Lacss.__call__).
-00000830: 4e29 15da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00000840: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000850: 6c6e 616d 655f 5f72 0800 0000 720e 0000  lname__r....r...
-00000860: 00da 026e 6eda 064d 6f64 756c 65da 0f5f  ...nn..Module.._
-00000870: 5f61 6e6e 6f74 6174 696f 6e73 5f5f 720a  _annotations__r.
-00000880: 0000 0072 0f00 0000 7209 0000 0072 1000  ...r....r....r..
-00000890: 0000 720c 0000 0072 1100 0000 da0b 636c  ..r....r......cl
-000008a0: 6173 736d 6574 686f 6472 1700 0000 722d  assmethodr....r-
-000008b0: 0000 00da 076e 6461 7272 6179 da04 626f  .....ndarray..bo
-000008c0: 6f6c 7233 0000 0072 3a00 0000 7215 0000  olr3...r:...r...
-000008d0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-000008e0: 720d 0000 0012 0000 0073 1e00 0000 0a01  r........s......
-000008f0: 1001 1001 1001 1002 0201 0a10 00fd 0205  ................
-00000900: 02fb 0402 0401 0402 0201 02fa 720d 0000  ............r...
-00000910: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000920: 0000 0400 0000 4000 0000 735c 0000 0065  ......@...s\...e
-00000930: 005a 0164 005a 0255 0065 0365 0464 018d  .Z.d.Z.U.e.e.d..
-00000940: 015a 0565 0465 0664 023c 0064 035a 0765  .Z.e.e.d.<.d.Z.e
-00000950: 086a 0965 0419 0065 0664 043c 0064 035a  .j.e...e.d.<.d.Z
-00000960: 0a65 086a 0965 0419 0065 0664 053c 0064  .e.j.e...e.d.<.d
-00000970: 0664 0784 005a 0b64 0c64 0864 099c 0164  .d...Z.d.d.d...d
-00000980: 0a64 0b84 035a 0c64 0353 0029 0dda 0f4c  .d...Z.d.S.)...L
-00000990: 6163 7373 5769 7468 4865 6c70 6572 2901  acssWithHelper).
-000009a0: da0f 6465 6661 756c 745f 6661 6374 6f72  ..default_factor
-000009b0: 79da 0363 6667 4eda 0c61 7578 5f65 6467  y..cfgN..aux_edg
-000009c0: 655f 6366 67da 0a61 7578 5f66 675f 6366  e_cfg..aux_fg_cf
-000009d0: 6763 0100 0000 0000 0000 0000 0000 0100  gc..............
-000009e0: 0000 0300 0000 4300 0000 7342 0000 0074  ......C...sB...t
-000009f0: 00a0 017c 006a 02a1 017c 005f 037c 006a  ...|.j...|._.|.j
-00000a00: 0464 006b 0972 2674 0566 007c 006a 048e  .d.k.r&t.f.|.j..
-00000a10: 017c 005f 067c 006a 0764 006b 0972 3e74  .|._.|.j.d.k.r>t
-00000a20: 0866 007c 006a 078e 017c 005f 0964 0053  .f.|.j...|._.d.S
-00000a30: 0029 014e 290a 720d 0000 0072 1700 0000  .).N).r....r....
-00000a40: 7246 0000 00da 065f 6c61 6373 7372 4700  rF....._lacssrG.
-00000a50: 0000 da0f 4175 7849 6e73 7461 6e63 6545  ....AuxInstanceE
-00000a60: 6467 65da 105f 6175 785f 6564 6765 5f6d  dge.._aux_edge_m
-00000a70: 6f64 756c 6572 4800 0000 da0d 4175 7846  odulerH.....AuxF
-00000a80: 6f72 6567 726f 756e 64da 0e5f 6175 785f  oreground.._aux_
-00000a90: 6667 5f6d 6f64 756c 6529 0172 3600 0000  fg_module).r6...
-00000aa0: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
-00000ab0: 0573 6574 7570 7600 0000 730a 0000 0000  .setupv...s.....
-00000ac0: 010e 010a 010e 010a 017a 154c 6163 7373  .........z.Lacss
-00000ad0: 5769 7468 4865 6c70 6572 2e73 6574 7570  WithHelper.setup
-00000ae0: 4672 1800 0000 6304 0000 0000 0000 0001  Fr....c.........
-00000af0: 0000 0006 0000 0006 0000 0043 0000 0073  ...........C...s
-00000b00: 5000 0000 7c00 6a00 7c01 7c02 7c04 6401  P...|.j.|.|.|.d.
-00000b10: 8d03 7d05 7c00 6a01 6400 6b09 722e 7c05  ..}.|.j.d.k.r.|.
-00000b20: a002 7c00 6a03 7c01 7c03 6402 8d02 a101  ..|.j.|.|.d.....
-00000b30: 0100 7c00 6a04 6400 6b09 724c 7c05 a002  ..|.j.d.k.rL|...
-00000b40: 7c00 6a05 7c01 7c03 6402 8d02 a101 0100  |.j.|.|.d.......
-00000b50: 7c05 5300 2903 4e72 1800 0000 2901 da08  |.S.).Nr....)...
-00000b60: 6361 7465 676f 7279 2906 7249 0000 0072  category).rI...r
-00000b70: 4700 0000 7235 0000 0072 4b00 0000 7248  G...r5...rK...rH
-00000b80: 0000 0072 4d00 0000 2906 7236 0000 0072  ...rM...).r6...r
-00000b90: 1a00 0000 721b 0000 0072 4f00 0000 7219  ....r....rO...r.
-00000ba0: 0000 00da 0570 7265 6473 7215 0000 0072  .....predsr....r
-00000bb0: 1500 0000 7216 0000 0072 3a00 0000 7d00  ....r....r:...}.
-00000bc0: 0000 7310 0000 0000 0210 020a 0214 020a  ..s.............
-00000bd0: 0204 010c ff04 047a 184c 6163 7373 5769  .......z.LacssWi
-00000be0: 7468 4865 6c70 6572 2e5f 5f63 616c 6c5f  thHelper.__call_
-00000bf0: 5f29 024e 4e29 0d72 3b00 0000 723c 0000  _).NN).r;...r<..
-00000c00: 0072 3d00 0000 7203 0000 0072 3300 0000  .r=...r....r3...
-00000c10: 7246 0000 0072 4000 0000 7247 0000 00da  rF...r@...rG....
-00000c20: 0274 70da 084f 7074 696f 6e61 6c72 4800  .tp..OptionalrH.
-00000c30: 0000 724e 0000 0072 3a00 0000 7215 0000  ..rN...r:...r...
-00000c40: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
-00000c50: 7244 0000 0071 0000 0073 0a00 0000 0a01  rD...q...s......
-00000c60: 1201 1201 1202 0807 7244 0000 0029 1dda  ........rD...)..
-00000c70: 0674 7970 696e 6772 5100 0000 da0b 6461  .typingrQ.....da
-00000c80: 7461 636c 6173 7365 7372 0200 0000 7203  taclassesr....r.
-00000c90: 0000 00da 0966 756e 6374 6f6f 6c73 7204  .....functoolsr.
-00000ca0: 0000 00da 0a66 6c61 782e 6c69 6e65 6eda  .....flax.linen.
-00000cb0: 056c 696e 656e 723e 0000 00da 036a 6178  .linenr>.....jax
-00000cc0: da09 6a61 782e 6e75 6d70 79da 056e 756d  ..jax.numpy..num
-00000cd0: 7079 722d 0000 00da 036f 7073 da09 6175  pyr-.....ops..au
-00000ce0: 7869 6c69 6172 79da 0863 6f6e 766e 6578  xiliary..convnex
-00000cf0: 7472 0800 0000 7210 0000 0072 0900 0000  tr....r....r....
-00000d00: 720f 0000 0072 0a00 0000 da06 7265 736e  r....r......resn
-00000d10: 6574 720b 0000 0072 1100 0000 720c 0000  etr....r....r...
-00000d20: 0072 3f00 0000 720d 0000 0072 4400 0000  .r?...r....rD...
-00000d30: 7215 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-00000d40: 1600 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00000d50: 0000 731c 0000 0008 0110 010c 020c 0108  ..s.............
-00000d60: 010c 0208 0108 010c 010c 010c 010c 010c  ................
-00000d70: 0312 5f                                  .._
+00000020: 0004 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
+00000040: 6402 6c03 6d04 5a05 0100 6400 6402 6c06  d.l.m.Z...d.d.l.
+00000050: 6d07 5a08 0100 6400 6403 6c09 5400 6400  m.Z...d.d.l.T.d.
+00000060: 6404 6c0a 6d0b 5a0b 0100 6405 6406 6c0c  d.l.m.Z...d.d.l.
+00000070: 6d0d 5a0d 0100 6405 6407 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
+00000080: 0100 6405 6408 6c10 6d11 5a11 0100 6405  ..d.d.l.m.Z...d.
+00000090: 6409 6c12 6d13 5a13 0100 4700 640a 640b  d.l.m.Z...G.d.d.
+000000a0: 8400 640b 6505 6a14 8303 5a15 6402 5300  ..d.e.j...Z.d.S.
+000000b0: 290c e900 0000 0029 02da 0661 7364 6963  )......)...asdic
+000000c0: 74da 0566 6965 6c64 4e29 01da 012a a901  t..fieldN)...*..
+000000d0: da13 6461 7461 636c 6173 735f 6672 6f6d  ..dataclass_from
+000000e0: 5f64 6963 74e9 0100 0000 2901 da08 436f  _dict.....)...Co
+000000f0: 6e76 4e65 5874 2901 da08 4465 7465 6374  nvNeXt)...Detect
+00000100: 6f72 2901 da03 4c50 4e29 01da 0953 6567  or)...LPN)...Seg
+00000110: 6d65 6e74 6f72 6300 0000 0000 0000 0000  mentorc.........
+00000120: 0000 0000 0000 0007 0000 0040 0000 0073  ...........@...s
+00000130: 9a00 0000 6500 5a01 6400 5a02 5500 6401  ....e.Z.d.Z.U.d.
+00000140: 5a03 6504 6505 6402 8d01 5a06 6505 6507  Z.e.e.d...Z.e.e.
+00000150: 6403 3c00 6504 6508 6402 8d01 5a09 6508  d.<.e.e.d...Z.e.
+00000160: 6507 6404 3c00 6504 650a 6402 8d01 5a0b  e.d.<.e.e.d...Z.
+00000170: 650a 6507 6405 3c00 6504 650c 6402 8d01  e.e.d.<.e.e.d...
+00000180: 5a0d 650c 6507 6406 3c00 650e 650f 6407  Z.e.e.d.<.e.e.d.
+00000190: 9c01 6408 6409 8404 8301 5a10 650f 640a  ..d.d.....Z.e.d.
+000001a0: 9c01 640b 640c 8404 5a11 6412 640d 640e  ..d.d...Z.d.d.d.
+000001b0: 9c01 6512 6a13 6512 6a13 6514 650f 640f  ..e.j.e.j.e.e.d.
+000001c0: 9c04 6410 6411 8407 5a15 640d 5300 2913  ..d.d...Z.d.S.).
+000001d0: da05 4c61 6373 737a f74d 6169 6e20 636c  ..Lacssz.Main cl
+000001e0: 6173 7320 666f 7220 4c41 4353 5320 6d6f  ass for LACSS mo
+000001f0: 6465 6c0a 0a20 2020 2041 7474 7269 6275  del..    Attribu
+00000200: 7465 733a 0a20 2020 2020 2020 2062 6163  tes:.        bac
+00000210: 6b62 6f6e 653a 2054 6865 2043 6f6e 764e  kbone: The ConvN
+00000220: 6558 7420 6261 636b 626f 6e65 0a20 2020  eXt backbone.   
+00000230: 2020 2020 206c 706e 3a20 5468 6520 4c50       lpn: The LP
+00000240: 4e20 6865 6164 2066 6f72 2064 6574 6563  N head for detec
+00000250: 7469 6e67 2063 656c 6c20 6c6f 6361 7469  ting cell locati
+00000260: 6f6e 0a20 2020 2020 2020 2064 6574 6563  on.        detec
+00000270: 746f 723a 2041 2077 6569 6768 742d 6c65  tor: A weight-le
+00000280: 7373 206d 6f64 756c 6520 696e 7465 7270  ss module interp
+00000290: 7265 7469 6e67 206c 706e 206f 7574 7075  reting lpn outpu
+000002a0: 740a 2020 2020 2020 2020 7365 676d 656e  t.        segmen
+000002b0: 746f 723a 2054 6865 2073 6567 6d65 6e74  tor: The segment
+000002c0: 6174 696f 6e20 6865 6164 0a0a 2020 2020  ation head..    
+000002d0: 2901 da0f 6465 6661 756c 745f 6661 6374  )...default_fact
+000002e0: 6f72 79da 0862 6163 6b62 6f6e 65da 036c  ory..backbone..l
+000002f0: 706e da08 6465 7465 6374 6f72 da09 7365  pn..detector..se
+00000300: 676d 656e 746f 7229 01da 0663 6f6e 6669  gmentor)...confi
+00000310: 6763 0200 0000 0000 0000 0000 0000 0200  gc..............
+00000320: 0000 0300 0000 4300 0000 730a 0000 0074  ......C...s....t
+00000330: 007c 007c 0183 0253 0029 017a c346 6163  .|.|...S.).z.Fac
+00000340: 746f 7279 206d 6574 686f 6420 746f 2062  tory method to b
+00000350: 7569 6c64 2061 6e20 4c61 6373 7320 696e  uild an Lacss in
+00000360: 7374 616e 6365 2066 726f 6d20 6120 636f  stance from a co
+00000370: 6e66 6967 7572 6174 696f 6e20 6469 6374  nfiguration dict
+00000380: 696f 6e61 7279 0a0a 2020 2020 2020 2020  ionary..        
+00000390: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+000003a0: 2020 636f 6e66 6967 3a20 4120 636f 6e66    config: A conf
+000003b0: 6967 7572 6174 696f 6e20 6469 6374 696f  iguration dictio
+000003c0: 6e61 7279 2e0a 0a20 2020 2020 2020 2052  nary...        R
+000003d0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+000003e0: 2020 2020 416e 204c 6163 7373 2069 6e73      An Lacss ins
+000003f0: 7461 6e63 652e 0a0a 2020 2020 2020 2020  tance...        
+00000400: 7205 0000 0029 02da 0363 6c73 7212 0000  r....)...clsr...
+00000410: 00a9 0072 1400 0000 fa36 2f68 6f6d 652f  ...r.....6/home/
+00000420: 4643 414d 2f6a 7975 2f70 726f 6a5f 6c61  FCAM/jyu/proj_la
+00000430: 6373 732f 6c61 6373 732f 6c61 6373 732f  css/lacss/lacss/
+00000440: 6d6f 6475 6c65 732f 6c61 6373 732e 7079  modules/lacss.py
+00000450: da0b 6672 6f6d 5f63 6f6e 6669 671f 0000  ..from_config...
+00000460: 0073 0200 0000 000b 7a11 4c61 6373 732e  .s......z.Lacss.
+00000470: 6672 6f6d 5f63 6f6e 6669 6729 01da 0672  from_config)...r
+00000480: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
+00000490: 0000 0100 0000 0200 0000 4300 0000 7308  ..........C...s.
+000004a0: 0000 0074 007c 0083 0153 0029 017a 8043  ...t.|...S.).z.C
+000004b0: 6f6e 7665 7274 2074 6f20 6120 636f 6e66  onvert to a conf
+000004c0: 6967 7572 6174 696f 6e20 6469 6374 2e20  iguration dict. 
+000004d0: 4361 6e20 6265 2073 6572 6961 6c69 7a65  Can be serialize
+000004e0: 6420 7769 7468 206a 736f 6e0a 0a20 2020  d with json..   
+000004f0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00000500: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00000510: 3a20 6120 636f 6e66 6967 7572 6174 696f  : a configuratio
+00000520: 6e20 6469 6374 0a20 2020 2020 2020 2029  n dict.        )
+00000530: 0172 0200 0000 2901 da04 7365 6c66 7214  .r....)...selfr.
+00000540: 0000 0072 1400 0000 7215 0000 00da 0a67  ...r....r......g
+00000550: 6574 5f63 6f6e 6669 672c 0000 0073 0200  et_config,...s..
+00000560: 0000 0006 7a10 4c61 6373 732e 6765 745f  ....z.Lacss.get_
+00000570: 636f 6e66 6967 4ea9 01da 0874 7261 696e  configN....train
+00000580: 696e 6729 04da 0569 6d61 6765 da0c 6774  ing)...image..gt
+00000590: 5f6c 6f63 6174 696f 6e73 721b 0000 0072  _locationsr....r
+000005a0: 1700 0000 6303 0000 0000 0000 0001 0000  ....c...........
+000005b0: 000f 0000 0008 0000 0043 0000 0073 6e01  .........C...sn.
+000005c0: 0000 7c01 6a00 5c03 7d04 7d05 7d06 7c06  ..|.j.\.}.}.}.|.
+000005d0: 6401 6b02 7226 7401 6a02 7c01 6402 6403  d.k.r&t.j.|.d.d.
+000005e0: 6404 8d03 7d01 6e2c 7c06 6405 6b02 7252  d...}.n,|.d.k.rR
+000005f0: 7401 6a03 7c01 7401 a004 7c01 6406 6407  t.j.|.t...|.d.d.
+00000600: 6401 8502 6602 1900 a101 6702 6403 6404  d...f.....g.d.d.
+00000610: 8d02 7d01 7c01 6a00 6403 1900 6402 6b02  ..}.|.j.d...d.k.
+00000620: 7364 7405 8201 7c04 6401 1800 6408 1a00  sdt...|.d...d...
+00000630: 6401 1700 6408 1400 7d07 7c05 6401 1800  d...d...}.|.d...
+00000640: 6408 1a00 6401 1700 6408 1400 7d08 7401  d...d...d...}.t.
+00000650: a006 7c01 6409 7c07 7c04 1800 6702 6409  ..|.d.|.|...g.d.
+00000660: 7c08 7c05 1800 6702 6409 6409 6702 6703  |.|...g.d.d.g.g.
+00000670: a102 7d01 7c00 6a07 7c01 7c03 640a 8d02  ..}.|.j.|.|.d...
+00000680: 5c02 7d09 7d0a 7408 7c09 7c0a 640b 8d02  \.}.}.t.|.|.d...
+00000690: 7d0b 7c02 6407 6b09 72ea 7c02 7401 a009  }.|.d.k.r.|.t...
+000006a0: 7c07 7c08 6702 a101 1b00 6e02 6407 7d0c  |.|.g.....n.d.}.
+000006b0: 7c0b a00a 7c00 6a0b 7c0a 7c0c 640c 8d02  |...|.j.|.|.d...
+000006c0: a101 0100 7c02 6407 6b09 9001 7312 7c03  ....|.d.k...s.|.
+000006d0: 9001 736a 7c0b a00a 7c00 6a0c 7c0b 640d  ..sj|...|.j.|.d.
+000006e0: 1900 7c0b 640e 1900 7c02 7c03 640f 8d04  ..|.d...|.|.d...
+000006f0: a101 0100 7c0b 7c03 9001 723e 6410 6e02  ....|.|...r>d.n.
+00000700: 6411 1900 7d0d 7c0d 7401 a009 7c07 7c08  d...}.|.t...|.|.
+00000710: 6702 a101 1b00 7d0e 7c0b a00a 7c00 6a0d  g.....}.|...|.j.
+00000720: 7c0a 7c0e 6412 8d02 a101 0100 7c0b 5300  |.|.d.......|.S.
+00000730: 2913 7aa7 0a20 2020 2020 2020 2041 7267  ).z..        Arg
+00000740: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+00000750: 6d61 6765 3a20 5b48 2c20 572c 2043 5d0a  mage: [H, W, C].
+00000760: 2020 2020 2020 2020 2020 2020 6774 5f6c              gt_l
+00000770: 6f63 6174 696f 6e73 3a20 5b4d 2c20 325d  ocations: [M, 2]
+00000780: 2069 6620 7472 6169 6e69 6e67 2c20 6f74   if training, ot
+00000790: 6865 7277 6973 6520 4e6f 6e65 0a20 2020  herwise None.   
+000007a0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+000007b0: 2020 2020 2020 2020 2020 6120 6469 6374            a dict
+000007c0: 206f 6620 6d6f 6465 6c20 6f75 7470 7574   of model output
+000007d0: 730a 0a20 2020 2020 2020 2072 0700 0000  s..        r....
+000007e0: e903 0000 00e9 ffff ffff 2901 da04 6178  ..........)...ax
+000007f0: 6973 e902 0000 002e 4ee9 2000 0000 7201  is......N. ...r.
+00000800: 0000 0072 1a00 0000 2902 da10 656e 636f  ...r....)...enco
+00000810: 6465 725f 6665 6174 7572 6573 5a10 6465  der_featuresZ.de
+00000820: 636f 6465 725f 6665 6174 7572 6573 2902  coder_features).
+00000830: da06 696e 7075 7473 da13 7363 616c 6564  ..inputs..scaled
+00000840: 5f67 745f 6c6f 6361 7469 6f6e 73da 0a6c  _gt_locations..l
+00000850: 706e 5f73 636f 7265 735a 0f6c 706e 5f72  pn_scoresZ.lpn_r
+00000860: 6567 7265 7373 696f 6e73 2904 da06 7363  egressions)...sc
+00000870: 6f72 6573 da0b 7265 6772 6573 7369 6f6e  ores..regression
+00000880: 7372 1d00 0000 721b 0000 00da 1274 7261  sr....r......tra
+00000890: 696e 696e 675f 6c6f 6361 7469 6f6e 73da  ining_locations.
+000008a0: 0e70 7265 645f 6c6f 6361 7469 6f6e 7329  .pred_locations)
+000008b0: 02da 0866 6561 7475 7265 73da 096c 6f63  ...features..loc
+000008c0: 6174 696f 6e73 290e da05 7368 6170 65da  ations)...shape.
+000008d0: 036a 6e70 da06 7265 7065 6174 da0b 636f  .jnp..repeat..co
+000008e0: 6e63 6174 656e 6174 65da 0a7a 6572 6f73  ncatenate..zeros
+000008f0: 5f6c 696b 65da 0e41 7373 6572 7469 6f6e  _like..Assertion
+00000900: 4572 726f 72da 0370 6164 720e 0000 00da  Error..padr.....
+00000910: 0464 6963 74da 0561 7272 6179 da06 7570  .dict..array..up
+00000920: 6461 7465 720f 0000 0072 1000 0000 7211  dater....r....r.
+00000930: 0000 0029 0f72 1800 0000 721c 0000 0072  ...).r....r....r
+00000940: 1d00 0000 721b 0000 005a 0b6f 7269 675f  ....r....Z.orig_
+00000950: 6865 6967 6874 5a0a 6f72 6967 5f77 6964  heightZ.orig_wid
+00000960: 7468 da02 6368 da06 6865 6967 6874 da05  th..ch..height..
+00000970: 7769 6474 6872 2300 0000 722b 0000 005a  widthr#...r+...Z
+00000980: 0c6d 6f64 656c 5f6f 7574 7075 7472 2500  .model_outputr%.
+00000990: 0000 722c 0000 005a 0b73 6361 6c65 645f  ..r,...Z.scaled_
+000009a0: 6c6f 6373 7214 0000 0072 1400 0000 7215  locsr....r....r.
+000009b0: 0000 00da 085f 5f63 616c 6c5f 5f34 0000  .....__call__4..
+000009c0: 0073 5e00 0000 000f 0c01 0801 1201 0801  .s^.............
+000009d0: 2402 1203 1401 1401 0401 0200 1cff 0405  $...............
+000009e0: 1201 0201 0201 02fe 0608 06ff 1402 02fd  ................
+000009f0: 0205 0401 0401 0201 02fe 04ff 0407 1002  ................
+00000a00: 0401 0401 0601 0601 0201 02fc 04ff 040a  ................
+00000a10: 0201 0cff 0403 1201 0401 0401 0201 02fe  ................
+00000a20: 04ff 0407 7a0e 4c61 6373 732e 5f5f 6361  ....z.Lacss.__ca
+00000a30: 6c6c 5f5f 2901 4e29 16da 085f 5f6e 616d  ll__).N)...__nam
+00000a40: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000a50: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
+00000a60: 5f64 6f63 5f5f 7203 0000 0072 0800 0000  _doc__r....r....
+00000a70: 720e 0000 00da 0f5f 5f61 6e6e 6f74 6174  r......__annotat
+00000a80: 696f 6e73 5f5f 720a 0000 0072 0f00 0000  ions__r....r....
+00000a90: 7209 0000 0072 1000 0000 720b 0000 0072  r....r....r....r
+00000aa0: 1100 0000 da0b 636c 6173 736d 6574 686f  ......classmetho
+00000ab0: 6472 3400 0000 7216 0000 0072 1900 0000  dr4...r....r....
+00000ac0: 722e 0000 00da 076e 6461 7272 6179 da04  r......ndarray..
+00000ad0: 626f 6f6c 723a 0000 0072 1400 0000 7214  boolr:...r....r.
+00000ae0: 0000 0072 1400 0000 7215 0000 0072 0c00  ...r....r....r..
+00000af0: 0000 0f00 0000 7322 0000 000a 0104 0a12  ......s"........
+00000b00: 0112 0112 0112 0202 0110 0c0e 0b00 fd02  ................
+00000b10: 0502 fb04 0204 0104 0202 0102 fa72 0c00  .............r..
+00000b20: 0000 2916 da0b 6461 7461 636c 6173 7365  ..)...dataclasse
+00000b30: 7372 0200 0000 7203 0000 00da 0a66 6c61  sr....r......fla
+00000b40: 782e 6c69 6e65 6eda 056c 696e 656e da02  x.linen..linen..
+00000b50: 6e6e da09 6a61 782e 6e75 6d70 79da 056e  nn..jax.numpy..n
+00000b60: 756d 7079 722e 0000 005a 096c 6163 7373  umpyr....Z.lacss
+00000b70: 2e6f 7073 5a0b 6c61 6373 732e 7574 696c  .opsZ.lacss.util
+00000b80: 7372 0600 0000 da08 636f 6e76 6e65 7874  sr......convnext
+00000b90: 7208 0000 0072 1000 0000 7209 0000 0072  r....r....r....r
+00000ba0: 0f00 0000 720a 0000 0072 1100 0000 720b  ....r....r....r.
+00000bb0: 0000 00da 064d 6f64 756c 6572 0c00 0000  .....Moduler....
+00000bc0: 7214 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+00000bd0: 1500 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000be0: 0000 7312 0000 0010 020c 010c 0208 010c  ..s.............
+00000bf0: 020c 010c 010c 010c 03                   .........
```

### Comparing `lacss-0.4.1/lacss/modules/__pycache__/lpn.cpython-38.pyc` & `lacss-0.4.2/lacss/modules/__pycache__/lpn.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 3339 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,184 +1,188 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 0b0d 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 f181 ad64 d90c 0000  U..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
-00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6401 6c04 6d05 5a06 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6401 6c07 5a07 6400 6401 6c08 6d09 5a0a  d.l.Z.d.d.l.m.Z.
-00000060: 0100 6403 6404 6c0b 6d0c 5a0c 0100 6405  ..d.d.l.m.Z...d.
-00000070: 6406 6c0d 6d0e 5a0e 0100 4700 6407 6408  d.l.m.Z...G.d.d.
-00000080: 8400 6408 6506 6a0f 8303 5a10 6401 5300  ..d.e.j...Z.d.S.
-00000090: 2909 e900 0000 004e 2901 da07 7061 7274  )......N)...part
-000000a0: 6961 6ce9 0200 0000 2901 da13 6c6f 6361  ial.....)...loca
-000000b0: 7469 6f6e 735f 746f 5f6c 6162 656c 73e9  tions_to_labels.
-000000c0: 0100 0000 2901 da10 4368 616e 6e65 6c41  ....)...ChannelA
-000000d0: 7474 656e 7469 6f6e 6300 0000 0000 0000  ttentionc.......
-000000e0: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
-000000f0: 0073 9200 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
-00000100: 6401 5a03 6402 5a04 6505 6a06 6507 1900  d.Z.d.Z.e.j.e...
-00000110: 6508 6403 3c00 6404 5a09 6505 6a0a 6505  e.d.<.d.Z.e.j.e.
-00000120: 6a06 6507 1900 6505 6a06 6507 1900 6602  j.e...e.j.e...f.
-00000130: 1900 6508 6405 3c00 6406 5a0b 650c 6508  ..e.d.<.d.Z.e.e.
-00000140: 6407 3c00 650d 6a0e 650f 6a10 6505 6a0a  d.<.e.j.e.j.e.j.
-00000150: 650f 6a10 650f 6a10 650f 6a10 6603 1900  e.j.e.j.e.j.f...
-00000160: 6408 9c02 6409 640a 8404 8301 5a11 640f  d...d.d.....Z.d.
-00000170: 6512 650f 6a10 6512 640c 9c03 640d 640e  e.e.j.e.d...d.d.
-00000180: 8405 5a13 640b 5300 2910 da03 4c50 4e7a  ..Z.d.S.)...LPNz
-00000190: d40a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-000001a0: 696e 5f63 6861 6e6e 656c 733a 206e 756d  in_channels: num
-000001b0: 6265 7220 6f66 2063 6861 6e6e 656c 7320  ber of channels 
-000001c0: 696e 2069 6e70 7574 2066 6561 7475 7265  in input feature
-000001d0: 0a20 2020 2066 6561 7475 7265 5f6c 6576  .    feature_lev
-000001e0: 656c 3a20 696e 7075 7420 6665 6174 7572  el: input featur
-000001f0: 6520 6c65 7665 6c20 6465 6661 756c 7420  e level default 
-00000200: 330a 2020 2020 636f 6e76 5f6c 6179 6572  3.    conv_layer
-00000210: 733a 2063 6f6e 7620 6c61 7965 7220 7370  s: conv layer sp
-00000220: 6563 0a20 2020 2077 6974 685f 6368 616e  ec.    with_chan
-00000230: 6e65 6c5f 6174 7465 6e74 696f 6e3a 2077  nel_attention: w
-00000240: 6865 7468 6572 2069 6e63 6c75 6465 2063  hether include c
-00000250: 6861 6e6e 656c 2061 7474 656e 7469 6f6e  hannel attention
-00000260: 0a20 2020 2029 03e9 0400 0000 e903 0000  .    )..........
-00000270: 0072 0300 0000 da0e 6665 6174 7572 655f  .r......feature_
-00000280: 6c65 7665 6c73 2902 2904 e980 0100 0072  levels).)......r
-00000290: 0b00 0000 720b 0000 0072 0b00 0000 a900  ....r....r......
-000002a0: da09 636f 6e76 5f73 7065 6367 0000 0000  ..conv_specg....
-000002b0: 0000 2040 da0d 6465 7465 6374 696f 6e5f  .. @..detection_
-000002c0: 726f 6929 02da 0766 6561 7475 7265 da06  roi)...feature..
-000002d0: 7265 7475 726e 6302 0000 0000 0000 0000  returnc.........
-000002e0: 0000 0007 0000 0006 0000 0043 0000 0073  ...........C...s
-000002f0: cc00 0000 7c00 6a00 7d02 7c01 7d03 7c02  ....|.j.}.|.}.|.
-00000300: 6401 1900 4400 5d3c 7d04 7401 6a02 7c04  d...D.]<}.t.j.|.
-00000310: 6402 6403 6404 8d03 7c03 8301 7d03 7401  d.d.d...|...}.t.
-00000320: 6a03 7c04 6405 8d01 7c03 6406 1900 8301  j.|.d...|.d.....
-00000330: 6401 1900 7d03 7404 6a01 a005 7c03 a101  d...}.t.j...|...
-00000340: 7d03 7112 7c02 6407 1900 4400 5d3c 7d04  }.q.|.d...D.]<}.
-00000350: 7401 6a02 7c04 6408 6403 6404 8d03 7c03  t.j.|.d.d.d...|.
-00000360: 8301 7d03 7401 6a03 7c04 6405 8d01 7c03  ..}.t.j.|.d...|.
-00000370: 6406 1900 8301 6401 1900 7d03 7404 6a01  d.....d...}.t.j.
-00000380: a005 7c03 a101 7d03 7158 7401 a002 6407  ..|...}.qXt...d.
-00000390: 6408 a102 7c03 8301 7d05 7404 6a01 a006  d...|...}.t.j...
-000003a0: 7c05 a101 7d05 7401 a002 6409 6408 a102  |...}.t...d.d...
-000003b0: 7c03 8301 7d06 7c05 7c06 7c03 6603 5300  |...}.|.|.|.f.S.
-000003c0: 290a 4e72 0100 0000 2902 7209 0000 0072  ).Nr....).r....r
-000003d0: 0900 0000 4629 01da 0875 7365 5f62 6961  ....F)...use_bia
-000003e0: 7329 01da 0a6e 756d 5f67 726f 7570 7329  s)...num_groups)
-000003f0: 024e 2e72 0500 0000 2902 7205 0000 0072  .N.r....).r....r
-00000400: 0500 0000 7203 0000 0029 0772 0d00 0000  ....r....).r....
-00000410: da02 6e6e da04 436f 6e76 da09 4772 6f75  ..nn..Conv..Grou
-00000420: 704e 6f72 6dda 036a 6178 da04 7265 6c75  pNorm..jax..relu
-00000430: da07 7369 676d 6f69 6429 07da 0473 656c  ..sigmoid)...sel
-00000440: 6672 0f00 0000 720d 0000 00da 0178 5a04  fr....r......xZ.
-00000450: 6e5f 6368 5a0a 7363 6f72 6573 5f6f 7574  n_chZ.scores_out
-00000460: 5a0e 7265 6772 6573 7369 6f6e 5f6f 7574  Z.regression_out
-00000470: 720c 0000 0072 0c00 0000 fa34 2f68 6f6d  r....r.....4/hom
-00000480: 652f 4643 414d 2f6a 7975 2f70 726f 6a5f  e/FCAM/jyu/proj_
-00000490: 6c61 6373 732f 6c61 6373 732f 6c61 6373  lacss/lacss/lacs
-000004a0: 732f 6d6f 6475 6c65 732f 6c70 6e2e 7079  s/modules/lpn.py
-000004b0: da10 5f70 726f 6365 7373 5f66 6561 7475  .._process_featu
-000004c0: 7265 1b00 0000 731c 0000 0000 0406 0204  re....s.........
-000004d0: 020c 0114 0118 010e 020c 0114 0118 010e  ................
-000004e0: 0210 010c 0210 027a 144c 504e 2e5f 7072  .......z.LPN._pr
-000004f0: 6f63 6573 735f 6665 6174 7572 654e 2903  ocess_featureN).
-00000500: da06 696e 7075 7473 da13 7363 616c 6564  ..inputs..scaled
-00000510: 5f67 745f 6c6f 6361 7469 6f6e 7372 1000  _gt_locationsr..
-00000520: 0000 6303 0000 0000 0000 0000 0000 0011  ..c.............
-00000530: 0000 0007 0000 0043 0000 0073 ec00 0000  .......C...s....
-00000540: 7400 8300 7d03 7400 8300 7d04 7400 8300  t...}.t...}.t...
-00000550: 7d05 7c00 6a01 4400 5d44 7d06 7c01 7402  }.|.j.D.]D}.|.t.
-00000560: 7c06 8301 1900 7d07 7c00 a003 7c07 a101  |.....}.|...|...
-00000570: 5c03 7d08 7d09 7d0a 7c08 7c03 7402 7c06  \.}.}.}.|.|.t.|.
-00000580: 8301 3c00 7c09 7c04 7402 7c06 8301 3c00  ..<.|.|.t.|...<.
-00000590: 7c0a 7c05 7402 7c06 8301 3c00 7118 7400  |.|.t.|...<.q.t.
-000005a0: 7c05 7c03 7c04 6401 8d03 7d0b 7c02 6402  |.|.|.d...}.|.d.
-000005b0: 6b09 72e8 7400 8300 7d0c 7400 8300 7d0d  k.r.t...}.t...}.
-000005c0: 7c00 6a01 4400 5d4e 7d06 7c01 7402 7c06  |.j.D.]N}.|.t.|.
-000005d0: 8301 1900 6a04 6403 6404 8502 1900 7d0e  ....j.d.d.....}.
-000005e0: 7405 7c02 7c0e 7c00 6a06 6405 7c06 1300  t.|.|.|.j.d.|...
-000005f0: 1b00 6406 8d03 5c02 7d0f 7d10 7c0f 7c0c  ..d...\.}.}.|.|.
-00000600: 7402 7c06 8301 3c00 7c10 7c0d 7402 7c06  t.|...<.|.|.t.|.
-00000610: 8301 3c00 7186 7c0b a007 7400 7c0c 7c0d  ..<.q.|...t.|.|.
-00000620: 6407 8d02 a101 0100 7c0b 5300 2908 61df  d.......|.S.).a.
-00000630: 0100 000a 2020 2020 2020 2020 4172 6773  ....        Args
-00000640: 3a0a 2020 2020 2020 2020 2020 2020 696e  :.            in
-00000650: 7075 7473 3a20 6665 6174 7572 6520 6469  puts: feature di
-00000660: 6374 3a20 7b27 6c76 6c27 3a20 5b48 2c20  ct: {'lvl': [H, 
-00000670: 572c 2043 5d7d 0a20 2020 2020 2020 2020  W, C]}.         
-00000680: 2020 2073 6361 6c65 645f 6774 5f6c 6f63     scaled_gt_loc
-00000690: 6174 696f 6e73 3a20 7363 616c 6564 2030  ations: scaled 0
-000006a0: 2e2e 3120 5b4e 2c20 325d 2c20 6f6e 6c79  ..1 [N, 2], only
-000006b0: 2076 616c 6964 2069 6e20 7472 6169 6e69   valid in traini
-000006c0: 6e67 0a20 2020 2020 2020 2052 6574 7572  ng.        Retur
-000006d0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-000006e0: 6f75 7470 7574 733a 0a20 2020 2020 2020  outputs:.       
-000006f0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00000700: 2020 2020 2020 206c 706e 5f73 636f 7265         lpn_score
-00000710: 733a 2064 6963 743a 207b 276c 766c 273a  s: dict: {'lvl':
-00000720: 205b 482c 2057 2c20 315d 7d0a 2020 2020   [H, W, 1]}.    
-00000730: 2020 2020 2020 2020 2020 2020 6c70 6e5f              lpn_
-00000740: 7265 6772 6573 7369 6f6e 733a 2064 6963  regressions: dic
-00000750: 7420 7b27 6c76 6c27 3a20 5b48 2c20 572c  t {'lvl': [H, W,
-00000760: 2032 5d7d 0a20 2020 2020 2020 2020 2020   2]}.           
-00000770: 2020 2020 2067 745f 6c70 6e5f 7363 6f72       gt_lpn_scor
-00000780: 6573 3a20 6469 6374 207b 276c 766c 273a  es: dict {'lvl':
-00000790: 205b 482c 2057 2c20 315d 7d2c 206f 6e6c   [H, W, 1]}, onl
-000007a0: 7920 6966 2074 7261 696e 696e 670a 2020  y if training.  
-000007b0: 2020 2020 2020 2020 2020 2020 2020 6774                gt
-000007c0: 5f6c 706e 5f72 6567 7265 7373 696f 6e73  _lpn_regressions
-000007d0: 3a20 6469 6374 207b 276c 766c 273a 205b  : dict {'lvl': [
-000007e0: 482c 2057 2c20 325d 7d2c 206f 6e6c 7920  H, W, 2]}, only 
-000007f0: 6966 2074 7261 696e 696e 670a 2020 2020  if training.    
-00000800: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000810: 2020 2903 5a0c 6c70 6e5f 6665 6174 7572    ).Z.lpn_featur
-00000820: 6573 da0a 6c70 6e5f 7363 6f72 6573 da0f  es..lpn_scores..
-00000830: 6c70 6e5f 7265 6772 6573 7369 6f6e 734e  lpn_regressionsN
-00000840: e9fd ffff ffe9 ffff ffff 7203 0000 0029  ..........r....)
-00000850: 02da 0c74 6172 6765 745f 7368 6170 65da  ...target_shape.
-00000860: 0974 6872 6573 686f 6c64 2902 da0d 6c70  .threshold)...lp
-00000870: 6e5f 6774 5f73 636f 7265 73da 126c 706e  n_gt_scores..lpn
-00000880: 5f67 745f 7265 6772 6573 7369 6f6e 7329  _gt_regressions)
-00000890: 08da 0464 6963 7472 0a00 0000 da03 7374  ...dictr......st
-000008a0: 7272 1c00 0000 da05 7368 6170 6572 0400  rr......shaper..
-000008b0: 0000 720e 0000 00da 0675 7064 6174 6529  ..r......update)
-000008c0: 1172 1900 0000 721d 0000 0072 1e00 0000  .r....r....r....
-000008d0: 5a0a 616c 6c5f 7363 6f72 6573 5a09 616c  Z.all_scoresZ.al
-000008e0: 6c5f 7265 6772 73da 0c61 6c6c 5f66 6561  l_regrs..all_fea
-000008f0: 7475 7265 73da 036c 766c 720f 0000 00da  tures..lvlr.....
-00000900: 0573 636f 7265 5a0a 7265 6772 6573 7369  .scoreZ.regressi
-00000910: 6f6e 5a0b 6c70 6e5f 6665 6174 7572 65da  onZ.lpn_feature.
-00000920: 076f 7574 7075 7473 5a0d 616c 6c5f 6774  .outputsZ.all_gt
-00000930: 5f73 636f 7265 735a 0c61 6c6c 5f67 745f  _scoresZ.all_gt_
-00000940: 7265 6772 73da 0d66 6561 7475 7265 5f73  regrs..feature_s
-00000950: 6861 7065 da0c 7363 6f72 655f 7461 7267  hape..score_targ
-00000960: 6574 da11 7265 6772 6573 7369 6f6e 5f74  et..regression_t
-00000970: 6172 6765 7472 0c00 0000 720c 0000 0072  argetr....r....r
-00000980: 1b00 0000 da08 5f5f 6361 6c6c 5f5f 3400  ......__call__4.
-00000990: 0000 7342 0000 0000 1306 0106 0106 020a  ..sB............
-000009a0: 020c 0110 010c 010c 010e 0202 0102 0102  ................
-000009b0: 0102 fd06 0608 0206 0106 020a 0216 0202  ................
-000009c0: 0102 0102 010c fd0a 050c 010e 0204 0102  ................
-000009d0: 0102 0102 fe04 ff04 077a 0c4c 504e 2e5f  .........z.LPN._
-000009e0: 5f63 616c 6c5f 5f29 014e 2914 da08 5f5f  _call__).N)...__
-000009f0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000a00: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000a10: da07 5f5f 646f 635f 5f72 0a00 0000 da02  ..__doc__r......
-00000a20: 7470 da08 5365 7175 656e 6365 da03 696e  tp..Sequence..in
-00000a30: 74da 0f5f 5f61 6e6e 6f74 6174 696f 6e73  t..__annotations
-00000a40: 5f5f 720d 0000 00da 0554 7570 6c65 720e  __r......Tupler.
-00000a50: 0000 00da 0566 6c6f 6174 7213 0000 00da  .....floatr.....
-00000a60: 0763 6f6d 7061 6374 da03 6a6e 70da 076e  .compact..jnp..n
-00000a70: 6461 7272 6179 721c 0000 0072 2700 0000  darrayr....r'...
-00000a80: 7232 0000 0072 0c00 0000 720c 0000 0072  r2...r....r....r
-00000a90: 0c00 0000 721b 0000 0072 0700 0000 0e00  ....r....r......
-00000aa0: 0000 731c 0000 000a 0104 0812 0122 010c  ..s.........."..
-00000ab0: 0204 0204 0114 fe0e 1b00 fd02 0202 0104  ................
-00000ac0: 0102 fc72 0700 0000 2911 da06 7479 7069  ...r....)...typi
-00000ad0: 6e67 7237 0000 00da 0966 756e 6374 6f6f  ngr7.....functoo
-00000ae0: 6c73 7202 0000 00da 0a66 6c61 782e 6c69  lsr......flax.li
-00000af0: 6e65 6eda 056c 696e 656e 7213 0000 0072  nen..linenr....r
-00000b00: 1600 0000 da09 6a61 782e 6e75 6d70 79da  ......jax.numpy.
-00000b10: 056e 756d 7079 723e 0000 00da 036f 7073  .numpyr>.....ops
-00000b20: 7204 0000 00da 0663 6f6d 6d6f 6e72 0600  r......commonr..
-00000b30: 0000 da06 4d6f 6475 6c65 7207 0000 0072  ....Moduler....r
-00000b40: 0c00 0000 720c 0000 0072 0c00 0000 721b  ....r....r....r.
-00000b50: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000b60: 0073 0e00 0000 0801 0c02 0c01 0801 0c02  .s..............
-00000b70: 0c01 0c05                                ....
+00000020: 0004 0000 0040 0010 0073 6a00 0000 6400  .....@...sj...d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
+00000050: 6403 6c06 6d07 5a08 0100 6400 6403 6c09  d.l.m.Z...d.d.l.
+00000060: 5a09 6400 6403 6c0a 6d0b 5a0c 0100 6400  Z.d.d.l.m.Z...d.
+00000070: 6404 6c0d 6d0e 5a0e 0100 6400 6405 6c0f  d.l.m.Z...d.d.l.
+00000080: 5400 4700 6406 6407 8400 6407 6508 6a10  T.G.d.d...d.e.j.
+00000090: 8303 5a11 6403 5300 2908 e900 0000 0029  ..Z.d.S.)......)
+000000a0: 01da 0b61 6e6e 6f74 6174 696f 6e73 2903  ...annotations).
+000000b0: da07 4d61 7070 696e 67da 0853 6571 7565  ..Mapping..Seque
+000000c0: 6e63 65da 0554 7570 6c65 4e29 01da 136c  nce..TupleN)...l
+000000d0: 6f63 6174 696f 6e73 5f74 6f5f 6c61 6265  ocations_to_labe
+000000e0: 6c73 2901 da01 2a63 0000 0000 0000 0000  ls)...*c........
+000000f0: 0000 0000 0000 0000 0500 0000 4000 1000  ............@...
+00000100: 7360 0000 0065 005a 0164 005a 0255 0064  s`...e.Z.d.Z.U.d
+00000110: 015a 0364 025a 0464 0365 0564 043c 0064  .Z.d.Z.d.e.d.<.d
+00000120: 055a 0664 0665 0564 073c 0064 085a 0764  .Z.d.e.d.<.d.Z.d
+00000130: 0965 0564 0a3c 0065 086a 0964 0b64 0c64  .e.d.<.e.j.d.d.d
+00000140: 0d9c 0264 0e64 0f84 0483 015a 0a64 1764  ...d.d.....Z.d.d
+00000150: 1164 1264 1364 149c 0364 1564 1684 055a  .d.d.d...d.d...Z
+00000160: 0b64 1053 0029 18da 034c 504e 7acc 4c6f  .d.S.)...LPNz.Lo
+00000170: 6361 7469 6f6e 2064 6574 6563 7469 6f6e  cation detection
+00000180: 2068 6561 640a 0a20 2020 2041 7474 7269   head..    Attri
+00000190: 6275 7465 733a 0a0a 2020 2020 2020 2020  butes:..        
+000001a0: 6665 6174 7572 655f 6c65 7665 6c73 3a20  feature_levels: 
+000001b0: 496e 7075 7420 6665 6174 7572 6520 6c65  Input feature le
+000001c0: 7665 6c2c 2065 2e67 2e20 5b32 2c20 332c  vel, e.g. [2, 3,
+000001d0: 2034 5d0a 2020 2020 2020 2020 636f 6e76   4].        conv
+000001e0: 5f73 7065 633a 2043 6f6e 7620 6c61 7965  _spec: Conv laye
+000001f0: 7220 7370 6563 6966 6963 6174 696f 6e0a  r specification.
+00000200: 2020 2020 2020 2020 6465 7465 6374 696f          detectio
+00000210: 6e5f 726f 693a 2050 6172 616d 6574 6572  n_roi: Parameter
+00000220: 2066 6f72 206c 6162 656c 2073 6d6f 6f74   for label smoot
+00000230: 6869 6e67 0a0a 2020 2020 2903 e904 0000  hing..    ).....
+00000240: 00e9 0300 0000 e902 0000 007a 0d53 6571  ...........z.Seq
+00000250: 7565 6e63 655b 696e 745d da0e 6665 6174  uence[int]..feat
+00000260: 7572 655f 6c65 7665 6c73 2902 2904 e980  ure_levels).)...
+00000270: 0100 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
+00000280: 0000 a900 7a23 5475 706c 655b 5365 7175  ....z#Tuple[Sequ
+00000290: 656e 6365 5b69 6e74 5d2c 2053 6571 7565  ence[int], Seque
+000002a0: 6e63 655b 696e 745d 5dda 0963 6f6e 765f  nce[int]]..conv_
+000002b0: 7370 6563 6700 0000 0000 0020 40da 0566  specg...... @..f
+000002c0: 6c6f 6174 da0d 6465 7465 6374 696f 6e5f  loat..detection_
+000002d0: 726f 69da 0941 7272 6179 4c69 6b65 7a26  roi..ArrayLikez&
+000002e0: 5475 706c 655b 4172 7261 794c 696b 652c  Tuple[ArrayLike,
+000002f0: 2041 7272 6179 4c69 6b65 2c20 4172 7261   ArrayLike, Arra
+00000300: 794c 696b 655d 2902 da07 6665 6174 7572  yLike])...featur
+00000310: 65da 0672 6574 7572 6e63 0200 0000 0000  e..returnc......
+00000320: 0000 0000 0000 0700 0000 0600 0000 4300  ..............C.
+00000330: 1000 73cc 0000 007c 006a 007d 027c 017d  ..s....|.j.}.|.}
+00000340: 037c 0264 0119 0044 005d 3c7d 0474 016a  .|.d...D.]<}.t.j
+00000350: 027c 0464 0264 0364 048d 037c 0383 017d  .|.d.d.d...|...}
+00000360: 0374 016a 037c 0464 058d 017c 0364 0619  .t.j.|.d...|.d..
+00000370: 0083 0164 0119 007d 0374 046a 01a0 057c  ...d...}.t.j...|
+00000380: 03a1 017d 0371 127c 0264 0719 0044 005d  ...}.q.|.d...D.]
+00000390: 3c7d 0474 016a 027c 0464 0864 0364 048d  <}.t.j.|.d.d.d..
+000003a0: 037c 0383 017d 0374 016a 037c 0464 058d  .|...}.t.j.|.d..
+000003b0: 017c 0364 0619 0083 0164 0119 007d 0374  .|.d.....d...}.t
+000003c0: 046a 01a0 057c 03a1 017d 0371 5874 01a0  .j...|...}.qXt..
+000003d0: 0264 0764 08a1 027c 0383 017d 0574 046a  .d.d...|...}.t.j
+000003e0: 01a0 067c 05a1 017d 0574 01a0 0264 0964  ...|...}.t...d.d
+000003f0: 08a1 027c 0383 017d 067c 057c 067c 0366  ...|...}.|.|.|.f
+00000400: 0353 0029 0a4e 7201 0000 0029 0272 0a00  .S.).Nr....).r..
+00000410: 0000 720a 0000 0046 2901 da08 7573 655f  ..r....F)...use_
+00000420: 6269 6173 2901 da0a 6e75 6d5f 6772 6f75  bias)...num_grou
+00000430: 7073 2902 4e2e e901 0000 0029 0272 1700  ps).N......).r..
+00000440: 0000 7217 0000 0072 0b00 0000 2907 720f  ..r....r....).r.
+00000450: 0000 00da 026e 6eda 0443 6f6e 76da 0947  .....nn..Conv..G
+00000460: 726f 7570 4e6f 726d da03 6a61 78da 0472  roupNorm..jax..r
+00000470: 656c 75da 0773 6967 6d6f 6964 2907 da04  elu..sigmoid)...
+00000480: 7365 6c66 7213 0000 0072 0f00 0000 da01  selfr....r......
+00000490: 785a 046e 5f63 685a 0a73 636f 7265 735f  xZ.n_chZ.scores_
+000004a0: 6f75 745a 0e72 6567 7265 7373 696f 6e5f  outZ.regression_
+000004b0: 6f75 7472 0e00 0000 720e 0000 00fa 342f  outr....r.....4/
+000004c0: 686f 6d65 2f46 4341 4d2f 6a79 752f 7072  home/FCAM/jyu/pr
+000004d0: 6f6a 5f6c 6163 7373 2f6c 6163 7373 2f6c  oj_lacss/lacss/l
+000004e0: 6163 7373 2f6d 6f64 756c 6573 2f6c 706e  acss/modules/lpn
+000004f0: 2e70 79da 105f 7072 6f63 6573 735f 6665  .py.._process_fe
+00000500: 6174 7572 651c 0000 0073 1c00 0000 0004  ature....s......
+00000510: 0602 0402 0c01 1401 1801 0e02 0c01 1401  ................
+00000520: 1801 0e02 1001 0c02 1002 7a14 4c50 4e2e  ..........z.LPN.
+00000530: 5f70 726f 6365 7373 5f66 6561 7475 7265  _process_feature
+00000540: 4e7a 174d 6170 7069 6e67 5b73 7472 2c20  Nz.Mapping[str, 
+00000550: 4172 7261 794c 696b 655d 7a13 4f70 7469  ArrayLike]z.Opti
+00000560: 6f6e 616c 5b41 7272 6179 4c69 6b65 5dda  onal[ArrayLike].
+00000570: 0464 6963 7429 03da 0669 6e70 7574 73da  .dict)...inputs.
+00000580: 1373 6361 6c65 645f 6774 5f6c 6f63 6174  .scaled_gt_locat
+00000590: 696f 6e73 7214 0000 0063 0300 0000 0000  ionsr....c......
+000005a0: 0000 0000 0000 1100 0000 0700 0000 4300  ..............C.
+000005b0: 1000 73ec 0000 0074 0083 007d 0374 0083  ..s....t...}.t..
+000005c0: 007d 0474 0083 007d 057c 006a 0144 005d  .}.t...}.|.j.D.]
+000005d0: 447d 067c 0174 027c 0683 0119 007d 077c  D}.|.t.|.....}.|
+000005e0: 00a0 037c 07a1 015c 037d 087d 097d 0a7c  ...|...\.}.}.}.|
+000005f0: 087c 0374 027c 0683 013c 007c 097c 0474  .|.t.|...<.|.|.t
+00000600: 027c 0683 013c 007c 0a7c 0574 027c 0683  .|...<.|.|.t.|..
+00000610: 013c 0071 1874 007c 057c 037c 0464 018d  .<.q.t.|.|.|.d..
+00000620: 037d 0b7c 0264 026b 0972 e874 0083 007d  .}.|.d.k.r.t...}
+00000630: 0c74 0083 007d 0d7c 006a 0144 005d 4e7d  .t...}.|.j.D.]N}
+00000640: 067c 0174 027c 0683 0119 006a 0464 0364  .|.t.|.....j.d.d
+00000650: 0485 0219 007d 0e74 057c 027c 0e7c 006a  .....}.t.|.|.|.j
+00000660: 0664 057c 0613 001b 0064 068d 035c 027d  .d.|.....d...\.}
+00000670: 0f7d 107c 0f7c 0c74 027c 0683 013c 007c  .}.|.|.t.|...<.|
+00000680: 107c 0d74 027c 0683 013c 0071 867c 0ba0  .|.t.|...<.q.|..
+00000690: 0774 007c 0c7c 0d64 078d 02a1 0101 007c  .t.|.|.d.......|
+000006a0: 0b53 0029 0861 d801 0000 0a20 2020 2020  .S.).a.....     
+000006b0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+000006c0: 2020 2020 2069 6e70 7574 733a 2066 6561       inputs: fea
+000006d0: 7475 7265 2064 6963 743a 207b 276c 766c  ture dict: {'lvl
+000006e0: 273a 205b 482c 2057 2c20 435d 7d0a 2020  ': [H, W, C]}.  
+000006f0: 2020 2020 2020 2020 2020 7363 616c 6564            scaled
+00000700: 5f67 745f 6c6f 6361 7469 6f6e 733a 2073  _gt_locations: s
+00000710: 6361 6c65 6420 302e 2e31 205b 4e2c 2032  caled 0..1 [N, 2
+00000720: 5d2c 206f 6e6c 7920 7661 6c69 6420 696e  ], only valid in
+00000730: 2074 7261 696e 696e 670a 0a20 2020 2020   training..     
+00000740: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00000750: 2020 2020 2020 2020 4120 6469 6374 206f          A dict o
+00000760: 6620 6665 6174 7572 6573 0a0a 2020 2020  f features..    
+00000770: 2020 2020 2020 2020 2020 2020 2a20 6c70              * lp
+00000780: 6e5f 7363 6f72 6573 3a20 6469 6374 3a20  n_scores: dict: 
+00000790: 7b27 6c76 6c27 3a20 5b48 2c20 572c 2031  {'lvl': [H, W, 1
+000007a0: 5d7d 0a20 2020 2020 2020 2020 2020 2020  ]}.             
+000007b0: 2020 202a 206c 706e 5f72 6567 7265 7373     * lpn_regress
+000007c0: 696f 6e73 3a20 6469 6374 207b 276c 766c  ions: dict {'lvl
+000007d0: 273a 205b 482c 2057 2c20 325d 7d0a 2020  ': [H, W, 2]}.  
+000007e0: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+000007f0: 6774 5f6c 706e 5f73 636f 7265 733a 2064  gt_lpn_scores: d
+00000800: 6963 7420 7b27 6c76 6c27 3a20 5b48 2c20  ict {'lvl': [H, 
+00000810: 572c 2031 5d7d 2c20 6f6e 6c79 2069 6620  W, 1]}, only if 
+00000820: 7472 6169 6e69 6e67 0a20 2020 2020 2020  training.       
+00000830: 2020 2020 2020 2020 202a 2067 745f 6c70           * gt_lp
+00000840: 6e5f 7265 6772 6573 7369 6f6e 733a 2064  n_regressions: d
+00000850: 6963 7420 7b27 6c76 6c27 3a20 5b48 2c20  ict {'lvl': [H, 
+00000860: 572c 2032 5d7d 2c20 6f6e 6c79 2069 6620  W, 2]}, only if 
+00000870: 7472 6169 6e69 6e67 0a0a 2020 2020 2020  training..      
+00000880: 2020 2903 5a0c 6c70 6e5f 6665 6174 7572    ).Z.lpn_featur
+00000890: 6573 da0a 6c70 6e5f 7363 6f72 6573 da0f  es..lpn_scores..
+000008a0: 6c70 6e5f 7265 6772 6573 7369 6f6e 734e  lpn_regressionsN
+000008b0: e9fd ffff ffe9 ffff ffff 720b 0000 0029  ..........r....)
+000008c0: 02da 0c74 6172 6765 745f 7368 6170 65da  ...target_shape.
+000008d0: 0974 6872 6573 686f 6c64 2902 5a0d 6c70  .threshold).Z.lp
+000008e0: 6e5f 6774 5f73 636f 7265 735a 126c 706e  n_gt_scoresZ.lpn
+000008f0: 5f67 745f 7265 6772 6573 7369 6f6e 7329  _gt_regressions)
+00000900: 0872 2200 0000 720c 0000 00da 0373 7472  .r"...r......str
+00000910: 7221 0000 00da 0573 6861 7065 7206 0000  r!.....shaper...
+00000920: 0072 1100 0000 da06 7570 6461 7465 2911  .r......update).
+00000930: 721e 0000 0072 2300 0000 7224 0000 005a  r....r#...r$...Z
+00000940: 0a61 6c6c 5f73 636f 7265 735a 0961 6c6c  .all_scoresZ.all
+00000950: 5f72 6567 7273 da0c 616c 6c5f 6665 6174  _regrs..all_feat
+00000960: 7572 6573 da03 6c76 6c72 1300 0000 da05  ures..lvlr......
+00000970: 7363 6f72 655a 0a72 6567 7265 7373 696f  scoreZ.regressio
+00000980: 6e5a 0b6c 706e 5f66 6561 7475 7265 da07  nZ.lpn_feature..
+00000990: 6f75 7470 7574 735a 0d61 6c6c 5f67 745f  outputsZ.all_gt_
+000009a0: 7363 6f72 6573 5a0c 616c 6c5f 6774 5f72  scoresZ.all_gt_r
+000009b0: 6567 7273 da0d 6665 6174 7572 655f 7368  egrs..feature_sh
+000009c0: 6170 65da 0c73 636f 7265 5f74 6172 6765  ape..score_targe
+000009d0: 74da 1172 6567 7265 7373 696f 6e5f 7461  t..regression_ta
+000009e0: 7267 6574 720e 0000 0072 0e00 0000 7220  rgetr....r....r 
+000009f0: 0000 00da 085f 5f63 616c 6c5f 5f35 0000  .....__call__5..
+00000a00: 0073 4200 0000 0013 0601 0601 0602 0a02  .sB.............
+00000a10: 0c01 1001 0c01 0c01 0e02 0201 0201 0201  ................
+00000a20: 02fd 0606 0802 0601 0602 0a02 1602 0201  ................
+00000a30: 0201 0201 0cfd 0a05 0c01 0e02 0401 0201  ................
+00000a40: 0201 02fe 04ff 0407 7a0c 4c50 4e2e 5f5f  ........z.LPN.__
+00000a50: 6361 6c6c 5f5f 2901 4e29 0cda 085f 5f6e  call__).N)...__n
+00000a60: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000a70: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000a80: 075f 5f64 6f63 5f5f 720c 0000 00da 0f5f  .__doc__r......_
+00000a90: 5f61 6e6e 6f74 6174 696f 6e73 5f5f 720f  _annotations__r.
+00000aa0: 0000 0072 1100 0000 7218 0000 00da 0763  ...r....r......c
+00000ab0: 6f6d 7061 6374 7221 0000 0072 3500 0000  ompactr!...r5...
+00000ac0: 720e 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000ad0: 2000 0000 7208 0000 000d 0000 0073 1000   ...r........s..
+00000ae0: 0000 0a01 040a 0c01 0c01 0c02 0401 121b  ................
+00000af0: 00fd 7208 0000 0029 12da 0a5f 5f66 7574  ..r....)...__fut
+00000b00: 7572 655f 5f72 0200 0000 da06 7479 7069  ure__r......typi
+00000b10: 6e67 7203 0000 0072 0400 0000 7205 0000  ngr....r....r...
+00000b20: 00da 0a66 6c61 782e 6c69 6e65 6eda 056c  ...flax.linen..l
+00000b30: 696e 656e 7218 0000 0072 1b00 0000 da09  inenr....r......
+00000b40: 6a61 782e 6e75 6d70 79da 056e 756d 7079  jax.numpy..numpy
+00000b50: da03 6a6e 70da 096c 6163 7373 2e6f 7073  ..jnp..lacss.ops
+00000b60: 7206 0000 00da 0b6c 6163 7373 2e74 7970  r......lacss.typ
+00000b70: 6573 da06 4d6f 6475 6c65 7208 0000 0072  es..Moduler....r
+00000b80: 0e00 0000 720e 0000 0072 0e00 0000 7220  ....r....r....r 
+00000b90: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000ba0: 0073 0e00 0000 0c02 1402 0c01 0801 0c02  .s..............
+00000bb0: 0c01 0803                                ....
```

### Comparing `lacss-0.4.1/lacss/modules/__pycache__/resnet.cpython-38.pyc` & `lacss-0.4.2/lacss/modules/__pycache__/resnet.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 3771 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 bb0e 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 5a80 9c64 bb0e 0000  U.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 0100 6400 6402 6c06  m.Z.m.Z...d.d.l.
 00000050: 6d07 5a08 0100 6400 6402 6c09 5a09 6400  m.Z...d.d.l.Z.d.
 00000060: 6402 6c0a 6d0b 5a0c 0100 6403 6404 6c0d  d.l.m.Z...d.d.l.
 00000070: 5400 4700 6405 6406 8400 6406 6508 6a0e  T.G.d.d...d.e.j.
@@ -97,15 +97,15 @@
 00000600: 0029 0272 3500 0000 e918 0000 0029 0272  .).r5........).r
 00000610: 3400 0000 7214 0000 0029 0272 3500 0000  4...r....).r5...
 00000620: e91d 0000 0029 0272 3600 0000 e935 0000  .....).r6....5..
 00000630: 0029 0272 3800 0000 7214 0000 0029 0272  .).r8...r....).r
 00000640: 3500 0000 723b 0000 0029 0272 3600 0000  5...r;...).r6...
 00000650: e948 0000 0029 0272 3500 0000 e92c 0000  .H...).r5....,..
 00000660: 0029 0272 3600 0000 e957 0000 0029 07da  .).r6....W...)..
-00000670: 0235 30da 0331 3031 da03 3135 32da 0332  .50..101..152..2
+00000670: 0235 305a 0331 3031 5a03 3135 325a 0332  .50Z.101Z.152Z.2
 00000680: 3030 5a03 3237 305a 0333 3530 5a03 3432  00Z.270Z.350Z.42
 00000690: 3063 0000 0000 0000 0000 0000 0000 0000  0c..............
 000006a0: 0000 0600 0000 4000 0000 738a 0000 0065  ......@...s....e
 000006b0: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
 000006c0: 0565 0665 0765 0865 0866 0219 0019 0066  .e.e.e.e.f.....f
 000006d0: 0219 0065 0964 023c 0064 035a 0a65 0865  ...e.d.<.d.Z.e.e
 000006e0: 0964 043c 0064 055a 0b65 0865 0964 063c  .d.<.d.Z.e.e.d.<
@@ -120,20 +120,20 @@
 00000770: 5f6c 6576 656c 720e 0000 0072 3600 0000  _levelr....r6...
 00000780: da0c 6f75 745f 6368 616e 6e65 6c73 e902  ..out_channels..
 00000790: 0000 00da 0a70 6174 6368 5f73 697a 6563  .....patch_sizec
 000007a0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
 000007b0: 0200 0000 4300 0000 7320 0000 007c 006a  ....C...s ...|.j
 000007c0: 0064 016b 0372 1c7c 006a 0064 026b 0372  .d.k.r.|.j.d.k.r
 000007d0: 1c74 0164 0383 0182 0164 0053 0029 044e  .t.d.....d.S.).N
-000007e0: 724a 0000 0072 1400 0000 7a41 496e 7661  rJ...r....zAInva
+000007e0: 7247 0000 0072 1400 0000 7a41 496e 7661  rG...r....zAInva
 000007f0: 6c75 6420 7061 7463 685f 7369 7a65 207b  lud patch_size {
 00000800: 7365 6c66 2e70 6174 6368 5f73 697a 657d  self.patch_size}
 00000810: 2e20 4974 2073 686f 756c 6520 6265 2065  . It shoule be e
 00000820: 6974 6865 7220 3220 6f72 2034 2e29 0272  ither 2 or 4.).r
-00000830: 4b00 0000 da0a 5661 6c75 6545 7272 6f72  K.....ValueError
+00000830: 4800 0000 da0a 5661 6c75 6545 7272 6f72  H.....ValueError
 00000840: 2901 7224 0000 0072 2700 0000 7227 0000  ).r$...r'...r'..
 00000850: 0072 2800 0000 da0d 5f5f 706f 7374 5f69  .r(.....__post_i
 00000860: 6e69 745f 5f46 0000 0073 0800 0000 0002  nit__F...s......
 00000870: 1401 0201 02ff 7a14 5265 734e 6574 2e5f  ......z.ResNet._
 00000880: 5f70 6f73 745f 696e 6974 5f5f 4e72 1000  _post_init__Nr..
 00000890: 0000 2903 7226 0000 0072 1100 0000 7213  ..).r&...r....r.
 000008a0: 0000 0063 0200 0000 0000 0000 0100 0000  ...c............
@@ -158,67 +158,67 @@
 000009d0: 017c 0264 098d 027d 0171 fe7c 03a0 057c  .|.d...}.q.|...|
 000009e0: 01a1 0101 0071 b87c 006a 107d 0d7c 006a  .....q.|.j.}.|.j
 000009f0: 117d 0e74 127c 0e83 017c 037c 0d64 0085  .}.t.|...|.|.d..
 00000a00: 0219 0083 017d 0f64 0a64 0b84 0074 0f74  .....}.d.d...t.t
 00000a10: 0d7c 0383 0183 0144 0083 017d 1074 1374  .|.....D...}.t.t
 00000a20: 147c 107c 0383 0283 017d 0374 1374 147c  .|.|.....}.t.t.|
 00000a30: 107c 0d64 0085 0219 007c 0f83 0283 017d  .|.d.....|.....}
-00000a40: 0f7c 037c 0f66 0253 0029 0c4e 724a 0000  .|.|.f.S.).NrJ..
+00000a40: 0f7c 037c 0f66 0253 0029 0c4e 7247 0000  .|.|.f.S.).NrG..
 00000a50: 0072 3c00 0000 7218 0000 0072 3400 0000  .r<...r....r4...
-00000a60: 2902 724a 0000 0072 4a00 0000 2901 720b  ).rJ...rJ...).r.
+00000a60: 2902 7247 0000 0072 4700 0000 2901 720b  ).rG...rG...).r.
 00000a70: 0000 0072 0700 0000 2902 720d 0000 0072  ...r....).r....r
 00000a80: 0f00 0000 7210 0000 0063 0100 0000 0000  ....r....c......
 00000a90: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
 00000aa0: 0000 7314 0000 0067 007c 005d 0c7d 0174  ..s....g.|.].}.t
 00000ab0: 007c 0183 0191 0271 0453 0072 2700 0000  .|.....q.S.r'...
 00000ac0: 2901 da03 7374 7229 02da 022e 30da 016b  )...str)....0..k
 00000ad0: 7227 0000 0072 2700 0000 7228 0000 00da  r'...r'...r(....
 00000ae0: 0a3c 6c69 7374 636f 6d70 3e72 0000 0073  .<listcomp>r...s
 00000af0: 0400 0000 0600 0200 7a23 5265 734e 6574  ........z#ResNet
 00000b00: 2e5f 5f63 616c 6c5f 5f2e 3c6c 6f63 616c  .__call__.<local
 00000b10: 733e 2e3c 6c69 7374 636f 6d70 3e29 1572  s>.<listcomp>).r
-00000b20: 4b00 0000 7220 0000 0072 1c00 0000 7221  K...r ...r....r!
+00000b20: 4800 0000 7220 0000 0072 1c00 0000 7221  H...r ...r....r!
 00000b30: 0000 0072 1d00 0000 da06 6170 7065 6e64  ...r......append
-00000b40: 7247 0000 00da 0a69 7369 6e73 7461 6e63  rG.....isinstanc
-00000b50: 6572 4e00 0000 da0d 5f52 4553 4e45 545f  erN....._RESNET_
+00000b40: 7244 0000 00da 0a69 7369 6e73 7461 6e63  rD.....isinstanc
+00000b50: 6572 4b00 0000 da0d 5f52 4553 4e45 545f  erK....._RESNET_
 00000b60: 5350 4543 5372 0d00 0000 da14 7374 6f63  SPECSr......stoc
 00000b70: 6861 7374 6963 5f64 726f 705f 7261 7465  hastic_drop_rate
 00000b80: da09 656e 756d 6572 6174 65da 036c 656e  ..enumerate..len
-00000b90: 7209 0000 00da 0572 616e 6765 7248 0000  r......rangerH..
-00000ba0: 0072 4900 0000 da03 4650 4eda 0464 6963  .rI.....FPN..dic
+00000b90: 7209 0000 00da 0572 616e 6765 7245 0000  r......rangerE..
+00000ba0: 0072 4600 0000 da03 4650 4eda 0464 6963  .rF.....FPN..dic
 00000bb0: 74da 037a 6970 2911 7224 0000 0072 2600  t..zip).r$...r&.
 00000bc0: 0000 7211 0000 00da 0b65 6e63 6f64 6572  ..r......encoder
-00000bd0: 5f6f 7574 7247 0000 00da 0473 7065 6372  _outrG.....specr
-00000be0: 0d00 0000 7255 0000 00da 0169 720a 0000  ....rU.....ir...
+00000bd0: 5f6f 7574 7244 0000 00da 0473 7065 6372  _outrD.....specr
+00000be0: 0d00 0000 7252 0000 00da 0169 720a 0000  ....rR.....ir...
 00000bf0: 005a 096e 5f72 6570 6561 7473 720f 0000  .Z.n_repeatsr...
-00000c00: 00da 015f 5a05 6c5f 6d69 6e72 4900 0000  ..._Z.l_minrI...
+00000c00: 00da 015f 5a05 6c5f 6d69 6e72 4600 0000  ..._Z.l_minrF...
 00000c10: da0b 6465 636f 6465 725f 6f75 74da 046b  ..decoder_out..k
 00000c20: 6579 7372 2700 0000 7227 0000 0072 2800  eysr'...r'...r(.
 00000c30: 0000 7229 0000 004d 0000 0073 4200 0000  ..r)...M...sB...
 00000c40: 0003 0a01 1801 1801 0802 0601 1c01 1801  ................
 00000c50: 0a02 0601 0a01 0a02 0402 0601 0601 1401  ................
 00000c60: 1801 0e01 0200 02ff 0603 0e01 0c01 0200  ................
 00000c70: 02ff 0803 0c02 0601 0602 1402 1601 0e01  ................
 00000c80: 1602 7a0f 5265 734e 6574 2e5f 5f63 616c  ..z.ResNet.__cal
 00000c90: 6c5f 5f29 1772 2a00 0000 722b 0000 0072  l__).r*...r+...r
-00000ca0: 2c00 0000 7247 0000 0072 0600 0000 724e  ,...rG...r....rN
+00000ca0: 2c00 0000 7244 0000 0072 0600 0000 724b  ,...rD...r....rK
 00000cb0: 0000 0072 0400 0000 7205 0000 0072 2d00  ...r....r....r-.
-00000cc0: 0000 722e 0000 0072 0d00 0000 7248 0000  ..r....r....rH..
-00000cd0: 0072 5500 0000 7249 0000 0072 4b00 0000  .rU...rI...rK...
-00000ce0: 724d 0000 0072 1c00 0000 7230 0000 0072  rM...r....r0...r
-00000cf0: 3100 0000 7232 0000 0072 3300 0000 725a  1...r2...r3...rZ
+00000cc0: 0000 722e 0000 0072 0d00 0000 7245 0000  ..r....r....rE..
+00000cd0: 0072 5200 0000 7246 0000 0072 4800 0000  .rR...rF...rH...
+00000ce0: 724a 0000 0072 1c00 0000 7230 0000 0072  rJ...r....r0...r
+00000cf0: 3100 0000 7232 0000 0072 3300 0000 7257  1...r2...r3...rW
 00000d00: 0000 0072 2900 0000 7227 0000 0072 2700  ...r)...r'...r'.
-00000d10: 0000 7227 0000 0072 2800 0000 7246 0000  ..r'...r(...rF..
+00000d10: 0000 7227 0000 0072 2800 0000 7243 0000  ..r'...r(...rC..
 00000d20: 003e 0000 0073 1200 0000 0a01 2001 0c01  .>...s...... ...
-00000d30: 0c01 0401 0c01 0c02 0807 0401 7246 0000  ............rF..
+00000d30: 0c01 0401 0c01 0c02 0807 0401 7243 0000  ............rC..
 00000d40: 0029 12da 0674 7970 696e 6772 0200 0000  .)...typingr....
 00000d50: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
 00000d60: 0600 0000 da0a 666c 6178 2e6c 696e 656e  ......flax.linen
 00000d70: da05 6c69 6e65 6e72 1c00 0000 7220 0000  ..linenr....r ..
 00000d80: 00da 096a 6178 2e6e 756d 7079 da05 6e75  ...jax.numpy..nu
 00000d90: 6d70 7972 3100 0000 da06 636f 6d6d 6f6e  mpyr1.....common
-00000da0: da06 4d6f 6475 6c65 7209 0000 0072 5400  ..Moduler....rT.
-00000db0: 0000 7246 0000 0072 2700 0000 7227 0000  ..rF...r'...r'..
+00000da0: da06 4d6f 6475 6c65 7209 0000 0072 5100  ..Moduler....rQ.
+00000db0: 0000 7243 0000 0072 2700 0000 7227 0000  ..rC...r'...r'..
 00000dc0: 0072 2700 0000 7228 0000 00da 083c 6d6f  .r'...r(.....<mo
 00000dd0: 6475 6c65 3e01 0000 0073 1c00 0000 1c02  dule>....s......
 00000de0: 0c01 0801 0c02 0803 122a 0a01 0a01 0a01  .........*......
 00000df0: 0a01 0a01 0a01 0af9 060b                 ..........
```

### Comparing `lacss-0.4.1/lacss/modules/__pycache__/segmentor.cpython-38.pyc` & `lacss-0.4.2/lacss/modules/__pycache__/segmentor.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun 27 17:32:18 2023 UTC, .py size: 5254 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,266 +1,279 @@
-00000000: 550d 0d0a 0000 0000 221d 9b64 8614 0000  U......."..d....
+00000000: 550d 0d0a 0000 0000 e67d ad64 5415 0000  U........}.dT...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6402 6c03 6d04 5a04 0100 6400 6401 6c05  d.l.m.Z...d.d.l.
-00000050: 6d06 5a07 0100 6400 6401 6c08 5a08 6400  m.Z...d.d.l.Z.d.
-00000060: 6401 6c09 6d0a 5a0b 0100 6403 6404 6c0c  d.l.m.Z...d.d.l.
-00000070: 6d0d 5a0d 0100 6405 6406 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
-00000080: 0100 4700 6407 6408 8400 6408 6507 6a10  ..G.d.d...d.e.j.
-00000090: 8303 5a11 4700 6409 640a 8400 640a 6507  ..Z.G.d.d...d.e.
-000000a0: 6a10 8303 5a12 6401 5300 290b e900 0000  j...Z.d.S.).....
-000000b0: 004e 2901 da07 7061 7274 6961 6ce9 0200  .N)...partial...
-000000c0: 0000 2901 da0e 6761 7468 6572 5f70 6174  ..)...gather_pat
-000000d0: 6368 6573 e901 0000 0029 01da 1053 7061  ches.....)...Spa
+00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6400 6401 6c03 6d04 5a05 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6401 6c06 5a06 6400 6401 6c07 6d08 5a09  d.l.Z.d.d.l.m.Z.
+00000060: 0100 6400 6403 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
+00000070: 6404 6c0c 5400 6405 6406 6c0d 6d0e 5a0e  d.l.T.d.d.l.m.Z.
+00000080: 0100 4700 6407 6408 8400 6408 6505 6a0f  ..G.d.d...d.e.j.
+00000090: 8303 5a10 4700 6409 640a 8400 640a 6505  ..Z.G.d.d...d.e.
+000000a0: 6a0f 8303 5a11 6401 5300 290b e900 0000  j...Z.d.S.).....
+000000b0: 004e 2901 da07 7061 7274 6961 6c29 01da  .N)...partial)..
+000000c0: 0e67 6174 6865 725f 7061 7463 6865 7329  .gather_patches)
+000000d0: 01da 012a e901 0000 0029 01da 1053 7061  ...*.....)...Spa
 000000e0: 7469 616c 4174 7465 6e74 696f 6e63 0000  tialAttentionc..
-000000f0: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00000100: 0000 4000 0000 7350 0000 0065 005a 0164  ..@...sP...e.Z.d
+000000f0: 0000 0000 0000 0000 0000 0000 0000 0500  ................
+00000100: 0000 4000 0000 7358 0000 0065 005a 0164  ..@...sX...e.Z.d
 00000110: 005a 0255 0065 0365 0464 013c 0065 0365  .Z.U.e.e.d.<.e.e
-00000120: 0464 023c 0064 035a 0565 066a 0765 0365  .d.<.d.Z.e.j.e.e
-00000130: 0365 0366 0319 0065 0464 043c 0064 055a  .e.f...e.d.<.d.Z
-00000140: 0865 0365 0464 063c 0065 096a 0a64 0764  .e.e.d.<.e.j.d.d
-00000150: 0884 0083 015a 0b64 0953 0029 0ada 085f  .....Z.d.S.)..._
-00000160: 456e 636f 6465 72da 116e 5f6f 7574 7075  Encoder..n_outpu
-00000170: 745f 6665 6174 7572 6573 da10 696e 7075  t_features..inpu
-00000180: 745f 7061 7463 685f 7369 7a65 a903 e908  t_patch_size....
-00000190: 0000 0072 0b00 0000 e904 0000 00da 0d65  ...r...........e
-000001a0: 6e63 6f64 696e 675f 6469 6d73 e9ff ffff  ncoding_dims....
-000001b0: ffda 116e 5f6c 6174 656e 745f 6665 6174  ...n_latent_feat
-000001c0: 7572 6573 6303 0000 0000 0000 0000 0000  uresc...........
-000001d0: 0009 0000 0008 0000 0043 0000 0073 e000  .........C...s..
-000001e0: 0000 7400 7c01 7c02 6401 6402 8d03 5c04  ..t.|.|.d.d...\.
-000001f0: 7d03 7d04 7d04 7d04 7c03 6a01 6403 6404  }.}.}.}.|.j.d.d.
-00000200: 8d01 7d05 7c00 6a02 7d06 7c06 6405 6b04  ..}.|.j.}.|.d.k.
-00000210: 7234 7c06 6e0a 7403 a004 7c00 6a05 a101  r4|.n.t...|.j...
-00000220: 7d06 7406 a007 7c06 a101 7c05 8301 7d05  }.t...|...|...}.
-00000230: 7408 6a06 a009 7c05 a101 7d05 7406 a007  t.j...|...}.t...
-00000240: 7c06 a101 7c05 8301 7d05 7408 6a06 a009  |...|...}.t.j...
-00000250: 7c05 a101 7d05 7403 a004 7c00 6a05 a101  |...}.t...|.j...
-00000260: 7d07 6406 7c00 6a05 1700 7d08 7406 a007  }.d.|.j...}.t...
-00000270: 7c07 a101 7c05 8301 a00a 7c08 a101 7d05  |...|.....|...}.
-00000280: 7408 6a0b a00c 7c05 7c05 6a0d 6405 1900  t.j...|.|.j.d...
-00000290: 7c00 6a0e 7c00 6a0e 7c00 6a05 6407 1900  |.j.|.j.|.j.d...
-000002a0: 6604 6408 a103 7d05 7406 6a0f 7c00 6a10  f.d...}.t.j.|.j.
-000002b0: 6409 640a 640b 8d03 7c05 8301 7d05 7c05  d.d.d...|...}.|.
-000002c0: 5300 290c 4e72 0300 0000 a901 da0a 7061  S.).Nr........pa
-000002d0: 7463 685f 7369 7a65 2902 e9fe ffff ffe9  tch_size).......
-000002e0: fdff ffff a901 da04 6178 6973 7201 0000  ........axisr...
-000002f0: 0029 0172 0e00 0000 720e 0000 00da 066c  .).r....r......l
-00000300: 696e 6561 72a9 0272 0500 0000 7205 0000  inear..r....r...
-00000310: 0046 a901 da08 7573 655f 6269 6173 2911  .F....use_bias).
-00000320: 7204 0000 00da 046d 6561 6e72 0f00 0000  r......meanr....
-00000330: da04 6d61 7468 da04 7072 6f64 720d 0000  ..math..prodr...
-00000340: 00da 026e 6eda 0544 656e 7365 da03 6a61  ...nn..Dense..ja
-00000350: 78da 0472 656c 75da 0772 6573 6861 7065  x..relu..reshape
-00000360: da05 696d 6167 65da 0672 6573 697a 65da  ..image..resize.
-00000370: 0573 6861 7065 7209 0000 00da 0443 6f6e  .shaper......Con
-00000380: 7672 0800 0000 2909 da04 7365 6c66 da07  vr....)...self..
-00000390: 6665 6174 7572 65da 036c 6f63 5a0c 7061  feature..locZ.pa
-000003a0: 7463 685f 6365 6e74 6572 da01 5fda 0965  tch_center.._..e
-000003b0: 6e63 6f64 696e 6773 da03 6469 6dda 076e  ncodings..dim..n
-000003c0: 6577 5f64 696d 5a0e 656e 636f 6469 6e67  ew_dimZ.encoding
-000003d0: 5f73 6861 7065 a900 722d 0000 00fa 3a2f  _shape..r-....:/
-000003e0: 686f 6d65 2f46 4341 4d2f 6a79 752f 7072  home/FCAM/jyu/pr
-000003f0: 6f6a 5f6c 6163 7373 2f6c 6163 7373 2f6c  oj_lacss/lacss/l
-00000400: 6163 7373 2f6d 6f64 756c 6573 2f73 6567  acss/modules/seg
-00000410: 6d65 6e74 6f72 2e70 79da 085f 5f63 616c  mentor.py..__cal
-00000420: 6c5f 5f13 0000 0073 2c00 0000 0002 1601  l__....s,.......
-00000430: 0c02 0601 1801 0e01 0c01 0e01 0c02 0c01  ................
-00000440: 0a01 1401 0601 0202 0801 0401 0401 08fc  ................
-00000450: 0206 02f8 040b 1602 7a11 5f45 6e63 6f64  ........z._Encod
-00000460: 6572 2e5f 5f63 616c 6c5f 5f4e 290c da08  er.__call__N)...
-00000470: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000480: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000490: 5f5f da03 696e 74da 0f5f 5f61 6e6e 6f74  __..int..__annot
-000004a0: 6174 696f 6e73 5f5f 720d 0000 00da 0274  ations__r......t
-000004b0: 70da 0554 7570 6c65 720f 0000 0072 1d00  p..Tupler....r..
-000004c0: 0000 da07 636f 6d70 6163 7472 2f00 0000  ....compactr/...
-000004d0: 722d 0000 0072 2d00 0000 722d 0000 0072  r-...r-...r-...r
-000004e0: 2e00 0000 7207 0000 000d 0000 0073 0c00  ....r........s..
-000004f0: 0000 0a01 0801 0801 1801 0c02 0401 7207  ..............r.
-00000500: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000510: 0000 0000 0500 0000 4000 0000 7390 0000  ........@...s...
-00000520: 0065 005a 0164 005a 0255 0064 015a 0364  .e.Z.d.Z.U.d.Z.d
-00000530: 025a 0465 0565 0664 033c 0064 045a 0765  .Z.e.e.d.<.d.Z.e
-00000540: 086a 0965 086a 0a65 0519 0065 086a 0a65  .j.e.j.e...e.j.e
-00000550: 0519 0066 0219 0065 0664 053c 0064 065a  ...f...e.d.<.d.Z
-00000560: 0b65 0565 0664 073c 0064 085a 0c65 0d65  .e.e.d.<.d.Z.e.e
-00000570: 0664 093c 0064 0a5a 0e65 0d65 0664 0b3c  .d.<.d.Z.e.e.d.<
-00000580: 0064 0c5a 0f65 086a 0a65 0519 0065 0664  .d.Z.e.j.e...e.d
-00000590: 0d3c 0065 106a 1165 1265 136a 1465 1264  .<.e.j.e.e.j.e.d
-000005a0: 0e9c 0364 0f64 1084 0483 015a 1564 1153  ...d.d.....Z.d.S
-000005b0: 0029 12da 0953 6567 6d65 6e74 6f72 61cb  .)...Segmentora.
-000005c0: 0100 004c 4143 5353 2073 6567 6d65 6e74  ...LACSS segment
-000005d0: 6f72 206d 6f64 756c 652e 0a0a 2020 2020  or module...    
-000005e0: 4174 7472 6962 7574 6573 3a0a 2020 2020  Attributes:.    
-000005f0: 2020 2020 6665 6174 7572 655f 6c65 7665      feature_leve
-00000600: 6c3a 2069 6e74 0a20 2020 2020 2020 2063  l: int.        c
-00000610: 6f6e 765f 7370 6563 3a20 636f 6e76 5f62  onv_spec: conv_b
-00000620: 6c6f 636b 2064 6566 696e 6974 696f 6e2c  lock definition,
-00000630: 2065 2e67 2e20 2828 3338 342c 3338 342c   e.g. ((384,384,
-00000640: 3338 3429 2c20 2836 342c 2929 0a20 2020  384), (64,)).   
-00000650: 2020 2020 2069 6e73 7461 6e63 655f 6372       instance_cr
-00000660: 6f70 5f73 697a 653a 2043 726f 7020 7369  op_size: Crop si
-00000670: 7a65 2e20 6465 6661 756c 7420 6973 2039  ze. default is 9
-00000680: 362e 0a20 2020 2020 2020 2077 6974 685f  6..        with_
-00000690: 6174 7465 6e74 696f 6e3a 2057 6865 7468  attention: Wheth
-000006a0: 6572 2075 7365 2073 7061 7469 616c 2061  er use spatial a
-000006b0: 7474 656e 7469 6f6e 206c 6179 6572 2e20  ttention layer. 
-000006c0: 4465 6661 756c 7420 6973 2046 616c 7365  Default is False
-000006d0: 0a20 2020 2020 2020 206c 6561 726e 6564  .        learned
-000006e0: 5f65 6e63 6f64 696e 673a 2057 6865 7468  _encoding: Wheth
-000006f0: 6572 2074 6f20 7573 6520 6861 7264 2d63  er to use hard-c
-00000700: 6f64 6564 2070 6f73 6974 696f 6e20 656e  oded position en
-00000710: 636f 6469 6e67 2e20 4465 6661 756c 7420  coding. Default 
-00000720: 6973 2046 616c 7365 0a20 2020 2020 2020  is False.       
-00000730: 2065 6e63 6f64 6572 5f64 696d 733a 2044   encoder_dims: D
-00000740: 696d 206f 6620 7468 6520 706f 7369 7469  im of the positi
-00000750: 6f6e 2065 6e63 6f64 6572 2c20 6966 2075  on encoder, if u
-00000760: 7369 6e67 206c 6561 726e 6564 2065 6e63  sing learned enc
-00000770: 6f64 696e 672e 2044 6566 6175 6c74 2069  oding. Default i
-00000780: 7320 2838 2c38 2c34 290a 2020 2020 7203  s (8,8,4).    r.
-00000790: 0000 00da 0d66 6561 7475 7265 5f6c 6576  .....feature_lev
-000007a0: 656c 2902 2903 e980 0100 0072 3a00 0000  el).)......r:...
-000007b0: 723a 0000 0029 01e9 4000 0000 da09 636f  r:...)..@.....co
-000007c0: 6e76 5f73 7065 63e9 6000 0000 da12 696e  nv_spec.`.....in
-000007d0: 7374 616e 6365 5f63 726f 705f 7369 7a65  stance_crop_size
-000007e0: 46da 0d75 7365 5f61 7474 656e 7469 6f6e  F..use_attention
-000007f0: 54da 106c 6561 726e 6564 5f65 6e63 6f64  T..learned_encod
-00000800: 696e 6772 0a00 0000 da0c 656e 636f 6465  ingr......encode
-00000810: 725f 6469 6d73 2903 da08 6665 6174 7572  r_dims)...featur
-00000820: 6573 da09 6c6f 6361 7469 6f6e 73da 0672  es..locations..r
-00000830: 6574 7572 6e63 0300 0000 0000 0000 0000  eturnc..........
-00000840: 0000 1400 0000 0700 0000 4300 0000 7388  ..........C...s.
-00000850: 0200 007c 006a 007d 037c 006a 017d 0464  ...|.j.}.|.j.}.d
-00000860: 017c 0413 007d 057c 006a 027d 067c 037c  .|...}.|.j.}.|.|
-00000870: 051a 007d 077c 0174 037c 0483 0119 007d  ...}.|.t.|.....}
-00000880: 087c 0664 0219 0044 005d 3c7d 0974 046a  .|.d...D.]<}.t.j
-00000890: 057c 0964 0364 0464 058d 037c 0883 017d  .|.d.d.d...|...}
-000008a0: 0874 046a 067c 0964 068d 017c 0864 0719  .t.j.|.d...|.d..
-000008b0: 0083 0164 0219 007d 0874 076a 04a0 087c  ...d...}.t.j...|
-000008c0: 08a1 017d 0871 367c 0664 0819 0064 0219  ...}.q6|.d...d..
-000008d0: 007d 0974 046a 057c 0964 0364 0464 058d  .}.t.j.|.d.d.d..
-000008e0: 037c 0883 017d 0874 097c 087c 027c 0764  .|...}.t.|.|.|.d
-000008f0: 098d 035c 047d 0a7d 0b7d 0c7d 0d7c 006a  ...\.}.}.}.}.|.j
-00000900: 0a73 ee74 0b6a 0c64 0a7c 0785 0264 0a7c  .s.t.j.d.|...d.|
-00000910: 0785 0266 0219 007c 071b 0064 0b18 00a0  ...f...|...d....
-00000920: 0d64 0864 0164 02a1 037d 0e74 046a 057c  .d.d.d...}.t.j.|
-00000930: 0964 0c64 0464 058d 037c 0e83 017d 0e6e  .d.d.d...|...}.n
-00000940: 1c74 0e7c 097c 077c 006a 0f83 037c 0174  .t.|.|.|.j...|.t
-00000950: 037c 0483 0119 007c 0283 027d 0e7c 0a7c  .|.....|...}.|.|
-00000960: 0e37 007d 0a74 0ba0 107c 0264 026b 056a  .7.}.t...|.d.k.j
-00000970: 1164 0d64 0e8d 0164 0fa1 027d 0f74 076a  .d.d...d...}.t.j
-00000980: 04a0 087c 0aa1 017d 0a7c 006a 1290 0172  ...|...}.|.j...r
-00000990: 4874 1383 007c 0a83 017d 0a7c 0664 0819  Ht...|...}.|.d..
-000009a0: 0064 0864 0a85 0219 0044 005d 227d 0974  .d.d.....D.]"}.t
-000009b0: 04a0 057c 0964 03a1 027c 0a83 017d 0a74  ...|.d...|...}.t
-000009c0: 076a 04a0 087c 0aa1 017d 0a90 0171 587c  .j...|...}...qX|
-000009d0: 0564 086b 0290 0172 9874 04a0 0564 0864  .d.k...r.t...d.d
-000009e0: 03a1 027c 0a83 017d 106e 4274 046a 1464  ...|...}.nBt.j.d
-000009f0: 0864 1064 1064 118d 037c 0a83 017d 107c  .d.d.d...|...}.|
-00000a00: 0564 126b 0290 0172 da74 076a 15a0 167c  .d.k...r.t.j...|
-00000a10: 107c 0a6a 1764 0a64 0885 0219 007c 037c  .|.j.d.d.....|.|
-00000a20: 0364 0866 0317 0064 13a1 037d 107c 10a0  .d.f...d...}.|..
-00000a30: 1864 0da1 017d 1074 076a 04a0 197c 10a1  .d...}.t.j...|..
-00000a40: 017d 1174 0b6a 0c64 0a7c 0385 0264 0a7c  .}.t.j.d.|...d.|
-00000a50: 0385 0266 0219 005c 027d 127d 137c 127c  ...f...\.}.}.|.|
-00000a60: 0b64 0a64 0a85 0264 0a64 0a66 0319 007c  .d.d...d.d.f...|
-00000a70: 0514 0017 007d 127c 137c 0c64 0a64 0a85  .....}.|.|.d.d..
-00000a80: 0264 0a64 0a66 0319 007c 0514 0017 007d  .d.d.f...|.....}
-00000a90: 1374 0ba0 1a7c 0f7c 1164 02a1 037d 1174  .t...|.|.d...}.t
-00000aa0: 0ba0 1a7c 0f7c 1064 02a1 037d 1074 0ba0  ...|.|.d...}.t..
-00000ab0: 1a7c 0f7c 1364 0da1 037d 1374 0ba0 1a7c  .|.|.d...}.t...|
-00000ac0: 0f7c 1264 0da1 037d 1274 1b7c 117c 127c  .|.d...}.t.|.|.|
-00000ad0: 137c 107c 0f64 148d 0553 0029 1561 a401  .|.|.d...S.).a..
-00000ae0: 0000 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00000af0: 0a20 2020 2020 2020 2020 2020 2066 6561  .            fea
-00000b00: 7475 7265 733a 207b 276c 766c 2720 5b48  tures: {'lvl' [H
-00000b10: 2c20 572c 2043 5d7d 2066 6561 7475 7265  , W, C]} feature
-00000b20: 2064 6963 7469 6f6e 6172 790a 2020 2020   dictionary.    
-00000b30: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
-00000b40: 733a 205b 4e2c 2032 5d20 2073 6361 6c65  s: [N, 2]  scale
-00000b50: 6420 302e 2e31 0a20 2020 2020 2020 206f  d 0..1.        o
-00000b60: 7574 7075 7473 3a0a 2020 2020 2020 2020  utputs:.        
-00000b70: 2020 2020 696e 7374 616e 6365 5f6f 7574      instance_out
-00000b80: 7075 743a 205b 4e2c 2063 726f 705f 7369  put: [N, crop_si
-00000b90: 7a65 2c20 6372 6f70 5f73 697a 655d 0a20  ze, crop_size]. 
-00000ba0: 2020 2020 2020 2020 2020 2069 6e73 7461             insta
-00000bb0: 6e63 655f 6d61 736b 3b20 5b4e 2c20 312c  nce_mask; [N, 1,
-00000bc0: 2031 5d20 626f 6f6c 6561 6e20 6d61 736b   1] boolean mask
-00000bd0: 2069 6e64 6963 6174 696e 6720 7661 6c69   indicating vali
-00000be0: 6420 6f75 7470 7574 730a 2020 2020 2020  d outputs.      
-00000bf0: 2020 2020 2020 696e 7374 616e 6365 5f79        instance_y
-00000c00: 633a 205b 4e2c 2063 726f 705f 7369 7a65  c: [N, crop_size
-00000c10: 2c20 6372 6f70 5f73 697a 655d 206d 6573  , crop_size] mes
-00000c20: 6867 7269 6420 7920 636f 6f72 6469 6e61  hgrid y coordina
-00000c30: 7465 730a 2020 2020 2020 2020 2020 2020  tes.            
-00000c40: 696e 7374 616e 6365 5f78 633a 205b 4e2c  instance_xc: [N,
-00000c50: 2063 726f 705f 7369 7a65 2c20 6372 6f70   crop_size, crop
-00000c60: 5f73 697a 655d 206d 6573 6867 7269 6420  _size] meshgrid 
-00000c70: 7820 636f 6f72 6469 6e61 7465 730a 2020  x coordinates.  
-00000c80: 2020 2020 2020 7203 0000 0072 0100 0000        r....r....
-00000c90: 2902 e903 0000 0072 4500 0000 4672 1800  )......rE...Fr..
-00000ca0: 0000 2901 da0a 6e75 6d5f 6772 6f75 7073  ..)...num_groups
-00000cb0: 2902 4e2e 7205 0000 0072 1000 0000 4e67  ).N.r....r....Ng
-00000cc0: 0000 0000 0000 e03f 7217 0000 0072 0e00  .......?r....r..
-00000cd0: 0000 7214 0000 0029 0272 0500 0000 7203  ..r....).r....r.
-00000ce0: 0000 0029 0272 0300 0000 7203 0000 0029  ...).r....r....)
-00000cf0: 01da 0773 7472 6964 6573 720c 0000 0072  ...stridesr....r
-00000d00: 1600 0000 2905 da0f 696e 7374 616e 6365  ....)...instance
-00000d10: 5f6f 7574 7075 74da 0b69 6e73 7461 6e63  _output..instanc
-00000d20: 655f 7963 da0b 696e 7374 616e 6365 5f78  e_yc..instance_x
-00000d30: 63da 0e69 6e73 7461 6e63 655f 6c6f 6769  c..instance_logi
-00000d40: 74da 0d69 6e73 7461 6e63 655f 6d61 736b  t..instance_mask
-00000d50: 291c 723e 0000 0072 3900 0000 723c 0000  ).r>...r9...r<..
-00000d60: 00da 0373 7472 721d 0000 0072 2500 0000  ...strr....r%...
-00000d70: da09 4772 6f75 704e 6f72 6d72 1f00 0000  ..GroupNormr....
-00000d80: 7220 0000 0072 0400 0000 7240 0000 00da  r ...r....r@....
-00000d90: 036a 6e70 da05 6d67 7269 64da 0974 7261  .jnp..mgrid..tra
-00000da0: 6e73 706f 7365 7207 0000 0072 4100 0000  nsposer....rA...
-00000db0: da0b 6578 7061 6e64 5f64 696d 73da 0361  ..expand_dims..a
-00000dc0: 6e79 723f 0000 0072 0600 0000 da0d 436f  nyr?...r......Co
-00000dd0: 6e76 5472 616e 7370 6f73 6572 2200 0000  nvTransposer"...
-00000de0: 7223 0000 0072 2400 0000 da07 7371 7565  r#...r$.....sque
-00000df0: 657a 65da 0773 6967 6d6f 6964 da05 7768  eze..sigmoid..wh
-00000e00: 6572 65da 0464 6963 7429 1472 2600 0000  ere..dict).r&...
-00000e10: 7242 0000 0072 4300 0000 da09 6372 6f70  rB...rC.....crop
-00000e20: 5f73 697a 65da 036c 766c da05 7363 616c  _size..lvl..scal
-00000e30: 6572 3c00 0000 7211 0000 00da 0178 da04  er<...r......x..
-00000e40: 6e5f 6368 da07 7061 7463 6865 73da 0279  n_ch..patches..y
-00000e50: 30da 0278 3072 2900 0000 722a 0000 00da  0..x0r)...r*....
-00000e60: 046d 6173 6bda 066c 6f67 6974 73da 076f  .mask..logits..o
-00000e70: 7574 7075 7473 da02 7963 da02 7863 722d  utputs..yc..xcr-
-00000e80: 0000 0072 2d00 0000 722e 0000 0072 2f00  ...r-...r....r/.
-00000e90: 0000 4c00 0000 737c 0000 0000 0c06 0106  ..L...s|........
-00000ea0: 0108 0106 0108 020c 040c 0114 0118 010e  ................
-00000eb0: 030c 0114 0116 0206 021e 0102 0002 0002  ................
-00000ec0: ff02 ff02 0316 0202 0102 0102 0104 fd02  ................
-00000ed0: 040a 0002 fc04 0608 0118 010c 0208 010a  ................
-00000ee0: 0314 0110 0110 030a 0112 0214 010a 0106  ................
-00000ef0: 0102 0016 0002 ff04 040a 010c 031a 011a  ................
-00000f00: 011a 030e 010e 010e 010e 0202 0102 0102  ................
-00000f10: 0102 0102 0102 fb7a 1253 6567 6d65 6e74  .......z.Segment
-00000f20: 6f72 2e5f 5f63 616c 6c5f 5f4e 2916 7230  or.__call__N).r0
-00000f30: 0000 0072 3100 0000 7232 0000 00da 075f  ...r1...r2....._
-00000f40: 5f64 6f63 5f5f 7239 0000 0072 3300 0000  _doc__r9...r3...
-00000f50: 7234 0000 0072 3c00 0000 7235 0000 0072  r4...r<...r5...r
-00000f60: 3600 0000 da08 5365 7175 656e 6365 723e  6.....Sequencer>
-00000f70: 0000 0072 3f00 0000 da04 626f 6f6c 7240  ...r?.....boolr@
-00000f80: 0000 0072 4100 0000 721d 0000 0072 3700  ...rA...r....r7.
-00000f90: 0000 7258 0000 0072 4f00 0000 da07 6e64  ..rX...rO.....nd
-00000fa0: 6172 7261 7972 2f00 0000 722d 0000 0072  arrayr/...r-...r
-00000fb0: 2d00 0000 722d 0000 0072 2e00 0000 7238  -...r-...r....r8
-00000fc0: 0000 0032 0000 0073 1200 0000 0a01 040b  ...2...s........
-00000fd0: 0c01 2204 0c01 0c01 0c01 1206 0401 7238  .."...........r8
-00000fe0: 0000 0029 1372 1b00 0000 da06 7479 7069  ...).r......typi
-00000ff0: 6e67 7235 0000 00da 0966 756e 6374 6f6f  ngr5.....functoo
-00001000: 6c73 7202 0000 00da 0a66 6c61 782e 6c69  lsr......flax.li
-00001010: 6e65 6eda 056c 696e 656e 721d 0000 0072  nen..linenr....r
-00001020: 1f00 0000 da09 6a61 782e 6e75 6d70 79da  ......jax.numpy.
-00001030: 056e 756d 7079 724f 0000 00da 036f 7073  .numpyrO.....ops
-00001040: 7204 0000 00da 0663 6f6d 6d6f 6e72 0600  r......commonr..
-00001050: 0000 da06 4d6f 6475 6c65 7207 0000 0072  ....Moduler....r
-00001060: 3800 0000 722d 0000 0072 2d00 0000 722d  8...r-...r-...r-
-00001070: 0000 0072 2e00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00001080: 653e 0100 0000 7312 0000 0008 0108 010c  e>....s.........
-00001090: 020c 0108 010c 020c 010c 0312 25         ............%
+00000120: 0464 023c 0064 035a 0565 0665 0365 0365  .d.<.d.Z.e.e.e.e
+00000130: 0366 0319 0065 0464 043c 0064 055a 0765  .f...e.d.<.d.Z.e
+00000140: 0365 0464 063c 0065 086a 0965 0a65 0a65  .e.d.<.e.j.e.e.e
+00000150: 0b64 079c 0364 0864 0984 0483 015a 0c64  .d...d.d.....Z.d
+00000160: 0a53 0029 0bda 085f 456e 636f 6465 72da  .S.)..._Encoder.
+00000170: 116e 5f6f 7574 7075 745f 6665 6174 7572  .n_output_featur
+00000180: 6573 da10 696e 7075 745f 7061 7463 685f  es..input_patch_
+00000190: 7369 7a65 a903 e908 0000 0072 0b00 0000  size.......r....
+000001a0: e904 0000 00da 0d65 6e63 6f64 696e 675f  .......encoding_
+000001b0: 6469 6d73 e9ff ffff ffda 116e 5f6c 6174  dims.......n_lat
+000001c0: 656e 745f 6665 6174 7572 6573 2903 da07  ent_features)...
+000001d0: 6665 6174 7572 65da 036c 6f63 da06 7265  feature..loc..re
+000001e0: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
+000001f0: 0009 0000 0008 0000 0043 0000 0073 e000  .........C...s..
+00000200: 0000 7400 7c01 7c02 6401 6402 8d03 5c04  ..t.|.|.d.d...\.
+00000210: 7d03 7d04 7d04 7d04 7c03 6a01 6403 6404  }.}.}.}.|.j.d.d.
+00000220: 8d01 7d05 7c00 6a02 7d06 7c06 6405 6b04  ..}.|.j.}.|.d.k.
+00000230: 7234 7c06 6e0a 7403 a004 7c00 6a05 a101  r4|.n.t...|.j...
+00000240: 7d06 7406 a007 7c06 a101 7c05 8301 7d05  }.t...|...|...}.
+00000250: 7408 6a06 a009 7c05 a101 7d05 7406 a007  t.j...|...}.t...
+00000260: 7c06 a101 7c05 8301 7d05 7408 6a06 a009  |...|...}.t.j...
+00000270: 7c05 a101 7d05 7403 a004 7c00 6a05 a101  |...}.t...|.j...
+00000280: 7d07 6406 7c00 6a05 1700 7d08 7406 a007  }.d.|.j...}.t...
+00000290: 7c07 a101 7c05 8301 a00a 7c08 a101 7d05  |...|.....|...}.
+000002a0: 7408 6a0b a00c 7c05 7c05 6a0d 6405 1900  t.j...|.|.j.d...
+000002b0: 7c00 6a0e 7c00 6a0e 7c00 6a05 6407 1900  |.j.|.j.|.j.d...
+000002c0: 6604 6408 a103 7d05 7406 6a0f 7c00 6a10  f.d...}.t.j.|.j.
+000002d0: 6409 640a 640b 8d03 7c05 8301 7d05 7c05  d.d.d...|...}.|.
+000002e0: 5300 290c 4ee9 0200 0000 a901 da0a 7061  S.).N.........pa
+000002f0: 7463 685f 7369 7a65 2902 e9fe ffff ffe9  tch_size).......
+00000300: fdff ffff a901 da04 6178 6973 7201 0000  ........axisr...
+00000310: 0029 0172 0e00 0000 720e 0000 00da 066c  .).r....r......l
+00000320: 696e 6561 72a9 0272 0500 0000 7205 0000  inear..r....r...
+00000330: 0046 a901 da08 7573 655f 6269 6173 2911  .F....use_bias).
+00000340: 7203 0000 00da 046d 6561 6e72 0f00 0000  r......meanr....
+00000350: da04 6d61 7468 da04 7072 6f64 720d 0000  ..math..prodr...
+00000360: 00da 026e 6eda 0544 656e 7365 da03 6a61  ...nn..Dense..ja
+00000370: 78da 0472 656c 75da 0772 6573 6861 7065  x..relu..reshape
+00000380: da05 696d 6167 65da 0672 6573 697a 65da  ..image..resize.
+00000390: 0573 6861 7065 7209 0000 00da 0443 6f6e  .shaper......Con
+000003a0: 7672 0800 0000 2909 da04 7365 6c66 7210  vr....)...selfr.
+000003b0: 0000 0072 1100 0000 5a0c 7061 7463 685f  ...r....Z.patch_
+000003c0: 6365 6e74 6572 da01 5fda 0965 6e63 6f64  center.._..encod
+000003d0: 696e 6773 da03 6469 6dda 076e 6577 5f64  ings..dim..new_d
+000003e0: 696d 5a0e 656e 636f 6469 6e67 5f73 6861  imZ.encoding_sha
+000003f0: 7065 a900 722f 0000 00fa 3a2f 686f 6d65  pe..r/....:/home
+00000400: 2f46 4341 4d2f 6a79 752f 7072 6f6a 5f6c  /FCAM/jyu/proj_l
+00000410: 6163 7373 2f6c 6163 7373 2f6c 6163 7373  acss/lacss/lacss
+00000420: 2f6d 6f64 756c 6573 2f73 6567 6d65 6e74  /modules/segment
+00000430: 6f72 2e70 79da 085f 5f63 616c 6c5f 5f14  or.py..__call__.
+00000440: 0000 0073 2c00 0000 0002 1601 0c02 0601  ...s,...........
+00000450: 1801 0e01 0c01 0e01 0c02 0c01 0a01 1401  ................
+00000460: 0601 0202 0801 0401 0401 08fc 0206 02f8  ................
+00000470: 040b 1602 7a11 5f45 6e63 6f64 6572 2e5f  ....z._Encoder._
+00000480: 5f63 616c 6c5f 5f4e 290d da08 5f5f 6e61  _call__N)...__na
+00000490: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+000004a0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da03  ..__qualname__..
+000004b0: 696e 74da 0f5f 5f61 6e6e 6f74 6174 696f  int..__annotatio
+000004c0: 6e73 5f5f 720d 0000 00da 0554 7570 6c65  ns__r......Tuple
+000004d0: 720f 0000 0072 2100 0000 da07 636f 6d70  r....r!.....comp
+000004e0: 6163 74da 0941 7272 6179 4c69 6b65 da05  act..ArrayLike..
+000004f0: 4172 7261 7972 3100 0000 722f 0000 0072  Arrayr1...r/...r
+00000500: 2f00 0000 722f 0000 0072 3000 0000 7207  /...r/...r0...r.
+00000510: 0000 000e 0000 0073 0c00 0000 0a01 0801  .......s........
+00000520: 0801 1601 0c02 0401 7207 0000 0063 0000  ........r....c..
+00000530: 0000 0000 0000 0000 0000 0000 0000 0500  ................
+00000540: 0000 4000 0000 738e 0000 0065 005a 0164  ..@...s....e.Z.d
+00000550: 005a 0255 0064 015a 0364 025a 0465 0565  .Z.U.d.Z.d.Z.e.e
+00000560: 0664 033c 0064 045a 0765 0865 0965 0519  .d.<.d.Z.e.e.e..
+00000570: 0065 0965 0519 0066 0219 0065 0664 053c  .e.e...f...e.d.<
+00000580: 0064 065a 0a65 0565 0664 073c 0064 085a  .d.Z.e.e.d.<.d.Z
+00000590: 0b65 0c65 0664 093c 0064 0a5a 0d65 0c65  .e.e.d.<.d.Z.e.e
+000005a0: 0664 0b3c 0064 0c5a 0e65 0965 0519 0065  .d.<.d.Z.e.e...e
+000005b0: 0664 0d3c 0065 0f6a 1065 1165 1265 1366  .d.<.e.j.e.e.e.f
+000005c0: 0219 0065 1365 1464 0e9c 0364 0f64 1084  ...e.e.d...d.d..
+000005d0: 0483 015a 1564 1153 0029 12da 0953 6567  ...Z.d.S.)...Seg
+000005e0: 6d65 6e74 6f72 61d8 0100 004c 4143 5353  mentora....LACSS
+000005f0: 2073 6567 6d65 6e74 6174 696f 6e20 6865   segmentation he
+00000600: 6164 2e0a 0a20 2020 2041 7474 7269 6275  ad...    Attribu
+00000610: 7465 733a 0a20 2020 2020 2020 2066 6561  tes:.        fea
+00000620: 7475 7265 5f6c 6576 656c 3a20 5468 6520  ture_level: The 
+00000630: 7363 616c 6520 6f66 2074 6865 2066 6561  scale of the fea
+00000640: 7475 7265 2075 7365 6420 666f 7220 7365  ture used for se
+00000650: 676d 656e 7461 7469 6f6e 0a20 2020 2020  gmentation.     
+00000660: 2020 2063 6f6e 765f 7370 6563 3a20 636f     conv_spec: co
+00000670: 6e76 5f62 6c6f 636b 2064 6566 696e 6974  nv_block definit
+00000680: 696f 6e2c 2065 2e67 2e20 2828 3338 342c  ion, e.g. ((384,
+00000690: 3338 342c 3338 3429 2c20 2836 342c 2929  384,384), (64,))
+000006a0: 0a20 2020 2020 2020 2069 6e73 7461 6e63  .        instanc
+000006b0: 655f 6372 6f70 5f73 697a 653a 2043 726f  e_crop_size: Cro
+000006c0: 7020 7369 7a65 2066 6f72 2073 6567 6d65  p size for segme
+000006d0: 6e74 6174 696f 6e2e 0a20 2020 2020 2020  ntation..       
+000006e0: 2077 6974 685f 6174 7465 6e74 696f 6e3a   with_attention:
+000006f0: 2057 6865 7468 6572 2075 7365 2073 7061   Whether use spa
+00000700: 7469 616c 2061 7474 656e 7469 6f6e 206c  tial attention l
+00000710: 6179 6572 2e0a 2020 2020 2020 2020 6c65  ayer..        le
+00000720: 6172 6e65 645f 656e 636f 6469 6e67 3a20  arned_encoding: 
+00000730: 5768 6574 6865 7220 746f 2075 7365 2068  Whether to use h
+00000740: 6172 642d 636f 6465 6420 706f 7369 7469  ard-coded positi
+00000750: 6f6e 2065 6e63 6f64 696e 672e 0a20 2020  on encoding..   
+00000760: 2020 2020 2065 6e63 6f64 6572 5f64 696d       encoder_dim
+00000770: 733a 2044 696d 206f 6620 7468 6520 706f  s: Dim of the po
+00000780: 7369 7469 6f6e 2065 6e63 6f64 6572 2c20  sition encoder, 
+00000790: 6966 2075 7369 6e67 206c 6561 726e 6564  if using learned
+000007a0: 2065 6e63 6f64 696e 672e 2044 6566 6175   encoding. Defau
+000007b0: 6c74 2069 7320 2838 2c38 2c34 290a 0a20  lt is (8,8,4).. 
+000007c0: 2020 2072 1300 0000 da0d 6665 6174 7572     r......featur
+000007d0: 655f 6c65 7665 6c29 0229 03e9 8001 0000  e_level).)......
+000007e0: 723d 0000 0072 3d00 0000 2901 e940 0000  r=...r=...)..@..
+000007f0: 00da 0963 6f6e 765f 7370 6563 e960 0000  ...conv_spec.`..
+00000800: 00da 1269 6e73 7461 6e63 655f 6372 6f70  ...instance_crop
+00000810: 5f73 697a 6546 da0d 7573 655f 6174 7465  _sizeF..use_atte
+00000820: 6e74 696f 6e54 da10 6c65 6172 6e65 645f  ntionT..learned_
+00000830: 656e 636f 6469 6e67 720a 0000 00da 0c65  encodingr......e
+00000840: 6e63 6f64 6572 5f64 696d 7329 03da 0866  ncoder_dims)...f
+00000850: 6561 7475 7265 73da 096c 6f63 6174 696f  eatures..locatio
+00000860: 6e73 7212 0000 0063 0300 0000 0000 0000  nsr....c........
+00000870: 0000 0000 1400 0000 0700 0000 4300 0000  ............C...
+00000880: 7388 0200 007c 006a 007d 037c 006a 017d  s....|.j.}.|.j.}
+00000890: 0464 017c 0413 007d 057c 006a 027d 067c  .d.|...}.|.j.}.|
+000008a0: 037c 051a 007d 077c 0174 037c 0483 0119  .|...}.|.t.|....
+000008b0: 007d 087c 0664 0219 0044 005d 3c7d 0974  .}.|.d...D.]<}.t
+000008c0: 046a 057c 0964 0364 0464 058d 037c 0883  .j.|.d.d.d...|..
+000008d0: 017d 0874 046a 067c 0964 068d 017c 0864  .}.t.j.|.d...|.d
+000008e0: 0719 0083 0164 0219 007d 0874 076a 04a0  .....d...}.t.j..
+000008f0: 087c 08a1 017d 0871 367c 0664 0819 0064  .|...}.q6|.d...d
+00000900: 0219 007d 0974 046a 057c 0964 0364 0464  ...}.t.j.|.d.d.d
+00000910: 058d 037c 0883 017d 0874 097c 087c 027c  ...|...}.t.|.|.|
+00000920: 0764 098d 035c 047d 0a7d 0b7d 0c7d 0d7c  .d...\.}.}.}.}.|
+00000930: 006a 0a73 ee74 0b6a 0c64 0a7c 0785 0264  .j.s.t.j.d.|...d
+00000940: 0a7c 0785 0266 0219 007c 071b 0064 0b18  .|...f...|...d..
+00000950: 00a0 0d64 0864 0164 02a1 037d 0e74 046a  ...d.d.d...}.t.j
+00000960: 057c 0964 0c64 0464 058d 037c 0e83 017d  .|.d.d.d...|...}
+00000970: 0e6e 1c74 0e7c 097c 077c 006a 0f83 037c  .n.t.|.|.|.j...|
+00000980: 0174 037c 0483 0119 007c 0283 027d 0e7c  .t.|.....|...}.|
+00000990: 0a7c 0e37 007d 0a74 0ba0 107c 0264 026b  .|.7.}.t...|.d.k
+000009a0: 056a 1164 0d64 0e8d 0164 0fa1 027d 0f74  .j.d.d...d...}.t
+000009b0: 076a 04a0 087c 0aa1 017d 0a7c 006a 1290  .j...|...}.|.j..
+000009c0: 0172 4874 1383 007c 0a83 017d 0a7c 0664  .rHt...|...}.|.d
+000009d0: 0819 0064 0864 0a85 0219 0044 005d 227d  ...d.d.....D.]"}
+000009e0: 0974 04a0 057c 0964 03a1 027c 0a83 017d  .t...|.d...|...}
+000009f0: 0a74 076a 04a0 087c 0aa1 017d 0a90 0171  .t.j...|...}...q
+00000a00: 587c 0564 086b 0290 0172 9874 04a0 0564  X|.d.k...r.t...d
+00000a10: 0864 03a1 027c 0a83 017d 106e 4274 046a  .d...|...}.nBt.j
+00000a20: 1464 0864 1064 1064 118d 037c 0a83 017d  .d.d.d.d...|...}
+00000a30: 107c 0564 126b 0290 0172 da74 076a 15a0  .|.d.k...r.t.j..
+00000a40: 167c 107c 0a6a 1764 0a64 0885 0219 007c  .|.|.j.d.d.....|
+00000a50: 037c 0364 0866 0317 0064 13a1 037d 107c  .|.d.f...d...}.|
+00000a60: 10a0 1864 0da1 017d 1074 076a 04a0 197c  ...d...}.t.j...|
+00000a70: 10a1 017d 1174 0b6a 0c64 0a7c 0385 0264  ...}.t.j.d.|...d
+00000a80: 0a7c 0385 0266 0219 005c 027d 127d 137c  .|...f...\.}.}.|
+00000a90: 127c 0b64 0a64 0a85 0264 0a64 0a66 0319  .|.d.d...d.d.f..
+00000aa0: 007c 0514 0017 007d 127c 137c 0c64 0a64  .|.....}.|.|.d.d
+00000ab0: 0a85 0264 0a64 0a66 0319 007c 0514 0017  ...d.d.f...|....
+00000ac0: 007d 1374 0ba0 1a7c 0f7c 1164 02a1 037d  .}.t...|.|.d...}
+00000ad0: 1174 0ba0 1a7c 0f7c 1064 02a1 037d 1074  .t...|.|.d...}.t
+00000ae0: 0ba0 1a7c 0f7c 1364 0da1 037d 1374 0ba0  ...|.|.d...}.t..
+00000af0: 1a7c 0f7c 1264 0da1 037d 1274 1b7c 117c  .|.|.d...}.t.|.|
+00000b00: 127c 137c 107c 0f64 148d 0553 0029 1561  .|.|.|.d...S.).a
+00000b10: 2702 0000 0a20 2020 2020 2020 2041 7267  '....        Arg
+00000b20: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
+00000b30: 6561 7475 7265 733a 207b 2773 6361 6c65  eatures: {'scale
+00000b40: 2720 5b48 2c20 572c 2043 5d7d 2066 6561  ' [H, W, C]} fea
+00000b50: 7475 7265 2064 6963 7469 6f6e 6172 7920  ture dictionary 
+00000b60: 6672 6f6d 2074 6865 2062 6163 6b62 6f6e  from the backbon
+00000b70: 652e 0a20 2020 2020 2020 2020 2020 206c  e..            l
+00000b80: 6f63 6174 696f 6e73 3a20 5b4e 2c20 325d  ocations: [N, 2]
+00000b90: 2020 6e6f 726d 616c 697a 6564 2074 6f20    normalized to 
+00000ba0: 696d 6167 6520 7369 7a65 2e0a 0a20 2020  image size...   
+00000bb0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00000bc0: 2020 2020 2020 2020 2020 4120 6469 6374            A dict
+00000bd0: 696f 6e61 7279 206f 6620 7661 6c75 6573  ionary of values
+00000be0: 2072 6570 7265 7365 6e74 696e 6720 7365   representing se
+00000bf0: 676d 656e 7461 7469 6f6e 206f 7574 7075  gmentation outpu
+00000c00: 7473 2e0a 0a20 2020 2020 2020 2020 2020  ts...           
+00000c10: 2020 2020 202a 2069 6e73 7461 6e63 655f       * instance_
+00000c20: 6f75 7470 7574 3a20 5b4e 2c20 6372 6f70  output: [N, crop
+00000c30: 5f73 697a 652c 2063 726f 705f 7369 7a65  _size, crop_size
+00000c40: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00000c50: 2020 2a20 696e 7374 616e 6365 5f6d 6173    * instance_mas
+00000c60: 6b3b 205b 4e2c 2031 2c20 315d 2062 6f6f  k; [N, 1, 1] boo
+00000c70: 6c65 616e 206d 6173 6b20 696e 6469 6361  lean mask indica
+00000c80: 7469 6e67 2076 616c 6964 206f 7574 7075  ting valid outpu
+00000c90: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
+00000ca0: 2020 202a 2069 6e73 7461 6e63 655f 7963     * instance_yc
+00000cb0: 3a20 5b4e 2c20 6372 6f70 5f73 697a 652c  : [N, crop_size,
+00000cc0: 2063 726f 705f 7369 7a65 5d20 6d65 7368   crop_size] mesh
+00000cd0: 6772 6964 2079 2063 6f6f 7264 696e 6174  grid y coordinat
+00000ce0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00000cf0: 2020 202a 2069 6e73 7461 6e63 655f 7863     * instance_xc
+00000d00: 3a20 5b4e 2c20 6372 6f70 5f73 697a 652c  : [N, crop_size,
+00000d10: 2063 726f 705f 7369 7a65 5d20 6d65 7368   crop_size] mesh
+00000d20: 6772 6964 2078 2063 6f6f 7264 696e 6174  grid x coordinat
+00000d30: 6573 0a20 2020 2020 2020 2072 1300 0000  es.        r....
+00000d40: 7201 0000 0029 02e9 0300 0000 7247 0000  r....)......rG..
+00000d50: 0046 721c 0000 0029 01da 0a6e 756d 5f67  .Fr....)...num_g
+00000d60: 726f 7570 7329 024e 2e72 0500 0000 7214  roups).N.r....r.
+00000d70: 0000 004e 6700 0000 0000 00e0 3f72 1b00  ...Ng.......?r..
+00000d80: 0000 720e 0000 0072 1800 0000 2902 7205  ..r....r....).r.
+00000d90: 0000 0072 1300 0000 2902 7213 0000 0072  ...r....).r....r
+00000da0: 1300 0000 2901 da07 7374 7269 6465 7372  ....)...stridesr
+00000db0: 0c00 0000 721a 0000 0029 05da 0f69 6e73  ....r....)...ins
+00000dc0: 7461 6e63 655f 6f75 7470 7574 da0b 696e  tance_output..in
+00000dd0: 7374 616e 6365 5f79 63da 0b69 6e73 7461  stance_yc..insta
+00000de0: 6e63 655f 7863 da0e 696e 7374 616e 6365  nce_xc..instance
+00000df0: 5f6c 6f67 6974 da0d 696e 7374 616e 6365  _logit..instance
+00000e00: 5f6d 6173 6b29 1c72 4100 0000 723c 0000  _mask).rA...r<..
+00000e10: 0072 3f00 0000 da03 7374 7272 2100 0000  .r?.....strr!...
+00000e20: 7229 0000 00da 0947 726f 7570 4e6f 726d  r).....GroupNorm
+00000e30: 7223 0000 0072 2400 0000 7203 0000 0072  r#...r$...r....r
+00000e40: 4300 0000 da03 6a6e 70da 056d 6772 6964  C.....jnp..mgrid
+00000e50: da09 7472 616e 7370 6f73 6572 0700 0000  ..transposer....
+00000e60: 7244 0000 00da 0b65 7870 616e 645f 6469  rD.....expand_di
+00000e70: 6d73 da03 616e 7972 4200 0000 7206 0000  ms..anyrB...r...
+00000e80: 00da 0d43 6f6e 7654 7261 6e73 706f 7365  ...ConvTranspose
+00000e90: 7226 0000 0072 2700 0000 7228 0000 00da  r&...r'...r(....
+00000ea0: 0773 7175 6565 7a65 da07 7369 676d 6f69  .squeeze..sigmoi
+00000eb0: 64da 0577 6865 7265 da04 6469 6374 2914  d..where..dict).
+00000ec0: 722a 0000 0072 4500 0000 7246 0000 00da  r*...rE...rF....
+00000ed0: 0963 726f 705f 7369 7a65 da03 6c76 6cda  .crop_size..lvl.
+00000ee0: 0573 6361 6c65 723f 0000 0072 1500 0000  .scaler?...r....
+00000ef0: da01 78da 046e 5f63 68da 0770 6174 6368  ..x..n_ch..patch
+00000f00: 6573 da02 7930 da02 7830 722b 0000 0072  es..y0..x0r+...r
+00000f10: 2c00 0000 da04 6d61 736b da06 6c6f 6769  ,.....mask..logi
+00000f20: 7473 da07 6f75 7470 7574 73da 0279 63da  ts..outputs..yc.
+00000f30: 0278 6372 2f00 0000 722f 0000 0072 3000  .xcr/...r/...r0.
+00000f40: 0000 7231 0000 004e 0000 0073 7c00 0000  ..r1...N...s|...
+00000f50: 0011 0601 0601 0801 0601 0802 0c04 0c01  ................
+00000f60: 1401 1801 0e03 0c01 1401 1602 0602 1e01  ................
+00000f70: 0200 0200 02ff 02ff 0203 1602 0201 0201  ................
+00000f80: 0201 04fd 0204 0a00 02fc 0406 0801 1801  ................
+00000f90: 0c02 0801 0a03 1401 1001 1003 0a01 1202  ................
+00000fa0: 1401 0a01 0601 0200 1600 02ff 0404 0a01  ................
+00000fb0: 0c03 1a01 1a01 1a03 0e01 0e01 0e01 0e02  ................
+00000fc0: 0201 0201 0201 0201 0201 02fb 7a12 5365  ............z.Se
+00000fd0: 676d 656e 746f 722e 5f5f 6361 6c6c 5f5f  gmentor.__call__
+00000fe0: 4e29 1672 3200 0000 7233 0000 0072 3400  N).r2...r3...r4.
+00000ff0: 0000 da07 5f5f 646f 635f 5f72 3c00 0000  ....__doc__r<...
+00001000: 7235 0000 0072 3600 0000 723f 0000 0072  r5...r6...r?...r
+00001010: 3700 0000 da08 5365 7175 656e 6365 7241  7.....SequencerA
+00001020: 0000 0072 4200 0000 da04 626f 6f6c 7243  ...rB.....boolrC
+00001030: 0000 0072 4400 0000 7221 0000 0072 3800  ...rD...r!...r8.
+00001040: 0000 da07 4d61 7070 696e 6772 4f00 0000  ....MappingrO...
+00001050: 7239 0000 00da 0844 6174 6144 6963 7472  r9.....DataDictr
+00001060: 3100 0000 722f 0000 0072 2f00 0000 722f  1...r/...r/...r/
+00001070: 0000 0072 3000 0000 723b 0000 0033 0000  ...r0...r;...3..
+00001080: 0073 1800 0000 0a01 040c 0c01 1c04 0c01  .s..............
+00001090: 0c01 0c01 1006 0402 0a00 0201 02fe 723b  ..............r;
+000010a0: 0000 0029 1272 1f00 0000 da09 6675 6e63  ...).r......func
+000010b0: 746f 6f6c 7372 0200 0000 da0a 666c 6178  toolsr......flax
+000010c0: 2e6c 696e 656e da05 6c69 6e65 6e72 2100  .linen..linenr!.
+000010d0: 0000 7223 0000 00da 096a 6178 2e6e 756d  ..r#.....jax.num
+000010e0: 7079 da05 6e75 6d70 7972 5100 0000 da09  py..numpyrQ.....
+000010f0: 6c61 6373 732e 6f70 7372 0300 0000 da0b  lacss.opsr......
+00001100: 6c61 6373 732e 7479 7065 73da 0663 6f6d  lacss.types..com
+00001110: 6d6f 6e72 0600 0000 da06 4d6f 6475 6c65  monr......Module
+00001120: 7207 0000 0072 3b00 0000 722f 0000 0072  r....r;...r/...r
+00001130: 2f00 0000 722f 0000 0072 3000 0000 da08  /...r/...r0.....
+00001140: 3c6d 6f64 756c 653e 0100 0000 7312 0000  <module>....s...
+00001150: 0008 010c 020c 0108 010c 020c 0108 020c  ................
+00001160: 0312 25                                  ..%
```

### Comparing `lacss-0.4.1/lacss/modules/common.py` & `lacss-0.4.2/lacss/modules/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-import typing as tp
+from __future__ import annotations
 
 import flax.linen as nn
 import jax
 import jax.numpy as jnp
 
+from lacss.types import *
+
 
 class ChannelAttention(nn.Module):
     squeeze_factor: int = 16
 
     @nn.compact
     def __call__(
         self,
-        x: jnp.ndarray,
-    ) -> jnp.ndarray:
+        x: ArrayLike,
+    ) -> Array:
 
         orig_shape = x.shape
 
         x = x.reshape(-1, orig_shape[-1])
         x_backup = x
 
         x = jnp.stack([x.max(axis=0), x.mean(axis=0)])
@@ -37,16 +39,16 @@
 
 class SpatialAttention(nn.Module):
     filter_size: int = 7
 
     @nn.compact
     def __call__(
         self,
-        x: jnp.ndarray,
-    ) -> jnp.ndarray:
+        x: ArrayLike,
+    ) -> Array:
 
         y = jnp.stack([x.max(axis=-1), x.mean(axis=-1)], axis=-1)
         y = nn.Conv(1, [self.filter_size, self.filter_size])(y)
         y = jax.nn.sigmoid(y)
 
         y = x * y
 
@@ -55,15 +57,17 @@
 
 class DropPath(nn.Module):
     """Drop paths (Stochastic Depth) per sample (when applied in main path of residual blocks)."""
 
     rate: float
 
     @nn.module.compact
-    def __call__(self, inputs, deterministic: tp.Optional[bool] = True):
+    def __call__(
+        self, inputs: ArrayLike, deterministic: Optional[bool] = True
+    ) -> Array:
         if self.rate == 0.0:
             return inputs
         keep_prob = 1.0 - self.rate
         if deterministic:
             return inputs
         else:
             rng = self.make_rng("droppath")
@@ -74,15 +78,15 @@
             return output
 
 
 class FPN(nn.Module):
     out_channels: int = 256
 
     @nn.compact
-    def __call__(self, inputs: tp.Sequence[jnp.ndarray]) -> tp.Sequence[jnp.ndarray]:
+    def __call__(self, inputs: Sequence[ArrayLike]) -> Sequence[Array]:
         out_channels = self.out_channels
 
         outputs = [jax.nn.relu(nn.Dense(out_channels)(x)) for x in inputs]
 
         for k in range(len(outputs) - 1, 0, -1):
             x = jax.image.resize(outputs[k], outputs[k - 1].shape, "nearest")
             x += outputs[k - 1]
```

### Comparing `lacss-0.4.1/lacss/modules/convnext.py` & `lacss-0.4.2/lacss/modules/convnext.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import List, Sequence, Union
 
 import flax.linen as nn
 import jax
 import jax.numpy as jnp
 
+from lacss.types import *
+
 from .common import *
 
 """ Implements the convnext encoder. Described in https://arxiv.org/abs/2201.03545
 Original implementation: https://github.com/facebookresearch/ConvNeXt
 """
 
 
@@ -19,15 +21,15 @@
     """
 
     drop_rate: int = 0.0
     layer_scale_init_value: float = 1e-6
     kernel_size: int = 7
 
     @nn.compact
-    def __call__(self, x: jnp.ndarray, *, training=None) -> jnp.ndarray:
+    def __call__(self, x: ArrayLike, *, training: Optional[bool] = None) -> Array:
         dim = x.shape[-1]
         ks = self.kernel_size
         scale = self.layer_scale_init_value
 
         shortcut = x
 
         x = nn.Conv(dim, (ks, ks), feature_group_count=dim)(x)
@@ -46,34 +48,64 @@
         x = DropPath(self.drop_rate)(x, deterministic=deterministic)
 
         x = x + shortcut
 
         return x
 
 
+# utility funcs
+
+_imagenet_weights_urls = {
+    "convnext_tiny_1k": "https://dl.fbaipublicfiles.com/convnext/convnext_tiny_1k_224_ema.pth",
+    "convnext_small_1k": "https://dl.fbaipublicfiles.com/convnext/convnext_small_1k_224_ema.pth",
+    "convnext_base_1k": "https://dl.fbaipublicfiles.com/convnext/convnext_base_1k_224_ema.pth",
+    "convnext_large_1k": "https://dl.fbaipublicfiles.com/convnext/convnext_large_1k_224_ema.pth",
+    "convnext_tiny_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_tiny_22k_224.pth",
+    "convnext_small_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_small_22k_224.pth",
+    "convnext_base_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_base_22k_224.pth",
+    "convnext_large_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_large_22k_224.pth",
+    "convnext_xlarge_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_xlarge_22k_224.pth",
+}
+
+
 class ConvNeXt(nn.Module):
-    """ConvNeXt
-    Args:
-        patch_size: for stem default 4
-        depths (tuple(int)): Number of blocks at each stage. Default: [3, 3, 9, 3]
-        dims (int): Feature dimension at each stage. Default: [96, 192, 384, 768]
-        drop_path_rate (float): Stochastic depth rate. Default: 0.
-        layer_scale_init_value (float): Init value for Layer Scale. Default: 1e-6.
-        out_channels (int): FPN output channels. Default: 256
+    """ConvNeXt CNN backbone
+
+    Attributes:
+        patch_size: Stem patch size
+        depths: Number of blocks at each stage.
+        dims: Feature dimension at each stage.
+        drop_path_rate: Stochastic depth rate.
+        layer_scale_init_value: Init value for Layer Scale.
+        out_channels:
+            FPN output channels. Setting this to -1 disable the FPN, in which case
+            the model output only encoder outputs.
     """
 
     patch_size: int = 4
     depths: Sequence[int] = (3, 3, 27, 3)
     dims: Sequence[int] = (96, 192, 384, 768)
     drop_path_rate: float = 0.0
     layer_scale_init_value: float = 1e-6
     out_channels: int = 384
 
     @nn.compact
-    def __call__(self, x: jnp.ndarray, *, training: bool = None) -> jnp.ndarray:
+    def __call__(
+        self, x: ArrayLike, *, training: Optional[bool] = None
+    ) -> Tuple[DataDict, DataDict]:
+        """
+        Args:
+            x: Image input.
+            training: Whether run the network in training mode (i.e. with stochastic depth)
+
+        Returns:
+            A tuple of (encoder_outputs, decoder_outputs). Both are dictionaries mapping
+                feature scale (e.g. "2") to features. If out_channels is -1, the decoder_output
+                is None.
+        """
         dp_rate = 0
         outputs = []
         for k in range(len(self.depths)):
             if k == 0:
                 ps = self.patch_size
                 x = nn.Conv(self.dims[k], (ps, ps), strides=(ps, ps))(x)
                 x = nn.LayerNorm(epsilon=1e-6)(x)
@@ -94,86 +126,91 @@
             decoder_out = FPN(self.out_channels)(outputs)
             decoder_out = dict(zip(keys, decoder_out))
         else:
             decoder_out = None
 
         return encoder_out, decoder_out
 
-
-# utility funcs
-
-model_urls = {
-    "convnext_tiny_1k": "https://dl.fbaipublicfiles.com/convnext/convnext_tiny_1k_224_ema.pth",
-    "convnext_small_1k": "https://dl.fbaipublicfiles.com/convnext/convnext_small_1k_224_ema.pth",
-    "convnext_base_1k": "https://dl.fbaipublicfiles.com/convnext/convnext_base_1k_224_ema.pth",
-    "convnext_large_1k": "https://dl.fbaipublicfiles.com/convnext/convnext_large_1k_224_ema.pth",
-    "convnext_tiny_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_tiny_22k_224.pth",
-    "convnext_small_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_small_22k_224.pth",
-    "convnext_base_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_base_22k_224.pth",
-    "convnext_large_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_large_22k_224.pth",
-    "convnext_xlarge_22k": "https://dl.fbaipublicfiles.com/convnext/convnext_xlarge_22k_224.pth",
-}
-
-
-def load_weight(jax_model, jax_params, url):
-    """Load pretrained convnext models
-    specs for pretrained models are:
-        tiny: dims=(96, 192, 384, 768), depths=(3,3,9,3)
-        small: dims=(96, 192, 384, 768), depths=(3,3,27,3)
-        base: dims=(128, 256, 512, 1024), depths=(3,3,27,3)
-        large: dims=(192, 384, 768, 1536), depths=(3,3,27,3)
-        X-large: dims=(256, 512, 1024, 2048), depths=(3,3,27,3)
-    """
-    import torch
-    from flax.core.frozen_dict import freeze, unfreeze
-
-    def t(m, new_value):
-        new_value = jnp.array(new_value)
-        assert m.shape == new_value.shape
-        m = new_value
-
-    checkpoint = torch.hub.load_state_dict_from_url(url=url, map_location="cpu")
-    params = checkpoint["model"]
-    jax_params = unfreeze(jax_params)
-
-    cnt = 0
-    for i in range(4):
-        for k in range(jax_model.depths[i]):
-            block = jax_params[f"_Block_{cnt}"]
-            t(block["gamma"], params[f"stages.{i}.{k}.gamma"])
-            t(block["Conv_0"]["bias"], params[f"stages.{i}.{k}.dwconv.bias"])
+    def _load_weight(self, jax_params, url):
+        import torch
+        from flax.core.frozen_dict import freeze, unfreeze
+
+        def t(m, new_value):
+            new_value = jnp.array(new_value)
+            assert m.shape == new_value.shape
+            m = new_value
+
+        checkpoint = torch.hub.load_state_dict_from_url(url=url, map_location="cpu")
+        params = checkpoint["model"]
+        jax_params = unfreeze(jax_params)
+
+        cnt = 0
+        for i in range(4):
+            for k in range(self.depths[i]):
+                block = jax_params[f"_Block_{cnt}"]
+                t(block["gamma"], params[f"stages.{i}.{k}.gamma"])
+                t(block["Conv_0"]["bias"], params[f"stages.{i}.{k}.dwconv.bias"])
+                t(
+                    block["Conv_0"]["kernel"],
+                    params[f"stages.{i}.{k}.dwconv.weight"].permute(2, 3, 1, 0),
+                )
+                t(block["LayerNorm_0"]["bias"], params[f"stages.{i}.{k}.norm.bias"])
+                t(block["LayerNorm_0"]["scale"], params[f"stages.{i}.{k}.norm.weight"])
+                t(block["Dense_0"]["bias"], params[f"stages.{i}.{k}.pwconv1.bias"])
+                t(
+                    block["Dense_0"]["kernel"],
+                    params[f"stages.{i}.{k}.pwconv1.weight"].transpose(0, 1),
+                )
+                t(block["Dense_1"]["bias"], params[f"stages.{i}.{k}.pwconv2.bias"])
+                t(
+                    block["Dense_1"]["kernel"],
+                    params[f"stages.{i}.{k}.pwconv2.weight"].transpose(0, 1),
+                )
+
+                cnt += 1
+
+        norm = jax_params[f"LayerNorm_0"]
+        t(norm["bias"], params["downsample_layers.0.1.bias"])
+        t(norm["scale"], params["downsample_layers.0.1.weight"])
+
+        conv = jax_params[f"Conv_0"]
+        t(conv["bias"], params["downsample_layers.0.0.bias"])
+        t(conv["kernel"], params["downsample_layers.0.0.weight"].permute(2, 3, 1, 0))
+
+        for i in range(1, 4):
+            norm = jax_params[f"LayerNorm_{i}"]
+            t(norm["bias"], params[f"downsample_layers.{i}.0.bias"])
+            t(norm["scale"], params[f"downsample_layers.{i}.0.weight"])
+            conv = jax_params[f"Conv_{i}"]
+            t(conv["bias"], params[f"downsample_layers.{i}.1.bias"])
             t(
-                block["Conv_0"]["kernel"],
-                params[f"stages.{i}.{k}.dwconv.weight"].permute(2, 3, 1, 0),
-            )
-            t(block["LayerNorm_0"]["bias"], params[f"stages.{i}.{k}.norm.bias"])
-            t(block["LayerNorm_0"]["scale"], params[f"stages.{i}.{k}.norm.weight"])
-            t(block["Dense_0"]["bias"], params[f"stages.{i}.{k}.pwconv1.bias"])
-            t(
-                block["Dense_0"]["kernel"],
-                params[f"stages.{i}.{k}.pwconv1.weight"].transpose(0, 1),
-            )
-            t(block["Dense_1"]["bias"], params[f"stages.{i}.{k}.pwconv2.bias"])
-            t(
-                block["Dense_1"]["kernel"],
-                params[f"stages.{i}.{k}.pwconv2.weight"].transpose(0, 1),
+                conv["kernel"],
+                params[f"downsample_layers.{i}.1.weight"].permute(2, 3, 1, 0),
             )
 
-            cnt += 1
+        return freeze(jax_params)
+
+    def get_imagenet_weights(self, model_type: str) -> Params:
+        """Get imagenet weights
 
-    norm = jax_params[f"LayerNorm_0"]
-    t(norm["bias"], params["downsample_layers.0.1.bias"])
-    t(norm["scale"], params["downsample_layers.0.1.weight"])
-
-    conv = jax_params[f"Conv_0"]
-    t(conv["bias"], params["downsample_layers.0.0.bias"])
-    t(conv["kernel"], params["downsample_layers.0.0.weight"].permute(2, 3, 1, 0))
-
-    for i in range(1, 4):
-        norm = jax_params[f"LayerNorm_{i}"]
-        t(norm["bias"], params[f"downsample_layers.{i}.0.bias"])
-        t(norm["scale"], params[f"downsample_layers.{i}.0.weight"])
-        conv = jax_params[f"Conv_{i}"]
-        t(conv["bias"], params[f"downsample_layers.{i}.1.bias"])
-        t(conv["kernel"], params[f"downsample_layers.{i}.1.weight"].permute(2, 3, 1, 0))
+        Args:
+            model_type: The expected model specification. This must match the current
+                instance attributes.
+
+                * tiny: dims=(96, 192, 384, 768), depths=(3,3,9,3)
+                * small: dims=(96, 192, 384, 768), depths=(3,3,27,3)
+                * base: dims=(128, 256, 512, 1024), depths=(3,3,27,3)
+                * large: dims=(192, 384, 768, 1536), depths=(3,3,27,3)
+                * X-large: dims=(256, 512, 1024, 2048), depths=(3,3,27,3)
+
+        Returns:
+            A frozen dict representing weights of the current module
+        """
+
+        init_params = self.init(jax.random.PRNGKey(0), jnp.zeros([64, 64, 3]))
+        init_params = init_params["params"]
+        params = self._load_weight(
+            init_params,
+            _imagenet_weights_urls[f"convnext_{model_type}_22k"],
+        )
 
-    return freeze(jax_params)
+        return params
```

### Comparing `lacss-0.4.1/lacss/modules/detector.py` & `lacss-0.4.2/lacss/modules/detector.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,37 @@
 from functools import partial
 from typing import List, Optional, Sequence, Tuple, Union
 
 import flax.linen as nn
 import jax
 import jax.numpy as jnp
 
-from ..ops import location_matching, sorted_non_max_suppression
+from lacss.ops import location_matching, sorted_non_max_suppression
+from lacss.types import *
 
 
 class Detector(nn.Module):
-    """A weightless layer that conver LPN output to a list of locations"""
+    """A weightless module that conver LPN output to a list of locations. Non-max-supression is
+        appplied to remove redundant detections.
+
+    Attributes:
+
+        train_nms_threshold: Threshold for non-max-suppression during training
+        train_pre_nms_topk: If > 0, only the top_k scored locations will be analyzed during training
+        train_max_output: Maximum number of outputs during training
+        train_min_score: Mininum scores to be considered during training
+        max_proposal_offset: During training, if a detected location is with in this distance threshold
+            of a ground-truth location, replacing the ground truth location with the detection one for
+            segmentation purpose.
+        test_nms_threshold: Threshold for non-max-suppression during testing
+        test_pre_nms_topk: If > 0, only the top_k scored locations will be analyzed during testing
+        test_max_output: Maximum number of outputs during testing
+        test_min_score: Mininum scores to be considered during testing
+
+    """
 
     train_nms_threshold: float = 8.0
     train_pre_nms_topk: int = -1
     train_max_output: int = 768
     train_min_score: float = 0.2
     max_proposal_offset: float = 12
     test_nms_threshold: float = 8.0
@@ -136,33 +154,36 @@
             ],  # out-of-bound error silently dropped in jax
         )
 
         return training_locations
 
     def __call__(
         self,
-        scores: jnp.ndarray,
-        regressions: jnp.ndarray,
-        gt_locations: jnp.ndarray = None,
+        scores: Mapping[str, ArrayLike],
+        regressions: Mapping[str, ArrayLike],
+        gt_locations: Optional[ArrayLike] = None,
         *,
-        training: bool = None,
-    ) -> Tuple[jnp.ndarray, jnp.ndarray]:
+        training: Optional[bool] = None,
+    ) -> DataDict:
         """
         Args:
-            score: {'lvl', [H, W, 1]) output from LPN
-            regression: ('lvl': [H, W, 2]) output from LPN
-            gt_locations: [N, 2] during training or None during inference. Maybe padded with -1
-        Outputs:
-            dict {
-                training_locations: [N, 2] only during training
-                pred_locations: [M, 2] sorted based on scores; M == test_max_output; padded with -1
-                pred_scores: [M] sorted, padded with -1
-            }
-        """
+                scores: {'scale', [H, W, 1]) output from LPN
+                regressions: {'scale': [H, W, 2]} output from LPN
+                gt_locations: Ground-truth call locations. This can be an array  of [N, 2] (training) or
+                    None (inference). Maybe padded with -1
+                training: Whether to run the module in training mode or not
 
+        Returns:
+                a dictionary of values.
+
+                    * pred_locations: Sorted array based on scores
+                    * pred_scores: Sorted array, padded with -1
+                    * training_locations: This value exists during training only.
+
+        """
         scores = jax.lax.stop_gradient(scores)
         regressions = jax.lax.stop_gradient(regressions)
 
         if training:
 
             if self.max_proposal_offset <= 0:
                 return dict(
```

### Comparing `lacss-0.4.1/lacss/modules/lacss.py` & `lacss-0.4.2/lacss/modules/lacss.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,72 @@
-import typing as tp
 from dataclasses import asdict, field
-from functools import partial
 
 import flax.linen as nn
-import jax
 import jax.numpy as jnp
 
-from ..ops import *
-from .auxiliary import *
+from lacss.ops import *
+from lacss.utils import dataclass_from_dict
+
 from .convnext import ConvNeXt
 from .detector import Detector
 from .lpn import LPN
-from .resnet import ResNet
 from .segmentor import Segmentor
 
 
 class Lacss(nn.Module):
-    backbone: nn.Module = ConvNeXt()
-    lpn: nn.Module = LPN()
-    detector: nn.Module = Detector()
-    segmentor: nn.Module = Segmentor()
+    """Main class for LACSS model
+
+    Attributes:
+        backbone: The ConvNeXt backbone
+        lpn: The LPN head for detecting cell location
+        detector: A weight-less module interpreting lpn output
+        segmentor: The segmentation head
+
+    """
+
+    backbone: ConvNeXt = field(default_factory=ConvNeXt)
+    lpn: LPN = field(default_factory=LPN)
+    detector: Detector = field(default_factory=Detector)
+    segmentor: Segmentor = field(default_factory=Segmentor)
 
     @classmethod
-    def from_config(cls, config):
-        config_dict = {}
-        if "backbone" in config:
-            config_dict["backbone"] = ConvNeXt(**config["backbone"])
-        if "lpn" in config:
-            config_dict["lpn"] = LPN(**config["lpn"])
-        if "detector" in config:
-            config_dict["detector"] = Detector(**config["detector"])
-        if "segmentor" in config:
-            config_dict["segmentor"] = Segmentor(**config["segmentor"])
+    def from_config(cls, config: dict):
+        """Factory method to build an Lacss instance from a configuration dictionary
+
+        Args:
+            config: A configuration dictionary.
+
+        Returns:
+            An Lacss instance.
 
-        return cls(**config_dict)
+        """
+        return dataclass_from_dict(cls, config)
+
+    def get_config(self) -> dict:
+        """Convert to a configuration dict. Can be serialized with json
+
+        Returns:
+            config: a configuration dict
+        """
+        return asdict(self)
 
     def __call__(
         self,
         image: jnp.ndarray,
         gt_locations: jnp.ndarray = None,
         *,
         training: bool = None,
     ) -> dict:
         """
         Args:
             image: [H, W, C]
             gt_locations: [M, 2] if training, otherwise None
         Returns:
             a dict of model outputs
+
         """
         orig_height, orig_width, ch = image.shape
         if ch == 1:
             image = jnp.repeat(image, 3, axis=-1)
         elif ch == 2:
             image = jnp.concatenate([image, jnp.zeros_like(image[..., :1])], axis=-1)
 
@@ -104,36 +119,7 @@
                 self.segmentor(
                     features=features,
                     locations=scaled_locs,
                 )
             )
 
         return model_output
-
-
-class LacssWithHelper(nn.Module):
-    cfg: dict = field(default_factory=dict)
-    aux_edge_cfg: tp.Optional[dict] = None
-    aux_fg_cfg: tp.Optional[dict] = None
-
-    def setup(self):
-        self._lacss = Lacss.from_config(self.cfg)
-        if self.aux_edge_cfg is not None:
-            self._aux_edge_module = AuxInstanceEdge(**self.aux_edge_cfg)
-        if self.aux_fg_cfg is not None:
-            self._aux_fg_module = AuxForeground(**self.aux_fg_cfg)
-
-    def __call__(self, image, gt_locations=None, category=None, *, training=False):
-
-        preds = self._lacss(image, gt_locations, training=training)
-
-        if self.aux_edge_cfg is not None:
-
-            preds.update(self._aux_edge_module(image, category=category))
-
-        if self.aux_fg_cfg is not None:
-
-            preds.update(
-                self._aux_fg_module(image, category=category)
-            )
-
-        return preds
```

### Comparing `lacss-0.4.1/lacss/modules/lpn.py` & `lacss-0.4.2/lacss/modules/lpn.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-import typing as tp
-from functools import partial
+from __future__ import annotations
+
+from typing import Mapping, Sequence, Tuple
 
 import flax.linen as nn
 import jax
 import jax.numpy as jnp
 
-from ..ops import locations_to_labels
-from .common import ChannelAttention
-
-# from typing import List, Optional, Sequence, Tuple, Union
+from lacss.ops import locations_to_labels
+from lacss.types import *
 
 
 class LPN(nn.Module):
-    """
-    Args:
-    in_channels: number of channels in input feature
-    feature_level: input feature level default 3
-    conv_layers: conv layer spec
-    with_channel_attention: whether include channel attention
+    """Location detection head
+
+    Attributes:
+
+        feature_levels: Input feature level, e.g. [2, 3, 4]
+        conv_spec: Conv layer specification
+        detection_roi: Parameter for label smoothing
+
     """
 
-    feature_levels: tp.Sequence[int] = (4, 3, 2)
-    conv_spec: tp.Tuple[tp.Sequence[int], tp.Sequence[int]] = ((384, 384, 384, 384), ())
+    feature_levels: Sequence[int] = (4, 3, 2)
+    conv_spec: Tuple[Sequence[int], Sequence[int]] = ((384, 384, 384, 384), ())
     detection_roi: float = 8.0
 
     @nn.compact
     def _process_feature(
-        self, feature: jnp.ndarray
-    ) -> tp.Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray]:
+        self, feature: ArrayLike
+    ) -> Tuple[ArrayLike, ArrayLike, ArrayLike]:
         conv_spec = self.conv_spec
 
         x = feature
 
         for n_ch in conv_spec[0]:
             x = nn.Conv(n_ch, (3, 3), use_bias=False)(x)
             x = nn.GroupNorm(num_groups=n_ch)(x[None, ...])[0]
@@ -47,31 +48,31 @@
 
         regression_out = nn.Conv(2, (1, 1))(x)
 
         return scores_out, regression_out, x
 
     def __call__(
         self,
-        inputs: dict,
-        scaled_gt_locations: jnp.ndarray = None,
+        inputs: Mapping[str, ArrayLike],
+        scaled_gt_locations: Optional[ArrayLike] = None,
     ) -> dict:
         """
         Args:
             inputs: feature dict: {'lvl': [H, W, C]}
             scaled_gt_locations: scaled 0..1 [N, 2], only valid in training
+
         Returns:
-            outputs:
-            {
-                lpn_scores: dict: {'lvl': [H, W, 1]}
-                lpn_regressions: dict {'lvl': [H, W, 2]}
-                gt_lpn_scores: dict {'lvl': [H, W, 1]}, only if training
-                gt_lpn_regressions: dict {'lvl': [H, W, 2]}, only if training
-            }
-        """
+            A dict of features
 
+                * lpn_scores: dict: {'lvl': [H, W, 1]}
+                * lpn_regressions: dict {'lvl': [H, W, 2]}
+                * gt_lpn_scores: dict {'lvl': [H, W, 1]}, only if training
+                * gt_lpn_regressions: dict {'lvl': [H, W, 2]}, only if training
+
+        """
         all_scores = dict()
         all_regrs = dict()
         all_features = dict()
 
         for lvl in self.feature_levels:
 
             feature = inputs[str(lvl)]
```

### Comparing `lacss-0.4.1/lacss/modules/resnet.py` & `lacss-0.4.2/lacss/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/modules/segmentor.py` & `lacss-0.4.2/lacss/modules/segmentor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import math
-import typing as tp
 from functools import partial
 
 import flax.linen as nn
 import jax
 import jax.numpy as jnp
 
-from ..ops import gather_patches
+from lacss.ops import gather_patches
+from lacss.types import *
+
 from .common import SpatialAttention
 
 
 class _Encoder(nn.Module):
     n_output_features: int
     input_patch_size: int
-    encoding_dims: tp.Tuple[int, int, int] = (8, 8, 4)
+    encoding_dims: Tuple[int, int, int] = (8, 8, 4)
     n_latent_features: int = -1
 
     @nn.compact
-    def __call__(self, feature, loc):
+    def __call__(self, feature: ArrayLike, loc: ArrayLike) -> Array:
         patch_center, _, _, _ = gather_patches(feature, loc, patch_size=2)
         encodings = patch_center.mean(axis=(-2, -3))
 
         dim = self.n_latent_features
         dim = dim if dim > 0 else math.prod(self.encoding_dims)
         encodings = nn.Dense(dim)(encodings)
         encodings = jax.nn.relu(encodings)
@@ -44,50 +45,56 @@
 
         encodings = nn.Conv(self.n_output_features, (1, 1), use_bias=False)(encodings)
 
         return encodings
 
 
 class Segmentor(nn.Module):
-    """LACSS segmentor module.
+    """LACSS segmentation head.
 
     Attributes:
-        feature_level: int
+        feature_level: The scale of the feature used for segmentation
         conv_spec: conv_block definition, e.g. ((384,384,384), (64,))
-        instance_crop_size: Crop size. default is 96.
-        with_attention: Whether use spatial attention layer. Default is False
-        learned_encoding: Whether to use hard-coded position encoding. Default is False
+        instance_crop_size: Crop size for segmentation.
+        with_attention: Whether use spatial attention layer.
+        learned_encoding: Whether to use hard-coded position encoding.
         encoder_dims: Dim of the position encoder, if using learned encoding. Default is (8,8,4)
+
     """
 
     feature_level: int = 2
-    conv_spec: tp.Tuple[tp.Sequence[int], tp.Sequence[int]] = (
+    conv_spec: Tuple[Sequence[int], Sequence[int]] = (
         (384, 384, 384),
         (64,),
     )
     instance_crop_size: int = 96
     use_attention: bool = False
     learned_encoding: bool = True
-    encoder_dims: tp.Sequence[int] = (8, 8, 4)
+    encoder_dims: Sequence[int] = (8, 8, 4)
     # n_cls: int = -1
 
     # if not feature_level in (0,1,2):
     #     raise ValueError('feature_level should be 1,2 or 0')
 
     @nn.compact
-    def __call__(self, features: dict, locations: jnp.ndarray) -> dict:
+    def __call__(
+        self, features: Mapping[str, ArrayLike], locations: ArrayLike
+    ) -> DataDict:
         """
         Args:
-            features: {'lvl' [H, W, C]} feature dictionary
-            locations: [N, 2]  scaled 0..1
-        outputs:
-            instance_output: [N, crop_size, crop_size]
-            instance_mask; [N, 1, 1] boolean mask indicating valid outputs
-            instance_yc: [N, crop_size, crop_size] meshgrid y coordinates
-            instance_xc: [N, crop_size, crop_size] meshgrid x coordinates
+            features: {'scale' [H, W, C]} feature dictionary from the backbone.
+            locations: [N, 2]  normalized to image size.
+
+        Returns:
+            A dictionary of values representing segmentation outputs.
+
+                * instance_output: [N, crop_size, crop_size]
+                * instance_mask; [N, 1, 1] boolean mask indicating valid outputs
+                * instance_yc: [N, crop_size, crop_size] meshgrid y coordinates
+                * instance_xc: [N, crop_size, crop_size] meshgrid x coordinates
         """
         crop_size = self.instance_crop_size
         lvl = self.feature_level
         scale = 2**lvl
         conv_spec = self.conv_spec
         patch_size = crop_size // scale
```

### Comparing `lacss-0.4.1/lacss/modules/unet.py` & `lacss-0.4.2/lacss/modules/unet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-import typing as tp
+from __future__ import annotations
 
 import flax.linen as nn
 import jax
 import jax.numpy as jnp
 
+from lacss.types import *
+
 from .common import *
 
 
 class UNet(nn.Module):
-    model_spec: tp.Sequence[int] = (32, 64, 128, 256, 512)
+    model_spec: Sequence[int] = (32, 64, 128, 256, 512)
     patch_size: int = 1
     se_ratio: int = -1
 
     def __post_init__(self):
         super().__post_init__()
         if not self.patch_size in [1, 2, 4]:
             raise ValueError("patch_size must be eith 1, 2 or 4")
 
     @nn.compact
-    def __call__(self, x: jnp.ndarray, *, training: bool = None) -> dict:
+    def __call__(self, x: ArrayLike) -> Tuple[DataDict, DataDict]:
 
         encoder_out = []
         fs = max(self.patch_size, 3)
         st = self.patch_size
 
         for ch in self.model_spec:
 
@@ -61,14 +63,14 @@
 
         encoder_out = dict(zip(keys, encoder_out))
         decoder_out = dict(zip(keys, decoder_out))
 
         return encoder_out, decoder_out
 
     @property
-    def start_level(self):
+    def start_level(self) -> int:
         if self.patch_size == 4:
             return 2
         elif self.patch_size == 2:
             return 1
         else:
             return 0
```

### Comparing `lacss-0.4.1/lacss/ops/__pycache__/boxes.cpython-38.pyc` & `lacss-0.4.2/lacss/ops/__pycache__/boxes.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 19:35:53 2023 UTC, .py size: 2321 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,134 +1,141 @@
-00000000: 550d 0d0a 0000 0000 99e8 9964 1109 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 e37d ad64 8a09 0000  U........}.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
+00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 6d03 5a04 0100 6401 6402 6c03 5a05 6403  m.Z...d.d.l.Z.d.
-00000050: 6404 8400 5a06 6405 6406 8400 5a07 6407  d...Z.d.d...Z.d.
-00000060: 6408 8400 5a08 6402 5300 2909 7a8a 204f  d...Z.d.S.).z. O
-00000070: 7073 206f 6e20 626f 756e 6469 6e67 2d62  ps on bounding-b
-00000080: 6f78 6573 0a0a 416c 6c20 6675 6e63 7469  oxes..All functi
-00000090: 6f6e 7320 6865 7265 2061 7265 2064 6567  ons here are deg
-000000a0: 6973 6e65 6420 746f 2077 6f72 6b20 6173  isned to work as
-000000b0: 2065 6974 6865 7220 6120 6e75 6d70 7920   either a numpy 
-000000c0: 6f70 206f 7220 6120 6a61 7820 6f70 2064  op or a jax op d
-000000d0: 6570 656e 6469 6e67 206f 6e0a 7468 6520  epending on.the 
-000000e0: 6461 7461 2074 7970 6520 6f66 2074 6865  data type of the
-000000f0: 2069 6e70 7574 2e0a e900 0000 004e 6301   input.......Nc.
-00000100: 0000 0000 0000 0000 0000 0006 0000 0005  ................
-00000110: 0000 0043 0000 0073 4800 0000 7400 7c00  ...C...sH...t.|.
-00000120: 7401 6a02 8302 7214 7401 6a03 7d01 6e06  t.j...r.t.j.}.n.
-00000130: 7404 6a03 7d01 7c01 7c00 6401 6402 6403  t.j.}.|.|.d.d.d.
-00000140: 8d03 5c04 7d02 7d03 7d04 7d05 7c04 7c02  ..\.}.}.}.}.|.|.
-00000150: 1800 7c05 7c03 1800 1400 6a05 6402 6403  ..|.|.....j.d.d.
-00000160: 8d01 5300 2904 7a83 436f 6d70 7574 6573  ..S.).z.Computes
-00000170: 2061 7265 6120 6f66 2062 6f78 6573 2e0a   area of boxes..
-00000180: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00000190: 626f 783a 2061 2066 6c6f 6174 2054 656e  box: a float Ten
-000001a0: 736f 7220 7769 7468 205b 2e2e 2e2c 204e  sor with [..., N
-000001b0: 2c20 345d 2e0a 0a20 2020 2052 6574 7572  , 4]...    Retur
-000001c0: 6e73 3a0a 2020 2020 2020 6120 666c 6f61  ns:.      a floa
-000001d0: 7420 5465 6e73 6f72 2077 6974 6820 5b2e  t Tensor with [.
-000001e0: 2e2e 2c20 4e5d 0a20 2020 20e9 0400 0000  .., N].    .....
-000001f0: e9ff ffff ffa9 01da 0461 7869 7329 06da  .........axis)..
-00000200: 0a69 7369 6e73 7461 6e63 65da 036a 6e70  .isinstance..jnp
-00000210: da07 6e64 6172 7261 79da 0573 706c 6974  ..ndarray..split
-00000220: da02 6e70 da07 7371 7565 657a 6529 06da  ..np..squeeze)..
-00000230: 0362 6f78 7209 0000 00da 0579 5f6d 696e  .boxr......y_min
-00000240: da05 785f 6d69 6eda 0579 5f6d 6178 da05  ..x_min..y_max..
-00000250: 785f 6d61 78a9 0072 1100 0000 fa32 2f68  x_max..r.....2/h
-00000260: 6f6d 652f 4643 414d 2f6a 7975 2f70 726f  ome/FCAM/jyu/pro
-00000270: 6a5f 6c61 6373 732f 6c61 6373 732f 6c61  j_lacss/lacss/la
-00000280: 6373 732f 6f70 732f 626f 7865 732e 7079  css/ops/boxes.py
-00000290: da08 626f 785f 6172 6561 0c00 0000 730a  ..box_area....s.
-000002a0: 0000 0000 080c 0108 0206 0216 0172 1300  .............r..
-000002b0: 0000 6302 0000 0000 0000 0000 0000 0013  ..c.............
-000002c0: 0000 0006 0000 0043 0000 0073 de00 0000  .......C...s....
-000002d0: 7400 7c00 7401 6a02 8302 7400 7c01 7401  t.|.t.j...t.|.t.
-000002e0: 6a02 8302 4000 722c 7401 6a03 7d02 7401  j...@.r,t.j.}.t.
-000002f0: 6a04 7d03 7401 6a05 7d04 6e12 7406 6a03  j.}.t.j.}.n.t.j.
-00000300: 7d02 7406 6a04 7d03 7406 6a05 7d04 7c02  }.t.j.}.t.j.}.|.
-00000310: 7c00 6401 6402 6403 8d03 5c04 7d05 7d06  |.d.d.d...\.}.}.
-00000320: 7d07 7d08 7c02 7c01 6401 6402 6403 8d03  }.}.|.|.d.d.d...
-00000330: 5c04 7d09 7d0a 7d0b 7d0c 7c03 7c07 7c0b  \.}.}.}.}.|.|.|.
-00000340: a007 6402 6404 a102 8302 7d0d 7c04 7c05  ..d.d.....}.|.|.
-00000350: 7c09 a007 6402 6404 a102 8302 7d0e 7c03  |...d.d.....}.|.
-00000360: 7c08 7c0c a007 6402 6404 a102 8302 7d0f  |.|...d.d.....}.
-00000370: 7c04 7c06 7c0a a007 6402 6404 a102 8302  |.|.|...d.d.....
-00000380: 7d10 7c0d 7c0e 1800 7d11 7c0f 7c10 1800  }.|.|...}.|.|...
-00000390: 7d12 7c04 6405 7c11 8302 7d11 7c04 6405  }.|.d.|...}.|.d.
-000003a0: 7c12 8302 7d12 7c11 7c12 1400 5300 2906  |...}.|.|...S.).
-000003b0: 7ad6 436f 6d70 7574 6520 7061 6972 7769  z.Compute pairwi
-000003c0: 7365 2069 6e74 6572 7365 6374 696f 6e20  se intersection 
-000003d0: 6172 6561 7320 6265 7477 6565 6e20 626f  areas between bo
-000003e0: 7865 732e 0a0a 2020 2020 4172 6773 3a0a  xes...    Args:.
-000003f0: 2020 2020 2020 6774 5f62 6f78 6573 3a20        gt_boxes: 
-00000400: 5b2e 2e2e 2c20 4e2c 2034 5d0a 2020 2020  [..., N, 4].    
-00000410: 2020 626f 7865 733a 205b 2e2e 2e2c 204d    boxes: [..., M
-00000420: 2c20 345d 0a0a 2020 2020 5265 7475 726e  , 4]..    Return
-00000430: 733a 0a20 2020 2020 2061 2066 6c6f 6174  s:.      a float
-00000440: 2054 656e 736f 7220 7769 7468 2073 6861   Tensor with sha
-00000450: 7065 205b 2e2e 2e2c 204e 2c20 4d5d 2072  pe [..., N, M] r
-00000460: 6570 7265 7365 6e74 696e 6720 7061 6972  epresenting pair
-00000470: 7769 7365 2069 6e74 6572 7365 6374 696f  wise intersectio
-00000480: 6e73 2e0a 2020 2020 7202 0000 0072 0300  ns..    r....r..
-00000490: 0000 7204 0000 00e9 feff ffff 7201 0000  ..r.........r...
-000004a0: 0029 0872 0600 0000 7207 0000 0072 0800  .).r....r....r..
-000004b0: 0000 7209 0000 00da 076d 696e 696d 756d  ..r......minimum
-000004c0: da07 6d61 7869 6d75 6d72 0a00 0000 da08  ..maximumr......
-000004d0: 7377 6170 6178 6573 2913 da08 6774 5f62  swapaxes)...gt_b
-000004e0: 6f78 6573 da05 626f 7865 7372 0900 0000  oxes..boxesr....
-000004f0: 7215 0000 0072 1600 0000 5a06 795f 6d69  r....r....Z.y_mi
-00000500: 6e31 5a06 785f 6d69 6e31 5a06 795f 6d61  n1Z.x_min1Z.y_ma
-00000510: 7831 5a06 785f 6d61 7831 5a06 795f 6d69  x1Z.x_max1Z.y_mi
-00000520: 6e32 5a06 785f 6d69 6e32 5a06 795f 6d61  n2Z.x_min2Z.y_ma
-00000530: 7832 5a06 785f 6d61 7832 5a09 795f 6d69  x2Z.x_max2Z.y_mi
-00000540: 6e5f 6d61 785a 0979 5f6d 6178 5f6d 696e  n_maxZ.y_max_min
-00000550: 5a09 785f 6d69 6e5f 6d61 785a 0978 5f6d  Z.x_min_maxZ.x_m
-00000560: 6178 5f6d 696e 5a11 696e 7465 7273 6563  ax_minZ.intersec
-00000570: 745f 6865 6967 6874 735a 1069 6e74 6572  t_heightsZ.inter
-00000580: 7365 6374 5f77 6964 7468 7372 1100 0000  sect_widthsr....
-00000590: 7211 0000 0072 1200 0000 da10 626f 785f  r....r......box_
-000005a0: 696e 7465 7273 6563 7469 6f6e 1d00 0000  intersection....
-000005b0: 7324 0000 0000 0a18 0106 0106 0108 0206  s$..............
-000005c0: 0106 0106 0216 0116 0312 0112 0112 0112  ................
-000005d0: 0208 0108 010a 010a 0272 1a00 0000 6302  .........r....c.
-000005e0: 0000 0000 0000 0000 0000 0007 0000 0006  ................
-000005f0: 0000 0043 0000 0073 4800 0000 7400 7c00  ...C...sH...t.|.
-00000600: 7c01 8302 7d02 7401 7c00 8301 7d03 7401  |...}.t.|...}.t.
-00000610: 7c01 8301 7d04 7c03 6401 1900 7c04 6402  |...}.|.d...|.d.
-00000620: 6403 6403 6403 8502 6603 1900 1700 7c02  d.d.d...f.....|.
-00000630: 1800 7d05 7c02 7c05 6404 1700 1b00 7d06  ..}.|.|.d.....}.
-00000640: 7c06 5300 2905 6107 0100 0043 6f6d 7075  |.S.).a....Compu
-00000650: 7465 7320 7061 6972 7769 7365 2069 6e74  tes pairwise int
-00000660: 6572 7365 6374 696f 6e2d 6f76 6572 2d75  ersection-over-u
-00000670: 6e69 6f6e 2062 6574 7765 656e 2062 6f78  nion between box
-00000680: 2063 6f6c 6c65 6374 696f 6e73 2e0a 0a20   collections... 
-00000690: 2020 2041 7267 733a 0a20 2020 2020 2067     Args:.      g
-000006a0: 745f 626f 7865 733a 2061 2066 6c6f 6174  t_boxes: a float
-000006b0: 2054 656e 736f 7220 7769 7468 205b 2e2e   Tensor with [..
-000006c0: 2e2c 204e 2c20 345d 2e0a 2020 2020 2020  ., N, 4]..      
-000006d0: 626f 7865 733a 2061 2066 6c6f 6174 2054  boxes: a float T
-000006e0: 656e 736f 7220 7769 7468 205b 2e2e 2e2c  ensor with [...,
-000006f0: 204d 2c20 345d 2e0a 0a20 2020 2052 6574   M, 4]...    Ret
-00000700: 7572 6e73 3a0a 2020 2020 2020 6120 5465  urns:.      a Te
-00000710: 6e73 6f72 2077 6974 6820 7368 6170 6520  nsor with shape 
-00000720: 5b2e 2e2e 2c20 4e2c 204d 5d20 7265 7072  [..., N, M] repr
-00000730: 6573 656e 7469 6e67 2070 6169 7277 6973  esenting pairwis
-00000740: 6520 696f 7520 7363 6f72 6573 2e0a 2020  e iou scores..  
-00000750: 2020 2902 2e4e 2e4e 678d edb5 a0f7 c6b0    )..N.Ng.......
-00000760: 3e29 0272 1a00 0000 7213 0000 0029 0772  >).r....r....).r
-00000770: 1800 0000 7219 0000 00da 0d69 6e74 6572  ....r......inter
-00000780: 7365 6374 696f 6e73 5a0e 6774 5f62 6f78  sectionsZ.gt_box
-00000790: 6573 5f61 7265 6173 5a0b 626f 7865 735f  es_areasZ.boxes_
-000007a0: 6172 6561 73da 0675 6e69 6f6e 735a 0469  areas..unionsZ.i
-000007b0: 6f75 7372 1100 0000 7211 0000 0072 1200  ousr....r....r..
-000007c0: 0000 da12 626f 785f 696f 755f 7369 6d69  ....box_iou_simi
-000007d0: 6c61 7269 7479 4100 0000 730c 0000 0000  larityA...s.....
-000007e0: 0a0a 0108 0108 011e 020c 0272 1d00 0000  ...........r....
-000007f0: 2909 da07 5f5f 646f 635f 5fda 036a 6178  )...__doc__..jax
-00000800: da09 6a61 782e 6e75 6d70 79da 056e 756d  ..jax.numpy..num
-00000810: 7079 7207 0000 0072 0a00 0000 7213 0000  pyr....r....r...
-00000820: 0072 1a00 0000 721d 0000 0072 1100 0000  .r....r....r....
-00000830: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00000840: 083c 6d6f 6475 6c65 3e01 0000 0073 0c00  .<module>....s..
-00000850: 0000 0406 0801 0c01 0803 0811 0824       .............$
+00000040: 6d03 5a04 0100 6401 6402 6c03 5a05 6401  m.Z...d.d.l.Z.d.
+00000050: 6403 6c06 5400 6507 6507 6404 9c02 6405  d.l.T.e.e.d...d.
+00000060: 6406 8404 5a08 6507 6507 6507 6407 9c03  d...Z.e.e.e.d...
+00000070: 6408 6409 8404 5a09 6507 6507 6507 6407  d.d...Z.e.e.e.d.
+00000080: 9c03 640a 640b 8404 5a0a 6402 5300 290c  ..d.d...Z.d.S.).
+00000090: 7a8a 204f 7073 206f 6e20 626f 756e 6469  z. Ops on boundi
+000000a0: 6e67 2d62 6f78 6573 0a0a 416c 6c20 6675  ng-boxes..All fu
+000000b0: 6e63 7469 6f6e 7320 6865 7265 2061 7265  nctions here are
+000000c0: 2064 6567 6973 6e65 6420 746f 2077 6f72   degisned to wor
+000000d0: 6b20 6173 2065 6974 6865 7220 6120 6e75  k as either a nu
+000000e0: 6d70 7920 6f70 206f 7220 6120 6a61 7820  mpy op or a jax 
+000000f0: 6f70 2064 6570 656e 6469 6e67 206f 6e0a  op depending on.
+00000100: 7468 6520 6461 7461 2074 7970 6520 6f66  the data type of
+00000110: 2074 6865 2069 6e70 7574 2e0a e900 0000   the input......
+00000120: 004e 2901 da01 2a29 02da 0362 6f78 da06  .N)...*)...box..
+00000130: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
+00000140: 0000 0006 0000 0005 0000 0043 0000 0073  ...........C...s
+00000150: 4800 0000 7400 7c00 7401 6a02 8302 7214  H...t.|.t.j...r.
+00000160: 7401 6a03 7d01 6e06 7404 6a03 7d01 7c01  t.j.}.n.t.j.}.|.
+00000170: 7c00 6401 6402 6403 8d03 5c04 7d02 7d03  |.d.d.d...\.}.}.
+00000180: 7d04 7d05 7c04 7c02 1800 7c05 7c03 1800  }.}.|.|...|.|...
+00000190: 1400 6a05 6402 6403 8d01 5300 2904 7a83  ..j.d.d...S.).z.
+000001a0: 436f 6d70 7574 6573 2061 7265 6120 6f66  Computes area of
+000001b0: 2062 6f78 6573 2e0a 2020 2020 4172 6773   boxes..    Args
+000001c0: 3a0a 2020 2020 2020 626f 783a 2061 2066  :.      box: a f
+000001d0: 6c6f 6174 2054 656e 736f 7220 7769 7468  loat Tensor with
+000001e0: 205b 2e2e 2e2c 204e 2c20 345d 2e0a 0a20   [..., N, 4]... 
+000001f0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00000200: 2020 6120 666c 6f61 7420 5465 6e73 6f72    a float Tensor
+00000210: 2077 6974 6820 5b2e 2e2e 2c20 4e5d 0a20   with [..., N]. 
+00000220: 2020 20e9 0400 0000 e9ff ffff ffa9 01da     .............
+00000230: 0461 7869 7329 06da 0a69 7369 6e73 7461  .axis)...isinsta
+00000240: 6e63 65da 036a 6e70 da07 6e64 6172 7261  nce..jnp..ndarra
+00000250: 79da 0573 706c 6974 da02 6e70 da07 7371  y..split..np..sq
+00000260: 7565 657a 6529 0672 0300 0000 720c 0000  ueeze).r....r...
+00000270: 00da 0579 5f6d 696e da05 785f 6d69 6eda  ...y_min..x_min.
+00000280: 0579 5f6d 6178 da05 785f 6d61 78a9 0072  .y_max..x_max..r
+00000290: 1300 0000 fa32 2f68 6f6d 652f 4643 414d  .....2/home/FCAM
+000002a0: 2f6a 7975 2f70 726f 6a5f 6c61 6373 732f  /jyu/proj_lacss/
+000002b0: 6c61 6373 732f 6c61 6373 732f 6f70 732f  lacss/lacss/ops/
+000002c0: 626f 7865 732e 7079 da08 626f 785f 6172  boxes.py..box_ar
+000002d0: 6561 0e00 0000 730a 0000 0000 080c 0108  ea....s.........
+000002e0: 0206 0216 0172 1500 0000 2903 da08 6774  .....r....)...gt
+000002f0: 5f62 6f78 6573 da05 626f 7865 7372 0400  _boxes..boxesr..
+00000300: 0000 6302 0000 0000 0000 0000 0000 0013  ..c.............
+00000310: 0000 0006 0000 0043 0000 0073 de00 0000  .......C...s....
+00000320: 7400 7c00 7401 6a02 8302 7400 7c01 7401  t.|.t.j...t.|.t.
+00000330: 6a02 8302 4000 722c 7401 6a03 7d02 7401  j...@.r,t.j.}.t.
+00000340: 6a04 7d03 7401 6a05 7d04 6e12 7406 6a03  j.}.t.j.}.n.t.j.
+00000350: 7d02 7406 6a04 7d03 7406 6a05 7d04 7c02  }.t.j.}.t.j.}.|.
+00000360: 7c00 6401 6402 6403 8d03 5c04 7d05 7d06  |.d.d.d...\.}.}.
+00000370: 7d07 7d08 7c02 7c01 6401 6402 6403 8d03  }.}.|.|.d.d.d...
+00000380: 5c04 7d09 7d0a 7d0b 7d0c 7c03 7c07 7c0b  \.}.}.}.}.|.|.|.
+00000390: a007 6402 6404 a102 8302 7d0d 7c04 7c05  ..d.d.....}.|.|.
+000003a0: 7c09 a007 6402 6404 a102 8302 7d0e 7c03  |...d.d.....}.|.
+000003b0: 7c08 7c0c a007 6402 6404 a102 8302 7d0f  |.|...d.d.....}.
+000003c0: 7c04 7c06 7c0a a007 6402 6404 a102 8302  |.|.|...d.d.....
+000003d0: 7d10 7c0d 7c0e 1800 7d11 7c0f 7c10 1800  }.|.|...}.|.|...
+000003e0: 7d12 7c04 6405 7c11 8302 7d11 7c04 6405  }.|.d.|...}.|.d.
+000003f0: 7c12 8302 7d12 7c11 7c12 1400 5300 2906  |...}.|.|...S.).
+00000400: 7ad6 436f 6d70 7574 6520 7061 6972 7769  z.Compute pairwi
+00000410: 7365 2069 6e74 6572 7365 6374 696f 6e20  se intersection 
+00000420: 6172 6561 7320 6265 7477 6565 6e20 626f  areas between bo
+00000430: 7865 732e 0a0a 2020 2020 4172 6773 3a0a  xes...    Args:.
+00000440: 2020 2020 2020 6774 5f62 6f78 6573 3a20        gt_boxes: 
+00000450: 5b2e 2e2e 2c20 4e2c 2034 5d0a 2020 2020  [..., N, 4].    
+00000460: 2020 626f 7865 733a 205b 2e2e 2e2c 204d    boxes: [..., M
+00000470: 2c20 345d 0a0a 2020 2020 5265 7475 726e  , 4]..    Return
+00000480: 733a 0a20 2020 2020 2061 2066 6c6f 6174  s:.      a float
+00000490: 2054 656e 736f 7220 7769 7468 2073 6861   Tensor with sha
+000004a0: 7065 205b 2e2e 2e2c 204e 2c20 4d5d 2072  pe [..., N, M] r
+000004b0: 6570 7265 7365 6e74 696e 6720 7061 6972  epresenting pair
+000004c0: 7769 7365 2069 6e74 6572 7365 6374 696f  wise intersectio
+000004d0: 6e73 2e0a 2020 2020 7205 0000 0072 0600  ns..    r....r..
+000004e0: 0000 7207 0000 00e9 feff ffff 7201 0000  ..r.........r...
+000004f0: 0029 0872 0900 0000 720a 0000 0072 0b00  .).r....r....r..
+00000500: 0000 720c 0000 00da 076d 696e 696d 756d  ..r......minimum
+00000510: da07 6d61 7869 6d75 6d72 0d00 0000 da08  ..maximumr......
+00000520: 7377 6170 6178 6573 2913 7216 0000 0072  swapaxes).r....r
+00000530: 1700 0000 720c 0000 0072 1900 0000 721a  ....r....r....r.
+00000540: 0000 005a 0679 5f6d 696e 315a 0678 5f6d  ...Z.y_min1Z.x_m
+00000550: 696e 315a 0679 5f6d 6178 315a 0678 5f6d  in1Z.y_max1Z.x_m
+00000560: 6178 315a 0679 5f6d 696e 325a 0678 5f6d  ax1Z.y_min2Z.x_m
+00000570: 696e 325a 0679 5f6d 6178 325a 0678 5f6d  in2Z.y_max2Z.x_m
+00000580: 6178 325a 0979 5f6d 696e 5f6d 6178 5a09  ax2Z.y_min_maxZ.
+00000590: 795f 6d61 785f 6d69 6e5a 0978 5f6d 696e  y_max_minZ.x_min
+000005a0: 5f6d 6178 5a09 785f 6d61 785f 6d69 6e5a  _maxZ.x_max_minZ
+000005b0: 1169 6e74 6572 7365 6374 5f68 6569 6768  .intersect_heigh
+000005c0: 7473 5a10 696e 7465 7273 6563 745f 7769  tsZ.intersect_wi
+000005d0: 6474 6873 7213 0000 0072 1300 0000 7214  dthsr....r....r.
+000005e0: 0000 00da 1062 6f78 5f69 6e74 6572 7365  .....box_interse
+000005f0: 6374 696f 6e1f 0000 0073 2400 0000 000a  ction....s$.....
+00000600: 1801 0601 0601 0802 0601 0601 0602 1601  ................
+00000610: 1603 1201 1201 1201 1202 0801 0801 0a01  ................
+00000620: 0a02 721c 0000 0063 0200 0000 0000 0000  ..r....c........
+00000630: 0000 0000 0700 0000 0600 0000 4300 0000  ............C...
+00000640: 7348 0000 0074 007c 007c 0183 027d 0274  sH...t.|.|...}.t
+00000650: 017c 0083 017d 0374 017c 0183 017d 047c  .|...}.t.|...}.|
+00000660: 0364 0119 007c 0464 0264 0364 0364 0385  .d...|.d.d.d.d..
+00000670: 0266 0319 0017 007c 0218 007d 057c 027c  .f.....|...}.|.|
+00000680: 0564 0417 001b 007d 067c 0653 0029 0561  .d.....}.|.S.).a
+00000690: 0701 0000 436f 6d70 7574 6573 2070 6169  ....Computes pai
+000006a0: 7277 6973 6520 696e 7465 7273 6563 7469  rwise intersecti
+000006b0: 6f6e 2d6f 7665 722d 756e 696f 6e20 6265  on-over-union be
+000006c0: 7477 6565 6e20 626f 7820 636f 6c6c 6563  tween box collec
+000006d0: 7469 6f6e 732e 0a0a 2020 2020 4172 6773  tions...    Args
+000006e0: 3a0a 2020 2020 2020 6774 5f62 6f78 6573  :.      gt_boxes
+000006f0: 3a20 6120 666c 6f61 7420 5465 6e73 6f72  : a float Tensor
+00000700: 2077 6974 6820 5b2e 2e2e 2c20 4e2c 2034   with [..., N, 4
+00000710: 5d2e 0a20 2020 2020 2062 6f78 6573 3a20  ]..      boxes: 
+00000720: 6120 666c 6f61 7420 5465 6e73 6f72 2077  a float Tensor w
+00000730: 6974 6820 5b2e 2e2e 2c20 4d2c 2034 5d2e  ith [..., M, 4].
+00000740: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
+00000750: 2020 2020 2061 2054 656e 736f 7220 7769       a Tensor wi
+00000760: 7468 2073 6861 7065 205b 2e2e 2e2c 204e  th shape [..., N
+00000770: 2c20 4d5d 2072 6570 7265 7365 6e74 696e  , M] representin
+00000780: 6720 7061 6972 7769 7365 2069 6f75 2073  g pairwise iou s
+00000790: 636f 7265 732e 0a20 2020 2029 022e 4e2e  cores..    )..N.
+000007a0: 4e67 8ded b5a0 f7c6 b03e 2902 721c 0000  Ng.......>).r...
+000007b0: 0072 1500 0000 2907 7216 0000 0072 1700  .r....).r....r..
+000007c0: 0000 da0d 696e 7465 7273 6563 7469 6f6e  ....intersection
+000007d0: 735a 0e67 745f 626f 7865 735f 6172 6561  sZ.gt_boxes_area
+000007e0: 735a 0b62 6f78 6573 5f61 7265 6173 da06  sZ.boxes_areas..
+000007f0: 756e 696f 6e73 5a04 696f 7573 7213 0000  unionsZ.iousr...
+00000800: 0072 1300 0000 7214 0000 00da 1262 6f78  .r....r......box
+00000810: 5f69 6f75 5f73 696d 696c 6172 6974 7943  _iou_similarityC
+00000820: 0000 0073 0c00 0000 000a 0a01 0801 0801  ...s............
+00000830: 1e02 0c02 721f 0000 0029 0bda 075f 5f64  ....r....)...__d
+00000840: 6f63 5f5f da03 6a61 78da 096a 6178 2e6e  oc__..jax..jax.n
+00000850: 756d 7079 da05 6e75 6d70 7972 0a00 0000  umpy..numpyr....
+00000860: 720d 0000 005a 0b6c 6163 7373 2e74 7970  r....Z.lacss.typ
+00000870: 6573 da09 4172 7261 794c 696b 6572 1500  es..ArrayLiker..
+00000880: 0000 721c 0000 0072 1f00 0000 7213 0000  ..r....r....r...
+00000890: 0072 1300 0000 7213 0000 0072 1400 0000  .r....r....r....
+000008a0: da08 3c6d 6f64 756c 653e 0100 0000 730e  ..<module>....s.
+000008b0: 0000 0004 0608 010c 0108 0208 0310 1112  ................
+000008c0: 24                                       $
```

### Comparing `lacss-0.4.1/lacss/ops/__pycache__/image.cpython-38.pyc` & `lacss-0.4.2/lacss/ops/__pycache__/image.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 19:35:53 2023 UTC, .py size: 3289 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,218 +1,232 @@
-00000000: 550d 0d0a 0000 0000 99e8 9964 d90c 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 e37d ad64 9c0d 0000  U........}.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
+00000020: 0007 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6502  Z.d.d.l.m.Z...e.
-00000050: 6a05 5a06 6404 6405 8400 5a07 640d 6406  j.Z.d.d...Z.d.d.
-00000060: 6407 8401 5a08 640e 6409 640a 8401 5a09  d...Z.d.d.d...Z.
-00000070: 640f 640b 640c 8401 5a0a 6402 5300 2910  d.d.d...Z.d.S.).
-00000080: e900 0000 0029 01da 0770 6172 7469 616c  .....)...partial
-00000090: 4e29 01da 0863 6f6e 766f 6c76 6563 0100  N)...convolvec..
-000000a0: 0000 0000 0000 0000 0000 0400 0000 0800  ................
-000000b0: 0000 4300 0000 7392 0000 0074 00a0 0164  ..C...s....t...d
-000000c0: 0164 0264 0167 0364 0364 0364 0367 0364  .d.d.g.d.d.d.g.d
-000000d0: 0464 0564 0467 0367 0364 0164 0364 0467  .d.d.g.g.d.d.d.g
-000000e0: 0364 0264 0364 0567 0364 0164 0364 0467  .d.d.d.g.d.d.d.g
-000000f0: 0367 0367 02a1 017d 0174 026a 0374 026a  .g.g...}.t.j.t.j
-00000100: 0374 0474 0564 0664 078d 0264 0364 0867  .t.t.d.d...d.d.g
-00000110: 0264 098d 0264 0864 0367 0264 098d 027d  .d...d.d.g.d...}
-00000120: 0274 00a0 067c 0064 0364 0367 0264 0464  .t...|.d.d.g.d.d
-00000130: 0467 0264 0464 0467 0267 03a1 027d 007c  .g.d.d.g.g...}.|
-00000140: 027c 007c 0183 027d 037c 0353 0029 0a61  .|.|...}.|.S.).a
-00000150: 7601 0000 5265 7475 726e 7320 6120 7465  v...Returns a te
-00000160: 6e73 6f72 2068 6f6c 6469 6e67 2053 6f62  nsor holding Sob
-00000170: 656c 2065 6467 6520 6d61 7073 2e0a 2020  el edge maps..  
-00000180: 2020 3e3e 3e20 696d 6167 6520 3d20 7261    >>> image = ra
-00000190: 6e64 6f6d 2e75 6e69 666f 726d 286b 6579  ndom.uniform(key
-000001a0: 2c20 7368 6170 653d 5b33 2c20 3238 2c20  , shape=[3, 28, 
-000001b0: 3238 5d29 0a20 2020 203e 3e3e 2073 6f62  28]).    >>> sob
-000001c0: 656c 203d 2073 6f62 656c 5f65 6467 6573  el = sobel_edges
-000001d0: 2869 6d61 6765 290a 2020 2020 3e3e 3e20  (image).    >>> 
-000001e0: 736f 6265 6c5f 7920 3d20 736f 6265 6c5b  sobel_y = sobel[
-000001f0: 302c 203a 2c20 3a2c 203a 5d20 2320 736f  0, :, :, :] # so
-00000200: 6265 6c20 696e 2079 2d64 6972 6563 7469  bel in y-directi
-00000210: 6f6e 0a20 2020 203e 3e3e 2073 6f62 656c  on.    >>> sobel
-00000220: 5f78 203d 2073 6f62 656c 5b31 2c20 3a2c  _x = sobel[1, :,
-00000230: 203a 2c20 3a5d 2023 2073 6f62 656c 2069   :, :] # sobel i
-00000240: 6e20 782d 6469 7265 6374 696f 6e0a 2020  n x-direction.  
-00000250: 2020 6060 600a 2020 2020 4172 6773 3a0a    ```.    Args:.
-00000260: 2020 2020 2020 2020 696d 6167 653a 205b          image: [
-00000270: 6e2c 2068 2c20 775d 0a20 2020 2052 6574  n, h, w].    Ret
-00000280: 7572 6e73 3a0a 2020 2020 2020 2020 5465  urns:.        Te
-00000290: 6e73 6f72 2068 6f6c 6469 6e67 2065 6467  nsor holding edg
-000002a0: 6520 6d61 7073 2066 6f72 2065 6163 6820  e maps for each 
-000002b0: 6368 616e 6e65 6c2e 205b 322c 206e 2c20  channel. [2, n, 
-000002c0: 682c 2077 5d0a 2020 2020 e9ff ffff ffe9  h, w].    ......
-000002d0: feff ffff 7201 0000 00e9 0100 0000 e902  ....r...........
-000002e0: 0000 00da 0576 616c 6964 2901 da04 6d6f  .....valid)...mo
-000002f0: 6465 4ea9 01da 0769 6e5f 6178 6573 2907  deN....in_axes).
-00000300: da03 6a6e 70da 0561 7272 6179 da03 6a61  ..jnp..array..ja
-00000310: 78da 0476 6d61 7072 0200 0000 7203 0000  x..vmapr....r...
-00000320: 00da 0370 6164 2904 da05 696d 6167 65da  ...pad)...image.
-00000330: 076b 6572 6e65 6c73 5a0d 736f 7262 656c  .kernelsZ.sorbel
-00000340: 5f66 696c 7465 72da 066f 7574 7075 74a9  _filter..output.
-00000350: 0072 1400 0000 fa32 2f68 6f6d 652f 4643  .r.....2/home/FC
-00000360: 414d 2f6a 7975 2f70 726f 6a5f 6c61 6373  AM/jyu/proj_lacs
-00000370: 732f 6c61 6373 732f 6c61 6373 732f 6f70  s/lacss/lacss/op
-00000380: 732f 696d 6167 652e 7079 da0c 736f 7262  s/image.py..sorb
-00000390: 656c 5f65 6467 6573 0900 0000 731a 0000  el_edges....s...
-000003a0: 0000 0d04 0136 ff04 0404 0104 010a 0106  .....6..........
-000003b0: fe04 0406 fb06 081e 010a 0272 1600 0000  ...........r....
-000003c0: 6303 0000 0000 0000 0000 0000 000b 0000  c...............
-000003d0: 0008 0000 0003 0000 0073 e000 0000 7400  .........s....t.
-000003e0: a001 8800 a101 a002 7403 a101 7d03 8800  ........t...}...
-000003f0: 7c03 1800 7d04 7400 a004 8700 6601 6401  |...}.t.....f.d.
-00000400: 6402 8408 7405 6403 7406 8800 8301 1300  d...t.d.t.......
-00000410: 8301 4400 8301 a101 7d05 7400 a007 7c03  ..D.....}.t...|.
-00000420: 7c05 1700 6404 6405 a103 7d06 7400 6a08  |...d.d...}.t.j.
-00000430: 7c04 7c05 6405 6b02 1400 6405 7c04 1800  |.|.d.k...d.|...
-00000440: 7c05 6404 6b02 1400 1700 6405 6406 8d02  |.d.k.....d.d...
-00000450: 7d07 7400 a004 7c00 6a09 a101 6400 7406  }.t...|.j...d.t.
-00000460: 8800 8301 8502 6400 6602 1900 7d08 7400  ......d.f...}.t.
-00000470: a00a 7c06 6404 6b05 6a0b 6404 6406 8d01  ..|.d.k.j.d.d...
-00000480: 7c06 7c08 6b00 6a0b 6404 6406 8d01 4000  |.|.k.j.d.d...@.
-00000490: 7400 a007 7c00 740c 7c06 8301 1900 6404  t...|.t.|.....d.
-000004a0: 6407 a103 7c02 a103 7d09 7c09 7c07 1400  d...|...}.|.|...
-000004b0: 6a0d 6407 6406 8d01 7d0a 7c0a 5300 2908  j.d.d...}.|.S.).
-000004c0: 4e63 0100 0000 0000 0000 0000 0000 0100  Nc..............
-000004d0: 0000 0600 0000 1300 0000 7326 0000 0067  ..........s&...g
-000004e0: 007c 005d 1e89 0087 0066 0164 0064 0184  .|.].....f.d.d..
-000004f0: 0874 0074 0188 0183 0183 0144 0083 0191  .t.t.......D....
-00000500: 0271 0453 0029 0263 0100 0000 0000 0000  .q.S.).c........
-00000510: 0000 0000 0200 0000 0400 0000 1300 0000  ................
-00000520: 7318 0000 0067 007c 005d 107d 0188 007c  s....g.|.].}...|
-00000530: 013f 0064 0016 0091 0271 0453 0029 0172  .?.d.....q.S.).r
-00000540: 0700 0000 7214 0000 0029 02da 022e 30da  ....r....)....0.
-00000550: 016a a901 da01 6972 1400 0000 7215 0000  .j....ir....r...
-00000560: 00da 0a3c 6c69 7374 636f 6d70 3e2e 0000  ...<listcomp>...
-00000570: 0073 0400 0000 0600 0200 7a31 5f72 6574  .s........z1_ret
-00000580: 7269 6576 655f 7661 6c75 655f 6174 2e3c  rieve_value_at.<
-00000590: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-000005a0: 703e 2e3c 6c69 7374 636f 6d70 3e29 02da  p>.<listcomp>)..
-000005b0: 0572 616e 6765 da03 6c65 6e29 0172 1700  .range..len).r..
-000005c0: 0000 a901 da03 6c6f 6372 1900 0000 7215  ......locr....r.
-000005d0: 0000 0072 1b00 0000 2e00 0000 7304 0000  ...r........s...
-000005e0: 0006 0002 007a 265f 7265 7472 6965 7665  .....z&_retrieve
-000005f0: 5f76 616c 7565 5f61 742e 3c6c 6f63 616c  _value_at.<local
-00000600: 733e 2e3c 6c69 7374 636f 6d70 3e72 0700  s>.<listcomp>r..
-00000610: 0000 7201 0000 0072 0600 0000 a901 da04  ..r....r........
-00000620: 6178 6973 7204 0000 0029 0e72 0c00 0000  axisr....).r....
-00000630: da05 666c 6f6f 72da 0661 7374 7970 65da  ..floor..astype.
-00000640: 0369 6e74 da07 6173 6172 7261 7972 1c00  .int..asarrayr..
-00000650: 0000 721d 0000 00da 0873 7761 7061 7865  ..r......swapaxe
-00000660: 73da 0470 726f 64da 0573 6861 7065 da05  s..prod..shape..
-00000670: 7768 6572 65da 0361 6c6c da05 7475 706c  where..all..tupl
-00000680: 65da 0373 756d 290b da03 696d 6772 1f00  e..sum)...imgr..
-00000690: 0000 da12 6f75 745f 6f66 5f62 6f75 6e64  ....out_of_bound
-000006a0: 5f76 616c 7565 da04 696c 6f63 da03 7265  _value..iloc..re
-000006b0: 73da 076f 6666 7365 7473 da05 696c 6f63  s..offsets..iloc
-000006c0: 73da 0677 6569 6768 745a 0b6d 6178 5f69  s..weightZ.max_i
-000006d0: 6e64 6963 6573 da06 7661 6c75 6573 da05  ndices..values..
-000006e0: 7661 6c75 6572 1400 0000 721e 0000 0072  valuer....r....r
-000006f0: 1500 0000 da12 5f72 6574 7269 6576 655f  ......_retrieve_
-00000700: 7661 6c75 655f 6174 2800 0000 731e 0000  value_at(...s...
-00000710: 0000 0210 0108 0204 011c ff04 0312 0226  ...............&
-00000720: 021c 0104 011e 0114 0102 fd04 0610 0272  ...............r
-00000730: 3600 0000 4663 0400 0000 0000 0000 0000  6...Fc..........
-00000740: 0000 0a00 0000 0500 0000 4300 0000 7388  ..........C...s.
-00000750: 0000 007c 016a 007d 047c 006a 007d 057c  ...|.j.}.|.j.}.|
-00000760: 0464 0119 007d 067c 0372 207c 0164 0218  .d...}.|.r |.d..
-00000770: 007d 017c 00a0 017c 0564 037c 0685 0219  .}.|...|.d.|....
-00000780: 0064 0417 00a1 017d 007c 01a0 0164 017c  .d.....}.|...d.|
-00000790: 06a1 027d 0174 0274 037c 0264 058d 027d  ...}.t.t.|.d...}
-000007a0: 0774 046a 057c 0764 0664 078d 027c 007c  .t.j.|.d.d...|.|
-000007b0: 0183 027d 087c 0464 0364 0185 0219 007c  ...}.|.d.d.....|
-000007c0: 057c 0664 0385 0219 0017 007d 097c 08a0  .|.d.......}.|..
-000007d0: 017c 09a1 017d 087c 0853 0029 0861 8d01  .|...}.|.S.).a..
-000007e0: 0000 5265 7472 6965 7665 2069 6d61 6765  ..Retrieve image
-000007f0: 2076 616c 7565 7320 6173 206e 6f6e 2d69   values as non-i
-00000800: 6e74 6567 6572 206c 6f63 6174 696f 6e73  nteger locations
-00000810: 2062 7920 696e 7465 7270 6f6c 6174 696f   by interpolatio
-00000820: 6e0a 2020 2020 4172 6773 3a0a 2020 2020  n.    Args:.    
-00000830: 2020 2020 696d 673a 2041 7272 6179 206f      img: Array o
-00000840: 6620 7368 6170 6520 5b44 312c 4432 2c2e  f shape [D1,D2,.
-00000850: 2e2c 446b 2c20 2e2e 2e5d 0a20 2020 2020  .,Dk, ...].     
-00000860: 2020 206c 6f63 733a 2041 7272 6179 206f     locs: Array o
-00000870: 6620 7368 6170 6520 5b64 312c 6432 2c2e  f shape [d1,d2,.
-00000880: 2e2c 646e 2c20 6b5d 0a20 2020 2020 2020  .,dn, k].       
-00000890: 206f 7574 5f6f 665f 626f 756e 645f 7661   out_of_bound_va
-000008a0: 6c75 653a 206f 7074 696f 6e61 6c20 666c  lue: optional fl
-000008b0: 6f61 7420 636f 6e73 7461 6e74 2c20 6465  oat constant, de
-000008c0: 6675 616c 7420 302e 0a20 2020 2020 2020  fualt 0..       
-000008d0: 2065 6467 655f 696e 6465 7869 6e67 3a20   edge_indexing: 
-000008e0: 6966 2054 7275 652c 2074 6865 2069 6e64  if True, the ind
-000008f0: 6578 2066 6f72 2074 6865 2066 6972 7374  ex for the first
-00000900: 2076 616c 7565 2069 6e20 696d 6720 6973   value in img is
-00000910: 2030 2e35 2c20 6f74 6865 7277 6973 6520   0.5, otherwise 
-00000920: 302e 2044 6566 6175 6c74 2069 7320 4661  0. Default is Fa
-00000930: 6c73 650a 2020 2020 5265 7475 726e 733a  lse.    Returns:
-00000940: 0a20 2020 2020 2020 2076 616c 7565 733a  .        values:
-00000950: 205b 6431 2c64 322c 2e2e 2c64 6e2c 202e   [d1,d2,..,dn, .
-00000960: 2e2e 5d2c 2066 6c6f 6174 0a20 2020 2072  ..], float.    r
-00000970: 0400 0000 6700 0000 0000 00e0 3f4e 2901  ....g.......?N).
-00000980: 7204 0000 0029 0172 2e00 0000 2902 4e72  r....).r....).Nr
-00000990: 0100 0000 720a 0000 0029 0672 2800 0000  ....r....).r(...
-000009a0: da07 7265 7368 6170 6572 0200 0000 7236  ..reshaper....r6
-000009b0: 0000 0072 0e00 0000 720f 0000 0029 0a72  ...r....r....).r
-000009c0: 2d00 0000 da04 6c6f 6373 722e 0000 00da  -.....locsr.....
-000009d0: 0d65 6467 655f 696e 6465 7869 6e67 5a09  .edge_indexingZ.
-000009e0: 6c6f 635f 7368 6170 65da 0969 6d67 5f73  loc_shape..img_s
-000009f0: 6861 7065 5a05 645f 6c6f 63da 026f 7072  hapeZ.d_loc..opr
-00000a00: 3400 0000 da09 6f75 745f 7368 6170 6572  4.....out_shaper
-00000a10: 1400 0000 7214 0000 0072 1500 0000 da11  ....r....r......
-00000a20: 7375 625f 7069 7865 6c5f 7361 6d70 6c65  sub_pixel_sample
-00000a30: 7340 0000 0073 1800 0000 000b 0601 0601  s@...s..........
-00000a40: 0802 0401 0802 1601 0c01 0c02 1401 1802  ................
-00000a50: 0a02 723d 0000 0063 0400 0000 0000 0000  ..r=...c........
-00000a60: 0000 0000 0e00 0000 0600 0000 4300 0000  ............C...
-00000a70: 738c 0000 0074 00a0 017c 01a1 017d 0174  s....t...|...}.t
-00000a80: 00a0 017c 00a1 017d 007c 015c 047d 047d  ...|...}.|.\.}.}
-00000a90: 057d 067d 077c 025c 027d 087d 097c 067c  .}.}.|.\.}.}.|.|
-00000aa0: 0418 007c 081b 007d 0a7c 077c 0518 007c  ...|...}.|.|...|
-00000ab0: 091b 007d 0b74 006a 027c 047c 0a64 011b  ...}.t.j.|.|.d..
-00000ac0: 0017 007c 067c 0a85 037c 057c 0b64 011b  ...|.|...|.|.d..
-00000ad0: 0017 007c 077c 0b85 0366 0219 005c 027d  ...|.|...f...\.}
-00000ae0: 0c7d 0d74 037c 0074 006a 047c 0c7c 0d67  .}.t.|.t.j.|.|.g
-00000af0: 0264 0264 038d 027c 0364 0464 058d 0453  .d.d...|.d.d...S
-00000b00: 0029 0661 2401 0000 5265 7472 6965 7665  .).a$...Retrieve
-00000b10: 2069 6d61 6765 2076 616c 7565 7320 6f66   image values of
-00000b20: 2061 2062 626f 7820 7265 7369 7a65 206f   a bbox resize o
-00000b30: 7574 7075 742e 2055 7365 6420 666f 7220  utput. Used for 
-00000b40: 524f 492d 416c 6967 6e0a 2020 2020 4172  ROI-Align.    Ar
-00000b50: 6773 3a0a 2020 2020 2020 2020 696d 673a  gs:.        img:
-00000b60: 2041 7272 6179 206f 6620 7368 6170 6520   Array of shape 
-00000b70: 5b48 2c20 572c 202e 2e2e 5d0a 2020 2020  [H, W, ...].    
-00000b80: 2020 2020 6262 6f78 3a20 5b79 302c 2078      bbox: [y0, x
-00000b90: 302c 2079 312c 2078 315d 0a20 2020 2020  0, y1, x1].     
-00000ba0: 2020 206f 7574 7075 745f 7368 6170 653a     output_shape:
-00000bb0: 205b 682c 2077 5d0a 2020 2020 2020 2020   [h, w].        
-00000bc0: 6f75 745f 6f66 5f62 6f75 6e64 5f76 616c  out_of_bound_val
-00000bd0: 7565 3a20 6f70 7469 6f6e 616c 2066 6c6f  ue: optional flo
-00000be0: 6174 2063 6f6e 7374 616e 742c 2064 6566  at constant, def
-00000bf0: 7561 6c74 2030 2e0a 2020 2020 5265 7475  ualt 0..    Retu
-00000c00: 726e 733a 0a20 2020 2020 2020 2076 616c  rns:.        val
-00000c10: 7565 733a 205b 682c 2077 2c20 2e2e 2e5d  ues: [h, w, ...]
-00000c20: 2c20 666c 6f61 740a 2020 2020 7207 0000  , float.    r...
-00000c30: 0072 0400 0000 7220 0000 0054 2902 722e  .r....r ...T).r.
-00000c40: 0000 0072 3900 0000 2905 720c 0000 0072  ...r9...).r....r
-00000c50: 2500 0000 da05 6d67 7269 6472 3d00 0000  %.....mgridr=...
-00000c60: da05 7374 6163 6b29 0e72 2d00 0000 da04  ..stack).r-.....
-00000c70: 6262 6f78 da0c 6f75 7470 7574 5f73 6861  bbox..output_sha
-00000c80: 7065 722e 0000 00da 0279 30da 0278 30da  per......y0..x0.
-00000c90: 0279 31da 0278 31da 0168 da01 77da 0264  .y1..x1..h..w..d
-00000ca0: 79da 0264 78da 0279 79da 0278 7872 1400  y..dx..yy..xxr..
-00000cb0: 0000 7214 0000 0072 1500 0000 da19 7375  ..r....r......su
-00000cc0: 625f 7069 7865 6c5f 6372 6f70 5f61 6e64  b_pixel_crop_and
-00000cd0: 5f72 6573 697a 655e 0000 0073 1a00 0000  _resize^...s....
-00000ce0: 000b 0a01 0a01 0c01 0802 0c01 0c02 2e01  ................
-00000cf0: 0201 0201 1001 0201 02fc 724c 0000 0029  ..........rL...)
-00000d00: 0172 0100 0000 2902 7201 0000 0046 2901  .r....).r....F).
-00000d10: 7201 0000 0029 0bda 0966 756e 6374 6f6f  r....)...functoo
-00000d20: 6c73 7202 0000 0072 0e00 0000 5a10 6a61  lsr....r....Z.ja
-00000d30: 782e 7363 6970 792e 7369 676e 616c 7203  x.scipy.signalr.
-00000d40: 0000 00da 056e 756d 7079 720c 0000 0072  .....numpyr....r
-00000d50: 1600 0000 7236 0000 0072 3d00 0000 724c  ....r6...r=...rL
-00000d60: 0000 0072 1400 0000 7214 0000 0072 1400  ...r....r....r..
-00000d70: 0000 7215 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000d80: 3e01 0000 0073 0e00 0000 0c02 0801 0c02  >....s..........
-00000d90: 0603 081f 0a18 0a1e                      ........
+00000050: 6a05 5a06 6400 6404 6c07 5400 6508 6509  j.Z.d.d.l.T.e.e.
+00000060: 6405 9c02 6406 6407 8404 5a0a 6411 6408  d...d.d...Z.d.d.
+00000070: 6409 8401 5a0b 6412 6508 6508 650c 650d  d...Z.d.e.e.e.e.
+00000080: 6509 640b 9c05 640c 640d 8405 5a0e 6413  e.d...d.d...Z.d.
+00000090: 6508 6508 650f 650c 6509 640e 9c05 640f  e.e.e.e.e.d...d.
+000000a0: 6410 8405 5a10 6402 5300 2914 e900 0000  d...Z.d.S.).....
+000000b0: 0029 01da 0770 6172 7469 616c 4e29 01da  .)...partialN)..
+000000c0: 0863 6f6e 766f 6c76 6529 01da 012a 2902  .convolve)...*).
+000000d0: da05 696d 6167 65da 0672 6574 7572 6e63  ..image..returnc
+000000e0: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+000000f0: 0800 0000 4300 0000 7392 0000 0074 00a0  ....C...s....t..
+00000100: 0164 0164 0264 0167 0364 0364 0364 0367  .d.d.d.g.d.d.d.g
+00000110: 0364 0464 0564 0467 0367 0364 0164 0364  .d.d.d.g.g.d.d.d
+00000120: 0467 0364 0264 0364 0567 0364 0164 0364  .g.d.d.d.g.d.d.d
+00000130: 0467 0367 0367 02a1 017d 0174 026a 0374  .g.g.g...}.t.j.t
+00000140: 026a 0374 0474 0564 0664 078d 0264 0364  .j.t.t.d.d...d.d
+00000150: 0867 0264 098d 0264 0864 0367 0264 098d  .g.d...d.d.g.d..
+00000160: 027d 0274 00a0 067c 0064 0364 0367 0264  .}.t...|.d.d.g.d
+00000170: 0464 0467 0264 0464 0467 0267 03a1 027d  .d.g.d.d.g.g...}
+00000180: 007c 027c 007c 0183 027d 037c 0353 0029  .|.|.|...}.|.S.)
+00000190: 0a61 9001 0000 5265 7475 726e 7320 6120  .a....Returns a 
+000001a0: 7465 6e73 6f72 2068 6f6c 6469 6e67 2053  tensor holding S
+000001b0: 6f62 656c 2065 6467 6520 6d61 7073 2e0a  obel edge maps..
+000001c0: 0a20 2020 2045 7861 6d70 6c65 733a 0a0a  .    Examples:..
+000001d0: 2020 2020 2020 2020 3e3e 3e20 696d 6167          >>> imag
+000001e0: 6520 3d20 7261 6e64 6f6d 2e75 6e69 666f  e = random.unifo
+000001f0: 726d 286b 6579 2c20 7368 6170 653d 5b33  rm(key, shape=[3
+00000200: 2c20 3238 2c20 3238 5d29 0a20 2020 2020  , 28, 28]).     
+00000210: 2020 203e 3e3e 2073 6f62 656c 203d 2073     >>> sobel = s
+00000220: 6f62 656c 5f65 6467 6573 2869 6d61 6765  obel_edges(image
+00000230: 290a 2020 2020 2020 2020 3e3e 3e20 736f  ).        >>> so
+00000240: 6265 6c5f 7920 3d20 736f 6265 6c5b 302c  bel_y = sobel[0,
+00000250: 203a 2c20 3a2c 203a 5d20 2320 736f 6265   :, :, :] # sobe
+00000260: 6c20 696e 2079 2d64 6972 6563 7469 6f6e  l in y-direction
+00000270: 0a20 2020 2020 2020 203e 3e3e 2073 6f62  .        >>> sob
+00000280: 656c 5f78 203d 2073 6f62 656c 5b31 2c20  el_x = sobel[1, 
+00000290: 3a2c 203a 2c20 3a5d 2023 2073 6f62 656c  :, :, :] # sobel
+000002a0: 2069 6e20 782d 6469 7265 6374 696f 6e0a   in x-direction.
+000002b0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+000002c0: 2020 2069 6d61 6765 3a20 5b6e 2c20 682c     image: [n, h,
+000002d0: 2077 5d0a 0a20 2020 2052 6574 7572 6e73   w]..    Returns
+000002e0: 3a0a 2020 2020 2020 2020 5465 6e73 6f72  :.        Tensor
+000002f0: 2068 6f6c 6469 6e67 2065 6467 6520 6d61   holding edge ma
+00000300: 7073 2066 6f72 2065 6163 6820 6368 616e  ps for each chan
+00000310: 6e65 6c2e 205b 322c 206e 2c20 682c 2077  nel. [2, n, h, w
+00000320: 5d0a 2020 2020 e9ff ffff ffe9 feff ffff  ].    ..........
+00000330: 7201 0000 00e9 0100 0000 e902 0000 00da  r...............
+00000340: 0576 616c 6964 2901 da04 6d6f 6465 4ea9  .valid)...modeN.
+00000350: 01da 0769 6e5f 6178 6573 2907 da03 6a6e  ...in_axes)...jn
+00000360: 70da 0561 7272 6179 da03 6a61 78da 0476  p..array..jax..v
+00000370: 6d61 7072 0200 0000 7203 0000 00da 0370  mapr....r......p
+00000380: 6164 2904 7205 0000 00da 076b 6572 6e65  ad).r......kerne
+00000390: 6c73 5a0d 736f 7262 656c 5f66 696c 7465  lsZ.sorbel_filte
+000003a0: 72da 066f 7574 7075 74a9 0072 1600 0000  r..output..r....
+000003b0: fa32 2f68 6f6d 652f 4643 414d 2f6a 7975  .2/home/FCAM/jyu
+000003c0: 2f70 726f 6a5f 6c61 6373 732f 6c61 6373  /proj_lacss/lacs
+000003d0: 732f 6c61 6373 732f 6f70 732f 696d 6167  s/lacss/ops/imag
+000003e0: 652e 7079 da0c 736f 7262 656c 5f65 6467  e.py..sorbel_edg
+000003f0: 6573 0b00 0000 731a 0000 0000 1104 0136  es....s........6
+00000400: ff04 0404 0104 010a 0106 fe04 0406 fb06  ................
+00000410: 081e 010a 0272 1800 0000 6303 0000 0000  .....r....c.....
+00000420: 0000 0000 0000 000b 0000 0008 0000 0003  ................
+00000430: 0000 0073 e000 0000 7400 a001 8800 a101  ...s....t.......
+00000440: a002 7403 a101 7d03 8800 7c03 1800 7d04  ..t...}...|...}.
+00000450: 7400 a004 8700 6601 6401 6402 8408 7405  t.....f.d.d...t.
+00000460: 6403 7406 8800 8301 1300 8301 4400 8301  d.t.........D...
+00000470: a101 7d05 7400 a007 7c03 7c05 1700 6404  ..}.t...|.|...d.
+00000480: 6405 a103 7d06 7400 6a08 7c04 7c05 6405  d...}.t.j.|.|.d.
+00000490: 6b02 1400 6405 7c04 1800 7c05 6404 6b02  k...d.|...|.d.k.
+000004a0: 1400 1700 6405 6406 8d02 7d07 7400 a004  ....d.d...}.t...
+000004b0: 7c00 6a09 a101 6400 7406 8800 8301 8502  |.j...d.t.......
+000004c0: 6400 6602 1900 7d08 7400 a00a 7c06 6404  d.f...}.t...|.d.
+000004d0: 6b05 6a0b 6404 6406 8d01 7c06 7c08 6b00  k.j.d.d...|.|.k.
+000004e0: 6a0b 6404 6406 8d01 4000 7400 a007 7c00  j.d.d...@.t...|.
+000004f0: 740c 7c06 8301 1900 6404 6407 a103 7c02  t.|.....d.d...|.
+00000500: a103 7d09 7c09 7c07 1400 6a0d 6407 6406  ..}.|.|...j.d.d.
+00000510: 8d01 7d0a 7c0a 5300 2908 4e63 0100 0000  ..}.|.S.).Nc....
+00000520: 0000 0000 0000 0000 0100 0000 0600 0000  ................
+00000530: 1300 0000 7326 0000 0067 007c 005d 1e89  ....s&...g.|.]..
+00000540: 0087 0066 0164 0064 0184 0874 0074 0188  ...f.d.d...t.t..
+00000550: 0183 0183 0144 0083 0191 0271 0453 0029  .....D.....q.S.)
+00000560: 0263 0100 0000 0000 0000 0000 0000 0200  .c..............
+00000570: 0000 0400 0000 1300 0000 7318 0000 0067  ..........s....g
+00000580: 007c 005d 107d 0188 007c 013f 0064 0016  .|.].}...|.?.d..
+00000590: 0091 0271 0453 0029 0172 0a00 0000 7216  ...q.S.).r....r.
+000005a0: 0000 0029 02da 022e 30da 016a a901 da01  ...)....0..j....
+000005b0: 6972 1600 0000 7217 0000 00da 0a3c 6c69  ir....r......<li
+000005c0: 7374 636f 6d70 3e34 0000 0073 0400 0000  stcomp>4...s....
+000005d0: 0600 0200 7a31 5f72 6574 7269 6576 655f  ....z1_retrieve_
+000005e0: 7661 6c75 655f 6174 2e3c 6c6f 6361 6c73  value_at.<locals
+000005f0: 3e2e 3c6c 6973 7463 6f6d 703e 2e3c 6c69  >.<listcomp>.<li
+00000600: 7374 636f 6d70 3e29 02da 0572 616e 6765  stcomp>)...range
+00000610: da03 6c65 6e29 0172 1900 0000 a901 da03  ..len).r........
+00000620: 6c6f 6372 1b00 0000 7217 0000 0072 1d00  locr....r....r..
+00000630: 0000 3400 0000 7304 0000 0006 0002 007a  ..4...s........z
+00000640: 265f 7265 7472 6965 7665 5f76 616c 7565  &_retrieve_value
+00000650: 5f61 742e 3c6c 6f63 616c 733e 2e3c 6c69  _at.<locals>.<li
+00000660: 7374 636f 6d70 3e72 0a00 0000 7201 0000  stcomp>r....r...
+00000670: 0072 0900 0000 a901 da04 6178 6973 7207  .r........axisr.
+00000680: 0000 0029 0e72 0f00 0000 da05 666c 6f6f  ...).r......floo
+00000690: 72da 0661 7374 7970 65da 0369 6e74 da07  r..astype..int..
+000006a0: 6173 6172 7261 7972 1e00 0000 721f 0000  asarrayr....r...
+000006b0: 00da 0873 7761 7061 7865 73da 0470 726f  ...swapaxes..pro
+000006c0: 64da 0573 6861 7065 da05 7768 6572 65da  d..shape..where.
+000006d0: 0361 6c6c da05 7475 706c 65da 0373 756d  .all..tuple..sum
+000006e0: 290b da03 696d 6772 2100 0000 da12 6f75  )...imgr!.....ou
+000006f0: 745f 6f66 5f62 6f75 6e64 5f76 616c 7565  t_of_bound_value
+00000700: da04 696c 6f63 da03 7265 73da 076f 6666  ..iloc..res..off
+00000710: 7365 7473 5a05 696c 6f63 73da 0677 6569  setsZ.ilocs..wei
+00000720: 6768 745a 0b6d 6178 5f69 6e64 6963 6573  ghtZ.max_indices
+00000730: da06 7661 6c75 6573 da05 7661 6c75 6572  ..values..valuer
+00000740: 1600 0000 7220 0000 0072 1700 0000 da12  ....r ...r......
+00000750: 5f72 6574 7269 6576 655f 7661 6c75 655f  _retrieve_value_
+00000760: 6174 2e00 0000 731e 0000 0000 0210 0108  at....s.........
+00000770: 0204 011c ff04 0312 0226 021c 0104 011e  .........&......
+00000780: 0114 0102 fd04 0610 0272 3700 0000 4629  .........r7...F)
+00000790: 0572 2f00 0000 da04 6c6f 6373 7230 0000  .r/.....locsr0..
+000007a0: 00da 0d65 6467 655f 696e 6465 7869 6e67  ...edge_indexing
+000007b0: 7206 0000 0063 0400 0000 0000 0000 0000  r....c..........
+000007c0: 0000 0a00 0000 0500 0000 4300 0000 7388  ..........C...s.
+000007d0: 0000 007c 016a 007d 047c 006a 007d 057c  ...|.j.}.|.j.}.|
+000007e0: 0464 0119 007d 067c 0372 207c 0164 0218  .d...}.|.r |.d..
+000007f0: 007d 017c 00a0 017c 0564 037c 0685 0219  .}.|...|.d.|....
+00000800: 0064 0417 00a1 017d 007c 01a0 0164 017c  .d.....}.|...d.|
+00000810: 06a1 027d 0174 0274 037c 0264 058d 027d  ...}.t.t.|.d...}
+00000820: 0774 046a 057c 0764 0664 078d 027c 007c  .t.j.|.d.d...|.|
+00000830: 0183 027d 087c 0464 0364 0185 0219 007c  ...}.|.d.d.....|
+00000840: 057c 0664 0385 0219 0017 007d 097c 08a0  .|.d.......}.|..
+00000850: 017c 09a1 017d 087c 0853 0029 0861 8f01  .|...}.|.S.).a..
+00000860: 0000 5265 7472 6965 7665 2069 6d61 6765  ..Retrieve image
+00000870: 2076 616c 7565 7320 6173 206e 6f6e 2d69   values as non-i
+00000880: 6e74 6567 6572 206c 6f63 6174 696f 6e73  nteger locations
+00000890: 2062 7920 696e 7465 7270 6f6c 6174 696f   by interpolatio
+000008a0: 6e0a 0a20 2020 2041 7267 733a 0a20 2020  n..    Args:.   
+000008b0: 2020 2020 2069 6d67 3a20 4172 7261 7920       img: Array 
+000008c0: 6f66 2073 6861 7065 205b 4431 2c44 322c  of shape [D1,D2,
+000008d0: 2e2e 2c44 6b2c 202e 2e2e 5d0a 2020 2020  ..,Dk, ...].    
+000008e0: 2020 2020 6c6f 6373 3a20 4172 7261 7920      locs: Array 
+000008f0: 6f66 2073 6861 7065 205b 6431 2c64 322c  of shape [d1,d2,
+00000900: 2e2e 2c64 6e2c 206b 5d0a 2020 2020 2020  ..,dn, k].      
+00000910: 2020 6f75 745f 6f66 5f62 6f75 6e64 5f76    out_of_bound_v
+00000920: 616c 7565 3a20 6f70 7469 6f6e 616c 2066  alue: optional f
+00000930: 6c6f 6174 2063 6f6e 7374 616e 742c 2064  loat constant, d
+00000940: 6566 7561 6c74 2030 2e0a 2020 2020 2020  efualt 0..      
+00000950: 2020 6564 6765 5f69 6e64 6578 696e 673a    edge_indexing:
+00000960: 2069 6620 5472 7565 2c20 7468 6520 696e   if True, the in
+00000970: 6465 7820 666f 7220 7468 6520 6669 7273  dex for the firs
+00000980: 7420 7661 6c75 6520 696e 2069 6d67 2069  t value in img i
+00000990: 7320 302e 352c 206f 7468 6572 7769 7365  s 0.5, otherwise
+000009a0: 2030 2e20 4465 6661 756c 7420 6973 2046   0. Default is F
+000009b0: 616c 7365 0a0a 2020 2020 5265 7475 726e  alse..    Return
+000009c0: 733a 0a20 2020 2020 2020 2076 616c 7565  s:.        value
+000009d0: 733a 205b 6431 2c64 322c 2e2e 2c64 6e2c  s: [d1,d2,..,dn,
+000009e0: 202e 2e2e 5d2c 2066 6c6f 6174 0a20 2020   ...], float.   
+000009f0: 2072 0700 0000 6700 0000 0000 00e0 3f4e   r....g.......?N
+00000a00: 2901 7207 0000 0029 0172 3000 0000 2902  ).r....).r0...).
+00000a10: 4e72 0100 0000 720d 0000 0029 0672 2a00  Nr....r....).r*.
+00000a20: 0000 da07 7265 7368 6170 6572 0200 0000  ....reshaper....
+00000a30: 7237 0000 0072 1100 0000 7212 0000 0029  r7...r....r....)
+00000a40: 0a72 2f00 0000 7238 0000 0072 3000 0000  .r/...r8...r0...
+00000a50: 7239 0000 005a 096c 6f63 5f73 6861 7065  r9...Z.loc_shape
+00000a60: da09 696d 675f 7368 6170 655a 0564 5f6c  ..img_shapeZ.d_l
+00000a70: 6f63 da02 6f70 7235 0000 00da 096f 7574  oc..opr5.....out
+00000a80: 5f73 6861 7065 7216 0000 0072 1600 0000  _shaper....r....
+00000a90: 7217 0000 00da 1173 7562 5f70 6978 656c  r......sub_pixel
+00000aa0: 5f73 616d 706c 6573 4600 0000 7318 0000  _samplesF...s...
+00000ab0: 0000 1206 0106 0108 0204 0108 0216 010c  ................
+00000ac0: 010c 0214 0118 020a 0272 3e00 0000 2905  .........r>...).
+00000ad0: 722f 0000 00da 0462 626f 78da 0c6f 7574  r/.....bbox..out
+00000ae0: 7075 745f 7368 6170 6572 3000 0000 7206  put_shaper0...r.
+00000af0: 0000 0063 0400 0000 0000 0000 0000 0000  ...c............
+00000b00: 0e00 0000 0600 0000 4300 0000 738c 0000  ........C...s...
+00000b10: 0074 00a0 017c 01a1 017d 0174 00a0 017c  .t...|...}.t...|
+00000b20: 00a1 017d 007c 015c 047d 047d 057d 067d  ...}.|.\.}.}.}.}
+00000b30: 077c 025c 027d 087d 097c 067c 0418 007c  .|.\.}.}.|.|...|
+00000b40: 081b 007d 0a7c 077c 0518 007c 091b 007d  ...}.|.|...|...}
+00000b50: 0b74 006a 027c 047c 0a64 011b 0017 007c  .t.j.|.|.d.....|
+00000b60: 067c 0a85 037c 057c 0b64 011b 0017 007c  .|...|.|.d.....|
+00000b70: 077c 0b85 0366 0219 005c 027d 0c7d 0d74  .|...f...\.}.}.t
+00000b80: 037c 0074 006a 047c 0c7c 0d67 0264 0264  .|.t.j.|.|.g.d.d
+00000b90: 038d 027c 0364 0464 058d 0453 0029 0661  ...|.d.d...S.).a
+00000ba0: 2401 0000 5265 7472 6965 7665 2069 6d61  $...Retrieve ima
+00000bb0: 6765 2076 616c 7565 7320 6f66 2061 2062  ge values of a b
+00000bc0: 626f 7820 7265 7369 7a65 206f 7574 7075  box resize outpu
+00000bd0: 742e 2055 7365 6420 666f 7220 524f 492d  t. Used for ROI-
+00000be0: 416c 6967 6e0a 2020 2020 4172 6773 3a0a  Align.    Args:.
+00000bf0: 2020 2020 2020 2020 696d 673a 2041 7272          img: Arr
+00000c00: 6179 206f 6620 7368 6170 6520 5b48 2c20  ay of shape [H, 
+00000c10: 572c 202e 2e2e 5d0a 2020 2020 2020 2020  W, ...].        
+00000c20: 6262 6f78 3a20 5b79 302c 2078 302c 2079  bbox: [y0, x0, y
+00000c30: 312c 2078 315d 0a20 2020 2020 2020 206f  1, x1].        o
+00000c40: 7574 7075 745f 7368 6170 653a 205b 682c  utput_shape: [h,
+00000c50: 2077 5d0a 2020 2020 2020 2020 6f75 745f   w].        out_
+00000c60: 6f66 5f62 6f75 6e64 5f76 616c 7565 3a20  of_bound_value: 
+00000c70: 6f70 7469 6f6e 616c 2066 6c6f 6174 2063  optional float c
+00000c80: 6f6e 7374 616e 742c 2064 6566 7561 6c74  onstant, defualt
+00000c90: 2030 2e0a 2020 2020 5265 7475 726e 733a   0..    Returns:
+00000ca0: 0a20 2020 2020 2020 2076 616c 7565 733a  .        values:
+00000cb0: 205b 682c 2077 2c20 2e2e 2e5d 2c20 666c   [h, w, ...], fl
+00000cc0: 6f61 740a 2020 2020 720a 0000 0072 0700  oat.    r....r..
+00000cd0: 0000 7222 0000 0054 2902 7230 0000 0072  ..r"...T).r0...r
+00000ce0: 3900 0000 2905 720f 0000 0072 2700 0000  9...).r....r'...
+00000cf0: da05 6d67 7269 6472 3e00 0000 da05 7374  ..mgridr>.....st
+00000d00: 6163 6b29 0e72 2f00 0000 723f 0000 0072  ack).r/...r?...r
+00000d10: 4000 0000 7230 0000 00da 0279 30da 0278  @...r0.....y0..x
+00000d20: 30da 0279 31da 0278 31da 0168 da01 77da  0..y1..x1..h..w.
+00000d30: 0264 79da 0264 78da 0279 79da 0278 7872  .dy..dx..yy..xxr
+00000d40: 1600 0000 7216 0000 0072 1700 0000 da19  ....r....r......
+00000d50: 7375 625f 7069 7865 6c5f 6372 6f70 5f61  sub_pixel_crop_a
+00000d60: 6e64 5f72 6573 697a 656b 0000 0073 1a00  nd_resizek...s..
+00000d70: 0000 000d 0a01 0a01 0c01 0802 0c01 0c02  ................
+00000d80: 2e01 0201 0201 1001 0201 02fc 724d 0000  ............rM..
+00000d90: 0029 0172 0100 0000 2902 7201 0000 0046  .).r....).r....F
+00000da0: 2901 7201 0000 0029 11da 0966 756e 6374  ).r....)...funct
+00000db0: 6f6f 6c73 7202 0000 0072 1100 0000 5a10  oolsr....r....Z.
+00000dc0: 6a61 782e 7363 6970 792e 7369 676e 616c  jax.scipy.signal
+00000dd0: 7203 0000 00da 056e 756d 7079 720f 0000  r......numpyr...
+00000de0: 00da 0b6c 6163 7373 2e74 7970 6573 da09  ...lacss.types..
+00000df0: 4172 7261 794c 696b 65da 0541 7272 6179  ArrayLike..Array
+00000e00: 7218 0000 0072 3700 0000 da05 666c 6f61  r....r7.....floa
+00000e10: 74da 0462 6f6f 6c72 3e00 0000 da05 5368  t..boolr>.....Sh
+00000e20: 6170 6572 4d00 0000 7216 0000 0072 1600  aperM...r....r..
+00000e30: 0000 7216 0000 0072 1700 0000 da08 3c6d  ..r....r......<m
+00000e40: 6f64 756c 653e 0100 0000 732e 0000 000c  odule>....s.....
+00000e50: 0208 010c 0206 0208 0310 230a 1b00 0100  ..........#.....
+00000e60: fc02 0102 0102 0102 0102 0102 fb0c 2600  ..............&.
+00000e70: ff02 0102 0002 0002 0002 0102 fe         .............
```

### Comparing `lacss-0.4.1/lacss/ops/__pycache__/locations.cpython-38.pyc` & `lacss-0.4.2/lacss/ops/__pycache__/locations.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 19:35:53 2023 UTC, .py size: 2843 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,154 +1,166 @@
-00000000: 550d 0d0a 0000 0000 99e8 9964 1b0b 0000  U..........d....
+00000000: 550d 0d0a 0000 0000 e37d ad64 c70b 0000  U........}.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
-00000030: 6401 6c00 5a00 6500 6a01 5a02 6409 6403  d.l.Z.e.j.Z.d.d.
-00000040: 6404 8401 5a03 6405 6406 8400 5a04 6407  d...Z.d.d...Z.d.
-00000050: 6408 8400 5a05 6401 5300 290a e900 0000  d...Z.d.S.).....
-00000060: 004e e700 0000 0000 00f8 3f63 0300 0000  .N........?c....
-00000070: 0000 0000 0000 0000 0e00 0000 0700 0000  ................
-00000080: 4300 0000 730c 0100 007c 015c 027d 037d  C...s....|.\.}.}
-00000090: 047c 027c 0214 007d 057c 0074 00a0 017c  .|.|...}.|.t...|
-000000a0: 01a1 0114 007d 0674 006a 0264 017c 0385  .....}.t.j.d.|..
-000000b0: 0264 017c 0485 0266 0219 0064 0217 007d  .d.|...f...d...}
-000000c0: 077c 0664 0164 0185 0264 0164 0185 0264  .|.d.d...d.d...d
-000000d0: 0164 0166 0419 007c 0718 007d 087c 087c  .d.f...|...}.|.|
-000000e0: 0814 006a 0364 0364 048d 017d 0974 00a0  ...j.d.d...}.t..
-000000f0: 047c 0664 0164 0185 0264 0164 0164 0566  .|.d.d...d.d.d.f
-00000100: 0419 0064 056b 057c 0974 0564 0683 01a1  ...d.k.|.t.d....
-00000110: 037d 0974 006a 067c 0964 0564 0764 088d  .}.t.j.|.d.d.d..
-00000120: 037d 0a74 00a0 077c 097c 0a64 05a1 037d  .}.t...|.|.d...}
-00000130: 0b7c 0b7c 056b 00a0 0874 09a1 017d 0c7c  .|.|.k...t...}.|
-00000140: 0c64 0519 0064 0164 0185 0264 0164 0185  .d...d.d...d.d..
-00000150: 0264 0166 0319 007d 0c7c 0a6a 0a64 0964  .d.f...}.|.j.d.d
-00000160: 0564 048d 0264 0a19 007d 0a74 00a0 077c  .d...d...}.t...|
-00000170: 087c 0a64 05a1 03a0 0b64 05a1 017d 0d7c  .|.d.....d...}.|
-00000180: 0da0 0c64 0364 0964 05a1 037d 0d7c 0c7c  ...d.d.d...}.|.|
-00000190: 0d66 0253 0029 0b61 5801 0000 4765 6e65  .f.S.).aX...Gene
-000001a0: 7261 7465 206c 6162 656c 7320 6173 204c  rate labels as L
-000001b0: 504e 2072 6567 7265 7373 696f 6e20 7461  PN regression ta
-000001c0: 7267 6574 730a 2020 2020 4172 6773 3a0a  rgets.    Args:.
-000001d0: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
-000001e0: 733a 205b 4e2c 2032 5d20 666c 6f61 7433  s: [N, 2] float3
-000001f0: 3220 7472 7565 206c 6f63 6174 696f 6e20  2 true location 
-00000200: 7661 6c75 6573 2e20 7363 616c 6564 2030  values. scaled 0
-00000210: 2e2e 312c 206d 6173 6b69 6e67 206f 7574  ..1, masking out
-00000220: 2069 6e76 616c 6964 2077 6974 6820 2d31   invalid with -1
-00000230: 0a20 2020 2020 2020 2074 6172 6765 745f  .        target_
-00000240: 7368 6170 653a 2028 482c 2057 2920 2069  shape: (H, W)  i
-00000250: 6e74 0a20 2020 2020 2020 2074 6872 6573  nt.        thres
-00000260: 686f 6c64 3a20 6469 7374 616e 6365 2074  hold: distance t
-00000270: 6872 6573 686f 6c64 2066 6f72 2070 6f73  hreshold for pos
-00000280: 7469 7665 206c 6162 656c 0a20 2020 2052  tive label.    R
-00000290: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-000002a0: 7363 6f72 655f 7461 7267 6574 3a20 5b48  score_target: [H
-000002b0: 2c20 572c 2031 5d20 696e 7433 320a 2020  , W, 1] int32.  
-000002c0: 2020 2020 2020 7265 6772 6573 7369 6f6e        regression
-000002d0: 5f74 6172 6765 743a 205b 482c 2057 2c20  _target: [H, W, 
-000002e0: 325d 2066 6c6f 6174 2074 656e 736f 720a  2] float tensor.
-000002f0: 2020 2020 4e67 0000 0000 0000 e03f e901      Ng.......?..
-00000300: 0000 00a9 01da 0461 7869 7372 0100 0000  .......axisr....
-00000310: da03 696e 6654 a902 7205 0000 00da 086b  ..infT..r......k
-00000320: 6565 7064 696d 73e9 0200 0000 2902 4e2e  eepdims.....).N.
-00000330: 290d da03 6a6e 70da 0561 7272 6179 da05  )...jnp..array..
-00000340: 6d67 7269 64da 0373 756d da05 7768 6572  mgrid..sum..wher
-00000350: 65da 0566 6c6f 6174 da06 6172 676d 696e  e..float..argmin
-00000360: da0f 7461 6b65 5f61 6c6f 6e67 5f61 7869  ..take_along_axi
-00000370: 73da 0661 7374 7970 65da 0369 6e74 da06  s..astype..int..
-00000380: 7265 7065 6174 da07 7371 7565 657a 65da  repeat..squeeze.
-00000390: 0974 7261 6e73 706f 7365 290e da09 6c6f  .transpose)...lo
-000003a0: 6361 7469 6f6e 73da 0c74 6172 6765 745f  cations..target_
-000003b0: 7368 6170 65da 0974 6872 6573 686f 6c64  shape..threshold
-000003c0: da06 6865 6967 6874 da05 7769 6474 685a  ..height..widthZ
-000003d0: 0c74 6872 6573 686f 6c64 5f73 715a 0e66  .threshold_sqZ.f
-000003e0: 6c61 745f 6c6f 6361 7469 6f6e 73da 046d  lat_locations..m
-000003f0: 6573 68da 0964 6973 7461 6e63 6573 5a0c  esh..distancesZ.
-00000400: 6469 7374 616e 6365 735f 7371 da07 696e  distances_sq..in
-00000410: 6469 6365 735a 0e62 6573 745f 6469 7374  dicesZ.best_dist
-00000420: 616e 6365 735a 0c73 636f 7265 5f74 6172  ancesZ.score_tar
-00000430: 6765 745a 1172 6567 7265 7373 696f 6e5f  getZ.regression_
-00000440: 7461 7267 6574 a900 721f 0000 00fa 362f  target..r.....6/
-00000450: 686f 6d65 2f46 4341 4d2f 6a79 752f 7072  home/FCAM/jyu/pr
-00000460: 6f6a 5f6c 6163 7373 2f6c 6163 7373 2f6c  oj_lacss/lacss/l
-00000470: 6163 7373 2f6f 7073 2f6c 6f63 6174 696f  acss/ops/locatio
-00000480: 6e73 2e70 79da 136c 6f63 6174 696f 6e73  ns.py..locations
-00000490: 5f74 6f5f 6c61 6265 6c73 0600 0000 732a  _to_labels....s*
-000004a0: 0000 0000 0a08 0108 020e 021a 011c 0110  ................
-000004b0: 0304 0116 0002 0006 ff04 0410 010e 010e  ................
-000004c0: 011a 0212 010e 0102 ff04 030e 0272 2100  .............r!.
-000004d0: 0000 6302 0000 0000 0000 0000 0000 0004  ..c.............
-000004e0: 0000 0005 0000 0043 0000 0073 7c00 0000  .......C...s|...
-000004f0: 7c00 6401 6401 8502 6401 6401 6401 8502  |.d.d...d.d.d...
-00000500: 6603 1900 7c01 1800 7d02 7400 a001 7c02  f...|...}.t...|.
-00000510: a101 6a02 6402 6403 8d01 7d02 6404 7c02  ..j.d.d...}.d.|.
-00000520: 6405 1700 1b00 7d03 7400 a003 7c00 6406  d.....}.t...|.d.
-00000530: 6b00 6a04 6402 6403 8d01 6401 6401 8502  k.j.d.d...d.d...
-00000540: 6401 6602 1900 6406 7c03 a103 7d03 7400  d.f...d.|...}.t.
-00000550: a003 7c01 6406 6b00 6a04 6402 6403 8d01  ..|.d.k.j.d.d...
-00000560: 6406 7c03 a103 7d03 7c03 5300 2907 610a  d.|...}.|.S.).a.
-00000570: 0100 0043 6f6d 7075 7465 2064 6973 7461  ...Compute dista
-00000580: 6e63 6520 7369 6d69 6c61 7269 7479 206d  nce similarity m
-00000590: 6174 7269 780a 2020 2020 7061 6972 7769  atrix.    pairwi
-000005a0: 7365 2073 696d 696c 6172 6974 7920 3d20  se similarity = 
-000005b0: 3120 2f20 6469 7374 616e 6365 205e 320a  1 / distance ^2.
-000005c0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000005d0: 7072 6564 5f6c 6f63 6174 696f 6e73 3a20  pred_locations: 
-000005e0: 5b4e 2c20 325d 2075 7365 202d 3120 746f  [N, 2] use -1 to
-000005f0: 206d 6173 6b20 6f75 7420 696e 7661 6c69   mask out invali
-00000600: 6420 6c6f 6361 7469 6f6e 730a 2020 2020  d locations.    
-00000610: 2020 6774 5f6c 6f63 6174 696f 6e73 3a20    gt_locations: 
-00000620: 5b4b 2c20 325d 2075 7365 202d 3120 746f  [K, 2] use -1 to
-00000630: 206d 6173 6b20 6f75 7420 696e 7661 6c69   mask out invali
-00000640: 6420 6c6f 6361 7469 6f6e 730a 2020 2020  d locations.    
-00000650: 5265 7475 726e 733a 0a20 2020 2020 2073  Returns:.      s
-00000660: 696d 696c 6172 6974 795f 6d61 7472 6978  imilarity_matrix
-00000670: 3a20 5b4e 2c20 6b5d 0a20 2020 204e e9ff  : [N, k].    N..
-00000680: ffff ff72 0400 0000 e700 0000 0000 00f0  ...r............
-00000690: 3f67 3a8c 30e2 8e79 453e 7201 0000 0029  ?g:.0..yE>r....)
-000006a0: 0572 0a00 0000 da06 7371 7561 7265 720d  .r......squarer.
-000006b0: 0000 0072 0e00 0000 da03 616c 6c29 04da  ...r......all)..
-000006c0: 0e70 7265 645f 6c6f 6361 7469 6f6e 73da  .pred_locations.
-000006d0: 0c67 745f 6c6f 6361 7469 6f6e 73da 1064  .gt_locations..d
-000006e0: 6973 7461 6e63 6573 5f6d 6174 7269 78da  istances_matrix.
-000006f0: 0273 6d72 1f00 0000 721f 0000 0072 2000  .smr....r....r .
-00000700: 0000 da13 6469 7374 616e 6365 5f73 696d  ....distance_sim
-00000710: 696c 6172 6974 792c 0000 0073 0c00 0000  ilarity,...s....
-00000720: 000a 1a01 1202 0c03 2601 1a02 722a 0000  ........&...r*..
-00000730: 0063 0300 0000 0000 0000 0000 0000 0600  .c..............
-00000740: 0000 0500 0000 4300 0000 734a 0000 0064  ......C...sJ...d
-00000750: 017c 027c 0214 001b 007d 0274 007c 007c  .|.|.....}.t.|.|
-00000760: 0183 027d 037c 036a 0164 0264 0364 048d  ...}.|.j.d.d.d..
-00000770: 027d 0474 02a0 037c 037c 0464 02a1 037c  .}.t...|.|.d...|
-00000780: 026b 047d 057c 04a0 0464 02a1 017c 05a0  .k.}.|...d...|..
-00000790: 0464 02a1 0166 0253 0029 0561 0e01 0000  .d...f.S.).a....
-000007a0: 4d61 7463 6820 7072 6564 6963 7465 6420  Match predicted 
-000007b0: 6c6f 6361 7469 6f6e 2074 6f20 6774 206c  location to gt l
-000007c0: 6f63 6174 696f 6e73 0a20 2020 2041 7267  ocations.    Arg
-000007d0: 733a 0a20 2020 2020 2070 7265 645f 6c6f  s:.      pred_lo
-000007e0: 6361 7469 6f6e 733a 7220 5b4e 2c20 325d  cations:r [N, 2]
-000007f0: 0a20 2020 2020 2067 745f 6c6f 6361 7469  .      gt_locati
-00000800: 6f6e 733a 205b 4b2c 2032 5d0a 2020 2020  ons: [K, 2].    
-00000810: 2020 7468 7265 7368 6f6c 643a 2066 6c6f    threshold: flo
-00000820: 6174 2e20 4d61 7869 6d75 6d20 6469 7374  at. Maximum dist
-00000830: 616e 6365 2074 6f20 6265 206d 6174 6368  ance to be match
-00000840: 6564 0a20 2020 2052 6574 7572 6e73 3a0a  ed.    Returns:.
-00000850: 2020 2020 2020 6d61 7463 6865 733a 205b        matches: [
-00000860: 4e5d 2c20 696e 6469 6365 7320 6f66 2074  N], indices of t
-00000870: 6865 206d 6174 6368 6573 206c 6f63 6174  he matches locat
-00000880: 696f 6e20 696e 2067 7420 6c69 7374 0a20  ion in gt list. 
-00000890: 2020 2020 2069 6e64 6963 6174 6f72 733a       indicators:
-000008a0: 205b 4e5d 2062 6f6f 6c0a 2020 2020 7223   [N] bool.    r#
-000008b0: 0000 0072 2200 0000 5472 0700 0000 2905  ...r"...Tr....).
-000008c0: 722a 0000 00da 0661 7267 6d61 7872 0a00  r*.....argmaxr..
-000008d0: 0000 7211 0000 0072 1500 0000 2906 7226  ..r....r....).r&
-000008e0: 0000 0072 2700 0000 7219 0000 0072 2800  ...r'...r....r(.
-000008f0: 0000 da07 6d61 7463 6865 73da 0a69 6e64  ....matches..ind
-00000900: 6963 6174 6f72 7372 1f00 0000 721f 0000  icatorsr....r...
-00000910: 0072 2000 0000 da11 6c6f 6361 7469 6f6e  .r .....location
-00000920: 5f6d 6174 6368 696e 6742 0000 0073 0a00  _matchingB...s..
-00000930: 0000 000b 0c02 0a02 0e01 1202 722e 0000  ............r...
-00000940: 0029 0172 0200 0000 2906 da03 6a61 78da  .).r....)...jax.
-00000950: 056e 756d 7079 720a 0000 0072 2100 0000  .numpyr....r!...
-00000960: 722a 0000 0072 2e00 0000 721f 0000 0072  r*...r....r....r
-00000970: 1f00 0000 721f 0000 0072 2000 0000 da08  ....r....r .....
-00000980: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
-00000990: 0008 0206 030a 2608 16                   ......&..
+00000020: 0007 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
+00000030: 6401 6c00 5a00 6500 6a01 5a02 6400 6402  d.l.Z.e.j.Z.d.d.
+00000040: 6c03 5400 640d 6504 6505 6506 6507 6508  l.T.d.e.e.e.e.e.
+00000050: 6508 6602 1900 6404 9c04 6405 6406 8405  e.f...d...d.d...
+00000060: 5a09 6504 6504 6508 6407 9c03 6408 6409  Z.e.e.e.d...d.d.
+00000070: 8404 5a0a 6504 6504 6506 6507 6508 6508  ..Z.e.e.e.e.e.e.
+00000080: 6602 1900 640a 9c04 640b 640c 8404 5a0b  f...d...d.d...Z.
+00000090: 6401 5300 290e e900 0000 004e 2901 da01  d.S.)......N)...
+000000a0: 2ae7 0000 0000 0000 f83f 2904 da09 6c6f  *........?)...lo
+000000b0: 6361 7469 6f6e 73da 0c74 6172 6765 745f  cations..target_
+000000c0: 7368 6170 65da 0974 6872 6573 686f 6c64  shape..threshold
+000000d0: da06 7265 7475 726e 6303 0000 0000 0000  ..returnc.......
+000000e0: 0000 0000 000e 0000 0007 0000 0043 0000  .............C..
+000000f0: 0073 0c01 0000 7c01 5c02 7d03 7d04 7c02  .s....|.\.}.}.|.
+00000100: 7c02 1400 7d05 7c00 7400 a001 7c01 a101  |...}.|.t...|...
+00000110: 1400 7d06 7400 6a02 6401 7c03 8502 6401  ..}.t.j.d.|...d.
+00000120: 7c04 8502 6602 1900 6402 1700 7d07 7c06  |...f...d...}.|.
+00000130: 6401 6401 8502 6401 6401 8502 6401 6401  d.d...d.d...d.d.
+00000140: 6604 1900 7c07 1800 7d08 7c08 7c08 1400  f...|...}.|.|...
+00000150: 6a03 6403 6404 8d01 7d09 7400 a004 7c06  j.d.d...}.t...|.
+00000160: 6401 6401 8502 6401 6401 6405 6604 1900  d.d...d.d.d.f...
+00000170: 6405 6b05 7c09 7405 6406 8301 a103 7d09  d.k.|.t.d.....}.
+00000180: 7400 6a06 7c09 6405 6407 6408 8d03 7d0a  t.j.|.d.d.d...}.
+00000190: 7400 a007 7c09 7c0a 6405 a103 7d0b 7c0b  t...|.|.d...}.|.
+000001a0: 7c05 6b00 a008 7409 a101 7d0c 7c0c 6405  |.k...t...}.|.d.
+000001b0: 1900 6401 6401 8502 6401 6401 8502 6401  ..d.d...d.d...d.
+000001c0: 6603 1900 7d0c 7c0a 6a0a 6409 6405 6404  f...}.|.j.d.d.d.
+000001d0: 8d02 640a 1900 7d0a 7400 a007 7c08 7c0a  ..d...}.t...|.|.
+000001e0: 6405 a103 a00b 6405 a101 7d0d 7c0d a00c  d.....d...}.|...
+000001f0: 6403 6409 6405 a103 7d0d 7c0c 7c0d 6602  d.d.d...}.|.|.f.
+00000200: 5300 290b 6158 0100 0047 656e 6572 6174  S.).aX...Generat
+00000210: 6520 6c61 6265 6c73 2061 7320 4c50 4e20  e labels as LPN 
+00000220: 7265 6772 6573 7369 6f6e 2074 6172 6765  regression targe
+00000230: 7473 0a20 2020 2041 7267 733a 0a20 2020  ts.    Args:.   
+00000240: 2020 2020 206c 6f63 6174 696f 6e73 3a20       locations: 
+00000250: 5b4e 2c20 325d 2066 6c6f 6174 3332 2074  [N, 2] float32 t
+00000260: 7275 6520 6c6f 6361 7469 6f6e 2076 616c  rue location val
+00000270: 7565 732e 2073 6361 6c65 6420 302e 2e31  ues. scaled 0..1
+00000280: 2c20 6d61 736b 696e 6720 6f75 7420 696e  , masking out in
+00000290: 7661 6c69 6420 7769 7468 202d 310a 2020  valid with -1.  
+000002a0: 2020 2020 2020 7461 7267 6574 5f73 6861        target_sha
+000002b0: 7065 3a20 2848 2c20 5729 2020 696e 740a  pe: (H, W)  int.
+000002c0: 2020 2020 2020 2020 7468 7265 7368 6f6c          threshol
+000002d0: 643a 2064 6973 7461 6e63 6520 7468 7265  d: distance thre
+000002e0: 7368 6f6c 6420 666f 7220 706f 7374 6976  shold for postiv
+000002f0: 6520 6c61 6265 6c0a 2020 2020 5265 7475  e label.    Retu
+00000300: 726e 733a 0a20 2020 2020 2020 2073 636f  rns:.        sco
+00000310: 7265 5f74 6172 6765 743a 205b 482c 2057  re_target: [H, W
+00000320: 2c20 315d 2069 6e74 3332 0a20 2020 2020  , 1] int32.     
+00000330: 2020 2072 6567 7265 7373 696f 6e5f 7461     regression_ta
+00000340: 7267 6574 3a20 5b48 2c20 572c 2032 5d20  rget: [H, W, 2] 
+00000350: 666c 6f61 7420 7465 6e73 6f72 0a20 2020  float tensor.   
+00000360: 204e 6700 0000 0000 00e0 3fe9 0100 0000   Ng.......?.....
+00000370: a901 da04 6178 6973 7201 0000 00da 0369  ....axisr......i
+00000380: 6e66 54a9 0272 0a00 0000 da08 6b65 6570  nfT..r......keep
+00000390: 6469 6d73 e902 0000 0029 024e 2e29 0dda  dims.....).N.)..
+000003a0: 036a 6e70 da05 6172 7261 79da 056d 6772  .jnp..array..mgr
+000003b0: 6964 da03 7375 6dda 0577 6865 7265 da05  id..sum..where..
+000003c0: 666c 6f61 74da 0661 7267 6d69 6eda 0f74  float..argmin..t
+000003d0: 616b 655f 616c 6f6e 675f 6178 6973 da06  ake_along_axis..
+000003e0: 6173 7479 7065 da03 696e 74da 0672 6570  astype..int..rep
+000003f0: 6561 74da 0773 7175 6565 7a65 da09 7472  eat..squeeze..tr
+00000400: 616e 7370 6f73 6529 0e72 0400 0000 7205  anspose).r....r.
+00000410: 0000 0072 0600 0000 da06 6865 6967 6874  ...r......height
+00000420: da05 7769 6474 685a 0c74 6872 6573 686f  ..widthZ.thresho
+00000430: 6c64 5f73 715a 0e66 6c61 745f 6c6f 6361  ld_sqZ.flat_loca
+00000440: 7469 6f6e 73da 046d 6573 68da 0964 6973  tions..mesh..dis
+00000450: 7461 6e63 6573 5a0c 6469 7374 616e 6365  tancesZ.distance
+00000460: 735f 7371 da07 696e 6469 6365 735a 0e62  s_sq..indicesZ.b
+00000470: 6573 745f 6469 7374 616e 6365 735a 0c73  est_distancesZ.s
+00000480: 636f 7265 5f74 6172 6765 745a 1172 6567  core_targetZ.reg
+00000490: 7265 7373 696f 6e5f 7461 7267 6574 a900  ression_target..
+000004a0: 7221 0000 00fa 362f 686f 6d65 2f46 4341  r!....6/home/FCA
+000004b0: 4d2f 6a79 752f 7072 6f6a 5f6c 6163 7373  M/jyu/proj_lacss
+000004c0: 2f6c 6163 7373 2f6c 6163 7373 2f6f 7073  /lacss/lacss/ops
+000004d0: 2f6c 6f63 6174 696f 6e73 2e70 79da 136c  /locations.py..l
+000004e0: 6f63 6174 696f 6e73 5f74 6f5f 6c61 6265  ocations_to_labe
+000004f0: 6c73 0800 0000 732a 0000 0000 0c08 0108  ls....s*........
+00000500: 020e 021a 011c 0110 0304 0116 0002 0006  ................
+00000510: ff04 0410 010e 010e 011a 0212 010e 0102  ................
+00000520: ff04 030e 0272 2300 0000 2903 da0e 7072  .....r#...)...pr
+00000530: 6564 5f6c 6f63 6174 696f 6e73 da0c 6774  ed_locations..gt
+00000540: 5f6c 6f63 6174 696f 6e73 7207 0000 0063  _locationsr....c
+00000550: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+00000560: 0500 0000 4300 0000 737c 0000 007c 0064  ....C...s|...|.d
+00000570: 0164 0185 0264 0164 0164 0185 0266 0319  .d...d.d.d...f..
+00000580: 007c 0118 007d 0274 00a0 017c 02a1 016a  .|...}.t...|...j
+00000590: 0264 0264 038d 017d 0264 047c 0264 0517  .d.d...}.d.|.d..
+000005a0: 001b 007d 0374 00a0 037c 0064 066b 006a  ...}.t...|.d.k.j
+000005b0: 0464 0264 038d 0164 0164 0185 0264 0166  .d.d...d.d...d.f
+000005c0: 0219 0064 067c 03a1 037d 0374 00a0 037c  ...d.|...}.t...|
+000005d0: 0164 066b 006a 0464 0264 038d 0164 067c  .d.k.j.d.d...d.|
+000005e0: 03a1 037d 037c 0353 0029 0761 0a01 0000  ...}.|.S.).a....
+000005f0: 436f 6d70 7574 6520 6469 7374 616e 6365  Compute distance
+00000600: 2073 696d 696c 6172 6974 7920 6d61 7472   similarity matr
+00000610: 6978 0a20 2020 2070 6169 7277 6973 6520  ix.    pairwise 
+00000620: 7369 6d69 6c61 7269 7479 203d 2031 202f  similarity = 1 /
+00000630: 2064 6973 7461 6e63 6520 5e32 0a20 2020   distance ^2.   
+00000640: 2041 7267 733a 0a20 2020 2020 2070 7265   Args:.      pre
+00000650: 645f 6c6f 6361 7469 6f6e 733a 205b 4e2c  d_locations: [N,
+00000660: 2032 5d20 7573 6520 2d31 2074 6f20 6d61   2] use -1 to ma
+00000670: 736b 206f 7574 2069 6e76 616c 6964 206c  sk out invalid l
+00000680: 6f63 6174 696f 6e73 0a20 2020 2020 2067  ocations.      g
+00000690: 745f 6c6f 6361 7469 6f6e 733a 205b 4b2c  t_locations: [K,
+000006a0: 2032 5d20 7573 6520 2d31 2074 6f20 6d61   2] use -1 to ma
+000006b0: 736b 206f 7574 2069 6e76 616c 6964 206c  sk out invalid l
+000006c0: 6f63 6174 696f 6e73 0a20 2020 2052 6574  ocations.    Ret
+000006d0: 7572 6e73 3a0a 2020 2020 2020 7369 6d69  urns:.      simi
+000006e0: 6c61 7269 7479 5f6d 6174 7269 783a 205b  larity_matrix: [
+000006f0: 4e2c 206b 5d0a 2020 2020 4ee9 ffff ffff  N, k].    N.....
+00000700: 7209 0000 00e7 0000 0000 0000 f03f 673a  r............?g:
+00000710: 8c30 e28e 7945 3e72 0100 0000 2905 720f  .0..yE>r....).r.
+00000720: 0000 00da 0673 7175 6172 6572 1200 0000  .....squarer....
+00000730: 7213 0000 00da 0361 6c6c 2904 7224 0000  r......all).r$..
+00000740: 0072 2500 0000 da10 6469 7374 616e 6365  .r%.....distance
+00000750: 735f 6d61 7472 6978 da02 736d 7221 0000  s_matrix..smr!..
+00000760: 0072 2100 0000 7222 0000 00da 1364 6973  .r!...r".....dis
+00000770: 7461 6e63 655f 7369 6d69 6c61 7269 7479  tance_similarity
+00000780: 3000 0000 730c 0000 0000 0a1a 0112 020c  0...s...........
+00000790: 0326 011a 0272 2c00 0000 2904 7224 0000  .&...r,...).r$..
+000007a0: 0072 2500 0000 7206 0000 0072 0700 0000  .r%...r....r....
+000007b0: 6303 0000 0000 0000 0000 0000 0006 0000  c...............
+000007c0: 0005 0000 0043 0000 0073 4a00 0000 6401  .....C...sJ...d.
+000007d0: 7c02 7c02 1400 1b00 7d02 7400 7c00 7c01  |.|.....}.t.|.|.
+000007e0: 8302 7d03 7c03 6a01 6402 6403 6404 8d02  ..}.|.j.d.d.d...
+000007f0: 7d04 7402 a003 7c03 7c04 6402 a103 7c02  }.t...|.|.d...|.
+00000800: 6b04 7d05 7c04 a004 6402 a101 7c05 a004  k.}.|...d...|...
+00000810: 6402 a101 6602 5300 2905 610e 0100 004d  d...f.S.).a....M
+00000820: 6174 6368 2070 7265 6469 6374 6564 206c  atch predicted l
+00000830: 6f63 6174 696f 6e20 746f 2067 7420 6c6f  ocation to gt lo
+00000840: 6361 7469 6f6e 730a 2020 2020 4172 6773  cations.    Args
+00000850: 3a0a 2020 2020 2020 7072 6564 5f6c 6f63  :.      pred_loc
+00000860: 6174 696f 6e73 3a72 205b 4e2c 2032 5d0a  ations:r [N, 2].
+00000870: 2020 2020 2020 6774 5f6c 6f63 6174 696f        gt_locatio
+00000880: 6e73 3a20 5b4b 2c20 325d 0a20 2020 2020  ns: [K, 2].     
+00000890: 2074 6872 6573 686f 6c64 3a20 666c 6f61   threshold: floa
+000008a0: 742e 204d 6178 696d 756d 2064 6973 7461  t. Maximum dista
+000008b0: 6e63 6520 746f 2062 6520 6d61 7463 6865  nce to be matche
+000008c0: 640a 2020 2020 5265 7475 726e 733a 0a20  d.    Returns:. 
+000008d0: 2020 2020 206d 6174 6368 6573 3a20 5b4e       matches: [N
+000008e0: 5d2c 2069 6e64 6963 6573 206f 6620 7468  ], indices of th
+000008f0: 6520 6d61 7463 6865 7320 6c6f 6361 7469  e matches locati
+00000900: 6f6e 2069 6e20 6774 206c 6973 740a 2020  on in gt list.  
+00000910: 2020 2020 696e 6469 6361 746f 7273 3a20      indicators: 
+00000920: 5b4e 5d20 626f 6f6c 0a20 2020 2072 2700  [N] bool.    r'.
+00000930: 0000 7226 0000 0054 720c 0000 0029 0572  ..r&...Tr....).r
+00000940: 2c00 0000 da06 6172 676d 6178 720f 0000  ,.....argmaxr...
+00000950: 0072 1600 0000 721a 0000 0029 0672 2400  .r....r....).r$.
+00000960: 0000 7225 0000 0072 0600 0000 722a 0000  ..r%...r....r*..
+00000970: 00da 076d 6174 6368 6573 da0a 696e 6469  ...matches..indi
+00000980: 6361 746f 7273 7221 0000 0072 2100 0000  catorsr!...r!...
+00000990: 7222 0000 00da 116c 6f63 6174 696f 6e5f  r".....location_
+000009a0: 6d61 7463 6869 6e67 4600 0000 730a 0000  matchingF...s...
+000009b0: 0000 0d0c 020a 020e 0112 0272 3000 0000  ...........r0...
+000009c0: 2901 7203 0000 0029 0cda 036a 6178 da05  ).r....)...jax..
+000009d0: 6e75 6d70 7972 0f00 0000 da0b 6c61 6373  numpyr......lacs
+000009e0: 732e 7479 7065 73da 0941 7272 6179 4c69  s.types..ArrayLi
+000009f0: 6b65 da05 5368 6170 6572 1400 0000 da05  ke..Shaper......
+00000a00: 5475 706c 65da 0541 7272 6179 7223 0000  Tuple..Arrayr#..
+00000a10: 0072 2c00 0000 7230 0000 0072 2100 0000  .r,...r0...r!...
+00000a20: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
+00000a30: 083c 6d6f 6475 6c65 3e01 0000 0073 1e00  .<module>....s..
+00000a40: 0000 0802 0602 0804 00ff 0201 0200 0200  ................
+00000a50: 0201 0afe 0c28 1217 0200 0200 0201 0afe  .....(..........
```

### Comparing `lacss-0.4.1/lacss/ops/__pycache__/masks.cpython-38.pyc` & `lacss-0.4.2/lacss/ops/__pycache__/masks.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 5967 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 4f17 0000  U........E.dO...
+00000000: 550d 0d0a 0000 0000 5a80 9c64 4f17 0000  U.......Z..dO...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6402 6404 6c03 6d04 5a04 0100 6500  ..d.d.l.m.Z...e.
 00000050: 6a05 5a06 4700 6405 6406 8400 6406 8302  j.Z.G.d.d...d...
 00000060: 5a07 6407 6408 8400 5a08 6409 640a 8400  Z.d.d...Z.d.d...
 00000070: 5a09 640b 640c 8400 5a0a 640d 640e 8400  Z.d.d...Z.d.d...
@@ -304,23 +304,23 @@
 000012f0: 6800 0000 720e 0000 00da 086d 6f76 6561  h...r......movea
 00001300: 7869 7372 0f00 0000 da07 7371 7565 657a  xisr......squeez
 00001310: 65da 0d63 6f75 6e74 5f6e 6f6e 7a65 726f  e..count_nonzero
 00001320: da0a 7a65 726f 735f 6c69 6b65 7254 0000  ..zeros_likerT..
 00001330: 0072 3000 0000 7234 0000 0029 0dda 0867  .r0...r4...)...g
 00001340: 745f 6c61 6265 6c72 5800 0000 da04 7072  t_labelrX.....pr
 00001350: 6564 7259 0000 005a 0969 7473 5f74 6162  edrY...Z.its_tab
-00001360: 6c65 5a06 6774 5f69 6473 5a08 7072 6564  leZ.gt_idsZ.pred
+00001360: 6c65 da06 6774 5f69 6473 da08 7072 6564  le..gt_ids..pred
 00001370: 5f69 6473 5a0c 7072 6564 5f70 6174 6368  _idsZ.pred_patch
 00001380: 6573 5a03 7963 735a 0378 6373 5a0a 6774  esZ.ycsZ.xcsZ.gt
 00001390: 5f70 6174 6368 6573 da03 6974 7372 4f00  _patches..itsrO.
 000013a0: 0000 720a 0000 0072 0a00 0000 720b 0000  ..r....r....r...
 000013b0: 00da 0f6d 6173 6b5f 696e 7465 7273 6563  ...mask_intersec
 000013c0: 7473 8e00 0000 731a 0000 0000 0108 010a  ts....s.........
 000013d0: 0118 020c 010c 0108 020c 010c 0122 0212  ............."..
-000013e0: 0210 0114 0272 7400 0000 6303 0000 0000  .....rt...c.....
+000013e0: 0210 0114 0272 7600 0000 6303 0000 0000  .....rv...c.....
 000013f0: 0000 0000 0000 0009 0000 0007 0000 0043  ...............C
 00001400: 0000 0073 8400 0000 7c00 a000 a100 7d03  ...s....|.....}.
 00001410: 7401 6a02 7c00 7401 a003 6401 7c03 6401  t.j.|.t...d.|.d.
 00001420: 1700 a102 6402 6402 8502 6402 6402 6603  ....d.d...d.d.f.
 00001430: 1900 6b02 6403 6404 8d02 7d04 7401 6a02  ..k.d.d...}.t.j.
 00001440: 7c02 6405 1900 6406 6b05 6403 6404 8d02  |.d...d.k.d.d...
 00001450: 7d05 7c04 6402 6402 8502 6402 6602 1900  }.|.d.d...d.f...
@@ -340,24 +340,24 @@
 00001530: 7369 6d69 6c61 7269 7479 5f6d 6174 7269  similarity_matri
 00001540: 783a 2054 656e 736f 7220 2866 6c6f 6174  x: Tensor (float
 00001550: 3332 2920 5b6e 5f70 7265 645f 6d61 736b  32) [n_pred_mask
 00001560: 732c 206e 5f67 745f 6d61 736b 735d 0a20  s, n_gt_masks]. 
 00001570: 2020 2072 0200 0000 4e72 4800 0000 7221     r....NrH...r!
 00001580: 0000 0072 6900 0000 726a 0000 0072 4900  ...ri...rj...rI.
 00001590: 0000 2906 da03 6d61 7872 0e00 0000 726f  ..)...maxr....ro
-000015a0: 0000 0072 2400 0000 7274 0000 0072 3b00  ...r$...rt...r;.
+000015a0: 0000 0072 2400 0000 7276 0000 0072 3b00  ...r$...rv...r;.
 000015b0: 0000 2909 7271 0000 0072 5800 0000 7272  ..).rq...rX...rr
-000015c0: 0000 005a 086e 5f6c 6162 656c 735a 0867  ...Z.n_labelsZ.g
-000015d0: 745f 6172 6561 735a 0a70 7265 645f 6172  t_areasZ.pred_ar
+000015c0: 0000 005a 086e 5f6c 6162 656c 73da 0867  ...Z.n_labels..g
+000015d0: 745f 6172 6561 73da 0a70 7265 645f 6172  t_areas..pred_ar
 000015e0: 6561 735a 0973 756d 5f61 7265 6173 724f  easZ.sum_areasrO
 000015f0: 0000 00da 0469 6f75 7372 0a00 0000 720a  .....iousr....r.
 00001600: 0000 0072 0b00 0000 da09 6d61 736b 5f69  ...r......mask_i
 00001610: 6f75 73a3 0000 0073 1400 0000 0009 0801  ous....s........
 00001620: 0401 2000 02ff 0603 1601 1401 0c01 1002  .. .............
-00001630: 7277 0000 0029 0c72 3800 0000 da05 626f  rw...).r8.....bo
+00001630: 727b 0000 0029 0c72 3800 0000 da05 626f  r{...).r8.....bo
 00001640: 7865 7372 0300 0000 7236 0000 0072 0400  xesr....r6...r..
 00001650: 0000 da05 6e75 6d70 7972 0e00 0000 7205  ....numpyr....r.
-00001660: 0000 0072 5100 0000 7268 0000 0072 7400  ...rQ...rh...rt.
-00001670: 0000 7277 0000 0072 0a00 0000 720a 0000  ..rw...r....r...
+00001660: 0000 0072 5100 0000 7268 0000 0072 7600  ...rQ...rh...rv.
+00001670: 0000 727b 0000 0072 0a00 0000 720a 0000  ..r{...r....r...
 00001680: 0072 0a00 0000 720b 0000 00da 083c 6d6f  .r....r......<mo
 00001690: 6475 6c65 3e01 0000 0073 1000 0000 0802  dule>....s......
 000016a0: 0c01 0c02 0603 0e48 082b 0812 0815       .......H.+....
```

### Comparing `lacss-0.4.1/lacss/ops/__pycache__/nms.cpython-38.pyc` & `lacss-0.4.2/lacss/ops/__pycache__/nms.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 19:35:53 2023 UTC, .py size: 4732 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,243 +1,266 @@
-00000000: 550d 0d0a 0000 0000 99e8 9964 7c12 0000  U..........d|...
+00000000: 550d 0d0a 0000 0000 f181 ad64 ed14 0000  U..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
+00000020: 0009 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 5a02 6403 6404 6c03 6d04 5a04 0100 6403  Z.d.d.l.m.Z...d.
-00000050: 6405 6c05 6d06 5a06 0100 6502 6a07 5a08  d.l.m.Z...e.j.Z.
-00000060: 6406 5a09 6407 6408 8400 5a0a 6409 640a  d.Z.d.d...Z.d.d.
-00000070: 8400 5a0b 640f 650c 650d 650d 640c 9c03  ..Z.d.e.e.e.d...
-00000080: 640d 640e 8405 5a0e 6402 5300 2910 e900  d.d...Z.d.S.)...
-00000090: 0000 0029 01da 0843 616c 6c61 626c 654e  ...)...CallableN
-000000a0: e901 0000 0029 01da 1262 6f78 5f69 6f75  .....)...box_iou
-000000b0: 5f73 696d 696c 6172 6974 7929 01da 1364  _similarity)...d
-000000c0: 6973 7461 6e63 655f 7369 6d69 6c61 7269  istance_similari
-000000d0: 7479 6900 0200 0063 0200 0000 0000 0000  tyi....c........
-000000e0: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
-000000f0: 731a 0000 0074 00a0 017c 0164 0064 0085  s....t...|.d.d..
-00000100: 0264 0066 0219 0064 017c 00a1 0353 00a9  .d.f...d.|...S..
-00000110: 024e e9ff ffff ff29 02da 036a 6e70 da05  .N.....)...jnp..
-00000120: 7768 6572 6529 02da 0562 6f78 6573 da04  where)...boxes..
-00000130: 6d61 736b a900 720c 0000 00fa 302f 686f  mask..r.....0/ho
-00000140: 6d65 2f46 4341 4d2f 6a79 752f 7072 6f6a  me/FCAM/jyu/proj
-00000150: 5f6c 6163 7373 2f6c 6163 7373 2f6c 6163  _lacss/lacss/lac
-00000160: 7373 2f6f 7073 2f6e 6d73 2e70 79da 095f  ss/ops/nms.py.._
-00000170: 7375 7070 7265 7373 0d00 0000 7302 0000  suppress....s...
-00000180: 0000 0172 0e00 0000 6301 0000 0000 0000  ...r....c.......
-00000190: 0000 0000 000a 0000 0006 0000 0003 0000  ................
-000001a0: 0073 f600 0000 7c00 5c04 7d01 8900 7d02  .s....|.\.}...}.
-000001b0: 8902 8800 7c01 1900 7d03 8800 6a00 6401  ....|...}...j.d.
-000001c0: 1900 6402 6b02 7226 7401 6e02 7402 8901  ..d.k.r&t.n.t...
-000001d0: 8700 8701 8702 6603 6403 6404 8408 7d04  ......f.d.d...}.
-000001e0: 7403 6a04 a005 6405 7c01 7c04 7c03 a104  t.j...d.|.|.|...
-000001f0: 7d03 8801 7c03 7c03 8302 7d05 7406 a007  }...|.|...}.t...
-00000200: 7408 a101 a009 6406 6401 6702 a101 7406  t.....d.d.g...t.
-00000210: a007 7408 a101 a009 6401 6406 6702 a101  ..t.....d.d.g...
-00000220: 6b04 7d06 7c06 7c05 8802 6b04 4000 7d06  k.}.|.|...k.@.}.
-00000230: 6407 6408 8400 7d07 6409 640a 8400 7d08  d.d...}.d.d...}.
-00000240: 7403 6a04 a00a 7c08 7c07 7c06 6405 6602  t.j...|.|.|.d.f.
-00000250: a103 5c02 7d06 7d09 740b 7c03 7c06 6a0c  ..\.}.}.t.|.|.j.
-00000260: 6405 640b 8d01 8302 7d03 8800 6a0d 7c01  d.d.....}...j.|.
-00000270: 1900 a00e 7c03 a101 8900 7c02 7406 a00f  ....|.....|.t...
-00000280: 7c03 6405 6b05 6a0c 6401 640b 8d01 a101  |.d.k.j.d.d.....
-00000290: 3700 7d02 8800 7c02 6602 5300 290c 6157  7.}...|.f.S.).aW
-000002a0: 0100 0050 726f 6365 7373 2062 6f78 6573  ...Process boxes
-000002b0: 2069 6e20 7468 6520 7261 6e67 6520 5b69   in the range [i
-000002c0: 6478 2a4e 4d53 5f54 494c 455f 5349 5a45  dx*NMS_TILE_SIZE
-000002d0: 2c20 2869 6478 2b31 292a 4e4d 535f 5449  , (idx+1)*NMS_TI
-000002e0: 4c45 5f53 495a 4529 2e0a 2020 2020 4172  LE_SIZE)..    Ar
-000002f0: 6773 3a0a 2020 2020 2020 2020 696e 7075  gs:.        inpu
-00000300: 7473 3a20 7475 706c 650a 2020 2020 2020  ts: tuple.      
-00000310: 2020 2020 2020 6964 783a 2063 7572 7265        idx: curre
-00000320: 6e74 2073 6c69 6365 0a20 2020 2020 2020  nt slice.       
-00000330: 2020 2020 2062 6f78 6573 3a20 6120 7465       boxes: a te
-00000340: 6e73 6f72 2077 6974 6820 6120 7368 6170  nsor with a shap
-00000350: 6520 6f66 205b 4e2c 2034 5d2e 0a20 2020  e of [N, 4]..   
-00000360: 2020 2020 2020 2020 206e 756d 5f73 656c           num_sel
-00000370: 6563 7465 643a 206e 756d 6265 7220 6f66  ected: number of
-00000380: 2073 656c 6563 7465 6420 626f 7865 7320   selected boxes 
-00000390: 736f 2066 6172 0a20 2020 2020 2020 2020  so far.         
-000003a0: 2020 2074 6872 6573 686f 6c64 3a20 666c     threshold: fl
-000003b0: 6f61 740a 2020 2020 5265 7475 726e 733a  oat.    Returns:
-000003c0: 0a20 2020 2020 2020 2062 6f78 6573 3a20  .        boxes: 
-000003d0: 7570 6461 7465 640a 2020 2020 2020 2020  updated.        
-000003e0: 6e75 6d5f 7365 6c65 6374 6564 3a20 7570  num_selected: up
-000003f0: 6461 7465 640a 2020 2020 7207 0000 00e9  dated.    r.....
-00000400: 0400 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000410: 0004 0000 0004 0000 0013 0000 0073 2a00  .............s*.
-00000420: 0000 8801 8800 7c00 1900 7c01 8302 7d02  ......|...|...}.
-00000430: 7400 6a01 7c02 8802 6b05 6401 6402 8d02  t.j.|...k.d.d...
-00000440: 7d03 7402 7c01 7c03 8302 5300 a903 4e72  }.t.|.|...S...Nr
-00000450: 0100 0000 a901 da04 6178 6973 2903 7208  ........axis).r.
-00000460: 0000 00da 0361 6e79 720e 0000 0029 04da  .....anyr....)..
-00000470: 0369 6478 da05 736c 6963 65da 0369 6f75  .idx..slice..iou
-00000480: da0a 7375 7070 7265 7373 6564 a903 720a  ..suppressed..r.
-00000490: 0000 005a 0f73 696d 696c 6172 6974 795f  ...Z.similarity_
-000004a0: 6675 6e63 da09 7468 7265 7368 6f6c 6472  func..thresholdr
-000004b0: 0c00 0000 720d 0000 00da 0e5f 666f 725f  ....r......_for_
-000004c0: 6c6f 6f70 5f66 756e 6327 0000 0073 0600  loop_func'...s..
-000004d0: 0000 0001 0e01 1201 7a2e 5f73 7570 7072  ........z._suppr
-000004e0: 6573 7369 6f6e 5f6c 6f6f 705f 626f 6479  ession_loop_body
-000004f0: 2e3c 6c6f 6361 6c73 3e2e 5f66 6f72 5f6c  .<locals>._for_l
-00000500: 6f6f 705f 6675 6e63 7201 0000 0072 0300  oop_funcr....r..
-00000510: 0000 6301 0000 0000 0000 0000 0000 0005  ..c.............
-00000520: 0000 0004 0000 0053 0000 0073 5a00 0000  .......S...sZ...
-00000530: 7c00 5c02 7d01 7d02 7400 a001 7c01 a101  |.\.}.}.t...|...
-00000540: 7d02 7c01 6a02 6401 6402 8d01 0f00 7d03  }.|.j.d.d.....}.
-00000550: 7c01 7c03 6400 6400 8502 6400 6602 1900  |.|.d.d...d.f...
-00000560: 4000 6a02 6401 6402 8d01 7d04 7c01 7c04  @.j.d.d...}.|.|.
-00000570: 6400 6400 8502 6400 6602 1900 0f00 4000  d.d...d.f.....@.
-00000580: 7d01 7c01 7c02 6602 5300 7210 0000 0029  }.|.|.f.S.r....)
-00000590: 0372 0800 0000 da0d 636f 756e 745f 6e6f  .r......count_no
-000005a0: 6e7a 6572 6f72 1300 0000 2905 da06 696e  nzeror....)...in
-000005b0: 7075 7473 720b 0000 00da 0363 6e74 da13  putsr......cnt..
-000005c0: 6361 6e5f 7375 7070 7265 7373 5f6f 7468  can_suppress_oth
-000005d0: 6572 7372 1700 0000 720c 0000 0072 0c00  ersr....r....r..
-000005e0: 0000 720d 0000 00da 105f 7768 696c 655f  ..r......_while_
-000005f0: 6c6f 6f70 5f66 756e 6335 0000 0073 0c00  loop_func5...s..
-00000600: 0000 0001 0801 0a01 0e01 1c01 1603 7a30  ..............z0
-00000610: 5f73 7570 7072 6573 7369 6f6e 5f6c 6f6f  _suppression_loo
-00000620: 705f 626f 6479 2e3c 6c6f 6361 6c73 3e2e  p_body.<locals>.
-00000630: 5f77 6869 6c65 5f6c 6f6f 705f 6675 6e63  _while_loop_func
-00000640: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00000650: 0003 0000 0053 0000 0073 1600 0000 7c00  .....S...s....|.
-00000660: 5c02 7d01 7d02 7400 a001 7c01 a101 7c02  \.}.}.t...|...|.
-00000670: 6b03 5300 2901 4e29 0272 0800 0000 721b  k.S.).N).r....r.
-00000680: 0000 0029 0372 1c00 0000 720b 0000 0072  ...).r....r....r
-00000690: 1d00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-000006a0: 0000 00da 105f 7768 696c 655f 636f 6e64  ....._while_cond
-000006b0: 5f66 756e 633f 0000 0073 0400 0000 0001  _func?...s......
-000006c0: 0801 7a30 5f73 7570 7072 6573 7369 6f6e  ..z0_suppression
-000006d0: 5f6c 6f6f 705f 626f 6479 2e3c 6c6f 6361  _loop_body.<loca
-000006e0: 6c73 3e2e 5f77 6869 6c65 5f63 6f6e 645f  ls>._while_cond_
-000006f0: 6675 6e63 7211 0000 0029 10da 0573 6861  funcr....)...sha
-00000700: 7065 7204 0000 0072 0500 0000 da03 6a61  per....r......ja
-00000710: 78da 036c 6178 da09 666f 7269 5f6c 6f6f  x..lax..fori_loo
-00000720: 7072 0800 0000 da06 6172 616e 6765 da0d  pr......arange..
-00000730: 4e4d 535f 5449 4c45 5f53 495a 45da 0772  NMS_TILE_SIZE..r
-00000740: 6573 6861 7065 da0a 7768 696c 655f 6c6f  eshape..while_lo
-00000750: 6f70 720e 0000 0072 1300 0000 da02 6174  opr....r......at
-00000760: da03 7365 7472 1b00 0000 290a 721c 0000  ..setr....).r...
-00000770: 0072 1400 0000 da0c 6e75 6d5f 7365 6c65  .r......num_sele
-00000780: 6374 6564 da09 626f 785f 736c 6963 6572  cted..box_slicer
-00000790: 1a00 0000 7216 0000 0072 0b00 0000 721f  ....r....r....r.
-000007a0: 0000 0072 2000 0000 da01 5f72 0c00 0000  ...r ....._r....
-000007b0: 7218 0000 0072 0d00 0000 da16 5f73 7570  r....r......_sup
-000007c0: 7072 6573 7369 6f6e 5f6c 6f6f 705f 626f  pression_loop_bo
-000007d0: 6479 1100 0000 7328 0000 0000 0f0c 0208  dy....s(........
-000007e0: 0214 ff02 0410 0512 030a 0116 0102 ff04  ................
-000007f0: 0206 fe06 030c 0208 0a08 0418 0112 0310  ................
-00000800: 031a 0272 2e00 0000 e700 0000 0000 00e0  ...r............
-00000810: 3f29 03da 0f6d 6178 5f6f 7574 7075 745f  ?)...max_output_
-00000820: 7369 7a65 7219 0000 00da 096d 696e 5f73  sizer......min_s
-00000830: 636f 7265 6305 0000 0000 0000 0000 0000  corec...........
-00000840: 000c 0000 000a 0000 0043 0000 0073 9601  .........C...s..
-00000850: 0000 7c01 6a00 6401 1900 7d05 7c05 6402  ..|.j.d...}.|.d.
-00000860: 6b03 7228 7c05 6403 6b03 7228 7401 6404  k.r(|.d.k.r(t.d.
-00000870: 7c05 9b00 9d02 8301 8201 7c02 6405 6b01  |.........|.d.k.
-00000880: 723a 7c01 6a00 6405 1900 7d02 7c01 6a00  r:|.j.d...}.|.j.
-00000890: 6405 1900 7d06 7402 6406 1800 7c06 6406  d...}.t.d...|.d.
-000008a0: 1800 7402 1600 1800 7d07 7403 6a04 7c01  ..t.....}.t.j.|.
-000008b0: 6405 7c07 6702 6405 6405 6702 6702 6401  d.|.g.d.d.g.g.d.
-000008c0: 6407 8d03 7d01 7403 6a04 7c00 6405 7c07  d...}.t.j.|.d.|.
-000008d0: 6702 6701 6401 6407 8d03 7d00 7c06 7c07  g.g.d.d...}.|.|.
-000008e0: 3700 7d06 7c01 a005 6401 7402 7c05 a103  7.}.|...d.t.|...
-000008f0: 7d01 6408 6409 8400 7d08 6405 7d09 7406  }.d.d...}.d.}.t.
-00000900: 7c06 7402 1a00 8301 4400 5d36 7d0a 7407  |.t.....D.]6}.t.
-00000910: 6a08 a009 7c00 7c0a 7402 1400 1900 7c04  j...|.|.t.....|.
-00000920: 6b05 7c09 7c02 6b00 4000 740a 7c08 7c0a  k.|.|.k.@.t.|.|.
-00000930: 7c01 7c09 7c03 6604 a104 5c02 7d01 7d09  |.|.|.f...\.}.}.
-00000940: 71b8 7c01 a005 6401 7c05 a102 7d01 7403  q.|...d.|...}.t.
-00000950: 6a0b 7c01 6405 6b05 6a0c 6401 640a 8d01  j.|.d.k.j.d.d...
-00000960: 7c02 6401 640b 8d03 a00d 6401 a101 7d0b  |.d.d.....d...}.
-00000970: 7403 a00e 7c0b 6405 6b05 7c00 7c0b 1900  t...|.d.k.|.|...
-00000980: 640c a103 7d00 7403 a00e 7c0b 640d 640d  d...}.t...|.d.d.
-00000990: 8502 640d 6602 1900 6405 6b05 7c01 7c0b  ..d.f...d.k.|.|.
-000009a0: 640d 640d 8502 6602 1900 640c a103 7d01  d.d...f...d...}.
-000009b0: 7c00 7c04 6b05 7d0b 7403 a00e 7c0b 7c00  |.|.k.}.t...|.|.
-000009c0: 6401 a103 7d00 7403 a00e 7c0b 640d 640d  d...}.t...|.d.d.
-000009d0: 8502 640d 6602 1900 7c01 6401 a103 7d01  ..d.f...|.d...}.
-000009e0: 7c00 7c01 6602 5300 290e 6107 0200 006e  |.|.f.S.).a....n
-000009f0: 6f6e 2d6d 6178 696d 756d 2073 7570 7072  on-maximum suppr
-00000a00: 6573 7369 6f6e 2066 6f72 2065 6974 6865  ession for eithe
-00000a10: 7220 6262 6f78 6573 206f 7220 706f 696e  r bboxes or poin
-00000a20: 7473 2e0a 2020 2020 4173 7375 6d70 7469  ts..    Assumpti
-00000a30: 6f6e 3a0a 2020 2020 2020 2020 2a20 5468  on:.        * Th
-00000a40: 6520 626f 7865 7320 6172 6520 736f 7274  e boxes are sort
-00000a50: 6564 2062 7920 7363 6f72 6573 0a20 2020  ed by scores.   
-00000a60: 2054 6865 206f 7665 7261 6c20 6465 7369   The overal desi
-00000a70: 676e 206f 6620 7468 6520 616c 676f 7269  gn of the algori
-00000a80: 7468 6d20 6973 2074 6f20 6861 6e64 6c65  thm is to handle
-00000a90: 2062 6f78 6573 2074 696c 652d 6279 2d74   boxes tile-by-t
-00000aa0: 696c 653a 0a20 2020 2041 7267 733a 0a20  ile:.    Args:. 
-00000ab0: 2020 2020 2020 2073 636f 7265 733a 205b         scores: [
-00000ac0: 4e5d 0a20 2020 2020 2020 2062 6f78 6573  N].        boxes
-00000ad0: 3a20 5b4e 2c20 435d 2020 433d 3420 666f  : [N, C]  C=4 fo
-00000ae0: 7220 626f 7865 732c 2043 3d32 2066 6f72  r boxes, C=2 for
-00000af0: 206c 6f63 6174 696f 6e73 0a20 2020 2020   locations.     
-00000b00: 2020 206d 6178 5f6f 7574 7075 745f 7369     max_output_si
-00000b10: 7a65 3a20 6120 706f 7369 7469 7665 2073  ze: a positive s
-00000b20: 6361 6c61 7220 696e 7465 6765 720a 2020  calar integer.  
-00000b30: 2020 2020 2020 7468 7265 7368 6f6c 643a        threshold:
-00000b40: 2061 2073 6361 6c61 7220 666c 6f61 742c   a scalar float,
-00000b50: 2063 616e 2062 6520 6e65 6761 7469 7665   can be negative
-00000b60: 0a20 2020 2020 2020 206d 696e 5f73 636f  .        min_sco
-00000b70: 7265 3a20 6d69 6e20 7363 6f72 6520 746f  re: min score to
-00000b80: 2062 6520 7365 6c65 6374 6564 2c20 6465   be selected, de
-00000b90: 6661 756c 7420 300a 2020 2020 5265 7475  fault 0.    Retu
-00000ba0: 726e 733a 0a20 2020 2020 2020 206e 6d73  rns:.        nms
-00000bb0: 5f73 636f 7265 733a 205b 4d5d 2e20 204d  _scores: [M].  M
-00000bc0: 203d 206d 6178 5f6f 7574 7075 745f 7369   = max_output_si
-00000bd0: 7a65 0a20 2020 2020 2020 206e 6d73 5f70  ze.        nms_p
-00000be0: 726f 706f 7361 6c73 3a20 5b4d 2c20 435d  roposals: [M, C]
-00000bf0: 2e0a 2020 2020 7207 0000 00e9 0200 0000  ..    r.........
-00000c00: 720f 0000 007a 2262 6f78 6573 2073 686f  r....z"boxes sho
-00000c10: 756c 6420 6265 204e 7834 206f 7220 4e78  uld be Nx4 or Nx
-00000c20: 322c 2067 6f74 204e 7872 0100 0000 7203  2, got Nxr....r.
-00000c30: 0000 0029 01da 0f63 6f6e 7374 616e 745f  ...)...constant_
-00000c40: 7661 6c75 6573 6301 0000 0000 0000 0000  valuesc.........
-00000c50: 0000 0005 0000 0004 0000 0053 0000 0073  ...........S...s
-00000c60: 2400 0000 7c00 5c04 7d01 7d02 7d03 7d04  $...|.\.}.}.}.}.
-00000c70: 7c02 6a00 7c01 1900 a001 6401 a101 7d02  |.j.|.....d...}.
-00000c80: 7c02 7c03 6602 5300 7206 0000 0029 0272  |.|.f.S.r....).r
-00000c90: 2900 0000 722a 0000 0029 0572 1c00 0000  )...r*...).r....
-00000ca0: 7214 0000 0072 0a00 0000 da0b 6e75 6d5f  r....r......num_
-00000cb0: 6f75 7470 7574 7372 2d00 0000 720c 0000  outputsr-...r...
-00000cc0: 0072 0c00 0000 720d 0000 00da 155f 7472  .r....r......_tr
-00000cd0: 6976 6961 6c5f 7375 7070 7265 7373 5f61  ivial_suppress_a
-00000ce0: 6c6c 7600 0000 7310 0000 0000 0602 fb02  llv...s.........
-00000cf0: 0102 0102 0102 0102 0210 017a 3973 6f72  ...........z9sor
-00000d00: 7465 645f 6e6f 6e5f 6d61 785f 7375 7070  ted_non_max_supp
-00000d10: 7265 7373 696f 6e2e 3c6c 6f63 616c 733e  ression.<locals>
-00000d20: 2e5f 7472 6976 6961 6c5f 7375 7070 7265  ._trivial_suppre
-00000d30: 7373 5f61 6c6c 7211 0000 0029 02da 0473  ss_allr....)...s
-00000d40: 697a 65da 0a66 696c 6c5f 7661 6c75 6567  ize..fill_valueg
-00000d50: 0000 0000 0000 f0bf 4e29 0f72 2100 0000  ........N).r!...
-00000d60: da0a 5661 6c75 6545 7272 6f72 7226 0000  ..ValueErrorr&..
-00000d70: 0072 0800 0000 da03 7061 6472 2700 0000  .r......padr'...
-00000d80: da05 7261 6e67 6572 2200 0000 7223 0000  ..ranger"...r#..
-00000d90: 00da 0463 6f6e 6472 2e00 0000 da08 6172  ...condr......ar
-00000da0: 6777 6865 7265 7213 0000 00da 0773 7175  gwherer......squ
-00000db0: 6565 7a65 7209 0000 0029 0cda 0673 636f  eezer....)...sco
-00000dc0: 7265 7372 0a00 0000 7230 0000 0072 1900  resr....r0...r..
-00000dd0: 0000 7231 0000 00da 0163 da09 6e75 6d5f  ..r1.....c..num_
-00000de0: 626f 7865 7372 3900 0000 7235 0000 0072  boxesr9...r5...r
-00000df0: 2b00 0000 7214 0000 00da 0873 656c 6563  +...r......selec
-00000e00: 7465 6472 0c00 0000 720c 0000 0072 0d00  tedr....r....r..
-00000e10: 0000 da1a 736f 7274 6564 5f6e 6f6e 5f6d  ....sorted_non_m
-00000e20: 6178 5f73 7570 7072 6573 7369 6f6e 4f00  ax_suppressionO.
-00000e30: 0000 7348 0000 0000 160a 0110 010e 0408  ..sH............
-00000e40: 010a 030a 0114 011c 0116 0108 010e 0208  ................
-00000e50: 0b04 0110 0106 010e 0106 ff02 0202 0102  ................
-00000e60: 010a fb0a 090c 0304 010e 0002 0002 ff06  ................
-00000e70: 0202 fe04 0316 012a 0308 010e 011a 0272  .......*.......r
-00000e80: 4200 0000 2902 722f 0000 0072 0100 0000  B...).r/...r....
-00000e90: 290f da06 7479 7069 6e67 7202 0000 0072  )...typingr....r
-00000ea0: 2200 0000 720a 0000 0072 0400 0000 da09  "...r....r......
-00000eb0: 6c6f 6361 7469 6f6e 7372 0500 0000 da05  locationsr......
-00000ec0: 6e75 6d70 7972 0800 0000 7226 0000 0072  numpyr....r&...r
-00000ed0: 0e00 0000 722e 0000 00da 0369 6e74 da05  ....r......int..
-00000ee0: 666c 6f61 7472 4200 0000 720c 0000 0072  floatrB...r....r
-00000ef0: 0c00 0000 720c 0000 0072 0d00 0000 da08  ....r....r......
-00000f00: 3c6d 6f64 756c 653e 0100 0000 731c 0000  <module>....s...
-00000f10: 000c 0208 020c 010c 0206 0204 0308 0408  ................
-00000f20: 4200 0100 fb02 0302 0102 0102 fb         B............
+00000040: 5a02 6400 6402 6c03 6d04 5a05 0100 6400  Z.d.d.l.m.Z...d.
+00000050: 6403 6c06 5400 6404 6405 6c07 6d08 5a08  d.l.T.d.d.l.m.Z.
+00000060: 0100 6404 6406 6c09 6d0a 5a0a 0100 6407  ..d.d.l.m.Z...d.
+00000070: 5a0b 6408 6409 8400 5a0c 640a 640b 8400  Z.d.d...Z.d.d...
+00000080: 5a0d 6410 650e 650e 650f 6510 6510 6511  Z.d.e.e.e.e.e.e.
+00000090: 6512 6512 6602 1900 640d 9c06 640e 640f  e.e.f...d...d.d.
+000000a0: 8405 5a13 6402 5300 2911 e900 0000 0029  ..Z.d.S.)......)
+000000b0: 01da 0843 616c 6c61 626c 654e 2901 da01  ...CallableN)...
+000000c0: 2ae9 0100 0000 2901 da12 626f 785f 696f  *.....)...box_io
+000000d0: 755f 7369 6d69 6c61 7269 7479 2901 da13  u_similarity)...
+000000e0: 6469 7374 616e 6365 5f73 696d 696c 6172  distance_similar
+000000f0: 6974 7969 0002 0000 6302 0000 0000 0000  ityi....c.......
+00000100: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
+00000110: 0073 1a00 0000 7400 a001 7c01 6400 6400  .s....t...|.d.d.
+00000120: 8502 6400 6602 1900 6401 7c00 a103 5300  ..d.f...d.|...S.
+00000130: a902 4ee9 ffff ffff 2902 da03 6a6e 70da  ..N.....)...jnp.
+00000140: 0577 6865 7265 2902 da05 626f 7865 73da  .where)...boxes.
+00000150: 046d 6173 6ba9 0072 0d00 0000 fa30 2f68  .mask..r.....0/h
+00000160: 6f6d 652f 4643 414d 2f6a 7975 2f70 726f  ome/FCAM/jyu/pro
+00000170: 6a5f 6c61 6373 732f 6c61 6373 732f 6c61  j_lacss/lacss/la
+00000180: 6373 732f 6f70 732f 6e6d 732e 7079 da09  css/ops/nms.py..
+00000190: 5f73 7570 7072 6573 730e 0000 0073 0200  _suppress....s..
+000001a0: 0000 0001 720f 0000 0063 0100 0000 0000  ....r....c......
+000001b0: 0000 0000 0000 0a00 0000 0600 0000 0300  ................
+000001c0: 0000 73f6 0000 007c 005c 047d 0189 007d  ..s....|.\.}...}
+000001d0: 0289 0288 007c 0119 007d 0388 006a 0064  .....|...}...j.d
+000001e0: 0119 0064 026b 0272 2674 016e 0274 0289  ...d.k.r&t.n.t..
+000001f0: 0187 0087 0187 0266 0364 0364 0484 087d  .......f.d.d...}
+00000200: 0474 036a 04a0 0564 057c 017c 047c 03a1  .t.j...d.|.|.|..
+00000210: 047d 0388 017c 037c 0383 027d 0574 06a0  .}...|.|...}.t..
+00000220: 0774 08a1 01a0 0964 0664 0167 02a1 0174  .t.....d.d.g...t
+00000230: 06a0 0774 08a1 01a0 0964 0164 0667 02a1  ...t.....d.d.g..
+00000240: 016b 047d 067c 067c 0588 026b 0440 007d  .k.}.|.|...k.@.}
+00000250: 0664 0764 0884 007d 0764 0964 0a84 007d  .d.d...}.d.d...}
+00000260: 0874 036a 04a0 0a7c 087c 077c 0664 0566  .t.j...|.|.|.d.f
+00000270: 02a1 035c 027d 067d 0974 0b7c 037c 066a  ...\.}.}.t.|.|.j
+00000280: 0c64 0564 0b8d 0183 027d 0388 006a 0d7c  .d.d.....}...j.|
+00000290: 0119 00a0 0e7c 03a1 0189 007c 0274 06a0  .....|.....|.t..
+000002a0: 0f7c 0364 056b 056a 0c64 0164 0b8d 01a1  .|.d.k.j.d.d....
+000002b0: 0137 007d 0288 007c 0266 0253 0029 0c61  .7.}...|.f.S.).a
+000002c0: 6101 0000 5072 6f63 6573 7320 626f 7865  a...Process boxe
+000002d0: 7320 696e 2074 6865 2072 616e 6765 205b  s in the range [
+000002e0: 6964 782a 4e4d 535f 5449 4c45 5f53 495a  idx*NMS_TILE_SIZ
+000002f0: 452c 2028 6964 782b 3129 2a4e 4d53 5f54  E, (idx+1)*NMS_T
+00000300: 494c 455f 5349 5a45 292e 0a20 2020 2041  ILE_SIZE)..    A
+00000310: 7267 733a 0a20 2020 2020 2020 2069 6e70  rgs:.        inp
+00000320: 7574 733a 2074 7570 6c65 0a20 2020 2020  uts: tuple.     
+00000330: 2020 2020 2020 2069 6478 3a20 6375 7272         idx: curr
+00000340: 656e 7420 736c 6963 650a 2020 2020 2020  ent slice.      
+00000350: 2020 2020 2020 626f 7865 733a 2061 2074        boxes: a t
+00000360: 656e 736f 7220 7769 7468 2061 2073 6861  ensor with a sha
+00000370: 7065 206f 6620 5b4e 2c20 345d 206f 7220  pe of [N, 4] or 
+00000380: 5b4e 2c20 325d 2e0a 2020 2020 2020 2020  [N, 2]..        
+00000390: 2020 2020 6e75 6d5f 7365 6c65 6374 6564      num_selected
+000003a0: 3a20 6e75 6d62 6572 206f 6620 7365 6c65  : number of sele
+000003b0: 6374 6564 2062 6f78 6573 2073 6f20 6661  cted boxes so fa
+000003c0: 720a 2020 2020 2020 2020 2020 2020 7468  r.            th
+000003d0: 7265 7368 6f6c 643a 2066 6c6f 6174 0a20  reshold: float. 
+000003e0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+000003f0: 2020 2020 626f 7865 733a 2075 7064 6174      boxes: updat
+00000400: 6564 0a20 2020 2020 2020 206e 756d 5f73  ed.        num_s
+00000410: 656c 6563 7465 643a 2075 7064 6174 6564  elected: updated
+00000420: 0a20 2020 2072 0800 0000 e904 0000 0063  .    r.........c
+00000430: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+00000440: 0400 0000 1300 0000 732a 0000 0088 0188  ........s*......
+00000450: 007c 0019 007c 0183 027d 0274 006a 017c  .|...|...}.t.j.|
+00000460: 0288 026b 0564 0164 028d 027d 0374 027c  ...k.d.d...}.t.|
+00000470: 017c 0383 0253 00a9 034e 7201 0000 00a9  .|...S...Nr.....
+00000480: 01da 0461 7869 7329 0372 0900 0000 da03  ...axis).r......
+00000490: 616e 7972 0f00 0000 2904 da03 6964 78da  anyr....)...idx.
+000004a0: 0573 6c69 6365 da03 696f 75da 0a73 7570  .slice..iou..sup
+000004b0: 7072 6573 7365 64a9 0372 0b00 0000 5a0f  pressed..r....Z.
+000004c0: 7369 6d69 6c61 7269 7479 5f66 756e 63da  similarity_func.
+000004d0: 0974 6872 6573 686f 6c64 720d 0000 0072  .thresholdr....r
+000004e0: 0e00 0000 da0e 5f66 6f72 5f6c 6f6f 705f  ......_for_loop_
+000004f0: 6675 6e63 2800 0000 7306 0000 0000 010e  func(...s.......
+00000500: 0112 017a 2e5f 7375 7070 7265 7373 696f  ...z._suppressio
+00000510: 6e5f 6c6f 6f70 5f62 6f64 792e 3c6c 6f63  n_loop_body.<loc
+00000520: 616c 733e 2e5f 666f 725f 6c6f 6f70 5f66  als>._for_loop_f
+00000530: 756e 6372 0100 0000 7204 0000 0063 0100  uncr....r....c..
+00000540: 0000 0000 0000 0000 0000 0500 0000 0400  ................
+00000550: 0000 5300 0000 735a 0000 007c 005c 027d  ..S...sZ...|.\.}
+00000560: 017d 0274 00a0 017c 01a1 017d 027c 016a  .}.t...|...}.|.j
+00000570: 0264 0164 028d 010f 007d 037c 017c 0364  .d.d.....}.|.|.d
+00000580: 0064 0085 0264 0066 0219 0040 006a 0264  .d...d.f...@.j.d
+00000590: 0164 028d 017d 047c 017c 0464 0064 0085  .d...}.|.|.d.d..
+000005a0: 0264 0066 0219 000f 0040 007d 017c 017c  .d.f.....@.}.|.|
+000005b0: 0266 0253 0072 1100 0000 2903 7209 0000  .f.S.r....).r...
+000005c0: 00da 0d63 6f75 6e74 5f6e 6f6e 7a65 726f  ...count_nonzero
+000005d0: 7214 0000 0029 05da 0669 6e70 7574 7372  r....)...inputsr
+000005e0: 0c00 0000 da03 636e 74da 1363 616e 5f73  ......cnt..can_s
+000005f0: 7570 7072 6573 735f 6f74 6865 7273 7218  uppress_othersr.
+00000600: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000610: 0000 da10 5f77 6869 6c65 5f6c 6f6f 705f  ...._while_loop_
+00000620: 6675 6e63 3600 0000 730c 0000 0000 0108  func6...s.......
+00000630: 010a 010e 011c 0116 037a 305f 7375 7070  .........z0_supp
+00000640: 7265 7373 696f 6e5f 6c6f 6f70 5f62 6f64  ression_loop_bod
+00000650: 792e 3c6c 6f63 616c 733e 2e5f 7768 696c  y.<locals>._whil
+00000660: 655f 6c6f 6f70 5f66 756e 6363 0100 0000  e_loop_funcc....
+00000670: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00000680: 5300 0000 7316 0000 007c 005c 027d 017d  S...s....|.\.}.}
+00000690: 0274 00a0 017c 01a1 017c 026b 0353 00a9  .t...|...|.k.S..
+000006a0: 014e 2902 7209 0000 0072 1c00 0000 2903  .N).r....r....).
+000006b0: 721d 0000 0072 0c00 0000 721e 0000 0072  r....r....r....r
+000006c0: 0d00 0000 720d 0000 0072 0e00 0000 da10  ....r....r......
+000006d0: 5f77 6869 6c65 5f63 6f6e 645f 6675 6e63  _while_cond_func
+000006e0: 4000 0000 7304 0000 0000 0108 017a 305f  @...s........z0_
+000006f0: 7375 7070 7265 7373 696f 6e5f 6c6f 6f70  suppression_loop
+00000700: 5f62 6f64 792e 3c6c 6f63 616c 733e 2e5f  _body.<locals>._
+00000710: 7768 696c 655f 636f 6e64 5f66 756e 6372  while_cond_funcr
+00000720: 1200 0000 2910 da05 7368 6170 6572 0500  ....)...shaper..
+00000730: 0000 7206 0000 00da 036a 6178 da03 6c61  ..r......jax..la
+00000740: 78da 0966 6f72 695f 6c6f 6f70 7209 0000  x..fori_loopr...
+00000750: 00da 0661 7261 6e67 65da 0d4e 4d53 5f54  ...arange..NMS_T
+00000760: 494c 455f 5349 5a45 da07 7265 7368 6170  ILE_SIZE..reshap
+00000770: 65da 0a77 6869 6c65 5f6c 6f6f 7072 0f00  e..while_loopr..
+00000780: 0000 7214 0000 00da 0261 74da 0373 6574  ..r......at..set
+00000790: 721c 0000 0029 0a72 1d00 0000 7215 0000  r....).r....r...
+000007a0: 00da 0c6e 756d 5f73 656c 6563 7465 64da  ...num_selected.
+000007b0: 0962 6f78 5f73 6c69 6365 721b 0000 0072  .box_slicer....r
+000007c0: 1700 0000 720c 0000 0072 2000 0000 7222  ....r....r ...r"
+000007d0: 0000 00da 015f 720d 0000 0072 1900 0000  ....._r....r....
+000007e0: 720e 0000 00da 165f 7375 7070 7265 7373  r......_suppress
+000007f0: 696f 6e5f 6c6f 6f70 5f62 6f64 7912 0000  ion_loop_body...
+00000800: 0073 2800 0000 000f 0c02 0802 14ff 0204  .s(.............
+00000810: 1005 1203 0a01 1601 02ff 0402 06fe 0603  ................
+00000820: 0c02 080a 0804 1801 1203 1003 1a02 7230  ..............r0
+00000830: 0000 00e7 0000 0000 0000 e03f 2906 da06  ...........?)...
+00000840: 7363 6f72 6573 720b 0000 00da 0f6d 6178  scoresr......max
+00000850: 5f6f 7574 7075 745f 7369 7a65 721a 0000  _output_sizer...
+00000860: 00da 096d 696e 5f73 636f 7265 da06 7265  ...min_score..re
+00000870: 7475 726e 6305 0000 0000 0000 0000 0000  turnc...........
+00000880: 000b 0000 0007 0000 0003 0000 0073 8401  .............s..
+00000890: 0000 7c01 6a00 6401 1900 7d05 7c05 6402  ..|.j.d...}.|.d.
+000008a0: 6b03 7228 7c05 6403 6b03 7228 7401 6404  k.r(|.d.k.r(t.d.
+000008b0: 7c05 9b00 9d02 8301 8201 8801 6405 6b01  |...........d.k.
+000008c0: 723a 7c01 6a00 6405 1900 8901 7c01 6a00  r:|.j.d.....|.j.
+000008d0: 6405 1900 7d06 7402 6406 1800 7c06 6406  d...}.t.d...|.d.
+000008e0: 1800 7402 1600 1800 7d07 7403 6a04 7c01  ..t.....}.t.j.|.
+000008f0: 6405 7c07 6702 6405 6405 6702 6702 6401  d.|.g.d.d.g.g.d.
+00000900: 6407 8d03 7d01 7403 6a04 8803 6405 7c07  d...}.t.j...d.|.
+00000910: 6702 6701 6401 6407 8d03 8903 7c06 7c07  g.g.d.d.....|.|.
+00000920: 3700 7d06 7c01 a005 6401 7402 7c05 a103  7.}.|...d.t.|...
+00000930: 7d01 6408 6409 8400 8900 8700 8701 8702  }.d.d...........
+00000940: 8703 8704 6605 640a 640b 8408 7d08 6405  ....f.d.d...}.d.
+00000950: 7d09 7406 6a07 a008 6405 7c06 7402 1a00  }.t.j...d.|.t...
+00000960: 7c08 7c01 7c09 6602 a104 5c02 7d01 7d09  |.|.|.f...\.}.}.
+00000970: 7c01 a005 6401 7c05 a102 7d01 7403 6a09  |...d.|...}.t.j.
+00000980: 7c01 6405 6b05 6a0a 6401 640c 8d01 8801  |.d.k.j.d.d.....
+00000990: 6401 640d 8d03 a00b 6401 a101 7d0a 7403  d.d.....d...}.t.
+000009a0: a00c 7c0a 6405 6b05 8803 7c0a 1900 640e  ..|.d.k...|...d.
+000009b0: a103 8903 7403 a00c 7c0a 640f 640f 8502  ....t...|.d.d...
+000009c0: 640f 6602 1900 6405 6b05 7c01 7c0a 640f  d.f...d.k.|.|.d.
+000009d0: 640f 8502 6602 1900 640e a103 7d01 8803  d...f...d...}...
+000009e0: 8802 6b05 7d0a 7403 a00c 7c0a 8803 6401  ..k.}.t...|...d.
+000009f0: a103 8903 7403 a00c 7c0a 640f 640f 8502  ....t...|.d.d...
+00000a00: 640f 6602 1900 7c01 6401 a103 7d01 8803  d.f...|.d...}...
+00000a10: 7c01 6602 5300 2910 610c 0200 006e 6f6e  |.f.S.).a....non
+00000a20: 2d6d 6178 696d 756d 2073 7570 7072 6573  -maximum suppres
+00000a30: 7369 6f6e 2066 6f72 2065 6974 6865 7220  sion for either 
+00000a40: 6262 6f78 6573 206f 7220 706f 696e 7473  bboxes or points
+00000a50: 2e0a 0a20 2020 2041 7373 756d 7074 696f  ...    Assumptio
+00000a60: 6e3a 0a0a 2020 2020 2020 2020 2a20 5468  n:..        * Th
+00000a70: 6520 626f 7865 7320 6172 6520 736f 7274  e boxes are sort
+00000a80: 6564 2062 7920 7363 6f72 6573 0a0a 2020  ed by scores..  
+00000a90: 2020 5468 6520 6f76 6572 616c 2064 6573    The overal des
+00000aa0: 6967 6e20 6f66 2074 6865 2061 6c67 6f72  ign of the algor
+00000ab0: 6974 686d 2069 7320 746f 2068 616e 646c  ithm is to handl
+00000ac0: 6520 626f 7865 7320 7469 6c65 2d62 792d  e boxes tile-by-
+00000ad0: 7469 6c65 3a0a 0a20 2020 2041 7267 733a  tile:..    Args:
+00000ae0: 0a20 2020 2020 2020 2073 636f 7265 733a  .        scores:
+00000af0: 205b 4e5d 0a20 2020 2020 2020 2062 6f78   [N].        box
+00000b00: 6573 3a20 5b4e 2c20 435d 2020 433d 3420  es: [N, C]  C=4 
+00000b10: 666f 7220 626f 7865 732c 2043 3d32 2066  for boxes, C=2 f
+00000b20: 6f72 206c 6f63 6174 696f 6e73 0a20 2020  or locations.   
+00000b30: 2020 2020 206d 6178 5f6f 7574 7075 745f       max_output_
+00000b40: 7369 7a65 3a20 6120 706f 7369 7469 7665  size: a positive
+00000b50: 2073 6361 6c61 7220 696e 7465 6765 720a   scalar integer.
+00000b60: 2020 2020 2020 2020 7468 7265 7368 6f6c          threshol
+00000b70: 643a 2061 2073 6361 6c61 7220 666c 6f61  d: a scalar floa
+00000b80: 742c 2063 616e 2062 6520 6e65 6761 7469  t, can be negati
+00000b90: 7665 0a20 2020 2020 2020 206d 696e 5f73  ve.        min_s
+00000ba0: 636f 7265 3a20 6d69 6e20 7363 6f72 6520  core: min score 
+00000bb0: 746f 2062 6520 7365 6c65 6374 6564 2c20  to be selected, 
+00000bc0: 6465 6661 756c 7420 300a 0a20 2020 2052  default 0..    R
+00000bd0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00000be0: 6e6d 735f 7363 6f72 6573 3a20 5b4d 5d2e  nms_scores: [M].
+00000bf0: 2020 4d20 3d20 6d61 785f 6f75 7470 7574    M = max_output
+00000c00: 5f73 697a 650a 2020 2020 2020 2020 6e6d  _size.        nm
+00000c10: 735f 7072 6f70 6f73 616c 733a 205b 4d2c  s_proposals: [M,
+00000c20: 2043 5d2e 0a20 2020 2072 0800 0000 e902   C]..    r......
+00000c30: 0000 0072 1000 0000 7a22 626f 7865 7320  ...r....z"boxes 
+00000c40: 7368 6f75 6c64 2062 6520 4e78 3420 6f72  should be Nx4 or
+00000c50: 204e 7832 2c20 676f 7420 4e78 7201 0000   Nx2, got Nxr...
+00000c60: 0072 0400 0000 2901 da0f 636f 6e73 7461  .r....)...consta
+00000c70: 6e74 5f76 616c 7565 7363 0100 0000 0000  nt_valuesc......
+00000c80: 0000 0000 0000 0500 0000 0400 0000 5300  ..............S.
+00000c90: 0000 7324 0000 007c 005c 047d 017d 027d  ..s$...|.\.}.}.}
+00000ca0: 037d 047c 026a 007c 0119 00a0 0164 01a1  .}.|.j.|.....d..
+00000cb0: 017d 027c 027c 0366 0253 0072 0700 0000  .}.|.|.f.S.r....
+00000cc0: 2902 722b 0000 0072 2c00 0000 2905 721d  ).r+...r,...).r.
+00000cd0: 0000 0072 1500 0000 720b 0000 00da 0b6e  ...r....r......n
+00000ce0: 756d 5f6f 7574 7075 7473 722f 0000 0072  um_outputsr/...r
+00000cf0: 0d00 0000 720d 0000 0072 0e00 0000 da15  ....r....r......
+00000d00: 5f74 7269 7669 616c 5f73 7570 7072 6573  _trivial_suppres
+00000d10: 735f 616c 6c7e 0000 0073 1000 0000 0006  s_all~...s......
+00000d20: 02fb 0201 0201 0201 0201 0202 1001 7a39  ..............z9
+00000d30: 736f 7274 6564 5f6e 6f6e 5f6d 6178 5f73  sorted_non_max_s
+00000d40: 7570 7072 6573 7369 6f6e 2e3c 6c6f 6361  uppression.<loca
+00000d50: 6c73 3e2e 5f74 7269 7669 616c 5f73 7570  ls>._trivial_sup
+00000d60: 7072 6573 735f 616c 6c63 0200 0000 0000  press_allc......
+00000d70: 0000 0000 0000 0400 0000 0900 0000 1300  ................
+00000d80: 0000 7336 0000 007c 015c 027d 027d 0374  ..s6...|.\.}.}.t
+00000d90: 006a 01a0 0288 037c 0074 0314 0019 0088  .j.....|.t......
+00000da0: 026b 057c 0388 016b 0040 0074 0488 007c  .k.|...k.@.t...|
+00000db0: 007c 027c 0388 0466 04a1 0453 0072 2100  .|.|...f...S.r!.
+00000dc0: 0000 2905 7224 0000 0072 2500 0000 da04  ..).r$...r%.....
+00000dd0: 636f 6e64 7228 0000 0072 3000 0000 2904  condr(...r0...).
+00000de0: 7215 0000 00da 0376 616c 720b 0000 0072  r......valr....r
+00000df0: 2d00 0000 a905 7239 0000 0072 3300 0000  -.....r9...r3...
+00000e00: 7234 0000 0072 3200 0000 721a 0000 0072  r4...r2...r....r
+00000e10: 0d00 0000 720e 0000 00da 105f 696e 6e65  ....r......_inne
+00000e20: 725f 6c6f 6f70 5f66 756e 6388 0000 0073  r_loop_func....s
+00000e30: 1200 0000 0001 0801 0601 0e01 06ff 0202  ................
+00000e40: 0201 0201 0afb 7a34 736f 7274 6564 5f6e  ......z4sorted_n
+00000e50: 6f6e 5f6d 6178 5f73 7570 7072 6573 7369  on_max_suppressi
+00000e60: 6f6e 2e3c 6c6f 6361 6c73 3e2e 5f69 6e6e  on.<locals>._inn
+00000e70: 6572 5f6c 6f6f 705f 6675 6e63 7212 0000  er_loop_funcr...
+00000e80: 0029 02da 0473 697a 65da 0a66 696c 6c5f  .)...size..fill_
+00000e90: 7661 6c75 6567 0000 0000 0000 f0bf 4e29  valueg........N)
+00000ea0: 0d72 2300 0000 da0a 5661 6c75 6545 7272  .r#.....ValueErr
+00000eb0: 6f72 7228 0000 0072 0900 0000 da03 7061  orr(...r......pa
+00000ec0: 6472 2900 0000 7224 0000 0072 2500 0000  dr)...r$...r%...
+00000ed0: 7226 0000 00da 0861 7267 7768 6572 6572  r&.....argwherer
+00000ee0: 1400 0000 da07 7371 7565 657a 6572 0a00  ......squeezer..
+00000ef0: 0000 290b 7232 0000 0072 0b00 0000 7233  ..).r2...r....r3
+00000f00: 0000 0072 1a00 0000 7234 0000 00da 0163  ...r....r4.....c
+00000f10: da09 6e75 6d5f 626f 7865 7372 4100 0000  ..num_boxesrA...
+00000f20: 723d 0000 0072 2d00 0000 da08 7365 6c65  r=...r-.....sele
+00000f30: 6374 6564 720d 0000 0072 3c00 0000 720e  ctedr....r<...r.
+00000f40: 0000 00da 1a73 6f72 7465 645f 6e6f 6e5f  .....sorted_non_
+00000f50: 6d61 785f 7375 7070 7265 7373 696f 6e50  max_suppressionP
+00000f60: 0000 0073 4400 0000 001c 0a01 1001 0e04  ...sD...........
+00000f70: 0801 0a03 0a01 1401 1c01 1601 0801 0e03  ................
+00000f80: 080a 140a 0401 0601 0201 0601 0201 06fc  ................
+00000f90: 0812 0c03 0401 0e00 0200 02ff 0602 02fe  ................
+00000fa0: 0403 1601 2a03 0801 0e01 1a02 7247 0000  ....*.......rG..
+00000fb0: 0029 0272 3100 0000 7201 0000 0029 14da  .).r1...r....)..
+00000fc0: 0674 7970 696e 6772 0200 0000 7224 0000  .typingr....r$..
+00000fd0: 00da 096a 6178 2e6e 756d 7079 da05 6e75  ...jax.numpy..nu
+00000fe0: 6d70 7972 0900 0000 da0b 6c61 6373 732e  mpyr......lacss.
+00000ff0: 7479 7065 7372 0b00 0000 7205 0000 00da  typesr....r.....
+00001000: 096c 6f63 6174 696f 6e73 7206 0000 0072  .locationsr....r
+00001010: 2800 0000 720f 0000 0072 3000 0000 da09  (...r....r0.....
+00001020: 4172 7261 794c 696b 65da 0369 6e74 da05  ArrayLike..int..
+00001030: 666c 6f61 74da 0554 7570 6c65 da05 4172  float..Tuple..Ar
+00001040: 7261 7972 4700 0000 720d 0000 0072 0d00  rayrG...r....r..
+00001050: 0000 720d 0000 0072 0e00 0000 da08 3c6d  ..r....r......<m
+00001060: 6f64 756c 653e 0100 0000 7324 0000 000c  odule>....s$....
+00001070: 0208 010c 0208 020c 010c 0204 0308 0408  ................
+00001080: 4200 0100 fb02 0102 0102 0102 0102 0102  B...............
+00001090: 010a fa                                  ...
```

### Comparing `lacss-0.4.1/lacss/ops/__pycache__/patches.cpython-38.pyc` & `lacss-0.4.2/lacss/ops/__pycache__/patches.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Jun 26 19:35:53 2023 UTC, .py size: 11768 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,637 +1,634 @@
-00000000: 550d 0d0a 0000 0000 99e8 9964 f82d 0000  U..........d.-..
+00000000: 550d 0d0a 0000 0000 a4bd ad64 b02d 0000  U..........d.-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 9001 0000 6400  .....@...s....d.
+00000020: 0009 0000 0040 0000 0073 6001 0000 6400  .....@...s`...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
-00000050: 6d07 5a07 6d08 5a08 0100 6401 6404 6c09  m.Z.m.Z...d.d.l.
-00000060: 5a09 6401 6404 6c0a 6d0b 5a0c 0100 6401  Z.d.d.l.m.Z...d.
-00000070: 6404 6c0b 5a0d 6405 6406 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
-00000080: 0100 6405 6407 6c10 6d11 5a11 0100 650c  ..d.d.l.m.Z...e.
-00000090: 6a12 650c 6a12 6513 6514 6408 9c04 6409  j.e.j.e.e.d...d.
-000000a0: 640a 8404 5a15 640b 640c 8400 5a16 6428  d...Z.d.d...Z.d(
-000000b0: 6508 6506 6504 6602 1900 6517 650c 6a12  e.e.e.f...e.e.j.
-000000c0: 640e 9c03 640f 6410 8405 5a18 6429 6508  d...d.d...Z.d)e.
-000000d0: 6506 6504 6602 1900 6507 6513 6513 6602  e.e.f...e.e.e.f.
-000000e0: 1900 6517 6514 6411 9c04 6412 6413 8405  ..e.e.d...d.d...
-000000f0: 5a19 642a 651a 650c 6a12 6513 6517 650c  Z.d*e.e.j.e.e.e.
-00000100: 6a12 6415 9c05 6416 6417 8405 5a1b 642b  j.d...d.d...Z.d+
-00000110: 651a 6507 6513 6513 6602 1900 6517 650c  e.e.e.e.f...e.e.
-00000120: 6a12 6411 9c04 6418 6419 8405 5a1c 642c  j.d...d.d...Z.d,
-00000130: 651a 6507 6513 6513 6602 1900 6505 650c  e.e.e.e.f...e.e.
-00000140: 6a12 1900 6517 6517 6513 650c 6a12 641a  j...e.e.e.e.j.d.
-00000150: 9c07 641b 641c 8405 5a1d 642d 651a 6517  ..d.d...Z.d-e.e.
-00000160: 650c 6a12 640e 9c03 641d 641e 8405 5a1e  e.j.d...d.d...Z.
-00000170: 642e 651a 6517 650c 6a12 6420 9c03 6421  d.e.e.e.j.d ..d!
-00000180: 6422 8405 5a1f 6509 a020 6502 6511 6423  d"..Z.e.. e.e.d#
-00000190: 6424 8d02 a101 5a21 651a 6517 6507 650c  d$....Z!e.e.e.e.
-000001a0: 6a12 650c 6a12 650c 6a12 6603 1900 6425  j.e.j.e.j.f...d%
-000001b0: 9c03 6426 6427 8404 5a22 6404 5300 292f  ..d&d'..Z"d.S.)/
-000001c0: 7a86 2056 6172 696f 7573 2066 756e 6374  z. Various funct
-000001d0: 696f 6e73 2064 6561 6c73 2077 6974 6820  ions deals with 
-000001e0: 7365 676d 656e 7461 7469 6f6e 2070 6174  segmentation pat
-000001f0: 6863 6573 0a0a 2020 2020 416c 6c20 6675  hces..    All fu
-00000200: 6e63 7469 6f6e 7320 6865 7265 2074 616b  nctions here tak
-00000210: 6573 2075 6e62 6174 6368 6564 2069 6e70  es unbatched inp
-00000220: 7574 2e20 5573 6520 766d 6170 2074 6f20  ut. Use vmap to 
-00000230: 636f 6e76 6572 7420 746f 2062 6174 6368  convert to batch
-00000240: 6564 2064 6174 610a e900 0000 0029 01da  ed data......)..
-00000250: 0770 6172 7469 616c 2905 da04 4469 6374  .partial)...Dict
-00000260: da08 4f70 7469 6f6e 616c da08 5365 7175  ..Optional..Sequ
-00000270: 656e 6365 da05 5475 706c 65da 0555 6e69  ence..Tuple..Uni
-00000280: 6f6e 4ee9 0100 0000 2901 da12 626f 785f  onN.....)...box_
-00000290: 696f 755f 7369 6d69 6c61 7269 7479 2901  iou_similarity).
-000002a0: da11 7375 625f 7069 7865 6c5f 7361 6d70  ..sub_pixel_samp
-000002b0: 6c65 7329 04da 0866 6561 7475 7265 73da  les)...features.
-000002c0: 096c 6f63 6174 696f 6e73 da0a 7061 7463  .locations..patc
-000002d0: 685f 7369 7a65 da06 7265 7475 726e 6303  h_size..returnc.
-000002e0: 0000 0000 0000 0000 0000 0010 0000 0006  ................
-000002f0: 0000 0043 0000 0073 3801 0000 7c00 6a00  ...C...s8...|.j.
-00000300: 5c03 7d03 7d04 7d05 7c01 7401 a002 7c03  \.}.}.}.|.t...|.
-00000310: 7c04 6702 a101 3900 7d01 7c01 a003 7404  |.g...9.}.|...t.
-00000320: a101 7d06 7401 a005 7c06 6401 6401 8502  ..}.t...|.d.d...
-00000330: 6402 6602 1900 6403 7c04 6402 1800 a103  d.f...d.|.d.....
-00000340: 7d07 7401 a005 7c06 6401 6401 8502 6403  }.t...|.d.d...d.
-00000350: 6602 1900 6403 7c03 6402 1800 a103 7d08  f...d.|.d.....}.
-00000360: 7401 6a06 6401 7c02 8502 6401 7c02 8502  t.j.d.|...d.|...
-00000370: 6602 1900 7c02 6404 1a00 1800 5c02 7d09  f...|.d.....\.}.
-00000380: 7d0a 7c0a 7c07 6401 6401 8502 6401 6401  }.|.|.d.d...d.d.
-00000390: 6603 1900 3700 7d0a 7c09 7c08 6401 6401  f...7.}.|.|.d.d.
-000003a0: 8502 6401 6401 6603 1900 3700 7d09 7c01  ..d.d.f...7.}.|.
-000003b0: 7401 6a07 7c08 7c07 6702 6405 6406 8d02  t.j.|.|.g.d.d...
-000003c0: 1800 7d0b 7c02 6404 1a00 6402 1700 7d0c  ..}.|.d...d...}.
-000003d0: 7c0c 7c0c 6702 7c0c 7c0c 6702 6403 6403  |.|.g.|.|.g.d.d.
-000003e0: 6702 6703 7d0d 7401 a008 7c00 7c0d a102  g.g.}.t...|.|...
-000003f0: 7d0e 7c0e 7c09 7c0c 1700 7c0a 7c0c 1700  }.|.|.|...|.|...
-00000400: 6401 6401 8502 6603 1900 7d0f 7c0f 7c09  d.d...f...}.|.|.
-00000410: 6401 6401 8502 6403 6403 6603 1900 7c0a  d.d...d.d.f...|.
-00000420: 6401 6401 8502 6403 6403 6603 1900 7c0b  d.d...d.d.f...|.
-00000430: 6604 5300 2907 6155 0100 0065 7874 7261  f.S.).aU...extra
-00000440: 6374 2066 6561 7475 7265 2070 6174 6368  ct feature patch
-00000450: 6573 2061 6363 6f72 6469 6e67 2074 6f20  es according to 
-00000460: 6120 6c69 7374 206f 6620 6c6f 6361 7469  a list of locati
-00000470: 6f6e 730a 0a20 2020 2041 7267 733a 0a20  ons..    Args:. 
-00000480: 2020 2020 2020 2066 6561 7475 7265 733a         features:
-00000490: 205b 482c 572c 435d 2073 7461 6e64 6172   [H,W,C] standar
-000004a0: 6420 3244 2066 6561 7475 7265 206d 6170  d 2D feature map
-000004b0: 0a20 2020 2020 2020 206c 6f63 6174 696f  .        locatio
-000004c0: 6e73 3a20 5b4e 2c20 325d 2066 6c6f 6174  ns: [N, 2] float
-000004d0: 3332 2c20 7363 616c 6564 2030 2e2e 310a  32, scaled 0..1.
-000004e0: 2020 2020 2020 2020 7061 7463 685f 7369          patch_si
-000004f0: 7a65 3a20 696e 740a 0a20 2020 2052 6574  ze: int..    Ret
-00000500: 7572 6e73 3a0a 2020 2020 2020 2020 7061  urns:.        pa
-00000510: 7463 6865 733a 205b 4e2c 2070 6174 6368  tches: [N, patch
-00000520: 5f73 697a 652c 2070 6174 6368 5f73 697a  _size, patch_siz
-00000530: 652c 2043 5d0a 2020 2020 2020 2020 7930  e, C].        y0
-00000540: 3a20 5b4e 5d3a 2079 3020 636f 6f72 6469  : [N]: y0 coordi
-00000550: 6e61 7465 7320 6f66 2070 6174 6368 6573  nates of patches
-00000560: 0a20 2020 2020 2020 2078 303a 205b 4e5d  .        x0: [N]
-00000570: 3a20 7830 2063 6f6f 7264 696e 6174 6573  : x0 coordinates
-00000580: 206f 6620 7061 7463 6865 730a 2020 2020   of patches.    
-00000590: 4e72 0800 0000 7201 0000 00e9 0200 0000  Nr....r.........
-000005a0: e9ff ffff ffa9 01da 0461 7869 7329 09da  .........axis)..
-000005b0: 0573 6861 7065 da03 6a6e 70da 0561 7272  .shape..jnp..arr
-000005c0: 6179 da06 6173 7479 7065 da03 696e 74da  ay..astype..int.
-000005d0: 0463 6c69 70da 056d 6772 6964 da05 7374  .clip..mgrid..st
-000005e0: 6163 6bda 0370 6164 2910 720b 0000 0072  ack..pad).r....r
-000005f0: 0c00 0000 720d 0000 00da 0668 6569 6768  ....r......heigh
-00000600: 74da 0577 6964 7468 da01 5f5a 0b69 5f6c  t..width.._Z.i_l
-00000610: 6f63 6174 696f 6e73 5a0d 695f 6c6f 6361  ocationsZ.i_loca
-00000620: 7469 6f6e 735f 785a 0d69 5f6c 6f63 6174  tions_xZ.i_locat
-00000630: 696f 6e73 5f79 da02 7979 da02 7878 da09  ions_y..yy..xx..
-00000640: 7265 6d61 696e 6465 72da 0c70 6164 6469  remainder..paddi
-00000650: 6e67 5f73 697a 65da 0870 6164 6469 6e67  ng_size..padding
-00000660: 735a 0f70 6164 6465 645f 6665 6174 7572  sZ.padded_featur
-00000670: 6573 da07 7061 7463 6865 73a9 0072 2500  es..patches..r%.
-00000680: 0000 fa34 2f68 6f6d 652f 4643 414d 2f6a  ...4/home/FCAM/j
-00000690: 7975 2f70 726f 6a5f 6c61 6373 732f 6c61  yu/proj_lacss/la
-000006a0: 6373 732f 6c61 6373 732f 6f70 732f 7061  css/lacss/ops/pa
-000006b0: 7463 6865 732e 7079 da0e 6761 7468 6572  tches.py..gather
-000006c0: 5f70 6174 6368 6573 1100 0000 7322 0000  _patches....s"..
-000006d0: 0000 0f0c 0212 020a 011e 011e 0122 0116  ............."..
-000006e0: 0116 0116 030c 0206 0106 0106 fd04 050c  ................
-000006f0: 021a 0272 2700 0000 6301 0000 0000 0000  ...r'...c.......
-00000700: 0000 0000 0004 0000 0003 0000 0043 0000  .............C..
-00000710: 0073 4e00 0000 7400 7c00 7401 8302 7224  .sN...t.|.t...r$
-00000720: 7c00 6401 1900 7d01 7c00 6402 1900 7d02  |.d...}.|.d...}.
-00000730: 7c00 6403 1900 7d03 6e0a 7c00 5c03 7d01  |.d...}.n.|.\.}.
-00000740: 7d02 7d03 7c01 6a02 7c02 6a02 6b04 7244  }.}.|.j.|.j.k.rD
-00000750: 7c01 a003 6404 a101 7d01 7c01 7c02 7c03  |...d...}.|.|.|.
-00000760: 6603 5300 2905 4eda 0f69 6e73 7461 6e63  f.S.).N..instanc
-00000770: 655f 6f75 7470 7574 da0b 696e 7374 616e  e_output..instan
-00000780: 6365 5f79 63da 0b69 6e73 7461 6e63 655f  ce_yc..instance_
-00000790: 7863 7210 0000 0029 04da 0a69 7369 6e73  xcr....)...isins
-000007a0: 7461 6e63 65da 0464 6963 74da 046e 6469  tance..dict..ndi
-000007b0: 6dda 0773 7175 6565 7a65 2904 da04 7072  m..squeeze)...pr
-000007c0: 6564 7224 0000 00da 0279 63da 0278 6372  edr$.....yc..xcr
-000007d0: 2500 0000 7225 0000 0072 2600 0000 da0f  %...r%...r&.....
-000007e0: 5f67 6574 5f70 6174 6368 5f64 6174 613a  _get_patch_data:
-000007f0: 0000 0073 1000 0000 0001 0a01 0801 0801  ...s............
-00000800: 0a02 0a02 0c01 0a02 7232 0000 00e7 0000  ........r2......
-00000810: 0000 0000 e03f 2903 722f 0000 00da 0974  .....?).r/.....t
-00000820: 6872 6573 686f 6c64 720e 0000 0063 0200  hresholdr....c..
-00000830: 0000 0000 0000 0000 0000 1000 0000 0600  ................
-00000840: 0000 4300 0000 7328 0100 0074 007c 0083  ..C...s(...t.|..
-00000850: 015c 037d 027d 037d 047c 026a 015c 037d  .\.}.}.}.|.j.\.}
-00000860: 057d 067d 0774 026a 037c 027c 016b 0464  .}.}.t.j.|.|.k.d
-00000870: 0164 028d 027d 0874 026a 037c 027c 016b  .d...}.t.j.|.|.k
-00000880: 0464 0364 028d 027d 097c 086a 0464 0164  .d.d...}.|.j.d.d
-00000890: 028d 017d 0a7c 077c 0864 0464 0485 0264  ...}.|.|.d.d...d
-000008a0: 0464 0464 0585 0366 0219 006a 0464 0164  .d.d...f...j.d.d
-000008b0: 028d 0118 007d 0b7c 096a 0464 0164 028d  .....}.|.j.d.d..
-000008c0: 017d 0c7c 067c 0964 0464 0485 0264 0464  .}.|.|.d.d...d.d
-000008d0: 0464 0585 0366 0219 006a 0464 0164 028d  .d...f...j.d.d..
-000008e0: 0118 007d 0d7c 0c7c 0364 0464 0485 0264  ...}.|.|.d.d...d
-000008f0: 0664 0666 0319 0037 007d 0c7c 0d7c 0364  .d.f...7.}.|.|.d
-00000900: 0464 0485 0264 0664 0666 0319 0037 007d  .d...d.d.f...7.}
-00000910: 0d7c 0a7c 0464 0464 0485 0264 0664 0666  .|.|.d.d...d.d.f
-00000920: 0319 0037 007d 0a7c 0b7c 0464 0464 0485  ...7.}.|.|.d.d..
-00000930: 0264 0664 0666 0319 0037 007d 0b7c 086a  .d.d.f...7.}.|.j
-00000940: 0364 0164 0764 088d 027d 0e74 026a 057c  .d.d.d...}.t.j.|
-00000950: 0c7c 0a7c 0d7c 0b67 0464 0564 028d 027d  .|.|.|.g.d.d...}
-00000960: 0f74 02a0 067c 0e7c 0f64 05a1 037d 0f7c  .t...|.|.d...}.|
-00000970: 0f53 0029 097a f043 6f6d 7075 7465 2074  .S.).z.Compute t
-00000980: 6865 2069 6e73 7461 6e63 6520 6262 6f78  he instance bbox
-00000990: 6573 2066 726f 6d20 6d6f 6465 6c20 7072  es from model pr
-000009a0: 6564 6963 7469 6f6e 730a 0a20 2020 2041  edictions..    A
-000009b0: 7267 733a 0a20 2020 2020 2020 2070 7265  rgs:.        pre
-000009c0: 643a 2041 206d 6f64 656c 2070 7265 6469  d: A model predi
-000009d0: 6374 696f 6e20 6469 6374 696f 6e61 7279  ction dictionary
-000009e0: 3a0a 2020 2020 2020 2020 7468 7265 7368  :.        thresh
-000009f0: 6f6c 643a 2066 6f72 2073 6567 6d65 6e74  old: for segment
-00000a00: 6174 696f 6e2c 2064 6566 6175 6c74 2030  ation, default 0
-00000a10: 2e35 0a0a 2020 2020 5265 7475 726e 733a  .5..    Returns:
-00000a20: 0a20 2020 2020 2020 2062 626f 7865 733a  .        bboxes:
-00000a30: 205b 6e2c 2034 5d20 6262 6f6f 7820 666f   [n, 4] bboox fo
-00000a40: 7220 656d 7074 7920 7061 7463 6865 7320  r empty patches 
-00000a50: 6172 6520 6669 6c6c 6564 2077 6974 6820  are filled with 
-00000a60: 2d31 0a20 2020 2072 0800 0000 7211 0000  -1.    r....r...
-00000a70: 0072 0f00 0000 4e72 1000 0000 7201 0000  .r....Nr....r...
-00000a80: 0054 2902 7212 0000 00da 086b 6565 7064  .T).r......keepd
-00000a90: 696d 7329 0772 3200 0000 7213 0000 0072  ims).r2...r....r
-00000aa0: 1400 0000 da03 616e 79da 0661 7267 6d61  ......any..argma
-00000ab0: 7872 1a00 0000 da05 7768 6572 6529 1072  xr......where).r
-00000ac0: 2f00 0000 7234 0000 0072 2400 0000 721f  /...r4...r$...r.
-00000ad0: 0000 0072 2000 0000 721e 0000 00da 0264  ...r ...r......d
-00000ae0: 30da 0264 31da 0872 6f77 5f6d 6173 6bda  0..d1..row_mask.
-00000af0: 0863 6f6c 5f6d 6173 6b5a 076d 696e 5f63  .col_maskZ.min_c
-00000b00: 6f6c 5a07 6d61 785f 636f 6c5a 076d 696e  olZ.max_colZ.min
-00000b10: 5f72 6f77 5a07 6d61 785f 726f 77da 0869  _rowZ.max_row..i
-00000b20: 735f 7661 6c69 64da 0662 626f 7865 7372  s_valid..bboxesr
-00000b30: 2500 0000 7225 0000 0072 2600 0000 da11  %...r%...r&.....
-00000b40: 6262 6f78 6573 5f6f 665f 7061 7463 6865  bboxes_of_patche
-00000b50: 7348 0000 0073 2000 0000 000c 0e02 0c01  sH...s .........
-00000b60: 1201 1202 0c01 2202 0c01 2202 1601 1601  ......"...".....
-00000b70: 1601 1602 0e01 1601 0e02 723f 0000 0029  ..........r?...)
-00000b80: 0472 2f00 0000 da0a 696e 7075 745f 7369  .r/.....input_si
-00000b90: 7a65 7234 0000 0072 0e00 0000 6303 0000  zer4...r....c...
-00000ba0: 0000 0000 0000 0000 000b 0000 0004 0000  ................
-00000bb0: 0043 0000 0073 9800 0000 7400 7c00 8301  .C...s....t.|...
-00000bc0: 5c03 7d03 7d04 7d05 7c03 7c02 6b05 7d06  \.}.}.}.|.|.k.}.
-00000bd0: 7c04 7c06 1900 7d04 7c05 7c06 1900 7d05  |.|...}.|.|...}.
-00000be0: 7401 a002 7c06 a101 6401 6401 8502 6402  t...|...d.d...d.
-00000bf0: 6602 1900 7d07 7c01 6401 6b09 7284 7c01  f...}.|.d.k.r.|.
-00000c00: 5c02 7d08 7d09 7c04 6402 6b05 7c04 7c08  \.}.}.|.d.k.|.|.
-00000c10: 6b00 4000 7c05 6402 6b05 7c05 7c09 6b00  k.@.|.d.k.|.|.k.
-00000c20: 4000 4000 7d0a 7c04 7c0a 1900 7d04 7c05  @.@.}.|.|...}.|.
-00000c30: 7c0a 1900 7d05 7c07 7c0a 1900 7d07 7401  |...}.|.|...}.t.
-00000c40: 6a03 7c04 7c05 7c07 6703 6403 6404 8d02  j.|.|.|.g.d.d...
-00000c50: 5300 2905 611b 0100 0043 6f6d 7075 7465  S.).a....Compute
-00000c60: 2079 7820 636f 6f64 696e 6174 6573 206f   yx coodinates o
-00000c70: 6620 616c 6c20 7365 676d 656e 7465 6420  f all segmented 
-00000c80: 696e 7374 616e 6365 730a 0a20 2020 2041  instances..    A
-00000c90: 7267 733a 0a20 2020 2020 2020 2070 7265  rgs:.        pre
-00000ca0: 643a 2041 206d 6f64 656c 2070 7265 6469  d: A model predi
-00000cb0: 6374 696f 6e20 6469 6374 696f 6e61 7279  ction dictionary
-00000cc0: 0a20 2020 2020 2020 2074 6872 6573 686f  .        thresho
-00000cd0: 6c64 3a20 666c 6f61 740a 0a20 2020 2052  ld: float..    R
-00000ce0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00000cf0: 5b4e 2c20 335d 2061 7272 6179 2e20 5468  [N, 3] array. Th
-00000d00: 6520 6669 7273 7420 7477 6f20 636f 6c75  e first two colu
-00000d10: 6d6e 7320 6172 6520 792d 7820 636f 6f72  mns are y-x coor
-00000d20: 6469 6e61 7465 732e 2054 6865 2074 6869  dinates. The thi
-00000d30: 7264 0a20 2020 2020 2020 2020 2020 2063  rd.            c
-00000d40: 6f6c 756d 6e20 6973 2061 2069 6e64 6578  olumn is a index
-00000d50: 2076 616c 7565 2066 6f72 2064 6966 6665   value for diffe
-00000d60: 7265 6e74 2069 6e73 7461 6e63 6573 2e0a  rent instances..
-00000d70: 2020 2020 4e72 0100 0000 7210 0000 0072      Nr....r....r
-00000d80: 1100 0000 2904 7232 0000 0072 1400 0000  ....).r2...r....
-00000d90: da08 6172 6777 6865 7265 721a 0000 0029  ..argwherer....)
-00000da0: 0b72 2f00 0000 7240 0000 0072 3400 0000  .r/...r@...r4...
-00000db0: 7224 0000 0072 1f00 0000 7220 0000 00da  r$...r....r ....
-00000dc0: 0769 6e64 6963 6573 5a06 726f 7769 6473  .indicesZ.rowids
-00000dd0: 721c 0000 0072 1d00 0000 5a0c 7661 6c69  r....r....Z.vali
-00000de0: 645f 636f 6f72 6473 7225 0000 0072 2500  d_coordsr%...r%.
-00000df0: 0000 7226 0000 00da 1269 6e64 6963 6573  ..r&.....indices
-00000e00: 5f6f 665f 7061 7463 6865 736c 0000 0073  _of_patchesl...s
-00000e10: 1800 0000 000f 0e02 0801 0801 0801 1602  ................
-00000e20: 0801 0801 2001 0801 0801 0802 7243 0000  .... .......rC..
-00000e30: 00e9 8000 0000 2905 722f 0000 00da 066c  ......).r/.....l
-00000e40: 6162 656c 73da 0a42 4c4f 434b 5f53 495a  abels..BLOCK_SIZ
-00000e50: 4572 3400 0000 720e 0000 0063 0400 0000  Er4...r....c....
-00000e60: 0000 0000 0000 0000 1200 0000 0800 0000  ................
-00000e70: 4300 0000 7362 0100 0074 007c 0083 015c  C...sb...t.|...\
-00000e80: 037d 047d 057d 067c 047c 036b 057d 0474  .}.}.}.|.|.k.}.t
-00000e90: 016a 027c 0464 0164 028d 027d 077c 01a0  .j.|.d.d...}.|..
-00000ea0: 0374 04a1 017d 017c 056a 0564 0319 0064  .t...}.|.j.d...d
-00000eb0: 041a 007d 0874 016a 067c 017c 0864 0564  ...}.t.j.|.|.d.d
-00000ec0: 068d 037d 097c 097c 057c 0817 007c 067c  ...}.|.|.|...|.|
-00000ed0: 0817 0066 0219 007d 0a7c 01a0 07a1 0064  ...f...}.|.....d
-00000ee0: 0718 007c 021a 0064 0717 007c 0214 007d  ...|...d...|...}
-00000ef0: 0b74 016a 027c 0164 0864 0885 0264 0864  .t.j.|.d.d...d.d
-00000f00: 0885 0264 0866 0319 0074 01a0 087c 0ba1  ...d.f...t...|..
-00000f10: 0164 0717 006b 0264 0964 028d 027d 0c67  .d...k.d.d...}.g
-00000f20: 007d 0d74 0964 077c 01a0 07a1 0064 0717  .}.t.d.|.....d..
-00000f30: 007c 0283 0344 005d 747d 0e7c 0a74 01a0  .|...D.]t}.|.t..
-00000f40: 087c 0e7c 0e7c 0217 00a1 02a0 0a64 0364  .|.|.|.......d.d
-00000f50: 0764 0764 07a1 046b 027d 0f7c 0c7c 0e64  .d.d...k.}.|.|.d
-00000f60: 0718 007c 0e7c 0217 0064 0718 0085 0219  ...|.|...d......
-00000f70: 007d 1074 016a 027c 0f7c 0440 0064 0164  .}.t.j.|.|.@.d.d
-00000f80: 028d 027d 117c 0da0 0b7c 117c 077c 1064  ...}.|...|.|.|.d
-00000f90: 0864 0885 0264 0866 0219 0017 007c 1118  .d...d.f.....|..
-00000fa0: 0064 0a17 001b 00a1 0101 0071 be74 016a  .d.........q.t.j
-00000fb0: 0c7c 0d64 0564 028d 02a0 0da1 007d 0d7c  .|.d.d.......}.|
-00000fc0: 0d64 0864 0885 0264 087c 01a0 07a1 0085  .d.d...d.|......
-00000fd0: 0266 0219 007d 0d7c 0d53 0029 0b61 0201  .f...}.|.S.).a..
-00000fe0: 0000 436f 6d70 7574 6520 696f 7520 6265  ..Compute iou be
-00000ff0: 7477 6565 6e20 7072 6564 6963 7469 6f6e  tween prediction
-00001000: 2061 6e64 2067 726f 756e 6420 7472 7574   and ground trut
-00001010: 6820 6c61 6265 6c2e 0a0a 2020 2020 4172  h label...    Ar
-00001020: 6773 3a0a 2020 2020 2020 2020 7072 6564  gs:.        pred
-00001030: 3a20 4120 6d6f 6465 6c20 7072 6564 6963  : A model predic
-00001040: 7469 6f6e 2064 6963 7469 6f6e 6172 790a  tion dictionary.
-00001050: 2020 2020 2020 2020 6c61 6265 6c73 3a20          labels: 
-00001060: 696d 6167 6520 6c61 6265 6c2e 2062 675f  image label. bg_
-00001070: 6c61 6265 6c20 3d20 300a 2020 2020 2020  label = 0.      
-00001080: 2020 7468 7265 7368 6f6c 643a 2066 6f72    threshold: for
-00001090: 2073 6567 6d65 6e74 6174 696f 6e2e 2064   segmentation. d
-000010a0: 6566 6175 6c74 2069 7320 302e 350a 0a20  efault is 0.5.. 
-000010b0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-000010c0: 2020 2020 5b6e 2c20 6d5d 2061 7272 6179      [n, m] array
-000010d0: 206f 6620 696f 7520 7661 6c75 6573 2e0a   of iou values..
-000010e0: 2020 2020 2902 7210 0000 00e9 feff ffff      ).r.........
-000010f0: 7211 0000 0072 1000 0000 720f 0000 0072  r....r....r....r
-00001100: 0100 0000 2901 da0f 636f 6e73 7461 6e74  ....)...constant
-00001110: 5f76 616c 7565 7372 0800 0000 4e29 0272  _valuesr....N).r
-00001120: 0100 0000 7208 0000 00e7 3a8c 30e2 8e79  ....r.....:.0..y
-00001130: 453e 290e 7232 0000 0072 1400 0000 da0d  E>).r2...r......
-00001140: 636f 756e 745f 6e6f 6e7a 6572 6f72 1600  count_nonzeror..
-00001150: 0000 7217 0000 0072 1300 0000 721b 0000  ..r....r....r...
-00001160: 00da 036d 6178 da06 6172 616e 6765 da05  ...max..arange..
-00001170: 7261 6e67 65da 0772 6573 6861 7065 da06  range..reshape..
-00001180: 6170 7065 6e64 da0b 636f 6e63 6174 656e  append..concaten
-00001190: 6174 65da 0974 7261 6e73 706f 7365 2912  ate..transpose).
-000011a0: 722f 0000 0072 4500 0000 7246 0000 0072  r/...rE...rF...r
-000011b0: 3400 0000 7224 0000 0072 3000 0000 7231  4...r$...r0...r1
-000011c0: 0000 00da 0a70 7265 645f 6172 6561 73da  .....pred_areas.
-000011d0: 0470 6164 735a 0d70 6164 6465 645f 6c61  .padsZ.padded_la
-000011e0: 6265 6c73 da0a 6774 5f70 6174 6368 6573  bels..gt_patches
-000011f0: da0b 6d61 785f 696e 6469 6365 735a 0c61  ..max_indicesZ.a
-00001200: 6c6c 5f67 745f 6172 6561 73da 0469 6f75  ll_gt_areas..iou
-00001210: 73da 016b da04 6774 5f70 da08 6774 5f61  s..k..gt_p..gt_a
-00001220: 7265 6173 da09 696e 7465 7273 6563 7472  reas..intersectr
-00001230: 2500 0000 7225 0000 0072 2600 0000 da16  %...r%...r&.....
-00001240: 696f 755f 7061 7463 6865 735f 616e 645f  iou_patches_and_
-00001250: 6c61 6265 6c73 8c00 0000 7334 0000 0000  labels....s4....
-00001260: 0d0e 0108 010e 010a 020e 0110 0114 0218  ................
-00001270: 0104 0122 0002 ff06 0404 0218 0112 0102  ..."............
-00001280: 0002 0002 0002 ff06 0318 0112 0128 0212  .............(..
-00001290: 0118 0272 5b00 0000 6303 0000 0000 0000  ...r[...c.......
-000012a0: 0000 0000 000b 0000 0005 0000 0043 0000  .............C..
-000012b0: 0073 6600 0000 7400 7c00 8301 5c03 7d03  .sf...t.|...\.}.
-000012c0: 7d04 7d05 7c04 6a01 5c03 7d06 7d07 7d08  }.}.|.j.\.}.}.}.
-000012d0: 7402 a003 7c06 a101 7d09 7402 a004 7c06  t...|...}.t...|.
-000012e0: 6601 7c01 1700 a101 7d0a 7c0a 6a05 7c09  f.|.....}.|.j.|.
-000012f0: 6401 6401 8502 6401 6401 6603 1900 7c04  d.d...d.d.f...|.
-00001300: 7c05 6603 1900 a006 7c03 a101 7d0a 7c0a  |.f.....|...}.|.
-00001310: 7c02 6b05 a007 7408 a101 5300 2902 61db  |.k...t...S.).a.
-00001320: 0100 0045 7870 616e 6420 7468 6520 7072  ...Expand the pr
-00001330: 6564 6963 7465 6420 7061 7463 6865 7320  edicted patches 
-00001340: 746f 2074 6865 2066 756c 6c20 696d 6167  to the full imag
-00001350: 6520 7369 7a65 2e0a 2020 2020 5468 6520  e size..    The 
-00001360: 6465 6661 756c 7420 6d6f 6465 6c20 7365  default model se
-00001370: 676d 656e 7461 7469 6f6e 206f 7574 7075  gmentation outpu
-00001380: 7420 7368 6f77 7320 6f6e 6c79 2061 2073  t shows only a s
-00001390: 6d61 6c6c 2070 6174 6368 2061 726f 756e  mall patch aroun
-000013a0: 6420 6561 6368 2069 6e73 7461 6e63 652e  d each instance.
-000013b0: 2054 6869 730a 2020 2020 6675 6e63 7469   This.    functi
-000013c0: 6f6e 2065 7870 616e 6420 6561 6368 2070  on expand each p
-000013d0: 6174 6368 2074 6f20 7468 6520 7369 7a65  atch to the size
-000013e0: 206f 6620 7468 6520 6f72 6769 6e61 6c20   of the orginal 
-000013f0: 696d 6167 652e 0a0a 2020 2020 4172 6773  image...    Args
-00001400: 3a0a 2020 2020 2020 2020 7072 6564 3a20  :.        pred: 
-00001410: 4120 6d6f 6465 6c20 7072 6564 6963 7469  A model predicti
-00001420: 6f6e 2064 6963 7469 6f6e 6172 790a 2020  on dictionary.  
-00001430: 2020 2020 2020 696e 7075 745f 7369 7a65        input_size
-00001440: 3a20 7368 6170 6520 6f66 2074 6865 2069  : shape of the i
-00001450: 6e70 7574 2069 6d61 6765 2e20 5475 706c  nput image. Tupl
-00001460: 6520 6f66 2048 2c20 570a 2020 2020 2020  e of H, W.      
-00001470: 2020 7468 7265 7368 6f6c 643a 2066 6f72    threshold: for
-00001480: 2073 6567 6d65 6e74 6174 696f 6e2e 2044   segmentation. D
-00001490: 6566 6175 6c74 2069 7320 302e 352e 0a0a  efault is 0.5...
-000014a0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-000014b0: 2020 2020 2073 6567 6d65 6e74 6174 696f       segmentatio
-000014c0: 6e73 3a20 5b6e 2c20 6865 6967 6874 2c20  ns: [n, height, 
-000014d0: 7769 6474 685d 206e 2066 756c 6c30 2d73  width] n full0-s
-000014e0: 697a 6520 7365 676d 656e 6174 6174 696f  ize segmenatatio
-000014f0: 6e20 6d61 736b 732e 0a0a 2020 2020 4e29  n masks...    N)
-00001500: 0972 3200 0000 7213 0000 0072 1400 0000  .r2...r....r....
-00001510: 724c 0000 00da 057a 6572 6f73 da02 6174  rL.....zeros..at
-00001520: da03 7365 7472 1600 0000 7217 0000 0029  ..setr....r....)
-00001530: 0b72 2f00 0000 7240 0000 0072 3400 0000  .r/...r@...r4...
-00001540: 7224 0000 0072 3000 0000 7231 0000 00da  r$...r0...r1....
-00001550: 096e 5f70 6174 6368 6573 720d 0000 0072  .n_patchesr....r
-00001560: 1e00 0000 5a09 7061 6765 5f6e 756d 735a  ....Z.page_numsZ
-00001570: 0573 6567 6d73 7225 0000 0072 2500 0000  .segmsr%...r%...
-00001580: 7226 0000 00da 1870 6174 6368 6573 5f74  r&.....patches_t
-00001590: 6f5f 7365 676d 656e 7461 7469 6f6e 73b7  o_segmentations.
-000015a0: 0000 0073 0c00 0000 0010 0e01 0c02 0a01  ...s............
-000015b0: 1001 2402 7260 0000 0029 0772 2f00 0000  ..$.r`...).r/...
-000015c0: 7240 0000 00da 046d 6173 6bda 0f73 636f  r@.....mask..sco
-000015d0: 7265 5f74 6872 6573 686f 6c64 7234 0000  re_thresholdr4..
-000015e0: 00da 0d6d 696e 5f63 656c 6c5f 6172 6561  ...min_cell_area
-000015f0: 720e 0000 0063 0600 0000 0000 0000 0000  r....c..........
-00001600: 0000 0d00 0000 0600 0000 4300 0000 7318  ..........C...s.
-00001610: 0100 0074 00a0 017c 01a1 017d 067c 0064  ...t...|...}.|.d
-00001620: 0119 007c 046b 047d 077c 076a 025c 037d  ...|.k.}.|.j.\.}
-00001630: 087d 097d 0a7c 0264 026b 0872 3a74 006a  .}.}.|.d.k.r:t.j
-00001640: 037c 0867 0174 0464 038d 027d 027c 027c  .|.g.t.d...}.|.|
-00001650: 0064 0419 006a 0564 0564 068d 014d 007d  .d...j.d.d...M.}
-00001660: 027c 0364 076b 0472 6e64 087c 006b 0772  .|.d.k.rnd.|.k.r
-00001670: 6e7c 027c 0064 0919 007c 036b 054d 007d  n|.|.d...|.k.M.}
-00001680: 027c 0274 006a 067c 0764 0564 068d 027c  .|.t.j.|.d.d...|
-00001690: 056b 044d 007d 027c 077c 046b 04a0 0774  .k.M.}.|.|.k...t
-000016a0: 08a1 0174 00a0 0964 0a7c 076a 0264 0719  ...t...d.|.j.d..
-000016b0: 0064 0a17 00a1 0264 0264 0285 0264 0264  .d.....d.d...d.d
-000016c0: 0266 0319 0014 007d 0774 00a0 0a7c 0264  .f.....}.t...|.d
-000016d0: 0264 0285 0264 0264 0266 0319 007c 0764  .d...d.d.f...|.d
-000016e0: 07a1 037d 0774 00a0 0a7c 0764 076b 0264  ...}.t...|.d.k.d
-000016f0: 077c 07a0 0ba1 0064 0a17 007c 0718 00a1  .|.....d...|....
-00001700: 037d 077c 0064 0b19 007d 0b7c 0064 0c19  .}.|.d...}.|.d..
-00001710: 007d 0c7c 066a 0c7c 0b7c 0c66 0219 00a0  .}.|.j.|.|.f....
-00001720: 0b7c 07a1 017d 067c 0653 0029 0d61 f701  .|...}.|.S.).a..
-00001730: 0000 636f 6e76 6572 7420 7061 7463 6820  ..convert patch 
-00001740: 6f75 7470 7574 2074 6f20 7468 6520 696d  output to the im
-00001750: 6167 6520 6c61 6265 6c0a 0a20 2020 2041  age label..    A
-00001760: 7267 733a 0a20 2020 2020 2020 2070 7265  rgs:.        pre
-00001770: 643a 2041 206d 6f64 656c 2070 7265 6469  d: A model predi
-00001780: 6374 696f 6e20 6469 6374 696f 6e61 7279  ction dictionary
-00001790: 0a20 2020 2020 2020 2069 6e70 7574 5f73  .        input_s
-000017a0: 697a 653a 2073 6861 7065 206f 6620 7468  ize: shape of th
-000017b0: 6520 696e 7075 7420 696d 6167 652e 2054  e input image. T
-000017c0: 7570 6c65 206f 6620 482c 2057 0a20 2020  uple of H, W.   
-000017d0: 2020 2020 206d 6173 6b3a 2062 6f6f 6c65       mask: boole
-000017e0: 616e 2069 6e64 6963 6174 6f72 7320 6d61  an indicators ma
-000017f0: 736b 696e 6720 6f75 7420 756e 7761 6e74  sking out unwant
-00001800: 6564 2069 6e73 7461 6e63 6573 2e20 4465  ed instances. De
-00001810: 6661 756c 7420 6973 204e 6f6e 6520 2861  fault is None (a
-00001820: 6c6c 2063 656c 6c73 290a 2020 2020 2020  ll cells).      
-00001830: 2020 7363 6f72 655f 7468 7265 7368 6f6c    score_threshol
-00001840: 643a 206f 7469 6f6e 616c 2c20 6d69 6e5f  d: otional, min_
-00001850: 7363 6f72 6520 746f 2062 6520 696e 636c  score to be incl
-00001860: 7564 6564 2e20 4465 6661 756c 7420 6973  uded. Default is
-00001870: 202e 352e 0a20 2020 2020 2020 2074 6872   .5..        thr
-00001880: 6573 686f 6c64 3a20 7365 676d 656e 7461  eshold: segmenta
-00001890: 7469 6f6e 2074 6872 6573 686f 6c64 2e20  tion threshold. 
-000018a0: 2044 6566 6175 6c74 202e 350a 2020 2020   Default .5.    
-000018b0: 2020 2020 6d69 6e5f 6365 6c6c 5f61 7265      min_cell_are
-000018c0: 613a 206f 7074 696f 6e61 6c20 6d69 6e69  a: optional mini
-000018d0: 6d61 6c20 6365 6c6c 2061 7265 6120 746f  mal cell area to
-000018e0: 2062 6520 706c 6f74 7465 642c 2064 6566   be plotted, def
-000018f0: 6175 6c74 2030 2e0a 0a20 2020 2052 6574  ault 0...    Ret
-00001900: 7572 6e73 3a0a 2020 2020 2020 2020 6c61  urns:.        la
-00001910: 6265 6c3a 205b 6865 6967 6874 2c20 7769  bel: [height, wi
-00001920: 6474 685d 0a20 2020 2072 2800 0000 4ea9  dth].    r(...N.
-00001930: 01da 0564 7479 7065 da0d 696e 7374 616e  ...dtype..instan
-00001940: 6365 5f6d 6173 6ba9 0272 0800 0000 720f  ce_mask..r....r.
-00001950: 0000 0072 1100 0000 7201 0000 00da 1274  ...r....r......t
-00001960: 7261 696e 696e 675f 6c6f 6361 7469 6f6e  raining_location
-00001970: 735a 0b70 7265 645f 7363 6f72 6573 7208  sZ.pred_scoresr.
-00001980: 0000 0072 2900 0000 722a 0000 0029 0d72  ...r)...r*...).r
-00001990: 1400 0000 725c 0000 0072 1300 0000 da04  ....r\...r......
-000019a0: 6f6e 6573 da04 626f 6f6c 722e 0000 0072  ones..boolr....r
-000019b0: 4a00 0000 7216 0000 0072 1700 0000 724c  J...r....r....rL
-000019c0: 0000 0072 3800 0000 724b 0000 0072 5d00  ...r8...rK...r].
-000019d0: 0000 290d 722f 0000 0072 4000 0000 7261  ..).r/...r@...ra
-000019e0: 0000 0072 6200 0000 7234 0000 0072 6300  ...rb...r4...rc.
-000019f0: 0000 da05 6c61 6265 6cda 0270 7272 5f00  ....label..prr_.
-00001a00: 0000 720d 0000 0072 1e00 0000 7230 0000  ..r....r....r0..
-00001a10: 0072 3100 0000 7225 0000 0072 2500 0000  .r1...r%...r%...
-00001a20: 7226 0000 00da 1070 6174 6368 6573 5f74  r&.....patches_t
-00001a30: 6f5f 6c61 6265 6cd1 0000 0073 2000 0000  o_label....s ...
-00001a40: 0015 0a01 0c01 0c02 0801 1001 1401 1001  ................
-00001a50: 1001 1602 3201 1c01 1e02 0801 0802 1402  ....2...........
-00001a60: 726d 0000 0063 0200 0000 0000 0000 0000  rm...c..........
-00001a70: 0000 1300 0000 0800 0000 4300 0000 73a4  ..........C...s.
-00001a80: 0100 0074 007c 0083 017d 0274 017c 027c  ...t.|...}.t.|.|
-00001a90: 0283 027d 0374 02a0 037c 0364 01a1 027d  ...}.t...|.d...}
-00001aa0: 0374 02a0 047c 0364 026b 04a1 015c 027d  .t...|.d.k...\.}
-00001ab0: 047d 057c 0064 0319 006a 0564 0419 007d  .}.|.d...j.d...}
-00001ac0: 0674 02a0 067c 0064 0319 00a1 017c 016b  .t...|.d.....|.k
-00001ad0: 057d 077c 077c 0419 007d 087c 077c 0519  .}.|.|...}.|.|..
-00001ae0: 007d 0974 026a 0774 087c 0483 017c 0664  .}.t.j.t.|...|.d
-00001af0: 0514 007c 0664 0514 0067 0374 0964 068d  ...|.d...g.t.d..
-00001b00: 027d 0a74 02a0 067c 0064 0719 00a1 017c  .}.t...|.d.....|
-00001b10: 0464 0264 0266 0319 0074 02a0 067c 0064  .d.d.f...t...|.d
-00001b20: 0719 00a1 017c 0564 0264 0266 0319 0018  .....|.d.d.f....
-00001b30: 007c 0617 007d 0b74 02a0 067c 0064 0819  .|...}.t...|.d..
-00001b40: 00a1 017c 0464 0264 0266 0319 0074 02a0  ...|.d.d.f...t..
-00001b50: 067c 0064 0819 00a1 017c 0564 0264 0266  .|.d.....|.d.d.f
-00001b60: 0319 0018 007c 0617 007d 0c74 0a74 087c  .....|...}.t.t.|
-00001b70: 0483 0183 0144 005d 367d 0d7c 087c 0d19  .....D.]6}.|.|..
-00001b80: 007c 0a7c 0d7c 0b7c 0d19 007c 0b7c 0d19  .|.|.|.|...|.|..
-00001b90: 007c 0617 0085 027c 0c7c 0d19 007c 0c7c  .|.....|.|...|.|
-00001ba0: 0d19 007c 0617 0085 0266 033c 0071 f47c  ...|.....f.<.q.|
-00001bb0: 0a64 0964 0985 027c 067c 0664 0a14 0085  .d.d...|.|.d....
-00001bc0: 027c 067c 0664 0a14 0085 0266 0319 007d  .|.|.d.....f...}
-00001bd0: 0a74 026a 0b7c 0a7c 0940 0064 0b64 0c8d  .t.j.|.|.@.d.d..
-00001be0: 027d 0e74 026a 0b7c 0864 0b64 0c8d 027d  .}.t.j.|.d.d...}
-00001bf0: 0f74 026a 0b7c 0964 0b64 0c8d 027d 107c  .t.j.|.d.d...}.|
-00001c00: 0e7c 107c 0f17 007c 0e18 0064 0d17 001b  .|.|...|...d....
-00001c10: 007d 117c 037d 127c 117c 127c 047c 0566  .}.|.}.|.|.|.|.f
-00001c20: 023c 007c 1253 0029 0e7a ff43 6f6d 7075  .<.|.S.).z.Compu
-00001c30: 7465 2049 4f55 7320 616d 6f6e 6720 696e  te IOUs among in
-00001c40: 7374 616e 6365 7320 6672 6f6d 2074 6865  stances from the
-00001c50: 2073 616d 6520 696d 6167 652e 204d 6f73   same image. Mos
-00001c60: 7420 6c69 6b65 6c79 2075 7365 6420 666f  t likely used fo
-00001c70: 7220 6e6d 732e 0a0a 2020 2020 4172 6773  r nms...    Args
-00001c80: 3a0a 2020 2020 2020 2020 7072 6564 3a20  :.        pred: 
-00001c90: 4120 6d6f 6465 6c20 7072 6564 6963 7469  A model predicti
-00001ca0: 6f6e 2064 6963 7469 6f6e 6172 790a 2020  on dictionary.  
-00001cb0: 2020 2020 2020 7468 7265 7368 6f6c 643a        threshold:
-00001cc0: 2053 6567 6d65 6e74 6174 696f 6e20 7468   Segmentation th
-00001cd0: 7265 7368 6f6c 642e 2044 6566 6175 6c74  reshold. Default
-00001ce0: 2069 7320 302e 352e 0a0a 2020 2020 5265   is 0.5...    Re
-00001cf0: 7475 726e 733a 0a20 2020 2020 2020 2069  turns:.        i
-00001d00: 6f75 733a 2049 4f55 7320 6173 2061 6e20  ous: IOUs as an 
-00001d10: 7570 7065 7220 7472 6961 676c 6520 6d61  upper triagle ma
-00001d20: 7472 6978 2e0a 2020 2020 7208 0000 0072  trix..    r....r
-00001d30: 0100 0000 7228 0000 0072 1000 0000 e903  ....r(...r......
-00001d40: 0000 0072 6400 0000 7229 0000 0072 2a00  ...rd...r)...r*.
-00001d50: 0000 4e72 0f00 0000 7267 0000 0072 1100  ..Nr....rg...r..
-00001d60: 0000 7249 0000 0029 0c72 3f00 0000 7209  ..rI...).r?...r.
-00001d70: 0000 00da 026e 70da 0474 7269 7572 3800  .....np..triur8.
-00001d80: 0000 7213 0000 00da 0761 7361 7272 6179  ..r......asarray
-00001d90: 725c 0000 00da 036c 656e 726a 0000 0072  r\.....lenrj...r
-00001da0: 4d00 0000 724a 0000 0029 1372 2f00 0000  M...rJ...).r/...
-00001db0: 7234 0000 0072 3e00 0000 5a08 626f 785f  r4...r>...Z.box_
-00001dc0: 696f 7573 da02 6379 da02 6378 da08 7061  ious..cy..cx..pa
-00001dd0: 645f 7369 7a65 7224 0000 005a 0970 6174  d_sizer$...Z.pat
-00001de0: 6368 6573 5f79 5a09 7061 7463 6865 735f  ches_yZ.patches_
-00001df0: 785a 0670 6c74 5f74 6fda 0264 79da 0264  xZ.plt_to..dy..d
-00001e00: 7872 5700 0000 da06 756e 696f 6e73 5a07  xrW.....unionsZ.
-00001e10: 6172 6561 735f 795a 0761 7265 6173 5f78  areas_yZ.areas_x
-00001e20: 7256 0000 00da 096d 6173 6b5f 696f 7573  rV.....mask_ious
-00001e30: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
-00001e40: 1f69 6f75 735f 6f66 5f70 6174 6368 6573  .ious_of_patches
-00001e50: 5f66 726f 6d5f 7361 6d65 5f69 6d61 6765  _from_same_image
-00001e60: fd00 0000 733e 0000 0000 0b08 010a 010c  ....s>..........
-00001e70: 0412 010e 0212 0108 0108 0120 0216 0116  ........... ....
-00001e80: ff02 0202 fe02 ff02 0616 0116 ff02 0202  ................
-00001e90: fe02 ff02 0610 0134 0122 0112 020e 010e  .......4."......
-00001ea0: 0214 0204 010c 0272 7a00 0000 e733 3333  .......rz....333
-00001eb0: 3333 33e3 3f29 0372 2f00 0000 da0d 696f  333.?).r/.....io
-00001ec0: 755f 7468 7265 7368 6f6c 6472 0e00 0000  u_thresholdr....
-00001ed0: 6302 0000 0000 0000 0000 0000 0007 0000  c...............
-00001ee0: 0004 0000 0043 0000 0073 7c00 0000 7400  .....C...s|...t.
-00001ef0: 7c00 8301 7d02 7c02 7c01 6b04 7d03 6401  |...}.|.|.k.}.d.
-00001f00: 7d04 7401 a002 7c03 a101 7c04 6b03 726e  }.t...|...|.k.rn
-00001f10: 7403 a002 7c03 a101 7d04 7c03 6a04 6401  t...|...}.|.j.d.
-00001f20: 6402 8d01 0f00 7d05 7c03 7c05 6403 6403  d.....}.|.|.d.d.
-00001f30: 8502 6403 6602 1900 4000 6a04 6401 6402  ..d.f...@.j.d.d.
-00001f40: 8d01 7d06 7c03 7c06 6403 6403 8502 6403  ..}.|.|.d.d...d.
-00001f50: 6602 1900 0f00 4000 7d03 7114 7c03 6a04  f.....@.}.q.|.j.
-00001f60: 6401 6402 8d01 0f00 5300 2904 7ad5 5065  d.d.....S.).z.Pe
-00001f70: 7266 6f72 6d20 6e6d 7320 6f6e 2074 6865  rform nms on the
-00001f80: 206d 6f64 656c 2070 7265 6469 6374 696f   model predictio
-00001f90: 6e20 6261 7365 6420 6f6e 206d 6173 6b20  n based on mask 
-00001fa0: 494f 550a 0a20 2020 2041 7267 733a 0a20  IOU..    Args:. 
-00001fb0: 2020 2020 2020 2070 7265 643a 2041 206d         pred: A m
-00001fc0: 6f64 656c 2070 7265 6469 6374 696f 6e20  odel prediction 
-00001fd0: 6469 6374 696f 6e61 7279 0a20 2020 2020  dictionary.     
-00001fe0: 2020 2069 6f75 735f 7468 7265 7368 6f6c     ious_threshol
-00001ff0: 643a 2064 6566 6175 6c74 2030 2e36 0a0a  d: default 0.6..
-00002000: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00002010: 2020 2020 206d 6173 6b3a 2062 6f6f 6c65       mask: boole
-00002020: 616e 206d 6173 6b20 6f66 2063 656c 6c73  an mask of cells
-00002030: 206e 6f74 2073 7570 7265 7373 6564 0a20   not supressed. 
-00002040: 2020 2072 0100 0000 7211 0000 004e 2905     r....r....N).
-00002050: 727a 0000 0072 6f00 0000 724a 0000 0072  rz...ro...rJ...r
-00002060: 1400 0000 7236 0000 0029 0772 2f00 0000  ....r6...).r/...
-00002070: 727c 0000 0072 5600 0000 7261 0000 00da  r|...rV...ra....
-00002080: 0363 6e74 da13 6361 6e5f 7375 7070 7265  .cnt..can_suppre
-00002090: 7373 5f6f 7468 6572 73da 0a73 7570 7072  ss_others..suppr
-000020a0: 6573 7365 6472 2500 0000 7225 0000 0072  essedr%...r%...r
-000020b0: 2600 0000 da1c 6e6f 6e5f 6d61 785f 7375  &.....non_max_su
-000020c0: 7070 7265 7373 5f70 7265 6469 6374 696f  ppress_predictio
-000020d0: 6e73 3001 0000 7312 0000 0000 0b08 0108  ns0...s.........
-000020e0: 0204 010e 010a 010e 011c 0118 0272 8000  .............r..
-000020f0: 0000 5429 01da 0d65 6467 655f 696e 6465  ..T)...edge_inde
-00002100: 7869 6e67 2903 722f 0000 00da 0573 6361  xing).r/.....sca
-00002110: 6c65 720e 0000 0063 0200 0000 0000 0000  ler....c........
-00002120: 0000 0000 0b00 0000 0600 0000 4300 0000  ............C...
-00002130: 732a 0100 007c 0064 0119 0064 0264 0285  s*...|.d...d.d..
-00002140: 0264 0364 0366 0319 0064 0417 007c 0114  .d.d.f...d...|..
-00002150: 007d 027c 0064 0519 0064 0264 0285 0264  .}.|.d...d.d...d
-00002160: 0364 0366 0319 0064 0417 007c 0114 007d  .d.f...d...|...}
-00002170: 037c 0064 0619 007d 0474 007c 046a 0164  .|.d...}.t.|.j.d
-00002180: 0719 007c 0114 0083 017d 0574 026a 0364  ...|.....}.t.j.d
-00002190: 027c 0585 0264 027c 0585 0266 0219 005c  .|...d.|...f...\
-000021a0: 027d 067d 0774 02a0 047c 0264 0264 0285  .}.}.t...|.d.d..
-000021b0: 0264 0264 0266 0319 00a1 01a0 0574 06a1  .d.d.f.......t..
-000021c0: 017c 0617 007d 0674 02a0 047c 0364 0264  .|...}.t...|.d.d
-000021d0: 0285 0264 0264 0266 0319 00a1 01a0 0574  ...d.d.f.......t
-000021e0: 06a1 017c 0717 007d 077c 0664 0417 007c  ...|...}.|.d...|
-000021f0: 011b 007c 0064 0119 0064 0264 0285 0264  ...|.d...d.d...d
-00002200: 0264 0885 0264 0264 0885 0266 0319 0018  .d...d.d...f....
-00002210: 007d 087c 0764 0417 007c 011b 007c 0064  .}.|.d...|...|.d
-00002220: 0519 0064 0264 0285 0264 0264 0885 0264  ...d.d...d.d...d
-00002230: 0264 0885 0266 0319 0018 007d 0974 077c  .d...f.....}.t.|
-00002240: 0474 086a 097c 087c 0967 0264 0764 098d  .t.j.|.|.g.d.d..
-00002250: 0283 027d 0a7c 0a7c 067c 0766 0353 0029  ...}.|.|.|.f.S.)
-00002260: 0a61 9902 0000 5265 7363 616c 652f 7265  .a....Rescale/re
-00002270: 7369 7a65 2069 6e73 7461 6e63 6520 6f75  size instance ou
-00002280: 7470 7574 7320 696e 2061 2073 7562 2d70  tputs in a sub-p
-00002290: 6978 656c 2061 6363 7572 6174 6520 7761  ixel accurate wa
-000022a0: 792e 0a20 2020 2049 6620 7468 6520 696e  y..    If the in
-000022b0: 7075 7420 696d 6167 6520 7761 7320 7265  put image was re
-000022c0: 7363 616c 6564 2c20 7468 6973 2066 756e  scaled, this fun
-000022d0: 6374 696f 6e20 7461 6b65 2063 6172 6520  ction take care 
-000022e0: 6f66 2072 6573 6361 6c69 6e67 2074 6865  of rescaling the
-000022f0: 2070 7265 6469 6374 696f 6e73 0a20 2020   predictions.   
-00002300: 2074 6f20 7468 6520 6f72 6769 6e61 6c20   to the orginal 
-00002310: 636f 6f64 696e 6174 6573 2e0a 0a20 2020  coodinates...   
-00002320: 2041 7267 733a 0a20 2020 2020 2020 2070   Args:.        p
-00002330: 7265 643a 2041 206d 6f64 656c 2070 7265  red: A model pre
-00002340: 6469 6374 696f 6e20 6469 6374 696f 6e61  diction dictiona
-00002350: 7279 0a20 2020 2020 2020 2073 6361 6c65  ry.        scale
-00002360: 3a20 5468 6520 7363 616c 696e 6720 7661  : The scaling va
-00002370: 6c75 652e 2054 6865 2066 756e 6374 696f  lue. The functio
-00002380: 6e20 646f 6573 206e 6f74 2074 616b 6520  n does not take 
-00002390: 6120 6e6f 6f70 2073 686f 7274 6375 7420  a noop shortcut 
-000023a0: 6576 656e 2069 6620 7363 616c 6520 6973  even if scale is
-000023b0: 2031 2e0a 0a20 2020 2052 6574 7572 6e73   1...    Returns
-000023c0: 3a20 4120 7475 706c 6520 6f66 2074 6872  : A tuple of thr
-000023d0: 6565 2061 7272 6179 730a 2020 2020 2020  ee arrays.      
-000023e0: 2020 7061 7463 6865 733a 2061 2033 4420    patches: a 3D 
-000023f0: 6172 7261 7920 6f66 2074 6865 2072 6573  array of the res
-00002400: 6361 6c65 6420 7365 676d 656e 7461 7469  caled segmentati
-00002410: 6f6e 2070 6174 6368 6573 2e20 5468 6520  on patches. The 
-00002420: 6172 7261 7920 7368 6170 6520 7368 6f75  array shape shou
-00002430: 6c64 2062 6520 6469 6666 6572 656e 7420  ld be different 
-00002440: 6672 6f6d 0a20 2020 2020 2020 2020 2020  from.           
-00002450: 2074 6865 206f 7269 676e 616c 2070 6174   the orignal pat
-00002460: 6368 6573 2069 6e20 6d6f 6465 6c20 7072  ches in model pr
-00002470: 6564 6974 696f 6e2e 0a20 2020 2020 2020  edition..       
-00002480: 2079 793a 2054 6865 2079 2d63 6f6f 7264   yy: The y-coord
-00002490: 696e 6174 6573 206f 6620 7468 6520 7061  inates of the pa
-000024a0: 7463 6865 7320 696e 206d 6573 682d 6772  tches in mesh-gr
-000024b0: 6964 2066 6f72 6d61 740a 2020 2020 2020  id format.      
-000024c0: 2020 7878 3a20 5468 6520 782d 636f 6f72    xx: The x-coor
-000024d0: 6469 6e61 7465 7320 6f66 2074 6865 2070  dinates of the p
-000024e0: 6174 6368 6573 2069 6e20 6d65 7368 2d67  atches in mesh-g
-000024f0: 7269 6420 666f 726d 6174 0a20 2020 2072  rid format.    r
-00002500: 2900 0000 4e72 0100 0000 7233 0000 0072  )...Nr....r3...r
-00002510: 2a00 0000 7228 0000 0072 1000 0000 7208  *...r(...r....r.
-00002520: 0000 0072 1100 0000 290a da05 726f 756e  ...r....)...roun
-00002530: 6472 1300 0000 7214 0000 0072 1900 0000  dr....r....r....
-00002540: da05 666c 6f6f 7272 1600 0000 7217 0000  ..floorr....r...
-00002550: 00da 0c5f 7361 6d70 6c69 6e67 5f6f 7072  ..._sampling_opr
-00002560: 6f00 0000 721a 0000 0029 0b72 2f00 0000  o...r....).r/...
-00002570: 7282 0000 005a 066e 6577 5f79 305a 066e  r....Z.new_y0Z.n
-00002580: 6577 5f78 30da 0570 6174 6368 da02 7073  ew_x0..patch..ps
-00002590: 721f 0000 0072 2000 0000 5a06 7265 6c5f  r....r ...Z.rel_
-000025a0: 7979 5a06 7265 6c5f 7878 5a09 6e65 775f  yyZ.rel_xxZ.new_
-000025b0: 7061 7463 6872 2500 0000 7225 0000 0072  patchr%...r%...r
-000025c0: 2600 0000 da0f 7265 7363 616c 655f 7061  &.....rescale_pa
-000025d0: 7463 6865 734b 0100 0073 3000 0000 0012  tchesK...s0.....
-000025e0: 1e01 1e01 0801 1202 1a02 20ff 0204 20ff  .......... ... .
-000025f0: 0204 1801 02ff 0401 02ff 0a03 1801 02ff  ................
-00002600: 0401 02ff 0a03 0201 0201 10fe 0405 7288  ..............r.
-00002610: 0000 0029 0172 3300 0000 2902 4e72 3300  ...).r3...).Nr3.
-00002620: 0000 2902 7244 0000 0072 3300 0000 2901  ..).rD...r3...).
-00002630: 7233 0000 0029 044e 7233 0000 0072 3300  r3...).Nr3...r3.
-00002640: 0000 7201 0000 0029 0172 3300 0000 2901  ..r....).r3...).
-00002650: 727b 0000 0029 23da 075f 5f64 6f63 5f5f  r{...)#..__doc__
-00002660: da09 6675 6e63 746f 6f6c 7372 0200 0000  ..functoolsr....
-00002670: da06 7479 7069 6e67 7203 0000 0072 0400  ..typingr....r..
-00002680: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
-00002690: 00da 036a 6178 da09 6a61 782e 6e75 6d70  ...jax..jax.nump
-000026a0: 79da 056e 756d 7079 7214 0000 0072 6f00  y..numpyr....ro.
-000026b0: 0000 da05 626f 7865 7372 0900 0000 da05  ....boxesr......
-000026c0: 696d 6167 6572 0a00 0000 da07 6e64 6172  imager......ndar
-000026d0: 7261 7972 1700 0000 da05 7475 706c 6572  rayr......tupler
-000026e0: 2700 0000 7232 0000 00da 0566 6c6f 6174  '...r2.....float
-000026f0: 723f 0000 0072 4300 0000 722c 0000 0072  r?...rC...r,...r
-00002700: 5b00 0000 7260 0000 0072 6d00 0000 727a  [...r`...rm...rz
-00002710: 0000 0072 8000 0000 da04 766d 6170 7285  ...r......vmapr.
-00002720: 0000 0072 8800 0000 7225 0000 0072 2500  ...r....r%...r%.
-00002730: 0000 7225 0000 0072 2600 0000 da08 3c6d  ..r%...r&.....<m
-00002740: 6f64 756c 653e 0100 0000 737e 0000 0004  odule>....s~....
-00002750: 050c 011c 0208 010c 0108 020c 010c 0404  ................
-00002760: 0004 0002 0102 fe0c 2908 0f00 ff02 010a  ........).......
-00002770: 0002 0104 fe0c 2600 0100 fd02 010a 010a  ......&.........
-00002780: 0102 0102 fc0c 2100 0000 ff02 0102 0004  ......!.........
-00002790: 0002 0002 0104 fe0c 2c00 ff02 0102 000a  ........,.......
-000027a0: 0002 0104 fe0c 1d00 0100 0100 0100 fa02  ................
-000027b0: 0102 010a 0108 0102 0102 0102 0104 f90c  ................
-000027c0: 2c16 3316 1812 0402 0002 0112 fe         ,.3..........
+00000040: 6403 6c03 5a03 6401 6403 6c04 6d05 5a06  d.l.Z.d.d.l.m.Z.
+00000050: 0100 6401 6403 6c05 5a07 6401 6404 6c08  ..d.d.l.Z.d.d.l.
+00000060: 5400 6405 6406 6c09 6d0a 5a0a 0100 6405  T.d.d.l.m.Z...d.
+00000070: 6407 6c0b 6d0c 5a0c 0100 650d 650d 650e  d.l.m.Z...e.e.e.
+00000080: 650f 6510 6510 6510 6510 6604 1900 6408  e.e.e.e.e.f...d.
+00000090: 9c04 6409 640a 8404 5a11 640b 640c 8400  ..d.d...Z.d.d...
+000000a0: 5a12 6428 6513 6514 6515 6602 1900 6516  Z.d(e.e.e.f...e.
+000000b0: 6506 6a17 640e 9c03 640f 6410 8405 5a18  e.j.d...d.d...Z.
+000000c0: 6429 6513 6514 6515 6602 1900 650f 650e  d)e.e.e.f...e.e.
+000000d0: 650e 6602 1900 6516 6510 6411 9c04 6412  e.f...e.e.d...d.
+000000e0: 6413 8405 5a19 642a 6515 650d 650e 6516  d...Z.d*e.e.e.e.
+000000f0: 6510 6415 9c05 6416 6417 8405 5a1a 642b  e.d...d.d...Z.d+
+00000100: 6515 651b 6516 6510 6411 9c04 6418 6419  e.e.e.e.d...d.d.
+00000110: 8405 5a1c 642c 6515 651b 651d 650d 1900  ..Z.d,e.e.e.e...
+00000120: 6516 6516 650e 6510 641a 9c07 641b 641c  e.e.e.e.d...d.d.
+00000130: 8405 5a1e 642d 6515 6516 6510 640e 9c03  ..Z.d-e.e.e.d...
+00000140: 641d 641e 8405 5a1f 642e 6515 6516 6510  d.d...Z.d.e.e.e.
+00000150: 6420 9c03 6421 6422 8405 5a20 6503 a021  d ..d!d"..Z e..!
+00000160: 6502 650c 6423 6424 8d02 a101 5a22 6515  e.e.d#d$....Z"e.
+00000170: 6516 650f 6510 6510 6510 6603 1900 6425  e.e.e.e.e.f...d%
+00000180: 9c03 6426 6427 8404 5a23 6403 5300 292f  ..d&d'..Z#d.S.)/
+00000190: 7a86 2056 6172 696f 7573 2066 756e 6374  z. Various funct
+000001a0: 696f 6e73 2064 6561 6c73 2077 6974 6820  ions deals with 
+000001b0: 7365 676d 656e 7461 7469 6f6e 2070 6174  segmentation pat
+000001c0: 6863 6573 0a0a 2020 2020 416c 6c20 6675  hces..    All fu
+000001d0: 6e63 7469 6f6e 7320 6865 7265 2074 616b  nctions here tak
+000001e0: 6573 2075 6e62 6174 6368 6564 2069 6e70  es unbatched inp
+000001f0: 7574 2e20 5573 6520 766d 6170 2074 6f20  ut. Use vmap to 
+00000200: 636f 6e76 6572 7420 746f 2062 6174 6368  convert to batch
+00000210: 6564 2064 6174 610a e900 0000 0029 01da  ed data......)..
+00000220: 0770 6172 7469 616c 4e29 01da 012a e901  .partialN)...*..
+00000230: 0000 0029 01da 1262 6f78 5f69 6f75 5f73  ...)...box_iou_s
+00000240: 696d 696c 6172 6974 7929 01da 1173 7562  imilarity)...sub
+00000250: 5f70 6978 656c 5f73 616d 706c 6573 2904  _pixel_samples).
+00000260: da08 6665 6174 7572 6573 da09 6c6f 6361  ..features..loca
+00000270: 7469 6f6e 73da 0a70 6174 6368 5f73 697a  tions..patch_siz
+00000280: 65da 0672 6574 7572 6e63 0300 0000 0000  e..returnc......
+00000290: 0000 0000 0000 1000 0000 0600 0000 4300  ..............C.
+000002a0: 0000 7338 0100 007c 006a 005c 037d 037d  ..s8...|.j.\.}.}
+000002b0: 047d 057c 0174 01a0 027c 037c 0467 02a1  .}.|.t...|.|.g..
+000002c0: 0139 007d 017c 01a0 0374 04a1 017d 0674  .9.}.|...t...}.t
+000002d0: 01a0 057c 0664 0164 0185 0264 0266 0219  ...|.d.d...d.f..
+000002e0: 0064 037c 0464 0218 00a1 037d 0774 01a0  .d.|.d.....}.t..
+000002f0: 057c 0664 0164 0185 0264 0366 0219 0064  .|.d.d...d.f...d
+00000300: 037c 0364 0218 00a1 037d 0874 016a 0664  .|.d.....}.t.j.d
+00000310: 017c 0285 0264 017c 0285 0266 0219 007c  .|...d.|...f...|
+00000320: 0264 041a 0018 005c 027d 097d 0a7c 0a7c  .d.....\.}.}.|.|
+00000330: 0764 0164 0185 0264 0164 0166 0319 0037  .d.d...d.d.f...7
+00000340: 007d 0a7c 097c 0864 0164 0185 0264 0164  .}.|.|.d.d...d.d
+00000350: 0166 0319 0037 007d 097c 0174 016a 077c  .f...7.}.|.t.j.|
+00000360: 087c 0767 0264 0564 068d 0218 007d 0b7c  .|.g.d.d.....}.|
+00000370: 0264 041a 0064 0217 007d 0c7c 0c7c 0c67  .d...d...}.|.|.g
+00000380: 027c 0c7c 0c67 0264 0364 0367 0267 037d  .|.|.g.d.d.g.g.}
+00000390: 0d74 01a0 087c 007c 0da1 027d 0e7c 0e7c  .t...|.|...}.|.|
+000003a0: 097c 0c17 007c 0a7c 0c17 0064 0164 0185  .|...|.|...d.d..
+000003b0: 0266 0319 007d 0f7c 0f7c 0964 0164 0185  .f...}.|.|.d.d..
+000003c0: 0264 0364 0366 0319 007c 0a64 0164 0185  .d.d.f...|.d.d..
+000003d0: 0264 0364 0366 0319 007c 0b66 0453 0029  .d.d.f...|.f.S.)
+000003e0: 0761 5501 0000 6578 7472 6163 7420 6665  .aU...extract fe
+000003f0: 6174 7572 6520 7061 7463 6865 7320 6163  ature patches ac
+00000400: 636f 7264 696e 6720 746f 2061 206c 6973  cording to a lis
+00000410: 7420 6f66 206c 6f63 6174 696f 6e73 0a0a  t of locations..
+00000420: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00000430: 2020 6665 6174 7572 6573 3a20 5b48 2c57    features: [H,W
+00000440: 2c43 5d20 7374 616e 6461 7264 2032 4420  ,C] standard 2D 
+00000450: 6665 6174 7572 6520 6d61 700a 2020 2020  feature map.    
+00000460: 2020 2020 6c6f 6361 7469 6f6e 733a 205b      locations: [
+00000470: 4e2c 2032 5d20 666c 6f61 7433 322c 2073  N, 2] float32, s
+00000480: 6361 6c65 6420 302e 2e31 0a20 2020 2020  caled 0..1.     
+00000490: 2020 2070 6174 6368 5f73 697a 653a 2069     patch_size: i
+000004a0: 6e74 0a0a 2020 2020 5265 7475 726e 733a  nt..    Returns:
+000004b0: 0a20 2020 2020 2020 2070 6174 6368 6573  .        patches
+000004c0: 3a20 5b4e 2c20 7061 7463 685f 7369 7a65  : [N, patch_size
+000004d0: 2c20 7061 7463 685f 7369 7a65 2c20 435d  , patch_size, C]
+000004e0: 0a20 2020 2020 2020 2079 303a 205b 4e5d  .        y0: [N]
+000004f0: 3a20 7930 2063 6f6f 7264 696e 6174 6573  : y0 coordinates
+00000500: 206f 6620 7061 7463 6865 730a 2020 2020   of patches.    
+00000510: 2020 2020 7830 3a20 5b4e 5d3a 2078 3020      x0: [N]: x0 
+00000520: 636f 6f72 6469 6e61 7465 7320 6f66 2070  coordinates of p
+00000530: 6174 6368 6573 0a20 2020 204e 7204 0000  atches.    Nr...
+00000540: 0072 0100 0000 e902 0000 00e9 ffff ffff  .r..............
+00000550: a901 da04 6178 6973 2909 da05 7368 6170  ....axis)...shap
+00000560: 65da 036a 6e70 da05 6172 7261 79da 0661  e..jnp..array..a
+00000570: 7374 7970 65da 0369 6e74 da04 636c 6970  stype..int..clip
+00000580: da05 6d67 7269 64da 0573 7461 636b da03  ..mgrid..stack..
+00000590: 7061 6429 1072 0700 0000 7208 0000 0072  pad).r....r....r
+000005a0: 0900 0000 da06 6865 6967 6874 da05 7769  ......height..wi
+000005b0: 6474 68da 015f 5a0b 695f 6c6f 6361 7469  dth.._Z.i_locati
+000005c0: 6f6e 735a 0d69 5f6c 6f63 6174 696f 6e73  onsZ.i_locations
+000005d0: 5f78 5a0d 695f 6c6f 6361 7469 6f6e 735f  _xZ.i_locations_
+000005e0: 79da 0279 79da 0278 78da 0972 656d 6169  y..yy..xx..remai
+000005f0: 6e64 6572 da0c 7061 6464 696e 675f 7369  nder..padding_si
+00000600: 7a65 da08 7061 6464 696e 6773 5a0f 7061  ze..paddingsZ.pa
+00000610: 6464 6564 5f66 6561 7475 7265 73da 0770  dded_features..p
+00000620: 6174 6368 6573 a900 7221 0000 00fa 342f  atches..r!....4/
+00000630: 686f 6d65 2f46 4341 4d2f 6a79 752f 7072  home/FCAM/jyu/pr
+00000640: 6f6a 5f6c 6163 7373 2f6c 6163 7373 2f6c  oj_lacss/lacss/l
+00000650: 6163 7373 2f6f 7073 2f70 6174 6368 6573  acss/ops/patches
+00000660: 2e70 79da 0e67 6174 6865 725f 7061 7463  .py..gather_patc
+00000670: 6865 7312 0000 0073 2200 0000 000f 0c02  hes....s".......
+00000680: 1202 0a01 1e01 1e01 2201 1601 1601 1603  ........".......
+00000690: 0c02 0601 0601 06fd 0405 0c02 1a02 7223  ..............r#
+000006a0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000006b0: 0400 0000 0300 0000 4300 0000 734e 0000  ........C...sN..
+000006c0: 0074 007c 0074 0183 0272 247c 0064 0119  .t.|.t...r$|.d..
+000006d0: 007d 017c 0064 0219 007d 027c 0064 0319  .}.|.d...}.|.d..
+000006e0: 007d 036e 0a7c 005c 037d 017d 027d 037c  .}.n.|.\.}.}.}.|
+000006f0: 016a 027c 026a 026b 0472 447c 01a0 0364  .j.|.j.k.rD|...d
+00000700: 04a1 017d 017c 017c 027c 0366 0353 0029  ...}.|.|.|.f.S.)
+00000710: 054e da0f 696e 7374 616e 6365 5f6f 7574  .N..instance_out
+00000720: 7075 74da 0b69 6e73 7461 6e63 655f 7963  put..instance_yc
+00000730: da0b 696e 7374 616e 6365 5f78 6372 0c00  ..instance_xcr..
+00000740: 0000 2904 da0a 6973 696e 7374 616e 6365  ..)...isinstance
+00000750: da04 6469 6374 da04 6e64 696d da07 7371  ..dict..ndim..sq
+00000760: 7565 657a 6529 04da 0470 7265 6472 2000  ueeze)...predr .
+00000770: 0000 da02 7963 da02 7863 7221 0000 0072  ....yc..xcr!...r
+00000780: 2100 0000 7222 0000 00da 0f5f 6765 745f  !...r"....._get_
+00000790: 7061 7463 685f 6461 7461 3b00 0000 7310  patch_data;...s.
+000007a0: 0000 0000 010a 0108 0108 010a 020a 020c  ................
+000007b0: 010a 0272 2e00 0000 e700 0000 0000 00e0  ...r............
+000007c0: 3f29 0372 2b00 0000 da09 7468 7265 7368  ?).r+.....thresh
+000007d0: 6f6c 6472 0a00 0000 6302 0000 0000 0000  oldr....c.......
+000007e0: 0000 0000 0010 0000 0006 0000 0043 0000  .............C..
+000007f0: 0073 2801 0000 7400 7c00 8301 5c03 7d02  .s(...t.|...\.}.
+00000800: 7d03 7d04 7c02 6a01 5c03 7d05 7d06 7d07  }.}.|.j.\.}.}.}.
+00000810: 7402 6a03 7c02 7c01 6b04 6401 6402 8d02  t.j.|.|.k.d.d...
+00000820: 7d08 7402 6a03 7c02 7c01 6b04 6403 6402  }.t.j.|.|.k.d.d.
+00000830: 8d02 7d09 7c08 6a04 6401 6402 8d01 7d0a  ..}.|.j.d.d...}.
+00000840: 7c07 7c08 6404 6404 8502 6404 6404 6405  |.|.d.d...d.d.d.
+00000850: 8503 6602 1900 6a04 6401 6402 8d01 1800  ..f...j.d.d.....
+00000860: 7d0b 7c09 6a04 6401 6402 8d01 7d0c 7c06  }.|.j.d.d...}.|.
+00000870: 7c09 6404 6404 8502 6404 6404 6405 8503  |.d.d...d.d.d...
+00000880: 6602 1900 6a04 6401 6402 8d01 1800 7d0d  f...j.d.d.....}.
+00000890: 7c0c 7c03 6404 6404 8502 6406 6406 6603  |.|.d.d...d.d.f.
+000008a0: 1900 3700 7d0c 7c0d 7c03 6404 6404 8502  ..7.}.|.|.d.d...
+000008b0: 6406 6406 6603 1900 3700 7d0d 7c0a 7c04  d.d.f...7.}.|.|.
+000008c0: 6404 6404 8502 6406 6406 6603 1900 3700  d.d...d.d.f...7.
+000008d0: 7d0a 7c0b 7c04 6404 6404 8502 6406 6406  }.|.|.d.d...d.d.
+000008e0: 6603 1900 3700 7d0b 7c08 6a03 6401 6407  f...7.}.|.j.d.d.
+000008f0: 6408 8d02 7d0e 7402 6a05 7c0c 7c0a 7c0d  d...}.t.j.|.|.|.
+00000900: 7c0b 6704 6405 6402 8d02 7d0f 7402 a006  |.g.d.d...}.t...
+00000910: 7c0e 7c0f 6405 a103 7d0f 7c0f 5300 2909  |.|.d...}.|.S.).
+00000920: 7af0 436f 6d70 7574 6520 7468 6520 696e  z.Compute the in
+00000930: 7374 616e 6365 2062 626f 7865 7320 6672  stance bboxes fr
+00000940: 6f6d 206d 6f64 656c 2070 7265 6469 6374  om model predict
+00000950: 696f 6e73 0a0a 2020 2020 4172 6773 3a0a  ions..    Args:.
+00000960: 2020 2020 2020 2020 7072 6564 3a20 4120          pred: A 
+00000970: 6d6f 6465 6c20 7072 6564 6963 7469 6f6e  model prediction
+00000980: 2064 6963 7469 6f6e 6172 793a 0a20 2020   dictionary:.   
+00000990: 2020 2020 2074 6872 6573 686f 6c64 3a20       threshold: 
+000009a0: 666f 7220 7365 676d 656e 7461 7469 6f6e  for segmentation
+000009b0: 2c20 6465 6661 756c 7420 302e 350a 0a20  , default 0.5.. 
+000009c0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+000009d0: 2020 2020 6262 6f78 6573 3a20 5b6e 2c20      bboxes: [n, 
+000009e0: 345d 2062 626f 6f78 2066 6f72 2065 6d70  4] bboox for emp
+000009f0: 7479 2070 6174 6368 6573 2061 7265 2066  ty patches are f
+00000a00: 696c 6c65 6420 7769 7468 202d 310a 2020  illed with -1.  
+00000a10: 2020 7204 0000 0072 0d00 0000 720b 0000    r....r....r...
+00000a20: 004e 720c 0000 0072 0100 0000 5429 0272  .Nr....r....T).r
+00000a30: 0e00 0000 da08 6b65 6570 6469 6d73 2907  ......keepdims).
+00000a40: 722e 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
+00000a50: 0361 6e79 da06 6172 676d 6178 7216 0000  .any..argmaxr...
+00000a60: 00da 0577 6865 7265 2910 722b 0000 0072  ...where).r+...r
+00000a70: 3000 0000 7220 0000 0072 1b00 0000 721c  0...r ...r....r.
+00000a80: 0000 0072 1a00 0000 da02 6430 da02 6431  ...r......d0..d1
+00000a90: da08 726f 775f 6d61 736b da08 636f 6c5f  ..row_mask..col_
+00000aa0: 6d61 736b 5a07 6d69 6e5f 636f 6cda 076d  maskZ.min_col..m
+00000ab0: 6178 5f63 6f6c 5a07 6d69 6e5f 726f 775a  ax_colZ.min_rowZ
+00000ac0: 076d 6178 5f72 6f77 da08 6973 5f76 616c  .max_row..is_val
+00000ad0: 6964 da06 6262 6f78 6573 7221 0000 0072  id..bboxesr!...r
+00000ae0: 2100 0000 7222 0000 00da 1162 626f 7865  !...r".....bboxe
+00000af0: 735f 6f66 5f70 6174 6368 6573 4900 0000  s_of_patchesI...
+00000b00: 7320 0000 0000 0c0e 020c 0112 0112 020c  s ..............
+00000b10: 0122 020c 0122 0216 0116 0116 0116 020e  ."..."..........
+00000b20: 0116 010e 0272 3c00 0000 2904 722b 0000  .....r<...).r+..
+00000b30: 00da 0a69 6e70 7574 5f73 697a 6572 3000  ...input_sizer0.
+00000b40: 0000 720a 0000 0063 0300 0000 0000 0000  ..r....c........
+00000b50: 0000 0000 0b00 0000 0400 0000 4300 0000  ............C...
+00000b60: 7398 0000 0074 007c 0083 015c 037d 037d  s....t.|...\.}.}
+00000b70: 047d 057c 037c 026b 057d 067c 047c 0619  .}.|.|.k.}.|.|..
+00000b80: 007d 047c 057c 0619 007d 0574 01a0 027c  .}.|.|...}.t...|
+00000b90: 06a1 0164 0164 0185 0264 0266 0219 007d  ...d.d...d.f...}
+00000ba0: 077c 0164 016b 0972 847c 015c 027d 087d  .|.d.k.r.|.\.}.}
+00000bb0: 097c 0464 026b 057c 047c 086b 0040 007c  .|.d.k.|.|.k.@.|
+00000bc0: 0564 026b 057c 057c 096b 0040 0040 007d  .d.k.|.|.k.@.@.}
+00000bd0: 0a7c 047c 0a19 007d 047c 057c 0a19 007d  .|.|...}.|.|...}
+00000be0: 057c 077c 0a19 007d 0774 016a 037c 047c  .|.|...}.t.j.|.|
+00000bf0: 057c 0767 0364 0364 048d 0253 0029 0561  .|.g.d.d...S.).a
+00000c00: 1b01 0000 436f 6d70 7574 6520 7978 2063  ....Compute yx c
+00000c10: 6f6f 6469 6e61 7465 7320 6f66 2061 6c6c  oodinates of all
+00000c20: 2073 6567 6d65 6e74 6564 2069 6e73 7461   segmented insta
+00000c30: 6e63 6573 0a0a 2020 2020 4172 6773 3a0a  nces..    Args:.
+00000c40: 2020 2020 2020 2020 7072 6564 3a20 4120          pred: A 
+00000c50: 6d6f 6465 6c20 7072 6564 6963 7469 6f6e  model prediction
+00000c60: 2064 6963 7469 6f6e 6172 790a 2020 2020   dictionary.    
+00000c70: 2020 2020 7468 7265 7368 6f6c 643a 2066      threshold: f
+00000c80: 6c6f 6174 0a0a 2020 2020 5265 7475 726e  loat..    Return
+00000c90: 733a 0a20 2020 2020 2020 205b 4e2c 2033  s:.        [N, 3
+00000ca0: 5d20 6172 7261 792e 2054 6865 2066 6972  ] array. The fir
+00000cb0: 7374 2074 776f 2063 6f6c 756d 6e73 2061  st two columns a
+00000cc0: 7265 2079 2d78 2063 6f6f 7264 696e 6174  re y-x coordinat
+00000cd0: 6573 2e20 5468 6520 7468 6972 640a 2020  es. The third.  
+00000ce0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+00000cf0: 2069 7320 6120 696e 6465 7820 7661 6c75   is a index valu
+00000d00: 6520 666f 7220 6469 6666 6572 656e 7420  e for different 
+00000d10: 696e 7374 616e 6365 732e 0a20 2020 204e  instances..    N
+00000d20: 7201 0000 0072 0c00 0000 720d 0000 0029  r....r....r....)
+00000d30: 0472 2e00 0000 7210 0000 00da 0861 7267  .r....r......arg
+00000d40: 7768 6572 6572 1600 0000 290b 722b 0000  wherer....).r+..
+00000d50: 0072 3d00 0000 7230 0000 0072 2000 0000  .r=...r0...r ...
+00000d60: 721b 0000 0072 1c00 0000 da07 696e 6469  r....r......indi
+00000d70: 6365 735a 0672 6f77 6964 7372 1800 0000  cesZ.rowidsr....
+00000d80: 7219 0000 005a 0c76 616c 6964 5f63 6f6f  r....Z.valid_coo
+00000d90: 7264 7372 2100 0000 7221 0000 0072 2200  rdsr!...r!...r".
+00000da0: 0000 da12 696e 6469 6365 735f 6f66 5f70  ....indices_of_p
+00000db0: 6174 6368 6573 6d00 0000 7318 0000 0000  atchesm...s.....
+00000dc0: 0f0e 0208 0108 0108 0116 0208 0108 0120  ............... 
+00000dd0: 0108 0108 0108 0272 4000 0000 e980 0000  .......r@.......
+00000de0: 0029 0572 2b00 0000 da06 6c61 6265 6c73  .).r+.....labels
+00000df0: da0a 424c 4f43 4b5f 5349 5a45 7230 0000  ..BLOCK_SIZEr0..
+00000e00: 0072 0a00 0000 6304 0000 0000 0000 0000  .r....c.........
+00000e10: 0000 0012 0000 0008 0000 0043 0000 0073  ...........C...s
+00000e20: 6201 0000 7400 7c00 8301 5c03 7d04 7d05  b...t.|...\.}.}.
+00000e30: 7d06 7c04 7c03 6b05 7d04 7401 6a02 7c04  }.|.|.k.}.t.j.|.
+00000e40: 6401 6402 8d02 7d07 7c01 a003 7404 a101  d.d...}.|...t...
+00000e50: 7d01 7c05 6a05 6403 1900 6404 1a00 7d08  }.|.j.d...d...}.
+00000e60: 7401 6a06 7c01 7c08 6405 6406 8d03 7d09  t.j.|.|.d.d...}.
+00000e70: 7c09 7c05 7c08 1700 7c06 7c08 1700 6602  |.|.|...|.|...f.
+00000e80: 1900 7d0a 7c01 a007 a100 6407 1800 7c02  ..}.|.....d...|.
+00000e90: 1a00 6407 1700 7c02 1400 7d0b 7401 6a02  ..d...|...}.t.j.
+00000ea0: 7c01 6408 6408 8502 6408 6408 8502 6408  |.d.d...d.d...d.
+00000eb0: 6603 1900 7401 a008 7c0b a101 6407 1700  f...t...|...d...
+00000ec0: 6b02 6409 6402 8d02 7d0c 6700 7d0d 7409  k.d.d...}.g.}.t.
+00000ed0: 6407 7c01 a007 a100 6407 1700 7c02 8303  d.|.....d...|...
+00000ee0: 4400 5d74 7d0e 7c0a 7401 a008 7c0e 7c0e  D.]t}.|.t...|.|.
+00000ef0: 7c02 1700 a102 a00a 6403 6407 6407 6407  |.......d.d.d.d.
+00000f00: a104 6b02 7d0f 7c0c 7c0e 6407 1800 7c0e  ..k.}.|.|.d...|.
+00000f10: 7c02 1700 6407 1800 8502 1900 7d10 7401  |...d.......}.t.
+00000f20: 6a02 7c0f 7c04 4000 6401 6402 8d02 7d11  j.|.|.@.d.d...}.
+00000f30: 7c0d a00b 7c11 7c07 7c10 6408 6408 8502  |...|.|.|.d.d...
+00000f40: 6408 6602 1900 1700 7c11 1800 640a 1700  d.f.....|...d...
+00000f50: 1b00 a101 0100 71be 7401 6a0c 7c0d 6405  ......q.t.j.|.d.
+00000f60: 6402 8d02 a00d a100 7d0d 7c0d 6408 6408  d.......}.|.d.d.
+00000f70: 8502 6408 7c01 a007 a100 8502 6602 1900  ..d.|.......f...
+00000f80: 7d0d 7c0d 5300 290b 6102 0100 0043 6f6d  }.|.S.).a....Com
+00000f90: 7075 7465 2069 6f75 2062 6574 7765 656e  pute iou between
+00000fa0: 2070 7265 6469 6374 696f 6e20 616e 6420   prediction and 
+00000fb0: 6772 6f75 6e64 2074 7275 7468 206c 6162  ground truth lab
+00000fc0: 656c 2e0a 0a20 2020 2041 7267 733a 0a20  el...    Args:. 
+00000fd0: 2020 2020 2020 2070 7265 643a 2041 206d         pred: A m
+00000fe0: 6f64 656c 2070 7265 6469 6374 696f 6e20  odel prediction 
+00000ff0: 6469 6374 696f 6e61 7279 0a20 2020 2020  dictionary.     
+00001000: 2020 206c 6162 656c 733a 2069 6d61 6765     labels: image
+00001010: 206c 6162 656c 2e20 6267 5f6c 6162 656c   label. bg_label
+00001020: 203d 2030 0a20 2020 2020 2020 2074 6872   = 0.        thr
+00001030: 6573 686f 6c64 3a20 666f 7220 7365 676d  eshold: for segm
+00001040: 656e 7461 7469 6f6e 2e20 6465 6661 756c  entation. defaul
+00001050: 7420 6973 2030 2e35 0a0a 2020 2020 5265  t is 0.5..    Re
+00001060: 7475 726e 733a 0a20 2020 2020 2020 205b  turns:.        [
+00001070: 6e2c 206d 5d20 6172 7261 7920 6f66 2069  n, m] array of i
+00001080: 6f75 2076 616c 7565 732e 0a20 2020 2029  ou values..    )
+00001090: 0272 0c00 0000 e9fe ffff ff72 0d00 0000  .r.........r....
+000010a0: 720c 0000 0072 0b00 0000 7201 0000 0029  r....r....r....)
+000010b0: 01da 0f63 6f6e 7374 616e 745f 7661 6c75  ...constant_valu
+000010c0: 6573 7204 0000 004e 2902 7201 0000 0072  esr....N).r....r
+000010d0: 0400 0000 e73a 8c30 e28e 7945 3e29 0e72  .....:.0..yE>).r
+000010e0: 2e00 0000 7210 0000 00da 0d63 6f75 6e74  ....r......count
+000010f0: 5f6e 6f6e 7a65 726f 7212 0000 0072 1300  _nonzeror....r..
+00001100: 0000 720f 0000 0072 1700 0000 da03 6d61  ..r....r......ma
+00001110: 78da 0661 7261 6e67 65da 0572 616e 6765  x..arange..range
+00001120: da07 7265 7368 6170 65da 0661 7070 656e  ..reshape..appen
+00001130: 64da 0b63 6f6e 6361 7465 6e61 7465 da09  d..concatenate..
+00001140: 7472 616e 7370 6f73 6529 1272 2b00 0000  transpose).r+...
+00001150: 7242 0000 0072 4300 0000 7230 0000 0072  rB...rC...r0...r
+00001160: 2000 0000 722c 0000 0072 2d00 0000 5a0a   ...r,...r-...Z.
+00001170: 7072 6564 5f61 7265 6173 da04 7061 6473  pred_areas..pads
+00001180: 5a0d 7061 6464 6564 5f6c 6162 656c 735a  Z.padded_labelsZ
+00001190: 0a67 745f 7061 7463 6865 73da 0b6d 6178  .gt_patches..max
+000011a0: 5f69 6e64 6963 6573 5a0c 616c 6c5f 6774  _indicesZ.all_gt
+000011b0: 5f61 7265 6173 da04 696f 7573 da01 6bda  _areas..ious..k.
+000011c0: 0467 745f 705a 0867 745f 6172 6561 73da  .gt_pZ.gt_areas.
+000011d0: 0969 6e74 6572 7365 6374 7221 0000 0072  .intersectr!...r
+000011e0: 2100 0000 7222 0000 00da 1669 6f75 5f70  !...r".....iou_p
+000011f0: 6174 6368 6573 5f61 6e64 5f6c 6162 656c  atches_and_label
+00001200: 738d 0000 0073 3400 0000 000d 0e01 0801  s....s4.........
+00001210: 0e01 0a02 0e01 1001 1402 1801 0401 2200  ..............".
+00001220: 02ff 0604 0402 1801 1201 0200 0200 0200  ................
+00001230: 02ff 0603 1801 1201 2802 1201 1802 7255  ........(.....rU
+00001240: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+00001250: 0b00 0000 0500 0000 4300 0000 7366 0000  ........C...sf..
+00001260: 0074 007c 0083 015c 037d 037d 047d 057c  .t.|...\.}.}.}.|
+00001270: 046a 015c 037d 067d 077d 0874 02a0 037c  .j.\.}.}.}.t...|
+00001280: 06a1 017d 0974 02a0 047c 0666 017c 0117  ...}.t...|.f.|..
+00001290: 00a1 017d 0a7c 0a6a 057c 0964 0164 0185  ...}.|.j.|.d.d..
+000012a0: 0264 0164 0166 0319 007c 047c 0566 0319  .d.d.f...|.|.f..
+000012b0: 00a0 067c 03a1 017d 0a7c 0a7c 026b 05a0  ...|...}.|.|.k..
+000012c0: 0774 08a1 0153 0029 0261 db01 0000 4578  .t...S.).a....Ex
+000012d0: 7061 6e64 2074 6865 2070 7265 6469 6374  pand the predict
+000012e0: 6564 2070 6174 6368 6573 2074 6f20 7468  ed patches to th
+000012f0: 6520 6675 6c6c 2069 6d61 6765 2073 697a  e full image siz
+00001300: 652e 0a20 2020 2054 6865 2064 6566 6175  e..    The defau
+00001310: 6c74 206d 6f64 656c 2073 6567 6d65 6e74  lt model segment
+00001320: 6174 696f 6e20 6f75 7470 7574 2073 686f  ation output sho
+00001330: 7773 206f 6e6c 7920 6120 736d 616c 6c20  ws only a small 
+00001340: 7061 7463 6820 6172 6f75 6e64 2065 6163  patch around eac
+00001350: 6820 696e 7374 616e 6365 2e20 5468 6973  h instance. This
+00001360: 0a20 2020 2066 756e 6374 696f 6e20 6578  .    function ex
+00001370: 7061 6e64 2065 6163 6820 7061 7463 6820  pand each patch 
+00001380: 746f 2074 6865 2073 697a 6520 6f66 2074  to the size of t
+00001390: 6865 206f 7267 696e 616c 2069 6d61 6765  he orginal image
+000013a0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+000013b0: 2020 2020 2070 7265 643a 2041 206d 6f64       pred: A mod
+000013c0: 656c 2070 7265 6469 6374 696f 6e20 6469  el prediction di
+000013d0: 6374 696f 6e61 7279 0a20 2020 2020 2020  ctionary.       
+000013e0: 2069 6e70 7574 5f73 697a 653a 2073 6861   input_size: sha
+000013f0: 7065 206f 6620 7468 6520 696e 7075 7420  pe of the input 
+00001400: 696d 6167 652e 2054 7570 6c65 206f 6620  image. Tuple of 
+00001410: 482c 2057 0a20 2020 2020 2020 2074 6872  H, W.        thr
+00001420: 6573 686f 6c64 3a20 666f 7220 7365 676d  eshold: for segm
+00001430: 656e 7461 7469 6f6e 2e20 4465 6661 756c  entation. Defaul
+00001440: 7420 6973 2030 2e35 2e0a 0a20 2020 2052  t is 0.5...    R
+00001450: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00001460: 7365 676d 656e 7461 7469 6f6e 733a 205b  segmentations: [
+00001470: 6e2c 2068 6569 6768 742c 2077 6964 7468  n, height, width
+00001480: 5d20 6e20 6675 6c6c 302d 7369 7a65 2073  ] n full0-size s
+00001490: 6567 6d65 6e61 7461 7469 6f6e 206d 6173  egmenatation mas
+000014a0: 6b73 2e0a 0a20 2020 204e 2909 722e 0000  ks...    N).r...
+000014b0: 0072 0f00 0000 7210 0000 0072 4900 0000  .r....r....rI...
+000014c0: da05 7a65 726f 73da 0261 74da 0373 6574  ..zeros..at..set
+000014d0: 7212 0000 0072 1300 0000 290b 722b 0000  r....r....).r+..
+000014e0: 0072 3d00 0000 7230 0000 0072 2000 0000  .r=...r0...r ...
+000014f0: 722c 0000 0072 2d00 0000 da09 6e5f 7061  r,...r-.....n_pa
+00001500: 7463 6865 7372 0900 0000 721a 0000 005a  tchesr....r....Z
+00001510: 0970 6167 655f 6e75 6d73 5a05 7365 676d  .page_numsZ.segm
+00001520: 7372 2100 0000 7221 0000 0072 2200 0000  sr!...r!...r"...
+00001530: da18 7061 7463 6865 735f 746f 5f73 6567  ..patches_to_seg
+00001540: 6d65 6e74 6174 696f 6e73 b800 0000 730c  mentations....s.
+00001550: 0000 0000 100e 010c 020a 0110 0124 0272  .............$.r
+00001560: 5a00 0000 2907 722b 0000 0072 3d00 0000  Z...).r+...r=...
+00001570: da04 6d61 736b da0f 7363 6f72 655f 7468  ..mask..score_th
+00001580: 7265 7368 6f6c 6472 3000 0000 da0d 6d69  resholdr0.....mi
+00001590: 6e5f 6365 6c6c 5f61 7265 6172 0a00 0000  n_cell_arear....
+000015a0: 6306 0000 0000 0000 0000 0000 000d 0000  c...............
+000015b0: 0006 0000 0043 0000 0073 1801 0000 7400  .....C...s....t.
+000015c0: a001 7c01 a101 7d06 7c00 6401 1900 7c04  ..|...}.|.d...|.
+000015d0: 6b04 7d07 7c07 6a02 5c03 7d08 7d09 7d0a  k.}.|.j.\.}.}.}.
+000015e0: 7c02 6402 6b08 723a 7400 6a03 7c08 6701  |.d.k.r:t.j.|.g.
+000015f0: 7404 6403 8d02 7d02 7c02 7c00 6404 1900  t.d...}.|.|.d...
+00001600: 6a05 6405 6406 8d01 4d00 7d02 7c03 6407  j.d.d...M.}.|.d.
+00001610: 6b04 726e 6408 7c00 6b07 726e 7c02 7c00  k.rnd.|.k.rn|.|.
+00001620: 6409 1900 7c03 6b05 4d00 7d02 7c02 7400  d...|.k.M.}.|.t.
+00001630: 6a06 7c07 6405 6406 8d02 7c05 6b04 4d00  j.|.d.d...|.k.M.
+00001640: 7d02 7c07 7c04 6b04 a007 7408 a101 7400  }.|.|.k...t...t.
+00001650: a009 640a 7c07 6a02 6407 1900 640a 1700  ..d.|.j.d...d...
+00001660: a102 6402 6402 8502 6402 6402 6603 1900  ..d.d...d.d.f...
+00001670: 1400 7d07 7400 a00a 7c02 6402 6402 8502  ..}.t...|.d.d...
+00001680: 6402 6402 6603 1900 7c07 6407 a103 7d07  d.d.f...|.d...}.
+00001690: 7400 a00a 7c07 6407 6b02 6407 7c07 a00b  t...|.d.k.d.|...
+000016a0: a100 640a 1700 7c07 1800 a103 7d07 7c00  ..d...|.....}.|.
+000016b0: 640b 1900 7d0b 7c00 640c 1900 7d0c 7c06  d...}.|.d...}.|.
+000016c0: 6a0c 7c0b 7c0c 6602 1900 a00b 7c07 a101  j.|.|.f.....|...
+000016d0: 7d06 7c06 5300 290d 61f7 0100 0063 6f6e  }.|.S.).a....con
+000016e0: 7665 7274 2070 6174 6368 206f 7574 7075  vert patch outpu
+000016f0: 7420 746f 2074 6865 2069 6d61 6765 206c  t to the image l
+00001700: 6162 656c 0a0a 2020 2020 4172 6773 3a0a  abel..    Args:.
+00001710: 2020 2020 2020 2020 7072 6564 3a20 4120          pred: A 
+00001720: 6d6f 6465 6c20 7072 6564 6963 7469 6f6e  model prediction
+00001730: 2064 6963 7469 6f6e 6172 790a 2020 2020   dictionary.    
+00001740: 2020 2020 696e 7075 745f 7369 7a65 3a20      input_size: 
+00001750: 7368 6170 6520 6f66 2074 6865 2069 6e70  shape of the inp
+00001760: 7574 2069 6d61 6765 2e20 5475 706c 6520  ut image. Tuple 
+00001770: 6f66 2048 2c20 570a 2020 2020 2020 2020  of H, W.        
+00001780: 6d61 736b 3a20 626f 6f6c 6561 6e20 696e  mask: boolean in
+00001790: 6469 6361 746f 7273 206d 6173 6b69 6e67  dicators masking
+000017a0: 206f 7574 2075 6e77 616e 7465 6420 696e   out unwanted in
+000017b0: 7374 616e 6365 732e 2044 6566 6175 6c74  stances. Default
+000017c0: 2069 7320 4e6f 6e65 2028 616c 6c20 6365   is None (all ce
+000017d0: 6c6c 7329 0a20 2020 2020 2020 2073 636f  lls).        sco
+000017e0: 7265 5f74 6872 6573 686f 6c64 3a20 6f74  re_threshold: ot
+000017f0: 696f 6e61 6c2c 206d 696e 5f73 636f 7265  ional, min_score
+00001800: 2074 6f20 6265 2069 6e63 6c75 6465 642e   to be included.
+00001810: 2044 6566 6175 6c74 2069 7320 2e35 2e0a   Default is .5..
+00001820: 2020 2020 2020 2020 7468 7265 7368 6f6c          threshol
+00001830: 643a 2073 6567 6d65 6e74 6174 696f 6e20  d: segmentation 
+00001840: 7468 7265 7368 6f6c 642e 2020 4465 6661  threshold.  Defa
+00001850: 756c 7420 2e35 0a20 2020 2020 2020 206d  ult .5.        m
+00001860: 696e 5f63 656c 6c5f 6172 6561 3a20 6f70  in_cell_area: op
+00001870: 7469 6f6e 616c 206d 696e 696d 616c 2063  tional minimal c
+00001880: 656c 6c20 6172 6561 2074 6f20 6265 2070  ell area to be p
+00001890: 6c6f 7474 6564 2c20 6465 6661 756c 7420  lotted, default 
+000018a0: 302e 0a0a 2020 2020 5265 7475 726e 733a  0...    Returns:
+000018b0: 0a20 2020 2020 2020 206c 6162 656c 3a20  .        label: 
+000018c0: 5b68 6569 6768 742c 2077 6964 7468 5d0a  [height, width].
+000018d0: 2020 2020 7224 0000 004e a901 da05 6474      r$...N....dt
+000018e0: 7970 65da 0d69 6e73 7461 6e63 655f 6d61  ype..instance_ma
+000018f0: 736b a902 7204 0000 0072 0b00 0000 720d  sk..r....r....r.
+00001900: 0000 0072 0100 0000 da12 7472 6169 6e69  ...r......traini
+00001910: 6e67 5f6c 6f63 6174 696f 6e73 5a0b 7072  ng_locationsZ.pr
+00001920: 6564 5f73 636f 7265 7372 0400 0000 7225  ed_scoresr....r%
+00001930: 0000 0072 2600 0000 290d 7210 0000 0072  ...r&...).r....r
+00001940: 5600 0000 720f 0000 00da 046f 6e65 73da  V...r......ones.
+00001950: 0462 6f6f 6c72 2a00 0000 7247 0000 0072  .boolr*...rG...r
+00001960: 1200 0000 7213 0000 0072 4900 0000 7234  ....r....rI...r4
+00001970: 0000 0072 4800 0000 7257 0000 0029 0d72  ...rH...rW...).r
+00001980: 2b00 0000 723d 0000 0072 5b00 0000 725c  +...r=...r[...r\
+00001990: 0000 0072 3000 0000 725d 0000 00da 056c  ...r0...r].....l
+000019a0: 6162 656c da02 7072 7259 0000 0072 0900  abel..prrY...r..
+000019b0: 0000 721a 0000 0072 2c00 0000 722d 0000  ..r....r,...r-..
+000019c0: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
+000019d0: da10 7061 7463 6865 735f 746f 5f6c 6162  ..patches_to_lab
+000019e0: 656c d200 0000 7320 0000 0000 150a 010c  el....s ........
+000019f0: 010c 0208 0110 0114 0110 0110 0116 0232  ...............2
+00001a00: 011c 011e 0208 0108 0214 0272 6700 0000  ...........rg...
+00001a10: 6302 0000 0000 0000 0000 0000 0013 0000  c...............
+00001a20: 0008 0000 0043 0000 0073 a401 0000 7400  .....C...s....t.
+00001a30: 7c00 8301 7d02 7401 7c02 7c02 8302 7d03  |...}.t.|.|...}.
+00001a40: 7402 a003 7c03 6401 a102 7d03 7402 a004  t...|.d...}.t...
+00001a50: 7c03 6402 6b04 a101 5c02 7d04 7d05 7c00  |.d.k...\.}.}.|.
+00001a60: 6403 1900 6a05 6404 1900 7d06 7402 a006  d...j.d...}.t...
+00001a70: 7c00 6403 1900 a101 7c01 6b05 7d07 7c07  |.d.....|.k.}.|.
+00001a80: 7c04 1900 7d08 7c07 7c05 1900 7d09 7402  |...}.|.|...}.t.
+00001a90: 6a07 7408 7c04 8301 7c06 6405 1400 7c06  j.t.|...|.d...|.
+00001aa0: 6405 1400 6703 7409 6406 8d02 7d0a 7402  d...g.t.d...}.t.
+00001ab0: a006 7c00 6407 1900 a101 7c04 6402 6402  ..|.d.....|.d.d.
+00001ac0: 6603 1900 7402 a006 7c00 6407 1900 a101  f...t...|.d.....
+00001ad0: 7c05 6402 6402 6603 1900 1800 7c06 1700  |.d.d.f.....|...
+00001ae0: 7d0b 7402 a006 7c00 6408 1900 a101 7c04  }.t...|.d.....|.
+00001af0: 6402 6402 6603 1900 7402 a006 7c00 6408  d.d.f...t...|.d.
+00001b00: 1900 a101 7c05 6402 6402 6603 1900 1800  ....|.d.d.f.....
+00001b10: 7c06 1700 7d0c 740a 7408 7c04 8301 8301  |...}.t.t.|.....
+00001b20: 4400 5d36 7d0d 7c08 7c0d 1900 7c0a 7c0d  D.]6}.|.|...|.|.
+00001b30: 7c0b 7c0d 1900 7c0b 7c0d 1900 7c06 1700  |.|...|.|...|...
+00001b40: 8502 7c0c 7c0d 1900 7c0c 7c0d 1900 7c06  ..|.|...|.|...|.
+00001b50: 1700 8502 6603 3c00 71f4 7c0a 6409 6409  ....f.<.q.|.d.d.
+00001b60: 8502 7c06 7c06 640a 1400 8502 7c06 7c06  ..|.|.d.....|.|.
+00001b70: 640a 1400 8502 6603 1900 7d0a 7402 6a0b  d.....f...}.t.j.
+00001b80: 7c0a 7c09 4000 640b 640c 8d02 7d0e 7402  |.|.@.d.d...}.t.
+00001b90: 6a0b 7c08 640b 640c 8d02 7d0f 7402 6a0b  j.|.d.d...}.t.j.
+00001ba0: 7c09 640b 640c 8d02 7d10 7c0e 7c10 7c0f  |.d.d...}.|.|.|.
+00001bb0: 1700 7c0e 1800 640d 1700 1b00 7d11 7c03  ..|...d.....}.|.
+00001bc0: 7d12 7c11 7c12 7c04 7c05 6602 3c00 7c12  }.|.|.|.|.f.<.|.
+00001bd0: 5300 290e 7aff 436f 6d70 7574 6520 494f  S.).z.Compute IO
+00001be0: 5573 2061 6d6f 6e67 2069 6e73 7461 6e63  Us among instanc
+00001bf0: 6573 2066 726f 6d20 7468 6520 7361 6d65  es from the same
+00001c00: 2069 6d61 6765 2e20 4d6f 7374 206c 696b   image. Most lik
+00001c10: 656c 7920 7573 6564 2066 6f72 206e 6d73  ely used for nms
+00001c20: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00001c30: 2020 2020 2070 7265 643a 2041 206d 6f64       pred: A mod
+00001c40: 656c 2070 7265 6469 6374 696f 6e20 6469  el prediction di
+00001c50: 6374 696f 6e61 7279 0a20 2020 2020 2020  ctionary.       
+00001c60: 2074 6872 6573 686f 6c64 3a20 5365 676d   threshold: Segm
+00001c70: 656e 7461 7469 6f6e 2074 6872 6573 686f  entation thresho
+00001c80: 6c64 2e20 4465 6661 756c 7420 6973 2030  ld. Default is 0
+00001c90: 2e35 2e0a 0a20 2020 2052 6574 7572 6e73  .5...    Returns
+00001ca0: 3a0a 2020 2020 2020 2020 696f 7573 3a20  :.        ious: 
+00001cb0: 494f 5573 2061 7320 616e 2075 7070 6572  IOUs as an upper
+00001cc0: 2074 7269 6167 6c65 206d 6174 7269 782e   triagle matrix.
+00001cd0: 0a20 2020 2072 0400 0000 7201 0000 0072  .    r....r....r
+00001ce0: 2400 0000 720c 0000 00e9 0300 0000 725e  $...r.........r^
+00001cf0: 0000 0072 2500 0000 7226 0000 004e 720b  ...r%...r&...Nr.
+00001d00: 0000 0072 6100 0000 720d 0000 0072 4600  ...ra...r....rF.
+00001d10: 0000 290c 723c 0000 0072 0500 0000 da02  ..).r<...r......
+00001d20: 6e70 da04 7472 6975 7234 0000 0072 0f00  np..triur4...r..
+00001d30: 0000 da07 6173 6172 7261 7972 5600 0000  ....asarrayrV...
+00001d40: da03 6c65 6e72 6400 0000 724a 0000 0072  ..lenrd...rJ...r
+00001d50: 4700 0000 2913 722b 0000 0072 3000 0000  G...).r+...r0...
+00001d60: 723b 0000 005a 0862 6f78 5f69 6f75 73da  r;...Z.box_ious.
+00001d70: 0263 79da 0263 78da 0870 6164 5f73 697a  .cy..cx..pad_siz
+00001d80: 6572 2000 0000 5a09 7061 7463 6865 735f  er ...Z.patches_
+00001d90: 795a 0970 6174 6368 6573 5f78 5a06 706c  yZ.patches_xZ.pl
+00001da0: 745f 746f da02 6479 da02 6478 7252 0000  t_to..dy..dxrR..
+00001db0: 00da 0675 6e69 6f6e 735a 0761 7265 6173  ...unionsZ.areas
+00001dc0: 5f79 5a07 6172 6561 735f 7872 5100 0000  _yZ.areas_xrQ...
+00001dd0: 5a09 6d61 736b 5f69 6f75 7372 2100 0000  Z.mask_iousr!...
+00001de0: 7221 0000 0072 2200 0000 da1f 696f 7573  r!...r".....ious
+00001df0: 5f6f 665f 7061 7463 6865 735f 6672 6f6d  _of_patches_from
+00001e00: 5f73 616d 655f 696d 6167 65fe 0000 0073  _same_image....s
+00001e10: 3e00 0000 000b 0801 0a01 0c04 1201 0e02  >...............
+00001e20: 1201 0801 0801 2002 1601 16ff 0202 02fe  ...... .........
+00001e30: 02ff 0206 1601 16ff 0202 02fe 02ff 0206  ................
+00001e40: 1001 3401 2201 1202 0e01 0e02 1402 0401  ..4."...........
+00001e50: 0c02 7273 0000 00e7 3333 3333 3333 e33f  ..rs....333333.?
+00001e60: 2903 722b 0000 00da 0d69 6f75 5f74 6872  ).r+.....iou_thr
+00001e70: 6573 686f 6c64 720a 0000 0063 0200 0000  esholdr....c....
+00001e80: 0000 0000 0000 0000 0700 0000 0400 0000  ................
+00001e90: 4300 0000 737c 0000 0074 007c 0083 017d  C...s|...t.|...}
+00001ea0: 027c 027c 016b 047d 0364 017d 0474 01a0  .|.|.k.}.d.}.t..
+00001eb0: 027c 03a1 017c 046b 0372 6e74 03a0 027c  .|...|.k.rnt...|
+00001ec0: 03a1 017d 047c 036a 0464 0164 028d 010f  ...}.|.j.d.d....
+00001ed0: 007d 057c 037c 0564 0364 0385 0264 0366  .}.|.|.d.d...d.f
+00001ee0: 0219 0040 006a 0464 0164 028d 017d 067c  ...@.j.d.d...}.|
+00001ef0: 037c 0664 0364 0385 0264 0366 0219 000f  .|.d.d...d.f....
+00001f00: 0040 007d 0371 147c 036a 0464 0164 028d  .@.}.q.|.j.d.d..
+00001f10: 010f 0053 0029 047a d550 6572 666f 726d  ...S.).z.Perform
+00001f20: 206e 6d73 206f 6e20 7468 6520 6d6f 6465   nms on the mode
+00001f30: 6c20 7072 6564 6963 7469 6f6e 2062 6173  l prediction bas
+00001f40: 6564 206f 6e20 6d61 736b 2049 4f55 0a0a  ed on mask IOU..
+00001f50: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00001f60: 2020 7072 6564 3a20 4120 6d6f 6465 6c20    pred: A model 
+00001f70: 7072 6564 6963 7469 6f6e 2064 6963 7469  prediction dicti
+00001f80: 6f6e 6172 790a 2020 2020 2020 2020 696f  onary.        io
+00001f90: 7573 5f74 6872 6573 686f 6c64 3a20 6465  us_threshold: de
+00001fa0: 6661 756c 7420 302e 360a 0a20 2020 2052  fault 0.6..    R
+00001fb0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00001fc0: 6d61 736b 3a20 626f 6f6c 6561 6e20 6d61  mask: boolean ma
+00001fd0: 736b 206f 6620 6365 6c6c 7320 6e6f 7420  sk of cells not 
+00001fe0: 7375 7072 6573 7365 640a 2020 2020 7201  supressed.    r.
+00001ff0: 0000 0072 0d00 0000 4e29 0572 7300 0000  ...r....N).rs...
+00002000: 7269 0000 0072 4700 0000 7210 0000 0072  ri...rG...r....r
+00002010: 3200 0000 2907 722b 0000 0072 7500 0000  2...).r+...ru...
+00002020: 7251 0000 0072 5b00 0000 da03 636e 74da  rQ...r[.....cnt.
+00002030: 1363 616e 5f73 7570 7072 6573 735f 6f74  .can_suppress_ot
+00002040: 6865 7273 da0a 7375 7070 7265 7373 6564  hers..suppressed
+00002050: 7221 0000 0072 2100 0000 7222 0000 00da  r!...r!...r"....
+00002060: 1c6e 6f6e 5f6d 6178 5f73 7570 7072 6573  .non_max_suppres
+00002070: 735f 7072 6564 6963 7469 6f6e 7331 0100  s_predictions1..
+00002080: 0073 1200 0000 000b 0801 0802 0401 0e01  .s..............
+00002090: 0a01 0e01 1c01 1802 7279 0000 0054 2901  ........ry...T).
+000020a0: da0d 6564 6765 5f69 6e64 6578 696e 6729  ..edge_indexing)
+000020b0: 0372 2b00 0000 da05 7363 616c 6572 0a00  .r+.....scaler..
+000020c0: 0000 6302 0000 0000 0000 0000 0000 000b  ..c.............
+000020d0: 0000 0006 0000 0043 0000 0073 3201 0000  .......C...s2...
+000020e0: 7c00 6401 1900 6402 6402 8502 6403 6403  |.d...d.d...d.d.
+000020f0: 6603 1900 6404 1700 7c01 1400 7d02 7c00  f...d...|...}.|.
+00002100: 6405 1900 6402 6402 8502 6403 6403 6603  d...d.d...d.d.f.
+00002110: 1900 6404 1700 7c01 1400 7d03 7c00 6406  ..d...|...}.|.d.
+00002120: 1900 7d04 7400 7c04 6a01 6407 1900 7c01  ..}.t.|.j.d...|.
+00002130: 1400 8301 7d05 7402 6a03 6402 7c05 8502  ....}.t.j.d.|...
+00002140: 6402 7c05 8502 6602 1900 5c02 7d06 7d07  d.|...f...\.}.}.
+00002150: 7402 a004 7c02 6402 6402 8502 6402 6402  t...|.d.d...d.d.
+00002160: 6603 1900 a101 a005 7406 a101 7c06 1700  f.......t...|...
+00002170: 7d06 7402 a004 7c03 6402 6402 8502 6402  }.t...|.d.d...d.
+00002180: 6402 6603 1900 a101 a005 7406 a101 7c07  d.f.......t...|.
+00002190: 1700 7d07 7c06 6404 1700 7c01 1b00 7d08  ..}.|.d...|...}.
+000021a0: 7c08 7c00 6401 1900 6402 6402 8502 6402  |.|.d...d.d...d.
+000021b0: 6408 8502 6402 6408 8502 6603 1900 3800  d...d.d...f...8.
+000021c0: 7d08 7c07 6404 1700 7c01 1b00 7d09 7c09  }.|.d...|...}.|.
+000021d0: 7c00 6405 1900 6402 6402 8502 6402 6408  |.d...d.d...d.d.
+000021e0: 8502 6402 6408 8502 6603 1900 3800 7d09  ..d.d...f...8.}.
+000021f0: 7407 7c04 7402 6a08 7c08 7c09 6702 6407  t.|.t.j.|.|.g.d.
+00002200: 6409 8d02 8302 7d0a 7c0a 7c06 7c07 6603  d.....}.|.|.|.f.
+00002210: 5300 290a 6199 0200 0052 6573 6361 6c65  S.).a....Rescale
+00002220: 2f72 6573 697a 6520 696e 7374 616e 6365  /resize instance
+00002230: 206f 7574 7075 7473 2069 6e20 6120 7375   outputs in a su
+00002240: 622d 7069 7865 6c20 6163 6375 7261 7465  b-pixel accurate
+00002250: 2077 6179 2e0a 2020 2020 4966 2074 6865   way..    If the
+00002260: 2069 6e70 7574 2069 6d61 6765 2077 6173   input image was
+00002270: 2072 6573 6361 6c65 642c 2074 6869 7320   rescaled, this 
+00002280: 6675 6e63 7469 6f6e 2074 616b 6520 6361  function take ca
+00002290: 7265 206f 6620 7265 7363 616c 696e 6720  re of rescaling 
+000022a0: 7468 6520 7072 6564 6963 7469 6f6e 730a  the predictions.
+000022b0: 2020 2020 746f 2074 6865 206f 7267 696e      to the orgin
+000022c0: 616c 2063 6f6f 6469 6e61 7465 732e 0a0a  al coodinates...
+000022d0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+000022e0: 2020 7072 6564 3a20 4120 6d6f 6465 6c20    pred: A model 
+000022f0: 7072 6564 6963 7469 6f6e 2064 6963 7469  prediction dicti
+00002300: 6f6e 6172 790a 2020 2020 2020 2020 7363  onary.        sc
+00002310: 616c 653a 2054 6865 2073 6361 6c69 6e67  ale: The scaling
+00002320: 2076 616c 7565 2e20 5468 6520 6675 6e63   value. The func
+00002330: 7469 6f6e 2064 6f65 7320 6e6f 7420 7461  tion does not ta
+00002340: 6b65 2061 206e 6f6f 7020 7368 6f72 7463  ke a noop shortc
+00002350: 7574 2065 7665 6e20 6966 2073 6361 6c65  ut even if scale
+00002360: 2069 7320 312e 0a0a 2020 2020 5265 7475   is 1...    Retu
+00002370: 726e 733a 2041 2074 7570 6c65 206f 6620  rns: A tuple of 
+00002380: 7468 7265 6520 6172 7261 7973 0a20 2020  three arrays.   
+00002390: 2020 2020 2070 6174 6368 6573 3a20 6120       patches: a 
+000023a0: 3344 2061 7272 6179 206f 6620 7468 6520  3D array of the 
+000023b0: 7265 7363 616c 6564 2073 6567 6d65 6e74  rescaled segment
+000023c0: 6174 696f 6e20 7061 7463 6865 732e 2054  ation patches. T
+000023d0: 6865 2061 7272 6179 2073 6861 7065 2073  he array shape s
+000023e0: 686f 756c 6420 6265 2064 6966 6665 7265  hould be differe
+000023f0: 6e74 2066 726f 6d0a 2020 2020 2020 2020  nt from.        
+00002400: 2020 2020 7468 6520 6f72 6967 6e61 6c20      the orignal 
+00002410: 7061 7463 6865 7320 696e 206d 6f64 656c  patches in model
+00002420: 2070 7265 6469 7469 6f6e 2e0a 2020 2020   predition..    
+00002430: 2020 2020 7979 3a20 5468 6520 792d 636f      yy: The y-co
+00002440: 6f72 6469 6e61 7465 7320 6f66 2074 6865  ordinates of the
+00002450: 2070 6174 6368 6573 2069 6e20 6d65 7368   patches in mesh
+00002460: 2d67 7269 6420 666f 726d 6174 0a20 2020  -grid format.   
+00002470: 2020 2020 2078 783a 2054 6865 2078 2d63       xx: The x-c
+00002480: 6f6f 7264 696e 6174 6573 206f 6620 7468  oordinates of th
+00002490: 6520 7061 7463 6865 7320 696e 206d 6573  e patches in mes
+000024a0: 682d 6772 6964 2066 6f72 6d61 740a 2020  h-grid format.  
+000024b0: 2020 7225 0000 004e 7201 0000 0072 2f00    r%...Nr....r/.
+000024c0: 0000 7226 0000 0072 2400 0000 720c 0000  ..r&...r$...r...
+000024d0: 0072 0400 0000 720d 0000 0029 09da 0572  .r....r....)...r
+000024e0: 6f75 6e64 720f 0000 0072 1000 0000 7215  oundr....r....r.
+000024f0: 0000 00da 0566 6c6f 6f72 7212 0000 0072  .....floorr....r
+00002500: 1300 0000 da0c 5f73 616d 706c 696e 675f  ......_sampling_
+00002510: 6f70 7216 0000 0029 0b72 2b00 0000 727b  opr....).r+...r{
+00002520: 0000 005a 066e 6577 5f79 305a 066e 6577  ...Z.new_y0Z.new
+00002530: 5f78 30da 0570 6174 6368 da02 7073 721b  _x0..patch..psr.
+00002540: 0000 0072 1c00 0000 5a06 7265 6c5f 7979  ...r....Z.rel_yy
+00002550: 5a06 7265 6c5f 7878 5a09 6e65 775f 7061  Z.rel_xxZ.new_pa
+00002560: 7463 6872 2100 0000 7221 0000 0072 2200  tchr!...r!...r".
+00002570: 0000 da0f 7265 7363 616c 655f 7061 7463  ....rescale_patc
+00002580: 6865 734c 0100 0073 2400 0000 0012 1e01  hesL...s$.......
+00002590: 1e01 0801 1202 1a02 20ff 0204 20ff 0205  ........ ... ...
+000025a0: 0c01 2201 0c01 2202 0201 0201 10fe 0405  .."...".........
+000025b0: 7281 0000 0029 0172 2f00 0000 2902 4e72  r....).r/...).Nr
+000025c0: 2f00 0000 2902 7241 0000 0072 2f00 0000  /...).rA...r/...
+000025d0: 2901 722f 0000 0029 044e 722f 0000 0072  ).r/...).Nr/...r
+000025e0: 2f00 0000 7201 0000 0029 0172 2f00 0000  /...r....).r/...
+000025f0: 2901 7274 0000 0029 24da 075f 5f64 6f63  ).rt...)$..__doc
+00002600: 5f5f da09 6675 6e63 746f 6f6c 7372 0200  __..functoolsr..
+00002610: 0000 da03 6a61 78da 096a 6178 2e6e 756d  ....jax..jax.num
+00002620: 7079 da05 6e75 6d70 7972 1000 0000 7269  py..numpyr....ri
+00002630: 0000 00da 0b6c 6163 7373 2e74 7970 6573  .....lacss.types
+00002640: da05 626f 7865 7372 0500 0000 da05 696d  ..boxesr......im
+00002650: 6167 6572 0600 0000 da09 4172 7261 794c  ager......ArrayL
+00002660: 696b 6572 1300 0000 da05 5475 706c 65da  iker......Tuple.
+00002670: 0541 7272 6179 7223 0000 0072 2e00 0000  .Arrayr#...r....
+00002680: da05 556e 696f 6eda 0853 6571 7565 6e63  ..Union..Sequenc
+00002690: 65da 0844 6174 6144 6963 74da 0566 6c6f  e..DataDict..flo
+000026a0: 6174 da07 6e64 6172 7261 7972 3c00 0000  at..ndarrayr<...
+000026b0: 7240 0000 0072 5500 0000 da05 5368 6170  r@...rU.....Shap
+000026c0: 6572 5a00 0000 da08 4f70 7469 6f6e 616c  erZ.....Optional
+000026d0: 7267 0000 0072 7300 0000 7279 0000 00da  rg...rs...ry....
+000026e0: 0476 6d61 7072 7e00 0000 7281 0000 0072  .vmapr~...r....r
+000026f0: 2100 0000 7221 0000 0072 2100 0000 7222  !...r!...r!...r"
+00002700: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00002710: 0073 7e00 0000 0405 0c02 0801 0c01 0802  .s~.............
+00002720: 0802 0c01 0c04 0200 0200 0201 0efe 0c29  ...............)
+00002730: 080f 00ff 0201 0a00 0201 04fe 0c26 0001  .............&..
+00002740: 00fd 0201 0a01 0a01 0201 02fc 0c21 0000  .............!..
+00002750: 00ff 0201 0200 0200 0200 0201 02fe 0c2c  ...............,
+00002760: 00ff 0201 0200 0200 0201 02fe 0c1d 0001  ................
+00002770: 0001 0001 00fa 0201 0201 0201 0601 0201  ................
+00002780: 0201 0201 02f9 0c2c 1433 1418 1204 0201  .......,.3......
+00002790: 0201 0cfd                                ....
```

### Comparing `lacss-0.4.1/lacss/ops/__pycache__/uda.cpython-38.pyc` & `lacss-0.4.2/lacss/ops/__pycache__/uda.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 225 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 e100 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 929d a964 e201 0000  U..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6500 6a01 6402 6403 8400  d.l.Z.e.j.d.d...
 00000040: 8301 5a02 6404 6405 8400 5a03 6406 6407  ..Z.d.d...Z.d.d.
 00000050: 8400 5a04 6502 a005 6503 6504 a102 0100  ..Z.e...e.e.....
 00000060: 6401 5300 2908 e900 0000 004e 6301 0000  d.S.)......Nc...
 00000070: 0000 0000 0000 0000 0001 0000 0001 0000  ................
@@ -35,8 +35,9 @@
 00000220: 0000 7203 0000 0072 0600 0000 da07 5f67  ..r....r......_g
 00000230: 725f 6277 640d 0000 0073 0200 0000 0001  r_bwd....s......
 00000240: 7211 0000 0029 0672 0c00 0000 da0a 6375  r....).r......cu
 00000250: 7374 6f6d 5f76 6a70 7207 0000 0072 0800  stom_vjpr....r..
 00000260: 0000 7211 0000 00da 0664 6566 766a 7072  ..r......defvjpr
 00000270: 0300 0000 7203 0000 0072 0300 0000 7206  ....r....r....r.
 00000280: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000290: 0073 0a00 0000 0803 0401 0a04 0804 0804  .s..............
+00000290: 0073 0c00 0000 0803 0401 0a04 0804 0804  .s..............
+000002a0: 0c01                                     ..
```

### Comparing `lacss-0.4.1/lacss/ops/boxes.py` & `lacss-0.4.2/lacss/ops/boxes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """ Ops on bounding-boxes
 
 All functions here are degisned to work as either a numpy op or a jax op depending on
 the data type of the input.
 """
+from __future__ import annotations
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
+from lacss.types import *
 
-def box_area(box):
+
+def box_area(box: ArrayLike) -> ArrayLike:
     """Computes area of boxes.
     Args:
       box: a float Tensor with [..., N, 4].
 
     Returns:
       a float Tensor with [..., N]
     """
@@ -22,15 +25,15 @@
     else:
         split = np.split
 
     y_min, x_min, y_max, x_max = split(box, 4, axis=-1)
     return ((y_max - y_min) * (x_max - x_min)).squeeze(axis=-1)
 
 
-def box_intersection(gt_boxes, boxes):
+def box_intersection(gt_boxes: ArrayLike, boxes: ArrayLike) -> ArrayLike:
     """Compute pairwise intersection areas between boxes.
 
     Args:
       gt_boxes: [..., N, 4]
       boxes: [..., M, 4]
 
     Returns:
@@ -58,15 +61,15 @@
     intersect_widths = x_min_max - x_max_min
     intersect_heights = maximum(0, intersect_heights)
     intersect_widths = maximum(0, intersect_widths)
 
     return intersect_heights * intersect_widths
 
 
-def box_iou_similarity(gt_boxes, boxes):
+def box_iou_similarity(gt_boxes: ArrayLike, boxes: ArrayLike) -> ArrayLike:
     """Computes pairwise intersection-over-union between box collections.
 
     Args:
       gt_boxes: a float Tensor with [..., N, 4].
       boxes: a float Tensor with [..., M, 4].
 
     Returns:
```

### Comparing `lacss-0.4.1/lacss/ops/image.py` & `lacss-0.4.2/lacss/ops/image.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,32 @@
+from __future__ import annotations
+
 from functools import partial
 
 import jax
 from jax.scipy.signal import convolve
 
 jnp = jax.numpy
 
+from lacss.types import *
+
 
-def sorbel_edges(image):
+def sorbel_edges(image: ArrayLike) -> Array:
     """Returns a tensor holding Sobel edge maps.
-    >>> image = random.uniform(key, shape=[3, 28, 28])
-    >>> sobel = sobel_edges(image)
-    >>> sobel_y = sobel[0, :, :, :] # sobel in y-direction
-    >>> sobel_x = sobel[1, :, :, :] # sobel in x-direction
-    ```
+
+    Examples:
+
+        >>> image = random.uniform(key, shape=[3, 28, 28])
+        >>> sobel = sobel_edges(image)
+        >>> sobel_y = sobel[0, :, :, :] # sobel in y-direction
+        >>> sobel_x = sobel[1, :, :, :] # sobel in x-direction
+
     Args:
         image: [n, h, w]
+
     Returns:
         Tensor holding edge maps for each channel. [2, n, h, w]
     """
 
     kernels = jnp.array(
         [[[-1, -2, -1], [0, 0, 0], [1, 2, 1]], [[-1, 0, 1], [-2, 0, 2], [-1, 0, 1]]]
     )
@@ -57,21 +65,28 @@
     )
 
     value = (values * weight).sum(axis=-1)
 
     return value
 
 
-def sub_pixel_samples(img, locs, out_of_bound_value=0, edge_indexing=False):
+def sub_pixel_samples(
+    img: ArrayLike,
+    locs: ArrayLike,
+    out_of_bound_value: float = 0,
+    edge_indexing: bool = False,
+) -> Array:
     """Retrieve image values as non-integer locations by interpolation
+
     Args:
         img: Array of shape [D1,D2,..,Dk, ...]
         locs: Array of shape [d1,d2,..,dn, k]
         out_of_bound_value: optional float constant, defualt 0.
         edge_indexing: if True, the index for the first value in img is 0.5, otherwise 0. Default is False
+
     Returns:
         values: [d1,d2,..,dn, ...], float
     """
 
     loc_shape = locs.shape
     img_shape = img.shape
     d_loc = loc_shape[-1]
@@ -87,15 +102,17 @@
     out_shape = loc_shape[:-1] + img_shape[d_loc:]
 
     values = values.reshape(out_shape)
 
     return values
 
 
-def sub_pixel_crop_and_resize(img, bbox, output_shape, out_of_bound_value=0):
+def sub_pixel_crop_and_resize(
+    img: ArrayLike, bbox: ArrayLike, output_shape: Shape, out_of_bound_value: float = 0
+) -> Array:
     """Retrieve image values of a bbox resize output. Used for ROI-Align
     Args:
         img: Array of shape [H, W, ...]
         bbox: [y0, x0, y1, x1]
         output_shape: [h, w]
         out_of_bound_value: optional float constant, defualt 0.
     Returns:
```

### Comparing `lacss-0.4.1/lacss/ops/locations.py` & `lacss-0.4.2/lacss/ops/locations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+from __future__ import annotations
+
 import jax
+import jax.numpy as jnp
 
-jnp = jax.numpy
+from lacss.types import *
 
 
-def locations_to_labels(locations, target_shape, threshold=1.5):
+def locations_to_labels(
+    locations: ArrayLike, target_shape: Shape, threshold: float = 1.5
+) -> Tuple[Array, Array]:
     """Generate labels as LPN regression targets
     Args:
         locations: [N, 2] float32 true location values. scaled 0..1, masking out invalid with -1
         target_shape: (H, W)  int
         threshold: distance threshold for postive label
     Returns:
         score_target: [H, W, 1] int32
@@ -37,15 +42,15 @@
         0
     )  # [2, H, W]
     regression_target = regression_target.transpose(1, 2, 0)  # [H, W, 2]
 
     return score_target, regression_target
 
 
-def distance_similarity(pred_locations, gt_locations):
+def distance_similarity(pred_locations: ArrayLike, gt_locations: ArrayLike) -> Array:
     """Compute distance similarity matrix
     pairwise similarity = 1 / distance ^2
     Args:
       pred_locations: [N, 2] use -1 to mask out invalid locations
       gt_locations: [K, 2] use -1 to mask out invalid locations
     Returns:
       similarity_matrix: [N, k]
@@ -59,15 +64,17 @@
     # negative locations are invalid
     sm = jnp.where((pred_locations < 0).all(axis=-1)[:, None], 0, sm)
     sm = jnp.where((gt_locations < 0).all(axis=-1), 0, sm)
 
     return sm
 
 
-def location_matching(pred_locations, gt_locations, threshold):
+def location_matching(
+    pred_locations: ArrayLike, gt_locations: ArrayLike, threshold: float
+) -> Tuple[Array, Array]:
     """Match predicted location to gt locations
     Args:
       pred_locations:r [N, 2]
       gt_locations: [K, 2]
       threshold: float. Maximum distance to be matched
     Returns:
       matches: [N], indices of the matches location in gt list
```

### Comparing `lacss-0.4.1/lacss/ops/masks.py` & `lacss-0.4.2/lacss/ops/masks.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/ops/nms.py` & `lacss-0.4.2/lacss/ops/nms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from typing import Callable
+from __future__ import annotations
 
 import jax
+import jax.numpy as jnp
+
+from lacss.types import *
 
 from .boxes import box_iou_similarity
 from .locations import distance_similarity
 
-jnp = jax.numpy
-
 NMS_TILE_SIZE = 512
 
 
 def _suppress(boxes, mask):
     return jnp.where(mask[:, None], -1, boxes)
 
 
 def _suppression_loop_body(inputs):
     """Process boxes in the range [idx*NMS_TILE_SIZE, (idx+1)*NMS_TILE_SIZE).
     Args:
         inputs: tuple
             idx: current slice
-            boxes: a tensor with a shape of [N, 4].
+            boxes: a tensor with a shape of [N, 4] or [N, 2].
             num_selected: number of selected boxes so far
             threshold: float
     Returns:
         boxes: updated
         num_selected: updated
     """
 
@@ -73,34 +74,40 @@
     # output_size.
     num_selected += jnp.count_nonzero((box_slice >= 0).any(axis=-1))
 
     return boxes, num_selected
 
 
 def sorted_non_max_suppression(
-    scores,
-    boxes,
+    scores: ArrayLike,
+    boxes: ArrayLike,
     max_output_size: int,
     threshold: float = 0.5,
     min_score: float = 0,
-):
+) -> Tuple[Array, Array]:
     """non-maximum suppression for either bboxes or points.
+
     Assumption:
+
         * The boxes are sorted by scores
+
     The overal design of the algorithm is to handle boxes tile-by-tile:
+
     Args:
         scores: [N]
         boxes: [N, C]  C=4 for boxes, C=2 for locations
         max_output_size: a positive scalar integer
         threshold: a scalar float, can be negative
         min_score: min score to be selected, default 0
+
     Returns:
         nms_scores: [M].  M = max_output_size
         nms_proposals: [M, C].
     """
+
     # preprocessing
     c = boxes.shape[-1]
     if c != 2 and c != 4:
         raise ValueError(f"boxes should be Nx4 or Nx2, got Nx{c}")
     # if similarity_func is None:
     #     similarity_func = box_iou_similarity if c == 4 else distance_similarity
 
@@ -111,35 +118,53 @@
     num_boxes = boxes.shape[0]
     pad = NMS_TILE_SIZE - 1 - (num_boxes - 1) % NMS_TILE_SIZE
     boxes = jnp.pad(boxes, [[0, pad], [0, 0]], constant_values=-1)
     scores = jnp.pad(scores, [[0, pad]], constant_values=-1)
     num_boxes += pad
     boxes = boxes.reshape(-1, NMS_TILE_SIZE, c)
 
+    # process all tiles until generating enough output
     def _trivial_suppress_all(inputs):
         (
             idx,
             boxes,
             num_outputs,
             _,
         ) = inputs
         boxes = boxes.at[idx].set(-1)
         return boxes, num_outputs
 
-    # process all tiles until generating enough output
-    num_selected = 0
-    for idx in range(num_boxes // NMS_TILE_SIZE):
-        boxes, num_selected = jax.lax.cond(
+    def _inner_loop_func(idx, val):
+        boxes, num_selected = val
+        return jax.lax.cond(
             (scores[idx * NMS_TILE_SIZE] >= min_score)
             & (num_selected < max_output_size),
             _suppression_loop_body,
             _trivial_suppress_all,
             (idx, boxes, num_selected, threshold),
         )
 
+    num_selected = 0
+    boxes, num_selected = jax.lax.fori_loop(
+        0,
+        num_boxes // NMS_TILE_SIZE,
+        _inner_loop_func,
+        (boxes, num_selected),
+    )
+
+    # num_selected = 0
+    # for idx in range(num_boxes // NMS_TILE_SIZE):
+    #     boxes, num_selected = jax.lax.cond(
+    #         (scores[idx * NMS_TILE_SIZE] >= min_score)
+    #         & (num_selected < max_output_size),
+    #         _suppression_loop_body,
+    #         _trivial_suppress_all,
+    #         (idx, boxes, num_selected, threshold),
+    #     )
+
     # reshape boxes back
     boxes = boxes.reshape(-1, c)
 
     # remove suppressed boxes
     selected = jnp.argwhere(
         (boxes >= 0).any(axis=-1), size=max_output_size, fill_value=-1
     ).squeeze(-1)
```

### Comparing `lacss-0.4.1/lacss/ops/patches.py` & `lacss-0.4.2/lacss/ops/patches.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """ Various functions deals with segmentation pathces
 
     All functions here takes unbatched input. Use vmap to convert to batched data
 """
+from __future__ import annotations
 
 from functools import partial
-from typing import Dict, Optional, Sequence, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
+from lacss.types import *
+
 from .boxes import box_iou_similarity
 from .image import sub_pixel_samples
 
 
 def gather_patches(
-    features: jnp.ndarray, locations: jnp.ndarray, patch_size: int
-) -> tuple:
+    features: ArrayLike, locations: ArrayLike, patch_size: int
+) -> Tuple[Array, Array, Array, Array]:
     """extract feature patches according to a list of locations
 
     Args:
         features: [H,W,C] standard 2D feature map
         locations: [N, 2] float32, scaled 0..1
         patch_size: int
 
@@ -66,15 +68,15 @@
     if patches.ndim > yc.ndim:
         patches = patches.squeeze(-1)
 
     return patches, yc, xc
 
 
 def bboxes_of_patches(
-    pred: Union[Sequence, Dict], threshold: float = 0.5
+    pred: Union[Sequence, DataDict], threshold: float = 0.5
 ) -> jnp.ndarray:
     """Compute the instance bboxes from model predictions
 
     Args:
         pred: A model prediction dictionary:
         threshold: for segmentation, default 0.5
 
@@ -102,18 +104,18 @@
     bboxes = jnp.stack([min_row, min_col, max_row, max_col], axis=-1)
     bboxes = jnp.where(is_valid, bboxes, -1)
 
     return bboxes
 
 
 def indices_of_patches(
-    pred: Union[Sequence, Dict],
+    pred: Union[Sequence, DataDict],
     input_size: Tuple[int, int] = None,
     threshold: float = 0.5,
-) -> tuple:
+) -> Array:
     """Compute yx coodinates of all segmented instances
 
     Args:
         pred: A model prediction dictionary
         threshold: float
 
     Returns:
@@ -134,16 +136,16 @@
         xx = xx[valid_coords]
         rowids = rowids[valid_coords]
 
     return jnp.stack([yy, xx, rowids], axis=-1)
 
 
 def iou_patches_and_labels(
-    pred: dict, labels: jnp.ndarray, BLOCK_SIZE: int = 128, threshold: float = 0.5
-) -> jnp.ndarray:
+    pred: DataDict, labels: ArrayLike, BLOCK_SIZE: int = 128, threshold: float = 0.5
+) -> Array:
     """Compute iou between prediction and ground truth label.
 
     Args:
         pred: A model prediction dictionary
         labels: image label. bg_label = 0
         threshold: for segmentation. default is 0.5
 
@@ -177,16 +179,16 @@
     ious = jnp.concatenate(ious, axis=0).transpose()  # [N, B * b]
     ious = ious[:, : labels.max()]  # this breaks JIT
 
     return ious
 
 
 def patches_to_segmentations(
-    pred: dict, input_size: Tuple[int, int], threshold: float = 0.5
-) -> jnp.ndarray:
+    pred: DataDict, input_size: Shape, threshold: float = 0.5
+) -> Array:
     """Expand the predicted patches to the full image size.
     The default model segmentation output shows only a small patch around each instance. This
     function expand each patch to the size of the orginal image.
 
     Args:
         pred: A model prediction dictionary
         input_size: shape of the input image. Tuple of H, W
@@ -203,21 +205,21 @@
     segms = jnp.zeros((n_patches,) + input_size)
     segms = segms.at[page_nums[:, None, None], yc, xc].set(patches)
 
     return (segms >= threshold).astype(int)
 
 
 def patches_to_label(
-    pred: dict,
-    input_size: Tuple[int, int],
-    mask: Optional[jnp.ndarray] = None,
+    pred: DataDict,
+    input_size: Shape,
+    mask: Optional[ArrayLike] = None,
     score_threshold: float = 0.5,
     threshold: float = 0.5,
     min_cell_area: int = 0,
-) -> jnp.ndarray:
+) -> Array:
     """convert patch output to the image label
 
     Args:
         pred: A model prediction dictionary
         input_size: shape of the input image. Tuple of H, W
         mask: boolean indicators masking out unwanted instances. Default is None (all cells)
         score_threshold: otional, min_score to be included. Default is .5.
@@ -246,15 +248,15 @@
     xc = pred["instance_xc"]
 
     label = label.at[yc, xc].max(pr)
 
     return label
 
 
-def ious_of_patches_from_same_image(pred: dict, threshold: float = 0.5) -> jnp.ndarray:
+def ious_of_patches_from_same_image(pred: DataDict, threshold: float = 0.5) -> Array:
     """Compute IOUs among instances from the same image. Most likely used for nms.
 
     Args:
         pred: A model prediction dictionary
         threshold: Segmentation threshold. Default is 0.5.
 
     Returns:
@@ -297,15 +299,15 @@
 
     mask_ious = box_ious
     mask_ious[(cy, cx)] = ious
 
     return mask_ious
 
 
-def non_max_suppress_predictions(pred: dict, iou_threshold: float = 0.6) -> jnp.ndarray:
+def non_max_suppress_predictions(pred: DataDict, iou_threshold: float = 0.6) -> Array:
     """Perform nms on the model prediction based on mask IOU
 
     Args:
         pred: A model prediction dictionary
         ious_threshold: default 0.6
 
     Returns:
@@ -325,49 +327,49 @@
     return ~mask.any(axis=0)
 
 
 _sampling_op = jax.vmap(partial(sub_pixel_samples, edge_indexing=True))
 
 
 def rescale_patches(
-    pred: dict, scale: float
-) -> Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray]:
+    pred: DataDict,
+    scale: float,
+) -> Tuple[Array, Array, Array]:
     """Rescale/resize instance outputs in a sub-pixel accurate way.
     If the input image was rescaled, this function take care of rescaling the predictions
     to the orginal coodinates.
 
     Args:
         pred: A model prediction dictionary
         scale: The scaling value. The function does not take a noop shortcut even if scale is 1.
 
     Returns: A tuple of three arrays
         patches: a 3D array of the rescaled segmentation patches. The array shape should be different from
             the orignal patches in model predition.
         yy: The y-coordinates of the patches in mesh-grid format
         xx: The x-coordinates of the patches in mesh-grid format
     """
-
     new_y0 = (pred["instance_yc"][:, 0, 0] + 0.5) * scale  # edge indexing in new scale
     new_x0 = (pred["instance_xc"][:, 0, 0] + 0.5) * scale  # edge indexing in new scale
     patch = pred["instance_output"]
     ps = round(patch.shape[-1] * scale)
 
     yy, xx = jnp.mgrid[:ps, :ps]
     yy = (
         jnp.floor(new_y0[:, None, None]).astype(int) + yy
     )  # center indexing in new scale
     xx = (
         jnp.floor(new_x0[:, None, None]).astype(int) + xx
     )  # center indexing in new scale
 
-    rel_yy = (yy + 0.5) / scale - pred["instance_yc"][
-        :, :1, :1
-    ]  # edge indexing in old scale
-    rel_xx = (xx + 0.5) / scale - pred["instance_xc"][
-        :, :1, :1
-    ]  # edge indexing in old scale
+    # edge indexing in old scale
+    rel_yy = (yy + 0.5) / scale
+    rel_yy -= pred["instance_yc"][:, :1, :1]
+    rel_xx = (xx + 0.5) / scale
+    rel_xx -= pred["instance_xc"][:, :1, :1]
+
     new_patch = _sampling_op(
         patch,
-        np.stack([rel_yy, rel_xx], axis=-1),
+        jnp.stack([rel_yy, rel_xx], axis=-1),
     )
 
     return new_patch, yy, xx
```

### Comparing `lacss-0.4.1/lacss/tracking/predict.py` & `lacss-0.4.2/lacss/tracking/predict.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/tracking/seqnms.py` & `lacss-0.4.2/lacss/tracking/seqnms.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/tracking/smc.py` & `lacss-0.4.2/lacss/tracking/smc.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/tracking/utils.py` & `lacss-0.4.2/lacss/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/train/__pycache__/loss.cpython-38.pyc` & `lacss-0.4.2/lacss/train/__pycache__/loss.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 6834 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 b21a 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 5a80 9c64 b21a 0000  U.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 0401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6401 6c07 6d08 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6401 6c08 5a0a 6400 6404 6c0b  ..d.d.l.Z.d.d.l.
 00000070: 6d0c 5a0c 0100 6405 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `lacss-0.4.1/lacss/train/__pycache__/metric.cpython-38.pyc` & `lacss-0.4.2/lacss/train/__pycache__/metric.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 222 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 de00 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 5a80 9c64 de00 0000  U.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 8302 5a04  ..G.d.d...d...Z.
 00000050: 6401 5300 2905 e900 0000 004e 2901 da0e  d.S.)......N)...
 00000060: 6162 7374 7261 6374 6d65 7468 6f64 6300  abstractmethodc.
 00000070: 0000 0000 0000 0000 0000 0000 0000 0004  ................
```

### Comparing `lacss-0.4.1/lacss/train/__pycache__/strategy.cpython-38.pyc` & `lacss-0.4.2/lacss/train/__pycache__/strategy.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun 27 19:00:57 2023 UTC, .py size: 4018 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 e931 9b64 b20f 0000  U........1.d....
+00000000: 550d 0d0a 0000 0000 be21 ac64 a210 0000  U........!.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c04 5a04 6400 6401 6c05  ..d.d.l.Z.d.d.l.
 00000050: 6d06 5a07 0100 6400 6401 6c08 6d09 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6403 6c0b 6d0c 5a0c 0100 6404  ..d.d.l.m.Z...d.
 00000070: 6405 6c0d 6d0e 5a0e 0100 6406 6407 6c0f  d.l.m.Z...d.d.l.
@@ -24,235 +24,248 @@
 00000170: 6503 6405 6406 8400 8301 5a06 6503 6507  e.d.d.....Z.e.e.
 00000180: 6508 6a09 650a 1900 6508 6a0b 6508 6a0b  e.j.e...e.j.e.j.
 00000190: 6508 6a0c 650d 1900 6508 6a0e 6507 6508  e.j.e...e.j.e.e.
 000001a0: 6a09 650a 1900 6508 6a0b 6603 1900 6407  j.e...e.j.f...d.
 000001b0: 9c06 6408 6409 8404 8301 5a0f 640a 5300  ..d.d.....Z.d.S.
 000001c0: 290b da05 4561 6765 7263 0700 0000 0000  )...Eagerc......
 000001d0: 0000 0000 0000 0b00 0000 0500 0000 0300  ................
-000001e0: 0000 736a 0000 0074 00a0 017c 04a1 017d  ..sj...t...|...}
+000001e0: 0000 7376 0000 0074 00a0 017c 04a1 017d  ..sv...t...|...}
 000001f0: 077c 026a 0264 017c 0169 0166 017c 076a  .|.j.d.|.i.f.|.j
 00000200: 039e 027c 076a 0464 027c 0669 0197 028e  ...|.j.d.|.i....
-00000210: 017d 0874 057c 087c 057c 0464 038d 0389  .}.t.|.|.|.d....
-00000220: 0074 0687 0066 0164 0464 0584 087c 0344  .t...f.d.d...|.D
-00000230: 0083 018e 005c 027d 097d 0374 077c 0983  .....\.}.}.t.|..
-00000240: 017d 0a7c 0a7c 027c 037c 0866 0366 0253  .}.|.|.|.|.f.f.S
-00000250: 0029 064e da06 7061 7261 6d73 da04 726e  .).N..params..rn
-00000260: 6773 2903 da05 7072 6564 73da 066c 6162  gs)...preds..lab
-00000270: 656c 73da 0669 6e70 7574 7363 0100 0000  els..inputsc....
-00000280: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00000290: 1300 0000 7318 0000 0067 007c 005d 107d  ....s....g.|.].}
-000002a0: 017c 016a 0066 0088 008e 0191 0271 0453  .|.j.f.......q.S
-000002b0: 00a9 0029 01da 0675 7064 6174 6529 02da  ...)...update)..
-000002c0: 022e 30da 076c 6f73 735f 666e a901 da04  ..0..loss_fn....
-000002d0: 6172 6773 720f 0000 00fa 372f 686f 6d65  argsr.....7/home
-000002e0: 2f46 4341 4d2f 6a79 752f 7072 6f6a 5f6c  /FCAM/jyu/proj_l
-000002f0: 6163 7373 2f6c 6163 7373 2f6c 6163 7373  acss/lacss/lacss
-00000300: 2f74 7261 696e 2f73 7472 6174 6567 792e  /train/strategy.
-00000310: 7079 da0a 3c6c 6973 7463 6f6d 703e 1e00  py..<listcomp>..
-00000320: 0000 7304 0000 0006 0002 007a 2145 6167  ..s........z!Eag
-00000330: 6572 2e6c 6f73 735f 666e 2e3c 6c6f 6361  er.loss_fn.<loca
-00000340: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2908  ls>.<listcomp>).
-00000350: 7205 0000 00da 0a66 726f 6d5f 7661 6c75  r......from_valu
-00000360: 65da 0861 7070 6c79 5f66 6e72 1400 0000  e..apply_fnr....
-00000370: da06 6b77 6172 6773 da04 6469 6374 da03  ..kwargs..dict..
-00000380: 7a69 70da 0373 756d 290b da03 636c 7372  zip..sum)...clsr
-00000390: 0a00 0000 da05 7374 6174 65da 096c 6f73  ......state..los
-000003a0: 735f 6c6f 6773 720e 0000 0072 0d00 0000  s_logsr....r....
-000003b0: 720b 0000 00da 0a69 6e70 7574 735f 6f62  r......inputs_ob
-000003c0: 6a72 0c00 0000 da06 6c6f 7373 6573 da0a  jr......losses..
-000003d0: 746f 7461 6c5f 6c6f 7373 720f 0000 0072  total_lossr....r
-000003e0: 1300 0000 7215 0000 0072 1200 0000 0e00  ....r....r......
-000003f0: 0000 7324 0000 0000 020a 0104 0106 ff02  ..s$............
-00000400: 0204 fe02 0304 fd02 0402 fc08 0702 0102  ................
-00000410: 0102 0102 fd06 061a 0108 027a 0d45 6167  ...........z.Eag
-00000420: 6572 2e6c 6f73 735f 666e 6304 0000 0000  er.loss_fnc.....
-00000430: 0000 0000 0000 0006 0000 0003 0000 0043  ...............C
-00000440: 0000 0073 2400 0000 7400 a001 7c03 a101  ...s$...t...|...
-00000450: 7d04 7c02 6a02 7c01 6601 7c04 6a03 9e02  }.|.j.|.f.|.j...
-00000460: 7c04 6a04 8e01 7d05 7c05 5300 a901 4e29  |.j...}.|.S...N)
-00000470: 0572 0500 0000 7217 0000 00da 0469 6e69  .r....r......ini
-00000480: 7472 1400 0000 7219 0000 0029 0672 1d00  tr....r....).r..
-00000490: 0000 da03 6b65 79da 056d 6f64 656c 720e  ....key..modelr.
-000004a0: 0000 0072 2000 0000 721e 0000 0072 0f00  ...r ...r....r..
-000004b0: 0000 720f 0000 0072 1500 0000 da07 696e  ..r....r......in
-000004c0: 6974 5f66 6e23 0000 0073 0600 0000 0002  it_fn#...s......
-000004d0: 0a02 1602 7a0d 4561 6765 722e 696e 6974  ....z.Eager.init
-000004e0: 5f66 6e63 0300 0000 0000 0000 0000 0000  _fnc............
-000004f0: 0500 0000 0300 0000 4300 0000 732a 0000  ........C...s*..
-00000500: 0074 00a0 017c 02a1 017d 037c 016a 0264  .t...|...}.|.j.d
-00000510: 017c 016a 0369 0166 017c 036a 049e 027c  .|.j.i.f.|.j...|
-00000520: 036a 058e 017d 047c 0453 0029 024e 720a  .j...}.|.S.).Nr.
-00000530: 0000 0029 0672 0500 0000 7217 0000 0072  ...).r....r....r
-00000540: 1800 0000 720a 0000 0072 1400 0000 7219  ....r....r....r.
-00000550: 0000 0029 0572 1d00 0000 721e 0000 0072  ...).r....r....r
-00000560: 0e00 0000 7220 0000 0072 0c00 0000 720f  ....r ...r....r.
-00000570: 0000 0072 0f00 0000 7215 0000 00da 0770  ...r....r......p
-00000580: 7265 6469 6374 2b00 0000 7312 0000 0000  redict+...s.....
-00000590: 030a 0104 0108 ff02 0104 ff02 0104 ff04  ................
-000005a0: 037a 0d45 6167 6572 2e70 7265 6469 6374  .z.Eager.predict
-000005b0: a906 721e 0000 0072 1f00 0000 720e 0000  ..r....r....r...
-000005c0: 0072 0d00 0000 720b 0000 00da 0672 6574  .r....r......ret
-000005d0: 7572 6e63 0600 0000 0000 0000 0000 0000  urnc............
-000005e0: 0800 0000 0700 0000 4300 0000 7340 0000  ........C...s@..
-000005f0: 0074 006a 017c 006a 0264 0164 028d 027c  .t.j.|.j.d.d...|
-00000600: 016a 037c 017c 027c 037c 047c 0583 065c  .j.|.|.|.|.|...\
-00000610: 027d 065c 037d 017d 027d 077c 016a 047c  .}.\.}.}.}.|.j.|
-00000620: 0664 038d 017d 017c 017c 027c 0766 0353  .d...}.|.|.|.f.S
-00000630: 0029 044e 54a9 01da 0768 6173 5f61 7578  .).NT....has_aux
-00000640: a901 da05 6772 6164 7329 05da 036a 6178  ....grads)...jax
-00000650: da04 6772 6164 7212 0000 0072 0a00 0000  ..gradr....r....
-00000660: da0f 6170 706c 795f 6772 6164 6965 6e74  ..apply_gradient
-00000670: 73a9 0872 1d00 0000 721e 0000 0072 1f00  s..r....r....r..
-00000680: 0000 720e 0000 0072 0d00 0000 720b 0000  ..r....r....r...
-00000690: 0072 2e00 0000 720c 0000 0072 0f00 0000  .r....r....r....
-000006a0: 720f 0000 0072 1500 0000 da0a 7472 6169  r....r......trai
-000006b0: 6e5f 7374 6570 3400 0000 7314 0000 0000  n_step4...s.....
-000006c0: 0b0e 0104 0102 0102 0102 0102 0102 fa0e  ................
-000006d0: 080c 027a 1045 6167 6572 2e74 7261 696e  ...z.Eager.train
-000006e0: 5f73 7465 704e 2910 da08 5f5f 6e61 6d65  _stepN)...__name
-000006f0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000700: 5f5f 7175 616c 6e61 6d65 5f5f da0b 636c  __qualname__..cl
-00000710: 6173 736d 6574 686f 6472 1200 0000 7227  assmethodr....r'
-00000720: 0000 0072 2800 0000 7203 0000 00da 0274  ...r(...r......t
-00000730: 70da 0853 6571 7565 6e63 6572 0800 0000  p..Sequencer....
-00000740: da03 416e 79da 084f 7074 696f 6e61 6c72  ..Any..Optionalr
-00000750: 1a00 0000 da05 5475 706c 6572 3300 0000  ......Tupler3...
-00000760: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
-00000770: 1500 0000 7209 0000 000d 0000 0073 1c00  ....r........s..
-00000780: 0000 0801 0201 0a14 0201 0a07 0201 0a08  ................
-00000790: 0203 0201 0801 0401 0401 0801 16f9 7209  ..............r.
-000007a0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000007b0: 0000 0000 0300 0000 4000 0000 7318 0000  ........@...s...
-000007c0: 0065 005a 0164 005a 0265 03a0 0465 056a  .e.Z.d.Z.e...e.j
-000007d0: 06a1 015a 0664 0153 0029 02da 0443 6f72  ...Z.d.S.)...Cor
-000007e0: 654e 2907 7234 0000 0072 3500 0000 7236  eN).r4...r5...r6
-000007f0: 0000 0072 2f00 0000 da03 6a69 7472 0900  ...r/.....jitr..
-00000800: 0000 7228 0000 0072 0f00 0000 720f 0000  ..r(...r....r...
-00000810: 0072 0f00 0000 7215 0000 0072 3d00 0000  .r....r....r=...
-00000820: 4c00 0000 7302 0000 0008 0172 3d00 0000  L...s......r=...
-00000830: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000840: 0003 0000 0040 0000 0073 1800 0000 6500  .....@...s....e.
-00000850: 5a01 6400 5a02 6503 a004 6505 6a06 a101  Z.d.Z.e...e.j...
-00000860: 5a06 6401 5300 2902 da03 4a49 544e 2907  Z.d.S.)...JITN).
-00000870: 7234 0000 0072 3500 0000 7236 0000 0072  r4...r5...r6...r
-00000880: 2f00 0000 723e 0000 0072 3d00 0000 7233  /...r>...r=...r3
-00000890: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
-000008a0: 0000 7215 0000 0072 3f00 0000 5000 0000  ..r....r?...P...
-000008b0: 7302 0000 0008 0172 3f00 0000 6300 0000  s......r?...c...
-000008c0: 0000 0000 0000 0000 0000 0000 000a 0000  ................
-000008d0: 0040 0000 0073 5800 0000 6500 5a01 6400  .@...sX...e.Z.d.
-000008e0: 5a02 6503 6504 6505 6a06 6507 1900 6505  Z.e.e.e.j.e...e.
-000008f0: 6a08 6505 6a08 6505 6a09 650a 1900 6505  j.e.j.e.j.e...e.
-00000900: 6a0b 6504 6505 6a06 6507 1900 6505 6a08  j.e.e.j.e...e.j.
-00000910: 6603 1900 6401 9c06 6402 6403 8404 8301  f...d...d.d.....
-00000920: 5a0c 6503 6404 6405 8400 8301 5a0d 6406  Z.e.d.d.....Z.d.
-00000930: 5300 2907 da0c 5f44 6973 7472 6962 7574  S.)..._Distribut
-00000940: 6564 7229 0000 0063 0600 0000 0000 0000  edr)...c........
-00000950: 0000 0000 0800 0000 0700 0000 0300 0000  ................
-00000960: 738a 0000 0074 006a 01a0 0264 01a1 0189  s....t.j...d....
-00000970: 0074 006a 03a0 0487 0066 0164 0264 0384  .t.j.....f.d.d..
-00000980: 087c 05a1 027d 0574 006a 057c 006a 0664  .|...}.t.j.|.j.d
-00000990: 0464 058d 027c 016a 077c 017c 027c 037c  .d...|.j.|.|.|.|
-000009a0: 047c 0583 065c 027d 065c 037d 017d 027d  .|...\.}.\.}.}.}
-000009b0: 0774 006a 016a 087c 0664 0164 068d 027d  .t.j.j.|.d.d...}
-000009c0: 067c 016a 097c 0664 078d 017d 0174 00a0  .|.j.|.d...}.t..
-000009d0: 0474 0a74 006a 016a 0864 0164 068d 027c  .t.t.j.j.d.d...|
-000009e0: 02a1 027d 027c 017c 027c 0766 0353 0029  ...}.|.|.|.f.S.)
-000009f0: 084e da06 6d61 7070 6564 6301 0000 0000  .N..mappedc.....
-00000a00: 0000 0000 0000 0001 0000 0004 0000 0013  ................
-00000a10: 0000 0073 0e00 0000 7400 6a01 a002 7c00  ...s....t.j...|.
-00000a20: 8800 a102 5300 7223 0000 0029 0372 2f00  ....S.r#...).r/.
-00000a30: 0000 da06 7261 6e64 6f6d da07 666f 6c64  ....random..fold
-00000a40: 5f69 6e29 0172 2500 0000 a901 da0a 6178  _in).r%.......ax
-00000a50: 6973 5f69 6e64 6578 720f 0000 0072 1500  is_indexr....r..
-00000a60: 0000 da08 3c6c 616d 6264 613e 6100 0000  ....<lambda>a...
-00000a70: f300 0000 007a 2a5f 4469 7374 7269 6275  .....z*_Distribu
-00000a80: 7465 642e 5f74 7261 696e 5f73 7465 702e  ted._train_step.
-00000a90: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-00000aa0: 3e54 722b 0000 0029 01da 0961 7869 735f  >Tr+...)...axis_
-00000ab0: 6e61 6d65 722d 0000 0029 0b72 2f00 0000  namer-...).r/...
-00000ac0: da03 6c61 7872 4500 0000 da09 7472 6565  ..laxrE.....tree
-00000ad0: 5f75 7469 6cda 0874 7265 655f 6d61 7072  _util..tree_mapr
-00000ae0: 3000 0000 7212 0000 0072 0a00 0000 da05  0...r....r......
-00000af0: 706d 6561 6e72 3100 0000 7202 0000 0072  pmeanr1...r....r
-00000b00: 3200 0000 720f 0000 0072 4400 0000 7215  2...r....rD...r.
-00000b10: 0000 00da 0b5f 7472 6169 6e5f 7374 6570  ....._train_step
-00000b20: 5500 0000 7322 0000 0000 0a0c 0106 010a  U...s"..........
-00000b30: 0002 ff04 040e 0104 0102 0102 0102 0102  ................
-00000b40: 0102 fa0e 0910 010c 0318 057a 185f 4469  ...........z._Di
-00000b50: 7374 7269 6275 7465 642e 5f74 7261 696e  stributed._train
-00000b60: 5f73 7465 7063 0400 0000 0000 0000 0000  _stepc..........
-00000b70: 0000 0400 0000 0500 0000 4300 0000 731e  ..........C...s.
-00000b80: 0000 0074 00a0 0164 0164 0284 007c 03a1  ...t...d.d...|..
-00000b90: 027d 0374 02a0 037c 017c 027c 03a1 0353  .}.t...|.|.|...S
-00000ba0: 0029 034e 6301 0000 0000 0000 0000 0000  .).Nc...........
-00000bb0: 0001 0000 0002 0000 0053 0000 0073 0800  .........S...s..
-00000bc0: 0000 7c00 6401 1900 5300 a902 4e72 0100  ..|.d...S...Nr..
-00000bd0: 0000 720f 0000 0029 01da 0176 720f 0000  ..r....)...vr...
-00000be0: 0072 0f00 0000 7215 0000 0072 4600 0000  .r....r....rF...
-00000bf0: 7a00 0000 7247 0000 007a 265f 4469 7374  z...rG...z&_Dist
-00000c00: 7269 6275 7465 642e 696e 6974 5f66 6e2e  ributed.init_fn.
-00000c10: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-00000c20: 3e29 0472 2f00 0000 724b 0000 0072 0900  >).r/...rK...r..
-00000c30: 0000 7227 0000 0029 0472 1d00 0000 7225  ..r'...).r....r%
-00000c40: 0000 0072 2600 0000 720e 0000 0072 0f00  ...r&...r....r..
-00000c50: 0000 720f 0000 0072 1500 0000 7227 0000  ..r....r....r'..
-00000c60: 0078 0000 0073 0400 0000 0002 1001 7a14  .x...s........z.
-00000c70: 5f44 6973 7472 6962 7574 6564 2e69 6e69  _Distributed.ini
-00000c80: 745f 666e 4e29 0e72 3400 0000 7235 0000  t_fnN).r4...r5..
-00000c90: 0072 3600 0000 7237 0000 0072 0300 0000  .r6...r7...r....
-00000ca0: 7238 0000 0072 3900 0000 7208 0000 0072  r8...r9...r....r
-00000cb0: 3a00 0000 723b 0000 0072 1a00 0000 723c  :...r;...r....r<
-00000cc0: 0000 0072 4d00 0000 7227 0000 0072 0f00  ...rM...r'...r..
-00000cd0: 0000 720f 0000 0072 0f00 0000 7215 0000  ..r....r....r...
-00000ce0: 0072 4000 0000 5400 0000 7314 0000 0008  .r@...T...s.....
-00000cf0: 0102 0302 0108 0104 0104 0108 0116 f90e  ................
-00000d00: 2202 0172 4000 0000 6300 0000 0000 0000  "..r@...c.......
-00000d10: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
-00000d20: 0073 3200 0000 6500 5a01 6400 5a02 6503  .s2...e.Z.d.Z.e.
-00000d30: 6a04 6505 6a06 6401 6402 6403 6404 8d04  j.e.j.d.d.d.d...
-00000d40: 5a07 6503 6a04 6508 6a09 6401 6405 6406  Z.e.j.e.j.d.d.d.
-00000d50: 8d03 5a09 6407 5300 2908 da0b 4469 7374  ..Z.d.S.)...Dist
-00000d60: 7269 6275 7465 6472 4100 0000 a905 4e4e  ributedrA.....NN
-00000d70: 7201 0000 0072 0100 0000 4ea9 034e 4e72  r....r....N..NNr
-00000d80: 0100 0000 a903 7248 0000 00da 0769 6e5f  ......rH.....in_
-00000d90: 6178 6573 da08 6f75 745f 6178 6573 724e  axes..out_axesrN
-00000da0: 0000 00a9 0272 4800 0000 7254 0000 004e  .....rH...rT...N
-00000db0: 290a 7234 0000 0072 3500 0000 7236 0000  ).r4...r5...r6..
-00000dc0: 0072 2f00 0000 da04 706d 6170 7240 0000  .r/.....pmapr@..
-00000dd0: 0072 4d00 0000 7233 0000 0072 0900 0000  .rM...r3...r....
-00000de0: 7228 0000 0072 0f00 0000 720f 0000 0072  r(...r....r....r
-00000df0: 0f00 0000 7215 0000 0072 5000 0000 7e00  ....r....rP...~.
-00000e00: 0000 7316 0000 0008 0104 0104 0102 0102  ..s.............
-00000e10: 0102 fc06 0704 0104 0102 0102 fd72 5000  .............rP.
-00000e20: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000e30: 0000 0008 0000 0040 0000 0073 3e00 0000  .......@...s>...
-00000e40: 6500 5a01 6400 5a02 6503 a004 6503 6a05  e.Z.d.Z.e...e.j.
-00000e50: 6506 6a07 6401 6402 6403 6404 8d04 a101  e.j.d.d.d.d.....
-00000e60: 5a08 6503 a004 6503 6a05 6509 6a0a 6401  Z.e...e.j.e.j.d.
-00000e70: 6405 6406 8d03 a101 5a0a 6407 5300 2908  d.d.....Z.d.S.).
-00000e80: da07 564d 6170 7065 6472 4100 0000 7251  ..VMappedrA...rQ
-00000e90: 0000 0072 5200 0000 7253 0000 0072 4e00  ...rR...rS...rN.
-00000ea0: 0000 7256 0000 004e 290b 7234 0000 0072  ..rV...N).r4...r
-00000eb0: 3500 0000 7236 0000 0072 2f00 0000 723e  5...r6...r/...r>
-00000ec0: 0000 00da 0476 6d61 7072 4000 0000 724d  .....vmapr@...rM
-00000ed0: 0000 0072 3300 0000 7209 0000 0072 2800  ...r3...r....r(.
-00000ee0: 0000 720f 0000 0072 0f00 0000 720f 0000  ..r....r....r...
-00000ef0: 0072 1500 0000 7258 0000 008d 0000 0073  .r....rX.......s
-00000f00: 1e00 0000 0801 0401 0401 0401 0201 0201  ................
-00000f10: 02fc 04ff 0409 0401 0401 0401 0201 02fd  ................
-00000f20: 04ff 7258 0000 0029 18da 0674 7970 696e  ..rX...)...typin
-00000f30: 6772 3800 0000 da09 6675 6e63 746f 6f6c  gr8.....functool
-00000f40: 7372 0200 0000 722f 0000 00da 096a 6178  sr....r/.....jax
-00000f50: 2e6e 756d 7079 da05 6e75 6d70 79da 036a  .numpy..numpy..j
-00000f60: 6e70 da0d 6a61 782e 7472 6565 5f75 7469  np..jax.tree_uti
-00000f70: 6c72 4a00 0000 da03 6a74 755a 1966 6c61  lrJ.....jtuZ.fla
-00000f80: 782e 7472 6169 6e69 6e67 2e74 7261 696e  x.training.train
-00000f90: 5f73 7461 7465 7203 0000 00da 0575 7469  _stater......uti
-00000fa0: 6c73 7205 0000 00da 046c 6f73 7372 0700  lsr......lossr..
-00000fb0: 0000 7208 0000 0072 0900 0000 723d 0000  ..r....r....r=..
-00000fc0: 0072 3f00 0000 7240 0000 0072 5000 0000  .r?...r@...rP...
-00000fd0: 7258 0000 0072 0f00 0000 720f 0000 0072  rX...r....r....r
-00000fe0: 0f00 0000 7215 0000 00da 083c 6d6f 6475  ....r......<modu
-00000ff0: 6c65 3e01 0000 0073 1a00 0000 0801 0c02  le>....s........
-00001000: 0801 0c01 0c01 0c02 0c01 1003 0e3f 1004  .............?..
-00001010: 1004 102a 100f                           ...*..
+00000210: 017d 0874 057c 087c 0564 006b 0972 3c7c  .}.t.|.|.d.k.r<|
+00000220: 056e 0269 007c 0464 038d 0389 0074 0687  .n.i.|.d.....t..
+00000230: 0066 0164 0464 0584 087c 0344 0083 018e  .f.d.d...|.D....
+00000240: 005c 027d 097d 0374 077c 0983 017d 0a7c  .\.}.}.t.|...}.|
+00000250: 0a7c 027c 037c 0866 0366 0253 0029 064e  .|.|.|.f.f.S.).N
+00000260: da06 7061 7261 6d73 da04 726e 6773 2903  ..params..rngs).
+00000270: da05 7072 6564 73da 066c 6162 656c 73da  ..preds..labels.
+00000280: 0669 6e70 7574 7363 0100 0000 0000 0000  .inputsc........
+00000290: 0000 0000 0200 0000 0500 0000 1300 0000  ................
+000002a0: 7318 0000 0067 007c 005d 107d 017c 016a  s....g.|.].}.|.j
+000002b0: 0066 0088 008e 0191 0271 0453 00a9 0029  .f.......q.S...)
+000002c0: 01da 0675 7064 6174 6529 02da 022e 30da  ...update)....0.
+000002d0: 076c 6f73 735f 666e a901 da04 6172 6773  .loss_fn....args
+000002e0: 720f 0000 00fa 372f 686f 6d65 2f46 4341  r.....7/home/FCA
+000002f0: 4d2f 6a79 752f 7072 6f6a 5f6c 6163 7373  M/jyu/proj_lacss
+00000300: 2f6c 6163 7373 2f6c 6163 7373 2f74 7261  /lacss/lacss/tra
+00000310: 696e 2f73 7472 6174 6567 792e 7079 da0a  in/strategy.py..
+00000320: 3c6c 6973 7463 6f6d 703e 1e00 0000 7304  <listcomp>....s.
+00000330: 0000 0006 0002 007a 2145 6167 6572 2e6c  .......z!Eager.l
+00000340: 6f73 735f 666e 2e3c 6c6f 6361 6c73 3e2e  oss_fn.<locals>.
+00000350: 3c6c 6973 7463 6f6d 703e 2908 7205 0000  <listcomp>).r...
+00000360: 00da 0a66 726f 6d5f 7661 6c75 65da 0861  ...from_value..a
+00000370: 7070 6c79 5f66 6e72 1400 0000 da06 6b77  pply_fnr......kw
+00000380: 6172 6773 da04 6469 6374 da03 7a69 70da  args..dict..zip.
+00000390: 0373 756d 290b da03 636c 7372 0a00 0000  .sum)...clsr....
+000003a0: da05 7374 6174 65da 096c 6f73 735f 6c6f  ..state..loss_lo
+000003b0: 6773 720e 0000 0072 0d00 0000 720b 0000  gsr....r....r...
+000003c0: 00da 0a69 6e70 7574 735f 6f62 6a72 0c00  ...inputs_objr..
+000003d0: 0000 da06 6c6f 7373 6573 da0a 746f 7461  ....losses..tota
+000003e0: 6c5f 6c6f 7373 720f 0000 0072 1300 0000  l_lossr....r....
+000003f0: 7215 0000 0072 1200 0000 0e00 0000 7324  r....r........s$
+00000400: 0000 0000 020a 0104 0106 ff02 0204 fe02  ................
+00000410: 0304 fd02 0402 fc08 0702 0102 010e 0102  ................
+00000420: fd06 061a 0108 027a 0d45 6167 6572 2e6c  .......z.Eager.l
+00000430: 6f73 735f 666e 6304 0000 0000 0000 0000  oss_fnc.........
+00000440: 0000 0006 0000 0003 0000 0043 0000 0073  ...........C...s
+00000450: 2400 0000 7400 a001 7c03 a101 7d04 7c02  $...t...|...}.|.
+00000460: 6a02 7c01 6601 7c04 6a03 9e02 7c04 6a04  j.|.f.|.j...|.j.
+00000470: 8e01 7d05 7c05 5300 a901 4e29 0572 0500  ..}.|.S...N).r..
+00000480: 0000 7217 0000 00da 0469 6e69 7472 1400  ..r......initr..
+00000490: 0000 7219 0000 00a9 0672 1d00 0000 da03  ..r......r......
+000004a0: 6b65 79da 056d 6f64 656c 720e 0000 0072  key..modelr....r
+000004b0: 2000 0000 721e 0000 0072 0f00 0000 720f   ...r....r....r.
+000004c0: 0000 0072 1500 0000 da07 696e 6974 5f66  ...r......init_f
+000004d0: 6e23 0000 0073 0600 0000 0002 0a02 1602  n#...s..........
+000004e0: 7a0d 4561 6765 722e 696e 6974 5f66 6e63  z.Eager.init_fnc
+000004f0: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+00000500: 0300 0000 4300 0000 732a 0000 0074 00a0  ....C...s*...t..
+00000510: 017c 02a1 017d 037c 016a 0264 017c 016a  .|...}.|.j.d.|.j
+00000520: 0369 0166 017c 036a 049e 027c 036a 058e  .i.f.|.j...|.j..
+00000530: 017d 047c 0453 0029 024e 720a 0000 0029  .}.|.S.).Nr....)
+00000540: 0672 0500 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000550: 720a 0000 0072 1400 0000 7219 0000 0029  r....r....r....)
+00000560: 0572 1d00 0000 721e 0000 0072 0e00 0000  .r....r....r....
+00000570: 7220 0000 0072 0c00 0000 720f 0000 0072  r ...r....r....r
+00000580: 0f00 0000 7215 0000 00da 0770 7265 6469  ....r......predi
+00000590: 6374 2b00 0000 7312 0000 0000 030a 0104  ct+...s.........
+000005a0: 0108 ff02 0104 ff02 0104 ff04 037a 0d45  .............z.E
+000005b0: 6167 6572 2e70 7265 6469 6374 a906 721e  ager.predict..r.
+000005c0: 0000 0072 1f00 0000 720e 0000 0072 0d00  ...r....r....r..
+000005d0: 0000 720b 0000 00da 0672 6574 7572 6e63  ..r......returnc
+000005e0: 0600 0000 0000 0000 0000 0000 0800 0000  ................
+000005f0: 0700 0000 4300 0000 7340 0000 0074 006a  ....C...s@...t.j
+00000600: 017c 006a 0264 0164 028d 027c 016a 037c  .|.j.d.d...|.j.|
+00000610: 017c 027c 037c 047c 0583 065c 027d 065c  .|.|.|.|...\.}.\
+00000620: 037d 017d 027d 077c 016a 047c 0664 038d  .}.}.}.|.j.|.d..
+00000630: 017d 017c 017c 027c 0766 0353 0029 044e  .}.|.|.|.f.S.).N
+00000640: 54a9 01da 0768 6173 5f61 7578 a901 da05  T....has_aux....
+00000650: 6772 6164 7329 05da 036a 6178 da04 6772  grads)...jax..gr
+00000660: 6164 7212 0000 0072 0a00 0000 da0f 6170  adr....r......ap
+00000670: 706c 795f 6772 6164 6965 6e74 73a9 0872  ply_gradients..r
+00000680: 1d00 0000 721e 0000 0072 1f00 0000 720e  ....r....r....r.
+00000690: 0000 0072 0d00 0000 720b 0000 0072 2f00  ...r....r....r/.
+000006a0: 0000 720c 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+000006b0: 0072 1500 0000 da0a 7472 6169 6e5f 7374  .r......train_st
+000006c0: 6570 3400 0000 7314 0000 0000 0b0e 0104  ep4...s.........
+000006d0: 0102 0102 0102 0102 0102 fa0e 080c 027a  ...............z
+000006e0: 1045 6167 6572 2e74 7261 696e 5f73 7465  .Eager.train_ste
+000006f0: 704e 2910 da08 5f5f 6e61 6d65 5f5f da0a  pN)...__name__..
+00000700: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000710: 616c 6e61 6d65 5f5f da0b 636c 6173 736d  alname__..classm
+00000720: 6574 686f 6472 1200 0000 7228 0000 0072  ethodr....r(...r
+00000730: 2900 0000 7203 0000 00da 0274 70da 0853  )...r......tp..S
+00000740: 6571 7565 6e63 6572 0800 0000 da03 416e  equencer......An
+00000750: 79da 084f 7074 696f 6e61 6c72 1a00 0000  y..Optionalr....
+00000760: da05 5475 706c 6572 3400 0000 720f 0000  ..Tupler4...r...
+00000770: 0072 0f00 0000 720f 0000 0072 1500 0000  .r....r....r....
+00000780: 7209 0000 000d 0000 0073 1c00 0000 0801  r........s......
+00000790: 0201 0a14 0201 0a07 0201 0a08 0203 0201  ................
+000007a0: 0801 0401 0401 0801 16f9 7209 0000 0063  ..........r....c
+000007b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007c0: 0300 0000 4000 0000 7324 0000 0065 005a  ....@...s$...e.Z
+000007d0: 0164 005a 0265 03a0 0465 056a 06a1 015a  .d.Z.e...e.j...Z
+000007e0: 0665 0764 0164 0284 0083 015a 0864 0353  .e.d.d.....Z.d.S
+000007f0: 0029 04da 0443 6f72 6563 0400 0000 0000  .)...Corec......
+00000800: 0000 0000 0000 0600 0000 0300 0000 4300  ..............C.
+00000810: 0000 732a 0000 0074 00a0 017c 03a1 017d  ..s*...t...|...}
+00000820: 0474 02a0 037c 026a 04a1 017c 0166 017c  .t...|.j...|.f.|
+00000830: 046a 059e 027c 046a 068e 017d 057c 0553  .j...|.j...}.|.S
+00000840: 0072 2300 0000 2907 7205 0000 0072 1700  .r#...).r....r..
+00000850: 0000 7230 0000 00da 036a 6974 7224 0000  ..r0.....jitr$..
+00000860: 0072 1400 0000 7219 0000 0072 2500 0000  .r....r....r%...
+00000870: 720f 0000 0072 0f00 0000 7215 0000 0072  r....r....r....r
+00000880: 2800 0000 4f00 0000 7306 0000 0000 020a  (...O...s.......
+00000890: 021c 027a 0c43 6f72 652e 696e 6974 5f66  ...z.Core.init_f
+000008a0: 6e4e 2909 7235 0000 0072 3600 0000 7237  nN).r5...r6...r7
+000008b0: 0000 0072 3000 0000 723f 0000 0072 0900  ...r0...r?...r..
+000008c0: 0000 7229 0000 0072 3800 0000 7228 0000  ..r)...r8...r(..
+000008d0: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
+000008e0: 7215 0000 0072 3e00 0000 4c00 0000 7306  r....r>...L...s.
+000008f0: 0000 0008 010c 0202 0172 3e00 0000 6300  .........r>...c.
+00000900: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000910: 0000 0040 0000 0073 1800 0000 6500 5a01  ...@...s....e.Z.
+00000920: 6400 5a02 6503 a004 6505 6a06 a101 5a06  d.Z.e...e.j...Z.
+00000930: 6401 5300 2902 da03 4a49 544e 2907 7235  d.S.)...JITN).r5
+00000940: 0000 0072 3600 0000 7237 0000 0072 3000  ...r6...r7...r0.
+00000950: 0000 723f 0000 0072 3e00 0000 7234 0000  ..r?...r>...r4..
+00000960: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
+00000970: 7215 0000 0072 4000 0000 5800 0000 7302  r....r@...X...s.
+00000980: 0000 0008 0172 4000 0000 6300 0000 0000  .....r@...c.....
+00000990: 0000 0000 0000 0000 0000 000a 0000 0040  ...............@
+000009a0: 0000 0073 5800 0000 6500 5a01 6400 5a02  ...sX...e.Z.d.Z.
+000009b0: 6503 6504 6505 6a06 6507 1900 6505 6a08  e.e.e.j.e...e.j.
+000009c0: 6505 6a08 6505 6a09 650a 1900 6505 6a0b  e.j.e.j.e...e.j.
+000009d0: 6504 6505 6a06 6507 1900 6505 6a08 6603  e.e.j.e...e.j.f.
+000009e0: 1900 6401 9c06 6402 6403 8404 8301 5a0c  ..d...d.d.....Z.
+000009f0: 6503 6404 6405 8400 8301 5a0d 6406 5300  e.d.d.....Z.d.S.
+00000a00: 2907 da0c 5f44 6973 7472 6962 7574 6564  )..._Distributed
+00000a10: 722a 0000 0063 0600 0000 0000 0000 0000  r*...c..........
+00000a20: 0000 0800 0000 0700 0000 0300 0000 738a  ..............s.
+00000a30: 0000 0074 006a 01a0 0264 01a1 0189 0074  ...t.j...d.....t
+00000a40: 006a 03a0 0487 0066 0164 0264 0384 087c  .j.....f.d.d...|
+00000a50: 05a1 027d 0574 006a 057c 006a 0664 0464  ...}.t.j.|.j.d.d
+00000a60: 058d 027c 016a 077c 017c 027c 037c 047c  ...|.j.|.|.|.|.|
+00000a70: 0583 065c 027d 065c 037d 017d 027d 0774  ...\.}.\.}.}.}.t
+00000a80: 006a 016a 087c 0664 0164 068d 027d 067c  .j.j.|.d.d...}.|
+00000a90: 016a 097c 0664 078d 017d 0174 00a0 0474  .j.|.d...}.t...t
+00000aa0: 0a74 006a 016a 0864 0164 068d 027c 02a1  .t.j.j.d.d...|..
+00000ab0: 027d 027c 017c 027c 0766 0353 0029 084e  .}.|.|.|.f.S.).N
+00000ac0: da06 6d61 7070 6564 6301 0000 0000 0000  ..mappedc.......
+00000ad0: 0000 0000 0001 0000 0004 0000 0013 0000  ................
+00000ae0: 0073 0e00 0000 7400 6a01 a002 7c00 8800  .s....t.j...|...
+00000af0: a102 5300 7223 0000 0029 0372 3000 0000  ..S.r#...).r0...
+00000b00: da06 7261 6e64 6f6d da07 666f 6c64 5f69  ..random..fold_i
+00000b10: 6e29 0172 2600 0000 a901 da0a 6178 6973  n).r&.......axis
+00000b20: 5f69 6e64 6578 720f 0000 0072 1500 0000  _indexr....r....
+00000b30: da08 3c6c 616d 6264 613e 6900 0000 f300  ..<lambda>i.....
+00000b40: 0000 007a 2a5f 4469 7374 7269 6275 7465  ...z*_Distribute
+00000b50: 642e 5f74 7261 696e 5f73 7465 702e 3c6c  d._train_step.<l
+00000b60: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e54  ocals>.<lambda>T
+00000b70: 722c 0000 0029 01da 0961 7869 735f 6e61  r,...)...axis_na
+00000b80: 6d65 722e 0000 0029 0b72 3000 0000 da03  mer....).r0.....
+00000b90: 6c61 7872 4600 0000 da09 7472 6565 5f75  laxrF.....tree_u
+00000ba0: 7469 6cda 0874 7265 655f 6d61 7072 3100  til..tree_mapr1.
+00000bb0: 0000 7212 0000 0072 0a00 0000 da05 706d  ..r....r......pm
+00000bc0: 6561 6e72 3200 0000 7202 0000 0072 3300  eanr2...r....r3.
+00000bd0: 0000 720f 0000 0072 4500 0000 7215 0000  ..r....rE...r...
+00000be0: 00da 0b5f 7472 6169 6e5f 7374 6570 5d00  ..._train_step].
+00000bf0: 0000 7322 0000 0000 0a0c 0106 010a 0002  ..s"............
+00000c00: ff04 040e 0104 0102 0102 0102 0102 0102  ................
+00000c10: fa0e 0910 010c 0318 057a 185f 4469 7374  .........z._Dist
+00000c20: 7269 6275 7465 642e 5f74 7261 696e 5f73  ributed._train_s
+00000c30: 7465 7063 0400 0000 0000 0000 0000 0000  tepc............
+00000c40: 0400 0000 0500 0000 4300 0000 731e 0000  ........C...s...
+00000c50: 0074 00a0 0164 0164 0284 007c 03a1 027d  .t...d.d...|...}
+00000c60: 0374 02a0 037c 017c 027c 03a1 0353 0029  .t...|.|.|...S.)
+00000c70: 034e 6301 0000 0000 0000 0000 0000 0001  .Nc.............
+00000c80: 0000 0002 0000 0053 0000 0073 0800 0000  .......S...s....
+00000c90: 7c00 6401 1900 5300 a902 4e72 0100 0000  |.d...S...Nr....
+00000ca0: 720f 0000 0029 01da 0176 720f 0000 0072  r....)...vr....r
+00000cb0: 0f00 0000 7215 0000 0072 4700 0000 8200  ....r....rG.....
+00000cc0: 0000 7248 0000 007a 265f 4469 7374 7269  ..rH...z&_Distri
+00000cd0: 6275 7465 642e 696e 6974 5f66 6e2e 3c6c  buted.init_fn.<l
+00000ce0: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e29  ocals>.<lambda>)
+00000cf0: 0472 3000 0000 724c 0000 0072 0900 0000  .r0...rL...r....
+00000d00: 7228 0000 0029 0472 1d00 0000 7226 0000  r(...).r....r&..
+00000d10: 0072 2700 0000 720e 0000 0072 0f00 0000  .r'...r....r....
+00000d20: 720f 0000 0072 1500 0000 7228 0000 0080  r....r....r(....
+00000d30: 0000 0073 0400 0000 0002 1001 7a14 5f44  ...s........z._D
+00000d40: 6973 7472 6962 7574 6564 2e69 6e69 745f  istributed.init_
+00000d50: 666e 4e29 0e72 3500 0000 7236 0000 0072  fnN).r5...r6...r
+00000d60: 3700 0000 7238 0000 0072 0300 0000 7239  7...r8...r....r9
+00000d70: 0000 0072 3a00 0000 7208 0000 0072 3b00  ...r:...r....r;.
+00000d80: 0000 723c 0000 0072 1a00 0000 723d 0000  ..r<...r....r=..
+00000d90: 0072 4e00 0000 7228 0000 0072 0f00 0000  .rN...r(...r....
+00000da0: 720f 0000 0072 0f00 0000 7215 0000 0072  r....r....r....r
+00000db0: 4100 0000 5c00 0000 7314 0000 0008 0102  A...\...s.......
+00000dc0: 0302 0108 0104 0104 0108 0116 f90e 2202  ..............".
+00000dd0: 0172 4100 0000 6300 0000 0000 0000 0000  .rA...c.........
+00000de0: 0000 0000 0000 0006 0000 0040 0000 0073  ...........@...s
+00000df0: 3200 0000 6500 5a01 6400 5a02 6503 6a04  2...e.Z.d.Z.e.j.
+00000e00: 6505 6a06 6401 6402 6403 6404 8d04 5a07  e.j.d.d.d.d...Z.
+00000e10: 6503 6a04 6508 6a09 6401 6405 6406 8d03  e.j.e.j.d.d.d...
+00000e20: 5a09 6407 5300 2908 da0b 4469 7374 7269  Z.d.S.)...Distri
+00000e30: 6275 7465 6472 4200 0000 a905 4e4e 7201  butedrB.....NNr.
+00000e40: 0000 0072 0100 0000 4ea9 034e 4e72 0100  ...r....N..NNr..
+00000e50: 0000 a903 7249 0000 00da 0769 6e5f 6178  ....rI.....in_ax
+00000e60: 6573 da08 6f75 745f 6178 6573 724f 0000  es..out_axesrO..
+00000e70: 00a9 0272 4900 0000 7255 0000 004e 290a  ...rI...rU...N).
+00000e80: 7235 0000 0072 3600 0000 7237 0000 0072  r5...r6...r7...r
+00000e90: 3000 0000 da04 706d 6170 7241 0000 0072  0.....pmaprA...r
+00000ea0: 4e00 0000 7234 0000 0072 0900 0000 7229  N...r4...r....r)
+00000eb0: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
+00000ec0: 0000 7215 0000 0072 5100 0000 8600 0000  ..r....rQ.......
+00000ed0: 7316 0000 0008 0104 0104 0102 0102 0102  s...............
+00000ee0: fc06 0704 0104 0102 0102 fd72 5100 0000  ...........rQ...
+00000ef0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000f00: 0008 0000 0040 0000 0073 3e00 0000 6500  .....@...s>...e.
+00000f10: 5a01 6400 5a02 6503 a004 6503 6a05 6506  Z.d.Z.e...e.j.e.
+00000f20: 6a07 6401 6402 6403 6404 8d04 a101 5a08  j.d.d.d.d.....Z.
+00000f30: 6503 a004 6503 6a05 6509 6a0a 6401 6405  e...e.j.e.j.d.d.
+00000f40: 6406 8d03 a101 5a0a 6407 5300 2908 da07  d.....Z.d.S.)...
+00000f50: 564d 6170 7065 6472 4200 0000 7252 0000  VMappedrB...rR..
+00000f60: 0072 5300 0000 7254 0000 0072 4f00 0000  .rS...rT...rO...
+00000f70: 7257 0000 004e 290b 7235 0000 0072 3600  rW...N).r5...r6.
+00000f80: 0000 7237 0000 0072 3000 0000 723f 0000  ..r7...r0...r?..
+00000f90: 00da 0476 6d61 7072 4100 0000 724e 0000  ...vmaprA...rN..
+00000fa0: 0072 3400 0000 7209 0000 0072 2900 0000  .r4...r....r)...
+00000fb0: 720f 0000 0072 0f00 0000 720f 0000 0072  r....r....r....r
+00000fc0: 1500 0000 7259 0000 0095 0000 0073 1e00  ....rY.......s..
+00000fd0: 0000 0801 0401 0401 0401 0201 0201 02fc  ................
+00000fe0: 04ff 0409 0401 0401 0401 0201 02fd 04ff  ................
+00000ff0: 7259 0000 0029 18da 0674 7970 696e 6772  rY...)...typingr
+00001000: 3900 0000 da09 6675 6e63 746f 6f6c 7372  9.....functoolsr
+00001010: 0200 0000 7230 0000 00da 096a 6178 2e6e  ....r0.....jax.n
+00001020: 756d 7079 da05 6e75 6d70 79da 036a 6e70  umpy..numpy..jnp
+00001030: da0d 6a61 782e 7472 6565 5f75 7469 6c72  ..jax.tree_utilr
+00001040: 4b00 0000 da03 6a74 755a 1966 6c61 782e  K.....jtuZ.flax.
+00001050: 7472 6169 6e69 6e67 2e74 7261 696e 5f73  training.train_s
+00001060: 7461 7465 7203 0000 00da 0575 7469 6c73  tater......utils
+00001070: 7205 0000 00da 046c 6f73 7372 0700 0000  r......lossr....
+00001080: 7208 0000 0072 0900 0000 723e 0000 0072  r....r....r>...r
+00001090: 4000 0000 7241 0000 0072 5100 0000 7259  @...rA...rQ...rY
+000010a0: 0000 0072 0f00 0000 720f 0000 0072 0f00  ...r....r....r..
+000010b0: 0000 7215 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000010c0: 3e01 0000 0073 1a00 0000 0801 0c02 0801  >....s..........
+000010d0: 0c01 0c01 0c02 0c01 1003 0e3f 100c 1004  ...........?....
+000010e0: 102a 100f                                .*..
```

### Comparing `lacss-0.4.1/lacss/train/__pycache__/trainer.cpython-38.pyc` & `lacss-0.4.2/lacss/train/__pycache__/trainer.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun 27 18:59:20 2023 UTC, .py size: 12919 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,759 +1,726 @@
-00000000: 550d 0d0a 0000 0000 8831 9b64 7732 0000  U........1.dw2..
+00000000: 550d 0d0a 0000 0000 e67d ad64 6733 0000  U........}.dg3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
-00000050: 6d06 5a06 0100 6400 6401 6c07 5a07 6400  m.Z...d.d.l.Z.d.
-00000060: 6401 6c08 6d09 5a0a 0100 6400 6401 6c0b  d.l.m.Z...d.d.l.
-00000070: 5a0b 6400 6401 6c0c 6d0d 5a0e 0100 6400  Z.d.d.l.m.Z...d.
-00000080: 6403 6c0f 6d10 5a10 6d11 5a11 0100 6400  d.l.m.Z.m.Z...d.
-00000090: 6404 6c12 6d13 5a13 0100 6400 6405 6c14  d.l.m.Z...d.d.l.
-000000a0: 6d15 5a15 0100 6406 6407 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
-000000b0: 6d18 5a18 0100 6408 6409 6c19 6d1a 5a1a  m.Z...d.d.l.m.Z.
-000000c0: 0100 6408 640a 6c1b 5400 6408 640b 6c1c  ..d.d.l.T.d.d.l.
-000000d0: 6d1d 5a1d 0100 6505 6506 8301 5a1e 6503  m.Z...e.e...Z.e.
-000000e0: 6a1f 6503 6a20 6503 6a21 6503 6a20 1900  j.e.j e.j!e.j ..
-000000f0: 6602 1900 5a22 640c 640d 8400 5a23 4700  f...Z"d.d...Z#G.
-00000100: 640e 640f 8400 640f 8302 5a24 6401 5300  d.d...d...Z$d.S.
-00000110: 2910 e900 0000 004e 2902 da09 6c72 755f  )......N)...lru_
-00000120: 6361 6368 65da 0770 6172 7469 616c 2902  cache..partial).
-00000130: da06 6672 6565 7a65 da08 756e 6672 6565  ..freeze..unfree
-00000140: 7a65 2901 da0a 5472 6169 6e53 7461 7465  ze)...TrainState
-00000150: 2901 da16 4772 6164 6965 6e74 5472 616e  )...GradientTran
-00000160: 7366 6f72 6d61 7469 6f6e e902 0000 0029  sformation.....)
-00000170: 02da 0649 6e70 7574 73da 095f 6765 745f  ...Inputs.._get_
-00000180: 6e61 6d65 e901 0000 00a9 01da 0873 7472  name.........str
-00000190: 6174 6567 7929 01da 012a a901 da07 4c6f  ategy)...*....Lo
-000001a0: 7373 4c6f 6763 0100 0000 0000 0000 0000  ssLogc..........
-000001b0: 0000 0200 0000 0600 0000 4300 0000 7328  ..........C...s(
-000001c0: 0000 007a 0c74 007c 0083 017d 0157 006e  ...z.t.|...}.W.n
-000001d0: 1601 0001 0001 0074 007c 0083 0083 017d  .......t.|.....}
-000001e0: 0159 006e 0258 007c 0153 00a9 014e 2901  .Y.n.X.|.S...N).
-000001f0: da04 6974 6572 2902 da01 67da 0269 74a9  ..iter)...g..it.
-00000200: 0072 1500 0000 fa36 2f68 6f6d 652f 4643  .r.....6/home/FC
-00000210: 414d 2f6a 7975 2f70 726f 6a5f 6c61 6373  AM/jyu/proj_lacs
-00000220: 732f 6c61 6373 732f 6c61 6373 732f 7472  s/lacss/lacss/tr
-00000230: 6169 6e2f 7472 6169 6e65 722e 7079 da0d  ain/trainer.py..
-00000240: 5f67 6574 5f69 7465 7261 746f 721a 0000  _get_iterator...
-00000250: 0073 0a00 0000 0001 0201 0c01 0601 1002  .s..............
-00000260: 7217 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000270: 0000 0000 0000 0700 0000 4000 0000 73f0  ..........@...s.
-00000280: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
-00000290: 0264 0264 0365 046a 0566 0465 066a 0765  .d.d.e.j.f.e.j.e
-000002a0: 086a 0965 0a19 0065 0b65 0c65 0d64 049c  .j.e...e.e.e.d..
-000002b0: 0564 0564 0684 055a 0e64 2664 0764 0884  .d.d...Z.d&d.d..
-000002c0: 015a 0f65 1064 0964 0a84 0083 015a 1164  .Z.e.d.d.....Z.d
-000002d0: 2765 0b64 0b9c 0164 0c64 0d84 055a 1264  'e.d...d.d...Z.d
-000002e0: 0264 0e9c 0164 0f64 1084 025a 1364 1164  .d...d.d...Z.d.d
-000002f0: 1284 005a 1464 2864 1364 1484 015a 1564  ...Z.d(d.d...Z.d
-00000300: 2965 086a 0965 1619 0064 159c 0164 1664  )e.j.e...d...d.d
-00000310: 1784 055a 1764 1864 1984 005a 1865 1964  ...Z.d.d...Z.e.d
-00000320: 1a64 1b84 0083 015a 1a64 2a64 1c64 1d84  .d.....Z.d*d.d..
-00000330: 015a 1b64 1e64 1f84 005a 1c65 1064 2064  .Z.d.d...Z.e.d d
-00000340: 2184 0083 015a 1d65 1d6a 1e64 2264 2184  !....Z.e.j.d"d!.
-00000350: 0083 015a 1d65 1064 2364 2484 0083 015a  ...Z.e.d#d$....Z
-00000360: 1f65 1f6a 1e64 2564 2484 0083 015a 1f64  .e.j.d%d$....Z.d
-00000370: 0253 0029 2bda 0754 7261 696e 6572 6160  .S.)+..Trainera`
-00000380: 0500 0020 464c 4158 2074 7261 696e 6572  ... FLAX trainer
-00000390: 0a20 2020 2054 6865 2064 6573 6967 6e20  .    The design 
-000003a0: 6973 2074 6f20 6265 206d 696e 696d 616c  is to be minimal
-000003b0: 2062 7574 2068 656c 7020 6176 6f69 6469   but help avoidi
-000003c0: 6e67 2063 6572 7461 696e 2062 696f 6c65  ng certain biole
-000003d0: 7270 6c61 7465 2063 6f64 6520 7768 656e  rplate code when
-000003e0: 2074 7261 696e 2077 6974 6820 464c 4158   train with FLAX
-000003f0: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
-00000400: 3a0a 2020 2020 2020 2020 6d6f 6465 6c3a  :.        model:
-00000410: 2041 2046 6c61 7820 6d6f 6475 6c65 0a20   A Flax module. 
-00000420: 2020 2020 2020 206c 6f73 7365 733a 2041         losses: A
-00000430: 206c 6973 7420 6f66 206c 6f73 7320 6675   list of loss fu
-00000440: 6e63 7469 6f6e 2028 6f72 206f 7468 6572  nction (or other
-00000450: 2063 616c 6c61 6265 6c73 292e 200a 2020   callabels). .  
-00000460: 2020 2020 2020 6f70 7469 6d69 7a65 723a        optimizer:
-00000470: 2041 6e20 6f70 7461 7820 6f70 7469 6d69   An optax optimi
-00000480: 7a65 720a 2020 2020 2020 2020 7365 6564  zer.        seed
-00000490: 3a20 524e 4720 7365 6564 0a20 2020 2020  : RNG seed.     
-000004a0: 2020 2073 7472 6174 6567 793a 2054 7261     strategy: Tra
-000004b0: 696e 696e 6720 7374 7261 7465 6779 2e20  ining strategy. 
-000004c0: 5365 6520 6c61 6373 732e 7472 6169 6e2e  See lacss.train.
-000004d0: 7374 7261 7465 6779 206d 6f64 756c 652e  strategy module.
-000004e0: 200a 2020 2020 2020 2020 7061 7261 6d73   .        params
-000004f0: 3a20 4375 7272 656e 7420 6d6f 6465 6c20  : Current model 
-00000500: 7061 7261 6d65 7465 7273 2e20 5468 6973  parameters. This
-00000510: 2069 7320 6120 6672 6f7a 656e 2064 6963   is a frozen dic
-00000520: 742e 2054 6869 7320 6973 2072 6561 642f  t. This is read/
-00000530: 7772 6974 652e 0a20 2020 2020 2020 2069  write..        i
-00000540: 6e69 7469 616c 697a 6564 3a20 5768 6574  nitialized: Whet
-00000550: 6865 7220 7468 6520 6d6f 6465 6c20 6861  her the model ha
-00000560: 7320 6265 656e 2069 6e69 7469 616c 697a  s been initializ
-00000570: 6564 2077 6974 6820 616e 206f 7074 696d  ed with an optim
-00000580: 697a 6572 2061 6e64 2069 6e69 7469 616c  izer and initial
-00000590: 2077 6569 6768 7473 2e0a 2020 2020 0a20   weights..    . 
-000005a0: 2020 2043 6f6e 7374 7275 6374 6f72 3a0a     Constructor:.
-000005b0: 2020 2020 2020 2020 6d6f 6465 6c3a 2041          model: A
-000005c0: 2046 6c61 7820 6d6f 6475 6c65 0a20 2020   Flax module.   
-000005d0: 2020 2020 206c 6f73 7365 733a 2041 206c       losses: A l
-000005e0: 6f73 7320 6675 6e63 7469 6f6e 2028 6361  oss function (ca
-000005f0: 6c6c 6162 656c 7329 206f 7220 6120 6c69  llabels) or a li
-00000600: 7374 206f 6620 6c6f 7373 2066 756e 6374  st of loss funct
-00000610: 696f 6e73 2c20 6f72 204e 6f6e 652e 2044  ions, or None. D
-00000620: 6566 6175 6c74 2069 7320 4e6f 6e65 2e0a  efault is None..
-00000630: 2020 2020 2020 2020 2020 2020 5468 6573              Thes
-00000640: 6520 7368 6f75 6c64 2068 6176 6520 7468  e should have th
-00000650: 6520 6361 6c6c 2073 6967 6e69 7475 7265  e call signiture
-00000660: 206f 663a 200a 2020 2020 2020 2020 2020   of: .          
-00000670: 2020 2020 2020 6c6f 7373 203d 206c 6f73        loss = los
-00000680: 735f 666e 2869 6e70 7574 732c 206c 6162  s_fn(inputs, lab
-00000690: 656c 732c 2070 7265 6473 290a 2020 2020  els, preds).    
-000006a0: 2020 2020 2020 2020 5468 6520 2270 7265          The "pre
-000006b0: 6473 2220 6973 2074 6865 206d 6f64 656c  ds" is the model
-000006c0: 206f 7574 7075 742e 2054 6865 2022 696e   output. The "in
-000006d0: 7075 7473 2220 616e 6420 226c 6162 656c  puts" and "label
-000006e0: 7322 2061 7265 2066 726f 6d20 7468 6520  s" are from the 
-000006f0: 7472 6169 6e20 6461 7461 7365 742e 0a20  train dataset.. 
-00000700: 2020 2020 2020 2020 2020 2054 6865 206d             The m
-00000710: 6f64 656c 2074 7261 696e 7320 6f6e 2074  odel trains on t
-00000720: 6865 2073 756d 206f 6620 616c 6c20 6c6f  he sum of all lo
-00000730: 7373 6573 2e0a 2020 2020 2020 2020 6f70  sses..        op
-00000740: 7469 6d69 7a65 723a 2041 6e20 6f70 7461  timizer: An opta
-00000750: 7820 6f70 7469 6d7a 6965 7220 6f72 204e  x optimzier or N
-00000760: 6f6e 650a 2020 2020 2020 2020 7365 6564  one.        seed
-00000770: 3a20 696e 7465 6765 7220 524e 4720 7365  : integer RNG se
-00000780: 6564 2e20 4465 6661 756c 7420 6973 2034  ed. Default is 4
-00000790: 322e 0a20 2020 2020 2020 2073 7472 6174  2..        strat
-000007a0: 6567 793a 2054 7261 696e 696e 6720 7374  egy: Training st
-000007b0: 7261 7465 6779 2e20 5365 6520 6c61 6373  rategy. See lacs
-000007c0: 732e 7472 6169 6e2e 7374 7261 7465 6779  s.train.strategy
-000007d0: 206d 6f64 756c 652e 2044 6566 6175 6c74   module. Default
-000007e0: 2069 7320 4a49 542c 2077 6869 6368 2074   is JIT, which t
-000007f0: 7261 696e 730a 2020 2020 2020 2020 2020  rains.          
-00000800: 2020 6f6e 2061 2073 696e 676c 6520 4750    on a single GP
-00000810: 5520 7769 7468 2075 6e62 6174 6368 6564  U with unbatched
-00000820: 2069 6e70 7574 2064 6174 612e 2055 7365   input data. Use
-00000830: 2056 4d61 7070 6564 2073 7472 6174 6567   VMapped strateg
-00000840: 7920 666f 7220 6261 7468 6365 6420 696e  y for bathced in
-00000850: 7075 742e 2055 7365 0a20 2020 2020 2020  put. Use.       
-00000860: 2020 2020 2044 6973 7472 6962 7574 6564       Distributed
-00000870: 2066 6f72 206d 756c 7469 2d47 5055 2074   for multi-GPU t
-00000880: 7261 696e 696e 672e 2055 7365 2045 6167  raining. Use Eag
-00000890: 6572 2066 6f72 2064 6562 7567 6769 6e67  er for debugging
-000008a0: 2028 6e6f 204a 4954 292e 2059 6f75 2063   (no JIT). You c
-000008b0: 616e 2073 7570 706c 7920 0a20 2020 2020  an supply .     
-000008c0: 2020 2020 2020 2079 6f75 7220 6f77 6e20         your own 
-000008d0: 7374 6174 6567 7920 636c 6173 732e 0a20  stategy class.. 
-000008e0: 2020 204e e92a 0000 0029 05da 056d 6f64     N.*...)...mod
-000008f0: 656c da06 6c6f 7373 6573 da09 6f70 7469  el..losses..opti
-00000900: 6d69 7a65 72da 0473 6565 6472 0d00 0000  mizer..seedr....
-00000910: 6306 0000 0000 0000 0000 0000 0006 0000  c...............
-00000920: 0003 0000 0043 0000 0073 4600 0000 7c01  .....C...sF...|.
-00000930: 7c00 5f00 7c02 7c00 5f01 6400 7c00 5f02  |._.|.|._.d.|._.
-00000940: 7403 7c04 7404 6a05 8302 7222 7c04 6e0a  t.|.t.j...r"|.n.
-00000950: 7406 6a07 a008 7c04 a101 7c00 5f09 7c03  t.j...|...|._.|.
-00000960: 7c00 5f0a 7c05 7c00 5f0b 6401 7c00 5f0c  |._.|.|._.d.|._.
-00000970: 6400 5300 2902 4e46 290d 721a 0000 0072  d.S.).NF).r....r
-00000980: 1b00 0000 da0d 5f6c 6f73 735f 7765 6967  ......_loss_weig
-00000990: 6874 73da 0a69 7369 6e73 7461 6e63 65da  hts..isinstance.
-000009a0: 036a 6e70 da07 6e64 6172 7261 79da 036a  .jnp..ndarray..j
-000009b0: 6178 da06 7261 6e64 6f6d da07 5052 4e47  ax..random..PRNG
-000009c0: 4b65 7972 1d00 0000 da0a 5f6f 7074 696d  Keyr......_optim
-000009d0: 697a 6572 da09 5f73 7472 6174 6567 79da  izer.._strategy.
-000009e0: 0c5f 696e 6974 6961 6c69 7a65 6429 06da  ._initialized)..
-000009f0: 0473 656c 6672 1a00 0000 721b 0000 0072  .selfr....r....r
-00000a00: 1c00 0000 721d 0000 0072 0d00 0000 7215  ....r....r....r.
-00000a10: 0000 0072 1500 0000 7216 0000 00da 085f  ...r....r......_
-00000a20: 5f69 6e69 745f 5f3e 0000 0073 0e00 0000  _init__>...s....
-00000a30: 0008 0601 0601 0602 1e01 0602 0601 7a10  ..............z.
-00000a40: 5472 6169 6e65 722e 5f5f 696e 6974 5f5f  Trainer.__init__
-00000a50: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-00000a60: 0006 0000 0043 0000 0073 aa00 0000 7c00  .....C...s....|.
-00000a70: 6a00 6401 6b08 7212 7401 6402 8301 8201  j.d.k.r.t.d.....
-00000a80: 7c00 6a00 7d02 7a0c 7402 7c02 8301 0100  |.j.}.z.t.|.....
-00000a90: 5700 6e12 0100 0100 0100 7c02 6601 7d02  W.n.......|.f.}.
-00000aa0: 5900 6e02 5800 7c01 6401 6b09 7248 7c01  Y.n.X.|.d.k.rH|.
-00000ab0: 7c00 5f03 6e06 7c00 6a03 7d01 7c01 6401  |._.n.|.j.}.|.d.
-00000ac0: 6b08 7262 6403 7404 7c02 8301 1400 7d01  k.rbd.t.|.....}.
-00000ad0: 7404 7c01 8301 7404 7c02 8301 6b03 728c  t.|...t.|...k.r.
-00000ae0: 7401 6404 7c01 9b00 6405 7404 7c02 8301  t.d.|...d.t.|...
-00000af0: 9b00 6406 9d05 8301 8201 7405 6407 6408  ..d.......t.d.d.
-00000b00: 8400 7406 7c02 7c01 8302 4400 8301 8301  ..t.|.|...D.....
-00000b10: 7c00 5f07 6401 5300 2909 7ac1 2052 6573  |._.d.S.).z. Res
-00000b20: 6574 2069 6e74 6572 6e61 6c20 6c6f 7373  et internal loss
-00000b30: 2076 616c 7565 2074 7261 636b 696e 670a   value tracking.
-00000b40: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00000b50: 2020 2020 2020 2020 2020 206c 6f73 735f             loss_
-00000b60: 7765 6967 6874 733a 204f 7074 696f 6e61  weights: Optiona
-00000b70: 6c20 7765 6967 6874 7320 6f66 2069 6e64  l weights of ind
-00000b80: 6976 6964 7561 6c20 6c6f 7373 2066 756e  ividual loss fun
-00000b90: 6374 696f 6e73 2e20 4966 206e 6f74 204e  ctions. If not N
-00000ba0: 6f6e 652c 2074 6865 0a20 2020 2020 2020  one, the.       
-00000bb0: 2020 2020 2020 2020 2074 6f74 616c 206c           total l
-00000bc0: 6f73 7320 6973 2077 6569 6768 7465 6420  oss is weighted 
-00000bd0: 7375 6d2e 0a20 2020 2020 2020 204e 7a1a  sum..        Nz.
-00000be0: 4e6f 206c 6f73 7320 6675 6e63 7469 6f6e  No loss function
-00000bf0: 7320 7072 6f76 6964 6564 2901 6700 0000  s provided).g...
-00000c00: 0000 00f0 3f7a 164c 6f73 7320 7765 6967  ....?z.Loss weig
-00000c10: 6874 7320 7375 7070 6c69 6564 207a 2e20  hts supplied z. 
-00000c20: 646f 6573 206e 6f74 206d 6174 6368 2074  does not match t
-00000c30: 6865 206e 756d 6265 7220 6f66 206c 6f73  he number of los
-00000c40: 7320 6675 6e63 7469 6f6e 7320 28fa 0129  s functions (..)
-00000c50: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00000c60: 0004 0000 0073 0000 0073 1c00 0000 7c00  .....s...s....|.
-00000c70: 5d14 5c02 7d01 7d02 7400 7c01 7c02 8302  ].\.}.}.t.|.|...
-00000c80: 5600 0100 7102 6400 5300 7211 0000 0072  V...q.d.S.r....r
-00000c90: 0f00 0000 2903 da02 2e30 da04 6c6f 7373  ....)....0..loss
-00000ca0: da01 7772 1500 0000 7215 0000 0072 1600  ..wr....r....r..
-00000cb0: 0000 da09 3c67 656e 6578 7072 3e6f 0000  ....<genexpr>o..
-00000cc0: 0073 0400 0000 0401 0600 7a20 5472 6169  .s........z Trai
-00000cd0: 6e65 722e 7265 7365 742e 3c6c 6f63 616c  ner.reset.<local
-00000ce0: 733e 2e3c 6765 6e65 7870 723e 2908 721b  s>.<genexpr>).r.
-00000cf0: 0000 00da 0a56 616c 7565 4572 726f 7272  .....ValueErrorr
-00000d00: 1200 0000 721e 0000 00da 036c 656e da05  ....r......len..
-00000d10: 7475 706c 65da 037a 6970 da09 6c6f 7373  tuple..zip..loss
-00000d20: 5f6c 6f67 7329 0372 2800 0000 da0c 6c6f  _logs).r(.....lo
-00000d30: 7373 5f77 6569 6768 7473 721b 0000 0072  ss_weightsr....r
-00000d40: 1500 0000 7215 0000 0072 1600 0000 da05  ....r....r......
-00000d50: 7265 7365 7452 0000 0073 2600 0000 0007  resetR...s&.....
-00000d60: 0a01 0802 0601 0201 0c01 0601 0c02 0801  ................
-00000d70: 0802 0602 0801 0c02 1001 0201 14ff 0404  ................
-00000d80: 0801 08ff 7a0d 5472 6169 6e65 722e 7265  ....z.Trainer.re
-00000d90: 7365 7463 0100 0000 0000 0000 0000 0000  setc............
-00000da0: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
-00000db0: 007c 006a 0053 0072 1100 0000 2901 7227  .|.j.S.r....).r'
-00000dc0: 0000 00a9 0172 2800 0000 7215 0000 0072  .....r(...r....r
-00000dd0: 1500 0000 7216 0000 00da 0b69 6e69 7469  ....r......initi
-00000de0: 616c 697a 6564 7300 0000 7302 0000 0000  alizeds...s.....
-00000df0: 027a 1354 7261 696e 6572 2e69 6e69 7469  .z.Trainer.initi
-00000e00: 616c 697a 6564 2901 da02 7478 6303 0000  alized)...txc...
-00000e10: 0000 0000 0000 0000 0008 0000 0005 0000  ................
-00000e20: 0043 0000 0073 a000 0000 7c02 6401 6b08  .C...s....|.d.k.
-00000e30: 720e 7c00 6a00 7d02 7c00 6a01 738e 7c00  r.|.j.}.|.j.s.|.
-00000e40: 6a02 6a03 6401 6b08 7262 7404 7405 7c01  j.j.d.k.rbt.t.|.
-00000e50: 8301 8301 7d03 7406 7c03 8301 5c03 7d04  ....}.t.|...\.}.
-00000e60: 7d05 7d05 7407 6a08 a009 7c00 6a0a a101  }.}.t.j...|.j...
-00000e70: 5c02 7c00 5f0a 7d06 7c00 6a0b a00c 7c06  \.|._.}.|.j...|.
-00000e80: 7c00 6a02 7c04 a103 7d07 6e10 7c00 6a02  |.j.|...}.n.|.j.
-00000e90: a00d a100 5c02 7c00 5f02 7d07 740e 6a0f  ....\.|._.}.t.j.
-00000ea0: 7c00 6a02 6a10 7c07 6402 1900 7c02 6403  |.j.j.|.d...|.d.
-00000eb0: 8d03 7c00 5f11 6e08 7412 6404 8301 8201  ..|._.n.t.d.....
-00000ec0: 6405 7c00 5f01 6401 5300 2906 614c 0200  d.|._.d.S.).aL..
-00000ed0: 0020 496e 6974 6961 6c69 7a65 2074 6865  . Initialize the
-00000ee0: 206d 6f64 656c 2077 6569 6768 7473 2061   model weights a
-00000ef0: 6e64 206f 7074 696d 697a 6572 2073 7461  nd optimizer sta
-00000f00: 7465 732e 0a0a 2020 2020 2020 2020 4172  tes...        Ar
-00000f10: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00000f20: 6461 7461 7365 743a 2041 6e20 6974 6572  dataset: An iter
-00000f30: 6174 6f72 206f 7220 6765 6e65 7261 746f  ator or generato
-00000f40: 7220 6675 6e63 7469 6f6e 2074 6f20 7375  r function to su
-00000f50: 7070 6c79 2074 6865 2074 7261 696e 696e  pply the trainin
-00000f60: 6720 6461 7461 7365 742e 0a20 2020 2020  g dataset..     
-00000f70: 2020 2020 2020 2020 2020 2054 6865 2064             The d
-00000f80: 6174 6173 6574 2073 686f 756c 6420 7969  ataset should yi
-00000f90: 656c 6420 2869 6e70 7574 732c 206c 6162  eld (inputs, lab
-00000fa0: 656c 7329 206f 7220 696e 7075 7473 2e20  els) or inputs. 
-00000fb0: 496e 2074 6865 206c 6174 7465 7220 6361  In the latter ca
-00000fc0: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-00000fd0: 2020 2074 6865 206c 6162 656c 7320 3d20     the labels = 
-00000fe0: 4e6f 6e65 2e20 5468 6520 696e 7075 7473  None. The inputs
-00000ff0: 2069 7320 6569 7468 6572 2061 2074 7570   is either a tup
-00001000: 6c65 206f 7220 6120 6469 6374 2e20 4966  le or a dict. If
-00001010: 2074 6865 2069 6e70 7574 7320 0a20 2020   the inputs .   
-00001020: 2020 2020 2020 2020 2020 2020 2069 7320               is 
-00001030: 6120 6469 6374 2c20 7468 6520 6b65 7973  a dict, the keys
-00001040: 2061 7265 2069 6e74 6572 7072 6574 6564   are interpreted
-00001050: 2061 7320 7468 6520 6e61 6d65 7320 666f   as the names fo
-00001060: 7220 6b65 7977 6f72 6420 6172 6773 206f  r keyword args o
-00001070: 6620 7468 6520 0a20 2020 2020 2020 2020  f the .         
-00001080: 2020 2020 2020 206d 6f64 656c 2773 205f         model's _
-00001090: 5f63 616c 6c5f 5f20 6675 6e63 7469 6f6e  _call__ function
-000010a0: 2e0a 2020 2020 2020 2020 2020 2020 7478  ..            tx
-000010b0: 3a20 4f70 7469 6f6e 616c 206f 7074 6178  : Optional optax
-000010c0: 206f 7074 696d 7a69 6572 2066 6f72 2077   optimzier for w
-000010d0: 6865 6e20 7468 6520 6f62 6a65 6374 2077  hen the object w
-000010e0: 6173 2063 6f6e 7374 7275 6374 6564 2077  as constructed w
-000010f0: 6974 686f 7574 2061 6e20 0a20 2020 2020  ithout an .     
-00001100: 2020 2020 2020 2020 2020 206f 7074 696d             optim
-00001110: 697a 6572 0a20 2020 2020 2020 204e da06  izer.        N..
-00001120: 7061 7261 6d73 a903 da08 6170 706c 795f  params....apply_
-00001130: 666e 7239 0000 0072 3800 0000 7a33 4361  fnr9...r8...z3Ca
-00001140: 6c6c 696e 6720 696e 6974 6961 6c69 7a65  lling initialize
-00001150: 2829 206f 6e20 616c 7265 6164 7920 696e  () on already in
-00001160: 6974 6961 6c69 7a65 6420 5472 6169 6e65  itialized Traine
-00001170: 7254 2913 721c 0000 0072 2700 0000 721a  rT).r....r'...r.
-00001180: 0000 00da 0573 636f 7065 da04 6e65 7874  .....scope..next
-00001190: 7217 0000 00da 1875 6e70 6163 6b5f 785f  r......unpack_x_
-000011a0: 795f 7361 6d70 6c65 5f77 6569 6768 7472  y_sample_weightr
-000011b0: 2200 0000 7223 0000 00da 0573 706c 6974  "...r#.....split
-000011c0: 721d 0000 0072 2600 0000 da07 696e 6974  r....r&.....init
-000011d0: 5f66 6eda 0675 6e62 696e 6472 0600 0000  _fn..unbindr....
-000011e0: da06 6372 6561 7465 da05 6170 706c 79da  ..create..apply.
-000011f0: 0573 7461 7465 722f 0000 0029 0872 2800  .stater/...).r(.
-00001200: 0000 da07 6461 7461 7365 7472 3800 0000  ....datasetr8...
-00001210: da04 7065 656b da06 696e 7075 7473 da01  ..peek..inputs..
-00001220: 5fda 036b 6579 da09 7661 7269 6162 6c65  _..key..variable
-00001230: 7372 1500 0000 7215 0000 0072 1600 0000  sr....r....r....
-00001240: da0a 696e 6974 6961 6c69 7a65 7700 0000  ..initializew...
-00001250: 7320 0000 0000 0c08 0106 0206 010c 010c  s ..............
-00001260: 010e 0214 0114 0310 0204 0106 0106 0102  ................
-00001270: fd0a 0708 027a 1254 7261 696e 6572 2e69  .....z.Trainer.i
-00001280: 6e69 7469 616c 697a 6572 0c00 0000 6302  nitializer....c.
-00001290: 0000 0000 0000 0001 0000 0007 0000 0004  ................
-000012a0: 0000 004b 0000 0073 4c00 0000 7c02 6401  ...K...sL...|.d.
-000012b0: 6b08 720e 7c00 6a00 7d02 7c02 6a01 7d04  k.r.|.j.}.|.j.}.
-000012c0: 7c00 6a02 7d05 7403 7c03 8301 6402 6b04  |.j.}.t.|...d.k.
-000012d0: 723e 7c05 6a04 7405 7c00 6a02 6a06 6601  r>|.j.t.|.j.j.f.
-000012e0: 7c03 8e01 6403 8d01 7d05 7c04 7c05 7c01  |...d...}.|.|.|.
-000012f0: 8302 7d06 7c06 5300 2904 6176 0100 0020  ..}.|.S.).av... 
-00001300: 4361 6c6c 696e 6720 7468 6520 756e 6465  Calling the unde
-00001310: 726c 7969 6e67 206d 6f64 656c 0a0a 2020  rlying model..  
-00001320: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00001330: 2020 2020 2020 2020 696e 7075 7473 3a20          inputs: 
-00001340: 4120 7475 706c 6520 6f72 2061 2064 6963  A tuple or a dic
-00001350: 7420 6173 2074 6865 2069 6e70 7574 7320  t as the inputs 
-00001360: 666f 7220 7468 6520 6d6f 6465 6c2e 0a20  for the model.. 
-00001370: 2020 2020 2020 2020 2020 2073 7472 6174             strat
-00001380: 6567 793a 204f 7074 696f 6e61 6c6c 7920  egy: Optionally 
-00001390: 7375 7070 6c79 2061 2064 6966 6665 726e  supply a differn
-000013a0: 7420 6361 6c6c 696e 6720 7374 7261 7465  t calling strate
-000013b0: 6779 2061 7320 7468 6520 6465 6661 756c  gy as the defaul
-000013c0: 7420 6f6e 650a 2020 2020 2020 2020 2020  t one.          
-000013d0: 2020 2020 2020 7375 7070 6c69 6564 2061        supplied a
-000013e0: 7420 7468 6520 636f 6e73 7472 7563 746f  t the constructo
-000013f0: 722e 0a20 2020 2020 2020 2020 2020 202a  r..            *
-00001400: 2a6b 7761 7267 733a 2041 6464 6974 696f  *kwargs: Additio
-00001410: 6e61 6c20 6b65 7977 6f72 6420 6172 6773  nal keyword args
-00001420: 2070 6173 7365 6420 6f6e 2074 6f20 7468   passed on to th
-00001430: 6520 6d6f 6465 6c0a 2020 2020 2020 2020  e model.        
-00001440: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00001450: 3a0a 2020 2020 2020 2020 2020 2020 4d6f  :.            Mo
-00001460: 6465 6c20 6f75 7470 7574 732e 0a20 2020  del outputs..   
-00001470: 2020 2020 204e 7201 0000 00a9 0172 3b00       Nr......r;.
-00001480: 0000 2907 7226 0000 00da 0770 7265 6469  ..).r&.....predi
-00001490: 6374 7244 0000 0072 3000 0000 da07 7265  ctrD...r0.....re
-000014a0: 706c 6163 65da 0f5f 6361 6368 6564 5f70  place.._cached_p
-000014b0: 6172 7469 616c 723b 0000 0029 0772 2800  artialr;...).r(.
-000014c0: 0000 7247 0000 0072 0d00 0000 da06 6b77  ..rG...r......kw
-000014d0: 6172 6773 da0a 7072 6564 6963 745f 666e  args..predict_fn
-000014e0: 7244 0000 00da 0570 7265 6473 7215 0000  rD.....predsr...
-000014f0: 0072 1500 0000 7216 0000 00da 085f 5f63  .r....r......__c
-00001500: 616c 6c5f 5f9c 0000 0073 1400 0000 000c  all__....s......
-00001510: 0801 0602 0602 0601 0c01 0401 0eff 0603  ................
-00001520: 0a02 7a10 5472 6169 6e65 722e 5f5f 6361  ..z.Trainer.__ca
-00001530: 6c6c 5f5f 6301 0000 0000 0000 0000 0000  ll__c...........
-00001540: 0001 0000 0002 0000 0043 0000 0073 1000  .........C...s..
-00001550: 0000 6401 6402 8400 7c00 6a00 4400 8301  ..d.d...|.j.D...
-00001560: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-00001570: 0000 0200 0000 0500 0000 5300 0000 731c  ..........S...s.
-00001580: 0000 0069 007c 005d 147d 0174 007c 016a  ...i.|.].}.t.|.j
-00001590: 0183 017c 01a0 02a1 0093 0271 0453 0072  ...|.......q.S.r
-000015a0: 1500 0000 2903 720a 0000 00da 076c 6f73  ....).r......los
-000015b0: 735f 666e da07 636f 6d70 7574 6529 0272  s_fn..compute).r
-000015c0: 2b00 0000 5a08 6c6f 7373 5f6c 6f67 7215  +...Z.loss_logr.
-000015d0: 0000 0072 1500 0000 7216 0000 00da 0a3c  ...r....r......<
-000015e0: 6469 6374 636f 6d70 3eb7 0000 0073 0600  dictcomp>....s..
-000015f0: 0000 0602 02ff 0800 7a2c 5472 6169 6e65  ........z,Traine
-00001600: 722e 636f 6d70 7574 655f 6c6f 7373 5f6c  r.compute_loss_l
-00001610: 6f67 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  og.<locals>.<dic
-00001620: 7463 6f6d 703e 2901 7233 0000 0072 3600  tcomp>).r3...r6.
-00001630: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00001640: 00da 1063 6f6d 7075 7465 5f6c 6f73 735f  ...compute_loss_
-00001650: 6c6f 67b6 0000 0073 0600 0000 0001 0602  log....s........
-00001660: 04fe 7a18 5472 6169 6e65 722e 636f 6d70  ..z.Trainer.comp
-00001670: 7574 655f 6c6f 7373 5f6c 6f67 6304 0000  ute_loss_logc...
-00001680: 0000 0000 0000 0000 0012 0000 0007 0000  ................
-00001690: 006b 0000 0073 fc00 0000 7c02 6401 6b08  .k...s....|.d.k.
-000016a0: 720e 7c00 6a00 7d02 7c00 6a01 731c 7402  r.|.j.}.|.j.s.t.
-000016b0: 6402 8301 8201 7c00 a003 a100 0100 7404  d.....|.......t.
-000016c0: 6a05 a006 7c00 6a07 a101 5c02 7c00 5f07  j...|.j...\.|._.
-000016d0: 7d05 7408 7409 7c01 8301 8301 4400 5db2  }.t.t.|.....D.].
-000016e0: 5c02 7d06 7d07 740a 7c07 8301 5c03 7d08  \.}.}.t.|...\.}.
-000016f0: 7d09 7d0a 7c03 6401 6b09 7298 7404 6a05  }.}.|.d.k.r.t.j.
-00001700: a00b 7c05 7c06 a102 7d0b 7404 6a05 a006  ..|.|...}.t.j...
-00001710: 7c0b 740c 7c03 8301 a102 7d0c 6403 6404  |.t.|.....}.d.d.
-00001720: 8400 740d 7c03 7c0c 8302 4400 8301 7d0d  ..t.|.|...D...}.
-00001730: 6e04 6401 7d0d 7c02 6a0e 7d0e 7c00 6a0f  n.d.}.|.j.}.|.j.
-00001740: 6a10 7411 7c00 6a0f 6a12 6601 7c04 8e01  j.t.|.j.j.f.|...
-00001750: 6405 8d01 7d0f 7c0e 7c0f 7c00 6a13 7c08  d...}.|.|.|.j.|.
-00001760: 7c09 7c0d 8305 5c03 7d0f 7c00 5f13 7d10  |.|...\.}.|._.}.
-00001770: 7c0f 6a10 7c00 6a0f 6a12 6405 8d01 7c00  |.j.|.j.j.d...|.
-00001780: 5f0f 7c00 a014 a100 7d11 7c11 5600 0100  _.|.....}.|.V...
-00001790: 7144 6401 5300 2906 6199 0300 0020 4372  qDd.S.).a.... Cr
-000017a0: 6561 7465 2074 6865 2074 7261 696e 696e  eate the trainin
-000017b0: 6720 6974 6572 6174 6f72 0a0a 2020 2020  g iterator..    
-000017c0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000017d0: 2020 2020 2020 6461 7461 7365 743a 2041        dataset: A
-000017e0: 6e20 6974 6572 6174 6f72 206f 7220 6765  n iterator or ge
-000017f0: 6e65 7261 746f 7220 6675 6e63 7469 6f6e  nerator function
-00001800: 2074 6f20 7375 7070 6c79 2074 6865 2074   to supply the t
-00001810: 7261 696e 696e 6720 6461 7461 7365 742e  raining dataset.
-00001820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001830: 2053 6565 2069 6e69 7469 616c 697a 6528   See initialize(
-00001840: 290a 2020 2020 2020 2020 2020 2020 7374  ).            st
-00001850: 7261 7465 6779 3a20 4f70 7469 6f6e 616c  rategy: Optional
-00001860: 6c79 206f 7665 7272 6964 6520 7468 6520  ly override the 
-00001870: 6465 6661 756c 7420 7374 7261 7465 6779  default strategy
-00001880: 2e0a 2020 2020 2020 2020 2020 2020 726e  ..            rn
-00001890: 675f 636f 6c73 3a20 4e61 6d65 7320 6f66  g_cols: Names of
-000018a0: 2061 6e79 2052 4e47 2075 7365 6420 6279   any RNG used by
-000018b0: 2074 6865 206d 6f64 656c 2e20 5368 6f75   the model. Shou
-000018c0: 6c64 2062 6520 6120 6c69 7374 206f 6620  ld be a list of 
-000018d0: 7374 7273 2e0a 2020 2020 2020 2020 2020  strs..          
-000018e0: 2020 2a2a 6b77 6172 6773 3a20 4164 6469    **kwargs: Addi
-000018f0: 7469 6f6e 616c 206b 6579 7761 7264 2061  tional keyward a
-00001900: 7267 7320 7061 7373 6564 2074 6f20 7468  rgs passed to th
-00001910: 6520 6d6f 6465 6c2e 2045 2e67 2e20 2274  e model. E.g. "t
-00001920: 7261 696e 696e 673d 5472 7565 220a 2020  raining=True".  
-00001930: 2020 2020 2020 0a20 2020 2020 2020 2052        .        R
-00001940: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00001950: 2020 2020 4120 6974 6572 6174 6f72 2e20      A iterator. 
-00001960: 5374 6570 7069 6e67 2074 6872 6f75 6768  Stepping through
-00001970: 2074 6865 2069 7465 7261 746f 7220 7769   the iterator wi
-00001980: 6c6c 2074 7261 696e 2074 6865 206d 6f64  ll train the mod
-00001990: 656c 2e20 5468 6520 6974 6572 6174 6f72  el. The iterator
-000019a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000019b0: 2069 7473 656c 6620 7265 7475 726e 7320   itself returns 
-000019c0: 6120 6c6f 7373 206c 6f67 2064 6963 742c  a loss log dict,
-000019d0: 2077 6869 6368 2061 7265 206d 6561 6e20   which are mean 
-000019e0: 6c6f 7373 2076 616c 7565 7320 666f 7220  loss values for 
-000019f0: 6561 6368 206c 6f73 730a 2020 2020 2020  each loss.      
-00001a00: 2020 2020 2020 2020 2020 6675 6e63 7469            functi
-00001a10: 6f6e 2e0a 2020 2020 2020 2020 0a20 2020  on..        .   
-00001a20: 2020 2020 2055 7361 6765 2065 7861 6d70       Usage examp
-00001a30: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-00001a40: 7472 6169 6e65 722e 7265 7365 7428 290a  trainer.reset().
-00001a50: 2020 2020 2020 2020 2020 2020 7472 6169              trai
-00001a60: 6e5f 6974 203d 2074 7261 696e 6572 2e74  n_it = trainer.t
-00001a70: 7261 696e 2874 7261 696e 5f64 6174 6173  rain(train_datas
-00001a80: 6574 2c20 7472 6169 6e69 6e67 3d54 7275  et, training=Tru
-00001a90: 6529 0a20 2020 2020 2020 2020 2020 2066  e).            f
-00001aa0: 6f72 206b 2069 6e20 7261 6e67 6528 7472  or k in range(tr
-00001ab0: 6169 6e5f 7374 6570 7329 3a0a 2020 2020  ain_steps):.    
-00001ac0: 2020 2020 2020 2020 2020 2020 6c6f 7373              loss
-00001ad0: 5f6c 6f67 7320 3d20 6e65 7874 2874 7261  _logs = next(tra
-00001ae0: 696e 5f69 7429 0a20 2020 2020 2020 2020  in_it).         
-00001af0: 2020 2020 2020 2069 6620 6b20 2520 3130         if k % 10
-00001b00: 3030 203d 3d20 303a 0a20 2020 2020 2020  00 == 0:.       
-00001b10: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00001b20: 6e74 286c 6f73 735f 6c6f 6773 290a 2020  nt(loss_logs).  
-00001b30: 2020 2020 2020 4e7a 2054 7279 2074 6f20        Nz Try to 
-00001b40: 7275 6e20 756e 696e 6974 6961 6c69 7a65  run uninitialize
-00001b50: 6420 7472 6169 6e65 7263 0100 0000 0000  d trainerc......
-00001b60: 0000 0000 0000 0300 0000 0400 0000 5300  ..............S.
-00001b70: 0000 7316 0000 0069 007c 005d 0e5c 027d  ..s....i.|.].\.}
-00001b80: 017d 027c 017c 0293 0271 0453 0072 1500  .}.|.|...q.S.r..
-00001b90: 0000 7215 0000 0029 0372 2b00 0000 da04  ..r....).r+.....
-00001ba0: 6e61 6d65 da01 6b72 1500 0000 7215 0000  name..kr....r...
-00001bb0: 0072 1600 0000 7256 0000 00e2 0000 0073  .r....rV.......s
-00001bc0: 0600 0000 0600 0600 0200 7a21 5472 6169  ..........z!Trai
-00001bd0: 6e65 722e 7472 6169 6e2e 3c6c 6f63 616c  ner.train.<local
-00001be0: 733e 2e3c 6469 6374 636f 6d70 3e72 4c00  s>.<dictcomp>rL.
-00001bf0: 0000 2915 7226 0000 0072 2700 0000 722f  ..).r&...r'...r/
-00001c00: 0000 0072 3500 0000 7222 0000 0072 2300  ...r5...r"...r#.
-00001c10: 0000 723f 0000 0072 1d00 0000 da09 656e  ..r?...r......en
-00001c20: 756d 6572 6174 6572 1700 0000 723e 0000  umerater....r>..
-00001c30: 00da 0766 6f6c 645f 696e 7230 0000 0072  ...fold_inr0...r
-00001c40: 3200 0000 da0a 7472 6169 6e5f 7374 6570  2.....train_step
-00001c50: 7244 0000 0072 4e00 0000 724f 0000 0072  rD...rN...rO...r
-00001c60: 3b00 0000 7233 0000 0072 5700 0000 2912  ;...r3...rW...).
-00001c70: 7228 0000 0072 4500 0000 720d 0000 005a  r(...rE...r....Z
-00001c80: 0872 6e67 5f63 6f6c 7372 5000 0000 721d  .rng_colsrP...r.
-00001c90: 0000 00da 0473 7465 70da 0464 6174 6172  .....step..datar
-00001ca0: 4700 0000 da06 6c61 6265 6c73 7248 0000  G.....labelsrH..
-00001cb0: 0072 4900 0000 da04 6b65 7973 da04 726e  .rI.....keys..rn
-00001cc0: 6773 da08 7472 6169 6e5f 666e 7244 0000  gs..train_fnrD..
-00001cd0: 0072 5200 0000 da0a 6261 7463 685f 6c6f  .rR.....batch_lo
-00001ce0: 6773 7215 0000 0072 1500 0000 7216 0000  gsr....r....r...
-00001cf0: 00da 0574 7261 696e bc00 0000 7336 0000  ...train....s6..
-00001d00: 0000 1708 0106 0206 0108 0208 0214 0114  ................
-00001d10: 010e 0208 010e 0112 0116 0204 0206 0206  ................
-00001d20: 010e ff06 0302 0102 0004 0002 0002 0002  ................
-00001d30: ff0c 0312 0208 027a 0d54 7261 696e 6572  .......z.Trainer
-00001d40: 2e74 7261 696e 2901 da0a 7375 625f 6d6f  .train)...sub_mo
-00001d50: 6475 6c65 6303 0000 0000 0000 0000 0000  dulec...........
-00001d60: 0006 0000 0009 0000 0043 0000 0073 9000  .........C...s..
-00001d70: 0000 7c00 6a00 7d03 7c00 6a01 7d04 7c02  ..|.j.}.|.j.}.|.
-00001d80: 6401 6b09 7242 7c03 a002 7403 7c04 6402  d.k.rB|...t.|.d.
-00001d90: 8d01 a101 7d03 7404 7c03 7c02 8302 7d03  ....}.t.|.|...}.
-00001da0: 7c03 a005 a100 5c02 7d03 7d04 7c04 6403  |.....\.}.}.|.d.
-00001db0: 1900 7d04 7406 7c01 7407 8302 7256 7408  ..}.t.|.t...rVt.
-00001dc0: a009 7c01 a101 7d01 7c01 6a0a 6a0b 6404  ..|...}.|.j.j.d.
-00001dd0: 6404 6405 8d02 0100 740c 7c01 6406 8302  d.d.....t.|.d...
-00001de0: 8f16 7d05 740d a00e 7c03 7c04 6602 7c05  ..}.t...|.|.f.|.
-00001df0: a102 0100 5700 3500 5100 5200 5800 6401  ....W.5.Q.R.X.d.
-00001e00: 5300 2907 6101 0100 0020 5361 7665 2074  S.).a.... Save t
-00001e10: 6865 206d 6f64 656c 2069 6e20 6120 7069  he model in a pi
-00001e20: 636b 6c65 6420 6669 6c65 2e20 5468 6520  ckled file. The 
-00001e30: 7069 636b 6c65 2069 7320 6120 7475 706c  pickle is a tupl
-00001e40: 6520 6f66 0a20 2020 2020 2020 2020 2020  e of.           
-00001e50: 2028 6d6f 6475 6c65 2c20 7765 6967 6874   (module, weight
-00001e60: 7329 2e0a 0a20 2020 2020 2020 2041 7267  s)...        Arg
-00001e70: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
-00001e80: 6174 683a 2054 6865 2066 696c 6520 7061  ath: The file pa
-00001e90: 7468 2e0a 2020 2020 2020 2020 2020 2020  th..            
-00001ea0: 7375 625f 6d6f 6475 6c65 3a20 4f70 7469  sub_module: Opti
-00001eb0: 6f6e 616c 6c79 206f 6e6c 7920 7361 7665  onally only save
-00001ec0: 2061 2073 7562 5f6d 6f64 756c 6520 6f66   a sub_module of
-00001ed0: 2074 6865 206d 6f64 656c 0a20 2020 2020   the model.     
-00001ee0: 2020 2020 2020 2020 2020 2062 7920 7370             by sp
-00001ef0: 6563 6966 7969 6e67 2074 6865 206e 616d  ecifying the nam
-00001f00: 650a 2020 2020 2020 2020 4ea9 0172 3900  e.        N..r9.
-00001f10: 0000 7239 0000 0054 a902 da07 7061 7265  ..r9...T....pare
-00001f20: 6e74 73da 0865 7869 7374 5f6f 6bda 0277  nts..exist_ok..w
-00001f30: 6229 0f72 1a00 0000 7239 0000 00da 0462  b).r....r9.....b
-00001f40: 696e 64da 0464 6963 74da 0767 6574 6174  ind..dict..getat
-00001f50: 7472 7241 0000 0072 1f00 0000 da03 7374  trrA...r......st
-00001f60: 72da 0770 6174 686c 6962 da04 5061 7468  r..pathlib..Path
-00001f70: da06 7061 7265 6e74 da05 6d6b 6469 72da  ..parent..mkdir.
-00001f80: 046f 7065 6eda 0b63 6c6f 7564 7069 636b  .open..cloudpick
-00001f90: 6c65 da04 6475 6d70 2906 7228 0000 00da  le..dump).r(....
-00001fa0: 0470 6174 6872 6500 0000 da06 6d6f 6475  .pathre.....modu
-00001fb0: 6c65 7239 0000 00da 0166 7215 0000 0072  ler9.....fr....r
-00001fc0: 1500 0000 7216 0000 00da 0a73 6176 655f  ....r......save_
-00001fd0: 6d6f 6465 6cf4 0000 0073 1800 0000 0009  model....s......
-00001fe0: 0601 0602 0801 1001 0a01 0c01 0802 0a01  ................
-00001ff0: 0a02 1001 0c01 7a12 5472 6169 6e65 722e  ......z.Trainer.
-00002000: 7361 7665 5f6d 6f64 656c 6302 0000 0000  save_modelc.....
-00002010: 0000 0000 0000 0003 0000 0009 0000 0043  ...............C
-00002020: 0000 0073 4a00 0000 7400 7c01 7401 8302  ...sJ...t.|.t...
-00002030: 7214 7402 a003 7c01 a101 7d01 7c01 6a04  r.t...|...}.|.j.
-00002040: 6a05 6401 6401 6402 8d02 0100 7406 7c01  j.d.d.d.....t.|.
-00002050: 6403 8302 8f12 7d02 7407 a008 7c00 7c02  d.....}.t...|.|.
-00002060: a102 0100 5700 3500 5100 5200 5800 6404  ....W.5.Q.R.X.d.
-00002070: 5300 2905 7a98 204d 616b 6520 6120 6368  S.).z. Make a ch
-00002080: 6563 6b70 6f69 6e74 206f 6620 7468 6520  eckpoint of the 
-00002090: 7472 6169 6e65 722e 2054 6869 7320 7361  trainer. This sa
-000020a0: 7665 7320 7468 6520 6d6f 6465 6c20 6173  ves the model as
-000020b0: 2077 656c 6c20 6173 0a20 2020 2020 2020   well as.       
-000020c0: 2074 6865 2074 7261 696e 696e 6720 7374   the training st
-000020d0: 6174 6573 2e0a 0a20 2020 2020 2020 2041  ates...        A
-000020e0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-000020f0: 2070 6174 683a 2054 6865 2066 696c 6520   path: The file 
-00002100: 7061 7468 2e0a 2020 2020 2020 2020 5472  path..        Tr
-00002110: 6700 0000 726a 0000 004e 2909 721f 0000  g...rj...N).r...
-00002120: 0072 6e00 0000 726f 0000 0072 7000 0000  .rn...ro...rp...
-00002130: 7271 0000 0072 7200 0000 7273 0000 0072  rq...rr...rs...r
-00002140: 7400 0000 7275 0000 0029 0372 2800 0000  t...ru...).r(...
-00002150: 7276 0000 0072 7800 0000 7215 0000 0072  rv...rx...r....r
-00002160: 1500 0000 7216 0000 00da 0a63 6865 636b  ....r......check
-00002170: 706f 696e 740d 0100 0073 0a00 0000 0007  point....s......
-00002180: 0a01 0a02 1002 0c01 7a12 5472 6169 6e65  ........z.Traine
-00002190: 722e 6368 6563 6b70 6f69 6e74 6301 0000  r.checkpointc...
-000021a0: 0000 0000 0000 0000 0004 0000 000a 0000  ................
-000021b0: 0043 0000 0073 7200 0000 7400 7c00 7401  .C...sr...t.|.t.
-000021c0: 8302 7214 7402 a003 7c00 a101 7d00 7a0c  ..r.t...|...}.z.
-000021d0: 7c00 a004 a100 7d01 5700 6e30 0400 7405  |.....}.W.n0..t.
-000021e0: 6b0a 7250 0100 7d02 0100 7a12 7406 6401  k.rP..}...z.t.d.
-000021f0: 7c02 9b00 9d02 8301 8201 5700 3500 6402  |.........W.5.d.
-00002200: 7d02 7e02 5800 5900 6e02 5800 7407 a008  }.~.X.Y.n.X.t...
-00002210: 7c01 a101 7d03 7400 7c03 7409 8302 736e  |...}.t.|.t...sn
-00002220: 740a 6403 8301 8201 7c03 5300 2904 7a95  t.d.....|.S.).z.
-00002230: 2052 6573 746f 7265 2066 726f 6d20 7468   Restore from th
-00002240: 6520 6368 6563 6b70 6f69 6e74 2e0a 0a20  e checkpoint... 
-00002250: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00002260: 2020 2020 2020 2020 2070 6174 683a 2054           path: T
-00002270: 6865 2063 6865 636b 706f 696e 7420 6669  he checkpoint fi
-00002280: 6c65 2070 6174 682e 0a0a 2020 2020 2020  le path...      
-00002290: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-000022a0: 2020 2020 2020 2041 206e 6577 2074 7261         A new tra
-000022b0: 696e 6572 206f 626a 6563 742e 0a20 2020  iner object..   
-000022c0: 2020 2020 207a 2e43 6f75 6c64 206e 6f74       z.Could not
-000022d0: 206c 6f61 6420 7468 6520 6368 6563 6b70   load the checkp
-000022e0: 6f69 6e74 2e20 476f 7420 6578 6365 7074  oint. Got except
-000022f0: 696f 6e3a 204e 7a29 5468 6520 7361 7665  ion: Nz)The save
-00002300: 6420 6f62 6a20 6973 206e 6f74 2061 2054  d obj is not a T
-00002310: 7261 696e 6572 2063 6865 636b 706f 696e  rainer checkpoin
-00002320: 7429 0b72 1f00 0000 726e 0000 0072 6f00  t).r....rn...ro.
-00002330: 0000 7270 0000 00da 0a72 6561 645f 6279  ..rp.....read_by
-00002340: 7465 73da 0d42 6173 6545 7863 6570 7469  tes..BaseExcepti
-00002350: 6f6e da07 4f53 4572 726f 7272 7400 0000  on..OSErrorrt...
-00002360: da05 6c6f 6164 7372 1800 0000 da09 5479  ..loadsr......Ty
-00002370: 7065 4572 726f 7229 0472 7600 0000 da06  peError).rv.....
-00002380: 5f62 7974 6573 da01 65da 0774 7261 696e  _bytes..e..train
-00002390: 6572 7215 0000 0072 1500 0000 7216 0000  err....r....r...
-000023a0: 00da 0f66 726f 6d5f 6368 6563 6b70 6f69  ...from_checkpoi
-000023b0: 6e74 1c01 0000 7314 0000 0000 0a0a 010a  nt....s.........
-000023c0: 0202 010c 0110 0120 020a 020a 0108 027a  ....... .......z
-000023d0: 1754 7261 696e 6572 2e66 726f 6d5f 6368  .Trainer.from_ch
-000023e0: 6563 6b70 6f69 6e74 6304 0000 0000 0000  eckpointc.......
-000023f0: 0000 0000 000c 0000 0008 0000 0063 0000  .............c..
-00002400: 0073 9800 0000 7c03 6401 6b08 720e 7c00  .s....|.d.k.r.|.
-00002410: 6a00 7d03 7a0c 7401 7c02 8301 0100 5700  j.}.z.t.|.....W.
-00002420: 6e1a 0400 7402 6b0a 7234 0100 0100 0100  n...t.k.r4......
-00002430: 7c02 6701 7d02 5900 6e02 5800 7403 7c01  |.g.}.Y.n.X.t.|.
-00002440: 8301 4400 5d54 7d04 7404 7c04 8301 5c03  ..D.]T}.t.|...\.
-00002450: 7d05 7d06 7d07 7c03 6a05 7d08 7c08 7c00  }.}.}.|.j.}.|.|.
-00002460: 6a06 7c05 8302 7d09 7407 6600 7c05 7c09  j.|...}.t.f.|.|.
-00002470: 6402 9c02 7c06 9702 8e01 7d0a 7c02 4400  d...|.....}.|.D.
-00002480: 5d10 7d0b 7c0b 6a08 6600 7c0a 8e01 0100  ].}.|.j.f.|.....
-00002490: 717a 7c02 5600 0100 713e 6401 5300 2903  qz|.V...q>d.S.).
-000024a0: 6140 0300 0020 4372 6561 7465 2074 6573  a@... Create tes
-000024b0: 742f 7661 6c69 6461 7469 6f6e 2069 7465  t/validation ite
-000024c0: 7261 746f 722e 0a0a 2020 2020 2020 2020  rator...        
-000024d0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-000024e0: 2020 6461 7461 7365 743a 2041 6e20 6974    dataset: An it
-000024f0: 6572 6174 6f72 206f 7220 6765 6e65 7261  erator or genera
-00002500: 746f 7220 6675 6e63 7469 6f6e 2074 6f20  tor function to 
-00002510: 7375 7070 6c79 2074 6865 2074 6573 7469  supply the testi
-00002520: 6e67 2064 6174 612e 0a20 2020 2020 2020  ng data..       
-00002530: 2020 2020 2020 2020 2054 6865 2069 7465           The ite
-00002540: 7261 746f 7220 7368 6f75 6c64 2079 6965  rator should yie
-00002550: 6c64 2061 2074 7570 706c 6520 6f66 2028  ld a tupple of (
-00002560: 696e 7075 7473 2c20 6c61 6265 6c73 292e  inputs, labels).
-00002570: 2054 6865 206c 6162 656c 730a 2020 2020   The labels.    
-00002580: 2020 2020 2020 2020 2020 2020 7368 6f75              shou
-00002590: 6c64 2062 6520 6120 6469 6374 2e0a 2020  ld be a dict..  
-000025a0: 2020 2020 2020 2020 2020 6d65 7472 6963            metric
-000025b0: 733a 2041 206c 6973 7420 6f66 204d 6574  s: A list of Met
-000025c0: 7269 6320 6f62 6a65 6374 732e 2054 6865  ric objects. The
-000025d0: 7920 7368 6f75 6c64 2068 6176 6520 7477  y should have tw
-000025e0: 6f20 6675 6e63 7469 6f6e 733a 0a20 2020  o functions:.   
-000025f0: 2020 2020 2020 2020 2020 2020 206d 2e75               m.u
-00002600: 7064 6174 6528 7072 6564 732c 202a 2a6b  pdate(preds, **k
-00002610: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-00002620: 2020 2020 2020 2020 2020 2020 7072 6564              pred
-00002630: 7320 6973 2074 6865 206d 6f64 656c 206f  s is the model o
-00002640: 7574 7075 742e 2074 6865 2072 656d 6169  utput. the remai
-00002650: 6e69 6e67 206b 7761 7267 7320 6172 6520  ning kwargs are 
-00002660: 636f 6e74 656e 7420 6f66 0a20 2020 2020  content of.     
-00002670: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00002680: 6162 656c 732e 0a20 2020 2020 2020 2020  abels..         
-00002690: 2020 2020 2020 206d 2e63 6f6d 7075 7465         m.compute
-000026a0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000026b0: 2020 2020 2020 2020 7768 6963 6820 7368          which sh
-000026c0: 6f75 6c64 2072 6574 7572 6e20 7468 6520  ould return the 
-000026d0: 6163 6375 6d75 6c61 7465 6420 6d65 7472  accumulated metr
-000026e0: 6963 2076 616c 7565 2e0a 2020 2020 2020  ic value..      
-000026f0: 2020 2020 2020 7374 7261 7465 6779 3a20        strategy: 
-00002700: 4f70 7469 6f6e 616c 6c79 206f 7665 7272  Optionally overr
-00002710: 6964 6520 7468 6520 6465 6661 756c 7420  ide the default 
-00002720: 7374 7261 7465 6779 2e0a 2020 2020 2020  strategy..      
-00002730: 2020 0a20 2020 2020 2020 2052 6574 7572    .        Retur
-00002740: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00002750: 416e 2069 7465 7261 746f 722e 2053 7465  An iterator. Ste
-00002760: 7070 696e 6720 7468 726f 7567 6820 6974  pping through it
-00002770: 2077 696c 6c20 6472 6976 6520 7468 6520   will drive the 
-00002780: 7570 6461 7469 6e67 206f 6620 6561 6368  updating of each
-00002790: 206d 6574 7269 630a 2020 2020 2020 2020   metric.        
-000027a0: 2020 2020 2020 2020 6f62 6a2e 2054 6865          obj. The
-000027b0: 2069 7465 7261 746f 7220 6974 7365 6c66   iterator itself
-000027c0: 2072 6574 7572 6e20 7468 6520 6c69 7374   return the list
-000027d0: 206f 6620 6d65 7472 6963 732e 0a20 2020   of metrics..   
-000027e0: 2020 2020 204e 2902 7247 0000 0072 5200       N).rG...rR.
-000027f0: 0000 2909 7226 0000 0072 1200 0000 727f  ..).r&...r....r.
-00002800: 0000 0072 1700 0000 723e 0000 0072 4d00  ...r....r>...rM.
-00002810: 0000 7244 0000 0072 6c00 0000 da06 7570  ..rD...rl.....up
-00002820: 6461 7465 290c 7228 0000 0072 4500 0000  date).r(...rE...
-00002830: da07 6d65 7472 6963 7372 0d00 0000 725e  ..metricsr....r^
-00002840: 0000 0072 4700 0000 725f 0000 0072 4800  ...rG...r_...rH.
-00002850: 0000 7251 0000 0072 5200 0000 7250 0000  ..rQ...rR...rP..
-00002860: 00da 016d 7215 0000 0072 1500 0000 7216  ...mr....r....r.
-00002870: 0000 00da 0474 6573 7435 0100 0073 2600  .....test5...s&.
-00002880: 0000 0013 0801 0602 0201 0c01 0e01 0c04  ................
-00002890: 0c01 0e01 0601 0c01 0401 0201 02fe 0403  ................
-000028a0: 02fd 0605 0801 0e02 7a0c 5472 6169 6e65  ........z.Traine
-000028b0: 722e 7465 7374 6301 0000 0000 0000 0000  r.testc.........
-000028c0: 0000 0004 0000 0003 0000 004f 0000 0073  ...........O...s
-000028d0: 2000 0000 7c00 6a00 7c01 7c02 8e01 4400   ...|.j.|.|...D.
-000028e0: 5d04 7d03 710c 6401 6402 8400 7c03 4400  ].}.q.d.d...|.D.
-000028f0: 8301 5300 2903 7ab8 2041 2063 6f6e 7669  ..S.).z. A convi
-00002900: 656e 7420 6675 6e63 7469 6f6e 2074 6f20  ent function to 
-00002910: 636f 6d70 7574 6520 616c 6c20 6d65 7472  compute all metr
-00002920: 6963 732e 0a0a 2020 2020 2020 2020 4172  ics...        Ar
-00002930: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00002940: 7361 6d65 2061 7320 7468 6520 7465 7374  same as the test
-00002950: 2829 2066 7563 6e74 696f 6e0a 2020 2020  () fucntion.    
-00002960: 2020 2020 0a20 2020 2020 2020 2052 6574      .        Ret
-00002970: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00002980: 2020 4120 6d65 7472 6963 2064 6963 742e    A metric dict.
-00002990: 204b 6579 7320 6172 6520 6d65 7472 6963   Keys are metric
-000029a0: 206e 616d 6573 2e0a 2020 2020 2020 2020   names..        
-000029b0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000029c0: 0005 0000 0053 0000 0073 1a00 0000 6900  .....S...s....i.
-000029d0: 7c00 5d12 7d01 7400 7c01 8301 7c01 a001  |.].}.t.|...|...
-000029e0: a100 9302 7104 5300 7215 0000 0029 0272  ....q.S.r....).r
-000029f0: 0a00 0000 7255 0000 0029 0272 2b00 0000  ....rU...).r+...
-00002a00: 7286 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-00002a10: 1600 0000 7256 0000 006b 0100 0073 0600  ....rV...k...s..
-00002a20: 0000 0600 0200 0600 7a2c 5472 6169 6e65  ........z,Traine
-00002a30: 722e 7465 7374 5f61 6e64 5f63 6f6d 7075  r.test_and_compu
-00002a40: 7465 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  te.<locals>.<dic
-00002a50: 7463 6f6d 703e 2901 7287 0000 0029 0472  tcomp>).r....).r
-00002a60: 2800 0000 da04 6172 6773 7250 0000 0072  (.....argsrP...r
-00002a70: 8500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-00002a80: 0000 00da 1074 6573 745f 616e 645f 636f  .....test_and_co
-00002a90: 6d70 7574 6560 0100 0073 0600 0000 0009  mpute`...s......
-00002aa0: 1001 0201 7a18 5472 6169 6e65 722e 7465  ....z.Trainer.te
-00002ab0: 7374 5f61 6e64 5f63 6f6d 7075 7465 6301  st_and_computec.
-00002ac0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00002ad0: 0000 0043 0000 0073 0800 0000 7c00 6a00  ...C...s....|.j.
-00002ae0: 6a01 5300 7211 0000 0029 0272 4400 0000  j.S.r....).rD...
-00002af0: 7239 0000 0072 3600 0000 7215 0000 0072  r9...r6...r....r
-00002b00: 1500 0000 7216 0000 0072 3900 0000 6d01  ....r....r9...m.
-00002b10: 0000 7302 0000 0000 027a 0e54 7261 696e  ..s......z.Train
-00002b20: 6572 2e70 6172 616d 7363 0200 0000 0000  er.paramsc......
-00002b30: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-00002b40: 0000 7314 0000 007c 006a 006a 017c 0164  ..s....|.j.j.|.d
-00002b50: 018d 017c 005f 0064 0053 0029 024e 7266  ...|._.d.S.).Nrf
-00002b60: 0000 0029 0272 4400 0000 724e 0000 0029  ...).rD...rN...)
-00002b70: 0272 2800 0000 da0a 6e65 775f 7061 7261  .r(.....new_para
-00002b80: 6d73 7215 0000 0072 1500 0000 7216 0000  msr....r....r...
-00002b90: 0072 3900 0000 7101 0000 7302 0000 0000  .r9...q...s.....
-00002ba0: 0263 0100 0000 0000 0000 0000 0000 0100  .c..............
-00002bb0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
-00002bc0: 006a 0053 0072 1100 0000 2901 7225 0000  .j.S.r....).r%..
-00002bd0: 0072 3600 0000 7215 0000 0072 1500 0000  .r6...r....r....
-00002be0: 7216 0000 0072 1c00 0000 7501 0000 7302  r....r....u...s.
-00002bf0: 0000 0000 027a 1154 7261 696e 6572 2e6f  .....z.Trainer.o
-00002c00: 7074 696d 697a 6572 6302 0000 0000 0000  ptimizerc.......
-00002c10: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
-00002c20: 0073 2800 0000 7c01 7c00 5f00 7c00 6a01  .s(...|.|._.|.j.
-00002c30: 7224 7402 6a03 7c00 6a04 6a05 7c00 6a06  r$t.j.|.j.j.|.j.
-00002c40: 7c01 6401 8d03 7c00 5f07 6400 5300 2902  |.d...|._.d.S.).
-00002c50: 4e72 3a00 0000 2908 7225 0000 0072 2700  Nr:...).r%...r'.
-00002c60: 0000 7206 0000 0072 4200 0000 721a 0000  ..r....rB...r...
-00002c70: 0072 4300 0000 7239 0000 0072 4400 0000  .rC...r9...rD...
-00002c80: 2902 7228 0000 0072 3800 0000 7215 0000  ).r(...r8...r...
-00002c90: 0072 1500 0000 7216 0000 0072 1c00 0000  .r....r....r....
-00002ca0: 7901 0000 730e 0000 0000 0206 0206 0104  y...s...........
-00002cb0: 0106 0104 0102 fd29 014e 2901 4e29 024e  .......).N).N).N
-00002cc0: 4e29 014e 2901 4e29 20da 085f 5f6e 616d  N).N).N) ..__nam
-00002cd0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00002ce0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
-00002cf0: 5f64 6f63 5f5f 720d 0000 00da 034a 4954  _doc__r......JIT
-00002d00: da02 6e6e da06 4d6f 6475 6c65 da02 7470  ..nn..Module..tp
-00002d10: da08 4f70 7469 6f6e 616c da06 4c4f 5353  ..Optional..LOSS
-00002d20: 4553 7207 0000 00da 0369 6e74 da04 7479  ESr......int..ty
-00002d30: 7065 7229 0000 0072 3500 0000 da08 7072  per)...r5.....pr
-00002d40: 6f70 6572 7479 7237 0000 0072 4b00 0000  opertyr7...rK...
-00002d50: 7253 0000 0072 5700 0000 7264 0000 0072  rS...rW...rd...r
-00002d60: 6e00 0000 7279 0000 0072 7a00 0000 da0c  n...ry...rz.....
-00002d70: 7374 6174 6963 6d65 7468 6f64 7283 0000  staticmethodr...
-00002d80: 0072 8700 0000 7289 0000 0072 3900 0000  .r....r....r9...
-00002d90: da06 7365 7474 6572 721c 0000 0072 1500  ..setterr....r..
-00002da0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00002db0: 0072 1800 0000 2300 0000 7342 0000 0008  .r....#...sB....
-00002dc0: 0104 1d02 0102 0102 0104 fa02 0204 0108  ................
-00002dd0: 0102 0102 0102 fa0c 140a 2102 010a 0310  ..........!.....
-00002de0: 250e 1a08 060a 3816 1908 0f02 010a 180a  %.....8.........
-00002df0: 2b08 0d02 010a 0304 010a 0302 010a 0304  +...............
-00002e00: 0172 1800 0000 2925 da0b 6461 7461 636c  .r....)%..datacl
-00002e10: 6173 7365 7372 6f00 0000 da06 7479 7069  assesro.....typi
-00002e20: 6e67 7292 0000 00da 0966 756e 6374 6f6f  ngr......functoo
-00002e30: 6c73 7202 0000 0072 0300 0000 7274 0000  lsr....r....rt..
-00002e40: 00da 0a66 6c61 782e 6c69 6e65 6eda 056c  ...flax.linen..l
-00002e50: 696e 656e 7290 0000 0072 2200 0000 da09  inenr....r".....
-00002e60: 6a61 782e 6e75 6d70 79da 056e 756d 7079  jax.numpy..numpy
-00002e70: 7220 0000 00da 1566 6c61 782e 636f 7265  r .....flax.core
-00002e80: 2e66 726f 7a65 6e5f 6469 6374 7204 0000  .frozen_dictr...
-00002e90: 0072 0500 0000 da19 666c 6178 2e74 7261  .r......flax.tra
-00002ea0: 696e 696e 672e 7472 6169 6e5f 7374 6174  ining.train_stat
-00002eb0: 6572 0600 0000 da05 6f70 7461 7872 0700  er......optaxr..
-00002ec0: 0000 da05 7574 696c 7372 0900 0000 720a  ....utilsr....r.
-00002ed0: 0000 00da 0072 0d00 0000 725e 0000 0072  .....r....r^...r
-00002ee0: 2c00 0000 7210 0000 0072 4f00 0000 da05  ,...r....rO.....
-00002ef0: 556e 696f 6eda 0843 616c 6c61 626c 65da  Union..Callable.
-00002f00: 0853 6571 7565 6e63 6572 9400 0000 7217  .Sequencer....r.
-00002f10: 0000 0072 1800 0000 7215 0000 0072 1500  ...r....r....r..
-00002f20: 0000 7215 0000 0072 1600 0000 da08 3c6d  ..r....r......<m
-00002f30: 6f64 756c 653e 0100 0000 7324 0000 0008  odule>....s$....
-00002f40: 0108 0108 0110 0208 010c 0108 010c 0110  ................
-00002f50: 010c 010c 0210 010c 0108 010c 0408 0218  ................
-00002f60: 0308 09                                  ...
+00000020: 0004 0000 0040 0000 0073 d200 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 6d03 5a03 0100 6400 6403 6c00 6d04 5a04  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6401 6c05 6d06 5a07 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6401 6c08 5a08 6400 6401 6c09 6d0a 5a0b  d.l.Z.d.d.l.m.Z.
+00000070: 0100 6400 6401 6c0c 5a0d 6400 6404 6c0e  ..d.d.l.Z.d.d.l.
+00000080: 6d0f 5a0f 6d10 5a10 0100 6400 6405 6c11  m.Z.m.Z...d.d.l.
+00000090: 6d12 5a12 0100 6400 6406 6c13 5400 6407  m.Z...d.d.l.T.d.
+000000a0: 6408 6c14 6d15 5a15 6d16 5a16 0100 6409  d.l.m.Z.m.Z...d.
+000000b0: 640a 6c17 6d18 5a18 0100 6409 6406 6c19  d.l.m.Z...d.d.l.
+000000c0: 5400 6409 640b 6c1a 6d1b 5a1b 0100 651c  T.d.d.l.m.Z...e.
+000000d0: 651d 651e 651d 1900 6602 1900 5a1f 6502  e.e.e...f...Z.e.
+000000e0: 6503 8301 5a20 640c 640d 8400 5a21 4700  e...Z d.d...Z!G.
+000000f0: 640e 640f 8400 640f 8302 5a22 6401 5300  d.d...d...Z"d.S.
+00000100: 2910 e900 0000 004e 2902 da09 6c72 755f  )......N)...lru_
+00000110: 6361 6368 65da 0770 6172 7469 616c 2901  cache..partial).
+00000120: da04 5061 7468 2902 da06 6672 6565 7a65  ..Path)...freeze
+00000130: da08 756e 6672 6565 7a65 2901 da0a 5472  ..unfreeze)...Tr
+00000140: 6169 6e53 7461 7465 2901 da01 2ae9 0200  ainState)...*...
+00000150: 0000 2902 da06 496e 7075 7473 da09 5f67  ..)...Inputs.._g
+00000160: 6574 5f6e 616d 65e9 0100 0000 a901 da08  et_name.........
+00000170: 7374 7261 7465 6779 a901 da07 4c6f 7373  strategy....Loss
+00000180: 4c6f 6763 0100 0000 0000 0000 0000 0000  Logc............
+00000190: 0200 0000 0600 0000 4300 0000 7328 0000  ........C...s(..
+000001a0: 007a 0c74 007c 0083 017d 0157 006e 1601  .z.t.|...}.W.n..
+000001b0: 0001 0001 0074 007c 0083 0083 017d 0159  .....t.|.....}.Y
+000001c0: 006e 0258 007c 0153 00a9 014e 2901 da04  .n.X.|.S...N)...
+000001d0: 6974 6572 2902 da01 67da 0269 74a9 0072  iter)...g..it..r
+000001e0: 1500 0000 fa36 2f68 6f6d 652f 4643 414d  .....6/home/FCAM
+000001f0: 2f6a 7975 2f70 726f 6a5f 6c61 6373 732f  /jyu/proj_lacss/
+00000200: 6c61 6373 732f 6c61 6373 732f 7472 6169  lacss/lacss/trai
+00000210: 6e2f 7472 6169 6e65 722e 7079 da0d 5f67  n/trainer.py.._g
+00000220: 6574 5f69 7465 7261 746f 721a 0000 0073  et_iterator....s
+00000230: 0a00 0000 0001 0201 0c01 0601 1002 7217  ..............r.
+00000240: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000250: 0000 0000 0700 0000 4000 0000 7344 0100  ........@...sD..
+00000260: 0065 005a 0164 005a 0264 015a 0364 0264  .e.Z.d.Z.d.Z.d.d
+00000270: 0264 0365 046a 0566 0465 066a 0765 0865  .d.e.j.f.e.j.e.e
+00000280: 0919 0065 0865 0a19 0065 0b65 0c65 0d66  ...e.e...e.e.e.f
+00000290: 0219 0065 0e64 049c 0564 0564 0684 055a  ...e.d...d.d...Z
+000002a0: 0f64 2a65 0865 1065 1119 0019 0064 079c  .d*e.e.e.....d..
+000002b0: 0164 0864 0984 055a 1265 1364 0a64 0b84  .d.d...Z.e.d.d..
+000002c0: 0083 015a 1464 2b65 0865 0a19 0064 0264  ...Z.d+e.e...d.d
+000002d0: 0c9c 0264 0d64 0e84 055a 1564 0264 0f9c  ...d.d...Z.d.d..
+000002e0: 0165 1665 0865 0e19 0065 1664 109c 0364  .e.e.e...e.d...d
+000002f0: 1164 1284 065a 1765 1864 139c 0164 1464  .d...Z.e.d...d.d
+00000300: 1584 045a 1964 2c65 1a65 0865 0e19 0065  ...Z.d,e.e.e...e
+00000310: 1065 1b19 0065 1c64 169c 0464 1764 1884  .e...e.d...d.d..
+00000320: 055a 1d65 1e64 0264 199c 0264 1a64 1b84  .Z.e.d.d...d.d..
+00000330: 045a 1f65 2065 1e64 1c9c 0164 1d64 1e84  .Z.e e.d...d.d..
+00000340: 0483 015a 2164 2d65 1a65 2265 0865 0e19  ...Z!d-e.e"e.e..
+00000350: 0065 1c64 1f9c 0464 2064 2184 055a 2365  .e.d...d d!..Z#e
+00000360: 1864 139c 0164 2264 2384 045a 2465 1364  .d...d"d#..Z$e.d
+00000370: 2464 2584 0083 015a 2565 256a 2664 2664  $d%....Z%e%j&d&d
+00000380: 2584 0083 015a 2565 1364 2764 2884 0083  %....Z%e.d'd(...
+00000390: 015a 2765 276a 2664 2964 2884 0083 015a  .Z'e'j&d)d(....Z
+000003a0: 2764 0253 0029 2eda 0754 7261 696e 6572  'd.S.)...Trainer
+000003b0: 61d2 0100 0046 4c41 5820 7472 6169 6e65  a....FLAX traine
+000003c0: 720a 2020 2020 5468 6520 6465 7369 676e  r.    The design
+000003d0: 2069 7320 746f 2062 6520 6d69 6e69 6d61   is to be minima
+000003e0: 6c20 6275 7420 6865 6c70 2061 766f 6964  l but help avoid
+000003f0: 696e 6720 6365 7274 6169 6e20 6269 6f6c  ing certain biol
+00000400: 6572 706c 6174 6520 636f 6465 2077 6865  erplate code whe
+00000410: 6e20 7472 6169 6e20 7769 7468 2046 4c41  n train with FLA
+00000420: 580a 0a20 2020 2041 7474 7269 6275 7465  X..    Attribute
+00000430: 733a 0a20 2020 2020 2020 206d 6f64 656c  s:.        model
+00000440: 3a20 4120 466c 6178 206d 6f64 756c 650a  : A Flax module.
+00000450: 2020 2020 2020 2020 6c6f 7373 6573 3a20          losses: 
+00000460: 4120 6c69 7374 206f 6620 6c6f 7373 2066  A list of loss f
+00000470: 756e 6374 696f 6e20 286f 7220 6f74 6865  unction (or othe
+00000480: 7220 6361 6c6c 6162 656c 7329 2e0a 2020  r callabels)..  
+00000490: 2020 2020 2020 6f70 7469 6d69 7a65 723a        optimizer:
+000004a0: 2041 6e20 6f70 7461 7820 6f70 7469 6d69   An optax optimi
+000004b0: 7a65 720a 2020 2020 2020 2020 7365 6564  zer.        seed
+000004c0: 3a20 524e 4720 7365 6564 0a20 2020 2020  : RNG seed.     
+000004d0: 2020 2070 6172 616d 733a 2043 7572 7265     params: Curre
+000004e0: 6e74 206d 6f64 656c 2070 6172 616d 6574  nt model paramet
+000004f0: 6572 732e 2054 6869 7320 6973 2061 2066  ers. This is a f
+00000500: 726f 7a65 6e20 6469 6374 2e20 5468 6973  rozen dict. This
+00000510: 2069 7320 7265 6164 2f77 7269 7465 2e0a   is read/write..
+00000520: 2020 2020 2020 2020 696e 6974 6961 6c69          initiali
+00000530: 7a65 643a 2057 6865 7468 6572 2074 6865  zed: Whether the
+00000540: 206d 6f64 656c 2068 6173 2062 6565 6e20   model has been 
+00000550: 696e 6974 6961 6c69 7a65 6420 7769 7468  initialized with
+00000560: 2061 6e20 6f70 7469 6d69 7a65 7220 616e   an optimizer an
+00000570: 6420 696e 6974 6961 6c20 7765 6967 6874  d initial weight
+00000580: 732e 0a20 2020 204e e92a 0000 0029 05da  s..    N.*...)..
+00000590: 056d 6f64 656c da06 6c6f 7373 6573 da09  .model..losses..
+000005a0: 6f70 7469 6d69 7a65 72da 0473 6565 6472  optimizer..seedr
+000005b0: 0e00 0000 6306 0000 0000 0000 0000 0000  ....c...........
+000005c0: 0006 0000 0003 0000 0043 0000 0073 4600  .........C...sF.
+000005d0: 0000 7c01 7c00 5f00 7c02 7c00 5f01 6401  ..|.|._.|.|._.d.
+000005e0: 7c00 5f02 7403 7c04 7404 6a05 8302 7222  |._.t.|.t.j...r"
+000005f0: 7c04 6e0a 7406 6a07 a008 7c04 a101 7c00  |.n.t.j...|...|.
+00000600: 5f09 7c03 7c00 5f0a 7c05 7c00 5f0b 6402  _.|.|._.|.|._.d.
+00000610: 7c00 5f0c 6401 5300 2903 617f 0200 0043  |._.d.S.).a....C
+00000620: 6f6e 7374 7275 6374 6f72 0a0a 2020 2020  onstructor..    
+00000630: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00000640: 2020 2020 2020 6d6f 6465 6c3a 2041 2046        model: A F
+00000650: 6c61 7820 6d6f 6475 6c65 2e20 4974 2063  lax module. It c
+00000660: 616e 2062 6520 6120 626f 756e 6420 6d6f  an be a bound mo
+00000670: 6475 6c65 2077 6974 6820 7061 7261 6d65  dule with parame
+00000680: 7465 7273 2e0a 2020 2020 2020 2020 2020  ters..          
+00000690: 2020 6c6f 7373 6573 3a20 4120 6c6f 7373    losses: A loss
+000006a0: 2066 756e 6374 696f 6e20 2863 616c 6c61   function (calla
+000006b0: 6265 6c73 2920 6f72 2061 206c 6973 7420  bels) or a list 
+000006c0: 6f66 206c 6f73 7320 6675 6e63 7469 6f6e  of loss function
+000006d0: 732c 206f 7220 4e6f 6e65 2e0a 2020 2020  s, or None..    
+000006e0: 2020 2020 2020 2020 2020 2020 5468 6573              Thes
+000006f0: 6520 7368 6f75 6c64 2068 6176 6520 7468  e should have th
+00000700: 6520 6361 6c6c 2073 6967 6e69 7475 7265  e call signiture
+00000710: 206f 663a 0a20 2020 2020 2020 2020 2020   of:.           
+00000720: 2020 2020 2020 2020 206c 6f73 7320 3d20           loss = 
+00000730: 6c6f 7373 5f66 6e28 696e 7075 7473 2c20  loss_fn(inputs, 
+00000740: 6c61 6265 6c73 2c20 7072 6564 7329 0a20  labels, preds). 
+00000750: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00000760: 6865 2022 7072 6564 7322 2069 7320 7468  he "preds" is th
+00000770: 6520 6d6f 6465 6c20 6f75 7470 7574 2e20  e model output. 
+00000780: 5468 6520 2269 6e70 7574 7322 2061 6e64  The "inputs" and
+00000790: 2022 6c61 6265 6c73 2220 6172 6520 6672   "labels" are fr
+000007a0: 6f6d 2074 6865 2074 7261 696e 2064 6174  om the train dat
+000007b0: 6173 6574 2e0a 2020 2020 2020 2020 2020  aset..          
+000007c0: 2020 2020 2020 5468 6520 6d6f 6465 6c20        The model 
+000007d0: 7472 6169 6e73 206f 6e20 7468 6520 7375  trains on the su
+000007e0: 6d20 6f66 2061 6c6c 206c 6f73 7365 732e  m of all losses.
+000007f0: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
+00000800: 696d 697a 6572 3a20 416e 206f 7074 6178  imizer: An optax
+00000810: 206f 7074 696d 7a69 6572 0a20 2020 2020   optimzier.     
+00000820: 2020 2020 2020 2073 6565 643a 2052 4e47         seed: RNG
+00000830: 2073 6565 642e 0a20 2020 2020 2020 2020   seed..         
+00000840: 2020 2073 7472 6174 6567 793a 2054 7261     strategy: Tra
+00000850: 696e 696e 6720 6261 636b 656e 642e 2053  ining backend. S
+00000860: 6565 205b 5472 6169 6e67 2062 6163 6b65  ee [Traing backe
+00000870: 6e64 735d 282f 6170 692f 7472 6169 6e2f  nds](/api/train/
+00000880: 2374 7261 696e 696e 672d 6261 636b 656e  #training-backen
+00000890: 6473 292e 0a0a 2020 2020 2020 2020 4e46  ds)...        NF
+000008a0: 290d 721a 0000 0072 1b00 0000 da0d 5f6c  ).r....r......_l
+000008b0: 6f73 735f 7765 6967 6874 73da 0a69 7369  oss_weights..isi
+000008c0: 6e73 7461 6e63 65da 036a 6e70 da07 6e64  nstance..jnp..nd
+000008d0: 6172 7261 79da 036a 6178 da06 7261 6e64  array..jax..rand
+000008e0: 6f6d da07 5052 4e47 4b65 7972 1d00 0000  om..PRNGKeyr....
+000008f0: da0a 5f6f 7074 696d 697a 6572 da09 5f73  .._optimizer.._s
+00000900: 7472 6174 6567 79da 0c5f 696e 6974 6961  trategy.._initia
+00000910: 6c69 7a65 6429 06da 0473 656c 6672 1a00  lized)...selfr..
+00000920: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00000930: 0072 0e00 0000 7215 0000 0072 1500 0000  .r....r....r....
+00000940: 7216 0000 00da 085f 5f69 6e69 745f 5f30  r......__init__0
+00000950: 0000 0073 0e00 0000 0016 0601 0601 0602  ...s............
+00000960: 1e01 0602 0601 7a10 5472 6169 6e65 722e  ......z.Trainer.
+00000970: 5f5f 696e 6974 5f5f 2901 da0c 6c6f 7373  __init__)...loss
+00000980: 5f77 6569 6768 7473 6302 0000 0000 0000  _weightsc.......
+00000990: 0000 0000 0003 0000 0006 0000 0043 0000  .............C..
+000009a0: 0073 aa00 0000 7c00 6a00 6401 6b08 7212  .s....|.j.d.k.r.
+000009b0: 7401 6402 8301 8201 7c00 6a00 7d02 7a0c  t.d.....|.j.}.z.
+000009c0: 7402 7c02 8301 0100 5700 6e12 0100 0100  t.|.....W.n.....
+000009d0: 0100 7c02 6601 7d02 5900 6e02 5800 7c01  ..|.f.}.Y.n.X.|.
+000009e0: 6401 6b09 7248 7c01 7c00 5f03 6e06 7c00  d.k.rH|.|._.n.|.
+000009f0: 6a03 7d01 7c01 6401 6b08 7262 6403 7404  j.}.|.d.k.rbd.t.
+00000a00: 7c02 8301 1400 7d01 7404 7c01 8301 7404  |.....}.t.|...t.
+00000a10: 7c02 8301 6b03 728c 7401 6404 7c01 9b00  |...k.r.t.d.|...
+00000a20: 6405 7404 7c02 8301 9b00 6406 9d05 8301  d.t.|.....d.....
+00000a30: 8201 7405 6407 6408 8400 7406 7c02 7c01  ..t.d.d...t.|.|.
+00000a40: 8302 4400 8301 8301 7c00 5f07 6401 5300  ..D.....|._.d.S.
+00000a50: 2909 7ac0 5265 7365 7420 696e 7465 726e  ).z.Reset intern
+00000a60: 616c 206c 6f73 7320 7661 6c75 6520 7472  al loss value tr
+00000a70: 6163 6b69 6e67 0a0a 2020 2020 2020 2020  acking..        
+00000a80: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00000a90: 2020 6c6f 7373 5f77 6569 6768 7473 3a20    loss_weights: 
+00000aa0: 4f70 7469 6f6e 616c 2077 6569 6768 7473  Optional weights
+00000ab0: 206f 6620 696e 6469 7669 6475 616c 206c   of individual l
+00000ac0: 6f73 7320 6675 6e63 7469 6f6e 732e 2049  oss functions. I
+00000ad0: 6620 6e6f 7420 4e6f 6e65 2c20 7468 650a  f not None, the.
+00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000af0: 746f 7461 6c20 6c6f 7373 2069 7320 7765  total loss is we
+00000b00: 6967 6874 6564 2073 756d 2e0a 2020 2020  ighted sum..    
+00000b10: 2020 2020 4e7a 1a4e 6f20 6c6f 7373 2066      Nz.No loss f
+00000b20: 756e 6374 696f 6e73 2070 726f 7669 6465  unctions provide
+00000b30: 6429 0167 0000 0000 0000 f03f 7a16 4c6f  d).g.......?z.Lo
+00000b40: 7373 2077 6569 6768 7473 2073 7570 706c  ss weights suppl
+00000b50: 6965 6420 7a2e 2064 6f65 7320 6e6f 7420  ied z. does not 
+00000b60: 6d61 7463 6820 7468 6520 6e75 6d62 6572  match the number
+00000b70: 206f 6620 6c6f 7373 2066 756e 6374 696f   of loss functio
+00000b80: 6e73 2028 fa01 2963 0100 0000 0000 0000  ns (..)c........
+00000b90: 0000 0000 0300 0000 0400 0000 7300 0000  ............s...
+00000ba0: 731c 0000 007c 005d 145c 027d 017d 0274  s....|.].\.}.}.t
+00000bb0: 007c 017c 0283 0256 0001 0071 0264 0053  .|.|...V...q.d.S
+00000bc0: 0072 1100 0000 720f 0000 0029 03da 022e  .r....r....)....
+00000bd0: 30da 046c 6f73 73da 0177 7215 0000 0072  0..loss..wr....r
+00000be0: 1500 0000 7216 0000 00da 093c 6765 6e65  ....r......<gene
+00000bf0: 7870 723e 6f00 0000 7304 0000 0004 0106  xpr>o...s.......
+00000c00: 007a 2054 7261 696e 6572 2e72 6573 6574  .z Trainer.reset
+00000c10: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
+00000c20: 7072 3e29 0872 1b00 0000 da0a 5661 6c75  pr>).r......Valu
+00000c30: 6545 7272 6f72 7212 0000 0072 1e00 0000  eErrorr....r....
+00000c40: da03 6c65 6eda 0574 7570 6c65 da03 7a69  ..len..tuple..zi
+00000c50: 70da 096c 6f73 735f 6c6f 6773 2903 7228  p..loss_logs).r(
+00000c60: 0000 0072 2a00 0000 721b 0000 0072 1500  ...r*...r....r..
+00000c70: 0000 7215 0000 0072 1600 0000 da05 7265  ..r....r......re
+00000c80: 7365 7452 0000 0073 2600 0000 0007 0a01  setR...s&.......
+00000c90: 0802 0601 0201 0c01 0601 0c02 0801 0802  ................
+00000ca0: 0602 0801 0c02 1001 0201 14ff 0404 0801  ................
+00000cb0: 08ff 7a0d 5472 6169 6e65 722e 7265 7365  ..z.Trainer.rese
+00000cc0: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
+00000cd0: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
+00000ce0: 006a 0053 0072 1100 0000 2901 7227 0000  .j.S.r....).r'..
+00000cf0: 00a9 0172 2800 0000 7215 0000 0072 1500  ...r(...r....r..
+00000d00: 0000 7216 0000 00da 0b69 6e69 7469 616c  ..r......initial
+00000d10: 697a 6564 7300 0000 7302 0000 0000 027a  izeds...s......z
+00000d20: 1354 7261 696e 6572 2e69 6e69 7469 616c  .Trainer.initial
+00000d30: 697a 6564 2902 da02 7478 da06 7265 7475  ized)...tx..retu
+00000d40: 726e 6303 0000 0000 0000 0000 0000 0008  rnc.............
+00000d50: 0000 0005 0000 0043 0000 0073 a000 0000  .......C...s....
+00000d60: 7c02 6401 6b08 720e 7c00 6a00 7d02 7c00  |.d.k.r.|.j.}.|.
+00000d70: 6a01 738e 7c00 6a02 6a03 6401 6b08 7262  j.s.|.j.j.d.k.rb
+00000d80: 7404 7405 7c01 8301 8301 7d03 7406 7c03  t.t.|.....}.t.|.
+00000d90: 8301 5c03 7d04 7d05 7d05 7407 6a08 a009  ..\.}.}.}.t.j...
+00000da0: 7c00 6a0a a101 5c02 7c00 5f0a 7d06 7c00  |.j...\.|._.}.|.
+00000db0: 6a0b a00c 7c06 7c00 6a02 7c04 a103 7d07  j...|.|.j.|...}.
+00000dc0: 6e10 7c00 6a02 a00d a100 5c02 7c00 5f02  n.|.j.....\.|._.
+00000dd0: 7d07 740e 6a0f 7c00 6a02 6a10 7c07 6402  }.t.j.|.j.j.|.d.
+00000de0: 1900 7c02 6403 8d03 7c00 5f11 6e08 7412  ..|.d...|._.n.t.
+00000df0: 6404 8301 8201 6405 7c00 5f01 6401 5300  d.....d.|._.d.S.
+00000e00: 2906 61a0 0100 0049 6e69 7469 616c 697a  ).a....Initializ
+00000e10: 6520 7468 6520 6d6f 6465 6c20 7765 6967  e the model weig
+00000e20: 6874 7320 616e 6420 6f70 7469 6d69 7a65  hts and optimize
+00000e30: 7220 7374 6174 6573 2e0a 0a20 2020 2020  r states...     
+00000e40: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00000e50: 2020 2020 2064 6174 613a 2041 6e20 6974       data: An it
+00000e60: 6572 6174 6f72 206f 7220 6765 6e65 7261  erator or genera
+00000e70: 746f 7220 6675 6e63 7469 6f6e 2074 6f20  tor function to 
+00000e80: 7072 6f64 7563 6520 7472 6169 6e69 6e67  produce training
+00000e90: 2064 6174 6173 6574 2e20 4974 2069 7320   dataset. It is 
+00000ea0: 6e6f 740a 2020 2020 2020 2020 2020 2020  not.            
+00000eb0: 2020 2020 7573 6564 2069 6620 6d6f 6465      used if mode
+00000ec0: 6c20 6973 2062 6f75 6e64 2077 6974 6820  l is bound with 
+00000ed0: 7765 6967 6874 7320 616c 7265 6164 792e  weights already.
+00000ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000ef0: 2073 6565 205b 7472 6169 6e28 295d 282f   see [train()](/
+00000f00: 6170 692f 7472 6169 6e23 6c61 6373 732e  api/train#lacss.
+00000f10: 7472 6169 6e2e 7472 6169 6e65 722e 5472  train.trainer.Tr
+00000f20: 6169 6e65 722e 7472 6169 6e29 0a20 2020  ainer.train).   
+00000f30: 2020 2020 2020 2020 2074 783a 204f 7074           tx: Opt
+00000f40: 696f 6e61 6c20 6f70 7461 7820 6f70 7469  ional optax opti
+00000f50: 6d7a 6965 7220 666f 7220 7768 656e 2074  mzier for when t
+00000f60: 6865 206f 626a 6563 7420 7761 7320 636f  he object was co
+00000f70: 6e73 7472 7563 7465 6420 7769 7468 6f75  nstructed withou
+00000f80: 7420 616e 0a20 2020 2020 2020 2020 2020  t an.           
+00000f90: 2020 2020 206f 7074 696d 697a 6572 0a20       optimizer. 
+00000fa0: 2020 2020 2020 204e da06 7061 7261 6d73         N..params
+00000fb0: a903 da08 6170 706c 795f 666e 723a 0000  ....apply_fnr:..
+00000fc0: 0072 3800 0000 7a33 4361 6c6c 696e 6720  .r8...z3Calling 
+00000fd0: 696e 6974 6961 6c69 7a65 2829 206f 6e20  initialize() on 
+00000fe0: 616c 7265 6164 7920 696e 6974 6961 6c69  already initiali
+00000ff0: 7a65 6420 5472 6169 6e65 7254 2913 721c  zed TrainerT).r.
+00001000: 0000 0072 2700 0000 721a 0000 00da 0573  ...r'...r......s
+00001010: 636f 7065 da04 6e65 7874 7217 0000 00da  cope..nextr.....
+00001020: 1875 6e70 6163 6b5f 785f 795f 7361 6d70  .unpack_x_y_samp
+00001030: 6c65 5f77 6569 6768 7472 2200 0000 7223  le_weightr"...r#
+00001040: 0000 00da 0573 706c 6974 721d 0000 0072  .....splitr....r
+00001050: 2600 0000 da07 696e 6974 5f66 6eda 0675  &.....init_fn..u
+00001060: 6e62 696e 6472 0700 0000 da06 6372 6561  nbindr......crea
+00001070: 7465 da05 6170 706c 79da 0573 7461 7465  te..apply..state
+00001080: 7230 0000 0029 0872 2800 0000 da04 6461  r0...).r(.....da
+00001090: 7461 7238 0000 00da 0470 6565 6bda 0669  tar8.....peek..i
+000010a0: 6e70 7574 73da 015f da03 6b65 79da 0976  nputs.._..key..v
+000010b0: 6172 6961 626c 6573 7215 0000 0072 1500  ariablesr....r..
+000010c0: 0000 7216 0000 00da 0a69 6e69 7469 616c  ..r......initial
+000010d0: 697a 6577 0000 0073 2000 0000 000a 0801  izew...s .......
+000010e0: 0602 0601 0c01 0c01 0e02 1401 1403 1002  ................
+000010f0: 0401 0601 0601 02fd 0a07 0802 7a12 5472  ............z.Tr
+00001100: 6169 6e65 722e 696e 6974 6961 6c69 7a65  ainer.initialize
+00001110: 720d 0000 0029 0372 4800 0000 720e 0000  r....).rH...r...
+00001120: 0072 3900 0000 6302 0000 0000 0000 0001  .r9...c.........
+00001130: 0000 0007 0000 0004 0000 004b 0000 0073  ...........K...s
+00001140: 4c00 0000 7c02 6401 6b08 720e 7c00 6a00  L...|.d.k.r.|.j.
+00001150: 7d02 7c02 6a01 7d04 7c00 6a02 7d05 7403  }.|.j.}.|.j.}.t.
+00001160: 7c03 8301 6402 6b04 723e 7c05 6a04 7405  |...d.k.r>|.j.t.
+00001170: 7c00 6a02 6a06 6601 7c03 8e01 6403 8d01  |.j.j.f.|...d...
+00001180: 7d05 7c04 7c05 7c01 8302 7d06 7c06 5300  }.|.|.|...}.|.S.
+00001190: 2904 616d 0100 0043 616c 6c69 6e67 2074  ).am...Calling t
+000011a0: 6865 2075 6e64 6572 6c79 696e 6720 6d6f  he underlying mo
+000011b0: 6465 6c0a 0a20 2020 2020 2020 2041 7267  del..        Arg
+000011c0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+000011d0: 6e70 7574 733a 2041 2074 7570 6c65 206f  nputs: A tuple o
+000011e0: 7220 6120 6469 6374 2061 7320 7468 6520  r a dict as the 
+000011f0: 696e 7075 7473 2066 6f72 2074 6865 206d  inputs for the m
+00001200: 6f64 656c 2e0a 2020 2020 2020 2020 2020  odel..          
+00001210: 2020 7374 7261 7465 6779 3a20 4f70 7469    strategy: Opti
+00001220: 6f6e 616c 6c79 2073 7570 706c 7920 6120  onally supply a 
+00001230: 6469 6666 6572 6e74 2063 616c 6c69 6e67  differnt calling
+00001240: 2073 7472 6174 6567 7920 6173 2074 6865   strategy as the
+00001250: 2064 6566 6175 6c74 206f 6e65 0a20 2020   default one.   
+00001260: 2020 2020 2020 2020 2020 2020 2073 7570               sup
+00001270: 706c 6965 6420 6174 2074 6865 2063 6f6e  plied at the con
+00001280: 7374 7275 6374 6f72 2e0a 2020 2020 2020  structor..      
+00001290: 2020 2020 2020 2a2a 6b77 6172 6773 3a20        **kwargs: 
+000012a0: 4164 6469 7469 6f6e 616c 206b 6579 776f  Additional keywo
+000012b0: 7264 2061 7267 7320 7061 7373 6564 206f  rd args passed o
+000012c0: 6e20 746f 2074 6865 206d 6f64 656c 0a0a  n to the model..
+000012d0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+000012e0: 0a20 2020 2020 2020 2020 2020 204d 6f64  .            Mod
+000012f0: 656c 206f 7574 7075 7473 2e0a 2020 2020  el outputs..    
+00001300: 2020 2020 4e72 0100 0000 a901 723c 0000      Nr......r<..
+00001310: 0029 0772 2600 0000 da07 7072 6564 6963  .).r&.....predic
+00001320: 7472 4500 0000 7231 0000 00da 0772 6570  trE...r1.....rep
+00001330: 6c61 6365 da0f 5f63 6163 6865 645f 7061  lace.._cached_pa
+00001340: 7274 6961 6c72 3c00 0000 2907 7228 0000  rtialr<...).r(..
+00001350: 0072 4800 0000 720e 0000 00da 066b 7761  .rH...r......kwa
+00001360: 7267 73da 0a70 7265 6469 6374 5f66 6e72  rgs..predict_fnr
+00001370: 4500 0000 da05 7072 6564 7372 1500 0000  E.....predsr....
+00001380: 7215 0000 0072 1600 0000 da08 5f5f 6361  r....r......__ca
+00001390: 6c6c 5f5f 9a00 0000 7314 0000 0000 0e08  ll__....s.......
+000013a0: 0106 0206 0206 010c 0104 010e ff06 030a  ................
+000013b0: 027a 1054 7261 696e 6572 2e5f 5f63 616c  .z.Trainer.__cal
+000013c0: 6c5f 5f29 0172 3900 0000 6301 0000 0000  l__).r9...c.....
+000013d0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+000013e0: 0000 0073 1000 0000 6401 6402 8400 7c00  ...s....d.d...|.
+000013f0: 6a00 4400 8301 5300 2903 4e63 0100 0000  j.D...S.).Nc....
+00001400: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00001410: 5300 0000 731c 0000 0069 007c 005d 147d  S...s....i.|.].}
+00001420: 0174 007c 016a 0183 017c 01a0 02a1 0093  .t.|.j...|......
+00001430: 0271 0453 0072 1500 0000 2903 720b 0000  .q.S.r....).r...
+00001440: 00da 076c 6f73 735f 666e da07 636f 6d70  ...loss_fn..comp
+00001450: 7574 6529 0272 2c00 0000 5a08 6c6f 7373  ute).r,...Z.loss
+00001460: 5f6c 6f67 7215 0000 0072 1500 0000 7216  _logr....r....r.
+00001470: 0000 00da 0a3c 6469 6374 636f 6d70 3eb7  .....<dictcomp>.
+00001480: 0000 0073 0600 0000 0602 02ff 0800 7a2c  ...s..........z,
+00001490: 5472 6169 6e65 722e 636f 6d70 7574 655f  Trainer.compute_
+000014a0: 6c6f 7373 5f6c 6f67 2e3c 6c6f 6361 6c73  loss_log.<locals
+000014b0: 3e2e 3c64 6963 7463 6f6d 703e 2901 7234  >.<dictcomp>).r4
+000014c0: 0000 0072 3600 0000 7215 0000 0072 1500  ...r6...r....r..
+000014d0: 0000 7216 0000 00da 1063 6f6d 7075 7465  ..r......compute
+000014e0: 5f6c 6f73 735f 6c6f 67b6 0000 0073 0600  _loss_log....s..
+000014f0: 0000 0001 0602 04fe 7a18 5472 6169 6e65  ........z.Traine
+00001500: 722e 636f 6d70 7574 655f 6c6f 7373 5f6c  r.compute_loss_l
+00001510: 6f67 2904 da07 6461 7461 7365 7472 0e00  og)...datasetr..
+00001520: 0000 da08 726e 675f 636f 6c73 7239 0000  ....rng_colsr9..
+00001530: 0063 0400 0000 0000 0000 0000 0000 1200  .c..............
+00001540: 0000 0700 0000 6b00 0000 73fc 0000 007c  ......k...s....|
+00001550: 0264 016b 0872 0e7c 006a 007d 027c 006a  .d.k.r.|.j.}.|.j
+00001560: 0173 1c74 0264 0283 0182 017c 00a0 03a1  .s.t.d.....|....
+00001570: 0001 0074 046a 05a0 067c 006a 07a1 015c  ...t.j...|.j...\
+00001580: 027c 005f 077d 0574 0874 097c 0183 0183  .|._.}.t.t.|....
+00001590: 0144 005d b25c 027d 067d 0774 0a7c 0783  .D.].\.}.}.t.|..
+000015a0: 015c 037d 087d 097d 0a7c 0364 016b 0972  .\.}.}.}.|.d.k.r
+000015b0: 9874 046a 05a0 0b7c 057c 06a1 027d 0b74  .t.j...|.|...}.t
+000015c0: 046a 05a0 067c 0b74 0c7c 0383 01a1 027d  .j...|.t.|.....}
+000015d0: 0c64 0364 0484 0074 0d7c 037c 0c83 0244  .d.d...t.|.|...D
+000015e0: 0083 017d 0d6e 0464 017d 0d7c 026a 0e7d  ...}.n.d.}.|.j.}
+000015f0: 0e7c 006a 0f6a 1074 117c 006a 0f6a 1266  .|.j.j.t.|.j.j.f
+00001600: 017c 048e 0164 058d 017d 0f7c 0e7c 0f7c  .|...d...}.|.|.|
+00001610: 006a 137c 087c 097c 0d83 055c 037d 0f7c  .j.|.|.|...\.}.|
+00001620: 005f 137d 107c 0f6a 107c 006a 0f6a 1264  ._.}.|.j.|.j.j.d
+00001630: 058d 017c 005f 0f7c 00a0 14a1 007d 117c  ...|._.|.....}.|
+00001640: 1156 0001 0071 4464 0153 0029 0661 df04  .V...qDd.S.).a..
+00001650: 0000 4372 6561 7465 2074 6865 2074 7261  ..Create the tra
+00001660: 696e 696e 6720 6974 6572 6174 6f72 0a0a  ining iterator..
+00001670: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00001680: 2020 2020 2020 2020 2020 6461 7461 7365            datase
+00001690: 743a 2041 6e20 6974 6572 6174 6f72 206f  t: An iterator o
+000016a0: 7220 6765 6e65 7261 746f 7220 6675 6e63  r generator func
+000016b0: 7469 6f6e 2074 6f20 7375 7070 6c79 2074  tion to supply t
+000016c0: 6865 2074 7261 696e 696e 6720 6461 7461  he training data
+000016d0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000016e0: 2020 5468 6520 6461 7461 7365 7420 7368    The dataset sh
+000016f0: 6f75 6c64 2079 6965 6c64 2060 6060 2869  ould yield ```(i
+00001700: 6e70 7574 732c 206c 6162 656c 7329 6060  nputs, labels)``
+00001710: 6020 6966 2074 6865 2064 6174 6120 636f  ` if the data co
+00001720: 6d65 2077 6974 6820 6c61 6265 6c73 206f  me with labels o
+00001730: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+00001740: 2020 6060 6028 696e 7075 7473 2c20 4e6f    ```(inputs, No
+00001750: 6e65 2960 6060 2069 6620 7468 6572 6520  ne)``` if there 
+00001760: 6973 206e 6f20 6c61 6265 6c2e 2054 6865  is no label. The
+00001770: 2069 6e70 7574 7320 6973 2065 6974 6865   inputs is eithe
+00001780: 7220 6120 7475 706c 6520 6f72 2061 0a20  r a tuple or a. 
+00001790: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000017a0: 6963 742e 2049 6620 7468 6520 696e 7075  ict. If the inpu
+000017b0: 7473 2069 7320 6120 6469 6374 2c20 7468  ts is a dict, th
+000017c0: 6520 6b65 7973 2061 7265 2069 6e74 6572  e keys are inter
+000017d0: 7072 6574 6564 2061 7320 7468 6520 6e61  preted as the na
+000017e0: 6d65 7320 666f 720a 2020 2020 2020 2020  mes for.        
+000017f0: 2020 2020 2020 2020 6b65 7977 6f72 6420          keyword 
+00001800: 6172 6773 206f 6620 7468 6520 6d6f 6465  args of the mode
+00001810: 6c27 7320 5f5f 6361 6c6c 5f5f 2066 756e  l's __call__ fun
+00001820: 6374 696f 6e2e 0a20 2020 2020 2020 2020  ction..         
+00001830: 2020 2073 7472 6174 6567 793a 204f 7074     strategy: Opt
+00001840: 696f 6e61 6c6c 7920 6f76 6572 7269 6465  ionally override
+00001850: 2074 6865 2064 6566 6175 6c74 2073 7472   the default str
+00001860: 6174 6567 792e 0a20 2020 2020 2020 2020  ategy..         
+00001870: 2020 2072 6e67 5f63 6f6c 733a 204e 616d     rng_cols: Nam
+00001880: 6573 206f 6620 616e 7920 524e 4720 7573  es of any RNG us
+00001890: 6564 2062 7920 7468 6520 6d6f 6465 6c2e  ed by the model.
+000018a0: 2053 686f 756c 6420 6265 2061 206c 6973   Should be a lis
+000018b0: 7420 6f66 2073 7472 696e 6773 2e0a 2020  t of strings..  
+000018c0: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
+000018d0: 6773 3a20 4164 6469 7469 6f6e 616c 206b  gs: Additional k
+000018e0: 6579 7761 7264 2061 7267 7320 7061 7373  eyward args pass
+000018f0: 6564 2074 6f20 7468 6520 6d6f 6465 6c2e  ed to the model.
+00001900: 2045 2e67 2e20 2274 7261 696e 696e 673d   E.g. "training=
+00001910: 5472 7565 220a 0a20 2020 2020 2020 2052  True"..        R
+00001920: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00001930: 2020 2020 4120 6974 6572 6174 6f72 2e20      A iterator. 
+00001940: 5374 6570 7069 6e67 2074 6872 6f75 6768  Stepping through
+00001950: 2074 6865 2069 7465 7261 746f 7220 7769   the iterator wi
+00001960: 6c6c 2074 7261 696e 2074 6865 206d 6f64  ll train the mod
+00001970: 656c 2e20 5468 6520 6974 6572 6174 6f72  el. The iterator
+00001980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001990: 2069 7473 656c 6620 7265 7475 726e 7320   itself returns 
+000019a0: 6120 6c6f 7373 206c 6f67 2064 6963 742c  a loss log dict,
+000019b0: 2077 6869 6368 2061 7265 206d 6561 6e20   which are mean 
+000019c0: 6c6f 7373 2076 616c 7565 7320 666f 7220  loss values for 
+000019d0: 6561 6368 206c 6f73 730a 2020 2020 2020  each loss.      
+000019e0: 2020 2020 2020 2020 2020 6675 6e63 7469            functi
+000019f0: 6f6e 2e0a 0a20 2020 2020 2020 2045 7861  on...        Exa
+00001a00: 6d70 6c65 733a 0a20 2020 2020 2020 2020  mples:.         
+00001a10: 2020 2060 6060 0a20 2020 2020 2020 2020     ```.         
+00001a20: 2020 2074 7261 696e 5f69 7420 3d20 7472     train_it = tr
+00001a30: 6169 6e65 722e 7472 6169 6e28 7472 6169  ainer.train(trai
+00001a40: 6e5f 6461 7461 7365 742c 2074 7261 696e  n_dataset, train
+00001a50: 696e 673d 5472 7565 290a 2020 2020 2020  ing=True).      
+00001a60: 2020 2020 2020 666f 7220 6b20 696e 2072        for k in r
+00001a70: 616e 6765 2874 7261 696e 5f73 7465 7073  ange(train_steps
+00001a80: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00001a90: 2020 206c 6f73 735f 6c6f 6773 203d 206e     loss_logs = n
+00001aa0: 6578 7428 7472 6169 6e5f 6974 290a 2020  ext(train_it).  
+00001ab0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00001ac0: 206b 2025 2031 3030 3020 3d3d 2030 3a0a   k % 1000 == 0:.
+00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ae0: 2020 2020 7072 696e 7428 6c6f 7373 5f6c      print(loss_l
+00001af0: 6f67 7329 0a20 2020 2020 2020 2020 2020  ogs).           
+00001b00: 2020 2020 2020 2020 2074 7261 696e 6572           trainer
+00001b10: 2e72 6573 6574 2829 0a20 2020 2020 2020  .reset().       
+00001b20: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
+00001b30: 204e 7a20 5472 7920 746f 2072 756e 2075   Nz Try to run u
+00001b40: 6e69 6e69 7469 616c 697a 6564 2074 7261  ninitialized tra
+00001b50: 696e 6572 6301 0000 0000 0000 0000 0000  inerc...........
+00001b60: 0003 0000 0004 0000 0053 0000 0073 1600  .........S...s..
+00001b70: 0000 6900 7c00 5d0e 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
+00001b80: 7c02 9302 7104 5300 7215 0000 0072 1500  |...q.S.r....r..
+00001b90: 0000 2903 722c 0000 00da 046e 616d 65da  ..).r,.....name.
+00001ba0: 016b 7215 0000 0072 1500 0000 7216 0000  .kr....r....r...
+00001bb0: 0072 5700 0000 ed00 0000 7306 0000 0006  .rW.......s.....
+00001bc0: 0006 0002 007a 2154 7261 696e 6572 2e74  .....z!Trainer.t
+00001bd0: 7261 696e 2e3c 6c6f 6361 6c73 3e2e 3c64  rain.<locals>.<d
+00001be0: 6963 7463 6f6d 703e 724d 0000 0029 1572  ictcomp>rM...).r
+00001bf0: 2600 0000 7227 0000 0072 3000 0000 7235  &...r'...r0...r5
+00001c00: 0000 0072 2200 0000 7223 0000 0072 4000  ...r"...r#...r@.
+00001c10: 0000 721d 0000 00da 0965 6e75 6d65 7261  ..r......enumera
+00001c20: 7465 7217 0000 0072 3f00 0000 da07 666f  ter....r?.....fo
+00001c30: 6c64 5f69 6e72 3100 0000 7233 0000 00da  ld_inr1...r3....
+00001c40: 0a74 7261 696e 5f73 7465 7072 4500 0000  .train_steprE...
+00001c50: 724f 0000 0072 5000 0000 723c 0000 0072  rO...rP...r<...r
+00001c60: 3400 0000 7258 0000 0029 1272 2800 0000  4...rX...).r(...
+00001c70: 7259 0000 0072 0e00 0000 725a 0000 0072  rY...r....rZ...r
+00001c80: 5100 0000 721d 0000 00da 0473 7465 7072  Q...r......stepr
+00001c90: 4600 0000 7248 0000 00da 066c 6162 656c  F...rH.....label
+00001ca0: 7372 4900 0000 724a 0000 00da 046b 6579  srI...rJ.....key
+00001cb0: 73da 0472 6e67 73da 0874 7261 696e 5f66  s..rngs..train_f
+00001cc0: 6e72 4500 0000 7253 0000 00da 0a62 6174  nrE...rS.....bat
+00001cd0: 6368 5f6c 6f67 7372 1500 0000 7215 0000  ch_logsr....r...
+00001ce0: 0072 1600 0000 da05 7472 6169 6ebc 0000  .r......train...
+00001cf0: 0073 3600 0000 0022 0801 0602 0601 0802  .s6...."........
+00001d00: 0802 1401 1401 0e02 0801 0e01 1201 1602  ................
+00001d10: 0402 0602 0601 0eff 0603 0201 0200 0400  ................
+00001d20: 0200 0200 02ff 0c03 1202 0802 7a0d 5472  ............z.Tr
+00001d30: 6169 6e65 722e 7472 6169 6e29 02da 0470  ainer.train)...p
+00001d40: 6174 6872 3900 0000 6302 0000 0000 0000  athr9...c.......
+00001d50: 0000 0000 0004 0000 0009 0000 0043 0000  .............C..
+00001d60: 0073 5200 0000 6401 6402 6c00 7d02 7401  .sR...d.d.l.}.t.
+00001d70: 7c01 7402 8302 721c 7403 a004 7c01 a101  |.t...r.t...|...
+00001d80: 7d01 7c01 6a05 6a06 6403 6403 6404 8d02  }.|.j.j.d.d.d...
+00001d90: 0100 7407 7c01 6405 8302 8f12 7d03 7c02  ..t.|.d.....}.|.
+00001da0: a008 7c00 7c03 a102 0100 5700 3500 5100  ..|.|.....W.5.Q.
+00001db0: 5200 5800 6402 5300 2906 7a98 4d61 6b65  R.X.d.S.).z.Make
+00001dc0: 2061 2070 6963 6b6c 6520 7361 7665 206f   a pickle save o
+00001dd0: 6620 7468 6520 7472 6169 6e65 722e 2054  f the trainer. T
+00001de0: 6869 7320 7361 7665 7320 7468 6520 6d6f  his saves the mo
+00001df0: 6465 6c20 6173 2077 656c 6c20 6173 0a20  del as well as. 
+00001e00: 2020 2020 2020 2074 6865 2074 7261 696e         the train
+00001e10: 696e 6720 7374 6174 6573 2e0a 0a20 2020  ing states...   
+00001e20: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00001e30: 2020 2020 2020 2070 6174 683a 2054 6865         path: The
+00001e40: 2066 696c 6520 7061 7468 2e0a 2020 2020   file path..    
+00001e50: 2020 2020 7201 0000 004e 5429 02da 0770      r....NT)...p
+00001e60: 6172 656e 7473 da08 6578 6973 745f 6f6b  arents..exist_ok
+00001e70: da02 7762 2909 da06 7069 636b 6c65 721f  ..wb)...pickler.
+00001e80: 0000 00da 0373 7472 da07 7061 7468 6c69  .....str..pathli
+00001e90: 6272 0400 0000 da06 7061 7265 6e74 da05  br......parent..
+00001ea0: 6d6b 6469 72da 046f 7065 6eda 0464 756d  mkdir..open..dum
+00001eb0: 7029 0472 2800 0000 7267 0000 0072 6b00  p).r(...rg...rk.
+00001ec0: 0000 da01 6672 1500 0000 7215 0000 0072  ....fr....r....r
+00001ed0: 1600 0000 726b 0000 0018 0100 0073 0c00  ....rk.......s..
+00001ee0: 0000 0007 0802 0a01 0a02 1002 0c01 7a0e  ..............z.
+00001ef0: 5472 6169 6e65 722e 7069 636b 6c65 2901  Trainer.pickle).
+00001f00: 7267 0000 0063 0100 0000 0000 0000 0000  rg...c..........
+00001f10: 0000 0500 0000 0a00 0000 4300 0000 737a  ..........C...sz
+00001f20: 0000 0064 0164 026c 007d 0174 017c 0074  ...d.d.l.}.t.|.t
+00001f30: 0283 0272 1c74 03a0 047c 00a1 017d 007a  ...r.t...|...}.z
+00001f40: 0c7c 00a0 05a1 007d 0257 006e 3004 0074  .|.....}.W.n0..t
+00001f50: 066b 0a72 5801 007d 0301 007a 1274 0764  .k.rX..}...z.t.d
+00001f60: 037c 039b 009d 0283 0182 0157 0035 0064  .|.........W.5.d
+00001f70: 027d 037e 0358 0059 006e 0258 007c 01a0  .}.~.X.Y.n.X.|..
+00001f80: 087c 02a1 017d 0474 017c 0474 0983 0273  .|...}.t.|.t...s
+00001f90: 7674 0a64 0483 0182 017c 0453 0029 057a  vt.d.....|.S.).z
+00001fa0: 9552 6573 746f 7265 2066 726f 6d20 7468  .Restore from th
+00001fb0: 6520 6120 7069 636b 6c65 6420 7361 7665  e a pickled save
+00001fc0: 642e 0a0a 2020 2020 2020 2020 4172 6773  d...        Args
+00001fd0: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+00001fe0: 7468 3a20 5468 6520 7069 636b 6c65 2066  th: The pickle f
+00001ff0: 696c 6520 7061 7468 2e0a 0a20 2020 2020  ile path...     
+00002000: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00002010: 2020 2020 2020 2020 4120 6e65 7720 7472          A new tr
+00002020: 6169 6e65 7220 6f62 6a65 6374 2e0a 2020  ainer object..  
+00002030: 2020 2020 2020 7201 0000 004e 7a2e 436f        r....Nz.Co
+00002040: 756c 6420 6e6f 7420 6c6f 6164 2074 6865  uld not load the
+00002050: 2063 6865 636b 706f 696e 742e 2047 6f74   checkpoint. Got
+00002060: 2065 7863 6570 7469 6f6e 3a20 7a29 5468   exception: z)Th
+00002070: 6520 7361 7665 6420 6f62 6a20 6973 206e  e saved obj is n
+00002080: 6f74 2061 2054 7261 696e 6572 2063 6865  ot a Trainer che
+00002090: 636b 706f 696e 7429 0b72 6b00 0000 721f  ckpoint).rk...r.
+000020a0: 0000 0072 6c00 0000 726d 0000 0072 0400  ...rl...rm...r..
+000020b0: 0000 da0a 7265 6164 5f62 7974 6573 da0d  ....read_bytes..
+000020c0: 4261 7365 4578 6365 7074 696f 6eda 074f  BaseException..O
+000020d0: 5345 7272 6f72 da05 6c6f 6164 7372 1800  SError..loadsr..
+000020e0: 0000 da09 5479 7065 4572 726f 7229 0572  ....TypeError).r
+000020f0: 6700 0000 726b 0000 00da 065f 6279 7465  g...rk....._byte
+00002100: 73da 0165 da07 7472 6169 6e65 7272 1500  s..e..trainerr..
+00002110: 0000 7215 0000 0072 1600 0000 da13 7265  ..r....r......re
+00002120: 7374 6f72 655f 6672 6f6d 5f70 6963 6b6c  store_from_pickl
+00002130: 6529 0100 0073 1600 0000 000a 0802 0a01  e)...s..........
+00002140: 0a02 0201 0c01 1001 2002 0a02 0a01 0802  ........ .......
+00002150: 7a1b 5472 6169 6e65 722e 7265 7374 6f72  z.Trainer.restor
+00002160: 655f 6672 6f6d 5f70 6963 6b6c 6529 0472  e_from_pickle).r
+00002170: 5900 0000 da07 6d65 7472 6963 7372 0e00  Y.....metricsr..
+00002180: 0000 7239 0000 0063 0400 0000 0000 0000  ..r9...c........
+00002190: 0000 0000 0c00 0000 0800 0000 6300 0000  ............c...
+000021a0: 7398 0000 007c 0364 016b 0872 0e7c 006a  s....|.d.k.r.|.j
+000021b0: 007d 037a 0c74 017c 0283 0101 0057 006e  .}.z.t.|.....W.n
+000021c0: 1a04 0074 026b 0a72 3401 0001 0001 007c  ...t.k.r4......|
+000021d0: 0267 017d 0259 006e 0258 0074 037c 0183  .g.}.Y.n.X.t.|..
+000021e0: 0144 005d 547d 0474 047c 0483 015c 037d  .D.]T}.t.|...\.}
+000021f0: 057d 067d 077c 036a 057d 087c 087c 006a  .}.}.|.j.}.|.|.j
+00002200: 067c 0583 027d 0974 0766 007c 057c 0964  .|...}.t.f.|.|.d
+00002210: 029c 027c 0697 028e 017d 0a7c 0244 005d  ...|.....}.|.D.]
+00002220: 107d 0b7c 0b6a 0866 007c 0a8e 0101 0071  .}.|.j.f.|.....q
+00002230: 7a7c 0256 0001 0071 3e64 0153 0029 0361  z|.V...q>d.S.).a
+00002240: 3703 0000 4372 6561 7465 2074 6573 742f  7...Create test/
+00002250: 7661 6c69 6461 7469 6f6e 2069 7465 7261  validation itera
+00002260: 746f 722e 0a0a 2020 2020 2020 2020 4172  tor...        Ar
+00002270: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00002280: 6461 7461 7365 743a 2041 6e20 6974 6572  dataset: An iter
+00002290: 6174 6f72 206f 7220 6765 6e65 7261 746f  ator or generato
+000022a0: 7220 6675 6e63 7469 6f6e 2074 6f20 7375  r function to su
+000022b0: 7070 6c79 2074 6865 2074 6573 7469 6e67  pply the testing
+000022c0: 2064 6174 612e 0a20 2020 2020 2020 2020   data..         
+000022d0: 2020 2020 2020 2054 6865 2069 7465 7261         The itera
+000022e0: 746f 7220 7368 6f75 6c64 2079 6965 6c64  tor should yield
+000022f0: 2061 2074 7570 706c 6520 6f66 2028 696e   a tupple of (in
+00002300: 7075 7473 2c20 6c61 6265 6c73 292e 2054  puts, labels). T
+00002310: 6865 206c 6162 656c 730a 2020 2020 2020  he labels.      
+00002320: 2020 2020 2020 2020 2020 7368 6f75 6c64            should
+00002330: 2062 6520 6120 6469 6374 2e0a 2020 2020   be a dict..    
+00002340: 2020 2020 2020 2020 6d65 7472 6963 733a          metrics:
+00002350: 2041 206c 6973 7420 6f66 204d 6574 7269   A list of Metri
+00002360: 6320 6f62 6a65 6374 732e 2054 6865 7920  c objects. They 
+00002370: 7368 6f75 6c64 2068 6176 6520 7477 6f20  should have two 
+00002380: 6675 6e63 7469 6f6e 733a 0a20 2020 2020  functions:.     
+00002390: 2020 2020 2020 2020 2020 206d 2e75 7064             m.upd
+000023a0: 6174 6528 7072 6564 732c 202a 2a6b 7761  ate(preds, **kwa
+000023b0: 7267 7329 3a0a 2020 2020 2020 2020 2020  rgs):.          
+000023c0: 2020 2020 2020 2020 2020 7072 6564 7320            preds 
+000023d0: 6973 2074 6865 206d 6f64 656c 206f 7574  is the model out
+000023e0: 7075 742e 2074 6865 2072 656d 6169 6e69  put. the remaini
+000023f0: 6e67 206b 7761 7267 7320 6172 6520 636f  ng kwargs are co
+00002400: 6e74 656e 7420 6f66 0a20 2020 2020 2020  ntent of.       
+00002410: 2020 2020 2020 2020 2020 2020 206c 6162               lab
+00002420: 656c 732e 0a20 2020 2020 2020 2020 2020  els..           
+00002430: 2020 2020 206d 2e63 6f6d 7075 7465 2829       m.compute()
+00002440: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002450: 2020 2020 2020 7768 6963 6820 7368 6f75        which shou
+00002460: 6c64 2072 6574 7572 6e20 7468 6520 6163  ld return the ac
+00002470: 6375 6d75 6c61 7465 6420 6d65 7472 6963  cumulated metric
+00002480: 2076 616c 7565 2e0a 2020 2020 2020 2020   value..        
+00002490: 2020 2020 7374 7261 7465 6779 3a20 4f70      strategy: Op
+000024a0: 7469 6f6e 616c 6c79 206f 7665 7272 6964  tionally overrid
+000024b0: 6520 7468 6520 6465 6661 756c 7420 7374  e the default st
+000024c0: 7261 7465 6779 2e0a 0a20 2020 2020 2020  rategy...       
+000024d0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+000024e0: 2020 2020 2020 416e 2069 7465 7261 746f        An iterato
+000024f0: 722e 2053 7465 7070 696e 6720 7468 726f  r. Stepping thro
+00002500: 7567 6820 6974 2077 696c 6c20 6472 6976  ugh it will driv
+00002510: 6520 7468 6520 7570 6461 7469 6e67 206f  e the updating o
+00002520: 6620 6561 6368 206d 6574 7269 630a 2020  f each metric.  
+00002530: 2020 2020 2020 2020 2020 2020 2020 6f62                ob
+00002540: 6a2e 2054 6865 2069 7465 7261 746f 7220  j. The iterator 
+00002550: 6974 7365 6c66 2072 6574 7572 6e20 7468  itself return th
+00002560: 6520 6c69 7374 206f 6620 6d65 7472 6963  e list of metric
+00002570: 732e 0a20 2020 2020 2020 204e 2902 7248  s..        N).rH
+00002580: 0000 0072 5300 0000 2909 7226 0000 0072  ...rS...).r&...r
+00002590: 1200 0000 7277 0000 0072 1700 0000 723f  ....rw...r....r?
+000025a0: 0000 0072 4e00 0000 7245 0000 00da 0464  ...rN...rE.....d
+000025b0: 6963 74da 0675 7064 6174 6529 0c72 2800  ict..update).r(.
+000025c0: 0000 7259 0000 0072 7c00 0000 720e 0000  ..rY...r|...r...
+000025d0: 0072 4600 0000 7248 0000 0072 6100 0000  .rF...rH...ra...
+000025e0: 7249 0000 0072 5200 0000 7253 0000 0072  rI...rR...rS...r
+000025f0: 5100 0000 da01 6d72 1500 0000 7215 0000  Q.....mr....r...
+00002600: 0072 1600 0000 da04 7465 7374 4401 0000  .r......testD...
+00002610: 7326 0000 0000 1508 0106 0202 010c 010e  s&..............
+00002620: 010c 040c 010e 0106 010c 0104 0102 0102  ................
+00002630: fe04 0302 fd06 0508 010e 027a 0c54 7261  ...........z.Tra
+00002640: 696e 6572 2e74 6573 7463 0100 0000 0000  iner.testc......
+00002650: 0000 0000 0000 0400 0000 0300 0000 4f00  ..............O.
+00002660: 0000 7320 0000 007c 006a 007c 017c 028e  ..s ...|.j.|.|..
+00002670: 0144 005d 047d 0371 0c64 0164 0284 007c  .D.].}.q.d.d...|
+00002680: 0344 0083 0153 0029 037a af41 2063 6f6e  .D...S.).z.A con
+00002690: 7669 656e 7420 6675 6e63 7469 6f6e 2074  vient function t
+000026a0: 6f20 636f 6d70 7574 6520 616c 6c20 6d65  o compute all me
+000026b0: 7472 6963 732e 0a0a 2020 2020 2020 2020  trics...        
+000026c0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+000026d0: 2020 7361 6d65 2061 7320 7468 6520 7465    same as the te
+000026e0: 7374 2829 2066 7563 6e74 696f 6e0a 0a20  st() fucntion.. 
+000026f0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00002700: 2020 2020 2020 2020 2020 2020 4120 6d65              A me
+00002710: 7472 6963 2064 6963 742e 204b 6579 7320  tric dict. Keys 
+00002720: 6172 6520 6d65 7472 6963 206e 616d 6573  are metric names
+00002730: 2e0a 2020 2020 2020 2020 6301 0000 0000  ..        c.....
+00002740: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+00002750: 0000 0073 1a00 0000 6900 7c00 5d12 7d01  ...s....i.|.].}.
+00002760: 7400 7c01 8301 7c01 a001 a100 9302 7104  t.|...|.......q.
+00002770: 5300 7215 0000 0029 0272 0b00 0000 7256  S.r....).r....rV
+00002780: 0000 0029 0272 2c00 0000 727f 0000 0072  ...).r,...r....r
+00002790: 1500 0000 7215 0000 0072 1600 0000 7257  ....r....r....rW
+000027a0: 0000 007c 0100 0073 0600 0000 0600 0200  ...|...s........
+000027b0: 0600 7a2c 5472 6169 6e65 722e 7465 7374  ..z,Trainer.test
+000027c0: 5f61 6e64 5f63 6f6d 7075 7465 2e3c 6c6f  _and_compute.<lo
+000027d0: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
+000027e0: 2901 7280 0000 0029 0472 2800 0000 da04  ).r....).r(.....
+000027f0: 6172 6773 7251 0000 0072 7c00 0000 7215  argsrQ...r|...r.
+00002800: 0000 0072 1500 0000 7216 0000 00da 1074  ...r....r......t
+00002810: 6573 745f 616e 645f 636f 6d70 7574 6571  est_and_computeq
+00002820: 0100 0073 0600 0000 0009 1001 0201 7a18  ...s..........z.
+00002830: 5472 6169 6e65 722e 7465 7374 5f61 6e64  Trainer.test_and
+00002840: 5f63 6f6d 7075 7465 6301 0000 0000 0000  _computec.......
+00002850: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00002860: 0073 0800 0000 7c00 6a00 6a01 5300 7211  .s....|.j.j.S.r.
+00002870: 0000 0029 0272 4500 0000 723a 0000 0072  ...).rE...r:...r
+00002880: 3600 0000 7215 0000 0072 1500 0000 7216  6...r....r....r.
+00002890: 0000 0072 3a00 0000 7e01 0000 7302 0000  ...r:...~...s...
+000028a0: 0000 027a 0e54 7261 696e 6572 2e70 6172  ...z.Trainer.par
+000028b0: 616d 7363 0200 0000 0000 0000 0000 0000  amsc............
+000028c0: 0200 0000 0300 0000 4300 0000 7314 0000  ........C...s...
+000028d0: 007c 006a 006a 017c 0164 018d 017c 005f  .|.j.j.|.d...|._
+000028e0: 0064 0053 0029 024e 2901 723a 0000 0029  .d.S.).N).r:...)
+000028f0: 0272 4500 0000 724f 0000 0029 0272 2800  .rE...rO...).r(.
+00002900: 0000 da0a 6e65 775f 7061 7261 6d73 7215  ....new_paramsr.
+00002910: 0000 0072 1500 0000 7216 0000 0072 3a00  ...r....r....r:.
+00002920: 0000 8201 0000 7302 0000 0000 0263 0100  ......s......c..
+00002930: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00002940: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
+00002950: 0072 1100 0000 2901 7225 0000 0072 3600  .r....).r%...r6.
+00002960: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00002970: 0072 1c00 0000 8601 0000 7302 0000 0000  .r........s.....
+00002980: 027a 1154 7261 696e 6572 2e6f 7074 696d  .z.Trainer.optim
+00002990: 697a 6572 6302 0000 0000 0000 0000 0000  izerc...........
+000029a0: 0002 0000 0005 0000 0043 0000 0073 2800  .........C...s(.
+000029b0: 0000 7c01 7c00 5f00 7c00 6a01 7224 7402  ..|.|._.|.j.r$t.
+000029c0: 6a03 7c00 6a04 6a05 7c00 6a06 7c01 6401  j.|.j.j.|.j.|.d.
+000029d0: 8d03 7c00 5f07 6400 5300 2902 4e72 3b00  ..|._.d.S.).Nr;.
+000029e0: 0000 2908 7225 0000 0072 2700 0000 7207  ..).r%...r'...r.
+000029f0: 0000 0072 4300 0000 721a 0000 0072 4400  ...rC...r....rD.
+00002a00: 0000 723a 0000 0072 4500 0000 2902 7228  ..r:...rE...).r(
+00002a10: 0000 0072 3800 0000 7215 0000 0072 1500  ...r8...r....r..
+00002a20: 0000 7216 0000 0072 1c00 0000 8a01 0000  ..r....r........
+00002a30: 730e 0000 0000 0206 0206 0104 0106 0104  s...............
+00002a40: 0102 fd29 014e 2901 4e29 024e 4e29 014e  ...).N).N).NN).N
+00002a50: 2928 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )(..__name__..__
+00002a60: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00002a70: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
+00002a80: 0e00 0000 da03 4a49 54da 026e 6eda 064d  ......JIT..nn..M
+00002a90: 6f64 756c 65da 084f 7074 696f 6e61 6cda  odule..Optional.
+00002aa0: 064c 4f53 5345 53da 094f 7074 696d 697a  .LOSSES..Optimiz
+00002ab0: 6572 da05 556e 696f 6eda 0369 6e74 da05  er..Union..int..
+00002ac0: 4172 7261 79da 0474 7970 6572 2900 0000  Array..typer)...
+00002ad0: da08 5365 7175 656e 6365 da05 666c 6f61  ..Sequence..floa
+00002ae0: 7472 3500 0000 da08 7072 6f70 6572 7479  tr5.....property
+00002af0: 7237 0000 0072 4c00 0000 da03 416e 7972  r7...rL.....Anyr
+00002b00: 5400 0000 727d 0000 0072 5800 0000 da0a  T...r}...rX.....
+00002b10: 4461 7461 536f 7572 6365 726c 0000 00da  DataSourcerl....
+00002b20: 0849 7465 7261 746f 7272 6600 0000 da08  .Iteratorrf.....
+00002b30: 5061 7468 4c69 6b65 726b 0000 00da 0c73  PathLikerk.....s
+00002b40: 7461 7469 636d 6574 686f 6472 7b00 0000  taticmethodr{...
+00002b50: da08 4361 6c6c 6162 6c65 7280 0000 0072  ..Callabler....r
+00002b60: 8200 0000 723a 0000 00da 0673 6574 7465  ....r:.....sette
+00002b70: 7272 1c00 0000 7215 0000 0072 1500 0000  rr....r....r....
+00002b80: 7215 0000 0072 1600 0000 7218 0000 0023  r....r....r....#
+00002b90: 0000 0073 6400 0000 0801 040f 0201 0201  ...sd...........
+00002ba0: 0201 04fa 0202 0401 0601 0601 0a01 02fa  ................
+00002bb0: 0c22 1821 0201 0a03 1624 02ff 0401 0200  .".!.....$......
+00002bc0: 0601 02fe 0c1c 0e09 0001 00fc 0202 0201  ................
+00002bd0: 0601 0602 02fa 0c5c 1011 0201 101b 00ff  .......\........
+00002be0: 0201 0200 0200 0601 02fe 0c2d 0e0d 0201  ...........-....
+00002bf0: 0a03 0401 0a03 0201 0a03 0401 7218 0000  ............r...
+00002c00: 0029 2372 6d00 0000 da09 6675 6e63 746f  .)#rm.....functo
+00002c10: 6f6c 7372 0200 0000 7203 0000 0072 0400  olsr....r....r..
+00002c20: 0000 da0a 666c 6178 2e6c 696e 656e da05  ....flax.linen..
+00002c30: 6c69 6e65 6e72 8900 0000 7222 0000 00da  linenr....r"....
+00002c40: 096a 6178 2e6e 756d 7079 da05 6e75 6d70  .jax.numpy..nump
+00002c50: 7972 2000 0000 da10 6f72 6261 782e 6368  yr .....orbax.ch
+00002c60: 6563 6b70 6f69 6e74 da05 6f72 6261 78da  eckpoint..orbax.
+00002c70: 1566 6c61 782e 636f 7265 2e66 726f 7a65  .flax.core.froze
+00002c80: 6e5f 6469 6374 7205 0000 0072 0600 0000  n_dictr....r....
+00002c90: da19 666c 6178 2e74 7261 696e 696e 672e  ..flax.training.
+00002ca0: 7472 6169 6e5f 7374 6174 6572 0700 0000  train_stater....
+00002cb0: da0b 6c61 6373 732e 7479 7065 73da 0575  ..lacss.types..u
+00002cc0: 7469 6c73 720a 0000 0072 0b00 0000 da00  tilsr....r......
+00002cd0: 720e 0000 0072 4600 0000 722d 0000 0072  r....rF...r-...r
+00002ce0: 1000 0000 728e 0000 00da 084c 6f73 7346  ....r......LossF
+00002cf0: 756e 6372 9200 0000 728c 0000 0072 5000  uncr....r....rP.
+00002d00: 0000 7217 0000 0072 1800 0000 7215 0000  ..r....r....r...
+00002d10: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
+00002d20: da08 3c6d 6f64 756c 653e 0100 0000 7322  ..<module>....s"
+00002d30: 0000 0008 0110 010c 020c 0108 010c 0108  ................
+00002d40: 0110 010c 0208 0210 010c 0108 010c 0210  ................
+00002d50: 0408 0308 09                             .....
```

### Comparing `lacss-0.4.1/lacss/train/data/__init__.py` & `lacss-0.4.2/lacss/train/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/train/data/__pycache__/__init__.cpython-38.pyc` & `lacss-0.4.2/lacss/train/data/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 718 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 ce02 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 5a80 9c64 ce02 0000  U.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
```

### Comparing `lacss-0.4.1/lacss/train/data/__pycache__/array_adapter.cpython-38.pyc` & `lacss-0.4.2/lacss/train/data/__pycache__/array_adapter.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 4076 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 ec0f 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 5a80 9c64 ec0f 0000  U.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6401 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a07 0100 6400 6401 6c06 5a08 6403  m.Z...d.d.l.Z.d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6403 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6406  m.Z.m.Z.m.Z...d.
```

### Comparing `lacss-0.4.1/lacss/train/data/__pycache__/data_adapter.cpython-38.pyc` & `lacss-0.4.2/lacss/train/data/__pycache__/data_adapter.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 5529 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 9915 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 5a80 9c64 9915 0000  U.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 4700  d.l.Z.d.d.l.Z.G.
 00000040: 6402 6403 8400 6403 6503 6500 6a04 6404  d.d...d.e.e.j.d.
 00000050: 8d04 5a05 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000060: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000070: 0004 0000 0040 0000 0073 9a00 0000 6500  .....@...s....e.
```

### Comparing `lacss-0.4.1/lacss/train/data/__pycache__/data_handler.cpython-38.pyc` & `lacss-0.4.2/lacss/train/data/__pycache__/data_handler.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 6287 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 8f18 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 5a80 9c64 8f18 0000  U.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 e800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 6402 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6402 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6402 6406 6c08 6d09 5a09 0100 7a10  ..d.d.l.m.Z...z.
 00000070: 6402 6407 6c0a 6d0b 5a0b 0100 5700 6e18  d.d.l.m.Z...W.n.
```

### Comparing `lacss-0.4.1/lacss/train/data/__pycache__/dataset.cpython-38.pyc` & `lacss-0.4.2/lacss/train/data/__pycache__/dataset.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 10656 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 a029 0000  U........E.d.)..
+00000000: 550d 0d0a 0000 0000 5a80 9c64 a029 0000  U.......Z..d.)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c06 6d07 5a08 0100 6400 6401 6c07  d.l.m.Z...d.d.l.
 00000060: 5a09 6402 6403 6c0a 6d0b 5a0b 0100 6402  Z.d.d.l.m.Z...d.
 00000070: 6404 6c0c 6d0d 5a0d 0100 6405 6406 6702  d.l.m.Z...d.d.g.
```

### Comparing `lacss-0.4.1/lacss/train/data/__pycache__/generator_adapter.cpython-38.pyc` & `lacss-0.4.2/lacss/train/data/__pycache__/generator_adapter.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 2599 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 270a 0000  U........E.d'...
+00000000: 550d 0d0a 0000 0000 5a80 9c64 270a 0000  U.......Z..d'...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c03 6d04 5a04 0100 6402 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 6504 8303 5a0b 6401 5300 2907 e900 0000  e...Z.d.S.).....
```

### Comparing `lacss-0.4.1/lacss/train/data/__pycache__/list_adapter.cpython-38.pyc` & `lacss-0.4.2/lacss/train/data/__pycache__/list_adapter.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 2105 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 3908 0000  U........E.d9...
+00000000: 550d 0d0a 0000 0000 5a80 9c64 3908 0000  U.......Z..d9...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c04 6d05 5a05 0100 6402 6404 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6508 6509 650a 6603 5a0b  m.Z...e.e.e.f.Z.
 00000060: 4700 6405 6406 8400 6406 6507 8303 5a0c  G.d.d...d.e...Z.
 00000070: 6401 5300 2907 e900 0000 004e e901 0000  d.S.)......N....
```

### Comparing `lacss-0.4.1/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-38.pyc` & `lacss-0.4.2/lacss/train/data/__pycache__/tf_dataset_adapter.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 3440 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 700d 0000  U........E.dp...
+00000000: 550d 0d0a 0000 0000 5a80 9c64 700d 0000  U.......Z..dp...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6403 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
 00000070: 6505 8303 5a0a 6408 5300 2909 e900 0000  e...Z.d.S.).....
```

### Comparing `lacss-0.4.1/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-38.pyc` & `lacss-0.4.2/lacss/train/data/__pycache__/torch_dataloader_adapter.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 2566 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 060a 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 5a80 9c64 060a 0000  U.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6403 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 4700 6406 6407 8400 6407  m.Z...G.d.d...d.
 00000070: 6505 8303 5a0a 6408 5300 2909 e900 0000  e...Z.d.S.).....
```

### Comparing `lacss-0.4.1/lacss/train/data/__pycache__/utils.cpython-38.pyc` & `lacss-0.4.2/lacss/train/data/__pycache__/utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun 22 13:00:43 2023 UTC, .py size: 6394 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 fb45 9464 fa18 0000  U........E.d....
+00000000: 550d 0d0a 0000 0000 5a80 9c64 fa18 0000  U.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ee00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a05 6400 6401 6c06 6d07 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6401 6c07 5a09 6400 6401 6c0a  ..d.d.l.Z.d.d.l.
 00000070: 5a0b 4700 6402 6403 8400 6403 650b 6a0c  Z.G.d.d...d.e.j.
```

### Comparing `lacss-0.4.1/lacss/train/data/array_adapter.py` & `lacss-0.4.2/lacss/train/data/array_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/train/data/data_adapter.py` & `lacss-0.4.2/lacss/train/data/data_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/train/data/data_handler.py` & `lacss-0.4.2/lacss/train/data/data_handler.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/train/data/dataset.py` & `lacss-0.4.2/lacss/train/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/train/data/generator_adapter.py` & `lacss-0.4.2/lacss/train/data/generator_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/train/data/list_adapter.py` & `lacss-0.4.2/lacss/train/data/list_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/train/data/tf_dataset_adapter.py` & `lacss-0.4.2/lacss/train/data/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/train/data/torch_dataloader_adapter.py` & `lacss-0.4.2/lacss/train/data/torch_dataloader_adapter.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/train/data/utils.py` & `lacss-0.4.2/lacss/train/data/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/train/loss.py` & `lacss-0.4.2/lacss/train/loss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.4.1/lacss/train/strategy.py` & `lacss-0.4.2/lacss/train/strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,22 @@
 
         return state, loss_logs, preds
 
 
 class Core(Eager):
     predict = jax.jit(Eager.predict)
 
+    @classmethod
+    def init_fn(cls, key, model, inputs):
+        inputs_obj = Inputs.from_value(inputs)
+
+        state = jax.jit(model.init)(key, *inputs_obj.args, **inputs_obj.kwargs)
+
+        return state
+
 
 class JIT(Core):
     train_step = jax.jit(Core.train_step)
 
 
 class _Distributed(Eager):
     @classmethod
```

### Comparing `lacss-0.4.1/lacss/train/trainer.py` & `lacss-0.4.2/lacss/train/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-import dataclasses
 import pathlib
-import typing as tp
 from functools import lru_cache, partial
+from pathlib import Path
 
-import cloudpickle
 import flax.linen as nn
 import jax
 import jax.numpy as jnp
+import orbax.checkpoint
 from flax.core.frozen_dict import freeze, unfreeze
 from flax.training.train_state import TrainState
-from optax import GradientTransformation
+
+from lacss.types import *
 
 from ..utils import Inputs, _get_name
 from . import strategy
 from .data import *
 from .loss import LossLog
 
+LOSSES = Union[LossFunc, Sequence[LossFunc]]
+
 # so that multiple calls return the same obj
 # this avoids JIT when supplying partial func as args
 _cached_partial = lru_cache(partial)
 
-LOSSES = tp.Union[tp.Callable, tp.Sequence[tp.Callable]]
-
 
 def _get_iterator(g):
     try:
         it = iter(g)
     except:
         it = iter(g())
 
     return it
 
 
 class Trainer:
-    """ FLAX trainer
+    """FLAX trainer
     The design is to be minimal but help avoiding certain biolerplate code when train with FLAX
 
     Attributes:
         model: A Flax module
-        losses: A list of loss function (or other callabels). 
+        losses: A list of loss function (or other callabels).
         optimizer: An optax optimizer
         seed: RNG seed
-        strategy: Training strategy. See lacss.train.strategy module. 
         params: Current model parameters. This is a frozen dict. This is read/write.
         initialized: Whether the model has been initialized with an optimizer and initial weights.
-    
-    Constructor:
-        model: A Flax module
-        losses: A loss function (callabels) or a list of loss functions, or None. Default is None.
-            These should have the call signiture of: 
-                loss = loss_fn(inputs, labels, preds)
-            The "preds" is the model output. The "inputs" and "labels" are from the train dataset.
-            The model trains on the sum of all losses.
-        optimizer: An optax optimzier or None
-        seed: integer RNG seed. Default is 42.
-        strategy: Training strategy. See lacss.train.strategy module. Default is JIT, which trains
-            on a single GPU with unbatched input data. Use VMapped strategy for bathced input. Use
-            Distributed for multi-GPU training. Use Eager for debugging (no JIT). You can supply 
-            your own stategy class.
     """
+
     def __init__(
         self,
         model: nn.Module,
-        losses: tp.Optional[LOSSES] = None,
-        optimizer: GradientTransformation = None,
-        seed: int = 42,
+        losses: Optional[LOSSES] = None,
+        optimizer: Optional[Optimizer] = None,
+        seed: Union[int, Array] = 42,
         strategy: type = strategy.JIT,
     ):
+        """Constructor
+
+        Args:
+            model: A Flax module. It can be a bound module with parameters.
+            losses: A loss function (callabels) or a list of loss functions, or None.
+                These should have the call signiture of:
+                    loss = loss_fn(inputs, labels, preds)
+                The "preds" is the model output. The "inputs" and "labels" are from the train dataset.
+                The model trains on the sum of all losses.
+            optimizer: An optax optimzier
+            seed: RNG seed.
+            strategy: Training backend. See [Traing backends](/api/train/#training-backends).
+
+        """
         self.model = model
         self.losses = losses
         self._loss_weights = None
 
         self.seed = seed if isinstance(seed, jnp.ndarray) else jax.random.PRNGKey(seed)
         self._optimizer = optimizer
 
         self._strategy = strategy
         self._initialized = False
 
         # self.reset()
 
-    def reset(self, loss_weights=None):
-        """ Reset internal loss value tracking
+    def reset(self, loss_weights: Optional[Sequence[float]] = None):
+        """Reset internal loss value tracking
 
         Args:
             loss_weights: Optional weights of individual loss functions. If not None, the
                 total loss is weighted sum.
         """
         if self.losses is None:
             raise ValueError(f"No loss functions provided")
@@ -112,32 +112,30 @@
             LossLog(loss, w) for loss, w in zip(losses, loss_weights)
         )
 
     @property
     def initialized(self):
         return self._initialized
 
-    def initialize(self, dataset, tx: GradientTransformation = None):
-        """ Initialize the model weights and optimizer states.
+    def initialize(self, data, tx: Optional[Optimizer] = None) -> None:
+        """Initialize the model weights and optimizer states.
 
         Args:
-            dataset: An iterator or generator function to supply the training dataset.
-                The dataset should yield (inputs, labels) or inputs. In the latter case
-                the labels = None. The inputs is either a tuple or a dict. If the inputs 
-                is a dict, the keys are interpreted as the names for keyword args of the 
-                model's __call__ function.
-            tx: Optional optax optimzier for when the object was constructed without an 
+            data: An iterator or generator function to produce training dataset. It is not
+                used if model is bound with weights already.
+                see [train()](/api/train#lacss.train.trainer.Trainer.train)
+            tx: Optional optax optimzier for when the object was constructed without an
                 optimizer
         """
         if tx is None:
             tx = self.optimizer
 
         if not self._initialized:
             if self.model.scope is None:
-                peek = next(_get_iterator(dataset))
+                peek = next(_get_iterator(data))
                 inputs, _, _ = unpack_x_y_sample_weight(peek)
 
                 self.seed, key = jax.random.split(self.seed)
                 variables = self._strategy.init_fn(key, self.model, inputs)
 
             else:
                 self.model, variables = self.model.unbind()
@@ -149,23 +147,25 @@
             )
 
         else:
             raise ValueError("Calling initialize() on already initialized Trainer")
 
         self._initialized = True
 
-    def __call__(self, inputs, *, strategy=None, **kwargs):
-        """ Calling the underlying model
+    def __call__(
+        self, inputs: Any, *, strategy: Optional[type] = None, **kwargs
+    ) -> Any:
+        """Calling the underlying model
 
         Args:
             inputs: A tuple or a dict as the inputs for the model.
             strategy: Optionally supply a differnt calling strategy as the default one
                 supplied at the constructor.
             **kwargs: Additional keyword args passed on to the model
-        
+
         Returns:
             Model outputs.
         """
         if strategy is None:
             strategy = self._strategy
 
         predict_fn = strategy.predict
@@ -175,42 +175,53 @@
             state = state.replace(
                 apply_fn=_cached_partial(self.state.apply_fn, **kwargs)
             )
         preds = predict_fn(state, inputs)
 
         return preds
 
-    def compute_loss_log(self):
+    def compute_loss_log(self) -> dict:
         return {
             _get_name(loss_log.loss_fn): loss_log.compute()
             for loss_log in self.loss_logs
         }
 
-    def train(self, dataset, strategy=None, rng_cols=None, **kwargs):
-        """ Create the training iterator
+    def train(
+        self,
+        dataset: DataSource,
+        strategy: Optional[type] = None,
+        rng_cols: Sequence[str] = None,
+        **kwargs,
+    ) -> Iterator:
+        """Create the training iterator
 
         Args:
-            dataset: An iterator or generator function to supply the training dataset.
-                See initialize()
+            dataset: An iterator or generator function to supply the training data.
+                The dataset should yield ```(inputs, labels)``` if the data come with labels or
+                ```(inputs, None)``` if there is no label. The inputs is either a tuple or a
+                dict. If the inputs is a dict, the keys are interpreted as the names for
+                keyword args of the model's __call__ function.
             strategy: Optionally override the default strategy.
-            rng_cols: Names of any RNG used by the model. Should be a list of strs.
+            rng_cols: Names of any RNG used by the model. Should be a list of strings.
             **kwargs: Additional keyward args passed to the model. E.g. "training=True"
-        
+
         Returns:
             A iterator. Stepping through the iterator will train the model. The iterator
                 itself returns a loss log dict, which are mean loss values for each loss
                 function.
-        
-        Usage example:
-            trainer.reset()
+
+        Examples:
+            ```
             train_it = trainer.train(train_dataset, training=True)
             for k in range(train_steps):
                 loss_logs = next(train_it)
                 if k % 1000 == 0:
                     print(loss_logs)
+                    trainer.reset()
+            ```
         """
         if strategy is None:
             strategy = self._strategy
 
         if not self._initialized:
             raise ValueError("Try to run uninitialized trainer")
 
@@ -237,94 +248,100 @@
             )
             self.state = state.replace(apply_fn=self.state.apply_fn)
 
             batch_logs = self.compute_loss_log()
 
             yield batch_logs
 
-    def save_model(self, path, sub_module: tp.Optional[str] = None):
-        """ Save the model in a pickled file. The pickle is a tuple of
-            (module, weights).
-
-        Args:
-            path: The file path.
-            sub_module: Optionally only save a sub_module of the model
-                by specifying the name
-        """
-        module = self.model
-        params = self.params
-
-        if sub_module is not None:
-            module = module.bind(dict(params=params))
-            module = getattr(module, sub_module)
-            module, params = module.unbind()
-            params = params["params"]
-
-        if isinstance(path, str):
-            path = pathlib.Path(path)
+    # def save_model(self, path: _PathLike, sub_module: Optional[str] = None) -> None:
+    #     """Save the model in a pickled file. The pickle is a tuple of
+    #         (module, weights).
+
+    #     Args:
+    #         path: The file path.
+    #         sub_module: Optionally only save a sub_module of the model
+    #             by specifying the name
+    #     """
+    #     module = self.model
+    #     params = self.params
+
+    #     if sub_module is not None:
+    #         module = module.bind(dict(params=params))
+    #         module = getattr(module, sub_module)
+    #         module, params = module.unbind()
+    #         params = params["params"]
+
+    #     if isinstance(path, str):
+    #         path = pathlib.Path(path)
+
+    #     path.parent.mkdir(parents=True, exist_ok=True)
+    #     with open(path, "wb") as f:
+    #         cloudpickle.dump((module, params), f)
 
-        path.parent.mkdir(parents=True, exist_ok=True)
-        with open(path, "wb") as f:
-            cloudpickle.dump((module, params), f)
-
-    def checkpoint(self, path):
-        """ Make a checkpoint of the trainer. This saves the model as well as
+    def pickle(self, path: PathLike) -> None:
+        """Make a pickle save of the trainer. This saves the model as well as
         the training states.
 
         Args:
             path: The file path.
         """
+        import pickle
+
         if isinstance(path, str):
             path = pathlib.Path(path)
 
         path.parent.mkdir(parents=True, exist_ok=True)
 
         with open(path, "wb") as f:
-            cloudpickle.dump(self, f)
+            pickle.dump(self, f)
 
     @staticmethod
-    def from_checkpoint(path):
-        """ Restore from the checkpoint.
+    def restore_from_pickle(path: PathLike):
+        """Restore from the a pickled saved.
 
         Args:
-            path: The checkpoint file path.
+            path: The pickle file path.
 
         Returns:
             A new trainer object.
         """
+        import pickle
+
         if isinstance(path, str):
             path = pathlib.Path(path)
 
         try:
             _bytes = path.read_bytes()
         except BaseException as e:
             raise OSError(f"Could not load the checkpoint. Got exception: {e}")
 
-        trainer = cloudpickle.loads(_bytes)
+        trainer = pickle.loads(_bytes)
 
         if not isinstance(trainer, Trainer):
             raise TypeError("The saved obj is not a Trainer checkpoint")
 
         return trainer
 
-    def test(self, dataset, metrics, strategy=None):
-        """ Create test/validation iterator.
+    def test(
+        self, dataset: DataSource, metrics: Callable, strategy: Optional[type] = None
+    ) -> Iterator:
+        """Create test/validation iterator.
 
         Args:
             dataset: An iterator or generator function to supply the testing data.
                 The iterator should yield a tupple of (inputs, labels). The labels
                 should be a dict.
             metrics: A list of Metric objects. They should have two functions:
                 m.update(preds, **kwargs):
                     preds is the model output. the remaining kwargs are content of
                     labels.
                 m.compute():
                     which should return the accumulated metric value.
             strategy: Optionally override the default strategy.
-        
+
         Returns:
             An iterator. Stepping through it will drive the updating of each metric
                 obj. The iterator itself return the list of metrics.
         """
         if strategy is None:
             strategy = self._strategy
 
@@ -345,20 +362,20 @@
                 **labels,
             )
             for m in metrics:
                 m.update(**kwargs)
 
             yield metrics
 
-    def test_and_compute(self, *args, **kwargs):
-        """ A convient function to compute all metrics.
+    def test_and_compute(self, *args, **kwargs) -> dict:
+        """A convient function to compute all metrics.
 
         Args:
             same as the test() fucntion
-        
+
         Returns:
             A metric dict. Keys are metric names.
         """
         for metrics in self.test(*args, **kwargs):
             pass
         return {_get_name(m): m.compute() for m in metrics}
```

### Comparing `lacss-0.4.1/lacss/utils.py` & `lacss-0.4.2/lacss/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -171,63 +171,78 @@
             for p in loc:
                 c = matplotlib.patches.Circle(
                     (p[1], p[0]), fill=False, edgecolor="white"
                 )
                 axs[k].add_patch(c)
     plt.tight_layout()
 
+
 def masks2label(inputs):
     import jax
-    boxes = inputs['bboxes'].numpy()
+
+    boxes = inputs["bboxes"].numpy()
     boxes = np.round(boxes).astype(int)
-    label = np.zeros(inputs['image'].shape[:2])
-    for k, (m, (y1,x1,y2,x2)) in enumerate(zip(inputs["masks"].numpy(), boxes)):
+    label = np.zeros(inputs["image"].shape[:2])
+    for k, (m, (y1, x1, y2, x2)) in enumerate(zip(inputs["masks"].numpy(), boxes)):
         if y1 > y2:
             y1, y2 = y2, y1
-            m=m[::-1,:]
+            m = m[::-1, :]
         if x1 > x2:
             x1, x2 = x2, x1
-            m = m[:,::-1]
-        patch = jax.image.resize(m, [y2-y1, x2-x1], "linear")
-        label[y1:y2,x1:x2] = np.maximum(
+            m = m[:, ::-1]
+        patch = jax.image.resize(m, [y2 - y1, x2 - x1], "linear")
+        label[y1:y2, x1:x2] = np.maximum(
             (patch >= 0.5).astype(label.dtype) * (k + 1),
-            label[y1:y2,x1:x2],
+            label[y1:y2, x1:x2],
         )
     return label
 
+
 def convert_old_cp(cp):
-    import lacss
     import pickle
     from pathlib import Path
+
     from flax.core.frozen_dict import freeze, unfreeze
 
+    import lacss
+
     cp = Path(cp)
     trainer = lacss.train.Trainer.from_checkpoint(cp)
 
     model = lacss.modules.Lacss(
-        backbone = lacss.modules.ConvNeXt(
-            depths=(3,3,27,3),
+        backbone=lacss.modules.ConvNeXt(
+            depths=(3, 3, 27, 3),
             drop_path_rate=0.4,
             out_channels=256,
         ),
-        lpn = lacss.modules.LPN(
-            conv_spec=((256,256,256,256),()),
+        lpn=lacss.modules.LPN(
+            conv_spec=((256, 256, 256, 256), ()),
         ),
-        detector = lacss.modules.Detector(
+        detector=lacss.modules.Detector(
             train_max_output=2560,
             test_max_output=2560,
         ),
-        segmentor = lacss.modules.Segmentor(
-            conv_spec=((256,256,256),(64,)),
+        segmentor=lacss.modules.Segmentor(
+            conv_spec=((256, 256, 256), (64,)),
             instance_crop_size=96,
         ),
     )
-    
-    params = trainer.params['_lacss']
-    params = freeze(dict(
-        backbone=params['_backbone'],
-        lpn=params['_lpn'],
-        segmentor=params['_segmentor']
-    ))
+
+    params = trainer.params["_lacss"]
+    params = freeze(
+        dict(
+            backbone=params["_backbone"],
+            lpn=params["_lpn"],
+            segmentor=params["_segmentor"],
+        )
+    )
 
     with open(cp.with_suffix(".pkl"), "wb") as f:
-        pickle.dump((model, params), f)
+        pickle.dump((model, params), f)
+
+
+def dataclass_from_dict(klass, dikt):
+    try:
+        fieldtypes = {f.name: f.type for f in dataclasses.fields(klass)}
+        return klass(**{f: dataclass_from_dict(fieldtypes[f], dikt[f]) for f in dikt})
+    except:
+        return dikt
```

### Comparing `lacss-0.4.1/pyproject.toml` & `lacss-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 [tool.poetry]
 name = "lacss"
-version = "0.4.1"
+version = "0.4.2"
 description = "Cell segmentation and tracking"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 flax = ">=0.4.1"
 tqdm = "^4.65.0"
 numpy = ">=1.18.0"
 imageio = "^2.9.0"
 scikit-image = ">=0.19.0"
 cloudpickle = "^2.2.1"
+mkdocs-material = "^9.1.17"
 
 [tool.poetry.group.dev.dependencies]
 jax = "0.4.2"
 jaxlib = "0.4.1+cuda11.cudnn82"
 typer = ">=0.4.0"
 tensorflow-cpu = "^2.8.0"
 setuptools = "67.4.0"
 pycocotools = "^2.0.6"
 pytest = "^7.2.2"
 jupyterlab = "^3.6.1"
 imagecodecs = "^2023.3.16"
 
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.4.3"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
+mkdocs-gen-files = "^0.5.0"
+
 [[tool.poetry.source]]
 name = "jax"
 url = "https://storage.googleapis.com/jax-releases/jax_cuda_releases.html"
 default = false
 secondary = false
 
 [build-system]
```

### Comparing `lacss-0.4.1/PKG-INFO` & `lacss-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: lacss
-Version: 0.4.1
+Version: 0.4.2
 Summary: Cell segmentation and tracking
 License: MIT
 Author: Ji Yu
 Author-email: jyu@uchc.edu
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: flax (>=0.4.1)
 Requires-Dist: imageio (>=2.9.0,<3.0.0)
+Requires-Dist: mkdocs-material (>=9.1.17,<10.0.0)
 Requires-Dist: numpy (>=1.18.0)
 Requires-Dist: scikit-image (>=0.19.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 ## LACSS
```


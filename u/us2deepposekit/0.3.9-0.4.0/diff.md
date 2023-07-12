# Comparing `tmp/us2deepposekit-0.3.9.tar.gz` & `tmp/us2deepposekit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "us2deepposekit-0.3.9.tar", last modified: Sun Jun 13 11:33:37 2021, max compression
+gzip compressed data, was "us2deepposekit-0.4.0.tar", last modified: Wed Jul 12 07:45:09 2023, max compression
```

## Comparing `us2deepposekit-0.3.9.tar` & `us2deepposekit-0.4.0.tar`

### file list

```diff
@@ -1,73 +1,68 @@
-drwxrwxrwx   0        0        0        0 2021-06-13 11:33:37.137297 us2deepposekit-0.3.9/
--rw-rw-rw-   0        0        0    14041 2021-06-13 11:33:37.136297 us2deepposekit-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0    12115 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2021-06-13 11:33:37.058199 us2deepposekit-0.3.9/deepposekit/
--rw-rw-rw-   0        0        0     1139 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-13 11:33:37.061205 us2deepposekit-0.3.9/deepposekit/annotate/
--rw-rw-rw-   0        0        0     5799 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/annotate/KMeansSampler.py
--rw-rw-rw-   0        0        0      863 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/annotate/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-13 11:33:37.067202 us2deepposekit-0.3.9/deepposekit/annotate/gui/
--rw-rw-rw-   0        0        0    11617 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/annotate/gui/Annotator.py
--rw-rw-rw-   0        0        0    22914 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/annotate/gui/GUI.py
--rw-rw-rw-   0        0        0     4508 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/annotate/gui/Skeleton.py
--rw-rw-rw-   0        0        0      799 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/annotate/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-13 11:33:37.071200 us2deepposekit-0.3.9/deepposekit/annotate/utils/
--rw-rw-rw-   0        0        0      683 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/annotate/utils/__init__.py
--rw-rw-rw-   0        0        0     1018 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/annotate/utils/hotkeys.py
--rw-rw-rw-   0        0        0     1092 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/annotate/utils/image.py
-drwxrwxrwx   0        0        0        0 2021-06-13 11:33:37.074199 us2deepposekit-0.3.9/deepposekit/augment/
--rw-rw-rw-   0        0        0     4506 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/augment/FlipAxis.py
--rw-rw-rw-   0        0        0      736 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/augment/__init__.py
--rw-rw-rw-   0        0        0    10248 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/callbacks.py
-drwxrwxrwx   0        0        0        0 2021-06-13 11:33:37.085199 us2deepposekit-0.3.9/deepposekit/io/
--rw-rw-rw-   0        0        0     5695 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/io/BaseGenerator.py
--rw-rw-rw-   0        0        0     3481 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/io/DLCDataGenerator.py
--rw-rw-rw-   0        0        0     6647 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/io/DataGenerator.py
--rw-rw-rw-   0        0        0     2268 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/io/ImageGenerator.py
--rw-rw-rw-   0        0        0    13070 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/io/TrainingGenerator.py
--rw-rw-rw-   0        0        0     1057 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/io/__init__.py
--rw-rw-rw-   0        0        0    11600 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/io/utils.py
--rw-rw-rw-   0        0        0     5485 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/io/video.py
-drwxrwxrwx   0        0        0        0 2021-06-13 11:33:37.098200 us2deepposekit-0.3.9/deepposekit/models/
--rw-rw-rw-   0        0        0     6591 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/DeepLabCut.py
--rw-rw-rw-   0        0        0     8164 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/LEAP.py
--rw-rw-rw-   0        0        0    10698 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/StackedDenseNet.py
--rw-rw-rw-   0        0        0     6720 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/StackedHourglass.py
--rw-rw-rw-   0        0        0     1014 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-13 11:33:37.103202 us2deepposekit-0.3.9/deepposekit/models/backend/
--rw-rw-rw-   0        0        0      683 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/backend/__init__.py
--rw-rw-rw-   0        0        0     9575 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/backend/backend.py
--rw-rw-rw-   0        0        0     7057 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/backend/registration.py
--rw-rw-rw-   0        0        0     2699 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/backend/utils.py
--rw-rw-rw-   0        0        0     9244 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/engine.py
-drwxrwxrwx   0        0        0        0 2021-06-13 11:33:37.123291 us2deepposekit-0.3.9/deepposekit/models/layers/
--rw-rw-rw-   0        0        0      836 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/__init__.py
--rw-rw-rw-   0        0        0    10783 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/convolutional.py
--rw-rw-rw-   0        0        0     6669 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/deeplabcut.py
--rw-rw-rw-   0        0        0    14065 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/densenet.py
--rw-rw-rw-   0        0        0     8724 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/hourglass.py
--rw-rw-rw-   0        0        0    13999 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/imagenet_densenet.py
--rw-rw-rw-   0        0        0    20491 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/imagenet_mobile.py
--rw-rw-rw-   0        0        0    12400 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/imagenet_resnet.py
--rw-rw-rw-   0        0        0    13457 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/imagenet_utils.py
--rw-rw-rw-   0        0        0    13273 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/imagenet_xception.py
--rw-rw-rw-   0        0        0     3317 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/leap.py
--rw-rw-rw-   0        0        0     2256 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/squeeze_excitation.py
--rw-rw-rw-   0        0        0     4355 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/subpixel.py
--rw-rw-rw-   0        0        0     1420 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/layers/util.py
--rw-rw-rw-   0        0        0     4604 2021-06-13 03:13:45.000000 us2deepposekit-0.3.9/deepposekit/models/loading.py
--rw-rw-rw-   0        0        0     1735 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/models/saving.py
-drwxrwxrwx   0        0        0        0 2021-06-13 11:33:37.128292 us2deepposekit-0.3.9/deepposekit/utils/
--rw-rw-rw-   0        0        0      797 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/utils/__init__.py
--rw-rw-rw-   0        0        0     1239 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/utils/image.py
--rw-rw-rw-   0        0        0     1674 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/utils/io.py
--rw-rw-rw-   0        0        0     6633 2021-06-13 03:12:53.000000 us2deepposekit-0.3.9/deepposekit/utils/keypoints.py
--rw-rw-rw-   0        0        0       42 2021-06-13 11:33:37.137297 us2deepposekit-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     2182 2021-06-13 11:31:56.000000 us2deepposekit-0.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-13 11:33:37.135294 us2deepposekit-0.3.9/us2deepposekit.egg-info/
--rw-rw-rw-   0        0        0    14041 2021-06-13 11:33:36.000000 us2deepposekit-0.3.9/us2deepposekit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2032 2021-06-13 11:33:36.000000 us2deepposekit-0.3.9/us2deepposekit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-13 11:33:36.000000 us2deepposekit-0.3.9/us2deepposekit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-06-13 11:31:31.000000 us2deepposekit-0.3.9/us2deepposekit.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       71 2021-06-13 11:33:36.000000 us2deepposekit-0.3.9/us2deepposekit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-06-13 11:33:36.000000 us2deepposekit-0.3.9/us2deepposekit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 07:45:09.184350 us2deepposekit-0.4.0/
+-rw-rw-rw-   0        0        0    11558 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0    12764 2023-07-12 07:45:09.182350 us2deepposekit-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12115 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 07:45:09.079879 us2deepposekit-0.4.0/deepposekit/
+-rw-rw-rw-   0        0        0      964 2023-07-12 07:43:49.000000 us2deepposekit-0.4.0/deepposekit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:45:09.084397 us2deepposekit-0.4.0/deepposekit/annotate/
+-rw-rw-rw-   0        0        0     5799 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/annotate/KMeansSampler.py
+-rw-rw-rw-   0        0        0      749 2023-07-12 07:43:49.000000 us2deepposekit-0.4.0/deepposekit/annotate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:45:09.089073 us2deepposekit-0.4.0/deepposekit/annotate/utils/
+-rw-rw-rw-   0        0        0      683 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/annotate/utils/__init__.py
+-rw-rw-rw-   0        0        0     1018 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/annotate/utils/hotkeys.py
+-rw-rw-rw-   0        0        0     1092 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/annotate/utils/image.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:45:09.093342 us2deepposekit-0.4.0/deepposekit/augment/
+-rw-rw-rw-   0        0        0     4506 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/augment/FlipAxis.py
+-rw-rw-rw-   0        0        0      736 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/augment/__init__.py
+-rw-rw-rw-   0        0        0    10248 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:45:09.107851 us2deepposekit-0.4.0/deepposekit/io/
+-rw-rw-rw-   0        0        0     5695 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/io/BaseGenerator.py
+-rw-rw-rw-   0        0        0     3481 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/io/DLCDataGenerator.py
+-rw-rw-rw-   0        0        0     6647 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/io/DataGenerator.py
+-rw-rw-rw-   0        0        0     2268 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/io/ImageGenerator.py
+-rw-rw-rw-   0        0        0    13070 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/io/TrainingGenerator.py
+-rw-rw-rw-   0        0        0     1021 2023-07-12 07:43:49.000000 us2deepposekit-0.4.0/deepposekit/io/__init__.py
+-rw-rw-rw-   0        0        0    11600 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/io/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:45:09.126877 us2deepposekit-0.4.0/deepposekit/models/
+-rw-rw-rw-   0        0        0     6591 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/DeepLabCut.py
+-rw-rw-rw-   0        0        0     8164 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/LEAP.py
+-rw-rw-rw-   0        0        0    10698 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/StackedDenseNet.py
+-rw-rw-rw-   0        0        0     6720 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/StackedHourglass.py
+-rw-rw-rw-   0        0        0     1014 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:45:09.133892 us2deepposekit-0.4.0/deepposekit/models/backend/
+-rw-rw-rw-   0        0        0      683 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/backend/__init__.py
+-rw-rw-rw-   0        0        0     9575 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/backend/backend.py
+-rw-rw-rw-   0        0        0     7057 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/backend/registration.py
+-rw-rw-rw-   0        0        0     2699 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/backend/utils.py
+-rw-rw-rw-   0        0        0     9244 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/engine.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:45:09.162245 us2deepposekit-0.4.0/deepposekit/models/layers/
+-rw-rw-rw-   0        0        0      836 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/__init__.py
+-rw-rw-rw-   0        0        0    10783 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/convolutional.py
+-rw-rw-rw-   0        0        0     6669 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/deeplabcut.py
+-rw-rw-rw-   0        0        0    14065 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/densenet.py
+-rw-rw-rw-   0        0        0     8724 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/hourglass.py
+-rw-rw-rw-   0        0        0    13999 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/imagenet_densenet.py
+-rw-rw-rw-   0        0        0    20491 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/imagenet_mobile.py
+-rw-rw-rw-   0        0        0    12400 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/imagenet_resnet.py
+-rw-rw-rw-   0        0        0    13457 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/imagenet_utils.py
+-rw-rw-rw-   0        0        0    13273 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/imagenet_xception.py
+-rw-rw-rw-   0        0        0     3317 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/leap.py
+-rw-rw-rw-   0        0        0     2256 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/squeeze_excitation.py
+-rw-rw-rw-   0        0        0     4355 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/subpixel.py
+-rw-rw-rw-   0        0        0     1420 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/layers/util.py
+-rw-rw-rw-   0        0        0     4604 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/loading.py
+-rw-rw-rw-   0        0        0     1735 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/models/saving.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:45:09.168913 us2deepposekit-0.4.0/deepposekit/utils/
+-rw-rw-rw-   0        0        0      797 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/utils/__init__.py
+-rw-rw-rw-   0        0        0     1239 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/utils/image.py
+-rw-rw-rw-   0        0        0     1674 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/utils/io.py
+-rw-rw-rw-   0        0        0     6633 2023-07-12 07:42:58.000000 us2deepposekit-0.4.0/deepposekit/utils/keypoints.py
+-rw-rw-rw-   0        0        0       42 2023-07-12 07:45:09.185353 us2deepposekit-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2187 2023-07-12 07:44:59.000000 us2deepposekit-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:45:09.180345 us2deepposekit-0.4.0/us2deepposekit.egg-info/
+-rw-rw-rw-   0        0        0    12764 2023-07-12 07:45:08.000000 us2deepposekit-0.4.0/us2deepposekit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1872 2023-07-12 07:45:08.000000 us2deepposekit-0.4.0/us2deepposekit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 07:45:08.000000 us2deepposekit-0.4.0/us2deepposekit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-12 07:45:08.000000 us2deepposekit-0.4.0/us2deepposekit.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       80 2023-07-12 07:45:08.000000 us2deepposekit-0.4.0/us2deepposekit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-12 07:45:08.000000 us2deepposekit-0.4.0/us2deepposekit.egg-info/top_level.txt
```

### Comparing `us2deepposekit-0.3.9/PKG-INFO` & `us2deepposekit-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,878 +1,758 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2075 7332  : 2.1..Name: us2
-00000020: 6465 6570 706f 7365 6b69 740d 0a56 6572  deepposekit..Ver
-00000030: 7369 6f6e 3a20 302e 332e 390d 0a53 756d  sion: 0.3.9..Sum
-00000040: 6d61 7279 3a20 6120 746f 6f6c 6b69 7420  mary: a toolkit 
-00000050: 666f 7220 706f 7365 2065 7374 696d 6174  for pose estimat
-00000060: 696f 6e20 7573 696e 6720 6465 6570 206c  ion using deep l
-00000070: 6561 726e 696e 670d 0a48 6f6d 652d 7061  earning..Home-pa
-00000080: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
-00000090: 7562 2e63 6f6d 2f6d 6f72 6269 7465 6368  ub.com/morbitech
-000000a0: 312f 6465 6570 706f 7365 6b69 740d 0a41  1/deepposekit..A
-000000b0: 7574 686f 723a 204a 6163 6f62 2047 7261  uthor: Jacob Gra
-000000c0: 7669 6e67 203c 6a67 7261 7669 6e67 4067  ving <jgraving@g
-000000d0: 6d61 696c 2e63 6f6d 3e0d 0a41 7574 686f  mail.com>..Autho
-000000e0: 722d 656d 6169 6c3a 206a 6772 6176 696e  r-email: jgravin
-000000f0: 6740 676d 6169 6c2e 636f 6d0d 0a4d 6169  g@gmail.com..Mai
-00000100: 6e74 6169 6e65 723a 204a 6163 6f62 2047  ntainer: Jacob G
-00000110: 7261 7669 6e67 203c 6a67 7261 7669 6e67  raving <jgraving
-00000120: 4067 6d61 696c 2e63 6f6d 3e0d 0a4d 6169  @gmail.com>..Mai
-00000130: 6e74 6169 6e65 722d 656d 6169 6c3a 206a  ntainer-email: j
-00000140: 6772 6176 696e 6740 676d 6169 6c2e 636f  graving@gmail.co
-00000150: 6d0d 0a4c 6963 656e 7365 3a20 4170 6163  m..License: Apac
-00000160: 6865 2032 2e30 0d0a 446f 776e 6c6f 6164  he 2.0..Download
-00000170: 2d55 524c 3a20 6874 7470 733a 2f2f 6769  -URL: https://gi
-00000180: 7468 7562 2e63 6f6d 2f6d 6f72 6269 7465  thub.com/morbite
-00000190: 6368 312f 6465 6570 706f 7365 6b69 742e  ch1/deepposekit.
-000001a0: 6769 740d 0a44 6573 6372 6970 7469 6f6e  git..Description
-000001b0: 3a20 3c70 2061 6c69 676e 3d22 6365 6e74  : <p align="cent
-000001c0: 6572 223e 0d0a 2020 2020 2020 2020 3c69  er">..        <i
-000001d0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000001e0: 6769 7468 7562 2e63 6f6d 2f6a 6772 6176  github.com/jgrav
-000001f0: 696e 672f 4465 6570 506f 7365 4b69 742f  ing/DeepPoseKit/
-00000200: 626c 6f62 2f6d 6173 7465 722f 6173 7365  blob/master/asse
-00000210: 7473 2f64 6565 7070 6f73 656b 6974 5f6c  ts/deepposekit_l
-00000220: 6f67 6f2e 706e 6722 2068 6569 6768 743d  ogo.png" height=
-00000230: 2233 3230 7078 223e 0d0a 2020 2020 2020  "320px">..      
-00000240: 2020 3c2f 703e 0d0a 2020 2020 2020 2020    </p>..        
-00000250: 0d0a 2020 2020 2020 2020 2320 596f 7520  ..        # You 
-00000260: 6861 7665 206a 7573 7420 666f 756e 6420  have just found 
-00000270: 4465 6570 506f 7365 4b69 742e 0d0a 2020  DeepPoseKit...  
-00000280: 2020 2020 2020 3c70 2061 6c69 676e 3d22        <p align="
-00000290: 6365 6e74 6572 223e 0d0a 2020 2020 2020  center">..      
-000002a0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-000002b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000002c0: 6772 6176 696e 672f 6a67 7261 7669 6e67  graving/jgraving
-000002d0: 2e67 6974 6875 622e 696f 2f62 6c6f 622f  .github.io/blob/
-000002e0: 6d61 7374 6572 2f66 696c 6573 2f69 6d61  master/files/ima
-000002f0: 6765 732f 4669 6775 7265 3176 6964 656f  ges/Figure1video
-00000300: 312e 6769 6622 2068 6569 6768 743d 2231  1.gif" height="1
-00000310: 3238 7078 223e 0d0a 2020 2020 2020 2020  28px">..        
-00000320: 3c2f 703e 0d0a 2020 2020 2020 2020 0d0a  </p>..        ..
-00000330: 2020 2020 2020 2020 4465 6570 506f 7365          DeepPose
-00000340: 4b69 7420 6973 2061 2073 6f66 7477 6172  Kit is a softwar
-00000350: 6520 746f 6f6c 6b69 7420 7769 7468 2061  e toolkit with a
-00000360: 2068 6967 682d 6c65 7665 6c20 4150 4920   high-level API 
-00000370: 666f 7220 3244 2070 6f73 6520 6573 7469  for 2D pose esti
-00000380: 6d61 7469 6f6e 206f 6620 7573 6572 2d64  mation of user-d
-00000390: 6566 696e 6564 206b 6579 706f 696e 7473  efined keypoints
-000003a0: 2075 7369 6e67 2064 6565 7020 6c65 6172   using deep lear
-000003b0: 6e69 6e67 e280 9477 7269 7474 656e 2069  ning...written i
-000003c0: 6e20 5079 7468 6f6e 2061 6e64 2062 7569  n Python and bui
-000003d0: 6c74 2075 7369 6e67 205b 5465 6e73 6f72  lt using [Tensor
-000003e0: 666c 6f77 5d28 6874 7470 733a 2f2f 6769  flow](https://gi
-000003f0: 7468 7562 2e63 6f6d 2f74 656e 736f 7266  thub.com/tensorf
-00000400: 6c6f 772f 7465 6e73 6f72 666c 6f77 2920  low/tensorflow) 
-00000410: 616e 6420 5b4b 6572 6173 5d28 6874 7470  and [Keras](http
-00000420: 733a 2f2f 7777 772e 7465 6e73 6f72 666c  s://www.tensorfl
-00000430: 6f77 2e6f 7267 2f67 7569 6465 2f6b 6572  ow.org/guide/ker
-00000440: 6173 292e 2055 7365 2044 6565 7050 6f73  as). Use DeepPos
-00000450: 654b 6974 2069 6620 796f 7520 6e65 6564  eKit if you need
-00000460: 3a0d 0a20 2020 2020 2020 200d 0a20 2020  :..        ..   
-00000470: 2020 2020 202d 2074 6f6f 6c73 2066 6f72       - tools for
-00000480: 2061 6e6e 6f74 6174 696e 6720 696d 6167   annotating imag
-00000490: 6573 206f 7220 7669 6465 6f20 6672 616d  es or video fram
-000004a0: 6573 2077 6974 6820 7573 6572 2d64 6566  es with user-def
-000004b0: 696e 6564 206b 6579 706f 696e 7473 0d0a  ined keypoints..
-000004c0: 2020 2020 2020 2020 2d20 6120 7374 7261          - a stra
-000004d0: 6967 6874 666f 7277 6172 6420 6275 7420  ightforward but 
-000004e0: 666c 6578 6962 6c65 2064 6174 6120 6175  flexible data au
-000004f0: 676d 656e 7461 7469 6f6e 2070 6970 656c  gmentation pipel
-00000500: 696e 6520 7573 696e 6720 7468 6520 5b69  ine using the [i
-00000510: 6d67 6175 6720 7061 636b 6167 655d 2868  mgaug package](h
-00000520: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000530: 6d2f 616c 656a 752f 696d 6761 7567 290d  m/aleju/imgaug).
-00000540: 0a20 2020 2020 2020 202d 2061 204b 6572  .        - a Ker
-00000550: 6173 2d62 6173 6564 2069 6e74 6572 6661  as-based interfa
-00000560: 6365 2066 6f72 2069 6e69 7469 616c 697a  ce for initializ
-00000570: 696e 672c 2074 7261 696e 696e 672c 2061  ing, training, a
-00000580: 6e64 2065 7661 6c75 6174 696e 6720 706f  nd evaluating po
-00000590: 7365 2065 7374 696d 6174 696f 6e20 6d6f  se estimation mo
-000005a0: 6465 6c73 0d0a 2020 2020 2020 2020 2d20  dels..        - 
-000005b0: 6561 7379 2d74 6f2d 7573 6520 6d65 7468  easy-to-use meth
-000005c0: 6f64 7320 666f 7220 7361 7669 6e67 2061  ods for saving a
-000005d0: 6e64 206c 6f61 6469 6e67 206d 6f64 656c  nd loading model
-000005e0: 7320 616e 6420 6d61 6b69 6e67 2070 7265  s and making pre
-000005f0: 6469 6374 696f 6e73 206f 6e20 6e65 7720  dictions on new 
-00000600: 6461 7461 0d0a 2020 2020 2020 2020 0d0a  data..        ..
-00000610: 2020 2020 2020 2020 4465 6570 506f 7365          DeepPose
-00000620: 4b69 7420 6973 2064 6573 6967 6e65 6420  Kit is designed 
-00000630: 7769 7468 2061 2066 6f63 7573 206f 6e20  with a focus on 
-00000640: 2a75 7361 6269 6c69 7479 2a20 616e 6420  *usability* and 
-00000650: 2a65 7874 656e 7369 6269 6c69 7479 2a2c  *extensibility*,
-00000660: 2061 7320 6265 696e 6720 6162 6c65 2074   as being able t
-00000670: 6f20 676f 2066 726f 6d20 6964 6561 2074  o go from idea t
-00000680: 6f20 7265 7375 6c74 2077 6974 6820 7468  o result with th
-00000690: 6520 6c65 6173 7420 706f 7373 6962 6c65  e least possible
-000006a0: 2064 656c 6179 2069 7320 6b65 7920 746f   delay is key to
-000006b0: 2064 6f69 6e67 2067 6f6f 6420 7265 7365   doing good rese
-000006c0: 6172 6368 2e0d 0a20 2020 2020 2020 200d  arch...        .
-000006d0: 0a20 2020 2020 2020 2044 6565 7050 6f73  .        DeepPos
-000006e0: 654b 6974 2069 7320 6375 7272 656e 746c  eKit is currentl
-000006f0: 7920 6c69 6d69 7465 6420 746f 202a 696e  y limited to *in
-00000700: 6469 7669 6475 616c 2070 6f73 6520 6573  dividual pose es
-00000710: 7469 6d61 7469 6f6e 2a2e 2049 6620 696e  timation*. If in
-00000720: 6469 7669 6475 616c 7320 6361 6e20 6265  dividuals can be
-00000730: 2065 6173 696c 7920 6469 7374 696e 6775   easily distingu
-00000740: 6973 6865 6420 7669 7375 616c 6c79 2028  ished visually (
-00000750: 692e 652e 2c20 7468 6579 2068 6176 6520  i.e., they have 
-00000760: 6469 6666 6572 656e 746c 7920 636f 6c6f  differently colo
-00000770: 7265 6420 626f 6469 6573 206f 7220 6172  red bodies or ar
-00000780: 6520 6d61 726b 6564 2069 6e20 736f 6d65  e marked in some
-00000790: 2077 6179 292c 2074 6865 6e20 6d75 6c74   way), then mult
-000007a0: 6970 6c65 2069 6e64 6976 6964 7561 6c73  iple individuals
-000007b0: 2063 616e 2073 696d 706c 7920 6265 206c   can simply be l
-000007c0: 6162 656c 6564 2077 6974 6820 7365 7061  abeled with sepa
-000007d0: 7261 7465 206b 6579 706f 696e 7473 2028  rate keypoints (
-000007e0: 6865 6164 312c 2074 6169 6c31 2c20 6865  head1, tail1, he
-000007f0: 6164 322c 2074 6169 6c32 2c20 6574 632e  ad2, tail2, etc.
-00000800: 292e 204f 7468 6572 7769 7365 2044 6565  ). Otherwise Dee
-00000810: 7050 6f73 654b 6974 2063 616e 2062 6520  pPoseKit can be 
-00000820: 6578 7465 6e64 6564 2074 6f20 6d75 6c74  extended to mult
-00000830: 6970 6c65 2069 6e64 6976 6964 7561 6c73  iple individuals
-00000840: 2062 7920 6669 7273 7420 6c6f 6361 6c69   by first locali
-00000850: 7a69 6e67 2c20 7472 6163 6b69 6e67 2c20  zing, tracking, 
-00000860: 616e 6420 6372 6f70 7069 6e67 2069 6e64  and cropping ind
-00000870: 6976 6964 7561 6c73 2077 6974 6820 6164  ividuals with ad
-00000880: 6469 7469 6f6e 616c 2073 6f66 7477 6172  ditional softwar
-00000890: 6520 7375 6368 2061 7320 5b69 6474 7261  e such as [idtra
-000008a0: 636b 6572 2e61 695d 2868 7474 7073 3a2f  cker.ai](https:/
-000008b0: 2f69 6474 7261 636b 6572 2e61 692f 292c  /idtracker.ai/),
-000008c0: 205b 7069 6e70 6f69 6e74 5d28 6874 7470   [pinpoint](http
-000008d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000008e0: 6772 6176 696e 672f 7069 6e70 6f69 6e74  graving/pinpoint
-000008f0: 292c 206f 7220 5b54 7261 636b 746f 725d  ), or [Tracktor]
-00000900: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000910: 636f 6d2f 7669 7665 6b68 7372 6964 6861  com/vivekhsridha
-00000920: 722f 7472 6163 6b74 6f72 292e 0d0a 2020  r/tracktor)...  
-00000930: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000940: 4c6f 6361 6c69 7a61 7469 6f6e 2028 7769  Localization (wi
-00000950: 7468 6f75 7420 7472 6163 6b69 6e67 2920  thout tracking) 
-00000960: 6361 6e20 616c 736f 2062 6520 6163 6869  can also be achi
-00000970: 6576 6564 2077 6974 6820 6465 6570 206c  eved with deep l
-00000980: 6561 726e 696e 6720 736f 6674 7761 7265  earning software
-00000990: 206c 696b 6520 5b6b 6572 6173 2d72 6574   like [keras-ret
-000009a0: 696e 616e 6574 5d28 6874 7470 733a 2f2f  inanet](https://
-000009b0: 6769 7468 7562 2e63 6f6d 2f66 697a 7972  github.com/fizyr
-000009c0: 2f6b 6572 6173 2d72 6574 696e 616e 6574  /keras-retinanet
-000009d0: 292c 2074 6865 205b 5465 6e73 6f72 666c  ), the [Tensorfl
-000009e0: 6f77 204f 626a 6563 7420 4465 7465 6374  ow Object Detect
-000009f0: 696f 6e20 4150 495d 2868 7474 7073 3a2f  ion API](https:/
-00000a00: 2f67 6974 6875 622e 636f 6d2f 7465 6e73  /github.com/tens
-00000a10: 6f72 666c 6f77 2f6d 6f64 656c 732f 7472  orflow/models/tr
-00000a20: 6565 2f6d 6173 7465 722f 7265 7365 6172  ee/master/resear
-00000a30: 6368 2f6f 626a 6563 745f 6465 7465 6374  ch/object_detect
-00000a40: 696f 6e29 2c20 6f72 205b 4d61 7474 6572  ion), or [Matter
-00000a50: 506f 7274 2773 204d 6173 6b20 522d 434e  Port's Mask R-CN
-00000a60: 4e5d 2868 7474 7073 3a2f 2f67 6974 6875  N](https://githu
-00000a70: 622e 636f 6d2f 6d61 7474 6572 706f 7274  b.com/matterport
-00000a80: 2f4d 6173 6b5f 5243 4e4e 292e 0d0a 2020  /Mask_RCNN)...  
-00000a90: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000aa0: 5b43 6865 636b 206f 7574 206f 7572 2070  [Check out our p
-00000ab0: 6170 6572 5d28 6874 7470 733a 2f2f 646f  aper](https://do
-00000ac0: 692e 6f72 672f 3130 2e37 3535 342f 654c  i.org/10.7554/eL
-00000ad0: 6966 652e 3437 3939 3429 2074 6f20 6669  ife.47994) to fi
-00000ae0: 6e64 206f 7574 206d 6f72 652e 0d0a 2020  nd out more...  
-00000af0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000b00: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000b10: 223e 0d0a 2020 2020 2020 2020 3c69 6d67  ">..        <img
-00000b20: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
-00000b30: 7468 7562 2e63 6f6d 2f6a 6772 6176 696e  thub.com/jgravin
-00000b40: 672f 6a67 7261 7669 6e67 2e67 6974 6875  g/jgraving.githu
-00000b50: 622e 696f 2f62 6c6f 622f 6d61 7374 6572  b.io/blob/master
-00000b60: 2f66 696c 6573 2f69 6d61 6765 732f 7a65  /files/images/ze
-00000b70: 6272 612e 6769 6622 2068 6569 6768 743d  bra.gif" height=
-00000b80: 2232 3536 7078 223e 0d0a 2020 2020 2020  "256px">..      
-00000b90: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000ba0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00000bb0: 6772 6176 696e 672f 6a67 7261 7669 6e67  graving/jgraving
-00000bc0: 2e67 6974 6875 622e 696f 2f62 6c6f 622f  .github.io/blob/
-00000bd0: 6d61 7374 6572 2f66 696c 6573 2f69 6d61  master/files/ima
-00000be0: 6765 732f 6c6f 6375 7374 2e67 6966 2220  ges/locust.gif" 
-00000bf0: 6865 6967 6874 3d22 3235 3670 7822 3e0d  height="256px">.
-00000c00: 0a20 2020 2020 2020 203c 2f70 3e0d 0a20  .        </p>.. 
-00000c10: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00000c20: 2023 2048 6f77 2074 6f20 7573 6520 4465   # How to use De
-00000c30: 6570 506f 7365 4b69 740d 0a20 2020 2020  epPoseKit..     
-00000c40: 2020 200d 0a20 2020 2020 2020 2044 6565     ..        Dee
-00000c50: 7050 6f73 654b 6974 2069 7320 6465 7369  pPoseKit is desi
-00000c60: 676e 6564 2066 6f72 2065 6173 7920 7573  gned for easy us
-00000c70: 652e 2046 6f72 2065 7861 6d70 6c65 2c20  e. For example, 
-00000c80: 7472 6169 6e69 6e67 2061 6e64 2073 6176  training and sav
-00000c90: 696e 6720 6120 6d6f 6465 6c20 7265 7175  ing a model requ
-00000ca0: 6972 6573 206f 6e6c 7920 6120 6665 7720  ires only a few 
-00000cb0: 6c69 6e65 7320 6f66 2063 6f64 653a 0d0a  lines of code:..
-00000cc0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-00000cd0: 6e0d 0a20 2020 2020 2020 2066 726f 6d20  n..        from 
-00000ce0: 6465 6570 706f 7365 6b69 742e 696f 2069  deepposekit.io i
-00000cf0: 6d70 6f72 7420 4461 7461 4765 6e65 7261  mport DataGenera
-00000d00: 746f 722c 2054 7261 696e 696e 6747 656e  tor, TrainingGen
-00000d10: 6572 6174 6f72 0d0a 2020 2020 2020 2020  erator..        
-00000d20: 6672 6f6d 2064 6565 7070 6f73 656b 6974  from deepposekit
-00000d30: 2e6d 6f64 656c 7320 696d 706f 7274 2053  .models import S
-00000d40: 7461 636b 6564 4465 6e73 654e 6574 0d0a  tackedDenseNet..
-00000d50: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00000d60: 2020 6461 7461 5f67 656e 6572 6174 6f72    data_generator
-00000d70: 203d 2044 6174 6147 656e 6572 6174 6f72   = DataGenerator
-00000d80: 2827 2f70 6174 682f 746f 2f61 6e6e 6f74  ('/path/to/annot
-00000d90: 6174 696f 6e5f 6461 7461 2e68 3527 290d  ation_data.h5').
-00000da0: 0a20 2020 2020 2020 2074 7261 696e 5f67  .        train_g
-00000db0: 656e 6572 6174 6f72 203d 2054 7261 696e  enerator = Train
-00000dc0: 696e 6747 656e 6572 6174 6f72 2864 6174  ingGenerator(dat
-00000dd0: 615f 6765 6e65 7261 746f 7229 0d0a 2020  a_generator)..  
-00000de0: 2020 2020 2020 6d6f 6465 6c20 3d20 5374        model = St
-00000df0: 6163 6b65 6444 656e 7365 4e65 7428 7472  ackedDenseNet(tr
-00000e00: 6169 6e5f 6765 6e65 7261 746f 7229 0d0a  ain_generator)..
-00000e10: 2020 2020 2020 2020 6d6f 6465 6c2e 6669          model.fi
-00000e20: 7428 6261 7463 685f 7369 7a65 3d31 362c  t(batch_size=16,
-00000e30: 206e 5f77 6f72 6b65 7273 3d38 290d 0a20   n_workers=8).. 
-00000e40: 2020 2020 2020 206d 6f64 656c 2e73 6176         model.sav
-00000e50: 6528 272f 7061 7468 2f74 6f2f 7361 7665  e('/path/to/save
-00000e60: 645f 6d6f 6465 6c2e 6835 2729 0d0a 2020  d_model.h5')..  
-00000e70: 2020 2020 2020 6060 600d 0a20 2020 2020        ```..     
-00000e80: 2020 204c 6f61 6469 6e67 2061 2074 7261     Loading a tra
-00000e90: 696e 6564 206d 6f64 656c 2061 6e64 2072  ined model and r
-00000ea0: 756e 6e69 6e67 2070 7265 6469 6374 696f  unning predictio
-00000eb0: 6e73 206f 6e20 6e65 7720 6461 7461 2069  ns on new data i
-00000ec0: 7320 616c 736f 2073 7472 6169 6768 7466  s also straightf
-00000ed0: 6f72 7761 7264 2e20 466f 7220 6578 616d  orward. For exam
-00000ee0: 706c 652c 2072 756e 6e69 6e67 2070 7265  ple, running pre
-00000ef0: 6469 6374 696f 6e73 206f 6e20 6120 6e65  dictions on a ne
-00000f00: 7720 7669 6465 6f3a 0d0a 2020 2020 2020  w video:..      
-00000f10: 2020 6060 6070 7974 686f 6e0d 0a20 2020    ```python..   
-00000f20: 2020 2020 2066 726f 6d20 6465 6570 706f       from deeppo
-00000f30: 7365 6b69 742e 6d6f 6465 6c73 2069 6d70  sekit.models imp
-00000f40: 6f72 7420 6c6f 6164 5f6d 6f64 656c 0d0a  ort load_model..
-00000f50: 2020 2020 2020 2020 6672 6f6d 2064 6565          from dee
-00000f60: 7070 6f73 656b 6974 2e69 6f20 696d 706f  pposekit.io impo
-00000f70: 7274 2056 6964 656f 5265 6164 6572 0d0a  rt VideoReader..
-00000f80: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00000f90: 2020 6d6f 6465 6c20 3d20 6c6f 6164 5f6d    model = load_m
-00000fa0: 6f64 656c 2827 2f70 6174 682f 746f 2f73  odel('/path/to/s
-00000fb0: 6176 6564 5f6d 6f64 656c 2e68 3527 290d  aved_model.h5').
-00000fc0: 0a20 2020 2020 2020 2072 6561 6465 7220  .        reader 
-00000fd0: 3d20 5669 6465 6f52 6561 6465 7228 272f  = VideoReader('/
-00000fe0: 7061 7468 2f74 6f2f 7669 6465 6f2e 6d70  path/to/video.mp
-00000ff0: 3427 290d 0a20 2020 2020 2020 2070 7265  4')..        pre
-00001000: 6469 6374 696f 6e73 203d 206d 6f64 656c  dictions = model
-00001010: 2e70 7265 6469 6374 2872 6561 6465 7229  .predict(reader)
-00001020: 0d0a 2020 2020 2020 2020 6060 600d 0a20  ..        ```.. 
-00001030: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00001040: 2023 2320 5573 696e 6720 4465 6570 506f   ## Using DeepPo
-00001050: 7365 4b69 7420 6973 2061 2034 2d73 7465  seKit is a 4-ste
-00001060: 7020 7072 6f63 6573 733a 0d0a 2020 2020  p process:..    
-00001070: 2020 2020 0d0a 2020 2020 2020 2020 2d20      ..        - 
-00001080: 2a2a 312e 2a2a 205b 4372 6561 7465 2061  **1.** [Create a
-00001090: 6e20 616e 6e6f 7461 7469 6f6e 2073 6574  n annotation set
-000010a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000010b0: 2e63 6f6d 2f6a 6772 6176 696e 672f 4465  .com/jgraving/De
-000010c0: 6570 506f 7365 4b69 742f 626c 6f62 2f6d  epPoseKit/blob/m
-000010d0: 6173 7465 722f 6578 616d 706c 6573 2f73  aster/examples/s
-000010e0: 7465 7031 5f63 7265 6174 655f 616e 6e6f  tep1_create_anno
-000010f0: 7461 7469 6f6e 5f73 6574 2e69 7079 6e62  tation_set.ipynb
-00001100: 2920 3c61 2068 7265 663d 2268 7474 7073  ) <a href="https
-00001110: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-00001120: 682e 676f 6f67 6c65 2e63 6f6d 2f67 6974  h.google.com/git
-00001130: 6875 622f 6a67 7261 7669 6e67 2f64 6565  hub/jgraving/dee
-00001140: 7070 6f73 656b 6974 2f62 6c6f 622f 6d61  pposekit/blob/ma
-00001150: 7374 6572 2f65 7861 6d70 6c65 732f 7374  ster/examples/st
-00001160: 6570 315f 6372 6561 7465 5f61 6e6e 6f74  ep1_create_annot
-00001170: 6174 696f 6e5f 7365 742e 6970 796e 6222  ation_set.ipynb"
-00001180: 2074 6172 6765 743d 225f 7061 7265 6e74   target="_parent
-00001190: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
-000011a0: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
-000011b0: 6368 2e67 6f6f 676c 652e 636f 6d2f 6173  ch.google.com/as
-000011c0: 7365 7473 2f63 6f6c 6162 2d62 6164 6765  sets/colab-badge
-000011d0: 2e73 7667 2220 616c 743d 224f 7065 6e20  .svg" alt="Open 
-000011e0: 496e 2043 6f6c 6162 222f 3e3c 2f61 3e0d  In Colab"/></a>.
-000011f0: 0a20 2020 2020 2020 202d 202a 2a32 2e2a  .        - **2.*
-00001200: 2a20 5b41 6e6e 6f74 6174 6520 796f 7572  * [Annotate your
-00001210: 2064 6174 615d 2868 7474 7073 3a2f 2f67   data](https://g
-00001220: 6974 6875 622e 636f 6d2f 6a67 7261 7669  ithub.com/jgravi
-00001230: 6e67 2f44 6565 7050 6f73 654b 6974 2f62  ng/DeepPoseKit/b
-00001240: 6c6f 622f 6d61 7374 6572 2f65 7861 6d70  lob/master/examp
-00001250: 6c65 732f 7374 6570 325f 616e 6e6f 7461  les/step2_annota
-00001260: 7465 5f64 6174 612e 6970 796e 6229 2077  te_data.ipynb) w
-00001270: 6974 6820 6f75 7220 6275 696c 742d 696e  ith our built-in
-00001280: 2047 5549 2028 6e6f 2043 6f6c 6162 2073   GUI (no Colab s
-00001290: 7570 706f 7274 290d 0a20 2020 2020 2020  upport)..       
-000012a0: 202d 202a 2a33 2e2a 2a20 5b53 656c 6563   - **3.** [Selec
-000012b0: 7420 616e 6420 7472 6169 6e5d 2868 7474  t and train](htt
-000012c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000012d0: 6a67 7261 7669 6e67 2f44 6565 7050 6f73  jgraving/DeepPos
-000012e0: 654b 6974 2f62 6c6f 622f 6d61 7374 6572  eKit/blob/master
-000012f0: 2f65 7861 6d70 6c65 732f 7374 6570 335f  /examples/step3_
-00001300: 7472 6169 6e5f 6d6f 6465 6c2e 6970 796e  train_model.ipyn
-00001310: 6229 206f 6e65 206f 7572 205b 706f 7365  b) one our [pose
-00001320: 2065 7374 696d 6174 696f 6e20 6d6f 6465   estimation mode
-00001330: 6c73 5d28 6874 7470 3a2f 2f6a 616b 6567  ls](http://jakeg
-00001340: 7261 7669 6e67 2e63 6f6d 2f44 6565 7050  raving.com/DeepP
-00001350: 6f73 654b 6974 2f68 746d 6c2f 6465 6570  oseKit/html/deep
-00001360: 706f 7365 6b69 742f 6d6f 6465 6c73 2f69  posekit/models/i
-00001370: 6e64 6578 2e68 746d 6c29 2069 6e63 6c75  ndex.html) inclu
-00001380: 6469 6e67 205b 6053 7461 636b 6564 4465  ding [`StackedDe
-00001390: 6e73 654e 6574 605d 2868 7474 703a 2f2f  nseNet`](http://
-000013a0: 6a61 6b65 6772 6176 696e 672e 636f 6d2f  jakegraving.com/
-000013b0: 4465 6570 506f 7365 4b69 742f 6874 6d6c  DeepPoseKit/html
-000013c0: 2f64 6565 7070 6f73 656b 6974 2f6d 6f64  /deepposekit/mod
-000013d0: 656c 732f 5374 6163 6b65 6444 656e 7365  els/StackedDense
-000013e0: 4e65 742e 6874 6d6c 292c 205b 6053 7461  Net.html), [`Sta
-000013f0: 636b 6564 486f 7572 676c 6173 7360 5d28  ckedHourglass`](
-00001400: 6874 7470 3a2f 2f6a 616b 6567 7261 7669  http://jakegravi
-00001410: 6e67 2e63 6f6d 2f44 6565 7050 6f73 654b  ng.com/DeepPoseK
-00001420: 6974 2f68 746d 6c2f 6465 6570 706f 7365  it/html/deeppose
-00001430: 6b69 742f 6d6f 6465 6c73 2f53 7461 636b  kit/models/Stack
-00001440: 6564 486f 7572 676c 6173 732e 6874 6d6c  edHourglass.html
-00001450: 292c 205b 6044 6565 704c 6162 4375 7460  ), [`DeepLabCut`
-00001460: 5d28 6874 7470 3a2f 2f6a 616b 6567 7261  ](http://jakegra
-00001470: 7669 6e67 2e63 6f6d 2f44 6565 7050 6f73  ving.com/DeepPos
-00001480: 654b 6974 2f68 746d 6c2f 6465 6570 706f  eKit/html/deeppo
-00001490: 7365 6b69 742f 6d6f 6465 6c73 2f44 6565  sekit/models/Dee
-000014a0: 704c 6162 4375 742e 6874 6d6c 292c 2061  pLabCut.html), a
-000014b0: 6e64 205b 604c 4541 5060 5d28 6874 7470  nd [`LEAP`](http
-000014c0: 3a2f 2f6a 616b 6567 7261 7669 6e67 2e63  ://jakegraving.c
-000014d0: 6f6d 2f44 6565 7050 6f73 654b 6974 2f68  om/DeepPoseKit/h
-000014e0: 746d 6c2f 6465 6570 706f 7365 6b69 742f  tml/deepposekit/
-000014f0: 6d6f 6465 6c73 2f4c 4541 502e 6874 6d6c  models/LEAP.html
-00001500: 292e 203c 6120 6872 6566 3d22 6874 7470  ). <a href="http
-00001510: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
-00001520: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
-00001530: 7468 7562 2f6a 6772 6176 696e 672f 6465  thub/jgraving/de
-00001540: 6570 706f 7365 6b69 742f 626c 6f62 2f6d  epposekit/blob/m
-00001550: 6173 7465 722f 6578 616d 706c 6573 2f73  aster/examples/s
-00001560: 7465 7033 5f74 7261 696e 5f6d 6f64 656c  tep3_train_model
-00001570: 2e69 7079 6e62 2220 7461 7267 6574 3d22  .ipynb" target="
-00001580: 5f70 6172 656e 7422 3e3c 696d 6720 7372  _parent"><img sr
-00001590: 633d 2268 7474 7073 3a2f 2f63 6f6c 6162  c="https://colab
-000015a0: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
-000015b0: 2e63 6f6d 2f61 7373 6574 732f 636f 6c61  .com/assets/cola
-000015c0: 622d 6261 6467 652e 7376 6722 2061 6c74  b-badge.svg" alt
-000015d0: 3d22 4f70 656e 2049 6e20 436f 6c61 6222  ="Open In Colab"
-000015e0: 2f3e 3c2f 613e 0d0a 2020 2020 2020 2020  /></a>..        
-000015f0: 2d20 2a2a 342e 2a2a 2055 7365 2074 6865  - **4.** Use the
-00001600: 2074 7261 696e 6564 206d 6f64 656c 2074   trained model t
-00001610: 6f3a 0d0a 2020 2020 2020 2020 092d 2061  o:..        .- a
-00001620: 2920 5b49 6e69 7469 616c 697a 6520 6b65  ) [Initialize ke
-00001630: 7970 6f69 6e74 7320 666f 7220 756e 616e  ypoints for unan
-00001640: 6e6f 7461 7465 6420 6461 7461 5d28 6874  notated data](ht
-00001650: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001660: 2f6a 6772 6176 696e 672f 4465 6570 506f  /jgraving/DeepPo
-00001670: 7365 4b69 742f 626c 6f62 2f6d 6173 7465  seKit/blob/maste
-00001680: 722f 6578 616d 706c 6573 2f73 7465 7034  r/examples/step4
-00001690: 615f 696e 6974 6961 6c69 7a65 5f61 6e6e  a_initialize_ann
-000016a0: 6f74 6174 696f 6e73 2e69 7079 6e62 2920  otations.ipynb) 
-000016b0: 666f 7220 6661 7374 6572 2061 6e6e 6f74  for faster annot
-000016c0: 6174 696f 6e73 2077 6974 6820 2a61 6374  ations with *act
-000016d0: 6976 6520 6c65 6172 6e69 6e67 2a2e 203c  ive learning*. <
-000016e0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000016f0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-00001700: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
-00001710: 2f6a 6772 6176 696e 672f 6465 6570 706f  /jgraving/deeppo
-00001720: 7365 6b69 742f 626c 6f62 2f6d 6173 7465  sekit/blob/maste
-00001730: 722f 6578 616d 706c 6573 2f73 7465 7034  r/examples/step4
-00001740: 615f 696e 6974 6961 6c69 7a65 5f61 6e6e  a_initialize_ann
-00001750: 6f74 6174 696f 6e73 2e69 7079 6e62 2220  otations.ipynb" 
-00001760: 7461 7267 6574 3d22 5f70 6172 656e 7422  target="_parent"
-00001770: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00001780: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-00001790: 682e 676f 6f67 6c65 2e63 6f6d 2f61 7373  h.google.com/ass
-000017a0: 6574 732f 636f 6c61 622d 6261 6467 652e  ets/colab-badge.
-000017b0: 7376 6722 2061 6c74 3d22 4f70 656e 2049  svg" alt="Open I
-000017c0: 6e20 436f 6c61 6222 2f3e 3c2f 613e 0d0a  n Colab"/></a>..
-000017d0: 2020 2020 2020 2020 092d 2062 2920 5b50          .- b) [P
-000017e0: 7265 6469 6374 206f 6e20 6e65 7720 6461  redict on new da
-000017f0: 7461 2061 6e64 2072 6566 696e 6520 7468  ta and refine th
-00001800: 6520 7472 6169 6e69 6e67 2073 6574 5d28  e training set](
-00001810: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001820: 6f6d 2f6a 6772 6176 696e 672f 4465 6570  om/jgraving/Deep
-00001830: 506f 7365 4b69 742f 626c 6f62 2f6d 6173  PoseKit/blob/mas
-00001840: 7465 722f 6578 616d 706c 6573 2f73 7465  ter/examples/ste
-00001850: 7034 625f 7072 6564 6963 745f 6e65 775f  p4b_predict_new_
-00001860: 6461 7461 2e69 7079 6e62 2920 746f 2069  data.ipynb) to i
-00001870: 6d70 726f 7665 2070 6572 666f 726d 616e  mprove performan
-00001880: 6365 2e20 3c61 2068 7265 663d 2268 7474  ce. <a href="htt
-00001890: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
-000018a0: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f67  rch.google.com/g
-000018b0: 6974 6875 622f 6a67 7261 7669 6e67 2f64  ithub/jgraving/d
-000018c0: 6565 7070 6f73 656b 6974 2f62 6c6f 622f  eepposekit/blob/
-000018d0: 6d61 7374 6572 2f65 7861 6d70 6c65 732f  master/examples/
-000018e0: 7374 6570 3462 5f70 7265 6469 6374 5f6e  step4b_predict_n
-000018f0: 6577 5f64 6174 612e 6970 796e 6222 2074  ew_data.ipynb" t
-00001900: 6172 6765 743d 225f 7061 7265 6e74 223e  arget="_parent">
-00001910: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001920: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-00001930: 2e67 6f6f 676c 652e 636f 6d2f 6173 7365  .google.com/asse
-00001940: 7473 2f63 6f6c 6162 2d62 6164 6765 2e73  ts/colab-badge.s
-00001950: 7667 2220 616c 743d 224f 7065 6e20 496e  vg" alt="Open In
-00001960: 2043 6f6c 6162 222f 3e3c 2f61 3e0d 0a20   Colab"/></a>.. 
-00001970: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00001980: 2023 2320 466f 7220 6d6f 7265 2064 6574   ## For more det
-00001990: 6169 6c73 3a0d 0a20 2020 2020 2020 200d  ails:..        .
-000019a0: 0a20 2020 2020 2020 202d 2053 6565 205b  .        - See [
-000019b0: 6f75 7220 6578 616d 706c 6520 6e6f 7465  our example note
-000019c0: 626f 6f6b 735d 2868 7474 7073 3a2f 2f67  books](https://g
-000019d0: 6974 6875 622e 636f 6d2f 6a67 7261 7669  ithub.com/jgravi
-000019e0: 6e67 2f64 6565 7070 6f73 656b 6974 2f62  ng/deepposekit/b
-000019f0: 6c6f 622f 6d61 7374 6572 2f65 7861 6d70  lob/master/examp
-00001a00: 6c65 732f 290d 0a20 2020 2020 2020 202d  les/)..        -
-00001a10: 2043 6865 636b 2074 6865 205b 646f 6375   Check the [docu
-00001a20: 6d65 6e74 6174 696f 6e5d 2868 7474 703a  mentation](http:
-00001a30: 2f2f 646f 6373 2e64 6565 7070 6f73 656b  //docs.deepposek
-00001a40: 6974 2e6f 7267 290d 0a20 2020 2020 2020  it.org)..       
-00001a50: 202d 2052 6561 6420 5b6f 7572 2070 6170   - Read [our pap
-00001a60: 6572 5d28 6874 7470 733a 2f2f 646f 692e  er](https://doi.
-00001a70: 6f72 672f 3130 2e37 3535 342f 654c 6966  org/10.7554/eLif
-00001a80: 652e 3437 3939 3429 0d0a 2020 2020 2020  e.47994)..      
-00001a90: 2020 0d0a 2020 2020 2020 2020 2323 2022    ..        ## "
-00001aa0: 4920 616c 7265 6164 7920 6861 7665 2061  I already have a
-00001ab0: 6e6e 6f74 6174 6564 2064 6174 6122 0d0a  nnotated data"..
-00001ac0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00001ad0: 2020 4465 6570 506f 7365 4b69 7420 6973    DeepPoseKit is
-00001ae0: 2064 6573 6967 6e65 6420 746f 2062 6520   designed to be 
-00001af0: 6578 7465 6e73 6962 6c65 2c20 736f 206c  extensible, so l
-00001b00: 6f61 6469 6e67 2064 6174 6120 696e 206f  oading data in o
-00001b10: 7468 6572 2066 6f72 6d61 7473 2069 7320  ther formats is 
-00001b20: 706f 7373 6962 6c65 2e0d 0a20 2020 2020  possible...     
-00001b30: 2020 200d 0a20 2020 2020 2020 2049 6620     ..        If 
-00001b40: 796f 7520 6861 7665 2061 6e6e 6f74 6174  you have annotat
-00001b50: 6564 2064 6174 6120 6672 6f6d 2044 6565  ed data from Dee
-00001b60: 704c 6162 4375 7420 2868 7474 703a 2f2f  pLabCut (http://
-00001b70: 6465 6570 6c61 6263 7574 2e6f 7267 292c  deeplabcut.org),
-00001b80: 2074 7279 205b 6f75 7220 2865 7870 6572   try [our (exper
-00001b90: 696d 656e 7461 6c29 2065 7861 6d70 6c65  imental) example
-00001ba0: 206e 6f74 6562 6f6f 6b20 5d28 6874 7470   notebook ](http
-00001bb0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00001bc0: 6772 6176 696e 672f 4465 6570 506f 7365  graving/DeepPose
-00001bd0: 4b69 742f 626c 6f62 2f6d 6173 7465 722f  Kit/blob/master/
-00001be0: 6578 616d 706c 6573 2f64 6565 706c 6162  examples/deeplab
-00001bf0: 6375 745f 6461 7461 5f65 7861 6d70 6c65  cut_data_example
-00001c00: 2e69 7079 6e62 2920 666f 7220 6c6f 6164  .ipynb) for load
-00001c10: 696e 6720 6461 7461 2069 6e20 7468 6973  ing data in this
-00001c20: 2066 6f72 6d61 742e 203c 6120 6872 6566   format. <a href
-00001c30: 3d22 6874 7470 733a 2f2f 636f 6c61 622e  ="https://colab.
-00001c40: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
-00001c50: 636f 6d2f 6769 7468 7562 2f6a 6772 6176  com/github/jgrav
-00001c60: 696e 672f 6465 6570 706f 7365 6b69 742f  ing/deepposekit/
-00001c70: 626c 6f62 2f6d 6173 7465 722f 6578 616d  blob/master/exam
-00001c80: 706c 6573 2f64 6565 706c 6162 6375 745f  ples/deeplabcut_
-00001c90: 6461 7461 5f65 7861 6d70 6c65 2e69 7079  data_example.ipy
-00001ca0: 6e62 2220 7461 7267 6574 3d22 5f70 6172  nb" target="_par
-00001cb0: 656e 7422 3e3c 696d 6720 7372 633d 2268  ent"><img src="h
-00001cc0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-00001cd0: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00001ce0: 2f61 7373 6574 732f 636f 6c61 622d 6261  /assets/colab-ba
-00001cf0: 6467 652e 7376 6722 2061 6c74 3d22 4f70  dge.svg" alt="Op
-00001d00: 656e 2049 6e20 436f 6c61 6222 2f3e 3c2f  en In Colab"/></
-00001d10: 613e 0d0a 2020 2020 2020 2020 0d0a 2020  a>..        ..  
-00001d20: 2020 2020 2020 4861 7665 2064 6174 6120        Have data 
-00001d30: 696e 2061 6e6f 7468 6572 2066 6f72 6d61  in another forma
-00001d40: 743f 2059 6f75 2063 616e 2077 7269 7465  t? You can write
-00001d50: 2079 6f75 7220 6f77 6e20 6375 7374 6f6d   your own custom
-00001d60: 2067 656e 6572 6174 6f72 2074 6f20 6c6f   generator to lo
-00001d70: 6164 2069 742e 0d0a 2020 2020 2020 2020  ad it...        
-00001d80: 4368 6563 6b20 6f75 7420 7468 6520 5b65  Check out the [e
-00001d90: 7861 6d70 6c65 2066 6f72 2077 7269 7469  xample for writi
-00001da0: 6e67 2063 7573 746f 6d20 6461 7461 2067  ng custom data g
-00001db0: 656e 6572 6174 6f72 735d 2868 7474 7073  enerators](https
-00001dc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a67  ://github.com/jg
-00001dd0: 7261 7669 6e67 2f44 6565 7050 6f73 654b  raving/DeepPoseK
-00001de0: 6974 2f62 6c6f 622f 6d61 7374 6572 2f65  it/blob/master/e
-00001df0: 7861 6d70 6c65 732f 6375 7374 6f6d 5f64  xamples/custom_d
-00001e00: 6174 615f 6765 6e65 7261 746f 722e 6970  ata_generator.ip
-00001e10: 796e 6229 2e20 3c61 2068 7265 663d 2268  ynb). <a href="h
-00001e20: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-00001e30: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00001e40: 2f67 6974 6875 622f 6a67 7261 7669 6e67  /github/jgraving
-00001e50: 2f64 6565 7070 6f73 656b 6974 2f62 6c6f  /deepposekit/blo
-00001e60: 622f 6d61 7374 6572 2f65 7861 6d70 6c65  b/master/example
-00001e70: 732f 6375 7374 6f6d 5f64 6174 615f 6765  s/custom_data_ge
-00001e80: 6e65 7261 746f 722e 6970 796e 6222 2074  nerator.ipynb" t
-00001e90: 6172 6765 743d 225f 7061 7265 6e74 223e  arget="_parent">
-00001ea0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001eb0: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-00001ec0: 2e67 6f6f 676c 652e 636f 6d2f 6173 7365  .google.com/asse
-00001ed0: 7473 2f63 6f6c 6162 2d62 6164 6765 2e73  ts/colab-badge.s
-00001ee0: 7667 2220 616c 743d 224f 7065 6e20 496e  vg" alt="Open In
-00001ef0: 2043 6f6c 6162 222f 3e3c 2f61 3e0d 0a20   Colab"/></a>.. 
-00001f00: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00001f10: 2023 2049 6e73 7461 6c6c 6174 696f 6e0d   # Installation.
-00001f20: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00001f30: 2020 2044 6565 7050 6f73 654b 6974 2072     DeepPoseKit r
-00001f40: 6571 7569 7265 7320 5b54 656e 736f 7266  equires [Tensorf
-00001f50: 6c6f 775d 2868 7474 7073 3a2f 2f67 6974  low](https://git
-00001f60: 6875 622e 636f 6d2f 7465 6e73 6f72 666c  hub.com/tensorfl
-00001f70: 6f77 2f74 656e 736f 7266 6c6f 7729 2066  ow/tensorflow) f
-00001f80: 6f72 2074 7261 696e 696e 6720 616e 6420  or training and 
-00001f90: 7573 696e 6720 706f 7365 2065 7374 696d  using pose estim
-00001fa0: 6174 696f 6e20 6d6f 6465 6c73 2e20 5b54  ation models. [T
-00001fb0: 656e 736f 7266 6c6f 775d 2868 7474 7073  ensorflow](https
-00001fc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7465  ://github.com/te
-00001fd0: 6e73 6f72 666c 6f77 2f74 656e 736f 7266  nsorflow/tensorf
-00001fe0: 6c6f 7729 2073 686f 756c 6420 6265 206d  low) should be m
-00001ff0: 616e 7561 6c6c 7920 696e 7374 616c 6c65  anually installe
-00002000: 642c 2061 6c6f 6e67 2077 6974 6820 6465  d, along with de
-00002010: 7065 6e64 656e 6369 6573 2073 7563 6820  pendencies such 
-00002020: 6173 2043 5544 4120 616e 6420 6375 444e  as CUDA and cuDN
-00002030: 4e2c 2062 6566 6f72 6520 696e 7374 616c  N, before instal
-00002040: 6c69 6e67 2044 6565 7050 6f73 654b 6974  ling DeepPoseKit
-00002050: 3a0d 0a20 2020 2020 2020 200d 0a20 2020  :..        ..   
-00002060: 2020 2020 202d 205b 5465 6e73 6f72 666c       - [Tensorfl
-00002070: 6f77 2049 6e73 7461 6c6c 6174 696f 6e20  ow Installation 
-00002080: 496e 7374 7275 6374 696f 6e73 5d28 6874  Instructions](ht
-00002090: 7470 733a 2f2f 7777 772e 7465 6e73 6f72  tps://www.tensor
-000020a0: 666c 6f77 2e6f 7267 2f69 6e73 7461 6c6c  flow.org/install
-000020b0: 290d 0a20 2020 2020 2020 202d 2041 6e79  )..        - Any
-000020c0: 2054 656e 736f 7266 6c6f 7720 7665 7273   Tensorflow vers
-000020d0: 696f 6e20 3e3d 312e 3133 2e30 2073 686f  ion >=1.13.0 sho
-000020e0: 756c 6420 6265 2063 6f6d 7061 7469 626c  uld be compatibl
-000020f0: 6520 2869 6e63 6c75 6469 6e67 2032 2e30  e (including 2.0
-00002100: 292e 0d0a 2020 2020 2020 2020 0d0a 2020  )...        ..  
-00002110: 2020 2020 2020 4465 6570 506f 7365 4b69        DeepPoseKi
-00002120: 7420 6861 7320 6f6e 6c79 2062 6565 6e20  t has only been 
-00002130: 7465 7374 6564 206f 6e20 5562 756e 7475  tested on Ubuntu
-00002140: 2031 382e 3034 2c20 7768 6963 6820 6973   18.04, which is
-00002150: 2074 6865 2072 6563 6f6d 6d65 6e64 6564   the recommended
-00002160: 2073 7973 7465 6d20 666f 7220 7573 696e   system for usin
-00002170: 6720 7468 6520 746f 6f6c 6b69 742e 200d  g the toolkit. .
-00002180: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00002190: 2020 2049 6e73 7461 6c6c 2074 6865 206c     Install the l
-000021a0: 6174 6573 7420 7374 6162 6c65 2072 656c  atest stable rel
-000021b0: 6561 7365 2077 6974 6820 7069 703a 0d0a  ease with pip:..
-000021c0: 2020 2020 2020 2020 6060 6062 6173 680d          ```bash.
-000021d0: 0a20 2020 2020 2020 2070 6970 2069 6e73  .        pip ins
-000021e0: 7461 6c6c 202d 2d75 7064 6174 6520 6465  tall --update de
-000021f0: 6570 706f 7365 6b69 740d 0a20 2020 2020  epposekit..     
-00002200: 2020 2060 6060 0d0a 2020 2020 2020 2020     ```..        
-00002210: 0d0a 2020 2020 2020 2020 496e 7374 616c  ..        Instal
-00002220: 6c20 7468 6520 6c61 7465 7374 2064 6576  l the latest dev
-00002230: 656c 6f70 6d65 6e74 2076 6572 7369 6f6e  elopment version
-00002240: 2077 6974 6820 7069 703a 0d0a 2020 2020   with pip:..    
-00002250: 2020 2020 6060 6062 6173 680d 0a20 2020      ```bash..   
-00002260: 2020 2020 2070 6970 2069 6e73 7461 6c6c       pip install
-00002270: 202d 2d75 7064 6174 6520 6769 742b 6874   --update git+ht
-00002280: 7470 733a 2f2f 7777 772e 6769 7468 7562  tps://www.github
-00002290: 2e63 6f6d 2f6a 6772 6176 696e 672f 6465  .com/jgraving/de
-000022a0: 6570 706f 7365 6b69 742e 6769 740d 0a20  epposekit.git.. 
-000022b0: 2020 2020 2020 2060 6060 0d0a 2020 2020         ```..    
-000022c0: 2020 2020 0d0a 2020 2020 2020 2020 596f      ..        Yo
-000022d0: 7520 6361 6e20 646f 776e 6c6f 6164 2065  u can download e
-000022e0: 7861 6d70 6c65 2064 6174 6173 6574 7320  xample datasets 
-000022f0: 6672 6f6d 206f 7572 205b 4465 6570 506f  from our [DeepPo
-00002300: 7365 4b69 7420 4461 7461 5d28 6874 7470  seKit Data](http
-00002310: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00002320: 6772 6176 696e 672f 6465 6570 706f 7365  graving/deeppose
-00002330: 6b69 742d 6461 7461 2920 7265 706f 7369  kit-data) reposi
-00002340: 746f 7279 3a0d 0a20 2020 2020 2020 2060  tory:..        `
-00002350: 6060 6261 7368 0d0a 2020 2020 2020 2020  ``bash..        
-00002360: 6769 7420 636c 6f6e 6520 6874 7470 733a  git clone https:
-00002370: 2f2f 7777 772e 6769 7468 7562 2e63 6f6d  //www.github.com
-00002380: 2f6a 6772 6176 696e 672f 6465 6570 706f  /jgraving/deeppo
-00002390: 7365 6b69 742d 6461 7461 0d0a 2020 2020  sekit-data..    
-000023a0: 2020 2020 6060 600d 0a20 2020 2020 2020      ```..       
-000023b0: 200d 0a20 2020 2020 2020 2023 2320 496e   ..        ## In
-000023c0: 7374 616c 6c69 6e67 2077 6974 6820 416e  stalling with An
-000023d0: 6163 6f6e 6461 206f 6e20 5769 6e64 6f77  aconda on Window
-000023e0: 730d 0a20 2020 2020 2020 200d 0a20 2020  s..        ..   
-000023f0: 2020 2020 2054 6f20 696e 7374 616c 6c20       To install 
-00002400: 4465 6570 506f 7365 4b69 7420 6f6e 2057  DeepPoseKit on W
-00002410: 696e 646f 7773 2c20 796f 7520 6d75 7374  indows, you must
-00002420: 2066 6972 7374 206d 616e 7561 6c6c 7920   first manually 
-00002430: 696e 7374 616c 6c20 6053 6861 7065 6c79  install `Shapely
-00002440: 602c 206f 6e65 206f 6620 7468 6520 6465  `, one of the de
-00002450: 7065 6e64 656e 6369 6573 2066 6f72 2074  pendencies for t
-00002460: 6865 205b 696d 6761 7567 2070 6163 6b61  he [imgaug packa
-00002470: 6765 5d28 6874 7470 733a 2f2f 6769 7468  ge](https://gith
-00002480: 7562 2e63 6f6d 2f61 6c65 6a75 2f69 6d67  ub.com/aleju/img
-00002490: 6175 6729 3a0d 0a20 2020 2020 2020 2060  aug):..        `
-000024a0: 6060 6261 7368 0d0a 2020 2020 2020 2020  ``bash..        
-000024b0: 636f 6e64 6120 696e 7374 616c 6c20 2d63  conda install -c
-000024c0: 2063 6f6e 6461 2d66 6f72 6765 2073 6861   conda-forge sha
-000024d0: 7065 6c79 0d0a 2020 2020 2020 2020 6060  pely..        ``
-000024e0: 600d 0a20 2020 2020 2020 2057 6520 616c  `..        We al
-000024f0: 736f 2072 6563 6f6d 6d65 6e64 2069 6e73  so recommend ins
-00002500: 7461 6c6c 696e 6720 4465 6570 506f 7365  talling DeepPose
-00002510: 4b69 7420 6672 6f6d 2077 6974 6869 6e20  Kit from within 
-00002520: 5079 7468 6f6e 2072 6174 6865 7220 7468  Python rather th
-00002530: 616e 2075 7369 6e67 2074 6865 2063 6f6d  an using the com
-00002540: 6d61 6e64 206c 696e 652c 2065 6974 6865  mand line, eithe
-00002550: 7220 6672 6f6d 2077 6974 6869 6e20 4a75  r from within Ju
-00002560: 7079 7465 7220 6f72 2061 6e6f 7468 6572  pyter or another
-00002570: 2049 4445 2c20 746f 2065 6e73 7572 6520   IDE, to ensure 
-00002580: 6974 2069 7320 696e 7374 616c 6c65 6420  it is installed 
-00002590: 696e 2074 6865 2063 6f72 7265 6374 2077  in the correct w
-000025a0: 6f72 6b69 6e67 2065 6e76 6972 6f6e 6d65  orking environme
-000025b0: 6e74 3a0d 0a20 2020 2020 2020 2060 6060  nt:..        ```
-000025c0: 7079 7468 6f6e 0d0a 2020 2020 2020 2020  python..        
-000025d0: 696d 706f 7274 2073 7973 0d0a 2020 2020  import sys..    
-000025e0: 2020 2020 217b 7379 732e 6578 6563 7574      !{sys.execut
-000025f0: 6162 6c65 7d20 2d6d 2070 6970 2069 6e73  able} -m pip ins
-00002600: 7461 6c6c 202d 2d75 7064 6174 6520 6465  tall --update de
-00002610: 6570 706f 7365 6b69 740d 0a20 2020 2020  epposekit..     
-00002620: 2020 2060 6060 0d0a 2020 2020 2020 2020     ```..        
-00002630: 2320 436f 6e74 7269 6275 746f 7273 2061  # Contributors a
-00002640: 6e64 2044 6576 656c 6f70 6d65 6e74 2020  nd Development  
-00002650: 0d0a 2020 2020 2020 2020 2020 200d 0a20  ..           .. 
-00002660: 2020 2020 2020 2044 6565 7050 6f73 654b         DeepPoseK
-00002670: 6974 2077 6173 2064 6576 656c 6f70 6564  it was developed
-00002680: 2062 7920 5b4a 616b 6520 4772 6176 696e   by [Jake Gravin
-00002690: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
-000026a0: 622e 636f 6d2f 6a67 7261 7669 6e67 2920  b.com/jgraving) 
-000026b0: 616e 6420 5b44 616e 6965 6c20 4368 6165  and [Daniel Chae
-000026c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000026d0: 2e63 6f6d 2f64 6368 6165 6261 6529 2c20  .com/dchaebae), 
-000026e0: 616e 6420 6973 2073 7469 6c6c 2062 6569  and is still bei
-000026f0: 6e67 2061 6374 6976 656c 7920 6465 7665  ng actively deve
-00002700: 6c6f 7065 642e 202e 0d0a 2020 2020 2020  loped. ...      
-00002710: 2020 0d0a 2020 2020 2020 2020 5765 2077    ..        We w
-00002720: 656c 636f 6d65 2063 6f6d 6d75 6e69 7479  elcome community
-00002730: 2069 6e76 6f6c 7665 6d65 6e74 2061 6e64   involvement and
-00002740: 2070 7562 6c69 6320 636f 6e74 7269 6275   public contribu
-00002750: 7469 6f6e 7320 746f 2074 6865 2074 6f6f  tions to the too
-00002760: 6c6b 6974 2e20 4966 2079 6f75 2077 6973  lkit. If you wis
-00002770: 6820 746f 2063 6f6e 7472 6962 7574 652c  h to contribute,
-00002780: 2070 6c65 6173 6520 5b66 6f72 6b20 7468   please [fork th
-00002790: 6520 7265 706f 7369 746f 7279 5d28 6874  e repository](ht
-000027a0: 7470 733a 2f2f 6865 6c70 2e67 6974 6875  tps://help.githu
-000027b0: 622e 636f 6d2f 656e 2f61 7274 6963 6c65  b.com/en/article
-000027c0: 732f 666f 726b 2d61 2d72 6570 6f29 2074  s/fork-a-repo) t
-000027d0: 6f20 6d61 6b65 2079 6f75 7220 6d6f 6469  o make your modi
-000027e0: 6669 6361 7469 6f6e 7320 616e 6420 5b73  fications and [s
-000027f0: 7562 6d69 7420 6120 7075 6c6c 2072 6571  ubmit a pull req
-00002800: 7565 7374 5d28 6874 7470 733a 2f2f 6865  uest](https://he
-00002810: 6c70 2e67 6974 6875 622e 636f 6d2f 656e  lp.github.com/en
-00002820: 2f61 7274 6963 6c65 732f 6372 6561 7469  /articles/creati
-00002830: 6e67 2d61 2d70 756c 6c2d 7265 7175 6573  ng-a-pull-reques
-00002840: 742d 6672 6f6d 2d61 2d66 6f72 6b29 2e0d  t-from-a-fork)..
-00002850: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00002860: 2020 2049 6620 796f 7527 6420 6c69 6b65     If you'd like
-00002870: 2074 6f20 6765 7420 696e 766f 6c76 6564   to get involved
-00002880: 2077 6974 6820 6465 7665 6c6f 7069 6e67   with developing
-00002890: 2044 6565 7050 6f73 654b 6974 2c20 6765   DeepPoseKit, ge
-000028a0: 7420 696e 2074 6f75 6368 2028 6a67 7261  t in touch (jgra
-000028b0: 7669 6e67 4067 6d61 696c 2e63 6f6d 2920  ving@gmail.com) 
-000028c0: 616e 6420 6368 6563 6b20 6f75 7420 5b6f  and check out [o
-000028d0: 7572 2064 6576 656c 6f70 6d65 6e74 2072  ur development r
-000028e0: 6f61 646d 6170 5d28 6874 7470 733a 2f2f  oadmap](https://
-000028f0: 6769 7468 7562 2e63 6f6d 2f6a 6772 6176  github.com/jgrav
-00002900: 696e 672f 4465 6570 506f 7365 4b69 742f  ing/DeepPoseKit/
-00002910: 626c 6f62 2f6d 6173 7465 722f 4445 5645  blob/master/DEVE
-00002920: 4c4f 504d 454e 542e 6d64 2920 746f 2073  LOPMENT.md) to s
-00002930: 6565 2066 7574 7572 6520 706c 616e 7320  ee future plans 
-00002940: 666f 7220 7468 6520 7061 636b 6167 652e  for the package.
-00002950: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
-00002960: 2020 2020 2020 2320 4973 7375 6573 2020        # Issues  
-00002970: 0d0a 2020 2020 2020 2020 200d 0a20 2020  ..         ..   
-00002980: 2020 2020 2050 6c65 6173 6520 7375 626d       Please subm
-00002990: 6974 2062 7567 7320 6f72 2066 6561 7475  it bugs or featu
-000029a0: 7265 2072 6571 7565 7374 7320 746f 2074  re requests to t
-000029b0: 6865 205b 4769 7448 7562 2069 7373 7565  he [GitHub issue
-000029c0: 2074 7261 636b 6572 5d28 6874 7470 733a   tracker](https:
-000029d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6772  //github.com/jgr
-000029e0: 6176 696e 672f 6465 6570 706f 7365 6b69  aving/deepposeki
-000029f0: 742f 6973 7375 6573 2f6e 6577 292e 2050  t/issues/new). P
-00002a00: 6c65 6173 6520 6c69 6d69 7420 7265 706f  lease limit repo
-00002a10: 7274 6564 2069 7373 7565 7320 746f 2074  rted issues to t
-00002a20: 6865 2044 6565 7050 6f73 654b 6974 2063  he DeepPoseKit c
-00002a30: 6f64 6562 6173 6520 616e 6420 7072 6f76  odebase and prov
-00002a40: 6964 6520 6173 206d 7563 6820 6465 7461  ide as much deta
-00002a50: 696c 2061 7320 796f 7520 6361 6e20 7769  il as you can wi
-00002a60: 7468 2061 206d 696e 696d 616c 2077 6f72  th a minimal wor
-00002a70: 6b69 6e67 2065 7861 6d70 6c65 2069 6620  king example if 
-00002a80: 706f 7373 6962 6c65 2e0d 0a20 2020 2020  possible...     
-00002a90: 2020 200d 0a20 2020 2020 2020 2049 6620     ..        If 
-00002aa0: 796f 7520 6578 7065 7269 656e 6365 2070  you experience p
-00002ab0: 726f 626c 656d 7320 7769 7468 205b 5465  roblems with [Te
-00002ac0: 6e73 6f72 666c 6f77 5d28 6874 7470 733a  nsorflow](https:
-00002ad0: 2f2f 6769 7468 7562 2e63 6f6d 2f74 656e  //github.com/ten
-00002ae0: 736f 7266 6c6f 772f 7465 6e73 6f72 666c  sorflow/tensorfl
-00002af0: 6f77 292c 2073 7563 6820 6173 2069 6e73  ow), such as ins
-00002b00: 7461 6c6c 696e 6720 4355 4441 206f 7220  talling CUDA or 
-00002b10: 6375 444e 4e20 6465 7065 6e64 656e 6369  cuDNN dependenci
-00002b20: 6573 2c20 7468 656e 2070 6c65 6173 6520  es, then please 
-00002b30: 6469 7265 6374 2069 7373 7565 7320 746f  direct issues to
-00002b40: 2074 686f 7365 2064 6576 656c 6f70 6d65   those developme
-00002b50: 6e74 2074 6561 6d73 2e0d 0a20 2020 2020  nt teams...     
-00002b60: 2020 200d 0a20 2020 2020 2020 2023 204c     ..        # L
-00002b70: 6963 656e 7365 0d0a 2020 2020 2020 2020  icense..        
-00002b80: 0d0a 2020 2020 2020 2020 5265 6c65 6173  ..        Releas
-00002b90: 6564 2075 6e64 6572 2061 2041 7061 6368  ed under a Apach
-00002ba0: 6520 322e 3020 4c69 6365 6e73 652e 2053  e 2.0 License. S
-00002bb0: 6565 205b 4c49 4345 4e53 455d 2868 7474  ee [LICENSE](htt
-00002bc0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002bd0: 6a67 7261 7669 6e67 2f64 6565 7070 6f73  jgraving/deeppos
-00002be0: 656b 6974 2f62 6c6f 622f 6d61 7374 6572  ekit/blob/master
-00002bf0: 2f4c 4943 454e 5345 2920 666f 7220 6465  /LICENSE) for de
-00002c00: 7461 696c 732e 0d0a 2020 2020 2020 2020  tails...        
-00002c10: 0d0a 2020 2020 2020 2020 2320 5265 6665  ..        # Refe
-00002c20: 7265 6e63 6573 0d0a 2020 2020 2020 2020  rences..        
-00002c30: 0d0a 2020 2020 2020 2020 4966 2079 6f75  ..        If you
-00002c40: 2075 7365 2044 6565 7050 6f73 654b 6974   use DeepPoseKit
-00002c50: 2066 6f72 2079 6f75 7220 7265 7365 6172   for your resear
-00002c60: 6368 2070 6c65 6173 6520 6369 7465 205b  ch please cite [
-00002c70: 6f75 7220 6f70 656e 2d61 6363 6573 7320  our open-access 
-00002c80: 7061 7065 725d 2868 7474 703a 2f2f 7061  paper](http://pa
-00002c90: 7065 722e 6465 6570 706f 7365 6b69 742e  per.deepposekit.
-00002ca0: 6f72 6729 3a0d 0a20 2020 2020 2020 200d  org):..        .
-00002cb0: 0a20 2020 2020 2020 2020 2020 2040 6172  .            @ar
-00002cc0: 7469 636c 657b 6772 6176 696e 6732 3031  ticle{graving201
-00002cd0: 3964 6565 7070 6f73 656b 6974 2c0d 0a20  9deepposekit,.. 
-00002ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cf0: 2020 2020 7469 746c 653d 7b44 6565 7050      title={DeepP
-00002d00: 6f73 654b 6974 2c20 6120 736f 6674 7761  oseKit, a softwa
-00002d10: 7265 2074 6f6f 6c6b 6974 2066 6f72 2066  re toolkit for f
-00002d20: 6173 7420 616e 6420 726f 6275 7374 2061  ast and robust a
-00002d30: 6e69 6d61 6c20 706f 7365 2065 7374 696d  nimal pose estim
-00002d40: 6174 696f 6e20 7573 696e 6720 6465 6570  ation using deep
-00002d50: 206c 6561 726e 696e 677d 2c0d 0a20 2020   learning},..   
-00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d70: 2020 6175 7468 6f72 3d7b 4772 6176 696e    author={Gravin
-00002d80: 672c 204a 6163 6f62 204d 2061 6e64 2043  g, Jacob M and C
-00002d90: 6861 652c 2044 616e 6965 6c20 616e 6420  hae, Daniel and 
-00002da0: 4e61 696b 2c20 4865 6d61 6c20 616e 6420  Naik, Hemal and 
-00002db0: 4c69 2c20 4c69 616e 6720 616e 6420 4b6f  Li, Liang and Ko
-00002dc0: 6765 722c 2042 656e 6a61 6d69 6e20 616e  ger, Benjamin an
-00002dd0: 6420 436f 7374 656c 6c6f 652c 2042 6c61  d Costelloe, Bla
-00002de0: 6972 2052 2061 6e64 2043 6f75 7a69 6e2c  ir R and Couzin,
-00002df0: 2049 6169 6e20 447d 2c0d 0a20 2020 2020   Iain D},..     
-00002e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e10: 6a6f 7572 6e61 6c3d 7b65 4c69 6665 7d2c  journal={eLife},
-00002e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002e30: 2020 2020 2020 2076 6f6c 756d 653d 7b38         volume={8
-00002e40: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00002e50: 2020 2020 2020 2020 2070 6167 6573 3d7b           pages={
-00002e60: 6534 3739 3934 7d2c 0d0a 2020 2020 2020  e47994},..      
-00002e70: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-00002e80: 6561 723d 7b32 3031 397d 2c0d 0a20 2020  ear={2019},..   
-00002e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ea0: 2020 7075 626c 6973 6865 723d 7b65 4c69    publisher={eLi
-00002eb0: 6665 2053 6369 656e 6365 7320 5075 626c  fe Sciences Publ
-00002ec0: 6963 6174 696f 6e73 204c 696d 6974 6564  ications Limited
-00002ed0: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-00002ee0: 2020 2020 2020 2020 7572 6c3d 7b68 7474          url={htt
-00002ef0: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
-00002f00: 3735 3534 2f65 4c69 6665 2e34 3739 3934  7554/eLife.47994
-00002f10: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00002f20: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00002f30: 2020 2020 0d0a 2020 2020 2020 2020 596f      ..        Yo
-00002f40: 7520 6361 6e20 616c 736f 2072 6561 6420  u can also read 
-00002f50: 5b6f 7572 206f 7065 6e2d 6163 6365 7373  [our open-access
-00002f60: 2070 7265 7072 696e 745d 2868 7474 703a   preprint](http:
-00002f70: 2f2f 7072 6570 7269 6e74 2e64 6565 7070  //preprint.deepp
-00002f80: 6f73 656b 6974 2e6f 7267 292e 0d0a 2020  osekit.org)...  
-00002f90: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00002fa0: 4966 2079 6f75 2075 7365 2074 6865 205b  If you use the [
-00002fb0: 696d 6761 7567 2070 6163 6b61 6765 5d28  imgaug package](
-00002fc0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002fd0: 6f6d 2f61 6c65 6a75 2f69 6d67 6175 6729  om/aleju/imgaug)
-00002fe0: 2066 6f72 2064 6174 6120 6175 676d 656e   for data augmen
-00002ff0: 7461 7469 6f6e 2c20 706c 6561 7365 2061  tation, please a
-00003000: 6c73 6f20 636f 6e73 6964 6572 205b 6369  lso consider [ci
-00003010: 7469 6e67 2069 745d 2868 7474 7073 3a2f  ting it](https:/
-00003020: 2f67 6974 6875 622e 636f 6d2f 616c 656a  /github.com/alej
-00003030: 752f 696d 6761 7567 2f62 6c6f 622f 6d61  u/imgaug/blob/ma
-00003040: 7374 6572 2f52 4541 444d 452e 6d64 2363  ster/README.md#c
-00003050: 6974 6174 696f 6e29 2e0d 0a20 2020 2020  itation)...     
-00003060: 2020 200d 0a20 2020 2020 2020 2049 6620     ..        If 
-00003070: 796f 7520 5b75 7365 2064 6174 615d 2868  you [use data](h
-00003080: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003090: 6d2f 6a67 7261 7669 6e67 2f44 6565 7050  m/jgraving/DeepP
-000030a0: 6f73 654b 6974 2369 2d61 6c72 6561 6479  oseKit#i-already
-000030b0: 2d68 6176 652d 616e 6e6f 7461 7465 642d  -have-annotated-
-000030c0: 6461 7461 2920 7468 6174 2077 6173 2061  data) that was a
-000030d0: 6e6e 6f74 6174 6564 2077 6974 6820 7468  nnotated with th
-000030e0: 6520 4465 6570 4c61 6243 7574 2070 6163  e DeepLabCut pac
-000030f0: 6b61 6765 2028 6874 7470 3a2f 2f64 6565  kage (http://dee
-00003100: 706c 6162 6375 742e 6f72 6729 2066 6f72  plabcut.org) for
-00003110: 2079 6f75 7220 7265 7365 6172 6368 2c20   your research, 
-00003120: 6265 2073 7572 6520 746f 205b 6369 7465  be sure to [cite
-00003130: 2069 745d 2868 7474 7073 3a2f 2f67 6974   it](https://git
-00003140: 6875 622e 636f 6d2f 416c 6578 454d 472f  hub.com/AlexEMG/
-00003150: 4465 6570 4c61 6243 7574 2f62 6c6f 622f  DeepLabCut/blob/
-00003160: 6d61 7374 6572 2f52 4541 444d 452e 6d64  master/README.md
-00003170: 2372 6566 6572 656e 6365 7329 2e0d 0a20  #references)... 
-00003180: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00003190: 2050 6c65 6173 6520 616c 736f 2063 6f6e   Please also con
-000031a0: 7369 6465 7220 6369 7469 6e67 2074 6865  sider citing the
-000031b0: 2072 656c 6576 616e 7420 7265 6665 7265   relevant refere
-000031c0: 6e63 6573 2066 6f72 2074 6865 2070 6f73  nces for the pos
-000031d0: 6520 6573 7469 6d61 7469 6f6e 206d 6f64  e estimation mod
-000031e0: 656c 2873 2920 7573 6564 2069 6e20 796f  el(s) used in yo
-000031f0: 7572 2072 6573 6561 7263 682c 2077 6869  ur research, whi
-00003200: 6368 2063 616e 2062 6520 666f 756e 6420  ch can be found 
-00003210: 696e 2074 6865 2064 6f63 756d 656e 7461  in the documenta
-00003220: 7469 6f6e 2028 692e 652e 2c20 5b60 5374  tion (i.e., [`St
-00003230: 6163 6b65 6444 656e 7365 4e65 7460 5d28  ackedDenseNet`](
-00003240: 6874 7470 3a2f 2f6a 616b 6567 7261 7669  http://jakegravi
-00003250: 6e67 2e63 6f6d 2f44 6565 7050 6f73 654b  ng.com/DeepPoseK
-00003260: 6974 2f68 746d 6c2f 6465 6570 706f 7365  it/html/deeppose
-00003270: 6b69 742f 6d6f 6465 6c73 2f53 7461 636b  kit/models/Stack
-00003280: 6564 4465 6e73 654e 6574 2e68 746d 6c23  edDenseNet.html#
-00003290: 7265 6665 7265 6e63 6573 292c 205b 6053  references), [`S
-000032a0: 7461 636b 6564 486f 7572 676c 6173 7360  tackedHourglass`
-000032b0: 5d28 6874 7470 3a2f 2f6a 616b 6567 7261  ](http://jakegra
-000032c0: 7669 6e67 2e63 6f6d 2f44 6565 7050 6f73  ving.com/DeepPos
-000032d0: 654b 6974 2f68 746d 6c2f 6465 6570 706f  eKit/html/deeppo
-000032e0: 7365 6b69 742f 6d6f 6465 6c73 2f53 7461  sekit/models/Sta
-000032f0: 636b 6564 486f 7572 676c 6173 732e 6874  ckedHourglass.ht
-00003300: 6d6c 2372 6566 6572 656e 6365 7329 2c20  ml#references), 
-00003310: 5b60 4465 6570 4c61 6243 7574 605d 2868  [`DeepLabCut`](h
-00003320: 7474 703a 2f2f 6a61 6b65 6772 6176 696e  ttp://jakegravin
-00003330: 672e 636f 6d2f 4465 6570 506f 7365 4b69  g.com/DeepPoseKi
-00003340: 742f 6874 6d6c 2f64 6565 7070 6f73 656b  t/html/deepposek
-00003350: 6974 2f6d 6f64 656c 732f 4465 6570 4c61  it/models/DeepLa
-00003360: 6243 7574 2e68 746d 6c23 7265 6665 7265  bCut.html#refere
-00003370: 6e63 6573 292c 205b 604c 4541 5060 5d28  nces), [`LEAP`](
-00003380: 6874 7470 3a2f 2f6a 616b 6567 7261 7669  http://jakegravi
-00003390: 6e67 2e63 6f6d 2f44 6565 7050 6f73 654b  ng.com/DeepPoseK
-000033a0: 6974 2f68 746d 6c2f 6465 6570 706f 7365  it/html/deeppose
-000033b0: 6b69 742f 6d6f 6465 6c73 2f4c 4541 502e  kit/models/LEAP.
-000033c0: 6874 6d6c 2372 6566 6572 656e 6365 7329  html#references)
-000033d0: 292e 0d0a 2020 2020 2020 2020 0d0a 2020  )...        ..  
-000033e0: 2020 2020 2020 2320 4e65 7773 0d0a 2020        # News..  
-000033f0: 2020 2020 2020 2d20 2a2a 4f63 746f 6265        - **Octobe
-00003400: 7220 3230 3139 3a2a 2a20 4f75 7220 7061  r 2019:** Our pa
-00003410: 7065 7220 6465 7363 7269 6269 6e67 2044  per describing D
-00003420: 6565 7050 6f73 654b 6974 2069 7320 7075  eepPoseKit is pu
-00003430: 626c 6973 6865 6420 6174 2065 4c69 6665  blished at eLife
-00003440: 2120 2868 7474 703a 2f2f 7061 7065 722e  ! (http://paper.
-00003450: 6465 6570 706f 7365 6b69 742e 6f72 6729  deepposekit.org)
-00003460: 0d0a 2020 2020 2020 2020 2d20 2a2a 5365  ..        - **Se
-00003470: 7074 656d 6265 7220 3230 3139 2a2a 3a20  ptember 2019**: 
-00003480: 0d0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
-00003490: 4e61 7475 7265 204e 6577 7320 636f 7665  Nature News cove
-000034a0: 7273 2044 6565 7050 6f73 654b 6974 3a20  rs DeepPoseKit: 
-000034b0: 5b44 6565 7020 6c65 6172 6e69 6e67 2070  [Deep learning p
-000034c0: 6f77 6572 7320 6120 6d6f 7469 6f6e 2d74  owers a motion-t
-000034d0: 7261 636b 696e 6720 7265 766f 6c75 7469  racking revoluti
-000034e0: 6f6e 5d28 6874 7470 3a2f 2f64 6f69 2e6f  on](http://doi.o
-000034f0: 7267 2f31 302e 3130 3338 2f64 3431 3538  rg/10.1038/d4158
-00003500: 362d 3031 392d 3032 3934 322d 3529 0d0a  6-019-02942-5)..
-00003510: 2020 2020 2020 2020 2020 2020 2d20 7630              - v0
-00003520: 2e33 2e30 2069 7320 7265 6c65 6173 6564  .3.0 is released
-00003530: 2e20 5365 6520 5b74 6865 2072 656c 6561  . See [the relea
-00003540: 7365 206e 6f74 6573 5d28 6874 7470 733a  se notes](https:
-00003550: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6772  //github.com/jgr
-00003560: 6176 696e 672f 4465 6570 506f 7365 4b69  aving/DeepPoseKi
-00003570: 742f 7265 6c65 6173 6573 2f74 6167 2f76  t/releases/tag/v
-00003580: 302e 332e 3029 2e0d 0a20 2020 2020 2020  0.3.0)...       
-00003590: 202d 202a 2a41 7072 696c 2032 3031 393a   - **April 2019:
-000035a0: 2a2a 2054 6865 2044 6565 7050 6f73 654b  ** The DeepPoseK
-000035b0: 6974 2070 7265 7072 696e 7420 6973 206f  it preprint is o
-000035c0: 6e20 6269 6f72 7869 7620 2868 7474 703a  n biorxiv (http:
-000035d0: 2f2f 7072 6570 7269 6e74 2e64 6565 7070  //preprint.deepp
-000035e0: 6f73 656b 6974 2e6f 7267 290d 0a20 2020  osekit.org)..   
-000035f0: 2020 2020 200d 0a50 6c61 7466 6f72 6d3a       ..Platform:
-00003600: 2055 4e4b 4e4f 574e 0d0a 436c 6173 7369   UNKNOWN..Classi
-00003610: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-00003620: 7564 6965 6e63 6520 3a3a 2053 6369 656e  udience :: Scien
-00003630: 6365 2f52 6573 6561 7263 680d 0a43 6c61  ce/Research..Cla
-00003640: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00003650: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00003660: 2050 7974 686f 6e20 3a3a 2033 0d0a 436c   Python :: 3..Cl
-00003670: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00003680: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
-00003690: 6769 6e65 6572 696e 6720 3a3a 2049 6d61  gineering :: Ima
-000036a0: 6765 2052 6563 6f67 6e69 7469 6f6e 0d0a  ge Recognition..
-000036b0: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
-000036c0: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
-000036d0: 6172 6b64 6f77 6e0d 0a                   arkdown..
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0d0a 3c69 6d67 2073 7263 3d22 6874  ">..<img src="ht
+00000020: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000030: 2f6a 6772 6176 696e 672f 4465 6570 506f  /jgraving/DeepPo
+00000040: 7365 4b69 742f 626c 6f62 2f6d 6173 7465  seKit/blob/maste
+00000050: 722f 6173 7365 7473 2f64 6565 7070 6f73  r/assets/deeppos
+00000060: 656b 6974 5f6c 6f67 6f2e 706e 6722 2068  ekit_logo.png" h
+00000070: 6569 6768 743d 2233 3230 7078 223e 0d0a  eight="320px">..
+00000080: 3c2f 703e 0d0a 0d0a 2320 596f 7520 6861  </p>....# You ha
+00000090: 7665 206a 7573 7420 666f 756e 6420 4465  ve just found De
+000000a0: 6570 506f 7365 4b69 742e 0d0a 3c70 2061  epPoseKit...<p a
+000000b0: 6c69 676e 3d22 6365 6e74 6572 223e 0d0a  lign="center">..
+000000c0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000000d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6772  //github.com/jgr
+000000e0: 6176 696e 672f 6a67 7261 7669 6e67 2e67  aving/jgraving.g
+000000f0: 6974 6875 622e 696f 2f62 6c6f 622f 6d61  ithub.io/blob/ma
+00000100: 7374 6572 2f66 696c 6573 2f69 6d61 6765  ster/files/image
+00000110: 732f 4669 6775 7265 3176 6964 656f 312e  s/Figure1video1.
+00000120: 6769 6622 2068 6569 6768 743d 2231 3238  gif" height="128
+00000130: 7078 223e 0d0a 3c2f 703e 0d0a 0d0a 4465  px">..</p>....De
+00000140: 6570 506f 7365 4b69 7420 6973 2061 2073  epPoseKit is a s
+00000150: 6f66 7477 6172 6520 746f 6f6c 6b69 7420  oftware toolkit 
+00000160: 7769 7468 2061 2068 6967 682d 6c65 7665  with a high-leve
+00000170: 6c20 4150 4920 666f 7220 3244 2070 6f73  l API for 2D pos
+00000180: 6520 6573 7469 6d61 7469 6f6e 206f 6620  e estimation of 
+00000190: 7573 6572 2d64 6566 696e 6564 206b 6579  user-defined key
+000001a0: 706f 696e 7473 2075 7369 6e67 2064 6565  points using dee
+000001b0: 7020 6c65 6172 6e69 6e67 e280 9477 7269  p learning...wri
+000001c0: 7474 656e 2069 6e20 5079 7468 6f6e 2061  tten in Python a
+000001d0: 6e64 2062 7569 6c74 2075 7369 6e67 205b  nd built using [
+000001e0: 5465 6e73 6f72 666c 6f77 5d28 6874 7470  Tensorflow](http
+000001f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
+00000200: 656e 736f 7266 6c6f 772f 7465 6e73 6f72  ensorflow/tensor
+00000210: 666c 6f77 2920 616e 6420 5b4b 6572 6173  flow) and [Keras
+00000220: 5d28 6874 7470 733a 2f2f 7777 772e 7465  ](https://www.te
+00000230: 6e73 6f72 666c 6f77 2e6f 7267 2f67 7569  nsorflow.org/gui
+00000240: 6465 2f6b 6572 6173 292e 2055 7365 2044  de/keras). Use D
+00000250: 6565 7050 6f73 654b 6974 2069 6620 796f  eepPoseKit if yo
+00000260: 7520 6e65 6564 3a0d 0a0d 0a2d 2074 6f6f  u need:....- too
+00000270: 6c73 2066 6f72 2061 6e6e 6f74 6174 696e  ls for annotatin
+00000280: 6720 696d 6167 6573 206f 7220 7669 6465  g images or vide
+00000290: 6f20 6672 616d 6573 2077 6974 6820 7573  o frames with us
+000002a0: 6572 2d64 6566 696e 6564 206b 6579 706f  er-defined keypo
+000002b0: 696e 7473 0d0a 2d20 6120 7374 7261 6967  ints..- a straig
+000002c0: 6874 666f 7277 6172 6420 6275 7420 666c  htforward but fl
+000002d0: 6578 6962 6c65 2064 6174 6120 6175 676d  exible data augm
+000002e0: 656e 7461 7469 6f6e 2070 6970 656c 696e  entation pipelin
+000002f0: 6520 7573 696e 6720 7468 6520 5b69 6d67  e using the [img
+00000300: 6175 6720 7061 636b 6167 655d 2868 7474  aug package](htt
+00000310: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000320: 616c 656a 752f 696d 6761 7567 290d 0a2d  aleju/imgaug)..-
+00000330: 2061 204b 6572 6173 2d62 6173 6564 2069   a Keras-based i
+00000340: 6e74 6572 6661 6365 2066 6f72 2069 6e69  nterface for ini
+00000350: 7469 616c 697a 696e 672c 2074 7261 696e  tializing, train
+00000360: 696e 672c 2061 6e64 2065 7661 6c75 6174  ing, and evaluat
+00000370: 696e 6720 706f 7365 2065 7374 696d 6174  ing pose estimat
+00000380: 696f 6e20 6d6f 6465 6c73 0d0a 2d20 6561  ion models..- ea
+00000390: 7379 2d74 6f2d 7573 6520 6d65 7468 6f64  sy-to-use method
+000003a0: 7320 666f 7220 7361 7669 6e67 2061 6e64  s for saving and
+000003b0: 206c 6f61 6469 6e67 206d 6f64 656c 7320   loading models 
+000003c0: 616e 6420 6d61 6b69 6e67 2070 7265 6469  and making predi
+000003d0: 6374 696f 6e73 206f 6e20 6e65 7720 6461  ctions on new da
+000003e0: 7461 0d0a 0d0a 4465 6570 506f 7365 4b69  ta....DeepPoseKi
+000003f0: 7420 6973 2064 6573 6967 6e65 6420 7769  t is designed wi
+00000400: 7468 2061 2066 6f63 7573 206f 6e20 2a75  th a focus on *u
+00000410: 7361 6269 6c69 7479 2a20 616e 6420 2a65  sability* and *e
+00000420: 7874 656e 7369 6269 6c69 7479 2a2c 2061  xtensibility*, a
+00000430: 7320 6265 696e 6720 6162 6c65 2074 6f20  s being able to 
+00000440: 676f 2066 726f 6d20 6964 6561 2074 6f20  go from idea to 
+00000450: 7265 7375 6c74 2077 6974 6820 7468 6520  result with the 
+00000460: 6c65 6173 7420 706f 7373 6962 6c65 2064  least possible d
+00000470: 656c 6179 2069 7320 6b65 7920 746f 2064  elay is key to d
+00000480: 6f69 6e67 2067 6f6f 6420 7265 7365 6172  oing good resear
+00000490: 6368 2e0d 0a0d 0a44 6565 7050 6f73 654b  ch.....DeepPoseK
+000004a0: 6974 2069 7320 6375 7272 656e 746c 7920  it is currently 
+000004b0: 6c69 6d69 7465 6420 746f 202a 696e 6469  limited to *indi
+000004c0: 7669 6475 616c 2070 6f73 6520 6573 7469  vidual pose esti
+000004d0: 6d61 7469 6f6e 2a2e 2049 6620 696e 6469  mation*. If indi
+000004e0: 7669 6475 616c 7320 6361 6e20 6265 2065  viduals can be e
+000004f0: 6173 696c 7920 6469 7374 696e 6775 6973  asily distinguis
+00000500: 6865 6420 7669 7375 616c 6c79 2028 692e  hed visually (i.
+00000510: 652e 2c20 7468 6579 2068 6176 6520 6469  e., they have di
+00000520: 6666 6572 656e 746c 7920 636f 6c6f 7265  fferently colore
+00000530: 6420 626f 6469 6573 206f 7220 6172 6520  d bodies or are 
+00000540: 6d61 726b 6564 2069 6e20 736f 6d65 2077  marked in some w
+00000550: 6179 292c 2074 6865 6e20 6d75 6c74 6970  ay), then multip
+00000560: 6c65 2069 6e64 6976 6964 7561 6c73 2063  le individuals c
+00000570: 616e 2073 696d 706c 7920 6265 206c 6162  an simply be lab
+00000580: 656c 6564 2077 6974 6820 7365 7061 7261  eled with separa
+00000590: 7465 206b 6579 706f 696e 7473 2028 6865  te keypoints (he
+000005a0: 6164 312c 2074 6169 6c31 2c20 6865 6164  ad1, tail1, head
+000005b0: 322c 2074 6169 6c32 2c20 6574 632e 292e  2, tail2, etc.).
+000005c0: 204f 7468 6572 7769 7365 2044 6565 7050   Otherwise DeepP
+000005d0: 6f73 654b 6974 2063 616e 2062 6520 6578  oseKit can be ex
+000005e0: 7465 6e64 6564 2074 6f20 6d75 6c74 6970  tended to multip
+000005f0: 6c65 2069 6e64 6976 6964 7561 6c73 2062  le individuals b
+00000600: 7920 6669 7273 7420 6c6f 6361 6c69 7a69  y first localizi
+00000610: 6e67 2c20 7472 6163 6b69 6e67 2c20 616e  ng, tracking, an
+00000620: 6420 6372 6f70 7069 6e67 2069 6e64 6976  d cropping indiv
+00000630: 6964 7561 6c73 2077 6974 6820 6164 6469  iduals with addi
+00000640: 7469 6f6e 616c 2073 6f66 7477 6172 6520  tional software 
+00000650: 7375 6368 2061 7320 5b69 6474 7261 636b  such as [idtrack
+00000660: 6572 2e61 695d 2868 7474 7073 3a2f 2f69  er.ai](https://i
+00000670: 6474 7261 636b 6572 2e61 692f 292c 205b  dtracker.ai/), [
+00000680: 7069 6e70 6f69 6e74 5d28 6874 7470 733a  pinpoint](https:
+00000690: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6772  //github.com/jgr
+000006a0: 6176 696e 672f 7069 6e70 6f69 6e74 292c  aving/pinpoint),
+000006b0: 206f 7220 5b54 7261 636b 746f 725d 2868   or [Tracktor](h
+000006c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000006d0: 6d2f 7669 7665 6b68 7372 6964 6861 722f  m/vivekhsridhar/
+000006e0: 7472 6163 6b74 6f72 292e 0d0a 0d0a 4c6f  tracktor).....Lo
+000006f0: 6361 6c69 7a61 7469 6f6e 2028 7769 7468  calization (with
+00000700: 6f75 7420 7472 6163 6b69 6e67 2920 6361  out tracking) ca
+00000710: 6e20 616c 736f 2062 6520 6163 6869 6576  n also be achiev
+00000720: 6564 2077 6974 6820 6465 6570 206c 6561  ed with deep lea
+00000730: 726e 696e 6720 736f 6674 7761 7265 206c  rning software l
+00000740: 696b 6520 5b6b 6572 6173 2d72 6574 696e  ike [keras-retin
+00000750: 616e 6574 5d28 6874 7470 733a 2f2f 6769  anet](https://gi
+00000760: 7468 7562 2e63 6f6d 2f66 697a 7972 2f6b  thub.com/fizyr/k
+00000770: 6572 6173 2d72 6574 696e 616e 6574 292c  eras-retinanet),
+00000780: 2074 6865 205b 5465 6e73 6f72 666c 6f77   the [Tensorflow
+00000790: 204f 626a 6563 7420 4465 7465 6374 696f   Object Detectio
+000007a0: 6e20 4150 495d 2868 7474 7073 3a2f 2f67  n API](https://g
+000007b0: 6974 6875 622e 636f 6d2f 7465 6e73 6f72  ithub.com/tensor
+000007c0: 666c 6f77 2f6d 6f64 656c 732f 7472 6565  flow/models/tree
+000007d0: 2f6d 6173 7465 722f 7265 7365 6172 6368  /master/research
+000007e0: 2f6f 626a 6563 745f 6465 7465 6374 696f  /object_detectio
+000007f0: 6e29 2c20 6f72 205b 4d61 7474 6572 506f  n), or [MatterPo
+00000800: 7274 2773 204d 6173 6b20 522d 434e 4e5d  rt's Mask R-CNN]
+00000810: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000820: 636f 6d2f 6d61 7474 6572 706f 7274 2f4d  com/matterport/M
+00000830: 6173 6b5f 5243 4e4e 292e 0d0a 0d0a 5b43  ask_RCNN).....[C
+00000840: 6865 636b 206f 7574 206f 7572 2070 6170  heck out our pap
+00000850: 6572 5d28 6874 7470 733a 2f2f 646f 692e  er](https://doi.
+00000860: 6f72 672f 3130 2e37 3535 342f 654c 6966  org/10.7554/eLif
+00000870: 652e 3437 3939 3429 2074 6f20 6669 6e64  e.47994) to find
+00000880: 206f 7574 206d 6f72 652e 0d0a 0d0a 3c70   out more.....<p
+00000890: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+000008a0: 0d0a 3c69 6d67 2073 7263 3d22 6874 7470  ..<img src="http
+000008b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+000008c0: 6772 6176 696e 672f 6a67 7261 7669 6e67  graving/jgraving
+000008d0: 2e67 6974 6875 622e 696f 2f62 6c6f 622f  .github.io/blob/
+000008e0: 6d61 7374 6572 2f66 696c 6573 2f69 6d61  master/files/ima
+000008f0: 6765 732f 7a65 6272 612e 6769 6622 2068  ges/zebra.gif" h
+00000900: 6569 6768 743d 2232 3536 7078 223e 0d0a  eight="256px">..
+00000910: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000920: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6772  //github.com/jgr
+00000930: 6176 696e 672f 6a67 7261 7669 6e67 2e67  aving/jgraving.g
+00000940: 6974 6875 622e 696f 2f62 6c6f 622f 6d61  ithub.io/blob/ma
+00000950: 7374 6572 2f66 696c 6573 2f69 6d61 6765  ster/files/image
+00000960: 732f 6c6f 6375 7374 2e67 6966 2220 6865  s/locust.gif" he
+00000970: 6967 6874 3d22 3235 3670 7822 3e0d 0a3c  ight="256px">..<
+00000980: 2f70 3e0d 0a0d 0a23 2048 6f77 2074 6f20  /p>....# How to 
+00000990: 7573 6520 4465 6570 506f 7365 4b69 740d  use DeepPoseKit.
+000009a0: 0a0d 0a44 6565 7050 6f73 654b 6974 2069  ...DeepPoseKit i
+000009b0: 7320 6465 7369 676e 6564 2066 6f72 2065  s designed for e
+000009c0: 6173 7920 7573 652e 2046 6f72 2065 7861  asy use. For exa
+000009d0: 6d70 6c65 2c20 7472 6169 6e69 6e67 2061  mple, training a
+000009e0: 6e64 2073 6176 696e 6720 6120 6d6f 6465  nd saving a mode
+000009f0: 6c20 7265 7175 6972 6573 206f 6e6c 7920  l requires only 
+00000a00: 6120 6665 7720 6c69 6e65 7320 6f66 2063  a few lines of c
+00000a10: 6f64 653a 0d0a 6060 6070 7974 686f 6e0d  ode:..```python.
+00000a20: 0a66 726f 6d20 6465 6570 706f 7365 6b69  .from deepposeki
+00000a30: 742e 696f 2069 6d70 6f72 7420 4461 7461  t.io import Data
+00000a40: 4765 6e65 7261 746f 722c 2054 7261 696e  Generator, Train
+00000a50: 696e 6747 656e 6572 6174 6f72 0d0a 6672  ingGenerator..fr
+00000a60: 6f6d 2064 6565 7070 6f73 656b 6974 2e6d  om deepposekit.m
+00000a70: 6f64 656c 7320 696d 706f 7274 2053 7461  odels import Sta
+00000a80: 636b 6564 4465 6e73 654e 6574 0d0a 0d0a  ckedDenseNet....
+00000a90: 6461 7461 5f67 656e 6572 6174 6f72 203d  data_generator =
+00000aa0: 2044 6174 6147 656e 6572 6174 6f72 2827   DataGenerator('
+00000ab0: 2f70 6174 682f 746f 2f61 6e6e 6f74 6174  /path/to/annotat
+00000ac0: 696f 6e5f 6461 7461 2e68 3527 290d 0a74  ion_data.h5')..t
+00000ad0: 7261 696e 5f67 656e 6572 6174 6f72 203d  rain_generator =
+00000ae0: 2054 7261 696e 696e 6747 656e 6572 6174   TrainingGenerat
+00000af0: 6f72 2864 6174 615f 6765 6e65 7261 746f  or(data_generato
+00000b00: 7229 0d0a 6d6f 6465 6c20 3d20 5374 6163  r)..model = Stac
+00000b10: 6b65 6444 656e 7365 4e65 7428 7472 6169  kedDenseNet(trai
+00000b20: 6e5f 6765 6e65 7261 746f 7229 0d0a 6d6f  n_generator)..mo
+00000b30: 6465 6c2e 6669 7428 6261 7463 685f 7369  del.fit(batch_si
+00000b40: 7a65 3d31 362c 206e 5f77 6f72 6b65 7273  ze=16, n_workers
+00000b50: 3d38 290d 0a6d 6f64 656c 2e73 6176 6528  =8)..model.save(
+00000b60: 272f 7061 7468 2f74 6f2f 7361 7665 645f  '/path/to/saved_
+00000b70: 6d6f 6465 6c2e 6835 2729 0d0a 6060 600d  model.h5')..```.
+00000b80: 0a4c 6f61 6469 6e67 2061 2074 7261 696e  .Loading a train
+00000b90: 6564 206d 6f64 656c 2061 6e64 2072 756e  ed model and run
+00000ba0: 6e69 6e67 2070 7265 6469 6374 696f 6e73  ning predictions
+00000bb0: 206f 6e20 6e65 7720 6461 7461 2069 7320   on new data is 
+00000bc0: 616c 736f 2073 7472 6169 6768 7466 6f72  also straightfor
+00000bd0: 7761 7264 2e20 466f 7220 6578 616d 706c  ward. For exampl
+00000be0: 652c 2072 756e 6e69 6e67 2070 7265 6469  e, running predi
+00000bf0: 6374 696f 6e73 206f 6e20 6120 6e65 7720  ctions on a new 
+00000c00: 7669 6465 6f3a 0d0a 6060 6070 7974 686f  video:..```pytho
+00000c10: 6e0d 0a66 726f 6d20 6465 6570 706f 7365  n..from deeppose
+00000c20: 6b69 742e 6d6f 6465 6c73 2069 6d70 6f72  kit.models impor
+00000c30: 7420 6c6f 6164 5f6d 6f64 656c 0d0a 6672  t load_model..fr
+00000c40: 6f6d 2064 6565 7070 6f73 656b 6974 2e69  om deepposekit.i
+00000c50: 6f20 696d 706f 7274 2056 6964 656f 5265  o import VideoRe
+00000c60: 6164 6572 0d0a 0d0a 6d6f 6465 6c20 3d20  ader....model = 
+00000c70: 6c6f 6164 5f6d 6f64 656c 2827 2f70 6174  load_model('/pat
+00000c80: 682f 746f 2f73 6176 6564 5f6d 6f64 656c  h/to/saved_model
+00000c90: 2e68 3527 290d 0a72 6561 6465 7220 3d20  .h5')..reader = 
+00000ca0: 5669 6465 6f52 6561 6465 7228 272f 7061  VideoReader('/pa
+00000cb0: 7468 2f74 6f2f 7669 6465 6f2e 6d70 3427  th/to/video.mp4'
+00000cc0: 290d 0a70 7265 6469 6374 696f 6e73 203d  )..predictions =
+00000cd0: 206d 6f64 656c 2e70 7265 6469 6374 2872   model.predict(r
+00000ce0: 6561 6465 7229 0d0a 6060 600d 0a0d 0a23  eader)..```....#
+00000cf0: 2320 5573 696e 6720 4465 6570 506f 7365  # Using DeepPose
+00000d00: 4b69 7420 6973 2061 2034 2d73 7465 7020  Kit is a 4-step 
+00000d10: 7072 6f63 6573 733a 0d0a 0d0a 2d20 2a2a  process:....- **
+00000d20: 312e 2a2a 205b 4372 6561 7465 2061 6e20  1.** [Create an 
+00000d30: 616e 6e6f 7461 7469 6f6e 2073 6574 5d28  annotation set](
+00000d40: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000d50: 6f6d 2f6a 6772 6176 696e 672f 4465 6570  om/jgraving/Deep
+00000d60: 506f 7365 4b69 742f 626c 6f62 2f6d 6173  PoseKit/blob/mas
+00000d70: 7465 722f 6578 616d 706c 6573 2f73 7465  ter/examples/ste
+00000d80: 7031 5f63 7265 6174 655f 616e 6e6f 7461  p1_create_annota
+00000d90: 7469 6f6e 5f73 6574 2e69 7079 6e62 2920  tion_set.ipynb) 
+00000da0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000db0: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
+00000dc0: 676f 6f67 6c65 2e63 6f6d 2f67 6974 6875  google.com/githu
+00000dd0: 622f 6a67 7261 7669 6e67 2f64 6565 7070  b/jgraving/deepp
+00000de0: 6f73 656b 6974 2f62 6c6f 622f 6d61 7374  osekit/blob/mast
+00000df0: 6572 2f65 7861 6d70 6c65 732f 7374 6570  er/examples/step
+00000e00: 315f 6372 6561 7465 5f61 6e6e 6f74 6174  1_create_annotat
+00000e10: 696f 6e5f 7365 742e 6970 796e 6222 2074  ion_set.ipynb" t
+00000e20: 6172 6765 743d 225f 7061 7265 6e74 223e  arget="_parent">
+00000e30: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000e40: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+00000e50: 2e67 6f6f 676c 652e 636f 6d2f 6173 7365  .google.com/asse
+00000e60: 7473 2f63 6f6c 6162 2d62 6164 6765 2e73  ts/colab-badge.s
+00000e70: 7667 2220 616c 743d 224f 7065 6e20 496e  vg" alt="Open In
+00000e80: 2043 6f6c 6162 222f 3e3c 2f61 3e0d 0a2d   Colab"/></a>..-
+00000e90: 202a 2a32 2e2a 2a20 5b41 6e6e 6f74 6174   **2.** [Annotat
+00000ea0: 6520 796f 7572 2064 6174 615d 2868 7474  e your data](htt
+00000eb0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000ec0: 6a67 7261 7669 6e67 2f44 6565 7050 6f73  jgraving/DeepPos
+00000ed0: 654b 6974 2f62 6c6f 622f 6d61 7374 6572  eKit/blob/master
+00000ee0: 2f65 7861 6d70 6c65 732f 7374 6570 325f  /examples/step2_
+00000ef0: 616e 6e6f 7461 7465 5f64 6174 612e 6970  annotate_data.ip
+00000f00: 796e 6229 2077 6974 6820 6f75 7220 6275  ynb) with our bu
+00000f10: 696c 742d 696e 2047 5549 2028 6e6f 2043  ilt-in GUI (no C
+00000f20: 6f6c 6162 2073 7570 706f 7274 290d 0a2d  olab support)..-
+00000f30: 202a 2a33 2e2a 2a20 5b53 656c 6563 7420   **3.** [Select 
+00000f40: 616e 6420 7472 6169 6e5d 2868 7474 7073  and train](https
+00000f50: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a67  ://github.com/jg
+00000f60: 7261 7669 6e67 2f44 6565 7050 6f73 654b  raving/DeepPoseK
+00000f70: 6974 2f62 6c6f 622f 6d61 7374 6572 2f65  it/blob/master/e
+00000f80: 7861 6d70 6c65 732f 7374 6570 335f 7472  xamples/step3_tr
+00000f90: 6169 6e5f 6d6f 6465 6c2e 6970 796e 6229  ain_model.ipynb)
+00000fa0: 206f 6e65 206f 7572 205b 706f 7365 2065   one our [pose e
+00000fb0: 7374 696d 6174 696f 6e20 6d6f 6465 6c73  stimation models
+00000fc0: 5d28 6874 7470 3a2f 2f6a 616b 6567 7261  ](http://jakegra
+00000fd0: 7669 6e67 2e63 6f6d 2f44 6565 7050 6f73  ving.com/DeepPos
+00000fe0: 654b 6974 2f68 746d 6c2f 6465 6570 706f  eKit/html/deeppo
+00000ff0: 7365 6b69 742f 6d6f 6465 6c73 2f69 6e64  sekit/models/ind
+00001000: 6578 2e68 746d 6c29 2069 6e63 6c75 6469  ex.html) includi
+00001010: 6e67 205b 6053 7461 636b 6564 4465 6e73  ng [`StackedDens
+00001020: 654e 6574 605d 2868 7474 703a 2f2f 6a61  eNet`](http://ja
+00001030: 6b65 6772 6176 696e 672e 636f 6d2f 4465  kegraving.com/De
+00001040: 6570 506f 7365 4b69 742f 6874 6d6c 2f64  epPoseKit/html/d
+00001050: 6565 7070 6f73 656b 6974 2f6d 6f64 656c  eepposekit/model
+00001060: 732f 5374 6163 6b65 6444 656e 7365 4e65  s/StackedDenseNe
+00001070: 742e 6874 6d6c 292c 205b 6053 7461 636b  t.html), [`Stack
+00001080: 6564 486f 7572 676c 6173 7360 5d28 6874  edHourglass`](ht
+00001090: 7470 3a2f 2f6a 616b 6567 7261 7669 6e67  tp://jakegraving
+000010a0: 2e63 6f6d 2f44 6565 7050 6f73 654b 6974  .com/DeepPoseKit
+000010b0: 2f68 746d 6c2f 6465 6570 706f 7365 6b69  /html/deepposeki
+000010c0: 742f 6d6f 6465 6c73 2f53 7461 636b 6564  t/models/Stacked
+000010d0: 486f 7572 676c 6173 732e 6874 6d6c 292c  Hourglass.html),
+000010e0: 205b 6044 6565 704c 6162 4375 7460 5d28   [`DeepLabCut`](
+000010f0: 6874 7470 3a2f 2f6a 616b 6567 7261 7669  http://jakegravi
+00001100: 6e67 2e63 6f6d 2f44 6565 7050 6f73 654b  ng.com/DeepPoseK
+00001110: 6974 2f68 746d 6c2f 6465 6570 706f 7365  it/html/deeppose
+00001120: 6b69 742f 6d6f 6465 6c73 2f44 6565 704c  kit/models/DeepL
+00001130: 6162 4375 742e 6874 6d6c 292c 2061 6e64  abCut.html), and
+00001140: 205b 604c 4541 5060 5d28 6874 7470 3a2f   [`LEAP`](http:/
+00001150: 2f6a 616b 6567 7261 7669 6e67 2e63 6f6d  /jakegraving.com
+00001160: 2f44 6565 7050 6f73 654b 6974 2f68 746d  /DeepPoseKit/htm
+00001170: 6c2f 6465 6570 706f 7365 6b69 742f 6d6f  l/deepposekit/mo
+00001180: 6465 6c73 2f4c 4541 502e 6874 6d6c 292e  dels/LEAP.html).
+00001190: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000011a0: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+000011b0: 2e67 6f6f 676c 652e 636f 6d2f 6769 7468  .google.com/gith
+000011c0: 7562 2f6a 6772 6176 696e 672f 6465 6570  ub/jgraving/deep
+000011d0: 706f 7365 6b69 742f 626c 6f62 2f6d 6173  posekit/blob/mas
+000011e0: 7465 722f 6578 616d 706c 6573 2f73 7465  ter/examples/ste
+000011f0: 7033 5f74 7261 696e 5f6d 6f64 656c 2e69  p3_train_model.i
+00001200: 7079 6e62 2220 7461 7267 6574 3d22 5f70  pynb" target="_p
+00001210: 6172 656e 7422 3e3c 696d 6720 7372 633d  arent"><img src=
+00001220: 2268 7474 7073 3a2f 2f63 6f6c 6162 2e72  "https://colab.r
+00001230: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+00001240: 6f6d 2f61 7373 6574 732f 636f 6c61 622d  om/assets/colab-
+00001250: 6261 6467 652e 7376 6722 2061 6c74 3d22  badge.svg" alt="
+00001260: 4f70 656e 2049 6e20 436f 6c61 6222 2f3e  Open In Colab"/>
+00001270: 3c2f 613e 0d0a 2d20 2a2a 342e 2a2a 2055  </a>..- **4.** U
+00001280: 7365 2074 6865 2074 7261 696e 6564 206d  se the trained m
+00001290: 6f64 656c 2074 6f3a 0d0a 092d 2061 2920  odel to:...- a) 
+000012a0: 5b49 6e69 7469 616c 697a 6520 6b65 7970  [Initialize keyp
+000012b0: 6f69 6e74 7320 666f 7220 756e 616e 6e6f  oints for unanno
+000012c0: 7461 7465 6420 6461 7461 5d28 6874 7470  tated data](http
+000012d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+000012e0: 6772 6176 696e 672f 4465 6570 506f 7365  graving/DeepPose
+000012f0: 4b69 742f 626c 6f62 2f6d 6173 7465 722f  Kit/blob/master/
+00001300: 6578 616d 706c 6573 2f73 7465 7034 615f  examples/step4a_
+00001310: 696e 6974 6961 6c69 7a65 5f61 6e6e 6f74  initialize_annot
+00001320: 6174 696f 6e73 2e69 7079 6e62 2920 666f  ations.ipynb) fo
+00001330: 7220 6661 7374 6572 2061 6e6e 6f74 6174  r faster annotat
+00001340: 696f 6e73 2077 6974 6820 2a61 6374 6976  ions with *activ
+00001350: 6520 6c65 6172 6e69 6e67 2a2e 203c 6120  e learning*. <a 
+00001360: 6872 6566 3d22 6874 7470 733a 2f2f 636f  href="https://co
+00001370: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
+00001380: 676c 652e 636f 6d2f 6769 7468 7562 2f6a  gle.com/github/j
+00001390: 6772 6176 696e 672f 6465 6570 706f 7365  graving/deeppose
+000013a0: 6b69 742f 626c 6f62 2f6d 6173 7465 722f  kit/blob/master/
+000013b0: 6578 616d 706c 6573 2f73 7465 7034 615f  examples/step4a_
+000013c0: 696e 6974 6961 6c69 7a65 5f61 6e6e 6f74  initialize_annot
+000013d0: 6174 696f 6e73 2e69 7079 6e62 2220 7461  ations.ipynb" ta
+000013e0: 7267 6574 3d22 5f70 6172 656e 7422 3e3c  rget="_parent"><
+000013f0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001400: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
+00001410: 676f 6f67 6c65 2e63 6f6d 2f61 7373 6574  google.com/asset
+00001420: 732f 636f 6c61 622d 6261 6467 652e 7376  s/colab-badge.sv
+00001430: 6722 2061 6c74 3d22 4f70 656e 2049 6e20  g" alt="Open In 
+00001440: 436f 6c61 6222 2f3e 3c2f 613e 0d0a 092d  Colab"/></a>...-
+00001450: 2062 2920 5b50 7265 6469 6374 206f 6e20   b) [Predict on 
+00001460: 6e65 7720 6461 7461 2061 6e64 2072 6566  new data and ref
+00001470: 696e 6520 7468 6520 7472 6169 6e69 6e67  ine the training
+00001480: 2073 6574 5d28 6874 7470 733a 2f2f 6769   set](https://gi
+00001490: 7468 7562 2e63 6f6d 2f6a 6772 6176 696e  thub.com/jgravin
+000014a0: 672f 4465 6570 506f 7365 4b69 742f 626c  g/DeepPoseKit/bl
+000014b0: 6f62 2f6d 6173 7465 722f 6578 616d 706c  ob/master/exampl
+000014c0: 6573 2f73 7465 7034 625f 7072 6564 6963  es/step4b_predic
+000014d0: 745f 6e65 775f 6461 7461 2e69 7079 6e62  t_new_data.ipynb
+000014e0: 2920 746f 2069 6d70 726f 7665 2070 6572  ) to improve per
+000014f0: 666f 726d 616e 6365 2e20 3c61 2068 7265  formance. <a hre
+00001500: 663d 2268 7474 7073 3a2f 2f63 6f6c 6162  f="https://colab
+00001510: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+00001520: 2e63 6f6d 2f67 6974 6875 622f 6a67 7261  .com/github/jgra
+00001530: 7669 6e67 2f64 6565 7070 6f73 656b 6974  ving/deepposekit
+00001540: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
+00001550: 6d70 6c65 732f 7374 6570 3462 5f70 7265  mples/step4b_pre
+00001560: 6469 6374 5f6e 6577 5f64 6174 612e 6970  dict_new_data.ip
+00001570: 796e 6222 2074 6172 6765 743d 225f 7061  ynb" target="_pa
+00001580: 7265 6e74 223e 3c69 6d67 2073 7263 3d22  rent"><img src="
+00001590: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
+000015a0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
+000015b0: 6d2f 6173 7365 7473 2f63 6f6c 6162 2d62  m/assets/colab-b
+000015c0: 6164 6765 2e73 7667 2220 616c 743d 224f  adge.svg" alt="O
+000015d0: 7065 6e20 496e 2043 6f6c 6162 222f 3e3c  pen In Colab"/><
+000015e0: 2f61 3e0d 0a0d 0a23 2320 466f 7220 6d6f  /a>....## For mo
+000015f0: 7265 2064 6574 6169 6c73 3a0d 0a0d 0a2d  re details:....-
+00001600: 2053 6565 205b 6f75 7220 6578 616d 706c   See [our exampl
+00001610: 6520 6e6f 7465 626f 6f6b 735d 2868 7474  e notebooks](htt
+00001620: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001630: 6a67 7261 7669 6e67 2f64 6565 7070 6f73  jgraving/deeppos
+00001640: 656b 6974 2f62 6c6f 622f 6d61 7374 6572  ekit/blob/master
+00001650: 2f65 7861 6d70 6c65 732f 290d 0a2d 2043  /examples/)..- C
+00001660: 6865 636b 2074 6865 205b 646f 6375 6d65  heck the [docume
+00001670: 6e74 6174 696f 6e5d 2868 7474 703a 2f2f  ntation](http://
+00001680: 646f 6373 2e64 6565 7070 6f73 656b 6974  docs.deepposekit
+00001690: 2e6f 7267 290d 0a2d 2052 6561 6420 5b6f  .org)..- Read [o
+000016a0: 7572 2070 6170 6572 5d28 6874 7470 733a  ur paper](https:
+000016b0: 2f2f 646f 692e 6f72 672f 3130 2e37 3535  //doi.org/10.755
+000016c0: 342f 654c 6966 652e 3437 3939 3429 0d0a  4/eLife.47994)..
+000016d0: 0d0a 2323 2022 4920 616c 7265 6164 7920  ..## "I already 
+000016e0: 6861 7665 2061 6e6e 6f74 6174 6564 2064  have annotated d
+000016f0: 6174 6122 0d0a 0d0a 4465 6570 506f 7365  ata"....DeepPose
+00001700: 4b69 7420 6973 2064 6573 6967 6e65 6420  Kit is designed 
+00001710: 746f 2062 6520 6578 7465 6e73 6962 6c65  to be extensible
+00001720: 2c20 736f 206c 6f61 6469 6e67 2064 6174  , so loading dat
+00001730: 6120 696e 206f 7468 6572 2066 6f72 6d61  a in other forma
+00001740: 7473 2069 7320 706f 7373 6962 6c65 2e0d  ts is possible..
+00001750: 0a0d 0a49 6620 796f 7520 6861 7665 2061  ...If you have a
+00001760: 6e6e 6f74 6174 6564 2064 6174 6120 6672  nnotated data fr
+00001770: 6f6d 2044 6565 704c 6162 4375 7420 2868  om DeepLabCut (h
+00001780: 7474 703a 2f2f 6465 6570 6c61 6263 7574  ttp://deeplabcut
+00001790: 2e6f 7267 292c 2074 7279 205b 6f75 7220  .org), try [our 
+000017a0: 2865 7870 6572 696d 656e 7461 6c29 2065  (experimental) e
+000017b0: 7861 6d70 6c65 206e 6f74 6562 6f6f 6b20  xample notebook 
+000017c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000017d0: 2e63 6f6d 2f6a 6772 6176 696e 672f 4465  .com/jgraving/De
+000017e0: 6570 506f 7365 4b69 742f 626c 6f62 2f6d  epPoseKit/blob/m
+000017f0: 6173 7465 722f 6578 616d 706c 6573 2f64  aster/examples/d
+00001800: 6565 706c 6162 6375 745f 6461 7461 5f65  eeplabcut_data_e
+00001810: 7861 6d70 6c65 2e69 7079 6e62 2920 666f  xample.ipynb) fo
+00001820: 7220 6c6f 6164 696e 6720 6461 7461 2069  r loading data i
+00001830: 6e20 7468 6973 2066 6f72 6d61 742e 203c  n this format. <
+00001840: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001850: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+00001860: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
+00001870: 2f6a 6772 6176 696e 672f 6465 6570 706f  /jgraving/deeppo
+00001880: 7365 6b69 742f 626c 6f62 2f6d 6173 7465  sekit/blob/maste
+00001890: 722f 6578 616d 706c 6573 2f64 6565 706c  r/examples/deepl
+000018a0: 6162 6375 745f 6461 7461 5f65 7861 6d70  abcut_data_examp
+000018b0: 6c65 2e69 7079 6e62 2220 7461 7267 6574  le.ipynb" target
+000018c0: 3d22 5f70 6172 656e 7422 3e3c 696d 6720  ="_parent"><img 
+000018d0: 7372 633d 2268 7474 7073 3a2f 2f63 6f6c  src="https://col
+000018e0: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
+000018f0: 6c65 2e63 6f6d 2f61 7373 6574 732f 636f  le.com/assets/co
+00001900: 6c61 622d 6261 6467 652e 7376 6722 2061  lab-badge.svg" a
+00001910: 6c74 3d22 4f70 656e 2049 6e20 436f 6c61  lt="Open In Cola
+00001920: 6222 2f3e 3c2f 613e 0d0a 0d0a 4861 7665  b"/></a>....Have
+00001930: 2064 6174 6120 696e 2061 6e6f 7468 6572   data in another
+00001940: 2066 6f72 6d61 743f 2059 6f75 2063 616e   format? You can
+00001950: 2077 7269 7465 2079 6f75 7220 6f77 6e20   write your own 
+00001960: 6375 7374 6f6d 2067 656e 6572 6174 6f72  custom generator
+00001970: 2074 6f20 6c6f 6164 2069 742e 0d0a 4368   to load it...Ch
+00001980: 6563 6b20 6f75 7420 7468 6520 5b65 7861  eck out the [exa
+00001990: 6d70 6c65 2066 6f72 2077 7269 7469 6e67  mple for writing
+000019a0: 2063 7573 746f 6d20 6461 7461 2067 656e   custom data gen
+000019b0: 6572 6174 6f72 735d 2868 7474 7073 3a2f  erators](https:/
+000019c0: 2f67 6974 6875 622e 636f 6d2f 6a67 7261  /github.com/jgra
+000019d0: 7669 6e67 2f44 6565 7050 6f73 654b 6974  ving/DeepPoseKit
+000019e0: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
+000019f0: 6d70 6c65 732f 6375 7374 6f6d 5f64 6174  mples/custom_dat
+00001a00: 615f 6765 6e65 7261 746f 722e 6970 796e  a_generator.ipyn
+00001a10: 6229 2e20 3c61 2068 7265 663d 2268 7474  b). <a href="htt
+00001a20: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+00001a30: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f67  rch.google.com/g
+00001a40: 6974 6875 622f 6a67 7261 7669 6e67 2f64  ithub/jgraving/d
+00001a50: 6565 7070 6f73 656b 6974 2f62 6c6f 622f  eepposekit/blob/
+00001a60: 6d61 7374 6572 2f65 7861 6d70 6c65 732f  master/examples/
+00001a70: 6375 7374 6f6d 5f64 6174 615f 6765 6e65  custom_data_gene
+00001a80: 7261 746f 722e 6970 796e 6222 2074 6172  rator.ipynb" tar
+00001a90: 6765 743d 225f 7061 7265 6e74 223e 3c69  get="_parent"><i
+00001aa0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00001ab0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
+00001ac0: 6f6f 676c 652e 636f 6d2f 6173 7365 7473  oogle.com/assets
+00001ad0: 2f63 6f6c 6162 2d62 6164 6765 2e73 7667  /colab-badge.svg
+00001ae0: 2220 616c 743d 224f 7065 6e20 496e 2043  " alt="Open In C
+00001af0: 6f6c 6162 222f 3e3c 2f61 3e0d 0a0d 0a23  olab"/></a>....#
+00001b00: 2049 6e73 7461 6c6c 6174 696f 6e0d 0a0d   Installation...
+00001b10: 0a44 6565 7050 6f73 654b 6974 2072 6571  .DeepPoseKit req
+00001b20: 7569 7265 7320 5b54 656e 736f 7266 6c6f  uires [Tensorflo
+00001b30: 775d 2868 7474 7073 3a2f 2f67 6974 6875  w](https://githu
+00001b40: 622e 636f 6d2f 7465 6e73 6f72 666c 6f77  b.com/tensorflow
+00001b50: 2f74 656e 736f 7266 6c6f 7729 2066 6f72  /tensorflow) for
+00001b60: 2074 7261 696e 696e 6720 616e 6420 7573   training and us
+00001b70: 696e 6720 706f 7365 2065 7374 696d 6174  ing pose estimat
+00001b80: 696f 6e20 6d6f 6465 6c73 2e20 5b54 656e  ion models. [Ten
+00001b90: 736f 7266 6c6f 775d 2868 7474 7073 3a2f  sorflow](https:/
+00001ba0: 2f67 6974 6875 622e 636f 6d2f 7465 6e73  /github.com/tens
+00001bb0: 6f72 666c 6f77 2f74 656e 736f 7266 6c6f  orflow/tensorflo
+00001bc0: 7729 2073 686f 756c 6420 6265 206d 616e  w) should be man
+00001bd0: 7561 6c6c 7920 696e 7374 616c 6c65 642c  ually installed,
+00001be0: 2061 6c6f 6e67 2077 6974 6820 6465 7065   along with depe
+00001bf0: 6e64 656e 6369 6573 2073 7563 6820 6173  ndencies such as
+00001c00: 2043 5544 4120 616e 6420 6375 444e 4e2c   CUDA and cuDNN,
+00001c10: 2062 6566 6f72 6520 696e 7374 616c 6c69   before installi
+00001c20: 6e67 2044 6565 7050 6f73 654b 6974 3a0d  ng DeepPoseKit:.
+00001c30: 0a0d 0a2d 205b 5465 6e73 6f72 666c 6f77  ...- [Tensorflow
+00001c40: 2049 6e73 7461 6c6c 6174 696f 6e20 496e   Installation In
+00001c50: 7374 7275 6374 696f 6e73 5d28 6874 7470  structions](http
+00001c60: 733a 2f2f 7777 772e 7465 6e73 6f72 666c  s://www.tensorfl
+00001c70: 6f77 2e6f 7267 2f69 6e73 7461 6c6c 290d  ow.org/install).
+00001c80: 0a2d 2041 6e79 2054 656e 736f 7266 6c6f  .- Any Tensorflo
+00001c90: 7720 7665 7273 696f 6e20 3e3d 312e 3133  w version >=1.13
+00001ca0: 2e30 2073 686f 756c 6420 6265 2063 6f6d  .0 should be com
+00001cb0: 7061 7469 626c 6520 2869 6e63 6c75 6469  patible (includi
+00001cc0: 6e67 2032 2e30 292e 0d0a 0d0a 4465 6570  ng 2.0).....Deep
+00001cd0: 506f 7365 4b69 7420 6861 7320 6f6e 6c79  PoseKit has only
+00001ce0: 2062 6565 6e20 7465 7374 6564 206f 6e20   been tested on 
+00001cf0: 5562 756e 7475 2031 382e 3034 2c20 7768  Ubuntu 18.04, wh
+00001d00: 6963 6820 6973 2074 6865 2072 6563 6f6d  ich is the recom
+00001d10: 6d65 6e64 6564 2073 7973 7465 6d20 666f  mended system fo
+00001d20: 7220 7573 696e 6720 7468 6520 746f 6f6c  r using the tool
+00001d30: 6b69 742e 200d 0a0d 0a49 6e73 7461 6c6c  kit. ....Install
+00001d40: 2074 6865 206c 6174 6573 7420 7374 6162   the latest stab
+00001d50: 6c65 2072 656c 6561 7365 2077 6974 6820  le release with 
+00001d60: 7069 703a 0d0a 6060 6062 6173 680d 0a70  pip:..```bash..p
+00001d70: 6970 2069 6e73 7461 6c6c 202d 2d75 7064  ip install --upd
+00001d80: 6174 6520 6465 6570 706f 7365 6b69 740d  ate deepposekit.
+00001d90: 0a60 6060 0d0a 0d0a 496e 7374 616c 6c20  .```....Install 
+00001da0: 7468 6520 6c61 7465 7374 2064 6576 656c  the latest devel
+00001db0: 6f70 6d65 6e74 2076 6572 7369 6f6e 2077  opment version w
+00001dc0: 6974 6820 7069 703a 0d0a 6060 6062 6173  ith pip:..```bas
+00001dd0: 680d 0a70 6970 2069 6e73 7461 6c6c 202d  h..pip install -
+00001de0: 2d75 7064 6174 6520 6769 742b 6874 7470  -update git+http
+00001df0: 733a 2f2f 7777 772e 6769 7468 7562 2e63  s://www.github.c
+00001e00: 6f6d 2f6a 6772 6176 696e 672f 6465 6570  om/jgraving/deep
+00001e10: 706f 7365 6b69 742e 6769 740d 0a60 6060  posekit.git..```
+00001e20: 0d0a 0d0a 596f 7520 6361 6e20 646f 776e  ....You can down
+00001e30: 6c6f 6164 2065 7861 6d70 6c65 2064 6174  load example dat
+00001e40: 6173 6574 7320 6672 6f6d 206f 7572 205b  asets from our [
+00001e50: 4465 6570 506f 7365 4b69 7420 4461 7461  DeepPoseKit Data
+00001e60: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001e70: 2e63 6f6d 2f6a 6772 6176 696e 672f 6465  .com/jgraving/de
+00001e80: 6570 706f 7365 6b69 742d 6461 7461 2920  epposekit-data) 
+00001e90: 7265 706f 7369 746f 7279 3a0d 0a60 6060  repository:..```
+00001ea0: 6261 7368 0d0a 6769 7420 636c 6f6e 6520  bash..git clone 
+00001eb0: 6874 7470 733a 2f2f 7777 772e 6769 7468  https://www.gith
+00001ec0: 7562 2e63 6f6d 2f6a 6772 6176 696e 672f  ub.com/jgraving/
+00001ed0: 6465 6570 706f 7365 6b69 742d 6461 7461  deepposekit-data
+00001ee0: 0d0a 6060 600d 0a0d 0a23 2320 496e 7374  ..```....## Inst
+00001ef0: 616c 6c69 6e67 2077 6974 6820 416e 6163  alling with Anac
+00001f00: 6f6e 6461 206f 6e20 5769 6e64 6f77 730d  onda on Windows.
+00001f10: 0a0d 0a54 6f20 696e 7374 616c 6c20 4465  ...To install De
+00001f20: 6570 506f 7365 4b69 7420 6f6e 2057 696e  epPoseKit on Win
+00001f30: 646f 7773 2c20 796f 7520 6d75 7374 2066  dows, you must f
+00001f40: 6972 7374 206d 616e 7561 6c6c 7920 696e  irst manually in
+00001f50: 7374 616c 6c20 6053 6861 7065 6c79 602c  stall `Shapely`,
+00001f60: 206f 6e65 206f 6620 7468 6520 6465 7065   one of the depe
+00001f70: 6e64 656e 6369 6573 2066 6f72 2074 6865  ndencies for the
+00001f80: 205b 696d 6761 7567 2070 6163 6b61 6765   [imgaug package
+00001f90: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001fa0: 2e63 6f6d 2f61 6c65 6a75 2f69 6d67 6175  .com/aleju/imgau
+00001fb0: 6729 3a0d 0a60 6060 6261 7368 0d0a 636f  g):..```bash..co
+00001fc0: 6e64 6120 696e 7374 616c 6c20 2d63 2063  nda install -c c
+00001fd0: 6f6e 6461 2d66 6f72 6765 2073 6861 7065  onda-forge shape
+00001fe0: 6c79 0d0a 6060 600d 0a57 6520 616c 736f  ly..```..We also
+00001ff0: 2072 6563 6f6d 6d65 6e64 2069 6e73 7461   recommend insta
+00002000: 6c6c 696e 6720 4465 6570 506f 7365 4b69  lling DeepPoseKi
+00002010: 7420 6672 6f6d 2077 6974 6869 6e20 5079  t from within Py
+00002020: 7468 6f6e 2072 6174 6865 7220 7468 616e  thon rather than
+00002030: 2075 7369 6e67 2074 6865 2063 6f6d 6d61   using the comma
+00002040: 6e64 206c 696e 652c 2065 6974 6865 7220  nd line, either 
+00002050: 6672 6f6d 2077 6974 6869 6e20 4a75 7079  from within Jupy
+00002060: 7465 7220 6f72 2061 6e6f 7468 6572 2049  ter or another I
+00002070: 4445 2c20 746f 2065 6e73 7572 6520 6974  DE, to ensure it
+00002080: 2069 7320 696e 7374 616c 6c65 6420 696e   is installed in
+00002090: 2074 6865 2063 6f72 7265 6374 2077 6f72   the correct wor
+000020a0: 6b69 6e67 2065 6e76 6972 6f6e 6d65 6e74  king environment
+000020b0: 3a0d 0a60 6060 7079 7468 6f6e 0d0a 696d  :..```python..im
+000020c0: 706f 7274 2073 7973 0d0a 217b 7379 732e  port sys..!{sys.
+000020d0: 6578 6563 7574 6162 6c65 7d20 2d6d 2070  executable} -m p
+000020e0: 6970 2069 6e73 7461 6c6c 202d 2d75 7064  ip install --upd
+000020f0: 6174 6520 6465 6570 706f 7365 6b69 740d  ate deepposekit.
+00002100: 0a60 6060 0d0a 2320 436f 6e74 7269 6275  .```..# Contribu
+00002110: 746f 7273 2061 6e64 2044 6576 656c 6f70  tors and Develop
+00002120: 6d65 6e74 2020 0d0a 2020 200d 0a44 6565  ment  ..   ..Dee
+00002130: 7050 6f73 654b 6974 2077 6173 2064 6576  pPoseKit was dev
+00002140: 656c 6f70 6564 2062 7920 5b4a 616b 6520  eloped by [Jake 
+00002150: 4772 6176 696e 675d 2868 7474 7073 3a2f  Graving](https:/
+00002160: 2f67 6974 6875 622e 636f 6d2f 6a67 7261  /github.com/jgra
+00002170: 7669 6e67 2920 616e 6420 5b44 616e 6965  ving) and [Danie
+00002180: 6c20 4368 6165 5d28 6874 7470 733a 2f2f  l Chae](https://
+00002190: 6769 7468 7562 2e63 6f6d 2f64 6368 6165  github.com/dchae
+000021a0: 6261 6529 2c20 616e 6420 6973 2073 7469  bae), and is sti
+000021b0: 6c6c 2062 6569 6e67 2061 6374 6976 656c  ll being activel
+000021c0: 7920 6465 7665 6c6f 7065 642e 202e 0d0a  y developed. ...
+000021d0: 0d0a 5765 2077 656c 636f 6d65 2063 6f6d  ..We welcome com
+000021e0: 6d75 6e69 7479 2069 6e76 6f6c 7665 6d65  munity involveme
+000021f0: 6e74 2061 6e64 2070 7562 6c69 6320 636f  nt and public co
+00002200: 6e74 7269 6275 7469 6f6e 7320 746f 2074  ntributions to t
+00002210: 6865 2074 6f6f 6c6b 6974 2e20 4966 2079  he toolkit. If y
+00002220: 6f75 2077 6973 6820 746f 2063 6f6e 7472  ou wish to contr
+00002230: 6962 7574 652c 2070 6c65 6173 6520 5b66  ibute, please [f
+00002240: 6f72 6b20 7468 6520 7265 706f 7369 746f  ork the reposito
+00002250: 7279 5d28 6874 7470 733a 2f2f 6865 6c70  ry](https://help
+00002260: 2e67 6974 6875 622e 636f 6d2f 656e 2f61  .github.com/en/a
+00002270: 7274 6963 6c65 732f 666f 726b 2d61 2d72  rticles/fork-a-r
+00002280: 6570 6f29 2074 6f20 6d61 6b65 2079 6f75  epo) to make you
+00002290: 7220 6d6f 6469 6669 6361 7469 6f6e 7320  r modifications 
+000022a0: 616e 6420 5b73 7562 6d69 7420 6120 7075  and [submit a pu
+000022b0: 6c6c 2072 6571 7565 7374 5d28 6874 7470  ll request](http
+000022c0: 733a 2f2f 6865 6c70 2e67 6974 6875 622e  s://help.github.
+000022d0: 636f 6d2f 656e 2f61 7274 6963 6c65 732f  com/en/articles/
+000022e0: 6372 6561 7469 6e67 2d61 2d70 756c 6c2d  creating-a-pull-
+000022f0: 7265 7175 6573 742d 6672 6f6d 2d61 2d66  request-from-a-f
+00002300: 6f72 6b29 2e0d 0a0d 0a49 6620 796f 7527  ork).....If you'
+00002310: 6420 6c69 6b65 2074 6f20 6765 7420 696e  d like to get in
+00002320: 766f 6c76 6564 2077 6974 6820 6465 7665  volved with deve
+00002330: 6c6f 7069 6e67 2044 6565 7050 6f73 654b  loping DeepPoseK
+00002340: 6974 2c20 6765 7420 696e 2074 6f75 6368  it, get in touch
+00002350: 2028 6a67 7261 7669 6e67 4067 6d61 696c   (jgraving@gmail
+00002360: 2e63 6f6d 2920 616e 6420 6368 6563 6b20  .com) and check 
+00002370: 6f75 7420 5b6f 7572 2064 6576 656c 6f70  out [our develop
+00002380: 6d65 6e74 2072 6f61 646d 6170 5d28 6874  ment roadmap](ht
+00002390: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000023a0: 2f6a 6772 6176 696e 672f 4465 6570 506f  /jgraving/DeepPo
+000023b0: 7365 4b69 742f 626c 6f62 2f6d 6173 7465  seKit/blob/maste
+000023c0: 722f 4445 5645 4c4f 504d 454e 542e 6d64  r/DEVELOPMENT.md
+000023d0: 2920 746f 2073 6565 2066 7574 7572 6520  ) to see future 
+000023e0: 706c 616e 7320 666f 7220 7468 6520 7061  plans for the pa
+000023f0: 636b 6167 652e 2020 0d0a 0d0a 2320 4973  ckage.  ....# Is
+00002400: 7375 6573 2020 0d0a 200d 0a50 6c65 6173  sues  .. ..Pleas
+00002410: 6520 7375 626d 6974 2062 7567 7320 6f72  e submit bugs or
+00002420: 2066 6561 7475 7265 2072 6571 7565 7374   feature request
+00002430: 7320 746f 2074 6865 205b 4769 7448 7562  s to the [GitHub
+00002440: 2069 7373 7565 2074 7261 636b 6572 5d28   issue tracker](
+00002450: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002460: 6f6d 2f6a 6772 6176 696e 672f 6465 6570  om/jgraving/deep
+00002470: 706f 7365 6b69 742f 6973 7375 6573 2f6e  posekit/issues/n
+00002480: 6577 292e 2050 6c65 6173 6520 6c69 6d69  ew). Please limi
+00002490: 7420 7265 706f 7274 6564 2069 7373 7565  t reported issue
+000024a0: 7320 746f 2074 6865 2044 6565 7050 6f73  s to the DeepPos
+000024b0: 654b 6974 2063 6f64 6562 6173 6520 616e  eKit codebase an
+000024c0: 6420 7072 6f76 6964 6520 6173 206d 7563  d provide as muc
+000024d0: 6820 6465 7461 696c 2061 7320 796f 7520  h detail as you 
+000024e0: 6361 6e20 7769 7468 2061 206d 696e 696d  can with a minim
+000024f0: 616c 2077 6f72 6b69 6e67 2065 7861 6d70  al working examp
+00002500: 6c65 2069 6620 706f 7373 6962 6c65 2e0d  le if possible..
+00002510: 0a0d 0a49 6620 796f 7520 6578 7065 7269  ...If you experi
+00002520: 656e 6365 2070 726f 626c 656d 7320 7769  ence problems wi
+00002530: 7468 205b 5465 6e73 6f72 666c 6f77 5d28  th [Tensorflow](
+00002540: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002550: 6f6d 2f74 656e 736f 7266 6c6f 772f 7465  om/tensorflow/te
+00002560: 6e73 6f72 666c 6f77 292c 2073 7563 6820  nsorflow), such 
+00002570: 6173 2069 6e73 7461 6c6c 696e 6720 4355  as installing CU
+00002580: 4441 206f 7220 6375 444e 4e20 6465 7065  DA or cuDNN depe
+00002590: 6e64 656e 6369 6573 2c20 7468 656e 2070  ndencies, then p
+000025a0: 6c65 6173 6520 6469 7265 6374 2069 7373  lease direct iss
+000025b0: 7565 7320 746f 2074 686f 7365 2064 6576  ues to those dev
+000025c0: 656c 6f70 6d65 6e74 2074 6561 6d73 2e0d  elopment teams..
+000025d0: 0a0d 0a23 204c 6963 656e 7365 0d0a 0d0a  ...# License....
+000025e0: 5265 6c65 6173 6564 2075 6e64 6572 2061  Released under a
+000025f0: 2041 7061 6368 6520 322e 3020 4c69 6365   Apache 2.0 Lice
+00002600: 6e73 652e 2053 6565 205b 4c49 4345 4e53  nse. See [LICENS
+00002610: 455d 2868 7474 7073 3a2f 2f67 6974 6875  E](https://githu
+00002620: 622e 636f 6d2f 6a67 7261 7669 6e67 2f64  b.com/jgraving/d
+00002630: 6565 7070 6f73 656b 6974 2f62 6c6f 622f  eepposekit/blob/
+00002640: 6d61 7374 6572 2f4c 4943 454e 5345 2920  master/LICENSE) 
+00002650: 666f 7220 6465 7461 696c 732e 0d0a 0d0a  for details.....
+00002660: 2320 5265 6665 7265 6e63 6573 0d0a 0d0a  # References....
+00002670: 4966 2079 6f75 2075 7365 2044 6565 7050  If you use DeepP
+00002680: 6f73 654b 6974 2066 6f72 2079 6f75 7220  oseKit for your 
+00002690: 7265 7365 6172 6368 2070 6c65 6173 6520  research please 
+000026a0: 6369 7465 205b 6f75 7220 6f70 656e 2d61  cite [our open-a
+000026b0: 6363 6573 7320 7061 7065 725d 2868 7474  ccess paper](htt
+000026c0: 703a 2f2f 7061 7065 722e 6465 6570 706f  p://paper.deeppo
+000026d0: 7365 6b69 742e 6f72 6729 3a0d 0a0d 0a20  sekit.org):.... 
+000026e0: 2020 2040 6172 7469 636c 657b 6772 6176     @article{grav
+000026f0: 696e 6732 3031 3964 6565 7070 6f73 656b  ing2019deepposek
+00002700: 6974 2c0d 0a20 2020 2020 2020 2020 2020  it,..           
+00002710: 2020 7469 746c 653d 7b44 6565 7050 6f73    title={DeepPos
+00002720: 654b 6974 2c20 6120 736f 6674 7761 7265  eKit, a software
+00002730: 2074 6f6f 6c6b 6974 2066 6f72 2066 6173   toolkit for fas
+00002740: 7420 616e 6420 726f 6275 7374 2061 6e69  t and robust ani
+00002750: 6d61 6c20 706f 7365 2065 7374 696d 6174  mal pose estimat
+00002760: 696f 6e20 7573 696e 6720 6465 6570 206c  ion using deep l
+00002770: 6561 726e 696e 677d 2c0d 0a20 2020 2020  earning},..     
+00002780: 2020 2020 2020 2020 6175 7468 6f72 3d7b          author={
+00002790: 4772 6176 696e 672c 204a 6163 6f62 204d  Graving, Jacob M
+000027a0: 2061 6e64 2043 6861 652c 2044 616e 6965   and Chae, Danie
+000027b0: 6c20 616e 6420 4e61 696b 2c20 4865 6d61  l and Naik, Hema
+000027c0: 6c20 616e 6420 4c69 2c20 4c69 616e 6720  l and Li, Liang 
+000027d0: 616e 6420 4b6f 6765 722c 2042 656e 6a61  and Koger, Benja
+000027e0: 6d69 6e20 616e 6420 436f 7374 656c 6c6f  min and Costello
+000027f0: 652c 2042 6c61 6972 2052 2061 6e64 2043  e, Blair R and C
+00002800: 6f75 7a69 6e2c 2049 6169 6e20 447d 2c0d  ouzin, Iain D},.
+00002810: 0a20 2020 2020 2020 2020 2020 2020 6a6f  .             jo
+00002820: 7572 6e61 6c3d 7b65 4c69 6665 7d2c 0d0a  urnal={eLife},..
+00002830: 2020 2020 2020 2020 2020 2020 2076 6f6c               vol
+00002840: 756d 653d 7b38 7d2c 0d0a 2020 2020 2020  ume={8},..      
+00002850: 2020 2020 2020 2070 6167 6573 3d7b 6534         pages={e4
+00002860: 3739 3934 7d2c 0d0a 2020 2020 2020 2020  7994},..        
+00002870: 2020 2020 2079 6561 723d 7b32 3031 397d       year={2019}
+00002880: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002890: 7075 626c 6973 6865 723d 7b65 4c69 6665  publisher={eLife
+000028a0: 2053 6369 656e 6365 7320 5075 626c 6963   Sciences Public
+000028b0: 6174 696f 6e73 204c 696d 6974 6564 7d0d  ations Limited}.
+000028c0: 0a20 2020 2020 2020 2020 2020 2020 7572  .             ur
+000028d0: 6c3d 7b68 7474 7073 3a2f 2f64 6f69 2e6f  l={https://doi.o
+000028e0: 7267 2f31 302e 3735 3534 2f65 4c69 6665  rg/10.7554/eLife
+000028f0: 2e34 3739 3934 7d2c 0d0a 2020 2020 2020  .47994},..      
+00002900: 2020 2020 2020 207d 0d0a 0d0a 596f 7520         }....You 
+00002910: 6361 6e20 616c 736f 2072 6561 6420 5b6f  can also read [o
+00002920: 7572 206f 7065 6e2d 6163 6365 7373 2070  ur open-access p
+00002930: 7265 7072 696e 745d 2868 7474 703a 2f2f  reprint](http://
+00002940: 7072 6570 7269 6e74 2e64 6565 7070 6f73  preprint.deeppos
+00002950: 656b 6974 2e6f 7267 292e 0d0a 0d0a 4966  ekit.org).....If
+00002960: 2079 6f75 2075 7365 2074 6865 205b 696d   you use the [im
+00002970: 6761 7567 2070 6163 6b61 6765 5d28 6874  gaug package](ht
+00002980: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002990: 2f61 6c65 6a75 2f69 6d67 6175 6729 2066  /aleju/imgaug) f
+000029a0: 6f72 2064 6174 6120 6175 676d 656e 7461  or data augmenta
+000029b0: 7469 6f6e 2c20 706c 6561 7365 2061 6c73  tion, please als
+000029c0: 6f20 636f 6e73 6964 6572 205b 6369 7469  o consider [citi
+000029d0: 6e67 2069 745d 2868 7474 7073 3a2f 2f67  ng it](https://g
+000029e0: 6974 6875 622e 636f 6d2f 616c 656a 752f  ithub.com/aleju/
+000029f0: 696d 6761 7567 2f62 6c6f 622f 6d61 7374  imgaug/blob/mast
+00002a00: 6572 2f52 4541 444d 452e 6d64 2363 6974  er/README.md#cit
+00002a10: 6174 696f 6e29 2e0d 0a0d 0a49 6620 796f  ation).....If yo
+00002a20: 7520 5b75 7365 2064 6174 615d 2868 7474  u [use data](htt
+00002a30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002a40: 6a67 7261 7669 6e67 2f44 6565 7050 6f73  jgraving/DeepPos
+00002a50: 654b 6974 2369 2d61 6c72 6561 6479 2d68  eKit#i-already-h
+00002a60: 6176 652d 616e 6e6f 7461 7465 642d 6461  ave-annotated-da
+00002a70: 7461 2920 7468 6174 2077 6173 2061 6e6e  ta) that was ann
+00002a80: 6f74 6174 6564 2077 6974 6820 7468 6520  otated with the 
+00002a90: 4465 6570 4c61 6243 7574 2070 6163 6b61  DeepLabCut packa
+00002aa0: 6765 2028 6874 7470 3a2f 2f64 6565 706c  ge (http://deepl
+00002ab0: 6162 6375 742e 6f72 6729 2066 6f72 2079  abcut.org) for y
+00002ac0: 6f75 7220 7265 7365 6172 6368 2c20 6265  our research, be
+00002ad0: 2073 7572 6520 746f 205b 6369 7465 2069   sure to [cite i
+00002ae0: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00002af0: 622e 636f 6d2f 416c 6578 454d 472f 4465  b.com/AlexEMG/De
+00002b00: 6570 4c61 6243 7574 2f62 6c6f 622f 6d61  epLabCut/blob/ma
+00002b10: 7374 6572 2f52 4541 444d 452e 6d64 2372  ster/README.md#r
+00002b20: 6566 6572 656e 6365 7329 2e0d 0a0d 0a50  eferences).....P
+00002b30: 6c65 6173 6520 616c 736f 2063 6f6e 7369  lease also consi
+00002b40: 6465 7220 6369 7469 6e67 2074 6865 2072  der citing the r
+00002b50: 656c 6576 616e 7420 7265 6665 7265 6e63  elevant referenc
+00002b60: 6573 2066 6f72 2074 6865 2070 6f73 6520  es for the pose 
+00002b70: 6573 7469 6d61 7469 6f6e 206d 6f64 656c  estimation model
+00002b80: 2873 2920 7573 6564 2069 6e20 796f 7572  (s) used in your
+00002b90: 2072 6573 6561 7263 682c 2077 6869 6368   research, which
+00002ba0: 2063 616e 2062 6520 666f 756e 6420 696e   can be found in
+00002bb0: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
+00002bc0: 6f6e 2028 692e 652e 2c20 5b60 5374 6163  on (i.e., [`Stac
+00002bd0: 6b65 6444 656e 7365 4e65 7460 5d28 6874  kedDenseNet`](ht
+00002be0: 7470 3a2f 2f6a 616b 6567 7261 7669 6e67  tp://jakegraving
+00002bf0: 2e63 6f6d 2f44 6565 7050 6f73 654b 6974  .com/DeepPoseKit
+00002c00: 2f68 746d 6c2f 6465 6570 706f 7365 6b69  /html/deepposeki
+00002c10: 742f 6d6f 6465 6c73 2f53 7461 636b 6564  t/models/Stacked
+00002c20: 4465 6e73 654e 6574 2e68 746d 6c23 7265  DenseNet.html#re
+00002c30: 6665 7265 6e63 6573 292c 205b 6053 7461  ferences), [`Sta
+00002c40: 636b 6564 486f 7572 676c 6173 7360 5d28  ckedHourglass`](
+00002c50: 6874 7470 3a2f 2f6a 616b 6567 7261 7669  http://jakegravi
+00002c60: 6e67 2e63 6f6d 2f44 6565 7050 6f73 654b  ng.com/DeepPoseK
+00002c70: 6974 2f68 746d 6c2f 6465 6570 706f 7365  it/html/deeppose
+00002c80: 6b69 742f 6d6f 6465 6c73 2f53 7461 636b  kit/models/Stack
+00002c90: 6564 486f 7572 676c 6173 732e 6874 6d6c  edHourglass.html
+00002ca0: 2372 6566 6572 656e 6365 7329 2c20 5b60  #references), [`
+00002cb0: 4465 6570 4c61 6243 7574 605d 2868 7474  DeepLabCut`](htt
+00002cc0: 703a 2f2f 6a61 6b65 6772 6176 696e 672e  p://jakegraving.
+00002cd0: 636f 6d2f 4465 6570 506f 7365 4b69 742f  com/DeepPoseKit/
+00002ce0: 6874 6d6c 2f64 6565 7070 6f73 656b 6974  html/deepposekit
+00002cf0: 2f6d 6f64 656c 732f 4465 6570 4c61 6243  /models/DeepLabC
+00002d00: 7574 2e68 746d 6c23 7265 6665 7265 6e63  ut.html#referenc
+00002d10: 6573 292c 205b 604c 4541 5060 5d28 6874  es), [`LEAP`](ht
+00002d20: 7470 3a2f 2f6a 616b 6567 7261 7669 6e67  tp://jakegraving
+00002d30: 2e63 6f6d 2f44 6565 7050 6f73 654b 6974  .com/DeepPoseKit
+00002d40: 2f68 746d 6c2f 6465 6570 706f 7365 6b69  /html/deepposeki
+00002d50: 742f 6d6f 6465 6c73 2f4c 4541 502e 6874  t/models/LEAP.ht
+00002d60: 6d6c 2372 6566 6572 656e 6365 7329 292e  ml#references)).
+00002d70: 0d0a 0d0a 2320 4e65 7773 0d0a 2d20 2a2a  ....# News..- **
+00002d80: 4f63 746f 6265 7220 3230 3139 3a2a 2a20  October 2019:** 
+00002d90: 4f75 7220 7061 7065 7220 6465 7363 7269  Our paper descri
+00002da0: 6269 6e67 2044 6565 7050 6f73 654b 6974  bing DeepPoseKit
+00002db0: 2069 7320 7075 626c 6973 6865 6420 6174   is published at
+00002dc0: 2065 4c69 6665 2120 2868 7474 703a 2f2f   eLife! (http://
+00002dd0: 7061 7065 722e 6465 6570 706f 7365 6b69  paper.deepposeki
+00002de0: 742e 6f72 6729 0d0a 2d20 2a2a 5365 7074  t.org)..- **Sept
+00002df0: 656d 6265 7220 3230 3139 2a2a 3a20 0d0a  ember 2019**: ..
+00002e00: 2020 2020 2d20 4e61 7475 7265 204e 6577      - Nature New
+00002e10: 7320 636f 7665 7273 2044 6565 7050 6f73  s covers DeepPos
+00002e20: 654b 6974 3a20 5b44 6565 7020 6c65 6172  eKit: [Deep lear
+00002e30: 6e69 6e67 2070 6f77 6572 7320 6120 6d6f  ning powers a mo
+00002e40: 7469 6f6e 2d74 7261 636b 696e 6720 7265  tion-tracking re
+00002e50: 766f 6c75 7469 6f6e 5d28 6874 7470 3a2f  volution](http:/
+00002e60: 2f64 6f69 2e6f 7267 2f31 302e 3130 3338  /doi.org/10.1038
+00002e70: 2f64 3431 3538 362d 3031 392d 3032 3934  /d41586-019-0294
+00002e80: 322d 3529 0d0a 2020 2020 2d20 7630 2e33  2-5)..    - v0.3
+00002e90: 2e30 2069 7320 7265 6c65 6173 6564 2e20  .0 is released. 
+00002ea0: 5365 6520 5b74 6865 2072 656c 6561 7365  See [the release
+00002eb0: 206e 6f74 6573 5d28 6874 7470 733a 2f2f   notes](https://
+00002ec0: 6769 7468 7562 2e63 6f6d 2f6a 6772 6176  github.com/jgrav
+00002ed0: 696e 672f 4465 6570 506f 7365 4b69 742f  ing/DeepPoseKit/
+00002ee0: 7265 6c65 6173 6573 2f74 6167 2f76 302e  releases/tag/v0.
+00002ef0: 332e 3029 2e0d 0a2d 202a 2a41 7072 696c  3.0)...- **April
+00002f00: 2032 3031 393a 2a2a 2054 6865 2044 6565   2019:** The Dee
+00002f10: 7050 6f73 654b 6974 2070 7265 7072 696e  pPoseKit preprin
+00002f20: 7420 6973 206f 6e20 6269 6f72 7869 7620  t is on biorxiv 
+00002f30: 2868 7474 703a 2f2f 7072 6570 7269 6e74  (http://preprint
+00002f40: 2e64 6565 7070 6f73 656b 6974 2e6f 7267  .deepposekit.org
+00002f50: 290d 0a                                  )..
```

### Comparing `us2deepposekit-0.3.9/README.md` & `us2deepposekit-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,758 +1,798 @@
-00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000010: 223e 0d0a 3c69 6d67 2073 7263 3d22 6874  ">..<img src="ht
-00000020: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000030: 2f6a 6772 6176 696e 672f 4465 6570 506f  /jgraving/DeepPo
-00000040: 7365 4b69 742f 626c 6f62 2f6d 6173 7465  seKit/blob/maste
-00000050: 722f 6173 7365 7473 2f64 6565 7070 6f73  r/assets/deeppos
-00000060: 656b 6974 5f6c 6f67 6f2e 706e 6722 2068  ekit_logo.png" h
-00000070: 6569 6768 743d 2233 3230 7078 223e 0d0a  eight="320px">..
-00000080: 3c2f 703e 0d0a 0d0a 2320 596f 7520 6861  </p>....# You ha
-00000090: 7665 206a 7573 7420 666f 756e 6420 4465  ve just found De
-000000a0: 6570 506f 7365 4b69 742e 0d0a 3c70 2061  epPoseKit...<p a
-000000b0: 6c69 676e 3d22 6365 6e74 6572 223e 0d0a  lign="center">..
-000000c0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000000d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6772  //github.com/jgr
-000000e0: 6176 696e 672f 6a67 7261 7669 6e67 2e67  aving/jgraving.g
-000000f0: 6974 6875 622e 696f 2f62 6c6f 622f 6d61  ithub.io/blob/ma
-00000100: 7374 6572 2f66 696c 6573 2f69 6d61 6765  ster/files/image
-00000110: 732f 4669 6775 7265 3176 6964 656f 312e  s/Figure1video1.
-00000120: 6769 6622 2068 6569 6768 743d 2231 3238  gif" height="128
-00000130: 7078 223e 0d0a 3c2f 703e 0d0a 0d0a 4465  px">..</p>....De
-00000140: 6570 506f 7365 4b69 7420 6973 2061 2073  epPoseKit is a s
-00000150: 6f66 7477 6172 6520 746f 6f6c 6b69 7420  oftware toolkit 
-00000160: 7769 7468 2061 2068 6967 682d 6c65 7665  with a high-leve
-00000170: 6c20 4150 4920 666f 7220 3244 2070 6f73  l API for 2D pos
-00000180: 6520 6573 7469 6d61 7469 6f6e 206f 6620  e estimation of 
-00000190: 7573 6572 2d64 6566 696e 6564 206b 6579  user-defined key
-000001a0: 706f 696e 7473 2075 7369 6e67 2064 6565  points using dee
-000001b0: 7020 6c65 6172 6e69 6e67 e280 9477 7269  p learning...wri
-000001c0: 7474 656e 2069 6e20 5079 7468 6f6e 2061  tten in Python a
-000001d0: 6e64 2062 7569 6c74 2075 7369 6e67 205b  nd built using [
-000001e0: 5465 6e73 6f72 666c 6f77 5d28 6874 7470  Tensorflow](http
-000001f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00000200: 656e 736f 7266 6c6f 772f 7465 6e73 6f72  ensorflow/tensor
-00000210: 666c 6f77 2920 616e 6420 5b4b 6572 6173  flow) and [Keras
-00000220: 5d28 6874 7470 733a 2f2f 7777 772e 7465  ](https://www.te
-00000230: 6e73 6f72 666c 6f77 2e6f 7267 2f67 7569  nsorflow.org/gui
-00000240: 6465 2f6b 6572 6173 292e 2055 7365 2044  de/keras). Use D
-00000250: 6565 7050 6f73 654b 6974 2069 6620 796f  eepPoseKit if yo
-00000260: 7520 6e65 6564 3a0d 0a0d 0a2d 2074 6f6f  u need:....- too
-00000270: 6c73 2066 6f72 2061 6e6e 6f74 6174 696e  ls for annotatin
-00000280: 6720 696d 6167 6573 206f 7220 7669 6465  g images or vide
-00000290: 6f20 6672 616d 6573 2077 6974 6820 7573  o frames with us
-000002a0: 6572 2d64 6566 696e 6564 206b 6579 706f  er-defined keypo
-000002b0: 696e 7473 0d0a 2d20 6120 7374 7261 6967  ints..- a straig
-000002c0: 6874 666f 7277 6172 6420 6275 7420 666c  htforward but fl
-000002d0: 6578 6962 6c65 2064 6174 6120 6175 676d  exible data augm
-000002e0: 656e 7461 7469 6f6e 2070 6970 656c 696e  entation pipelin
-000002f0: 6520 7573 696e 6720 7468 6520 5b69 6d67  e using the [img
-00000300: 6175 6720 7061 636b 6167 655d 2868 7474  aug package](htt
-00000310: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000320: 616c 656a 752f 696d 6761 7567 290d 0a2d  aleju/imgaug)..-
-00000330: 2061 204b 6572 6173 2d62 6173 6564 2069   a Keras-based i
-00000340: 6e74 6572 6661 6365 2066 6f72 2069 6e69  nterface for ini
-00000350: 7469 616c 697a 696e 672c 2074 7261 696e  tializing, train
-00000360: 696e 672c 2061 6e64 2065 7661 6c75 6174  ing, and evaluat
-00000370: 696e 6720 706f 7365 2065 7374 696d 6174  ing pose estimat
-00000380: 696f 6e20 6d6f 6465 6c73 0d0a 2d20 6561  ion models..- ea
-00000390: 7379 2d74 6f2d 7573 6520 6d65 7468 6f64  sy-to-use method
-000003a0: 7320 666f 7220 7361 7669 6e67 2061 6e64  s for saving and
-000003b0: 206c 6f61 6469 6e67 206d 6f64 656c 7320   loading models 
-000003c0: 616e 6420 6d61 6b69 6e67 2070 7265 6469  and making predi
-000003d0: 6374 696f 6e73 206f 6e20 6e65 7720 6461  ctions on new da
-000003e0: 7461 0d0a 0d0a 4465 6570 506f 7365 4b69  ta....DeepPoseKi
-000003f0: 7420 6973 2064 6573 6967 6e65 6420 7769  t is designed wi
-00000400: 7468 2061 2066 6f63 7573 206f 6e20 2a75  th a focus on *u
-00000410: 7361 6269 6c69 7479 2a20 616e 6420 2a65  sability* and *e
-00000420: 7874 656e 7369 6269 6c69 7479 2a2c 2061  xtensibility*, a
-00000430: 7320 6265 696e 6720 6162 6c65 2074 6f20  s being able to 
-00000440: 676f 2066 726f 6d20 6964 6561 2074 6f20  go from idea to 
-00000450: 7265 7375 6c74 2077 6974 6820 7468 6520  result with the 
-00000460: 6c65 6173 7420 706f 7373 6962 6c65 2064  least possible d
-00000470: 656c 6179 2069 7320 6b65 7920 746f 2064  elay is key to d
-00000480: 6f69 6e67 2067 6f6f 6420 7265 7365 6172  oing good resear
-00000490: 6368 2e0d 0a0d 0a44 6565 7050 6f73 654b  ch.....DeepPoseK
-000004a0: 6974 2069 7320 6375 7272 656e 746c 7920  it is currently 
-000004b0: 6c69 6d69 7465 6420 746f 202a 696e 6469  limited to *indi
-000004c0: 7669 6475 616c 2070 6f73 6520 6573 7469  vidual pose esti
-000004d0: 6d61 7469 6f6e 2a2e 2049 6620 696e 6469  mation*. If indi
-000004e0: 7669 6475 616c 7320 6361 6e20 6265 2065  viduals can be e
-000004f0: 6173 696c 7920 6469 7374 696e 6775 6973  asily distinguis
-00000500: 6865 6420 7669 7375 616c 6c79 2028 692e  hed visually (i.
-00000510: 652e 2c20 7468 6579 2068 6176 6520 6469  e., they have di
-00000520: 6666 6572 656e 746c 7920 636f 6c6f 7265  fferently colore
-00000530: 6420 626f 6469 6573 206f 7220 6172 6520  d bodies or are 
-00000540: 6d61 726b 6564 2069 6e20 736f 6d65 2077  marked in some w
-00000550: 6179 292c 2074 6865 6e20 6d75 6c74 6970  ay), then multip
-00000560: 6c65 2069 6e64 6976 6964 7561 6c73 2063  le individuals c
-00000570: 616e 2073 696d 706c 7920 6265 206c 6162  an simply be lab
-00000580: 656c 6564 2077 6974 6820 7365 7061 7261  eled with separa
-00000590: 7465 206b 6579 706f 696e 7473 2028 6865  te keypoints (he
-000005a0: 6164 312c 2074 6169 6c31 2c20 6865 6164  ad1, tail1, head
-000005b0: 322c 2074 6169 6c32 2c20 6574 632e 292e  2, tail2, etc.).
-000005c0: 204f 7468 6572 7769 7365 2044 6565 7050   Otherwise DeepP
-000005d0: 6f73 654b 6974 2063 616e 2062 6520 6578  oseKit can be ex
-000005e0: 7465 6e64 6564 2074 6f20 6d75 6c74 6970  tended to multip
-000005f0: 6c65 2069 6e64 6976 6964 7561 6c73 2062  le individuals b
-00000600: 7920 6669 7273 7420 6c6f 6361 6c69 7a69  y first localizi
-00000610: 6e67 2c20 7472 6163 6b69 6e67 2c20 616e  ng, tracking, an
-00000620: 6420 6372 6f70 7069 6e67 2069 6e64 6976  d cropping indiv
-00000630: 6964 7561 6c73 2077 6974 6820 6164 6469  iduals with addi
-00000640: 7469 6f6e 616c 2073 6f66 7477 6172 6520  tional software 
-00000650: 7375 6368 2061 7320 5b69 6474 7261 636b  such as [idtrack
-00000660: 6572 2e61 695d 2868 7474 7073 3a2f 2f69  er.ai](https://i
-00000670: 6474 7261 636b 6572 2e61 692f 292c 205b  dtracker.ai/), [
-00000680: 7069 6e70 6f69 6e74 5d28 6874 7470 733a  pinpoint](https:
-00000690: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6772  //github.com/jgr
-000006a0: 6176 696e 672f 7069 6e70 6f69 6e74 292c  aving/pinpoint),
-000006b0: 206f 7220 5b54 7261 636b 746f 725d 2868   or [Tracktor](h
-000006c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000006d0: 6d2f 7669 7665 6b68 7372 6964 6861 722f  m/vivekhsridhar/
-000006e0: 7472 6163 6b74 6f72 292e 0d0a 0d0a 4c6f  tracktor).....Lo
-000006f0: 6361 6c69 7a61 7469 6f6e 2028 7769 7468  calization (with
-00000700: 6f75 7420 7472 6163 6b69 6e67 2920 6361  out tracking) ca
-00000710: 6e20 616c 736f 2062 6520 6163 6869 6576  n also be achiev
-00000720: 6564 2077 6974 6820 6465 6570 206c 6561  ed with deep lea
-00000730: 726e 696e 6720 736f 6674 7761 7265 206c  rning software l
-00000740: 696b 6520 5b6b 6572 6173 2d72 6574 696e  ike [keras-retin
-00000750: 616e 6574 5d28 6874 7470 733a 2f2f 6769  anet](https://gi
-00000760: 7468 7562 2e63 6f6d 2f66 697a 7972 2f6b  thub.com/fizyr/k
-00000770: 6572 6173 2d72 6574 696e 616e 6574 292c  eras-retinanet),
-00000780: 2074 6865 205b 5465 6e73 6f72 666c 6f77   the [Tensorflow
-00000790: 204f 626a 6563 7420 4465 7465 6374 696f   Object Detectio
-000007a0: 6e20 4150 495d 2868 7474 7073 3a2f 2f67  n API](https://g
-000007b0: 6974 6875 622e 636f 6d2f 7465 6e73 6f72  ithub.com/tensor
-000007c0: 666c 6f77 2f6d 6f64 656c 732f 7472 6565  flow/models/tree
-000007d0: 2f6d 6173 7465 722f 7265 7365 6172 6368  /master/research
-000007e0: 2f6f 626a 6563 745f 6465 7465 6374 696f  /object_detectio
-000007f0: 6e29 2c20 6f72 205b 4d61 7474 6572 506f  n), or [MatterPo
-00000800: 7274 2773 204d 6173 6b20 522d 434e 4e5d  rt's Mask R-CNN]
-00000810: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000820: 636f 6d2f 6d61 7474 6572 706f 7274 2f4d  com/matterport/M
-00000830: 6173 6b5f 5243 4e4e 292e 0d0a 0d0a 5b43  ask_RCNN).....[C
-00000840: 6865 636b 206f 7574 206f 7572 2070 6170  heck out our pap
-00000850: 6572 5d28 6874 7470 733a 2f2f 646f 692e  er](https://doi.
-00000860: 6f72 672f 3130 2e37 3535 342f 654c 6966  org/10.7554/eLif
-00000870: 652e 3437 3939 3429 2074 6f20 6669 6e64  e.47994) to find
-00000880: 206f 7574 206d 6f72 652e 0d0a 0d0a 3c70   out more.....<p
-00000890: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-000008a0: 0d0a 3c69 6d67 2073 7263 3d22 6874 7470  ..<img src="http
-000008b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000008c0: 6772 6176 696e 672f 6a67 7261 7669 6e67  graving/jgraving
-000008d0: 2e67 6974 6875 622e 696f 2f62 6c6f 622f  .github.io/blob/
-000008e0: 6d61 7374 6572 2f66 696c 6573 2f69 6d61  master/files/ima
-000008f0: 6765 732f 7a65 6272 612e 6769 6622 2068  ges/zebra.gif" h
-00000900: 6569 6768 743d 2232 3536 7078 223e 0d0a  eight="256px">..
-00000910: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000920: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6772  //github.com/jgr
-00000930: 6176 696e 672f 6a67 7261 7669 6e67 2e67  aving/jgraving.g
-00000940: 6974 6875 622e 696f 2f62 6c6f 622f 6d61  ithub.io/blob/ma
-00000950: 7374 6572 2f66 696c 6573 2f69 6d61 6765  ster/files/image
-00000960: 732f 6c6f 6375 7374 2e67 6966 2220 6865  s/locust.gif" he
-00000970: 6967 6874 3d22 3235 3670 7822 3e0d 0a3c  ight="256px">..<
-00000980: 2f70 3e0d 0a0d 0a23 2048 6f77 2074 6f20  /p>....# How to 
-00000990: 7573 6520 4465 6570 506f 7365 4b69 740d  use DeepPoseKit.
-000009a0: 0a0d 0a44 6565 7050 6f73 654b 6974 2069  ...DeepPoseKit i
-000009b0: 7320 6465 7369 676e 6564 2066 6f72 2065  s designed for e
-000009c0: 6173 7920 7573 652e 2046 6f72 2065 7861  asy use. For exa
-000009d0: 6d70 6c65 2c20 7472 6169 6e69 6e67 2061  mple, training a
-000009e0: 6e64 2073 6176 696e 6720 6120 6d6f 6465  nd saving a mode
-000009f0: 6c20 7265 7175 6972 6573 206f 6e6c 7920  l requires only 
-00000a00: 6120 6665 7720 6c69 6e65 7320 6f66 2063  a few lines of c
-00000a10: 6f64 653a 0d0a 6060 6070 7974 686f 6e0d  ode:..```python.
-00000a20: 0a66 726f 6d20 6465 6570 706f 7365 6b69  .from deepposeki
-00000a30: 742e 696f 2069 6d70 6f72 7420 4461 7461  t.io import Data
-00000a40: 4765 6e65 7261 746f 722c 2054 7261 696e  Generator, Train
-00000a50: 696e 6747 656e 6572 6174 6f72 0d0a 6672  ingGenerator..fr
-00000a60: 6f6d 2064 6565 7070 6f73 656b 6974 2e6d  om deepposekit.m
-00000a70: 6f64 656c 7320 696d 706f 7274 2053 7461  odels import Sta
-00000a80: 636b 6564 4465 6e73 654e 6574 0d0a 0d0a  ckedDenseNet....
-00000a90: 6461 7461 5f67 656e 6572 6174 6f72 203d  data_generator =
-00000aa0: 2044 6174 6147 656e 6572 6174 6f72 2827   DataGenerator('
-00000ab0: 2f70 6174 682f 746f 2f61 6e6e 6f74 6174  /path/to/annotat
-00000ac0: 696f 6e5f 6461 7461 2e68 3527 290d 0a74  ion_data.h5')..t
-00000ad0: 7261 696e 5f67 656e 6572 6174 6f72 203d  rain_generator =
-00000ae0: 2054 7261 696e 696e 6747 656e 6572 6174   TrainingGenerat
-00000af0: 6f72 2864 6174 615f 6765 6e65 7261 746f  or(data_generato
-00000b00: 7229 0d0a 6d6f 6465 6c20 3d20 5374 6163  r)..model = Stac
-00000b10: 6b65 6444 656e 7365 4e65 7428 7472 6169  kedDenseNet(trai
-00000b20: 6e5f 6765 6e65 7261 746f 7229 0d0a 6d6f  n_generator)..mo
-00000b30: 6465 6c2e 6669 7428 6261 7463 685f 7369  del.fit(batch_si
-00000b40: 7a65 3d31 362c 206e 5f77 6f72 6b65 7273  ze=16, n_workers
-00000b50: 3d38 290d 0a6d 6f64 656c 2e73 6176 6528  =8)..model.save(
-00000b60: 272f 7061 7468 2f74 6f2f 7361 7665 645f  '/path/to/saved_
-00000b70: 6d6f 6465 6c2e 6835 2729 0d0a 6060 600d  model.h5')..```.
-00000b80: 0a4c 6f61 6469 6e67 2061 2074 7261 696e  .Loading a train
-00000b90: 6564 206d 6f64 656c 2061 6e64 2072 756e  ed model and run
-00000ba0: 6e69 6e67 2070 7265 6469 6374 696f 6e73  ning predictions
-00000bb0: 206f 6e20 6e65 7720 6461 7461 2069 7320   on new data is 
-00000bc0: 616c 736f 2073 7472 6169 6768 7466 6f72  also straightfor
-00000bd0: 7761 7264 2e20 466f 7220 6578 616d 706c  ward. For exampl
-00000be0: 652c 2072 756e 6e69 6e67 2070 7265 6469  e, running predi
-00000bf0: 6374 696f 6e73 206f 6e20 6120 6e65 7720  ctions on a new 
-00000c00: 7669 6465 6f3a 0d0a 6060 6070 7974 686f  video:..```pytho
-00000c10: 6e0d 0a66 726f 6d20 6465 6570 706f 7365  n..from deeppose
-00000c20: 6b69 742e 6d6f 6465 6c73 2069 6d70 6f72  kit.models impor
-00000c30: 7420 6c6f 6164 5f6d 6f64 656c 0d0a 6672  t load_model..fr
-00000c40: 6f6d 2064 6565 7070 6f73 656b 6974 2e69  om deepposekit.i
-00000c50: 6f20 696d 706f 7274 2056 6964 656f 5265  o import VideoRe
-00000c60: 6164 6572 0d0a 0d0a 6d6f 6465 6c20 3d20  ader....model = 
-00000c70: 6c6f 6164 5f6d 6f64 656c 2827 2f70 6174  load_model('/pat
-00000c80: 682f 746f 2f73 6176 6564 5f6d 6f64 656c  h/to/saved_model
-00000c90: 2e68 3527 290d 0a72 6561 6465 7220 3d20  .h5')..reader = 
-00000ca0: 5669 6465 6f52 6561 6465 7228 272f 7061  VideoReader('/pa
-00000cb0: 7468 2f74 6f2f 7669 6465 6f2e 6d70 3427  th/to/video.mp4'
-00000cc0: 290d 0a70 7265 6469 6374 696f 6e73 203d  )..predictions =
-00000cd0: 206d 6f64 656c 2e70 7265 6469 6374 2872   model.predict(r
-00000ce0: 6561 6465 7229 0d0a 6060 600d 0a0d 0a23  eader)..```....#
-00000cf0: 2320 5573 696e 6720 4465 6570 506f 7365  # Using DeepPose
-00000d00: 4b69 7420 6973 2061 2034 2d73 7465 7020  Kit is a 4-step 
-00000d10: 7072 6f63 6573 733a 0d0a 0d0a 2d20 2a2a  process:....- **
-00000d20: 312e 2a2a 205b 4372 6561 7465 2061 6e20  1.** [Create an 
-00000d30: 616e 6e6f 7461 7469 6f6e 2073 6574 5d28  annotation set](
-00000d40: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000d50: 6f6d 2f6a 6772 6176 696e 672f 4465 6570  om/jgraving/Deep
-00000d60: 506f 7365 4b69 742f 626c 6f62 2f6d 6173  PoseKit/blob/mas
-00000d70: 7465 722f 6578 616d 706c 6573 2f73 7465  ter/examples/ste
-00000d80: 7031 5f63 7265 6174 655f 616e 6e6f 7461  p1_create_annota
-00000d90: 7469 6f6e 5f73 6574 2e69 7079 6e62 2920  tion_set.ipynb) 
-00000da0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000db0: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
-00000dc0: 676f 6f67 6c65 2e63 6f6d 2f67 6974 6875  google.com/githu
-00000dd0: 622f 6a67 7261 7669 6e67 2f64 6565 7070  b/jgraving/deepp
-00000de0: 6f73 656b 6974 2f62 6c6f 622f 6d61 7374  osekit/blob/mast
-00000df0: 6572 2f65 7861 6d70 6c65 732f 7374 6570  er/examples/step
-00000e00: 315f 6372 6561 7465 5f61 6e6e 6f74 6174  1_create_annotat
-00000e10: 696f 6e5f 7365 742e 6970 796e 6222 2074  ion_set.ipynb" t
-00000e20: 6172 6765 743d 225f 7061 7265 6e74 223e  arget="_parent">
-00000e30: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000e40: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-00000e50: 2e67 6f6f 676c 652e 636f 6d2f 6173 7365  .google.com/asse
-00000e60: 7473 2f63 6f6c 6162 2d62 6164 6765 2e73  ts/colab-badge.s
-00000e70: 7667 2220 616c 743d 224f 7065 6e20 496e  vg" alt="Open In
-00000e80: 2043 6f6c 6162 222f 3e3c 2f61 3e0d 0a2d   Colab"/></a>..-
-00000e90: 202a 2a32 2e2a 2a20 5b41 6e6e 6f74 6174   **2.** [Annotat
-00000ea0: 6520 796f 7572 2064 6174 615d 2868 7474  e your data](htt
-00000eb0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000ec0: 6a67 7261 7669 6e67 2f44 6565 7050 6f73  jgraving/DeepPos
-00000ed0: 654b 6974 2f62 6c6f 622f 6d61 7374 6572  eKit/blob/master
-00000ee0: 2f65 7861 6d70 6c65 732f 7374 6570 325f  /examples/step2_
-00000ef0: 616e 6e6f 7461 7465 5f64 6174 612e 6970  annotate_data.ip
-00000f00: 796e 6229 2077 6974 6820 6f75 7220 6275  ynb) with our bu
-00000f10: 696c 742d 696e 2047 5549 2028 6e6f 2043  ilt-in GUI (no C
-00000f20: 6f6c 6162 2073 7570 706f 7274 290d 0a2d  olab support)..-
-00000f30: 202a 2a33 2e2a 2a20 5b53 656c 6563 7420   **3.** [Select 
-00000f40: 616e 6420 7472 6169 6e5d 2868 7474 7073  and train](https
-00000f50: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a67  ://github.com/jg
-00000f60: 7261 7669 6e67 2f44 6565 7050 6f73 654b  raving/DeepPoseK
-00000f70: 6974 2f62 6c6f 622f 6d61 7374 6572 2f65  it/blob/master/e
-00000f80: 7861 6d70 6c65 732f 7374 6570 335f 7472  xamples/step3_tr
-00000f90: 6169 6e5f 6d6f 6465 6c2e 6970 796e 6229  ain_model.ipynb)
-00000fa0: 206f 6e65 206f 7572 205b 706f 7365 2065   one our [pose e
-00000fb0: 7374 696d 6174 696f 6e20 6d6f 6465 6c73  stimation models
-00000fc0: 5d28 6874 7470 3a2f 2f6a 616b 6567 7261  ](http://jakegra
-00000fd0: 7669 6e67 2e63 6f6d 2f44 6565 7050 6f73  ving.com/DeepPos
-00000fe0: 654b 6974 2f68 746d 6c2f 6465 6570 706f  eKit/html/deeppo
-00000ff0: 7365 6b69 742f 6d6f 6465 6c73 2f69 6e64  sekit/models/ind
-00001000: 6578 2e68 746d 6c29 2069 6e63 6c75 6469  ex.html) includi
-00001010: 6e67 205b 6053 7461 636b 6564 4465 6e73  ng [`StackedDens
-00001020: 654e 6574 605d 2868 7474 703a 2f2f 6a61  eNet`](http://ja
-00001030: 6b65 6772 6176 696e 672e 636f 6d2f 4465  kegraving.com/De
-00001040: 6570 506f 7365 4b69 742f 6874 6d6c 2f64  epPoseKit/html/d
-00001050: 6565 7070 6f73 656b 6974 2f6d 6f64 656c  eepposekit/model
-00001060: 732f 5374 6163 6b65 6444 656e 7365 4e65  s/StackedDenseNe
-00001070: 742e 6874 6d6c 292c 205b 6053 7461 636b  t.html), [`Stack
-00001080: 6564 486f 7572 676c 6173 7360 5d28 6874  edHourglass`](ht
-00001090: 7470 3a2f 2f6a 616b 6567 7261 7669 6e67  tp://jakegraving
-000010a0: 2e63 6f6d 2f44 6565 7050 6f73 654b 6974  .com/DeepPoseKit
-000010b0: 2f68 746d 6c2f 6465 6570 706f 7365 6b69  /html/deepposeki
-000010c0: 742f 6d6f 6465 6c73 2f53 7461 636b 6564  t/models/Stacked
-000010d0: 486f 7572 676c 6173 732e 6874 6d6c 292c  Hourglass.html),
-000010e0: 205b 6044 6565 704c 6162 4375 7460 5d28   [`DeepLabCut`](
-000010f0: 6874 7470 3a2f 2f6a 616b 6567 7261 7669  http://jakegravi
-00001100: 6e67 2e63 6f6d 2f44 6565 7050 6f73 654b  ng.com/DeepPoseK
-00001110: 6974 2f68 746d 6c2f 6465 6570 706f 7365  it/html/deeppose
-00001120: 6b69 742f 6d6f 6465 6c73 2f44 6565 704c  kit/models/DeepL
-00001130: 6162 4375 742e 6874 6d6c 292c 2061 6e64  abCut.html), and
-00001140: 205b 604c 4541 5060 5d28 6874 7470 3a2f   [`LEAP`](http:/
-00001150: 2f6a 616b 6567 7261 7669 6e67 2e63 6f6d  /jakegraving.com
-00001160: 2f44 6565 7050 6f73 654b 6974 2f68 746d  /DeepPoseKit/htm
-00001170: 6c2f 6465 6570 706f 7365 6b69 742f 6d6f  l/deepposekit/mo
-00001180: 6465 6c73 2f4c 4541 502e 6874 6d6c 292e  dels/LEAP.html).
-00001190: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-000011a0: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
-000011b0: 2e67 6f6f 676c 652e 636f 6d2f 6769 7468  .google.com/gith
-000011c0: 7562 2f6a 6772 6176 696e 672f 6465 6570  ub/jgraving/deep
-000011d0: 706f 7365 6b69 742f 626c 6f62 2f6d 6173  posekit/blob/mas
-000011e0: 7465 722f 6578 616d 706c 6573 2f73 7465  ter/examples/ste
-000011f0: 7033 5f74 7261 696e 5f6d 6f64 656c 2e69  p3_train_model.i
-00001200: 7079 6e62 2220 7461 7267 6574 3d22 5f70  pynb" target="_p
-00001210: 6172 656e 7422 3e3c 696d 6720 7372 633d  arent"><img src=
-00001220: 2268 7474 7073 3a2f 2f63 6f6c 6162 2e72  "https://colab.r
-00001230: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
-00001240: 6f6d 2f61 7373 6574 732f 636f 6c61 622d  om/assets/colab-
-00001250: 6261 6467 652e 7376 6722 2061 6c74 3d22  badge.svg" alt="
-00001260: 4f70 656e 2049 6e20 436f 6c61 6222 2f3e  Open In Colab"/>
-00001270: 3c2f 613e 0d0a 2d20 2a2a 342e 2a2a 2055  </a>..- **4.** U
-00001280: 7365 2074 6865 2074 7261 696e 6564 206d  se the trained m
-00001290: 6f64 656c 2074 6f3a 0d0a 092d 2061 2920  odel to:...- a) 
-000012a0: 5b49 6e69 7469 616c 697a 6520 6b65 7970  [Initialize keyp
-000012b0: 6f69 6e74 7320 666f 7220 756e 616e 6e6f  oints for unanno
-000012c0: 7461 7465 6420 6461 7461 5d28 6874 7470  tated data](http
-000012d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-000012e0: 6772 6176 696e 672f 4465 6570 506f 7365  graving/DeepPose
-000012f0: 4b69 742f 626c 6f62 2f6d 6173 7465 722f  Kit/blob/master/
-00001300: 6578 616d 706c 6573 2f73 7465 7034 615f  examples/step4a_
-00001310: 696e 6974 6961 6c69 7a65 5f61 6e6e 6f74  initialize_annot
-00001320: 6174 696f 6e73 2e69 7079 6e62 2920 666f  ations.ipynb) fo
-00001330: 7220 6661 7374 6572 2061 6e6e 6f74 6174  r faster annotat
-00001340: 696f 6e73 2077 6974 6820 2a61 6374 6976  ions with *activ
-00001350: 6520 6c65 6172 6e69 6e67 2a2e 203c 6120  e learning*. <a 
-00001360: 6872 6566 3d22 6874 7470 733a 2f2f 636f  href="https://co
-00001370: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00001380: 676c 652e 636f 6d2f 6769 7468 7562 2f6a  gle.com/github/j
-00001390: 6772 6176 696e 672f 6465 6570 706f 7365  graving/deeppose
-000013a0: 6b69 742f 626c 6f62 2f6d 6173 7465 722f  kit/blob/master/
-000013b0: 6578 616d 706c 6573 2f73 7465 7034 615f  examples/step4a_
-000013c0: 696e 6974 6961 6c69 7a65 5f61 6e6e 6f74  initialize_annot
-000013d0: 6174 696f 6e73 2e69 7079 6e62 2220 7461  ations.ipynb" ta
-000013e0: 7267 6574 3d22 5f70 6172 656e 7422 3e3c  rget="_parent"><
-000013f0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00001400: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
-00001410: 676f 6f67 6c65 2e63 6f6d 2f61 7373 6574  google.com/asset
-00001420: 732f 636f 6c61 622d 6261 6467 652e 7376  s/colab-badge.sv
-00001430: 6722 2061 6c74 3d22 4f70 656e 2049 6e20  g" alt="Open In 
-00001440: 436f 6c61 6222 2f3e 3c2f 613e 0d0a 092d  Colab"/></a>...-
-00001450: 2062 2920 5b50 7265 6469 6374 206f 6e20   b) [Predict on 
-00001460: 6e65 7720 6461 7461 2061 6e64 2072 6566  new data and ref
-00001470: 696e 6520 7468 6520 7472 6169 6e69 6e67  ine the training
-00001480: 2073 6574 5d28 6874 7470 733a 2f2f 6769   set](https://gi
-00001490: 7468 7562 2e63 6f6d 2f6a 6772 6176 696e  thub.com/jgravin
-000014a0: 672f 4465 6570 506f 7365 4b69 742f 626c  g/DeepPoseKit/bl
-000014b0: 6f62 2f6d 6173 7465 722f 6578 616d 706c  ob/master/exampl
-000014c0: 6573 2f73 7465 7034 625f 7072 6564 6963  es/step4b_predic
-000014d0: 745f 6e65 775f 6461 7461 2e69 7079 6e62  t_new_data.ipynb
-000014e0: 2920 746f 2069 6d70 726f 7665 2070 6572  ) to improve per
-000014f0: 666f 726d 616e 6365 2e20 3c61 2068 7265  formance. <a hre
-00001500: 663d 2268 7474 7073 3a2f 2f63 6f6c 6162  f="https://colab
-00001510: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
-00001520: 2e63 6f6d 2f67 6974 6875 622f 6a67 7261  .com/github/jgra
-00001530: 7669 6e67 2f64 6565 7070 6f73 656b 6974  ving/deepposekit
-00001540: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
-00001550: 6d70 6c65 732f 7374 6570 3462 5f70 7265  mples/step4b_pre
-00001560: 6469 6374 5f6e 6577 5f64 6174 612e 6970  dict_new_data.ip
-00001570: 796e 6222 2074 6172 6765 743d 225f 7061  ynb" target="_pa
-00001580: 7265 6e74 223e 3c69 6d67 2073 7263 3d22  rent"><img src="
-00001590: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-000015a0: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-000015b0: 6d2f 6173 7365 7473 2f63 6f6c 6162 2d62  m/assets/colab-b
-000015c0: 6164 6765 2e73 7667 2220 616c 743d 224f  adge.svg" alt="O
-000015d0: 7065 6e20 496e 2043 6f6c 6162 222f 3e3c  pen In Colab"/><
-000015e0: 2f61 3e0d 0a0d 0a23 2320 466f 7220 6d6f  /a>....## For mo
-000015f0: 7265 2064 6574 6169 6c73 3a0d 0a0d 0a2d  re details:....-
-00001600: 2053 6565 205b 6f75 7220 6578 616d 706c   See [our exampl
-00001610: 6520 6e6f 7465 626f 6f6b 735d 2868 7474  e notebooks](htt
-00001620: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001630: 6a67 7261 7669 6e67 2f64 6565 7070 6f73  jgraving/deeppos
-00001640: 656b 6974 2f62 6c6f 622f 6d61 7374 6572  ekit/blob/master
-00001650: 2f65 7861 6d70 6c65 732f 290d 0a2d 2043  /examples/)..- C
-00001660: 6865 636b 2074 6865 205b 646f 6375 6d65  heck the [docume
-00001670: 6e74 6174 696f 6e5d 2868 7474 703a 2f2f  ntation](http://
-00001680: 646f 6373 2e64 6565 7070 6f73 656b 6974  docs.deepposekit
-00001690: 2e6f 7267 290d 0a2d 2052 6561 6420 5b6f  .org)..- Read [o
-000016a0: 7572 2070 6170 6572 5d28 6874 7470 733a  ur paper](https:
-000016b0: 2f2f 646f 692e 6f72 672f 3130 2e37 3535  //doi.org/10.755
-000016c0: 342f 654c 6966 652e 3437 3939 3429 0d0a  4/eLife.47994)..
-000016d0: 0d0a 2323 2022 4920 616c 7265 6164 7920  ..## "I already 
-000016e0: 6861 7665 2061 6e6e 6f74 6174 6564 2064  have annotated d
-000016f0: 6174 6122 0d0a 0d0a 4465 6570 506f 7365  ata"....DeepPose
-00001700: 4b69 7420 6973 2064 6573 6967 6e65 6420  Kit is designed 
-00001710: 746f 2062 6520 6578 7465 6e73 6962 6c65  to be extensible
-00001720: 2c20 736f 206c 6f61 6469 6e67 2064 6174  , so loading dat
-00001730: 6120 696e 206f 7468 6572 2066 6f72 6d61  a in other forma
-00001740: 7473 2069 7320 706f 7373 6962 6c65 2e0d  ts is possible..
-00001750: 0a0d 0a49 6620 796f 7520 6861 7665 2061  ...If you have a
-00001760: 6e6e 6f74 6174 6564 2064 6174 6120 6672  nnotated data fr
-00001770: 6f6d 2044 6565 704c 6162 4375 7420 2868  om DeepLabCut (h
-00001780: 7474 703a 2f2f 6465 6570 6c61 6263 7574  ttp://deeplabcut
-00001790: 2e6f 7267 292c 2074 7279 205b 6f75 7220  .org), try [our 
-000017a0: 2865 7870 6572 696d 656e 7461 6c29 2065  (experimental) e
-000017b0: 7861 6d70 6c65 206e 6f74 6562 6f6f 6b20  xample notebook 
-000017c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000017d0: 2e63 6f6d 2f6a 6772 6176 696e 672f 4465  .com/jgraving/De
-000017e0: 6570 506f 7365 4b69 742f 626c 6f62 2f6d  epPoseKit/blob/m
-000017f0: 6173 7465 722f 6578 616d 706c 6573 2f64  aster/examples/d
-00001800: 6565 706c 6162 6375 745f 6461 7461 5f65  eeplabcut_data_e
-00001810: 7861 6d70 6c65 2e69 7079 6e62 2920 666f  xample.ipynb) fo
-00001820: 7220 6c6f 6164 696e 6720 6461 7461 2069  r loading data i
-00001830: 6e20 7468 6973 2066 6f72 6d61 742e 203c  n this format. <
-00001840: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001850: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-00001860: 6f6f 676c 652e 636f 6d2f 6769 7468 7562  oogle.com/github
-00001870: 2f6a 6772 6176 696e 672f 6465 6570 706f  /jgraving/deeppo
-00001880: 7365 6b69 742f 626c 6f62 2f6d 6173 7465  sekit/blob/maste
-00001890: 722f 6578 616d 706c 6573 2f64 6565 706c  r/examples/deepl
-000018a0: 6162 6375 745f 6461 7461 5f65 7861 6d70  abcut_data_examp
-000018b0: 6c65 2e69 7079 6e62 2220 7461 7267 6574  le.ipynb" target
-000018c0: 3d22 5f70 6172 656e 7422 3e3c 696d 6720  ="_parent"><img 
-000018d0: 7372 633d 2268 7474 7073 3a2f 2f63 6f6c  src="https://col
-000018e0: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
-000018f0: 6c65 2e63 6f6d 2f61 7373 6574 732f 636f  le.com/assets/co
-00001900: 6c61 622d 6261 6467 652e 7376 6722 2061  lab-badge.svg" a
-00001910: 6c74 3d22 4f70 656e 2049 6e20 436f 6c61  lt="Open In Cola
-00001920: 6222 2f3e 3c2f 613e 0d0a 0d0a 4861 7665  b"/></a>....Have
-00001930: 2064 6174 6120 696e 2061 6e6f 7468 6572   data in another
-00001940: 2066 6f72 6d61 743f 2059 6f75 2063 616e   format? You can
-00001950: 2077 7269 7465 2079 6f75 7220 6f77 6e20   write your own 
-00001960: 6375 7374 6f6d 2067 656e 6572 6174 6f72  custom generator
-00001970: 2074 6f20 6c6f 6164 2069 742e 0d0a 4368   to load it...Ch
-00001980: 6563 6b20 6f75 7420 7468 6520 5b65 7861  eck out the [exa
-00001990: 6d70 6c65 2066 6f72 2077 7269 7469 6e67  mple for writing
-000019a0: 2063 7573 746f 6d20 6461 7461 2067 656e   custom data gen
-000019b0: 6572 6174 6f72 735d 2868 7474 7073 3a2f  erators](https:/
-000019c0: 2f67 6974 6875 622e 636f 6d2f 6a67 7261  /github.com/jgra
-000019d0: 7669 6e67 2f44 6565 7050 6f73 654b 6974  ving/DeepPoseKit
-000019e0: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
-000019f0: 6d70 6c65 732f 6375 7374 6f6d 5f64 6174  mples/custom_dat
-00001a00: 615f 6765 6e65 7261 746f 722e 6970 796e  a_generator.ipyn
-00001a10: 6229 2e20 3c61 2068 7265 663d 2268 7474  b). <a href="htt
-00001a20: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
-00001a30: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f67  rch.google.com/g
-00001a40: 6974 6875 622f 6a67 7261 7669 6e67 2f64  ithub/jgraving/d
-00001a50: 6565 7070 6f73 656b 6974 2f62 6c6f 622f  eepposekit/blob/
-00001a60: 6d61 7374 6572 2f65 7861 6d70 6c65 732f  master/examples/
-00001a70: 6375 7374 6f6d 5f64 6174 615f 6765 6e65  custom_data_gene
-00001a80: 7261 746f 722e 6970 796e 6222 2074 6172  rator.ipynb" tar
-00001a90: 6765 743d 225f 7061 7265 6e74 223e 3c69  get="_parent"><i
-00001aa0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001ab0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-00001ac0: 6f6f 676c 652e 636f 6d2f 6173 7365 7473  oogle.com/assets
-00001ad0: 2f63 6f6c 6162 2d62 6164 6765 2e73 7667  /colab-badge.svg
-00001ae0: 2220 616c 743d 224f 7065 6e20 496e 2043  " alt="Open In C
-00001af0: 6f6c 6162 222f 3e3c 2f61 3e0d 0a0d 0a23  olab"/></a>....#
-00001b00: 2049 6e73 7461 6c6c 6174 696f 6e0d 0a0d   Installation...
-00001b10: 0a44 6565 7050 6f73 654b 6974 2072 6571  .DeepPoseKit req
-00001b20: 7569 7265 7320 5b54 656e 736f 7266 6c6f  uires [Tensorflo
-00001b30: 775d 2868 7474 7073 3a2f 2f67 6974 6875  w](https://githu
-00001b40: 622e 636f 6d2f 7465 6e73 6f72 666c 6f77  b.com/tensorflow
-00001b50: 2f74 656e 736f 7266 6c6f 7729 2066 6f72  /tensorflow) for
-00001b60: 2074 7261 696e 696e 6720 616e 6420 7573   training and us
-00001b70: 696e 6720 706f 7365 2065 7374 696d 6174  ing pose estimat
-00001b80: 696f 6e20 6d6f 6465 6c73 2e20 5b54 656e  ion models. [Ten
-00001b90: 736f 7266 6c6f 775d 2868 7474 7073 3a2f  sorflow](https:/
-00001ba0: 2f67 6974 6875 622e 636f 6d2f 7465 6e73  /github.com/tens
-00001bb0: 6f72 666c 6f77 2f74 656e 736f 7266 6c6f  orflow/tensorflo
-00001bc0: 7729 2073 686f 756c 6420 6265 206d 616e  w) should be man
-00001bd0: 7561 6c6c 7920 696e 7374 616c 6c65 642c  ually installed,
-00001be0: 2061 6c6f 6e67 2077 6974 6820 6465 7065   along with depe
-00001bf0: 6e64 656e 6369 6573 2073 7563 6820 6173  ndencies such as
-00001c00: 2043 5544 4120 616e 6420 6375 444e 4e2c   CUDA and cuDNN,
-00001c10: 2062 6566 6f72 6520 696e 7374 616c 6c69   before installi
-00001c20: 6e67 2044 6565 7050 6f73 654b 6974 3a0d  ng DeepPoseKit:.
-00001c30: 0a0d 0a2d 205b 5465 6e73 6f72 666c 6f77  ...- [Tensorflow
-00001c40: 2049 6e73 7461 6c6c 6174 696f 6e20 496e   Installation In
-00001c50: 7374 7275 6374 696f 6e73 5d28 6874 7470  structions](http
-00001c60: 733a 2f2f 7777 772e 7465 6e73 6f72 666c  s://www.tensorfl
-00001c70: 6f77 2e6f 7267 2f69 6e73 7461 6c6c 290d  ow.org/install).
-00001c80: 0a2d 2041 6e79 2054 656e 736f 7266 6c6f  .- Any Tensorflo
-00001c90: 7720 7665 7273 696f 6e20 3e3d 312e 3133  w version >=1.13
-00001ca0: 2e30 2073 686f 756c 6420 6265 2063 6f6d  .0 should be com
-00001cb0: 7061 7469 626c 6520 2869 6e63 6c75 6469  patible (includi
-00001cc0: 6e67 2032 2e30 292e 0d0a 0d0a 4465 6570  ng 2.0).....Deep
-00001cd0: 506f 7365 4b69 7420 6861 7320 6f6e 6c79  PoseKit has only
-00001ce0: 2062 6565 6e20 7465 7374 6564 206f 6e20   been tested on 
-00001cf0: 5562 756e 7475 2031 382e 3034 2c20 7768  Ubuntu 18.04, wh
-00001d00: 6963 6820 6973 2074 6865 2072 6563 6f6d  ich is the recom
-00001d10: 6d65 6e64 6564 2073 7973 7465 6d20 666f  mended system fo
-00001d20: 7220 7573 696e 6720 7468 6520 746f 6f6c  r using the tool
-00001d30: 6b69 742e 200d 0a0d 0a49 6e73 7461 6c6c  kit. ....Install
-00001d40: 2074 6865 206c 6174 6573 7420 7374 6162   the latest stab
-00001d50: 6c65 2072 656c 6561 7365 2077 6974 6820  le release with 
-00001d60: 7069 703a 0d0a 6060 6062 6173 680d 0a70  pip:..```bash..p
-00001d70: 6970 2069 6e73 7461 6c6c 202d 2d75 7064  ip install --upd
-00001d80: 6174 6520 6465 6570 706f 7365 6b69 740d  ate deepposekit.
-00001d90: 0a60 6060 0d0a 0d0a 496e 7374 616c 6c20  .```....Install 
-00001da0: 7468 6520 6c61 7465 7374 2064 6576 656c  the latest devel
-00001db0: 6f70 6d65 6e74 2076 6572 7369 6f6e 2077  opment version w
-00001dc0: 6974 6820 7069 703a 0d0a 6060 6062 6173  ith pip:..```bas
-00001dd0: 680d 0a70 6970 2069 6e73 7461 6c6c 202d  h..pip install -
-00001de0: 2d75 7064 6174 6520 6769 742b 6874 7470  -update git+http
-00001df0: 733a 2f2f 7777 772e 6769 7468 7562 2e63  s://www.github.c
-00001e00: 6f6d 2f6a 6772 6176 696e 672f 6465 6570  om/jgraving/deep
-00001e10: 706f 7365 6b69 742e 6769 740d 0a60 6060  posekit.git..```
-00001e20: 0d0a 0d0a 596f 7520 6361 6e20 646f 776e  ....You can down
-00001e30: 6c6f 6164 2065 7861 6d70 6c65 2064 6174  load example dat
-00001e40: 6173 6574 7320 6672 6f6d 206f 7572 205b  asets from our [
-00001e50: 4465 6570 506f 7365 4b69 7420 4461 7461  DeepPoseKit Data
-00001e60: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001e70: 2e63 6f6d 2f6a 6772 6176 696e 672f 6465  .com/jgraving/de
-00001e80: 6570 706f 7365 6b69 742d 6461 7461 2920  epposekit-data) 
-00001e90: 7265 706f 7369 746f 7279 3a0d 0a60 6060  repository:..```
-00001ea0: 6261 7368 0d0a 6769 7420 636c 6f6e 6520  bash..git clone 
-00001eb0: 6874 7470 733a 2f2f 7777 772e 6769 7468  https://www.gith
-00001ec0: 7562 2e63 6f6d 2f6a 6772 6176 696e 672f  ub.com/jgraving/
-00001ed0: 6465 6570 706f 7365 6b69 742d 6461 7461  deepposekit-data
-00001ee0: 0d0a 6060 600d 0a0d 0a23 2320 496e 7374  ..```....## Inst
-00001ef0: 616c 6c69 6e67 2077 6974 6820 416e 6163  alling with Anac
-00001f00: 6f6e 6461 206f 6e20 5769 6e64 6f77 730d  onda on Windows.
-00001f10: 0a0d 0a54 6f20 696e 7374 616c 6c20 4465  ...To install De
-00001f20: 6570 506f 7365 4b69 7420 6f6e 2057 696e  epPoseKit on Win
-00001f30: 646f 7773 2c20 796f 7520 6d75 7374 2066  dows, you must f
-00001f40: 6972 7374 206d 616e 7561 6c6c 7920 696e  irst manually in
-00001f50: 7374 616c 6c20 6053 6861 7065 6c79 602c  stall `Shapely`,
-00001f60: 206f 6e65 206f 6620 7468 6520 6465 7065   one of the depe
-00001f70: 6e64 656e 6369 6573 2066 6f72 2074 6865  ndencies for the
-00001f80: 205b 696d 6761 7567 2070 6163 6b61 6765   [imgaug package
-00001f90: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001fa0: 2e63 6f6d 2f61 6c65 6a75 2f69 6d67 6175  .com/aleju/imgau
-00001fb0: 6729 3a0d 0a60 6060 6261 7368 0d0a 636f  g):..```bash..co
-00001fc0: 6e64 6120 696e 7374 616c 6c20 2d63 2063  nda install -c c
-00001fd0: 6f6e 6461 2d66 6f72 6765 2073 6861 7065  onda-forge shape
-00001fe0: 6c79 0d0a 6060 600d 0a57 6520 616c 736f  ly..```..We also
-00001ff0: 2072 6563 6f6d 6d65 6e64 2069 6e73 7461   recommend insta
-00002000: 6c6c 696e 6720 4465 6570 506f 7365 4b69  lling DeepPoseKi
-00002010: 7420 6672 6f6d 2077 6974 6869 6e20 5079  t from within Py
-00002020: 7468 6f6e 2072 6174 6865 7220 7468 616e  thon rather than
-00002030: 2075 7369 6e67 2074 6865 2063 6f6d 6d61   using the comma
-00002040: 6e64 206c 696e 652c 2065 6974 6865 7220  nd line, either 
-00002050: 6672 6f6d 2077 6974 6869 6e20 4a75 7079  from within Jupy
-00002060: 7465 7220 6f72 2061 6e6f 7468 6572 2049  ter or another I
-00002070: 4445 2c20 746f 2065 6e73 7572 6520 6974  DE, to ensure it
-00002080: 2069 7320 696e 7374 616c 6c65 6420 696e   is installed in
-00002090: 2074 6865 2063 6f72 7265 6374 2077 6f72   the correct wor
-000020a0: 6b69 6e67 2065 6e76 6972 6f6e 6d65 6e74  king environment
-000020b0: 3a0d 0a60 6060 7079 7468 6f6e 0d0a 696d  :..```python..im
-000020c0: 706f 7274 2073 7973 0d0a 217b 7379 732e  port sys..!{sys.
-000020d0: 6578 6563 7574 6162 6c65 7d20 2d6d 2070  executable} -m p
-000020e0: 6970 2069 6e73 7461 6c6c 202d 2d75 7064  ip install --upd
-000020f0: 6174 6520 6465 6570 706f 7365 6b69 740d  ate deepposekit.
-00002100: 0a60 6060 0d0a 2320 436f 6e74 7269 6275  .```..# Contribu
-00002110: 746f 7273 2061 6e64 2044 6576 656c 6f70  tors and Develop
-00002120: 6d65 6e74 2020 0d0a 2020 200d 0a44 6565  ment  ..   ..Dee
-00002130: 7050 6f73 654b 6974 2077 6173 2064 6576  pPoseKit was dev
-00002140: 656c 6f70 6564 2062 7920 5b4a 616b 6520  eloped by [Jake 
-00002150: 4772 6176 696e 675d 2868 7474 7073 3a2f  Graving](https:/
-00002160: 2f67 6974 6875 622e 636f 6d2f 6a67 7261  /github.com/jgra
-00002170: 7669 6e67 2920 616e 6420 5b44 616e 6965  ving) and [Danie
-00002180: 6c20 4368 6165 5d28 6874 7470 733a 2f2f  l Chae](https://
-00002190: 6769 7468 7562 2e63 6f6d 2f64 6368 6165  github.com/dchae
-000021a0: 6261 6529 2c20 616e 6420 6973 2073 7469  bae), and is sti
-000021b0: 6c6c 2062 6569 6e67 2061 6374 6976 656c  ll being activel
-000021c0: 7920 6465 7665 6c6f 7065 642e 202e 0d0a  y developed. ...
-000021d0: 0d0a 5765 2077 656c 636f 6d65 2063 6f6d  ..We welcome com
-000021e0: 6d75 6e69 7479 2069 6e76 6f6c 7665 6d65  munity involveme
-000021f0: 6e74 2061 6e64 2070 7562 6c69 6320 636f  nt and public co
-00002200: 6e74 7269 6275 7469 6f6e 7320 746f 2074  ntributions to t
-00002210: 6865 2074 6f6f 6c6b 6974 2e20 4966 2079  he toolkit. If y
-00002220: 6f75 2077 6973 6820 746f 2063 6f6e 7472  ou wish to contr
-00002230: 6962 7574 652c 2070 6c65 6173 6520 5b66  ibute, please [f
-00002240: 6f72 6b20 7468 6520 7265 706f 7369 746f  ork the reposito
-00002250: 7279 5d28 6874 7470 733a 2f2f 6865 6c70  ry](https://help
-00002260: 2e67 6974 6875 622e 636f 6d2f 656e 2f61  .github.com/en/a
-00002270: 7274 6963 6c65 732f 666f 726b 2d61 2d72  rticles/fork-a-r
-00002280: 6570 6f29 2074 6f20 6d61 6b65 2079 6f75  epo) to make you
-00002290: 7220 6d6f 6469 6669 6361 7469 6f6e 7320  r modifications 
-000022a0: 616e 6420 5b73 7562 6d69 7420 6120 7075  and [submit a pu
-000022b0: 6c6c 2072 6571 7565 7374 5d28 6874 7470  ll request](http
-000022c0: 733a 2f2f 6865 6c70 2e67 6974 6875 622e  s://help.github.
-000022d0: 636f 6d2f 656e 2f61 7274 6963 6c65 732f  com/en/articles/
-000022e0: 6372 6561 7469 6e67 2d61 2d70 756c 6c2d  creating-a-pull-
-000022f0: 7265 7175 6573 742d 6672 6f6d 2d61 2d66  request-from-a-f
-00002300: 6f72 6b29 2e0d 0a0d 0a49 6620 796f 7527  ork).....If you'
-00002310: 6420 6c69 6b65 2074 6f20 6765 7420 696e  d like to get in
-00002320: 766f 6c76 6564 2077 6974 6820 6465 7665  volved with deve
-00002330: 6c6f 7069 6e67 2044 6565 7050 6f73 654b  loping DeepPoseK
-00002340: 6974 2c20 6765 7420 696e 2074 6f75 6368  it, get in touch
-00002350: 2028 6a67 7261 7669 6e67 4067 6d61 696c   (jgraving@gmail
-00002360: 2e63 6f6d 2920 616e 6420 6368 6563 6b20  .com) and check 
-00002370: 6f75 7420 5b6f 7572 2064 6576 656c 6f70  out [our develop
-00002380: 6d65 6e74 2072 6f61 646d 6170 5d28 6874  ment roadmap](ht
-00002390: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000023a0: 2f6a 6772 6176 696e 672f 4465 6570 506f  /jgraving/DeepPo
-000023b0: 7365 4b69 742f 626c 6f62 2f6d 6173 7465  seKit/blob/maste
-000023c0: 722f 4445 5645 4c4f 504d 454e 542e 6d64  r/DEVELOPMENT.md
-000023d0: 2920 746f 2073 6565 2066 7574 7572 6520  ) to see future 
-000023e0: 706c 616e 7320 666f 7220 7468 6520 7061  plans for the pa
-000023f0: 636b 6167 652e 2020 0d0a 0d0a 2320 4973  ckage.  ....# Is
-00002400: 7375 6573 2020 0d0a 200d 0a50 6c65 6173  sues  .. ..Pleas
-00002410: 6520 7375 626d 6974 2062 7567 7320 6f72  e submit bugs or
-00002420: 2066 6561 7475 7265 2072 6571 7565 7374   feature request
-00002430: 7320 746f 2074 6865 205b 4769 7448 7562  s to the [GitHub
-00002440: 2069 7373 7565 2074 7261 636b 6572 5d28   issue tracker](
-00002450: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002460: 6f6d 2f6a 6772 6176 696e 672f 6465 6570  om/jgraving/deep
-00002470: 706f 7365 6b69 742f 6973 7375 6573 2f6e  posekit/issues/n
-00002480: 6577 292e 2050 6c65 6173 6520 6c69 6d69  ew). Please limi
-00002490: 7420 7265 706f 7274 6564 2069 7373 7565  t reported issue
-000024a0: 7320 746f 2074 6865 2044 6565 7050 6f73  s to the DeepPos
-000024b0: 654b 6974 2063 6f64 6562 6173 6520 616e  eKit codebase an
-000024c0: 6420 7072 6f76 6964 6520 6173 206d 7563  d provide as muc
-000024d0: 6820 6465 7461 696c 2061 7320 796f 7520  h detail as you 
-000024e0: 6361 6e20 7769 7468 2061 206d 696e 696d  can with a minim
-000024f0: 616c 2077 6f72 6b69 6e67 2065 7861 6d70  al working examp
-00002500: 6c65 2069 6620 706f 7373 6962 6c65 2e0d  le if possible..
-00002510: 0a0d 0a49 6620 796f 7520 6578 7065 7269  ...If you experi
-00002520: 656e 6365 2070 726f 626c 656d 7320 7769  ence problems wi
-00002530: 7468 205b 5465 6e73 6f72 666c 6f77 5d28  th [Tensorflow](
-00002540: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002550: 6f6d 2f74 656e 736f 7266 6c6f 772f 7465  om/tensorflow/te
-00002560: 6e73 6f72 666c 6f77 292c 2073 7563 6820  nsorflow), such 
-00002570: 6173 2069 6e73 7461 6c6c 696e 6720 4355  as installing CU
-00002580: 4441 206f 7220 6375 444e 4e20 6465 7065  DA or cuDNN depe
-00002590: 6e64 656e 6369 6573 2c20 7468 656e 2070  ndencies, then p
-000025a0: 6c65 6173 6520 6469 7265 6374 2069 7373  lease direct iss
-000025b0: 7565 7320 746f 2074 686f 7365 2064 6576  ues to those dev
-000025c0: 656c 6f70 6d65 6e74 2074 6561 6d73 2e0d  elopment teams..
-000025d0: 0a0d 0a23 204c 6963 656e 7365 0d0a 0d0a  ...# License....
-000025e0: 5265 6c65 6173 6564 2075 6e64 6572 2061  Released under a
-000025f0: 2041 7061 6368 6520 322e 3020 4c69 6365   Apache 2.0 Lice
-00002600: 6e73 652e 2053 6565 205b 4c49 4345 4e53  nse. See [LICENS
-00002610: 455d 2868 7474 7073 3a2f 2f67 6974 6875  E](https://githu
-00002620: 622e 636f 6d2f 6a67 7261 7669 6e67 2f64  b.com/jgraving/d
-00002630: 6565 7070 6f73 656b 6974 2f62 6c6f 622f  eepposekit/blob/
-00002640: 6d61 7374 6572 2f4c 4943 454e 5345 2920  master/LICENSE) 
-00002650: 666f 7220 6465 7461 696c 732e 0d0a 0d0a  for details.....
-00002660: 2320 5265 6665 7265 6e63 6573 0d0a 0d0a  # References....
-00002670: 4966 2079 6f75 2075 7365 2044 6565 7050  If you use DeepP
-00002680: 6f73 654b 6974 2066 6f72 2079 6f75 7220  oseKit for your 
-00002690: 7265 7365 6172 6368 2070 6c65 6173 6520  research please 
-000026a0: 6369 7465 205b 6f75 7220 6f70 656e 2d61  cite [our open-a
-000026b0: 6363 6573 7320 7061 7065 725d 2868 7474  ccess paper](htt
-000026c0: 703a 2f2f 7061 7065 722e 6465 6570 706f  p://paper.deeppo
-000026d0: 7365 6b69 742e 6f72 6729 3a0d 0a0d 0a20  sekit.org):.... 
-000026e0: 2020 2040 6172 7469 636c 657b 6772 6176     @article{grav
-000026f0: 696e 6732 3031 3964 6565 7070 6f73 656b  ing2019deepposek
-00002700: 6974 2c0d 0a20 2020 2020 2020 2020 2020  it,..           
-00002710: 2020 7469 746c 653d 7b44 6565 7050 6f73    title={DeepPos
-00002720: 654b 6974 2c20 6120 736f 6674 7761 7265  eKit, a software
-00002730: 2074 6f6f 6c6b 6974 2066 6f72 2066 6173   toolkit for fas
-00002740: 7420 616e 6420 726f 6275 7374 2061 6e69  t and robust ani
-00002750: 6d61 6c20 706f 7365 2065 7374 696d 6174  mal pose estimat
-00002760: 696f 6e20 7573 696e 6720 6465 6570 206c  ion using deep l
-00002770: 6561 726e 696e 677d 2c0d 0a20 2020 2020  earning},..     
-00002780: 2020 2020 2020 2020 6175 7468 6f72 3d7b          author={
-00002790: 4772 6176 696e 672c 204a 6163 6f62 204d  Graving, Jacob M
-000027a0: 2061 6e64 2043 6861 652c 2044 616e 6965   and Chae, Danie
-000027b0: 6c20 616e 6420 4e61 696b 2c20 4865 6d61  l and Naik, Hema
-000027c0: 6c20 616e 6420 4c69 2c20 4c69 616e 6720  l and Li, Liang 
-000027d0: 616e 6420 4b6f 6765 722c 2042 656e 6a61  and Koger, Benja
-000027e0: 6d69 6e20 616e 6420 436f 7374 656c 6c6f  min and Costello
-000027f0: 652c 2042 6c61 6972 2052 2061 6e64 2043  e, Blair R and C
-00002800: 6f75 7a69 6e2c 2049 6169 6e20 447d 2c0d  ouzin, Iain D},.
-00002810: 0a20 2020 2020 2020 2020 2020 2020 6a6f  .             jo
-00002820: 7572 6e61 6c3d 7b65 4c69 6665 7d2c 0d0a  urnal={eLife},..
-00002830: 2020 2020 2020 2020 2020 2020 2076 6f6c               vol
-00002840: 756d 653d 7b38 7d2c 0d0a 2020 2020 2020  ume={8},..      
-00002850: 2020 2020 2020 2070 6167 6573 3d7b 6534         pages={e4
-00002860: 3739 3934 7d2c 0d0a 2020 2020 2020 2020  7994},..        
-00002870: 2020 2020 2079 6561 723d 7b32 3031 397d       year={2019}
-00002880: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00002890: 7075 626c 6973 6865 723d 7b65 4c69 6665  publisher={eLife
-000028a0: 2053 6369 656e 6365 7320 5075 626c 6963   Sciences Public
-000028b0: 6174 696f 6e73 204c 696d 6974 6564 7d0d  ations Limited}.
-000028c0: 0a20 2020 2020 2020 2020 2020 2020 7572  .             ur
-000028d0: 6c3d 7b68 7474 7073 3a2f 2f64 6f69 2e6f  l={https://doi.o
-000028e0: 7267 2f31 302e 3735 3534 2f65 4c69 6665  rg/10.7554/eLife
-000028f0: 2e34 3739 3934 7d2c 0d0a 2020 2020 2020  .47994},..      
-00002900: 2020 2020 2020 207d 0d0a 0d0a 596f 7520         }....You 
-00002910: 6361 6e20 616c 736f 2072 6561 6420 5b6f  can also read [o
-00002920: 7572 206f 7065 6e2d 6163 6365 7373 2070  ur open-access p
-00002930: 7265 7072 696e 745d 2868 7474 703a 2f2f  reprint](http://
-00002940: 7072 6570 7269 6e74 2e64 6565 7070 6f73  preprint.deeppos
-00002950: 656b 6974 2e6f 7267 292e 0d0a 0d0a 4966  ekit.org).....If
-00002960: 2079 6f75 2075 7365 2074 6865 205b 696d   you use the [im
-00002970: 6761 7567 2070 6163 6b61 6765 5d28 6874  gaug package](ht
-00002980: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002990: 2f61 6c65 6a75 2f69 6d67 6175 6729 2066  /aleju/imgaug) f
-000029a0: 6f72 2064 6174 6120 6175 676d 656e 7461  or data augmenta
-000029b0: 7469 6f6e 2c20 706c 6561 7365 2061 6c73  tion, please als
-000029c0: 6f20 636f 6e73 6964 6572 205b 6369 7469  o consider [citi
-000029d0: 6e67 2069 745d 2868 7474 7073 3a2f 2f67  ng it](https://g
-000029e0: 6974 6875 622e 636f 6d2f 616c 656a 752f  ithub.com/aleju/
-000029f0: 696d 6761 7567 2f62 6c6f 622f 6d61 7374  imgaug/blob/mast
-00002a00: 6572 2f52 4541 444d 452e 6d64 2363 6974  er/README.md#cit
-00002a10: 6174 696f 6e29 2e0d 0a0d 0a49 6620 796f  ation).....If yo
-00002a20: 7520 5b75 7365 2064 6174 615d 2868 7474  u [use data](htt
-00002a30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002a40: 6a67 7261 7669 6e67 2f44 6565 7050 6f73  jgraving/DeepPos
-00002a50: 654b 6974 2369 2d61 6c72 6561 6479 2d68  eKit#i-already-h
-00002a60: 6176 652d 616e 6e6f 7461 7465 642d 6461  ave-annotated-da
-00002a70: 7461 2920 7468 6174 2077 6173 2061 6e6e  ta) that was ann
-00002a80: 6f74 6174 6564 2077 6974 6820 7468 6520  otated with the 
-00002a90: 4465 6570 4c61 6243 7574 2070 6163 6b61  DeepLabCut packa
-00002aa0: 6765 2028 6874 7470 3a2f 2f64 6565 706c  ge (http://deepl
-00002ab0: 6162 6375 742e 6f72 6729 2066 6f72 2079  abcut.org) for y
-00002ac0: 6f75 7220 7265 7365 6172 6368 2c20 6265  our research, be
-00002ad0: 2073 7572 6520 746f 205b 6369 7465 2069   sure to [cite i
-00002ae0: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
-00002af0: 622e 636f 6d2f 416c 6578 454d 472f 4465  b.com/AlexEMG/De
-00002b00: 6570 4c61 6243 7574 2f62 6c6f 622f 6d61  epLabCut/blob/ma
-00002b10: 7374 6572 2f52 4541 444d 452e 6d64 2372  ster/README.md#r
-00002b20: 6566 6572 656e 6365 7329 2e0d 0a0d 0a50  eferences).....P
-00002b30: 6c65 6173 6520 616c 736f 2063 6f6e 7369  lease also consi
-00002b40: 6465 7220 6369 7469 6e67 2074 6865 2072  der citing the r
-00002b50: 656c 6576 616e 7420 7265 6665 7265 6e63  elevant referenc
-00002b60: 6573 2066 6f72 2074 6865 2070 6f73 6520  es for the pose 
-00002b70: 6573 7469 6d61 7469 6f6e 206d 6f64 656c  estimation model
-00002b80: 2873 2920 7573 6564 2069 6e20 796f 7572  (s) used in your
-00002b90: 2072 6573 6561 7263 682c 2077 6869 6368   research, which
-00002ba0: 2063 616e 2062 6520 666f 756e 6420 696e   can be found in
-00002bb0: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
-00002bc0: 6f6e 2028 692e 652e 2c20 5b60 5374 6163  on (i.e., [`Stac
-00002bd0: 6b65 6444 656e 7365 4e65 7460 5d28 6874  kedDenseNet`](ht
-00002be0: 7470 3a2f 2f6a 616b 6567 7261 7669 6e67  tp://jakegraving
-00002bf0: 2e63 6f6d 2f44 6565 7050 6f73 654b 6974  .com/DeepPoseKit
-00002c00: 2f68 746d 6c2f 6465 6570 706f 7365 6b69  /html/deepposeki
-00002c10: 742f 6d6f 6465 6c73 2f53 7461 636b 6564  t/models/Stacked
-00002c20: 4465 6e73 654e 6574 2e68 746d 6c23 7265  DenseNet.html#re
-00002c30: 6665 7265 6e63 6573 292c 205b 6053 7461  ferences), [`Sta
-00002c40: 636b 6564 486f 7572 676c 6173 7360 5d28  ckedHourglass`](
-00002c50: 6874 7470 3a2f 2f6a 616b 6567 7261 7669  http://jakegravi
-00002c60: 6e67 2e63 6f6d 2f44 6565 7050 6f73 654b  ng.com/DeepPoseK
-00002c70: 6974 2f68 746d 6c2f 6465 6570 706f 7365  it/html/deeppose
-00002c80: 6b69 742f 6d6f 6465 6c73 2f53 7461 636b  kit/models/Stack
-00002c90: 6564 486f 7572 676c 6173 732e 6874 6d6c  edHourglass.html
-00002ca0: 2372 6566 6572 656e 6365 7329 2c20 5b60  #references), [`
-00002cb0: 4465 6570 4c61 6243 7574 605d 2868 7474  DeepLabCut`](htt
-00002cc0: 703a 2f2f 6a61 6b65 6772 6176 696e 672e  p://jakegraving.
-00002cd0: 636f 6d2f 4465 6570 506f 7365 4b69 742f  com/DeepPoseKit/
-00002ce0: 6874 6d6c 2f64 6565 7070 6f73 656b 6974  html/deepposekit
-00002cf0: 2f6d 6f64 656c 732f 4465 6570 4c61 6243  /models/DeepLabC
-00002d00: 7574 2e68 746d 6c23 7265 6665 7265 6e63  ut.html#referenc
-00002d10: 6573 292c 205b 604c 4541 5060 5d28 6874  es), [`LEAP`](ht
-00002d20: 7470 3a2f 2f6a 616b 6567 7261 7669 6e67  tp://jakegraving
-00002d30: 2e63 6f6d 2f44 6565 7050 6f73 654b 6974  .com/DeepPoseKit
-00002d40: 2f68 746d 6c2f 6465 6570 706f 7365 6b69  /html/deepposeki
-00002d50: 742f 6d6f 6465 6c73 2f4c 4541 502e 6874  t/models/LEAP.ht
-00002d60: 6d6c 2372 6566 6572 656e 6365 7329 292e  ml#references)).
-00002d70: 0d0a 0d0a 2320 4e65 7773 0d0a 2d20 2a2a  ....# News..- **
-00002d80: 4f63 746f 6265 7220 3230 3139 3a2a 2a20  October 2019:** 
-00002d90: 4f75 7220 7061 7065 7220 6465 7363 7269  Our paper descri
-00002da0: 6269 6e67 2044 6565 7050 6f73 654b 6974  bing DeepPoseKit
-00002db0: 2069 7320 7075 626c 6973 6865 6420 6174   is published at
-00002dc0: 2065 4c69 6665 2120 2868 7474 703a 2f2f   eLife! (http://
-00002dd0: 7061 7065 722e 6465 6570 706f 7365 6b69  paper.deepposeki
-00002de0: 742e 6f72 6729 0d0a 2d20 2a2a 5365 7074  t.org)..- **Sept
-00002df0: 656d 6265 7220 3230 3139 2a2a 3a20 0d0a  ember 2019**: ..
-00002e00: 2020 2020 2d20 4e61 7475 7265 204e 6577      - Nature New
-00002e10: 7320 636f 7665 7273 2044 6565 7050 6f73  s covers DeepPos
-00002e20: 654b 6974 3a20 5b44 6565 7020 6c65 6172  eKit: [Deep lear
-00002e30: 6e69 6e67 2070 6f77 6572 7320 6120 6d6f  ning powers a mo
-00002e40: 7469 6f6e 2d74 7261 636b 696e 6720 7265  tion-tracking re
-00002e50: 766f 6c75 7469 6f6e 5d28 6874 7470 3a2f  volution](http:/
-00002e60: 2f64 6f69 2e6f 7267 2f31 302e 3130 3338  /doi.org/10.1038
-00002e70: 2f64 3431 3538 362d 3031 392d 3032 3934  /d41586-019-0294
-00002e80: 322d 3529 0d0a 2020 2020 2d20 7630 2e33  2-5)..    - v0.3
-00002e90: 2e30 2069 7320 7265 6c65 6173 6564 2e20  .0 is released. 
-00002ea0: 5365 6520 5b74 6865 2072 656c 6561 7365  See [the release
-00002eb0: 206e 6f74 6573 5d28 6874 7470 733a 2f2f   notes](https://
-00002ec0: 6769 7468 7562 2e63 6f6d 2f6a 6772 6176  github.com/jgrav
-00002ed0: 696e 672f 4465 6570 506f 7365 4b69 742f  ing/DeepPoseKit/
-00002ee0: 7265 6c65 6173 6573 2f74 6167 2f76 302e  releases/tag/v0.
-00002ef0: 332e 3029 2e0d 0a2d 202a 2a41 7072 696c  3.0)...- **April
-00002f00: 2032 3031 393a 2a2a 2054 6865 2044 6565   2019:** The Dee
-00002f10: 7050 6f73 654b 6974 2070 7265 7072 696e  pPoseKit preprin
-00002f20: 7420 6973 206f 6e20 6269 6f72 7869 7620  t is on biorxiv 
-00002f30: 2868 7474 703a 2f2f 7072 6570 7269 6e74  (http://preprint
-00002f40: 2e64 6565 7070 6f73 656b 6974 2e6f 7267  .deepposekit.org
-00002f50: 290d 0a                                  )..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310d 0a4e 616d 653a 2075 7332  : 2.1..Name: us2
+00000020: 6465 6570 706f 7365 6b69 740d 0a56 6572  deepposekit..Ver
+00000030: 7369 6f6e 3a20 302e 342e 300d 0a53 756d  sion: 0.4.0..Sum
+00000040: 6d61 7279 3a20 6120 746f 6f6c 6b69 7420  mary: a toolkit 
+00000050: 666f 7220 706f 7365 2065 7374 696d 6174  for pose estimat
+00000060: 696f 6e20 7573 696e 6720 6465 6570 206c  ion using deep l
+00000070: 6561 726e 696e 670d 0a48 6f6d 652d 7061  earning..Home-pa
+00000080: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
+00000090: 7562 2e63 6f6d 2f6a 6772 6176 696e 672f  ub.com/jgraving/
+000000a0: 6465 6570 706f 7365 6b69 740d 0a44 6f77  deepposekit..Dow
+000000b0: 6e6c 6f61 642d 5552 4c3a 2068 7474 7073  nload-URL: https
+000000c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a67  ://github.com/jg
+000000d0: 7261 7669 6e67 2f64 6565 7070 6f73 656b  raving/deepposek
+000000e0: 6974 2e67 6974 0d0a 4175 7468 6f72 3a20  it.git..Author: 
+000000f0: 4a61 636f 6220 4772 6176 696e 6720 3c6a  Jacob Graving <j
+00000100: 6772 6176 696e 6740 676d 6169 6c2e 636f  graving@gmail.co
+00000110: 6d3e 0d0a 4175 7468 6f72 2d65 6d61 696c  m>..Author-email
+00000120: 3a20 6a67 7261 7669 6e67 4067 6d61 696c  : jgraving@gmail
+00000130: 2e63 6f6d 0d0a 4d61 696e 7461 696e 6572  .com..Maintainer
+00000140: 3a20 4a61 636f 6220 4772 6176 696e 6720  : Jacob Graving 
+00000150: 3c6a 6772 6176 696e 6740 676d 6169 6c2e  <jgraving@gmail.
+00000160: 636f 6d3e 0d0a 4d61 696e 7461 696e 6572  com>..Maintainer
+00000170: 2d65 6d61 696c 3a20 6a67 7261 7669 6e67  -email: jgraving
+00000180: 4067 6d61 696c 2e63 6f6d 0d0a 4c69 6365  @gmail.com..Lice
+00000190: 6e73 653a 2041 7061 6368 6520 322e 300d  nse: Apache 2.0.
+000001a0: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
+000001b0: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+000001c0: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
+000001d0: 6368 0d0a 436c 6173 7369 6669 6572 3a20  ch..Classifier: 
+000001e0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001f0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000200: 3a20 330d 0a43 6c61 7373 6966 6965 723a  : 3..Classifier:
+00000210: 2054 6f70 6963 203a 3a20 5363 6965 6e74   Topic :: Scient
+00000220: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
+00000230: 203a 3a20 496d 6167 6520 5265 636f 676e   :: Image Recogn
+00000240: 6974 696f 6e0d 0a44 6573 6372 6970 7469  ition..Descripti
+00000250: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00000260: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
+00000270: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+00000280: 4345 4e53 450d 0a0d 0a3c 7020 616c 6967  CENSE....<p alig
+00000290: 6e3d 2263 656e 7465 7222 3e0d 0a3c 696d  n="center">..<im
+000002a0: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
+000002b0: 6974 6875 622e 636f 6d2f 6a67 7261 7669  ithub.com/jgravi
+000002c0: 6e67 2f44 6565 7050 6f73 654b 6974 2f62  ng/DeepPoseKit/b
+000002d0: 6c6f 622f 6d61 7374 6572 2f61 7373 6574  lob/master/asset
+000002e0: 732f 6465 6570 706f 7365 6b69 745f 6c6f  s/deepposekit_lo
+000002f0: 676f 2e70 6e67 2220 6865 6967 6874 3d22  go.png" height="
+00000300: 3332 3070 7822 3e0d 0a3c 2f70 3e0d 0a0d  320px">..</p>...
+00000310: 0a23 2059 6f75 2068 6176 6520 6a75 7374  .# You have just
+00000320: 2066 6f75 6e64 2044 6565 7050 6f73 654b   found DeepPoseK
+00000330: 6974 2e0d 0a3c 7020 616c 6967 6e3d 2263  it...<p align="c
+00000340: 656e 7465 7222 3e0d 0a3c 696d 6720 7372  enter">..<img sr
+00000350: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00000360: 622e 636f 6d2f 6a67 7261 7669 6e67 2f6a  b.com/jgraving/j
+00000370: 6772 6176 696e 672e 6769 7468 7562 2e69  graving.github.i
+00000380: 6f2f 626c 6f62 2f6d 6173 7465 722f 6669  o/blob/master/fi
+00000390: 6c65 732f 696d 6167 6573 2f46 6967 7572  les/images/Figur
+000003a0: 6531 7669 6465 6f31 2e67 6966 2220 6865  e1video1.gif" he
+000003b0: 6967 6874 3d22 3132 3870 7822 3e0d 0a3c  ight="128px">..<
+000003c0: 2f70 3e0d 0a0d 0a44 6565 7050 6f73 654b  /p>....DeepPoseK
+000003d0: 6974 2069 7320 6120 736f 6674 7761 7265  it is a software
+000003e0: 2074 6f6f 6c6b 6974 2077 6974 6820 6120   toolkit with a 
+000003f0: 6869 6768 2d6c 6576 656c 2041 5049 2066  high-level API f
+00000400: 6f72 2032 4420 706f 7365 2065 7374 696d  or 2D pose estim
+00000410: 6174 696f 6e20 6f66 2075 7365 722d 6465  ation of user-de
+00000420: 6669 6e65 6420 6b65 7970 6f69 6e74 7320  fined keypoints 
+00000430: 7573 696e 6720 6465 6570 206c 6561 726e  using deep learn
+00000440: 696e 67e2 8094 7772 6974 7465 6e20 696e  ing...written in
+00000450: 2050 7974 686f 6e20 616e 6420 6275 696c   Python and buil
+00000460: 7420 7573 696e 6720 5b54 656e 736f 7266  t using [Tensorf
+00000470: 6c6f 775d 2868 7474 7073 3a2f 2f67 6974  low](https://git
+00000480: 6875 622e 636f 6d2f 7465 6e73 6f72 666c  hub.com/tensorfl
+00000490: 6f77 2f74 656e 736f 7266 6c6f 7729 2061  ow/tensorflow) a
+000004a0: 6e64 205b 4b65 7261 735d 2868 7474 7073  nd [Keras](https
+000004b0: 3a2f 2f77 7777 2e74 656e 736f 7266 6c6f  ://www.tensorflo
+000004c0: 772e 6f72 672f 6775 6964 652f 6b65 7261  w.org/guide/kera
+000004d0: 7329 2e20 5573 6520 4465 6570 506f 7365  s). Use DeepPose
+000004e0: 4b69 7420 6966 2079 6f75 206e 6565 643a  Kit if you need:
+000004f0: 0d0a 0d0a 2d20 746f 6f6c 7320 666f 7220  ....- tools for 
+00000500: 616e 6e6f 7461 7469 6e67 2069 6d61 6765  annotating image
+00000510: 7320 6f72 2076 6964 656f 2066 7261 6d65  s or video frame
+00000520: 7320 7769 7468 2075 7365 722d 6465 6669  s with user-defi
+00000530: 6e65 6420 6b65 7970 6f69 6e74 730d 0a2d  ned keypoints..-
+00000540: 2061 2073 7472 6169 6768 7466 6f72 7761   a straightforwa
+00000550: 7264 2062 7574 2066 6c65 7869 626c 6520  rd but flexible 
+00000560: 6461 7461 2061 7567 6d65 6e74 6174 696f  data augmentatio
+00000570: 6e20 7069 7065 6c69 6e65 2075 7369 6e67  n pipeline using
+00000580: 2074 6865 205b 696d 6761 7567 2070 6163   the [imgaug pac
+00000590: 6b61 6765 5d28 6874 7470 733a 2f2f 6769  kage](https://gi
+000005a0: 7468 7562 2e63 6f6d 2f61 6c65 6a75 2f69  thub.com/aleju/i
+000005b0: 6d67 6175 6729 0d0a 2d20 6120 4b65 7261  mgaug)..- a Kera
+000005c0: 732d 6261 7365 6420 696e 7465 7266 6163  s-based interfac
+000005d0: 6520 666f 7220 696e 6974 6961 6c69 7a69  e for initializi
+000005e0: 6e67 2c20 7472 6169 6e69 6e67 2c20 616e  ng, training, an
+000005f0: 6420 6576 616c 7561 7469 6e67 2070 6f73  d evaluating pos
+00000600: 6520 6573 7469 6d61 7469 6f6e 206d 6f64  e estimation mod
+00000610: 656c 730d 0a2d 2065 6173 792d 746f 2d75  els..- easy-to-u
+00000620: 7365 206d 6574 686f 6473 2066 6f72 2073  se methods for s
+00000630: 6176 696e 6720 616e 6420 6c6f 6164 696e  aving and loadin
+00000640: 6720 6d6f 6465 6c73 2061 6e64 206d 616b  g models and mak
+00000650: 696e 6720 7072 6564 6963 7469 6f6e 7320  ing predictions 
+00000660: 6f6e 206e 6577 2064 6174 610d 0a0d 0a44  on new data....D
+00000670: 6565 7050 6f73 654b 6974 2069 7320 6465  eepPoseKit is de
+00000680: 7369 676e 6564 2077 6974 6820 6120 666f  signed with a fo
+00000690: 6375 7320 6f6e 202a 7573 6162 696c 6974  cus on *usabilit
+000006a0: 792a 2061 6e64 202a 6578 7465 6e73 6962  y* and *extensib
+000006b0: 696c 6974 792a 2c20 6173 2062 6569 6e67  ility*, as being
+000006c0: 2061 626c 6520 746f 2067 6f20 6672 6f6d   able to go from
+000006d0: 2069 6465 6120 746f 2072 6573 756c 7420   idea to result 
+000006e0: 7769 7468 2074 6865 206c 6561 7374 2070  with the least p
+000006f0: 6f73 7369 626c 6520 6465 6c61 7920 6973  ossible delay is
+00000700: 206b 6579 2074 6f20 646f 696e 6720 676f   key to doing go
+00000710: 6f64 2072 6573 6561 7263 682e 0d0a 0d0a  od research.....
+00000720: 4465 6570 506f 7365 4b69 7420 6973 2063  DeepPoseKit is c
+00000730: 7572 7265 6e74 6c79 206c 696d 6974 6564  urrently limited
+00000740: 2074 6f20 2a69 6e64 6976 6964 7561 6c20   to *individual 
+00000750: 706f 7365 2065 7374 696d 6174 696f 6e2a  pose estimation*
+00000760: 2e20 4966 2069 6e64 6976 6964 7561 6c73  . If individuals
+00000770: 2063 616e 2062 6520 6561 7369 6c79 2064   can be easily d
+00000780: 6973 7469 6e67 7569 7368 6564 2076 6973  istinguished vis
+00000790: 7561 6c6c 7920 2869 2e65 2e2c 2074 6865  ually (i.e., the
+000007a0: 7920 6861 7665 2064 6966 6665 7265 6e74  y have different
+000007b0: 6c79 2063 6f6c 6f72 6564 2062 6f64 6965  ly colored bodie
+000007c0: 7320 6f72 2061 7265 206d 6172 6b65 6420  s or are marked 
+000007d0: 696e 2073 6f6d 6520 7761 7929 2c20 7468  in some way), th
+000007e0: 656e 206d 756c 7469 706c 6520 696e 6469  en multiple indi
+000007f0: 7669 6475 616c 7320 6361 6e20 7369 6d70  viduals can simp
+00000800: 6c79 2062 6520 6c61 6265 6c65 6420 7769  ly be labeled wi
+00000810: 7468 2073 6570 6172 6174 6520 6b65 7970  th separate keyp
+00000820: 6f69 6e74 7320 2868 6561 6431 2c20 7461  oints (head1, ta
+00000830: 696c 312c 2068 6561 6432 2c20 7461 696c  il1, head2, tail
+00000840: 322c 2065 7463 2e29 2e20 4f74 6865 7277  2, etc.). Otherw
+00000850: 6973 6520 4465 6570 506f 7365 4b69 7420  ise DeepPoseKit 
+00000860: 6361 6e20 6265 2065 7874 656e 6465 6420  can be extended 
+00000870: 746f 206d 756c 7469 706c 6520 696e 6469  to multiple indi
+00000880: 7669 6475 616c 7320 6279 2066 6972 7374  viduals by first
+00000890: 206c 6f63 616c 697a 696e 672c 2074 7261   localizing, tra
+000008a0: 636b 696e 672c 2061 6e64 2063 726f 7070  cking, and cropp
+000008b0: 696e 6720 696e 6469 7669 6475 616c 7320  ing individuals 
+000008c0: 7769 7468 2061 6464 6974 696f 6e61 6c20  with additional 
+000008d0: 736f 6674 7761 7265 2073 7563 6820 6173  software such as
+000008e0: 205b 6964 7472 6163 6b65 722e 6169 5d28   [idtracker.ai](
+000008f0: 6874 7470 733a 2f2f 6964 7472 6163 6b65  https://idtracke
+00000900: 722e 6169 2f29 2c20 5b70 696e 706f 696e  r.ai/), [pinpoin
+00000910: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00000920: 622e 636f 6d2f 6a67 7261 7669 6e67 2f70  b.com/jgraving/p
+00000930: 696e 706f 696e 7429 2c20 6f72 205b 5472  inpoint), or [Tr
+00000940: 6163 6b74 6f72 5d28 6874 7470 733a 2f2f  acktor](https://
+00000950: 6769 7468 7562 2e63 6f6d 2f76 6976 656b  github.com/vivek
+00000960: 6873 7269 6468 6172 2f74 7261 636b 746f  hsridhar/trackto
+00000970: 7229 2e0d 0a0d 0a4c 6f63 616c 697a 6174  r).....Localizat
+00000980: 696f 6e20 2877 6974 686f 7574 2074 7261  ion (without tra
+00000990: 636b 696e 6729 2063 616e 2061 6c73 6f20  cking) can also 
+000009a0: 6265 2061 6368 6965 7665 6420 7769 7468  be achieved with
+000009b0: 2064 6565 7020 6c65 6172 6e69 6e67 2073   deep learning s
+000009c0: 6f66 7477 6172 6520 6c69 6b65 205b 6b65  oftware like [ke
+000009d0: 7261 732d 7265 7469 6e61 6e65 745d 2868  ras-retinanet](h
+000009e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000009f0: 6d2f 6669 7a79 722f 6b65 7261 732d 7265  m/fizyr/keras-re
+00000a00: 7469 6e61 6e65 7429 2c20 7468 6520 5b54  tinanet), the [T
+00000a10: 656e 736f 7266 6c6f 7720 4f62 6a65 6374  ensorflow Object
+00000a20: 2044 6574 6563 7469 6f6e 2041 5049 5d28   Detection API](
+00000a30: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000a40: 6f6d 2f74 656e 736f 7266 6c6f 772f 6d6f  om/tensorflow/mo
+00000a50: 6465 6c73 2f74 7265 652f 6d61 7374 6572  dels/tree/master
+00000a60: 2f72 6573 6561 7263 682f 6f62 6a65 6374  /research/object
+00000a70: 5f64 6574 6563 7469 6f6e 292c 206f 7220  _detection), or 
+00000a80: 5b4d 6174 7465 7250 6f72 7427 7320 4d61  [MatterPort's Ma
+00000a90: 736b 2052 2d43 4e4e 5d28 6874 7470 733a  sk R-CNN](https:
+00000aa0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6174  //github.com/mat
+00000ab0: 7465 7270 6f72 742f 4d61 736b 5f52 434e  terport/Mask_RCN
+00000ac0: 4e29 2e0d 0a0d 0a5b 4368 6563 6b20 6f75  N).....[Check ou
+00000ad0: 7420 6f75 7220 7061 7065 725d 2868 7474  t our paper](htt
+00000ae0: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
+00000af0: 3735 3534 2f65 4c69 6665 2e34 3739 3934  7554/eLife.47994
+00000b00: 2920 746f 2066 696e 6420 6f75 7420 6d6f  ) to find out mo
+00000b10: 7265 2e0d 0a0d 0a3c 7020 616c 6967 6e3d  re.....<p align=
+00000b20: 2263 656e 7465 7222 3e0d 0a3c 696d 6720  "center">..<img 
+00000b30: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+00000b40: 6875 622e 636f 6d2f 6a67 7261 7669 6e67  hub.com/jgraving
+00000b50: 2f6a 6772 6176 696e 672e 6769 7468 7562  /jgraving.github
+00000b60: 2e69 6f2f 626c 6f62 2f6d 6173 7465 722f  .io/blob/master/
+00000b70: 6669 6c65 732f 696d 6167 6573 2f7a 6562  files/images/zeb
+00000b80: 7261 2e67 6966 2220 6865 6967 6874 3d22  ra.gif" height="
+00000b90: 3235 3670 7822 3e0d 0a3c 696d 6720 7372  256px">..<img sr
+00000ba0: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
+00000bb0: 622e 636f 6d2f 6a67 7261 7669 6e67 2f6a  b.com/jgraving/j
+00000bc0: 6772 6176 696e 672e 6769 7468 7562 2e69  graving.github.i
+00000bd0: 6f2f 626c 6f62 2f6d 6173 7465 722f 6669  o/blob/master/fi
+00000be0: 6c65 732f 696d 6167 6573 2f6c 6f63 7573  les/images/locus
+00000bf0: 742e 6769 6622 2068 6569 6768 743d 2232  t.gif" height="2
+00000c00: 3536 7078 223e 0d0a 3c2f 703e 0d0a 0d0a  56px">..</p>....
+00000c10: 2320 486f 7720 746f 2075 7365 2044 6565  # How to use Dee
+00000c20: 7050 6f73 654b 6974 0d0a 0d0a 4465 6570  pPoseKit....Deep
+00000c30: 506f 7365 4b69 7420 6973 2064 6573 6967  PoseKit is desig
+00000c40: 6e65 6420 666f 7220 6561 7379 2075 7365  ned for easy use
+00000c50: 2e20 466f 7220 6578 616d 706c 652c 2074  . For example, t
+00000c60: 7261 696e 696e 6720 616e 6420 7361 7669  raining and savi
+00000c70: 6e67 2061 206d 6f64 656c 2072 6571 7569  ng a model requi
+00000c80: 7265 7320 6f6e 6c79 2061 2066 6577 206c  res only a few l
+00000c90: 696e 6573 206f 6620 636f 6465 3a0d 0a60  ines of code:..`
+00000ca0: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2064  ``python..from d
+00000cb0: 6565 7070 6f73 656b 6974 2e69 6f20 696d  eepposekit.io im
+00000cc0: 706f 7274 2044 6174 6147 656e 6572 6174  port DataGenerat
+00000cd0: 6f72 2c20 5472 6169 6e69 6e67 4765 6e65  or, TrainingGene
+00000ce0: 7261 746f 720d 0a66 726f 6d20 6465 6570  rator..from deep
+00000cf0: 706f 7365 6b69 742e 6d6f 6465 6c73 2069  posekit.models i
+00000d00: 6d70 6f72 7420 5374 6163 6b65 6444 656e  mport StackedDen
+00000d10: 7365 4e65 740d 0a0d 0a64 6174 615f 6765  seNet....data_ge
+00000d20: 6e65 7261 746f 7220 3d20 4461 7461 4765  nerator = DataGe
+00000d30: 6e65 7261 746f 7228 272f 7061 7468 2f74  nerator('/path/t
+00000d40: 6f2f 616e 6e6f 7461 7469 6f6e 5f64 6174  o/annotation_dat
+00000d50: 612e 6835 2729 0d0a 7472 6169 6e5f 6765  a.h5')..train_ge
+00000d60: 6e65 7261 746f 7220 3d20 5472 6169 6e69  nerator = Traini
+00000d70: 6e67 4765 6e65 7261 746f 7228 6461 7461  ngGenerator(data
+00000d80: 5f67 656e 6572 6174 6f72 290d 0a6d 6f64  _generator)..mod
+00000d90: 656c 203d 2053 7461 636b 6564 4465 6e73  el = StackedDens
+00000da0: 654e 6574 2874 7261 696e 5f67 656e 6572  eNet(train_gener
+00000db0: 6174 6f72 290d 0a6d 6f64 656c 2e66 6974  ator)..model.fit
+00000dc0: 2862 6174 6368 5f73 697a 653d 3136 2c20  (batch_size=16, 
+00000dd0: 6e5f 776f 726b 6572 733d 3829 0d0a 6d6f  n_workers=8)..mo
+00000de0: 6465 6c2e 7361 7665 2827 2f70 6174 682f  del.save('/path/
+00000df0: 746f 2f73 6176 6564 5f6d 6f64 656c 2e68  to/saved_model.h
+00000e00: 3527 290d 0a60 6060 0d0a 4c6f 6164 696e  5')..```..Loadin
+00000e10: 6720 6120 7472 6169 6e65 6420 6d6f 6465  g a trained mode
+00000e20: 6c20 616e 6420 7275 6e6e 696e 6720 7072  l and running pr
+00000e30: 6564 6963 7469 6f6e 7320 6f6e 206e 6577  edictions on new
+00000e40: 2064 6174 6120 6973 2061 6c73 6f20 7374   data is also st
+00000e50: 7261 6967 6874 666f 7277 6172 642e 2046  raightforward. F
+00000e60: 6f72 2065 7861 6d70 6c65 2c20 7275 6e6e  or example, runn
+00000e70: 696e 6720 7072 6564 6963 7469 6f6e 7320  ing predictions 
+00000e80: 6f6e 2061 206e 6577 2076 6964 656f 3a0d  on a new video:.
+00000e90: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
+00000ea0: 2064 6565 7070 6f73 656b 6974 2e6d 6f64   deepposekit.mod
+00000eb0: 656c 7320 696d 706f 7274 206c 6f61 645f  els import load_
+00000ec0: 6d6f 6465 6c0d 0a66 726f 6d20 6465 6570  model..from deep
+00000ed0: 706f 7365 6b69 742e 696f 2069 6d70 6f72  posekit.io impor
+00000ee0: 7420 5669 6465 6f52 6561 6465 720d 0a0d  t VideoReader...
+00000ef0: 0a6d 6f64 656c 203d 206c 6f61 645f 6d6f  .model = load_mo
+00000f00: 6465 6c28 272f 7061 7468 2f74 6f2f 7361  del('/path/to/sa
+00000f10: 7665 645f 6d6f 6465 6c2e 6835 2729 0d0a  ved_model.h5')..
+00000f20: 7265 6164 6572 203d 2056 6964 656f 5265  reader = VideoRe
+00000f30: 6164 6572 2827 2f70 6174 682f 746f 2f76  ader('/path/to/v
+00000f40: 6964 656f 2e6d 7034 2729 0d0a 7072 6564  ideo.mp4')..pred
+00000f50: 6963 7469 6f6e 7320 3d20 6d6f 6465 6c2e  ictions = model.
+00000f60: 7072 6564 6963 7428 7265 6164 6572 290d  predict(reader).
+00000f70: 0a60 6060 0d0a 0d0a 2323 2055 7369 6e67  .```....## Using
+00000f80: 2044 6565 7050 6f73 654b 6974 2069 7320   DeepPoseKit is 
+00000f90: 6120 342d 7374 6570 2070 726f 6365 7373  a 4-step process
+00000fa0: 3a0d 0a0d 0a2d 202a 2a31 2e2a 2a20 5b43  :....- **1.** [C
+00000fb0: 7265 6174 6520 616e 2061 6e6e 6f74 6174  reate an annotat
+00000fc0: 696f 6e20 7365 745d 2868 7474 7073 3a2f  ion set](https:/
+00000fd0: 2f67 6974 6875 622e 636f 6d2f 6a67 7261  /github.com/jgra
+00000fe0: 7669 6e67 2f44 6565 7050 6f73 654b 6974  ving/DeepPoseKit
+00000ff0: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
+00001000: 6d70 6c65 732f 7374 6570 315f 6372 6561  mples/step1_crea
+00001010: 7465 5f61 6e6e 6f74 6174 696f 6e5f 7365  te_annotation_se
+00001020: 742e 6970 796e 6229 203c 6120 6872 6566  t.ipynb) <a href
+00001030: 3d22 6874 7470 733a 2f2f 636f 6c61 622e  ="https://colab.
+00001040: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00001050: 636f 6d2f 6769 7468 7562 2f6a 6772 6176  com/github/jgrav
+00001060: 696e 672f 6465 6570 706f 7365 6b69 742f  ing/deepposekit/
+00001070: 626c 6f62 2f6d 6173 7465 722f 6578 616d  blob/master/exam
+00001080: 706c 6573 2f73 7465 7031 5f63 7265 6174  ples/step1_creat
+00001090: 655f 616e 6e6f 7461 7469 6f6e 5f73 6574  e_annotation_set
+000010a0: 2e69 7079 6e62 2220 7461 7267 6574 3d22  .ipynb" target="
+000010b0: 5f70 6172 656e 7422 3e3c 696d 6720 7372  _parent"><img sr
+000010c0: 633d 2268 7474 7073 3a2f 2f63 6f6c 6162  c="https://colab
+000010d0: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+000010e0: 2e63 6f6d 2f61 7373 6574 732f 636f 6c61  .com/assets/cola
+000010f0: 622d 6261 6467 652e 7376 6722 2061 6c74  b-badge.svg" alt
+00001100: 3d22 4f70 656e 2049 6e20 436f 6c61 6222  ="Open In Colab"
+00001110: 2f3e 3c2f 613e 0d0a 2d20 2a2a 322e 2a2a  /></a>..- **2.**
+00001120: 205b 416e 6e6f 7461 7465 2079 6f75 7220   [Annotate your 
+00001130: 6461 7461 5d28 6874 7470 733a 2f2f 6769  data](https://gi
+00001140: 7468 7562 2e63 6f6d 2f6a 6772 6176 696e  thub.com/jgravin
+00001150: 672f 4465 6570 506f 7365 4b69 742f 626c  g/DeepPoseKit/bl
+00001160: 6f62 2f6d 6173 7465 722f 6578 616d 706c  ob/master/exampl
+00001170: 6573 2f73 7465 7032 5f61 6e6e 6f74 6174  es/step2_annotat
+00001180: 655f 6461 7461 2e69 7079 6e62 2920 7769  e_data.ipynb) wi
+00001190: 7468 206f 7572 2062 7569 6c74 2d69 6e20  th our built-in 
+000011a0: 4755 4920 286e 6f20 436f 6c61 6220 7375  GUI (no Colab su
+000011b0: 7070 6f72 7429 0d0a 2d20 2a2a 332e 2a2a  pport)..- **3.**
+000011c0: 205b 5365 6c65 6374 2061 6e64 2074 7261   [Select and tra
+000011d0: 696e 5d28 6874 7470 733a 2f2f 6769 7468  in](https://gith
+000011e0: 7562 2e63 6f6d 2f6a 6772 6176 696e 672f  ub.com/jgraving/
+000011f0: 4465 6570 506f 7365 4b69 742f 626c 6f62  DeepPoseKit/blob
+00001200: 2f6d 6173 7465 722f 6578 616d 706c 6573  /master/examples
+00001210: 2f73 7465 7033 5f74 7261 696e 5f6d 6f64  /step3_train_mod
+00001220: 656c 2e69 7079 6e62 2920 6f6e 6520 6f75  el.ipynb) one ou
+00001230: 7220 5b70 6f73 6520 6573 7469 6d61 7469  r [pose estimati
+00001240: 6f6e 206d 6f64 656c 735d 2868 7474 703a  on models](http:
+00001250: 2f2f 6a61 6b65 6772 6176 696e 672e 636f  //jakegraving.co
+00001260: 6d2f 4465 6570 506f 7365 4b69 742f 6874  m/DeepPoseKit/ht
+00001270: 6d6c 2f64 6565 7070 6f73 656b 6974 2f6d  ml/deepposekit/m
+00001280: 6f64 656c 732f 696e 6465 782e 6874 6d6c  odels/index.html
+00001290: 2920 696e 636c 7564 696e 6720 5b60 5374  ) including [`St
+000012a0: 6163 6b65 6444 656e 7365 4e65 7460 5d28  ackedDenseNet`](
+000012b0: 6874 7470 3a2f 2f6a 616b 6567 7261 7669  http://jakegravi
+000012c0: 6e67 2e63 6f6d 2f44 6565 7050 6f73 654b  ng.com/DeepPoseK
+000012d0: 6974 2f68 746d 6c2f 6465 6570 706f 7365  it/html/deeppose
+000012e0: 6b69 742f 6d6f 6465 6c73 2f53 7461 636b  kit/models/Stack
+000012f0: 6564 4465 6e73 654e 6574 2e68 746d 6c29  edDenseNet.html)
+00001300: 2c20 5b60 5374 6163 6b65 6448 6f75 7267  , [`StackedHourg
+00001310: 6c61 7373 605d 2868 7474 703a 2f2f 6a61  lass`](http://ja
+00001320: 6b65 6772 6176 696e 672e 636f 6d2f 4465  kegraving.com/De
+00001330: 6570 506f 7365 4b69 742f 6874 6d6c 2f64  epPoseKit/html/d
+00001340: 6565 7070 6f73 656b 6974 2f6d 6f64 656c  eepposekit/model
+00001350: 732f 5374 6163 6b65 6448 6f75 7267 6c61  s/StackedHourgla
+00001360: 7373 2e68 746d 6c29 2c20 5b60 4465 6570  ss.html), [`Deep
+00001370: 4c61 6243 7574 605d 2868 7474 703a 2f2f  LabCut`](http://
+00001380: 6a61 6b65 6772 6176 696e 672e 636f 6d2f  jakegraving.com/
+00001390: 4465 6570 506f 7365 4b69 742f 6874 6d6c  DeepPoseKit/html
+000013a0: 2f64 6565 7070 6f73 656b 6974 2f6d 6f64  /deepposekit/mod
+000013b0: 656c 732f 4465 6570 4c61 6243 7574 2e68  els/DeepLabCut.h
+000013c0: 746d 6c29 2c20 616e 6420 5b60 4c45 4150  tml), and [`LEAP
+000013d0: 605d 2868 7474 703a 2f2f 6a61 6b65 6772  `](http://jakegr
+000013e0: 6176 696e 672e 636f 6d2f 4465 6570 506f  aving.com/DeepPo
+000013f0: 7365 4b69 742f 6874 6d6c 2f64 6565 7070  seKit/html/deepp
+00001400: 6f73 656b 6974 2f6d 6f64 656c 732f 4c45  osekit/models/LE
+00001410: 4150 2e68 746d 6c29 2e20 3c61 2068 7265  AP.html). <a hre
+00001420: 663d 2268 7474 7073 3a2f 2f63 6f6c 6162  f="https://colab
+00001430: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+00001440: 2e63 6f6d 2f67 6974 6875 622f 6a67 7261  .com/github/jgra
+00001450: 7669 6e67 2f64 6565 7070 6f73 656b 6974  ving/deepposekit
+00001460: 2f62 6c6f 622f 6d61 7374 6572 2f65 7861  /blob/master/exa
+00001470: 6d70 6c65 732f 7374 6570 335f 7472 6169  mples/step3_trai
+00001480: 6e5f 6d6f 6465 6c2e 6970 796e 6222 2074  n_model.ipynb" t
+00001490: 6172 6765 743d 225f 7061 7265 6e74 223e  arget="_parent">
+000014a0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000014b0: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+000014c0: 2e67 6f6f 676c 652e 636f 6d2f 6173 7365  .google.com/asse
+000014d0: 7473 2f63 6f6c 6162 2d62 6164 6765 2e73  ts/colab-badge.s
+000014e0: 7667 2220 616c 743d 224f 7065 6e20 496e  vg" alt="Open In
+000014f0: 2043 6f6c 6162 222f 3e3c 2f61 3e0d 0a2d   Colab"/></a>..-
+00001500: 202a 2a34 2e2a 2a20 5573 6520 7468 6520   **4.** Use the 
+00001510: 7472 6169 6e65 6420 6d6f 6465 6c20 746f  trained model to
+00001520: 3a0d 0a09 2d20 6129 205b 496e 6974 6961  :...- a) [Initia
+00001530: 6c69 7a65 206b 6579 706f 696e 7473 2066  lize keypoints f
+00001540: 6f72 2075 6e61 6e6e 6f74 6174 6564 2064  or unannotated d
+00001550: 6174 615d 2868 7474 7073 3a2f 2f67 6974  ata](https://git
+00001560: 6875 622e 636f 6d2f 6a67 7261 7669 6e67  hub.com/jgraving
+00001570: 2f44 6565 7050 6f73 654b 6974 2f62 6c6f  /DeepPoseKit/blo
+00001580: 622f 6d61 7374 6572 2f65 7861 6d70 6c65  b/master/example
+00001590: 732f 7374 6570 3461 5f69 6e69 7469 616c  s/step4a_initial
+000015a0: 697a 655f 616e 6e6f 7461 7469 6f6e 732e  ize_annotations.
+000015b0: 6970 796e 6229 2066 6f72 2066 6173 7465  ipynb) for faste
+000015c0: 7220 616e 6e6f 7461 7469 6f6e 7320 7769  r annotations wi
+000015d0: 7468 202a 6163 7469 7665 206c 6561 726e  th *active learn
+000015e0: 696e 672a 2e20 3c61 2068 7265 663d 2268  ing*. <a href="h
+000015f0: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
+00001600: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
+00001610: 2f67 6974 6875 622f 6a67 7261 7669 6e67  /github/jgraving
+00001620: 2f64 6565 7070 6f73 656b 6974 2f62 6c6f  /deepposekit/blo
+00001630: 622f 6d61 7374 6572 2f65 7861 6d70 6c65  b/master/example
+00001640: 732f 7374 6570 3461 5f69 6e69 7469 616c  s/step4a_initial
+00001650: 697a 655f 616e 6e6f 7461 7469 6f6e 732e  ize_annotations.
+00001660: 6970 796e 6222 2074 6172 6765 743d 225f  ipynb" target="_
+00001670: 7061 7265 6e74 223e 3c69 6d67 2073 7263  parent"><img src
+00001680: 3d22 6874 7470 733a 2f2f 636f 6c61 622e  ="https://colab.
+00001690: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+000016a0: 636f 6d2f 6173 7365 7473 2f63 6f6c 6162  com/assets/colab
+000016b0: 2d62 6164 6765 2e73 7667 2220 616c 743d  -badge.svg" alt=
+000016c0: 224f 7065 6e20 496e 2043 6f6c 6162 222f  "Open In Colab"/
+000016d0: 3e3c 2f61 3e0d 0a09 2d20 6229 205b 5072  ></a>...- b) [Pr
+000016e0: 6564 6963 7420 6f6e 206e 6577 2064 6174  edict on new dat
+000016f0: 6120 616e 6420 7265 6669 6e65 2074 6865  a and refine the
+00001700: 2074 7261 696e 696e 6720 7365 745d 2868   training set](h
+00001710: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001720: 6d2f 6a67 7261 7669 6e67 2f44 6565 7050  m/jgraving/DeepP
+00001730: 6f73 654b 6974 2f62 6c6f 622f 6d61 7374  oseKit/blob/mast
+00001740: 6572 2f65 7861 6d70 6c65 732f 7374 6570  er/examples/step
+00001750: 3462 5f70 7265 6469 6374 5f6e 6577 5f64  4b_predict_new_d
+00001760: 6174 612e 6970 796e 6229 2074 6f20 696d  ata.ipynb) to im
+00001770: 7072 6f76 6520 7065 7266 6f72 6d61 6e63  prove performanc
+00001780: 652e 203c 6120 6872 6566 3d22 6874 7470  e. <a href="http
+00001790: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+000017a0: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
+000017b0: 7468 7562 2f6a 6772 6176 696e 672f 6465  thub/jgraving/de
+000017c0: 6570 706f 7365 6b69 742f 626c 6f62 2f6d  epposekit/blob/m
+000017d0: 6173 7465 722f 6578 616d 706c 6573 2f73  aster/examples/s
+000017e0: 7465 7034 625f 7072 6564 6963 745f 6e65  tep4b_predict_ne
+000017f0: 775f 6461 7461 2e69 7079 6e62 2220 7461  w_data.ipynb" ta
+00001800: 7267 6574 3d22 5f70 6172 656e 7422 3e3c  rget="_parent"><
+00001810: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001820: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
+00001830: 676f 6f67 6c65 2e63 6f6d 2f61 7373 6574  google.com/asset
+00001840: 732f 636f 6c61 622d 6261 6467 652e 7376  s/colab-badge.sv
+00001850: 6722 2061 6c74 3d22 4f70 656e 2049 6e20  g" alt="Open In 
+00001860: 436f 6c61 6222 2f3e 3c2f 613e 0d0a 0d0a  Colab"/></a>....
+00001870: 2323 2046 6f72 206d 6f72 6520 6465 7461  ## For more deta
+00001880: 696c 733a 0d0a 0d0a 2d20 5365 6520 5b6f  ils:....- See [o
+00001890: 7572 2065 7861 6d70 6c65 206e 6f74 6562  ur example noteb
+000018a0: 6f6f 6b73 5d28 6874 7470 733a 2f2f 6769  ooks](https://gi
+000018b0: 7468 7562 2e63 6f6d 2f6a 6772 6176 696e  thub.com/jgravin
+000018c0: 672f 6465 6570 706f 7365 6b69 742f 626c  g/deepposekit/bl
+000018d0: 6f62 2f6d 6173 7465 722f 6578 616d 706c  ob/master/exampl
+000018e0: 6573 2f29 0d0a 2d20 4368 6563 6b20 7468  es/)..- Check th
+000018f0: 6520 5b64 6f63 756d 656e 7461 7469 6f6e  e [documentation
+00001900: 5d28 6874 7470 3a2f 2f64 6f63 732e 6465  ](http://docs.de
+00001910: 6570 706f 7365 6b69 742e 6f72 6729 0d0a  epposekit.org)..
+00001920: 2d20 5265 6164 205b 6f75 7220 7061 7065  - Read [our pape
+00001930: 725d 2868 7474 7073 3a2f 2f64 6f69 2e6f  r](https://doi.o
+00001940: 7267 2f31 302e 3735 3534 2f65 4c69 6665  rg/10.7554/eLife
+00001950: 2e34 3739 3934 290d 0a0d 0a23 2320 2249  .47994)....## "I
+00001960: 2061 6c72 6561 6479 2068 6176 6520 616e   already have an
+00001970: 6e6f 7461 7465 6420 6461 7461 220d 0a0d  notated data"...
+00001980: 0a44 6565 7050 6f73 654b 6974 2069 7320  .DeepPoseKit is 
+00001990: 6465 7369 676e 6564 2074 6f20 6265 2065  designed to be e
+000019a0: 7874 656e 7369 626c 652c 2073 6f20 6c6f  xtensible, so lo
+000019b0: 6164 696e 6720 6461 7461 2069 6e20 6f74  ading data in ot
+000019c0: 6865 7220 666f 726d 6174 7320 6973 2070  her formats is p
+000019d0: 6f73 7369 626c 652e 0d0a 0d0a 4966 2079  ossible.....If y
+000019e0: 6f75 2068 6176 6520 616e 6e6f 7461 7465  ou have annotate
+000019f0: 6420 6461 7461 2066 726f 6d20 4465 6570  d data from Deep
+00001a00: 4c61 6243 7574 2028 6874 7470 3a2f 2f64  LabCut (http://d
+00001a10: 6565 706c 6162 6375 742e 6f72 6729 2c20  eeplabcut.org), 
+00001a20: 7472 7920 5b6f 7572 2028 6578 7065 7269  try [our (experi
+00001a30: 6d65 6e74 616c 2920 6578 616d 706c 6520  mental) example 
+00001a40: 6e6f 7465 626f 6f6b 205d 2868 7474 7073  notebook ](https
+00001a50: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a67  ://github.com/jg
+00001a60: 7261 7669 6e67 2f44 6565 7050 6f73 654b  raving/DeepPoseK
+00001a70: 6974 2f62 6c6f 622f 6d61 7374 6572 2f65  it/blob/master/e
+00001a80: 7861 6d70 6c65 732f 6465 6570 6c61 6263  xamples/deeplabc
+00001a90: 7574 5f64 6174 615f 6578 616d 706c 652e  ut_data_example.
+00001aa0: 6970 796e 6229 2066 6f72 206c 6f61 6469  ipynb) for loadi
+00001ab0: 6e67 2064 6174 6120 696e 2074 6869 7320  ng data in this 
+00001ac0: 666f 726d 6174 2e20 3c61 2068 7265 663d  format. <a href=
+00001ad0: 2268 7474 7073 3a2f 2f63 6f6c 6162 2e72  "https://colab.r
+00001ae0: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+00001af0: 6f6d 2f67 6974 6875 622f 6a67 7261 7669  om/github/jgravi
+00001b00: 6e67 2f64 6565 7070 6f73 656b 6974 2f62  ng/deepposekit/b
+00001b10: 6c6f 622f 6d61 7374 6572 2f65 7861 6d70  lob/master/examp
+00001b20: 6c65 732f 6465 6570 6c61 6263 7574 5f64  les/deeplabcut_d
+00001b30: 6174 615f 6578 616d 706c 652e 6970 796e  ata_example.ipyn
+00001b40: 6222 2074 6172 6765 743d 225f 7061 7265  b" target="_pare
+00001b50: 6e74 223e 3c69 6d67 2073 7263 3d22 6874  nt"><img src="ht
+00001b60: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
+00001b70: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
+00001b80: 6173 7365 7473 2f63 6f6c 6162 2d62 6164  assets/colab-bad
+00001b90: 6765 2e73 7667 2220 616c 743d 224f 7065  ge.svg" alt="Ope
+00001ba0: 6e20 496e 2043 6f6c 6162 222f 3e3c 2f61  n In Colab"/></a
+00001bb0: 3e0d 0a0d 0a48 6176 6520 6461 7461 2069  >....Have data i
+00001bc0: 6e20 616e 6f74 6865 7220 666f 726d 6174  n another format
+00001bd0: 3f20 596f 7520 6361 6e20 7772 6974 6520  ? You can write 
+00001be0: 796f 7572 206f 776e 2063 7573 746f 6d20  your own custom 
+00001bf0: 6765 6e65 7261 746f 7220 746f 206c 6f61  generator to loa
+00001c00: 6420 6974 2e0d 0a43 6865 636b 206f 7574  d it...Check out
+00001c10: 2074 6865 205b 6578 616d 706c 6520 666f   the [example fo
+00001c20: 7220 7772 6974 696e 6720 6375 7374 6f6d  r writing custom
+00001c30: 2064 6174 6120 6765 6e65 7261 746f 7273   data generators
+00001c40: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001c50: 2e63 6f6d 2f6a 6772 6176 696e 672f 4465  .com/jgraving/De
+00001c60: 6570 506f 7365 4b69 742f 626c 6f62 2f6d  epPoseKit/blob/m
+00001c70: 6173 7465 722f 6578 616d 706c 6573 2f63  aster/examples/c
+00001c80: 7573 746f 6d5f 6461 7461 5f67 656e 6572  ustom_data_gener
+00001c90: 6174 6f72 2e69 7079 6e62 292e 203c 6120  ator.ipynb). <a 
+00001ca0: 6872 6566 3d22 6874 7470 733a 2f2f 636f  href="https://co
+00001cb0: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
+00001cc0: 676c 652e 636f 6d2f 6769 7468 7562 2f6a  gle.com/github/j
+00001cd0: 6772 6176 696e 672f 6465 6570 706f 7365  graving/deeppose
+00001ce0: 6b69 742f 626c 6f62 2f6d 6173 7465 722f  kit/blob/master/
+00001cf0: 6578 616d 706c 6573 2f63 7573 746f 6d5f  examples/custom_
+00001d00: 6461 7461 5f67 656e 6572 6174 6f72 2e69  data_generator.i
+00001d10: 7079 6e62 2220 7461 7267 6574 3d22 5f70  pynb" target="_p
+00001d20: 6172 656e 7422 3e3c 696d 6720 7372 633d  arent"><img src=
+00001d30: 2268 7474 7073 3a2f 2f63 6f6c 6162 2e72  "https://colab.r
+00001d40: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+00001d50: 6f6d 2f61 7373 6574 732f 636f 6c61 622d  om/assets/colab-
+00001d60: 6261 6467 652e 7376 6722 2061 6c74 3d22  badge.svg" alt="
+00001d70: 4f70 656e 2049 6e20 436f 6c61 6222 2f3e  Open In Colab"/>
+00001d80: 3c2f 613e 0d0a 0d0a 2320 496e 7374 616c  </a>....# Instal
+00001d90: 6c61 7469 6f6e 0d0a 0d0a 4465 6570 506f  lation....DeepPo
+00001da0: 7365 4b69 7420 7265 7175 6972 6573 205b  seKit requires [
+00001db0: 5465 6e73 6f72 666c 6f77 5d28 6874 7470  Tensorflow](http
+00001dc0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
+00001dd0: 656e 736f 7266 6c6f 772f 7465 6e73 6f72  ensorflow/tensor
+00001de0: 666c 6f77 2920 666f 7220 7472 6169 6e69  flow) for traini
+00001df0: 6e67 2061 6e64 2075 7369 6e67 2070 6f73  ng and using pos
+00001e00: 6520 6573 7469 6d61 7469 6f6e 206d 6f64  e estimation mod
+00001e10: 656c 732e 205b 5465 6e73 6f72 666c 6f77  els. [Tensorflow
+00001e20: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001e30: 2e63 6f6d 2f74 656e 736f 7266 6c6f 772f  .com/tensorflow/
+00001e40: 7465 6e73 6f72 666c 6f77 2920 7368 6f75  tensorflow) shou
+00001e50: 6c64 2062 6520 6d61 6e75 616c 6c79 2069  ld be manually i
+00001e60: 6e73 7461 6c6c 6564 2c20 616c 6f6e 6720  nstalled, along 
+00001e70: 7769 7468 2064 6570 656e 6465 6e63 6965  with dependencie
+00001e80: 7320 7375 6368 2061 7320 4355 4441 2061  s such as CUDA a
+00001e90: 6e64 2063 7544 4e4e 2c20 6265 666f 7265  nd cuDNN, before
+00001ea0: 2069 6e73 7461 6c6c 696e 6720 4465 6570   installing Deep
+00001eb0: 506f 7365 4b69 743a 0d0a 0d0a 2d20 5b54  PoseKit:....- [T
+00001ec0: 656e 736f 7266 6c6f 7720 496e 7374 616c  ensorflow Instal
+00001ed0: 6c61 7469 6f6e 2049 6e73 7472 7563 7469  lation Instructi
+00001ee0: 6f6e 735d 2868 7474 7073 3a2f 2f77 7777  ons](https://www
+00001ef0: 2e74 656e 736f 7266 6c6f 772e 6f72 672f  .tensorflow.org/
+00001f00: 696e 7374 616c 6c29 0d0a 2d20 416e 7920  install)..- Any 
+00001f10: 5465 6e73 6f72 666c 6f77 2076 6572 7369  Tensorflow versi
+00001f20: 6f6e 203e 3d31 2e31 332e 3020 7368 6f75  on >=1.13.0 shou
+00001f30: 6c64 2062 6520 636f 6d70 6174 6962 6c65  ld be compatible
+00001f40: 2028 696e 636c 7564 696e 6720 322e 3029   (including 2.0)
+00001f50: 2e0d 0a0d 0a44 6565 7050 6f73 654b 6974  .....DeepPoseKit
+00001f60: 2068 6173 206f 6e6c 7920 6265 656e 2074   has only been t
+00001f70: 6573 7465 6420 6f6e 2055 6275 6e74 7520  ested on Ubuntu 
+00001f80: 3138 2e30 342c 2077 6869 6368 2069 7320  18.04, which is 
+00001f90: 7468 6520 7265 636f 6d6d 656e 6465 6420  the recommended 
+00001fa0: 7379 7374 656d 2066 6f72 2075 7369 6e67  system for using
+00001fb0: 2074 6865 2074 6f6f 6c6b 6974 2e20 0d0a   the toolkit. ..
+00001fc0: 0d0a 496e 7374 616c 6c20 7468 6520 6c61  ..Install the la
+00001fd0: 7465 7374 2073 7461 626c 6520 7265 6c65  test stable rele
+00001fe0: 6173 6520 7769 7468 2070 6970 3a0d 0a60  ase with pip:..`
+00001ff0: 6060 6261 7368 0d0a 7069 7020 696e 7374  ``bash..pip inst
+00002000: 616c 6c20 2d2d 7570 6461 7465 2064 6565  all --update dee
+00002010: 7070 6f73 656b 6974 0d0a 6060 600d 0a0d  pposekit..```...
+00002020: 0a49 6e73 7461 6c6c 2074 6865 206c 6174  .Install the lat
+00002030: 6573 7420 6465 7665 6c6f 706d 656e 7420  est development 
+00002040: 7665 7273 696f 6e20 7769 7468 2070 6970  version with pip
+00002050: 3a0d 0a60 6060 6261 7368 0d0a 7069 7020  :..```bash..pip 
+00002060: 696e 7374 616c 6c20 2d2d 7570 6461 7465  install --update
+00002070: 2067 6974 2b68 7474 7073 3a2f 2f77 7777   git+https://www
+00002080: 2e67 6974 6875 622e 636f 6d2f 6a67 7261  .github.com/jgra
+00002090: 7669 6e67 2f64 6565 7070 6f73 656b 6974  ving/deepposekit
+000020a0: 2e67 6974 0d0a 6060 600d 0a0d 0a59 6f75  .git..```....You
+000020b0: 2063 616e 2064 6f77 6e6c 6f61 6420 6578   can download ex
+000020c0: 616d 706c 6520 6461 7461 7365 7473 2066  ample datasets f
+000020d0: 726f 6d20 6f75 7220 5b44 6565 7050 6f73  rom our [DeepPos
+000020e0: 654b 6974 2044 6174 615d 2868 7474 7073  eKit Data](https
+000020f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a67  ://github.com/jg
+00002100: 7261 7669 6e67 2f64 6565 7070 6f73 656b  raving/deepposek
+00002110: 6974 2d64 6174 6129 2072 6570 6f73 6974  it-data) reposit
+00002120: 6f72 793a 0d0a 6060 6062 6173 680d 0a67  ory:..```bash..g
+00002130: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
+00002140: 2f77 7777 2e67 6974 6875 622e 636f 6d2f  /www.github.com/
+00002150: 6a67 7261 7669 6e67 2f64 6565 7070 6f73  jgraving/deeppos
+00002160: 656b 6974 2d64 6174 610d 0a60 6060 0d0a  ekit-data..```..
+00002170: 0d0a 2323 2049 6e73 7461 6c6c 696e 6720  ..## Installing 
+00002180: 7769 7468 2041 6e61 636f 6e64 6120 6f6e  with Anaconda on
+00002190: 2057 696e 646f 7773 0d0a 0d0a 546f 2069   Windows....To i
+000021a0: 6e73 7461 6c6c 2044 6565 7050 6f73 654b  nstall DeepPoseK
+000021b0: 6974 206f 6e20 5769 6e64 6f77 732c 2079  it on Windows, y
+000021c0: 6f75 206d 7573 7420 6669 7273 7420 6d61  ou must first ma
+000021d0: 6e75 616c 6c79 2069 6e73 7461 6c6c 2060  nually install `
+000021e0: 5368 6170 656c 7960 2c20 6f6e 6520 6f66  Shapely`, one of
+000021f0: 2074 6865 2064 6570 656e 6465 6e63 6965   the dependencie
+00002200: 7320 666f 7220 7468 6520 5b69 6d67 6175  s for the [imgau
+00002210: 6720 7061 636b 6167 655d 2868 7474 7073  g package](https
+00002220: 3a2f 2f67 6974 6875 622e 636f 6d2f 616c  ://github.com/al
+00002230: 656a 752f 696d 6761 7567 293a 0d0a 6060  eju/imgaug):..``
+00002240: 6062 6173 680d 0a63 6f6e 6461 2069 6e73  `bash..conda ins
+00002250: 7461 6c6c 202d 6320 636f 6e64 612d 666f  tall -c conda-fo
+00002260: 7267 6520 7368 6170 656c 790d 0a60 6060  rge shapely..```
+00002270: 0d0a 5765 2061 6c73 6f20 7265 636f 6d6d  ..We also recomm
+00002280: 656e 6420 696e 7374 616c 6c69 6e67 2044  end installing D
+00002290: 6565 7050 6f73 654b 6974 2066 726f 6d20  eepPoseKit from 
+000022a0: 7769 7468 696e 2050 7974 686f 6e20 7261  within Python ra
+000022b0: 7468 6572 2074 6861 6e20 7573 696e 6720  ther than using 
+000022c0: 7468 6520 636f 6d6d 616e 6420 6c69 6e65  the command line
+000022d0: 2c20 6569 7468 6572 2066 726f 6d20 7769  , either from wi
+000022e0: 7468 696e 204a 7570 7974 6572 206f 7220  thin Jupyter or 
+000022f0: 616e 6f74 6865 7220 4944 452c 2074 6f20  another IDE, to 
+00002300: 656e 7375 7265 2069 7420 6973 2069 6e73  ensure it is ins
+00002310: 7461 6c6c 6564 2069 6e20 7468 6520 636f  talled in the co
+00002320: 7272 6563 7420 776f 726b 696e 6720 656e  rrect working en
+00002330: 7669 726f 6e6d 656e 743a 0d0a 6060 6070  vironment:..```p
+00002340: 7974 686f 6e0d 0a69 6d70 6f72 7420 7379  ython..import sy
+00002350: 730d 0a21 7b73 7973 2e65 7865 6375 7461  s..!{sys.executa
+00002360: 626c 657d 202d 6d20 7069 7020 696e 7374  ble} -m pip inst
+00002370: 616c 6c20 2d2d 7570 6461 7465 2064 6565  all --update dee
+00002380: 7070 6f73 656b 6974 0d0a 6060 600d 0a23  pposekit..```..#
+00002390: 2043 6f6e 7472 6962 7574 6f72 7320 616e   Contributors an
+000023a0: 6420 4465 7665 6c6f 706d 656e 7420 200d  d Development  .
+000023b0: 0a20 2020 0d0a 4465 6570 506f 7365 4b69  .   ..DeepPoseKi
+000023c0: 7420 7761 7320 6465 7665 6c6f 7065 6420  t was developed 
+000023d0: 6279 205b 4a61 6b65 2047 7261 7669 6e67  by [Jake Graving
+000023e0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000023f0: 2e63 6f6d 2f6a 6772 6176 696e 6729 2061  .com/jgraving) a
+00002400: 6e64 205b 4461 6e69 656c 2043 6861 655d  nd [Daniel Chae]
+00002410: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00002420: 636f 6d2f 6463 6861 6562 6165 292c 2061  com/dchaebae), a
+00002430: 6e64 2069 7320 7374 696c 6c20 6265 696e  nd is still bein
+00002440: 6720 6163 7469 7665 6c79 2064 6576 656c  g actively devel
+00002450: 6f70 6564 2e20 2e0d 0a0d 0a57 6520 7765  oped. .....We we
+00002460: 6c63 6f6d 6520 636f 6d6d 756e 6974 7920  lcome community 
+00002470: 696e 766f 6c76 656d 656e 7420 616e 6420  involvement and 
+00002480: 7075 626c 6963 2063 6f6e 7472 6962 7574  public contribut
+00002490: 696f 6e73 2074 6f20 7468 6520 746f 6f6c  ions to the tool
+000024a0: 6b69 742e 2049 6620 796f 7520 7769 7368  kit. If you wish
+000024b0: 2074 6f20 636f 6e74 7269 6275 7465 2c20   to contribute, 
+000024c0: 706c 6561 7365 205b 666f 726b 2074 6865  please [fork the
+000024d0: 2072 6570 6f73 6974 6f72 795d 2868 7474   repository](htt
+000024e0: 7073 3a2f 2f68 656c 702e 6769 7468 7562  ps://help.github
+000024f0: 2e63 6f6d 2f65 6e2f 6172 7469 636c 6573  .com/en/articles
+00002500: 2f66 6f72 6b2d 612d 7265 706f 2920 746f  /fork-a-repo) to
+00002510: 206d 616b 6520 796f 7572 206d 6f64 6966   make your modif
+00002520: 6963 6174 696f 6e73 2061 6e64 205b 7375  ications and [su
+00002530: 626d 6974 2061 2070 756c 6c20 7265 7175  bmit a pull requ
+00002540: 6573 745d 2868 7474 7073 3a2f 2f68 656c  est](https://hel
+00002550: 702e 6769 7468 7562 2e63 6f6d 2f65 6e2f  p.github.com/en/
+00002560: 6172 7469 636c 6573 2f63 7265 6174 696e  articles/creatin
+00002570: 672d 612d 7075 6c6c 2d72 6571 7565 7374  g-a-pull-request
+00002580: 2d66 726f 6d2d 612d 666f 726b 292e 0d0a  -from-a-fork)...
+00002590: 0d0a 4966 2079 6f75 2764 206c 696b 6520  ..If you'd like 
+000025a0: 746f 2067 6574 2069 6e76 6f6c 7665 6420  to get involved 
+000025b0: 7769 7468 2064 6576 656c 6f70 696e 6720  with developing 
+000025c0: 4465 6570 506f 7365 4b69 742c 2067 6574  DeepPoseKit, get
+000025d0: 2069 6e20 746f 7563 6820 286a 6772 6176   in touch (jgrav
+000025e0: 696e 6740 676d 6169 6c2e 636f 6d29 2061  ing@gmail.com) a
+000025f0: 6e64 2063 6865 636b 206f 7574 205b 6f75  nd check out [ou
+00002600: 7220 6465 7665 6c6f 706d 656e 7420 726f  r development ro
+00002610: 6164 6d61 705d 2868 7474 7073 3a2f 2f67  admap](https://g
+00002620: 6974 6875 622e 636f 6d2f 6a67 7261 7669  ithub.com/jgravi
+00002630: 6e67 2f44 6565 7050 6f73 654b 6974 2f62  ng/DeepPoseKit/b
+00002640: 6c6f 622f 6d61 7374 6572 2f44 4556 454c  lob/master/DEVEL
+00002650: 4f50 4d45 4e54 2e6d 6429 2074 6f20 7365  OPMENT.md) to se
+00002660: 6520 6675 7475 7265 2070 6c61 6e73 2066  e future plans f
+00002670: 6f72 2074 6865 2070 6163 6b61 6765 2e20  or the package. 
+00002680: 200d 0a0d 0a23 2049 7373 7565 7320 200d   ....# Issues  .
+00002690: 0a20 0d0a 506c 6561 7365 2073 7562 6d69  . ..Please submi
+000026a0: 7420 6275 6773 206f 7220 6665 6174 7572  t bugs or featur
+000026b0: 6520 7265 7175 6573 7473 2074 6f20 7468  e requests to th
+000026c0: 6520 5b47 6974 4875 6220 6973 7375 6520  e [GitHub issue 
+000026d0: 7472 6163 6b65 725d 2868 7474 7073 3a2f  tracker](https:/
+000026e0: 2f67 6974 6875 622e 636f 6d2f 6a67 7261  /github.com/jgra
+000026f0: 7669 6e67 2f64 6565 7070 6f73 656b 6974  ving/deepposekit
+00002700: 2f69 7373 7565 732f 6e65 7729 2e20 506c  /issues/new). Pl
+00002710: 6561 7365 206c 696d 6974 2072 6570 6f72  ease limit repor
+00002720: 7465 6420 6973 7375 6573 2074 6f20 7468  ted issues to th
+00002730: 6520 4465 6570 506f 7365 4b69 7420 636f  e DeepPoseKit co
+00002740: 6465 6261 7365 2061 6e64 2070 726f 7669  debase and provi
+00002750: 6465 2061 7320 6d75 6368 2064 6574 6169  de as much detai
+00002760: 6c20 6173 2079 6f75 2063 616e 2077 6974  l as you can wit
+00002770: 6820 6120 6d69 6e69 6d61 6c20 776f 726b  h a minimal work
+00002780: 696e 6720 6578 616d 706c 6520 6966 2070  ing example if p
+00002790: 6f73 7369 626c 652e 0d0a 0d0a 4966 2079  ossible.....If y
+000027a0: 6f75 2065 7870 6572 6965 6e63 6520 7072  ou experience pr
+000027b0: 6f62 6c65 6d73 2077 6974 6820 5b54 656e  oblems with [Ten
+000027c0: 736f 7266 6c6f 775d 2868 7474 7073 3a2f  sorflow](https:/
+000027d0: 2f67 6974 6875 622e 636f 6d2f 7465 6e73  /github.com/tens
+000027e0: 6f72 666c 6f77 2f74 656e 736f 7266 6c6f  orflow/tensorflo
+000027f0: 7729 2c20 7375 6368 2061 7320 696e 7374  w), such as inst
+00002800: 616c 6c69 6e67 2043 5544 4120 6f72 2063  alling CUDA or c
+00002810: 7544 4e4e 2064 6570 656e 6465 6e63 6965  uDNN dependencie
+00002820: 732c 2074 6865 6e20 706c 6561 7365 2064  s, then please d
+00002830: 6972 6563 7420 6973 7375 6573 2074 6f20  irect issues to 
+00002840: 7468 6f73 6520 6465 7665 6c6f 706d 656e  those developmen
+00002850: 7420 7465 616d 732e 0d0a 0d0a 2320 4c69  t teams.....# Li
+00002860: 6365 6e73 650d 0a0d 0a52 656c 6561 7365  cense....Release
+00002870: 6420 756e 6465 7220 6120 4170 6163 6865  d under a Apache
+00002880: 2032 2e30 204c 6963 656e 7365 2e20 5365   2.0 License. Se
+00002890: 6520 5b4c 4943 454e 5345 5d28 6874 7470  e [LICENSE](http
+000028a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+000028b0: 6772 6176 696e 672f 6465 6570 706f 7365  graving/deeppose
+000028c0: 6b69 742f 626c 6f62 2f6d 6173 7465 722f  kit/blob/master/
+000028d0: 4c49 4345 4e53 4529 2066 6f72 2064 6574  LICENSE) for det
+000028e0: 6169 6c73 2e0d 0a0d 0a23 2052 6566 6572  ails.....# Refer
+000028f0: 656e 6365 730d 0a0d 0a49 6620 796f 7520  ences....If you 
+00002900: 7573 6520 4465 6570 506f 7365 4b69 7420  use DeepPoseKit 
+00002910: 666f 7220 796f 7572 2072 6573 6561 7263  for your researc
+00002920: 6820 706c 6561 7365 2063 6974 6520 5b6f  h please cite [o
+00002930: 7572 206f 7065 6e2d 6163 6365 7373 2070  ur open-access p
+00002940: 6170 6572 5d28 6874 7470 3a2f 2f70 6170  aper](http://pap
+00002950: 6572 2e64 6565 7070 6f73 656b 6974 2e6f  er.deepposekit.o
+00002960: 7267 293a 0d0a 0d0a 2020 2020 4061 7274  rg):....    @art
+00002970: 6963 6c65 7b67 7261 7669 6e67 3230 3139  icle{graving2019
+00002980: 6465 6570 706f 7365 6b69 742c 0d0a 2020  deepposekit,..  
+00002990: 2020 2020 2020 2020 2020 2074 6974 6c65             title
+000029a0: 3d7b 4465 6570 506f 7365 4b69 742c 2061  ={DeepPoseKit, a
+000029b0: 2073 6f66 7477 6172 6520 746f 6f6c 6b69   software toolki
+000029c0: 7420 666f 7220 6661 7374 2061 6e64 2072  t for fast and r
+000029d0: 6f62 7573 7420 616e 696d 616c 2070 6f73  obust animal pos
+000029e0: 6520 6573 7469 6d61 7469 6f6e 2075 7369  e estimation usi
+000029f0: 6e67 2064 6565 7020 6c65 6172 6e69 6e67  ng deep learning
+00002a00: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
+00002a10: 2061 7574 686f 723d 7b47 7261 7669 6e67   author={Graving
+00002a20: 2c20 4a61 636f 6220 4d20 616e 6420 4368  , Jacob M and Ch
+00002a30: 6165 2c20 4461 6e69 656c 2061 6e64 204e  ae, Daniel and N
+00002a40: 6169 6b2c 2048 656d 616c 2061 6e64 204c  aik, Hemal and L
+00002a50: 692c 204c 6961 6e67 2061 6e64 204b 6f67  i, Liang and Kog
+00002a60: 6572 2c20 4265 6e6a 616d 696e 2061 6e64  er, Benjamin and
+00002a70: 2043 6f73 7465 6c6c 6f65 2c20 426c 6169   Costelloe, Blai
+00002a80: 7220 5220 616e 6420 436f 757a 696e 2c20  r R and Couzin, 
+00002a90: 4961 696e 2044 7d2c 0d0a 2020 2020 2020  Iain D},..      
+00002aa0: 2020 2020 2020 206a 6f75 726e 616c 3d7b         journal={
+00002ab0: 654c 6966 657d 2c0d 0a20 2020 2020 2020  eLife},..       
+00002ac0: 2020 2020 2020 766f 6c75 6d65 3d7b 387d        volume={8}
+00002ad0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002ae0: 7061 6765 733d 7b65 3437 3939 347d 2c0d  pages={e47994},.
+00002af0: 0a20 2020 2020 2020 2020 2020 2020 7965  .             ye
+00002b00: 6172 3d7b 3230 3139 7d2c 0d0a 2020 2020  ar={2019},..    
+00002b10: 2020 2020 2020 2020 2070 7562 6c69 7368           publish
+00002b20: 6572 3d7b 654c 6966 6520 5363 6965 6e63  er={eLife Scienc
+00002b30: 6573 2050 7562 6c69 6361 7469 6f6e 7320  es Publications 
+00002b40: 4c69 6d69 7465 647d 0d0a 2020 2020 2020  Limited}..      
+00002b50: 2020 2020 2020 2075 726c 3d7b 6874 7470         url={http
+00002b60: 733a 2f2f 646f 692e 6f72 672f 3130 2e37  s://doi.org/10.7
+00002b70: 3535 342f 654c 6966 652e 3437 3939 347d  554/eLife.47994}
+00002b80: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002b90: 7d0d 0a0d 0a59 6f75 2063 616e 2061 6c73  }....You can als
+00002ba0: 6f20 7265 6164 205b 6f75 7220 6f70 656e  o read [our open
+00002bb0: 2d61 6363 6573 7320 7072 6570 7269 6e74  -access preprint
+00002bc0: 5d28 6874 7470 3a2f 2f70 7265 7072 696e  ](http://preprin
+00002bd0: 742e 6465 6570 706f 7365 6b69 742e 6f72  t.deepposekit.or
+00002be0: 6729 2e0d 0a0d 0a49 6620 796f 7520 7573  g).....If you us
+00002bf0: 6520 7468 6520 5b69 6d67 6175 6720 7061  e the [imgaug pa
+00002c00: 636b 6167 655d 2868 7474 7073 3a2f 2f67  ckage](https://g
+00002c10: 6974 6875 622e 636f 6d2f 616c 656a 752f  ithub.com/aleju/
+00002c20: 696d 6761 7567 2920 666f 7220 6461 7461  imgaug) for data
+00002c30: 2061 7567 6d65 6e74 6174 696f 6e2c 2070   augmentation, p
+00002c40: 6c65 6173 6520 616c 736f 2063 6f6e 7369  lease also consi
+00002c50: 6465 7220 5b63 6974 696e 6720 6974 5d28  der [citing it](
+00002c60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002c70: 6f6d 2f61 6c65 6a75 2f69 6d67 6175 672f  om/aleju/imgaug/
+00002c80: 626c 6f62 2f6d 6173 7465 722f 5245 4144  blob/master/READ
+00002c90: 4d45 2e6d 6423 6369 7461 7469 6f6e 292e  ME.md#citation).
+00002ca0: 0d0a 0d0a 4966 2079 6f75 205b 7573 6520  ....If you [use 
+00002cb0: 6461 7461 5d28 6874 7470 733a 2f2f 6769  data](https://gi
+00002cc0: 7468 7562 2e63 6f6d 2f6a 6772 6176 696e  thub.com/jgravin
+00002cd0: 672f 4465 6570 506f 7365 4b69 7423 692d  g/DeepPoseKit#i-
+00002ce0: 616c 7265 6164 792d 6861 7665 2d61 6e6e  already-have-ann
+00002cf0: 6f74 6174 6564 2d64 6174 6129 2074 6861  otated-data) tha
+00002d00: 7420 7761 7320 616e 6e6f 7461 7465 6420  t was annotated 
+00002d10: 7769 7468 2074 6865 2044 6565 704c 6162  with the DeepLab
+00002d20: 4375 7420 7061 636b 6167 6520 2868 7474  Cut package (htt
+00002d30: 703a 2f2f 6465 6570 6c61 6263 7574 2e6f  p://deeplabcut.o
+00002d40: 7267 2920 666f 7220 796f 7572 2072 6573  rg) for your res
+00002d50: 6561 7263 682c 2062 6520 7375 7265 2074  earch, be sure t
+00002d60: 6f20 5b63 6974 6520 6974 5d28 6874 7470  o [cite it](http
+00002d70: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00002d80: 6c65 7845 4d47 2f44 6565 704c 6162 4375  lexEMG/DeepLabCu
+00002d90: 742f 626c 6f62 2f6d 6173 7465 722f 5245  t/blob/master/RE
+00002da0: 4144 4d45 2e6d 6423 7265 6665 7265 6e63  ADME.md#referenc
+00002db0: 6573 292e 0d0a 0d0a 506c 6561 7365 2061  es).....Please a
+00002dc0: 6c73 6f20 636f 6e73 6964 6572 2063 6974  lso consider cit
+00002dd0: 696e 6720 7468 6520 7265 6c65 7661 6e74  ing the relevant
+00002de0: 2072 6566 6572 656e 6365 7320 666f 7220   references for 
+00002df0: 7468 6520 706f 7365 2065 7374 696d 6174  the pose estimat
+00002e00: 696f 6e20 6d6f 6465 6c28 7329 2075 7365  ion model(s) use
+00002e10: 6420 696e 2079 6f75 7220 7265 7365 6172  d in your resear
+00002e20: 6368 2c20 7768 6963 6820 6361 6e20 6265  ch, which can be
+00002e30: 2066 6f75 6e64 2069 6e20 7468 6520 646f   found in the do
+00002e40: 6375 6d65 6e74 6174 696f 6e20 2869 2e65  cumentation (i.e
+00002e50: 2e2c 205b 6053 7461 636b 6564 4465 6e73  ., [`StackedDens
+00002e60: 654e 6574 605d 2868 7474 703a 2f2f 6a61  eNet`](http://ja
+00002e70: 6b65 6772 6176 696e 672e 636f 6d2f 4465  kegraving.com/De
+00002e80: 6570 506f 7365 4b69 742f 6874 6d6c 2f64  epPoseKit/html/d
+00002e90: 6565 7070 6f73 656b 6974 2f6d 6f64 656c  eepposekit/model
+00002ea0: 732f 5374 6163 6b65 6444 656e 7365 4e65  s/StackedDenseNe
+00002eb0: 742e 6874 6d6c 2372 6566 6572 656e 6365  t.html#reference
+00002ec0: 7329 2c20 5b60 5374 6163 6b65 6448 6f75  s), [`StackedHou
+00002ed0: 7267 6c61 7373 605d 2868 7474 703a 2f2f  rglass`](http://
+00002ee0: 6a61 6b65 6772 6176 696e 672e 636f 6d2f  jakegraving.com/
+00002ef0: 4465 6570 506f 7365 4b69 742f 6874 6d6c  DeepPoseKit/html
+00002f00: 2f64 6565 7070 6f73 656b 6974 2f6d 6f64  /deepposekit/mod
+00002f10: 656c 732f 5374 6163 6b65 6448 6f75 7267  els/StackedHourg
+00002f20: 6c61 7373 2e68 746d 6c23 7265 6665 7265  lass.html#refere
+00002f30: 6e63 6573 292c 205b 6044 6565 704c 6162  nces), [`DeepLab
+00002f40: 4375 7460 5d28 6874 7470 3a2f 2f6a 616b  Cut`](http://jak
+00002f50: 6567 7261 7669 6e67 2e63 6f6d 2f44 6565  egraving.com/Dee
+00002f60: 7050 6f73 654b 6974 2f68 746d 6c2f 6465  pPoseKit/html/de
+00002f70: 6570 706f 7365 6b69 742f 6d6f 6465 6c73  epposekit/models
+00002f80: 2f44 6565 704c 6162 4375 742e 6874 6d6c  /DeepLabCut.html
+00002f90: 2372 6566 6572 656e 6365 7329 2c20 5b60  #references), [`
+00002fa0: 4c45 4150 605d 2868 7474 703a 2f2f 6a61  LEAP`](http://ja
+00002fb0: 6b65 6772 6176 696e 672e 636f 6d2f 4465  kegraving.com/De
+00002fc0: 6570 506f 7365 4b69 742f 6874 6d6c 2f64  epPoseKit/html/d
+00002fd0: 6565 7070 6f73 656b 6974 2f6d 6f64 656c  eepposekit/model
+00002fe0: 732f 4c45 4150 2e68 746d 6c23 7265 6665  s/LEAP.html#refe
+00002ff0: 7265 6e63 6573 2929 2e0d 0a0d 0a23 204e  rences)).....# N
+00003000: 6577 730d 0a2d 202a 2a4f 6374 6f62 6572  ews..- **October
+00003010: 2032 3031 393a 2a2a 204f 7572 2070 6170   2019:** Our pap
+00003020: 6572 2064 6573 6372 6962 696e 6720 4465  er describing De
+00003030: 6570 506f 7365 4b69 7420 6973 2070 7562  epPoseKit is pub
+00003040: 6c69 7368 6564 2061 7420 654c 6966 6521  lished at eLife!
+00003050: 2028 6874 7470 3a2f 2f70 6170 6572 2e64   (http://paper.d
+00003060: 6565 7070 6f73 656b 6974 2e6f 7267 290d  eepposekit.org).
+00003070: 0a2d 202a 2a53 6570 7465 6d62 6572 2032  .- **September 2
+00003080: 3031 392a 2a3a 200d 0a20 2020 202d 204e  019**: ..    - N
+00003090: 6174 7572 6520 4e65 7773 2063 6f76 6572  ature News cover
+000030a0: 7320 4465 6570 506f 7365 4b69 743a 205b  s DeepPoseKit: [
+000030b0: 4465 6570 206c 6561 726e 696e 6720 706f  Deep learning po
+000030c0: 7765 7273 2061 206d 6f74 696f 6e2d 7472  wers a motion-tr
+000030d0: 6163 6b69 6e67 2072 6576 6f6c 7574 696f  acking revolutio
+000030e0: 6e5d 2868 7474 703a 2f2f 646f 692e 6f72  n](http://doi.or
+000030f0: 672f 3130 2e31 3033 382f 6434 3135 3836  g/10.1038/d41586
+00003100: 2d30 3139 2d30 3239 3432 2d35 290d 0a20  -019-02942-5).. 
+00003110: 2020 202d 2076 302e 332e 3020 6973 2072     - v0.3.0 is r
+00003120: 656c 6561 7365 642e 2053 6565 205b 7468  eleased. See [th
+00003130: 6520 7265 6c65 6173 6520 6e6f 7465 735d  e release notes]
+00003140: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00003150: 636f 6d2f 6a67 7261 7669 6e67 2f44 6565  com/jgraving/Dee
+00003160: 7050 6f73 654b 6974 2f72 656c 6561 7365  pPoseKit/release
+00003170: 732f 7461 672f 7630 2e33 2e30 292e 0d0a  s/tag/v0.3.0)...
+00003180: 2d20 2a2a 4170 7269 6c20 3230 3139 3a2a  - **April 2019:*
+00003190: 2a20 5468 6520 4465 6570 506f 7365 4b69  * The DeepPoseKi
+000031a0: 7420 7072 6570 7269 6e74 2069 7320 6f6e  t preprint is on
+000031b0: 2062 696f 7278 6976 2028 6874 7470 3a2f   biorxiv (http:/
+000031c0: 2f70 7265 7072 696e 742e 6465 6570 706f  /preprint.deeppo
+000031d0: 7365 6b69 742e 6f72 6729 0d0a            sekit.org)..
```

### Comparing `us2deepposekit-0.3.9/deepposekit/__init__.py` & `us2deepposekit-0.4.0/deepposekit/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,16 +16,12 @@
 from __future__ import absolute_import
 import sys
 import warnings
 
 from deepposekit.io import TrainingGenerator, DataGenerator
 from deepposekit.augment.FlipAxis import FlipAxis
 
-from deepposekit.annotate.gui.Annotator import Annotator
-from deepposekit.annotate.gui.Skeleton import Skeleton
 from deepposekit.annotate.KMeansSampler import KMeansSampler
 
-from deepposekit.io.video import VideoReader, VideoWriter
-
 
 __doc__ = """ """  # open('README.md').read()
-__version__ = "0.3.9"
+__version__ = "0.4.0"
```

### Comparing `us2deepposekit-0.3.9/deepposekit/annotate/KMeansSampler.py` & `us2deepposekit-0.4.0/deepposekit/annotate/KMeansSampler.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/annotate/__init__.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,13 +9,12 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
 from __future__ import absolute_import
 
-from deepposekit.annotate.gui.Annotator import Annotator
-from deepposekit.annotate.gui.Skeleton import Skeleton
-from deepposekit.annotate.KMeansSampler import KMeansSampler
+from deepposekit.models.layers.convolutional import *
+from deepposekit.models.layers.subpixel import *
+from deepposekit.models.layers.util import *
```

### Comparing `us2deepposekit-0.3.9/deepposekit/annotate/gui/Annotator.py` & `us2deepposekit-0.4.0/deepposekit/io/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,322 +12,299 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
 import h5py
 import os
+import pandas as pd
 
-from deepposekit.annotate.gui.GUI import GUI
-from deepposekit.annotate.utils import hotkeys as keys
+from deepposekit.io.DataGenerator import DataGenerator
 
-__all__ = ["Annotator"]
+__all__ = ["initialize_dataset", "initialize_skeleton", "merge_new_images"]
 
 
-class Annotator(GUI):
+def initialize_skeleton(skeleton):
+    """ Initialize the skeleton from input data.
 
-    """
-    A GUI for annotating images.
-
-    ------------------------------------------------------------
-         Keys             |   Action
-    ------------------------------------------------------------
-    >    +,-              |   Rescale the image
-    >    Left mouse       |   Move active keypoint
-    >    W, A, S, D       |   Move active keypoint
-    >    space            |   Changes W,A,S,D mode (swaps between 1px or 10px)
-    >    J, L             |   Load previous or next image
-    >    <, >             |   Jump 10 images backward or forward
-    >    I, K or          |
-         tab, shift+tab   |   Switch active keypoint
-    >    R                |   Mark frame as unannotated, or "reset"
-    >    F                |   Mark frame as annotated or "finished"
-    >    Esc, Q           |   Quit the Annotator GUI
-    ------------------------------------------------------------
-
-    Note: Data is automatically saved when moving between frames.
+    Takes in either a .csv or .xlsx file and makes a DataFrame.
 
     Parameters
     ----------
-    datapath: str
-        Filepath of the HDF5 (.h5) file that contains the images to
-        be annotated.
+    skeleton: pandas.DataFrame
+        Filepath of the .csv or .xlsx file that has indexed information
+        on name of the keypoint (part, e.g. head), parent (the direct
+        connecting part, e.g. neck connects to head, parent is head),
+        and swap (swapping positions with a part when reflected over X).
+    """
 
-    dataset: str
-        Key name to access the images in the .h5 file.
+    if isinstance(skeleton, str):
+        if skeleton.endswith(".csv"):
+            skeleton = pd.read_csv(skeleton)
+        elif skeleton.endswith(".xlsx"):
+            skeleton = pd.read_excel(skeleton)
+        else:
+            raise ValueError("skeleton must be .csv or .xlsx file")
+    elif isinstance(skeleton, pd.DataFrame):
+        skeleton = skeleton
+    else:
+        raise TypeError("skeleton must be type `str` or pandas.DataFrame")
+
+    if "name" not in skeleton.columns:
+        raise KeyError("skeleton file must contain a `name` column")
+    elif "parent" not in skeleton.columns:
+        raise KeyError("skeleton file must contain a `parent` column")
+
+    if "x" not in skeleton.columns:
+        skeleton["x"] = -1
+    if "y" not in skeleton.columns:
+        skeleton["y"] = -1
+
+    if "tree" not in skeleton.columns:
+        skeleton["tree"] = -1
+        for idx, name in enumerate(skeleton["parent"].values):
+            branch = np.where(skeleton["name"] == name)[0]
+            if branch.shape[0] > 0:
+                branch = branch[0]
+                skeleton.loc[idx, "tree"] = branch
+    if "swap_index" not in skeleton.columns:
+        skeleton["swap_index"] = -1
+        for idx, name in enumerate(skeleton["name"].values):
+            for jdx, swap_name in enumerate(skeleton["swap"].values):
+                if swap_name == name:
+                    skeleton.loc[idx, "swap_index"] = jdx
+    return skeleton
+
+
+def initialize_dataset(
+    datapath, images, skeleton, keypoints=None, dataset="images", overwrite=False
+):
+    """
+    Intialize an image dataset for annotation as an h5 file
 
-    skeleton: str
+    Parameters
+    ----------
+    datapath : str
+        The path to the annotations file. Must be .h5
+        e.g. '/path/to/file.h5'
+    images : ndarray, shape (n_images, height, width, channels)
+        A numpy array containing image data. 
+        `images.dtype` should be np.uint8
+    skeleton: str or pandas.DataFrame
         Filepath of the .csv or .xlsx file that has indexed information
         on name of the keypoint (part, e.g. head), parent (the direct
         connecting part, e.g. neck connects to head, parent is head),
         and swap (swapping positions with a part when reflected).
+        See example files for more information.
+    keypoints : None or ndarray, shape (n_images, n_keypoints, 2)
+        Optionally pass keypoints for initializing annotations for the
+        new images.
+    dataset : str, default = "images"
+        The name of the dataset within the h5 file to save the images.
+    overwrite: bool, default = False
+        Whether to overwrite an existing .h5 file with the same name.
+    """
+    if os.path.exists(datapath) and overwrite is False:
+        raise OSError(
+            "Annotation set {} already exists. Delete the file or set `overwrite=True`.".format(
+                datapath
+            )
+        )
+    if not isinstance(images, np.ndarray):
+        raise TypeError(
+            "images must be ndarray with shape (n_images, height, width, channels)"
+        )
+    elif images.ndim != 4:
+        raise TypeError(
+            "images must be ndarray with shape (n_images, height, width, channels)"
+        )
+    elif images.dtype != np.uint8:
+        raise TypeError("`images` must be ndarray with dtype np.uint8")
+
+    if keypoints is not None:
+        if not isinstance(keypoints, np.ndarray):
+            raise TypeError(
+                "keypoints must be None or ndarray with shape (n_images, n_keypoints, 2)"
+            )
+        elif keypoints.ndim != 3:
+            raise TypeError(
+                "images must be ndarray with shape (n_images, n_keypoints, 2)"
+            )
+        elif keypoints.shape[0] != images.shape[0]:
+            raise IndexError(
+                "shape for `images` and `keypoints` must match along axis 0."
+            )
+
+    n_images = images.shape[0]
+    height = images.shape[1]
+    width = images.shape[2]
+    n_channels = images.shape[3]
+    skeleton = initialize_skeleton(skeleton)
+    skeleton_names = skeleton["name"].values
+    skeleton = skeleton[["tree", "swap_index"]].values
+    n_keypoints = skeleton.shape[0]
+
+    with h5py.File(datapath, mode="w") as h5file:
+        h5file.create_dataset(
+            dataset,
+            shape=images.shape,
+            dtype=np.uint8,
+            data=images,
+            maxshape=(None,) + images.shape[1:],
+        )
+        data = keypoints if keypoints is not None else -np.ones((n_images, n_keypoints, 2))
+        h5file.create_dataset(
+            "annotations",
+            (n_images, n_keypoints, 2),
+            dtype=np.float64,
+            data=data,
+            maxshape=(None,) + data.shape[1:],
+        )
+        data = np.zeros((n_images, n_keypoints), dtype=bool)
+        h5file.create_dataset(
+            "annotated",
+            (n_images, n_keypoints),
+            dtype=bool,
+            data=data,
+            maxshape=(None,) + data.shape[1:],
+        )
+
+        h5file.create_dataset("skeleton", skeleton.shape, dtype=np.int32, data=skeleton)
+        h5file.create_dataset(
+            "skeleton_names",
+            (skeleton.shape[0],),
+            dtype="S10",
+            data=skeleton_names.astype("S10"),
+        )
+
+
+def merge_new_images(
+    datapath,
+    merged_datapath,
+    images,
+    keypoints=None,
+    dataset="images",
+    overwrite=False,
+    mode="full",
+):
+    """
+    Merge new images with an annotation set
 
-        See example file for more information.
-
-    scale: int/float, default 1
-        Scaling factor for the GUI (e.g. used in zooming).
-
-    text_scale: float
-        Scaling factor for the GUI font.
-        A text_scale of 1 works well for 1920x1080 (1080p) images
-    
-    shuffle_colors: bool, default = True
-        Whether to shuffle the color order for drawing keypoints
-
-    refresh: int, default 100
-        Delay on receiving next keyboard input in milliseconds.
-
-    Attributes
+    Parameters
     ----------
-    window_name: str
-        Name of the Annotation window when running program.
-        Set to be 'Annotation' unless otherwise changed.
-
-    n_images: int
-        Number of images in the .h5 file.
-
-    n_keypoints: int
-        Number of keypoints in the skeleton.
-
-    key: int
-        The key that is pressed on the keyboard.
-
-    image_idx: int
-        Index of a specific image in the .h5 file.
-
-    image: numpy.ndarray
-        One image accessed using image_idx.
-
-    Example
-    -------
-    >>> from deepposekit import Annotator
-    >>> app = Annotator('annotation.h5', 'images', 'skeleton.csv')
-    >>> app.run()
+    datapath : str
+        The path to the annotations file. Must be .h5
+        e.g. '/path/to/file.h5'
+    merged_datapath : str
+        The path to save the merged annotations file. Must be .h5
+        e.g. '/path/to/merged_file.h5'
+    images : ndarray, shape (n_images, height, width, channels)
+        A numpy array containing image data. 
+        `images.dtype` should be np.uint8
+    keypoints : None or ndarray, shape (n_images, n_keypoints, 2)
+        Optionally pass keypoints for initializing annotations for the
+        new images.
+    dataset : str, default = "images"
+        The dataset within the h5 file to save the images.
+    overwrite: bool, default = False
+        Whether to overwrite an existing .h5 file with the same name.
+    mode : str
+        The mode for loading the existing data. 
+        Must be "annotated", or "full" (the full dataset)
 
     """
 
-    def __init__(
-        self,
-        datapath,
-        dataset,
-        skeleton,
-        scale=1,
-        text_scale=0.15,
-        shuffle_colors=True,
-        refresh=100,
-    ):
-        super(GUI, self).__init__()
-
-        self.window_name = "Annotation"
-        self.shuffle_colors = shuffle_colors
-        self._init_skeleton(skeleton)
-        if os.path.exists(datapath):
-            self._init_data(datapath, dataset)
-        else:
-            raise ValueError("datapath file or path does not exist")
-        self._init_gui(scale, text_scale, shuffle_colors, refresh)
-
-    def _init_data(self, datapath, dataset):
-        """ Initializes the images from the .h5 file (called in init).
-
-        Parameters
-        ----------
-        datapath: str
-            Path of the .h5 file that contains the images to be annotated.
-
-        dataset: str
-            Key name to access the images in the .h5 file.
-
-        """
-        if isinstance(datapath, str):
-            if datapath.endswith(".h5"):
-                self.datapath = datapath
-            else:
-                raise ValueError("datapath must be .h5 file")
-        else:
-            raise TypeError("datapath must be type `str`")
-
-        if isinstance(dataset, str):
-            self.dataset = dataset
-        else:
-            raise TypeError("dataset must be type `str`")
-
-        with h5py.File(self.datapath, "r+") as h5file:
-
-            self.n_images = h5file[self.dataset].shape[0]
-            # Check that all parts of the file exist
-            if "annotations" not in list(h5file.keys()):
-                empty_array = np.zeros((self.n_images, self.n_keypoints, 2))
-                h5file.create_dataset(
-                    "annotations",
-                    (self.n_images, self.n_keypoints, 2),
-                    dtype=np.float64,
-                    data=empty_array,
+    if os.path.exists(merged_datapath) and overwrite is False:
+        raise OSError(
+            "Annotation set {} already exists. Delete the file or set `overwrite=True`.".format(
+                merged_datapath
+            )
+        )
+    if not isinstance(images, np.ndarray):
+        raise TypeError(
+            "images must be ndarray with shape (n_images, height, width, channels)"
+        )
+    elif images.ndim != 4:
+        raise TypeError(
+            "images must be ndarray with shape (n_images, height, width, channels)"
+        )
+    elif images.dtype != np.uint8:
+        raise TypeError("`images` must be ndarray with dtype np.uint8")
+
+    if keypoints is not None:
+        if not isinstance(keypoints, np.ndarray):
+            raise TypeError(
+                "keypoints must be None or ndarray with shape (n_images, n_keypoints, 2)"
+            )
+        elif keypoints.ndim != 3:
+            raise TypeError(
+                "images must be ndarray with shape (n_images, n_keypoints, 2)"
+            )
+        elif keypoints.shape[0] != images.shape[0]:
+            raise IndexError(
+                "shape for `images` and `keypoints` must match along axis 0."
+            )
+
+    data_generator = DataGenerator(datapath, dataset=dataset, mode="full")
+
+    if images.shape[1:] != data_generator.image_shape:
+        raise IndexError(
+            "`images` shape {} does not match existing dataset {}".format(
+                images.shape[1:], data_generator.image_shape
+            )
+        )
+    if keypoints is not None:
+        if keypoints.shape[-1] == 3:
+            keypoints = keypoints[:, :, :2]
+        if keypoints.shape[1:] != data_generator.keypoints_shape:
+            raise IndexError(
+                "`keypoints` shape {} does not match existing dataset {}".format(
+                    keypoints.shape[1:], data_generator.keypoints_shape
                 )
-                for idx in range(self.n_images):
-                    h5file["annotations"][idx] = self.skeleton.loc[:, ["x", "y"]].values
+            )
 
-            if "annotated" not in list(h5file.keys()):
-                empty_array = np.zeros((self.n_images, self.n_keypoints), dtype=bool)
-                h5file.create_dataset(
-                    "annotated",
-                    (self.n_images, self.n_keypoints),
-                    dtype=bool,
-                    data=empty_array,
-                )
+    h5file = h5py.File(datapath, mode="r")
 
-            if "skeleton" not in list(h5file.keys()):
-                skeleton = self.skeleton[["tree", "swap_index"]].values
-                h5file.create_dataset(
-                    "skeleton", skeleton.shape, dtype=np.int32, data=skeleton
-                )
+    n_samples_merged = h5file[dataset].shape[0] + images.shape[0]
 
-            # Unpack the images from the file
-            self.image_idx = np.sum(np.all(h5file["annotated"].value, axis=1)) - 1
+    merged_h5file = h5py.File(merged_datapath, "w")
+    merged_h5file.create_dataset(
+        dataset,
+        shape=(n_samples_merged,) + data_generator.image_shape,
+        dtype=np.uint8,
+        maxshape=(None,) + data_generator.image_shape,
+    )
+    merged_h5file.create_dataset(
+        "annotations",
+        shape=(n_samples_merged,) + data_generator.keypoints_shape,
+        dtype=np.float64,
+        maxshape=(None,) + data_generator.keypoints_shape,
+    )
+    merged_h5file.create_dataset(
+        "annotated",
+        (n_samples_merged, data_generator.keypoints_shape[0]),
+        dtype=bool,
+        maxshape=(None, data_generator.keypoints_shape[0]),
+    )
+    merged_h5file.create_dataset(
+        "skeleton", h5file["skeleton"].shape, dtype=np.int32, data=h5file["skeleton"][:]
+    )
+
+    for idx in range(h5file[dataset].shape[0]):
+        merged_h5file[dataset][idx] = h5file[dataset][idx]
+        merged_h5file["annotations"][idx] = h5file["annotations"][idx]
+        merged_h5file["annotated"][idx] = h5file["annotated"][idx]
+
+    for idx in range(h5file[dataset].shape[0], n_samples_merged):
+        merged_h5file[dataset][idx] = images[idx - h5file[dataset].shape[0]]
+        if keypoints is not None:
+            merged_h5file["annotations"][idx] = keypoints[
+                idx - h5file[dataset].shape[0]
+            ]
+        else:
+            merged_h5file["annotations"][idx] = np.zeros(data_generator.keypoints_shape)
+        merged_h5file["annotated"][idx] = np.zeros(
+            data_generator.keypoints_shape[0], dtype=bool
+        )
 
-            self.image = h5file[self.dataset][self.image_idx]
-            self._check_grayscale()
-            self.skeleton.loc[:, ["x", "y"]] = h5file["annotations"][self.image_idx]
-            self.skeleton.loc[:, "annotated"] = h5file["annotated"][self.image_idx]
-
-    def _save(self):
-        """ Saves an image.
-
-        Automatically called when moving to new images or invoked manually
-        using 'ctrl + s' keys.
-
-        """
-        with h5py.File(self.datapath) as h5file:
-
-            h5file["annotations"][self.image_idx] = self.skeleton.loc[
-                :, ["x", "y"]
-            ].values
-            h5file["annotated"][self.image_idx] = self.skeleton.loc[
-                :, "annotated"
-            ].values
-            self.skeleton.loc[:, ["x", "y"]] = h5file["annotations"][self.image_idx]
-            self.skeleton.loc[:, "annotated"] = h5file["annotated"][self.image_idx]
-
-    def _load(self):
-        """ Loads an image.
-
-        This method is called in _move_image_idx when moving to different
-        images. The image of specified image_idx will be loaded onto the GUI.
-
-        """
-
-        with h5py.File(self.datapath) as h5file:
-
-            self.image = h5file[self.dataset][self.image_idx]
-            self._check_grayscale()
-            self.skeleton.loc[:, ["x", "y"]] = h5file["annotations"][self.image_idx]
-            self.skeleton.loc[:, "annotated"] = h5file["annotated"][self.image_idx]
-
-    def _last_image(self):
-        """ Checks if image index is on the last index.
-    
-        Helper method to check for the index of the last image in the h5 file.
-
-        Returns
-        -------
-        bool
-            Indicate if image_idx is the last index.
-
-        """
-
-        return self.image_idx == self.n_images - 1
-
-    def _move_image_idx(self):
-        """ Move to different image.
-        
-        Based on the key pressed, updates the image on the GUI.
-        The scheme is as follows:
-        ------------------------------------------------------------
-             Keys             |   Action                           
-        ------------------------------------------------------------
-        >    <- , ->          |   Load previous or next image
-        >    ,  ,  .          |   Jump 10 images backward or forward
-        ------------------------------------------------------------
-
-        Every time the user moves from the image, the annotations
-        on the image is saved before loading the next image.
-
-        """
-
-        # <- (left arrow) key
-        if self.key is keys.LEFTARROW:
-            self._save()
-            if self.image_idx == 0:
-                self.image_idx = self.n_images - 1
-            else:
-                self.image_idx -= 1
-            self._load()
-        # -> (right arrow) key
-        elif self.key is keys.RIGHTARROW:
-            self._save()
-            if self._last_image():
-                self.image_idx = 0
-            else:
-                self.image_idx += 1
-            self._load()
-
-        # . (period) key
-        elif self.key is keys.LESSTHAN:
-            self._save()
-            if self.image_idx - 10 < 0:
-                self.image_idx = self.n_images + self.image_idx - 10
-            else:
-                self.image_idx -= 10
-            self._load()
-        # , (comma) key
-        elif self.key is keys.GREATERTHAN:
-            self._save()
-            if self.image_idx + 10 > self.n_images - 1:
-                self.image_idx = self.image_idx + 10 - self.n_images
-            else:
-                self.image_idx += 10
-            self._load()
-
-    def _data(self):
-        """ Activates key bindings for annotated and save.
-        
-        Creates additional key bindings for the program.
-        The bindings are as follows:
-        
-        ------------------------------------------------------------
-             Keys             |   Action                           
-        ------------------------------------------------------------
-        >    Ctrl-R           |   Mark frame as unannotated
-        >    Ctrl-F           |   Mark frame as annotated
-        >    Ctrl-S           |   Save
-        ------------------------------------------------------------
-
-        """
-
-        if self.key is keys.R:
-            self.skeleton["annotated"] = False
-        elif self.key is keys.F:
-            self.skeleton["annotated"] = True
-        elif self.key is keys.V:
-            if self.skeleton.loc[self.idx, ["x", "y"]].isnull()[0]:
-                self.skeleton.loc[self.idx, ["x", "y"]] = -1
-            else:
-                self.skeleton.loc[self.idx, ["x", "y"]] = np.nan
-        elif self.key in [keys.Q, keys.ESC]:
-            self._save()
-            print("Saved")
-
-    def _hotkeys(self):
-        """ Activates all key bindings.
-        
-        Enables all the key functionalities described at the
-        start of the file.
-
-        """
-
-        if self.key != keys.NONE:
-            self._wasd()
-            self._move_idx()
-            self._move_image_idx()
-            self._zoom()
-            self._data()
-            self._update_canvas()
+    h5file.close()
+    merged_h5file.close()
```

### Comparing `us2deepposekit-0.3.9/deepposekit/annotate/gui/Skeleton.py` & `us2deepposekit-0.4.0/deepposekit/augment/FlipAxis.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,128 +10,109 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
-import cv2
+from deepposekit.io.BaseGenerator import BaseGenerator
+from imgaug.augmenters import meta
+from imgaug import parameters as iap
 
-from deepposekit.annotate.gui.GUI import GUI
-from deepposekit.annotate.utils import hotkeys as keys
+__all__ = ["FlipAxis"]
 
-__all__ = ["Skeleton"]
 
+class FlipAxis(meta.Augmenter):
+    """ Flips the input image and keypoints across an axis.
 
-class Skeleton(GUI):
-    """
-    A GUI for initializing a skeleton for a new dataset.
-
-    ------------------------------------------------------------
-         Keys             |   Action
-    ------------------------------------------------------------
-    >    +,-              |   Rescale the image
-    >    Left mouse       |   Move active keypoint
-    >    W, A, S, D       |   Move active keypoint
-    >    space            |   Changes W,A,S,D mode (swaps between 1px or 10px)
-    >    J, L             |   Load previous or next image
-    >    <, >             |   Jump 10 images backward or forward
-    >    I, K or          |
-         tab, shift+tab   |   Switch active keypoint
-    >    R                |   Mark frame as unannotated, or "reset"
-    >    F                |   Mark frame as annotated or "finished"
-    >    Esc, Q           |   Quit the GUI
-    ------------------------------------------------------------
+    A generalized class for flipping images and keypoints
+    either horizontally and vertically during augmentation.
+    This class requires a swap_index parameter, which indicates the
+    relationships between keypoint labels when flipping the image
+    (e.g. left leg is swapped with right leg, etc.)
 
     Parameters
     ----------
-    image: str
-        Filepath of the image to be labeled.
-
-    skeleton: str
-        Filepath of the .csv or .xlsx file that has indexed information
-        on name of the keypoint (part, e.g. head), parent (the direct
-        connecting part, e.g. neck connects to head, parent is head),
-        and swap (swapping positions with a part when reflected over X)
-
-        Consult example of such a file for more information
-
-    scale: int/float, default 1
-        Scaling factor for the GUI (e.g. used in zooming).
-
-    text_scale: float
-        Scaling factor for the GUI font.
-        A text_scale of 1 works well for 1920x1080 (1080p) images
+    swap_index: deepposekit.io.BaseGenerator or array
+        The keypoint indices to swap when the image is flipped.
+        This can be a deepposekit.io.BaseGenerator for annotations
+        or an array of integers specifying which keypoint indices
+        to swap.
+        
+    p: int, default 0.5
+        The probability that an image is flipped
 
-    shuffle_colors: bool, default = True
-        Whether to shuffle the color order for drawing keypoints
+    axis: int, default 0
+        Axis over which images are flipped
+        axis=0 flips up-down (np.flipud)
+        axis=1 flips left-right (np.fliplr)
+        
+    seed: None or int or np.random.RandomState, default None
+        The random state for the augmenter.
+        
+    name: None or str, default None
+        Name given to the Augmenter object. The name is used in print().
+        If left as None, will print 'UnnamedX'
+        
+    deterministic: bool, default False
+        If set to true, each batch will be augmented the same way.
 
-    refresh: int, default 100
-        Delay on receiving next keyboard input in milliseconds.
 
     Attributes
     ----------
-    window_name: str
-        Name of the Annotation window when running program.
-        Set to be 'Annotation' unless otherwise changed.
-
-    n_images: int
-        Number of images in question (1 in this case).
-
-    key: int
-        The key that is pressed on the keyboard.
-
-    image_idx: int
-        Index of a specific image in the .h5 file.
-
-    save: method
-        Output method is set to be to_csv
-
-    Examples
-    --------
-    >>> from deepposekit import Skeleton
-    >>> app = Skeleton('input_image.png', 'skeleton.csv')
-    >>> app.run()
-    >>>
-    >>> app.save('skeleton_initialized.csv') # save the labels in skeleton.csv file
+    p: int
+        The probability that an image is flipped
+    
+    axis: int
+        The axis to reflect the image.
 
-    Note: must use app.save('file.csv') to save! Unlike the
-    Annotator, will not automatically save until that line runs.
+    swap_index: array
+        The keypoint indices to swap when the image is flipped
+        
 
     """
 
-    def __init__(
-        self,
-        image,
-        skeleton,
-        scale=1,
-        text_scale=0.15,
-        shuffle_colors=True,
-        refresh=100,
-    ):
-
-        if isinstance(image, str):
-            self.image = cv2.imread(image)
-        elif isinstance(image, np.ndarray):
-            self.image = image
-
-        super(GUI, self).__init__()
-        self.image_idx = 0
-        self.n_images = 1
-        self.window_name = "Skeleton Creator"
-        self.shuffle_colors = shuffle_colors
-        self._init_skeleton(skeleton)
-        self._init_gui(scale, text_scale, shuffle_colors, refresh)
-        self.save = self.skeleton.to_csv
-
-    def _hotkeys(self):
-        """ Activates all key bindings.
-        
-        Enables all the key functionalities described at the
-        start of the file.
-
-        """
-        if self.key != keys.NONE:
-            self._wasd()
-            self._move_idx()
-            self._zoom()
-            self._update_canvas()
+    def __init__(self, swap_index, p=0.5, axis=0, seed=None, name=None, deterministic=False):
+        super(FlipAxis, self).__init__(seed=seed, name=name, random_state="deprecated", deterministic=deterministic)
+        self.p = iap.handle_probability_param(p, "p")
+        self.axis = axis
+        if isinstance(swap_index, BaseGenerator):
+            if hasattr(swap_index, "swap_index"):
+                self.swap_index = swap_index.swap_index
+        elif isinstance(swap_index, np.ndarray):
+            self.swap_index = swap_index
+        
+    
+    def _augment_batch_(self, batch, random_state, parents, hooks):
+        samples = self.p.draw_samples((batch.nb_rows,),
+                                      random_state=random_state)
+        for i, sample in enumerate(samples):
+            if sample >= 0.5:
+                
+                if batch.images is not None:
+                    if self.axis == 0:
+                        batch.images[i] = np.flipud(batch.images[i])
+                    if self.axis == 1:
+                        batch.images[i] = np.fliplr(batch.images[i])
+
+
+                if batch.keypoints is not None:
+                    kpsoi = batch.keypoints[i]
+                    if self.axis == 0:
+                        height = kpsoi.shape[0]
+                        for kp in kpsoi.keypoints:
+                            kp.y = (height-1) - kp.y
+                    if self.axis == 1:
+                        width = kpsoi.shape[1]
+                        for kp in kpsoi.keypoints:
+                            kp.x = (width-1) - kp.x
+                    swapped = kpsoi.keypoints.copy()
+                    for r in range(len(kpsoi.keypoints)):
+                        idx = self.swap_index[r]
+                        if idx >= 0:
+                            kpsoi.keypoints[r] = swapped[idx]
+
+        return batch
+
+    def get_parameters(self):
+        """See :func:`~imgaug.augmenters.meta.Augmenter.get_parameters`."""
+        return [self.p, self.axis, self.swap_index]
```

### Comparing `us2deepposekit-0.3.9/deepposekit/annotate/gui/__init__.py` & `us2deepposekit-0.4.0/deepposekit/augment/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,9 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import absolute_import
 
-from deepposekit.annotate.gui.Annotator import Annotator
-from deepposekit.annotate.gui.Skeleton import Skeleton
+from deepposekit.augment.FlipAxis import FlipAxis
```

### Comparing `us2deepposekit-0.3.9/deepposekit/annotate/utils/__init__.py` & `us2deepposekit-0.4.0/deepposekit/annotate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/annotate/utils/hotkeys.py` & `us2deepposekit-0.4.0/deepposekit/annotate/utils/hotkeys.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/annotate/utils/image.py` & `us2deepposekit-0.4.0/deepposekit/annotate/utils/image.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/augment/__init__.py` & `us2deepposekit-0.4.0/deepposekit/utils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,8 +11,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import absolute_import
 
-from deepposekit.augment.FlipAxis import FlipAxis
+from deepposekit.utils import keypoints
+from deepposekit.utils import image
+from deepposekit.utils import io
```

### Comparing `us2deepposekit-0.3.9/deepposekit/callbacks.py` & `us2deepposekit-0.4.0/deepposekit/callbacks.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/io/BaseGenerator.py` & `us2deepposekit-0.4.0/deepposekit/io/BaseGenerator.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/io/DLCDataGenerator.py` & `us2deepposekit-0.4.0/deepposekit/io/DLCDataGenerator.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/io/DataGenerator.py` & `us2deepposekit-0.4.0/deepposekit/io/DataGenerator.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/io/ImageGenerator.py` & `us2deepposekit-0.4.0/deepposekit/io/ImageGenerator.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/io/TrainingGenerator.py` & `us2deepposekit-0.4.0/deepposekit/io/TrainingGenerator.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/io/__init__.py` & `us2deepposekit-0.4.0/deepposekit/io/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,9 +18,8 @@
 from deepposekit.io.BaseGenerator import BaseGenerator
 from deepposekit.io.DataGenerator import DataGenerator
 from deepposekit.io.ImageGenerator import ImageGenerator
 from deepposekit.io.DLCDataGenerator import DLCDataGenerator
 
 from deepposekit.io.TrainingGenerator import TrainingGenerator
 
-from deepposekit.io.video import *
 from deepposekit.io.utils import *
```

### Comparing `us2deepposekit-0.3.9/deepposekit/models/DeepLabCut.py` & `us2deepposekit-0.4.0/deepposekit/models/DeepLabCut.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/LEAP.py` & `us2deepposekit-0.4.0/deepposekit/models/LEAP.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/StackedDenseNet.py` & `us2deepposekit-0.4.0/deepposekit/models/StackedDenseNet.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/StackedHourglass.py` & `us2deepposekit-0.4.0/deepposekit/models/StackedHourglass.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/__init__.py` & `us2deepposekit-0.4.0/deepposekit/models/__init__.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/backend/__init__.py` & `us2deepposekit-0.4.0/deepposekit/models/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/backend/backend.py` & `us2deepposekit-0.4.0/deepposekit/models/backend/backend.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/backend/registration.py` & `us2deepposekit-0.4.0/deepposekit/models/backend/registration.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/backend/utils.py` & `us2deepposekit-0.4.0/deepposekit/models/backend/utils.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/engine.py` & `us2deepposekit-0.4.0/deepposekit/models/engine.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/layers/convolutional.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/convolutional.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/layers/deeplabcut.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/deeplabcut.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/layers/densenet.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/densenet.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/layers/hourglass.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/hourglass.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/layers/imagenet_densenet.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/imagenet_densenet.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/layers/imagenet_mobile.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/imagenet_mobile.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/layers/imagenet_resnet.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/imagenet_resnet.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/layers/imagenet_utils.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/layers/imagenet_xception.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/imagenet_xception.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/layers/leap.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/leap.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/layers/squeeze_excitation.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/squeeze_excitation.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/layers/subpixel.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/subpixel.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/layers/util.py` & `us2deepposekit-0.4.0/deepposekit/models/layers/util.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/loading.py` & `us2deepposekit-0.4.0/deepposekit/models/loading.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/models/saving.py` & `us2deepposekit-0.4.0/deepposekit/models/saving.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/utils/__init__.py` & `us2deepposekit-0.4.0/deepposekit/annotate/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,12 +9,11 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
 from __future__ import absolute_import
 
-from deepposekit.utils import keypoints
-from deepposekit.utils import image
-from deepposekit.utils import io
+from deepposekit.annotate.KMeansSampler import KMeansSampler
```

### Comparing `us2deepposekit-0.3.9/deepposekit/utils/image.py` & `us2deepposekit-0.4.0/deepposekit/utils/image.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/utils/io.py` & `us2deepposekit-0.4.0/deepposekit/utils/io.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/deepposekit/utils/keypoints.py` & `us2deepposekit-0.4.0/deepposekit/utils/keypoints.py`

 * *Files identical despite different names*

### Comparing `us2deepposekit-0.3.9/setup.py` & `us2deepposekit-0.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 import warnings
 from setuptools import setup, find_packages
 
 DESCRIPTION = "a toolkit for pose estimation using deep learning"
 DISTNAME = "us2deepposekit"
 MAINTAINER = "Jacob Graving <jgraving@gmail.com>"
 MAINTAINER_EMAIL = "jgraving@gmail.com"
-URL = "https://github.com/morbitech1/deepposekit"
+URL = "https://github.com/jgraving/deepposekit"
 LICENSE = "Apache 2.0"
-DOWNLOAD_URL = "https://github.com/morbitech1/deepposekit.git"
-VERSION = "0.3.9"
+DOWNLOAD_URL = "https://github.com/jgraving/deepposekit.git"
+VERSION = "0.4.0"
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 if __name__ == "__main__":
 
@@ -50,15 +50,15 @@
         download_url=DOWNLOAD_URL,
         install_requires=[
             "numpy",
             "matplotlib",
             "pandas",
             "h5py>=3.1.0",
             "imgaug>=0.2.9",
-            "opencv-python",
+            "opencv-python-headless",
             "pyyaml",
         ],
         packages=find_packages(),
         zip_safe=False,
         classifiers=[
             "Intended Audience :: Science/Research",
             "Programming Language :: Python :: 3",
```

### Comparing `us2deepposekit-0.3.9/us2deepposekit.egg-info/PKG-INFO` & `us2deepposekit-0.4.0/us2deepposekit.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,175 +1,175 @@
 Metadata-Version: 2.1
 Name: us2deepposekit
-Version: 0.3.9
+Version: 0.4.0
 Summary: a toolkit for pose estimation using deep learning
-Home-page: https://github.com/morbitech1/deepposekit
+Home-page: https://github.com/jgraving/deepposekit
+Download-URL: https://github.com/jgraving/deepposekit.git
 Author: Jacob Graving <jgraving@gmail.com>
 Author-email: jgraving@gmail.com
 Maintainer: Jacob Graving <jgraving@gmail.com>
 Maintainer-email: jgraving@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/morbitech1/deepposekit.git
-Description: <p align="center">
-        <img src="https://github.com/jgraving/DeepPoseKit/blob/master/assets/deepposekit_logo.png" height="320px">
-        </p>
-        
-        # You have just found DeepPoseKit.
-        <p align="center">
-        <img src="https://github.com/jgraving/jgraving.github.io/blob/master/files/images/Figure1video1.gif" height="128px">
-        </p>
-        
-        DeepPoseKit is a software toolkit with a high-level API for 2D pose estimation of user-defined keypoints using deep learning—written in Python and built using [Tensorflow](https://github.com/tensorflow/tensorflow) and [Keras](https://www.tensorflow.org/guide/keras). Use DeepPoseKit if you need:
-        
-        - tools for annotating images or video frames with user-defined keypoints
-        - a straightforward but flexible data augmentation pipeline using the [imgaug package](https://github.com/aleju/imgaug)
-        - a Keras-based interface for initializing, training, and evaluating pose estimation models
-        - easy-to-use methods for saving and loading models and making predictions on new data
-        
-        DeepPoseKit is designed with a focus on *usability* and *extensibility*, as being able to go from idea to result with the least possible delay is key to doing good research.
-        
-        DeepPoseKit is currently limited to *individual pose estimation*. If individuals can be easily distinguished visually (i.e., they have differently colored bodies or are marked in some way), then multiple individuals can simply be labeled with separate keypoints (head1, tail1, head2, tail2, etc.). Otherwise DeepPoseKit can be extended to multiple individuals by first localizing, tracking, and cropping individuals with additional software such as [idtracker.ai](https://idtracker.ai/), [pinpoint](https://github.com/jgraving/pinpoint), or [Tracktor](https://github.com/vivekhsridhar/tracktor).
-        
-        Localization (without tracking) can also be achieved with deep learning software like [keras-retinanet](https://github.com/fizyr/keras-retinanet), the [Tensorflow Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection), or [MatterPort's Mask R-CNN](https://github.com/matterport/Mask_RCNN).
-        
-        [Check out our paper](https://doi.org/10.7554/eLife.47994) to find out more.
-        
-        <p align="center">
-        <img src="https://github.com/jgraving/jgraving.github.io/blob/master/files/images/zebra.gif" height="256px">
-        <img src="https://github.com/jgraving/jgraving.github.io/blob/master/files/images/locust.gif" height="256px">
-        </p>
-        
-        # How to use DeepPoseKit
-        
-        DeepPoseKit is designed for easy use. For example, training and saving a model requires only a few lines of code:
-        ```python
-        from deepposekit.io import DataGenerator, TrainingGenerator
-        from deepposekit.models import StackedDenseNet
-        
-        data_generator = DataGenerator('/path/to/annotation_data.h5')
-        train_generator = TrainingGenerator(data_generator)
-        model = StackedDenseNet(train_generator)
-        model.fit(batch_size=16, n_workers=8)
-        model.save('/path/to/saved_model.h5')
-        ```
-        Loading a trained model and running predictions on new data is also straightforward. For example, running predictions on a new video:
-        ```python
-        from deepposekit.models import load_model
-        from deepposekit.io import VideoReader
-        
-        model = load_model('/path/to/saved_model.h5')
-        reader = VideoReader('/path/to/video.mp4')
-        predictions = model.predict(reader)
-        ```
-        
-        ## Using DeepPoseKit is a 4-step process:
-        
-        - **1.** [Create an annotation set](https://github.com/jgraving/DeepPoseKit/blob/master/examples/step1_create_annotation_set.ipynb) <a href="https://colab.research.google.com/github/jgraving/deepposekit/blob/master/examples/step1_create_annotation_set.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
-        - **2.** [Annotate your data](https://github.com/jgraving/DeepPoseKit/blob/master/examples/step2_annotate_data.ipynb) with our built-in GUI (no Colab support)
-        - **3.** [Select and train](https://github.com/jgraving/DeepPoseKit/blob/master/examples/step3_train_model.ipynb) one our [pose estimation models](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/index.html) including [`StackedDenseNet`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/StackedDenseNet.html), [`StackedHourglass`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/StackedHourglass.html), [`DeepLabCut`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/DeepLabCut.html), and [`LEAP`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/LEAP.html). <a href="https://colab.research.google.com/github/jgraving/deepposekit/blob/master/examples/step3_train_model.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
-        - **4.** Use the trained model to:
-        	- a) [Initialize keypoints for unannotated data](https://github.com/jgraving/DeepPoseKit/blob/master/examples/step4a_initialize_annotations.ipynb) for faster annotations with *active learning*. <a href="https://colab.research.google.com/github/jgraving/deepposekit/blob/master/examples/step4a_initialize_annotations.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
-        	- b) [Predict on new data and refine the training set](https://github.com/jgraving/DeepPoseKit/blob/master/examples/step4b_predict_new_data.ipynb) to improve performance. <a href="https://colab.research.google.com/github/jgraving/deepposekit/blob/master/examples/step4b_predict_new_data.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
-        
-        ## For more details:
-        
-        - See [our example notebooks](https://github.com/jgraving/deepposekit/blob/master/examples/)
-        - Check the [documentation](http://docs.deepposekit.org)
-        - Read [our paper](https://doi.org/10.7554/eLife.47994)
-        
-        ## "I already have annotated data"
-        
-        DeepPoseKit is designed to be extensible, so loading data in other formats is possible.
-        
-        If you have annotated data from DeepLabCut (http://deeplabcut.org), try [our (experimental) example notebook ](https://github.com/jgraving/DeepPoseKit/blob/master/examples/deeplabcut_data_example.ipynb) for loading data in this format. <a href="https://colab.research.google.com/github/jgraving/deepposekit/blob/master/examples/deeplabcut_data_example.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
-        
-        Have data in another format? You can write your own custom generator to load it.
-        Check out the [example for writing custom data generators](https://github.com/jgraving/DeepPoseKit/blob/master/examples/custom_data_generator.ipynb). <a href="https://colab.research.google.com/github/jgraving/deepposekit/blob/master/examples/custom_data_generator.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
-        
-        # Installation
-        
-        DeepPoseKit requires [Tensorflow](https://github.com/tensorflow/tensorflow) for training and using pose estimation models. [Tensorflow](https://github.com/tensorflow/tensorflow) should be manually installed, along with dependencies such as CUDA and cuDNN, before installing DeepPoseKit:
-        
-        - [Tensorflow Installation Instructions](https://www.tensorflow.org/install)
-        - Any Tensorflow version >=1.13.0 should be compatible (including 2.0).
-        
-        DeepPoseKit has only been tested on Ubuntu 18.04, which is the recommended system for using the toolkit. 
-        
-        Install the latest stable release with pip:
-        ```bash
-        pip install --update deepposekit
-        ```
-        
-        Install the latest development version with pip:
-        ```bash
-        pip install --update git+https://www.github.com/jgraving/deepposekit.git
-        ```
-        
-        You can download example datasets from our [DeepPoseKit Data](https://github.com/jgraving/deepposekit-data) repository:
-        ```bash
-        git clone https://www.github.com/jgraving/deepposekit-data
-        ```
-        
-        ## Installing with Anaconda on Windows
-        
-        To install DeepPoseKit on Windows, you must first manually install `Shapely`, one of the dependencies for the [imgaug package](https://github.com/aleju/imgaug):
-        ```bash
-        conda install -c conda-forge shapely
-        ```
-        We also recommend installing DeepPoseKit from within Python rather than using the command line, either from within Jupyter or another IDE, to ensure it is installed in the correct working environment:
-        ```python
-        import sys
-        !{sys.executable} -m pip install --update deepposekit
-        ```
-        # Contributors and Development  
-           
-        DeepPoseKit was developed by [Jake Graving](https://github.com/jgraving) and [Daniel Chae](https://github.com/dchaebae), and is still being actively developed. .
-        
-        We welcome community involvement and public contributions to the toolkit. If you wish to contribute, please [fork the repository](https://help.github.com/en/articles/fork-a-repo) to make your modifications and [submit a pull request](https://help.github.com/en/articles/creating-a-pull-request-from-a-fork).
-        
-        If you'd like to get involved with developing DeepPoseKit, get in touch (jgraving@gmail.com) and check out [our development roadmap](https://github.com/jgraving/DeepPoseKit/blob/master/DEVELOPMENT.md) to see future plans for the package.  
-        
-        # Issues  
-         
-        Please submit bugs or feature requests to the [GitHub issue tracker](https://github.com/jgraving/deepposekit/issues/new). Please limit reported issues to the DeepPoseKit codebase and provide as much detail as you can with a minimal working example if possible.
-        
-        If you experience problems with [Tensorflow](https://github.com/tensorflow/tensorflow), such as installing CUDA or cuDNN dependencies, then please direct issues to those development teams.
-        
-        # License
-        
-        Released under a Apache 2.0 License. See [LICENSE](https://github.com/jgraving/deepposekit/blob/master/LICENSE) for details.
-        
-        # References
-        
-        If you use DeepPoseKit for your research please cite [our open-access paper](http://paper.deepposekit.org):
-        
-            @article{graving2019deepposekit,
-                     title={DeepPoseKit, a software toolkit for fast and robust animal pose estimation using deep learning},
-                     author={Graving, Jacob M and Chae, Daniel and Naik, Hemal and Li, Liang and Koger, Benjamin and Costelloe, Blair R and Couzin, Iain D},
-                     journal={eLife},
-                     volume={8},
-                     pages={e47994},
-                     year={2019},
-                     publisher={eLife Sciences Publications Limited}
-                     url={https://doi.org/10.7554/eLife.47994},
-                     }
-        
-        You can also read [our open-access preprint](http://preprint.deepposekit.org).
-        
-        If you use the [imgaug package](https://github.com/aleju/imgaug) for data augmentation, please also consider [citing it](https://github.com/aleju/imgaug/blob/master/README.md#citation).
-        
-        If you [use data](https://github.com/jgraving/DeepPoseKit#i-already-have-annotated-data) that was annotated with the DeepLabCut package (http://deeplabcut.org) for your research, be sure to [cite it](https://github.com/AlexEMG/DeepLabCut/blob/master/README.md#references).
-        
-        Please also consider citing the relevant references for the pose estimation model(s) used in your research, which can be found in the documentation (i.e., [`StackedDenseNet`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/StackedDenseNet.html#references), [`StackedHourglass`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/StackedHourglass.html#references), [`DeepLabCut`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/DeepLabCut.html#references), [`LEAP`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/LEAP.html#references)).
-        
-        # News
-        - **October 2019:** Our paper describing DeepPoseKit is published at eLife! (http://paper.deepposekit.org)
-        - **September 2019**: 
-            - Nature News covers DeepPoseKit: [Deep learning powers a motion-tracking revolution](http://doi.org/10.1038/d41586-019-02942-5)
-            - v0.3.0 is released. See [the release notes](https://github.com/jgraving/DeepPoseKit/releases/tag/v0.3.0).
-        - **April 2019:** The DeepPoseKit preprint is on biorxiv (http://preprint.deepposekit.org)
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+<img src="https://github.com/jgraving/DeepPoseKit/blob/master/assets/deepposekit_logo.png" height="320px">
+</p>
+
+# You have just found DeepPoseKit.
+<p align="center">
+<img src="https://github.com/jgraving/jgraving.github.io/blob/master/files/images/Figure1video1.gif" height="128px">
+</p>
+
+DeepPoseKit is a software toolkit with a high-level API for 2D pose estimation of user-defined keypoints using deep learning—written in Python and built using [Tensorflow](https://github.com/tensorflow/tensorflow) and [Keras](https://www.tensorflow.org/guide/keras). Use DeepPoseKit if you need:
+
+- tools for annotating images or video frames with user-defined keypoints
+- a straightforward but flexible data augmentation pipeline using the [imgaug package](https://github.com/aleju/imgaug)
+- a Keras-based interface for initializing, training, and evaluating pose estimation models
+- easy-to-use methods for saving and loading models and making predictions on new data
+
+DeepPoseKit is designed with a focus on *usability* and *extensibility*, as being able to go from idea to result with the least possible delay is key to doing good research.
+
+DeepPoseKit is currently limited to *individual pose estimation*. If individuals can be easily distinguished visually (i.e., they have differently colored bodies or are marked in some way), then multiple individuals can simply be labeled with separate keypoints (head1, tail1, head2, tail2, etc.). Otherwise DeepPoseKit can be extended to multiple individuals by first localizing, tracking, and cropping individuals with additional software such as [idtracker.ai](https://idtracker.ai/), [pinpoint](https://github.com/jgraving/pinpoint), or [Tracktor](https://github.com/vivekhsridhar/tracktor).
+
+Localization (without tracking) can also be achieved with deep learning software like [keras-retinanet](https://github.com/fizyr/keras-retinanet), the [Tensorflow Object Detection API](https://github.com/tensorflow/models/tree/master/research/object_detection), or [MatterPort's Mask R-CNN](https://github.com/matterport/Mask_RCNN).
+
+[Check out our paper](https://doi.org/10.7554/eLife.47994) to find out more.
+
+<p align="center">
+<img src="https://github.com/jgraving/jgraving.github.io/blob/master/files/images/zebra.gif" height="256px">
+<img src="https://github.com/jgraving/jgraving.github.io/blob/master/files/images/locust.gif" height="256px">
+</p>
+
+# How to use DeepPoseKit
+
+DeepPoseKit is designed for easy use. For example, training and saving a model requires only a few lines of code:
+```python
+from deepposekit.io import DataGenerator, TrainingGenerator
+from deepposekit.models import StackedDenseNet
+
+data_generator = DataGenerator('/path/to/annotation_data.h5')
+train_generator = TrainingGenerator(data_generator)
+model = StackedDenseNet(train_generator)
+model.fit(batch_size=16, n_workers=8)
+model.save('/path/to/saved_model.h5')
+```
+Loading a trained model and running predictions on new data is also straightforward. For example, running predictions on a new video:
+```python
+from deepposekit.models import load_model
+from deepposekit.io import VideoReader
+
+model = load_model('/path/to/saved_model.h5')
+reader = VideoReader('/path/to/video.mp4')
+predictions = model.predict(reader)
+```
+
+## Using DeepPoseKit is a 4-step process:
+
+- **1.** [Create an annotation set](https://github.com/jgraving/DeepPoseKit/blob/master/examples/step1_create_annotation_set.ipynb) <a href="https://colab.research.google.com/github/jgraving/deepposekit/blob/master/examples/step1_create_annotation_set.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+- **2.** [Annotate your data](https://github.com/jgraving/DeepPoseKit/blob/master/examples/step2_annotate_data.ipynb) with our built-in GUI (no Colab support)
+- **3.** [Select and train](https://github.com/jgraving/DeepPoseKit/blob/master/examples/step3_train_model.ipynb) one our [pose estimation models](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/index.html) including [`StackedDenseNet`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/StackedDenseNet.html), [`StackedHourglass`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/StackedHourglass.html), [`DeepLabCut`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/DeepLabCut.html), and [`LEAP`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/LEAP.html). <a href="https://colab.research.google.com/github/jgraving/deepposekit/blob/master/examples/step3_train_model.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+- **4.** Use the trained model to:
+	- a) [Initialize keypoints for unannotated data](https://github.com/jgraving/DeepPoseKit/blob/master/examples/step4a_initialize_annotations.ipynb) for faster annotations with *active learning*. <a href="https://colab.research.google.com/github/jgraving/deepposekit/blob/master/examples/step4a_initialize_annotations.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+	- b) [Predict on new data and refine the training set](https://github.com/jgraving/DeepPoseKit/blob/master/examples/step4b_predict_new_data.ipynb) to improve performance. <a href="https://colab.research.google.com/github/jgraving/deepposekit/blob/master/examples/step4b_predict_new_data.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+
+## For more details:
+
+- See [our example notebooks](https://github.com/jgraving/deepposekit/blob/master/examples/)
+- Check the [documentation](http://docs.deepposekit.org)
+- Read [our paper](https://doi.org/10.7554/eLife.47994)
+
+## "I already have annotated data"
+
+DeepPoseKit is designed to be extensible, so loading data in other formats is possible.
+
+If you have annotated data from DeepLabCut (http://deeplabcut.org), try [our (experimental) example notebook ](https://github.com/jgraving/DeepPoseKit/blob/master/examples/deeplabcut_data_example.ipynb) for loading data in this format. <a href="https://colab.research.google.com/github/jgraving/deepposekit/blob/master/examples/deeplabcut_data_example.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+
+Have data in another format? You can write your own custom generator to load it.
+Check out the [example for writing custom data generators](https://github.com/jgraving/DeepPoseKit/blob/master/examples/custom_data_generator.ipynb). <a href="https://colab.research.google.com/github/jgraving/deepposekit/blob/master/examples/custom_data_generator.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+
+# Installation
+
+DeepPoseKit requires [Tensorflow](https://github.com/tensorflow/tensorflow) for training and using pose estimation models. [Tensorflow](https://github.com/tensorflow/tensorflow) should be manually installed, along with dependencies such as CUDA and cuDNN, before installing DeepPoseKit:
+
+- [Tensorflow Installation Instructions](https://www.tensorflow.org/install)
+- Any Tensorflow version >=1.13.0 should be compatible (including 2.0).
+
+DeepPoseKit has only been tested on Ubuntu 18.04, which is the recommended system for using the toolkit. 
+
+Install the latest stable release with pip:
+```bash
+pip install --update deepposekit
+```
+
+Install the latest development version with pip:
+```bash
+pip install --update git+https://www.github.com/jgraving/deepposekit.git
+```
+
+You can download example datasets from our [DeepPoseKit Data](https://github.com/jgraving/deepposekit-data) repository:
+```bash
+git clone https://www.github.com/jgraving/deepposekit-data
+```
+
+## Installing with Anaconda on Windows
+
+To install DeepPoseKit on Windows, you must first manually install `Shapely`, one of the dependencies for the [imgaug package](https://github.com/aleju/imgaug):
+```bash
+conda install -c conda-forge shapely
+```
+We also recommend installing DeepPoseKit from within Python rather than using the command line, either from within Jupyter or another IDE, to ensure it is installed in the correct working environment:
+```python
+import sys
+!{sys.executable} -m pip install --update deepposekit
+```
+# Contributors and Development  
+   
+DeepPoseKit was developed by [Jake Graving](https://github.com/jgraving) and [Daniel Chae](https://github.com/dchaebae), and is still being actively developed. .
+
+We welcome community involvement and public contributions to the toolkit. If you wish to contribute, please [fork the repository](https://help.github.com/en/articles/fork-a-repo) to make your modifications and [submit a pull request](https://help.github.com/en/articles/creating-a-pull-request-from-a-fork).
+
+If you'd like to get involved with developing DeepPoseKit, get in touch (jgraving@gmail.com) and check out [our development roadmap](https://github.com/jgraving/DeepPoseKit/blob/master/DEVELOPMENT.md) to see future plans for the package.  
+
+# Issues  
+ 
+Please submit bugs or feature requests to the [GitHub issue tracker](https://github.com/jgraving/deepposekit/issues/new). Please limit reported issues to the DeepPoseKit codebase and provide as much detail as you can with a minimal working example if possible.
+
+If you experience problems with [Tensorflow](https://github.com/tensorflow/tensorflow), such as installing CUDA or cuDNN dependencies, then please direct issues to those development teams.
+
+# License
+
+Released under a Apache 2.0 License. See [LICENSE](https://github.com/jgraving/deepposekit/blob/master/LICENSE) for details.
+
+# References
+
+If you use DeepPoseKit for your research please cite [our open-access paper](http://paper.deepposekit.org):
+
+    @article{graving2019deepposekit,
+             title={DeepPoseKit, a software toolkit for fast and robust animal pose estimation using deep learning},
+             author={Graving, Jacob M and Chae, Daniel and Naik, Hemal and Li, Liang and Koger, Benjamin and Costelloe, Blair R and Couzin, Iain D},
+             journal={eLife},
+             volume={8},
+             pages={e47994},
+             year={2019},
+             publisher={eLife Sciences Publications Limited}
+             url={https://doi.org/10.7554/eLife.47994},
+             }
+
+You can also read [our open-access preprint](http://preprint.deepposekit.org).
+
+If you use the [imgaug package](https://github.com/aleju/imgaug) for data augmentation, please also consider [citing it](https://github.com/aleju/imgaug/blob/master/README.md#citation).
+
+If you [use data](https://github.com/jgraving/DeepPoseKit#i-already-have-annotated-data) that was annotated with the DeepLabCut package (http://deeplabcut.org) for your research, be sure to [cite it](https://github.com/AlexEMG/DeepLabCut/blob/master/README.md#references).
+
+Please also consider citing the relevant references for the pose estimation model(s) used in your research, which can be found in the documentation (i.e., [`StackedDenseNet`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/StackedDenseNet.html#references), [`StackedHourglass`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/StackedHourglass.html#references), [`DeepLabCut`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/DeepLabCut.html#references), [`LEAP`](http://jakegraving.com/DeepPoseKit/html/deepposekit/models/LEAP.html#references)).
+
+# News
+- **October 2019:** Our paper describing DeepPoseKit is published at eLife! (http://paper.deepposekit.org)
+- **September 2019**: 
+    - Nature News covers DeepPoseKit: [Deep learning powers a motion-tracking revolution](http://doi.org/10.1038/d41586-019-02942-5)
+    - v0.3.0 is released. See [the release notes](https://github.com/jgraving/DeepPoseKit/releases/tag/v0.3.0).
+- **April 2019:** The DeepPoseKit preprint is on biorxiv (http://preprint.deepposekit.org)
```

### Comparing `us2deepposekit-0.3.9/us2deepposekit.egg-info/SOURCES.txt` & `us2deepposekit-0.4.0/us2deepposekit.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,26 @@
+LICENSE
 README.md
 setup.py
 deepposekit/__init__.py
 deepposekit/callbacks.py
 deepposekit/annotate/KMeansSampler.py
 deepposekit/annotate/__init__.py
-deepposekit/annotate/gui/Annotator.py
-deepposekit/annotate/gui/GUI.py
-deepposekit/annotate/gui/Skeleton.py
-deepposekit/annotate/gui/__init__.py
 deepposekit/annotate/utils/__init__.py
 deepposekit/annotate/utils/hotkeys.py
 deepposekit/annotate/utils/image.py
 deepposekit/augment/FlipAxis.py
 deepposekit/augment/__init__.py
 deepposekit/io/BaseGenerator.py
 deepposekit/io/DLCDataGenerator.py
 deepposekit/io/DataGenerator.py
 deepposekit/io/ImageGenerator.py
 deepposekit/io/TrainingGenerator.py
 deepposekit/io/__init__.py
 deepposekit/io/utils.py
-deepposekit/io/video.py
 deepposekit/models/DeepLabCut.py
 deepposekit/models/LEAP.py
 deepposekit/models/StackedDenseNet.py
 deepposekit/models/StackedHourglass.py
 deepposekit/models/__init__.py
 deepposekit/models/engine.py
 deepposekit/models/loading.py
```


# Comparing `tmp/easy_local_features-0.3.3.tar.gz` & `tmp/easy_local_features-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_local_features-0.3.3.tar", last modified: Tue Jul 11 16:39:47 2023, max compression
+gzip compressed data, was "easy_local_features-0.3.4.tar", last modified: Wed Jul 12 06:52:32 2023, max compression
```

## Comparing `easy_local_features-0.3.3.tar` & `easy_local_features-0.3.4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.866134 easy_local_features-0.3.3/
--rw-r--r--   0 cadar      (501) staff       (20)    32722 2023-07-01 15:16:15.000000 easy_local_features-0.3.3/LICENSE_DISK.txt
--rw-r--r--   0 cadar      (501) staff       (20)    21121 2023-07-01 17:04:24.000000 easy_local_features-0.3.3/LICENSE_R2D2.txt
--rw-r--r--   0 cadar      (501) staff       (20)     7009 2023-07-01 16:24:52.000000 easy_local_features-0.3.3/LICENSE_SUPERGLUE.txt
--rw-r--r--   0 cadar      (501) staff       (20)     2023 2023-07-11 16:39:47.865922 easy_local_features-0.3.3/PKG-INFO
--rw-r--r--   0 cadar      (501) staff       (20)     1771 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/README.md
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.847938 easy_local_features-0.3.3/easy_local_features/
--rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-01 15:35:14.000000 easy_local_features-0.3.3/easy_local_features/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.850061 easy_local_features-0.3.3/easy_local_features/datasets/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-06-12 19:58:13.000000 easy_local_features-0.3.3/easy_local_features/datasets/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)    10235 2023-07-11 16:37:31.000000 easy_local_features-0.3.3/easy_local_features/datasets/augmentor.py
--rw-r--r--   0 cadar      (501) staff       (20)     3034 2023-06-12 19:58:13.000000 easy_local_features-0.3.3/easy_local_features/datasets/download.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.851981 easy_local_features-0.3.3/easy_local_features/feature/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/feature/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)    34684 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/feature/baseline_dalf.py
--rw-r--r--   0 cadar      (501) staff       (20)     2624 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/feature/baseline_deal.py
--rw-r--r--   0 cadar      (501) staff       (20)     6746 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/feature/baseline_disk.py
--rw-r--r--   0 cadar      (501) staff       (20)     6012 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/feature/baseline_r2d2.py
--rw-r--r--   0 cadar      (501) staff       (20)     2857 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/feature/baseline_superpoint.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.852959 easy_local_features-0.3.3/easy_local_features/matching/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 21:59:23.000000 easy_local_features-0.3.3/easy_local_features/matching/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2103 2023-07-04 22:47:59.000000 easy_local_features-0.3.3/easy_local_features/matching/baseline_loftr.py
--rw-r--r--   0 cadar      (501) staff       (20)     5116 2023-07-01 16:48:02.000000 easy_local_features-0.3.3/easy_local_features/matching/baseline_superglue.py
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 22:06:22.000000 easy_local_features-0.3.3/easy_local_features/matching/core.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.853072 easy_local_features-0.3.3/easy_local_features/submodules/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:42:35.000000 easy_local_features-0.3.3/easy_local_features/submodules/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.853186 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:23:41.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.853302 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/
--rw-r--r--   0 cadar      (501) staff       (20)       24 2023-07-01 15:39:51.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.853906 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/common/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:40:58.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/common/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2652 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/common/structs.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.855327 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/
--rw-r--r--   0 cadar      (501) staff       (20)       79 2023-07-01 08:54:41.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)      291 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/distance_matrix.py
--rw-r--r--   0 cadar      (501) staff       (20)     2096 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/epi.py
--rw-r--r--   0 cadar      (501) staff       (20)     3406 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/pose.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.856653 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/
--rw-r--r--   0 cadar      (501) staff       (20)      113 2023-07-01 08:54:41.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2732 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py
--rw-r--r--   0 cadar      (501) staff       (20)     2566 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py
--rw-r--r--   0 cadar      (501) staff       (20)     5454 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/detector.py
--rw-r--r--   0 cadar      (501) staff       (20)     2177 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/disk.py
--rw-r--r--   0 cadar      (501) staff       (20)      865 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/nms.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.857757 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/
--rw-r--r--   0 cadar      (501) staff       (20)      249 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     4159 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/blocks.py
--rw-r--r--   0 cadar      (501) staff       (20)     2070 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/ops.py
--rw-r--r--   0 cadar      (501) staff       (20)     3289 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/unet.py
--rw-r--r--   0 cadar      (501) staff       (20)     1291 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/utils.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.859159 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:53:50.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     6223 2023-07-01 17:01:09.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/extract.py
--rw-r--r--   0 cadar      (501) staff       (20)     9927 2023-07-01 16:26:30.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/extract_kapture.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.861444 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:54.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     2360 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/ap_loss.py
--rw-r--r--   0 cadar      (501) staff       (20)     1720 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/losses.py
--rw-r--r--   0 cadar      (501) staff       (20)     7158 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/patchnet.py
--rw-r--r--   0 cadar      (501) staff       (20)     1760 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py
--rw-r--r--   0 cadar      (501) staff       (20)     2006 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py
--rw-r--r--   0 cadar      (501) staff       (20)    15031 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/sampler.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.863207 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:23.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     1080 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/common.py
--rw-r--r--   0 cadar      (501) staff       (20)    14318 2023-07-01 17:00:44.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/dataloader.py
--rw-r--r--   0 cadar      (501) staff       (20)     2208 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/trainer.py
--rw-r--r--   0 cadar      (501) staff       (20)    18298 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/transforms.py
--rw-r--r--   0 cadar      (501) staff       (20)     7160 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py
--rw-r--r--   0 cadar      (501) staff       (20)     5647 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/viz.py
--rw-r--r--   0 cadar      (501) staff       (20)     5018 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/train.py
--rw-r--r--   0 cadar      (501) staff       (20)     4203 2023-07-01 16:26:31.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/viz_heatmaps.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.863465 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:22:28.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/__init__.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.864874 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:16:09.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)     3417 2023-07-01 16:16:09.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/matching.py
--rw-r--r--   0 cadar      (501) staff       (20)    11537 2023-07-01 16:40:16.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/superglue.py
--rw-r--r--   0 cadar      (501) staff       (20)     8092 2023-07-01 16:40:03.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/superpoint.py
--rw-r--r--   0 cadar      (501) staff       (20)    20039 2023-07-01 16:16:09.000000 easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/utils.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.865448 easy_local_features-0.3.3/easy_local_features/utils/
--rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/utils/__init__.py
--rw-r--r--   0 cadar      (501) staff       (20)      293 2023-07-11 16:38:37.000000 easy_local_features-0.3.3/easy_local_features/utils/generic_match.py
-drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-11 16:39:47.849012 easy_local_features-0.3.3/easy_local_features.egg-info/
--rw-r--r--   0 cadar      (501) staff       (20)     2023 2023-07-11 16:39:47.000000 easy_local_features-0.3.3/easy_local_features.egg-info/PKG-INFO
--rw-r--r--   0 cadar      (501) staff       (20)     3649 2023-07-11 16:39:47.000000 easy_local_features-0.3.3/easy_local_features.egg-info/SOURCES.txt
--rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-11 16:39:47.000000 easy_local_features-0.3.3/easy_local_features.egg-info/dependency_links.txt
--rw-r--r--   0 cadar      (501) staff       (20)       68 2023-07-11 16:39:47.000000 easy_local_features-0.3.3/easy_local_features.egg-info/requires.txt
--rw-r--r--   0 cadar      (501) staff       (20)       20 2023-07-11 16:39:47.000000 easy_local_features-0.3.3/easy_local_features.egg-info/top_level.txt
--rw-r--r--   0 cadar      (501) staff       (20)       38 2023-07-11 16:39:47.866195 easy_local_features-0.3.3/setup.cfg
--rw-r--r--   0 cadar      (501) staff       (20)      910 2023-07-11 16:39:34.000000 easy_local_features-0.3.3/setup.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.782101 easy_local_features-0.3.4/
+-rw-r--r--   0 cadar      (501) staff       (20)    32722 2023-07-01 15:16:15.000000 easy_local_features-0.3.4/LICENSE_DISK.txt
+-rw-r--r--   0 cadar      (501) staff       (20)    21121 2023-07-01 17:04:24.000000 easy_local_features-0.3.4/LICENSE_R2D2.txt
+-rw-r--r--   0 cadar      (501) staff       (20)     7009 2023-07-01 16:24:52.000000 easy_local_features-0.3.4/LICENSE_SUPERGLUE.txt
+-rw-r--r--   0 cadar      (501) staff       (20)     2023 2023-07-12 06:52:32.781855 easy_local_features-0.3.4/PKG-INFO
+-rw-r--r--   0 cadar      (501) staff       (20)     1771 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/README.md
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.763865 easy_local_features-0.3.4/easy_local_features/
+-rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-01 15:35:14.000000 easy_local_features-0.3.4/easy_local_features/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.765560 easy_local_features-0.3.4/easy_local_features/datasets/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-06-12 19:58:13.000000 easy_local_features-0.3.4/easy_local_features/datasets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)    10688 2023-07-11 20:37:33.000000 easy_local_features-0.3.4/easy_local_features/datasets/augmentor.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3034 2023-06-12 19:58:13.000000 easy_local_features-0.3.4/easy_local_features/datasets/download.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.767572 easy_local_features-0.3.4/easy_local_features/feature/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/feature/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)    34684 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/feature/baseline_dalf.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2624 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/feature/baseline_deal.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6746 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/feature/baseline_disk.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6012 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/feature/baseline_r2d2.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2857 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/feature/baseline_superpoint.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.768392 easy_local_features-0.3.4/easy_local_features/matching/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 21:59:23.000000 easy_local_features-0.3.4/easy_local_features/matching/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2103 2023-07-04 22:47:59.000000 easy_local_features-0.3.4/easy_local_features/matching/baseline_loftr.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5116 2023-07-01 16:48:02.000000 easy_local_features-0.3.4/easy_local_features/matching/baseline_superglue.py
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-04 22:06:22.000000 easy_local_features-0.3.4/easy_local_features/matching/core.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.768563 easy_local_features-0.3.4/easy_local_features/submodules/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:42:35.000000 easy_local_features-0.3.4/easy_local_features/submodules/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.768741 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:23:41.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.769301 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/
+-rw-r--r--   0 cadar      (501) staff       (20)       24 2023-07-01 15:39:51.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.769763 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/common/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 15:40:58.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/common/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2652 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/common/structs.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.770640 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/geom/
+-rw-r--r--   0 cadar      (501) staff       (20)       79 2023-07-01 08:54:41.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/geom/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)      291 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/geom/distance_matrix.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2096 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/geom/epi.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3406 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/geom/pose.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.772179 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/model/
+-rw-r--r--   0 cadar      (501) staff       (20)      113 2023-07-01 08:54:41.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/model/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2732 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2566 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5454 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/model/detector.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2177 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/model/disk.py
+-rw-r--r--   0 cadar      (501) staff       (20)      865 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/model/nms.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.773444 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/unets/
+-rw-r--r--   0 cadar      (501) staff       (20)      249 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/unets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     4159 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/unets/blocks.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2070 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/unets/ops.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3289 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/unets/unet.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1291 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/unets/utils.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.774910 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:53:50.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     6223 2023-07-01 17:01:09.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/extract.py
+-rw-r--r--   0 cadar      (501) staff       (20)     9927 2023-07-01 16:26:30.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/extract_kapture.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.776491 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:54.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2360 2023-07-01 16:26:31.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/ap_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1720 2023-07-01 16:26:31.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/losses.py
+-rw-r--r--   0 cadar      (501) staff       (20)     7158 2023-07-01 16:26:31.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/patchnet.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1760 2023-07-01 16:26:31.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2006 2023-07-01 16:26:31.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py
+-rw-r--r--   0 cadar      (501) staff       (20)    15031 2023-07-01 16:26:31.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/sampler.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.779807 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:54:23.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     1080 2023-07-01 16:26:31.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/common.py
+-rw-r--r--   0 cadar      (501) staff       (20)    14318 2023-07-01 17:00:44.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/dataloader.py
+-rw-r--r--   0 cadar      (501) staff       (20)     2208 2023-07-01 16:26:31.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/trainer.py
+-rw-r--r--   0 cadar      (501) staff       (20)    18298 2023-07-01 16:26:31.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/transforms.py
+-rw-r--r--   0 cadar      (501) staff       (20)     7160 2023-07-01 16:26:31.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5647 2023-07-01 16:26:31.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/viz.py
+-rw-r--r--   0 cadar      (501) staff       (20)     5018 2023-07-01 16:26:31.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/train.py
+-rw-r--r--   0 cadar      (501) staff       (20)     4203 2023-07-01 16:26:31.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/viz_heatmaps.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.780156 easy_local_features-0.3.4/easy_local_features/submodules/git_superglue/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:22:28.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_superglue/__init__.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.781120 easy_local_features-0.3.4/easy_local_features/submodules/git_superglue/models/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-01 16:16:09.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_superglue/models/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)     3417 2023-07-01 16:16:09.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_superglue/models/matching.py
+-rw-r--r--   0 cadar      (501) staff       (20)    11537 2023-07-01 16:40:16.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_superglue/models/superglue.py
+-rw-r--r--   0 cadar      (501) staff       (20)     8092 2023-07-01 16:40:03.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_superglue/models/superpoint.py
+-rw-r--r--   0 cadar      (501) staff       (20)    20039 2023-07-01 16:16:09.000000 easy_local_features-0.3.4/easy_local_features/submodules/git_superglue/models/utils.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.781515 easy_local_features-0.3.4/easy_local_features/utils/
+-rw-r--r--   0 cadar      (501) staff       (20)        0 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/utils/__init__.py
+-rw-r--r--   0 cadar      (501) staff       (20)      293 2023-07-11 16:38:37.000000 easy_local_features-0.3.4/easy_local_features/utils/generic_match.py
+drwxr-xr-x   0 cadar      (501) staff       (20)        0 2023-07-12 06:52:32.764996 easy_local_features-0.3.4/easy_local_features.egg-info/
+-rw-r--r--   0 cadar      (501) staff       (20)     2023 2023-07-12 06:52:32.000000 easy_local_features-0.3.4/easy_local_features.egg-info/PKG-INFO
+-rw-r--r--   0 cadar      (501) staff       (20)     3649 2023-07-12 06:52:32.000000 easy_local_features-0.3.4/easy_local_features.egg-info/SOURCES.txt
+-rw-r--r--   0 cadar      (501) staff       (20)        1 2023-07-12 06:52:32.000000 easy_local_features-0.3.4/easy_local_features.egg-info/dependency_links.txt
+-rw-r--r--   0 cadar      (501) staff       (20)       68 2023-07-12 06:52:32.000000 easy_local_features-0.3.4/easy_local_features.egg-info/requires.txt
+-rw-r--r--   0 cadar      (501) staff       (20)       20 2023-07-12 06:52:32.000000 easy_local_features-0.3.4/easy_local_features.egg-info/top_level.txt
+-rw-r--r--   0 cadar      (501) staff       (20)       38 2023-07-12 06:52:32.782168 easy_local_features-0.3.4/setup.cfg
+-rw-r--r--   0 cadar      (501) staff       (20)      910 2023-07-12 06:52:14.000000 easy_local_features-0.3.4/setup.py
```

### Comparing `easy_local_features-0.3.3/LICENSE_DISK.txt` & `easy_local_features-0.3.4/LICENSE_DISK.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/LICENSE_R2D2.txt` & `easy_local_features-0.3.4/LICENSE_R2D2.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/LICENSE_SUPERGLUE.txt` & `easy_local_features-0.3.4/LICENSE_SUPERGLUE.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/PKG-INFO` & `easy_local_features-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_local_features
-Version: 0.3.3
+Version: 0.3.4
 Author: eucadar
 Author-email: python@eucadar.com
 Description-Content-Type: text/markdown
 License-File: LICENSE_DISK.txt
 License-File: LICENSE_R2D2.txt
 License-File: LICENSE_SUPERGLUE.txt
```

### Comparing `easy_local_features-0.3.3/README.md` & `easy_local_features-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/datasets/augmentor.py` & `easy_local_features-0.3.4/easy_local_features/datasets/augmentor.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     return H
 
 class AugmentationPipe(nn.Module):
     def __init__(
                 self, device,
                 img_dir=None,
                 load_dataset = False,
-                warp_resolution = (1200, 900),
+                warp_resolution = (448, 448),
                 out_resolution = (400, 300),
                 max_num_imgs = 40,
                 num_test_imgs = 200,
                 batch_size = 6,
                 sample_img = None
                 ):
         super(AugmentationPipe, self).__init__()
@@ -159,14 +159,25 @@
                         cv2.resize(cv2.imread(p), self.dims)                 
                         for p in tqdm.tqdm(self.all_imgs[-num_test_imgs:],
                                            desc='loading test')
                         ] 
 
             self.TPS = True
 
+    def load_image(self, path):
+        im = cv2.imread(path)
+        halfH, halfW = im.shape[0]//2, im.shape[1]//2
+        if halfH > halfW:
+            im = np.rot90(im)
+            halfH, halfW = halfW, halfH
+        im = im[halfH-self.dims[1]//2:halfH+self.dims[1]//2, halfW-self.dims[0]//2:halfW+self.dims[0]//2, :]
+        if im.shape[0] != self.dims[1] or im.shape[1] != self.dims[0]:
+            im = cv2.resize(im, self.dims)
+
+        return im
 
     def norm_pts_grid(self, x):
         if len(x.size()) == 2:
             return (x.view(1,-1,2) * self.dims_s / self.dims_t) * 2. - 1 
         return (x * self.dims_s / self.dims_t) * 2. - 1
 
     def denorm_pts_grid(self, x):
```

### Comparing `easy_local_features-0.3.3/easy_local_features/datasets/download.py` & `easy_local_features-0.3.4/easy_local_features/datasets/download.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/feature/baseline_dalf.py` & `easy_local_features-0.3.4/easy_local_features/feature/baseline_dalf.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/feature/baseline_deal.py` & `easy_local_features-0.3.4/easy_local_features/feature/baseline_deal.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/feature/baseline_disk.py` & `easy_local_features-0.3.4/easy_local_features/feature/baseline_disk.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/feature/baseline_r2d2.py` & `easy_local_features-0.3.4/easy_local_features/feature/baseline_r2d2.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/feature/baseline_superpoint.py` & `easy_local_features-0.3.4/easy_local_features/feature/baseline_superpoint.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/matching/baseline_loftr.py` & `easy_local_features-0.3.4/easy_local_features/matching/baseline_loftr.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/matching/baseline_superglue.py` & `easy_local_features-0.3.4/easy_local_features/matching/baseline_superglue.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/common/structs.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/common/structs.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/epi.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/geom/epi.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/geom/pose.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/geom/pose.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/model/consistent_matcher.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/model/cycle_matcher.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/detector.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/model/detector.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/disk.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/model/disk.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/model/nms.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/model/nms.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/blocks.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/unets/blocks.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/ops.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/unets/ops.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/unet.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/unets/unet.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_disk/disk/unets/utils.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_disk/disk/unets/utils.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/extract.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/extract.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/extract_kapture.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/extract_kapture.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/ap_loss.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/ap_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/losses.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/losses.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/patchnet.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/patchnet.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/reliability_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/repeatability_loss.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/nets/sampler.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/nets/sampler.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/common.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/common.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/dataloader.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/dataloader.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/trainer.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/transforms.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/transforms.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/transforms_tools.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/tools/viz.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/tools/viz.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/train.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/train.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_r2d2/viz_heatmaps.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_r2d2/viz_heatmaps.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/matching.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_superglue/models/matching.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/superglue.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_superglue/models/superglue.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/superpoint.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_superglue/models/superpoint.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features/submodules/git_superglue/models/utils.py` & `easy_local_features-0.3.4/easy_local_features/submodules/git_superglue/models/utils.py`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/easy_local_features.egg-info/PKG-INFO` & `easy_local_features-0.3.4/easy_local_features.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-local-features
-Version: 0.3.3
+Version: 0.3.4
 Author: eucadar
 Author-email: python@eucadar.com
 Description-Content-Type: text/markdown
 License-File: LICENSE_DISK.txt
 License-File: LICENSE_R2D2.txt
 License-File: LICENSE_SUPERGLUE.txt
```

### Comparing `easy_local_features-0.3.3/easy_local_features.egg-info/SOURCES.txt` & `easy_local_features-0.3.4/easy_local_features.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easy_local_features-0.3.3/setup.py` & `easy_local_features-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         long_description = f.read()
 else:
     with open('README.md', encoding='utf-8') as f:
         long_description = f.read()
 
 setup(
     name='easy_local_features',
-    version='0.3.3',
+    version='0.3.4',
     author='eucadar',
     author_email='python@eucadar.com',
     packages=find_packages(exclude=('tests', 'docs', 'assets')),
     include_package_data=True,
     install_requires=[
         'numpy',
         'scipy',
```


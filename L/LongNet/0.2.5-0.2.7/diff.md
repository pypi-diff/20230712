# Comparing `tmp/LongNet-0.2.5.tar.gz` & `tmp/LongNet-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.2.5.tar", last modified: Mon Jul 10 19:46:26 2023, max compression
+gzip compressed data, was "LongNet-0.2.7.tar", last modified: Wed Jul 12 17:54:57 2023, max compression
```

## Comparing `LongNet-0.2.5.tar` & `LongNet-0.2.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:26.197374 LongNet-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 19:46:16.000000 LongNet-0.2.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:26.193374 LongNet-0.2.5/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-10 19:46:16.000000 LongNet-0.2.5/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-10 19:46:16.000000 LongNet-0.2.5/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-07-10 19:46:16.000000 LongNet-0.2.5/LongNet/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-10 19:46:16.000000 LongNet-0.2.5/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-10 19:46:16.000000 LongNet-0.2.5/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-10 19:46:16.000000 LongNet-0.2.5/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:26.193374 LongNet-0.2.5/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 19:46:26.000000 LongNet-0.2.5/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-10 19:46:26.000000 LongNet-0.2.5/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:46:26.000000 LongNet-0.2.5/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 19:46:26.000000 LongNet-0.2.5/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-10 19:46:26.000000 LongNet-0.2.5/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 19:46:26.197374 LongNet-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-07-10 19:46:16.000000 LongNet-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:26.193374 LongNet-0.2.5/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:26.193374 LongNet-0.2.5/flash_attn/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/bert_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/flash_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/flash_attn_triton.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/flash_attn_triton_og.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/flash_blocksparse_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/flash_blocksparse_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/fused_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:26.193374 LongNet-0.2.5/flash_attn/flash_attn/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/layers/patch_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/layers/rotary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:26.193374 LongNet-0.2.5/flash_attn/flash_attn/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/losses/cross_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:26.193374 LongNet-0.2.5/flash_attn/flash_attn/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/models/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/models/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/models/gpt_neox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/models/gptj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/models/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/models/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/models/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:26.197374 LongNet-0.2.5/flash_attn/flash_attn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/modules/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/modules/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/modules/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:26.197374 LongNet-0.2.5/flash_attn/flash_attn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/ops/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/ops/fused_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    19306 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/ops/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/ops/rms_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:26.197374 LongNet-0.2.5/flash_attn/flash_attn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/utils/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/utils/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/flash_attn/utils/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-10 19:46:16.000000 LongNet-0.2.5/flash_attn/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:46:26.197374 LongNet-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-10 19:46:16.000000 LongNet-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:46:26.197374 LongNet-0.2.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-10 19:46:16.000000 LongNet-0.2.5/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.616438 LongNet-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 17:54:41.000000 LongNet-0.2.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.600437 LongNet-0.2.7/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-12 17:54:41.000000 LongNet-0.2.7/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-12 17:54:41.000000 LongNet-0.2.7/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-12 17:54:41.000000 LongNet-0.2.7/LongNet/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-12 17:54:41.000000 LongNet-0.2.7/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-12 17:54:41.000000 LongNet-0.2.7/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-12 17:54:41.000000 LongNet-0.2.7/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.600437 LongNet-0.2.7/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 17:54:57.000000 LongNet-0.2.7/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-12 17:54:57.000000 LongNet-0.2.7/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:54:57.000000 LongNet-0.2.7/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 17:54:57.000000 LongNet-0.2.7/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:54:57.000000 LongNet-0.2.7/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 17:54:57.616438 LongNet-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-07-12 17:54:41.000000 LongNet-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.600437 LongNet-0.2.7/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.604438 LongNet-0.2.7/flash_attn/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/bert_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/flash_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/flash_attn_triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/flash_attn_triton_og.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/flash_blocksparse_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/flash_blocksparse_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/fused_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.608438 LongNet-0.2.7/flash_attn/flash_attn/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/layers/patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/layers/rotary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.608438 LongNet-0.2.7/flash_attn/flash_attn/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/losses/cross_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.608438 LongNet-0.2.7/flash_attn/flash_attn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/gpt_neox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/gptj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.612438 LongNet-0.2.7/flash_attn/flash_attn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/modules/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/modules/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/modules/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.612438 LongNet-0.2.7/flash_attn/flash_attn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/ops/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/ops/fused_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19306 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/ops/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/ops/rms_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.616438 LongNet-0.2.7/flash_attn/flash_attn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/utils/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/utils/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:54:57.616438 LongNet-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 17:54:41.000000 LongNet-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.616438 LongNet-0.2.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 17:54:41.000000 LongNet-0.2.7/test/test.py
```

### Comparing `LongNet-0.2.5/LICENSE` & `LongNet-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/LongNet/attend.py` & `LongNet-0.2.7/LongNet/attend.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,33 @@
+from torch._C import dtype
+# !pip install torch
+# !pip install einops
+
+import math
+from collections import namedtuple
+from functools import wraps
+from packaging import version
 
-from einops import rearrange
-from functools import partial
 import torch
 from torch import nn, einsum, Tensor
 import torch.nn.functional as F
 
-from collections import namedtuple
-from functools import wraps
-from packaging import version
-from dataclasses import dataclass
+from einops import rearrange
 
-import math
+from dataclasses import dataclass
 
 # constants
 
 EfficientAttentionConfig = namedtuple('EfficientAttentionConfig', ['enable_flash', 'enable_math', 'enable_mem_efficient'])
 
-@dataclass
-class Intermediates:
-    qk_similarities: Tensor = None
-    pre_softmax_attn: Tensor = None
-    post_softmax_attn: Tensor = None
-
 # helpers
 
 def exists(val):
     return val is not None
 
-def default(val, d):
-    return val if exists(val) else d
-
 def once(fn):
     called = False
     @wraps(fn)
     def inner(x):
         nonlocal called
         if called:
             return
@@ -41,48 +35,40 @@
         return fn(x)
     return inner
 
 print_once = once(print)
 
 # main class
 
+
+@dataclass
+class Intermediates:
+    qk_similarities: Tensor = None
+    pre_softmax_attn: Tensor = None
+    post_softmax_attn: Tensor = None
+
+    def to_tuple(self):
+        return (self.qk_similarities, self.pre_softmax_attn, self.post_softmax_attn)
+
+# helpers
+
+
 class FlashAttention(nn.Module):
     def __init__(
         self,
-        *,
-        dropout = 0.,
-        attention_dropout=0.,
         causal = False,
-        heads = None,
-        talking_heads = False,
-        scale = None,
-        qk_norm = True,
-        flash = True,
+        dropout = 0.,
+        flash = True
     ):
         super().__init__()
-        self.scale = scale
-        self.qk_norm = qk_norm
-        self.causal = causal
-        self.attn_fn = partial(F.softmax, dtype = torch.float32) if not qk_norm else F.softmax
 
         self.dropout = dropout
+        self.attn_dropout = nn.Dropout(dropout)
 
-        self.attn_dropout = nn.Dropout(attention_dropout)   # modify this line
-
-        # talking heads
-
-        assert not (flash and talking_heads), 'talking heads not compatible with flash attention'
-
-        self.talking_heads = talking_heads
-        if talking_heads:
-            self.pre_softmax_talking_heads = nn.Conv2d(heads, heads, 1, bias = False)
-            self.post_softmax_talking_heads = nn.Conv2d(heads, heads, 1, bias = False)
-
-        # flash attention
-
+        self.causal = causal
         self.flash = flash
         assert not (flash and version.parse(torch.__version__) < version.parse('2.0.0')), 'in order to use flash attention, you must be using pytorch 2.0 or above'
 
         # determine efficient attention configs for cuda and cpu
 
         self.cpu_config = EfficientAttentionConfig(True, True, True)
         self.cuda_config = None
@@ -95,14 +81,18 @@
         if device_properties.major == 8 and device_properties.minor == 0:
             print_once('A100 GPU detected, using flash attention if input tensor is on cuda')
             self.cuda_config = EfficientAttentionConfig(True, False, False)
         else:
             print_once('Non-A100 GPU detected, using math or mem efficient attention if input tensor is on cuda')
             self.cuda_config = EfficientAttentionConfig(False, True, True)
 
+    def get_mask(self, i, j, device):
+        return torch.ones((i, j), device=device, dtype=torch.bool).triu(j - i + 1)
+
+
     def flash_attn(
         self,
         q, k, v,
         mask = None,
         attn_bias = None
     ):
         batch, heads, q_len, _, k_len, is_cuda, device = *q.shape, k.shape[-2], q.is_cuda, q.device
@@ -113,50 +103,45 @@
         if k.ndim == 3:
             k = rearrange(k, 'b ... -> b 1 ...').expand_as(q)
 
         if v.ndim == 3:
             v = rearrange(v, 'b ... -> b 1 ...').expand_as(q)
 
         # handle scale - by default they scale by dim_head ** -0.5, but need to take care if using cosine sim attention
-
-        if self.qk_norm:
-            default_scale = q.shape[-1] ** -0.5
-            q = q * (default_scale / self.scale)
-
         # Check if mask exists and expand to compatible shape
         # The mask is B L, so it would have to be expanded to B H N L
 
         causal = self.causal
 
         if exists(mask):
             assert mask.ndim == 4
             mask = mask.expand(batch, heads, q_len, k_len)
 
             # manually handle causal mask, if another mask was given
 
             if causal:
-                causal_mask = torch.ones((q_len, k_len), dtype = torch.bool, device = device).triu(k_len - q_len + 1)
-                mask = mask | causal_mask
+                causal_mask = self.create_causal_mask(q_len, k_len, device = device)
+                mask = mask & ~causal_mask
                 causal = False
 
         # handle alibi positional bias
         # convert from bool to float
 
         if exists(attn_bias):
             attn_bias = rearrange(attn_bias, 'h i j -> 1 h i j').expand(batch, -1, -1, -1)
 
             # if mask given, the mask would already contain the causal mask from above logic
             # otherwise, if no mask given but still causal, mask out alibi positional bias to a large negative number
 
             mask_value = -torch.finfo(q.dtype).max
 
             if exists(mask):
-                attn_bias = attn_bias.masked_fill(mask, mask_value // 2)
+                attn_bias = attn_bias.masked_fill(~mask, mask_value // 2)
             elif causal:
-                causal_mask = torch.ones((q_len, k_len), dtype = torch.bool, device = device).triu(k_len - q_len + 1)
+                causal_mask = self.create_causal_mask(q_len, k_len, device = device)
                 attn_bias = attn_bias.masked_fill(causal_mask, mask_value // 2)
                 causal = False
 
             # scaled_dot_product_attention handles attn_mask either as bool or additive bias
             # make it an additive bias here
 
             mask = attn_bias
@@ -171,157 +156,82 @@
             out = F.scaled_dot_product_attention(
                 q, k, v,
                 attn_mask = mask,
                 dropout_p = self.dropout if self.training else 0., 
                 is_causal = causal
             )
 
-        return out, Intermediates()
+            return out
 
-    def forward(
-        self,
-        q, k, v,
-        mask = None,
-        attn_bias = None,
-        prev_attn = None
-    ):
+    def forward(self, q, k, v, mask = None, attn_bias = None):
         """
         einstein notation
         b - batch
         h - heads
         n, i, j - sequence length (base sequence length, source, target)
         d - feature dimension
         """
 
-        n, device = q.shape[-2], q.device
+        q_len, k_len, device = q.shape[-2], k.shape[-2], q.device
 
-        scale = default(self.scale, q.shape[-1] ** -0.5)
-
-        if self.flash:
-            assert not exists(prev_attn), 'residual attention not compatible with flash attention'
-            return self.flash_attn(q, k, v, mask = mask, attn_bias = attn_bias)
+        scale = q.shape[-1] ** -0.5
 
         kv_einsum_eq = 'b j d' if k.ndim == 3 else 'b h j d'
 
-        dots = einsum(f'b h i d, {kv_einsum_eq} -> b h i j', q, k) * scale
+        if self.flash:
+            return self.flash_attn(q, k, v, mask = mask, attn_bias = attn_bias)
 
-        if exists(prev_attn):
-            dots = dots + prev_attn
+        # similarity
 
-        qk_similarities = dots.clone()
+        sim = einsum(f"b h i d, {kv_einsum_eq} -> b h i j", q, k) * scale
 
-        if self.talking_heads:
-            dots = self.pre_softmax_talking_heads(dots)
+        # attention bias
 
         if exists(attn_bias):
-            dots = dots + attn_bias
+            sim = sim + attn_bias
 
-        dtype = dots.dtype
-        pre_softmax_attn = dots.clone()
-
-        mask_value = -torch.finfo(dots.dtype).max
-
-        if exists(mask):
-            dots = dots.masked_fill(mask, mask_value)
+        # causal mask
 
         if self.causal:
-            i, j = dots.shape[-2:]
-            causal_mask = torch.ones((i, j), dtype = torch.bool, device = device).triu(j - i + 1)
-            dots = dots.masked_fill(causal_mask, mask_value)
+            causal_mask = self.get_mask(q_len, k_len, device)
+            sim = sim.masked_fill(causal_mask, -torch.finfo(sim.dtype).max)
 
-        attn = self.attn_fn(dots, dim = -1)
-        attn = attn.type(dtype)
-
-        post_softmax_attn = attn.clone()
+        # attention
 
+        attn = sim.softmax(dim=-1)
         attn = self.attn_dropout(attn)
 
-        if self.talking_heads:
-            attn = self.post_softmax_talking_heads(attn)
-
-        out = einsum(f'b h i j, {kv_einsum_eq} -> b h i d', attn, v)
+        # aggregate values
 
-        intermediates = Intermediates(
-            qk_similarities = qk_similarities,
-            pre_softmax_attn = pre_softmax_attn,
-            post_softmax_attn = post_softmax_attn
-        )
-
-        return out, intermediates
+        out = einsum(f"b h i j, {kv_einsum_eq} -> b h i d", attn, v)
 
+        return out
+    
+import torch
+from collections import namedtuple
+from einops import rearrange
 
+EfficientAttentionConfig = namedtuple('EfficientAttentionConfig', ['enable_flash', 'enable_math', 'enable_mem_efficient'])
 
 class FlashMHA(nn.Module):
-    def __init__(
-            self,
-            embed_dim,
-            num_heads,
-            dropout=0.0,
-            device=None,
-            dtype=None
-        ):
-            super().__init__()
-            self.embed_dim = embed_dim
-            self.num_heads = num_heads
-
-            self.head_dim = embed_dim // num_heads
-            self.scaling = self.head_dim**-0.5
-
-            factory_kwargs = {'device': device, 'dtype': dtype}
-
-            self.k_proj = nn.Linear(embed_dim, embed_dim, bias=True, **factory_kwargs)
-            self.v_proj = nn.Linear(embed_dim, embed_dim, bias=True, **factory_kwargs)
-            self.q_proj = nn.Linear(embed_dim, embed_dim, bias=True, **factory_kwargs)
-            self.outproj = nn.Linear(embed_dim, embed_dim, bias=True, **factory_kwargs)
-            
-            self.dropout_module = torch.nn.Dropout(dropout).to(device=device, dtype=dtype)
-
-            # init flash attention
-            self.flash_attention = FlashAttention(dropout=dropout, heads=num_heads, dropout=dropout, device=device, dtype=dtype)
-
-    def reset_parameters(self):
-        nn.init.xavier_uniform_(self.k_proj.weight, gain=1 / math.sqrt(2))
-        nn.init.xavier_uniform_(self.v_proj.weight, gain=1 / math.sqrt(2))
-        nn.init.xavier_uniform_(self.q_proj.weight, gain=1 / math.sqrt(2))
-        nn.init.xavier_uniform_(self.out_proj.weight)
-        nn.init.constant_(self.out_proj.bias, 0.0)
-    
-    def forward(
-            self,
-            query,
-            key,
-            value,
-            mask=None,
-            attn_mask=None,
-            incremental_state=None,
-            is_first_step=False
-        ):
-        # type: (Tensor, Tensor, Tensor, Optional[Tensor], Optional[Tensor], Optional[Dict[str, Tensor]], Optional[bool]) -> Tuple[Tensor, Optional[Tensor]]
-        tgt_len, bsz, embed_dim = query.size()
-
-        assert embed_dim == self.embed_dim
-        assert list(query.size()) == [tgt_len, bsz, embed_dim]
-
-        q = self.q_proj(query)
-        k = self.k_proj(key)
-        v = self.v_proj(value)
-
-        q *= self.scaling
-
-        q = q.view(tgt_len, bsz * self.num_heads, self.head_dim).transpose(0, 1)
-        k = k.view(-1, bsz * self.num_heads, self.head_dim).transpose(0, 1)
-        v = v.view(-1, bsz * self.num_heads, self.head_dim).transpose(0, 1)
-
-        if mask is not None:
-            mask = mask.unsqueeze(1).expand(-1, tgt_len, -1)
-            mask = mask.view(mask.size(0) * self.num_heads, tgt_len, -1)
-        
-        attn_weights, _ = self.flash_attention(q, k, v, mask)
-        assert list(attn_weights.size()) == [bsz * self.num_heads, tgt_len, k.size(1)]
-
-        attn_weights = self.dropout_module(attn_weights)
-        attn = torch.bmm(attn_weights, v)
-        assert list(attn.size()) == [bsz * self.num_heads, tgt_len, self.head_dim]
-        attn = attn.transpose(0, 1).contiguous().view(tgt_len, bsz, embed_dim)
-        attn = self.out_proj(attn)
+    def __init__(self, embed_dim, num_heads, bias=True, batch_first=True, dropout=0.0,
+                 causal=False, device=None, dtype=None) -> None:
+        assert batch_first
+        factory_kwargs = {'device': device, 'dtype': dtype}
+        super().__init__()
+        self.embed_dim = embed_dim
+        self.causal = causal
 
-        return attn, attn_weights
+        self.num_heads = num_heads
+        assert self.embed_dim % num_heads == 0, "self.kdim must be divisible by num_heads"
+        self.head_dim = self.embed_dim // num_heads
+        assert self.head_dim % 8 == 0 and self.head_dim <= 128, "Only support head_dim <= 128 and divisible by 8"
+
+        self.Wqkv = nn.Linear(embed_dim, 3 * embed_dim, bias=bias, **factory_kwargs)
+        self.inner_attn = FlashAttention(dropout=dropout, causal=causal)
+        self.out_proj = nn.Linear(embed_dim, embed_dim, bias=bias, **factory_kwargs)
+
+    def forward(self, query, key, value):
+        qkv = self.Wqkv(query)
+        q, k, v = rearrange(qkv, 'b s (three h d) -> three b s h d', three=3, h=self.num_heads, d=self.head_dim).unbind(dim=0)
+        context = self.inner_attn(q, k, v)
+        return self.out_proj(rearrange(context, 'b s h d -> b s (h d)'))
```

### Comparing `LongNet-0.2.5/LongNet/model.py` & `LongNet-0.2.7/LongNet/model.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/LongNet/training.py` & `LongNet-0.2.7/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/LongNet/utils.py` & `LongNet-0.2.7/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/LongNet.egg-info/PKG-INFO` & `LongNet-0.2.7/LongNet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.2.5
+Version: 0.2.7
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.2.5/LongNet.egg-info/SOURCES.txt` & `LongNet-0.2.7/LongNet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/PKG-INFO` & `LongNet-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.2.5
+Version: 0.2.7
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.2.5/README.md` & `LongNet-0.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Agora
 This implementation of LongNet is brought to you by Agora, we're an all-new open source AI research organization with 1,500+ AI researchers all striving to advance Humanity!
 
 ![Agora banner](agora-banner-water.png)
 
-[Join us and help contribute to LongNet and or recieve support in the Agora discord!](https://discord.gg/qUtxnK2NMf)
+[Join us and help contribute to LongNet and or recieve FAST support in the Agora discord!](https://discord.gg/qUtxnK2NMf)
 
 # LongNet: Scaling Transformers to 1,000,000,000 Tokens
 
-This is an implementation for the paper [LongNet: Scaling Transformers to 1,000,000,000 Tokens](https://arxiv.org/abs/xxx.xxxxx) by Jiayu Ding, Shuming Ma, Li Dong, Xingxing Zhang, Shaohan Huang, Wenhui Wang, Furu Wei. The LongNet is a Transformer variant designed to scale sequence length up to more than 1 billion tokens without sacrificing performance on shorter sequences.
+This is an open source implementation for the paper [LongNet: Scaling Transformers to 1,000,000,000 Tokens](https://arxiv.org/abs/2307.02486) by Jiayu Ding, Shuming Ma, Li Dong, Xingxing Zhang, Shaohan Huang, Wenhui Wang, Furu Wei. The LongNet is a Transformer variant designed to scale sequence length up to more than 1 billion tokens without sacrificing performance on shorter sequences.
 
 ## Introduction
 
 Scaling sequence length has become a critical bottleneck in the era of large language models. However, existing methods struggle with either computational complexity or model expressivity, rendering the maximum sequence length restricted. In this paper, they introduce LongNet, a Transformer variant that can scale sequence length to more than 1 billion tokens, without sacrificing the performance on shorter sequences. Specifically, they propose dilated attention, which expands the attentive field exponentially as the distance grows.
 
 ## Features
 LongNet has significant advantages:
@@ -20,15 +20,15 @@
 3. Its dilated attention is a drop-in replacement for standard attention, which can be seamlessly integrated with the existing Transformer-based optimization.
 
 Experiment results demonstrate that LongNet yields strong performance on both long-sequence modeling and general language tasks. Their work opens up new possibilities for modeling very long sequences, e.g., treating a whole corpus or even the entire Internet as a sequence.
 
 Here's the updated usage and installation section with two methods: git clone or pip install LongNet:
 
 ## Installation
-
+c
 You can install LongNet using one of the following methods:
 
 ### Method 1: Git Clone
 
 1. Clone the LongNet repository from GitHub:
 
 ```shell
@@ -37,33 +37,35 @@
 
 2. Navigate to the cloned directory:
 
 ```shell
 cd LongNet
 ```
 
-3. Install the required dependencies:
+3. Prepare `flash_attn` library
 
-```shell
-pip install -r requirements.txt
-```
+```bash
 
-4. Then Install dependencies for flash_attn
+cd flash_attn
 
-* `cd flash_attn`
+python setup.py install
 
-* `python setup.py install`
+cd ..
 
-* `cd ..`
+```
 
-* `python3 example.py`
+4. Install the required dependencies:
+
+```shell
+pip install -r requirements.txt
+```
 
 
 ### Method 2: Pip Install
-* Note that pip install does not work as the `flash-attn` library cannot be compiled since it has custom CUDA Kernels.
+* Note that pip install does not work as the `flash-attn` library cannot be compiled since it has custom CUDA Kernels and they need to be built manually.
 
 1. Install LongNet directly from PyPI using pip:
 
 ```shell
 pip install LongNet
 ```
 
@@ -133,14 +135,25 @@
 ```
 
 In the example above, we create an instance of the `DilatedAttention` class with the specified hyperparameters. We then generate some dummy input data and pass it through the attention mechanism to obtain the outputs. Finally, we print the shape of the output tensor.
 
 
 # DilatedAttention Documentation
 
+## Algorithmic Psueodocode:
+```
+1. Initialize the input (Q, K, V) and split them into segments {(Qei, Kei, Vei)} with equal segment length w.
+2. Sparsify each segment along the sequence dimension by selecting the rows with an interval r.
+3. Feed the sparsified segments into the attention in parallel.
+4. Scatter and concatenate the output O from the attention.
+5. Implement a mixture of dilated attentions with different segment sizes and dilation rates {ri, wi}.
+6. For multi-head dilated attention, differ the computation among different heads by sparsifying different parts of the query-key-value pairs.
+7. Concatenate the outputs of different heads into a final output.
+```
+
 
 ## Class Definition
 
 ```python
 class DilatedAttention(nn.Module):
     def __init__(self, d_model, num_heads, dilation_rate, segment_size, dropout=0.0, causal=False, use_xpos=False, use_rel_pos_bias=False ):
         ...
@@ -284,34 +297,22 @@
 [Share LongNet Repository](https://github.com/kyegomez/LongNet)
 
 
 
 
 # Roadmap
 
-* Test and evaluate
-
-* And, create an interation of `DilatedAttention` `FlashBlocksparseMHA`
-
-* Integrate Model, tokenizer, and train function without file path
+* Test and evaluate and patch.
 
-* Create a benchmarking suite against other attentions
+* And, create an interation of `DilatedAttention` with `FlashBlocksparseMHA`
 
-* Add unit testing for `DilationAttention`
-
-* Create a multi-modal `DilationAttention` with multiway, sub layernorm, and xpos?
+* Create a multi-modal `DilationAttention` with multiway, sub layernorm, and xpos, sub layernorm, QK Layernorm, One write query head maybe
 
 * Integrate Alibi and xpos for even further ridicoulus length extrapolation
 
-* Create a multi-modality verison with sub layer norm
-
-* Integrate QK Layernorm
-
-* Integrate One write query head maybe
-
 * Recreate in Triton or Jax for ultra mega speed boost
 
 
 ## Citation
 ```
 @inproceedings{ding2023longnet,
   title={LongNet: Scaling Transformers to 1,000,000,000 Tokens},
```

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/bert_padding.py` & `LongNet-0.2.7/flash_attn/flash_attn/bert_padding.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/flash_attention.py` & `LongNet-0.2.7/flash_attn/flash_attn/flash_attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/flash_attn_interface.py` & `LongNet-0.2.7/flash_attn/flash_attn/flash_attn_interface.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/flash_attn_triton.py` & `LongNet-0.2.7/flash_attn/flash_attn/flash_attn_triton.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/flash_attn_triton_og.py` & `LongNet-0.2.7/flash_attn/flash_attn/flash_attn_triton_og.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/flash_blocksparse_attention.py` & `LongNet-0.2.7/flash_attn/flash_attn/flash_blocksparse_attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/flash_blocksparse_attn_interface.py` & `LongNet-0.2.7/flash_attn/flash_attn/flash_blocksparse_attn_interface.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/fused_softmax.py` & `LongNet-0.2.7/flash_attn/flash_attn/fused_softmax.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/layers/patch_embed.py` & `LongNet-0.2.7/flash_attn/flash_attn/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/layers/rotary.py` & `LongNet-0.2.7/flash_attn/flash_attn/layers/rotary.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/losses/cross_entropy.py` & `LongNet-0.2.7/flash_attn/flash_attn/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/models/bert.py` & `LongNet-0.2.7/flash_attn/flash_attn/models/bert.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/models/gpt.py` & `LongNet-0.2.7/flash_attn/flash_attn/models/gpt.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/models/gpt_neox.py` & `LongNet-0.2.7/flash_attn/flash_attn/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/models/gptj.py` & `LongNet-0.2.7/flash_attn/flash_attn/models/gptj.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/models/llama.py` & `LongNet-0.2.7/flash_attn/flash_attn/models/llama.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/models/opt.py` & `LongNet-0.2.7/flash_attn/flash_attn/models/opt.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/models/vit.py` & `LongNet-0.2.7/flash_attn/flash_attn/models/vit.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/modules/block.py` & `LongNet-0.2.7/flash_attn/flash_attn/modules/block.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/modules/embedding.py` & `LongNet-0.2.7/flash_attn/flash_attn/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/modules/mha.py` & `LongNet-0.2.7/flash_attn/flash_attn/modules/mha.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/modules/mlp.py` & `LongNet-0.2.7/flash_attn/flash_attn/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/ops/activations.py` & `LongNet-0.2.7/flash_attn/flash_attn/ops/activations.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/ops/fused_dense.py` & `LongNet-0.2.7/flash_attn/flash_attn/ops/fused_dense.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/ops/layer_norm.py` & `LongNet-0.2.7/flash_attn/flash_attn/ops/layer_norm.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/ops/rms_norm.py` & `LongNet-0.2.7/flash_attn/flash_attn/ops/rms_norm.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/utils/benchmark.py` & `LongNet-0.2.7/flash_attn/flash_attn/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/utils/distributed.py` & `LongNet-0.2.7/flash_attn/flash_attn/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/utils/generation.py` & `LongNet-0.2.7/flash_attn/flash_attn/utils/generation.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/flash_attn/utils/pretrained.py` & `LongNet-0.2.7/flash_attn/flash_attn/utils/pretrained.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/flash_attn/setup.py` & `LongNet-0.2.7/flash_attn/setup.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.5/setup.py` & `LongNet-0.2.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.2.5',
+  version = '0.2.7',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

### Comparing `LongNet-0.2.5/test/test.py` & `LongNet-0.2.7/test/test.py`

 * *Files identical despite different names*


# Comparing `tmp/LongNet-0.2.7.tar.gz` & `tmp/LongNet-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.2.7.tar", last modified: Wed Jul 12 17:54:57 2023, max compression
+gzip compressed data, was "LongNet-0.2.9.tar", last modified: Wed Jul 12 18:26:05 2023, max compression
```

## Comparing `LongNet-0.2.7.tar` & `LongNet-0.2.9.tar`

### file list

```diff
@@ -1,68 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.616438 LongNet-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 17:54:41.000000 LongNet-0.2.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.600437 LongNet-0.2.7/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-12 17:54:41.000000 LongNet-0.2.7/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-12 17:54:41.000000 LongNet-0.2.7/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-12 17:54:41.000000 LongNet-0.2.7/LongNet/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-12 17:54:41.000000 LongNet-0.2.7/LongNet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-12 17:54:41.000000 LongNet-0.2.7/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-12 17:54:41.000000 LongNet-0.2.7/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.600437 LongNet-0.2.7/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 17:54:57.000000 LongNet-0.2.7/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-12 17:54:57.000000 LongNet-0.2.7/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:54:57.000000 LongNet-0.2.7/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 17:54:57.000000 LongNet-0.2.7/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 17:54:57.000000 LongNet-0.2.7/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 17:54:57.616438 LongNet-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-07-12 17:54:41.000000 LongNet-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.600437 LongNet-0.2.7/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.604438 LongNet-0.2.7/flash_attn/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/bert_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/flash_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/flash_attn_triton.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/flash_attn_triton_og.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/flash_blocksparse_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/flash_blocksparse_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/fused_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.608438 LongNet-0.2.7/flash_attn/flash_attn/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/layers/patch_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/layers/rotary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.608438 LongNet-0.2.7/flash_attn/flash_attn/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/losses/cross_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.608438 LongNet-0.2.7/flash_attn/flash_attn/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/gpt_neox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/gptj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/models/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.612438 LongNet-0.2.7/flash_attn/flash_attn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/modules/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/modules/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/modules/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.612438 LongNet-0.2.7/flash_attn/flash_attn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/ops/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/ops/fused_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    19306 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/ops/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/ops/rms_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.616438 LongNet-0.2.7/flash_attn/flash_attn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/utils/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/utils/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/flash_attn/utils/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-12 17:54:41.000000 LongNet-0.2.7/flash_attn/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:54:57.616438 LongNet-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 17:54:41.000000 LongNet-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:54:57.616438 LongNet-0.2.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 17:54:41.000000 LongNet-0.2.7/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.557095 LongNet-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 18:25:48.000000 LongNet-0.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.541095 LongNet-0.2.9/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.541095 LongNet-0.2.9/LongNet/torchscale/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.541095 LongNet-0.2.9/LongNet/torchscale/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/criterions/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/criterions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/criterions/masked_lm_moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18556 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/models/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/models/language_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22559 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/models/machine_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/data/basic_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/data/mlm_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/pretraining.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/utils/sparse_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/tests/test_encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/torchscale/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.549095 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.549095 LongNet-0.2.9/LongNet/torchscale/torchscale/component/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/droppath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/feedforward_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/multiway_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/relative_position_bias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.549095 LongNet-0.2.9/LongNet/torchscale/torchscale/component/xmoe/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/xmoe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/xmoe/global_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/xmoe/moe_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/xmoe/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/xpos_relative_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.549095 LongNet-0.2.9/LongNet/torchscale/torchscale/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/model/BEiT3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.541095 LongNet-0.2.9/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 18:26:05.000000 LongNet-0.2.9/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-12 18:26:05.000000 LongNet-0.2.9/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:26:05.000000 LongNet-0.2.9/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 18:26:05.000000 LongNet-0.2.9/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 18:26:05.000000 LongNet-0.2.9/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 18:26:05.557095 LongNet-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-07-12 18:25:48.000000 LongNet-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.549095 LongNet-0.2.9/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.553095 LongNet-0.2.9/flash_attn/flash_attn/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/bert_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/flash_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/flash_attn_triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/flash_attn_triton_og.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/flash_blocksparse_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/flash_blocksparse_attn_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/fused_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.553095 LongNet-0.2.9/flash_attn/flash_attn/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/layers/patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/layers/rotary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.553095 LongNet-0.2.9/flash_attn/flash_attn/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/losses/cross_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.557095 LongNet-0.2.9/flash_attn/flash_attn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/gpt_neox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/gptj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.557095 LongNet-0.2.9/flash_attn/flash_attn/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/modules/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/modules/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/modules/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/modules/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.557095 LongNet-0.2.9/flash_attn/flash_attn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/ops/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/ops/fused_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19306 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/ops/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/ops/rms_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.557095 LongNet-0.2.9/flash_attn/flash_attn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/utils/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/utils/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:26:05.557095 LongNet-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 18:25:48.000000 LongNet-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.557095 LongNet-0.2.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 18:25:48.000000 LongNet-0.2.9/test/test.py
```

### Comparing `LongNet-0.2.7/LICENSE` & `LongNet-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/LongNet/attend.py` & `LongNet-0.2.9/LongNet/attend.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/LongNet/attention.py` & `LongNet-0.2.9/LongNet/attention.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,117 @@
 import torch 
 import torch.nn as nn
 import torch.nn.functional as F
 
-from torchscale.torchscale.component.xpos_relative_position import XPOS
-from torchscale.torchscale.component.relative_position_bias import RelativePositionBias
+# from torchscale.component.xpos_relative_position import XPOS
+# from torchscale.component.relative_position_bias import RelativePositionBias
 
+from torchscale import XPOS, RelativePositionBias
 
 from LongNet.attend import FlashMHA
 
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
 
 
+#
 
 
-#second iteration the weighted sum of the different dilated + offsets for the different heads
+# Define the attention module
 class DilatedAttention(nn.Module):
     def __init__(self, d_model, num_heads, dilation_rate, segment_size, dropout=0.0, casual=False, use_xpos=False, use_rel_pos_bias=False):
         super(DilatedAttention, self).__init__()
-        self.d_model = d_model
-        self.num_heads = num_heads
-
-        self.dilation_rate = dilation_rate
-        self.segment_size = segment_size
+        
+        # Initialize parameters
+        self.d_model = d_model               # model dimension
+        self.num_heads = num_heads           # number of attention heads
+        self.dilation_rate = dilation_rate   # dilation rate
+        self.segment_size = segment_size     # segment size
 
+        # Initialize attention for each head with dilation
         self.attentions = nn.ModuleList([FlashMHA(embed_dim=d_model, num_heads=num_heads, device=device, dtype=dtype) for _ in range(self.dilation_rate)])
+
+        # Initialize dropout layer
         self.dropout = nn.Dropout(dropout)
+        
+        # If casual attention is used
         self.casual = casual
 
+        # If using positional encoding
         self.use_xpos = use_xpos
+
+        # If using relative positional bias
         self.use_rel_pos_bias = use_rel_pos_bias
 
+        # If using positional encoding, initialize it
         if use_xpos:
             self.xpos = XPOS(head_dim=d_model//num_heads)
+
+        # If using relative positional bias, initialize it
         if use_rel_pos_bias:
             self.relative_bias = RelativePositionBias(num_buckets=32, max_distance=128, n_heads=num_heads)
 
+        # Initialize softmax for later use in weights
         self.softmax = nn.Softmax(dim=-1)
 
+    # Function to get mask for casual attention
     def get_mask(self, i, j):
         return torch.ones((i, j), device=device, dtype=torch.bool).triu(j - i + 2)
 
+    # Forward function
     def forward(self, x):
+        # Get batch size, sequence length and model dimension
         batch_size, seq_len, _ = x.shape
 
+        # If using positional encoding, add it
         if self.use_xpos:
             x = self.xpos(x)
 
-        #collect outputs from each attention head
+        # Initialize list to store outputs from each attention head
         all_head_outputs = []
+        
+        # For each attention head
         for head_idx, attention in enumerate(self.attentions):
+            # Calculate offset for this head
             offset = head_idx % self.dilation_rate
 
-            x_ = x[:, offset::self.dilation_rate, :]  # Apply offset for each head
+            # Apply offset and segment for this head
+            x_ = x[:, offset::self.dilation_rate, :]
             x_ = x_.contiguous().view(batch_size, -1, self.segment_size, self.d_model)
 
+            # Pass through attention
             attn_output, _ = attention(x_, x_, x_)
+            
+            # If using relative positional bias, add it
             if self.use_rel_pos_bias:
                 attn_output += self.relative_bias(batch_size, attn_output.size(1), attn_output.size(1))
 
+            # If using casual attention, apply mask
             if self.casual:
                 mask = self.get_mask(attn_output.size(1), attn_output.size(1))
                 attn_output = attn_output.masked_fill(mask, float('-inf'))
 
+            # Apply dropout
             attn_output = self.dropout(attn_output)
 
-            #resize back to original size
+            # Resize back to original size
             attn_output_resized = torch.zeros((batch_size, seq_len, self.d_model), device=device, dtype=dtype)
             attn_output_resized[:, offset::self.dilation_rate, :] = attn_output.contiguous().view(batch_size, -1, self.d_model)
             
+            # Append output to list of all outputs
             all_head_outputs.append(attn_output_resized)
 
-        #calculate the weights for the different dilated attentions
+        # Calculate the weights for the different dilated attentions
         weights = self.softmax(torch.tensor([1.0 / self.dilation_rate for _ in range(self.dilation_rate)], device=device, dtype=dtype))
 
-        #apply the weights to the outputs of the different heads
+        # Apply the weights to the outputs of the different heads
         outputs_weighted = sum(w * out for w, out in zip(weights, all_head_outputs))
 
+        # Return the weighted outputs
         return outputs_weighted
```

### Comparing `LongNet-0.2.7/LongNet/model.py` & `LongNet-0.2.9/LongNet/model.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/LongNet/training.py` & `LongNet-0.2.9/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/LongNet/utils.py` & `LongNet-0.2.9/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/LongNet.egg-info/PKG-INFO` & `LongNet-0.2.9/LongNet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.2.7
+Version: 0.2.9
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.2.7/PKG-INFO` & `LongNet-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.2.7
+Version: 0.2.9
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.2.7/README.md` & `LongNet-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/bert_padding.py` & `LongNet-0.2.9/flash_attn/flash_attn/bert_padding.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/flash_attention.py` & `LongNet-0.2.9/flash_attn/flash_attn/flash_attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/flash_attn_interface.py` & `LongNet-0.2.9/flash_attn/flash_attn/flash_attn_interface.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/flash_attn_triton.py` & `LongNet-0.2.9/flash_attn/flash_attn/flash_attn_triton.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/flash_attn_triton_og.py` & `LongNet-0.2.9/flash_attn/flash_attn/flash_attn_triton_og.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/flash_blocksparse_attention.py` & `LongNet-0.2.9/flash_attn/flash_attn/flash_blocksparse_attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/flash_blocksparse_attn_interface.py` & `LongNet-0.2.9/flash_attn/flash_attn/flash_blocksparse_attn_interface.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/fused_softmax.py` & `LongNet-0.2.9/flash_attn/flash_attn/fused_softmax.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/layers/patch_embed.py` & `LongNet-0.2.9/flash_attn/flash_attn/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/layers/rotary.py` & `LongNet-0.2.9/flash_attn/flash_attn/layers/rotary.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/losses/cross_entropy.py` & `LongNet-0.2.9/flash_attn/flash_attn/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/models/bert.py` & `LongNet-0.2.9/flash_attn/flash_attn/models/bert.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/models/gpt.py` & `LongNet-0.2.9/flash_attn/flash_attn/models/gpt.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/models/gpt_neox.py` & `LongNet-0.2.9/flash_attn/flash_attn/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/models/gptj.py` & `LongNet-0.2.9/flash_attn/flash_attn/models/gptj.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/models/llama.py` & `LongNet-0.2.9/flash_attn/flash_attn/models/llama.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/models/opt.py` & `LongNet-0.2.9/flash_attn/flash_attn/models/opt.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/models/vit.py` & `LongNet-0.2.9/flash_attn/flash_attn/models/vit.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/modules/block.py` & `LongNet-0.2.9/flash_attn/flash_attn/modules/block.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/modules/embedding.py` & `LongNet-0.2.9/flash_attn/flash_attn/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/modules/mha.py` & `LongNet-0.2.9/flash_attn/flash_attn/modules/mha.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/modules/mlp.py` & `LongNet-0.2.9/flash_attn/flash_attn/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/ops/activations.py` & `LongNet-0.2.9/flash_attn/flash_attn/ops/activations.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/ops/fused_dense.py` & `LongNet-0.2.9/flash_attn/flash_attn/ops/fused_dense.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/ops/layer_norm.py` & `LongNet-0.2.9/flash_attn/flash_attn/ops/layer_norm.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/ops/rms_norm.py` & `LongNet-0.2.9/flash_attn/flash_attn/ops/rms_norm.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/utils/benchmark.py` & `LongNet-0.2.9/flash_attn/flash_attn/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/utils/distributed.py` & `LongNet-0.2.9/flash_attn/flash_attn/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/utils/generation.py` & `LongNet-0.2.9/flash_attn/flash_attn/utils/generation.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/flash_attn/utils/pretrained.py` & `LongNet-0.2.9/flash_attn/flash_attn/utils/pretrained.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/flash_attn/setup.py` & `LongNet-0.2.9/flash_attn/setup.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.7/setup.py` & `LongNet-0.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.2.7',
+  version = '0.2.9',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

### Comparing `LongNet-0.2.7/test/test.py` & `LongNet-0.2.9/test/test.py`

 * *Files identical despite different names*


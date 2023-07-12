# Comparing `tmp/LongNet-0.2.9.tar.gz` & `tmp/LongNet-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.2.9.tar", last modified: Wed Jul 12 18:26:05 2023, max compression
+gzip compressed data, was "LongNet-0.3.0.tar", last modified: Wed Jul 12 18:55:04 2023, max compression
```

## Comparing `LongNet-0.2.9.tar` & `LongNet-0.3.0.tar`

### file list

```diff
@@ -1,128 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.557095 LongNet-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 18:25:48.000000 LongNet-0.2.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.541095 LongNet-0.2.9/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.541095 LongNet-0.2.9/LongNet/torchscale/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.541095 LongNet-0.2.9/LongNet/torchscale/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/criterions/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/criterions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/criterions/masked_lm_moe.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18556 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/models/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/models/language_modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)    22559 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/models/machine_translation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/data/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/data/basic_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/data/mlm_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/tasks/pretraining.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/examples/fairseq/utils/sparse_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/tests/test_encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.545095 LongNet-0.2.9/LongNet/torchscale/torchscale/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.549095 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/architecture/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.549095 LongNet-0.2.9/LongNet/torchscale/torchscale/component/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/droppath.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/feedforward_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/multiway_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/relative_position_bias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.549095 LongNet-0.2.9/LongNet/torchscale/torchscale/component/xmoe/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/xmoe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/xmoe/global_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/xmoe/moe_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/xmoe/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/component/xpos_relative_position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.549095 LongNet-0.2.9/LongNet/torchscale/torchscale/model/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/model/BEiT3.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/torchscale/torchscale/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-12 18:25:48.000000 LongNet-0.2.9/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.541095 LongNet-0.2.9/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 18:26:05.000000 LongNet-0.2.9/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-12 18:26:05.000000 LongNet-0.2.9/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:26:05.000000 LongNet-0.2.9/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 18:26:05.000000 LongNet-0.2.9/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 18:26:05.000000 LongNet-0.2.9/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 18:26:05.557095 LongNet-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-07-12 18:25:48.000000 LongNet-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.549095 LongNet-0.2.9/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.553095 LongNet-0.2.9/flash_attn/flash_attn/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/bert_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    20510 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/flash_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    38148 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/flash_attn_triton.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/flash_attn_triton_og.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/flash_blocksparse_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/flash_blocksparse_attn_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/fused_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.553095 LongNet-0.2.9/flash_attn/flash_attn/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/layers/patch_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/layers/rotary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.553095 LongNet-0.2.9/flash_attn/flash_attn/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/losses/cross_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.557095 LongNet-0.2.9/flash_attn/flash_attn/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26570 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/gpt_neox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/gptj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/models/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.557095 LongNet-0.2.9/flash_attn/flash_attn/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/modules/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/modules/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34955 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/modules/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/modules/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.557095 LongNet-0.2.9/flash_attn/flash_attn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/ops/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    26087 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/ops/fused_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    19306 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/ops/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/ops/rms_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.557095 LongNet-0.2.9/flash_attn/flash_attn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/utils/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/utils/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/flash_attn/utils/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-12 18:25:48.000000 LongNet-0.2.9/flash_attn/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:26:05.557095 LongNet-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 18:25:48.000000 LongNet-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:26:05.557095 LongNet-0.2.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 18:25:48.000000 LongNet-0.2.9/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:55:04.102929 LongNet-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 18:54:48.000000 LongNet-0.3.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:55:04.098929 LongNet-0.3.0/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-12 18:54:48.000000 LongNet-0.3.0/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-07-12 18:54:48.000000 LongNet-0.3.0/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-12 18:54:48.000000 LongNet-0.3.0/LongNet/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-12 18:54:48.000000 LongNet-0.3.0/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-12 18:54:48.000000 LongNet-0.3.0/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-12 18:54:48.000000 LongNet-0.3.0/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:55:04.098929 LongNet-0.3.0/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 18:55:04.000000 LongNet-0.3.0/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-12 18:55:04.000000 LongNet-0.3.0/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:55:04.000000 LongNet-0.3.0/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 18:55:04.000000 LongNet-0.3.0/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 18:55:04.000000 LongNet-0.3.0/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-12 18:55:04.102929 LongNet-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14309 2023-07-12 18:54:48.000000 LongNet-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:55:04.102929 LongNet-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-12 18:54:48.000000 LongNet-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:55:04.098929 LongNet-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-12 18:54:48.000000 LongNet-0.3.0/test/test.py
```

### Comparing `LongNet-0.2.9/LICENSE` & `LongNet-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.9/LongNet/attend.py` & `LongNet-0.3.0/LongNet/attend.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.9/LongNet/attention.py` & `LongNet-0.3.0/LongNet/attention.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 import torch 
 import torch.nn as nn
 import torch.nn.functional as F
 
-# from torchscale.component.xpos_relative_position import XPOS
-# from torchscale.component.relative_position_bias import RelativePositionBias
-
-from torchscale import XPOS, RelativePositionBias
+from LongNet.utils import XPOS, RelativePositionBias
 
 from LongNet.attend import FlashMHA
 
-# Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
 
 
-#
-
 
 # Define the attention module
 class DilatedAttention(nn.Module):
     def __init__(self, d_model, num_heads, dilation_rate, segment_size, dropout=0.0, casual=False, use_xpos=False, use_rel_pos_bias=False):
         super(DilatedAttention, self).__init__()
         
         # Initialize parameters
```

### Comparing `LongNet-0.2.9/LongNet/model.py` & `LongNet-0.3.0/LongNet/model.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.9/LongNet/training.py` & `LongNet-0.3.0/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.9/LongNet.egg-info/PKG-INFO` & `LongNet-0.3.0/LongNet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.2.9
+Version: 0.3.0
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.2.9/PKG-INFO` & `LongNet-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.2.9
+Version: 0.3.0
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.2.9/README.md` & `LongNet-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `LongNet-0.2.9/setup.py` & `LongNet-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.2.9',
+  version = '0.3.0',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

### Comparing `LongNet-0.2.9/test/test.py` & `LongNet-0.3.0/test/test.py`

 * *Files identical despite different names*


# Comparing `tmp/fuxictr-2.0.2.tar.gz` & `tmp/fuxictr-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuxictr-2.0.2.tar", last modified: Sun May 14 08:27:02 2023, max compression
+gzip compressed data, was "dist/fuxictr-2.0.3.tar", last modified: Wed Jul 12 07:12:56 2023, max compression
```

## Comparing `fuxictr-2.0.2.tar` & `fuxictr-2.0.3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    29709 2023-05-14 08:27:02.000000 fuxictr-2.0.2/PKG-INFO
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    27403 2023-05-14 08:13:39.000000 fuxictr-2.0.2/README.md
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:01.000000 fuxictr-2.0.2/fuxictr/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       32 2022-11-14 09:29:53.000000 fuxictr-2.0.2/fuxictr/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6557 2023-05-11 07:17:04.000000 fuxictr-2.0.2/fuxictr/autotuner.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/datasets/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       64 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/datasets/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1592 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/datasets/avazu.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1231 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/datasets/criteo.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1826 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/datasets/kkbox.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5503 2023-02-17 01:18:00.000000 fuxictr-2.0.2/fuxictr/features.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4369 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/metrics.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/preprocess/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       62 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/preprocess/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5950 2023-02-14 09:50:19.000000 fuxictr-2.0.2/fuxictr/preprocess/build_dataset.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    18559 2023-02-14 07:01:51.000000 fuxictr-2.0.2/fuxictr/preprocess/feature_processor.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9373 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/preprocess/utils.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2021-08-10 06:39:20.000000 fuxictr-2.0.2/fuxictr/pytorch/__init__.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/dataloaders/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       91 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/dataloaders/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5429 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/dataloaders/h5_block_dataloader.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3907 2023-02-14 07:16:49.000000 fuxictr-2.0.2/fuxictr/pytorch/dataloaders/h5_dataloader.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      164 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1463 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/activations.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      108 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1810 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/dot_product_attention.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1750 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5616 2023-02-14 09:15:25.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/target_attention.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      100 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1416 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/factorization_machine.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1489 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/logistic_regression.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2797 2023-05-14 00:04:17.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/mlp_block.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/embeddings/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       36 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/embeddings/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11489 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/embeddings/feature_embedding.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      244 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4734 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2303 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5228 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/cross_net.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2940 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/holographic_interaction.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2924 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/inner_product.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2780 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/interaction_machine.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1820 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/layers/pooling.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/pytorch/models/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       77 2023-05-14 00:00:11.000000 fuxictr-2.0.2/fuxictr/pytorch/models/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    12709 2023-02-14 07:18:08.000000 fuxictr-2.0.2/fuxictr/pytorch/models/ctr_model.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6182 2023-04-18 04:15:15.000000 fuxictr-2.0.2/fuxictr/pytorch/models/multitask_model.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5363 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/pytorch/torch_utils.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/__init__.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/dataloaders/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       45 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/dataloaders/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3344 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/dataloaders/tf_dataloader.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      107 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/__init__.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      123 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1482 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/factorization_machine.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1517 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/linear.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1673 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/logistic_regression.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3619 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/mlp_block.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/embeddings/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       36 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/embeddings/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11853 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/interactions/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       58 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/interactions/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2088 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/interactions/cross_net.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2969 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/interactions/inner_product.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1065 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/layers/pooling.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr/tensorflow/models/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       32 2023-05-14 00:02:55.000000 fuxictr-2.0.2/fuxictr/tensorflow/models/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9272 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/models/ctr_model.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2713 2023-01-27 08:57:12.000000 fuxictr-2.0.2/fuxictr/tensorflow/tf_utils.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4649 2023-02-15 05:02:33.000000 fuxictr-2.0.2/fuxictr/utils.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       23 2023-05-14 08:25:19.000000 fuxictr-2.0.2/fuxictr/version.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/fuxictr.egg-info/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    29709 2023-05-14 08:27:01.000000 fuxictr-2.0.2/fuxictr.egg-info/PKG-INFO
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2726 2023-05-14 08:27:01.000000 fuxictr-2.0.2/fuxictr.egg-info/SOURCES.txt
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        1 2023-05-14 08:27:01.000000 fuxictr-2.0.2/fuxictr.egg-info/dependency_links.txt
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       48 2023-05-14 08:27:01.000000 fuxictr-2.0.2/fuxictr.egg-info/requires.txt
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       18 2023-05-14 08:27:01.000000 fuxictr-2.0.2/fuxictr.egg-info/top_level.txt
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/model_zoo/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1399 2023-04-18 04:15:15.000000 fuxictr-2.0.2/model_zoo/__init__.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-14 08:27:02.000000 fuxictr-2.0.2/model_zoo/multitask/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       69 2023-04-18 04:15:15.000000 fuxictr-2.0.2/model_zoo/multitask/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       38 2023-05-14 08:27:02.000000 fuxictr-2.0.2/setup.cfg
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1551 2023-05-14 08:25:35.000000 fuxictr-2.0.2/setup.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:56.000000 fuxictr-2.0.3/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    29106 2023-07-12 07:12:56.000000 fuxictr-2.0.3/PKG-INFO
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    26784 2023-06-22 09:06:24.000000 fuxictr-2.0.3/README.md
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:54.000000 fuxictr-2.0.3/fuxictr/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       32 2022-11-14 09:29:53.000000 fuxictr-2.0.3/fuxictr/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6557 2023-05-28 13:18:32.000000 fuxictr-2.0.3/fuxictr/autotuner.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:54.000000 fuxictr-2.0.3/fuxictr/datasets/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       64 2023-05-16 14:41:26.000000 fuxictr-2.0.3/fuxictr/datasets/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1592 2023-05-16 14:41:36.000000 fuxictr-2.0.3/fuxictr/datasets/avazu.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1231 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/datasets/criteo.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1826 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/datasets/kkbox.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5503 2023-02-17 01:18:00.000000 fuxictr-2.0.3/fuxictr/features.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4369 2023-05-26 10:25:02.000000 fuxictr-2.0.3/fuxictr/metrics.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:54.000000 fuxictr-2.0.3/fuxictr/preprocess/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       62 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/preprocess/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5950 2023-02-14 09:50:19.000000 fuxictr-2.0.3/fuxictr/preprocess/build_dataset.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    18559 2023-02-14 07:01:51.000000 fuxictr-2.0.3/fuxictr/preprocess/feature_processor.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9373 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/preprocess/utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:54.000000 fuxictr-2.0.3/fuxictr/pytorch/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2021-08-10 06:39:20.000000 fuxictr-2.0.3/fuxictr/pytorch/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:54.000000 fuxictr-2.0.3/fuxictr/pytorch/dataloaders/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       91 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/dataloaders/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5429 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/dataloaders/h5_block_dataloader.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3907 2023-02-14 07:16:49.000000 fuxictr-2.0.3/fuxictr/pytorch/dataloaders/h5_dataloader.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:54.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      164 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1463 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/activations.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:55.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/attentions/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      108 2023-05-31 09:23:26.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/attentions/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1810 2023-05-31 09:23:26.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/attentions/dot_product_attention.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1750 2023-05-31 09:23:26.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5616 2023-05-31 09:23:26.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/attentions/target_attention.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:55.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/blocks/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      100 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/blocks/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1416 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/blocks/factorization_machine.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1489 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/blocks/logistic_regression.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2740 2023-05-19 04:47:42.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/blocks/mlp_block.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:55.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/embeddings/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       36 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/embeddings/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11574 2023-05-26 06:43:32.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/embeddings/feature_embedding.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:55.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      244 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4734 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2303 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5228 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/cross_net.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2940 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/holographic_interaction.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2924 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/inner_product.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2780 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/interaction_machine.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1820 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/layers/pooling.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:55.000000 fuxictr-2.0.3/fuxictr/pytorch/models/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       78 2023-06-06 11:51:39.000000 fuxictr-2.0.3/fuxictr/pytorch/models/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6182 2023-04-18 04:15:15.000000 fuxictr-2.0.3/fuxictr/pytorch/models/multitask_model.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    12678 2023-06-06 11:55:17.000000 fuxictr-2.0.3/fuxictr/pytorch/models/rank_model.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5363 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/pytorch/torch_utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:55.000000 fuxictr-2.0.3/fuxictr/tensorflow/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:55.000000 fuxictr-2.0.3/fuxictr/tensorflow/dataloaders/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       45 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/dataloaders/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3344 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/dataloaders/tf_dataloader.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:55.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      107 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:55.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/blocks/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      123 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/blocks/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1482 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/blocks/factorization_machine.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1517 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/blocks/linear.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1673 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/blocks/logistic_regression.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3619 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/blocks/mlp_block.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:55.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/embeddings/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       36 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/embeddings/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11938 2023-05-26 06:50:13.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:56.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/interactions/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       58 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/interactions/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2088 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/interactions/cross_net.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2969 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/interactions/inner_product.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1065 2023-01-27 08:57:12.000000 fuxictr-2.0.3/fuxictr/tensorflow/layers/pooling.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:56.000000 fuxictr-2.0.3/fuxictr/tensorflow/models/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       33 2023-05-19 02:03:38.000000 fuxictr-2.0.3/fuxictr/tensorflow/models/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9279 2023-06-08 01:29:48.000000 fuxictr-2.0.3/fuxictr/tensorflow/models/rank_model.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2730 2023-05-19 02:30:53.000000 fuxictr-2.0.3/fuxictr/tensorflow/tf_utils.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4649 2023-02-15 05:02:33.000000 fuxictr-2.0.3/fuxictr/utils.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       21 2023-07-12 07:11:26.000000 fuxictr-2.0.3/fuxictr/version.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:54.000000 fuxictr-2.0.3/fuxictr.egg-info/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    29106 2023-07-12 07:12:52.000000 fuxictr-2.0.3/fuxictr.egg-info/PKG-INFO
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2728 2023-07-12 07:12:52.000000 fuxictr-2.0.3/fuxictr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        1 2023-07-12 07:12:52.000000 fuxictr-2.0.3/fuxictr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       48 2023-07-12 07:12:52.000000 fuxictr-2.0.3/fuxictr.egg-info/requires.txt
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       18 2023-07-12 07:12:52.000000 fuxictr-2.0.3/fuxictr.egg-info/top_level.txt
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:56.000000 fuxictr-2.0.3/model_zoo/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1420 2023-06-08 03:05:12.000000 fuxictr-2.0.3/model_zoo/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-07-12 07:12:56.000000 fuxictr-2.0.3/model_zoo/multitask/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       69 2023-04-18 04:15:15.000000 fuxictr-2.0.3/model_zoo/multitask/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       38 2023-07-12 07:12:56.000000 fuxictr-2.0.3/setup.cfg
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1551 2023-07-12 07:11:06.000000 fuxictr-2.0.3/setup.py
```

### Comparing `fuxictr-2.0.2/PKG-INFO` & `fuxictr-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.0.2
+Version: 2.0.3
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/xue-pai/FuxiCTR
 Author: zhujiem
 Author-email: zhujiem@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/xue-pai/FuxiCTR/tags
 Description: <div align="center">
@@ -14,15 +14,14 @@
         <div align="center">
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/python-3.6+-blue" style="max-width: 100%;" alt="Python version"></a>
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/pytorch-1.10+-blue" style="max-width: 100%;" alt="Pytorch version"></a>
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/tensorflow-2.1+-blue" style="max-width: 100%;" alt="Pytorch version"></a>
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/pypi/v/fuxictr.svg" style="max-width: 100%;" alt="Pypi version"></a>
         <a href="https://pepy.tech/project/fuxictr"><img src="https://pepy.tech/badge/fuxictr" style="max-width: 100%;" alt="Downloads"></a>
         <a href="https://github.com/xue-pai/FuxiCTR/blob/main/LICENSE"><img src="https://img.shields.io/github/license/xue-pai/fuxictr.svg" style="max-width: 100%;" alt="License"></a>
-        <a href="https://fuxictr.github.io/tutorials"><img src="https://img.shields.io/badge/tutorials-passing-brightgreen?style=flat" style="max-width: 100%;" alt="Wechat QR code"></a>
         </div>
         <hr/>
         
         <div align="center">
         <a href="https://github.com/xue-pai/FuxiCTR/stargazers"><img src="https://reporoster.com/stars/xue-pai/FuxiCTR" /><a/>
         </div>
         
@@ -40,15 +39,15 @@
         + **Extensible**: It supports both pytorch and tensorflow models, and can be easily extended to any new models.
         
         
         ## Model Zoo
         
         | No  | Publication       | Model                                    | Paper                                                                                                                                                                                                           | Benchmark                                                                                                       | Version       |
         |:---:|:-----------------:|:----------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:---------------------------------------------------------------------------------------------------------------:|:-------------:|
-        |     |                   |                                          | :point_down:**Feature Interaction Models**                                                                                                                                                                      |                                                                                                                 |               |
+        |<tr><th colspan=6 align="center">:open_file_folder: **Feature Interaction Models**</th></tr>|
         | 1   | WWW'07            | [LR](./model_zoo/LR)                     | [Predicting Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft**                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LR)           | `torch`       |
         | 2   | ICDM'10           | [FM](./model_zoo/FM)                     | [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)                                                                                                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FM)           | `torch`       |
         | 3   | CIKM'13           | [DSSM](./model_zoo/DSSM)                 | [Learning Deep Structured Semantic Models  for Web Search using Clickthrough Data ](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DSSM)         | `torch`       |
         | 4   | CIKM'15           | [CCPM](./model_zoo/CCPM)                 | [A Convolutional Click Prediction Model](http://www.escience.cn/system/download/73676)                                                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/CCPM)         | `torch`       |
         | 5   | RecSys'16         | [FFM](./model_zoo/FFM)                   | [Field-aware Factorization Machines for CTR Prediction](https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:**Criteo**                                                                         | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FFM)          | `torch`       |
         | 6   | RecSys'16         | [DNN](./model_zoo/DNN)            | [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:**Google**                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DNN)          | `torch`, `tf` |
         | 7   | DLRS'16           | [Wide&Deep](./model_zoo/WideDeep)        | [Wide & Deep Learning for Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:**Google**                                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/WideDeep)     | `torch`, `tf` |
@@ -63,42 +62,45 @@
         | 16  | KDD'18            | [xDeepFM](./model_zoo/xDeepFM)           | [xDeepFM: Combining Explicit and Implicit Feature Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf) :triangular_flag_on_post:**Microsoft**                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/xDeepFM)      | `torch`       |
         | 17  | CIKM'19           | [FiGNN](./model_zoo/FiGNN)               | [FiGNN: Modeling Feature Interactions via Graph Neural Networks for CTR Prediction](https://arxiv.org/abs/1910.05552)                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiGNN)        | `torch`       |
         | 18  | CIKM'19           | [AutoInt/AutoInt+](./model_zoo/AutoInt)  | [AutoInt: Automatic Feature Interaction Learning via Self-Attentive Neural Networks](https://arxiv.org/abs/1810.11921)                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AutoInt)      | `torch`       |
         | 19  | RecSys'19         | [FiBiNET](./model_zoo/FiBiNET)           | [FiBiNET: Combining Feature Importance and Bilinear feature Interaction for Click-Through Rate Prediction](https://arxiv.org/abs/1905.09433) :triangular_flag_on_post:**Sina Weibo**                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiBiNET)      | `torch`       |
         | 20  | WWW'19            | [FGCNN](./model_zoo/FGCNN)               | [Feature Generation by Convolutional Neural Network for Click-Through Rate Prediction](https://arxiv.org/abs/1904.04447) :triangular_flag_on_post:**Huawei**                                                    | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FGCNN)        | `torch`       |
         | 21  | AAAI'19           | [HFM/HFM+](./model_zoo/HFM)              | [Holographic Factorization Machines for Recommendation](https://ojs.aaai.org//index.php/AAAI/article/view/4448)                                                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HFM)          | `torch`       |
         | 22  | Arxiv'19          | [DLRM](./model_zoo/DLRM)                 | [Deep Learning Recommendation Model for Personalization and Recommendation Systems](https://arxiv.org/abs/1906.00091) :triangular_flag_on_post:**Facebook**                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DLRM)         | `torch`       |
-        | 23  | NeuralNetworks'20 | [ONN](./model_zoo/ONN)                   | [Operation-aware Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)                                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/ONN)          | `torch`       |
+        | 23  | NeuralNetworks'20 | [ONN](./model_zoo/ONN)                   | [Operation-aware Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)                                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/ONN)          | `torch`, `tf`      |
         | 24  | AAAI'20           | [AFN/AFN+](./model_zoo/AFN)              | [Adaptive Factorization Network: Learning Adaptive-Order Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768)                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AFN)          | `torch`       |
         | 25  | AAAI'20           | [LorentzFM](./model_zoo/LorentzFM)       | [Learning Feature Interactions with Lorentzian Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:**eBay**                                                                               | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LorentzFM)    | `torch`       |
         | 26  | WSDM'20           | [InterHAt](./model_zoo/InterHAt)         | [Interpretable Click-through Rate Prediction through Hierarchical Attention](https://dl.acm.org/doi/10.1145/3336191.3371785) :triangular_flag_on_post:**NEC Labs, Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/InterHAt)     | `torch`       |
         | 27  | DLP-KDD'20        | [FLEN](./model_zoo/FLEN)                 | [FLEN: Leveraging Field for Scalable CTR Prediction](https://arxiv.org/abs/1911.04690) :triangular_flag_on_post:**Tencent**                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FLEN)         | `torch`       |
         | 28  | CIKM'20           | [DeepIM](./model_zoo/DeepIM)             | [Deep Interaction Machine: A Simple but Effective Model for High-order Feature Interactions](https://dl.acm.org/doi/abs/10.1145/3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepIM)       | `torch`       |
         | 29  | WWW'21            | [FmFM](./model_zoo/FmFM)                 | [FM^2: Field-matrixed Factorization Machines for Recommender Systems](https://arxiv.org/abs/2102.12994) :triangular_flag_on_post:**Yahoo**                                                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FmFM)         | `torch`       |
         | 30  | WWW'21            | [DCN-V2](./model_zoo/DCNv2)              | [DCN V2: Improved Deep & Cross Network and Practical Lessons for Web-scale Learning to Rank Systems](https://arxiv.org/abs/2008.13535) :triangular_flag_on_post:**Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DCNv2)        | `torch`       |
         | 31  | CIKM'21           | [DESTINE](./model_zoo/DESTINE)           | [Disentangled Self-Attentive Neural Networks for Click-Through Rate Prediction](https://arxiv.org/abs/2101.03654) :triangular_flag_on_post:**Alibaba**                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DESTINE)      | `torch`       |
         | 32  | CIKM'21           | [EDCN](./model_zoo/EDCN)                 | [Enhancing Explicit and Implicit Feature Interactions via Information Sharing for Parallel Deep CTR Models](https://dlp-kdd.github.io/assets/pdf/DLP-KDD_2021_paper_12.pdf) :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/EDCN)         | `torch`       |
         | 33  | DLP-KDD'21        | [MaskNet](./model_zoo/MaskNet)           | [MaskNet: Introducing Feature-Wise Multiplication to CTR Ranking Models by Instance-Guided Mask](https://arxiv.org/abs/2102.07619) :triangular_flag_on_post:**Sina Weibo**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/MaskNet)      | `torch`       |
         | 34  | SIGIR'21          | [SAM](./model_zoo/SAM)                   | [Looking at CTR Prediction Again: Is Attention All You Need?](https://arxiv.org/abs/2105.05563) :triangular_flag_on_post:**BOSS Zhipin**                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/SAM)          | `torch`       |
         | 35  | KDD'21            | [AOANet](./model_zoo/AOANet)             | [Architecture and Operation Adaptive Network for Online Recommendations](https://dl.acm.org/doi/10.1145/3447548.3467133) :triangular_flag_on_post:**Didi Chuxing**                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AOANet)       | `torch`       |
         | 36  | AAAI'23           | [FinalMLP](./model_zoo/FinalMLP)         | [FinalMLP: An Enhanced Two-Stream MLP Model for CTR Prediction](https://arxiv.org/abs/2304.00902) :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FinalMLP)         | `torch`       |
-        | 37  | SIGIR'23           | [FINAL](./model_zoo/FINAL)         | FINAL: Factorized Interaction Layer for CTR Prediction :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FINAL)         | `torch`       |
-        |     |                   |                                          | :point_down:**User Behavior Modeling**                                                                                                                                                                          |                                                                                                                 |               |
+        | 37  | SIGIR'23          | [FINAL](./model_zoo/FINAL)               | FINAL: Factorized Interaction Layer for CTR Prediction :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FINAL)         | `torch`       |
+        |<tr><th colspan=6 align="center">:open_file_folder: **Behavior Sequence Modeling**</th></tr>|
         | 38  | KDD'18            | [DIN](./model_zoo/DIN)                   | [Deep Interest Network for Click-Through Rate Prediction](https://www.kdd.org/kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-prediction) :triangular_flag_on_post:**Alibaba**        |   [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIN)       | `torch`       |
         | 39  | AAAI'19           | [DIEN](./model_zoo/DIEN)                 | [Deep Interest Evolution Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672) :triangular_flag_on_post:**Alibaba**                                                                      |   [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIEN)        | `torch`       |
         | 40  | DLP-KDD'19        | [BST](./model_zoo/BST)                   | [Behavior Sequence Transformer for E-commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874) :triangular_flag_on_post:**Alibaba**                                                                 |  [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/BST)     | `torch`       |
         | 41  | CIKM'20           | [DMIN](./model_zoo/DMIN)                 | [Deep Multi-Interest Network for Click-through Rate Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092) :triangular_flag_on_post:**Alibaba**                                                            |                                                                                                                 | `torch`       |
         | 42  | AAAI'20           | [DMR](./model_zoo/DMR)                   | [Deep Match to Rank Model for Personalized Click-Through Rate Prediction](https://ojs.aaai.org/index.php/AAAI/article/view/5346) :triangular_flag_on_post:**Alibaba**                                           |                                                                                                                 | `torch`       |
         | 43  | Arxiv'21          | [ETA](./model_zoo/ETA)                   | [End-to-End User Behavior Retrieval in Click-Through RatePrediction Model](https://arxiv.org/abs/2108.04468) :triangular_flag_on_post:**Alibaba**                                                               |                                                                                                                 | `torch`       |
         | 44  | CIKM'22           | [SDIM](./model_zoo/SDIM)                 | [Sampling Is All You Need on Modeling Long-Term User Behaviors for CTR Prediction](https://arxiv.org/abs/2205.10249) :triangular_flag_on_post:**Meituan**                                                       |                                                                                                                 | `torch`       |
-        |     |                   |                                          | :point_down:**Multi-Task Models**                                                                                                                                                                          |                                                                                                                 |               |
-        | 45  |     MachineLearn'97      | [SharedBottom](./model_zoo/multitask/SharedBottom)               | [Multitask Learning](https://link.springer.com/article/10.1023/A:1007379606734)                                                                                            |                                                                                                                 | `torch`       |
-        | 46  | KDD'18          | [MMoE](./model_zoo/multitask/MMOE)               | [Modeling Task Relationships in Multi-task Learning with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/3219819.3220007) :triangular_flag_on_post:**Google**                                                                                            |                                                                                                                 | `torch`       |
-        |     |                   |                                          | :point_down:**Multi-Domain Models**                                                                                                                                                                          |                                                                                                                 |               |
-        | 47  | Arxiv'23           | [PPNet](./model_zoo/PPNet)/PEPNet              | [PEPNet: Parameter and Embedding Personalized Network for Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115) :triangular_flag_on_post:**KuaiShou**                                                                                            |                                                                                                                 | `torch`       |
+        |<tr><th colspan=6 align="center">:open_file_folder: **Dynamic Weight Network**</th></tr>|
+        | 45  | NeurIPS'22          | [APG](./model_zoo/APG)               | [APG: Adaptive Parameter Generation Network for Click-Through Rate Prediction](https://arxiv.org/abs/2203.16218) :triangular_flag_on_post:**Alibaba**                                |                                                                                                  | `torch`       |
+        | 46  | Arxiv'23        | [PPNet](./model_zoo/PEPNet)             | [PEPNet: Parameter and Embedding Personalized Network for Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115) :triangular_flag_on_post:**KuaiShou**                          |                                                                                                  | `torch`       |
+        |<tr><th colspan=6 align="center">:open_file_folder: **Multi-Task Modeling**</th></tr>|
+        | 47  |     MachineLearn'97      | [SharedBottom](./model_zoo/multitask/SharedBottom)               | [Multitask Learning](https://link.springer.com/article/10.1023/A:1007379606734)                                                                                            |                                                                                                                 | `torch`       |
+        | 48  | KDD'18          | [MMoE](./model_zoo/multitask/MMOE)               | [Modeling Task Relationships in Multi-task Learning with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/3219819.3220007) :triangular_flag_on_post:**Google**                                                                                            |                                                                                                                 | `torch`       |
+        |<tr><th colspan=6 align="center">:open_file_folder: **Multi-Domain Modeling**</th></tr>|
+        | 49  | Arxiv'23           | PEPNet              | [PEPNet: Parameter and Embedding Personalized Network for Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115) :triangular_flag_on_post:**KuaiShou**                                                                                            |                                                                                                                 | `torch`       |
         
         
         + :point_right: See [reusable dataset splits for CTR prediction](https://openbenchmark.github.io/BARS/datasets/README.html).
         + :point_right: See [benchmarking configurations and steps](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks).
         + :point_right: See [the BARS benchmark leaderboard](https://openbenchmark.github.io/BARS/ctr_prediction/leaderboard/README.html#).
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.0.2 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.0.3 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/xue-pai/FuxiCTR Author: zhujiem Author-email:
 zhujiem@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/xue-pai/FuxiCTR/tags Description:
                                     [Logo]
 [Python_version] [Pytorch_version] [Pytorch_version] [Pypi_version] [Downloads]
-                          [License] [Wechat_QR_code]
+                                   [License]
 ===============================================================================
                 [https://reporoster.com/stars/xue-pai/FuxiCTR]
 Click-through rate (CTR) prediction is a critical task for many industrial
 applications such as online advertising, recommender systems, and sponsored
 search. FuxiCTR provides an open-source library for CTR prediction, with key
 features in configurability, tunability, and reproducibility. We hope this
 project could benefit both researchers and practitioners with the goal of open
@@ -20,49 +20,50 @@
 **Extensible**: It supports both pytorch and tensorflow models, and can be
 easily extended to any new models. ## Model Zoo | No | Publication | Model |
 Paper | Benchmark | Version | |:---:|:-----------------:|:---------------------
 -------------------:|:---------------------------------------------------------
 -------------------------------------------------------------------------------
 ----------------------------------------------------------------------- |:-----
 -------------------------------------------------------------------------------
----------------------------:|:-------------:| | | | | :point_down:**Feature
-Interaction Models** | | | | 1 | WWW'07 | [LR](./model_zoo/LR) | [Predicting
-Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/
-citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
-ctr_prediction/benchmarks/LR) | `torch` | | 2 | ICDM'10 | [FM](./model_zoo/FM)
-| [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/
-Rendle2010FM.pdf) | [:arrow_upper_right:](https://github.com/openbenchmark/
-BARS/tree/main/ctr_prediction/benchmarks/FM) | `torch` | | 3 | CIKM'13 | [DSSM]
-(./model_zoo/DSSM) | [Learning Deep Structured Semantic Models for Web Search
-using Clickthrough Data ](https://posenhuang.github.io/papers/
-cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
-ctr_prediction/benchmarks/DSSM) | `torch` | | 4 | CIKM'15 | [CCPM](./model_zoo/
-CCPM) | [A Convolutional Click Prediction Model](http://www.escience.cn/system/
-download/73676) | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/
-tree/main/ctr_prediction/benchmarks/CCPM) | `torch` | | 5 | RecSys'16 | [FFM]
-(./model_zoo/FFM) | [Field-aware Factorization Machines for CTR Prediction]
-(https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:
-**Criteo** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
-main/ctr_prediction/benchmarks/FFM) | `torch` | | 6 | RecSys'16 | [DNN](./
-model_zoo/DNN) | [Deep Neural Networks for YouTube Recommendations](http://
-art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:
-**Google** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
-main/ctr_prediction/benchmarks/DNN) | `torch`, `tf` | | 7 | DLRS'16 |
-[Wide&Deep](./model_zoo/WideDeep) | [Wide & Deep Learning for Recommender
-Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:
-**Google** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
-main/ctr_prediction/benchmarks/WideDeep) | `torch`, `tf` | | 8 | ICDM'16 |
-[IPNN](./model_zoo/PNN) | [Product-based Neural Networks for User Response
-Prediction](https://arxiv.org/pdf/1611.00144.pdf) | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/
-IPNN) | `torch` | | 9 | KDD'16 | [DeepCrossing](./model_zoo/DeepCrossing) |
-[Deep Crossing: Web-Scale Modeling without Manually Crafted Combinatorial
-Features](https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :
+---------------------------:|:-------------:| |
+:open_file_folder: **Feature Interaction Models**
+| | 1 | WWW'07 | [LR](./model_zoo/LR) | [Predicting Clicks: Estimating the
+Click-Through Rate for New Ads](https://dl.acm.org/citation.cfm?id=1242643) :
+triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LR) | `torch`
+| | 2 | ICDM'10 | [FM](./model_zoo/FM) | [Factorization Machines](https://
+www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf) | [:arrow_upper_right:]
+(https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FM)
+| `torch` | | 3 | CIKM'13 | [DSSM](./model_zoo/DSSM) | [Learning Deep
+Structured Semantic Models for Web Search using Clickthrough Data ](https://
+posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf) :
+triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DSSM) |
+`torch` | | 4 | CIKM'15 | [CCPM](./model_zoo/CCPM) | [A Convolutional Click
+Prediction Model](http://www.escience.cn/system/download/73676) | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/CCPM) | `torch` | | 5 | RecSys'16 | [FFM](./
+model_zoo/FFM) | [Field-aware Factorization Machines for CTR Prediction](https:
+//dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:**Criteo** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/FFM) | `torch` | | 6 | RecSys'16 | [DNN](./model_zoo/
+DNN) | [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/
+file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:**Google** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/DNN) | `torch`, `tf` | | 7 | DLRS'16 | [Wide&Deep](./
+model_zoo/WideDeep) | [Wide & Deep Learning for Recommender Systems](https://
+arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:**Google** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/WideDeep) | `torch`, `tf` | | 8 | ICDM'16 | [IPNN](./
+model_zoo/PNN) | [Product-based Neural Networks for User Response Prediction]
+(https://arxiv.org/pdf/1611.00144.pdf) | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/IPNN) |
+`torch` | | 9 | KDD'16 | [DeepCrossing](./model_zoo/DeepCrossing) | [Deep
+Crossing: Web-Scale Modeling without Manually Crafted Combinatorial Features]
+(https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :
 triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
 github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepCrossing)
 | `torch` | | 10 | NIPS'16 | [HOFM](./model_zoo/HOFM) | [Higher-Order
 Factorization Machines](https://papers.nips.cc/paper/6144-higher-order-
 factorization-machines.pdf) | [:arrow_upper_right:](https://github.com/
 openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HOFM) | `torch` | | 11 |
 IJCAI'17 | [DeepFM](./model_zoo/DeepFM) | [DeepFM: A Factorization-Machine
@@ -114,15 +115,15 @@
 model_zoo/DLRM) | [Deep Learning Recommendation Model for Personalization and
 Recommendation Systems](https://arxiv.org/abs/1906.00091) :
 triangular_flag_on_post:**Facebook** | [:arrow_upper_right:](https://
 github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DLRM) |
 `torch` | | 23 | NeuralNetworks'20 | [ONN](./model_zoo/ONN) | [Operation-aware
 Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)
 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
-ctr_prediction/benchmarks/ONN) | `torch` | | 24 | AAAI'20 | [AFN/AFN+](./
+ctr_prediction/benchmarks/ONN) | `torch`, `tf` | | 24 | AAAI'20 | [AFN/AFN+](./
 model_zoo/AFN) | [Adaptive Factorization Network: Learning Adaptive-Order
 Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768) |
 [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/AFN) | `torch` | | 25 | AAAI'20 | [LorentzFM](./
 model_zoo/LorentzFM) | [Learning Feature Interactions with Lorentzian
 Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:
 **eBay** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
@@ -173,82 +174,91 @@
 `torch` | | 36 | AAAI'23 | [FinalMLP](./model_zoo/FinalMLP) | [FinalMLP: An
 Enhanced Two-Stream MLP Model for CTR Prediction](https://arxiv.org/abs/
 2304.00902)Â :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https:
 //github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FinalMLP) |
 `torch` | | 37 | SIGIR'23 | [FINAL](./model_zoo/FINAL) | FINAL: Factorized
 Interaction Layer for CTR PredictionÂ :triangular_flag_on_post:**Huawei** | [:
 arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
-ctr_prediction/benchmarks/FINAL) | `torch` | | | | | :point_down:**User
-Behavior Modeling** | | | | 38 | KDD'18 | [DIN](./model_zoo/DIN) | [Deep
-Interest Network for Click-Through Rate Prediction](https://www.kdd.org/
-kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-
-prediction) :triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https:
-//github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIN) |
-`torch` | | 39 | AAAI'19 | [DIEN](./model_zoo/DIEN) | [Deep Interest Evolution
-Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672)Â :
-triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIEN) | `torch` | | 40 |
-DLP-KDD'19 | [BST](./model_zoo/BST) | [Behavior Sequence Transformer for E-
-commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874)Â :
-triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/BST) | `torch` | | 41 |
-CIKM'20 | [DMIN](./model_zoo/DMIN) | [Deep Multi-Interest Network for Click-
-through Rate Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092)Â :
+ctr_prediction/benchmarks/FINAL) | `torch` | |
+:open_file_folder: **Behavior Sequence Modeling**
+| | 38 | KDD'18 | [DIN](./model_zoo/DIN) | [Deep Interest Network for Click-
+Through Rate Prediction](https://www.kdd.org/kdd2018/accepted-papers/view/deep-
+interest-network-for-click-through-rate-prediction) :triangular_flag_on_post:
+**Alibaba** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/DIN) | `torch` | | 39 | AAAI'19 | [DIEN](./
+model_zoo/DIEN) | [Deep Interest Evolution Network for Click-Through Rate
+Prediction](https://arxiv.org/abs/1809.03672)Â :triangular_flag_on_post:
+**Alibaba** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/DIEN) | `torch` | | 40 | DLP-KDD'19 | [BST](./
+model_zoo/BST) | [Behavior Sequence Transformer for E-commerce Recommendation
+in Alibaba](https://arxiv.org/abs/1905.06874)Â :triangular_flag_on_post:
+**Alibaba** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/BST) | `torch` | | 41 | CIKM'20 | [DMIN](./
+model_zoo/DMIN) | [Deep Multi-Interest Network for Click-through Rate
+Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092)Â :
 triangular_flag_on_post:**Alibaba** | | `torch` | | 42 | AAAI'20 | [DMR](./
 model_zoo/DMR) | [Deep Match to Rank Model for Personalized Click-Through Rate
 Prediction](https://ojs.aaai.org/index.php/AAAI/article/view/5346)Â :
 triangular_flag_on_post:**Alibaba** | | `torch` | | 43 | Arxiv'21 | [ETA](./
 model_zoo/ETA) | [End-to-End User Behavior Retrieval in Click-Through
 RatePrediction Model](https://arxiv.org/abs/2108.04468)Â :
 triangular_flag_on_post:**Alibaba** | | `torch` | | 44 | CIKM'22 | [SDIM](./
 model_zoo/SDIM) | [Sampling Is All You Need on Modeling Long-Term User
 Behaviors for CTR Prediction](https://arxiv.org/abs/2205.10249)Â :
-triangular_flag_on_post:**Meituan** | | `torch` | | | | | :point_down:**Multi-
-Task Models** | | | | 45 | MachineLearn'97 | [SharedBottom](./model_zoo/
-multitask/SharedBottom) | [Multitask Learning](https://link.springer.com/
-article/10.1023/A:1007379606734) | | `torch` | | 46 | KDD'18 | [MMoE](./
-model_zoo/multitask/MMOE) | [Modeling Task Relationships in Multi-task Learning
-with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/
-3219819.3220007) :triangular_flag_on_post:**Google** | | `torch` | | | | | :
-point_down:**Multi-Domain Models** | | | | 47 | Arxiv'23 | [PPNet](./model_zoo/
-PPNet)/PEPNet | [PEPNet: Parameter and Embedding Personalized Network for
-Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115)
-:triangular_flag_on_post:**KuaiShou** | | `torch` | + :point_right: See
-[reusable dataset splits for CTR prediction](https://openbenchmark.github.io/
-BARS/datasets/README.html). + :point_right: See [benchmarking configurations
-and steps](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/
-benchmarks). + :point_right: See [the BARS benchmark leaderboard](https://
-openbenchmark.github.io/BARS/ctr_prediction/leaderboard/README.html#). ##
-Dependencies FuxiCTR has the following dependency requirements. + python 3.6+ +
-pytorch 1.0/1.10+ (required only for torch models) + tensorflow 2.1+ (required
-only for tf models) Other packages can be installed via `pip install -
-r requirements.txt`. ## Quick Start 1. Run the demo examples Examples are
-provided in the demo directory to show some basic usage of FuxiCTR. Users can
-run the examples for quick start and to understand the workflow. ``` cd demo
-python example1_build_dataset_to_h5.py python example2_DeepFM_with_h5_input.py
-``` 2. Run an existing model Users can easily run each model in the model zoo
-following the commands below, which is a demo for running DCN. In addition,
-users can modify the dataset config and model config files to run on their own
-datasets or with new hyper-parameters. More details can be found in the [readme
-file](./model_zoo/DCN/DCN_torch/README.md). ``` cd model_zoo/DCN/DCN_torch
-python run_expid.py --expid DCN_test --gpu 0 # Change `MODEL` according to the
-target model name cd model_zoo/MODEL_PATH python run_expid.py --expid
-MODEL_test --gpu 0 ``` 3. Implement a new model The FuxiCTR code structure is
-modularized, so that every part can be overwritten by users according to their
-needs. In many cases, only the model class needs to be implemented for a new
-customized model. If data preprocessing or data loader is not directly
-applicable, one can also overwrite a new one through the [core APIs](https://
-www.processon.com/view/link/63cfcfab4e30670eac4a81c7). We show a concrete
-example which implements our new model [FinalMLP](https://github.com/xue-pai/
-FinalMLP) that has been recently published in AAAI 2023. More examples can be
-found in the [model zoo](./model_zoo/). ## Citation *:bell: If you find our
-code or benchmarks helpful in your research, please kindly cite the following
-papers.* > Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang He. [Open
-Benchmarking for Click-Through Rate Prediction](https://arxiv.org/abs/
-2009.05794). *The 30th ACM International Conference on Information and
+triangular_flag_on_post:**Meituan** | | `torch` | |
+:open_file_folder: **Dynamic Weight Network**
+| | 45 | NeurIPS'22 | [APG](./model_zoo/APG) | [APG: Adaptive Parameter
+Generation Network for Click-Through Rate Prediction](https://arxiv.org/abs/
+2203.16218) :triangular_flag_on_post:**Alibaba** | | `torch` | | 46 | Arxiv'23
+| [PPNet](./model_zoo/PEPNet) | [PEPNet: Parameter and Embedding Personalized
+Network for Infusing with Personalized Prior Information](https://arxiv.org/
+abs/2302.01115) :triangular_flag_on_post:**KuaiShou** | | `torch` | |
+:open_file_folder: **Multi-Task Modeling**
+| | 47 | MachineLearn'97 | [SharedBottom](./model_zoo/multitask/SharedBottom) |
+[Multitask Learning](https://link.springer.com/article/10.1023/A:1007379606734)
+| | `torch` | | 48 | KDD'18 | [MMoE](./model_zoo/multitask/MMOE) | [Modeling
+Task Relationships in Multi-task Learning with Multi-Gate Mixture-of-Experts]
+(https://dl.acm.org/doi/pdf/10.1145/3219819.3220007) :triangular_flag_on_post:
+**Google** | | `torch` | |
+:open_file_folder: **Multi-Domain Modeling**
+| | 49 | Arxiv'23 | PEPNet | [PEPNet: Parameter and Embedding Personalized
+Network for Infusing with Personalized Prior Information](https://arxiv.org/
+abs/2302.01115) :triangular_flag_on_post:**KuaiShou** | | `torch` | + :
+point_right: See [reusable dataset splits for CTR prediction](https://
+openbenchmark.github.io/BARS/datasets/README.html). + :point_right: See
+[benchmarking configurations and steps](https://github.com/openbenchmark/BARS/
+tree/main/ctr_prediction/benchmarks). + :point_right: See [the BARS benchmark
+leaderboard](https://openbenchmark.github.io/BARS/ctr_prediction/leaderboard/
+README.html#). ## Dependencies FuxiCTR has the following dependency
+requirements. + python 3.6+ + pytorch 1.0/1.10+ (required only for torch
+models) + tensorflow 2.1+ (required only for tf models) Other packages can be
+installed via `pip install -r requirements.txt`. ## Quick Start 1. Run the demo
+examples Examples are provided in the demo directory to show some basic usage
+of FuxiCTR. Users can run the examples for quick start and to understand the
+workflow. ``` cd demo python example1_build_dataset_to_h5.py python
+example2_DeepFM_with_h5_input.py ``` 2. Run an existing model Users can easily
+run each model in the model zoo following the commands below, which is a demo
+for running DCN. In addition, users can modify the dataset config and model
+config files to run on their own datasets or with new hyper-parameters. More
+details can be found in the [readme file](./model_zoo/DCN/DCN_torch/README.md).
+``` cd model_zoo/DCN/DCN_torch python run_expid.py --expid DCN_test --gpu 0 #
+Change `MODEL` according to the target model name cd model_zoo/MODEL_PATH
+python run_expid.py --expid MODEL_test --gpu 0 ``` 3. Implement a new model The
+FuxiCTR code structure is modularized, so that every part can be overwritten by
+users according to their needs. In many cases, only the model class needs to be
+implemented for a new customized model. If data preprocessing or data loader is
+not directly applicable, one can also overwrite a new one through the [core
+APIs](https://www.processon.com/view/link/63cfcfab4e30670eac4a81c7). We show a
+concrete example which implements our new model [FinalMLP](https://github.com/
+xue-pai/FinalMLP) that has been recently published in AAAI 2023. More examples
+can be found in the [model zoo](./model_zoo/). ## Citation *:bell: If you find
+our code or benchmarks helpful in your research, please kindly cite the
+following papers.* > Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang
+He. [Open Benchmarking for Click-Through Rate Prediction](https://arxiv.org/
+abs/2009.05794). *The 30th ACM International Conference on Information and
 Knowledge Management (CIKM)*, 2021. [[Bibtex](https://dblp.org/rec/conf/cikm/
 ZhuLYZH21.html?view=bibtex)] > Jieming Zhu, Quanyu Dai, Liangcai Su, Rong Ma,
 Jinyang Liu, Guohao Cai, Xi Xiao, Rui Zhang. [BARS: Towards Open Benchmarking
 for Recommender Systems](https://arxiv.org/abs/2205.09626). *The 45th
 International ACM SIGIR Conference on Research and Development in Information
 Retrieval (SIGIR)*, 2022. [[Bibtex](https://dblp.org/rec/conf/sigir/
 ZhuDSMLCXZ22.html?view=bibtex)] ## Discussion Welcome to join our WeChat group
```

### Comparing `fuxictr-2.0.2/README.md` & `fuxictr-2.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 <div align="center">
 <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/python-3.6+-blue" style="max-width: 100%;" alt="Python version"></a>
 <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/pytorch-1.10+-blue" style="max-width: 100%;" alt="Pytorch version"></a>
 <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/tensorflow-2.1+-blue" style="max-width: 100%;" alt="Pytorch version"></a>
 <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/pypi/v/fuxictr.svg" style="max-width: 100%;" alt="Pypi version"></a>
 <a href="https://pepy.tech/project/fuxictr"><img src="https://pepy.tech/badge/fuxictr" style="max-width: 100%;" alt="Downloads"></a>
 <a href="https://github.com/xue-pai/FuxiCTR/blob/main/LICENSE"><img src="https://img.shields.io/github/license/xue-pai/fuxictr.svg" style="max-width: 100%;" alt="License"></a>
-<a href="https://fuxictr.github.io/tutorials"><img src="https://img.shields.io/badge/tutorials-passing-brightgreen?style=flat" style="max-width: 100%;" alt="Wechat QR code"></a>
 </div>
 <hr/>
 
 <div align="center">
 <a href="https://github.com/xue-pai/FuxiCTR/stargazers"><img src="https://reporoster.com/stars/xue-pai/FuxiCTR" /><a/>
 </div>
 
@@ -31,15 +30,15 @@
 + **Extensible**: It supports both pytorch and tensorflow models, and can be easily extended to any new models.
 
 
 ## Model Zoo
 
 | No  | Publication       | Model                                    | Paper                                                                                                                                                                                                           | Benchmark                                                                                                       | Version       |
 |:---:|:-----------------:|:----------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:---------------------------------------------------------------------------------------------------------------:|:-------------:|
-|     |                   |                                          | :point_down:**Feature Interaction Models**                                                                                                                                                                      |                                                                                                                 |               |
+|<tr><th colspan=6 align="center">:open_file_folder: **Feature Interaction Models**</th></tr>|
 | 1   | WWW'07            | [LR](./model_zoo/LR)                     | [Predicting Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft**                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LR)           | `torch`       |
 | 2   | ICDM'10           | [FM](./model_zoo/FM)                     | [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)                                                                                                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FM)           | `torch`       |
 | 3   | CIKM'13           | [DSSM](./model_zoo/DSSM)                 | [Learning Deep Structured Semantic Models  for Web Search using Clickthrough Data ](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DSSM)         | `torch`       |
 | 4   | CIKM'15           | [CCPM](./model_zoo/CCPM)                 | [A Convolutional Click Prediction Model](http://www.escience.cn/system/download/73676)                                                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/CCPM)         | `torch`       |
 | 5   | RecSys'16         | [FFM](./model_zoo/FFM)                   | [Field-aware Factorization Machines for CTR Prediction](https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:**Criteo**                                                                         | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FFM)          | `torch`       |
 | 6   | RecSys'16         | [DNN](./model_zoo/DNN)            | [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:**Google**                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DNN)          | `torch`, `tf` |
 | 7   | DLRS'16           | [Wide&Deep](./model_zoo/WideDeep)        | [Wide & Deep Learning for Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:**Google**                                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/WideDeep)     | `torch`, `tf` |
@@ -54,42 +53,45 @@
 | 16  | KDD'18            | [xDeepFM](./model_zoo/xDeepFM)           | [xDeepFM: Combining Explicit and Implicit Feature Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf) :triangular_flag_on_post:**Microsoft**                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/xDeepFM)      | `torch`       |
 | 17  | CIKM'19           | [FiGNN](./model_zoo/FiGNN)               | [FiGNN: Modeling Feature Interactions via Graph Neural Networks for CTR Prediction](https://arxiv.org/abs/1910.05552)                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiGNN)        | `torch`       |
 | 18  | CIKM'19           | [AutoInt/AutoInt+](./model_zoo/AutoInt)  | [AutoInt: Automatic Feature Interaction Learning via Self-Attentive Neural Networks](https://arxiv.org/abs/1810.11921)                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AutoInt)      | `torch`       |
 | 19  | RecSys'19         | [FiBiNET](./model_zoo/FiBiNET)           | [FiBiNET: Combining Feature Importance and Bilinear feature Interaction for Click-Through Rate Prediction](https://arxiv.org/abs/1905.09433) :triangular_flag_on_post:**Sina Weibo**                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiBiNET)      | `torch`       |
 | 20  | WWW'19            | [FGCNN](./model_zoo/FGCNN)               | [Feature Generation by Convolutional Neural Network for Click-Through Rate Prediction](https://arxiv.org/abs/1904.04447) :triangular_flag_on_post:**Huawei**                                                    | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FGCNN)        | `torch`       |
 | 21  | AAAI'19           | [HFM/HFM+](./model_zoo/HFM)              | [Holographic Factorization Machines for Recommendation](https://ojs.aaai.org//index.php/AAAI/article/view/4448)                                                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HFM)          | `torch`       |
 | 22  | Arxiv'19          | [DLRM](./model_zoo/DLRM)                 | [Deep Learning Recommendation Model for Personalization and Recommendation Systems](https://arxiv.org/abs/1906.00091) :triangular_flag_on_post:**Facebook**                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DLRM)         | `torch`       |
-| 23  | NeuralNetworks'20 | [ONN](./model_zoo/ONN)                   | [Operation-aware Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)                                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/ONN)          | `torch`       |
+| 23  | NeuralNetworks'20 | [ONN](./model_zoo/ONN)                   | [Operation-aware Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)                                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/ONN)          | `torch`, `tf`      |
 | 24  | AAAI'20           | [AFN/AFN+](./model_zoo/AFN)              | [Adaptive Factorization Network: Learning Adaptive-Order Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768)                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AFN)          | `torch`       |
 | 25  | AAAI'20           | [LorentzFM](./model_zoo/LorentzFM)       | [Learning Feature Interactions with Lorentzian Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:**eBay**                                                                               | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LorentzFM)    | `torch`       |
 | 26  | WSDM'20           | [InterHAt](./model_zoo/InterHAt)         | [Interpretable Click-through Rate Prediction through Hierarchical Attention](https://dl.acm.org/doi/10.1145/3336191.3371785) :triangular_flag_on_post:**NEC Labs, Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/InterHAt)     | `torch`       |
 | 27  | DLP-KDD'20        | [FLEN](./model_zoo/FLEN)                 | [FLEN: Leveraging Field for Scalable CTR Prediction](https://arxiv.org/abs/1911.04690) :triangular_flag_on_post:**Tencent**                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FLEN)         | `torch`       |
 | 28  | CIKM'20           | [DeepIM](./model_zoo/DeepIM)             | [Deep Interaction Machine: A Simple but Effective Model for High-order Feature Interactions](https://dl.acm.org/doi/abs/10.1145/3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepIM)       | `torch`       |
 | 29  | WWW'21            | [FmFM](./model_zoo/FmFM)                 | [FM^2: Field-matrixed Factorization Machines for Recommender Systems](https://arxiv.org/abs/2102.12994) :triangular_flag_on_post:**Yahoo**                                                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FmFM)         | `torch`       |
 | 30  | WWW'21            | [DCN-V2](./model_zoo/DCNv2)              | [DCN V2: Improved Deep & Cross Network and Practical Lessons for Web-scale Learning to Rank Systems](https://arxiv.org/abs/2008.13535) :triangular_flag_on_post:**Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DCNv2)        | `torch`       |
 | 31  | CIKM'21           | [DESTINE](./model_zoo/DESTINE)           | [Disentangled Self-Attentive Neural Networks for Click-Through Rate Prediction](https://arxiv.org/abs/2101.03654) :triangular_flag_on_post:**Alibaba**                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DESTINE)      | `torch`       |
 | 32  | CIKM'21           | [EDCN](./model_zoo/EDCN)                 | [Enhancing Explicit and Implicit Feature Interactions via Information Sharing for Parallel Deep CTR Models](https://dlp-kdd.github.io/assets/pdf/DLP-KDD_2021_paper_12.pdf) :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/EDCN)         | `torch`       |
 | 33  | DLP-KDD'21        | [MaskNet](./model_zoo/MaskNet)           | [MaskNet: Introducing Feature-Wise Multiplication to CTR Ranking Models by Instance-Guided Mask](https://arxiv.org/abs/2102.07619) :triangular_flag_on_post:**Sina Weibo**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/MaskNet)      | `torch`       |
 | 34  | SIGIR'21          | [SAM](./model_zoo/SAM)                   | [Looking at CTR Prediction Again: Is Attention All You Need?](https://arxiv.org/abs/2105.05563) :triangular_flag_on_post:**BOSS Zhipin**                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/SAM)          | `torch`       |
 | 35  | KDD'21            | [AOANet](./model_zoo/AOANet)             | [Architecture and Operation Adaptive Network for Online Recommendations](https://dl.acm.org/doi/10.1145/3447548.3467133) :triangular_flag_on_post:**Didi Chuxing**                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AOANet)       | `torch`       |
 | 36  | AAAI'23           | [FinalMLP](./model_zoo/FinalMLP)         | [FinalMLP: An Enhanced Two-Stream MLP Model for CTR Prediction](https://arxiv.org/abs/2304.00902) :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FinalMLP)         | `torch`       |
-| 37  | SIGIR'23           | [FINAL](./model_zoo/FINAL)         | FINAL: Factorized Interaction Layer for CTR Prediction :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FINAL)         | `torch`       |
-|     |                   |                                          | :point_down:**User Behavior Modeling**                                                                                                                                                                          |                                                                                                                 |               |
+| 37  | SIGIR'23          | [FINAL](./model_zoo/FINAL)               | FINAL: Factorized Interaction Layer for CTR Prediction :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FINAL)         | `torch`       |
+|<tr><th colspan=6 align="center">:open_file_folder: **Behavior Sequence Modeling**</th></tr>|
 | 38  | KDD'18            | [DIN](./model_zoo/DIN)                   | [Deep Interest Network for Click-Through Rate Prediction](https://www.kdd.org/kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-prediction) :triangular_flag_on_post:**Alibaba**        |   [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIN)       | `torch`       |
 | 39  | AAAI'19           | [DIEN](./model_zoo/DIEN)                 | [Deep Interest Evolution Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672) :triangular_flag_on_post:**Alibaba**                                                                      |   [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIEN)        | `torch`       |
 | 40  | DLP-KDD'19        | [BST](./model_zoo/BST)                   | [Behavior Sequence Transformer for E-commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874) :triangular_flag_on_post:**Alibaba**                                                                 |  [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/BST)     | `torch`       |
 | 41  | CIKM'20           | [DMIN](./model_zoo/DMIN)                 | [Deep Multi-Interest Network for Click-through Rate Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092) :triangular_flag_on_post:**Alibaba**                                                            |                                                                                                                 | `torch`       |
 | 42  | AAAI'20           | [DMR](./model_zoo/DMR)                   | [Deep Match to Rank Model for Personalized Click-Through Rate Prediction](https://ojs.aaai.org/index.php/AAAI/article/view/5346) :triangular_flag_on_post:**Alibaba**                                           |                                                                                                                 | `torch`       |
 | 43  | Arxiv'21          | [ETA](./model_zoo/ETA)                   | [End-to-End User Behavior Retrieval in Click-Through RatePrediction Model](https://arxiv.org/abs/2108.04468) :triangular_flag_on_post:**Alibaba**                                                               |                                                                                                                 | `torch`       |
 | 44  | CIKM'22           | [SDIM](./model_zoo/SDIM)                 | [Sampling Is All You Need on Modeling Long-Term User Behaviors for CTR Prediction](https://arxiv.org/abs/2205.10249) :triangular_flag_on_post:**Meituan**                                                       |                                                                                                                 | `torch`       |
-|     |                   |                                          | :point_down:**Multi-Task Models**                                                                                                                                                                          |                                                                                                                 |               |
-| 45  |     MachineLearn'97      | [SharedBottom](./model_zoo/multitask/SharedBottom)               | [Multitask Learning](https://link.springer.com/article/10.1023/A:1007379606734)                                                                                            |                                                                                                                 | `torch`       |
-| 46  | KDD'18          | [MMoE](./model_zoo/multitask/MMOE)               | [Modeling Task Relationships in Multi-task Learning with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/3219819.3220007) :triangular_flag_on_post:**Google**                                                                                            |                                                                                                                 | `torch`       |
-|     |                   |                                          | :point_down:**Multi-Domain Models**                                                                                                                                                                          |                                                                                                                 |               |
-| 47  | Arxiv'23           | [PPNet](./model_zoo/PPNet)/PEPNet              | [PEPNet: Parameter and Embedding Personalized Network for Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115) :triangular_flag_on_post:**KuaiShou**                                                                                            |                                                                                                                 | `torch`       |
+|<tr><th colspan=6 align="center">:open_file_folder: **Dynamic Weight Network**</th></tr>|
+| 45  | NeurIPS'22          | [APG](./model_zoo/APG)               | [APG: Adaptive Parameter Generation Network for Click-Through Rate Prediction](https://arxiv.org/abs/2203.16218) :triangular_flag_on_post:**Alibaba**                                |                                                                                                  | `torch`       |
+| 46  | Arxiv'23        | [PPNet](./model_zoo/PEPNet)             | [PEPNet: Parameter and Embedding Personalized Network for Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115) :triangular_flag_on_post:**KuaiShou**                          |                                                                                                  | `torch`       |
+|<tr><th colspan=6 align="center">:open_file_folder: **Multi-Task Modeling**</th></tr>|
+| 47  |     MachineLearn'97      | [SharedBottom](./model_zoo/multitask/SharedBottom)               | [Multitask Learning](https://link.springer.com/article/10.1023/A:1007379606734)                                                                                            |                                                                                                                 | `torch`       |
+| 48  | KDD'18          | [MMoE](./model_zoo/multitask/MMOE)               | [Modeling Task Relationships in Multi-task Learning with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/3219819.3220007) :triangular_flag_on_post:**Google**                                                                                            |                                                                                                                 | `torch`       |
+|<tr><th colspan=6 align="center">:open_file_folder: **Multi-Domain Modeling**</th></tr>|
+| 49  | Arxiv'23           | PEPNet              | [PEPNet: Parameter and Embedding Personalized Network for Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115) :triangular_flag_on_post:**KuaiShou**                                                                                            |                                                                                                                 | `torch`       |
 
 
 + :point_right: See [reusable dataset splits for CTR prediction](https://openbenchmark.github.io/BARS/datasets/README.html).
 + :point_right: See [benchmarking configurations and steps](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks).
 + :point_right: See [the BARS benchmark leaderboard](https://openbenchmark.github.io/BARS/ctr_prediction/leaderboard/README.html#).
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
                                     [Logo]
 [Python_version] [Pytorch_version] [Pytorch_version] [Pypi_version] [Downloads]
-                          [License] [Wechat_QR_code]
+                                   [License]
 ===============================================================================
                 [https://reporoster.com/stars/xue-pai/FuxiCTR]
 Click-through rate (CTR) prediction is a critical task for many industrial
 applications such as online advertising, recommender systems, and sponsored
 search. FuxiCTR provides an open-source library for CTR prediction, with key
 features in configurability, tunability, and reproducibility. We hope this
 project could benefit both researchers and practitioners with the goal of open
@@ -15,49 +15,50 @@
 **Extensible**: It supports both pytorch and tensorflow models, and can be
 easily extended to any new models. ## Model Zoo | No | Publication | Model |
 Paper | Benchmark | Version | |:---:|:-----------------:|:---------------------
 -------------------:|:---------------------------------------------------------
 -------------------------------------------------------------------------------
 ----------------------------------------------------------------------- |:-----
 -------------------------------------------------------------------------------
----------------------------:|:-------------:| | | | | :point_down:**Feature
-Interaction Models** | | | | 1 | WWW'07 | [LR](./model_zoo/LR) | [Predicting
-Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/
-citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
-ctr_prediction/benchmarks/LR) | `torch` | | 2 | ICDM'10 | [FM](./model_zoo/FM)
-| [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/
-Rendle2010FM.pdf) | [:arrow_upper_right:](https://github.com/openbenchmark/
-BARS/tree/main/ctr_prediction/benchmarks/FM) | `torch` | | 3 | CIKM'13 | [DSSM]
-(./model_zoo/DSSM) | [Learning Deep Structured Semantic Models for Web Search
-using Clickthrough Data ](https://posenhuang.github.io/papers/
-cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
-ctr_prediction/benchmarks/DSSM) | `torch` | | 4 | CIKM'15 | [CCPM](./model_zoo/
-CCPM) | [A Convolutional Click Prediction Model](http://www.escience.cn/system/
-download/73676) | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/
-tree/main/ctr_prediction/benchmarks/CCPM) | `torch` | | 5 | RecSys'16 | [FFM]
-(./model_zoo/FFM) | [Field-aware Factorization Machines for CTR Prediction]
-(https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:
-**Criteo** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
-main/ctr_prediction/benchmarks/FFM) | `torch` | | 6 | RecSys'16 | [DNN](./
-model_zoo/DNN) | [Deep Neural Networks for YouTube Recommendations](http://
-art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:
-**Google** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
-main/ctr_prediction/benchmarks/DNN) | `torch`, `tf` | | 7 | DLRS'16 |
-[Wide&Deep](./model_zoo/WideDeep) | [Wide & Deep Learning for Recommender
-Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:
-**Google** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
-main/ctr_prediction/benchmarks/WideDeep) | `torch`, `tf` | | 8 | ICDM'16 |
-[IPNN](./model_zoo/PNN) | [Product-based Neural Networks for User Response
-Prediction](https://arxiv.org/pdf/1611.00144.pdf) | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/
-IPNN) | `torch` | | 9 | KDD'16 | [DeepCrossing](./model_zoo/DeepCrossing) |
-[Deep Crossing: Web-Scale Modeling without Manually Crafted Combinatorial
-Features](https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :
+---------------------------:|:-------------:| |
+:open_file_folder: **Feature Interaction Models**
+| | 1 | WWW'07 | [LR](./model_zoo/LR) | [Predicting Clicks: Estimating the
+Click-Through Rate for New Ads](https://dl.acm.org/citation.cfm?id=1242643) :
+triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LR) | `torch`
+| | 2 | ICDM'10 | [FM](./model_zoo/FM) | [Factorization Machines](https://
+www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf) | [:arrow_upper_right:]
+(https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FM)
+| `torch` | | 3 | CIKM'13 | [DSSM](./model_zoo/DSSM) | [Learning Deep
+Structured Semantic Models for Web Search using Clickthrough Data ](https://
+posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf) :
+triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DSSM) |
+`torch` | | 4 | CIKM'15 | [CCPM](./model_zoo/CCPM) | [A Convolutional Click
+Prediction Model](http://www.escience.cn/system/download/73676) | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/CCPM) | `torch` | | 5 | RecSys'16 | [FFM](./
+model_zoo/FFM) | [Field-aware Factorization Machines for CTR Prediction](https:
+//dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:**Criteo** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/FFM) | `torch` | | 6 | RecSys'16 | [DNN](./model_zoo/
+DNN) | [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/
+file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:**Google** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/DNN) | `torch`, `tf` | | 7 | DLRS'16 | [Wide&Deep](./
+model_zoo/WideDeep) | [Wide & Deep Learning for Recommender Systems](https://
+arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:**Google** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/WideDeep) | `torch`, `tf` | | 8 | ICDM'16 | [IPNN](./
+model_zoo/PNN) | [Product-based Neural Networks for User Response Prediction]
+(https://arxiv.org/pdf/1611.00144.pdf) | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/IPNN) |
+`torch` | | 9 | KDD'16 | [DeepCrossing](./model_zoo/DeepCrossing) | [Deep
+Crossing: Web-Scale Modeling without Manually Crafted Combinatorial Features]
+(https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :
 triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
 github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepCrossing)
 | `torch` | | 10 | NIPS'16 | [HOFM](./model_zoo/HOFM) | [Higher-Order
 Factorization Machines](https://papers.nips.cc/paper/6144-higher-order-
 factorization-machines.pdf) | [:arrow_upper_right:](https://github.com/
 openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HOFM) | `torch` | | 11 |
 IJCAI'17 | [DeepFM](./model_zoo/DeepFM) | [DeepFM: A Factorization-Machine
@@ -109,15 +110,15 @@
 model_zoo/DLRM) | [Deep Learning Recommendation Model for Personalization and
 Recommendation Systems](https://arxiv.org/abs/1906.00091) :
 triangular_flag_on_post:**Facebook** | [:arrow_upper_right:](https://
 github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DLRM) |
 `torch` | | 23 | NeuralNetworks'20 | [ONN](./model_zoo/ONN) | [Operation-aware
 Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)
 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
-ctr_prediction/benchmarks/ONN) | `torch` | | 24 | AAAI'20 | [AFN/AFN+](./
+ctr_prediction/benchmarks/ONN) | `torch`, `tf` | | 24 | AAAI'20 | [AFN/AFN+](./
 model_zoo/AFN) | [Adaptive Factorization Network: Learning Adaptive-Order
 Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768) |
 [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/AFN) | `torch` | | 25 | AAAI'20 | [LorentzFM](./
 model_zoo/LorentzFM) | [Learning Feature Interactions with Lorentzian
 Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:
 **eBay** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
@@ -168,82 +169,91 @@
 `torch` | | 36 | AAAI'23 | [FinalMLP](./model_zoo/FinalMLP) | [FinalMLP: An
 Enhanced Two-Stream MLP Model for CTR Prediction](https://arxiv.org/abs/
 2304.00902)Â :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https:
 //github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FinalMLP) |
 `torch` | | 37 | SIGIR'23 | [FINAL](./model_zoo/FINAL) | FINAL: Factorized
 Interaction Layer for CTR PredictionÂ :triangular_flag_on_post:**Huawei** | [:
 arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
-ctr_prediction/benchmarks/FINAL) | `torch` | | | | | :point_down:**User
-Behavior Modeling** | | | | 38 | KDD'18 | [DIN](./model_zoo/DIN) | [Deep
-Interest Network for Click-Through Rate Prediction](https://www.kdd.org/
-kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-
-prediction) :triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https:
-//github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIN) |
-`torch` | | 39 | AAAI'19 | [DIEN](./model_zoo/DIEN) | [Deep Interest Evolution
-Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672)Â :
-triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIEN) | `torch` | | 40 |
-DLP-KDD'19 | [BST](./model_zoo/BST) | [Behavior Sequence Transformer for E-
-commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874)Â :
-triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/BST) | `torch` | | 41 |
-CIKM'20 | [DMIN](./model_zoo/DMIN) | [Deep Multi-Interest Network for Click-
-through Rate Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092)Â :
+ctr_prediction/benchmarks/FINAL) | `torch` | |
+:open_file_folder: **Behavior Sequence Modeling**
+| | 38 | KDD'18 | [DIN](./model_zoo/DIN) | [Deep Interest Network for Click-
+Through Rate Prediction](https://www.kdd.org/kdd2018/accepted-papers/view/deep-
+interest-network-for-click-through-rate-prediction) :triangular_flag_on_post:
+**Alibaba** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/DIN) | `torch` | | 39 | AAAI'19 | [DIEN](./
+model_zoo/DIEN) | [Deep Interest Evolution Network for Click-Through Rate
+Prediction](https://arxiv.org/abs/1809.03672)Â :triangular_flag_on_post:
+**Alibaba** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/DIEN) | `torch` | | 40 | DLP-KDD'19 | [BST](./
+model_zoo/BST) | [Behavior Sequence Transformer for E-commerce Recommendation
+in Alibaba](https://arxiv.org/abs/1905.06874)Â :triangular_flag_on_post:
+**Alibaba** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/BST) | `torch` | | 41 | CIKM'20 | [DMIN](./
+model_zoo/DMIN) | [Deep Multi-Interest Network for Click-through Rate
+Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092)Â :
 triangular_flag_on_post:**Alibaba** | | `torch` | | 42 | AAAI'20 | [DMR](./
 model_zoo/DMR) | [Deep Match to Rank Model for Personalized Click-Through Rate
 Prediction](https://ojs.aaai.org/index.php/AAAI/article/view/5346)Â :
 triangular_flag_on_post:**Alibaba** | | `torch` | | 43 | Arxiv'21 | [ETA](./
 model_zoo/ETA) | [End-to-End User Behavior Retrieval in Click-Through
 RatePrediction Model](https://arxiv.org/abs/2108.04468)Â :
 triangular_flag_on_post:**Alibaba** | | `torch` | | 44 | CIKM'22 | [SDIM](./
 model_zoo/SDIM) | [Sampling Is All You Need on Modeling Long-Term User
 Behaviors for CTR Prediction](https://arxiv.org/abs/2205.10249)Â :
-triangular_flag_on_post:**Meituan** | | `torch` | | | | | :point_down:**Multi-
-Task Models** | | | | 45 | MachineLearn'97 | [SharedBottom](./model_zoo/
-multitask/SharedBottom) | [Multitask Learning](https://link.springer.com/
-article/10.1023/A:1007379606734) | | `torch` | | 46 | KDD'18 | [MMoE](./
-model_zoo/multitask/MMOE) | [Modeling Task Relationships in Multi-task Learning
-with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/
-3219819.3220007) :triangular_flag_on_post:**Google** | | `torch` | | | | | :
-point_down:**Multi-Domain Models** | | | | 47 | Arxiv'23 | [PPNet](./model_zoo/
-PPNet)/PEPNet | [PEPNet: Parameter and Embedding Personalized Network for
-Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115)
-:triangular_flag_on_post:**KuaiShou** | | `torch` | + :point_right: See
-[reusable dataset splits for CTR prediction](https://openbenchmark.github.io/
-BARS/datasets/README.html). + :point_right: See [benchmarking configurations
-and steps](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/
-benchmarks). + :point_right: See [the BARS benchmark leaderboard](https://
-openbenchmark.github.io/BARS/ctr_prediction/leaderboard/README.html#). ##
-Dependencies FuxiCTR has the following dependency requirements. + python 3.6+ +
-pytorch 1.0/1.10+ (required only for torch models) + tensorflow 2.1+ (required
-only for tf models) Other packages can be installed via `pip install -
-r requirements.txt`. ## Quick Start 1. Run the demo examples Examples are
-provided in the demo directory to show some basic usage of FuxiCTR. Users can
-run the examples for quick start and to understand the workflow. ``` cd demo
-python example1_build_dataset_to_h5.py python example2_DeepFM_with_h5_input.py
-``` 2. Run an existing model Users can easily run each model in the model zoo
-following the commands below, which is a demo for running DCN. In addition,
-users can modify the dataset config and model config files to run on their own
-datasets or with new hyper-parameters. More details can be found in the [readme
-file](./model_zoo/DCN/DCN_torch/README.md). ``` cd model_zoo/DCN/DCN_torch
-python run_expid.py --expid DCN_test --gpu 0 # Change `MODEL` according to the
-target model name cd model_zoo/MODEL_PATH python run_expid.py --expid
-MODEL_test --gpu 0 ``` 3. Implement a new model The FuxiCTR code structure is
-modularized, so that every part can be overwritten by users according to their
-needs. In many cases, only the model class needs to be implemented for a new
-customized model. If data preprocessing or data loader is not directly
-applicable, one can also overwrite a new one through the [core APIs](https://
-www.processon.com/view/link/63cfcfab4e30670eac4a81c7). We show a concrete
-example which implements our new model [FinalMLP](https://github.com/xue-pai/
-FinalMLP) that has been recently published in AAAI 2023. More examples can be
-found in the [model zoo](./model_zoo/). ## Citation *:bell: If you find our
-code or benchmarks helpful in your research, please kindly cite the following
-papers.* > Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang He. [Open
-Benchmarking for Click-Through Rate Prediction](https://arxiv.org/abs/
-2009.05794). *The 30th ACM International Conference on Information and
+triangular_flag_on_post:**Meituan** | | `torch` | |
+:open_file_folder: **Dynamic Weight Network**
+| | 45 | NeurIPS'22 | [APG](./model_zoo/APG) | [APG: Adaptive Parameter
+Generation Network for Click-Through Rate Prediction](https://arxiv.org/abs/
+2203.16218) :triangular_flag_on_post:**Alibaba** | | `torch` | | 46 | Arxiv'23
+| [PPNet](./model_zoo/PEPNet) | [PEPNet: Parameter and Embedding Personalized
+Network for Infusing with Personalized Prior Information](https://arxiv.org/
+abs/2302.01115) :triangular_flag_on_post:**KuaiShou** | | `torch` | |
+:open_file_folder: **Multi-Task Modeling**
+| | 47 | MachineLearn'97 | [SharedBottom](./model_zoo/multitask/SharedBottom) |
+[Multitask Learning](https://link.springer.com/article/10.1023/A:1007379606734)
+| | `torch` | | 48 | KDD'18 | [MMoE](./model_zoo/multitask/MMOE) | [Modeling
+Task Relationships in Multi-task Learning with Multi-Gate Mixture-of-Experts]
+(https://dl.acm.org/doi/pdf/10.1145/3219819.3220007) :triangular_flag_on_post:
+**Google** | | `torch` | |
+:open_file_folder: **Multi-Domain Modeling**
+| | 49 | Arxiv'23 | PEPNet | [PEPNet: Parameter and Embedding Personalized
+Network for Infusing with Personalized Prior Information](https://arxiv.org/
+abs/2302.01115) :triangular_flag_on_post:**KuaiShou** | | `torch` | + :
+point_right: See [reusable dataset splits for CTR prediction](https://
+openbenchmark.github.io/BARS/datasets/README.html). + :point_right: See
+[benchmarking configurations and steps](https://github.com/openbenchmark/BARS/
+tree/main/ctr_prediction/benchmarks). + :point_right: See [the BARS benchmark
+leaderboard](https://openbenchmark.github.io/BARS/ctr_prediction/leaderboard/
+README.html#). ## Dependencies FuxiCTR has the following dependency
+requirements. + python 3.6+ + pytorch 1.0/1.10+ (required only for torch
+models) + tensorflow 2.1+ (required only for tf models) Other packages can be
+installed via `pip install -r requirements.txt`. ## Quick Start 1. Run the demo
+examples Examples are provided in the demo directory to show some basic usage
+of FuxiCTR. Users can run the examples for quick start and to understand the
+workflow. ``` cd demo python example1_build_dataset_to_h5.py python
+example2_DeepFM_with_h5_input.py ``` 2. Run an existing model Users can easily
+run each model in the model zoo following the commands below, which is a demo
+for running DCN. In addition, users can modify the dataset config and model
+config files to run on their own datasets or with new hyper-parameters. More
+details can be found in the [readme file](./model_zoo/DCN/DCN_torch/README.md).
+``` cd model_zoo/DCN/DCN_torch python run_expid.py --expid DCN_test --gpu 0 #
+Change `MODEL` according to the target model name cd model_zoo/MODEL_PATH
+python run_expid.py --expid MODEL_test --gpu 0 ``` 3. Implement a new model The
+FuxiCTR code structure is modularized, so that every part can be overwritten by
+users according to their needs. In many cases, only the model class needs to be
+implemented for a new customized model. If data preprocessing or data loader is
+not directly applicable, one can also overwrite a new one through the [core
+APIs](https://www.processon.com/view/link/63cfcfab4e30670eac4a81c7). We show a
+concrete example which implements our new model [FinalMLP](https://github.com/
+xue-pai/FinalMLP) that has been recently published in AAAI 2023. More examples
+can be found in the [model zoo](./model_zoo/). ## Citation *:bell: If you find
+our code or benchmarks helpful in your research, please kindly cite the
+following papers.* > Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang
+He. [Open Benchmarking for Click-Through Rate Prediction](https://arxiv.org/
+abs/2009.05794). *The 30th ACM International Conference on Information and
 Knowledge Management (CIKM)*, 2021. [[Bibtex](https://dblp.org/rec/conf/cikm/
 ZhuLYZH21.html?view=bibtex)] > Jieming Zhu, Quanyu Dai, Liangcai Su, Rong Ma,
 Jinyang Liu, Guohao Cai, Xi Xiao, Rui Zhang. [BARS: Towards Open Benchmarking
 for Recommender Systems](https://arxiv.org/abs/2205.09626). *The 45th
 International ACM SIGIR Conference on Research and Development in Information
 Retrieval (SIGIR)*, 2022. [[Bibtex](https://dblp.org/rec/conf/sigir/
 ZhuDSMLCXZ22.html?view=bibtex)] ## Discussion Welcome to join our WeChat group
```

### Comparing `fuxictr-2.0.2/fuxictr/autotuner.py` & `fuxictr-2.0.3/fuxictr/autotuner.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/datasets/avazu.py` & `fuxictr-2.0.3/fuxictr/datasets/avazu.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/datasets/criteo.py` & `fuxictr-2.0.3/fuxictr/datasets/criteo.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/datasets/kkbox.py` & `fuxictr-2.0.3/fuxictr/datasets/kkbox.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/features.py` & `fuxictr-2.0.3/fuxictr/features.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/metrics.py` & `fuxictr-2.0.3/fuxictr/metrics.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/preprocess/build_dataset.py` & `fuxictr-2.0.3/fuxictr/preprocess/build_dataset.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/preprocess/feature_processor.py` & `fuxictr-2.0.3/fuxictr/preprocess/feature_processor.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/preprocess/utils.py` & `fuxictr-2.0.3/fuxictr/preprocess/utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/dataloaders/h5_block_dataloader.py` & `fuxictr-2.0.3/fuxictr/pytorch/dataloaders/h5_block_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/dataloaders/h5_dataloader.py` & `fuxictr-2.0.3/fuxictr/pytorch/dataloaders/h5_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/activations.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/activations.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/dot_product_attention.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/attentions/dot_product_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/squeeze_excitation.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/attentions/squeeze_excitation.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/attentions/target_attention.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/attentions/target_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/factorization_machine.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/logistic_regression.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/blocks/mlp_block.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/blocks/mlp_block.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,34 +25,32 @@
                  input_dim, 
                  hidden_units=[], 
                  hidden_activations="ReLU",
                  output_dim=None,
                  output_activation=None, 
                  dropout_rates=0.0,
                  batch_norm=False, 
-                 norm_before_activation=True,
+                 bn_only_once=False, # Set True for inference speed up
                  use_bias=True):
         super(MLP_Block, self).__init__()
         dense_layers = []
         if not isinstance(dropout_rates, list):
             dropout_rates = [dropout_rates] * len(hidden_units)
         if not isinstance(hidden_activations, list):
             hidden_activations = [hidden_activations] * len(hidden_units)
         hidden_activations = get_activation(hidden_activations, hidden_units)
         hidden_units = [input_dim] + hidden_units
+        if batch_norm and bn_only_once:
+            dense_layers.append(nn.BatchNorm1d(input_dim))
         for idx in range(len(hidden_units) - 1):
             dense_layers.append(nn.Linear(hidden_units[idx], hidden_units[idx + 1], bias=use_bias))
-            if norm_before_activation:
-                if batch_norm:
-                    dense_layers.append(nn.BatchNorm1d(hidden_units[idx + 1]))
+            if batch_norm and not bn_only_once:
+                dense_layers.append(nn.BatchNorm1d(hidden_units[idx + 1]))
             if hidden_activations[idx]:
                 dense_layers.append(hidden_activations[idx])
-            if not norm_before_activation:
-                if batch_norm:
-                    dense_layers.append(nn.BatchNorm1d(hidden_units[idx + 1]))
             if dropout_rates[idx] > 0:
                 dense_layers.append(nn.Dropout(p=dropout_rates[idx]))
         if output_dim is not None:
             dense_layers.append(nn.Linear(hidden_units[-1], output_dim, bias=use_bias))
         if output_activation is not None:
             dense_layers.append(get_activation(output_activation))
         self.mlp = nn.Sequential(*dense_layers) # * used to unpack list
```

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/embeddings/feature_embedding.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/embeddings/feature_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,17 @@
                                                     embedding_dim,
                                                     embedding_initializer=embedding_initializer,
                                                     required_feature_columns=required_feature_columns,
                                                     not_required_feature_columns=not_required_feature_columns,
                                                     use_pretrain=use_pretrain,
                                                     use_sharing=use_sharing)
 
-    def forward(self, X, feature_source=[], feature_type=[], dynamic_emb_dim=False):
+    def forward(self, X, feature_source=[], feature_type=[], flatten_emb=False):
         feature_emb_dict = self.embedding_layer(X, feature_source=feature_source, feature_type=feature_type)
-        feature_emb = self.embedding_layer.dict2tensor(feature_emb_dict, dynamic_emb_dim=dynamic_emb_dim)
+        feature_emb = self.embedding_layer.dict2tensor(feature_emb_dict, flatten_emb=flatten_emb)
         return feature_emb
 
 
 class FeatureEmbeddingDict(nn.Module):
     def __init__(self, 
                  feature_map, 
                  embedding_dim, 
@@ -162,28 +162,30 @@
             "{}\'s embedding_dim is not correctly set to match its pretrained_emb shape".format(feature_name)
         embeddings = torch.from_numpy(embeddings).float()
         embedding_matrix.weight = torch.nn.Parameter(embeddings)
         if freeze:
             embedding_matrix.weight.requires_grad = False
         return embedding_matrix
 
-    def dict2tensor(self, embedding_dict, feature_source=[], feature_type=[], dynamic_emb_dim=False):
+    def dict2tensor(self, embedding_dict, feature_list=[], feature_source=[], feature_type=[], flatten_emb=False):
         if type(feature_source) != list:
             feature_source = [feature_source]
         if type(feature_type) != list:
             feature_type = [feature_type]
         feature_emb_list = []
         for feature, feature_spec in self._feature_map.features.items():
             if feature_source and feature_spec["source"] not in feature_source:
                 continue
             if feature_type and feature_spec["type"] not in feature_type:
                 continue
+            if feature_list and feature not in feature_list:
+                continue
             if feature in embedding_dict:
                 feature_emb_list.append(embedding_dict[feature])
-        if dynamic_emb_dim:
+        if flatten_emb:
             feature_emb = torch.cat(feature_emb_list, dim=-1)
         else:
             feature_emb = torch.stack(feature_emb_list, dim=1)
         return feature_emb
 
     def forward(self, inputs, feature_source=[], feature_type=[]):
         if type(feature_source) != list:
```

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/bilinear_interaction.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/bilinear_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/cross_net.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/holographic_interaction.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/holographic_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/inner_product.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/interactions/interaction_machine.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/interactions/interaction_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/layers/pooling.py` & `fuxictr-2.0.3/fuxictr/pytorch/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/models/ctr_model.py` & `fuxictr-2.0.3/fuxictr/pytorch/models/rank_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,21 +59,15 @@
         self.checkpoint = os.path.abspath(os.path.join(self.model_dir, self.model_id + ".model"))
         self.validation_metrics = kwargs["metrics"]
 
     def compile(self, optimizer, loss, lr):
         self.optimizer = get_optimizer(optimizer, self.parameters(), lr)
         self.loss_fn = get_loss(loss)
 
-    def add_loss(self, inputs):
-        return_dict = self.forward(inputs)
-        y_true = self.get_labels(inputs)
-        loss = self.loss_fn(return_dict["y_pred"], y_true, reduction='mean')
-        return loss
-
-    def add_regularization(self):
+    def regularization_loss(self):
         reg_term = 0
         if self._embedding_regularizer or self._net_regularizer:
             emb_reg = get_regularizer(self._embedding_regularizer)
             net_reg = get_regularizer(self._net_regularizer)
             for name, param in self.named_parameters():
                 if param.requires_grad:
                     if "embedding_layer" in name:
@@ -82,46 +76,49 @@
                                 reg_term += (emb_lambda / emb_p) * torch.norm(param, emb_p) ** emb_p
                     else:
                         if self._net_regularizer:
                             for net_p, net_lambda in net_reg:
                                 reg_term += (net_lambda / net_p) * torch.norm(param, net_p) ** net_p
         return reg_term
 
-    def get_total_loss(self, inputs):
-        total_loss = self.add_loss(inputs) + self.add_regularization()
-        return total_loss
+    def compute_loss(self, return_dict, y_true):
+        loss = self.loss_fn(return_dict["y_pred"], y_true, reduction='mean')
+        loss += self.regularization_loss()
+        return loss
 
     def reset_parameters(self):
         def reset_default_params(m):
             # initialize nn.Linear/nn.Conv1d layers by default
             if type(m) in [nn.Linear, nn.Conv1d]:
                 nn.init.xavier_normal_(m.weight)
                 if m.bias is not None:
                     m.bias.data.fill_(0)
         def reset_custom_params(m):
             # initialize layers with customized reset_parameters
-            pass
+            if hasattr(m, 'reset_custom_params'):
+                m.reset_custom_params()
         self.apply(reset_default_params)
         self.apply(reset_custom_params)
-        
+
     def get_inputs(self, inputs, feature_source=None):
         if feature_source and type(feature_source) == str:
             feature_source = [feature_source]
         X_dict = dict()
         for feature, spec in self.feature_map.features.items():
             if (feature_source is not None) and (spec["source"] not in feature_source):
                 continue
             if spec["type"] == "meta":
                 continue
             X_dict[feature] = inputs[:, self.feature_map.get_column_index(feature)].to(self.device)
         return X_dict
 
     def get_labels(self, inputs):
+        """ Please override get_labels() when using multiple labels!
+        """
         labels = self.feature_map.labels
-        assert len(labels) == 1, "Please override get_labels(), add_loss(), evaluate() when using multiple labels!"
         y = inputs[:, self.feature_map.get_column_index(labels[0])].to(self.device)
         return y.float().view(-1, 1)
                 
     def get_group_id(self, inputs):
         return inputs[:, self.feature_map.get_column_index(self.feature_map.group_id)]
 
     def model_to_device(self):
@@ -186,15 +183,17 @@
         logging.info('Evaluation @epoch {} - batch {}: '.format(self._epoch_index + 1, self._batch_index + 1))
         val_logs = self.evaluate(self.valid_gen, metrics=self._monitor.get_metrics())
         self.checkpoint_and_earlystop(val_logs)
         self.train()
 
     def train_step(self, batch_data):
         self.optimizer.zero_grad()
-        loss = self.get_total_loss(batch_data)
+        return_dict = self.forward(batch_data)
+        y_true = self.get_labels(batch_data)
+        loss = self.compute_loss(return_dict, y_true)
         loss.backward()
         nn.utils.clip_grad_norm_(self.parameters(), self._max_gradient_norm)
         self.optimizer.step()
         return loss
 
     def train_epoch(self, data_generator):
         self._batch_index = 0
```

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/models/multitask_model.py` & `fuxictr-2.0.3/fuxictr/pytorch/models/multitask_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/pytorch/torch_utils.py` & `fuxictr-2.0.3/fuxictr/pytorch/torch_utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/tensorflow/dataloaders/tf_dataloader.py` & `fuxictr-2.0.3/fuxictr/tensorflow/dataloaders/tf_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/factorization_machine.py` & `fuxictr-2.0.3/fuxictr/tensorflow/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/linear.py` & `fuxictr-2.0.3/fuxictr/tensorflow/layers/blocks/linear.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/logistic_regression.py` & `fuxictr-2.0.3/fuxictr/tensorflow/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/tensorflow/layers/blocks/mlp_block.py` & `fuxictr-2.0.3/fuxictr/tensorflow/layers/blocks/mlp_block.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/tensorflow/layers/embeddings/feature_embedding.py` & `fuxictr-2.0.3/fuxictr/tensorflow/layers/embeddings/feature_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,17 @@
                                                     embedding_regularizer=embedding_regularizer,
                                                     required_feature_columns=required_feature_columns,
                                                     not_required_feature_columns=not_required_feature_columns,
                                                     use_pretrain=use_pretrain,
                                                     use_sharing=use_sharing,
                                                     name_prefix=name_prefix)
 
-    def call(self, X, feature_source=[], feature_type=[], dynamic_emb_dim=False):
+    def call(self, X, feature_source=[], feature_type=[], flatten_emb=False):
         feature_emb_dict = self.embedding_layer(X, feature_source=feature_source, feature_type=feature_type)
-        feature_emb = self.embedding_layer.dict2tensor(feature_emb_dict, dynamic_emb_dim=dynamic_emb_dim)
+        feature_emb = self.embedding_layer.dict2tensor(feature_emb_dict, flatten_emb=flatten_emb)
         return feature_emb
 
 
 class FeatureEmbeddingDict(Layer):
     def __init__(self, 
                  feature_map,
                  embedding_dim,
@@ -162,28 +162,30 @@
         assert embeddings.shape[-1] == embedding_matrix.embedding_dim, \
             "{}\'s embedding_dim is not correctly set to match its pretrained_emb shape".format(feature_name)
         embedding_matrix.set_weights([embeddings])
         if freeze:
             embedding_matrix.trainable = False
         return embedding_matrix
 
-    def dict2tensor(self, embedding_dict, feature_source=[], feature_type=[], dynamic_emb_dim=False):
+    def dict2tensor(self, embedding_dict, feature_list=[], feature_source=[], feature_type=[], flatten_emb=False):
         if type(feature_source) != list:
             feature_source = [feature_source]
         if type(feature_type) != list:
             feature_type = [feature_type]
         feature_emb_list = []
         for feature, feature_spec in self._feature_map.features.items():
             if feature_source and feature_spec["source"] not in feature_source:
                 continue
             if feature_type and feature_spec["type"] not in feature_type:
                 continue
+            if feature_list and feature not in feature_list:
+                continue
             if feature in embedding_dict:
                 feature_emb_list.append(embedding_dict[feature])
-        if dynamic_emb_dim:
+        if flatten_emb:
             feature_emb = tf.squeeze(tf.concat(feature_emb_list, axis=-1), axis=1)
         else:
             feature_emb = tf.concat(feature_emb_list, axis=1)
         return feature_emb
 
     def call(self, inputs, feature_source=[], feature_type=[]):
         if type(feature_source) != list:
```

### Comparing `fuxictr-2.0.2/fuxictr/tensorflow/layers/interactions/cross_net.py` & `fuxictr-2.0.3/fuxictr/tensorflow/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/tensorflow/layers/interactions/inner_product.py` & `fuxictr-2.0.3/fuxictr/tensorflow/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/tensorflow/layers/pooling.py` & `fuxictr-2.0.3/fuxictr/tensorflow/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr/tensorflow/models/ctr_model.py` & `fuxictr-2.0.3/fuxictr/tensorflow/models/rank_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,20 +51,21 @@
         self.output_activation = self.get_output_activation(task)
         self.model_id = model_id
         self.model_dir = os.path.join(kwargs["model_root"], feature_map.dataset_id)
         self.checkpoint = os.path.abspath(os.path.join(self.model_dir, self.model_id + ".model"))
         self.validation_metrics = kwargs["metrics"]
 
     def compile(self, optimizer, loss, lr):
-        super().compile(optimizer=get_optimizer(optimizer, lr), loss=get_loss(loss))
+        self.optimizer = get_optimizer(optimizer, lr)
+        self.loss_fn = get_loss(loss)
 
     def add_loss(self, inputs):
-        return_dict = self.call(inputs, training=True)
+        return_dict = self(inputs, training=True)
         y_true = self.get_labels(inputs)
-        loss = self.loss(return_dict["y_pred"], y_true)
+        loss = self.loss_fn(return_dict["y_pred"], y_true)
         return loss
     
     def get_total_loss(self, inputs):
         total_loss = self.add_loss(inputs) + sum(self.losses) # with regularization
         return total_loss
 
     def get_inputs(self, inputs, feature_source=None):
@@ -76,16 +77,17 @@
                 continue
             if spec["type"] == "meta":
                 continue
             X_dict[feature] = inputs[feature]
         return X_dict
 
     def get_labels(self, inputs):
+        """ assert len(labels) == 1, "Please override get_labels() when using multiple labels!"
+        """
         labels = self.feature_map.labels
-        assert len(labels) == 1, "Please override get_labels(), add_loss(), evaluate() when using multiple labels!"
         y = inputs[labels[0]]
         return y
 
     def get_group_id(self, inputs):
         return inputs[self.feature_map.group_id]
 
     def lr_decay(self, factor=0.1, min_lr=1e-6):
@@ -112,14 +114,36 @@
                 break
             else:
                 logging.info("************ Epoch={} end ************".format(self._epoch_index + 1))
         logging.info("Training finished.")
         logging.info("Load best model: {}".format(self.checkpoint))
         self.load_weights(self.checkpoint)
 
+    def train_epoch(self, data_generator):
+        self._batch_index = 0
+        train_loss = 0
+        if self._verbose == 0:
+            batch_iterator = data_generator
+        else:
+            batch_iterator = tqdm(data_generator, disable=False, file=sys.stdout)
+        for batch_index, batch_data in enumerate(batch_iterator):
+            self._batch_index = batch_index
+            self._total_steps += 1
+            loss = self.train_step(batch_data)
+            train_loss += loss.numpy()
+            if (self._eval_steps is not None) and (self._total_steps % self._eval_steps == 0):
+                logging.info("Train loss: {:.6f}".format(train_loss / self._eval_steps))
+                train_loss = 0
+                self.eval_step()
+            if self._stop_training:
+                break
+        if self._eval_steps is None:
+            logging.info("Train loss: {:.6f}".format(train_loss / (self._batch_index + 1)))
+            self.eval_step()
+
     @tf.function
     def train_step(self, batch_data):
         with tf.GradientTape() as tape:
             loss = self.get_total_loss(batch_data)
             grads = tape.gradient(loss, self.trainable_variables)
             grads, _ = tf.clip_by_global_norm(grads, self._max_gradient_norm)
             self.optimizer.apply_gradients(zip(grads, self.trainable_variables))
@@ -148,44 +172,22 @@
                 self.save_weights(self.checkpoint)
         if self._stopping_steps >= self._early_stop_patience:
             self._stop_training = True
             logging.info("********* Epoch=={} early stop *********".format(self._epoch_index + 1))
         if not self._save_best_only:
             self.save_weights(self.checkpoint)
 
-    def train_epoch(self, data_generator):
-        self._batch_index = 0
-        train_loss = 0
-        if self._verbose == 0:
-            batch_iterator = data_generator
-        else:
-            batch_iterator = tqdm(data_generator, disable=False, file=sys.stdout)
-        for batch_index, batch_data in enumerate(batch_iterator):
-            self._batch_index = batch_index
-            self._total_steps += 1
-            loss = self.train_step(batch_data)
-            train_loss += loss.numpy()
-            if (self._eval_steps is not None) and (self._total_steps % self._eval_steps == 0):
-                logging.info("Train loss: {:.6f}".format(train_loss / self._eval_steps))
-                train_loss = 0
-                self.eval_step()
-            if self._stop_training:
-                break
-        if self._eval_steps is None:
-            logging.info("Train loss: {:.6f}".format(train_loss / (self._batch_index + 1)))
-            self.eval_step()
-
     def evaluate(self, data_generator, metrics=None):
         y_pred = []
         y_true = []
         group_id = []
         if self._verbose > 0:
             data_generator = tqdm(data_generator, disable=False, file=sys.stdout)
         for batch_data in data_generator:
-            return_dict = self.call(batch_data)
+            return_dict = self(batch_data, training=True)
             y_pred.extend(return_dict["y_pred"].numpy().reshape(-1))
             y_true.extend(self.get_labels(batch_data).numpy().reshape(-1))
             if self.feature_map.group_id is not None:
                 group_id.extend(self.get_group_id(batch_data).numpy().reshape(-1))
         y_pred = np.array(y_pred, np.float64)
         y_true = np.array(y_true, np.float64)
         group_id = np.array(group_id) if len(group_id) > 0 else None
```

### Comparing `fuxictr-2.0.2/fuxictr/tensorflow/tf_utils.py` & `fuxictr-2.0.3/fuxictr/tensorflow/tf_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             except:
                 raise ValueError('optimizer={} is not supported.'.format(optimizer))
     return optimizer
 
 def get_loss(loss):
     if isinstance(loss, str):
         if loss in ['bce', 'binary_crossentropy', 'binary_cross_entropy']:
-            loss = tf.keras.losses.BinaryCrossentropy()
+            loss = tf.keras.losses.BinaryCrossentropy(from_logits=False)
         else:
             raise ValueError('loss={} is not supported.'.format(loss))
     return loss
 
 def get_regularizer(reg):
     if type(reg) in [int, float]:
         return l2(reg)
```

### Comparing `fuxictr-2.0.2/fuxictr/utils.py` & `fuxictr-2.0.3/fuxictr/utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.0.2/fuxictr.egg-info/PKG-INFO` & `fuxictr-2.0.3/fuxictr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.0.2
+Version: 2.0.3
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/xue-pai/FuxiCTR
 Author: zhujiem
 Author-email: zhujiem@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/xue-pai/FuxiCTR/tags
 Description: <div align="center">
@@ -14,15 +14,14 @@
         <div align="center">
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/python-3.6+-blue" style="max-width: 100%;" alt="Python version"></a>
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/pytorch-1.10+-blue" style="max-width: 100%;" alt="Pytorch version"></a>
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/badge/tensorflow-2.1+-blue" style="max-width: 100%;" alt="Pytorch version"></a>
         <a href="https://pypi.org/project/fuxictr"><img src="https://img.shields.io/pypi/v/fuxictr.svg" style="max-width: 100%;" alt="Pypi version"></a>
         <a href="https://pepy.tech/project/fuxictr"><img src="https://pepy.tech/badge/fuxictr" style="max-width: 100%;" alt="Downloads"></a>
         <a href="https://github.com/xue-pai/FuxiCTR/blob/main/LICENSE"><img src="https://img.shields.io/github/license/xue-pai/fuxictr.svg" style="max-width: 100%;" alt="License"></a>
-        <a href="https://fuxictr.github.io/tutorials"><img src="https://img.shields.io/badge/tutorials-passing-brightgreen?style=flat" style="max-width: 100%;" alt="Wechat QR code"></a>
         </div>
         <hr/>
         
         <div align="center">
         <a href="https://github.com/xue-pai/FuxiCTR/stargazers"><img src="https://reporoster.com/stars/xue-pai/FuxiCTR" /><a/>
         </div>
         
@@ -40,15 +39,15 @@
         + **Extensible**: It supports both pytorch and tensorflow models, and can be easily extended to any new models.
         
         
         ## Model Zoo
         
         | No  | Publication       | Model                                    | Paper                                                                                                                                                                                                           | Benchmark                                                                                                       | Version       |
         |:---:|:-----------------:|:----------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:---------------------------------------------------------------------------------------------------------------:|:-------------:|
-        |     |                   |                                          | :point_down:**Feature Interaction Models**                                                                                                                                                                      |                                                                                                                 |               |
+        |<tr><th colspan=6 align="center">:open_file_folder: **Feature Interaction Models**</th></tr>|
         | 1   | WWW'07            | [LR](./model_zoo/LR)                     | [Predicting Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft**                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LR)           | `torch`       |
         | 2   | ICDM'10           | [FM](./model_zoo/FM)                     | [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf)                                                                                                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FM)           | `torch`       |
         | 3   | CIKM'13           | [DSSM](./model_zoo/DSSM)                 | [Learning Deep Structured Semantic Models  for Web Search using Clickthrough Data ](https://posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DSSM)         | `torch`       |
         | 4   | CIKM'15           | [CCPM](./model_zoo/CCPM)                 | [A Convolutional Click Prediction Model](http://www.escience.cn/system/download/73676)                                                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/CCPM)         | `torch`       |
         | 5   | RecSys'16         | [FFM](./model_zoo/FFM)                   | [Field-aware Factorization Machines for CTR Prediction](https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:**Criteo**                                                                         | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FFM)          | `torch`       |
         | 6   | RecSys'16         | [DNN](./model_zoo/DNN)            | [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:**Google**                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DNN)          | `torch`, `tf` |
         | 7   | DLRS'16           | [Wide&Deep](./model_zoo/WideDeep)        | [Wide & Deep Learning for Recommender Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:**Google**                                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/WideDeep)     | `torch`, `tf` |
@@ -63,42 +62,45 @@
         | 16  | KDD'18            | [xDeepFM](./model_zoo/xDeepFM)           | [xDeepFM: Combining Explicit and Implicit Feature Interactions for Recommender Systems](https://arxiv.org/pdf/1803.05170.pdf) :triangular_flag_on_post:**Microsoft**                                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/xDeepFM)      | `torch`       |
         | 17  | CIKM'19           | [FiGNN](./model_zoo/FiGNN)               | [FiGNN: Modeling Feature Interactions via Graph Neural Networks for CTR Prediction](https://arxiv.org/abs/1910.05552)                                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiGNN)        | `torch`       |
         | 18  | CIKM'19           | [AutoInt/AutoInt+](./model_zoo/AutoInt)  | [AutoInt: Automatic Feature Interaction Learning via Self-Attentive Neural Networks](https://arxiv.org/abs/1810.11921)                                                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AutoInt)      | `torch`       |
         | 19  | RecSys'19         | [FiBiNET](./model_zoo/FiBiNET)           | [FiBiNET: Combining Feature Importance and Bilinear feature Interaction for Click-Through Rate Prediction](https://arxiv.org/abs/1905.09433) :triangular_flag_on_post:**Sina Weibo**                            | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FiBiNET)      | `torch`       |
         | 20  | WWW'19            | [FGCNN](./model_zoo/FGCNN)               | [Feature Generation by Convolutional Neural Network for Click-Through Rate Prediction](https://arxiv.org/abs/1904.04447) :triangular_flag_on_post:**Huawei**                                                    | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FGCNN)        | `torch`       |
         | 21  | AAAI'19           | [HFM/HFM+](./model_zoo/HFM)              | [Holographic Factorization Machines for Recommendation](https://ojs.aaai.org//index.php/AAAI/article/view/4448)                                                                                                 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HFM)          | `torch`       |
         | 22  | Arxiv'19          | [DLRM](./model_zoo/DLRM)                 | [Deep Learning Recommendation Model for Personalization and Recommendation Systems](https://arxiv.org/abs/1906.00091) :triangular_flag_on_post:**Facebook**                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DLRM)         | `torch`       |
-        | 23  | NeuralNetworks'20 | [ONN](./model_zoo/ONN)                   | [Operation-aware Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)                                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/ONN)          | `torch`       |
+        | 23  | NeuralNetworks'20 | [ONN](./model_zoo/ONN)                   | [Operation-aware Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)                                                                                                                | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/ONN)          | `torch`, `tf`      |
         | 24  | AAAI'20           | [AFN/AFN+](./model_zoo/AFN)              | [Adaptive Factorization Network: Learning Adaptive-Order Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768)                                                                           | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AFN)          | `torch`       |
         | 25  | AAAI'20           | [LorentzFM](./model_zoo/LorentzFM)       | [Learning Feature Interactions with Lorentzian Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:**eBay**                                                                               | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LorentzFM)    | `torch`       |
         | 26  | WSDM'20           | [InterHAt](./model_zoo/InterHAt)         | [Interpretable Click-through Rate Prediction through Hierarchical Attention](https://dl.acm.org/doi/10.1145/3336191.3371785) :triangular_flag_on_post:**NEC Labs, Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/InterHAt)     | `torch`       |
         | 27  | DLP-KDD'20        | [FLEN](./model_zoo/FLEN)                 | [FLEN: Leveraging Field for Scalable CTR Prediction](https://arxiv.org/abs/1911.04690) :triangular_flag_on_post:**Tencent**                                                                                     | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FLEN)         | `torch`       |
         | 28  | CIKM'20           | [DeepIM](./model_zoo/DeepIM)             | [Deep Interaction Machine: A Simple but Effective Model for High-order Feature Interactions](https://dl.acm.org/doi/abs/10.1145/3340531.3412077) :triangular_flag_on_post:**Alibaba, RealAI**                   | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepIM)       | `torch`       |
         | 29  | WWW'21            | [FmFM](./model_zoo/FmFM)                 | [FM^2: Field-matrixed Factorization Machines for Recommender Systems](https://arxiv.org/abs/2102.12994) :triangular_flag_on_post:**Yahoo**                                                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FmFM)         | `torch`       |
         | 30  | WWW'21            | [DCN-V2](./model_zoo/DCNv2)              | [DCN V2: Improved Deep & Cross Network and Practical Lessons for Web-scale Learning to Rank Systems](https://arxiv.org/abs/2008.13535) :triangular_flag_on_post:**Google**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DCNv2)        | `torch`       |
         | 31  | CIKM'21           | [DESTINE](./model_zoo/DESTINE)           | [Disentangled Self-Attentive Neural Networks for Click-Through Rate Prediction](https://arxiv.org/abs/2101.03654) :triangular_flag_on_post:**Alibaba**                                                          | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DESTINE)      | `torch`       |
         | 32  | CIKM'21           | [EDCN](./model_zoo/EDCN)                 | [Enhancing Explicit and Implicit Feature Interactions via Information Sharing for Parallel Deep CTR Models](https://dlp-kdd.github.io/assets/pdf/DLP-KDD_2021_paper_12.pdf) :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/EDCN)         | `torch`       |
         | 33  | DLP-KDD'21        | [MaskNet](./model_zoo/MaskNet)           | [MaskNet: Introducing Feature-Wise Multiplication to CTR Ranking Models by Instance-Guided Mask](https://arxiv.org/abs/2102.07619) :triangular_flag_on_post:**Sina Weibo**                                      | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/MaskNet)      | `torch`       |
         | 34  | SIGIR'21          | [SAM](./model_zoo/SAM)                   | [Looking at CTR Prediction Again: Is Attention All You Need?](https://arxiv.org/abs/2105.05563) :triangular_flag_on_post:**BOSS Zhipin**                                                                        | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/SAM)          | `torch`       |
         | 35  | KDD'21            | [AOANet](./model_zoo/AOANet)             | [Architecture and Operation Adaptive Network for Online Recommendations](https://dl.acm.org/doi/10.1145/3447548.3467133) :triangular_flag_on_post:**Didi Chuxing**                                              | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/AOANet)       | `torch`       |
         | 36  | AAAI'23           | [FinalMLP](./model_zoo/FinalMLP)         | [FinalMLP: An Enhanced Two-Stream MLP Model for CTR Prediction](https://arxiv.org/abs/2304.00902) :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FinalMLP)         | `torch`       |
-        | 37  | SIGIR'23           | [FINAL](./model_zoo/FINAL)         | FINAL: Factorized Interaction Layer for CTR Prediction :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FINAL)         | `torch`       |
-        |     |                   |                                          | :point_down:**User Behavior Modeling**                                                                                                                                                                          |                                                                                                                 |               |
+        | 37  | SIGIR'23          | [FINAL](./model_zoo/FINAL)               | FINAL: Factorized Interaction Layer for CTR Prediction :triangular_flag_on_post:**Huawei**                                                                                                               |     [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FINAL)         | `torch`       |
+        |<tr><th colspan=6 align="center">:open_file_folder: **Behavior Sequence Modeling**</th></tr>|
         | 38  | KDD'18            | [DIN](./model_zoo/DIN)                   | [Deep Interest Network for Click-Through Rate Prediction](https://www.kdd.org/kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-prediction) :triangular_flag_on_post:**Alibaba**        |   [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIN)       | `torch`       |
         | 39  | AAAI'19           | [DIEN](./model_zoo/DIEN)                 | [Deep Interest Evolution Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672) :triangular_flag_on_post:**Alibaba**                                                                      |   [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIEN)        | `torch`       |
         | 40  | DLP-KDD'19        | [BST](./model_zoo/BST)                   | [Behavior Sequence Transformer for E-commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874) :triangular_flag_on_post:**Alibaba**                                                                 |  [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/BST)     | `torch`       |
         | 41  | CIKM'20           | [DMIN](./model_zoo/DMIN)                 | [Deep Multi-Interest Network for Click-through Rate Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092) :triangular_flag_on_post:**Alibaba**                                                            |                                                                                                                 | `torch`       |
         | 42  | AAAI'20           | [DMR](./model_zoo/DMR)                   | [Deep Match to Rank Model for Personalized Click-Through Rate Prediction](https://ojs.aaai.org/index.php/AAAI/article/view/5346) :triangular_flag_on_post:**Alibaba**                                           |                                                                                                                 | `torch`       |
         | 43  | Arxiv'21          | [ETA](./model_zoo/ETA)                   | [End-to-End User Behavior Retrieval in Click-Through RatePrediction Model](https://arxiv.org/abs/2108.04468) :triangular_flag_on_post:**Alibaba**                                                               |                                                                                                                 | `torch`       |
         | 44  | CIKM'22           | [SDIM](./model_zoo/SDIM)                 | [Sampling Is All You Need on Modeling Long-Term User Behaviors for CTR Prediction](https://arxiv.org/abs/2205.10249) :triangular_flag_on_post:**Meituan**                                                       |                                                                                                                 | `torch`       |
-        |     |                   |                                          | :point_down:**Multi-Task Models**                                                                                                                                                                          |                                                                                                                 |               |
-        | 45  |     MachineLearn'97      | [SharedBottom](./model_zoo/multitask/SharedBottom)               | [Multitask Learning](https://link.springer.com/article/10.1023/A:1007379606734)                                                                                            |                                                                                                                 | `torch`       |
-        | 46  | KDD'18          | [MMoE](./model_zoo/multitask/MMOE)               | [Modeling Task Relationships in Multi-task Learning with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/3219819.3220007) :triangular_flag_on_post:**Google**                                                                                            |                                                                                                                 | `torch`       |
-        |     |                   |                                          | :point_down:**Multi-Domain Models**                                                                                                                                                                          |                                                                                                                 |               |
-        | 47  | Arxiv'23           | [PPNet](./model_zoo/PPNet)/PEPNet              | [PEPNet: Parameter and Embedding Personalized Network for Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115) :triangular_flag_on_post:**KuaiShou**                                                                                            |                                                                                                                 | `torch`       |
+        |<tr><th colspan=6 align="center">:open_file_folder: **Dynamic Weight Network**</th></tr>|
+        | 45  | NeurIPS'22          | [APG](./model_zoo/APG)               | [APG: Adaptive Parameter Generation Network for Click-Through Rate Prediction](https://arxiv.org/abs/2203.16218) :triangular_flag_on_post:**Alibaba**                                |                                                                                                  | `torch`       |
+        | 46  | Arxiv'23        | [PPNet](./model_zoo/PEPNet)             | [PEPNet: Parameter and Embedding Personalized Network for Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115) :triangular_flag_on_post:**KuaiShou**                          |                                                                                                  | `torch`       |
+        |<tr><th colspan=6 align="center">:open_file_folder: **Multi-Task Modeling**</th></tr>|
+        | 47  |     MachineLearn'97      | [SharedBottom](./model_zoo/multitask/SharedBottom)               | [Multitask Learning](https://link.springer.com/article/10.1023/A:1007379606734)                                                                                            |                                                                                                                 | `torch`       |
+        | 48  | KDD'18          | [MMoE](./model_zoo/multitask/MMOE)               | [Modeling Task Relationships in Multi-task Learning with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/3219819.3220007) :triangular_flag_on_post:**Google**                                                                                            |                                                                                                                 | `torch`       |
+        |<tr><th colspan=6 align="center">:open_file_folder: **Multi-Domain Modeling**</th></tr>|
+        | 49  | Arxiv'23           | PEPNet              | [PEPNet: Parameter and Embedding Personalized Network for Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115) :triangular_flag_on_post:**KuaiShou**                                                                                            |                                                                                                                 | `torch`       |
         
         
         + :point_right: See [reusable dataset splits for CTR prediction](https://openbenchmark.github.io/BARS/datasets/README.html).
         + :point_right: See [benchmarking configurations and steps](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks).
         + :point_right: See [the BARS benchmark leaderboard](https://openbenchmark.github.io/BARS/ctr_prediction/leaderboard/README.html#).
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.0.2 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.0.3 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/xue-pai/FuxiCTR Author: zhujiem Author-email:
 zhujiem@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/xue-pai/FuxiCTR/tags Description:
                                     [Logo]
 [Python_version] [Pytorch_version] [Pytorch_version] [Pypi_version] [Downloads]
-                          [License] [Wechat_QR_code]
+                                   [License]
 ===============================================================================
                 [https://reporoster.com/stars/xue-pai/FuxiCTR]
 Click-through rate (CTR) prediction is a critical task for many industrial
 applications such as online advertising, recommender systems, and sponsored
 search. FuxiCTR provides an open-source library for CTR prediction, with key
 features in configurability, tunability, and reproducibility. We hope this
 project could benefit both researchers and practitioners with the goal of open
@@ -20,49 +20,50 @@
 **Extensible**: It supports both pytorch and tensorflow models, and can be
 easily extended to any new models. ## Model Zoo | No | Publication | Model |
 Paper | Benchmark | Version | |:---:|:-----------------:|:---------------------
 -------------------:|:---------------------------------------------------------
 -------------------------------------------------------------------------------
 ----------------------------------------------------------------------- |:-----
 -------------------------------------------------------------------------------
----------------------------:|:-------------:| | | | | :point_down:**Feature
-Interaction Models** | | | | 1 | WWW'07 | [LR](./model_zoo/LR) | [Predicting
-Clicks: Estimating the Click-Through Rate for New Ads](https://dl.acm.org/
-citation.cfm?id=1242643) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
-ctr_prediction/benchmarks/LR) | `torch` | | 2 | ICDM'10 | [FM](./model_zoo/FM)
-| [Factorization Machines](https://www.csie.ntu.edu.tw/~b97053/paper/
-Rendle2010FM.pdf) | [:arrow_upper_right:](https://github.com/openbenchmark/
-BARS/tree/main/ctr_prediction/benchmarks/FM) | `torch` | | 3 | CIKM'13 | [DSSM]
-(./model_zoo/DSSM) | [Learning Deep Structured Semantic Models for Web Search
-using Clickthrough Data ](https://posenhuang.github.io/papers/
-cikm2013_DSSM_fullversion.pdf) :triangular_flag_on_post:**Microsoft** | [:
-arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
-ctr_prediction/benchmarks/DSSM) | `torch` | | 4 | CIKM'15 | [CCPM](./model_zoo/
-CCPM) | [A Convolutional Click Prediction Model](http://www.escience.cn/system/
-download/73676) | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/
-tree/main/ctr_prediction/benchmarks/CCPM) | `torch` | | 5 | RecSys'16 | [FFM]
-(./model_zoo/FFM) | [Field-aware Factorization Machines for CTR Prediction]
-(https://dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:
-**Criteo** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
-main/ctr_prediction/benchmarks/FFM) | `torch` | | 6 | RecSys'16 | [DNN](./
-model_zoo/DNN) | [Deep Neural Networks for YouTube Recommendations](http://
-art.yale.edu/file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:
-**Google** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
-main/ctr_prediction/benchmarks/DNN) | `torch`, `tf` | | 7 | DLRS'16 |
-[Wide&Deep](./model_zoo/WideDeep) | [Wide & Deep Learning for Recommender
-Systems](https://arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:
-**Google** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
-main/ctr_prediction/benchmarks/WideDeep) | `torch`, `tf` | | 8 | ICDM'16 |
-[IPNN](./model_zoo/PNN) | [Product-based Neural Networks for User Response
-Prediction](https://arxiv.org/pdf/1611.00144.pdf) | [:arrow_upper_right:]
-(https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/
-IPNN) | `torch` | | 9 | KDD'16 | [DeepCrossing](./model_zoo/DeepCrossing) |
-[Deep Crossing: Web-Scale Modeling without Manually Crafted Combinatorial
-Features](https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :
+---------------------------:|:-------------:| |
+:open_file_folder: **Feature Interaction Models**
+| | 1 | WWW'07 | [LR](./model_zoo/LR) | [Predicting Clicks: Estimating the
+Click-Through Rate for New Ads](https://dl.acm.org/citation.cfm?id=1242643) :
+triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/LR) | `torch`
+| | 2 | ICDM'10 | [FM](./model_zoo/FM) | [Factorization Machines](https://
+www.csie.ntu.edu.tw/~b97053/paper/Rendle2010FM.pdf) | [:arrow_upper_right:]
+(https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FM)
+| `torch` | | 3 | CIKM'13 | [DSSM](./model_zoo/DSSM) | [Learning Deep
+Structured Semantic Models for Web Search using Clickthrough Data ](https://
+posenhuang.github.io/papers/cikm2013_DSSM_fullversion.pdf) :
+triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DSSM) |
+`torch` | | 4 | CIKM'15 | [CCPM](./model_zoo/CCPM) | [A Convolutional Click
+Prediction Model](http://www.escience.cn/system/download/73676) | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/CCPM) | `torch` | | 5 | RecSys'16 | [FFM](./
+model_zoo/FFM) | [Field-aware Factorization Machines for CTR Prediction](https:
+//dl.acm.org/citation.cfm?id=2959134) :triangular_flag_on_post:**Criteo** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/FFM) | `torch` | | 6 | RecSys'16 | [DNN](./model_zoo/
+DNN) | [Deep Neural Networks for YouTube Recommendations](http://art.yale.edu/
+file_columns/0001/1132/covington.pdf) :triangular_flag_on_post:**Google** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/DNN) | `torch`, `tf` | | 7 | DLRS'16 | [Wide&Deep](./
+model_zoo/WideDeep) | [Wide & Deep Learning for Recommender Systems](https://
+arxiv.org/pdf/1606.07792.pdf) :triangular_flag_on_post:**Google** | [:
+arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
+ctr_prediction/benchmarks/WideDeep) | `torch`, `tf` | | 8 | ICDM'16 | [IPNN](./
+model_zoo/PNN) | [Product-based Neural Networks for User Response Prediction]
+(https://arxiv.org/pdf/1611.00144.pdf) | [:arrow_upper_right:](https://
+github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/IPNN) |
+`torch` | | 9 | KDD'16 | [DeepCrossing](./model_zoo/DeepCrossing) | [Deep
+Crossing: Web-Scale Modeling without Manually Crafted Combinatorial Features]
+(https://www.kdd.org/kdd2016/papers/files/adf0975-shanA.pdf) :
 triangular_flag_on_post:**Microsoft** | [:arrow_upper_right:](https://
 github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DeepCrossing)
 | `torch` | | 10 | NIPS'16 | [HOFM](./model_zoo/HOFM) | [Higher-Order
 Factorization Machines](https://papers.nips.cc/paper/6144-higher-order-
 factorization-machines.pdf) | [:arrow_upper_right:](https://github.com/
 openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/HOFM) | `torch` | | 11 |
 IJCAI'17 | [DeepFM](./model_zoo/DeepFM) | [DeepFM: A Factorization-Machine
@@ -114,15 +115,15 @@
 model_zoo/DLRM) | [Deep Learning Recommendation Model for Personalization and
 Recommendation Systems](https://arxiv.org/abs/1906.00091) :
 triangular_flag_on_post:**Facebook** | [:arrow_upper_right:](https://
 github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DLRM) |
 `torch` | | 23 | NeuralNetworks'20 | [ONN](./model_zoo/ONN) | [Operation-aware
 Neural Networks for User Response Prediction](https://arxiv.org/pdf/1904.12579)
 | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
-ctr_prediction/benchmarks/ONN) | `torch` | | 24 | AAAI'20 | [AFN/AFN+](./
+ctr_prediction/benchmarks/ONN) | `torch`, `tf` | | 24 | AAAI'20 | [AFN/AFN+](./
 model_zoo/AFN) | [Adaptive Factorization Network: Learning Adaptive-Order
 Feature Interactions](https://ojs.aaai.org/index.php/AAAI/article/view/5768) |
 [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
 ctr_prediction/benchmarks/AFN) | `torch` | | 25 | AAAI'20 | [LorentzFM](./
 model_zoo/LorentzFM) | [Learning Feature Interactions with Lorentzian
 Factorization](https://arxiv.org/abs/1911.09821) :triangular_flag_on_post:
 **eBay** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
@@ -173,82 +174,91 @@
 `torch` | | 36 | AAAI'23 | [FinalMLP](./model_zoo/FinalMLP) | [FinalMLP: An
 Enhanced Two-Stream MLP Model for CTR Prediction](https://arxiv.org/abs/
 2304.00902)Â :triangular_flag_on_post:**Huawei** | [:arrow_upper_right:](https:
 //github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/FinalMLP) |
 `torch` | | 37 | SIGIR'23 | [FINAL](./model_zoo/FINAL) | FINAL: Factorized
 Interaction Layer for CTR PredictionÂ :triangular_flag_on_post:**Huawei** | [:
 arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/main/
-ctr_prediction/benchmarks/FINAL) | `torch` | | | | | :point_down:**User
-Behavior Modeling** | | | | 38 | KDD'18 | [DIN](./model_zoo/DIN) | [Deep
-Interest Network for Click-Through Rate Prediction](https://www.kdd.org/
-kdd2018/accepted-papers/view/deep-interest-network-for-click-through-rate-
-prediction) :triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https:
-//github.com/openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIN) |
-`torch` | | 39 | AAAI'19 | [DIEN](./model_zoo/DIEN) | [Deep Interest Evolution
-Network for Click-Through Rate Prediction](https://arxiv.org/abs/1809.03672)Â :
-triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/DIEN) | `torch` | | 40 |
-DLP-KDD'19 | [BST](./model_zoo/BST) | [Behavior Sequence Transformer for E-
-commerce Recommendation in Alibaba](https://arxiv.org/abs/1905.06874)Â :
-triangular_flag_on_post:**Alibaba** | [:arrow_upper_right:](https://github.com/
-openbenchmark/BARS/tree/main/ctr_prediction/benchmarks/BST) | `torch` | | 41 |
-CIKM'20 | [DMIN](./model_zoo/DMIN) | [Deep Multi-Interest Network for Click-
-through Rate Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092)Â :
+ctr_prediction/benchmarks/FINAL) | `torch` | |
+:open_file_folder: **Behavior Sequence Modeling**
+| | 38 | KDD'18 | [DIN](./model_zoo/DIN) | [Deep Interest Network for Click-
+Through Rate Prediction](https://www.kdd.org/kdd2018/accepted-papers/view/deep-
+interest-network-for-click-through-rate-prediction) :triangular_flag_on_post:
+**Alibaba** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/DIN) | `torch` | | 39 | AAAI'19 | [DIEN](./
+model_zoo/DIEN) | [Deep Interest Evolution Network for Click-Through Rate
+Prediction](https://arxiv.org/abs/1809.03672)Â :triangular_flag_on_post:
+**Alibaba** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/DIEN) | `torch` | | 40 | DLP-KDD'19 | [BST](./
+model_zoo/BST) | [Behavior Sequence Transformer for E-commerce Recommendation
+in Alibaba](https://arxiv.org/abs/1905.06874)Â :triangular_flag_on_post:
+**Alibaba** | [:arrow_upper_right:](https://github.com/openbenchmark/BARS/tree/
+main/ctr_prediction/benchmarks/BST) | `torch` | | 41 | CIKM'20 | [DMIN](./
+model_zoo/DMIN) | [Deep Multi-Interest Network for Click-through Rate
+Prediction](https://dl.acm.org/doi/10.1145/3340531.3412092)Â :
 triangular_flag_on_post:**Alibaba** | | `torch` | | 42 | AAAI'20 | [DMR](./
 model_zoo/DMR) | [Deep Match to Rank Model for Personalized Click-Through Rate
 Prediction](https://ojs.aaai.org/index.php/AAAI/article/view/5346)Â :
 triangular_flag_on_post:**Alibaba** | | `torch` | | 43 | Arxiv'21 | [ETA](./
 model_zoo/ETA) | [End-to-End User Behavior Retrieval in Click-Through
 RatePrediction Model](https://arxiv.org/abs/2108.04468)Â :
 triangular_flag_on_post:**Alibaba** | | `torch` | | 44 | CIKM'22 | [SDIM](./
 model_zoo/SDIM) | [Sampling Is All You Need on Modeling Long-Term User
 Behaviors for CTR Prediction](https://arxiv.org/abs/2205.10249)Â :
-triangular_flag_on_post:**Meituan** | | `torch` | | | | | :point_down:**Multi-
-Task Models** | | | | 45 | MachineLearn'97 | [SharedBottom](./model_zoo/
-multitask/SharedBottom) | [Multitask Learning](https://link.springer.com/
-article/10.1023/A:1007379606734) | | `torch` | | 46 | KDD'18 | [MMoE](./
-model_zoo/multitask/MMOE) | [Modeling Task Relationships in Multi-task Learning
-with Multi-Gate Mixture-of-Experts](https://dl.acm.org/doi/pdf/10.1145/
-3219819.3220007) :triangular_flag_on_post:**Google** | | `torch` | | | | | :
-point_down:**Multi-Domain Models** | | | | 47 | Arxiv'23 | [PPNet](./model_zoo/
-PPNet)/PEPNet | [PEPNet: Parameter and Embedding Personalized Network for
-Infusing with Personalized Prior Information](https://arxiv.org/abs/2302.01115)
-:triangular_flag_on_post:**KuaiShou** | | `torch` | + :point_right: See
-[reusable dataset splits for CTR prediction](https://openbenchmark.github.io/
-BARS/datasets/README.html). + :point_right: See [benchmarking configurations
-and steps](https://github.com/openbenchmark/BARS/tree/main/ctr_prediction/
-benchmarks). + :point_right: See [the BARS benchmark leaderboard](https://
-openbenchmark.github.io/BARS/ctr_prediction/leaderboard/README.html#). ##
-Dependencies FuxiCTR has the following dependency requirements. + python 3.6+ +
-pytorch 1.0/1.10+ (required only for torch models) + tensorflow 2.1+ (required
-only for tf models) Other packages can be installed via `pip install -
-r requirements.txt`. ## Quick Start 1. Run the demo examples Examples are
-provided in the demo directory to show some basic usage of FuxiCTR. Users can
-run the examples for quick start and to understand the workflow. ``` cd demo
-python example1_build_dataset_to_h5.py python example2_DeepFM_with_h5_input.py
-``` 2. Run an existing model Users can easily run each model in the model zoo
-following the commands below, which is a demo for running DCN. In addition,
-users can modify the dataset config and model config files to run on their own
-datasets or with new hyper-parameters. More details can be found in the [readme
-file](./model_zoo/DCN/DCN_torch/README.md). ``` cd model_zoo/DCN/DCN_torch
-python run_expid.py --expid DCN_test --gpu 0 # Change `MODEL` according to the
-target model name cd model_zoo/MODEL_PATH python run_expid.py --expid
-MODEL_test --gpu 0 ``` 3. Implement a new model The FuxiCTR code structure is
-modularized, so that every part can be overwritten by users according to their
-needs. In many cases, only the model class needs to be implemented for a new
-customized model. If data preprocessing or data loader is not directly
-applicable, one can also overwrite a new one through the [core APIs](https://
-www.processon.com/view/link/63cfcfab4e30670eac4a81c7). We show a concrete
-example which implements our new model [FinalMLP](https://github.com/xue-pai/
-FinalMLP) that has been recently published in AAAI 2023. More examples can be
-found in the [model zoo](./model_zoo/). ## Citation *:bell: If you find our
-code or benchmarks helpful in your research, please kindly cite the following
-papers.* > Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang He. [Open
-Benchmarking for Click-Through Rate Prediction](https://arxiv.org/abs/
-2009.05794). *The 30th ACM International Conference on Information and
+triangular_flag_on_post:**Meituan** | | `torch` | |
+:open_file_folder: **Dynamic Weight Network**
+| | 45 | NeurIPS'22 | [APG](./model_zoo/APG) | [APG: Adaptive Parameter
+Generation Network for Click-Through Rate Prediction](https://arxiv.org/abs/
+2203.16218) :triangular_flag_on_post:**Alibaba** | | `torch` | | 46 | Arxiv'23
+| [PPNet](./model_zoo/PEPNet) | [PEPNet: Parameter and Embedding Personalized
+Network for Infusing with Personalized Prior Information](https://arxiv.org/
+abs/2302.01115) :triangular_flag_on_post:**KuaiShou** | | `torch` | |
+:open_file_folder: **Multi-Task Modeling**
+| | 47 | MachineLearn'97 | [SharedBottom](./model_zoo/multitask/SharedBottom) |
+[Multitask Learning](https://link.springer.com/article/10.1023/A:1007379606734)
+| | `torch` | | 48 | KDD'18 | [MMoE](./model_zoo/multitask/MMOE) | [Modeling
+Task Relationships in Multi-task Learning with Multi-Gate Mixture-of-Experts]
+(https://dl.acm.org/doi/pdf/10.1145/3219819.3220007) :triangular_flag_on_post:
+**Google** | | `torch` | |
+:open_file_folder: **Multi-Domain Modeling**
+| | 49 | Arxiv'23 | PEPNet | [PEPNet: Parameter and Embedding Personalized
+Network for Infusing with Personalized Prior Information](https://arxiv.org/
+abs/2302.01115) :triangular_flag_on_post:**KuaiShou** | | `torch` | + :
+point_right: See [reusable dataset splits for CTR prediction](https://
+openbenchmark.github.io/BARS/datasets/README.html). + :point_right: See
+[benchmarking configurations and steps](https://github.com/openbenchmark/BARS/
+tree/main/ctr_prediction/benchmarks). + :point_right: See [the BARS benchmark
+leaderboard](https://openbenchmark.github.io/BARS/ctr_prediction/leaderboard/
+README.html#). ## Dependencies FuxiCTR has the following dependency
+requirements. + python 3.6+ + pytorch 1.0/1.10+ (required only for torch
+models) + tensorflow 2.1+ (required only for tf models) Other packages can be
+installed via `pip install -r requirements.txt`. ## Quick Start 1. Run the demo
+examples Examples are provided in the demo directory to show some basic usage
+of FuxiCTR. Users can run the examples for quick start and to understand the
+workflow. ``` cd demo python example1_build_dataset_to_h5.py python
+example2_DeepFM_with_h5_input.py ``` 2. Run an existing model Users can easily
+run each model in the model zoo following the commands below, which is a demo
+for running DCN. In addition, users can modify the dataset config and model
+config files to run on their own datasets or with new hyper-parameters. More
+details can be found in the [readme file](./model_zoo/DCN/DCN_torch/README.md).
+``` cd model_zoo/DCN/DCN_torch python run_expid.py --expid DCN_test --gpu 0 #
+Change `MODEL` according to the target model name cd model_zoo/MODEL_PATH
+python run_expid.py --expid MODEL_test --gpu 0 ``` 3. Implement a new model The
+FuxiCTR code structure is modularized, so that every part can be overwritten by
+users according to their needs. In many cases, only the model class needs to be
+implemented for a new customized model. If data preprocessing or data loader is
+not directly applicable, one can also overwrite a new one through the [core
+APIs](https://www.processon.com/view/link/63cfcfab4e30670eac4a81c7). We show a
+concrete example which implements our new model [FinalMLP](https://github.com/
+xue-pai/FinalMLP) that has been recently published in AAAI 2023. More examples
+can be found in the [model zoo](./model_zoo/). ## Citation *:bell: If you find
+our code or benchmarks helpful in your research, please kindly cite the
+following papers.* > Jieming Zhu, Jinyang Liu, Shuai Yang, Qi Zhang, Xiuqiang
+He. [Open Benchmarking for Click-Through Rate Prediction](https://arxiv.org/
+abs/2009.05794). *The 30th ACM International Conference on Information and
 Knowledge Management (CIKM)*, 2021. [[Bibtex](https://dblp.org/rec/conf/cikm/
 ZhuLYZH21.html?view=bibtex)] > Jieming Zhu, Quanyu Dai, Liangcai Su, Rong Ma,
 Jinyang Liu, Guohao Cai, Xi Xiao, Rui Zhang. [BARS: Towards Open Benchmarking
 for Recommender Systems](https://arxiv.org/abs/2205.09626). *The 45th
 International ACM SIGIR Conference on Research and Development in Information
 Retrieval (SIGIR)*, 2022. [[Bibtex](https://dblp.org/rec/conf/sigir/
 ZhuDSMLCXZ22.html?view=bibtex)] ## Discussion Welcome to join our WeChat group
```

### Comparing `fuxictr-2.0.2/fuxictr.egg-info/SOURCES.txt` & `fuxictr-2.0.3/fuxictr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 fuxictr/pytorch/layers/interactions/bilinear_interaction.py
 fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
 fuxictr/pytorch/layers/interactions/cross_net.py
 fuxictr/pytorch/layers/interactions/holographic_interaction.py
 fuxictr/pytorch/layers/interactions/inner_product.py
 fuxictr/pytorch/layers/interactions/interaction_machine.py
 fuxictr/pytorch/models/__init__.py
-fuxictr/pytorch/models/ctr_model.py
 fuxictr/pytorch/models/multitask_model.py
+fuxictr/pytorch/models/rank_model.py
 fuxictr/tensorflow/__init__.py
 fuxictr/tensorflow/tf_utils.py
 fuxictr/tensorflow/dataloaders/__init__.py
 fuxictr/tensorflow/dataloaders/tf_dataloader.py
 fuxictr/tensorflow/layers/__init__.py
 fuxictr/tensorflow/layers/pooling.py
 fuxictr/tensorflow/layers/blocks/__init__.py
@@ -60,10 +60,10 @@
 fuxictr/tensorflow/layers/blocks/mlp_block.py
 fuxictr/tensorflow/layers/embeddings/__init__.py
 fuxictr/tensorflow/layers/embeddings/feature_embedding.py
 fuxictr/tensorflow/layers/interactions/__init__.py
 fuxictr/tensorflow/layers/interactions/cross_net.py
 fuxictr/tensorflow/layers/interactions/inner_product.py
 fuxictr/tensorflow/models/__init__.py
-fuxictr/tensorflow/models/ctr_model.py
+fuxictr/tensorflow/models/rank_model.py
 model_zoo/__init__.py
 model_zoo/multitask/__init__.py
```

### Comparing `fuxictr-2.0.2/model_zoo/__init__.py` & `fuxictr-2.0.3/model_zoo/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from .DeepCrossing.src import DeepCrossing
 from .DeepFM.DeepFM_torch.src import DeepFM
 from .DeepIM.src import DeepIM
 from .DESTINE.src import DESTINE
 from .DIEN.src import DIEN
 from .DIN.src import DIN
 from .DLRM.src import DLRM
-from .DMIN.src import DMIN
-from .DMR.src import DMR
+from .DMIN.model import DMIN
+from .DMR.model import DMR
 from .DNN.DNN_torch.src import DNN
 from .DSSM.src import DSSM
 from .EDCN.src import EDCN
 from .ETA.src import ETA
 from .FFM.src import FFM, FFMv2
 from .FGCNN.src import FGCNN
 from .FiBiNET.src import FiBiNET
@@ -31,15 +31,15 @@
 from .HFM.src import HFM
 from .HOFM.src import HOFM
 from .InterHAt.src import InterHAt
 from .LorentzFM.src import LorentzFM
 from .LR.src import LR
 from .MaskNet.src import MaskNet
 from .NFM.src import NFM
-from .ONN.src import ONN, ONNv2
+from .ONN.ONN_torch.model import ONN, ONNv2
 from .PNN.src import PNN
-from .PPNet.src import PPNet
 from .SAM.src import SAM
 from .SDIM.src import SDIM
 from .WideDeep.WideDeep_torch.src import WideDeep
 from .xDeepFM.src import xDeepFM
-from .multitask import SharedBottom, MMoE
+from .PEPNet.model import PPNet
+from .multitask import SharedBottom, MMoE
```

### Comparing `fuxictr-2.0.2/setup.py` & `fuxictr-2.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setuptools.setup(
     name="fuxictr",
-    version="2.0.2",
+    version="2.0.3",
     author="zhujiem",
     author_email="zhujiem@users.noreply.github.com",
     description="A configurable, tunable, and reproducible library for CTR prediction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xue-pai/FuxiCTR",
     download_url='https://github.com/xue-pai/FuxiCTR/tags',
```

